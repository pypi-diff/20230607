# Comparing `tmp/sqlite_jsonschema-0.2.3a2-py3-none-win_amd64.whl.zip` & `tmp/sqlite_jsonschema-0.2.3a3-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1560643 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 17:45 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      327 b- defN 23-Jun-07 17:44 sqlite_jsonschema/__init__.py
--rw-rw-rw-  2.0 fat  3678720 b- defN 23-Jun-07 17:45 sqlite_jsonschema/jsonschema0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-07 17:44 sqlite_jsonschema/version.py
--rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-07 17:45 sqlite_jsonschema-0.2.3a2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-07 17:45 sqlite_jsonschema-0.2.3a2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 17:45 sqlite_jsonschema-0.2.3a2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      685 b- defN 23-Jun-07 17:45 sqlite_jsonschema-0.2.3a2.dist-info/RECORD
-8 files, 3680483 bytes uncompressed, 1559433 bytes compressed:  57.6%
+Zip file size: 1560657 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-07 18:10 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      327 b- defN 23-Jun-07 18:09 sqlite_jsonschema/__init__.py
+-rw-rw-rw-  2.0 fat  3678720 b- defN 23-Jun-07 18:09 sqlite_jsonschema/jsonschema0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-07 18:09 sqlite_jsonschema/version.py
+-rw-rw-rw-  2.0 fat      545 b- defN 23-Jun-07 18:10 sqlite_jsonschema-0.2.3a3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-07 18:10 sqlite_jsonschema-0.2.3a3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-07 18:10 sqlite_jsonschema-0.2.3a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      685 b- defN 23-Jun-07 18:10 sqlite_jsonschema-0.2.3a3.dist-info/RECORD
+8 files, 3680483 bytes uncompressed, 1559447 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_jsonschema/jsonschema0.dll
 Comment: 
 
 Filename: sqlite_jsonschema/version.py
 Comment: 
 
-Filename: sqlite_jsonschema-0.2.3a2.dist-info/METADATA
+Filename: sqlite_jsonschema-0.2.3a3.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_jsonschema-0.2.3a2.dist-info/WHEEL
+Filename: sqlite_jsonschema-0.2.3a3.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_jsonschema-0.2.3a2.dist-info/top_level.txt
+Filename: sqlite_jsonschema-0.2.3a3.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_jsonschema-0.2.3a2.dist-info/RECORD
+Filename: sqlite_jsonschema-0.2.3a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_jsonschema/jsonschema0.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802528f8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Jun  7 17:44:27 2023
+Time/Date		Wed Jun  7 18:08:41 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	36
 SizeOfCode		000000000025c000
 SizeOfInitializedData	0000000000126c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002528f8
@@ -296,17 +296,17 @@
  00000001803650cc:	00000001800025f0 0000000180002703 0000000180318e10
  00000001803650d8:	0000000180002710 000000018000275b 0000000180318e24
  00000001803650e4:	0000000180002760 000000018000278d 0000000180318e38
  00000001803650f0:	0000000180002790 00000001800027f7 0000000180318e88
  00000001803650fc:	0000000180002800 0000000180002830 0000000180318e9c
  0000000180365108:	0000000180002830 00000001800028b9 0000000180318ef0
  0000000180365114:	00000001800028c0 00000001800028e0 0000000180318f04
- 0000000180365120:	00000001800028f0 0000000180002983 0000000180318f58
- 000000018036512c:	0000000180002990 00000001800029de 0000000180318f70
- 0000000180365138:	00000001800029e0 0000000180002a5e 0000000180318fc4
+ 0000000180365120:	00000001800028f0 000000018000296e 0000000180318f58
+ 000000018036512c:	0000000180002970 00000001800029be 0000000180318f70
+ 0000000180365138:	00000001800029c0 0000000180002a53 0000000180318fc4
  0000000180365144:	0000000180002a60 0000000180002aae 0000000180318fdc
  0000000180365150:	0000000180002ab0 0000000180002b84 0000000180319030
  000000018036515c:	0000000180002b90 0000000180002bb2 0000000180319048
  0000000180365168:	0000000180002bc0 0000000180002bfb 0000000180319054
  0000000180365174:	0000000180002c00 0000000180002d27 00000001803190b8
  0000000180365180:	0000000180002d30 0000000180002d72 00000001803190d4
  000000018036518c:	0000000180002db0 0000000180002e1f 0000000180319194
@@ -339,24 +339,24 @@
  00000001803652d0:	0000000180004b50 0000000180004b72 0000000180319748
  00000001803652dc:	0000000180004b80 0000000180004bcc 0000000180319798
  00000001803652e8:	0000000180004bd0 0000000180004bf2 00000001803197ac
  00000001803652f4:	0000000180004c00 0000000180004c9b 00000001803197fc
  0000000180365300:	0000000180004ca0 0000000180004cd9 0000000180319810
  000000018036530c:	0000000180004ce0 0000000180004d26 0000000180319864
  0000000180365318:	0000000180004d30 0000000180004d4e 0000000180319878
- 0000000180365324:	0000000180004d80 0000000180004f41 0000000180319300
- 0000000180365330:	0000000180004f50 00000001800050de 00000001803198c8
+ 0000000180365324:	0000000180004d80 0000000180004f0e 00000001803198c8
+ 0000000180365330:	0000000180004f10 00000001800050d1 0000000180319300
  000000018036533c:	00000001800050e0 0000000180005169 00000001803198d4
  0000000180365348:	0000000180005170 0000000180005232 00000001803198e0
- 0000000180365354:	0000000180005240 0000000180005386 00000001803198ec
- 0000000180365360:	0000000180005390 00000001800053b9 0000000180319904
- 000000018036536c:	00000001800053c0 00000001800054f7 0000000180319958
- 0000000180365378:	0000000180005500 0000000180005529 0000000180319970
- 0000000180365384:	0000000180005530 000000018000561f 00000001803199c4
- 0000000180365390:	0000000180005620 0000000180005648 00000001803199dc
+ 0000000180365354:	0000000180005240 000000018000532f 00000001803198ec
+ 0000000180365360:	0000000180005330 0000000180005358 0000000180319904
+ 000000018036536c:	0000000180005360 0000000180005497 000000018031995c
+ 0000000180365378:	00000001800054a0 00000001800054c9 0000000180319974
+ 0000000180365384:	00000001800054d0 0000000180005616 00000001803199c8
+ 0000000180365390:	0000000180005620 0000000180005649 00000001803199e0
  000000018036539c:	0000000180005650 000000018000573f 0000000180319a34
  00000001803653a8:	0000000180005740 000000018000576b 0000000180319a50
  00000001803653b4:	0000000180005770 000000018000585f 0000000180319aa8
  00000001803653c0:	0000000180005860 000000018000588b 0000000180319ac4
  00000001803653cc:	0000000180005890 000000018000597f 0000000180319b1c
  00000001803653d8:	0000000180005980 00000001800059ab 0000000180319b38
  00000001803653e4:	00000001800059d0 0000000180005a1a 0000000180319b90
@@ -385,19 +385,19 @@
  00000001803654f8:	00000001800069a0 00000001800069d6 0000000180319f30
  0000000180365504:	00000001800069e0 0000000180006a23 0000000180319f44
  0000000180365510:	0000000180006a30 0000000180006a6d 0000000180319f58
  000000018036551c:	0000000180006a70 0000000180006aaf 0000000180319f6c
  0000000180365528:	0000000180006ab0 0000000180006aef 0000000180319f80
  0000000180365534:	0000000180006af0 0000000180006b23 0000000180319f94
  0000000180365540:	0000000180006b30 0000000180006b66 0000000180319fa8
- 000000018036554c:	0000000180006c00 0000000180006d2f 000000018031a0cc
- 0000000180365558:	0000000180006d30 0000000180006d69 000000018031a0e0
- 0000000180365564:	0000000180006d70 0000000180006d97 000000018031a0ec
- 0000000180365570:	0000000180006da0 0000000180006e43 000000018031a150
- 000000018036557c:	0000000180006e50 0000000180006e70 000000018031a164
+ 000000018036554c:	0000000180006c00 0000000180006ca3 000000018031a0cc
+ 0000000180365558:	0000000180006cb0 0000000180006cd0 000000018031a0e0
+ 0000000180365564:	0000000180006cd0 0000000180006dff 000000018031a134
+ 0000000180365570:	0000000180006e00 0000000180006e39 000000018031a148
+ 000000018036557c:	0000000180006e40 0000000180006e67 000000018031a154
  0000000180365588:	0000000180006e70 0000000180006edb 00000001803198d4
  0000000180365594:	0000000180006ee0 00000001800071ce 000000018031a1b8
  00000001803655a0:	00000001800071d0 00000001800071fc 000000018031a1d4
  00000001803655ac:	0000000180007200 00000001800073fd 000000018031a230
  00000001803655b8:	0000000180007400 00000001800077de 000000018031a248
  00000001803655c4:	00000001800077e0 0000000180007817 000000018031a26c
  00000001803655d0:	0000000180007820 0000000180007857 000000018031a284
@@ -9336,39 +9336,39 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 38 8f 31 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 40 8f 31 00 30 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff c0 28 00 00
 	  030: 30 28 00 00 ff ff ff ff 65 28 00 00 00 00 00 00
 	  040: 6e 28 00 00 ff ff ff ff
- 0000000180318f58 (rva: 00318f58): 00000001800028f0 - 0000000180002983
+ 0000000180318f58 (rva: 00318f58): 00000001800028f0 - 000000018000296e
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 5, Prologue size: 0x0c, Frame offset: 0x4, Frame reg: rbp
 	  pc+0x0c: FPReg: rbp = rsp + 0x40 (info = 0x0)
 	  pc+0x07: alloc small area: rsp = rsp - 0x40
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001802534f5.
 	User data:
 	  000: 7c 8f 31 00
- 0000000180318f70 (rva: 00318f70): 0000000180002990 - 00000001800029de
+ 0000000180318f70 (rva: 00318f70): 0000000180002970 - 00000001800029be
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x10, Frame offset: 0x0, Frame reg: none
 	  pc+0x0c: alloc small area: rsp = rsp - 0x20
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 a4 8f 31 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 ac 8f 31 00 38 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 90 29 00 00
-	  030: f0 28 00 00 ff ff ff ff 56 29 00 00 00 00 00 00
-	  040: 5c 29 00 00 ff ff ff ff
- 0000000180318fc4 (rva: 00318fc4): 00000001800029e0 - 0000000180002a5e
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 70 29 00 00
+	  030: f0 28 00 00 ff ff ff ff 42 29 00 00 00 00 00 00
+	  040: 44 29 00 00 ff ff ff ff
+ 0000000180318fc4 (rva: 00318fc4): 00000001800029c0 - 0000000180002a53
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 5, Prologue size: 0x0c, Frame offset: 0x4, Frame reg: rbp
 	  pc+0x0c: FPReg: rbp = rsp + 0x40 (info = 0x0)
 	  pc+0x07: alloc small area: rsp = rsp - 0x40
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
@@ -9382,16 +9382,16 @@
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 10 90 31 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 18 90 31 00 38 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 60 2a 00 00
-	  030: e0 29 00 00 ff ff ff ff 32 2a 00 00 00 00 00 00
-	  040: 34 2a 00 00 ff ff ff ff
+	  030: c0 29 00 00 ff ff ff ff 26 2a 00 00 00 00 00 00
+	  040: 2c 2a 00 00 ff ff ff ff
  0000000180319030 (rva: 00319030): 0000000180002ab0 - 0000000180002b84
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 5, Prologue size: 0x0c, Frame offset: 0x5, Frame reg: rbp
 	  pc+0x0c: FPReg: rbp = rsp + 0x50 (info = 0x0)
 	  pc+0x07: alloc small area: rsp = rsp - 0x50
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
@@ -9854,116 +9854,116 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 a8 98 31 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 b0 98 31 00 28 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 30 4d 00 00
 	  030: e0 4c 00 00 ff ff ff ff f3 4c 00 00 00 00 00 00
 	  040: fc 4c 00 00 ff ff ff ff
- 0000000180319300 (rva: 00319300): 0000000180004d80 - 0000000180004f41
+ 00000001803198c8 (rva: 003198c8): 0000000180004d80 - 0000000180004f0e
+	Version: 1, Flags: none
+	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
+	  pc+0x06: alloc small area: rsp = rsp - 0x38
+	  pc+0x02: push rdi
+	  pc+0x01: push rsi
+ 0000000180319300 (rva: 00319300): 0000000180004f10 - 00000001800050d1
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0b, Frame offset: 0x0, Frame reg: none
 	  pc+0x0b: alloc small area: rsp = rsp - 0x40
 	  pc+0x07: push rbx
 	  pc+0x06: push rdi
 	  pc+0x05: push rsi
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000001803198c8 (rva: 003198c8): 0000000180004f50 - 00000001800050de
-	Version: 1, Flags: none
-	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
-	  pc+0x06: alloc small area: rsp = rsp - 0x38
-	  pc+0x02: push rdi
-	  pc+0x01: push rsi
  00000001803198d4 (rva: 003198d4): 00000001800050e0 - 0000000180005169
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rdi
 	  pc+0x01: push rsi
  00000001803198e0 (rva: 003198e0): 0000000180005170 - 0000000180005232
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x58
 	  pc+0x02: push rdi
 	  pc+0x01: push rsi
- 00000001803198ec (rva: 003198ec): 0000000180005240 - 0000000180005386
+ 00000001803198ec (rva: 003198ec): 0000000180005240 - 000000018000532f
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
-	Nbr codes: 6, Prologue size: 0x12, Frame offset: 0x8, Frame reg: rbp
-	  pc+0x12: FPReg: rbp = rsp + 0x80 (info = 0x0)
-	  pc+0x0a: alloc large area: rsp = rsp - 0xa0
+	Nbr codes: 6, Prologue size: 0x0d, Frame offset: 0x4, Frame reg: rbp
+	  pc+0x0d: FPReg: rbp = rsp + 0x40 (info = 0x0)
+	  pc+0x08: alloc small area: rsp = rsp - 0x48
+	  pc+0x04: push rbx
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001802534f5.
 	User data:
-	  000: 10 99 31 00
- 0000000180319904 (rva: 00319904): 0000000180005390 - 00000001800053b9
+	  000: 14 99 31 00
+ 0000000180319904 (rva: 00319904): 0000000180005330 - 0000000180005358
 	Version: 1, Flags: none
-	Nbr codes: 4, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
-	  pc+0x0c: alloc small area: rsp = rsp - 0x20
+	Nbr codes: 5, Prologue size: 0x11, Frame offset: 0x0, Frame reg: none
+	  pc+0x0d: alloc small area: rsp = rsp - 0x28
+	  pc+0x09: push rbx
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
-	  000: 22 05 93 19 01 00 00 00 38 99 31 00 00 00 00 00
-	  010: 00 00 00 00 03 00 00 00 40 99 31 00 98 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 90 53 00 00
-	  030: 40 52 00 00 ff ff ff ff eb 52 00 00 00 00 00 00
-	  040: f7 52 00 00 ff ff ff ff
- 0000000180319958 (rva: 00319958): 00000001800053c0 - 00000001800054f7
+	  000: 22 05 93 19 01 00 00 00 3c 99 31 00 00 00 00 00
+	  010: 00 00 00 00 03 00 00 00 44 99 31 00 40 00 00 00
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 30 53 00 00
+	  030: 40 52 00 00 ff ff ff ff 8e 52 00 00 00 00 00 00
+	  040: 9a 52 00 00 ff ff ff ff
+ 000000018031995c (rva: 0031995c): 0000000180005360 - 0000000180005497
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x12, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x12: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x0a: alloc large area: rsp = rsp - 0x90
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001802534f5.
 	User data:
-	  000: 7c 99 31 00
- 0000000180319970 (rva: 00319970): 0000000180005500 - 0000000180005529
+	  000: 80 99 31 00
+ 0000000180319974 (rva: 00319974): 00000001800054a0 - 00000001800054c9
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x0c: alloc small area: rsp = rsp - 0x20
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
-	  000: 22 05 93 19 01 00 00 00 a4 99 31 00 00 00 00 00
-	  010: 00 00 00 00 03 00 00 00 ac 99 31 00 88 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 00 55 00 00
-	  030: c0 53 00 00 ff ff ff ff 5c 54 00 00 00 00 00 00
-	  040: 68 54 00 00 ff ff ff ff
- 00000001803199c4 (rva: 003199c4): 0000000180005530 - 000000018000561f
+	  000: 22 05 93 19 01 00 00 00 a8 99 31 00 00 00 00 00
+	  010: 00 00 00 00 03 00 00 00 b0 99 31 00 88 00 00 00
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff a0 54 00 00
+	  030: 60 53 00 00 ff ff ff ff fc 53 00 00 00 00 00 00
+	  040: 08 54 00 00 ff ff ff ff
+ 00000001803199c8 (rva: 003199c8): 00000001800054d0 - 0000000180005616
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
-	Nbr codes: 6, Prologue size: 0x0d, Frame offset: 0x4, Frame reg: rbp
-	  pc+0x0d: FPReg: rbp = rsp + 0x40 (info = 0x0)
-	  pc+0x08: alloc small area: rsp = rsp - 0x48
-	  pc+0x04: push rbx
+	Nbr codes: 6, Prologue size: 0x12, Frame offset: 0x8, Frame reg: rbp
+	  pc+0x12: FPReg: rbp = rsp + 0x80 (info = 0x0)
+	  pc+0x0a: alloc large area: rsp = rsp - 0xa0
 	  pc+0x03: push rdi
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001802534f5.
 	User data:
 	  000: ec 99 31 00
- 00000001803199dc (rva: 003199dc): 0000000180005620 - 0000000180005648
+ 00000001803199e0 (rva: 003199e0): 0000000180005620 - 0000000180005649
 	Version: 1, Flags: none
-	Nbr codes: 5, Prologue size: 0x11, Frame offset: 0x0, Frame reg: none
-	  pc+0x0d: alloc small area: rsp = rsp - 0x28
-	  pc+0x09: push rbx
+	Nbr codes: 4, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
+	  pc+0x0c: alloc small area: rsp = rsp - 0x20
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 14 9a 31 00 00 00 00 00
-	  010: 00 00 00 00 03 00 00 00 1c 9a 31 00 40 00 00 00
+	  010: 00 00 00 00 03 00 00 00 1c 9a 31 00 98 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 20 56 00 00
-	  030: 30 55 00 00 ff ff ff ff 7e 55 00 00 00 00 00 00
-	  040: 8a 55 00 00 ff ff ff ff
+	  030: d0 54 00 00 ff ff ff ff 7b 55 00 00 00 00 00 00
+	  040: 87 55 00 00 ff ff ff ff
  0000000180319a34 (rva: 00319a34): 0000000180005650 - 000000018000573f
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 8, Prologue size: 0x15, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x15: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x0d: alloc large area: rsp = rsp - 0x90
 	  pc+0x06: push rbx
 	  pc+0x05: push rdi
@@ -10381,65 +10381,65 @@
 	  0a0: 16 66 00 00 ff ff ff ff 36 66 00 00 03 00 00 00
 	  0b0: 47 66 00 00 01 00 00 00 53 66 00 00 ff ff ff ff
 	  0c0: 0c 67 00 00 04 00 00 00 57 67 00 00 08 00 00 00
 	  0d0: 99 67 00 00 04 00 00 00 12 68 00 00 06 00 00 00
 	  0e0: 41 68 00 00 07 00 00 00 75 68 00 00 04 00 00 00
 	  0f0: ac 68 00 00 05 00 00 00 f0 68 00 00 04 00 00 00
 	  100: 01 69 00 00 02 00 00 00 10 69 00 00 ff ff ff ff
- 000000018031a0cc (rva: 0031a0cc): 0000000180006c00 - 0000000180006d2f
+ 000000018031a0cc (rva: 0031a0cc): 0000000180006c00 - 0000000180006ca3
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x0b, Frame offset: 0x3, Frame reg: rbp
 	  pc+0x0b: FPReg: rbp = rsp + 0x30 (info = 0x0)
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001802534f5.
 	User data:
-	  000: f8 a0 31 00
- 000000018031a0e0 (rva: 0031a0e0): 0000000180006d30 - 0000000180006d69
-	Version: 1, Flags: none
-	Nbr codes: 3, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
-	  pc+0x0b: alloc small area: rsp = rsp - 0x28
-	  pc+0x07: push rsi
-	  pc+0x06: push rbp
- 000000018031a0ec (rva: 0031a0ec): 0000000180006d70 - 0000000180006d97
+	  000: ec a0 31 00
+ 000000018031a0e0 (rva: 0031a0e0): 0000000180006cb0 - 0000000180006cd0
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0b: alloc small area: rsp = rsp - 0x28
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
-	  000: 22 05 93 19 02 00 00 00 20 a1 31 00 00 00 00 00
-	  010: 00 00 00 00 04 00 00 00 30 a1 31 00 30 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 70 6d 00 00
-	  030: 00 00 00 00 30 6d 00 00 00 6c 00 00 ff ff ff ff
-	  040: 3b 6c 00 00 01 00 00 00 b8 6c 00 00 00 00 00 00
-	  050: bd 6c 00 00 ff ff ff ff
- 000000018031a150 (rva: 0031a150): 0000000180006da0 - 0000000180006e43
+	  000: 22 05 93 19 01 00 00 00 14 a1 31 00 00 00 00 00
+	  010: 00 00 00 00 03 00 00 00 1c a1 31 00 30 00 00 00
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff b0 6c 00 00
+	  030: 00 6c 00 00 ff ff ff ff 2f 6c 00 00 00 00 00 00
+	  040: 38 6c 00 00 ff ff ff ff
+ 000000018031a134 (rva: 0031a134): 0000000180006cd0 - 0000000180006dff
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x0b, Frame offset: 0x3, Frame reg: rbp
 	  pc+0x0b: FPReg: rbp = rsp + 0x30 (info = 0x0)
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 00000001802534f5.
 	User data:
-	  000: 70 a1 31 00
- 000000018031a164 (rva: 0031a164): 0000000180006e50 - 0000000180006e70
+	  000: 60 a1 31 00
+ 000000018031a148 (rva: 0031a148): 0000000180006e00 - 0000000180006e39
+	Version: 1, Flags: none
+	Nbr codes: 3, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
+	  pc+0x0b: alloc small area: rsp = rsp - 0x28
+	  pc+0x07: push rsi
+	  pc+0x06: push rbp
+ 000000018031a154 (rva: 0031a154): 0000000180006e40 - 0000000180006e67
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0b: alloc small area: rsp = rsp - 0x28
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
-	  000: 22 05 93 19 01 00 00 00 98 a1 31 00 00 00 00 00
-	  010: 00 00 00 00 03 00 00 00 a0 a1 31 00 30 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 50 6e 00 00
-	  030: a0 6d 00 00 ff ff ff ff cf 6d 00 00 00 00 00 00
-	  040: d8 6d 00 00 ff ff ff ff
+	  000: 22 05 93 19 02 00 00 00 88 a1 31 00 00 00 00 00
+	  010: 00 00 00 00 04 00 00 00 98 a1 31 00 30 00 00 00
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 40 6e 00 00
+	  030: 00 00 00 00 00 6e 00 00 d0 6c 00 00 ff ff ff ff
+	  040: 0b 6d 00 00 01 00 00 00 88 6d 00 00 00 00 00 00
+	  050: 8d 6d 00 00 ff ff ff ff
  00000001803198d4 (rva: 003198d4): 0000000180006e70 - 0000000180006edb
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rdi
 	  pc+0x01: push rsi
@@ -108674,15 +108674,15 @@
 	reloc   50 offset  8b8 [3638b8] DIR64
 	reloc   51 offset  908 [363908] DIR64
 
 There is a debug directory in .rdata at 0x180318380
 
 Type                Size     Rva      Offset
   2        CodeView 0000006b 00318620 00317a20
-(format RSDS signature 765bb4e191d74f2eae89ec7630096478 age 1 pdb D:\a\sqlite-jsonschema\sqlite-jsonschema\target\release\deps\sqlite_jsonschema.pdb)
+(format RSDS signature e996a8b17a85441fabae4244aa02bf23 age 1 pdb D:\a\sqlite-jsonschema\sqlite-jsonschema\target\release\deps\sqlite_jsonschema.pdb)
  12         Feature 00000014 0031868c 00317a8c
  13         CoffGrp 00000318 003186a0 00317aa0
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
   0 .text         0025be57  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
@@ -110134,15 +110134,15 @@
    180002699:	call   0x180007910
    18000269e:	dec    %r14
    1800026a1:	mov    -0x8(%rbx),%rax
    1800026a5:	lock decq (%rax)
    1800026a9:	jne    0x180002630
    1800026ab:	add    $0xfffffffffffffff8,%rbx
    1800026af:	mov    %rbx,%rcx
