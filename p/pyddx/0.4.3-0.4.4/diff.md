# Comparing `tmp/pyddx-0.4.3.tar.gz` & `tmp/pyddx-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyddx-0.4.3.tar", last modified: Fri May 12 13:05:00 2023, max compression
+gzip compressed data, was "pyddx-0.4.4.tar", last modified: Wed Jun  7 16:10:44 2023, max compression
```

## Comparing `pyddx-0.4.3.tar` & `pyddx-0.4.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:05:00.552627 pyddx-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-12 13:02:43.000000 pyddx-0.4.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-12 13:02:43.000000 pyddx-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-12 13:02:43.000000 pyddx-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-12 13:05:00.552627 pyddx-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-12 13:02:43.000000 pyddx-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:05:00.548627 pyddx-0.4.3/pyddx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:02:52.000000 pyddx-0.4.3/pyddx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 13:05:00.000000 pyddx-0.4.3/pyddx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 13:02:43.000000 pyddx-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-12 13:05:00.552627 pyddx-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-05-12 13:02:43.000000 pyddx-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:05:00.552627 pyddx-0.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/cbessel.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx.f90
--rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx.h
--rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_cinterface.f90
--rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_constants.f90
--rw-r--r--   0 runner    (1001) docker     (123)   122788 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_cosmo.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_definitions.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_driver.f90
--rw-r--r--   0 runner    (1001) docker     (123)    73336 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_gradients.f90
--rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_harmonics.f90
--rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_lpb.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_lpb_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_mkrhs.f90
--rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_multipolar_solutes.f90
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_operators.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_parameters.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_pcm.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_solvers.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/ddx_workspace.f90
--rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/llgnew.f
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/matrix_debug.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/pyddx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31313 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/pyddx_classes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-05-12 13:02:43.000000 pyddx-0.4.3/src/pyddx_data.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.276300 pyddx-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-07 16:08:50.000000 pyddx-0.4.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-07 16:08:50.000000 pyddx-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-07 16:08:50.000000 pyddx-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-07 16:10:44.276300 pyddx-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-07 16:08:50.000000 pyddx-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.272300 pyddx-0.4.4/pyddx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:08:58.000000 pyddx-0.4.4/pyddx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-07 16:08:50.000000 pyddx-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-07 16:10:44.276300 pyddx-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-06-07 16:08:50.000000 pyddx-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.276300 pyddx-0.4.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/cbessel.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_cinterface.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_constants.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   122890 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_cosmo.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_definitions.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_driver.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    73336 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_gradients.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_harmonics.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_lpb.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_lpb_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_mkrhs.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_multipolar_solutes.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_operators.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_pcm.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_solvers.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_workspace.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/llgnew.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/matrix_debug.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/pyddx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31313 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/pyddx_classes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/pyddx_data.cpp
```

### Comparing `pyddx-0.4.3/CMakeLists.txt` & `pyddx-0.4.4/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Restrict building in top-level directory
 if("${CMAKE_CURRENT_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_BINARY_DIR}")
     message(FATAL_ERROR "In-source builds are not allowed.\nPlease create a "
         "build directory first and execute cmake configuration from this "
         "directory. Example: mkdir build && cd build && cmake ..")
 endif()
 
-project(ddX VERSION 0.4.3 LANGUAGES Fortran CXX)
+project(ddX VERSION 0.4.4 LANGUAGES Fortran CXX)
 # If ddX is a subproject, append ddx_ prefix to all targets.
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
     set(ddx_is_subproject false)
     set(ddx_ "")
 else()
     set(ddx_is_subproject true)
     set(ddx_ "ddx_")
```

### Comparing `pyddx-0.4.3/LICENSE.txt` & `pyddx-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/PKG-INFO` & `pyddx-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.3
+Version: 0.4.4
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.3/README.md` & `pyddx-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/pyddx.egg-info/PKG-INFO` & `pyddx-0.4.4/pyddx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.3
+Version: 0.4.4
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.3/pyddx.egg-info/SOURCES.txt` & `pyddx-0.4.4/pyddx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/setup.py` & `pyddx-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyddx",
     description="ddx continuum solvation library",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
