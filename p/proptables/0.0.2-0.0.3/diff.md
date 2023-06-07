# Comparing `tmp/proptables-0.0.2.tar.gz` & `tmp/proptables-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proptables-0.0.2.tar", last modified: Mon Jun  5 16:05:49 2023, max compression
+gzip compressed data, was "proptables-0.0.3.tar", last modified: Wed Jun  7 09:31:51 2023, max compression
```

## Comparing `proptables-0.0.2.tar` & `proptables-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:05:49.692846 proptables-0.0.2/
--rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       24 2023-06-05 13:17:38.000000 proptables-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1243 2023-06-05 16:05:49.692846 proptables-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-06-05 13:17:20.000000 proptables-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:05:49.682834 proptables-0.0.2/proptables/
--rw-rw-rw-   0        0        0     2347 2023-06-02 17:01:37.000000 proptables-0.0.2/proptables/R134a_PresSat.csv
--rw-rw-rw-   0        0        0      239 2023-06-03 09:24:40.000000 proptables-0.0.2/proptables/R134a_SupPreSat.csv
--rw-rw-rw-   0        0        0     9777 2023-06-03 09:06:51.000000 proptables-0.0.2/proptables/R134a_Super.csv
--rw-rw-rw-   0        0        0     3736 2023-06-02 17:03:14.000000 proptables-0.0.2/proptables/R134a_TempSat.csv
--rw-rw-rw-   0        0        0       33 2023-06-05 13:16:54.000000 proptables-0.0.2/proptables/__init__.py
--rw-rw-rw-   0        0        0     3340 2023-06-05 15:23:13.000000 proptables-0.0.2/proptables/calSatData.py
--rw-rw-rw-   0        0        0     5031 2023-06-05 15:22:59.000000 proptables-0.0.2/proptables/calSuperHeatData.py
--rw-rw-rw-   0        0        0      621 2023-06-05 16:05:15.000000 proptables-0.0.2/proptables/import_data.py
--rw-rw-rw-   0        0        0      113 2023-06-02 19:28:41.000000 proptables-0.0.2/proptables/interpolate.py
--rw-rw-rw-   0        0        0     1155 2023-06-05 14:57:32.000000 proptables-0.0.2/proptables/main.py
--rw-rw-rw-   0        0        0     5646 2023-06-05 15:23:49.000000 proptables-0.0.2/proptables/superheated.py
--rw-rw-rw-   0        0        0     1704 2023-06-05 15:16:17.000000 proptables-0.0.2/proptables/test.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:05:49.692846 proptables-0.0.2/proptables.egg-info/
--rw-rw-rw-   0        0        0     1243 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 16:05:49.000000 proptables-0.0.2/proptables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-06-05 16:05:49.692846 proptables-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 09:31:51.762473 proptables-0.0.3/
+-rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       24 2023-06-05 13:17:38.000000 proptables-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2452 2023-06-07 09:31:51.762473 proptables-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-06-07 09:25:23.000000 proptables-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 09:31:51.740815 proptables-0.0.3/proptables/
+-rw-rw-rw-   0        0        0     2347 2023-06-02 17:01:37.000000 proptables-0.0.3/proptables/R134a_PresSat.csv
+-rw-rw-rw-   0        0        0      239 2023-06-03 09:24:40.000000 proptables-0.0.3/proptables/R134a_SupPreSat.csv
+-rw-rw-rw-   0        0        0     9777 2023-06-03 09:06:51.000000 proptables-0.0.3/proptables/R134a_Super.csv
+-rw-rw-rw-   0        0        0     3736 2023-06-02 17:03:14.000000 proptables-0.0.3/proptables/R134a_TempSat.csv
+-rw-rw-rw-   0        0        0       33 2023-06-05 13:16:54.000000 proptables-0.0.3/proptables/__init__.py
+-rw-rw-rw-   0        0        0     4497 2023-06-07 09:24:02.000000 proptables-0.0.3/proptables/calSatData.py
+-rw-rw-rw-   0        0        0     5031 2023-06-05 15:22:59.000000 proptables-0.0.3/proptables/calSuperHeatData.py
+-rw-rw-rw-   0        0        0      594 2023-06-06 19:26:47.000000 proptables-0.0.3/proptables/import_data.py
+-rw-rw-rw-   0        0        0      113 2023-06-02 19:28:41.000000 proptables-0.0.3/proptables/interpolate.py
+-rw-rw-rw-   0        0        0     1377 2023-06-06 19:18:38.000000 proptables-0.0.3/proptables/main.py
+-rw-rw-rw-   0        0        0     5646 2023-06-05 15:23:49.000000 proptables-0.0.3/proptables/superheated.py
+-rw-rw-rw-   0        0        0     2070 2023-06-07 09:11:58.000000 proptables-0.0.3/proptables/test.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:31:51.762473 proptables-0.0.3/proptables.egg-info/
+-rw-rw-rw-   0        0        0     2452 2023-06-07 09:31:51.000000 proptables-0.0.3/proptables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-07 09:31:51.000000 proptables-0.0.3/proptables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 09:31:51.000000 proptables-0.0.3/proptables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 09:31:51.000000 proptables-0.0.3/proptables.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-06-07 09:31:51.772529 proptables-0.0.3/setup.cfg
```

### Comparing `proptables-0.0.2/LICENCE.txt` & `proptables-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `proptables-0.0.2/proptables/R134a_PresSat.csv` & `proptables-0.0.3/proptables/R134a_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.2/proptables/R134a_Super.csv` & `proptables-0.0.3/proptables/R134a_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.2/proptables/R134a_TempSat.csv` & `proptables-0.0.3/proptables/R134a_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.2/proptables/calSatData.py` & `proptables-0.0.3/proptables/calSatData.py`

 * *Files 19% similar despite different names*

