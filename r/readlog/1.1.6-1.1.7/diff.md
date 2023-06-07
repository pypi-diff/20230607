# Comparing `tmp/readlog-1.1.6.tar.gz` & `tmp/readlog-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.6.tar", last modified: Fri Jun  2 09:20:10 2023, max compression
+gzip compressed data, was "readlog-1.1.7.tar", last modified: Wed Jun  7 06:46:39 2023, max compression
```

## Comparing `readlog-1.1.6.tar` & `readlog-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.349255 readlog-1.1.6/
--rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      759 2023-06-02 09:20:10.348256 readlog-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-06-02 09:15:04.000000 readlog-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.320907 readlog-1.1.6/demo/
-drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.322905 readlog-1.1.6/demo/__pycache__/
--rw-rw-rw-   0        0        0     5361 2023-06-02 08:42:26.000000 readlog-1.1.6/demo/__pycache__/readlog.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.328214 readlog-1.1.6/demo/imgs/
--rw-rw-rw-   0        0        0   220194 2023-06-02 08:49:13.000000 readlog-1.1.6/demo/imgs/PotEng.png
--rw-rw-rw-   0        0        0   219866 2023-06-02 08:52:03.000000 readlog-1.1.6/demo/imgs/PotEng_incomplete.png
--rw-rw-rw-   0        0        0    80925 2023-06-02 08:38:09.000000 readlog-1.1.6/demo/log.lammps
--rw-rw-rw-   0        0        0    76031 2023-06-02 08:50:50.000000 readlog-1.1.6/demo/log_incomplete.lammps
--rw-rw-rw-   0        0        0     1235 2023-06-02 08:51:24.000000 readlog-1.1.6/demo/plot_themo.py
--rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 09:20:10.349255 readlog-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-06-02 09:19:57.000000 readlog-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.331206 readlog-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.345277 readlog-1.1.6/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      759 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3000 2023-06-02 08:51:40.000000 readlog-1.1.6/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.228189 readlog-1.1.7/
+-rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      849 2023-06-07 06:46:39.227189 readlog-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-06-07 06:46:18.000000 readlog-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.204596 readlog-1.1.7/demo/
+-rw-rw-rw-   0        0        0   235181 2023-06-07 06:29:27.000000 readlog-1.1.7/demo/1_hydrate_dissociation_log.lammps
+drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.206597 readlog-1.1.7/demo/__pycache__/
+-rw-rw-rw-   0        0        0     5413 2023-06-07 06:40:50.000000 readlog-1.1.7/demo/__pycache__/readlog.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.211597 readlog-1.1.7/demo/imgs/
+-rw-rw-rw-   0        0        0   220194 2023-06-07 06:41:45.000000 readlog-1.1.7/demo/imgs/PotEng.png
+-rw-rw-rw-   0        0        0   222242 2023-06-07 06:35:07.000000 readlog-1.1.7/demo/imgs/PotEng_incomplete.png
+-rw-rw-rw-   0        0        0    80925 2023-06-02 08:38:09.000000 readlog-1.1.7/demo/log.lammps
+-rw-rw-rw-   0        0        0    28861 2023-06-07 06:32:27.000000 readlog-1.1.7/demo/log_incomplete.lammps
+-rw-rw-rw-   0        0        0     1272 2023-06-07 06:41:43.000000 readlog-1.1.7/demo/plot_themo.py
+-rw-rw-rw-   0        0        0     3060 2023-06-07 06:40:48.000000 readlog-1.1.7/demo/readlog.py
+-rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:46:39.228189 readlog-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-06-07 06:42:10.000000 readlog-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.213597 readlog-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.223648 readlog-1.1.7/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-07 06:46:39.000000 readlog-1.1.7/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3060 2023-06-07 06:40:48.000000 readlog-1.1.7/src/readlog.py
```

### Comparing `readlog-1.1.6/PKG-INFO` & `readlog-1.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.6
+Version: 1.1.7
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
 
