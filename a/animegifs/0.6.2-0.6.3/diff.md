# Comparing `tmp/animegifs-0.6.2.tar.gz` & `tmp/animegifs-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.6.2.tar", last modified: Mon Jun  5 17:35:12 2023, max compression
+gzip compressed data, was "animegifs-0.6.3.tar", last modified: Tue Jun  6 22:57:06 2023, max compression
```

## Comparing `animegifs-0.6.2.tar` & `animegifs-0.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.933744 animegifs-0.6.2/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     3270 2023-06-05 17:35:12.933744 animegifs-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     2463 2023-06-05 17:30:38.000000 animegifs-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.913743 animegifs-0.6.2/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.2/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3388 2023-06-05 16:14:15.000000 animegifs-0.6.2/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.931744 animegifs-0.6.2/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.2/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     2319 2023-06-05 17:31:41.000000 animegifs-0.6.2/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     2010 2023-06-05 17:23:15.000000 animegifs-0.6.2/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:35:12.922743 animegifs-0.6.2/animegifs.egg-info/
--rw-rw-rw-   0        0        0     3270 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 17:35:12.000000 animegifs-0.6.2/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 17:35:12.934744 animegifs-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1282 2023-06-05 17:26:13.000000 animegifs-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.187573 animegifs-0.6.3/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0     3248 2023-06-06 22:57:06.186570 animegifs-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2464 2023-06-05 17:42:11.000000 animegifs-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.168570 animegifs-0.6.3/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.3/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3388 2023-06-05 16:14:15.000000 animegifs-0.6.3/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.184570 animegifs-0.6.3/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.3/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     2320 2023-06-06 22:10:28.000000 animegifs-0.6.3/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     2011 2023-06-06 22:09:58.000000 animegifs-0.6.3/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.179569 animegifs-0.6.3/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     3248 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 22:57:06.188571 animegifs-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2023-06-06 22:09:58.000000 animegifs-0.6.3/setup.py
```

### Comparing `animegifs-0.6.2/LICENSE` & `animegifs-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.2/PKG-INFO` & `animegifs-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.6.2
+Version: 0.6.3
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -117,13 +116,11 @@
 * Yawn
 
 **Special Category List**
 
 * Random
 * Steal-magic
 
-#Troubleshooting and other
+# Troubleshooting and other
 
 If you encounter an error raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues 
 or join the discord server to request new categories, new functions, feedback and even errors.
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.6.2 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.6.3 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
-anime,gif,python,anime-gif,discord Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # animegifs.py
+anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
 flawlessly or at all. Version below v0.6 will not have the gifs library updated
 anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
@@ -21,11 +21,11 @@
 gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page. ```
 **Category list:** * Attack * Bite * Bloodsuck * Blush * Bonk * Brofist * Cry *
 Cuddle * Dance * Disgust * Exploding * Facedesk * Facepalm * Flick * Flirt *
 Handhold * Happy * Harass * Highfive * Hug * Icecream * Insult * Kill * Kiss *
 Lick * Love * Marry * Nod * Nosebleed * Nuzzle * Pat * Peck * Poke * Popcorn *
 Pout * Punch * Punish * Run * Sad * Scared * Shoot * Shrug * Sip * Slap * Smirk
 * Sorry * Spank * Stare * Tease * Threat * Tickle * Tired * Wave * Yawn
-**Special Category List** * Random * Steal-magic #Troubleshooting and other If
+**Special Category List** * Random * Steal-magic # Troubleshooting and other If
 you encounter an error raise an issue on the issue page: https://github.com/
 MarcoSa-2000/animegifs/issues or join the discord server to request new
 categories, new functions, feedback and even errors.
```

### Comparing `animegifs-0.6.2/README.md` & `animegifs-0.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -96,11 +96,11 @@
 * Yawn
 
 **Special Category List**
 
 * Random
 * Steal-magic
 
-#Troubleshooting and other
+# Troubleshooting and other
 
 If you encounter an error raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues 
 or join the discord server to request new categories, new functions, feedback and even errors.
