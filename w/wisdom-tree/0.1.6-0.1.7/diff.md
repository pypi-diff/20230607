# Comparing `tmp/wisdom-tree-0.1.6.tar.gz` & `tmp/wisdom-tree-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisdom-tree-0.1.6.tar", last modified: Tue Jun  6 17:40:20 2023, max compression
+gzip compressed data, was "wisdom-tree-0.1.7.tar", last modified: Wed Jun  7 16:14:44 2023, max compression
```

## Comparing `wisdom-tree-0.1.6.tar` & `wisdom-tree-0.1.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:40:20.695158 wisdom-tree-0.1.6/
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)     1066 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/LICENSE
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)      117 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/MANIFEST.in
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4933 2023-06-06 17:40:20.695158 wisdom-tree-0.1.6/PKG-INFO
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4008 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/README.md
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       38 2023-06-06 17:40:20.695158 wisdom-tree-0.1.6/setup.cfg
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)     8553 2023-06-06 17:38:56.000000 wisdom-tree-0.1.6/setup.py
-drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:40:20.395156 wisdom-tree-0.1.6/wisdom_tree/
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       44 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/__init__.py
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4211 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/edit_quotes.py
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)    33079 2023-06-06 17:38:19.000000 wisdom-tree-0.1.6/wisdom_tree/main.py
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)   302977 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/qts.txt
-drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:40:20.688491 wisdom-tree-0.1.6/wisdom_tree/res/
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)  1325622 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/alarm.wav
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)   738851 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/forest.ogg
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)   828761 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/forest2.ogg
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)  1116740 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/growth.waw
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)    84480 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/logo_512x512.png
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)        4 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p1.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)        7 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p2.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)        8 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p3.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       15 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p4.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       26 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p5.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       46 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p6.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)      102 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p7.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)      205 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p8.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)      244 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/p9.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)   924377 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/rain.ogg
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)      865 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/rain1.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)        4 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/seed.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)   493892 2023-06-06 15:22:14.000000 wisdom-tree-0.1.6/wisdom_tree/res/timerstart.wav
-drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-06 17:40:20.435156 wisdom-tree-0.1.6/wisdom_tree.egg-info/
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4933 2023-06-06 17:40:19.000000 wisdom-tree-0.1.6/wisdom_tree.egg-info/PKG-INFO
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)      796 2023-06-06 17:40:19.000000 wisdom-tree-0.1.6/wisdom_tree.egg-info/SOURCES.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)        1 2023-06-06 17:40:19.000000 wisdom-tree-0.1.6/wisdom_tree.egg-info/dependency_links.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       52 2023-06-06 17:40:19.000000 wisdom-tree-0.1.6/wisdom_tree.egg-info/entry_points.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       18 2023-06-06 17:40:19.000000 wisdom-tree-0.1.6/wisdom_tree.egg-info/requires.txt
--rw-r--r--   0 hacker097  (1000) hacker097  (1000)       12 2023-06-06 17:40:19.000000 wisdom-tree-0.1.6/wisdom_tree.egg-info/top_level.txt
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-07 16:14:44.560880 wisdom-tree-0.1.7/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     1066 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/LICENSE
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      117 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/MANIFEST.in
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4933 2023-06-07 16:14:44.560880 wisdom-tree-0.1.7/PKG-INFO
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4008 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/README.md
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       38 2023-06-07 16:14:44.560880 wisdom-tree-0.1.7/setup.cfg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     8553 2023-06-07 16:14:11.000000 wisdom-tree-0.1.7/setup.py
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-07 16:14:44.430878 wisdom-tree-0.1.7/wisdom_tree/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       44 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/__init__.py
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4211 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/edit_quotes.py
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)    33174 2023-06-07 15:45:41.000000 wisdom-tree-0.1.7/wisdom_tree/main.py
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   302977 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/qts.txt
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-07 16:14:44.557547 wisdom-tree-0.1.7/wisdom_tree/res/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)  1325622 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/alarm.wav
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   738851 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/forest.ogg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   828761 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/forest2.ogg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)  1116740 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/growth.waw
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)    84480 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/logo_512x512.png
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        4 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p1.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        7 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p2.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        8 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p3.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       15 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p4.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       26 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p5.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       46 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p6.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      102 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p7.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      205 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p8.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      244 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/p9.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   924377 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/rain.ogg
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      865 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/rain1.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        4 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/seed.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)   493892 2023-06-06 15:22:14.000000 wisdom-tree-0.1.7/wisdom_tree/res/timerstart.wav
+drwxr-xr-x   0 hacker097  (1000) hacker097  (1000)        0 2023-06-07 16:14:44.430878 wisdom-tree-0.1.7/wisdom_tree.egg-info/
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)     4933 2023-06-07 16:14:43.000000 wisdom-tree-0.1.7/wisdom_tree.egg-info/PKG-INFO
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)      796 2023-06-07 16:14:43.000000 wisdom-tree-0.1.7/wisdom_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)        1 2023-06-07 16:14:43.000000 wisdom-tree-0.1.7/wisdom_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       52 2023-06-07 16:14:43.000000 wisdom-tree-0.1.7/wisdom_tree.egg-info/entry_points.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       18 2023-06-07 16:14:43.000000 wisdom-tree-0.1.7/wisdom_tree.egg-info/requires.txt
+-rw-r--r--   0 hacker097  (1000) hacker097  (1000)       12 2023-06-07 16:14:43.000000 wisdom-tree-0.1.7/wisdom_tree.egg-info/top_level.txt
```

### Comparing `wisdom-tree-0.1.6/LICENSE` & `wisdom-tree-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/PKG-INFO` & `wisdom-tree-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisdom-tree
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tui concentration app
 Home-page: https://github.com/HACKER097/wisdom-tree
 Author: HACKER097
 Project-URL: Bug Reports, https://github.com/HACKER097/wisdom-tree/issues
 Project-URL: Source, https://github.com/HACKER097/wisdom-tree/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wisdom-tree-0.1.6/README.md` & `wisdom-tree-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/setup.py` & `wisdom-tree-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PE 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.6',  # Required