-- A python code to read thermo info from lammps log file 
+- A python code to read thermo info from the log file of lammps output
 
 ### Installation 
 
 ```bash
 git clone https://github.com/eastsheng/readlog.git
 cd readlog
 pip install .
 # or
 pip install readlog
+pip install readlog -i https://pypi.org/simple
 ```
 
 ### Requirements
 
 - numpy
 - pandas
 - matplotlib
@@ -38,11 +39,11 @@
 - out:
 - ![](./demo/imgs/PotEng.png)
 
 
 
 ### Fixed
 
-- [x] Adapting to incomplete thermo information.
+- [x] Fixed a read error in the complete message frame under incomplete message
+
 
-
```

### Comparing `readlog-1.1.6/demo/__pycache__/readlog.cpython-311.pyc` & `readlog-1.1.7/demo/__pycache__/readlog.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x70ab7964 (Fri Jun  2 08:42:24 2023 UTC)
-files sz: 3000
+moddate:  0x70268064 (Wed Jun  7 06:40:48 2023 UTC)
+files sz: 3060
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c015a02640164026c035a04640164026c056d
@@ -58,125 +58,125 @@
                 40 MAKE_FUNCTION            0
                 42 LOAD_CONST               4 ('ReadLog')
                 44 LOAD_NAME                8 (object)
                 46 PRECALL                  3
                 50 CALL                     3
                 60 STORE_NAME               9 (ReadLog)
    
-    70          62 LOAD_NAME               10 (__name__)
+    72          62 LOAD_NAME               10 (__name__)
                 64 LOAD_CONST               5 ('__main__')
                 66 COMPARE_OP               2 (==)
                 72 EXTENDED_ARG             1
                 74 POP_JUMP_FORWARD_IF_FALSE   298 (to 672)
    
-    71          76 LOAD_CONST               6 ('./')
+    73          76 LOAD_CONST               6 ('./')
                 78 STORE_NAME              11 (path)
    
-    72          80 LOAD_CONST               7 ('log.lammps')
+    74          80 LOAD_CONST               7 ('log.lammps')
                 82 STORE_NAME              12 (logfile)
    
-    73          84 LOAD_CONST               8 (0.101325)
+    75          84 LOAD_CONST               8 (0.101325)
                 86 STORE_NAME              13 (atm2mPa)
    
-    74          88 LOAD_CONST               1 (0)
+    76          88 LOAD_CONST               1 (0)
                 90 STORE_NAME              14 (nf_log)
    
-    77          92 PUSH_NULL
+    79          92 PUSH_NULL
                 94 LOAD_NAME                9 (ReadLog)
                 96 LOAD_NAME               11 (path)
                 98 LOAD_NAME               12 (logfile)
                100 BINARY_OP                0 (+)
                104 PRECALL                  1
                108 CALL                     1
                118 STORE_NAME              15 (rl)
    
-    78         120 PUSH_NULL
+    80         120 PUSH_NULL
                122 LOAD_NAME               16 (print)
                124 LOAD_CONST               9 ('*')
                126 LOAD_CONST              10 ('--------------------')
                128 LOAD_CONST              11 ('Reading frames of themo')
                130 LOAD_CONST              10 ('--------------------')
                132 LOAD_CONST               9 ('*')
                134 PRECALL                  5
                138 CALL                     5
                148 POP_TOP
    
-    79         150 LOAD_NAME               15 (rl)
+    81         150 LOAD_NAME               15 (rl)
                152 LOAD_METHOD             17 (ReadUD)
                174 LOAD_NAME               11 (path)
                176 LOAD_NAME               12 (logfile)
                178 BINARY_OP                0 (+)
                182 PRECALL                  1
                186 CALL                     1
                196 UNPACK_SEQUENCE          2
                200 STORE_NAME              18 (thermou_list)
                202 STORE_NAME              19 (thermod_list)
    
-    80         204 LOAD_NAME               15 (rl)
+    82         204 LOAD_NAME               15 (rl)
                206 LOAD_METHOD             20 (ReadThermo)
                228 LOAD_NAME               11 (path)
                230 LOAD_NAME               12 (logfile)
                232 BINARY_OP                0 (+)
                236 LOAD_NAME               18 (thermou_list)
                238 LOAD_NAME               19 (thermod_list)
                240 LOAD_NAME               14 (nf_log)
                242 PRECALL                  4
                246 CALL                     4
                256 STORE_NAME              21 (pd_thermo)
    
