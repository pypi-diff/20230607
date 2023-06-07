# Comparing `tmp/xspf_fixup-0.9.2.tar.gz` & `tmp/xspf_fixup-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspf_fixup-0.9.2.tar", last modified: Mon Jun  5 00:35:00 2023, max compression
+gzip compressed data, was "xspf_fixup-0.9.3.tar", last modified: Wed Jun  7 00:46:47 2023, max compression
```

## Comparing `xspf_fixup-0.9.2.tar` & `xspf_fixup-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:35:00.479229 xspf_fixup-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 00:34:51.000000 xspf_fixup-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-05 00:35:00.479229 xspf_fixup-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-05 00:34:51.000000 xspf_fixup-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 00:35:00.479229 xspf_fixup-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-05 00:34:51.000000 xspf_fixup-0.9.2/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-06-05 00:34:51.000000 xspf_fixup-0.9.2/xspf_fixup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:35:00.479229 xspf_fixup-0.9.2/xspf_fixup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-05 00:35:00.000000 xspf_fixup-0.9.2/xspf_fixup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-05 00:35:00.000000 xspf_fixup-0.9.2/xspf_fixup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:35:00.000000 xspf_fixup-0.9.2/xspf_fixup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 00:35:00.000000 xspf_fixup-0.9.2/xspf_fixup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:35:00.000000 xspf_fixup-0.9.2/xspf_fixup.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     9505 2023-06-05 00:34:51.000000 xspf_fixup-0.9.2/xspf_fixup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:46:47.337441 xspf_fixup-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 00:46:37.000000 xspf_fixup-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-07 00:46:47.337441 xspf_fixup-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-07 00:46:37.000000 xspf_fixup-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:46:47.337441 xspf_fixup-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-07 00:46:37.000000 xspf_fixup-0.9.3/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-06-07 00:46:37.000000 xspf_fixup-0.9.3/to_xspf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-06-07 00:46:37.000000 xspf_fixup-0.9.3/to_xspf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-06-07 00:46:37.000000 xspf_fixup-0.9.3/xspf_fixup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:46:47.337441 xspf_fixup-0.9.3/xspf_fixup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-07 00:46:47.000000 xspf_fixup-0.9.3/xspf_fixup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-07 00:46:47.000000 xspf_fixup-0.9.3/xspf_fixup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:46:47.000000 xspf_fixup-0.9.3/xspf_fixup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 00:46:47.000000 xspf_fixup-0.9.3/xspf_fixup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:46:47.000000 xspf_fixup-0.9.3/xspf_fixup.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14659 2023-06-07 00:46:37.000000 xspf_fixup-0.9.3/xspf_fixup.py
```

### Comparing `xspf_fixup-0.9.2/LICENSE` & `xspf_fixup-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xspf_fixup-0.9.2/PKG-INFO` & `xspf_fixup-0.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspf_fixup
-Version: 0.9.2
+Version: 0.9.3
 Summary: A simple command line program to fix playlist (.xspf files) with broken links.
 Author: Juan S. Bokser
 Author-email: juan.bokser@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -63,42 +63,71 @@
 
 
 
 ## Usage
 
 ```shell
 user@host:~/tmp/xspf_fixup/examples$ xspf_fixup --help
-Usage: xspf_fixup.py [OPTIONS] [FILES]...
+Usage: xspf_fixup [OPTIONS] [FILES]...
 
   A simple command line program to fix playlist (.xspf files) with broken
   links.
 
+  For more info: (https://github.com/jbokser/xspf_fixup).
+
 Options:
   -v, --version    Show version and exit.
   -s, --show       Show .xspf file info and exit.
   -o, --overwrite  Overwrite the .xspf file.
+  -r, --report     Make a report in markdown for each .xspf file.
   -h, --help       Show this message and exit.
 user@host:~/tmp/xspf_fixup/examples$ xspf_fixup -o ./test.xspf 
 
-Title             Duration    Location                     Result
-----------------  ----------  ---------------------------  --------
-Rockland Agus     03:01       videos/Rockland Agus.mp4     Fixed
-Honky Tonk Way    04:06       videos/Honky Tonk Way.mp4    Fixed
-Forge Ahead Agos  03:24       videos/Forge Ahead Agos.mp4  Fixed
+   Title             Duration    Location                     Result
+-- ----------------  ----------  ---------------------------  --------
+ 1 Rockland Agus     03:01       videos/Rockland Agus.mp4     Fixed
+ 2 Honky Tonk Way    04:06       videos/Honky Tonk Way.mp4    Fixed
+ 3 Forge Ahead Agos  03:24       videos/Forge Ahead Agos.mp4  Fixed
 
 Tracks count: ..... 3 (Fixed: 3)
 Total duration: ... 10:32
 
-user@host:~/tmp/xspf_fixup/examples$  
+user@host:~/tmp/xspf_fixup/examples$
+```
+
+
+```shell
+user@host:~/tmp/xspf_fixup/examples$ to_xspf -h
+Usage: to_xspf [OPTIONS]
+
+  A simple command line program to generate a playlist (.xspf file) with a
+  list of files.
+
+  Example:
+
+  $ ls examples/videos/*.mp4 | to_xspf.py > file.xspf
+
+  For more info: (https://github.com/jbokser/xspf_fixup).
+
+Options:
+  -v, --version              Show version and exit.
+  -i, --input-file FILENAME  Input text file (or stdin).
+  -h, --help                 Show this message and exit.
+user@host:~/tmp/xspf_fixup/examples$ ls videos/*.mp4 | to_xspf > files.xspf
+File 'videos/Forge Ahead Agos.mp4': Ok
+File 'videos/Honky Tonk Way.mp4': Ok
+File 'videos/Rockland Agus.mp4': Ok
+
+user@host:~/tmp/xspf_fixup/examples$
 ```
 
 
 
 ## Why? (The rationale behind this)
 
