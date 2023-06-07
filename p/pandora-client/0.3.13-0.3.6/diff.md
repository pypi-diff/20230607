# Comparing `tmp/pandora_client-0.3.13.tar.gz` & `tmp/pandora_client-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandora_client-0.3.13.tar", last modified: Wed Jun  7 14:22:03 2023, max compression
+gzip compressed data, was "dist/pandora_client-0.3.6.tar", last modified: Sat Dec 21 17:34:56 2019, max compression
```

## Comparing `pandora_client-0.3.13.tar` & `pandora_client-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-06-07 14:22:03.297333 pandora_client-0.3.13/
--rw-r--r--   0 j         (1000) j         (1000)      603 2023-06-07 14:22:03.297333 pandora_client-0.3.13/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     2012 2019-12-21 18:34:41.000000 pandora_client-0.3.13/README.md
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-06-07 14:22:03.293333 pandora_client-0.3.13/bin/
--rwxr-xr-x   0 j         (1000) j         (1000)     2861 2020-05-30 01:46:42.000000 pandora_client-0.3.13/bin/pandora_client
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-06-07 14:22:03.297333 pandora_client-0.3.13/pandora_client/
--rwxr-xr-x   0 j         (1000) j         (1000)    45307 2021-09-16 16:42:38.000000 pandora_client-0.3.13/pandora_client/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     4427 2021-03-22 11:26:42.000000 pandora_client-0.3.13/pandora_client/client.py
--rw-r--r--   0 j         (1000) j         (1000)    10628 2023-06-07 14:18:12.000000 pandora_client-0.3.13/pandora_client/extract.py
--rw-r--r--   0 j         (1000) j         (1000)     3688 2017-07-01 14:49:54.000000 pandora_client-0.3.13/pandora_client/localnode.py
--rw-r--r--   0 j         (1000) j         (1000)     8480 2018-02-28 16:12:50.000000 pandora_client-0.3.13/pandora_client/server.py
--rw-r--r--   0 j         (1000) j         (1000)     3096 2017-06-01 07:59:42.000000 pandora_client-0.3.13/pandora_client/utils.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2023-06-07 14:22:03.297333 pandora_client-0.3.13/pandora_client.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      603 2023-06-07 14:22:03.000000 pandora_client-0.3.13/pandora_client.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      414 2023-06-07 14:22:03.000000 pandora_client-0.3.13/pandora_client.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2023-06-07 14:22:03.000000 pandora_client-0.3.13/pandora_client.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       47 2015-09-29 13:38:05.000000 pandora_client-0.3.13/pandora_client.egg-info/pbr.json
--rw-rw-r--   0 j         (1000) j         (1000)       54 2023-06-07 14:22:03.000000 pandora_client-0.3.13/pandora_client.egg-info/requires.txt
--rw-rw-r--   0 j         (1000) j         (1000)       15 2023-06-07 14:22:03.000000 pandora_client-0.3.13/pandora_client.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) j         (1000)       38 2023-06-07 14:22:03.297333 pandora_client-0.3.13/setup.cfg
--rw-r--r--   0 j         (1000) j         (1000)     1724 2023-06-07 14:22:02.000000 pandora_client-0.3.13/setup.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/
+-rw-r--r--   0 j         (1000) j         (1000)      633 2019-12-21 17:34:56.000000 pandora_client-0.3.6/PKG-INFO
+-rw-r--r--   0 j         (1000) j         (1000)     1494 2018-04-03 08:27:32.000000 pandora_client-0.3.6/README.md
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/bin/
+-rwxr-xr-x   0 j         (1000) j         (1000)     2854 2017-06-07 07:20:35.000000 pandora_client-0.3.6/bin/pandora_client
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client/
+-rwxr-xr-x   0 j         (1000) j         (1000)    45873 2019-12-19 11:15:56.000000 pandora_client-0.3.6/pandora_client/__init__.py
+-rw-r--r--   0 j         (1000) j         (1000)     4342 2018-06-06 07:58:05.000000 pandora_client-0.3.6/pandora_client/client.py
+-rw-r--r--   0 j         (1000) j         (1000)    10633 2019-11-01 20:50:01.000000 pandora_client-0.3.6/pandora_client/extract.py
+-rw-r--r--   0 j         (1000) j         (1000)     3688 2017-07-01 14:49:54.000000 pandora_client-0.3.6/pandora_client/localnode.py
+-rw-r--r--   0 j         (1000) j         (1000)     8480 2018-02-28 16:12:50.000000 pandora_client-0.3.6/pandora_client/server.py
+-rw-r--r--   0 j         (1000) j         (1000)     3096 2017-06-01 07:59:42.000000 pandora_client-0.3.6/pandora_client/utils.py
+drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      633 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      414 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/dependency_links.txt
+-rw-r--r--   0 j         (1000) j         (1000)       47 2015-09-29 13:38:05.000000 pandora_client-0.3.6/pandora_client.egg-info/pbr.json
+-rw-rw-r--   0 j         (1000) j         (1000)       54 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/requires.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       15 2019-12-21 17:34:56.000000 pandora_client-0.3.6/pandora_client.egg-info/top_level.txt
+-rw-r--r--   0 j         (1000) j         (1000)       38 2019-12-21 17:34:56.000000 pandora_client-0.3.6/setup.cfg
+-rw-r--r--   0 j         (1000) j         (1000)     1715 2019-12-21 17:34:56.000000 pandora_client-0.3.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pandora_client-0.3.13/README.md` & `pandora_client-0.3.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,9 @@
 # pandora_client - python client and libary to access a pan.do/ra instances
 
