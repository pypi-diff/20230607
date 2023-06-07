# Comparing `tmp/TorchSisso-1.0.4.tar.gz` & `tmp/TorchSisso-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.4.tar", last modified: Tue Jun  6 18:28:56 2023, max compression
+gzip compressed data, was "TorchSisso-1.0.5.tar", last modified: Wed Jun  7 16:24:42 2023, max compression
```

## Comparing `TorchSisso-1.0.4.tar` & `TorchSisso-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:28:56.247574 TorchSisso-1.0.4/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:28:56.246578 TorchSisso-1.0.4/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:28:56.226563 TorchSisso-1.0.4/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    22981 2023-06-04 21:51:26.000000 TorchSisso-1.0.4/TorchSisso/FC_copy.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23771 2023-06-03 02:04:32.000000 TorchSisso-1.0.4/TorchSisso/FC_copy_working.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23659 2023-06-06 18:18:09.000000 TorchSisso-1.0.4/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20266 2023-06-03 02:11:41.000000 TorchSisso-1.0.4/TorchSisso/Feature_space_construction_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10954 2023-06-05 21:48:28.000000 TorchSisso-1.0.4/TorchSisso/SISSORegressor.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10758 2023-06-04 15:54:54.000000 TorchSisso-1.0.4/TorchSisso/SISSORegressor_L1L0.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7986 2023-06-06 18:28:21.000000 TorchSisso-1.0.4/TorchSisso/SISSO_REGRESSOR_TORCH.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7620 2023-06-06 17:19:57.000000 TorchSisso-1.0.4/TorchSisso/SISSO_Torch.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7986 2023-06-06 18:27:13.000000 TorchSisso-1.0.4/TorchSisso/SISSO_Torch_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      272 2023-06-06 18:05:22.000000 TorchSisso-1.0.4/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6639 2023-06-04 19:54:48.000000 TorchSisso-1.0.4/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-06 18:28:56.243578 TorchSisso-1.0.4/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      515 2023-06-06 18:28:56.000000 TorchSisso-1.0.4/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-06 18:28:55.000000 TorchSisso-1.0.4/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-06 18:28:56.248565 TorchSisso-1.0.4/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-06 18:18:23.000000 TorchSisso-1.0.4/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 16:24:42.657213 TorchSisso-1.0.5/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-07 16:24:42.656221 TorchSisso-1.0.5/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 16:24:42.639213 TorchSisso-1.0.5/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    22981 2023-06-04 21:51:26.000000 TorchSisso-1.0.5/TorchSisso/FC_copy.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23771 2023-06-03 02:04:32.000000 TorchSisso-1.0.5/TorchSisso/FC_copy_working.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23773 2023-06-07 15:20:59.000000 TorchSisso-1.0.5/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20266 2023-06-03 02:11:41.000000 TorchSisso-1.0.5/TorchSisso/Feature_space_construction_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10954 2023-06-05 21:48:28.000000 TorchSisso-1.0.5/TorchSisso/SISSORegressor.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10758 2023-06-04 15:54:54.000000 TorchSisso-1.0.5/TorchSisso/SISSORegressor_L1L0.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7986 2023-06-06 18:28:21.000000 TorchSisso-1.0.5/TorchSisso/SISSO_REGRESSOR_TORCH.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7620 2023-06-06 17:19:57.000000 TorchSisso-1.0.5/TorchSisso/SISSO_Torch.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     7976 2023-06-07 00:20:00.000000 TorchSisso-1.0.5/TorchSisso/SISSO_Torch_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      273 2023-06-07 16:24:26.000000 TorchSisso-1.0.5/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6163 2023-06-07 00:30:46.000000 TorchSisso-1.0.5/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 16:24:42.653213 TorchSisso-1.0.5/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-07 16:24:42.000000 TorchSisso-1.0.5/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      515 2023-06-07 16:24:42.000000 TorchSisso-1.0.5/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-07 16:24:42.000000 TorchSisso-1.0.5/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-07 16:24:42.000000 TorchSisso-1.0.5/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-07 16:24:42.000000 TorchSisso-1.0.5/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-07 16:24:42.658213 TorchSisso-1.0.5/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-07 16:24:06.000000 TorchSisso-1.0.5/setup.py
```

### Comparing `TorchSisso-1.0.4/TorchSisso/FC_copy.py` & `TorchSisso-1.0.5/TorchSisso/FC_copy.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/TorchSisso/FC_copy_working.py` & `TorchSisso-1.0.5/TorchSisso/FC_copy_working.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.0.5/TorchSisso/FeatureSpaceConstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,14 +428,15 @@
     self.df_feature_values = torch.tensor(space.values).to(self.device)
     print('Second Feature Space building is completed with features count: ',int(space.shape[1]))
     print('Time taken to create and remove redundant features in phi2 is ', round(time.time() - start_time,3), ' seconds')
 
     if self.no_of_operators >3: 
       for i in range(4,self.no_of_operators+1):
         if i == 4:
