# Comparing `tmp/nxsrecselector-3.28.0.tar.gz` & `tmp/nxsrecselector-3.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxsrecselector-3.28.0.tar", last modified: Fri Jun  2 09:07:25 2023, max compression
+gzip compressed data, was "nxsrecselector-3.29.0.tar", last modified: Wed Jun  7 08:19:18 2023, max compression
```

## Comparing `nxsrecselector-3.28.0.tar` & `nxsrecselector-3.29.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.28.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.28.0/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2017-06-19 15:02:38.000000 nxsrecselector-3.28.0/NXSRecSelector
--rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     4306 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.338510 nxsrecselector-3.28.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.28.0/man/NXSRecSelector.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.28.0/man/nxsrecconfig.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/nxsrecconfig/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/CheckerThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.28.0/nxsrecconfig/Converter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/Describer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/DynamicComponent.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/MacroServerPools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    75512 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/NXSConfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    59225 2023-05-26 09:16:32.000000 nxsrecselector-3.28.0/nxsrecconfig/ProfileManager.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-06-01 15:59:20.000000 nxsrecselector-3.28.0/nxsrecconfig/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.28.0/nxsrecconfig/Selection.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    44983 2023-06-02 09:06:46.000000 nxsrecselector-3.28.0/nxsrecconfig/Settings.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.28.0/nxsrecconfig/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.28.0/nxsrecconfig/Utils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.28.0/nxsrecconfig/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/nxsrecselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-06-02 09:07:25.000000 nxsrecselector-3.28.0/nxsrecselector.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-06-02 09:07:25.342510 nxsrecselector-3.28.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.28.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.465016 nxsrecselector-3.29.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.29.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.29.0/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2017-06-19 15:02:38.000000 nxsrecselector-3.29.0/NXSRecSelector
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7058 2023-06-07 08:19:18.465016 nxsrecselector-3.29.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4303 2023-06-07 07:08:17.000000 nxsrecselector-3.29.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.461016 nxsrecselector-3.29.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.29.0/man/NXSRecSelector.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.29.0/man/nxsrecconfig.1
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.461016 nxsrecselector-3.29.0/nxsrecconfig/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6669 2023-06-07 07:18:20.000000 nxsrecselector-3.29.0/nxsrecconfig/CheckerThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.29.0/nxsrecconfig/Converter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/Describer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/DynamicComponent.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19957 2023-06-07 07:18:50.000000 nxsrecselector-3.29.0/nxsrecconfig/MacroServerPools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    75512 2023-06-07 07:18:35.000000 nxsrecselector-3.29.0/nxsrecconfig/NXSConfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59225 2023-05-26 09:16:32.000000 nxsrecselector-3.29.0/nxsrecconfig/ProfileManager.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-06-07 07:15:39.000000 nxsrecselector-3.29.0/nxsrecconfig/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.29.0/nxsrecconfig/Selection.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    44983 2023-06-02 09:06:46.000000 nxsrecselector-3.29.0/nxsrecconfig/Settings.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.29.0/nxsrecconfig/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.29.0/nxsrecconfig/Utils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.29.0/nxsrecconfig/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-06-07 08:19:18.461016 nxsrecselector-3.29.0/nxsrecselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7058 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-06-07 08:19:18.000000 nxsrecselector-3.29.0/nxsrecselector.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-06-07 08:19:18.465016 nxsrecselector-3.29.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.29.0/setup.py
```

### Comparing `nxsrecselector-3.28.0/COPYRIGHT` & `nxsrecselector-3.29.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/NXSRecSelector` & `nxsrecselector-3.29.0/NXSRecSelector`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/PKG-INFO` & `nxsrecselector-3.29.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.28.0
+Version: 3.29.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
@@ -62,29 +62,29 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian stretch (and jessie, wheezy) or ubuntu bionic nad xenial packages can be found in the HDRI repository.
+        Debian bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/stretch-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
         
         Finally, install module
         
         .. code-block:: console
         
         	  $ apt-get update
         	  $ apt-get install python-nxsrecselector
```

### Comparing `nxsrecselector-3.28.0/README.rst` & `nxsrecselector-3.29.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -54,29 +54,29 @@
 .. code-block:: console
 
 	  $ python setup.py install
 
 Debian packages
 ^^^^^^^^^^^^^^^
 
-Debian stretch (and jessie, wheezy) or ubuntu bionic nad xenial packages can be found in the HDRI repository.
+Debian bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
 
 To install the debian packages, add the PGP repository key
 
 .. code-block:: console
 
 	  $ sudo su
 	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
 
 and then download the corresponding source list
 
 .. code-block:: console
 
 	  $ cd /etc/apt/sources.list.d
-	  $ wget http://repos.pni-hdri.de/stretch-pni-hdri.list
+	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
 
 Finally, install module
 
 .. code-block:: console
 
 	  $ apt-get update
 	  $ apt-get install python-nxsrecselector