-   1800026b2:	call   0x180006da0
+   1800026b2:	call   0x180006c00
    1800026b7:	jmp    0x180002630
    1800026bc:	mov    %rsi,%rax
    1800026bf:	shl    $0x5,%rax
    1800026c3:	add    %rax,%rsi
    1800026c6:	add    $0x31,%rsi
    1800026ca:	je     0x1800026f3
    1800026cc:	mov    0x18(%rdi),%rcx
@@ -110341,121 +110341,121 @@
    1800028f1:	push   %rsi
    1800028f2:	push   %rdi
    1800028f3:	sub    $0x40,%rsp
    1800028f7:	lea    0x40(%rsp),%rbp
    1800028fc:	movq   $0xfffffffffffffffe,-0x8(%rbp)
    180002904:	mov    0x10(%rcx),%rax
    180002908:	test   %rax,%rax
-   18000290b:	je     0x18000297b
+   18000290b:	je     0x180002966
    18000290d:	mov    0x8(%rcx),%rsi
-   180002911:	add    $0x28,%rsi
+   180002911:	add    $0x10,%rsi
    180002915:	mov    $0x1,%ecx
    18000291a:	sub    %rax,%rcx
    18000291d:	jmp    0x180002931
    18000291f:	nop
-   180002920:	add    $0x28,%rsi
+   180002920:	add    $0x10,%rsi
    180002924:	mov    -0x18(%rbp),%rcx
    180002928:	inc    %rcx
    18000292b:	cmp    $0x1,%rcx
-   18000292f:	je     0x18000297b
-   180002931:	mov    %rcx,-0x18(%rbp)
-   180002935:	mov    -0x28(%rsi),%rdx
-   180002939:	test   %rdx,%rdx
-   18000293c:	je     0x18000294d
-   18000293e:	mov    -0x20(%rsi),%rcx
-   180002942:	mov    $0x1,%r8d
-   180002948:	call   0x180007910
-   18000294d:	mov    -0x10(%rsi),%rcx
-   180002951:	mov    -0x8(%rsi),%rax
-   180002955:	mov    %rsi,-0x10(%rbp)
-   180002959:	call   *(%rax)
-   18000295b:	mov    -0x10(%rbp),%rsi
-   18000295f:	mov    -0x8(%rsi),%rax
-   180002963:	mov    0x8(%rax),%rdx
-   180002967:	test   %rdx,%rdx
-   18000296a:	je     0x180002920
-   18000296c:	mov    0x10(%rax),%r8
-   180002970:	mov    -0x10(%rsi),%rcx
-   180002974:	call   0x180007910
-   180002979:	jmp    0x180002920
-   18000297b:	add    $0x40,%rsp
-   18000297f:	pop    %rdi
-   180002980:	pop    %rsi
-   180002981:	pop    %rbp
-   180002982:	ret
-   180002983:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180002990:	mov    %rdx,0x10(%rsp)
-   180002995:	push   %rbp
-   180002996:	push   %rsi
-   180002997:	push   %rdi
-   180002998:	sub    $0x20,%rsp
-   18000299c:	lea    0x40(%rdx),%rbp
-   1800029a0:	mov    -0x10(%rbp),%rsi
-   1800029a4:	mov    -0x10(%rsi),%rcx
-   1800029a8:	mov    -0x8(%rsi),%rax
-   1800029ac:	mov    0x8(%rax),%rdx
-   1800029b0:	mov    0x10(%rax),%r8
-   1800029b4:	call   0x1800028e0
-   1800029b9:	mov    -0x18(%rbp),%rdi
-   1800029bd:	test   %rdi,%rdi
-   1800029c0:	je     0x1800029d6
-   1800029c2:	neg    %rdi
-   1800029c5:	mov    %rsi,%rcx
-   1800029c8:	call   0x180002790
-   1800029cd:	add    $0x28,%rsi
-   1800029d1:	dec    %rdi
-   1800029d4:	jne    0x1800029c5
-   1800029d6:	add    $0x20,%rsp
-   1800029da:	pop    %rdi
-   1800029db:	pop    %rsi
-   1800029dc:	pop    %rbp
-   1800029dd:	ret
-   1800029de:	int3
-   1800029df:	int3
-   1800029e0:	push   %rbp
-   1800029e1:	push   %rsi
-   1800029e2:	push   %rdi
-   1800029e3:	sub    $0x40,%rsp
-   1800029e7:	lea    0x40(%rsp),%rbp
-   1800029ec:	movq   $0xfffffffffffffffe,-0x8(%rbp)
-   1800029f4:	mov    0x10(%rcx),%rax
-   1800029f8:	test   %rax,%rax
-   1800029fb:	je     0x180002a56
-   1800029fd:	mov    0x8(%rcx),%rsi
-   180002a01:	add    $0x10,%rsi
-   180002a05:	mov    $0x1,%ecx
-   180002a0a:	sub    %rax,%rcx
-   180002a0d:	jmp    0x180002a21
-   180002a0f:	nop
-   180002a10:	add    $0x10,%rsi
-   180002a14:	mov    -0x18(%rbp),%rcx
-   180002a18:	inc    %rcx
-   180002a1b:	cmp    $0x1,%rcx
-   180002a1f:	je     0x180002a56
-   180002a21:	mov    %rsi,-0x10(%rbp)
-   180002a25:	mov    %rcx,-0x18(%rbp)
-   180002a29:	mov    -0x10(%rsi),%rcx
-   180002a2d:	mov    -0x8(%rsi),%rax
-   180002a31:	call   *(%rax)
-   180002a33:	mov    -0x10(%rbp),%rcx
-   180002a37:	mov    -0x8(%rcx),%rax
-   180002a3b:	mov    0x8(%rax),%rdx
-   180002a3f:	test   %rdx,%rdx
-   180002a42:	mov    %rcx,%rsi
-   180002a45:	je     0x180002a10
-   180002a47:	mov    0x10(%rax),%r8
-   180002a4b:	mov    -0x10(%rsi),%rcx
-   180002a4f:	call   0x180007910
-   180002a54:	jmp    0x180002a10
-   180002a56:	add    $0x40,%rsp
-   180002a5a:	pop    %rdi
-   180002a5b:	pop    %rsi
-   180002a5c:	pop    %rbp
-   180002a5d:	ret
-   180002a5e:	xchg   %ax,%ax
+   18000292f:	je     0x180002966
+   180002931:	mov    %rsi,-0x10(%rbp)
+   180002935:	mov    %rcx,-0x18(%rbp)
+   180002939:	mov    -0x10(%rsi),%rcx
+   18000293d:	mov    -0x8(%rsi),%rax
+   180002941:	call   *(%rax)
+   180002943:	mov    -0x10(%rbp),%rcx
+   180002947:	mov    -0x8(%rcx),%rax
+   18000294b:	mov    0x8(%rax),%rdx
+   18000294f:	test   %rdx,%rdx
+   180002952:	mov    %rcx,%rsi
+   180002955:	je     0x180002920
+   180002957:	mov    0x10(%rax),%r8
+   18000295b:	mov    -0x10(%rsi),%rcx
+   18000295f:	call   0x180007910
+   180002964:	jmp    0x180002920
+   180002966:	add    $0x40,%rsp
+   18000296a:	pop    %rdi
+   18000296b:	pop    %rsi
+   18000296c:	pop    %rbp
+   18000296d:	ret
+   18000296e:	xchg   %ax,%ax
+   180002970:	mov    %rdx,0x10(%rsp)
+   180002975:	push   %rbp
+   180002976:	push   %rsi
+   180002977:	push   %rdi
+   180002978:	sub    $0x20,%rsp
+   18000297c:	lea    0x40(%rdx),%rbp
+   180002980:	mov    -0x10(%rbp),%rsi
+   180002984:	mov    -0x10(%rsi),%rcx
+   180002988:	mov    -0x8(%rsi),%rax
+   18000298c:	mov    0x8(%rax),%rdx
+   180002990:	mov    0x10(%rax),%r8
+   180002994:	call   0x1800028e0
+   180002999:	mov    -0x18(%rbp),%rdi
+   18000299d:	test   %rdi,%rdi
+   1800029a0:	je     0x1800029b6
+   1800029a2:	neg    %rdi
+   1800029a5:	mov    %rsi,%rcx
+   1800029a8:	call   0x180002710
+   1800029ad:	add    $0x10,%rsi
+   1800029b1:	dec    %rdi
+   1800029b4:	jne    0x1800029a5
+   1800029b6:	add    $0x20,%rsp
+   1800029ba:	pop    %rdi
+   1800029bb:	pop    %rsi
+   1800029bc:	pop    %rbp
+   1800029bd:	ret
+   1800029be:	int3
+   1800029bf:	int3
+   1800029c0:	push   %rbp
+   1800029c1:	push   %rsi
+   1800029c2:	push   %rdi
+   1800029c3:	sub    $0x40,%rsp
+   1800029c7:	lea    0x40(%rsp),%rbp
+   1800029cc:	movq   $0xfffffffffffffffe,-0x8(%rbp)
+   1800029d4:	mov    0x10(%rcx),%rax
+   1800029d8:	test   %rax,%rax
+   1800029db:	je     0x180002a4b
+   1800029dd:	mov    0x8(%rcx),%rsi
+   1800029e1:	add    $0x28,%rsi
+   1800029e5:	mov    $0x1,%ecx
+   1800029ea:	sub    %rax,%rcx
+   1800029ed:	jmp    0x180002a01
+   1800029ef:	nop
+   1800029f0:	add    $0x28,%rsi
+   1800029f4:	mov    -0x18(%rbp),%rcx
+   1800029f8:	inc    %rcx
+   1800029fb:	cmp    $0x1,%rcx
+   1800029ff:	je     0x180002a4b
+   180002a01:	mov    %rcx,-0x18(%rbp)
+   180002a05:	mov    -0x28(%rsi),%rdx
+   180002a09:	test   %rdx,%rdx
+   180002a0c:	je     0x180002a1d
+   180002a0e:	mov    -0x20(%rsi),%rcx
+   180002a12:	mov    $0x1,%r8d
+   180002a18:	call   0x180007910
+   180002a1d:	mov    -0x10(%rsi),%rcx
+   180002a21:	mov    -0x8(%rsi),%rax
+   180002a25:	mov    %rsi,-0x10(%rbp)
+   180002a29:	call   *(%rax)
+   180002a2b:	mov    -0x10(%rbp),%rsi
+   180002a2f:	mov    -0x8(%rsi),%rax
+   180002a33:	mov    0x8(%rax),%rdx
+   180002a37:	test   %rdx,%rdx
+   180002a3a:	je     0x1800029f0
+   180002a3c:	mov    0x10(%rax),%r8
+   180002a40:	mov    -0x10(%rsi),%rcx
+   180002a44:	call   0x180007910
+   180002a49:	jmp    0x1800029f0
+   180002a4b:	add    $0x40,%rsp
+   180002a4f:	pop    %rdi
+   180002a50:	pop    %rsi
+   180002a51:	pop    %rbp
+   180002a52:	ret
+   180002a53:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
    180002a60:	mov    %rdx,0x10(%rsp)
    180002a65:	push   %rbp
    180002a66:	push   %rsi
    180002a67:	push   %rdi
    180002a68:	sub    $0x20,%rsp
    180002a6c:	lea    0x40(%rdx),%rbp
    180002a70:	mov    -0x10(%rbp),%rsi
@@ -110465,16 +110465,16 @@
    180002a80:	mov    0x10(%rax),%r8
    180002a84:	call   0x1800028e0
    180002a89:	mov    -0x18(%rbp),%rdi
    180002a8d:	test   %rdi,%rdi
    180002a90:	je     0x180002aa6
    180002a92:	neg    %rdi
    180002a95:	mov    %rsi,%rcx
-   180002a98:	call   0x180002710
-   180002a9d:	add    $0x10,%rsi
+   180002a98:	call   0x180002790
+   180002a9d:	add    $0x28,%rsi
    180002aa1:	dec    %rdi
    180002aa4:	jne    0x180002a95
    180002aa6:	add    $0x20,%rsp
    180002aaa:	pop    %rdi
    180002aab:	pop    %rsi
    180002aac:	pop    %rbp
    180002aad:	ret
@@ -110770,15 +110770,15 @@
    180002e33:	lea    0x80(%rsp),%rbp
    180002e3b:	movq   $0xfffffffffffffffe,0xb0(%rbp)
    180002e46:	mov    %rcx,%rsi
    180002e49:	mov    %rdx,0x70(%rbp)
    180002e4d:	mov    %r8b,0x78(%rbp)
    180002e51:	lea    0x80(%rbp),%rcx
    180002e58:	lea    0x70(%rbp),%rdx
-   180002e5c:	call   0x180004f50
+   180002e5c:	call   0x180004d80
    180002e61:	cmpq   $0x0,0x80(%rbp)
    180002e69:	mov    0x88(%rbp),%rdx
    180002e70:	je     0x180002e7e
    180002e72:	mov    %rdx,0x8(%rsi)
    180002e76:	movb   $0x6,(%rsi)
    180002e79:	jmp    0x180002fb3
    180002e7e:	mov    0x90(%rbp),%r8
@@ -110886,15 +110886,15 @@
    180003045:	call   0x180003310
    18000304a:	lea    -0x5f(%rbp),%r13
    18000304e:	lea    0x50(%rbp),%rdi
    180003052:	lea    0x70(%rbp),%rbx
    180003056:	lea    0x80(%rbp),%r14
    18000305d:	mov    %rdi,%rcx
    180003060:	mov    %rbx,%rdx
-   180003063:	call   0x180004d80
+   180003063:	call   0x180004f10
    180003068:	cmpq   $0x0,0x50(%rbp)
    18000306d:	jne    0x1800031d1
    180003073:	mov    0x60(%rbp),%rax
    180003077:	test   %rax,%rax
    18000307a:	je     0x1800031d7
    180003080:	mov    %rax,0xa8(%rbp)
    180003087:	mov    0x58(%rbp),%rax
@@ -113065,244 +113065,244 @@
    180004d6c:	int3
    180004d6d:	int3
    180004d6e:	int3
    180004d6f:	int3
    180004d70:	mov    $0x18,%edx
    180004d75:	mov    $0x8,%r8d
    180004d7b:	jmp    0x180007910
-   180004d80:	push   %r15
-   180004d82:	push   %r14
-   180004d84:	push   %rsi
-   180004d85:	push   %rdi
-   180004d86:	push   %rbx
-   180004d87:	sub    $0x40,%rsp
-   180004d8b:	mov    %rdx,%rax
-   180004d8e:	mov    %rcx,%rsi
-   180004d91:	mov    (%rdx),%rdx
-   180004d94:	mov    0x8(%rdx),%r8
-   180004d98:	mov    0x10(%rdx),%rcx
-   180004d9c:	cmp    %r8,%rcx
-   180004d9f:	jae    0x180004dcd
-   180004da1:	mov    (%rdx),%r9
-   180004da4:	movabs $0x100002600,%r10
-   180004dae:	xchg   %ax,%ax
-   180004db0:	movzbl (%r9,%rcx,1),%r11d
-   180004db5:	cmp    $0x2c,%r11
-   180004db9:	ja     0x180004e38
-   180004dbb:	bt     %r11,%r10
-   180004dbf:	jae    0x180004deb
-   180004dc1:	inc    %rcx
-   180004dc4:	mov    %rcx,0x10(%rdx)
-   180004dc8:	cmp    %rcx,%r8
-   180004dcb:	jne    0x180004db0
-   180004dcd:	movq   $0x3,0x28(%rsp)
-   180004dd6:	lea    0x28(%rsp),%rax
-   180004ddb:	mov    %rdx,%rcx
-   180004dde:	mov    %rax,%rdx
-   180004de1:	call   0x180253660
-   180004de6:	jmp    0x180004e8c
-   180004deb:	cmp    $0x2c,%r11
-   180004def:	jne    0x180004e38
-   180004df1:	cmpb   $0x0,0x8(%rax)
-   180004df5:	jne    0x180004e55
-   180004df7:	inc    %rcx
-   180004dfa:	mov    %rcx,0x10(%rdx)
-   180004dfe:	cmp    %r8,%rcx
-   180004e01:	jae    0x180004e2d
-   180004e03:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180004e10:	movzbl (%r9,%rcx,1),%r11d
-   180004e15:	cmp    $0x20,%r11
-   180004e19:	ja     0x180004e59
-   180004e1b:	bt     %r11,%r10
-   180004e1f:	jae    0x180004e59
-   180004e21:	inc    %rcx
-   180004e24:	mov    %rcx,0x10(%rdx)
-   180004e28:	cmp    %rcx,%r8
-   180004e2b:	jne    0x180004e10
-   180004e2d:	movq   $0x5,0x28(%rsp)
-   180004e36:	jmp    0x180004dd6
-   180004e38:	cmp    $0x7d,%r11d
-   180004e3c:	jne    0x180004e4b
-   180004e3e:	movq   $0x0,0x10(%rsi)
-   180004e46:	jmp    0x180004ef3
-   180004e4b:	cmpb   $0x0,0x8(%rax)
-   180004e4f:	je     0x180004f2c
-   180004e55:	movb   $0x0,0x8(%rax)
-   180004e59:	cmp    $0x22,%r11b
-   180004e5d:	jne    0x180004f07
-   180004e63:	inc    %rcx
-   180004e66:	mov    %rcx,0x10(%rdx)
-   180004e6a:	lea    0x18(%rdx),%r8
-   180004e6e:	movq   $0x0,0x28(%rdx)
-   180004e76:	lea    0x28(%rsp),%rcx
-   180004e7b:	call   0x180163fb0
-   180004e80:	cmpl   $0x2,0x28(%rsp)
-   180004e85:	jne    0x180004e97
-   180004e87:	mov    0x30(%rsp),%rax
-   180004e8c:	mov    %rax,0x8(%rsi)
-   180004e90:	mov    $0x1,%eax
-   180004e95:	jmp    0x180004ef5
-   180004e97:	mov    0x30(%rsp),%rbx
-   180004e9c:	mov    0x38(%rsp),%rdi
-   180004ea1:	test   %rdi,%rdi
-   180004ea4:	je     0x180004ed3
-   180004ea6:	setns  %al
-   180004ea9:	js     0x180004f3a
-   180004eaf:	movzbl %al,%r15d
-   180004eb3:	mov    %rdi,%rcx
-   180004eb6:	mov    %r15,%rdx
-   180004eb9:	call   0x180007900
-   180004ebe:	mov    %rax,%r14
-   180004ec1:	test   %rax,%rax
-   180004ec4:	jne    0x180004ed9
-   180004ec6:	mov    %rdi,%rcx
-   180004ec9:	mov    %r15,%rdx
-   180004ecc:	call   0x18025c650
-   180004ed1:	ud2
-   180004ed3:	mov    $0x1,%r14d
-   180004ed9:	mov    %r14,%rcx
-   180004edc:	mov    %rbx,%rdx
-   180004edf:	mov    %rdi,%r8
-   180004ee2:	call   0x1802534fb
-   180004ee7:	mov    %rdi,0x8(%rsi)
-   180004eeb:	mov    %r14,0x10(%rsi)
-   180004eef:	mov    %rdi,0x18(%rsi)
-   180004ef3:	xor    %eax,%eax
-   180004ef5:	mov    %rax,(%rsi)
-   180004ef8:	mov    %rsi,%rax
-   180004efb:	add    $0x40,%rsp
-   180004eff:	pop    %rbx
-   180004f00:	pop    %rdi
-   180004f01:	pop    %rsi
-   180004f02:	pop    %r14
-   180004f04:	pop    %r15
-   180004f06:	ret
-   180004f07:	movzbl %r11b,%eax
-   180004f0b:	cmp    $0x7d,%eax
-   180004f0e:	jne    0x180004f1e
-   180004f10:	movq   $0x12,0x28(%rsp)
-   180004f19:	jmp    0x180004dd6
-   180004f1e:	movq   $0x10,0x28(%rsp)
-   180004f27:	jmp    0x180004dd6
-   180004f2c:	movq   $0x8,0x28(%rsp)
-   180004f35:	jmp    0x180004dd6
-   180004f3a:	call   0x18017cb30
-   180004f3f:	ud2
-   180004f41:	int3
-   180004f42:	int3
-   180004f43:	int3
-   180004f44:	int3
-   180004f45:	int3
-   180004f46:	int3
-   180004f47:	int3
-   180004f48:	int3
-   180004f49:	int3
-   180004f4a:	int3
-   180004f4b:	int3
-   180004f4c:	int3
-   180004f4d:	int3
-   180004f4e:	int3
-   180004f4f:	int3
-   180004f50:	push   %rsi
-   180004f51:	push   %rdi
-   180004f52:	sub    $0x38,%rsp
-   180004f56:	mov    %rdx,%rax
-   180004f59:	mov    %rcx,%rsi
-   180004f5c:	mov    (%rdx),%rdx
-   180004f5f:	mov    0x8(%rdx),%r10
-   180004f63:	mov    0x10(%rdx),%rcx
-   180004f67:	cmp    %r10,%rcx
-   180004f6a:	jae    0x180004fba
-   180004f6c:	mov    (%rdx),%r8
-   180004f6f:	inc    %rcx
-   180004f72:	mov    %r10,%rdi
-   180004f75:	neg    %rdi
-   180004f78:	movabs $0x100002600,%r9
-   180004f82:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180004f90:	movzbl -0x1(%r8,%rcx,1),%r11d
-   180004f96:	cmp    $0x2c,%r11
-   180004f9a:	ja     0x180005041
-   180004fa0:	bt     %r11,%r9
-   180004fa4:	jae    0x180004fe3
-   180004fa6:	mov    %rcx,0x10(%rdx)
-   180004faa:	lea    (%rdi,%rcx,1),%r11
-   180004fae:	inc    %r11
+   180004d80:	push   %rsi
+   180004d81:	push   %rdi
+   180004d82:	sub    $0x38,%rsp
+   180004d86:	mov    %rdx,%rax
+   180004d89:	mov    %rcx,%rsi
+   180004d8c:	mov    (%rdx),%rdx
+   180004d8f:	mov    0x8(%rdx),%r10
+   180004d93:	mov    0x10(%rdx),%rcx
+   180004d97:	cmp    %r10,%rcx
+   180004d9a:	jae    0x180004dea
+   180004d9c:	mov    (%rdx),%r8
+   180004d9f:	inc    %rcx
+   180004da2:	mov    %r10,%rdi
+   180004da5:	neg    %rdi
+   180004da8:	movabs $0x100002600,%r9
+   180004db2:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   180004dc0:	movzbl -0x1(%r8,%rcx,1),%r11d
+   180004dc6:	cmp    $0x2c,%r11
+   180004dca:	ja     0x180004e71
+   180004dd0:	bt     %r11,%r9
+   180004dd4:	jae    0x180004e13
+   180004dd6:	mov    %rcx,0x10(%rdx)
+   180004dda:	lea    (%rdi,%rcx,1),%r11
+   180004dde:	inc    %r11
+   180004de1:	inc    %rcx
+   180004de4:	cmp    $0x1,%r11
+   180004de8:	jne    0x180004dc0
+   180004dea:	movq   $0x3,0x20(%rsp)
+   180004df3:	lea    0x20(%rsp),%rax
+   180004df8:	mov    %rdx,%rcx
+   180004dfb:	mov    %rax,%rdx
+   180004dfe:	call   0x180253660
+   180004e03:	mov    %rax,0x8(%rsi)
+   180004e07:	movq   $0x1,(%rsi)
+   180004e0e:	jmp    0x180004ed1
+   180004e13:	cmp    $0x2c,%r11
+   180004e17:	jne    0x180004e71
+   180004e19:	cmpb   $0x0,0x8(%rax)
+   180004e1d:	jne    0x180004e8e
+   180004e1f:	mov    %rcx,0x10(%rdx)
+   180004e23:	cmp    %r10,%rcx
+   180004e26:	jae    0x180004e66
+   180004e28:	inc    %rcx
+   180004e2b:	mov    $0x1,%eax
+   180004e30:	sub    %r10,%rax
+   180004e33:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   180004e40:	movzbl -0x1(%r8,%rcx,1),%r11d
+   180004e46:	cmp    $0x20,%r11
+   180004e4a:	ja     0x180004e92
+   180004e4c:	bt     %r11,%r9
+   180004e50:	jae    0x180004e92
+   180004e52:	mov    %rcx,0x10(%rdx)
+   180004e56:	lea    (%rax,%rcx,1),%r10
+   180004e5a:	inc    %r10
+   180004e5d:	inc    %rcx
+   180004e60:	cmp    $0x2,%r10
+   180004e64:	jne    0x180004e40
+   180004e66:	movq   $0x5,0x20(%rsp)
+   180004e6f:	jmp    0x180004df3
+   180004e71:	cmp    $0x7d,%r11d
+   180004e75:	jne    0x180004e88
+   180004e77:	movq   $0x0,0x10(%rsi)
+   180004e7f:	movq   $0x0,(%rsi)
+   180004e86:	jmp    0x180004ed1
+   180004e88:	cmpb   $0x0,0x8(%rax)
+   180004e8c:	je     0x180004f00
+   180004e8e:	movb   $0x0,0x8(%rax)
+   180004e92:	cmp    $0x22,%r11b
+   180004e96:	jne    0x180004edb
+   180004e98:	lea    0x20(%rsp),%rcx
+   180004e9d:	call   0x1800033d0
+   180004ea2:	cmpq   $0x0,0x28(%rsp)
+   180004ea8:	je     0x180004ec0
+   180004eaa:	mov    0x30(%rsp),%rax
+   180004eaf:	mov    %rax,0x18(%rsi)
+   180004eb3:	movups 0x20(%rsp),%xmm0
+   180004eb8:	movups %xmm0,0x8(%rsi)
+   180004ebc:	xor    %eax,%eax
+   180004ebe:	jmp    0x180004ece
+   180004ec0:	mov    0x20(%rsp),%rax
+   180004ec5:	mov    %rax,0x8(%rsi)
+   180004ec9:	mov    $0x1,%eax
+   180004ece:	mov    %rax,(%rsi)
+   180004ed1:	mov    %rsi,%rax
+   180004ed4:	add    $0x38,%rsp
+   180004ed8:	pop    %rdi
+   180004ed9:	pop    %rsi
+   180004eda:	ret
+   180004edb:	movzbl %r11b,%eax
+   180004edf:	cmp    $0x7d,%eax
+   180004ee2:	jne    0x180004ef2
+   180004ee4:	movq   $0x12,0x20(%rsp)
+   180004eed:	jmp    0x180004df3
+   180004ef2:	movq   $0x10,0x20(%rsp)
+   180004efb:	jmp    0x180004df3
+   180004f00:	movq   $0x8,0x20(%rsp)
+   180004f09:	jmp    0x180004df3
+   180004f0e:	int3
+   180004f0f:	int3
+   180004f10:	push   %r15
+   180004f12:	push   %r14
+   180004f14:	push   %rsi
+   180004f15:	push   %rdi
+   180004f16:	push   %rbx
+   180004f17:	sub    $0x40,%rsp
+   180004f1b:	mov    %rdx,%rax
+   180004f1e:	mov    %rcx,%rsi
+   180004f21:	mov    (%rdx),%rdx
+   180004f24:	mov    0x8(%rdx),%r8
+   180004f28:	mov    0x10(%rdx),%rcx
+   180004f2c:	cmp    %r8,%rcx
+   180004f2f:	jae    0x180004f5d
+   180004f31:	mov    (%rdx),%r9
+   180004f34:	movabs $0x100002600,%r10
+   180004f3e:	xchg   %ax,%ax
+   180004f40:	movzbl (%r9,%rcx,1),%r11d
+   180004f45:	cmp    $0x2c,%r11
+   180004f49:	ja     0x180004fc8
+   180004f4b:	bt     %r11,%r10
+   180004f4f:	jae    0x180004f7b
+   180004f51:	inc    %rcx
+   180004f54:	mov    %rcx,0x10(%rdx)
+   180004f58:	cmp    %rcx,%r8
+   180004f5b:	jne    0x180004f40
+   180004f5d:	movq   $0x3,0x28(%rsp)
+   180004f66:	lea    0x28(%rsp),%rax
+   180004f6b:	mov    %rdx,%rcx
+   180004f6e:	mov    %rax,%rdx
+   180004f71:	call   0x180253660
+   180004f76:	jmp    0x18000501c
+   180004f7b:	cmp    $0x2c,%r11
+   180004f7f:	jne    0x180004fc8
+   180004f81:	cmpb   $0x0,0x8(%rax)
+   180004f85:	jne    0x180004fe5
+   180004f87:	inc    %rcx
+   180004f8a:	mov    %rcx,0x10(%rdx)
+   180004f8e:	cmp    %r8,%rcx
+   180004f91:	jae    0x180004fbd
+   180004f93:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   180004fa0:	movzbl (%r9,%rcx,1),%r11d
+   180004fa5:	cmp    $0x20,%r11
+   180004fa9:	ja     0x180004fe9
+   180004fab:	bt     %r11,%r10
+   180004faf:	jae    0x180004fe9
    180004fb1:	inc    %rcx
