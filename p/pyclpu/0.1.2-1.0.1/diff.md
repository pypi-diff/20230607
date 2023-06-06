# Comparing `tmp/pyclpu-0.1.2.tar.gz` & `tmp/pyclpu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyclpu-0.1.2.tar", last modified: Mon Jun  5 18:16:42 2023, max compression
+gzip compressed data, was "pyclpu-1.0.1.tar", last modified: Tue Jun  6 23:26:26 2023, max compression
```

## Comparing `pyclpu-0.1.2.tar` & `pyclpu-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 18:16:42.000000 pyclpu-0.1.2/
--rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4942 2023-06-05 18:16:42.000000 pyclpu-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu/
--rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/constants.py
--rw-rw-rw-   0        0        0      942 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/formats.py
--rw-rw-rw-   0        0        0    17586 2023-06-05 18:10:54.000000 pyclpu-0.1.2/pyclpu/image.py
--rw-rw-rw-   0        0        0    30733 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/main.py
--rw-rw-rw-   0        0        0    11328 2023-06-05 15:34:37.000000 pyclpu-0.1.2/pyclpu/manager.py
--rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/s33293804.py
--rw-rw-rw-   0        0        0      629 2023-06-05 18:14:49.000000 pyclpu-0.1.2/pyclpu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4942 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0      311 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4512 2023-06-05 18:16:30.000000 pyclpu-0.1.2/README.md
--rw-rw-rw-   0        0        0       92 2023-06-05 18:16:42.000000 pyclpu-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2090 2023-06-02 13:14:02.000000 pyclpu-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:26:26.914511 pyclpu-1.0.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7118 2023-06-06 23:26:26.914511 pyclpu-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6710 2023-06-06 23:24:20.000000 pyclpu-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 23:26:26.898608 pyclpu-1.0.1/pyclpu/
+-rw-rw-rw-   0        0        0      629 2023-06-06 23:23:32.000000 pyclpu-1.0.1/pyclpu/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-1.0.1/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      942 2023-06-02 09:58:39.000000 pyclpu-1.0.1/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    20399 2023-06-06 22:44:46.000000 pyclpu-1.0.1/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30305 2023-06-06 17:11:29.000000 pyclpu-1.0.1/pyclpu/main.py
+-rw-rw-rw-   0        0        0    13273 2023-06-06 23:18:44.000000 pyclpu-1.0.1/pyclpu/manager.py
+-rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-1.0.1/pyclpu/s33293804.py
+drwxrwxrwx   0        0        0        0 2023-06-06 23:26:26.914511 pyclpu-1.0.1/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0     7118 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 23:26:26.000000 pyclpu-1.0.1/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-06-06 23:26:26.914511 pyclpu-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2295 2023-06-06 23:25:59.000000 pyclpu-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyclpu-0.1.2/LICENSE` & `pyclpu-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.2/pyclpu/constants.py` & `pyclpu-1.0.1/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.2/pyclpu/formats.py` & `pyclpu-1.0.1/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.2/pyclpu/image.py` & `pyclpu-1.0.1/pyclpu/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-This is the CLPU module for image manipulation. Please do only add or modify but not delete content.
-
-project             standardized modules for often used python functions at CLPU
-acronym             pyCLPU
-created on          2023-05-31 20:11:00
-
-@author             Micha (MEmx), CLPU, Villamayor, Spain
-@moderator          Eduardo, CLPU, Villamayor, Spain
-@updator            Diego (MEmx), CLPU, Villamayor, Spain
-            
-@contact            mehret@clpu.es
+""" This is the CLPU module for image manipulation.
 
-interpreter         python > 3.5
-version control     git
+Please do only add or modify but not delete content.
 
 requires explicitely {
  - os
  - sys
  - numpy
  - cv2
  - PIL
@@ -91,36 +79,89 @@
 
 
 # =============================================================================
 # METHODS
 # =============================================================================
 # INTEGRATION AND TESTING
 def test_pingpong(*args, **kwargs):
+    """ Tests functionality of functions. 
+ 
+    Function prints any input.
+ 
+    Args:
+        `*args`   : Any number of positional arguments.
+        `**kwargs`: Any number of named keyval arguments.
+    
+    Returns:
+        exit_stat (bool) : True in case of success and False else.
+    
+    Examples:
+        ```python
+        test_pingpong(True,kwa=True)
+        ```
+        returns
+        ```
+        True
+        kwa : True
+        ```
+    """
     try:
         for arg in args:
             print(arg)
         for key, value in kwargs.items():
             print(str(key) + " : "+ str(value))
     except:
         return False
     return True
 
 # IMAGE T/I/O
-def isimg(path):
+def isimg(path: str) -> bool:
+    """ Checks for image file. 
+ 
+    The function looks up if the argument of type string describes the path to an image file.
+ 
+    Args:
+        path (str) : The path which is to be checked.
+    
+    Returns:
+        exit_stat (bool) : True in case there is an image file and False else.
+    
+    Examples:
+        ```python
+        isimg("")
+        ```
+        returns
+        ```
+        False
+        ```
+        
+    Todo:
+        * accept image object as input as well
+    """
     global global_load_method
     try:
         extension = give_extension(path)
         if extension in formats.acceptedinput[global_load_method]:
             return True
         else:
             return False
     except:
         error(isimg.__name__,"",code=1287)
 
 def imread(path):
+    """ Reads image file. 
+ 
+    The function tries to read an image file to a numpy array as `[channel,y,x]`.
+ 
+    Args:
+        path (str) : The path to an image file.
+    
+    Returns:
+        img (:obj: `numpy.array`) : Matrix of color values as ``[channel,y,x]``
+    """
     global global_load_method
     if global_load_method == 'opencv':
         img = cv2.imread(path,cv2.IMREAD_UNCHANGED)
         if img is None: # happens if there is trouble with the path -> 8bit PIL
             try:
                 img = PIL.Image.open(path)
                 img = img.convert("RGB")
@@ -212,34 +253,78 @@
 # INTERACTIVE IMAGE
 class Interactive:
     def __new__(cls, *args, **kwargs):
         #1) Create from this class as cls a new instance of an object Main
         return Main(*args, **kwargs)
         
 class PointPicker():
-    """
+    """ Interactive point picker.
     The class allows interactive picking of a veriable number of points in a picture.
     
-    Call as a = image.PointPicker("n" = 4, image = image.imread("path/to/test.jpg"))
+    Args:
+        image  (:obj: ``numpy.array``,optional) : Source image.
+        n      (int,optional) : Number of points that should be picked.
+    
+    Attributes:
+        status (bool) : True if processing was successfull, else False.
+            Initializes to False.
+    
+    Returns:
+        point_list (:obj: ``numpy.array``) : List of picked or parsed points of shape `(n,2)`.
+        
+    Note:
+        The source image is not part of the object after processing.
+        
+    Examples:
+        The class can be used in a functional way
+
+        ```python 
+        from pyclpu import image
+        pick = image.PointPicker(image = image.imread("path/to/test.jpg"))
+        ```
+
+        A more object oriented use case demonstrates how a run can be started after initialization
+
+        ```python 
+        from pyclpu import image
+        pick = image.PointPicker()
+        image = image.imread("path/to/test.jpg")
+        pick.image = image
+        pick.n = 3
+        pick.run()
+        pick.status
+        ```
+        returns
+        ```
+        True
+        ```
     """
     # INI
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         self.__dict__.update(kwargs)
+        self.status = False
         # INTEGRITY
         if not hasattr(self, 'image'):
             warning(self.__class__.__name__,"No source image `IMG` defined, expect key `image` as `image=IMG`.")
         if not hasattr(self, 'n'):
             warning(self.__class__.__name__,"No number of points defined, expect key `n` as `n=INT`.")
         # IN PLACE
         if hasattr(self, 'image') and hasattr(self, 'n'):
             self.__run__()
         return None