+          start = time.time()
           values, names = self.combinations(basic_operators)
           values1,names1 = self.single_variable(other_operators)
           space_created_3 = torch.cat((self.df_feature_values,values,values1),dim=1).to(self.device)
           #space_created_3 = torch.cat((values,self.df_feature_values),dim=1).to(self.device)
           del space_created_2
           self.columns = self.columns + names + names1
           #self.columns = names + self.columns
@@ -444,15 +445,16 @@
           space = space.dropna(axis=1, how='any')
           space = space.round(7)
           # Transpose the dataframe
           space = space.T.drop_duplicates().T
           del values, names,
           self.columns = space.columns.tolist()
           self.df_feature_values = torch.tensor(space.values).to(self.device)
-          print('Third Feature Space building is completed',space.shape)
+          print('Third Feature Space building is completed',space.shape[1])
+          print(f'Time taken to build the phi3 is  {time.time()-start} seconds')
           if self.no_of_operators+1 == 5:
             space.insert(0,'Target',self.Target_column)
             space = space.dropna(axis=1, how='any')
             #returniung the dataframe
             return space
           else:
             continue
```

### Comparing `TorchSisso-1.0.4/TorchSisso/Feature_space_construction_1.py` & `TorchSisso-1.0.5/TorchSisso/Feature_space_construction_1.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/TorchSisso/SISSORegressor.py` & `TorchSisso-1.0.5/TorchSisso/SISSORegressor.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/TorchSisso/SISSORegressor_L1L0.py` & `TorchSisso-1.0.5/TorchSisso/SISSORegressor_L1L0.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/TorchSisso/SISSO_REGRESSOR_TORCH.py` & `TorchSisso-1.0.5/TorchSisso/SISSO_REGRESSOR_TORCH.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/TorchSisso/SISSO_Torch.py` & `TorchSisso-1.0.5/TorchSisso/SISSO_Torch.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/TorchSisso/SISSO_Torch_1.py` & `TorchSisso-1.0.5/TorchSisso/SISSO_Torch_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,19 +83,18 @@
         terms = []
         for i in range(len(non_std_coeff.squeeze())):
             term = str(round(float(non_std_coeff.squeeze()[i]),3)) + "*" + str(self.names[int(indices_min[i])])
             terms.append(term)
         return float(rmse),terms,non_std_intercept,non_std_coeff
     
     def SISSO(self):
-        
         if self.x.shape[1] > self.sis_features*self.dimension :
             print(f"Starting SISSO in {self.device}")
         else:
-            return RuntimeError(f'Number of features in SIS screening are greater than total number of features, SISSO cannot be performed. Please input the valid number when product of {self.dimension}*{self.sis_features} that is less than  {self.x.shape[1]}')
+            raise RuntimeError(f'Number of features in SIS screening are greater than total number of features, SISSO cannot be performed. Please input the valid number when product of {self.dimension}*{self.sis_features} that is less than  {self.x.shape[1]}')
         
         #Looping over the dimensions 
         for i in range(1,self.dimension+1):
             
             if i ==1:
                 
                 start_1D = time.time()