-   180004fb4:	cmp    $0x1,%r11
-   180004fb8:	jne    0x180004f90
-   180004fba:	movq   $0x3,0x20(%rsp)
-   180004fc3:	lea    0x20(%rsp),%rax
-   180004fc8:	mov    %rdx,%rcx
-   180004fcb:	mov    %rax,%rdx
-   180004fce:	call   0x180253660
-   180004fd3:	mov    %rax,0x8(%rsi)
-   180004fd7:	movq   $0x1,(%rsi)
-   180004fde:	jmp    0x1800050a1
-   180004fe3:	cmp    $0x2c,%r11
-   180004fe7:	jne    0x180005041
-   180004fe9:	cmpb   $0x0,0x8(%rax)
-   180004fed:	jne    0x18000505e
-   180004fef:	mov    %rcx,0x10(%rdx)
-   180004ff3:	cmp    %r10,%rcx
-   180004ff6:	jae    0x180005036
-   180004ff8:	inc    %rcx
-   180004ffb:	mov    $0x1,%eax
-   180005000:	sub    %r10,%rax
-   180005003:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180005010:	movzbl -0x1(%r8,%rcx,1),%r11d
-   180005016:	cmp    $0x20,%r11
-   18000501a:	ja     0x180005062
-   18000501c:	bt     %r11,%r9
-   180005020:	jae    0x180005062
-   180005022:	mov    %rcx,0x10(%rdx)
-   180005026:	lea    (%rax,%rcx,1),%r10
-   18000502a:	inc    %r10
-   18000502d:	inc    %rcx
-   180005030:	cmp    $0x2,%r10
-   180005034:	jne    0x180005010
-   180005036:	movq   $0x5,0x20(%rsp)
-   18000503f:	jmp    0x180004fc3
-   180005041:	cmp    $0x7d,%r11d
-   180005045:	jne    0x180005058
-   180005047:	movq   $0x0,0x10(%rsi)
-   18000504f:	movq   $0x0,(%rsi)
-   180005056:	jmp    0x1800050a1
-   180005058:	cmpb   $0x0,0x8(%rax)
-   18000505c:	je     0x1800050d0
-   18000505e:	movb   $0x0,0x8(%rax)
-   180005062:	cmp    $0x22,%r11b
-   180005066:	jne    0x1800050ab
-   180005068:	lea    0x20(%rsp),%rcx
-   18000506d:	call   0x1800033d0
-   180005072:	cmpq   $0x0,0x28(%rsp)
-   180005078:	je     0x180005090
-   18000507a:	mov    0x30(%rsp),%rax
-   18000507f:	mov    %rax,0x18(%rsi)
-   180005083:	movups 0x20(%rsp),%xmm0
-   180005088:	movups %xmm0,0x8(%rsi)
-   18000508c:	xor    %eax,%eax
-   18000508e:	jmp    0x18000509e
-   180005090:	mov    0x20(%rsp),%rax
-   180005095:	mov    %rax,0x8(%rsi)
-   180005099:	mov    $0x1,%eax
-   18000509e:	mov    %rax,(%rsi)
-   1800050a1:	mov    %rsi,%rax
-   1800050a4:	add    $0x38,%rsp
-   1800050a8:	pop    %rdi
-   1800050a9:	pop    %rsi
-   1800050aa:	ret
-   1800050ab:	movzbl %r11b,%eax
-   1800050af:	cmp    $0x7d,%eax
-   1800050b2:	jne    0x1800050c2
-   1800050b4:	movq   $0x12,0x20(%rsp)
-   1800050bd:	jmp    0x180004fc3
-   1800050c2:	movq   $0x10,0x20(%rsp)
-   1800050cb:	jmp    0x180004fc3
-   1800050d0:	movq   $0x8,0x20(%rsp)
-   1800050d9:	jmp    0x180004fc3
+   180004fb4:	mov    %rcx,0x10(%rdx)
+   180004fb8:	cmp    %rcx,%r8
+   180004fbb:	jne    0x180004fa0
+   180004fbd:	movq   $0x5,0x28(%rsp)
+   180004fc6:	jmp    0x180004f66
+   180004fc8:	cmp    $0x7d,%r11d
+   180004fcc:	jne    0x180004fdb
+   180004fce:	movq   $0x0,0x10(%rsi)
+   180004fd6:	jmp    0x180005083
+   180004fdb:	cmpb   $0x0,0x8(%rax)
+   180004fdf:	je     0x1800050bc
+   180004fe5:	movb   $0x0,0x8(%rax)
+   180004fe9:	cmp    $0x22,%r11b
+   180004fed:	jne    0x180005097
+   180004ff3:	inc    %rcx
+   180004ff6:	mov    %rcx,0x10(%rdx)
+   180004ffa:	lea    0x18(%rdx),%r8
+   180004ffe:	movq   $0x0,0x28(%rdx)
+   180005006:	lea    0x28(%rsp),%rcx
+   18000500b:	call   0x180163fb0
+   180005010:	cmpl   $0x2,0x28(%rsp)
+   180005015:	jne    0x180005027
+   180005017:	mov    0x30(%rsp),%rax
+   18000501c:	mov    %rax,0x8(%rsi)
+   180005020:	mov    $0x1,%eax
+   180005025:	jmp    0x180005085
+   180005027:	mov    0x30(%rsp),%rbx
+   18000502c:	mov    0x38(%rsp),%rdi
+   180005031:	test   %rdi,%rdi
+   180005034:	je     0x180005063
+   180005036:	setns  %al
+   180005039:	js     0x1800050ca
+   18000503f:	movzbl %al,%r15d
+   180005043:	mov    %rdi,%rcx
+   180005046:	mov    %r15,%rdx
+   180005049:	call   0x180007900
+   18000504e:	mov    %rax,%r14
+   180005051:	test   %rax,%rax
+   180005054:	jne    0x180005069
+   180005056:	mov    %rdi,%rcx
+   180005059:	mov    %r15,%rdx
+   18000505c:	call   0x18025c650
+   180005061:	ud2
+   180005063:	mov    $0x1,%r14d
+   180005069:	mov    %r14,%rcx
+   18000506c:	mov    %rbx,%rdx
+   18000506f:	mov    %rdi,%r8
+   180005072:	call   0x1802534fb
+   180005077:	mov    %rdi,0x8(%rsi)
+   18000507b:	mov    %r14,0x10(%rsi)
+   18000507f:	mov    %rdi,0x18(%rsi)
+   180005083:	xor    %eax,%eax
+   180005085:	mov    %rax,(%rsi)
+   180005088:	mov    %rsi,%rax
+   18000508b:	add    $0x40,%rsp
+   18000508f:	pop    %rbx
+   180005090:	pop    %rdi
+   180005091:	pop    %rsi
+   180005092:	pop    %r14
+   180005094:	pop    %r15
+   180005096:	ret
+   180005097:	movzbl %r11b,%eax
+   18000509b:	cmp    $0x7d,%eax
+   18000509e:	jne    0x1800050ae
+   1800050a0:	movq   $0x12,0x28(%rsp)
+   1800050a9:	jmp    0x180004f66
+   1800050ae:	movq   $0x10,0x28(%rsp)
+   1800050b7:	jmp    0x180004f66
+   1800050bc:	movq   $0x8,0x28(%rsp)
+   1800050c5:	jmp    0x180004f66
+   1800050ca:	call   0x18017cb30
+   1800050cf:	ud2
+   1800050d1:	int3
+   1800050d2:	int3
+   1800050d3:	int3
+   1800050d4:	int3
+   1800050d5:	int3
+   1800050d6:	int3
+   1800050d7:	int3
+   1800050d8:	int3
+   1800050d9:	int3
+   1800050da:	int3
+   1800050db:	int3
+   1800050dc:	int3
+   1800050dd:	int3
    1800050de:	int3
    1800050df:	int3
    1800050e0:	push   %rsi
    1800050e1:	push   %rdi
    1800050e2:	push   %rbx
    1800050e3:	sub    $0x20,%rsp
    1800050e7:	mov    %rdx,%rdi
@@ -113419,314 +113419,314 @@
    18000523c:	int3
    18000523d:	int3
    18000523e:	int3
    18000523f:	int3
    180005240:	push   %rbp
    180005241:	push   %rsi
    180005242:	push   %rdi
-   180005243:	sub    $0xa0,%rsp
-   18000524a:	lea    0x80(%rsp),%rbp
-   180005252:	movq   $0xfffffffffffffffe,0x18(%rbp)
+   180005243:	push   %rbx
+   180005244:	sub    $0x48,%rsp
+   180005248:	lea    0x40(%rsp),%rbp
+   18000524d:	movq   $0xfffffffffffffffe,0x0(%rbp)
+   180005255:	mov    %r8,%rdi
+   180005258:	mov    %edx,%ebx
    18000525a:	mov    %rcx,%rsi
    18000525d:	call   0x18018e500
