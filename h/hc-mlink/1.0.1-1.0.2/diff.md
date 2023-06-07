# Comparing `tmp/hc-mlink-1.0.1.tar.gz` & `tmp/hc-mlink-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hc-mlink-1.0.1.tar", last modified: Fri Jun  2 09:13:03 2023, max compression
+gzip compressed data, was "hc-mlink-1.0.2.tar", last modified: Wed Jun  7 15:03:09 2023, max compression
```

## Comparing `hc-mlink-1.0.1.tar` & `hc-mlink-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-02 09:13:03.901094 hc-mlink-1.0.1/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      600 2023-06-02 09:13:03.901094 hc-mlink-1.0.1/PKG-INFO
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-02 09:13:03.891095 hc-mlink-1.0.1/hc_mlink.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      600 2023-06-02 09:13:03.000000 hc-mlink-1.0.1/hc_mlink.egg-info/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      200 2023-06-02 09:13:03.000000 hc-mlink-1.0.1/hc_mlink.egg-info/SOURCES.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-06-02 09:13:03.000000 hc-mlink-1.0.1/hc_mlink.egg-info/dependency_links.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        7 2023-06-02 09:13:03.000000 hc-mlink-1.0.1/hc_mlink.egg-info/requires.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        6 2023-06-02 09:13:03.000000 hc-mlink-1.0.1/hc_mlink.egg-info/top_level.txt
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-02 09:13:03.901094 hc-mlink-1.0.1/mLink/
--rw-r--r--   0 andrew    (1000) andrew    (1000)       49 2023-06-01 16:43:09.000000 hc-mlink-1.0.1/mLink/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    26607 2023-06-02 08:56:01.000000 hc-mlink-1.0.1/mLink/mLink.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)       38 2023-06-02 09:13:03.901094 hc-mlink-1.0.1/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)      858 2023-06-02 09:12:16.000000 hc-mlink-1.0.1/setup.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-07 15:03:09.360670 hc-mlink-1.0.2/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      600 2023-06-07 15:03:09.360670 hc-mlink-1.0.2/PKG-INFO
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-07 15:03:09.350671 hc-mlink-1.0.2/hc_mlink.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      600 2023-06-07 15:03:08.000000 hc-mlink-1.0.2/hc_mlink.egg-info/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      200 2023-06-07 15:03:09.000000 hc-mlink-1.0.2/hc_mlink.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-06-07 15:03:08.000000 hc-mlink-1.0.2/hc_mlink.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        7 2023-06-07 15:03:08.000000 hc-mlink-1.0.2/hc_mlink.egg-info/requires.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        6 2023-06-07 15:03:08.000000 hc-mlink-1.0.2/hc_mlink.egg-info/top_level.txt
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-07 15:03:09.360670 hc-mlink-1.0.2/mLink/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       49 2023-06-01 16:43:09.000000 hc-mlink-1.0.2/mLink/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    27192 2023-06-07 15:00:04.000000 hc-mlink-1.0.2/mLink/mLink.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       38 2023-06-07 15:03:09.360670 hc-mlink-1.0.2/setup.cfg
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      858 2023-06-07 15:01:50.000000 hc-mlink-1.0.2/setup.py
```

### Comparing `hc-mlink-1.0.1/PKG-INFO` & `hc-mlink-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc-mlink
-Version: 1.0.1
+Version: 1.0.2
 Summary: mLink module for Hobby Components range of mLink I2C devices
 Home-page: UNKNOWN
 Author: HobbyComponents (Andrew Davies)
 Author-email: <support@hobbycomponents.com.com>
 License: UNKNOWN
 Description: mLink module for Hobby Components range of mLink I2C devices
 Keywords: mLink,I2C,sensors,relay,interface,serial
