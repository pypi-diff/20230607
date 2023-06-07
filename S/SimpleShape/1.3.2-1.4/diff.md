# Comparing `tmp/SimpleShape-1.3.2.tar.gz` & `tmp/SimpleShape-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleShape-1.3.2.tar", last modified: Tue Jun  6 15:36:37 2023, max compression
+gzip compressed data, was "SimpleShape-1.4.tar", last modified: Wed Jun  7 14:19:03 2023, max compression
```

## Comparing `SimpleShape-1.3.2.tar` & `SimpleShape-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/
--rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.3.2/License.txt
--rw-rw-rw-   0        0        0     4945 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4539 2023-06-06 12:50:04.000000 SimpleShape-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 15:36:37.129231 SimpleShape-1.3.2/SimpleShape/
--rw-rw-rw-   0        0        0      780 2023-06-06 06:03:25.000000 SimpleShape-1.3.2/SimpleShape/Example.py
--rw-rw-rw-   0        0        0    14010 2023-06-06 11:28:46.000000 SimpleShape-1.3.2/SimpleShape/SimpleShape.py
--rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.3.2/SimpleShape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/SimpleShape.egg-info/
--rw-rw-rw-   0        0        0     4945 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-06-06 15:24:47.000000 SimpleShape-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:19:03.276669 SimpleShape-1.4/
+-rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.4/License.txt
+-rw-rw-rw-   0        0        0     5050 2023-06-07 14:19:03.276669 SimpleShape-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4646 2023-06-07 10:02:13.000000 SimpleShape-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:19:03.269768 SimpleShape-1.4/SimpleShape/
+-rw-rw-rw-   0        0        0      797 2023-06-06 15:53:11.000000 SimpleShape-1.4/SimpleShape/Example.py
+-rw-rw-rw-   0        0        0    14277 2023-06-07 13:39:33.000000 SimpleShape-1.4/SimpleShape/SimpleShape.py
+-rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.4/SimpleShape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:19:03.276669 SimpleShape-1.4/SimpleShape.egg-info/
+-rw-rw-rw-   0        0        0     5050 2023-06-07 14:19:02.000000 SimpleShape-1.4/SimpleShape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-07 14:19:03.000000 SimpleShape-1.4/SimpleShape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:19:02.000000 SimpleShape-1.4/SimpleShape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 14:19:02.000000 SimpleShape-1.4/SimpleShape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-07 14:19:03.276669 SimpleShape-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      972 2023-06-07 14:17:00.000000 SimpleShape-1.4/setup.py
```

### Comparing `SimpleShape-1.3.2/License.txt` & `SimpleShape-1.4/License.txt`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.3.2/PKG-INFO` & `SimpleShape-1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-Metadata-Version: 2.1
-Name: SimpleShape
-Version: 1.3.2
-Summary: A simple package for creating geometric objects
-Author: Tilen Žel
-Author-email: tilen.zel@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: License.txt
-
 # README
 
 This project enables the creation of different geometric objects, on which we can perform different operations, like calculation of their perimeter.
 
 ## Features
 
 - Create and visualise various geometric objects: Triangle, Rectangle, Polygon, Circle and Ellipse
 - Calculate their perimeter and their area
 - Check if two objects intersect
 - Save and load geometric objects to and from JSON files
 
 ## Installation
 
-Download and expand the zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
+Download the project with **pip install SimpleShape** and then call it in your python document with **from SimpleShape import SimpleShape**. Alternatively, download and expand the .zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document and then write **import SimpleShape** in it.
 
 ## 1. Instructions
 
 To start using this project, create the Geometric object with available classes and perform different methods (see section 1.1). You can also check example.py, located in the SimpleShape subfolder, for a quick overwiev on how to use this package.
 
 This package also provides various functions that are described in section 1.2.
 
@@ -40,38 +27,38 @@
 
 ###### Parent class has following methods:
 
 - \_\_init__(self, coordinates): Initialization method for the object.
 - \_\_str__(self) -> str: String representation of the object, obtained using print(object)
 - perimeter(self) -> float: Returns the perimeter of the geometric object
 - area(self) -> float: Returns the area of the geometric object
-- intersect(self, other) -> bool: Check if two objects intersect. Note that tangency also counts as intersection
+- intersect(self, other) -> bool: Check if two objects intersect. **Note that tangency also counts as intersection**
 - visualize(self): Visualize the object using matplotlib module
 
 Aside from these methods, there are various functions to convert geometric objects to and from JSON format. See section 1.2 for more details.
 
 ##### Class Triangle(coordinates):
 
 A class for creating triangles using three points (f.e. coordinates = [(0,0), (2,0), (4,4)]).
 
 ##### Class Rectangle(coordinates):
 
 A class for creating rectangles using four points that need to be inserted in clockwise or counter-clockwise order. 
 
 ##### Class Polygon(coordinates):
 
-A class for creating polygons using three or more points that need to be inserted in fixed order. If the polygon is self-intersecting, the area() method does not return correct values.
+A class for creating polygons using three or more points that need to be inserted in fixed order. If the polygon is self-intersecting, the .area() method does not return correct values.
 
 ##### Class Circle(r, center = (0, 0)):
 
 A class for creating circles. Here, r is radius (r > 0) and center (default value (0,0)) represents center of the circle on x-y plane. 
 
-##### Class Ellipse(a, b, f = 0, center = (0, 0)):
+##### Class Ellipse(width, height, f = 0, center = (0, 0)):
 
-A class for creating ellipses. Here, a is the width of the ellipse, b is its height (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
+A class for creating ellipses. Here, width is width of the ellipse, height is its height (width, height > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
 
 ### 1.2 Functions
 
 This package contains functions for working with JSON data as well as other functions that perform different operations on geometric objects.
 
 ##### JSON functions:
 
@@ -84,8 +71,8 @@
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
 - **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
 - **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
-**Note: Tangency also counts as intersection!**
+**Note: Tangency also counts as intersection!**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SimpleShape-1.3.2/README.md` & `SimpleShape-1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+Metadata-Version: 2.1
+Name: SimpleShape
+Version: 1.4
+Summary: A simple package for creating geometric objects
+Author: Tilen Žel
+Author-email: tilen.zel@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: License.txt
+
 # README
 
 This project enables the creation of different geometric objects, on which we can perform different operations, like calculation of their perimeter.
 
 ## Features
 
 - Create and visualise various geometric objects: Triangle, Rectangle, Polygon, Circle and Ellipse
 - Calculate their perimeter and their area
 - Check if two objects intersect
 - Save and load geometric objects to and from JSON files
 
 ## Installation
 
-Download and expand the zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
+Download the project with **pip install SimpleShape** and then call it in your python document with **from SimpleShape import SimpleShape**. Alternatively, download and expand the .zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document and then write **import SimpleShape** in it.
 
 ## 1. Instructions
 
 To start using this project, create the Geometric object with available classes and perform different methods (see section 1.1). You can also check example.py, located in the SimpleShape subfolder, for a quick overwiev on how to use this package.
 
 This package also provides various functions that are described in section 1.2.
 
@@ -27,38 +40,38 @@
 
 ###### Parent class has following methods:
 
 - \_\_init__(self, coordinates): Initialization method for the object.
 - \_\_str__(self) -> str: String representation of the object, obtained using print(object)
 - perimeter(self) -> float: Returns the perimeter of the geometric object
 - area(self) -> float: Returns the area of the geometric object
-- intersect(self, other) -> bool: Check if two objects intersect. Note that tangency also counts as intersection
+- intersect(self, other) -> bool: Check if two objects intersect. **Note that tangency also counts as intersection**
 - visualize(self): Visualize the object using matplotlib module
 
 Aside from these methods, there are various functions to convert geometric objects to and from JSON format. See section 1.2 for more details.
 
 ##### Class Triangle(coordinates):
 
 A class for creating triangles using three points (f.e. coordinates = [(0,0), (2,0), (4,4)]).
 
 ##### Class Rectangle(coordinates):
 
 A class for creating rectangles using four points that need to be inserted in clockwise or counter-clockwise order. 
 
 ##### Class Polygon(coordinates):
 
-A class for creating polygons using three or more points that need to be inserted in fixed order. If the polygon is self-intersecting, the area() method does not return correct values.
+A class for creating polygons using three or more points that need to be inserted in fixed order. If the polygon is self-intersecting, the .area() method does not return correct values.
 
 ##### Class Circle(r, center = (0, 0)):
 
 A class for creating circles. Here, r is radius (r > 0) and center (default value (0,0)) represents center of the circle on x-y plane. 
 
-##### Class Ellipse(a, b, f = 0, center = (0, 0)):
+##### Class Ellipse(width, height, f = 0, center = (0, 0)):
 
-A class for creating ellipses. Here, a is the width of the ellipse, b is its height (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
+A class for creating ellipses. Here, width is width of the ellipse, height is its height (width, height > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
 
 ### 1.2 Functions
 
 This package contains functions for working with JSON data as well as other functions that perform different operations on geometric objects.
 
 ##### JSON functions:
 
@@ -71,8 +84,8 @@
 
 - **random_shape(shape)**: Create a geometric object of random dimensions. If the shape parameter is not specified, an arbitrary geometric object will be returned. Otherwise, insert one of the following as an argument: "Rectangle", "Triangle", "Circle", "Ellipse", "Polygon".
 - **rotate(P1, P2, f)**: Rotate point P1 (x1,y1) around point P2 (x2,y2) for angle f in radians.        
 - **intersect(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) intersect
 - **parallel(A,B,C,D)**: Check if two line segments (AB and CD, where each capital letter represents a point (x, y) on x-y plane) are parallel
 - **Line_Intersect_Circle(A, B, c, r)**: Check if line segment AB intersect a circle with radius r > 0 and central point c (x, y).
 
-**Note: Tangency also counts as intersection!**
+**Note: Tangency also counts as intersection!**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `SimpleShape-1.3.2/SimpleShape/Example.py` & `SimpleShape-1.4/SimpleShape/Example.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Example document to provide a quick overwiev on how to use this package
 """
 
 # Import the Main file
-import SimpleShape as sh
+from SimpleShape import SimpleShape as sh
 
 # a) Create a Triangle and perform simple operations
 
 My_triangle = sh.Triangle([[1,1],[3,1],[4,3]])
 print(My_triangle)
 print("Perimeter of this triangle is " + str(My_triangle.perimeter()))
 print("Area of this triangle is " + str(My_triangle.area()))
```

### Comparing `SimpleShape-1.3.2/SimpleShape/SimpleShape.py` & `SimpleShape-1.4/SimpleShape/SimpleShape.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,26 +46,24 @@
                   self.coordinates[i][0] * self.coordinates[i-1][1])
         return abs(s/2)
             
     
     def intersect(self, other) -> bool:
         """Check if there is an intersection. This includes tangency"""
         if self.__class__.__name__ in ('Triangle','Rectangle','Polygon'):
-            if isinstance(other, (Triangle or Rectangle or Polygon)):
+            if other.__class__.__name__ in ('Triangle','Rectangle','Polygon'):
                 for i in range(len(self.coordinates)):
                     for j in range(len(other.coordinates)):
                         if intersect(self.coordinates[i-1],self.coordinates[i],
                                      other.coordinates[j-1],other.coordinates[j]):
                             return True
                 return False
             elif isinstance(other, Circle):
                 for i in range(len(self.coordinates)):
-                    if Line_Intersect_Circle(self.coordinates[i-1], 
-                                             self.coordinates[i], 
-                                             other.center, other.r):
+                    if Line_Intersect_Circle(self.coordinates[i-1], self.coordinates[i], other.center, other.r):
                         return True
                 return False
             
             elif isinstance(other, Ellipse):
                 return "This feature has yet to be implemented"
             else:
                 raise Warning("Invalid shape type for intersection check")
@@ -75,19 +73,17 @@
         elif self.__class__.__name__ == ('Circle'):
             if isinstance(other, Circle):
                 distance = sqrt((self.center[0]-other.center[0])**2+
                             (self.center[1]-other.center[1])**2)
                 if distance > abs(self.r - other.r): 
                     return distance <= (self.r + other.r)
                 return False
-            elif isinstance(other, (Triangle or Rectangle or Polygon)):
+            elif other.__class__.__name__ in ('Triangle','Rectangle','Polygon'):
                 for i in range(len(other.coordinates)):
-                    if Line_Intersect_Circle(other.coordinates[i-1], 
-                                             other.coordinates[i], 
-                                             self.center, self.r):
+                    if Line_Intersect_Circle(other.coordinates[i-1], other.coordinates[i], self.center, self.r):
                         return True
                 return False
             elif isinstance(other, Ellipse):
                 return "This feature has yet to be implemented"
             else:
                 raise Warning("Invalid shape type for intersection check")
 
@@ -95,15 +91,15 @@
         elif self.__class__.__name__ == ('Ellipse'):
             return "This feature has yet to be implemented"
         else:
             raise Warning("Invalid shape type for intersection check")
             
     
     def visualize(self) -> None:
-        
+        """Visualize the object using Matplotlib module"""
         X = np.array(self.coordinates)
         plt.figure()
         plt.scatter(X[:, 0], X[:, 1], s = 20)
         t1 = plt.Polygon(X[:,:])
         plt.gca().add_patch(t1)
         plt.show()
 
@@ -140,15 +136,15 @@
         self.bc = (self.b[0]-self.c[0],self.b[1]-self.c[1])
         self.cd = (self.c[0]-self.d[0],self.c[1]-self.d[1])
         self.da = (self.d[0]-self.a[0],self.d[1]-self.a[1])
         
         self.ac = sqrt((self.a[0]-self.c[0])**2+(self.a[1]-self.c[1])**2)
         self.bd = sqrt((self.b[0]-self.d[0])**2+(self.b[1]-self.d[1])**2)
 
-        eps = 1e-6
+        eps = 1e-8
         if (len(self.coordinates) != 4):
             raise Warning("Provide a 4x2 array or tuple")
         if (self.ab[0]+self.cd[0]>eps or self.bc[0]+self.da[0]>eps or self.ac-self.bd>eps):
             raise Warning('Not a rectangle. Try again')
         if (self.ab[1]+self.cd[1]>eps or self.bc[1]+self.da[1]>eps):
             raise Warning('Not a rectangle. Try again')
         if self.a in (self.b, self.c, self.d):
@@ -193,63 +189,66 @@
         if len(self.center) != 2: raise Warning("Use a center point with two dimensions")
     
     def __str__(self):
         return ("Circle with radius " + str(self.r) + " and center in " +
                 str(self.center)) 
 
     def area(self):
+        """pi * r**2"""
         return pi * self.r**2
 
     def perimeter(self):
+        """2 * pi * r"""
         return 2 * pi * self.r
            
            
     def visualize(self):
         circle=plt.Circle(self.center, self.r)
         fig, ax = plt.subplots()
         ax.set_xlim((self.center[0]-1.1*self.r, self.center[0]+self.r*1.1))
         ax.set_ylim((self.center[1]-1.1*self.r, self.center[1]+self.r*1.1))
         ax.add_patch(circle)
         plt.show()
 
     
 class Ellipse(Geometry):
-    def __init__(self, a, b, f = 0, center = (0,0)):
+    def __init__(self, width, height, f = 0, center = (0,0)):
         self.type = self.__class__.__name__
-        self.a = a
-        self.b = b
+        self.width = width
+        self.height = height
         self.f = f
         self.center = center
 
-        if a <= 0: raise Warning("a is 0 or less. Use another a")
-        if b <= 0: raise Warning("b is 0 or less. Use another b")
+        if self.width <= 0: raise Warning("Width is 0 or less. Use another width")
+        if self.height <= 0: raise Warning("Height is 0 or less. Use another height")
         if len(self.center) != 2: raise Warning("Use a center point with two dimensions")
         
     def __str__(self):
-        return ("Ellipse with a = " + str(self.a) + ", b = " + str(self.b) +
+        return ("Ellipse with width = " + str(self.width) + ", height = " + str(self.height) +
                 ", rotation of " + str(self.f) + "° and center at " + str(self.center)) 
 
     def area(self):
-        return pi * self.a * self.b
+        """pi * width * height"""
+        return pi * self.width * self.height
 
     def perimeter(self):
-        """Approximate calculation using Ramaujan formula"""
-        return pi * (3*(self.a+self.b) - 
-                     sqrt((3*self.a + self.b) * (self.a + 3*self.b)))
+        """Approximate calculation using Ramanujan formula"""
+        return pi * (3*(self.width+self.height) - 
+                     sqrt((3*self.width + self.height) * (self.width + 3 * self.height)))
            
     def visualize(self):
         fig, ax = plt.subplots()
 
         ax.axis('equal')
-        ell = _Ellipse(xy=self.center, width=self.a, height=self.b, angle=self.f
+        ell = _Ellipse(xy=self.center, width=self.width, height=self.height, angle=self.f
                        , lw=4)
         
         ax.add_artist(ell)
         
-        temp = max(self.a,self.b)
+        temp = max(self.width,self.height)
         ax.set_xlim((self.center[0]-1.1*temp, self.center[0]+temp*1.1))
         ax.set_ylim((self.center[1]-1.1*temp, self.center[1]+temp*1.1))
         
         plt.show()
 
 
 # JSON functions
@@ -260,68 +259,68 @@
     
 def save_shapes(json_data, filename):
     """Write JSON string to a .json file"""
     with open(filename, 'w') as outfile:
         outfile.write(json_data)
         
 def load_shapes(filename):
-    """Convert a .json file to a JSON string"""
+    """Create JSON string from a .json file"""
     with open(filename, 'r') as file:
         json_data = json.load(file)
     return json_data 
         
 
 def from_json(json_data):
-    """Create a list of objects from JSON string"""
+    """Create a list of objects from a JSON string"""
     object_list = []
     for element in json_data:
         if element['type'] == 'Triangle':
             object_list.append(Triangle(element['coordinates']))
         elif element['type'] == 'Rectangle':
             object_list.append(Rectangle(element['coordinates']))
         elif element['type'] == 'Polygon':
             object_list.append(Polygon(element['coordinates']))
         elif element['type'] == 'Circle':
             object_list.append(Circle(element['r'], element['center']))
         elif element['type'] == 'Ellipse':
-            object_list.append(Ellipse(element['a'],element['b'],
+            object_list.append(Ellipse(element['width'],element['height'],
                            element['f'], element['center']))
         else:
             print('Invalid JSON data. Will not be used to create an object')
     return object_list
 
 # Other functions
 
 def random_shape(shape = next(iter({"Rectangle", "Triangle", "Circle", "Ellipse", "Polygon"}))):
     
     if shape == "Triangle":
         a,b,c = np.random.uniform(-1000, 1000,(3,2))
         return Triangle(([a[0],a[1]],[b[0],b[1]],[c[0],c[1]]))
     elif shape == "Rectangle":
-        [a, b] = np.random.uniform(-1000,1000, (2,1))
-        _min = min(a,b)[0]
-        _max = max(a,b)[0]
+        [a, b] = np.random.uniform(-1000,1000, 2)
+        _min = min(a,b)
+        _max = max(a,b)
         avg = (_min+_max)/2
         center=(avg,avg)
         f = 2*pi*np.random.uniform(0,1) # Radians
         P1,P2,P3,P4 = [_min,_min],[_max,_min],[_max,_max],[_min,_max]
         P1,P2,P3,P4 = rotate(P1,center,f),rotate(P2,center,f), rotate(P3,center,f), rotate(P4,center,f)
         return Rectangle([P1,P2,P3,P4])
     elif shape == "Polygon":
         num = np.random.randint(3,100)	
         return Polygon(np.random.uniform(-1000, 1000, (num,2)))
     elif shape == "Circle":
         r = np.random.uniform(0.1,1000)
-        [x, y] = np.random.uniform(-1000,1000, (2,1))
-        return Circle(r,(x[0],y[0]))
+        [x, y] = np.random.uniform(-1000,1000, 2)
+        return Circle(r,(x,y))
     elif shape =="Ellipse":
-        [a, b] = np.random.uniform(0.1,1000, (2,1))
-        [x, y] = np.random.uniform(-1000,1000, (2,1))
+        [a, b] = np.random.uniform(0.1,1000, 2)
+        [x, y] = np.random.uniform(-1000,1000, 2)
         f = 360*np.random.uniform(0,1)
-        return Ellipse(a[0], b[0], f, (x[0],y[0]))
+        return Ellipse(a, b, f, (x, y))
     else:
         raise ValueError("Invalid shape type for creating random shape")
 
 # Rotate P1 around P2 for angle f in radians        
 # https://stackoverflow.com/questions/4465931/rotate-rectangle-around-a-point
 
 def rotate(P1, P2, f):
@@ -342,27 +341,29 @@
 def parallel(A,B,C,D):
     if B[0] == A[0]: return (True if C[0] == D[0] else False)
     if C[0] == D[0]: return (True if A[0] == B[0] else False)
     return (B[1]-A[1])/(B[0]-A[0]) == (D[1]-C[1])/(D[0]-C[0])
 
 # Taken and modified from 
 # https://stackoverflow.com/questions/1073336/circle-line-segment-collision-detection-algorithm
-# (chmike answer)
+# (bobobobo answer)
 
-def Line_Intersect_Circle(A, B, c, r):
 
-    LAB = sqrt((B[0]-A[0])**2 + (B[1]-A[1])**2)
-    
-    Dx = (B[0]-A[0])/LAB
-    Dy = (B[1]-A[1])/LAB
-    
-    t = Dx * (c[0] - A[0]) + Dy * (c[1] - A[1])    
-    
-    Ex = t*Dx+A[0]
-    Ey = t*Dy+A[1]
-    
-    LEC = sqrt((Ex-c[0])**2+(Ey-c[1])**2)
-    
-    if LEC <= r: return True
-
-    return False
-    
+def Line_Intersect_Circle(A, B, C, r):
+    d = (B[0]-A[0],B[1]-A[1])
+    f = (A[0]-C[0],A[1]-C[1])
+
+    a = d[0]*d[0]+d[1]*d[1]
+    b = 2*(f[0]*d[0]+f[1]*d[1])
+    c = f[0]*f[0]+f[1]*f[1]- r*r
+    discriminant = b*b - 4*a*c
+    if discriminant < 0:
+        return False
+    else:
+        discriminant = sqrt(discriminant)
+        t1 = (-b - discriminant)/(2*a)
+        t2 = (-b + discriminant)/(2*a)
+        if t1 >= 0 and t1 <= 1:
+            return True
+        if t2 >= 0 and t2 <= 1:
+            return True
+        return False
```

### Comparing `SimpleShape-1.3.2/SimpleShape.egg-info/PKG-INFO` & `SimpleShape-1.4/SimpleShape.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleShape
-Version: 1.3.2
+Version: 1.4
 Summary: A simple package for creating geometric objects
 Author: Tilen Žel
 Author-email: tilen.zel@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 - Create and visualise various geometric objects: Triangle, Rectangle, Polygon, Circle and Ellipse
 - Calculate their perimeter and their area
 - Check if two objects intersect
 - Save and load geometric objects to and from JSON files
 
 ## Installation
 
-Download and expand the zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document, or use **pip install SimpleShape**. Then, write **import SimpleShape** in your python document to begin using the package.
+Download the project with **pip install SimpleShape** and then call it in your python document with **from SimpleShape import SimpleShape**. Alternatively, download and expand the .zip (.tar.gz) file and insert the SimpleShape.py function, located in the SimpleShape subfolder, to location of your python document and then write **import SimpleShape** in it.
 
 ## 1. Instructions
 
 To start using this project, create the Geometric object with available classes and perform different methods (see section 1.1). You can also check example.py, located in the SimpleShape subfolder, for a quick overwiev on how to use this package.
 
 This package also provides various functions that are described in section 1.2.
 
@@ -40,38 +40,38 @@
 
 ###### Parent class has following methods:
 
 - \_\_init__(self, coordinates): Initialization method for the object.
 - \_\_str__(self) -> str: String representation of the object, obtained using print(object)
 - perimeter(self) -> float: Returns the perimeter of the geometric object
 - area(self) -> float: Returns the area of the geometric object
-- intersect(self, other) -> bool: Check if two objects intersect. Note that tangency also counts as intersection
+- intersect(self, other) -> bool: Check if two objects intersect. **Note that tangency also counts as intersection**
 - visualize(self): Visualize the object using matplotlib module
 
 Aside from these methods, there are various functions to convert geometric objects to and from JSON format. See section 1.2 for more details.
 
 ##### Class Triangle(coordinates):
 
 A class for creating triangles using three points (f.e. coordinates = [(0,0), (2,0), (4,4)]).
 
 ##### Class Rectangle(coordinates):
 
 A class for creating rectangles using four points that need to be inserted in clockwise or counter-clockwise order. 
 
 ##### Class Polygon(coordinates):
 
-A class for creating polygons using three or more points that need to be inserted in fixed order. If the polygon is self-intersecting, the area() method does not return correct values.
+A class for creating polygons using three or more points that need to be inserted in fixed order. If the polygon is self-intersecting, the .area() method does not return correct values.
 
 ##### Class Circle(r, center = (0, 0)):
 
 A class for creating circles. Here, r is radius (r > 0) and center (default value (0,0)) represents center of the circle on x-y plane. 
 
-##### Class Ellipse(a, b, f = 0, center = (0, 0)):
+##### Class Ellipse(width, height, f = 0, center = (0, 0)):
 
-A class for creating ellipses. Here, a is the width of the ellipse, b is its height (a,b > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
+A class for creating ellipses. Here, width is width of the ellipse, height is its height (width, height > 0), f is the rotation in counter-clockwise direction (in degrees, default value 0) and center represents center of ellipse on x-y plane (default value (0,0)). 
 
 ### 1.2 Functions
 
 This package contains functions for working with JSON data as well as other functions that perform different operations on geometric objects.
 
 ##### JSON functions:
```