```

### Comparing `nxsrecselector-3.28.0/man/NXSRecSelector.1` & `nxsrecselector-3.29.0/man/NXSRecSelector.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/man/nxsrecconfig.1` & `nxsrecselector-3.29.0/man/nxsrecconfig.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/CheckerThread.py` & `nxsrecselector-3.29.0/nxsrecconfig/CheckerThread.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,18 +104,18 @@
         #: (:obj:`int`) thread index
         self.index = index
         #: (:class:`Queue.Queue`) queue with runnable elements
         self.__queue = queue
 
         #: (:obj:`list` <:obj:`str`>) tango datasources error states
         self.tangoSourceErrorStates = [
-            "OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN", "FAULT", "DISABLE"]
+            "OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN", "FAULT"]
 
         #: (:obj:`list` <:obj:`str`>) tango datasources warning states
-        self.tangoSourceWarningStates = ["ALARM"]
+        self.tangoSourceWarningStates = ["ALARM", "DISABLE"]
 
     def run(self):
         """ runner
 
         :brief: It runs the defined thread
         """
         full = True
```

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/Converter.py` & `nxsrecselector-3.29.0/nxsrecconfig/Converter.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/Describer.py` & `nxsrecselector-3.29.0/nxsrecconfig/Describer.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/DynamicComponent.py` & `nxsrecselector-3.29.0/nxsrecconfig/DynamicComponent.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/MacroServerPools.py` & `nxsrecselector-3.29.0/nxsrecconfig/MacroServerPools.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,18 +80,18 @@
             "Door",
             "MntGrp",
             "ScanDir"
         ]
 
         #: (:obj:`list` <:obj:`str`>) tango datasources off states
         self.tangoSourceErrorStates = [
-            "OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN", "FAULT", "DISABLE"]
+            "OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN", "FAULT"]
 
         #: (:obj:`list` <:obj:`str`>) tango datasources warning states
-        self.tangoSourceWarningStates = ["ALARM"]
+        self.tangoSourceWarningStates = ["ALARM", "DISABLE"]
 
     def updateMacroServer(self, door):
         """ updates MacroServer and sardana pools for given door
 
         :param door: door device name
         :type door: :obj:`str`
         """
```

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/NXSConfig.py` & `nxsrecselector-3.29.0/nxsrecconfig/NXSConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1895,19 +1895,19 @@
         [tango.DevVarStringArray,
          "list of default datasources in the CanFail mode",
          []],
         'TangoSourceErrorStates':
         [tango.DevVarStringArray,
          "list of tango error states for tango datasources",
          ["OFF", "INIT", "INSERT", "CLOSE", "UNKNOWN",
-          "FAULT", "DISABLE"]],
+          "FAULT"]],
         'TangoSourceWarningStates':
         [tango.DevVarStringArray,
          "list of tango warning states for tango datasources",
-         ["ALARM"]],
+         ["ALARM", "DISABLE"]],
     }
 
     #: (:obj:`dict` <:obj:`str`, \
     #:       [[ :class:`tango.CmdArgType`, :obj:`str`]] >)
     #:       Command definitions
     cmd_list = {
         'SetScanEnvVariables':
```

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/ProfileManager.py` & `nxsrecselector-3.29.0/nxsrecconfig/ProfileManager.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/Release.py` & `nxsrecselector-3.29.0/nxsrecconfig/Release.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NeXus Sardana Recorder Settings - Release """
 
 #: (:obj:`str`) package version
-__version__ = "3.28.0"
+__version__ = "3.29.0"
```

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/Selection.py` & `nxsrecselector-3.29.0/nxsrecconfig/Selection.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/Selector.py` & `nxsrecselector-3.29.0/nxsrecconfig/Selector.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/Settings.py` & `nxsrecselector-3.29.0/nxsrecconfig/Settings.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/StreamSet.py` & `nxsrecselector-3.29.0/nxsrecconfig/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/Utils.py` & `nxsrecselector-3.29.0/nxsrecconfig/Utils.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecconfig/__init__.py` & `nxsrecselector-3.29.0/nxsrecconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/nxsrecselector.egg-info/PKG-INFO` & `nxsrecselector-3.29.0/nxsrecselector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.28.0
+Version: 3.29.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
@@ -62,29 +62,29 @@
         .. code-block:: console
         
         	  $ python setup.py install
         
         Debian packages
         ^^^^^^^^^^^^^^^
         
-        Debian stretch (and jessie, wheezy) or ubuntu bionic nad xenial packages can be found in the HDRI repository.
+        Debian bullseye and buster or ubuntu lunar, jammy nad focal packages can be found in the HDRI repository.
         
         To install the debian packages, add the PGP repository key
         
         .. code-block:: console
         
         	  $ sudo su
         	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
         
         and then download the corresponding source list
         
         .. code-block:: console
         
         	  $ cd /etc/apt/sources.list.d
-        	  $ wget http://repos.pni-hdri.de/stretch-pni-hdri.list
+        	  $ wget http://repos.pni-hdri.de/bullseye-pni-hdri.list
         
         Finally, install module
         
         .. code-block:: console
         
         	  $ apt-get update
         	  $ apt-get install python-nxsrecselector
```

### Comparing `nxsrecselector-3.28.0/nxsrecselector.egg-info/SOURCES.txt` & `nxsrecselector-3.29.0/nxsrecselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.28.0/setup.py` & `nxsrecselector-3.29.0/setup.py`

 * *Files identical despite different names*