```

#### html2text {}

```diff
@@ -13,11 +13,11 @@
 gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page. ```
 **Category list:** * Attack * Bite * Bloodsuck * Blush * Bonk * Brofist * Cry *
 Cuddle * Dance * Disgust * Exploding * Facedesk * Facepalm * Flick * Flirt *
 Handhold * Happy * Harass * Highfive * Hug * Icecream * Insult * Kill * Kiss *
 Lick * Love * Marry * Nod * Nosebleed * Nuzzle * Pat * Peck * Poke * Popcorn *
 Pout * Punch * Punish * Run * Sad * Scared * Shoot * Shrug * Sip * Slap * Smirk
 * Sorry * Spank * Stare * Tease * Threat * Tickle * Tired * Wave * Yawn
-**Special Category List** * Random * Steal-magic #Troubleshooting and other If
+**Special Category List** * Random * Steal-magic # Troubleshooting and other If
 you encounter an error raise an issue on the issue page: https://github.com/
 MarcoSa-2000/animegifs/issues or join the discord server to request new
 categories, new functions, feedback and even errors.
```

### Comparing `animegifs-0.6.2/animegifs/animegifs.py` & `animegifs-0.6.3/animegifs/animegifs.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.2/animegifs/distutils/errors.py` & `animegifs-0.6.3/animegifs/distutils/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.exc = exc
         self.error = error
         super().__init__(self.error)
 
 class AuthError(Exception):
     """
     Authentication request returned an error. Probably status error 4xx.
-    It will be resolved soon, if it persist,
+    It will be resolved soon, if it persists,
     issue an issue on https://github.com/MarcoSa-2000/animegifs/issues.
     """
 
     def __init__(self, exc, error="Authentication request returned an error."):
         self.exc = exc
         self.error = error
         super().__init__(self.error)
```

### Comparing `animegifs-0.6.2/animegifs/distutils/gifs.py` & `animegifs-0.6.3/animegifs/distutils/gifs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
                   'sad', 'scared', 'shoot', 'shrug', 'sip', 'slap', 'smirk', 'sorry', 'spank', 'stare',
                   'tease', 'threat', 'tickle', 'tired',
                   'wave',
                   'yawn']
 
 def authentication():
     try:
-        response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1", timeout=10)
+        response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1", timeout=100)
     except requests.exceptions.Timeout:
         try:
-            response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1", timeout=25)
+            response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key2", timeout=25)
         except requests.exceptions.Timeout as exc:
             raise errors.AuthTimeout(exc)
     if response.status_code == 200:
         auth_key = response.json()['key']
     else:
         exc = response.status_code
         raise errors.AuthError(exc)
```

### Comparing `animegifs-0.6.2/animegifs.egg-info/PKG-INFO` & `animegifs-0.6.3/animegifs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.6.2
+Version: 0.6.3
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -117,13 +116,11 @@
 * Yawn
 
 **Special Category List**
 
 * Random
 * Steal-magic
 
-#Troubleshooting and other
+# Troubleshooting and other
 
 If you encounter an error raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues 
 or join the discord server to request new categories, new functions, feedback and even errors.
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.6.2 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.6.3 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
-anime,gif,python,anime-gif,discord Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # animegifs.py
+anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
 flawlessly or at all. Version below v0.6 will not have the gifs library updated
 anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
@@ -21,11 +21,11 @@
 gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page. ```
 **Category list:** * Attack * Bite * Bloodsuck * Blush * Bonk * Brofist * Cry *
 Cuddle * Dance * Disgust * Exploding * Facedesk * Facepalm * Flick * Flirt *
 Handhold * Happy * Harass * Highfive * Hug * Icecream * Insult * Kill * Kiss *
 Lick * Love * Marry * Nod * Nosebleed * Nuzzle * Pat * Peck * Poke * Popcorn *
 Pout * Punch * Punish * Run * Sad * Scared * Shoot * Shrug * Sip * Slap * Smirk
 * Sorry * Spank * Stare * Tease * Threat * Tickle * Tired * Wave * Yawn
-**Special Category List** * Random * Steal-magic #Troubleshooting and other If
+**Special Category List** * Random * Steal-magic # Troubleshooting and other If
 you encounter an error raise an issue on the issue page: https://github.com/
 MarcoSa-2000/animegifs/issues or join the discord server to request new
 categories, new functions, feedback and even errors.
```

### Comparing `animegifs-0.6.2/setup.py` & `animegifs-0.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.6.2'
+VERSION = '0.6.3'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Marco-Sa2000',
     author_email='grest0grest@gmail.com',
     license='MIT',
     url="https://github.com/MarcoSa-2000/animegifs",
     install_requires=[
-       'requests==2.28.2,<=2.29.0',
+       'requests>=2.28.2,<=2.29.0',
        'mal-api==0.5.3',
        'PyJWT>=2.4.0,<=2.7.0'
     ],
     python_requires='>=3.8',
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

