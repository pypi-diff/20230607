# Comparing `tmp/sqlite_url-0.1.0a3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_url-0.1.0a4-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 238980 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15784 b- defN 23-Mar-28 01:22 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      302 b- defN 23-Mar-28 01:22 sqlite_url/__init__.py
--rw-r--r--  2.0 unx   514456 b- defN 23-Mar-28 01:22 sqlite_url/url0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-28 01:22 sqlite_url/version.py
--rw-r--r--  2.0 unx      496 b- defN 23-Mar-28 01:22 sqlite_url-0.1.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Mar-28 01:22 sqlite_url-0.1.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-28 01:22 sqlite_url-0.1.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      643 b- defN 23-Mar-28 01:22 sqlite_url-0.1.0a3.dist-info/RECORD
-8 files, 531881 bytes uncompressed, 237860 bytes compressed:  55.3%
+Zip file size: 238977 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-Jun-07 00:13 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      302 b- defN 23-Jun-07 00:13 sqlite_url/__init__.py
+-rw-r--r--  2.0 unx   514456 b- defN 23-Jun-07 00:13 sqlite_url/url0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-07 00:13 sqlite_url/version.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jun-07 00:13 sqlite_url-0.1.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-07 00:13 sqlite_url-0.1.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-07 00:13 sqlite_url-0.1.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-07 00:13 sqlite_url-0.1.0a4.dist-info/RECORD
+8 files, 531881 bytes uncompressed, 237857 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_url/url0.so
 Comment: 
 
 Filename: sqlite_url/version.py
 Comment: 
 
-Filename: sqlite_url-0.1.0a3.dist-info/METADATA
+Filename: sqlite_url-0.1.0a4.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_url-0.1.0a3.dist-info/WHEEL
+Filename: sqlite_url-0.1.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_url-0.1.0a3.dist-info/top_level.txt
+Filename: sqlite_url-0.1.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_url-0.1.0a3.dist-info/RECORD
+Filename: sqlite_url-0.1.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## noop.cpython-311-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --dynamic {}

```diff
@@ -1,11 +1,11 @@
 
 Dynamic section at offset 0x2e80 contains 18 entries:
   Tag        Type                         Name/Value
- 0x000000000000001d (RUNPATH)            Library runpath: [/opt/hostedtoolcache/Python/3.11.2/x64/lib]
+ 0x000000000000001d (RUNPATH)            Library runpath: [/opt/hostedtoolcache/Python/3.11.3/x64/lib]
  0x000000000000000c (INIT)               0x1000
  0x000000000000000d (FINI)               0x10fc
  0x0000000000000019 (INIT_ARRAY)         0x3e70
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x3e78
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2b8
```

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 4cbc6fa6e145c1c8cc75814f05582d7af4a2e275
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 22abf3459c13b13cb4c502c2be97fd489e62d6b3
```

### strings --all --bytes=8 {}

```diff
@@ -1,12 +1,12 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
-/opt/hostedtoolcache/Python/3.11.2/x64/lib
+/opt/hostedtoolcache/Python/3.11.3/x64/lib
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
 /home/runner/work/sqlite-url/sqlite-url/python/sqlite_url
 GNU C17 9.4.0 -mtune=generic -march=x86-64 -g -O3 -fwrapv -fPIC -fasynchronous-unwind-tables -fstack-protector-strong -fstack-clash-protection -fcf-protection
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8061
```

### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -3,9 +3,9 @@
   0x00000350 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
   0x00000360 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
   0x00000370 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
   0x00000380 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
   0x00000390 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
   0x000003a0 6c697a65 002f6f70 742f686f 73746564 lize./opt/hosted
   0x000003b0 746f6f6c 63616368 652f5079 74686f6e toolcache/Python
-  0x000003c0 2f332e31 312e322f 7836342f 6c696200 /3.11.2/x64/lib.
+  0x000003c0 2f332e31 312e332f 7836342f 6c696200 /3.11.3/x64/lib.
```

## sqlite_url/url0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 86858346a51fe7a3e829074ba187669604f49609
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: e9e27a9bc10eb318f076333d4850a5b724d75f75
```

### strings --all --bytes=8 {}

```diff
@@ -478,17 +478,17 @@
 []A\A]A^A_
 A\A]A^A_
 A\A]A^A_
 AWAVAUATI
 []A\A]A^A_
 []A\A]A^A_
  ]A\A]A^A_