```diff
@@ -68,20 +68,50 @@
         Hg=result.iat[0,8]
         x=(Enthalpy-Hf)/Hg
         result["x"]=x
         return result
     
     def calculate_x_pressure(self,Pressure,Enthalpy):
         result=self.FindbyPressure(Pressure)
+        result=pd.DataFrame(result)
         if result.shape[0]==3:        
             result.drop([0],inplace=True)
             result=result.reset_index(drop=True)
             result.drop([1],inplace=True)
             result=result.reset_index(drop=True)
         Hf=result.iat[0,6]
         Hg=result.iat[0,8]
         x=(Enthalpy-Hf)/Hg
         result["x"]=x
         return result
+
+    ############################################################# version 0.0.3 ##################################
+
+    def calculate_x_temp_entropy(self,Temperature,Entropy):
+        result=self.FindbyTemp(Temperature)
+        result=pd.DataFrame(result)
+        if result.shape[0]==3:        
+            result.drop([0],inplace=True)
+            result=result.reset_index(drop=True)
+            result.drop([1],inplace=True)
+            result=result.reset_index(drop=True)
+        Sf=result.iat[0,9]
+        Sg=result.iat[0,10]
+        x=(Entropy-Sf)/Sg
+        result["x"]=x
+        return result
     
+    def calculate_x_pressure_entropy(self,Pressure,Entropy):
+        result=self.FindbyPressure(Pressure)
+        result=pd.DataFrame(result)
+        if result.shape[0]==3:        
+            result.drop([0],inplace=True)
+            result=result.reset_index(drop=True)
+            result.drop([1],inplace=True)
+            result=result.reset_index(drop=True)
+        Sf=result.iat[0,9]
+        Sg=result.iat[0,10]
+        x=(Entropy-Sf)/Sg
+        result["x"]=x
+        return result
 
 SatData=SaturatedData()
```

### Comparing `proptables-0.0.2/proptables/calSuperHeatData.py` & `proptables-0.0.3/proptables/calSuperHeatData.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.2/proptables/superheated.py` & `proptables-0.0.3/proptables/superheated.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.2/proptables/test.py` & `proptables-0.0.3/proptables/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,61 +13,75 @@
 check_2=True
 
 if check_2:
     print(R134a(Pressure=230))
 
 #######################3 Check for Saturated liquid Temp ##################
 
-check_3=True
+check_3=False
 if check_3:
     print(R134a(Temperature=98,Enthalpy=300))
 
 ####################### check for Saturated liquid Pressure ##############
 
-check_4=True
+check_4=False
 
 if check_4:
     print(R134a(Pressure=1334,Enthalpy=223))
 
 ##################### check for Superheated Vapour #####################
 
-check_5=True
+check_5=False
 
 pre=[60,100,140,180,200,240,280,320,400,500,600,700,800,900,1000,1200,1400,1600,1800,2000]
 
 if check_5:
     print(R134a(Pressure=60,Superheated=True))
 
-check_5_sub=True
+check_5_sub=False
 
 if check_5_sub:
     for num in pre:
         print(R134a(Pressure=num,Superheated=True))
 
 
 ########################## Check for superheated pressure and Temperature#######
 
-check_6=True
+check_6=False
 
 if check_6:
     print(R134a(Pressure=100,Temperature=95))
 
 ########################### Check for superheated pressure and enthalpy ##########
 
-check_7=True
+check_7=False
 
 if check_7:
     print(R134a(Pressure=240,Enthalpy=331,Superheated=True))
 
 ########################### Check for superheated pressure and entropy ##########
 
-check_8=True
+check_8=False
 
 if check_8:
     print(R134a(Pressure=400,Entropy=1.2,Superheated=True))
 
 ########################### Check for superheated pressure and specificvolume ##########
 
-check_9=True
+check_9=False
 
 if check_9:
-    print(R134a(Superheated=True,Pressure=400,specificvolume=0.06))
+    print(R134a(Superheated=True,Pressure=400,specificvolume=0.06))
+
+################################### check for entropy and temp ##################################
+
+check_10=True
+
+if check_10:
+    print(R134a(Temperature=49,Entropy=0.8))
+
+################################### check for entropy and pres ##################################
+
+check_11=True
+
+if check_11:
+    print(R134a(Pressure=230,Entropy=0.8))
```

### Comparing `proptables-0.0.2/setup.cfg` & `proptables-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7074 6162 6c65 730d 0a76   = proptables..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e33 0d0a  ersion = 0.0.3..
 00000030: 6175 7468 6f72 203d 2042 7564 6468 6920  author = Buddhi 
 00000040: 5769 6a65 6e61 7961 6b65 0d0a 6175 7468  Wijenayake..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696a 656e  or_email = wijen
 00000060: 6179 616b 6562 7564 6468 6933 3438 3032  ayakebuddhi34802
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 466f 7220 6765  ription = For ge
 00000090: 6e65 7261 7469 6e67 2070 726f 7065 7274  nerating propert
```

