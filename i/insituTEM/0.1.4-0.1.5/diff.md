# Comparing `tmp/insituTEM-0.1.4.tar.gz` & `tmp/insituTEM-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insituTEM-0.1.4.tar", last modified: Wed Jun  7 01:58:24 2023, max compression
+gzip compressed data, was "insituTEM-0.1.5.tar", last modified: Wed Jun  7 02:38:37 2023, max compression
```

## Comparing `insituTEM-0.1.4.tar` & `insituTEM-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:58:24.543040 insituTEM-0.1.4/
--rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:58:24.542874 insituTEM-0.1.4/PKG-INFO
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:58:24.541849 insituTEM-0.1.4/insituTEM/
--rw-r--r--   0 monali     (501) staff       (20)        0 2023-06-07 00:56:09.000000 insituTEM-0.1.4/insituTEM/__ init __.py
--rw-r--r--   0 monali     (501) staff       (20)     4228 2021-08-11 23:48:44.000000 insituTEM-0.1.4/insituTEM/insitu_DP.py
--rw-r--r--   0 monali     (501) staff       (20)    12479 2023-02-20 17:08:48.000000 insituTEM-0.1.4/insituTEM/insitu_IO.py
--rw-r--r--   0 monali     (501) staff       (20)     6070 2023-02-07 23:34:02.000000 insituTEM-0.1.4/insituTEM/insitu_Preprocess.py
--rw-r--r--   0 monali     (501) staff       (20)     8779 2023-02-20 21:40:28.000000 insituTEM-0.1.4/insituTEM/insitu_alignment.py
-drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 01:58:24.542622 insituTEM-0.1.4/insituTEM.egg-info/
--rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/PKG-INFO
--rw-r--r--   0 monali     (501) staff       (20)      303 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/SOURCES.txt
--rw-r--r--   0 monali     (501) staff       (20)        1 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/dependency_links.txt
--rw-r--r--   0 monali     (501) staff       (20)       59 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/requires.txt
--rw-r--r--   0 monali     (501) staff       (20)       10 2023-06-07 01:58:24.000000 insituTEM-0.1.4/insituTEM.egg-info/top_level.txt
--rw-r--r--   0 monali     (501) staff       (20)       38 2023-06-07 01:58:24.543095 insituTEM-0.1.4/setup.cfg
--rw-r--r--   0 monali     (501) staff       (20)      366 2023-06-07 01:58:11.000000 insituTEM-0.1.4/setup.py
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 02:38:37.524142 insituTEM-0.1.5/
+-rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 02:38:37.523973 insituTEM-0.1.5/PKG-INFO
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 02:38:37.522764 insituTEM-0.1.5/insituTEM/
+-rw-r--r--   0 monali     (501) staff       (20)        0 2023-06-07 00:56:09.000000 insituTEM-0.1.5/insituTEM/__ init __.py
+-rw-r--r--   0 monali     (501) staff       (20)     4494 2023-06-07 02:34:33.000000 insituTEM-0.1.5/insituTEM/insitu_DP.py
+-rw-r--r--   0 monali     (501) staff       (20)    12479 2023-02-20 17:08:48.000000 insituTEM-0.1.5/insituTEM/insitu_IO.py
+-rw-r--r--   0 monali     (501) staff       (20)     6070 2023-02-07 23:34:02.000000 insituTEM-0.1.5/insituTEM/insitu_Preprocess.py
+-rw-r--r--   0 monali     (501) staff       (20)     8779 2023-02-20 21:40:28.000000 insituTEM-0.1.5/insituTEM/insitu_alignment.py
+drwxr-xr-x   0 monali     (501) staff       (20)        0 2023-06-07 02:38:37.523716 insituTEM-0.1.5/insituTEM.egg-info/
+-rw-r--r--   0 monali     (501) staff       (20)      129 2023-06-07 02:38:37.000000 insituTEM-0.1.5/insituTEM.egg-info/PKG-INFO
+-rw-r--r--   0 monali     (501) staff       (20)      303 2023-06-07 02:38:37.000000 insituTEM-0.1.5/insituTEM.egg-info/SOURCES.txt
+-rw-r--r--   0 monali     (501) staff       (20)        1 2023-06-07 02:38:37.000000 insituTEM-0.1.5/insituTEM.egg-info/dependency_links.txt
+-rw-r--r--   0 monali     (501) staff       (20)       59 2023-06-07 02:38:37.000000 insituTEM-0.1.5/insituTEM.egg-info/requires.txt
+-rw-r--r--   0 monali     (501) staff       (20)       10 2023-06-07 02:38:37.000000 insituTEM-0.1.5/insituTEM.egg-info/top_level.txt
+-rw-r--r--   0 monali     (501) staff       (20)       38 2023-06-07 02:38:37.524195 insituTEM-0.1.5/setup.cfg
+-rw-r--r--   0 monali     (501) staff       (20)      366 2023-06-07 02:38:13.000000 insituTEM-0.1.5/setup.py
```

### Comparing `insituTEM-0.1.4/insituTEM/insitu_DP.py` & `insituTEM-0.1.5/insituTEM/insitu_DP.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,161 @@
-# -*- coding: utf-8 -*-
-"""
-in-situ TEM Toolbox - Data process 
-
-Assembles of functions related to movie input output
-
-Example:
-    
-    import insitu_DP as DP
-    IO.f2tif(path,1)
-
-Created on Tue Jun 11 10:25:25 2019
-@author: Mona
-"""
-import numpy as np
-
-def readcsvCol(path,col):
-    """
-    Function to read csv rol into array 
-    Inputs: file path; col number
-    Output: 1D np array
-        
-    Example: 
-        x = readcsvCol(path,1)
-    """
-    import csv
-    x=[]
-    with open(path,'r') as csvfile:
-        plots = csv.reader(csvfile, delimiter=',')
-        for row in plots:
-            if row[col]=='':
-                x.append(np.nan)
-            else:
-                x.append(float(row[col]))
-#        plt.plot(x,y) #to check if  the read  result is correct
-    return x
-def readcsv(path,col_list):
-    """
-    Function to read csv rol into array 
-    Inputs: file path; col number list
-    Output: 1D np array
-        
-    Example: 
-        x = readcsv(path,[0:3])
-    """
-#    w= len(col_list)
-    x=readcsvCol(path,col_list[0])
-#    l = len(x)
-    D=np.zeros((len(x),len(col_list)))
-    i=0
-    for col in col_list:
-        
-        x=readcsvCol(path,col)
-        D[:,i]=x
-        i=i+1
-#        D = [D, x]
-    return D
-
-    
-def writeCSV(pathout,data):
-#    import csv
-    import numpy as np
-#    (length,width)=np.shape(data)
-#    np.savetxt(pathout, data, fmt='%1.4d', delimiter=",") 
-    np.savetxt(pathout, data, fmt='%.4f', delimiter=",")   
-    
-def plot2ani(x,y,outpath,label,w=800,h=600,fps=10,dpi=72,tl_size=20,c='r'):
-    """
-    Function to make plot into animation 
-    Inputs: 
-        data: x y; 
-        Movie setting: size: w,h ;
-                       fps; savepath
-                       label: ['xlabel','ylabel'] str array
-                       tl_size: title font size
-                       c: color of the plot line
-                       dpi: dpi for screen : 72 for 4k screen, 96 for 1080p screen
-    Output: mp4 movie
-        
-    Example: 
-        plot2ani(x,y,w,h,fps,outpath,dpi,tl_size,'r')
-
-    """
-    
-    import matplotlib.pyplot as plt
-    import matplotlib.animation as animation
-    interV=1000/fps #time interval for each frame: ms
-#    w_in=w/dpi
-#    h_in=h/dpi
-    fig, ax = plt.subplots(figsize=(w/dpi, h/dpi))#figsize unit: inch
-    plt.rcParams.update({'font.size': tl_size})
-    plt.xlabel(label[0])#Change xy label if needed
-    plt.ylabel(label[1])
-    l=plt.plot(x,y,'grey') #For inital plot
-    redLine, = plt.plot(x[:0],y[:0],color=c, lw=3)
-    time_text = ax.text(5,7,str(y[0])+'°',fontsize=20)
-#    plt.text(5, 7, str(y[0],fontsize=20))
-    def animate(i):
-        redLine.set_data(x[:i], y[:i])
-#        plt.text(5, 7, str(y[i])+'°',fontsize=20) # Text is overlapping with previous frames
-        time_text.set_text(str(round(y[i],1))+'°') 
-#        print(str(i)/len(x))
-        return tuple([redLine,]) + tuple([time_text])
-    
-    plt.tight_layout() #To avoid boarder
-    # create animation using the animate() function
-    ani = animation.FuncAnimation(fig, animate, frames=len(x), \
-                                      interval=interV, blit=True, repeat=True)
-    ani.save(outpath)
-    plt.show()
-    
- 
-def findconnectingpoints(points,startpoint,r,level):
-    """
-    FUnction for find all surrounding points within distance r betwwen each other from startpoint
-    return: index of all connected points
-    """
-    from scipy import spatial
-    tree = spatial.cKDTree(points, leafsize=30)
-    idx =tree.query_ball_point(startpoint,r)
-    i=0
-    while i<level:
-        for results in idx:
-            nearby_point = points[results]
-            idx2=tree.query_ball_point(nearby_point ,r)
-            idx=list(set(idx)|set(idx2))                
-        idx=list(set(idx)|set(idx2))
-        i=i+1
-    print(idx)
-    return idx    
-
-#Automatic find ROI bg color from 
-def AutoROIbg(img):
-    """
-    Function to find ROI color from BW image:
-        if ROI is 255, then the bg is 0
-    """
-    bg=int(np.mean(img))
-    if bg<128:
-        ROI =255
-    else:
-        ROI = 0
-    return ROI
+# -*- coding: utf-8 -*-
+"""
+in-situ TEM Toolbox - Data process 
+
+Assembles of functions related to movie input output
+
+Example:
+    
+    import insitu_DP as DP
+    IO.f2tif(path,1)
+
+Created on Tue Jun 11 10:25:25 2019
+@author: Mona
+"""
+import numpy as np
+
+def readcsvCol(path,col):
+    """
+    Function to read csv rol into array 
+    Inputs: file path; col number
+    Output: 1D np array
+        
+    Example: 
+        x = readcsvCol(path,1)
+    """
+    import csv
+    x=[]
+    with open(path,'r') as csvfile:
+        plots = csv.reader(csvfile, delimiter=',')
+        for row in plots:
+            if row[col]=='':
+                x.append(np.nan)
+            else:
+                x.append(float(row[col]))
+#        plt.plot(x,y) #to check if  the read  result is correct
+    return x
+def readcsv(path,col_list):
+    """
+    Function to read csv rol into array 
+    Inputs: file path; col number list
+    Output: 1D np array
+        
+    Example: 
+        x = readcsv(path,[0:3])
+    """
+#    w= len(col_list)
+    x=readcsvCol(path,col_list[0])
+#    l = len(x)
+    D=np.zeros((len(x),len(col_list)))
+    i=0
+    for col in col_list:
+        
+        x=readcsvCol(path,col)
+        D[:,i]=x
+        i=i+1
+#        D = [D, x]
+    return D
+
+    
+def writeCSV(pathout,data):
+#    import csv
+    import numpy as np
+#    (length,width)=np.shape(data)
+#    np.savetxt(pathout, data, fmt='%1.4d', delimiter=",") 
+    np.savetxt(pathout, data, fmt='%.4f', delimiter=",")   
+    
+def plot2ani(x,y,outpath,label,w=800,h=600,fps=10,dpi=72,tl_size=20,c='r'):
+    """
+    Function to make plot into animation 
+    Inputs: 
+        data: x y; 
+        Movie setting: size: w,h ;
+                       fps; savepath
+                       label: ['xlabel','ylabel'] str array
+                       tl_size: title font size
+                       c: color of the plot line
+                       dpi: dpi for screen : 72 for 4k screen, 96 for 1080p screen
+    Output: mp4 movie
+        
+    Example: 
+        plot2ani(x,y,w,h,fps,outpath,dpi,tl_size,'r')
+
+    """
+    
+    import matplotlib.pyplot as plt
+    import matplotlib.animation as animation
+    interV=1000/fps #time interval for each frame: ms
+#    w_in=w/dpi
+#    h_in=h/dpi
+    fig, ax = plt.subplots(figsize=(w/dpi, h/dpi))#figsize unit: inch
+    plt.rcParams.update({'font.size': tl_size})
+    plt.xlabel(label[0])#Change xy label if needed
+    plt.ylabel(label[1])
+    l=plt.plot(x,y,'grey') #For inital plot
+    redLine, = plt.plot(x[:0],y[:0],color=c, lw=3)
+    time_text = ax.text(5,7,str(y[0])+'°',fontsize=20)
+#    plt.text(5, 7, str(y[0],fontsize=20))
+    def animate(i):
+        redLine.set_data(x[:i], y[:i])
+#        plt.text(5, 7, str(y[i])+'°',fontsize=20) # Text is overlapping with previous frames
+        time_text.set_text(str(round(y[i],1))+'°') 
+#        print(str(i)/len(x))
+        return tuple([redLine,]) + tuple([time_text])
+    
+    plt.tight_layout() #To avoid boarder
+    # create animation using the animate() function
+    ani = animation.FuncAnimation(fig, animate, frames=len(x), \
+                                      interval=interV, blit=True, repeat=True)
+    ani.save(outpath)
+    plt.show()
+    
+def getintensity(x,y,disk,img):
+    """
+    Function to get intensity of a disk region at point (x,y) 
+    Inputs:
+        x,y: coordinates of the detection point
+        disk: size of pixels for detection region
+        img: 2D grayscale image
+    """
+    x_l=int(x-disk)
+    x_r=int(x+disk)
+    y_l=int(y-disk)
+    y_r=int(y+disk)
+    intensity=int(np.mean(img[y_l:y_r,x_l:x_r]))
+    return intensity
+    
+
+def findconnectingpoints(points,startpoint,r,level):
+    """
+    FUnction for find all surrounding points within distance r betwwen each other from startpoint
+    return: index of all connected points
+    """
+    from scipy import spatial
+    tree = spatial.cKDTree(points, leafsize=30)
+    idx =tree.query_ball_point(startpoint,r)
+    i=0
+    while i<level:
+        for results in idx:
+            nearby_point = points[results]
+            idx2=tree.query_ball_point(nearby_point ,r)
+            idx=list(set(idx)|set(idx2))                
+        idx=list(set(idx)|set(idx2))
+        i=i+1
+    print(idx)
+    return idx    
+
+
+
+#Automatic find ROI bg color from 
+def AutoROIbg(img):
+    """
+    Function to find ROI color from BW image:
+        if ROI is 255, then the bg is 0
+    """
+    bg=int(np.mean(img))
+    if bg<128:
+        ROI =255
+    else:
+        ROI = 0
+    return ROI
```

### Comparing `insituTEM-0.1.4/insituTEM/insitu_IO.py` & `insituTEM-0.1.5/insituTEM/insitu_IO.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.4/insituTEM/insitu_Preprocess.py` & `insituTEM-0.1.5/insituTEM/insitu_Preprocess.py`

 * *Files identical despite different names*

### Comparing `insituTEM-0.1.4/insituTEM/insitu_alignment.py` & `insituTEM-0.1.5/insituTEM/insitu_alignment.py`

 * *Files identical despite different names*