-    81         258 PUSH_NULL
+    83         258 PUSH_NULL
                260 LOAD_NAME               16 (print)
                262 LOAD_CONST              12 ('Your label list of thermo :\n')
                264 LOAD_NAME               21 (pd_thermo)
                266 LOAD_ATTR               22 (columns)
                276 PRECALL                  2
                280 CALL                     2
                290 POP_TOP
    
-    82         292 PUSH_NULL
+    84         292 PUSH_NULL
                294 LOAD_NAME               16 (print)
                296 LOAD_CONST               9 ('*')
                298 LOAD_CONST              10 ('--------------------')
                300 LOAD_CONST              13 ('Reading END!!!!!!!!!!!!')
                302 LOAD_CONST              10 ('--------------------')
                304 LOAD_CONST               9 ('*')
                306 PRECALL                  5
                310 CALL                     5
                320 POP_TOP
    
-    83         322 PUSH_NULL
+    85         322 PUSH_NULL
                324 LOAD_NAME                7 (plt)
                326 LOAD_ATTR               23 (rc)
                336 LOAD_CONST              14 ('font')
                338 LOAD_CONST              15 ('Times New Roman')
                340 LOAD_CONST              16 (22)
                342 KW_NAMES                17
                344 PRECALL                  3
                348 CALL                     3
                358 POP_TOP
    
-    84         360 PUSH_NULL
+    86         360 PUSH_NULL
                362 LOAD_NAME                7 (plt)
                364 LOAD_ATTR               24 (figure)
                374 LOAD_CONST              18 ((12, 10))
                376 KW_NAMES                19
                378 PRECALL                  1
                382 CALL                     1
                392 STORE_NAME              25 (fig)
    
-    85         394 LOAD_NAME               25 (fig)
+    87         394 LOAD_NAME               25 (fig)
                396 LOAD_METHOD             26 (add_subplot)
                418 LOAD_CONST              20 (1)
                420 LOAD_CONST              20 (1)
                422 LOAD_CONST              20 (1)
                424 PRECALL                  3
                428 CALL                     3
                438 STORE_NAME              27 (ax)
    
-    86         440 LOAD_NAME               27 (ax)
+    88         440 LOAD_NAME               27 (ax)
                442 LOAD_METHOD             28 (plot)
                464 LOAD_NAME               21 (pd_thermo)
                466 LOAD_CONST              21 ('Step')
                468 BINARY_SUBSCR
                478 LOAD_CONST              22 (0.001)
                480 BINARY_OP                5 (*)
                484 LOAD_NAME               21 (pd_thermo)
@@ -185,47 +185,47 @@
                498 LOAD_CONST              24 ('r')
                500 LOAD_CONST              23 ('PotEng')
                502 KW_NAMES                25
                504 PRECALL                  4
                508 CALL                     4
                518 POP_TOP
    
-    87         520 PUSH_NULL
+    89         520 PUSH_NULL
                522 LOAD_NAME                7 (plt)
                524 LOAD_ATTR               29 (legend)
                534 LOAD_CONST              26 ('best')
                536 KW_NAMES                27
                538 PRECALL                  1
                542 CALL                     1
                552 POP_TOP
    
-    90         554 LOAD_NAME               27 (ax)
+    92         554 LOAD_NAME               27 (ax)
                556 LOAD_METHOD             30 (set_xlabel)
                578 LOAD_CONST              28 ('Time (ps)')
                580 PRECALL                  1
                584 CALL                     1
                594 POP_TOP
    
-    91         596 LOAD_NAME               27 (ax)
+    93         596 LOAD_NAME               27 (ax)
                598 LOAD_METHOD             31 (set_ylabel)
                620 LOAD_CONST              29 ('PotEng (kcal/mol)')
                622 PRECALL                  1
                626 CALL                     1
                636 POP_TOP
    
-    95         638 PUSH_NULL
+    97         638 PUSH_NULL
                640 LOAD_NAME                7 (plt)
                642 LOAD_ATTR               32 (show)
                652 PRECALL                  0
                656 CALL                     0
                666 POP_TOP
                668 LOAD_CONST               2 (None)
                670 RETURN_VALUE
    