```

### Comparing `TorchSisso-1.0.4/TorchSisso/testRegressor.py` & `TorchSisso-1.0.5/TorchSisso/testRegressor.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @author: muthyala.7
 """
 
 import FeatureSpaceConstruction
 import Feature_space_construction_1
 import SISSORegressor
 import SISSORegressor_L1L0
+import SISSO_Torch_1
 import FC_copy
 import torch
 import numpy as np 
 import pandas as pd 
 import time
 import os 
 from sklearn.linear_model import LassoCV
@@ -31,43 +32,28 @@
 for i in range(len(x)):
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 operators = ['+','/']
 y = 10*((df.iloc[:,0])/(df.iloc[:,1]*(df.iloc[:,2]+df.iloc[:,3]))) + 3 + 0.01*np.random.normal(0,1,10)
 df.insert(0,'Target',y)
 start = time.time()
-fc = FeatureSpaceConstruction.feature_space_construction(operators,df,3,'cuda')
+fc = FeatureSpaceConstruction.feature_space_construction(operators,df,3,'cpu')
 df_created = fc.feature_space()
 
 #Create Instace for class 
 x = torch.tensor(df_created.iloc[:,1:].values)
 y = torch.tensor(df_created.iloc[:,0])
 names = df_created.iloc[:,1:].columns
-sr = SISSORegressor.SISSO_Regressor(x,y,names,1,20,'cuda','L0')
-rmse, equation = sr.SISSO()
+sr = SISSO_Torch_1.SISSORegressor(x, y, names,1,20,'L0','cpu')
+sr.SISSO()
+#sr = SISSORegressor.SISSO_Regressor(x,y,names,1,20,'cpu','L0')
+#rmse, equation = sr.SISSO()
 print('SISSO Completed',time.time()-start,'\n')
 print('\n')
 
-#Implementing LASSO on the initial dataset
-x = df.iloc[:,1:]
-y = df.iloc[:,0]
-lasso = LassoCV(cv=10)
-lasso.fit(x,y)
-y_pred = lasso.predict(x)
-rmse1 = np.sqrt(mean_squared_error(y,y_pred))
-print('RMSE of the LASSO implementation on initial dataset: ',rmse1)
-'''
-x = df_created.iloc[:,1:]
-y = df_created.iloc[:,0]
-lasso = LassoCV(cv=10)
-lasso.fit(x,y)
-y_pred = lasso.predict(x)
-rmse1 = np.sqrt(mean_squared_error(y,y_pred))
-print('RMSE of the LASSO implementation on expanded dataset: ',rmse1)
-'''
 os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/1/')
 df.to_csv('train.csv')
 df.insert(0,'Index',df.index)
 df.to_csv('train.dat',sep='\t',index=False)
 
 '''
 ###############################################################################################
@@ -80,45 +66,41 @@
 for i in range(len(x)):
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 y1 = 3*np.sqrt(df.iloc[:,1]) + 2.10*np.sin(df.iloc[:,2]) + 2.10 + 0.010*np.random.normal(0,1,10)
 df.insert(0,'Target',y1)
 operators = ['sqrt','sin']
 start_c = time.time()
-FC = FC_copy.feature_space_construction(operators, df,3,'cpu')
+FC = FeatureSpaceConstruction.feature_space_construction(operators, df,3,'cpu')
 df_created = FC.feature_space()
 #Create Instace for class 
 x = torch.tensor(df_created.iloc[:,1:].values)
 y = torch.tensor(df_created.iloc[:,0])
 names = df_created.iloc[:,1:].columns
 start = time.time()
-sr = SISSORegressor.SISSO_Regressor(x,y,names,2,10,'cpu')
-rmse, equation = sr.SISSO()
+sr = SISSO_Torch_1.SISSORegressor(x,y,names,2,10,'L0','cpu')
+sr.SISSO()
 print(time.time()-start)
 #sr = SISSORegressor_L1L0.SISSO_Regressor(x,y,names,2,10,'cuda','L1L0')
 #rmse, equation = sr.SISSO()
-start = time.time()
-sr = SISSORegressor.SISSO_Regressor(x,y,names,2,10,'cuda')
-rmse, equation = sr.SISSO()
-print(time.time()-start)
 print("SISSO Completed: ",time.time()-start_c,'\n')
 import os 
 os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/2/')
 df.to_csv('train.csv')
 df.insert(0,'Index',df.index)
 df.to_csv('train.dat',sep='\t',index=False)
-
+'''
 '''
 ##########################################################################################################
 
 #CaseStudy-3
 
 #########################################################################################################
 '''
-x = [np.random.uniform(0,2,size=10) for i in range(3)]
+x = [np.random.uniform(0,2,size=10) for i in range(4)]
 df = pd.DataFrame()
 for i in range(len(x)):
   variable = 'x'+str(i+1)
   df[variable] = x[i]
 y2 = 3*(np.exp(df.iloc[:,3])/(df.iloc[:,2]+np.exp(df.iloc[:,1]))) + 0.01*np.random.normal(0,1,10)
 df.insert(0,'Target',y2)
 operators = ['/','+','exp']
@@ -142,34 +124,35 @@
 print("SISSO Completed: ",time.time()-start_c,'\n')
 os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/3/')
 df.to_csv('train.csv')
 df.insert(0,'Index',df.index)
 df.to_csv('train.dat',sep='\t',index=False)
 
 '''
+'''
 ##############################################################################################################
 
 #CaseStudy 4
 
 ##############################################################################################################
 
 '''
 df = pd.read_csv('/home/muthyala.7/Downloads/NOMAD_TEST_FILE.csv')
 
 operators = ['+','-','*','/']
 start_time = time.time()
-FC = FC_copy.feature_space_construction(operators, df,3,'cpu')
+FC = FeatureSpaceConstruction.feature_space_construction(operators, df,3,'cpu')
 df_created = FC.feature_space()
 x = torch.tensor(df_created.iloc[:,1:].values)
 y = torch.tensor(df_created.iloc[:,0])
 names = df_created.iloc[:,1:].columns
 
-sr = SISSORegressor.SISSO_Regressor(x,y,names,3,20,'cpu')
-rmse, equation = sr.SISSO()
-print(rmse,'\n',equation,'\n')
+sr = SISSO_Torch_1.SISSORegressor(x,y,names,3,20,'L0','cpu')
+sr.SISSO()
+
 print("SISSO Completed: ",time.time()-start_time,'\n')
 
 '''
 ##########################################################################################################
 
 #CaseStudy-5
 
@@ -186,20 +169,23 @@
 start_c = time.time()
 start_f = time.time()
 FC = FeatureSpaceConstruction.feature_space_construction(operators, df,3,'cpu')
 df_created= FC.feature_space()
 x = torch.tensor(df_created.iloc[:,1:].values)
 y = torch.tensor(df_created.iloc[:,0])
 names = df_created.iloc[:,1:].columns
-sr = SISSORegressor.SISSO_Regressor(x,y,names,3,5,'cpu')
-rmse, equation = sr.SISSO()
+sr = SISSO_Torch_1.SISSORegressor(x,y,names,3,5,'L0','cpu')
+sr.SISSO()
+#sr = SISSORegressor.SISSO_Regressor(x,y,names,3,5,'cpu')
+#rmse, equation = sr.SISSO()
 print("SISSO Completed: ",time.time()-start_c,'\n')
 #os.mkdir('/home/muthyala.7/TorchSisso/Case_Studies/4')
 os.chdir('/home/muthyala.7/TorchSisso/Case_Studies/4/')
 df.to_csv('train.csv')
 df.insert(0,'Index',df.index)
 df.to_csv('train.dat',sep='\t',index=False)
 
 
 
 
 
+
```

### Comparing `TorchSisso-1.0.4/TorchSisso.egg-info/SOURCES.txt` & `TorchSisso-1.0.5/TorchSisso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.4/setup.py` & `TorchSisso-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.4",
+    version="1.0.5",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