-Documentation at: https://code.0x2620.org/0x2620/pandora_client/wiki
-
-## Installation
-
-### Linux
-
-- install dependencies
-
-        sudo apt install python3 python3-pip ffmpeg
-
-- install pandora_client
-
-        sudo pip3 install pandora_client
-
-
-### macOS
-
-- install brew (https://brew.sh/)
-- install dependencies
-
-        brew install python3
-        brew install libvpx libvorbis
-        brew install ffmpeg --with-libvpx --with-libvorbis --with-libopus
-
-- install pandora_client
-
-        pip3 install pandora_client
-
 
 ## pandora client example:
 
   import pandora_client
   #example config.json
   '''
   {
```

### Comparing `pandora_client-0.3.13/bin/pandora_client` & `pandora_client-0.3.6/bin/pandora_client`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     config = ('config', 'add_volume')
     server = ('server', 'client')
     if not args or args[0] not in actions + config + server:
         parser.error('''you must specify a valid action.
 \t\tknown actions are: %s
 \t\tconfiguration:     config, add_volume
 \t\tdistributed encoding: server, client
-for more information visit https://code.0x2620.org/0x2620/pandora_client/wiki''' % ', '.join(actions))
+for more information visit https://wiki.0x2620.org/wiki/pandora_client''' % ', '.join(actions))
 
     action = args[0]
 
     offline = action in config or action == 'client' or \
         (action == 'extract' and len(args) == 2 and args[1] in ('offline', 'all'))
     if action == 'client':
         opts.config = {'url': '', 'cache': '~/.ox/client.sqlite', 'media-cache': '~/.ox/media'}
```

### Comparing `pandora_client-0.3.13/pandora_client/__init__.py` & `pandora_client-0.3.6/pandora_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # vi:si:et:sw=4:sts=4:ts=4
 # GPL 2012-2016
 from __future__ import division, with_statement, print_function, absolute_import
 
 import getpass
 from glob import glob
-import importlib.util
+import imp
 import json
 import math
 import os
 import socket
 import sqlite3
 import sys
 import tempfile
@@ -222,36 +222,27 @@
                 c.execute(i)
             conn.commit()
         conn.close()
 
     def load_plugins(self, base=os.path.join(utils.basedir(), 'client.d')):
         global parse_path, example_path, ignore_file, sync_extensions, encode
         base = os.path.expanduser(base)
-        if not os.path.exists(base):
-            return
-        for name in sorted(os.listdir(base)):
-            if not name.endswith('.py'):
-                continue
-            path = os.path.join(base, name)
-
-            module_name = os.path.basename(path).split('.')[0]
-            spec = importlib.util.spec_from_file_location(module_name, path)
-            module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(module)
-
-            if hasattr(module, 'parse_path'):
-                parse_path = module.parse_path
-            if hasattr(module, 'example_path'):
-                example_path = module.example_path
-            if hasattr(module, 'ignore_file'):
-                ignore_file = module.ignore_file
-            if hasattr(module, 'sync_extensions'):
-                sync_extensions = module.sync_extensions
-            if hasattr(module, 'encode'):
-                encode = module.encode
+        for path in sorted(glob('%s%s*.py' % (base, os.sep))):
+            with open(path) as fp:
+                module = imp.load_source(os.path.basename(path).split('.')[0], base, fp)
+                if hasattr(module, 'parse_path'):
+                    parse_path = module.parse_path
+                if hasattr(module, 'example_path'):
+                    example_path = module.example_path
+                if hasattr(module, 'ignore_file'):
+                    ignore_file = module.ignore_file
+                if hasattr(module, 'sync_extensions'):
+                    sync_extensions = module.sync_extensions
+                if hasattr(module, 'encode'):
+                    encode = module.encode
 
     def _conn(self):
         db_conn = self._config['cache']
         if isinstance(db_conn, bytes):
             db_conn = db_conn.decode('utf-8')
         db_conn = os.path.expanduser(db_conn)
         if not os.path.exists(os.path.dirname(db_conn)):
@@ -475,14 +466,35 @@
         if password:
             self._config['password'] = password
         url = input('Pan.do/ra URL (i.e. https://pandora.local/api/): ')
         if url:
             self._config['url'] = url
         self.save_config()
         print("\nconfiguration updated.")
+        self.install_programs()
+
+    def install_programs(self, args=[]):
+        update = 'update' in args
+        # install required programs
+        if sys.platform == 'darwin':
+            osext = 'macosx'
+        elif sys.platform.startswith('win'):
+            osext = 'exe'
+        else:
+            osext = 'linux'
+        bindir = os.path.join(utils.basedir(), 'bin')
+        ox.makedirs(bindir)
+        for p in ('ffmpeg', 'ffmpeg2theora'):
+            path = os.path.join(bindir, p)
+            if sys.platform.startswith('win'):
+                p += '.exe'
+            if not os.path.exists(path) or update:
+                print("installing %s in %s" % (p, bindir))
+                ox.net.save_url('http://firefogg.org/bin/%s.%s' % (p, osext), path, True)
+                os.chmod(path, 0o755)
 
     def add_volume(self, args):
         usage = "Usage: %s add_volume name path" % sys.argv[0]
         if len(args) != 2:
             print(usage)
             sys.exit(1)
         name = args[0]
```

### Comparing `pandora_client-0.3.13/pandora_client/client.py` & `pandora_client-0.3.6/pandora_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,14 @@
 
 class DistributedClient:
 
     interrupted = False
 
     def __init__(self, url, name, threads):
         self.url = url
-        while self.url and self.url[-1] == '/':
-            self.url = self.url[:-1]
         self.name = name
         self.threads = threads
         self.supported_formats = extract.supported_formats()
 
     def ping(self, oshash):
         try:
             url = '%s/ping/%s/%s' % (self.url, oshash, self.name)
```

### Comparing `pandora_client-0.3.13/pandora_client/extract.py` & `pandora_client-0.3.6/pandora_client/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,21 @@
     ffmpeg = command('ffmpeg')
     if ffmpeg is None:
         return None
     p = subprocess.Popen([ffmpeg, '-codecs'],
                          stdout=subprocess.PIPE, stderr=subprocess.PIPE, close_fds=True)
     stdout, stderr = p.communicate()
     stdout = stdout.decode('utf-8')
-    mp4 = 'libx264' in stdout and bool(re.compile('DEA.L. aac').findall(stdout))
     return {
         'ogg': 'libtheora' in stdout and 'libvorbis' in stdout,
         'webm': 'libvpx' in stdout and 'libvorbis' in stdout,
         'vp8': 'libvpx' in stdout and 'libvorbis' in stdout,
         'vp9': 'libvpx-vp9' in stdout and 'libopus' in stdout,
-        'mp4': mp4,
-        'h264': mp4,
+        'mp4': 'libx264' in stdout and 'DEA.L. aac' in stdout,
+        'h264': 'libx264' in stdout and 'DEA.L. aac' in stdout,
     }
 
 def video_cmd(video, target, profile, info):
 
     if not os.path.exists(target):
         ox.makedirs(os.path.dirname(target))
```

### Comparing `pandora_client-0.3.13/pandora_client/localnode.py` & `pandora_client-0.3.6/pandora_client/localnode.py`

 * *Files identical despite different names*

### Comparing `pandora_client-0.3.13/pandora_client/server.py` & `pandora_client-0.3.6/pandora_client/server.py`

 * *Files identical despite different names*

### Comparing `pandora_client-0.3.13/pandora_client/utils.py` & `pandora_client-0.3.6/pandora_client/utils.py`

 * *Files identical despite different names*

### Comparing `pandora_client-0.3.13/setup.py` & `pandora_client-0.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 
 def get_version():
-    return 13 #import os
+    return 6 #import os
     import re
     import subprocess
     dot_git = os.path.join(os.path.dirname(__file__), '.git')
     changelog = os.path.join(os.path.dirname(__file__), 'debian/changelog')
     if os.path.exists(dot_git):
         cmd = ['git', 'rev-list', 'HEAD', '--count']
         p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
@@ -26,15 +26,15 @@
 
 setup(
     name="pandora_client",
     version="0.3.%s" % get_version(),
     description="pandora_client is a commandline client for pan.do/ra. You can use it to import videos into a pan.do/ra system. It is currently known to work on Linux and Mac OS X.",
     author="j",
     author_email="j@mailb.org",
-    url="https://code.0x2620.org/0x2620/pandora_client/wiki",
+    url="http://wiki.0x2620.org/wiki/pandora_client",
     license="GPLv3",
     scripts=[
         'bin/pandora_client',
     ],
     packages=[
         'pandora_client'
     ],
```