-    70     >>  672 LOAD_CONST               2 (None)
+    72     >>  672 LOAD_CONST               2 (None)
                674 RETURN_VALUE
    consts
       '\nread lammps log file for some thermo data\n'
       0
       None
       code
          argcount  : 0
@@ -586,26 +586,27 @@
                nlocals   : 12
                stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000007c02a6010000ab0100000000000000
                   007d057401000000000000000000007c03a6010000ab0100000000000000
                   007d067403000000000000000000007c05a6010000ab0100000000000000
-                  0044005da47d077c057c066b020000000072157c037c0719000000000000
+                  0044005db47d077c057c066b020000000072157c037c0719000000000000
                   0000007c027c07190000000000000000007a0a000064017a0a00007d086e
-                  2a7c057404000000000000000000006b0400000000721f7c077c0564017a
-                  0a00006b020000000072167c006a03000000000000000064017a0a00007c
-                  027c07190000000000000000007a0a000064017a0a00007d087c047c076b
-                  020000000072577409000000000000000000006a0500000000000000007c
-                  01640264037c027c071900000000000000000064017a0a00006401ac04a6
-                  050000ab0500000000000000007d097409000000000000000000006a0500
-                  000000000000007c017c027c07190000000000000000007c086403ac05a6
-                  040000ab0400000000000000007d0a740d000000000000000000006a0700
-                  000000000000007c0a7c09ac06a6020000ab0200000000000000007d0b8c
-                  a48ca57c0b5300
+                  3a7c057c066b040000000072347c077c0564017a0a00006b020000000072
+                  177c006a02000000000000000064017a0a00007c027c0719000000000000
+                  0000007a0a000064017a0a00007d086e147c037c07190000000000000000
+                  007c027c07190000000000000000007a0a000064017a0a00007d087c047c
+                  076b020000000072577407000000000000000000006a0400000000000000
+                  007c01640264037c027c071900000000000000000064017a0a00006401ac
+                  04a6050000ab0500000000000000007d097407000000000000000000006a
+                  0400000000000000007c017c027c07190000000000000000007c086403ac
+                  05a6040000ab0400000000000000007d0a740b000000000000000000006a
+                  0600000000000000007c0a7c09ac06a6020000ab0200000000000000007d
+                  0b8cb48cb57c0b5300
                 51           0 RESUME                   0
                
                 52           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                2 (thermou_list)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_FAST               5 (L_u)
@@ -617,15 +618,15 @@
                             60 STORE_FAST               6 (L_d)
                
                 55          62 LOAD_GLOBAL              3 (NULL + range)
                             74 LOAD_FAST                5 (L_u)
                             76 PRECALL                  1
                             80 CALL                     1
                             90 GET_ITER
-                       >>   92 FOR_ITER               164 (to 422)
+                       >>   92 FOR_ITER               180 (to 454)
                             94 STORE_FAST               7 (i)
                
                 56          96 LOAD_FAST                5 (L_u)
                             98 LOAD_FAST                6 (L_d)
                            100 COMPARE_OP               2 (==)
                            106 POP_JUMP_FORWARD_IF_FALSE    21 (to 150)
                
@@ -635,104 +636,118 @@
                            122 LOAD_FAST                2 (thermou_list)
                            124 LOAD_FAST                7 (i)
                            126 BINARY_SUBSCR
                            136 BINARY_OP               10 (-)
                            140 LOAD_CONST               1 (1)
                            142 BINARY_OP               10 (-)
                            146 STORE_FAST               8 (n_line)
-                           148 JUMP_FORWARD            42 (to 234)
+                           148 JUMP_FORWARD            58 (to 266)
                
                 58     >>  150 LOAD_FAST                5 (L_u)