-   180005262:	lea    0x258737(%rip),%rax        # 0x18025d9a0
-   180005269:	mov    %rax,-0x40(%rbp)
-   18000526d:	lea    -0x24f4(%rip),%rax        # 0x180002d80
-   180005274:	mov    %rax,-0x38(%rbp)
-   180005278:	lea    0x2587a1(%rip),%rcx        # 0x18025da20
-   18000527f:	mov    %rcx,-0x30(%rbp)
-   180005283:	mov    %rax,-0x28(%rbp)
-   180005287:	lea    0x25873a(%rip),%rax        # 0x18025d9c8
-   18000528e:	mov    %rax,-0x10(%rbp)
-   180005292:	movq   $0x3,-0x8(%rbp)
-   18000529a:	movq   $0x0,-0x20(%rbp)
-   1800052a2:	lea    -0x40(%rbp),%rax
-   1800052a6:	mov    %rax,0x0(%rbp)
-   1800052aa:	movq   $0x2,0x8(%rbp)
-   1800052b2:	lea    -0x58(%rbp),%rdi
-   1800052b6:	lea    -0x20(%rbp),%rdx
-   1800052ba:	mov    %rdi,%rcx
-   1800052bd:	call   0x18017d070
-   1800052c2:	mov    %rsi,%rcx
-   1800052c5:	mov    %rdi,%rdx
-   1800052c8:	call   0x180003490
-   1800052cd:	test   %rax,%rax
-   1800052d0:	je     0x18000536c
-   1800052d6:	lea    -0x20(%rbp),%rcx
-   1800052da:	mov    %rax,%rdx
-   1800052dd:	call   0x180007c90
-   1800052e2:	mov    -0x18(%rbp),%rdx
-   1800052e6:	mov    -0x10(%rbp),%r8
-   1800052ea:	mov    %rsi,%rcx
-   1800052ed:	mov    %rdx,0x10(%rbp)
-   1800052f1:	call   0x180008170
-   1800052f6:	mov    %rax,%rdi
-   1800052f9:	test   %rax,%rax
-   1800052fc:	je     0x180005342
-   1800052fe:	mov    (%rdi),%eax
-   180005300:	lea    -0x2(%rax),%rcx
-   180005304:	cmp    $0x2,%rcx
-   180005308:	jb     0x18000532f
-   18000530a:	test   %rax,%rax
-   18000530d:	je     0x18000532f
-   18000530f:	cmp    $0x1,%eax
-   180005312:	jne    0x180005378
-   180005314:	lea    0x10(%rdi),%rax
-   180005318:	mov    (%rax),%rdx
-   18000531b:	test   %rdx,%rdx
-   18000531e:	je     0x18000532f
-   180005320:	mov    0x8(%rax),%rcx
-   180005324:	mov    $0x1,%r8d
-   18000532a:	call   0x180007910
-   18000532f:	mov    $0x28,%edx
-   180005334:	mov    $0x8,%r8d
-   18000533a:	mov    %rdi,%rcx
-   18000533d:	call   0x180007910
-   180005342:	mov    -0x20(%rbp),%rdx
-   180005346:	test   %rdx,%rdx
-   180005349:	je     0x18000535a
-   18000534b:	mov    $0x1,%r8d
-   180005351:	mov    0x10(%rbp),%rcx
-   180005355:	call   0x180007910
-   18000535a:	test   %rdi,%rdi
-   18000535d:	je     0x18000536c
-   18000535f:	mov    %rsi,%rcx
-   180005362:	mov    $0x2,%edx
-   180005367:	call   0x180008290
-   18000536c:	nop
-   18000536d:	add    $0xa0,%rsp
-   180005374:	pop    %rdi
-   180005375:	pop    %rsi
-   180005376:	pop    %rbp
-   180005377:	ret
-   180005378:	lea    0x8(%rdi),%rax
-   18000537c:	mov    (%rax),%rdx
-   18000537f:	test   %rdx,%rdx
-   180005382:	jne    0x180005320
-   180005384:	jmp    0x18000532f
-   180005386:	cs nopw 0x0(%rax,%rax,1)
-   180005390:	mov    %rdx,0x10(%rsp)
-   180005395:	push   %rbp
-   180005396:	push   %rsi
-   180005397:	push   %rdi
-   180005398:	sub    $0x20,%rsp
-   18000539c:	lea    0x80(%rdx),%rbp
-   1800053a3:	mov    -0x20(%rbp),%rcx
-   1800053a7:	mov    0x10(%rbp),%rdx
-   1800053ab:	call   0x1800032f0
-   1800053b0:	nop
-   1800053b1:	add    $0x20,%rsp
-   1800053b5:	pop    %rdi
-   1800053b6:	pop    %rsi
-   1800053b7:	pop    %rbp
-   1800053b8:	ret
-   1800053b9:	int3
-   1800053ba:	int3
-   1800053bb:	int3
-   1800053bc:	int3
-   1800053bd:	int3
-   1800053be:	int3
-   1800053bf:	int3
-   1800053c0:	push   %rbp
-   1800053c1:	push   %rsi
-   1800053c2:	push   %rdi
-   1800053c3:	sub    $0x90,%rsp
-   1800053ca:	lea    0x80(%rsp),%rbp
-   1800053d2:	movq   $0xfffffffffffffffe,0x8(%rbp)
-   1800053da:	mov    %rcx,%rsi
-   1800053dd:	call   0x18018e500
-   1800053e2:	lea    0x2585b7(%rip),%rax        # 0x18025d9a0
-   1800053e9:	mov    %rax,-0x40(%rbp)
-   1800053ed:	lea    -0x2674(%rip),%rax        # 0x180002d80
-   1800053f4:	mov    %rax,-0x38(%rbp)
-   1800053f8:	lea    0x258581(%rip),%rax        # 0x18025d980
-   1800053ff:	mov    %rax,-0x20(%rbp)
-   180005403:	movq   $0x1,-0x18(%rbp)
-   18000540b:	movq   $0x0,-0x30(%rbp)
-   180005413:	lea    -0x40(%rbp),%rax
-   180005417:	mov    %rax,-0x10(%rbp)
-   18000541b:	movq   $0x1,-0x8(%rbp)
-   180005423:	lea    -0x58(%rbp),%rdi
-   180005427:	lea    -0x30(%rbp),%rdx
-   18000542b:	mov    %rdi,%rcx
-   18000542e:	call   0x18017d070
-   180005433:	mov    %rsi,%rcx
-   180005436:	mov    %rdi,%rdx
-   180005439:	call   0x180003490
-   18000543e:	test   %rax,%rax
-   180005441:	je     0x1800054dd
-   180005447:	lea    -0x30(%rbp),%rcx
-   18000544b:	mov    %rax,%rdx
-   18000544e:	call   0x180007c90
-   180005453:	mov    -0x28(%rbp),%rdx
-   180005457:	mov    -0x20(%rbp),%r8
-   18000545b:	mov    %rsi,%rcx
-   18000545e:	mov    %rdx,0x0(%rbp)
-   180005462:	call   0x180008170
-   180005467:	mov    %rax,%rdi
-   18000546a:	test   %rax,%rax
-   18000546d:	je     0x1800054b3
-   18000546f:	mov    (%rdi),%eax
-   180005471:	lea    -0x2(%rax),%rcx
-   180005475:	cmp    $0x2,%rcx
-   180005479:	jb     0x1800054a0
-   18000547b:	test   %rax,%rax
-   18000547e:	je     0x1800054a0
-   180005480:	cmp    $0x1,%eax
-   180005483:	jne    0x1800054e9
-   180005485:	lea    0x10(%rdi),%rax
-   180005489:	mov    (%rax),%rdx
-   18000548c:	test   %rdx,%rdx
-   18000548f:	je     0x1800054a0
-   180005491:	mov    0x8(%rax),%rcx
-   180005495:	mov    $0x1,%r8d
-   18000549b:	call   0x180007910
-   1800054a0:	mov    $0x28,%edx
-   1800054a5:	mov    $0x8,%r8d
-   1800054ab:	mov    %rdi,%rcx
-   1800054ae:	call   0x180007910
-   1800054b3:	mov    -0x30(%rbp),%rdx
-   1800054b7:	test   %rdx,%rdx
-   1800054ba:	je     0x1800054cb
-   1800054bc:	mov    $0x1,%r8d
-   1800054c2:	mov    0x0(%rbp),%rcx
-   1800054c6:	call   0x180007910
-   1800054cb:	test   %rdi,%rdi
-   1800054ce:	je     0x1800054dd
-   1800054d0:	mov    %rsi,%rcx
-   1800054d3:	mov    $0x2,%edx
-   1800054d8:	call   0x180008290
-   1800054dd:	nop
-   1800054de:	add    $0x90,%rsp
-   1800054e5:	pop    %rdi
-   1800054e6:	pop    %rsi
-   1800054e7:	pop    %rbp
-   1800054e8:	ret
-   1800054e9:	lea    0x8(%rdi),%rax
-   1800054ed:	mov    (%rax),%rdx
-   1800054f0:	test   %rdx,%rdx
-   1800054f3:	jne    0x180005491
-   1800054f5:	jmp    0x1800054a0
-   1800054f7:	nopw   0x0(%rax,%rax,1)
-   180005500:	mov    %rdx,0x10(%rsp)
-   180005505:	push   %rbp
-   180005506:	push   %rsi
-   180005507:	push   %rdi
-   180005508:	sub    $0x20,%rsp
-   18000550c:	lea    0x80(%rdx),%rbp
-   180005513:	mov    -0x30(%rbp),%rcx
-   180005517:	mov    0x0(%rbp),%rdx
-   18000551b:	call   0x1800032f0
-   180005520:	nop
-   180005521:	add    $0x20,%rsp
-   180005525:	pop    %rdi
-   180005526:	pop    %rsi
-   180005527:	pop    %rbp
-   180005528:	ret
-   180005529:	int3
-   18000552a:	int3
-   18000552b:	int3
-   18000552c:	int3
-   18000552d:	int3
-   18000552e:	int3
-   18000552f:	int3
-   180005530:	push   %rbp
-   180005531:	push   %rsi
-   180005532:	push   %rdi
-   180005533:	push   %rbx
-   180005534:	sub    $0x48,%rsp
-   180005538:	lea    0x40(%rsp),%rbp
-   18000553d:	movq   $0xfffffffffffffffe,0x0(%rbp)
-   180005545:	mov    %r8,%rdi
-   180005548:	mov    %edx,%ebx
-   18000554a:	mov    %rcx,%rsi
-   18000554d:	call   0x18018e500
-   180005552:	movslq %ebx,%r8
-   180005555:	mov    %rsi,%rcx
-   180005558:	mov    %rdi,%rdx
-   18000555b:	call   0x1800064a0
-   180005560:	test   %rax,%rax
-   180005563:	je     0x180005607
-   180005569:	lea    -0x20(%rbp),%rcx
-   18000556d:	mov    %rax,%rdx
-   180005570:	call   0x180007c90
-   180005575:	mov    -0x18(%rbp),%rdx
-   180005579:	mov    -0x10(%rbp),%r8
-   18000557d:	mov    %rsi,%rcx
-   180005580:	mov    %rdx,-0x8(%rbp)
-   180005584:	call   0x180008170
-   180005589:	mov    %rax,%rdi
-   18000558c:	test   %rax,%rax
-   18000558f:	je     0x1800055d5
-   180005591:	mov    (%rdi),%eax
-   180005593:	lea    -0x2(%rax),%rcx
-   180005597:	cmp    $0x2,%rcx
-   18000559b:	jb     0x1800055c2
-   18000559d:	test   %rax,%rax
-   1800055a0:	je     0x1800055c2
-   1800055a2:	cmp    $0x1,%eax
-   1800055a5:	jne    0x180005611
-   1800055a7:	lea    0x10(%rdi),%rax
-   1800055ab:	mov    (%rax),%rdx
-   1800055ae:	test   %rdx,%rdx
-   1800055b1:	je     0x1800055c2
-   1800055b3:	mov    0x8(%rax),%rcx
-   1800055b7:	mov    $0x1,%r8d
-   1800055bd:	call   0x180007910
-   1800055c2:	mov    $0x28,%edx
-   1800055c7:	mov    $0x8,%r8d
-   1800055cd:	mov    %rdi,%rcx
-   1800055d0:	call   0x180007910
-   1800055d5:	mov    -0x20(%rbp),%rdx
-   1800055d9:	test   %rdx,%rdx
-   1800055dc:	je     0x1800055ed
-   1800055de:	mov    $0x1,%r8d
-   1800055e4:	mov    -0x8(%rbp),%rcx
-   1800055e8:	call   0x180007910
-   1800055ed:	test   %rdi,%rdi
-   1800055f0:	je     0x180005607
-   1800055f2:	mov    %rsi,%rcx
-   1800055f5:	mov    $0x2,%edx
-   1800055fa:	add    $0x48,%rsp
-   1800055fe:	pop    %rbx
-   1800055ff:	pop    %rdi
-   180005600:	pop    %rsi
-   180005601:	pop    %rbp
-   180005602:	jmp    0x180008290
-   180005607:	nop
-   180005608:	add    $0x48,%rsp
-   18000560c:	pop    %rbx
-   18000560d:	pop    %rdi
-   18000560e:	pop    %rsi
-   18000560f:	pop    %rbp
-   180005610:	ret
-   180005611:	lea    0x8(%rdi),%rax
-   180005615:	mov    (%rax),%rdx
-   180005618:	test   %rdx,%rdx
-   18000561b:	jne    0x1800055b3
-   18000561d:	jmp    0x1800055c2
-   18000561f:	nop
+   180005262:	movslq %ebx,%r8
+   180005265:	mov    %rsi,%rcx
+   180005268:	mov    %rdi,%rdx
+   18000526b:	call   0x1800064a0
+   180005270:	test   %rax,%rax
+   180005273:	je     0x180005317
+   180005279:	lea    -0x20(%rbp),%rcx
+   18000527d:	mov    %rax,%rdx
+   180005280:	call   0x180007c90
+   180005285:	mov    -0x18(%rbp),%rdx
+   180005289:	mov    -0x10(%rbp),%r8
+   18000528d:	mov    %rsi,%rcx
+   180005290:	mov    %rdx,-0x8(%rbp)
+   180005294:	call   0x180008170
+   180005299:	mov    %rax,%rdi
+   18000529c:	test   %rax,%rax
+   18000529f:	je     0x1800052e5
+   1800052a1:	mov    (%rdi),%eax
+   1800052a3:	lea    -0x2(%rax),%rcx
+   1800052a7:	cmp    $0x2,%rcx
+   1800052ab:	jb     0x1800052d2
+   1800052ad:	test   %rax,%rax
+   1800052b0:	je     0x1800052d2
+   1800052b2:	cmp    $0x1,%eax
+   1800052b5:	jne    0x180005321
+   1800052b7:	lea    0x10(%rdi),%rax
+   1800052bb:	mov    (%rax),%rdx
+   1800052be:	test   %rdx,%rdx
+   1800052c1:	je     0x1800052d2
+   1800052c3:	mov    0x8(%rax),%rcx
+   1800052c7:	mov    $0x1,%r8d
+   1800052cd:	call   0x180007910
+   1800052d2:	mov    $0x28,%edx
+   1800052d7:	mov    $0x8,%r8d
+   1800052dd:	mov    %rdi,%rcx
+   1800052e0:	call   0x180007910
+   1800052e5:	mov    -0x20(%rbp),%rdx
+   1800052e9:	test   %rdx,%rdx
+   1800052ec:	je     0x1800052fd
+   1800052ee:	mov    $0x1,%r8d
+   1800052f4:	mov    -0x8(%rbp),%rcx
+   1800052f8:	call   0x180007910
+   1800052fd:	test   %rdi,%rdi
+   180005300:	je     0x180005317
+   180005302:	mov    %rsi,%rcx
+   180005305:	mov    $0x2,%edx
+   18000530a:	add    $0x48,%rsp
+   18000530e:	pop    %rbx
+   18000530f:	pop    %rdi
+   180005310:	pop    %rsi
+   180005311:	pop    %rbp
+   180005312:	jmp    0x180008290
+   180005317:	nop
+   180005318:	add    $0x48,%rsp
+   18000531c:	pop    %rbx
+   18000531d:	pop    %rdi
+   18000531e:	pop    %rsi
+   18000531f:	pop    %rbp
+   180005320:	ret
+   180005321:	lea    0x8(%rdi),%rax
+   180005325:	mov    (%rax),%rdx
+   180005328:	test   %rdx,%rdx
+   18000532b:	jne    0x1800052c3
+   18000532d:	jmp    0x1800052d2
+   18000532f:	nop
+   180005330:	mov    %rdx,0x10(%rsp)
+   180005335:	push   %rbp
+   180005336:	push   %rsi
+   180005337:	push   %rdi
+   180005338:	push   %rbx
+   180005339:	sub    $0x28,%rsp
+   18000533d:	lea    0x40(%rdx),%rbp
+   180005341:	mov    -0x20(%rbp),%rcx
+   180005345:	mov    -0x8(%rbp),%rdx
+   180005349:	call   0x1800032f0
+   18000534e:	nop
+   18000534f:	add    $0x28,%rsp
+   180005353:	pop    %rbx
+   180005354:	pop    %rdi
+   180005355:	pop    %rsi
+   180005356:	pop    %rbp
+   180005357:	ret
+   180005358:	int3
+   180005359:	int3
+   18000535a:	int3
+   18000535b:	int3
+   18000535c:	int3
+   18000535d:	int3
+   18000535e:	int3
+   18000535f:	int3
+   180005360:	push   %rbp
+   180005361:	push   %rsi
+   180005362:	push   %rdi
+   180005363:	sub    $0x90,%rsp
+   18000536a:	lea    0x80(%rsp),%rbp
+   180005372:	movq   $0xfffffffffffffffe,0x8(%rbp)
+   18000537a:	mov    %rcx,%rsi
+   18000537d:	call   0x18018e500
+   180005382:	lea    0x258617(%rip),%rax        # 0x18025d9a0
+   180005389:	mov    %rax,-0x40(%rbp)
+   18000538d:	lea    -0x2614(%rip),%rax        # 0x180002d80
+   180005394:	mov    %rax,-0x38(%rbp)
+   180005398:	lea    0x2585e1(%rip),%rax        # 0x18025d980
+   18000539f:	mov    %rax,-0x20(%rbp)
+   1800053a3:	movq   $0x1,-0x18(%rbp)
+   1800053ab:	movq   $0x0,-0x30(%rbp)
+   1800053b3:	lea    -0x40(%rbp),%rax
+   1800053b7:	mov    %rax,-0x10(%rbp)
+   1800053bb:	movq   $0x1,-0x8(%rbp)
+   1800053c3:	lea    -0x58(%rbp),%rdi
+   1800053c7:	lea    -0x30(%rbp),%rdx
+   1800053cb:	mov    %rdi,%rcx
+   1800053ce:	call   0x18017d070
+   1800053d3:	mov    %rsi,%rcx
+   1800053d6:	mov    %rdi,%rdx
+   1800053d9:	call   0x180003490
+   1800053de:	test   %rax,%rax
+   1800053e1:	je     0x18000547d
+   1800053e7:	lea    -0x30(%rbp),%rcx
+   1800053eb:	mov    %rax,%rdx
+   1800053ee:	call   0x180007c90
+   1800053f3:	mov    -0x28(%rbp),%rdx
+   1800053f7:	mov    -0x20(%rbp),%r8
+   1800053fb:	mov    %rsi,%rcx
+   1800053fe:	mov    %rdx,0x0(%rbp)
+   180005402:	call   0x180008170
+   180005407:	mov    %rax,%rdi
+   18000540a:	test   %rax,%rax
+   18000540d:	je     0x180005453
+   18000540f:	mov    (%rdi),%eax
+   180005411:	lea    -0x2(%rax),%rcx
+   180005415:	cmp    $0x2,%rcx
+   180005419:	jb     0x180005440
+   18000541b:	test   %rax,%rax
+   18000541e:	je     0x180005440
+   180005420:	cmp    $0x1,%eax
+   180005423:	jne    0x180005489
+   180005425:	lea    0x10(%rdi),%rax
+   180005429:	mov    (%rax),%rdx
+   18000542c:	test   %rdx,%rdx
+   18000542f:	je     0x180005440
+   180005431:	mov    0x8(%rax),%rcx
+   180005435:	mov    $0x1,%r8d
+   18000543b:	call   0x180007910
+   180005440:	mov    $0x28,%edx
+   180005445:	mov    $0x8,%r8d
+   18000544b:	mov    %rdi,%rcx
+   18000544e:	call   0x180007910
+   180005453:	mov    -0x30(%rbp),%rdx
+   180005457:	test   %rdx,%rdx
+   18000545a:	je     0x18000546b
+   18000545c:	mov    $0x1,%r8d
+   180005462:	mov    0x0(%rbp),%rcx
+   180005466:	call   0x180007910
+   18000546b:	test   %rdi,%rdi
+   18000546e:	je     0x18000547d
+   180005470:	mov    %rsi,%rcx
+   180005473:	mov    $0x2,%edx
+   180005478:	call   0x180008290
+   18000547d:	nop
+   18000547e:	add    $0x90,%rsp
+   180005485:	pop    %rdi
+   180005486:	pop    %rsi
+   180005487:	pop    %rbp
+   180005488:	ret
+   180005489:	lea    0x8(%rdi),%rax
+   18000548d:	mov    (%rax),%rdx
+   180005490:	test   %rdx,%rdx
+   180005493:	jne    0x180005431
+   180005495:	jmp    0x180005440
+   180005497:	nopw   0x0(%rax,%rax,1)
+   1800054a0:	mov    %rdx,0x10(%rsp)
+   1800054a5:	push   %rbp
+   1800054a6:	push   %rsi
+   1800054a7:	push   %rdi
+   1800054a8:	sub    $0x20,%rsp
+   1800054ac:	lea    0x80(%rdx),%rbp
+   1800054b3:	mov    -0x30(%rbp),%rcx
+   1800054b7:	mov    0x0(%rbp),%rdx
+   1800054bb:	call   0x1800032f0
+   1800054c0:	nop
+   1800054c1:	add    $0x20,%rsp
+   1800054c5:	pop    %rdi
+   1800054c6:	pop    %rsi
+   1800054c7:	pop    %rbp
+   1800054c8:	ret
+   1800054c9:	int3
+   1800054ca:	int3
+   1800054cb:	int3
+   1800054cc:	int3
+   1800054cd:	int3
+   1800054ce:	int3
+   1800054cf:	int3
+   1800054d0:	push   %rbp
+   1800054d1:	push   %rsi
+   1800054d2:	push   %rdi
+   1800054d3:	sub    $0xa0,%rsp
+   1800054da:	lea    0x80(%rsp),%rbp
+   1800054e2:	movq   $0xfffffffffffffffe,0x18(%rbp)
+   1800054ea:	mov    %rcx,%rsi
+   1800054ed:	call   0x18018e500
+   1800054f2:	lea    0x2584a7(%rip),%rax        # 0x18025d9a0
+   1800054f9:	mov    %rax,-0x40(%rbp)
+   1800054fd:	lea    -0x2784(%rip),%rax        # 0x180002d80
+   180005504:	mov    %rax,-0x38(%rbp)
+   180005508:	lea    0x258511(%rip),%rcx        # 0x18025da20
+   18000550f:	mov    %rcx,-0x30(%rbp)
+   180005513:	mov    %rax,-0x28(%rbp)
+   180005517:	lea    0x2584aa(%rip),%rax        # 0x18025d9c8
+   18000551e:	mov    %rax,-0x10(%rbp)
+   180005522:	movq   $0x3,-0x8(%rbp)
+   18000552a:	movq   $0x0,-0x20(%rbp)
+   180005532:	lea    -0x40(%rbp),%rax
+   180005536:	mov    %rax,0x0(%rbp)
+   18000553a:	movq   $0x2,0x8(%rbp)
+   180005542:	lea    -0x58(%rbp),%rdi
+   180005546:	lea    -0x20(%rbp),%rdx
+   18000554a:	mov    %rdi,%rcx
+   18000554d:	call   0x18017d070
+   180005552:	mov    %rsi,%rcx
+   180005555:	mov    %rdi,%rdx
+   180005558:	call   0x180003490
+   18000555d:	test   %rax,%rax
+   180005560:	je     0x1800055fc
+   180005566:	lea    -0x20(%rbp),%rcx
+   18000556a:	mov    %rax,%rdx
+   18000556d:	call   0x180007c90
+   180005572:	mov    -0x18(%rbp),%rdx
+   180005576:	mov    -0x10(%rbp),%r8
+   18000557a:	mov    %rsi,%rcx
+   18000557d:	mov    %rdx,0x10(%rbp)
+   180005581:	call   0x180008170
+   180005586:	mov    %rax,%rdi
+   180005589:	test   %rax,%rax
+   18000558c:	je     0x1800055d2
+   18000558e:	mov    (%rdi),%eax
+   180005590:	lea    -0x2(%rax),%rcx
+   180005594:	cmp    $0x2,%rcx
+   180005598:	jb     0x1800055bf
+   18000559a:	test   %rax,%rax
+   18000559d:	je     0x1800055bf
+   18000559f:	cmp    $0x1,%eax
+   1800055a2:	jne    0x180005608
+   1800055a4:	lea    0x10(%rdi),%rax
+   1800055a8:	mov    (%rax),%rdx
+   1800055ab:	test   %rdx,%rdx
+   1800055ae:	je     0x1800055bf
+   1800055b0:	mov    0x8(%rax),%rcx
+   1800055b4:	mov    $0x1,%r8d
+   1800055ba:	call   0x180007910
+   1800055bf:	mov    $0x28,%edx
+   1800055c4:	mov    $0x8,%r8d
+   1800055ca:	mov    %rdi,%rcx
+   1800055cd:	call   0x180007910
+   1800055d2:	mov    -0x20(%rbp),%rdx
+   1800055d6:	test   %rdx,%rdx
+   1800055d9:	je     0x1800055ea
+   1800055db:	mov    $0x1,%r8d
+   1800055e1:	mov    0x10(%rbp),%rcx
+   1800055e5:	call   0x180007910
+   1800055ea:	test   %rdi,%rdi
+   1800055ed:	je     0x1800055fc
+   1800055ef:	mov    %rsi,%rcx
+   1800055f2:	mov    $0x2,%edx
+   1800055f7:	call   0x180008290
+   1800055fc:	nop
+   1800055fd:	add    $0xa0,%rsp
+   180005604:	pop    %rdi
+   180005605:	pop    %rsi
+   180005606:	pop    %rbp
+   180005607:	ret
+   180005608:	lea    0x8(%rdi),%rax
+   18000560c:	mov    (%rax),%rdx
+   18000560f:	test   %rdx,%rdx
+   180005612:	jne    0x1800055b0
+   180005614:	jmp    0x1800055bf
+   180005616:	cs nopw 0x0(%rax,%rax,1)
    180005620:	mov    %rdx,0x10(%rsp)
    180005625:	push   %rbp
    180005626:	push   %rsi
    180005627:	push   %rdi
-   180005628:	push   %rbx
-   180005629:	sub    $0x28,%rsp
-   18000562d:	lea    0x40(%rdx),%rbp
-   180005631:	mov    -0x20(%rbp),%rcx
-   180005635:	mov    -0x8(%rbp),%rdx
-   180005639:	call   0x1800032f0
-   18000563e:	nop
-   18000563f:	add    $0x28,%rsp
-   180005643:	pop    %rbx
-   180005644:	pop    %rdi
-   180005645:	pop    %rsi
-   180005646:	pop    %rbp
-   180005647:	ret
-   180005648:	int3
+   180005628:	sub    $0x20,%rsp
+   18000562c:	lea    0x80(%rdx),%rbp
+   180005633:	mov    -0x20(%rbp),%rcx
+   180005637:	mov    0x10(%rbp),%rdx
+   18000563b:	call   0x1800032f0
+   180005640:	nop
+   180005641:	add    $0x20,%rsp
+   180005645:	pop    %rdi
+   180005646:	pop    %rsi
+   180005647:	pop    %rbp
+   180005648:	ret
    180005649:	int3
    18000564a:	int3
    18000564b:	int3
    18000564c:	int3
    18000564d:	int3
    18000564e:	int3
    18000564f:	int3
@@ -113757,15 +113757,15 @@
    1800056aa:	mov    %rax,%rbx
    1800056ad:	jmp    0x180005722
    1800056af:	mov    0x60(%rbp),%r9d
    1800056b3:	mov    %rdi,-0x30(%rbp)
    1800056b7:	mov    %rsi,-0x28(%rbp)
    1800056bb:	xorps  %xmm0,%xmm0
    1800056be:	movups %xmm0,0x30(%rsp)
-   1800056c3:	lea    -0x19a(%rip),%rax        # 0x180005530
+   1800056c3:	lea    -0x1fa(%rip),%rax        # 0x1800054d0
    1800056ca:	mov    %rax,0x28(%rsp)
    1800056cf:	movq   $0x0,0x40(%rsp)
    1800056d8:	movq   $0x1,0x20(%rsp)
    1800056e1:	mov    %r14,%rcx
    1800056e4:	mov    %rdi,%rdx
    1800056e7:	mov    %ebx,%r8d
    1800056ea:	call   0x1800079b0
@@ -113937,15 +113937,15 @@
    1800058ea:	mov    %rax,%rbx
    1800058ed:	jmp    0x180005962
    1800058ef:	mov    0x60(%rbp),%r9d
    1800058f3:	mov    %rdi,-0x30(%rbp)
    1800058f7:	mov    %rsi,-0x28(%rbp)
    1800058fb:	xorps  %xmm0,%xmm0
    1800058fe:	movups %xmm0,0x30(%rsp)
-   180005903:	lea    -0x54a(%rip),%rax        # 0x1800053c0
+   180005903:	lea    -0x5aa(%rip),%rax        # 0x180005360
    18000590a:	mov    %rax,0x28(%rsp)
    18000590f:	movq   $0x0,0x40(%rsp)
    180005918:	movq   $0x1,0x20(%rsp)
    180005921:	mov    %r14,%rcx
    180005924:	mov    %rdi,%rdx
    180005927:	mov    %ebx,%r8d
    18000592a:	call   0x1800079b0
@@ -114013,15 +114013,15 @@
    1800059ce:	int3
    1800059cf:	int3
    1800059d0:	push   %rbp
    1800059d1:	sub    $0x30,%rsp
    1800059d5:	lea    0x30(%rsp),%rbp
    1800059da:	movq   $0xfffffffffffffffe,-0x8(%rbp)
    1800059e2:	mov    %rcx,-0x10(%rbp)
-   1800059e6:	call   0x1800028f0
+   1800059e6:	call   0x1800029c0
    1800059eb:	mov    -0x10(%rbp),%rcx
    1800059ef:	mov    (%rcx),%rax
    1800059f2:	test   %rax,%rax
    1800059f5:	je     0x180005a13
    1800059f7:	mov    0x8(%rcx),%rcx
    1800059fb:	shl    $0x3,%rax
    1800059ff:	lea    (%rax,%rax,4),%rdx
@@ -114337,15 +114337,15 @@
    180005dda:	je     0x180005de9
    180005ddc:	mov    -0x10(%rbp),%rax
    180005de0:	lea    0x20(%rax),%rcx
    180005de4:	call   0x180002410
    180005de9:	mov    -0x10(%rbp),%rsi
    180005ded:	lea    0x40(%rsi),%rcx
    180005df1:	mov    %rcx,-0x18(%rbp)
-   180005df5:	call   0x1800028f0
+   180005df5:	call   0x1800029c0
    180005dfa:	mov    -0x18(%rbp),%rax
    180005dfe:	mov    (%rax),%rax
    180005e01:	test   %rax,%rax
    180005e04:	mov    -0x8(%rbp),%rbx
    180005e08:	je     0x180005e21
    180005e0a:	mov    0x48(%rsi),%rcx
    180005e0e:	shl    $0x3,%rax
@@ -114367,15 +114367,15 @@
    180005e4b:	test   %rdx,%rdx
    180005e4e:	je     0x180005e8a
    180005e50:	mov    0x10(%rax),%r8
    180005e54:	mov    0x8(%rbx),%rcx
    180005e58:	jmp    0x180005e85
    180005e5a:	lea    0x8(%rbx),%rcx
    180005e5e:	mov    %rcx,-0x10(%rbp)
-   180005e62:	call   0x1800029e0
+   180005e62:	call   0x1800028f0
    180005e67:	mov    -0x10(%rbp),%rax
    180005e6b:	mov    (%rax),%rdx
    180005e6e:	test   %rdx,%rdx
    180005e71:	mov    -0x8(%rbp),%rbx
    180005e75:	je     0x180005e8a
    180005e77:	mov    0x10(%rbx),%rcx
    180005e7b:	shl    $0x4,%rdx
@@ -114422,15 +114422,15 @@
    180005f14:	add    $0x90,%rbx
    180005f1b:	mov    %rbx,%rcx
    180005f1e:	add    $0x48,%rsp
    180005f22:	pop    %rbx
    180005f23:	pop    %rdi
    180005f24:	pop    %rsi
    180005f25:	pop    %rbp
-   180005f26:	jmp    0x180006c00
+   180005f26:	jmp    0x180006cd0
    180005f2b:	nop
    180005f2c:	add    $0x48,%rsp
    180005f30:	pop    %rbx
    180005f31:	pop    %rdi
    180005f32:	pop    %rsi
    180005f33:	pop    %rbp
    180005f34:	ret
@@ -114513,15 +114513,15 @@
    180006016:	push   %rsi
    180006017:	push   %rdi
    180006018:	push   %rbx
    180006019:	sub    $0x28,%rsp
    18000601d:	lea    0x40(%rdx),%rbp
    180006021:	mov    -0x8(%rbp),%rax
    180006025:	mov    0x8(%rax),%rcx
-   180006029:	call   0x180006480
+   180006029:	call   0x180006490
    18000602e:	nop
    18000602f:	add    $0x28,%rsp
    180006033:	pop    %rbx
    180006034:	pop    %rdi
    180006035:	pop    %rsi
    180006036:	pop    %rbp
    180006037:	ret
@@ -114701,15 +114701,15 @@
    180006296:	push   %rsi
    180006297:	push   %rdi
    180006298:	push   %rbx
    180006299:	sub    $0x28,%rsp
    18000629d:	lea    0x30(%rdx),%rbp
    1800062a1:	mov    -0x8(%rbp),%rax
    1800062a5:	mov    (%rax),%rcx
-   1800062a8:	call   0x180006490
+   1800062a8:	call   0x180006480
    1800062ad:	nop
    1800062ae:	add    $0x28,%rsp
    1800062b2:	pop    %rbx
    1800062b3:	pop    %rdi
    1800062b4:	pop    %rsi
    1800062b5:	pop    %rbp
    1800062b6:	ret
@@ -114931,24 +114931,24 @@
    18000645c:	int3
    18000645d:	int3
    18000645e:	int3
    18000645f:	int3
    180006460:	mov    (%rcx),%rax
    180006463:	lock decq (%rax)
    180006467:	jne    0x18000646e
-   180006469:	jmp    0x180006c00
+   180006469:	jmp    0x180006cd0
    18000646e:	ret
    18000646f:	int3
    180006470:	mov    $0x98,%edx
    180006475:	mov    $0x8,%r8d
    18000647b:	jmp    0x180007910
-   180006480:	mov    $0x58,%edx
+   180006480:	mov    $0xb0,%edx
    180006485:	mov    $0x8,%r8d
    18000648b:	jmp    0x180007910
-   180006490:	mov    $0xb0,%edx
+   180006490:	mov    $0x58,%edx
    180006495:	mov    $0x8,%r8d
    18000649b:	jmp    0x180007910
    1800064a0:	push   %rbp
    1800064a1:	push   %r15
    1800064a3:	push   %r14
    1800064a5:	push   %r12
    1800064a7:	push   %rsi