-    version="0.4.3",
+    version="0.4.4",
     #
     author="ddx developers",
     author_email="best@ians.uni-stuttgart.de",
     license="LGPL v3",
     url="https://ddsolvation.github.io/ddX",
     project_urls={
         "Source": "https://github.com/ddsolvation/ddX",
```

### Comparing `pyddx-0.4.3/src/CMakeLists.txt` & `pyddx-0.4.4/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/cbessel.f90` & `pyddx-0.4.4/src/cbessel.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx.f90` & `pyddx-0.4.4/src/ddx.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx.h` & `pyddx-0.4.4/src/ddx.h`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_cinterface.f90` & `pyddx-0.4.4/src/ddx_cinterface.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_constants.f90` & `pyddx-0.4.4/src/ddx_constants.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_core.f90` & `pyddx-0.4.4/src/ddx_core.f90`

 * *Files 2% similar despite different names*

```diff
@@ -709,159 +709,159 @@
     open(unit=100, file=fname, form='formatted', access='sequential')
     ! Printing flag
     read(100, *) output_filename
     ! Number of OpenMP threads to be used
     read(100, *) nproc
     if(nproc .lt. 0) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 2nd line of a config file ", fname, &
+            & "Error on the 2nd line of a config file ", trim(fname), &
             & ": `nproc` must be a positive integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Model to be used: 1 for COSMO, 2 for PCM and 3 for LPB
     read(100, *) model
     if((model .lt. 1) .or. (model .gt. 3)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 3rd line of a config file ", fname, &
+            & "Error on the 3rd line of a config file ", trim(fname), &
             & ": `model` must be an integer of a value 1, 2 or 3."
         ddx_data % error_flag = 1
         return
     end if
     ! Max degree of modeling spherical harmonics
     read(100, *) lmax
     if(lmax .lt. 0) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 4th line of a config file ", fname, &
+            & "Error on the 4th line of a config file ", trim(fname), &
             & ": `lmax` must be a non-negative integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Approximate number of Lebedev points
     read(100, *) ngrid
     if(ngrid .lt. 0) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 5th line of a config file ", fname, &
+            & "Error on the 5th line of a config file ", trim(fname), &
             & ": `ngrid` must be a non-negative integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Dielectric permittivity constant of the solvent
     read(100, *) eps
     if(eps .lt. zero) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 6th line of a config file ", fname, &
+            & "Error on the 6th line of a config file ", trim(fname), &
             & ": `eps` must be a non-negative floating point value."
         ddx_data % error_flag = 1
         return
     end if
     ! Shift of the regularized characteristic function
     read(100, *) se
     if((se .lt. -one) .or. (se .gt. one)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 7th line of a config file ", fname, &
+            & "Error on the 7th line of a config file ", trim(fname), &
             & ": `se` must be a floating point value in a range [-1, 1]."
         ddx_data % error_flag = 1
         return
     end if
     ! Regularization parameter
     read(100, *) eta
     if((eta .lt. zero) .or. (eta .gt. one)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 8th line of a config file ", fname, &
+            & "Error on the 8th line of a config file ", trim(fname), &
             & ": `eta` must be a floating point value in a range [0, 1]."
         ddx_data % error_flag = 1
         return
     end if
     ! Debye H\"{u}ckel parameter
     read(100, *) kappa
     if(kappa .lt. zero) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 9th line of a config file ", fname, &
+            & "Error on the 9th line of a config file ", trim(fname), &
             & ": `kappa` must be a non-negative floating point value."
         ddx_data % error_flag = 1
         return
     end if
     ! whether the (sparse) matrices are precomputed and kept in memory (1) or not (0).
     read(100, *) matvecmem 
     if((matvecmem.lt. 0) .or. (matvecmem .gt. 1)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 10th line of a config file ", fname, &
+            & "Error on the 10th line of a config file ", trim(fname), &
             & ": `matvecmem` must be an integer value of a value 0 or 1."
         ddx_data % error_flag = 1
         return
     end if
     ! Relative convergence threshold for the iterative solver
     read(100, *) tol
     if((tol .lt. 1d-14) .or. (tol .gt. one)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 12th line of a config file ", fname, &
+            & "Error on the 12th line of a config file ", trim(fname), &
             & ": `tol` must be a floating point value in a range [1d-14, 1]."
         ddx_data % error_flag = 1
         return
     end if
     ! Maximum number of iterations for the iterative solver
     read(100, *) maxiter
     if((maxiter .le. 0)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 13th line of a config file ", fname, &
+            & "Error on the 13th line of a config file ", trim(fname), &
             & ": `maxiter` must be a positive integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Number of extrapolation points for Jacobi/DIIS solver
     read(100, *) jacobi_ndiis
     if((jacobi_ndiis .lt. 0)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 14th line of a config file ", fname, &
+            & "Error on the 14th line of a config file ", trim(fname), &
             & ": `jacobi_ndiis` must be a non-negative integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Whether to compute (1) or not (0) forces as analytical gradients
     read(100, *) force
     if((force .lt. 0) .or. (force .gt. 1)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 17th line of a config file ", fname, &
+            & "Error on the 17th line of a config file ", trim(fname), &
             & ": `force` must be an integer value of a value 0 or 1."
         ddx_data % error_flag = 1
         return
     end if
     ! Whether to use (1) or not (0) the FMM to accelerate computations
     read(100, *) fmm
     if((fmm .lt. 0) .or. (fmm .gt. 1)) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 18th line of a config file ", fname, &
+            & "Error on the 18th line of a config file ", trim(fname), &
             & ": `fmm` must be an integer value of a value 0 or 1."
         ddx_data % error_flag = 1
         return
     end if
     ! Max degree of multipole spherical harmonics for the FMM
     read(100, *) pm
     if(pm .lt. 0) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 19th line of a config file ", fname, &
+            & "Error on the 19th line of a config file ", trim(fname), &
             & ": `pm` must be a non-negative integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Max degree of local spherical harmonics for the FMM
     read(100, *) pl
     if(pl .lt. 0) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 20th line of a config file ", fname, &
+            & "Error on the 20th line of a config file ", trim(fname), &
             & ": `pl` must be a non-negative integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Number of input spheres
     read(100, *) nsph
     if(nsph .le. 0) then
         write(ddx_data % error_message, "(3A)") &
-            & "Error on the 21th line of a config file ", fname, &
+            & "Error on the 21th line of a config file ", trim(fname), &
             & ": `nsph` must be a positive integer value."
         ddx_data % error_flag = 1
         return
     end if
     ! Coordinates, radii and charges
     allocate(charges(nsph), x(nsph), y(nsph), z(nsph), rvdw(nsph), stat=istatus)
     if(istatus .ne. 0) then
@@ -3021,15 +3021,15 @@
 !!
 !! @param[out] string: container for the logo
 !!
 subroutine get_banner(string)
     implicit none
     character (len=2047), intent(out) :: string
     character (len=10) :: vstr
-    write(vstr, *) "0.4.3"
+    write(vstr, *) "0.4.4"
     write(string, *) &
         & " +----------------------------------------------------------------+", &
         & NEW_LINE('a'), &
         & "  |                                                                |", &
         & NEW_LINE('a'), &
         & "  |                        888      888 Y8b    d8Y                 |", &
         & NEW_LINE('a'), &
```

### Comparing `pyddx-0.4.3/src/ddx_cosmo.f90` & `pyddx-0.4.4/src/ddx_cosmo.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_definitions.f90` & `pyddx-0.4.4/src/ddx_definitions.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_driver.f90` & `pyddx-0.4.4/src/ddx_driver.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_gradients.f90` & `pyddx-0.4.4/src/ddx_gradients.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_harmonics.f90` & `pyddx-0.4.4/src/ddx_harmonics.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_lpb.f90` & `pyddx-0.4.4/src/ddx_lpb.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_lpb_core.f90` & `pyddx-0.4.4/src/ddx_lpb_core.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_mkrhs.f90` & `pyddx-0.4.4/src/ddx_mkrhs.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_multipolar_solutes.f90` & `pyddx-0.4.4/src/ddx_multipolar_solutes.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_operators.f90` & `pyddx-0.4.4/src/ddx_operators.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_parameters.f90` & `pyddx-0.4.4/src/ddx_parameters.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_pcm.f90` & `pyddx-0.4.4/src/ddx_pcm.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/ddx_solvers.f90` & `pyddx-0.4.4/src/ddx_solvers.f90`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         ! y = rhs - O x
         call matvec(params, constants, workspace, x, workspace % tmp_y)
         workspace % tmp_y = rhs - workspace % tmp_y
         ! x_new = D^-1 y
         call dm1vec(params, constants, workspace, workspace % tmp_y, &
             & workspace % tmp_x_new)
         ! DIIS extrapolation
-        if (params % jacobi_ndiis .gt. 0) then
+        if (params % jacobi_ndiis .gt. 2) then
             workspace % tmp_x_diis(:, nmat) = workspace % tmp_x_new
             workspace % tmp_e_diis(:, nmat) = workspace % tmp_x_new - x
             call diis(constants % n, nmat, params % jacobi_ndiis, &
                 & workspace % tmp_x_diis, workspace % tmp_e_diis, &
                 & workspace % tmp_bmat, workspace % tmp_x_new)
         end if
         ! Norm of increment
@@ -155,15 +155,17 @@
     real(dp), dimension(ndiis+1,ndiis+1), intent(inout) :: b
     real(dp), dimension(n), intent(inout) :: xnew
     integer :: nmat1, i, istatus, info
     integer :: j, k
     real(dp), allocatable :: bloc(:,:), cex(:)
     integer,  allocatable :: ipiv(:)
     real(dp), parameter :: zero = 0.0d0, one = 1.0d0
-    integer,  parameter :: delta = 10
+    integer :: delta
+
+    delta = min(10, ndiis-1)
 
     if (nmat.ge.ndiis) then
         do j = 2, nmat - delta
             do k = 2, nmat - delta
                 b(j, k) = b(j+delta, k+delta)
             end do
         end do
```

### Comparing `pyddx-0.4.3/src/ddx_workspace.f90` & `pyddx-0.4.4/src/ddx_workspace.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/llgnew.f` & `pyddx-0.4.4/src/llgnew.f`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/matrix_debug.f90` & `pyddx-0.4.4/src/matrix_debug.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/pyddx.cpp` & `pyddx-0.4.4/src/pyddx.cpp`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/pyddx_classes.cpp` & `pyddx-0.4.4/src/pyddx_classes.cpp`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.3/src/pyddx_data.cpp` & `pyddx-0.4.4/src/pyddx_data.cpp`

 * *Files identical despite different names*

