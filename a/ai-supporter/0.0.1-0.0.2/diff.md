# Comparing `tmp/ai-supporter-0.0.1.tar.gz` & `tmp/ai-supporter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-supporter-0.0.1.tar", last modified: Thu Mar 16 12:41:42 2023, max compression
+gzip compressed data, was "ai-supporter-0.0.2.tar", last modified: Wed Jun  7 03:15:14 2023, max compression
```

## Comparing `ai-supporter-0.0.1.tar` & `ai-supporter-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 12:41:42.847690 ai-supporter-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      356 2023-03-16 12:41:42.847690 ai-supporter-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       92 2023-03-16 12:41:41.000000 ai-supporter-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 12:41:42.845690 ai-supporter-0.0.1/ai_supporter/
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-16 12:41:41.000000 ai-supporter-0.0.1/ai_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-03-16 12:41:41.000000 ai-supporter-0.0.1/ai_supporter/tts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 12:41:42.847690 ai-supporter-0.0.1/ai_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      356 2023-03-16 12:41:42.000000 ai-supporter-0.0.1/ai_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2023-03-16 12:41:42.000000 ai-supporter-0.0.1/ai_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 12:41:42.000000 ai-supporter-0.0.1/ai_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 12:41:42.000000 ai-supporter-0.0.1/ai_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-16 12:41:42.000000 ai-supporter-0.0.1/ai_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-16 12:41:42.000000 ai-supporter-0.0.1/ai_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-16 12:41:42.847690 ai-supporter-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-16 12:41:41.000000 ai-supporter-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 03:15:14.170587 ai-supporter-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-07 03:15:14.170587 ai-supporter-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       92 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 03:15:14.169587 ai-supporter-0.0.2/ai_supporter/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter/tts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 03:15:14.170587 ai-supporter-0.0.2/ai_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-07 03:15:14.000000 ai-supporter-0.0.2/ai_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 03:15:14.171587 ai-supporter-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/setup.py
```

### Comparing `ai-supporter-0.0.1/ai_supporter/tts.py` & `ai-supporter-0.0.2/ai_supporter/tts.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 #https://levelup.gitconnected.com/make-your-python-program-speak-310766534fbf
 def speak(text):
     thread = threading.Thread(target=run, args=[text])
     thread.daemon = True
     thread.start()
 
 def run(text):
-    tts = gTTS(text=text, lang='ko', slow=False)
-    file = f"speak_{random.random()}.mp3"
-    tts.save(file)     
-    print(dir(tts))
- 
-    pygame.mixer.init()
-    pygame.mixer.music.load(file)
-    pygame.mixer.music.play()
-    
-    while pygame.mixer.music.get_busy():
-        time.sleep(0.01)
-    
-    pygame.quit()
-    os.remove(file)    
+    try:
+        tts = gTTS(text=text, lang='ko', slow=False)
+        file = f"speak_{random.random()}.mp3"
+        tts.save(file)     
+        #print(dir(tts))
+
+        pygame.mixer.init()
+        pygame.mixer.music.load(file)
+        pygame.mixer.music.play()
+
+        while pygame.mixer.music.get_busy():
+            time.sleep(0.01)
+    finally:
+        pygame.quit()
+        os.remove(file)
```

### Comparing `ai-supporter-0.0.1/setup.py` & `ai-supporter-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='ai-supporter',
-	version='0.0.1',
+	version='0.0.2',
 	description='Ai supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/ai-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

