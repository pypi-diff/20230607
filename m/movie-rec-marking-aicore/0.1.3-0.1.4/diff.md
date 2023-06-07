# Comparing `tmp/movie-rec-marking-aicore-0.1.3.tar.gz` & `tmp/movie-rec-marking-aicore-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-rec-marking-aicore-0.1.3.tar", last modified: Tue Apr 11 08:31:43 2023, max compression
+gzip compressed data, was "movie-rec-marking-aicore-0.1.4.tar", last modified: Wed Jun  7 11:45:32 2023, max compression
```

## Comparing `movie-rec-marking-aicore-0.1.3.tar` & `movie-rec-marking-aicore-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tianwenwangye   (501) staff       (20)        0 2023-04-11 08:31:43.546223 movie-rec-marking-aicore-0.1.3/
--rw-r--r--   0 tianwenwangye   (501) staff       (20)      216 2023-04-11 08:31:43.544014 movie-rec-marking-aicore-0.1.3/PKG-INFO
-drwxr-xr-x   0 tianwenwangye   (501) staff       (20)        0 2023-04-11 08:31:43.535237 movie-rec-marking-aicore-0.1.3/movie_rec_marking/
--rw-r--r--   0 tianwenwangye   (501) staff       (20)        0 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/__init__.py
--rw-r--r--   0 tianwenwangye   (501) staff       (20)     2099 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_1.py
--rw-r--r--   0 tianwenwangye   (501) staff       (20)     7331 2023-04-11 08:18:46.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_2.py
--rw-r--r--   0 tianwenwangye   (501) staff       (20)     5308 2023-04-11 08:31:37.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_3.py
--rw-r--r--   0 tianwenwangye   (501) staff       (20)     6242 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_4.py
--rw-r--r--   0 tianwenwangye   (501) staff       (20)     9059 2023-03-17 16:01:21.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_5.py
-drwxr-xr-x   0 tianwenwangye   (501) staff       (20)        0 2023-04-11 08:31:43.542802 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/
--rw-r--r--   0 tianwenwangye   (501) staff       (20)      216 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/PKG-INFO
--rw-r--r--   0 tianwenwangye   (501) staff       (20)      467 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/SOURCES.txt
--rw-r--r--   0 tianwenwangye   (501) staff       (20)        1 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/dependency_links.txt
--rw-r--r--   0 tianwenwangye   (501) staff       (20)       26 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/requires.txt
--rw-r--r--   0 tianwenwangye   (501) staff       (20)       18 2023-04-11 08:31:43.000000 movie-rec-marking-aicore-0.1.3/movie_rec_marking_aicore.egg-info/top_level.txt
--rw-r--r--   0 tianwenwangye   (501) staff       (20)       38 2023-04-11 08:31:43.546377 movie-rec-marking-aicore-0.1.3/setup.cfg
--rw-r--r--   0 tianwenwangye   (501) staff       (20)      390 2023-04-11 08:20:09.000000 movie-rec-marking-aicore-0.1.3/setup.py
+drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-07 11:45:32.222988 movie-rec-marking-aicore-0.1.4/
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      216 2023-06-07 11:45:32.222988 movie-rec-marking-aicore-0.1.4/PKG-INFO
+drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-07 11:45:32.222988 movie-rec-marking-aicore-0.1.4/movie_rec_marking/
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking/__init__.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     2099 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_1.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     7646 2023-06-07 11:44:47.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_2.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     5308 2023-05-12 11:04:27.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_3.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     6242 2023-03-30 14:28:25.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_4.py
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)     9059 2023-02-09 15:42:55.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_5.py
+drwxrwxr-x   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        0 2023-06-07 11:45:32.222988 movie-rec-marking-aicore-0.1.4/movie_rec_marking_aicore.egg-info/
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      216 2023-06-07 11:45:31.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking_aicore.egg-info/PKG-INFO
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      467 2023-06-07 11:45:31.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking_aicore.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)        1 2023-06-07 11:45:31.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking_aicore.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       26 2023-06-07 11:45:31.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking_aicore.egg-info/requires.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       18 2023-06-07 11:45:31.000000 movie-rec-marking-aicore-0.1.4/movie_rec_marking_aicore.egg-info/top_level.txt
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)       38 2023-06-07 11:45:32.222988 movie-rec-marking-aicore-0.1.4/setup.cfg
+-rw-rw-r--   0 ivanyingxuan  (1001) ivanyingxuan  (1001)      390 2023-06-07 11:45:21.000000 movie-rec-marking-aicore-0.1.4/setup.py
```

### Comparing `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_1.py` & `movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_1.py`

 * *Files identical despite different names*

### Comparing `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_2.py` & `movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,18 +64,23 @@
 
 def check_get_movie_description_length(func, task_1):
     # Check that the function returns the correct length of the description\
     if not task_1:
         print("You haven't completed the previous task correctly")
         return False
     movie = movies[1]
+    print("testing  the function with movie: ", movie["title"])
+   
+    print("Testing that the function can accept a movie as an argument, and that it returns the correct length of the description as an integer type")
     try:
         actual = func(movie)
+        
     except Exception as e:
-        print("Running the function with a movie as an argument results in an error")
+        
+        print("Attempting to pass a movie dictionary to the function as an argument resulted in an error. Your function should accept a dictionary as an argument")
         print('Check the error here: ', e)
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
     if not actual:
         print("The function doesn't return anything")
         print('Please, try again, and don\'t continue until you get the correct output')
         return False
```

### Comparing `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_3.py` & `movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_3.py`

 * *Files identical despite different names*

### Comparing `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_4.py` & `movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_4.py`

 * *Files identical despite different names*

### Comparing `movie-rec-marking-aicore-0.1.3/movie_rec_marking/test_milestone_5.py` & `movie-rec-marking-aicore-0.1.4/movie_rec_marking/test_milestone_5.py`

 * *Files identical despite different names*