@@ -115448,191 +115448,191 @@
    180006bfa:	jmp    0x180007910
    180006bff:	ret
    180006c00:	push   %rbp
    180006c01:	push   %rsi
    180006c02:	sub    $0x38,%rsp
    180006c06:	lea    0x30(%rsp),%rbp
    180006c0b:	movq   $0xfffffffffffffffe,0x0(%rbp)
-   180006c13:	mov    (%rcx),%rax
-   180006c16:	mov    %rax,-0x8(%rbp)
-   180006c1a:	mov    0x110(%rax),%rcx
-   180006c21:	lock decq (%rcx)
-   180006c25:	jne    0x180006c3f
-   180006c27:	mov    -0x8(%rbp),%rax
-   180006c2b:	lea    0x10(%rax),%rdx
-   180006c2f:	mov    %rdx,-0x10(%rbp)
-   180006c33:	mov    0x118(%rax),%rdx
-   180006c3a:	call   0x180006e70
-   180006c3f:	mov    -0x8(%rbp),%rsi
-   180006c43:	mov    0x30(%rsi),%r9
-   180006c47:	test   %r9,%r9
-   180006c4a:	je     0x180006c7e
-   180006c4c:	lea    0x1(%r9),%rax
-   180006c50:	mov    $0x18,%ecx
-   180006c55:	mul    %rcx
-   180006c58:	add    $0xf,%rax
-   180006c5c:	and    $0xfffffffffffffff0,%rax
-   180006c60:	add    %rax,%r9
-   180006c63:	add    $0x11,%r9
-   180006c67:	je     0x180006c7e
-   180006c69:	mov    0x48(%rsi),%rcx
-   180006c6d:	sub    %rax,%rcx
-   180006c70:	mov    $0x10,%r8d
-   180006c76:	mov    %r9,%rdx
-   180006c79:	call   0x180007910
-   180006c7e:	mov    0x70(%rsi),%rdx
-   180006c82:	test   %rdx,%rdx
-   180006c85:	je     0x180006cb0
-   180006c87:	mov    %rdx,%rax
-   180006c8a:	shl    $0x5,%rax
-   180006c8e:	add    %rax,%rdx
-   180006c91:	add    $0x31,%rdx
-   180006c95:	je     0x180006cb0
-   180006c97:	mov    0x88(%rsi),%rcx
-   180006c9e:	sub    %rax,%rcx
-   180006ca1:	add    $0xffffffffffffffe0,%rcx
-   180006ca5:	mov    $0x10,%r8d
-   180006cab:	call   0x180007910
-   180006cb0:	lea    0xb0(%rsi),%rcx
-   180006cb7:	call   0x1800025f0
-   180006cbc:	mov    -0x8(%rbp),%rsi
-   180006cc0:	mov    0xf0(%rsi),%r9
-   180006cc7:	test   %r9,%r9
-   180006cca:	je     0x180006d01
-   180006ccc:	lea    0x1(%r9),%rax
-   180006cd0:	mov    $0x18,%ecx
-   180006cd5:	mul    %rcx
-   180006cd8:	add    $0xf,%rax
-   180006cdc:	and    $0xfffffffffffffff0,%rax
-   180006ce0:	add    %rax,%r9
-   180006ce3:	add    $0x11,%r9
-   180006ce7:	je     0x180006d01
-   180006ce9:	mov    0x108(%rsi),%rcx
-   180006cf0:	sub    %rax,%rcx
-   180006cf3:	mov    $0x10,%r8d
-   180006cf9:	mov    %r9,%rdx
-   180006cfc:	call   0x180007910
-   180006d01:	cmp    $0xffffffffffffffff,%rsi
-   180006d05:	je     0x180006d27
-   180006d07:	lock decq 0x8(%rsi)
-   180006d0c:	jne    0x180006d27
-   180006d0e:	mov    $0x128,%edx
-   180006d13:	mov    $0x8,%r8d
-   180006d19:	mov    %rsi,%rcx
-   180006d1c:	add    $0x38,%rsp
-   180006d20:	pop    %rsi
-   180006d21:	pop    %rbp
-   180006d22:	jmp    0x180007910
-   180006d27:	nop
-   180006d28:	add    $0x38,%rsp
-   180006d2c:	pop    %rsi
-   180006d2d:	pop    %rbp
-   180006d2e:	ret
-   180006d2f:	nop
-   180006d30:	mov    %rdx,0x10(%rsp)
-   180006d35:	push   %rbp
-   180006d36:	push   %rsi
-   180006d37:	sub    $0x28,%rsp
-   180006d3b:	lea    0x30(%rdx),%rbp
-   180006d3f:	mov    -0x10(%rbp),%rcx
-   180006d43:	call   0x180006b80
-   180006d48:	mov    -0x8(%rbp),%rsi
-   180006d4c:	lea    0x50(%rsi),%rcx
-   180006d50:	call   0x180006bd0
-   180006d55:	lea    0x90(%rsi),%rcx
-   180006d5c:	call   0x180006bc0
-   180006d61:	nop
-   180006d62:	add    $0x28,%rsp
-   180006d66:	pop    %rsi
-   180006d67:	pop    %rbp
-   180006d68:	ret
-   180006d69:	nopl   0x0(%rax)
-   180006d70:	mov    %rdx,0x10(%rsp)
-   180006d75:	push   %rbp
-   180006d76:	push   %rsi
-   180006d77:	sub    $0x28,%rsp
-   180006d7b:	lea    0x30(%rdx),%rbp
-   180006d7f:	mov    -0x8(%rbp),%rcx
-   180006d83:	add    $0xd0,%rcx
-   180006d8a:	call   0x180006b80
-   180006d8f:	nop
-   180006d90:	add    $0x28,%rsp
-   180006d94:	pop    %rsi
-   180006d95:	pop    %rbp
-   180006d96:	ret
-   180006d97:	int3
-   180006d98:	int3
-   180006d99:	int3
-   180006d9a:	int3
-   180006d9b:	int3
-   180006d9c:	int3
-   180006d9d:	int3
-   180006d9e:	int3
-   180006d9f:	int3
-   180006da0:	push   %rbp
-   180006da1:	push   %rsi
-   180006da2:	sub    $0x38,%rsp
-   180006da6:	lea    0x30(%rsp),%rbp
-   180006dab:	movq   $0xfffffffffffffffe,0x0(%rbp)
-   180006db3:	mov    (%rcx),%rsi
-   180006db6:	movzbl 0x10(%rsi),%eax
-   180006dba:	cmp    $0x3,%rax
-   180006dbe:	jb     0x180006e0b
-   180006dc0:	cmp    $0x3,%eax
-   180006dc3:	je     0x180006df3
-   180006dc5:	lea    0x18(%rsi),%rcx
-   180006dc9:	cmp    $0x4,%eax
-   180006dcc:	jne    0x180006e31
-   180006dce:	mov    %rcx,-0x8(%rbp)
-   180006dd2:	call   0x180002ab0
-   180006dd7:	mov    -0x8(%rbp),%rax
-   180006ddb:	mov    (%rax),%rdx
-   180006dde:	test   %rdx,%rdx
-   180006de1:	je     0x180006e0b
-   180006de3:	mov    0x20(%rsi),%rcx
-   180006de7:	shl    $0x5,%rdx
-   180006deb:	mov    $0x8,%r8d
-   180006df1:	jmp    0x180006e06
-   180006df3:	mov    0x18(%rsi),%rdx
-   180006df7:	test   %rdx,%rdx
-   180006dfa:	je     0x180006e0b
-   180006dfc:	mov    0x20(%rsi),%rcx
-   180006e00:	mov    $0x1,%r8d
-   180006e06:	call   0x180007910
-   180006e0b:	cmp    $0xffffffffffffffff,%rsi
-   180006e0f:	je     0x180006e3c
-   180006e11:	lock decq 0x8(%rsi)
-   180006e16:	jne    0x180006e3c
-   180006e18:	mov    $0x30,%edx
-   180006e1d:	mov    $0x8,%r8d
-   180006e23:	mov    %rsi,%rcx
-   180006e26:	add    $0x38,%rsp
-   180006e2a:	pop    %rsi
-   180006e2b:	pop    %rbp
-   180006e2c:	jmp    0x180007910
-   180006e31:	call   0x180007400
-   180006e36:	cmp    $0xffffffffffffffff,%rsi
-   180006e3a:	jne    0x180006e11
-   180006e3c:	add    $0x38,%rsp
-   180006e40:	pop    %rsi
-   180006e41:	pop    %rbp
-   180006e42:	ret
-   180006e43:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180006e50:	mov    %rdx,0x10(%rsp)
-   180006e55:	push   %rbp
-   180006e56:	push   %rsi
-   180006e57:	sub    $0x28,%rsp
-   180006e5b:	lea    0x30(%rdx),%rbp
-   180006e5f:	mov    -0x8(%rbp),%rcx
-   180006e63:	call   0x180001100
-   180006e68:	nop
-   180006e69:	add    $0x28,%rsp
-   180006e6d:	pop    %rsi
-   180006e6e:	pop    %rbp
-   180006e6f:	ret
+   180006c13:	mov    (%rcx),%rsi
+   180006c16:	movzbl 0x10(%rsi),%eax
+   180006c1a:	cmp    $0x3,%rax
+   180006c1e:	jb     0x180006c6b
+   180006c20:	cmp    $0x3,%eax
+   180006c23:	je     0x180006c53
+   180006c25:	lea    0x18(%rsi),%rcx
+   180006c29:	cmp    $0x4,%eax
+   180006c2c:	jne    0x180006c91
+   180006c2e:	mov    %rcx,-0x8(%rbp)
+   180006c32:	call   0x180002ab0
+   180006c37:	mov    -0x8(%rbp),%rax
+   180006c3b:	mov    (%rax),%rdx
+   180006c3e:	test   %rdx,%rdx
+   180006c41:	je     0x180006c6b
+   180006c43:	mov    0x20(%rsi),%rcx
+   180006c47:	shl    $0x5,%rdx
+   180006c4b:	mov    $0x8,%r8d
+   180006c51:	jmp    0x180006c66
+   180006c53:	mov    0x18(%rsi),%rdx
+   180006c57:	test   %rdx,%rdx
+   180006c5a:	je     0x180006c6b
+   180006c5c:	mov    0x20(%rsi),%rcx
+   180006c60:	mov    $0x1,%r8d
+   180006c66:	call   0x180007910
+   180006c6b:	cmp    $0xffffffffffffffff,%rsi
+   180006c6f:	je     0x180006c9c
+   180006c71:	lock decq 0x8(%rsi)
+   180006c76:	jne    0x180006c9c
+   180006c78:	mov    $0x30,%edx
+   180006c7d:	mov    $0x8,%r8d
+   180006c83:	mov    %rsi,%rcx
+   180006c86:	add    $0x38,%rsp
+   180006c8a:	pop    %rsi
+   180006c8b:	pop    %rbp
+   180006c8c:	jmp    0x180007910
+   180006c91:	call   0x180007400
+   180006c96:	cmp    $0xffffffffffffffff,%rsi
+   180006c9a:	jne    0x180006c71
+   180006c9c:	add    $0x38,%rsp
+   180006ca0:	pop    %rsi
+   180006ca1:	pop    %rbp
+   180006ca2:	ret
+   180006ca3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   180006cb0:	mov    %rdx,0x10(%rsp)
+   180006cb5:	push   %rbp
+   180006cb6:	push   %rsi
+   180006cb7:	sub    $0x28,%rsp
+   180006cbb:	lea    0x30(%rdx),%rbp
+   180006cbf:	mov    -0x8(%rbp),%rcx
+   180006cc3:	call   0x180001100
+   180006cc8:	nop
+   180006cc9:	add    $0x28,%rsp
+   180006ccd:	pop    %rsi
+   180006cce:	pop    %rbp
+   180006ccf:	ret
+   180006cd0:	push   %rbp
+   180006cd1:	push   %rsi
+   180006cd2:	sub    $0x38,%rsp
+   180006cd6:	lea    0x30(%rsp),%rbp
+   180006cdb:	movq   $0xfffffffffffffffe,0x0(%rbp)
+   180006ce3:	mov    (%rcx),%rax
+   180006ce6:	mov    %rax,-0x8(%rbp)
+   180006cea:	mov    0x110(%rax),%rcx
+   180006cf1:	lock decq (%rcx)
+   180006cf5:	jne    0x180006d0f
+   180006cf7:	mov    -0x8(%rbp),%rax
+   180006cfb:	lea    0x10(%rax),%rdx
+   180006cff:	mov    %rdx,-0x10(%rbp)
+   180006d03:	mov    0x118(%rax),%rdx
+   180006d0a:	call   0x180006e70
+   180006d0f:	mov    -0x8(%rbp),%rsi
+   180006d13:	mov    0x30(%rsi),%r9
+   180006d17:	test   %r9,%r9
+   180006d1a:	je     0x180006d4e
+   180006d1c:	lea    0x1(%r9),%rax
+   180006d20:	mov    $0x18,%ecx
+   180006d25:	mul    %rcx
+   180006d28:	add    $0xf,%rax
+   180006d2c:	and    $0xfffffffffffffff0,%rax
+   180006d30:	add    %rax,%r9
+   180006d33:	add    $0x11,%r9
+   180006d37:	je     0x180006d4e
+   180006d39:	mov    0x48(%rsi),%rcx
+   180006d3d:	sub    %rax,%rcx
+   180006d40:	mov    $0x10,%r8d
+   180006d46:	mov    %r9,%rdx
+   180006d49:	call   0x180007910
+   180006d4e:	mov    0x70(%rsi),%rdx
+   180006d52:	test   %rdx,%rdx
+   180006d55:	je     0x180006d80
+   180006d57:	mov    %rdx,%rax
+   180006d5a:	shl    $0x5,%rax
+   180006d5e:	add    %rax,%rdx
+   180006d61:	add    $0x31,%rdx
+   180006d65:	je     0x180006d80
+   180006d67:	mov    0x88(%rsi),%rcx
+   180006d6e:	sub    %rax,%rcx
+   180006d71:	add    $0xffffffffffffffe0,%rcx
+   180006d75:	mov    $0x10,%r8d
+   180006d7b:	call   0x180007910
+   180006d80:	lea    0xb0(%rsi),%rcx
+   180006d87:	call   0x1800025f0
+   180006d8c:	mov    -0x8(%rbp),%rsi
+   180006d90:	mov    0xf0(%rsi),%r9
+   180006d97:	test   %r9,%r9
+   180006d9a:	je     0x180006dd1
+   180006d9c:	lea    0x1(%r9),%rax
+   180006da0:	mov    $0x18,%ecx
+   180006da5:	mul    %rcx
+   180006da8:	add    $0xf,%rax
+   180006dac:	and    $0xfffffffffffffff0,%rax
+   180006db0:	add    %rax,%r9
+   180006db3:	add    $0x11,%r9
+   180006db7:	je     0x180006dd1
+   180006db9:	mov    0x108(%rsi),%rcx
+   180006dc0:	sub    %rax,%rcx
+   180006dc3:	mov    $0x10,%r8d
+   180006dc9:	mov    %r9,%rdx
+   180006dcc:	call   0x180007910
+   180006dd1:	cmp    $0xffffffffffffffff,%rsi
+   180006dd5:	je     0x180006df7
+   180006dd7:	lock decq 0x8(%rsi)
+   180006ddc:	jne    0x180006df7
+   180006dde:	mov    $0x128,%edx
+   180006de3:	mov    $0x8,%r8d
+   180006de9:	mov    %rsi,%rcx
+   180006dec:	add    $0x38,%rsp
+   180006df0:	pop    %rsi
+   180006df1:	pop    %rbp
+   180006df2:	jmp    0x180007910
+   180006df7:	nop
+   180006df8:	add    $0x38,%rsp
+   180006dfc:	pop    %rsi
+   180006dfd:	pop    %rbp
+   180006dfe:	ret
+   180006dff:	nop
+   180006e00:	mov    %rdx,0x10(%rsp)
+   180006e05:	push   %rbp
+   180006e06:	push   %rsi
+   180006e07:	sub    $0x28,%rsp
+   180006e0b:	lea    0x30(%rdx),%rbp
+   180006e0f:	mov    -0x10(%rbp),%rcx
+   180006e13:	call   0x180006b80
+   180006e18:	mov    -0x8(%rbp),%rsi
+   180006e1c:	lea    0x50(%rsi),%rcx
+   180006e20:	call   0x180006bd0
+   180006e25:	lea    0x90(%rsi),%rcx
+   180006e2c:	call   0x180006bc0
+   180006e31:	nop
+   180006e32:	add    $0x28,%rsp
+   180006e36:	pop    %rsi
+   180006e37:	pop    %rbp
+   180006e38:	ret
+   180006e39:	nopl   0x0(%rax)
+   180006e40:	mov    %rdx,0x10(%rsp)
+   180006e45:	push   %rbp
+   180006e46:	push   %rsi
+   180006e47:	sub    $0x28,%rsp
+   180006e4b:	lea    0x30(%rdx),%rbp
+   180006e4f:	mov    -0x8(%rbp),%rcx
+   180006e53:	add    $0xd0,%rcx
+   180006e5a:	call   0x180006b80
+   180006e5f:	nop
+   180006e60:	add    $0x28,%rsp
+   180006e64:	pop    %rsi
+   180006e65:	pop    %rbp
+   180006e66:	ret
+   180006e67:	int3
+   180006e68:	int3
+   180006e69:	int3
+   180006e6a:	int3
+   180006e6b:	int3
+   180006e6c:	int3
+   180006e6d:	int3
+   180006e6e:	int3
+   180006e6f:	int3
    180006e70:	push   %rsi
    180006e71:	push   %rdi
    180006e72:	push   %rbx
    180006e73:	sub    $0x20,%rsp
    180006e77:	mov    %rdx,%rdi
    180006e7a:	mov    %rcx,%rsi
    180006e7d:	mov    0x10(%rdx),%rbx
@@ -116304,23 +116304,23 @@
    180007890:	test   %rax,%rax
    180007893:	jne    0x1800078e2
    180007895:	movl   $0x801,0x20(%rsp)
    18000789d:	lea    0x25619e(%rip),%rdx        # 0x18025da42
    1800078a4:	mov    $0x10,%r8d
    1800078aa:	mov    %rsi,%rcx
    1800078ad:	xor    %r9d,%r9d
-   1800078b0:	call   0x180005770
+   1800078b0:	call   0x180005650
    1800078b5:	test   %rax,%rax
    1800078b8:	jne    0x1800078e2
    1800078ba:	movl   $0x1,0x20(%rsp)
    1800078c2:	lea    0x256189(%rip),%rdx        # 0x18025da52
    1800078c9:	mov    $0x12,%r8d
    1800078cf:	mov    %rsi,%rcx
    1800078d2:	mov    $0x2,%r9d
-   1800078d8:	call   0x180005650
+   1800078d8:	call   0x180005770
    1800078dd:	test   %rax,%rax
    1800078e0:	je     0x1800078ef
    1800078e2:	mov    %rax,%rcx
    1800078e5:	add    $0x30,%rsp
    1800078e9:	pop    %rsi
    1800078ea:	jmp    0x180007c20
    1800078ef:	xor    %eax,%eax
@@ -120153,15 +120153,15 @@
    18000a9aa:	je     0x18000a9b9
    18000a9ac:	mov    -0x10(%rbp),%rax
    18000a9b0:	lea    0x20(%rax),%rcx
    18000a9b4:	call   0x180038cc0
    18000a9b9:	mov    -0x10(%rbp),%rsi
    18000a9bd:	lea    0x40(%rsi),%rcx
    18000a9c1:	mov    %rcx,-0x18(%rbp)
-   18000a9c5:	call   0x1800028f0
+   18000a9c5:	call   0x1800029c0
    18000a9ca:	mov    -0x18(%rbp),%rax
    18000a9ce:	mov    (%rax),%rax
    18000a9d1:	test   %rax,%rax
    18000a9d4:	mov    -0x8(%rbp),%rbx
    18000a9d8:	je     0x18000a9f1
    18000a9da:	mov    0x48(%rsi),%rcx
    18000a9de:	shl    $0x3,%rax
@@ -120183,15 +120183,15 @@
    18000aa1b:	test   %rdx,%rdx
    18000aa1e:	je     0x18000aa5a
    18000aa20:	mov    0x10(%rax),%r8
    18000aa24:	mov    0x8(%rbx),%rcx
    18000aa28:	jmp    0x18000aa55
    18000aa2a:	lea    0x8(%rbx),%rcx
    18000aa2e:	mov    %rcx,-0x10(%rbp)
-   18000aa32:	call   0x1800029e0
+   18000aa32:	call   0x1800028f0
    18000aa37:	mov    -0x10(%rbp),%rax
    18000aa3b:	mov    (%rax),%rdx
    18000aa3e:	test   %rdx,%rdx
    18000aa41:	mov    -0x8(%rbp),%rbx
    18000aa45:	je     0x18000aa5a
    18000aa47:	mov    0x10(%rbx),%rcx
    18000aa4b:	shl    $0x4,%rdx
@@ -120323,15 +120323,15 @@
    18000abc6:	push   %rsi
    18000abc7:	push   %rdi
    18000abc8:	push   %rbx
    18000abc9:	sub    $0x28,%rsp
    18000abcd:	lea    0x40(%rdx),%rbp
    18000abd1:	mov    -0x8(%rbp),%rax
    18000abd5:	mov    0x8(%rax),%rcx
-   18000abd9:	call   0x180006480
+   18000abd9:	call   0x180006490
    18000abde:	nop
    18000abdf:	add    $0x28,%rsp
    18000abe3:	pop    %rbx
    18000abe4:	pop    %rdi
    18000abe5:	pop    %rsi
    18000abe6:	pop    %rbp
    18000abe7:	ret
@@ -120604,15 +120604,15 @@
    18000af56:	push   %rsi
    18000af57:	push   %rdi
    18000af58:	push   %rbx
    18000af59:	sub    $0x28,%rsp
    18000af5d:	lea    0x40(%rdx),%rbp
    18000af61:	mov    -0x8(%rbp),%rax
    18000af65:	mov    (%rax),%rcx
-   18000af68:	call   0x180006490
+   18000af68:	call   0x180006480
    18000af6d:	nop
    18000af6e:	add    $0x28,%rsp
    18000af72:	pop    %rbx
    18000af73:	pop    %rdi
    18000af74:	pop    %rsi
    18000af75:	pop    %rbp
    18000af76:	ret
@@ -127800,15 +127800,15 @@
    18001100e:	int3
    18001100f:	int3
    180011010:	push   %rbp
    180011011:	sub    $0x30,%rsp
    180011015:	lea    0x30(%rsp),%rbp
    18001101a:	movq   $0xfffffffffffffffe,-0x8(%rbp)
    180011022:	mov    %rcx,-0x10(%rbp)
-   180011026:	call   0x1800029e0
+   180011026:	call   0x1800028f0
    18001102b:	mov    -0x10(%rbp),%rax
    18001102f:	mov    (%rax),%rdx
    180011032:	test   %rdx,%rdx
    180011035:	je     0x18001104f
    180011037:	mov    0x8(%rax),%rcx
    18001103b:	shl    $0x4,%rdx
    18001103f:	mov    $0x8,%r8d
@@ -127875,15 +127875,15 @@
    1800110fe:	int3
    1800110ff:	int3
    180011100:	push   %rbp
    180011101:	sub    $0x30,%rsp
    180011105:	lea    0x30(%rsp),%rbp
    18001110a:	movq   $0xfffffffffffffffe,-0x8(%rbp)
    180011112:	mov    %rcx,-0x10(%rbp)
-   180011116:	call   0x1800028f0
+   180011116:	call   0x1800029c0
    18001111b:	mov    -0x10(%rbp),%rcx
    18001111f:	mov    (%rcx),%rax
    180011122:	test   %rax,%rax
    180011125:	je     0x180011143
    180011127:	mov    0x8(%rcx),%rcx
    18001112b:	shl    $0x3,%rax
    18001112f:	lea    (%rax,%rax,4),%rdx
@@ -128331,15 +128331,15 @@
    1800116e6:	push   %rsi
    1800116e7:	push   %rdi
    1800116e8:	push   %rbx
    1800116e9:	sub    $0x28,%rsp
    1800116ed:	lea    0x40(%rdx),%rbp
    1800116f1:	mov    -0x8(%rbp),%rax
    1800116f5:	mov    (%rax),%rcx
-   1800116f8:	call   0x180006490
+   1800116f8:	call   0x180006480
    1800116fd:	nop
    1800116fe:	add    $0x28,%rsp
    180011702:	pop    %rbx
    180011703:	pop    %rdi
    180011704:	pop    %rsi
    180011705:	pop    %rbp
    180011706:	ret
