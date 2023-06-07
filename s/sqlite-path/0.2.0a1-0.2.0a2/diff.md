# Comparing `tmp/sqlite_path-0.2.0a1-py3-none-win_amd64.whl.zip` & `tmp/sqlite_path-0.2.0a2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21067 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-28 00:06 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      315 b- defN 23-Mar-28 00:05 sqlite_path/__init__.py
--rw-rw-rw-  2.0 fat    63330 b- defN 23-Mar-28 00:05 sqlite_path/path0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Mar-28 00:05 sqlite_path/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Mar-28 00:06 sqlite_path-0.2.0a1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Mar-28 00:06 sqlite_path-0.2.0a1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Mar-28 00:06 sqlite_path-0.2.0a1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      635 b- defN 23-Mar-28 00:06 sqlite_path-0.2.0a1.dist-info/RECORD
-8 files, 64995 bytes uncompressed, 19953 bytes compressed:  69.3%
+Zip file size: 21070 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 00:15 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      315 b- defN 23-Jun-07 00:14 sqlite_path/__init__.py
+-rw-rw-rw-  2.0 fat    63330 b- defN 23-Jun-07 00:15 sqlite_path/path0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-07 00:14 sqlite_path/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-07 00:15 sqlite_path-0.2.0a2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-07 00:15 sqlite_path-0.2.0a2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-07 00:15 sqlite_path-0.2.0a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      635 b- defN 23-Jun-07 00:15 sqlite_path-0.2.0a2.dist-info/RECORD
+8 files, 64995 bytes uncompressed, 19956 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_path/path0.dll
 Comment: 
 
 Filename: sqlite_path/version.py
 Comment: 
 
-Filename: sqlite_path-0.2.0a1.dist-info/METADATA
+Filename: sqlite_path-0.2.0a2.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_path-0.2.0a1.dist-info/WHEEL
+Filename: sqlite_path-0.2.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_path-0.2.0a1.dist-info/top_level.txt
+Filename: sqlite_path-0.2.0a2.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_path-0.2.0a1.dist-info/RECORD
+Filename: sqlite_path-0.2.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_path/path0.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 28 00:04:23 2023
+Time/Date		Wed Jun  7 00:14:20 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	37
 SizeOfCode		0000000000005400
 SizeOfInitializedData	0000000000007e00
 SizeOfUninitializedData	0000000000000200
 AddressOfEntryPoint	0000000000001290
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00018000
 SizeOfHeaders		00000600
-CheckSum		0001de10
+CheckSum		0001e17b
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
@@ -111,15 +111,15 @@
  0000e028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x2e05fd000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		64222f07
+Time/Date stamp 		647fcbdc
 Major/Minor 			0/0
 Name 				000000000000d032 path0.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000001
 	[Name Pointer/Ordinal] Table	00000001
 Table Addresses
@@ -8152,38 +8152,37 @@
 	...
 
 00000002e05f8050 <.rdata>:
    2e05f8050:	jbe    2e05f8082 <.rdata+0x32>
    2e05f8052:	cs xor (%rsi),%ch
    2e05f8055:	xor    %ch,0x68706c61(%rip)        # 348cfecbc <.debug_line_str+0x686f7c72>
    2e05f805b:	(bad)