-    def __run__(self):    
+    def __run__(self):
+        # INTEGRITY
+        if not hasattr(self, 'image'):
+            error(self.__class__.__name__,"No source image `IMG` defined, expect key `image` as `image=IMG`. DO NOTHING.",1169)
+            return None
+        if not hasattr(self, 'n'):
+            error(self.__class__.__name__,"No number of points defined, expect key `n` as `n=INT`. DO NOTHING.",1169)
+            return None
         # VARIABLES
         self.point_list = np.zeros((self.n, 2), dtype = "int")
         self.point_list_pointer = 0
         # METHODS
         def click_and_get(event, x, y, flags, param):
             '''
             HELPER FUNCTION: CLICK EVENT FUNCTION
@@ -294,60 +379,69 @@
             self.status = True
         # housekeeping
         cv2.destroyAllWindows()
         del self.image
         del self.enhanced
         del self.drawing
         return None
+    def start(self):
+        # START
+        self.__run__()
 
 # IMAGE MANIPULATION
 class Manipulate:
     def __new__(cls, *args, **kwargs):
         #1) Create from this class as cls a new instance of an object Main
         return Main(*args, **kwargs)
         
 class PerspectiveTransform():
     """
     The class allows to transform a linearly distorted input image into a trapez-corrected view on it. Coordinates are interpreted as (x,y).
     
-    The class can be used in a functional way
-
-    ```
-    from pyclpu import image
-
-    warp = image.PerspectiveTransform(source = image.imread("path/to/test.jpg")) 
-    ```
-
-    with output
-    - the warped image in `warp.warped` and 
-    - the coordinates of cornes from the source image stored in `warp.sourcecorners`.
-
-    Note that the source image is not part of the object in its final form. The coordinates of the corner points of the target rectangle can also be parsed to the function as `np.array()` of shape `(4,2)` with the keyword `sourcecorners`. A more object oriented use case can deal with loops where all warps have the same source corner coordinates
-
-    ```
-    from pyclpu import image
-
-    warp_it = image.PerspectiveTransform()
-
-    image_stack = image.imread(path/to/directory/with/many/images/)
-
-    warp = []
-
-    for image in image_stack:
-        warp_it.source = image
-        warp.append[{"warped" : warp.warped, "sourcecorners" : warp.sourcecorners}]
-    ```
+    Args:
+        source  (:obj: ``numpy.array``,optional) : Source image.
+        sourcecorners (:obj: ``PointPicker``,optional) : Object of type `PointPicker`, i.e. `sourcecorners.point_list` is a list of shape `(4,2)` which describe the source's corner coordinates in the original image matrix;`sourcecorners.n` equals 4; and `sourcecorners.status` should return True.
+    
+    Attributes:
+        status (bool) : True if processing was successfull, else False.
+            Initializes to False.
+    
+    Returns:
+        warped  (:obj: ``numpy.array``) : Warped image.
+        
+    Note:
+        The source image is not part of the object in its final form.
+    
+    Examples:
+        The class can be used in a functional way
 
-    with results beeing stored in a list `warp`. The dynamic modification of `warp.sourcecorners` is possible.
+        ```python 
+        from pyclpu import image
+        warp = image.PerspectiveTransform(source = image.imread("path/to/test.jpg"))
+        ```
+
+        A more object oriented use case can deal with loops where all warps have the same source corner coordinates
+
+        ```python 
+        from pyclpu import image
+        warp_it = image.PerspectiveTransform()
+        image_stack = image.imread("path/to/directory/with/many/images/")
+        warp = []
+        for image in image_stack:
+            warp_it.source = image
+            warp.append[{"warped" : warp.warped, "sourcecorners" : warp.sourcecorners}]
+        ```
+        with results beeing stored in a list `warp`. The dynamic modification of `warp.sourcecorners` is possible.
     """
     # INI
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         self.__dict__.update(kwargs)
+        self.status = False
         # INTEGRITY
         if not hasattr(self, 'source'):
             warning(self.__class__.__name__,"No source image `IMG` defined, expect key `source` as `source=IMG`.")
         if not hasattr(self, 'sourcecorners'):
             warning(self.__class__.__name__,"Found no corners (x,y) of target rectangle, optional key `sourcecorners` as `sourcecorners=np.array((4,2),dtype='int')`.")
         # IN PLACE
         if hasattr(self, 'source'):
@@ -405,14 +499,15 @@
         message(self.__class__.__name__,"PRESS ANY KEY TO CLOSE IMAGE AND PROCEED",headline="DISPLAY WARP")
         cv2.namedWindow(self.__class__.__name__)
         cv2.imshow(self.__class__.__name__, self.warped)
         cv2.waitKey(0)
         # housekeeping
         cv2.destroyAllWindows()
         del self.source
+        self.status = True
         return None
         
     
 # =============================================================================
 # PYTHON MAIN
 # =============================================================================
 # SELF AND TEST
```

### Comparing `pyclpu-0.1.2/pyclpu/main.py` & `pyclpu-1.0.1/pyclpu/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-This is the CLPU module. Please do only add or modify but not delete content.
+"""This is the main CLPU module. 
 
-project             standardized modules for often used python functions at CLPU
-acronym             pyCLPU
-created on          2022-05-20:11:00
-
-@author             Micha (MEmx), CLPU, Villamayor, Spain
-@moderator          Eduardo, CLPU, Villamayor, Spain
-@updator            Diego (MEmx), CLPU, Villamayor, Spain
-            
-@contact            mehret@clpu.es
-
-interpreter         python > 3.5
-version control     git
+Please do only add or modify but not delete content.
 
 requires explicitely {
   - os
   - sys
   - importlib
   - math
   - numpy
```

### Comparing `pyclpu-0.1.2/pyclpu/manager.py` & `pyclpu-1.0.1/pyclpu/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-This is the CLPU module for management tasks. Please do only add or modify but not delete content.
-
-project             standardized modules for often used python functions at CLPU
-acronym             pyCLPU
-created on          2023-06-01 20:11:00
-
-@author             Micha (MEmx), CLPU, Villamayor, Spain
-@moderator          Eduardo, CLPU, Villamayor, Spain
-@updator            Diego (MEmx), CLPU, Villamayor, Spain
-            
-@contact            mehret@clpu.es
+""" This is the CLPU module for management tasks.
 
-interpreter         python > 3.5
-version control     git
+Please do only add or modify but not delete content.
 
 requires explicitely {
  - os
  - sys
  - numpy
 }
 
@@ -43,14 +31,15 @@
 import sys
 import threading
 import time
 
 from inspect import getsourcefile
 from importlib import reload
 
+import math
 import numpy as np
 
 # INTERNAL
 root = os.path.dirname(os.path.abspath(getsourcefile(lambda:0))) # get environment
 sys.path.append(os.path.abspath(root))                           # add environment
 sys.path.append(os.path.abspath(root)+os.path.sep+"LIB")         # add library
 
@@ -185,18 +174,52 @@
         string = "(\n"
         for att in self.__dict__:
             string = string + str(att) + " -> " + str( getattr(self,att) ) + "\n"
         return str(type(self).__name__) + string + ")"
 
 # INTERACTIVE
 class CatchAndRename():
-    """
-    The class allows interactive picking of a veriable number of points in a picture.
+    """ Responsive file catcher
+    This class waits for new files in a directory and renames them upon arrival.
     
-    Call as a = image.PointPicker("n" = 4, image = image.imread("path/to/test.jpg"))
+    Args:
+        directory (str) : Path to directory where new files are expected.
+        prefix (str, optional) : Prefix of renamed filename. Defaults to `""`.
+        number (int, optional) : Suffix of renamed filename. Defaults to `0`.
+        extension (str, optional) : Extension of renamed files. Defaults to the old extension.
+        loop (bool, optional) : Activity status of the catcher. Inactive if `False`, active if `True`.
+        
+    Attributes:
+        ignored (list) : List of files which is ignored 
+    
+    Notes:
+        Rename freshly arriving files to `str(prefix+number+"."+extension)` when loop is activated by setting the input parameter `loop = True`. If elements from the list `inored` are purged during `loop = True`, then corresponding files will be renamed as they are recognized as new.
+        
+    Examples:
+        The class can be used in a functional way
+        ```
+        from pyclpu import manager
+        chase = manager.CatchAndRename(directory = "path/to/directory/", prefix = "any_string", number = 42, loop=True)
+        ```
+        A more object oriented use case is described below. The chase for new files is activated by setting the input parameter `loop = True` and paused by setting `loop = False`.
+        ```
+        from pyclpu import manager
+        import time
+
+        chase = manager.CatchAndRename()
+
+        chase.directory = "path/to/test"
+        chase.prefix = "any_string"
+        chase.number = 42
+
+        chase.loop = True
+        time.sleep(100)
+        chase.loop = False`
+        ```
+        Files that arrive in the directory during a pause will be ignored when switching on the loop again with `loop = True`.
     """
     # INI
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         # INPUT
         self.__dict__.update(kwargs)
@@ -222,14 +245,17 @@
         # INTEGRITY
         if not hasattr(self, 'directory'):
             warning(self.__class__.__name__,"No source directory defined, expect key `directory` as `directory=path/to/directorty`.")
             return None
         if not hasattr(self, 'number'):
             warning(self.__class__.__name__,"No starting integer defined, expect key `number` as `number=integer`. Set `number = 0`.")
             self.number = 0
+        if not hasattr(self, 'extension'):
+            warning(self.__class__.__name__,"No extension defined, expect key `extension`. Remain with original extension.")
+            self.extension = ""
         if not hasattr(self, 'prefix'):
             warning(self.__class__.__name__,"No prefix defined, expect key `prefix` as `prefix=any_string`. Set `prefix = ''`.")
             self.prefix = ""
         # METHODS
         #@classmethod
         def _worker(event):
             self.ignored = os.listdir(self.directory)
@@ -237,22 +263,31 @@
                 time.sleep(self.timeout)
                 file_list = os.listdir(self.directory)
                 for file in file_list:
                     if file in self.ignored:
                         continue
                     else:
                         message(self.__class__.__name__,"WORK ON  "+file)
-                        filename_and_extension = file.rsplit( ".", 1 )
                         try:
-                            extension = filename_and_extension[1]
+                            filename_and_extension = file.rsplit( ".", 1 )
+                            old_extension = filename_and_extension[1]
+                            old_basename  = filename_and_extension[0]
                         except:
-                            extension = ""
-                        new_file = self.prefix+str(self.number).zfill(3)+'.'+extension
+                            old_extension = ""
+                            old_basename  = file
+                        if self.extension == "":
+                            new_extension = old_extension
+                        else:
+                            new_extension = self.extension
+                        if math.isnan(self.number):
+                            new_file = self.prefix+old_basename+'.'+new_extension
+                        else:
+                            new_file = self.prefix+str(self.number).zfill(3)+'.'+new_extension
+                            self.number = self.number + 1
                         self.ignored.append(new_file)
-                        self.number = self.number + 1
                         old_name = os.path.join(self.directory,file)
                         new_name = os.path.join(self.directory,new_file)
                         if os.path.isfile(new_name):
                             warning(self.__class__.__name__,"FILE ALREADY EXISTS: DO NOTHING FOR "+old_name)
                             break
                         else:
                             message(self.__class__.__name__,"CREATE  "+new_name)
```

### Comparing `pyclpu-0.1.2/pyclpu/s33293804.py` & `pyclpu-1.0.1/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.2/pyclpu/__init__.py` & `pyclpu-1.0.1/pyclpu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "0.1.2"
+__version__ = "1.0.1"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-0.1.2/setup.py` & `pyclpu-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 #! anaconda create -n CLPU python=3.5 && conda activate CLPU && pip install .
-"""
-This is the setup file for pythonic CLPU utilities.
+""" Setup for pythonic CLPU utilities
+
+This module is the setup file for pythonic CLPU utilities.
 
-project             standardized modules for often used python functions at CLPU
-acronym             pyCLPU
-created on          2022-01-01 00:00:00
-
-@author             Micha (MEmx), CLPU, Villamayor, Spain
-@moderator          Eduardo, CLPU, Villamayor, Spain
-@updator            Diego (MEmx), CLPU, Villamayor, Spain
-            
-@contact            mehret@clpu.es
-
-interpreter         python > 3.5
-version control     git
-url                 https://git.clpu.es/mehret/pyclpu
+| --------------- | ---------- |
+| project         | standardized modules for often used python functions at CLPU |
+| acronym         | pyCLPU |
+| created         | 2023-05-31 20:11:00|
+| @author         | Michael Ehret (MEmx), CLPU, Villamayor, Spain |
+| @moderator      | Eduardo Flores, CLPU, Villamayor, Spain |
+| @updator        | Diego de Luis (MEmx), CLPU, Villamayor, Spain |
+| @contact        | tic@clpu.es |
+| interpreter     | python 3.11.3 |
+| version control | [git](https://git.clpu.es/mehret/pyclpu) |
+| documentation   | [html](./html/pydoc/index.html) and [markdown](./md/pydoc/index.md) |
+| --------------- | ---------- |
 
 requires explicitely {
  - setuptools
  - glob
 }
 
 execute installation via {
@@ -62,10 +62,10 @@
         'numpy','scipy','opencv-python','cython','pillow',\
         'matplotlib',\
     ],\
     # and build in modules cython, importlib.reload, inspect.getsourcefile, glob, math, opencv, pillow, os, sys, time
     classifiers=[\
         'Development Status :: 1 - Planning',\
         'Intended Audience :: Science/Research',\
-        'Programming Language :: Python :: 3.5',\
+        'Programming Language :: Python :: 3.11',\
     ],\
 )
```