@@ -128543,15 +128543,15 @@
    18001189c:	je     0x1800118ab
    18001189e:	mov    -0x8(%rbp),%rax
    1800118a2:	lea    0x20(%rax),%rcx
    1800118a6:	call   0x180038cc0
    1800118ab:	mov    -0x8(%rbp),%rsi
    1800118af:	lea    0x40(%rsi),%rcx
    1800118b3:	mov    %rcx,-0x10(%rbp)
-   1800118b7:	call   0x1800028f0
+   1800118b7:	call   0x1800029c0
    1800118bc:	mov    -0x10(%rbp),%rax
    1800118c0:	mov    (%rax),%rax
    1800118c3:	test   %rax,%rax
    1800118c6:	je     0x1800118e5
    1800118c8:	mov    0x48(%rsi),%rcx
    1800118cc:	shl    $0x3,%rax
    1800118d0:	lea    (%rax,%rax,4),%rdx
@@ -135148,15 +135148,15 @@
    180017846:	push   %rsi
    180017847:	push   %rdi
    180017848:	push   %rbx
    180017849:	sub    $0x28,%rsp
    18001784d:	lea    0x30(%rdx),%rbp
    180017851:	mov    -0x8(%rbp),%rax
    180017855:	mov    (%rax),%rcx
-   180017858:	call   0x180006490
+   180017858:	call   0x180006480
    18001785d:	nop
    18001785e:	add    $0x28,%rsp
    180017862:	pop    %rbx
    180017863:	pop    %rdi
    180017864:	pop    %rsi
    180017865:	pop    %rbp
    180017866:	ret
@@ -142246,15 +142246,15 @@
    18001df86:	push   %rsi
    18001df87:	push   %rdi
    18001df88:	push   %rbx
    18001df89:	sub    $0x28,%rsp
    18001df8d:	lea    0x30(%rdx),%rbp
    18001df91:	mov    -0x8(%rbp),%rax
    18001df95:	mov    (%rax),%rcx
-   18001df98:	call   0x180006490
+   18001df98:	call   0x180006480
    18001df9d:	nop
    18001df9e:	add    $0x28,%rsp
    18001dfa2:	pop    %rbx
    18001dfa3:	pop    %rdi
    18001dfa4:	pop    %rsi
    18001dfa5:	pop    %rbp
    18001dfa6:	ret
@@ -152527,15 +152527,15 @@
    180026af6:	push   %rsi
    180026af7:	push   %rdi
    180026af8:	push   %rbx
    180026af9:	sub    $0x28,%rsp
    180026afd:	lea    0x30(%rdx),%rbp
    180026b01:	mov    -0x8(%rbp),%rax
    180026b05:	mov    (%rax),%rcx
-   180026b08:	call   0x180006490
+   180026b08:	call   0x180006480
    180026b0d:	nop
    180026b0e:	add    $0x28,%rsp
    180026b12:	pop    %rbx
    180026b13:	pop    %rdi
    180026b14:	pop    %rsi
    180026b15:	pop    %rbp
    180026b16:	ret
@@ -158411,15 +158411,15 @@
    18002be36:	push   %rsi
    18002be37:	push   %rdi
    18002be38:	push   %rbx
    18002be39:	sub    $0x28,%rsp
    18002be3d:	lea    0x40(%rdx),%rbp
    18002be41:	mov    -0x8(%rbp),%rax
    18002be45:	mov    (%rax),%rcx
-   18002be48:	call   0x180006490
+   18002be48:	call   0x180006480
    18002be4d:	nop
    18002be4e:	add    $0x28,%rsp
    18002be52:	pop    %rbx
    18002be53:	pop    %rdi
    18002be54:	pop    %rsi
    18002be55:	pop    %rbp
    18002be56:	ret
@@ -165166,15 +165166,15 @@
    180032046:	push   %rsi
    180032047:	push   %rdi
    180032048:	push   %rbx
    180032049:	sub    $0x28,%rsp
    18003204d:	lea    0x40(%rdx),%rbp
    180032051:	mov    -0x8(%rbp),%rax
    180032055:	mov    (%rax),%rcx
-   180032058:	call   0x180006490
+   180032058:	call   0x180006480
    18003205d:	nop
    18003205e:	add    $0x28,%rsp
    180032062:	pop    %rbx
    180032063:	pop    %rdi
    180032064:	pop    %rsi
    180032065:	pop    %rbp
    180032066:	ret
@@ -171770,15 +171770,15 @@
    180037eaa:	je     0x180037eb9
    180037eac:	mov    -0x10(%rbp),%rax
    180037eb0:	lea    0x20(%rax),%rcx
    180037eb4:	call   0x180038cc0
    180037eb9:	mov    -0x10(%rbp),%rsi
    180037ebd:	lea    0x40(%rsi),%rcx
    180037ec1:	mov    %rcx,-0x18(%rbp)
-   180037ec5:	call   0x1800028f0
+   180037ec5:	call   0x1800029c0
    180037eca:	mov    -0x18(%rbp),%rax
    180037ece:	mov    (%rax),%rax
    180037ed1:	test   %rax,%rax
    180037ed4:	mov    -0x8(%rbp),%rbx
    180037ed8:	je     0x180037ef1
    180037eda:	mov    0x48(%rsi),%rcx
    180037ede:	shl    $0x3,%rax
@@ -171800,15 +171800,15 @@
    180037f1b:	test   %rdx,%rdx
    180037f1e:	je     0x180037f5a
    180037f20:	mov    0x10(%rax),%r8
    180037f24:	mov    0x8(%rbx),%rcx
    180037f28:	jmp    0x180037f55
    180037f2a:	lea    0x8(%rbx),%rcx
    180037f2e:	mov    %rcx,-0x10(%rbp)
-   180037f32:	call   0x1800029e0
+   180037f32:	call   0x1800028f0
    180037f37:	mov    -0x10(%rbp),%rax
    180037f3b:	mov    (%rax),%rdx
    180037f3e:	test   %rdx,%rdx
    180037f41:	mov    -0x8(%rbp),%rbx
    180037f45:	je     0x180037f5a
    180037f47:	mov    0x10(%rbx),%rcx
    180037f4b:	shl    $0x4,%rdx
@@ -171940,15 +171940,15 @@
    1800380c6:	push   %rsi
    1800380c7:	push   %rdi
    1800380c8:	push   %rbx
    1800380c9:	sub    $0x28,%rsp
    1800380cd:	lea    0x40(%rdx),%rbp
    1800380d1:	mov    -0x8(%rbp),%rax
    1800380d5:	mov    0x8(%rax),%rcx
-   1800380d9:	call   0x180006480
+   1800380d9:	call   0x180006490
    1800380de:	nop
    1800380df:	add    $0x28,%rsp
    1800380e3:	pop    %rbx
    1800380e4:	pop    %rdi
    1800380e5:	pop    %rsi
    1800380e6:	pop    %rbp
    1800380e7:	ret
@@ -178936,15 +178936,15 @@
    18003dd6e:	int3
    18003dd6f:	int3
    18003dd70:	push   %rbp
    18003dd71:	sub    $0x30,%rsp
    18003dd75:	lea    0x30(%rsp),%rbp
    18003dd7a:	movq   $0xfffffffffffffffe,-0x8(%rbp)
    18003dd82:	mov    %rcx,-0x10(%rbp)
-   18003dd86:	call   0x1800028f0
+   18003dd86:	call   0x1800029c0
    18003dd8b:	mov    -0x10(%rbp),%rcx
    18003dd8f:	mov    (%rcx),%rax
    18003dd92:	test   %rax,%rax
    18003dd95:	je     0x18003ddb3
    18003dd97:	mov    0x8(%rcx),%rcx
    18003dd9b:	shl    $0x3,%rax
    18003dd9f:	lea    (%rax,%rax,4),%rdx
@@ -180451,15 +180451,15 @@
    18003f05a:	je     0x18003f069
    18003f05c:	mov    -0x10(%rbp),%rax
    18003f060:	lea    0x20(%rax),%rcx
    18003f064:	call   0x180038cc0
    18003f069:	mov    -0x10(%rbp),%rsi
    18003f06d:	lea    0x40(%rsi),%rcx
    18003f071:	mov    %rcx,-0x18(%rbp)
-   18003f075:	call   0x1800028f0
+   18003f075:	call   0x1800029c0
    18003f07a:	mov    -0x18(%rbp),%rax
    18003f07e:	mov    (%rax),%rax
    18003f081:	test   %rax,%rax
    18003f084:	mov    -0x8(%rbp),%rbx
    18003f088:	je     0x18003f0a1
    18003f08a:	mov    0x48(%rsi),%rcx
    18003f08e:	shl    $0x3,%rax
@@ -180481,15 +180481,15 @@
    18003f0cb:	test   %rdx,%rdx
    18003f0ce:	je     0x18003f10a
    18003f0d0:	mov    0x10(%rax),%r8
    18003f0d4:	mov    0x8(%rbx),%rcx
    18003f0d8:	jmp    0x18003f105
    18003f0da:	lea    0x8(%rbx),%rcx
    18003f0de:	mov    %rcx,-0x10(%rbp)
-   18003f0e2:	call   0x1800029e0
+   18003f0e2:	call   0x1800028f0
    18003f0e7:	mov    -0x10(%rbp),%rax
    18003f0eb:	mov    (%rax),%rdx
    18003f0ee:	test   %rdx,%rdx
    18003f0f1:	mov    -0x8(%rbp),%rbx
    18003f0f5:	je     0x18003f10a
    18003f0f7:	mov    0x10(%rbx),%rcx
    18003f0fb:	shl    $0x4,%rdx
@@ -180621,15 +180621,15 @@
    18003f276:	push   %rsi
    18003f277:	push   %rdi
    18003f278:	push   %rbx
    18003f279:	sub    $0x28,%rsp
    18003f27d:	lea    0x40(%rdx),%rbp
    18003f281:	mov    -0x8(%rbp),%rax
    18003f285:	mov    0x8(%rax),%rcx
-   18003f289:	call   0x180006480
+   18003f289:	call   0x180006490
    18003f28e:	nop
    18003f28f:	add    $0x28,%rsp
    18003f293:	pop    %rbx
    18003f294:	pop    %rdi
    18003f295:	pop    %rsi
    18003f296:	pop    %rbp
    18003f297:	ret
@@ -181090,15 +181090,15 @@
    18003f8c6:	push   %rsi
    18003f8c7:	push   %rdi
    18003f8c8:	push   %rbx
    18003f8c9:	sub    $0x28,%rsp
    18003f8cd:	lea    0x40(%rdx),%rbp
    18003f8d1:	mov    -0x8(%rbp),%rax
    18003f8d5:	mov    (%rax),%rcx
-   18003f8d8:	call   0x180006490
+   18003f8d8:	call   0x180006480
    18003f8dd:	nop
    18003f8de:	add    $0x28,%rsp
    18003f8e2:	pop    %rbx
    18003f8e3:	pop    %rdi
    18003f8e4:	pop    %rsi
    18003f8e5:	pop    %rbp
    18003f8e6:	ret
@@ -194428,15 +194428,15 @@
    18004b44a:	je     0x18004b459
    18004b44c:	mov    -0x10(%rbp),%rax
    18004b450:	lea    0x20(%rax),%rcx
    18004b454:	call   0x180038cc0
    18004b459:	mov    -0x10(%rbp),%rsi
    18004b45d:	lea    0x40(%rsi),%rcx
    18004b461:	mov    %rcx,-0x18(%rbp)
-   18004b465:	call   0x1800028f0
+   18004b465:	call   0x1800029c0
    18004b46a:	mov    -0x18(%rbp),%rax
    18004b46e:	mov    (%rax),%rax
    18004b471:	test   %rax,%rax
    18004b474:	mov    -0x8(%rbp),%rbx
    18004b478:	je     0x18004b491
    18004b47a:	mov    0x48(%rsi),%rcx
    18004b47e:	shl    $0x3,%rax
@@ -194458,15 +194458,15 @@
    18004b4bb:	test   %rdx,%rdx
    18004b4be:	je     0x18004b4fa
    18004b4c0:	mov    0x10(%rax),%r8
    18004b4c4:	mov    0x8(%rbx),%rcx
    18004b4c8:	jmp    0x18004b4f5
    18004b4ca:	lea    0x8(%rbx),%rcx
    18004b4ce:	mov    %rcx,-0x10(%rbp)
-   18004b4d2:	call   0x1800029e0
+   18004b4d2:	call   0x1800028f0
    18004b4d7:	mov    -0x10(%rbp),%rax
    18004b4db:	mov    (%rax),%rdx
    18004b4de:	test   %rdx,%rdx
    18004b4e1:	mov    -0x8(%rbp),%rbx
    18004b4e5:	je     0x18004b4fa
    18004b4e7:	mov    0x10(%rbx),%rcx
    18004b4eb:	shl    $0x4,%rdx
@@ -194598,15 +194598,15 @@
    18004b666:	push   %rsi
    18004b667:	push   %rdi
    18004b668:	push   %rbx
    18004b669:	sub    $0x28,%rsp
    18004b66d:	lea    0x40(%rdx),%rbp
    18004b671:	mov    -0x8(%rbp),%rax
    18004b675:	mov    0x8(%rax),%rcx
-   18004b679:	call   0x180006480
+   18004b679:	call   0x180006490
    18004b67e:	nop
    18004b67f:	add    $0x28,%rsp
    18004b683:	pop    %rbx
    18004b684:	pop    %rdi
    18004b685:	pop    %rsi
    18004b686:	pop    %rbp
    18004b687:	ret
@@ -194796,15 +194796,15 @@
    18004b8e6:	push   %rsi
    18004b8e7:	push   %rdi
    18004b8e8:	push   %rbx
    18004b8e9:	sub    $0x28,%rsp
    18004b8ed:	lea    0x30(%rdx),%rbp
    18004b8f1:	mov    -0x8(%rbp),%rax
    18004b8f5:	mov    (%rax),%rcx
-   18004b8f8:	call   0x180006490
+   18004b8f8:	call   0x180006480
    18004b8fd:	nop
    18004b8fe:	add    $0x28,%rsp
    18004b902:	pop    %rbx
    18004b903:	pop    %rdi
    18004b904:	pop    %rsi
    18004b905:	pop    %rbp
    18004b906:	ret
@@ -199018,15 +199018,15 @@
    18004fec8:	mov    0x180(%rbp),%rdx
    18004fecf:	test   %rdx,%rdx
    18004fed2:	je     0x18004fee6
    18004fed4:	mov    0x188(%rbp),%rcx
    18004fedb:	mov    $0x1,%r8d
    18004fee1:	call   0x180007910
    18004fee6:	lea    0x438(%rbp),%rcx
-   18004feed:	call   0x1800028f0
+   18004feed:	call   0x1800029c0
    18004fef2:	mov    0x438(%rbp),%rax
    18004fef9:	test   %rax,%rax
    18004fefc:	je     0x18004ff18
    18004fefe:	mov    0x440(%rbp),%rcx
    18004ff05:	shl    $0x3,%rax
    18004ff09:	lea    (%rax,%rax,4),%rdx
    18004ff0d:	mov    $0x8,%r8d
@@ -199137,15 +199137,15 @@
    18005016d:	lea    0x1f0(%rbp),%rcx
    180050174:	call   0x18017cb90
    180050179:	jmp    0x180051034
    18005017e:	mov    0x450(%rbp),%r14
    180050185:	mov    0x458(%rbp),%r12
    18005018c:	mov    0x460(%rbp),%rsi
    180050193:	lea    0x438(%rbp),%rcx
-   18005019a:	call   0x1800028f0
+   18005019a:	call   0x1800029c0
    18005019f:	mov    0x438(%rbp),%rax
    1800501a6:	test   %rax,%rax
    1800501a9:	je     0x1800501c5
    1800501ab:	mov    0x440(%rbp),%rcx
    1800501b2:	shl    $0x3,%rax
    1800501b6:	lea    (%rax,%rax,4),%rdx
    1800501ba:	mov    $0x8,%r8d
@@ -199774,15 +199774,15 @@
    180050f83:	mov    0x288(%rbp),%rcx
    180050f8a:	mov    $0x1,%r8d
    180050f90:	call   0x180007910
    180050f95:	lea    0x3c0(%rbp),%rcx
    180050f9c:	movb   $0x1,0x722(%rbp)
    180050fa3:	call   0x180038cc0
    180050fa8:	lea    0x570(%rbp),%rcx
-   180050faf:	call   0x1800028f0
+   180050faf:	call   0x1800029c0
    180050fb4:	mov    0x570(%rbp),%rax
    180050fbb:	test   %rax,%rax
    180050fbe:	je     0x180050fda
    180050fc0:	mov    0x578(%rbp),%rcx
    180050fc7:	shl    $0x3,%rax
    180050fcb:	lea    (%rax,%rax,4),%rdx
    180050fcf:	mov    $0x8,%r8d
@@ -206328,15 +206328,15 @@
    1800576a3:	lea    0x80(%rsp),%rbp
    1800576ab:	movq   $0xfffffffffffffffe,0x90(%rbp)
    1800576b6:	mov    %rcx,%rsi
    1800576b9:	mov    %rdx,0x48(%rbp)
    1800576bd:	mov    %r8b,0x50(%rbp)
    1800576c1:	lea    0x70(%rbp),%rcx
    1800576c5:	lea    0x48(%rbp),%rdx
-   1800576c9:	call   0x180004f50
+   1800576c9:	call   0x180004d80
    1800576ce:	cmpq   $0x0,0x70(%rbp)
    1800576d3:	mov    0x78(%rbp),%rdi
    1800576d7:	je     0x1800576e5
    1800576d9:	mov    %rdi,0x8(%rsi)
    1800576dd:	movb   $0x6,(%rsi)
    1800576e0:	jmp    0x1800577f2
    1800576e5:	mov    0x80(%rbp),%rbx
@@ -206445,15 +206445,15 @@
    180057885:	lea    0x28(%rbp),%rcx
    180057889:	call   0x18000a2d0
    18005788e:	lea    0x28(%rbp),%rdi
    180057892:	lea    0x48(%rbp),%rbx
    180057896:	lea    0x70(%rbp),%r14
    18005789a:	mov    %rdi,%rcx
    18005789d:	mov    %rbx,%rdx
-   1800578a0:	call   0x180004d80
+   1800578a0:	call   0x180004f10
    1800578a5:	cmpq   $0x0,0x28(%rbp)
    1800578aa:	jne    0x1800579e6
    1800578b0:	mov    0x38(%rbp),%r12
    1800578b4:	test   %r12,%r12
    1800578b7:	je     0x1800579ec
    1800578bd:	mov    0x30(%rbp),%r15
    1800578c1:	mov    0x40(%rbp),%rax
@@ -208450,15 +208450,15 @@
    1800592e6:	push   %rsi
    1800592e7:	push   %rdi
    1800592e8:	push   %rbx
    1800592e9:	sub    $0x28,%rsp
    1800592ed:	lea    0x40(%rdx),%rbp
    1800592f1:	mov    -0x8(%rbp),%rax
    1800592f5:	mov    (%rax),%rcx
-   1800592f8:	call   0x180006490
+   1800592f8:	call   0x180006480
    1800592fd:	nop
    1800592fe:	add    $0x28,%rsp
    180059302:	pop    %rbx
    180059303:	pop    %rdi
    180059304:	pop    %rsi
    180059305:	pop    %rbp
    180059306:	ret
@@ -210875,15 +210875,15 @@
    18005b72d:	mov    0xc0(%rbp),%eax
    18005b733:	mov    %eax,0x9c(%rcx)
    18005b739:	movq   $0x0,0xa0(%rcx)
    18005b744:	movq   $0x8,0xa8(%rcx)
    18005b74f:	movq   $0x0,0xb0(%rcx)
    18005b75a:	movq   $0x1,(%rcx)
    18005b761:	lea    0x1a8(%rbp),%rcx
-   18005b768:	call   0x1800028f0
+   18005b768:	call   0x1800029c0
    18005b76d:	lea    0x2f0(%rbp),%rcx
    18005b774:	movb   $0x0,0x3c5(%rbp)
    18005b77b:	call   0x180038cc0
    18005b780:	jmp    0x18005c4ab
    18005b785:	mov    $0x8,%eax
    18005b78a:	jmp    0x18005b90f
    18005b78f:	mov    $0x1,%ebx
@@ -210917,15 +210917,15 @@
    18005b814:	movups %xmm0,0x98(%rax)
    18005b81b:	movq   $0x8,0xa8(%rax)
    18005b826:	movq   $0x0,0xb0(%rax)
    18005b831:	movq   $0x0,0x8(%rax)
    18005b839:	movl   $0x14,0x48(%rax)
    18005b840:	movq   $0x1,(%rax)
    18005b847:	lea    0x1a8(%rbp),%rcx
-   18005b84e:	call   0x1800028f0
+   18005b84e:	call   0x1800029c0
    18005b853:	lea    0x2f0(%rbp),%rcx
    18005b85a:	movb   $0x1,0x3c5(%rbp)
    18005b861:	call   0x180038cc0
    18005b866:	jmp    0x18005c43f
    18005b86b:	mov    0x1d0(%rbp),%rcx
    18005b872:	mov    %rcx,0x280(%rbp)
    18005b879:	movups 0x1c1(%rbp),%xmm0
@@ -211479,15 +211479,15 @@
    18005c3eb:	mov    0x60(%rbp),%rcx
    18005c3ef:	mov    $0x1,%r8d
    18005c3f5:	call   0x180007910
    18005c3fa:	lea    0x2f0(%rbp),%rcx
    18005c401:	movb   $0x1,0x3c4(%rbp)
    18005c408:	call   0x180038cc0
    18005c40d:	lea    0x370(%rbp),%rcx
-   18005c414:	call   0x1800028f0
+   18005c414:	call   0x1800029c0
    18005c419:	mov    0x370(%rbp),%rax
    18005c420:	test   %rax,%rax
    18005c423:	je     0x18005c43f
    18005c425:	mov    0x378(%rbp),%rcx
    18005c42c:	shl    $0x3,%rax
    18005c430:	lea    (%rax,%rax,4),%rdx
    18005c434:	mov    $0x8,%r8d
@@ -224761,15 +224761,15 @@
    18006812a:	je     0x180068139
    18006812c:	mov    -0x10(%rbp),%rax
    180068130:	lea    0x20(%rax),%rcx
    180068134:	call   0x180038cc0
    180068139:	mov    -0x10(%rbp),%rsi
    18006813d:	lea    0x40(%rsi),%rcx
    180068141:	mov    %rcx,-0x18(%rbp)
-   180068145:	call   0x1800028f0
+   180068145:	call   0x1800029c0
    18006814a:	mov    -0x18(%rbp),%rax
    18006814e:	mov    (%rax),%rax
    180068151:	test   %rax,%rax
    180068154:	mov    -0x8(%rbp),%rbx
    180068158:	je     0x180068171
    18006815a:	mov    0x48(%rsi),%rcx
    18006815e:	shl    $0x3,%rax
@@ -224791,15 +224791,15 @@
    18006819b:	test   %rdx,%rdx
    18006819e:	je     0x1800681da
    1800681a0:	mov    0x10(%rax),%r8
    1800681a4:	mov    0x8(%rbx),%rcx
    1800681a8:	jmp    0x1800681d5
    1800681aa:	lea    0x8(%rbx),%rcx
    1800681ae:	mov    %rcx,-0x10(%rbp)
-   1800681b2:	call   0x1800029e0
+   1800681b2:	call   0x1800028f0
    1800681b7:	mov    -0x10(%rbp),%rax
    1800681bb:	mov    (%rax),%rdx
    1800681be:	test   %rdx,%rdx
    1800681c1:	mov    -0x8(%rbp),%rbx
    1800681c5:	je     0x1800681da
    1800681c7:	mov    0x10(%rbx),%rcx
    1800681cb:	shl    $0x4,%rdx
@@ -224931,15 +224931,15 @@
    180068346:	push   %rsi
    180068347:	push   %rdi
    180068348:	push   %rbx
    180068349:	sub    $0x28,%rsp
    18006834d:	lea    0x40(%rdx),%rbp
    180068351:	mov    -0x8(%rbp),%rax
    180068355:	mov    0x8(%rax),%rcx
-   180068359:	call   0x180006480
+   180068359:	call   0x180006490
    18006835e:	nop
    18006835f:	add    $0x28,%rsp
    180068363:	pop    %rbx
    180068364:	pop    %rdi
    180068365:	pop    %rsi
    180068366:	pop    %rbp
    180068367:	ret
@@ -225148,15 +225148,15 @@
    180068606:	push   %rsi
    180068607:	push   %rdi
    180068608:	push   %rbx
    180068609:	sub    $0x28,%rsp
    18006860d:	lea    0x30(%rdx),%rbp
    180068611:	mov    -0x8(%rbp),%rax
    180068615:	mov    (%rax),%rcx