-                           152 LOAD_GLOBAL              4 (l_d)
-                           164 COMPARE_OP               4 (>)
-                           170 POP_JUMP_FORWARD_IF_FALSE    31 (to 234)
-               
-                59         172 LOAD_FAST                7 (i)
-                           174 LOAD_FAST                5 (L_u)
-                           176 LOAD_CONST               1 (1)
-                           178 BINARY_OP               10 (-)
-                           182 COMPARE_OP               2 (==)
-                           188 POP_JUMP_FORWARD_IF_FALSE    22 (to 234)
-               
-                60         190 LOAD_FAST                0 (self)
-                           192 LOAD_ATTR                3 (tot_line_number)
-                           202 LOAD_CONST               1 (1)
-                           204 BINARY_OP               10 (-)
-                           208 LOAD_FAST                2 (thermou_list)
-                           210 LOAD_FAST                7 (i)
-                           212 BINARY_SUBSCR
-                           222 BINARY_OP               10 (-)
-                           226 LOAD_CONST               1 (1)
-                           228 BINARY_OP               10 (-)
-                           232 STORE_FAST               8 (n_line)
-               
-                62     >>  234 LOAD_FAST                4 (nf_log)
-                           236 LOAD_FAST                7 (i)
-                           238 COMPARE_OP               2 (==)
-                           244 POP_JUMP_FORWARD_IF_FALSE    87 (to 420)
-               
-                63         246 LOAD_GLOBAL              9 (NULL + np)
-                           258 LOAD_ATTR                5 (loadtxt)
-                           268 LOAD_FAST                1 (LogFile)
-                           270 LOAD_CONST               2 ('str')
-                           272 LOAD_CONST               3 ('utf-8')
-                           274 LOAD_FAST                2 (thermou_list)
-                           276 LOAD_FAST                7 (i)
-                           278 BINARY_SUBSCR
-                           288 LOAD_CONST               1 (1)
-                           290 BINARY_OP               10 (-)
-                           294 LOAD_CONST               1 (1)
-                           296 KW_NAMES                 4
-                           298 PRECALL                  5
-                           302 CALL                     5
-                           312 STORE_FAST               9 (thermo_col)
-               
-                64         314 LOAD_GLOBAL              9 (NULL + np)
-                           326 LOAD_ATTR                5 (loadtxt)
-                           336 LOAD_FAST                1 (LogFile)
-                           338 LOAD_FAST                2 (thermou_list)
-                           340 LOAD_FAST                7 (i)
-                           342 BINARY_SUBSCR
-                           352 LOAD_FAST                8 (n_line)
-                           354 LOAD_CONST               3 ('utf-8')
-                           356 KW_NAMES                 5
-                           358 PRECALL                  4
-                           362 CALL                     4
-                           372 STORE_FAST              10 (thermo_data)
-               
-                65         374 LOAD_GLOBAL             13 (NULL + pd)
-                           386 LOAD_ATTR                7 (DataFrame)
-                           396 LOAD_FAST               10 (thermo_data)
-                           398 LOAD_FAST                9 (thermo_col)
-                           400 KW_NAMES                 6
-                           402 PRECALL                  2
-                           406 CALL                     2
-                           416 STORE_FAST              11 (pd_thermo)
-                           418 JUMP_BACKWARD          164 (to 92)
+                           152 LOAD_FAST                6 (L_d)
+                           154 COMPARE_OP               4 (>)
+                           160 POP_JUMP_FORWARD_IF_FALSE    52 (to 266)
+               
+                59         162 LOAD_FAST                7 (i)
+                           164 LOAD_FAST                5 (L_u)
+                           166 LOAD_CONST               1 (1)
+                           168 BINARY_OP               10 (-)
+                           172 COMPARE_OP               2 (==)
+                           178 POP_JUMP_FORWARD_IF_FALSE    23 (to 226)
+               
+                60         180 LOAD_FAST                0 (self)
+                           182 LOAD_ATTR                2 (tot_line_number)
+                           192 LOAD_CONST               1 (1)
+                           194 BINARY_OP               10 (-)
+                           198 LOAD_FAST                2 (thermou_list)
+                           200 LOAD_FAST                7 (i)
+                           202 BINARY_SUBSCR
+                           212 BINARY_OP               10 (-)
+                           216 LOAD_CONST               1 (1)
+                           218 BINARY_OP               10 (-)
+                           222 STORE_FAST               8 (n_line)
+                           224 JUMP_FORWARD            20 (to 266)
+               
+                62     >>  226 LOAD_FAST                3 (thermod_list)
+                           228 LOAD_FAST                7 (i)
+                           230 BINARY_SUBSCR
+                           240 LOAD_FAST                2 (thermou_list)
+                           242 LOAD_FAST                7 (i)
+                           244 BINARY_SUBSCR
+                           254 BINARY_OP               10 (-)
+                           258 LOAD_CONST               1 (1)
+                           260 BINARY_OP               10 (-)
+                           264 STORE_FAST               8 (n_line)
+               
+                64     >>  266 LOAD_FAST                4 (nf_log)
+                           268 LOAD_FAST                7 (i)
+                           270 COMPARE_OP               2 (==)
+                           276 POP_JUMP_FORWARD_IF_FALSE    87 (to 452)
+               
+                65         278 LOAD_GLOBAL              7 (NULL + np)
+                           290 LOAD_ATTR                4 (loadtxt)
+                           300 LOAD_FAST                1 (LogFile)
+                           302 LOAD_CONST               2 ('str')
+                           304 LOAD_CONST               3 ('utf-8')
+                           306 LOAD_FAST                2 (thermou_list)
+                           308 LOAD_FAST                7 (i)
+                           310 BINARY_SUBSCR
+                           320 LOAD_CONST               1 (1)
+                           322 BINARY_OP               10 (-)
+                           326 LOAD_CONST               1 (1)
+                           328 KW_NAMES                 4
+                           330 PRECALL                  5
+                           334 CALL                     5
+                           344 STORE_FAST               9 (thermo_col)
+               
+                66         346 LOAD_GLOBAL              7 (NULL + np)
+                           358 LOAD_ATTR                4 (loadtxt)
+                           368 LOAD_FAST                1 (LogFile)
+                           370 LOAD_FAST                2 (thermou_list)
+                           372 LOAD_FAST                7 (i)
+                           374 BINARY_SUBSCR
+                           384 LOAD_FAST                8 (n_line)
+                           386 LOAD_CONST               3 ('utf-8')
+                           388 KW_NAMES                 5
+                           390 PRECALL                  4
+                           394 CALL                     4
+                           404 STORE_FAST              10 (thermo_data)
+               
+                67         406 LOAD_GLOBAL             11 (NULL + pd)
+                           418 LOAD_ATTR                6 (DataFrame)
+                           428 LOAD_FAST               10 (thermo_data)
+                           430 LOAD_FAST                9 (thermo_col)
+                           432 KW_NAMES                 6
+                           434 PRECALL                  2
+                           438 CALL                     2
+                           448 STORE_FAST              11 (pd_thermo)
+                           450 JUMP_BACKWARD          180 (to 92)
                