+    version='0.1.7',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A tui concentration app',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `wisdom-tree-0.1.6/wisdom_tree/edit_quotes.py` & `wisdom-tree-0.1.7/wisdom_tree/edit_quotes.py`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/main.py` & `wisdom-tree-0.1.7/wisdom_tree/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,33 +233,33 @@
 
     if key == ord(" "):
         if tree1.media.is_playing():
             tree1.media.pause()
         tree1.pause = True
         tree1.pausetime = time.time()
 
-        if key == ord("m"):
-            tree1.media.pause()
+    if key == ord("m"):
+        tree1.media.pause()
 
     if not tree1.isloading and key == ord("n"):
         tree1.lofiradio()
 
     if key == ord("]"):
-        new_volume = tree1.media.audio_get_volume()+1
+        new_volume = min(tree1.media.audio_get_volume()+1, 100)
         
         tree1.media.audio_set_volume(min(100, new_volume))
         tree1.notifyendtime = int(time.time()) + 2
         volumeStr = str(round(new_volume)) + "%"
 
         tree1.notifystring = " "*round(maxx*(new_volume/100)-len(volumeStr)-2) + volumeStr
         tree1.invert = True
         tree1.isnotify = True
 
     if key == ord("["):
-        new_volume = tree1.media.audio_get_volume()-1
+        new_volume = max(tree1.media.audio_get_volume()-1, 0)
         
         tree1.media.audio_set_volume(min(100, new_volume))
         tree1.notifyendtime = int(time.time()) + 2
         volumeStr = str(round(new_volume)) + "%"
 
         tree1.notifystring = " "*round(maxx*(new_volume/100)-len(volumeStr)-2) + volumeStr
         tree1.invert = True
@@ -410,17 +410,15 @@
         self.playlist = Playlist("https://www.youtube.com/playlist?list=PL6fhs6TSspZvN45CPJApnMYVsWhkt55h7")
         self.radiomode = False
         self.isloading = False
         self.invert = False
         self.breakendtext = "BREAK IS OVER, PRESS ENTER TO START NEW TIMER"
         self.isloop = False
 