-   180068618:	call   0x180006490
+   180068618:	call   0x180006480
    18006861d:	nop
    18006861e:	add    $0x28,%rsp
    180068622:	pop    %rbx
    180068623:	pop    %rdi
    180068624:	pop    %rsi
    180068625:	pop    %rbp
    180068626:	ret
@@ -228052,15 +228052,15 @@
    18006ac2e:	mov    0xb0(%rbp),%eax
    18006ac34:	mov    %eax,0x9c(%rcx)
    18006ac3a:	movq   $0x0,0xa0(%rcx)
    18006ac45:	movq   $0x8,0xa8(%rcx)
    18006ac50:	movq   $0x0,0xb0(%rcx)
    18006ac5b:	movq   $0x1,(%rcx)
    18006ac62:	lea    0x2e0(%rbp),%rcx
-   18006ac69:	call   0x1800028f0
+   18006ac69:	call   0x1800029c0
    18006ac6e:	lea    0x260(%rbp),%rcx
    18006ac75:	movb   $0x0,0x3a5(%rbp)
    18006ac7c:	call   0x180038cc0
    18006ac81:	jmp    0x18006b9ab
    18006ac86:	mov    $0x8,%eax
    18006ac8b:	jmp    0x18006ae34
    18006ac90:	mov    $0x1,%ecx
@@ -228092,15 +228092,15 @@
    18006ad1b:	movups %xmm0,0x98(%rax)
    18006ad22:	movq   $0x8,0xa8(%rax)
    18006ad2d:	movq   $0x0,0xb0(%rax)
    18006ad38:	movq   $0x0,0x8(%rax)
    18006ad40:	movl   $0x14,0x48(%rax)
    18006ad47:	movq   $0x1,(%rax)
    18006ad4e:	lea    0x2e0(%rbp),%rcx
-   18006ad55:	call   0x1800028f0
+   18006ad55:	call   0x1800029c0
    18006ad5a:	lea    0x260(%rbp),%rcx
    18006ad61:	movb   $0x1,0x3a5(%rbp)
    18006ad68:	call   0x180038cc0
    18006ad6d:	jmp    0x18006b93f
    18006ad72:	movzbl %bl,%eax
    18006ad75:	mov    %rax,0x360(%rbp)
    18006ad7c:	movzbl 0x197(%rbp),%eax
@@ -228659,15 +228659,15 @@
    18006b8eb:	mov    0x50(%rbp),%rcx
    18006b8ef:	mov    $0x1,%r8d
    18006b8f5:	call   0x180007910
    18006b8fa:	lea    0x2c0(%rbp),%rcx
    18006b901:	movb   $0x1,0x3a4(%rbp)
    18006b908:	call   0x180038cc0
    18006b90d:	lea    0x340(%rbp),%rcx
-   18006b914:	call   0x1800028f0
+   18006b914:	call   0x1800029c0
    18006b919:	mov    0x340(%rbp),%rax
    18006b920:	test   %rax,%rax
    18006b923:	je     0x18006b93f
    18006b925:	mov    0x348(%rbp),%rcx
    18006b92c:	shl    $0x3,%rax
    18006b930:	lea    (%rax,%rax,4),%rdx
    18006b934:	mov    $0x8,%r8d
@@ -257765,15 +257765,15 @@
    18008962a:	mov    0xb0(%rbp),%eax
    180089630:	mov    %eax,0x9c(%rcx)
    180089636:	movq   $0x0,0xa0(%rcx)
    180089641:	movq   $0x8,0xa8(%rcx)
    18008964c:	movq   $0x0,0xb0(%rcx)
    180089657:	movq   $0x1,(%rcx)
    18008965e:	lea    0x1e8(%rbp),%rcx
-   180089665:	call   0x1800028f0
+   180089665:	call   0x1800029c0
    18008966a:	lea    0x1b0(%rbp),%rcx
    180089671:	movb   $0x0,0x3a5(%rbp)
    180089678:	call   0x180038cc0
    18008967d:	jmp    0x18008a3ab
    180089682:	mov    $0x8,%eax
    180089687:	jmp    0x18008982f
    18008968c:	mov    $0x1,%ecx
@@ -257805,15 +257805,15 @@
    180089717:	movups %xmm0,0x98(%rax)
    18008971e:	movq   $0x8,0xa8(%rax)
    180089729:	movq   $0x0,0xb0(%rax)
    180089734:	movq   $0x0,0x8(%rax)
    18008973c:	movl   $0x14,0x48(%rax)
    180089743:	movq   $0x1,(%rax)
    18008974a:	lea    0x1e8(%rbp),%rcx
-   180089751:	call   0x1800028f0
+   180089751:	call   0x1800029c0
    180089756:	lea    0x1b0(%rbp),%rcx
    18008975d:	movb   $0x1,0x3a5(%rbp)
    180089764:	call   0x180038cc0
    180089769:	jmp    0x18008a33f
    18008976e:	movzbl %bl,%eax
    180089771:	mov    %rax,0x370(%rbp)
    180089778:	movzbl 0x247(%rbp),%eax
@@ -258373,15 +258373,15 @@
    18008a2eb:	mov    0x50(%rbp),%rcx
    18008a2ef:	mov    $0x1,%r8d
    18008a2f5:	call   0x180007910
    18008a2fa:	lea    0x220(%rbp),%rcx
    18008a301:	movb   $0x1,0x3a4(%rbp)
    18008a308:	call   0x180038cc0
    18008a30d:	lea    0x350(%rbp),%rcx
-   18008a314:	call   0x1800028f0
+   18008a314:	call   0x1800029c0
    18008a319:	mov    0x350(%rbp),%rax
    18008a320:	test   %rax,%rax
    18008a323:	je     0x18008a33f
    18008a325:	mov    0x358(%rbp),%rcx
    18008a32c:	shl    $0x3,%rax
    18008a330:	lea    (%rax,%rax,4),%rdx
    18008a334:	mov    $0x8,%r8d
@@ -776453,15 +776453,15 @@
    18025d989:	add    %al,(%rax)
    18025d98b:	add    %al,(%rax)
    18025d98d:	add    %al,(%rax)
    18025d98f:	add    %dh,(%rax)
    18025d991:	cs xor (%rsi),%ch
    18025d994:	xor    0x68706c61(%rip),%ebp        # 0x1e89645fb
    18025d99a:	(bad)
-   18025d99b:	cs xor (%rax),%al
+   18025d99b:	cs xor (%rax),%eax
    18025d99e:	add    %al,(%rax)
    18025d9a0:	nop
    18025d9a1:	fldenv 0x180(%rip)        # 0x18025db27
    18025d9a7:	add    %cl,0x0(%rip)        # 0x18025d9ad
    18025d9ad:	add    %al,(%rax)
    18025d9af:	add    %dl,0x65(%rsi)
    18025d9b2:	jb     0x18025da27
@@ -776487,34 +776487,37 @@
    18025d9e5:	add    %al,(%rax)
    18025d9e7:	add    %al,%bl
    18025d9e9:	fldenv 0x180(%rip)        # 0x18025db6f
    18025d9ef:	add    %al,(%rcx)
    18025d9f1:	add    %al,(%rax)
    18025d9f3:	add    %al,(%rax)
    18025d9f5:	add    %al,(%rax)
-   18025d9f7:	add    %dh,(%rdx)
-   18025d9f9:	ss xor (%rsi),%dh
-   18025d9fc:	movsxd (%rcx),%esi
-   18025d9fe:	data16 xor 0x33383533(%rip),%dh        # 0x1b35e0f38
-   18025da05:	cmp    %dh,(%rsi,%rsi,1)
-   18025da08:	ss data16 xor %dh,(%rdi)
-   18025da0c:	ss cmp %esi,(%rcx)
-   18025da0f:	xor    %esp,0x65(%rsi)
-   18025da12:	cmp    %bh,(%rax)
-   18025da14:	xor    $0x35,%al
-   18025da16:	ss cmp %esp,0x33(%rbx)
-   18025da1a:	data16 xor $0x34,%al
-   18025da1d:	cmp    %bh,(%rax)
-   18025da1f:	xor    %edi,%eax
-   18025da21:	fldenv 0x180(%rip)        # 0x18025dba7
-   18025da27:	add    %ch,(%rax)
-   18025da29:	add    %al,(%rax)
-   18025da2b:	add    %al,(%rax)
-   18025da2d:	add    %al,(%rax)
-   18025da2f:	add    %ch,0x73(%rdx)
+   18025d9f7:	add    %ah,0x33(%rbx)
+   18025d9fa:	(bad)
+   18025d9fb:	xor    %bh,(%rax)
+   18025d9fd:	xor    (%rax),%bh
+   18025d9ff:	fs xor %esp,%gs:0x64(%rcx)
+   18025da04:	xor    0x65343863(%rip),%dh        # 0x1e55a126d
+   18025da0a:	xor    $0x39,%al
+   18025da0c:	xor    %esi,0x39313263(%rip)        # 0x1b9570c75
+   18025da12:	movsxd %fs:(%rsi),%esi
+   18025da15:	(bad)
+   18025da16:	cmp    %dh,(%rcx)
+   18025da18:	(bad)
+   18025da19:	xor    (%rax),%bh
+   18025da1b:	xor    %esi,(%rax)
+   18025da1d:	xor    (%rax),%dh
+   18025da1f:	xor    $0x8025d9f8,%eax
+   18025da24:	add    %eax,(%rax)
+   18025da26:	add    %al,(%rax)
+   18025da28:	sub    %al,(%rax)
+   18025da2a:	add    %al,(%rax)
+   18025da2c:	add    %al,(%rax)
+   18025da2e:	add    %al,(%rax)
+   18025da30:	push   $0x73
    18025da32:	outsl  %ds:(%rsi),(%dx)
    18025da33:	outsb  %ds:(%rsi),(%dx)
    18025da34:	jae    0x18025da99
    18025da36:	push   $0x5f616d65
    18025da3b:	jbe    0x18025daa2
    18025da3d:	jb     0x18025dab2
    18025da3f:	imul   $0x6e6f736a,0x6e(%rdi),%ebp
@@ -1095363,38 +1095366,37 @@
    18031836d:	add    %al,(%rax)
    18031836f:	add    %ch,0x18025d4(%rax)
    180318375:	add    %al,(%rax)
    180318377:	add    %dh,0x18025d4(%rax)
    18031837d:	add    %al,(%rax)
    18031837f:	add    %al,(%rax)
    180318381:	add    %al,(%rax)
-   180318383:	add    %bh,%bl
-   180318385:	roll   $0x0,0x64(%rax)
-   18031838c:	add    (%rax),%al
-   18031838e:	add    %al,(%rax)
-   180318390:	imul   $0x0,(%rax),%eax
-   180318393:	add    %ah,(%rax)
-   180318395:	xchg   %dh,(%rcx)
-   180318397:	add    %ah,(%rax)
-   180318399:	jp     0x1803183cc
-   18031839b:	add    %al,(%rax)
-   18031839d:	add    %al,(%rax)
-   18031839f:	add    %bh,%bl
-   1803183a1:	roll   $0x0,0x64(%rax)
-   1803183a8:	or     $0x0,%al
+   180318383:	add    %ch,0x6480c7(%rcx)
+   180318389:	add    %al,(%rax)
+   18031838b:	add    %al,(%rdx)
+   18031838d:	add    %al,(%rax)
+   18031838f:	add    %ch,0x0(%rbx)
+   180318392:	add    %al,(%rax)
+   180318394:	and    %al,0x7a200031(%rsi)
+   18031839a:	xor    %eax,(%rax)
+   18031839c:	add    %al,(%rax)
+   18031839e:	add    %al,(%rax)
+   1803183a0:	test   $0x6480c7,%eax
+   1803183a5:	add    %al,(%rax)
+   1803183a7:	add    %cl,(%rax,%rax,1)
    1803183aa:	add    %al,(%rax)
    1803183ac:	adc    $0x0,%al
    1803183ae:	add    %al,(%rax)
    1803183b0:	mov    %es,0x7a8c0031(%rsi)
    1803183b6:	xor    %eax,(%rax)
    1803183b8:	add    %al,(%rax)
    1803183ba:	add    %al,(%rax)
-   1803183bc:	sti
-   1803183bd:	roll   $0x0,0x64(%rax)
-   1803183c4:	or     $0x18000000,%eax
+   1803183bc:	test   $0x6480c7,%eax
+   1803183c1:	add    %al,(%rax)
+   1803183c3:	add    %cl,0x18000000(%rip)        # 0x1983183c9
    1803183c9:	add    (%rax),%eax
    1803183cb:	add    %ah,-0x5fffce7a(%rax)
    1803183d1:	jp     0x180318404
 	...
    1803183ff:	add    %bl,%al
    180318401:	mov    %esi,(%rcx)
    180318403:	addb   $0x0,(%rcx)
@@ -1095590,23 +1095592,22 @@
    18031860a:	and    $0x81500,%eax
    18031860f:	add    %dl,0xc0025(%rbp,%rsi,1)
    180318616:	add    %al,(%rax)
    180318618:	(bad)
    18031861b:	add    %dl,0x52000000(%rdx)
    180318621:	push   %rbx
    180318622:	rex.R push %rbx
-   180318624:	loope  0x1803185da
-   180318626:	pop    %rbx
-   180318627:	jbe    0x180318600
-   180318629:	xchg   %eax,%ecx
-   18031862a:	cs rex.WRXB scas %es:(%rdi),%al
-   18031862d:	mov    %ebp,%esp
-   18031862f:	jbe    0x180318661
-   180318631:	or     %esp,0x1(%rax,%rdi,2)
-   180318635:	add    %al,(%rax)
+   180318624:	mov    $0xa8,%cl
+   180318626:	xchg   %eax,%esi
+   180318627:	jmp    0x1c45100b1
+   18031862c:	stos   %eax,%es:(%rdi)
+   18031862d:	scas   %es:(%rdi),%al
+   18031862e:	rex.X
+   18031862f:	rex.R stos %al,%es:(%rdi)
+   180318631:	add    0x123(%rdi),%bh
    180318637:	add    %al,0x5c(%rdx,%rdi,1)
    18031863b:	(bad)
    18031863c:	pop    %rsp
    18031863d:	jae    0x1803186b0
    18031863f:	insb   (%dx),%es:(%rdi)
    180318640:	imul   $0x6e6f736a,0x2d(%rbp,%riz,2),%esi
    180318648:	jae    0x1803186ad
@@ -1096541,25 +1096542,25 @@
    180318f9c:	add    %al,(%rax)
    180318f9e:	add    %al,(%rax)
    180318fa0:	add    %eax,(%rax)
    180318fa2:	add    %al,(%rax)
    180318fa4:	(bad)
    180318fa5:	(bad)
    180318fa6:	(bad)
-   180318fa7:	call   *-0xfffffd7(%rax)
-   180318fad:	sub    %al,(%rax)
+   180318fa7:	push   0x29(%rax)
+   180318faa:	add    %al,(%rax)
+   180318fac:	lock sub %al,(%rax)
    180318faf:	add    %bh,%bh
    180318fb1:	(bad)
    180318fb2:	(bad)
-   180318fb3:	call   *0x29(%rsi)
+   180318fb3:	incl   0x29(%rdx)
    180318fb6:	add    %al,(%rax)
    180318fb8:	add    %al,(%rax)
    180318fba:	add    %al,(%rax)
-   180318fbc:	pop    %rsp
-   180318fbd:	sub    %eax,(%rax)
+   180318fbc:	sub    %r8d,(%rax)
    180318fbf:	add    %bh,%bh
    180318fc1:	(bad)
    180318fc2:	(bad)
    180318fc3:	lcall  *(%rcx)
    180318fc5:	or     $0x5,%al
    180318fc7:	rex.RB or $0x3,%al
    180318fca:	(bad)
@@ -1096594,24 +1096595,23 @@
    18031900c:	add    %eax,(%rax)
    18031900e:	add    %al,(%rax)
    180319010:	(bad)
    180319011:	(bad)
    180319012:	(bad)
    180319013:	jmp    *0x2a(%rax)
    180319016:	add    %al,(%rax)
-   180319018:	loopne 0x180319043
-   18031901a:	add    %al,(%rax)
-   18031901c:	(bad)
+   180319018:	shrb   $0x0,(%rcx)
+   18031901b:	add    %bh,%bh
    18031901d:	(bad)
    18031901e:	(bad)
-   18031901f:	push   (%rdx)
+   18031901f:	jmp    *(%rsi)
    180319021:	sub    (%rax),%al
    180319023:	add    %al,(%rax)
    180319025:	add    %al,(%rax)
-   180319027:	add    %dh,(%rdx,%rbp,1)
+   180319027:	add    %ch,(%rdx,%rbp,1)
    18031902a:	add    %al,(%rax)
    18031902c:	(bad)
    18031902d:	(bad)
    18031902e:	(bad)
    18031902f:	lcall  *(%rcx)
    180319031:	or     $0x5,%al
    180319033:	push   %rbp
@@ -1097589,168 +1097589,163 @@
    1803198d9:	xor    (%rbx),%al
    1803198db:	xor    %al,(%rdx)
    1803198dd:	jo     0x1803198e0
    1803198df:	(bad)
    1803198e0:	add    %eax,(%rsi)
    1803198e2:	add    (%rax),%eax
    1803198e4:	(bad)
-   1803198e5:	movabs %al,0x1219000060017002
+   1803198e5:	movabs %al,0xd19000060017002
    1803198ee:	(bad)
-   1803198ef:	test   %edx,(%rdx)
-   1803198f1:	add    (%rdx),%ecx
-   1803198f3:	add    %edx,(%rax,%rax,1)
-   1803198f6:	add    0x2(%rax),%esi
+   1803198ef:	rex.RB or $0x4820803,%eax
+   1803198f5:	xor    %al,(%rbx)
+   1803198f7:	jo     0x1803198fb
    1803198f9:	(bad)
    1803198fa:	add    %edx,-0xb(%rax)
    1803198fd:	xor    $0x25,%al
-   1803198ff:	add    %dl,(%rax)
-   180319901:	cltd
+   1803198ff:	add    %dl,(%rcx,%rbx,4)
    180319902:	xor    %eax,(%rax)
-   180319904:	add    %edx,(%rbx)
-   180319906:	add    $0x0,%al
-   180319908:	or     $0x32,%al
-   18031990a:	or     %dh,0x7(%rax)
-   18031990d:	(bad)
-   18031990e:	(bad)
-   18031990f:	push   %rax
-   180319910:	and    0x11993(%rip),%al        # 0x18032b2a9
-   180319916:	add    %al,(%rax)
-   180319918:	cmp    %bl,0x31(%rcx)
-   18031991e:	add    %al,(%rax)
-   180319920:	add    %al,(%rax)
-   180319922:	add    %al,(%rax)
-   180319924:	add    (%rax),%eax
-   180319926:	add    %al,(%rax)
-   180319928:	rex cltd
-   18031992a:	xor    %eax,(%rax)
-   18031992c:	cwtl
-   18031992d:	add    %al,(%rax)
-   18031992f:	add    %al,(%rax)
-   180319931:	add    %al,(%rax)
-   180319933:	add    %al,(%rcx)
+   180319904:	add    %edx,(%rcx)
+   180319906:	add    $0x9420d00,%eax
+   18031990b:	xor    %cl,(%rax)
+   18031990d:	jo     0x180319916
+   18031990f:	(bad)
+   180319910:	(bad)
+   180319911:	push   %rax
+   180319912:	add    %al,(%rax)
+   180319914:	and    0x11993(%rip),%al        # 0x18032b2ad
+   18031991a:	add    %al,(%rax)
+   18031991c:	cmp    $0x99,%al
+   18031991e:	xor    %eax,(%rax)
+	...
+   180319928:	add    (%rax),%eax
+   18031992a:	add    %al,(%rax)
+   18031992c:	rex.R cltd
+   18031992e:	xor    %eax,(%rax)
+   180319930:	rex add %al,(%rax)
+   180319933:	add    %al,(%rax)
    180319935:	add    %al,(%rax)
-   180319937:	add    %bh,%bh
-   180319939:	(bad)
-   18031993a:	(bad)
-   18031993b:	call   *0x40000053(%rax)
-   180319941:	push   %rdx
+   180319937:	add    %al,(%rcx)
+   180319939:	add    %al,(%rax)
+   18031993b:	add    %bh,%bh
+   18031993d:	(bad)
+   18031993e:	(bad)
+   18031993f:	push   (%rax)
+   180319941:	push   %rbx
    180319942:	add    %al,(%rax)
-   180319944:	(bad)
-   180319945:	(bad)
-   180319946:	(bad)
-   180319947:	(bad)
-   180319948:	jmp    0x18031999c
-   18031994a:	add    %al,(%rax)
-   18031994c:	add    %al,(%rax)
-   18031994e:	add    %al,(%rax)
-   180319950:	notl   0x0(%rdx)
-   180319953:	add    %bh,%bh
-   180319955:	(bad)
-   180319956:	(bad)
-   180319957:	lcall  *(%rcx)
-   180319959:	adc    (%rsi),%al
-   18031995b:	test   %edx,(%rdx)
-   18031995d:	add    (%rdx),%ecx
-   18031995f:	add    %edx,(%rdx)
-   180319961:	add    %al,(%rbx)
-   180319963:	jo     0x180319967
-   180319965:	(bad)
-   180319966:	add    %edx,-0xb(%rax)
-   180319969:	xor    $0x25,%al
-   18031996b:	add    %bh,0x31(%rcx,%rbx,4)
-   18031996f:	add    %al,(%rcx)
-   180319971:	adc    (%rax,%rax,1),%eax
-   180319974:	or     $0x32,%al
-   180319976:	or     %dh,0x7(%rax)
-   180319979:	(bad)
-   18031997a:	(bad)
-   18031997b:	push   %rax
-   18031997c:	and    0x11993(%rip),%al        # 0x18032b315
-   180319982:	add    %al,(%rax)
-   180319984:	movsb  %ds:(%rsi),%es:(%rdi)
-   180319985:	cltd
-   180319986:	xor    %eax,(%rax)
-	...
-   180319990:	add    (%rax),%eax
-   180319992:	add    %al,(%rax)
-   180319994:	lods   %ds:(%rsi),%al
-   180319995:	cltd
-   180319996:	xor    %eax,(%rax)
-   180319998:	mov    %al,(%rax)
-   18031999a:	add    %al,(%rax)
-   18031999c:	add    %al,(%rax)
+   180319944:	rex push %rdx
+   180319946:	add    %al,(%rax)
+   180319948:	(bad)
+   180319949:	(bad)
+   18031994a:	(bad)
+   18031994b:	decl   0x52(%rsi)
+   180319951:	add    %al,(%rax)
+   180319953:	add    %bl,-0xffffae(%rdx)
+   180319959:	(bad)
+   18031995a:	(bad)
+   18031995b:	lcall  *(%rcx)
+   18031995d:	adc    (%rsi),%al
+   18031995f:	test   %edx,(%rdx)
+   180319961:	add    (%rdx),%ecx
+   180319963:	add    %edx,(%rdx)
+   180319965:	add    %al,(%rbx)
+   180319967:	jo     0x18031996b
+   180319969:	(bad)
+   18031996a:	add    %edx,-0xb(%rax)
+   18031996d:	xor    $0x25,%al
+   18031996f:	add    %al,0x1003199(%rax)
+   180319975:	adc    (%rax,%rax,1),%eax
+   180319978:	or     $0x32,%al
+   18031997a:	or     %dh,0x7(%rax)
+   18031997d:	(bad)
+   18031997e:	(bad)
+   18031997f:	push   %rax
+   180319980:	and    0x11993(%rip),%al        # 0x18032b319
+   180319986:	add    %al,(%rax)
+   180319988:	test   $0x99,%al
+   18031998a:	xor    %eax,(%rax)
+	...
+   180319994:	add    (%rax),%eax
+   180319996:	add    %al,(%rax)
+   180319998:	mov    $0x99,%al
+   18031999a:	xor    %eax,(%rax)
+   18031999c:	mov    %al,(%rax)
    18031999e:	add    %al,(%rax)
-   1803199a0:	add    %eax,(%rax)
+   1803199a0:	add    %al,(%rax)
    1803199a2:	add    %al,(%rax)