-                67     >>  420 JUMP_BACKWARD          165 (to 92)
+                69     >>  452 JUMP_BACKWARD          181 (to 92)
                
-                68     >>  422 LOAD_FAST               11 (pd_thermo)
-                           424 RETURN_VALUE
+                70     >>  454 LOAD_FAST               11 (pd_thermo)
+                           456 RETURN_VALUE
                consts
                   None
                   1
                   'str'
                   'utf-8'
                   ('dtype', 'encoding', 'skiprows', 'max_rows')
                   ('skiprows', 'max_rows', 'encoding')
                   ('columns',)
-               names      ('len', 'range', 'l_d', 'tot_line_number', 'np', 'loadtxt', 'pd', 'DataFrame')
+               names      ('len', 'range', 'tot_line_number', 'np', 'loadtxt', 'pd', 'DataFrame')
                varnames   ('self', 'LogFile', 'thermou_list', 'thermod_list', 'nf_log', 'L_u', 'L_d', 'i', 'n_line', 'thermo_col', 'thermo_data', 'pd_thermo')
                freevars   ()
                cellvars   ()
                filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\readlog\\demo\\readlog.py'
                name       'ReadThermo'
                firstlineno 51
-               lnotab 0x02011e011e0222010c012a01160112012c020c0144013c012e020201
+               lnotab
+                  0x02011e011e0222010c012a010c0112012e0228020c0144013c012e0202
+                  01
             (0,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'timeunit', 'ReadUD', 'ReadThermo', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\readlog\\demo\\readlog.py'
          name       'ReadLog'
@@ -768,9 +783,9 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'E:\\DongshengChen\\OneDrive - student.cup.edu.cn\\Github\\MyRepos\\readlog\\demo\\readlog.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010403080108020c021c3d0e0104010401040104031c011e0136
+      0x00ff02010403080108020c021c3f0e0104010401040104031c011e0136
       01360122011e01260122012e01500122032a012a0422e7
```

### Comparing `readlog-1.1.6/demo/imgs/PotEng.png` & `readlog-1.1.7/demo/imgs/PotEng.png`

 * *Files identical despite different names*

### Comparing `readlog-1.1.6/demo/log.lammps` & `readlog-1.1.7/demo/log.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.6/demo/plot_themo.py` & `readlog-1.1.7/demo/plot_themo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import readlog as RLog
 from pathlib import Path
 import matplotlib.pyplot as plt
 
 if __name__ == '__main__':
 	path = "./"
-	logfile = "log_incomplete.lammps"
+	logfile = "log.lammps"
 	atm2mPa = 0.101325
 	nf_log = 0 # The number of logs in logfile
 	time_step = 1 # fs
 
 	Path(path+"imgs/").mkdir(parents=True,exist_ok=True)
 	rl = RLog.ReadLog(path+logfile) 
 	print("*",20*"-","Reading frames of themo",20*"-","*")
@@ -28,9 +28,10 @@
 	# ax.set_xlim([0,10000])
 	# ax.set_ylim([-20000,-15000])
 	ax.set_xlabel("Time (ns)",fontweight="bold",fontsize=26)
 	ax.set_ylabel("PotEng (kcal/mol)",fontweight="bold",fontsize=26)
 	# ax.grid(True)
 
 	# pd_thermo.to_csv(path+"imgs/themo.csv")	
-	plt.savefig(path+"imgs/PotEng_incomplete.png",dpi=300)
+	plt.savefig(path+"imgs/PotEng.png",dpi=300)
+	# plt.savefig(path+"imgs/PotEng_incomplete.png",dpi=300)
 	plt.show()
```

### Comparing `readlog-1.1.6/setup.py` & `readlog-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.6',
+version      = '1.1.7',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
```

### Comparing `readlog-1.1.6/src/readlog.egg-info/PKG-INFO` & `readlog-1.1.7/src/readlog.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.6
+Version: 1.1.7
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
 
-- A python code to read thermo info from lammps log file 
+- A python code to read thermo info from the log file of lammps output
 
 ### Installation 
 
 ```bash
 git clone https://github.com/eastsheng/readlog.git
 cd readlog
 pip install .
 # or
 pip install readlog
+pip install readlog -i https://pypi.org/simple
 ```
 
 ### Requirements
 
 - numpy
 - pandas
 - matplotlib
@@ -38,11 +39,11 @@
 - out:
 - ![](./demo/imgs/PotEng.png)
 
 
 
 ### Fixed
 
-- [x] Adapting to incomplete thermo information.
+- [x] Fixed a read error in the complete message frame under incomplete message
+
 
-
```

### Comparing `readlog-1.1.6/src/readlog.py` & `readlog-1.1.7/demo/readlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
 		for i in range(L_u):
 			if L_u == L_d:
 				n_line = thermod_list[i]-thermou_list[i]-1
 			elif L_u>L_d:
 				if i==L_u-1:
 					n_line = self.tot_line_number-1-thermou_list[i]-1
+				else:
+					n_line = thermod_list[i]-thermou_list[i]-1
 
 			if nf_log==i:
 				thermo_col = np.loadtxt(LogFile,dtype="str",encoding='utf-8',skiprows=thermou_list[i]-1,max_rows=1)
 				thermo_data = np.loadtxt(LogFile,skiprows=thermou_list[i],max_rows=n_line,encoding='utf-8')#.reshape((1,-1))
 				pd_thermo = pd.DataFrame(thermo_data,columns=thermo_col)
 			else:
 				pass
```