```

### Comparing `hc-mlink-1.0.1/hc_mlink.egg-info/PKG-INFO` & `hc-mlink-1.0.2/hc_mlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc-mlink
-Version: 1.0.1
+Version: 1.0.2
 Summary: mLink module for Hobby Components range of mLink I2C devices
 Home-page: UNKNOWN
 Author: HobbyComponents (Andrew Davies)
 Author-email: <support@hobbycomponents.com.com>
 License: UNKNOWN
 Description: mLink module for Hobby Components range of mLink I2C devices
 Keywords: mLink,I2C,sensors,relay,interface,serial
```

### Comparing `hc-mlink-1.0.1/mLink/mLink.py` & `hc-mlink-1.0.2/mLink/mLink.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 ########################################################################
 # FILE:    mLink.py
-# DATE:    01/06/23
-# VERSION: 1.0
+# DATE:    07/06/23
+# VERSION: 1.0.2
 # AUTHOR:  Andrew Davies
    
-# 01/06/23 version 1.0: Original version
+# 01/06/23 version 1.0.1: Original release version
+# 07/06/23 version 1.0.2: Added additional bPad_Read_Key_Index() & 
+#						  bPad_Read_Key() function for keypad module
 
 # This library adds hardware support for the Hobby Components mLink 
 # range of serial I2C modules. Current supported boards:
 
 # mLink 12 Bit port expander (SKU: HCMODU0180)
 # mLink DHT22 temperature and humidity sensor (SKU: HCMODU0181)
 # mLink 1 channel relay module (SKU: HCMODU0182)
@@ -601,27 +603,27 @@
 	CLCD_CURS_LTOR =				0
 	CLCD_CURS_RTOL =				1
 
 	CLCD_TYPE_1602 =				0
 	CLCD_TYPE_2004 =				1
 	
 	# Moves the cursor to the specified col & row
-	def CLCD_Cursor(self, add, col, row):
+	def cLCD_Cursor(self, add, col, row):
 		data = (row << 8) | col
 		self.writeInt(add, self.CLCD_CURS_COL_REG, data)
 	
 	# Prints a string to the display starting at the current cursor
 	# position
-	def CLCD_Print(self, add, text):
+	def cLCD_Print(self, add, text):
 		for c in text:
 			data = ord(c)
 			self.write(add, self.CLCD_PRINT_CHAR_REG, data)
 
 	# Clears the display
-	def CLCD_Clear(self, add):
+	def cLCD_Clear(self, add):
 		self.writeBit(add, self.CLCD_CR1, self.CLCD_CLEAR_BIT, 1)
 		while self.busy(add):
 			pass
 	
 	# Turns the display on or off where state = 0 is off and state = 1
 	# is on
 	def cLCD_on(self, add, state):
@@ -734,14 +736,36 @@
 	# Returns True if there is one or more keys present in the buffer
 	# False if not
 	def bPad_New_Key(self, add):
 		if self.read(add, self.BPAD_BUFF_STATUS_REG) == 0:
 			return True
 		else:
 			return False
+	
+	# Returns the index number of the next key
+	def bPad_Read_Key_Index(self, add):
+		return self.read(add, self.BPAD_BUFFER_REG)
+	
+	# Returns the name of the next key
+	def bPad_Read_Key(self, add):
+		i = self.read(add, self.BPAD_BUFFER_REG)
+		if i == 0:
+			return "UP"
+		elif i == 1:
+			return "LEFT"
+		elif i == 2:
+			return "DOWN"
+		elif i == 3:
+			return "RIGHT"
+		elif i == 4:
+			return "SELECT"
+		elif i == 5:
+			return "BACK"
+		else:
+			return ""
 
 	# Returns True if the UP button is currently pressed, False if not
 	def bPad_Up_State(self, add):
 		if self.read(add, self.BPAD_KEY_STATE_REG) & self.BPAD_UP_BIT:
 			return True
 		else:
 			return False
```

### Comparing `hc-mlink-1.0.1/setup.py` & `hc-mlink-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'mLink module for Hobby Components range of mLink I2C devices'
 LONG_DESCRIPTION = 'mLink module for Hobby Components range of mLink I2C devices'
 
 # Setting up
 setup(
     name="hc-mlink",
     version=VERSION,
```