-
-
-    def display(self, maxx, maxy, seconds):
+    def setartfile(self):
         if self.age >= 1 and self.age < 5:
             self.artfile = str(RES_FOLDER/"p1.txt")
         if self.age >= 5 and self.age < 10:
             self.artfile = str(RES_FOLDER/"p2.txt")
         if self.age >= 10 and self.age < 20:
             self.artfile = str(RES_FOLDER/"p3.txt")
         if self.age >= 20 and self.age < 30:
@@ -432,14 +430,16 @@
         if self.age >= 70 and self.age < 120:
             self.artfile = str(RES_FOLDER/"p7.txt")
         if self.age >= 120 and self.age < 200:
             self.artfile = str(RES_FOLDER/"p8.txt")
         if self.age >= 200:
             self.artfile = str(RES_FOLDER/"p9.txt")
 
+    def display(self, maxx, maxy, seconds):
+
         printart(self.stdscr, self.artfile, int(maxx / 2), int(maxy * 3 / 4), 1)
         addtext(
             int(maxx / 2),
             int(maxy * 3 / 4),
             "age: " + str(int(self.age)) + " ",
             -1,
             self.stdscr,
@@ -839,15 +839,14 @@
     stdscr = curses.initscr()
     stdscr.nodelay(True)
     stdscr.keypad(True)
     curses.curs_set(0)
     curses.start_color()
     curses.noecho()
     curses.cbreak()
-
     curses.use_default_colors()
 
     try:
 
         curses.init_pair(1, 113, -1)  # passive selected text inner, outer
         curses.init_pair(2, 85, -1)  # timer color inner, outer
         curses.init_pair(3, 3, -1)  # active selected inner, outer
@@ -884,14 +883,15 @@
         treedata_in = open(RES_FOLDER/ "treedata", "rb")
         tree1.age = pickle.load(treedata_in)
 
     except:
 
         tree1.age = 1
 
+    tree1.setartfile()
 
     try:
         while run:
 
             start = time.time()
 
             try:
@@ -904,15 +904,15 @@
                     anilen = 150
                     
                 if (seconds % (100 * 60 * 10) == 0):  # show another quote every 5 min, and grow tree
                     quote = getqt()
                     tree1.age += 1
                     anilen = 1
                     play_sound(GROWTH_SOUND)
-
+                    tree1.setartfile()
       
                 tree1.display(maxx, maxy, seconds)
 
                 tree1.seasons(maxx, maxy, seconds)
 
                 tree1.menudisplay(stdscr, maxy, maxx)
```

### Comparing `wisdom-tree-0.1.6/wisdom_tree/qts.txt` & `wisdom-tree-0.1.7/wisdom_tree/qts.txt`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/res/alarm.wav` & `wisdom-tree-0.1.7/wisdom_tree/res/alarm.wav`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/res/forest.ogg` & `wisdom-tree-0.1.7/wisdom_tree/res/forest.ogg`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/res/forest2.ogg` & `wisdom-tree-0.1.7/wisdom_tree/res/forest2.ogg`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/res/growth.waw` & `wisdom-tree-0.1.7/wisdom_tree/res/growth.waw`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/res/logo_512x512.png` & `wisdom-tree-0.1.7/wisdom_tree/res/logo_512x512.png`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/res/rain.ogg` & `wisdom-tree-0.1.7/wisdom_tree/res/rain.ogg`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree/res/timerstart.wav` & `wisdom-tree-0.1.7/wisdom_tree/res/timerstart.wav`

 * *Files identical despite different names*

### Comparing `wisdom-tree-0.1.6/wisdom_tree.egg-info/PKG-INFO` & `wisdom-tree-0.1.7/wisdom_tree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisdom-tree
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tui concentration app
 Home-page: https://github.com/HACKER097/wisdom-tree
 Author: HACKER097
 Project-URL: Bug Reports, https://github.com/HACKER097/wisdom-tree/issues
 Project-URL: Source, https://github.com/HACKER097/wisdom-tree/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wisdom-tree-0.1.6/wisdom_tree.egg-info/SOURCES.txt` & `wisdom-tree-0.1.7/wisdom_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