-   1803199a4:	(bad)
-   1803199a5:	(bad)
-   1803199a6:	(bad)
-   1803199a7:	incl   (%rax)
-   1803199a9:	push   %rbp
-   1803199aa:	add    %al,(%rax)
-   1803199ac:	rclb   $0x0,0x0(%rbx)
-   1803199b0:	(bad)
-   1803199b1:	(bad)
-   1803199b2:	(bad)
-   1803199b3:	lcall  *0x0(%rsp,%rdx,2)
-   1803199b7:	add    %al,(%rax)
-   1803199b9:	add    %al,(%rax)
-   1803199bb:	add    %ch,0x54(%rax)
+   1803199a4:	add    %eax,(%rax)
+   1803199a6:	add    %al,(%rax)
+   1803199a8:	(bad)
+   1803199a9:	(bad)
+   1803199aa:	(bad)
+   1803199ab:	jmp    *0x60000054(%rax)
+   1803199b1:	push   %rbx
+   1803199b2:	add    %al,(%rax)
+   1803199b4:	(bad)
+   1803199b5:	(bad)
+   1803199b6:	(bad)
+   1803199b7:	(bad)
+   1803199b8:	cld
+   1803199b9:	push   %rbx
+   1803199ba:	add    %al,(%rax)
+   1803199bc:	add    %al,(%rax)
    1803199be:	add    %al,(%rax)
-   1803199c0:	(bad)
-   1803199c1:	(bad)
-   1803199c2:	(bad)
-   1803199c3:	lcall  *(%rcx)
-   1803199c5:	or     $0x30d4506,%eax
-   1803199ca:	or     %al,0x70033004(%rdx)
-   1803199d0:	add    0x1(%rax),%ah
-   1803199d3:	push   %rax
-   1803199d4:	cmc
-   1803199d5:	xor    $0x25,%al
-   1803199d7:	add    %ch,%ah
-   1803199d9:	cltd
-   1803199da:	xor    %eax,(%rax)
-   1803199dc:	add    %edx,(%rcx)
-   1803199de:	add    $0x9420d00,%eax
-   1803199e3:	xor    %cl,(%rax)
-   1803199e5:	jo     0x1803199ee
-   1803199e7:	(bad)
-   1803199e8:	(bad)
-   1803199e9:	push   %rax
-   1803199ea:	add    %al,(%rax)
+   1803199c0:	or     %dl,0x0(%rax,%rax,1)
+   1803199c4:	(bad)
+   1803199c5:	(bad)
+   1803199c6:	(bad)
+   1803199c7:	lcall  *(%rcx)
+   1803199c9:	adc    (%rsi),%al
+   1803199cb:	test   %edx,(%rdx)
+   1803199cd:	add    (%rdx),%ecx
+   1803199cf:	add    %edx,(%rax,%rax,1)
+   1803199d2:	add    0x2(%rax),%esi
+   1803199d5:	(bad)
+   1803199d6:	add    %edx,-0xb(%rax)
+   1803199d9:	xor    $0x25,%al
+   1803199db:	add    %ch,%ah
+   1803199dd:	cltd
+   1803199de:	xor    %eax,(%rax)
+   1803199e0:	add    %edx,(%rbx)
+   1803199e2:	add    $0x0,%al
+   1803199e4:	or     $0x32,%al
+   1803199e6:	or     %dh,0x7(%rax)
+   1803199e9:	(bad)
+   1803199ea:	(bad)
+   1803199eb:	push   %rax
    1803199ec:	and    0x11993(%rip),%al        # 0x18032b385
    1803199f2:	add    %al,(%rax)
    1803199f4:	adc    $0x9a,%al
    1803199f6:	xor    %eax,(%rax)
 	...
    180319a00:	add    (%rax),%eax
    180319a02:	add    %al,(%rax)
    180319a04:	sbb    $0x9a,%al
    180319a06:	xor    %eax,(%rax)
-   180319a08:	rex add %al,(%rax)
+   180319a08:	cwtl
+   180319a09:	add    %al,(%rax)
    180319a0b:	add    %al,(%rax)
    180319a0d:	add    %al,(%rax)
    180319a0f:	add    %al,(%rcx)
    180319a11:	add    %al,(%rax)
    180319a13:	add    %bh,%bh
    180319a15:	(bad)
    180319a16:	(bad)
    180319a17:	jmp    *(%rax)
    180319a19:	push   %rsi
    180319a1a:	add    %al,(%rax)
-   180319a1c:	xor    %dl,0x0(%rbp)
-   180319a1f:	add    %bh,%bh
+   180319a1c:	rclb   0x0(%rax,%rax,1)
+   180319a20:	(bad)
    180319a21:	(bad)
    180319a22:	(bad)
    180319a23:	(bad)
-   180319a24:	jle    0x180319a7b
+   180319a24:	jnp    0x180319a7b
    180319a26:	add    %al,(%rax)
    180319a28:	add    %al,(%rax)
    180319a2a:	add    %al,(%rax)
-   180319a2c:	mov    0x0(%rbp),%dl
+   180319a2c:	xchg   %edx,0x0(%rbp)
    180319a2f:	add    %bh,%bh
    180319a31:	(bad)
    180319a32:	(bad)
    180319a33:	lcall  *(%rcx)
    180319a35:	adc    $0x3158508,%eax
    180319a3a:	or     $0x6001201,%eax
    180319a3f:	xor    %al,0x3600470(%rip)        # 0x183919eb5
@@ -1098544,103 +1098539,112 @@
    18031a0c5:	imul   $0xffffff00,(%rax),%eax
    18031a0cb:	lcall  *(%rcx)
    18031a0cd:	or     0x6206030b(,%rsi,1),%eax
    18031a0d4:	add    0x1(%rax),%ah
    18031a0d7:	push   %rax
    18031a0d8:	cmc
    18031a0d9:	xor    $0x25,%al
-   18031a0db:	add    %bh,%al
+   18031a0db:	add    %ch,%ah
    18031a0dd:	movabs 0x420b00030f010031,%al
    18031a0e6:	(bad)
    18031a0e7:	(bad)
    18031a0e8:	(bad)
    18031a0e9:	push   %rax
    18031a0ea:	add    %al,(%rax)
-   18031a0ec:	add    %ecx,(%rdi)
-   18031a0ee:	add    (%rax),%eax
-   18031a0f0:	or     0x7(%rdx),%eax
-   18031a0f3:	(bad)
-   18031a0f4:	(bad)
-   18031a0f5:	push   %rax
-   18031a0f6:	add    %al,(%rax)
-   18031a0f8:	and    0x21993(%rip),%al        # 0x18033ba91
-   18031a0fe:	add    %al,(%rax)
-   18031a100:	and    %ah,0x31(%rcx)
-   18031a106:	add    %al,(%rax)
-   18031a108:	add    %al,(%rax)
+   18031a0ec:	and    0x11993(%rip),%al        # 0x18032ba85
+   18031a0f2:	add    %al,(%rax)
+   18031a0f4:	adc    $0xa1,%al
+   18031a0f6:	xor    %eax,(%rax)
+	...
+   18031a100:	add    (%rax),%eax
+   18031a102:	add    %al,(%rax)
+   18031a104:	sbb    $0xa1,%al
+   18031a106:	xor    %eax,(%rax)
+   18031a108:	xor    %al,(%rax)
    18031a10a:	add    %al,(%rax)
-   18031a10c:	add    $0x0,%al
+   18031a10c:	add    %al,(%rax)
    18031a10e:	add    %al,(%rax)
-   18031a110:	xor    %ah,0x300031(%rcx)
-   18031a116:	add    %al,(%rax)
-   18031a118:	add    %al,(%rax)
-   18031a11a:	add    %al,(%rax)
-   18031a11c:	add    %eax,(%rax)
+   18031a110:	add    %eax,(%rax)
+   18031a112:	add    %al,(%rax)
+   18031a114:	(bad)
+   18031a115:	(bad)
+   18031a116:	(bad)
+   18031a117:	push   0x6c(%rax)
+   18031a11d:	insb   (%dx),%es:(%rdi)
    18031a11e:	add    %al,(%rax)
    18031a120:	(bad)
    18031a121:	(bad)
    18031a122:	(bad)
-   18031a123:	push   0x6d(%rax)
+   18031a123:	ljmp   *(%rdi)
+   18031a125:	insb   (%dx),%es:(%rdi)
    18031a126:	add    %al,(%rax)
    18031a128:	add    %al,(%rax)
    18031a12a:	add    %al,(%rax)
-   18031a12c:	xor    %ch,0x0(%rbp)
-   18031a12f:	add    %al,(%rax)
-   18031a131:	insb   (%dx),%es:(%rdi)
-   18031a132:	add    %al,(%rax)
-   18031a134:	(bad)
-   18031a135:	(bad)
-   18031a136:	(bad)
-   18031a137:	(bad)
-   18031a138:	cmp    0x0(%rax,%rax,1),%ebp
-   18031a13c:	add    %eax,(%rax)
-   18031a13e:	add    %al,(%rax)
-   18031a140:	mov    $0x6c,%eax
-   18031a145:	add    %al,(%rax)
-   18031a147:	add    %bh,-0xffff94(%rbp)
-   18031a14d:	(bad)
-   18031a14e:	(bad)
-   18031a14f:	lcall  *(%rcx)
-   18031a151:	or     0x6206030b(,%rsi,1),%eax
-   18031a158:	add    0x1(%rax),%ah
-   18031a15b:	push   %rax
-   18031a15c:	cmc
-   18031a15d:	xor    $0x25,%al
-   18031a15f:	add    %dh,-0x5f(%rax)
-   18031a162:	xor    %eax,(%rax)
-   18031a164:	add    %ecx,(%rdi)
-   18031a166:	add    (%rax),%eax
-   18031a168:	or     0x7(%rdx),%eax
-   18031a16b:	(bad)
-   18031a16c:	(bad)
-   18031a16d:	push   %rax
+   18031a12c:	cmp    %ch,0x0(%rax,%rax,1)
+   18031a130:	(bad)
+   18031a131:	(bad)
+   18031a132:	(bad)
+   18031a133:	lcall  *(%rcx)
+   18031a135:	or     0x6206030b(,%rsi,1),%eax
+   18031a13c:	add    0x1(%rax),%ah
+   18031a13f:	push   %rax
+   18031a140:	cmc
+   18031a141:	xor    $0x25,%al
+   18031a143:	add    %ah,-0x5f(%rax)
+   18031a146:	xor    %eax,(%rax)
+   18031a148:	add    %ecx,(%rdi)
+   18031a14a:	add    (%rax),%eax
+   18031a14c:	or     0x7(%rdx),%eax
+   18031a14f:	(bad)
+   18031a150:	(bad)
+   18031a151:	push   %rax
+   18031a152:	add    %al,(%rax)
+   18031a154:	add    %ecx,(%rdi)
+   18031a156:	add    (%rax),%eax
+   18031a158:	or     0x7(%rdx),%eax
+   18031a15b:	(bad)
+   18031a15c:	(bad)
+   18031a15d:	push   %rax
+   18031a15e:	add    %al,(%rax)
+   18031a160:	and    0x21993(%rip),%al        # 0x18033baf9
+   18031a166:	add    %al,(%rax)
+   18031a168:	mov    %ah,0x31(%rcx)
    18031a16e:	add    %al,(%rax)
-   18031a170:	and    0x11993(%rip),%al        # 0x18032bb09
+   18031a170:	add    %al,(%rax)
+   18031a172:	add    %al,(%rax)
+   18031a174:	add    $0x0,%al
    18031a176:	add    %al,(%rax)
    18031a178:	cwtl
-   18031a179:	movabs 0x31,%eax
+   18031a179:	movabs 0x300031,%eax
    18031a182:	add    %al,(%rax)
-   18031a184:	add    (%rax),%eax
+   18031a184:	add    %eax,(%rax)
    18031a186:	add    %al,(%rax)
-   18031a188:	movabs 0x300031a1,%al
-   18031a191:	add    %al,(%rax)
-   18031a193:	add    %al,(%rcx)
-   18031a195:	add    %al,(%rax)
-   18031a197:	add    %bh,%bh
-   18031a199:	(bad)
-   18031a19a:	(bad)
-   18031a19b:	call   *0x6e(%rax)
-   18031a19e:	add    %al,(%rax)
-   18031a1a0:	movabs 0xcfffffffff00006d,%al
-   18031a1a9:	insl   (%dx),%es:(%rdi)
-   18031a1aa:	add    %al,(%rax)
-   18031a1ac:	add    %al,(%rax)
-   18031a1ae:	add    %al,(%rax)
-   18031a1b0:	fsubrs 0x0(%rbp)
-   18031a1b3:	add    %bh,%bh
+   18031a188:	(bad)
+   18031a189:	(bad)
+   18031a18a:	(bad)
+   18031a18b:	incl   0x6e(%rax)
+   18031a18e:	add    %al,(%rax)
+   18031a190:	add    %al,(%rax)
+   18031a192:	add    %al,(%rax)
+   18031a194:	add    %ch,0x0(%rsi)
+   18031a197:	add    %dl,%al
+   18031a199:	insb   (%dx),%es:(%rdi)
+   18031a19a:	add    %al,(%rax)
+   18031a19c:	(bad)
+   18031a19d:	(bad)
+   18031a19e:	(bad)
+   18031a19f:	decl   (%rbx)
+   18031a1a1:	insl   (%dx),%es:(%rdi)
+   18031a1a2:	add    %al,(%rax)
+   18031a1a4:	add    %eax,(%rax)
+   18031a1a6:	add    %al,(%rax)
+   18031a1a8:	mov    %ch,0x0(%rbp)
+   18031a1ab:	add    %al,(%rax)
+   18031a1ad:	add    %al,(%rax)
+   18031a1af:	add    %cl,-0xffff93(%rbp)
    18031a1b5:	(bad)
    18031a1b6:	(bad)
    18031a1b7:	lcall  *(%rcx)
    18031a1b9:	adc    %ecx,(%rax)
    18031a1bb:	adc    %r8d,(%r11)
    18031a1be:	or     $0x82,%al
    18031a1c0:	or     %dh,(%rax)
@@ -1224932,28 +1224936,28 @@
    180365113:	add    %al,%al
    180365115:	sub    %al,(%rax)
    180365117:	add    %ah,%al
    180365119:	sub    %al,(%rax)
    18036511b:	add    %al,(%rdi,%rcx,4)
    18036511e:	xor    %eax,(%rax)
    180365120:	lock sub %al,(%rax)
-   180365123:	add    %al,0x58000029(%rbx)
+   180365123:	add    %ch,0x29(%rsi)
+   180365126:	add    %al,(%rax)
+   180365128:	pop    %rax
    180365129:	(bad)
    18036512a:	xor    %eax,(%rax)
-   18036512c:	nop
-   18036512d:	sub    %eax,(%rax)
-   18036512f:	add    %bl,%dh
-   180365131:	sub    %eax,(%rax)
-   180365133:	add    %dh,-0x71(%rax)
+   18036512c:	jo     0x180365157
+   18036512e:	add    %al,(%rax)
+   180365130:	mov    $0x70000029,%esi
+   180365135:	(bad)
    180365136:	xor    %eax,(%rax)
-   180365138:	loopne 0x180365163
-   18036513a:	add    %al,(%rax)
-   18036513c:	pop    %rsi
-   18036513d:	sub    (%rax),%al
-   18036513f:	add    %al,%ah
+   180365138:	shrb   $0x0,(%rcx)
+   18036513b:	add    %dl,0x2a(%rbx)
+   18036513e:	add    %al,(%rax)
+   180365140:	(bad)
    180365141:	(bad)
    180365142:	xor    %eax,(%rax)
    180365144:	(bad)
    180365145:	sub    (%rax),%al
    180365147:	add    %ch,-0x23ffffd6(%rsi)
    18036514d:	(bad)
    18036514e:	xor    %eax,(%rax)
@@ -1225145,65 +1225149,67 @@
    180365316:	xor    %eax,(%rax)
    180365318:	xor    %cl,0x0(%rbp)
    18036531b:	add    %cl,0x4d(%rsi)
    18036531e:	add    %al,(%rax)
    180365320:	js     0x1803652ba
    180365322:	xor    %eax,(%rax)
    180365324:	orb    $0x0,0x0(%rbp)
-   180365328:	rex.B
+   180365328:	(bad)
    180365329:	rex.WRXB add %r8b,(%r8)
-   18036532c:	add    %dl,0x4f500031(%rbx)
-   180365332:	add    %al,(%rax)
-   180365334:	ficoms 0x0(%rax)
-   180365337:	add    %cl,%al
-   180365339:	cwtl
-   18036533a:	xor    %eax,(%rax)
-   18036533c:	loopne 0x18036538e
+   18036532c:	enter  $0x3198,$0x0
+   180365330:	adc    %cl,0x0(%rdi)
+   180365333:	add    %dl,%cl
+   180365335:	push   %rax
+   180365336:	add    %al,(%rax)
+   180365338:	add    %dl,0x50e00031(%rbx)
    18036533e:	add    %al,(%rax)
    180365340:	imul   $0x3198d400,0x0(%rcx),%edx
    180365347:	add    %dh,0x51(%rax)
    18036534a:	add    %al,(%rax)
    18036534c:	xor    0x0(%rdx),%dl
    18036534f:	add    %ah,%al
    180365351:	cwtl
    180365352:	xor    %eax,(%rax)
    180365354:	rex push %rdx
    180365356:	add    %al,(%rax)
-   180365358:	xchg   %dl,0x0(%rbx)
-   18036535b:	add    %ch,%ah
+   180365358:	(bad)
+   180365359:	push   %rbx
+   18036535a:	add    %al,(%rax)
+   18036535c:	in     (%dx),%al
    18036535d:	cwtl
    18036535e:	xor    %eax,(%rax)
-   180365360:	nop
-   180365361:	push   %rbx
-   180365362:	add    %al,(%rax)
-   180365364:	mov    $0x4000053,%ecx
-   180365369:	cltd
+   180365360:	xor    %dl,0x0(%rbx)
+   180365363:	add    %bl,0x53(%rax)
+   180365366:	add    %al,(%rax)
+   180365368:	add    $0x99,%al
    18036536a:	xor    %eax,(%rax)
-   18036536c:	rclb   $0x0,0x0(%rbx)
-   180365370:	notl   0x0(%rax,%rax,1)
-   180365374:	pop    %rax
+   18036536c:	(bad)
+   18036536d:	push   %rbx
+   18036536e:	add    %al,(%rax)
+   180365370:	xchg   %eax,%edi
+   180365371:	push   %rsp
+   180365372:	add    %al,(%rax)
+   180365374:	pop    %rsp
    180365375:	cltd
    180365376:	xor    %eax,(%rax)
-   180365378:	add    %dl,0x0(%rbp)
-   18036537b:	add    %ch,(%rcx)
-   18036537d:	push   %rbp
-   18036537e:	add    %al,(%rax)
-   180365380:	jo     0x18036531b
+   180365378:	movabs 0x74000054c9000054,%al
+   180365381:	cltd
    180365382:	xor    %eax,(%rax)
-   180365384:	xor    %dl,0x0(%rbp)
-   180365387:	add    %bl,(%rdi)
+   180365384:	rclb   0x0(%rax,%rax,1)
+   180365388:	(bad)
    180365389:	push   %rsi
    18036538a:	add    %al,(%rax)
-   18036538c:	(bad)
-   18036538d:	cltd
-   18036538e:	xor    %eax,(%rax)
+   18036538c:	enter  $0x3199,$0x0
    180365390:	and    %dl,0x0(%rsi)
-   180365393:	add    %cl,0x56(%rax)
+   180365393:	add    %cl,0x56(%rcx)
    180365396:	add    %al,(%rax)
-   180365398:	fcompl 0x56500031(%rcx)
+   180365398:	loopne 0x180365333
+   18036539a:	xor    %eax,(%rax)
+   18036539c:	push   %rax
+   18036539d:	push   %rsi
    18036539e:	add    %al,(%rax)
    1803653a0:	(bad)
    1803653a1:	push   %rdi
    1803653a2:	add    %al,(%rax)
    1803653a4:	xor    $0x9a,%al
    1803653a6:	xor    %eax,(%rax)
    1803653a8:	rex push %rdi
@@ -1225387,34 +1225393,32 @@
    18036553e:	xor    %eax,(%rax)
    180365540:	xor    %ch,0x0(%rbx)
    180365543:	add    %ah,0x6b(%rsi)
    180365546:	add    %al,(%rax)
    180365548:	test   $0x9f,%al
    18036554a:	xor    %eax,(%rax)
    18036554c:	add    %ch,0x0(%rax,%rax,1)
-   180365550:	(bad)
-   180365551:	insl   (%dx),%es:(%rdi)
-   180365552:	add    %al,(%rax)
-   180365554:	int3
-   180365555:	movabs 0x6d6900006d300031,%al
-   18036555e:	add    %al,(%rax)
+   180365550:	movabs %eax,0xb00031a0cc00006c
+   180365559:	insb   (%dx),%es:(%rdi)
+   18036555a:	add    %al,(%rax)
+   18036555c:	shrb   0x0(%rax,%rax,1)
    180365560:	loopne 0x180365502
    180365562:	xor    %eax,(%rax)
-   180365564:	jo     0x1803655d3
-   180365566:	add    %al,(%rax)
-   180365568:	xchg   %eax,%edi
-   180365569:	insl   (%dx),%es:(%rdi)
-   18036556a:	add    %al,(%rax)
-   18036556c:	in     (%dx),%al
-   18036556d:	movabs 0x6e4300006da00031,%al
+   180365564:	shrb   0x0(%rax,%rax,1)
+   180365568:	ljmp   *0x0(%rbp)
+   18036556b:	add    %dh,(%rcx,%riz,4)
+   18036556e:	xor    %eax,(%rax)
+   180365570:	add    %ch,0x0(%rsi)
+   180365573:	add    %bh,(%rcx)
+   180365575:	outsb  %ds:(%rsi),(%dx)
    180365576:	add    %al,(%rax)
-   180365578:	push   %rax
-   180365579:	movabs 0x6e7000006e500031,%eax
+   180365578:	movabs 0x6e6700006e400031,%rax
    180365582:	add    %al,(%rax)
-   180365584:	movabs %fs:0x6edb00006e700031,%eax
+   180365584:	push   %rsp
+   180365585:	movabs 0x6edb00006e700031,%eax
    18036558e:	add    %al,(%rax)
    180365590:	(bad)
    180365591:	cwtl
    180365592:	xor    %eax,(%rax)
    180365594:	loopne 0x180365604
    180365596:	add    %al,(%rax)
    180365598:	(bad)
```

## sqlite_jsonschema/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.3-alpha.2"
+__version__ = "0.2.3-alpha.3"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_jsonschema-0.2.3a2.dist-info/METADATA` & `sqlite_jsonschema-0.2.3a3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-jsonschema
-Version: 0.2.3a2
+Version: 0.2.3a3
 Home-page: https://github.com/asg017/sqlite-jsonschema
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-jsonschema/issues
 Project-URL: CI, https://github.com/asg017/sqlite-jsonschema/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-jsonschema/releases
 Requires-Python: >=3.7
```

## Comparing `sqlite_jsonschema-0.2.3a2.dist-info/RECORD` & `sqlite_jsonschema-0.2.3a3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noop.cp311-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sqlite_jsonschema/__init__.py,sha256=fcxu6_RD16yOn7qHg6A0Fz-1dUwYFtjGgb0Ed9NYGtM,327
-sqlite_jsonschema/jsonschema0.dll,sha256=_itR82oC101Rm1r83C3P6pzlckdcqPw0Dt-38HAnldM,3678720
-sqlite_jsonschema/version.py,sha256=ANbjAmRjKGnW5TFhoQySZjvBjdSCDX56vddFXG73vFs,81
-sqlite_jsonschema-0.2.3a2.dist-info/METADATA,sha256=tQlYfJOCsIt3ooX7Kr2vA42-UsonoKn6eJrMbHSaL3Q,545
-sqlite_jsonschema-0.2.3a2.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-sqlite_jsonschema-0.2.3a2.dist-info/top_level.txt,sha256=bjaT4NMmoRGkmwknql8eLZwNXpEbb2PSJJgQCBbXocw,23
-sqlite_jsonschema-0.2.3a2.dist-info/RECORD,,
+sqlite_jsonschema/jsonschema0.dll,sha256=52Je57kOAaJcmUUjFUck3PQyf0co5Tc0lY0cH44JnFk,3678720
+sqlite_jsonschema/version.py,sha256=loD2WkJvu18mGozuRGcYKEAqzDOZJlOwq4Fww4UHNLQ,81
+sqlite_jsonschema-0.2.3a3.dist-info/METADATA,sha256=l5QuUfStavcMsy9txEzXCvCcwfWPAfNM4BiGrtERA8Q,545
+sqlite_jsonschema-0.2.3a3.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+sqlite_jsonschema-0.2.3a3.dist-info/top_level.txt,sha256=bjaT4NMmoRGkmwknql8eLZwNXpEbb2PSJJgQCBbXocw,23
+sqlite_jsonschema-0.2.3a3.dist-info/RECORD,,
```

