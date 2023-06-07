# Comparing `tmp/ExpdFtpService-0.8.0.tar.gz` & `tmp/ExpdFtpService-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ExpdFtpService-0.8.0.tar", last modified: Wed Apr 19 01:22:14 2023, max compression
+gzip compressed data, was "dist\ExpdFtpService-0.9.0.tar", last modified: Wed Jun  7 02:28:48 2023, max compression
```

## Comparing `ExpdFtpService-0.8.0.tar` & `ExpdFtpService-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/
--rw-rw-rw-   0        0        0      305 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-04-18 05:39:20.000000 ExpdFtpService-0.8.0/README.md
--rw-rw-rw-   0        0        0      115 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-04-19 01:16:48.000000 ExpdFtpService-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService/
--rw-rw-rw-   0        0        0     4512 2023-04-19 01:21:54.000000 ExpdFtpService-0.8.0/src/ExpdFtpService/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/
--rw-rw-rw-   0        0        0      305 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 01:22:14.000000 ExpdFtpService-0.8.0/src/ExpdFtpService.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/
+-rw-rw-rw-   0        0        0      276 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-04-18 05:39:20.000000 ExpdFtpService-0.9.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-07 02:27:21.000000 ExpdFtpService-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/ExpdFtpService/
+-rw-rw-rw-   0        0        0     4366 2023-06-07 02:25:59.000000 ExpdFtpService-0.9.0/src/ExpdFtpService/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/ExpdFtpService.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/ExpdFtpService.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/ExpdFtpService.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/ExpdFtpService.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/ExpdFtpService.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-07 02:28:48.000000 ExpdFtpService-0.9.0/src/ExpdFtpService.egg-info/top_level.txt
```

### Comparing `ExpdFtpService-0.8.0/README.md` & `ExpdFtpService-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ExpdFtpService-0.8.0/src/ExpdFtpService/__init__.py` & `ExpdFtpService-0.9.0/src/ExpdFtpService/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from os import path, sys
 sys.path.append(path.dirname(path.dirname(path.abspath(__file__))))
 
 from loguru import logger
 from ftplib import FTP
+from datetime import datetime
 
 
 class ConnFtpServer:
     """
     The ConnFtpServer class is used for connecting to a FTP Server. The constructor accepts the following parameters with the indicated types:
         hostname (str): The hostname of the FTP server.
         username (str): The username to login to the FTP server.
@@ -38,20 +39,15 @@
             files = [x for x in self.ftp.nlst() if x.endswith(self.filendwith)]
         else:
             files = [x for x in self.ftp.nlst() if str(x).lower() != 'history']
         logger.debug(f"Ftp server {self.servercode} total files: [{len(files)}]")
         return files
     
     def archive(self, from_file, to_path, to_file):
-        history = self.ftp.nlst(to_path)
-        if to_file not in history:
-            self.ftp.rename(f"{from_file}", f"{to_path}\{to_file}")
-        else:
-            logger.warning(f"file exist in history folder, delete: {from_file}")
-            self.ftp.delete(from_file)
+        self.ftp.rename(f"{from_file}", f'{to_path}\{datetime.now().strftime("%Y%m%d%H%M%S")}_{to_file}')
 
     @logger.catch(reraise=True)
     def download(self, numbers):
         try:
             for count, file in enumerate(self.files, 1):
                 if count <= numbers:
                     with open(path.join(self.savefolder, f"{file}"), 'wb') as rd:
```