-Mainly used by [me](#author) to fix the `.xspf` files that *Luis "la cosa muerta" Musa* gave me.
+Mainly used by [me](https://github.com/jbokser) to fix the `.xspf` files that *Luis "la cosa muerta" Musa* gave me.
 
 
 
 ## Author
 
-Juan S. Bokser <juan.bokser@gmail.com>
+[Juan S. Bokser](https://github.com/jbokser) <juan.bokser@gmail.com>
```

### Comparing `xspf_fixup-0.9.2/README.md` & `xspf_fixup-0.9.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -49,42 +49,71 @@
 
 
 
 ## Usage
 
 ```shell
 user@host:~/tmp/xspf_fixup/examples$ xspf_fixup --help
-Usage: xspf_fixup.py [OPTIONS] [FILES]...
+Usage: xspf_fixup [OPTIONS] [FILES]...
 
   A simple command line program to fix playlist (.xspf files) with broken
   links.
 
+  For more info: (https://github.com/jbokser/xspf_fixup).
+
 Options:
   -v, --version    Show version and exit.
   -s, --show       Show .xspf file info and exit.
   -o, --overwrite  Overwrite the .xspf file.
+  -r, --report     Make a report in markdown for each .xspf file.
   -h, --help       Show this message and exit.
 user@host:~/tmp/xspf_fixup/examples$ xspf_fixup -o ./test.xspf 
 
-Title             Duration    Location                     Result
-----------------  ----------  ---------------------------  --------
-Rockland Agus     03:01       videos/Rockland Agus.mp4     Fixed
-Honky Tonk Way    04:06       videos/Honky Tonk Way.mp4    Fixed
-Forge Ahead Agos  03:24       videos/Forge Ahead Agos.mp4  Fixed
+   Title             Duration    Location                     Result
+-- ----------------  ----------  ---------------------------  --------
+ 1 Rockland Agus     03:01       videos/Rockland Agus.mp4     Fixed
+ 2 Honky Tonk Way    04:06       videos/Honky Tonk Way.mp4    Fixed
+ 3 Forge Ahead Agos  03:24       videos/Forge Ahead Agos.mp4  Fixed
 
 Tracks count: ..... 3 (Fixed: 3)
 Total duration: ... 10:32
 
-user@host:~/tmp/xspf_fixup/examples$  
+user@host:~/tmp/xspf_fixup/examples$
+```
+
+
+```shell
+user@host:~/tmp/xspf_fixup/examples$ to_xspf -h
+Usage: to_xspf [OPTIONS]
+
+  A simple command line program to generate a playlist (.xspf file) with a
+  list of files.
+
+  Example:
+
+  $ ls examples/videos/*.mp4 | to_xspf.py > file.xspf
+
+  For more info: (https://github.com/jbokser/xspf_fixup).
+
+Options:
+  -v, --version              Show version and exit.
+  -i, --input-file FILENAME  Input text file (or stdin).
+  -h, --help                 Show this message and exit.
+user@host:~/tmp/xspf_fixup/examples$ ls videos/*.mp4 | to_xspf > files.xspf
+File 'videos/Forge Ahead Agos.mp4': Ok
+File 'videos/Honky Tonk Way.mp4': Ok
+File 'videos/Rockland Agus.mp4': Ok
+
+user@host:~/tmp/xspf_fixup/examples$
 ```
 
 
 
 ## Why? (The rationale behind this)
 
-Mainly used by [me](#author) to fix the `.xspf` files that *Luis "la cosa muerta" Musa* gave me.
+Mainly used by [me](https://github.com/jbokser) to fix the `.xspf` files that *Luis "la cosa muerta" Musa* gave me.
 
 
 
 ## Author
 
-Juan S. Bokser <juan.bokser@gmail.com>
+[Juan S. Bokser](https://github.com/jbokser) <juan.bokser@gmail.com>
```

### Comparing `xspf_fixup-0.9.2/setup.py` & `xspf_fixup-0.9.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,9 +46,9 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6'
     ],
     python_requires='>=3.6',
     install_requires=requirements,
-    scripts=['xspf_fixup', 'xspf_fixup.py']
+    scripts=['xspf_fixup', 'xspf_fixup.py', 'to_xspf', 'to_xspf.py']
 )
```

### Comparing `xspf_fixup-0.9.2/xspf_fixup.egg-info/PKG-INFO` & `xspf_fixup-0.9.3/xspf_fixup.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspf-fixup
-Version: 0.9.2
+Version: 0.9.3
 Summary: A simple command line program to fix playlist (.xspf files) with broken links.
 Author: Juan S. Bokser
 Author-email: juan.bokser@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -63,42 +63,71 @@
 
 
 
 ## Usage
 
 ```shell
 user@host:~/tmp/xspf_fixup/examples$ xspf_fixup --help
-Usage: xspf_fixup.py [OPTIONS] [FILES]...
+Usage: xspf_fixup [OPTIONS] [FILES]...
 
   A simple command line program to fix playlist (.xspf files) with broken
   links.
 
+  For more info: (https://github.com/jbokser/xspf_fixup).
+
 Options:
   -v, --version    Show version and exit.
   -s, --show       Show .xspf file info and exit.
   -o, --overwrite  Overwrite the .xspf file.
+  -r, --report     Make a report in markdown for each .xspf file.
   -h, --help       Show this message and exit.
 user@host:~/tmp/xspf_fixup/examples$ xspf_fixup -o ./test.xspf 
 
-Title             Duration    Location                     Result
-----------------  ----------  ---------------------------  --------
-Rockland Agus     03:01       videos/Rockland Agus.mp4     Fixed
-Honky Tonk Way    04:06       videos/Honky Tonk Way.mp4    Fixed
-Forge Ahead Agos  03:24       videos/Forge Ahead Agos.mp4  Fixed
+   Title             Duration    Location                     Result
+-- ----------------  ----------  ---------------------------  --------
+ 1 Rockland Agus     03:01       videos/Rockland Agus.mp4     Fixed
+ 2 Honky Tonk Way    04:06       videos/Honky Tonk Way.mp4    Fixed
+ 3 Forge Ahead Agos  03:24       videos/Forge Ahead Agos.mp4  Fixed
 
 Tracks count: ..... 3 (Fixed: 3)
 Total duration: ... 10:32
 
-user@host:~/tmp/xspf_fixup/examples$  
+user@host:~/tmp/xspf_fixup/examples$
+```
+
+
+```shell
+user@host:~/tmp/xspf_fixup/examples$ to_xspf -h
+Usage: to_xspf [OPTIONS]
+
+  A simple command line program to generate a playlist (.xspf file) with a
+  list of files.
+
+  Example:
+
+  $ ls examples/videos/*.mp4 | to_xspf.py > file.xspf
+
+  For more info: (https://github.com/jbokser/xspf_fixup).
+
+Options:
+  -v, --version              Show version and exit.
+  -i, --input-file FILENAME  Input text file (or stdin).
+  -h, --help                 Show this message and exit.
+user@host:~/tmp/xspf_fixup/examples$ ls videos/*.mp4 | to_xspf > files.xspf
+File 'videos/Forge Ahead Agos.mp4': Ok
+File 'videos/Honky Tonk Way.mp4': Ok
+File 'videos/Rockland Agus.mp4': Ok
+
+user@host:~/tmp/xspf_fixup/examples$
 ```
 
 
 
 ## Why? (The rationale behind this)
 
-Mainly used by [me](#author) to fix the `.xspf` files that *Luis "la cosa muerta" Musa* gave me.
+Mainly used by [me](https://github.com/jbokser) to fix the `.xspf` files that *Luis "la cosa muerta" Musa* gave me.
 
 
 
 ## Author
 
-Juan S. Bokser <juan.bokser@gmail.com>
+[Juan S. Bokser](https://github.com/jbokser) <juan.bokser@gmail.com>
```