-v0.1.0-alpha.3
-3231bda6f0e725bf214587722c2ae623d44da8df
-2023-03-28T01:22:13Z+0000
+v0.1.0-alpha.4
+2d06fd4a10570296673bd0441d0bcc9a12998fc1
+2023-06-07T00:13:26Z+0000
 Version: %s
 Date: %s
 Source: %s
 libcurl: %s
 url() requires odd number of arguments
 Error initializating URL in the first argument
 Invalid 'host' value
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,14 +1,14 @@
 
 Hex dump of section '.rodata':
-  0x00059000 76302e31 2e302d61 6c706861 2e330000 v0.1.0-alpha.3..
-  0x00059010 33323331 62646136 66306537 32356266 3231bda6f0e725bf
-  0x00059020 32313435 38373732 32633261 65363233 214587722c2ae623
-  0x00059030 64343464 61386466 00323032 332d3033 d44da8df.2023-03
-  0x00059040 2d323854 30313a32 323a3133 5a2b3030 -28T01:22:13Z+00
+  0x00059000 76302e31 2e302d61 6c706861 2e340000 v0.1.0-alpha.4..
+  0x00059010 32643036 66643461 31303537 30323936 2d06fd4a10570296
+  0x00059020 36373362 64303434 31643062 63633961 673bd0441d0bcc9a
+  0x00059030 31323939 38666331 00323032 332d3036 12998fc1.2023-06
+  0x00059040 2d303754 30303a31 333a3236 5a2b3030 -07T00:13:26Z+00
   0x00059050 30300000 00000000 56657273 696f6e3a 00......Version:
   0x00059060 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00059070 7263653a 2025730a 6c696263 75726c3a rce: %s.libcurl:
   0x00059080 20257300 00000000 75726c28 29207265  %s.....url() re
   0x00059090 71756972 6573206f 6464206e 756d6265 quires odd numbe
   0x000590a0 72206f66 20617267 756d656e 74730000 r of arguments..
   0x000590b0 4572726f 7220696e 69746961 6c697a61 Error initializa
```

## sqlite_url/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.3"
+__version__ = "0.1.0-alpha.4"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_url-0.1.0a3.dist-info/RECORD` & `sqlite_url-0.1.0a4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-noop.cpython-311-x86_64-linux-gnu.so,sha256=h3kqhchKGNlu6Qagh1KipnzvF5jpj0DWAwBQdRvnIbc,15784
+noop.cpython-311-x86_64-linux-gnu.so,sha256=kAfc9eDElEqFC2BGRJUPi-X2s78FFdmb-Xv3x7jyOaU,15784
 sqlite_url/__init__.py,sha256=PdL2nBKNZstu0_AZr97lI-WiLmcfNt3Tf--ULY-ET0s,302
-sqlite_url/url0.so,sha256=9ra_yOL4VFDxyigAnxw7FVryRjKCxV0rxoqt8lh-Kio,514456
-sqlite_url/version.py,sha256=UsYOyUf0to_Ob8SXHxxquepi8gVho4EnFOtvMVe3xNc,79
-sqlite_url-0.1.0a3.dist-info/METADATA,sha256=uJg3snGuxUqYkGt9l8D8jmgtsjZkwqbk0oAbVO1_qbI,496
-sqlite_url-0.1.0a3.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_url-0.1.0a3.dist-info/top_level.txt,sha256=UugqZCwj0DKQ1KbtV1KaQH9BIWTZKYaMjlbkw5ecKS0,16
-sqlite_url-0.1.0a3.dist-info/RECORD,,
+sqlite_url/url0.so,sha256=3eTJCJ2OQuI2Mv_Y_gdUl-wqc2OypjVxvigmy_oG8dQ,514456
+sqlite_url/version.py,sha256=_9iw-Vd8eX6yNm_UJ00B-r49sQ9eJXJWWZXiQTepATw,79
+sqlite_url-0.1.0a4.dist-info/METADATA,sha256=UHX7wpUlXy6bvic5iKS8eVzNSvNzDoTCBjuGnanYVpI,496
+sqlite_url-0.1.0a4.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
+sqlite_url-0.1.0a4.dist-info/top_level.txt,sha256=UugqZCwj0DKQ1KbtV1KaQH9BIWTZKYaMjlbkw5ecKS0,16
+sqlite_url-0.1.0a4.dist-info/RECORD,,
```