-   2e05f805c:	cs xor %eax,(%rax)
-   2e05f805f:	add    %ah,0x30(%rbp)
-   2e05f8062:	(bad)
-   2e05f8063:	cmp    %esi,(%rcx)
-   2e05f8065:	xor    $0x62,%al
-   2e05f8067:	movsxd 0x63(%rax,%rdi,1),%esp
-   2e05f806b:	cmp    %esp,0x65(%rsi)
-   2e05f806e:	gs xor $0x31,%al
-   2e05f8071:	xor    %dh,(%rcx,%riz,2)
-   2e05f8074:	(bad)
-   2e05f8075:	cmp    %esp,0x32(%rcx)
-   2e05f8078:	xor    %dh,%fs:(%rbx)
-   2e05f807b:	(bad)
-   2e05f807c:	xor    %esi,(%rdi)
-   2e05f807e:	xor    $0x39643032,%eax
-   2e05f8083:	xor    $0x36,%al
-   2e05f8085:	ss (bad)
-   2e05f8087:	ss add %dh,(%rdx)
-   2e05f808a:	xor    %dh,(%rdx)
-   2e05f808c:	xor    0x322d3330(%rip),%ebp        # 3128cb3c2 <.debug_line_str+0x322c4378>
-   2e05f8092:	cmp    %dl,0x30(%rax,%rsi,1)
-   2e05f8096:	cmp    (%rax),%dh
+   2e05f805c:	cs xor (%rax),%al
+   2e05f805f:	add    %dh,(%rsi)
+   2e05f8061:	xor    $0x66616538,%eax
+   2e05f8066:	xor    $0x65,%al
+   2e05f8068:	(bad)
+   2e05f8069:	xor    %esp,0x31(%rbx)
+   2e05f806c:	xor    $0x30393535,%eax
+   2e05f8071:	cmp    %sp,%gs:0x62(%rbx)
+   2e05f8076:	xor    0x32(%rbp),%esp
+   2e05f8079:	gs cmp %esp,%fs:0x31(%rdx)
+   2e05f807e:	cmp    %esp,%gs:0x35(%rbp)
+   2e05f8082:	xor    0x63(%rcx),%esp
+   2e05f8085:	cmp    %dh,(%rsi)
+   2e05f8087:	xor    %eax,(%rax)
+   2e05f8089:	xor    (%rax),%dh
+   2e05f808b:	xor    (%rbx),%dh
+   2e05f808d:	sub    $0x302d3630,%eax
+   2e05f8092:	(bad)
+   2e05f8093:	push   %rsp
+   2e05f8094:	xor    %dh,(%rax)
+   2e05f8096:	cmp    (%rcx),%dh
    2e05f8098:	xor    $0x3a,%al
-   2e05f809a:	xor    %bh,(%rcx)
+   2e05f809a:	xor    %bh,(%rax)
    2e05f809c:	pop    %rdx
    2e05f809d:	sub    (%rax),%esi
    2e05f809f:	xor    %dh,(%rax)
    2e05f80a1:	xor    %al,(%rax)
    2e05f80a3:	add    %al,(%rax)
    2e05f80a5:	add    %al,(%rax)
    2e05f80a7:	add    %dl,0x65(%rsi)
@@ -10369,17 +10368,17 @@
 	...
 
 Disassembly of section .edata:
 
 00000002e05fd000 <.edata>:
    2e05fd000:	add    %al,(%rax)
    2e05fd002:	add    %al,(%rax)
-   2e05fd004:	(bad)
-   2e05fd005:	(bad)
-   2e05fd006:	and    0x0(%rax,%rax,1),%ah
+   2e05fd004:	fmul   %st,%st(3)
+   2e05fd006:	jg     2e05fd06c <__bss_end__+0xeec>
+   2e05fd008:	add    %al,(%rax)
    2e05fd00a:	add    %al,(%rax)
    2e05fd00c:	xor    %al,%dl
    2e05fd00e:	add    %al,(%rax)
    2e05fd010:	add    %eax,(%rax)
    2e05fd012:	add    %al,(%rax)
    2e05fd014:	add    %eax,(%rax)
    2e05fd016:	add    %al,(%rax)
```

## sqlite_path/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.0-alpha.1"
+__version__ = "0.2.0-alpha.2"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_path-0.2.0a1.dist-info/METADATA` & `sqlite_path-0.2.0a2.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-path
-Version: 0.2.0a1
+Version: 0.2.0a2
 Home-page: https://github.com/asg017/sqlite-path
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-path/issues
 Project-URL: CI, https://github.com/asg017/sqlite-path/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-path/releases
 Requires-Python: >=3.7
```

