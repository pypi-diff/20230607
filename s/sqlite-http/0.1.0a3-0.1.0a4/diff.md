# Comparing `tmp/sqlite_http-0.1.0a3-py3-none-win_amd64.whl.zip` & `tmp/sqlite_http-0.1.0a4-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 4903142 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 23:24 noop.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      556 b- defN 23-Jun-06 23:23 sqlite_http/__init__.py
--rw-rw-rw-  2.0 fat 15210365 b- defN 23-Jun-06 23:23 sqlite_http/http0.dll
--rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-06 23:23 sqlite_http/version.py
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-06 23:24 sqlite_http-0.1.0a3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-06 23:24 sqlite_http-0.1.0a3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 23:24 sqlite_http-0.1.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      638 b- defN 23-Jun-06 23:24 sqlite_http-0.1.0a3.dist-info/RECORD
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 23:29 noop.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      556 b- defN 23-Jun-06 23:28 sqlite_http/__init__.py
+-rw-rw-rw-  2.0 fat 15210365 b- defN 23-Jun-06 23:29 sqlite_http/http0.dll
+-rw-rw-rw-  2.0 fat       81 b- defN 23-Jun-06 23:28 sqlite_http/version.py
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-06 23:29 sqlite_http-0.1.0a4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-06 23:29 sqlite_http-0.1.0a4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-06 23:29 sqlite_http-0.1.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      638 b- defN 23-Jun-06 23:29 sqlite_http-0.1.0a4.dist-info/RECORD
 8 files, 15212274 bytes uncompressed, 4902028 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_http/http0.dll
 Comment: 
 
 Filename: sqlite_http/version.py
 Comment: 
 
-Filename: sqlite_http-0.1.0a3.dist-info/METADATA
+Filename: sqlite_http-0.1.0a4.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_http-0.1.0a3.dist-info/WHEEL
+Filename: sqlite_http-0.1.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_http-0.1.0a3.dist-info/top_level.txt
+Filename: sqlite_http-0.1.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_http-0.1.0a3.dist-info/RECORD
+Filename: sqlite_http-0.1.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_http/http0.dll

### objdump

```diff
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	1
 Win32Version		00000000
 SizeOfImage		00e61000
 SizeOfHeaders		00000600
-CheckSum		00e9096a
+CheckSum		00e84127
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00008160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					TERMINAL_SERVICE_AWARE
 SizeOfStackReserve	0000000000200000
@@ -41648,58 +41648,47 @@
    377b6159a:	nopw   0x0(%rax,%rax,1)
 
 0000000377b615a0 <go:buildid>:
    377b615a0:	jmp    *(%rax)
    377b615a2:	rex.RXB outsl %ds:(%rsi),(%dx)
    377b615a4:	and    %ah,0x75(%rdx)
    377b615a7:	imul   $0x203a4449,0x20(%rsp,%riz,2),%ebp
-   377b615af:	and    0x30(%rax),%dl
-   377b615b2:	cmp    %r13,0x34(%rdx)
-   377b615b6:	push   %rdi
-   377b615b7:	outsl  %ds:(%rsi),(%dx)
-   377b615b8:	jno    377b6161f <go:buildid+0x7f>
-   377b615ba:	js     377b61613 <go:buildid+0x73>
-   377b615bc:	jb     377b6160e <go:buildid+0x6e>
-   377b615be:	rex.X
-   377b615bf:	rex.R outsl %ds:(%rsi),(%dx)
-   377b615c1:	imul   $0x2f,0x59(%rdx),%eax
-   377b615c5:	movsxd 0x39(%rcx),%ebp
-   377b615c8:	xor    %ebx,0x62(%rax)
-   377b615cb:	rex.W
-   377b615cc:	rex.XB
-   377b615cd:	gs push $0x5a
-   377b615d0:	ja     377b61627 <internal/cpu.Initialize+0x7>
-   377b615d2:	(bad)
-   377b615d3:	jp     377b61622 <internal/cpu.Initialize+0x2>
-   377b615d5:	rex.R
-   377b615d6:	rex.RXB xor $0x55,%al
-   377b615d9:	(bad)
-   377b615da:	cmp    %ecx,0x52(%rax)
+   377b615af:	and    0x5a(%rcx),%dh
+   377b615b2:	rex.WRX jp 377b61607 <go:buildid+0x67>
+   377b615b5:	movslq 0x4d(%r11),%rsi
+   377b615b9:	ja     377b6161f <go:buildid+0x7f>
+   377b615bb:	pop    %rdi
+   377b615bc:	xor    %gs:0x5f(%rdi),%esp
+   377b615c0:	push   $0x51
+   377b615c2:	js     377b61614 <go:buildid+0x74>
+   377b615c4:	(bad)
+   377b615c5:	xor    %dh,0x706e2d6f(%rip)        # 3e824433a <.debug_line_str+0x6f8842f0>
+   377b615cb:	jp     377b61644 <internal/cpu.Initialize+0x24>
+   377b615cd:	xor    $0x3856454f,%eax
+   377b615d2:	jbe    377b61623 <internal/cpu.Initialize+0x3>
+   377b615d4:	rex.XB jae 377b61650 <internal/cpu.Initialize+0x30>
+   377b615d7:	sub    $0x48392f52,%eax
+   377b615dc:	push   %rdx
    377b615dd:	rex.WB
    377b615de:	rex.WRX
    377b615df:	rex.WR jo 377b61639 <internal/cpu.Initialize+0x19>
    377b615e2:	rex.RB push %r11
    377b615e4:	rex.R
    377b615e5:	xor    (%r14),%r14
    377b615e8:	rex.RXB xor %r9d,0x31(%r13)
    377b615ec:	rex.WXB insl (%dx),%es:(%rdi)
    377b615ee:	(bad)
-   377b615ef:	addr32 jns 377b61622 <internal/cpu.Initialize+0x2>
-   377b615f2:	rex.W jae 377b6164a <internal/cpu.Initialize+0x2a>
-   377b615f5:	push   %rcx
-   377b615f6:	rex.RB
-   377b615f7:	rex.RB
-   377b615f8:	rex.WR
-   377b615f9:	rex.WR
-   377b615fa:	rex.RXB push %r15
-   377b615fc:	push   %rsi
-   377b615fd:	push   %rdi
-   377b615fe:	rex.B
-   377b615ff:	gs pop %rcx
-   377b61601:	push   $0x39
+   377b615ef:	pop    %rcx
+   377b615f0:	jbe    377b61624 <internal/cpu.Initialize+0x4>
+   377b615f2:	rex.RB xor $0x35,%al
+   377b615f5:	pop    %rdx
+   377b615f6:	sub    $0x3374774c,%eax
+   377b615fb:	cmp    %ah,0x74(%rdi)
+   377b615fe:	rex.R jae 377b61679 <internal/cpu.Initialize+0x59>
+   377b61601:	jno    377b61651 <internal/cpu.Initialize+0x31>
    377b61603:	and    (%rdx),%cl
    377b61605:	and    %bh,%bh
    377b61607:	int3
    377b61608:	int3
    377b61609:	int3
    377b6160a:	int3
    377b6160b:	int3
@@ -1067838,40 +1067827,41 @@
    377e6425c:	addr32 jae 377e6429c <go:buildinfo+0x27c>
    377e6425f:	and    0x616d2058(%rip),%ch        # 3d95362bd <.debug_line_str+0x60b76273>
    377e64265:	imul   $0x73726556,0x2e(%rsi),%ebp
    377e6426c:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377e64273:	xor    %ebp,(%rsi)
    377e64275:	xor    %ch,0x68706c61(%rip)        # 3e056aedc <.debug_line_str+0x67baae92>
    377e6427b:	(bad)
-   377e6427c:	cs xor (%rax),%esp
+   377e6427c:	cs xor $0x20,%al
    377e6427f:	sub    $0x616d2058,%eax
    377e64284:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377e6428b:	imul   $0x34383937,0x31(%rbp,%rdi,1),%esi
+   377e6428b:	imul   $0x36616662,0x65(%rbp,%rdi,1),%esi
    377e64293:	(bad)
-   377e64294:	xor    $0x33643461,%eax
-   377e64299:	xor    $0x36663938,%eax
-   377e6429e:	movsxd %gs:(%rcx),%esi
-   377e642a1:	(bad)
-   377e642a3:	xor    %bh,(%rcx)
-   377e642a5:	movsxd (%rsi),%esi
-   377e642a7:	xor    (%rdx),%dh
-   377e642a9:	xor    %esi,0x35646664(%rip)        # 3ad4aa913 <.debug_line_str+0x34aea8c9>
-   377e642af:	xor    $0x33,%al
-   377e642b1:	fs xor $0x20666166,%eax
+   377e64294:	vpminsb 0x198(%rdx){1to8},%ymm3,%ymm12
+   377e6429b:	xor    %esi,(%rbx)
+   377e6429d:	cmp    %dh,(%rbx)
+   377e6429f:	cmp    %esp,0x39(%rcx)
+   377e642a2:	xor    %dh,(%rax)
+   377e642a4:	xor    $0x62,%al
+   377e642a6:	xor    %esi,(%rdi)
+   377e642a8:	ss xor 0x65(%rdi,%rsi,1),%ah
+   377e642ad:	xor    %esi,(%rax)
+   377e642af:	movsxd (%rbx),%esi
+   377e642b1:	cmp    %dh,(%rax)
+   377e642b3:	xor    (%rdi),%esi
+   377e642b5:	xor    %ah,(%rax)
    377e642b7:	sub    $0x616d2058,%eax
    377e642bc:	imul   $0x65746144,0x2e(%rsi),%ebp
    377e642c3:	cmp    $0x33323032,%eax
    377e642c8:	sub    $0x302d3630,%eax
    377e642cd:	ss push %rsp
    377e642cf:	xor    (%rbx),%dh
    377e642d1:	cmp    (%rdx),%dh
-   377e642d3:	xor    %edi,(%rdx)
-   377e642d5:	xor    $0x39,%al
-   377e642d7:	pop    %rdx
-   377e642d8:	sub    (%rax),%esi
+   377e642d3:	(bad)
+   377e642d4:	cmp    0x302b5a34(%rip),%dh        # 3a8119d0e <.debug_line_str+0x2f759cc4>
    377e642da:	xor    %dh,(%rax)
    377e642dc:	xor    %ah,(%rdx)
    377e642de:	or     0x75(%rdx),%ah
    377e642e1:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377e642e9:	jae    377e64328 <go:buildinfo+0x308>
    377e642eb:	jae    377e64355 <go:buildinfo+0x335>
    377e642ed:	(bad)
@@ -1067951,39 +1067941,41 @@
    377e643ad:	or     %esi,0x63(%rsi)
    377e643b0:	jae    377e643e0 <go:buildinfo+0x3c0>
    377e643b2:	jb     377e64419 <go:buildinfo+0x3f9>
    377e643b4:	jbe    377e6441f <go:buildinfo+0x3ff>
    377e643b6:	jae    377e64421 <go:buildinfo+0x401>
    377e643b8:	outsl  %ds:(%rsi),(%dx)
    377e643b9:	outsb  %ds:(%rsi),(%dx)
-   377e643ba:	cmp    $0x38393731,%eax
-   377e643bf:	xor    $0x37,%al
-   377e643c1:	xor    $0x33643461,%eax
-   377e643c6:	xor    $0x36663938,%eax
-   377e643cb:	movsxd %gs:(%rcx),%esi
-   377e643ce:	(bad)
-   377e643d0:	xor    %bh,(%rcx)
-   377e643d2:	movsxd (%rsi),%esi
-   377e643d4:	xor    (%rdx),%dh
-   377e643d6:	xor    %esi,0x35646664(%rip)        # 3ad4aaa40 <.debug_line_str+0x34aea9f6>
-   377e643dc:	xor    $0x33,%al
-   377e643de:	fs xor $0xa666166,%eax
+   377e643ba:	cmp    $0x61666265,%eax
+   377e643bf:	ss (bad)
+   377e643c1:	vpminsb 0x198(%rdx){1to8},%ymm3,%ymm12
+   377e643c8:	xor    %esi,(%rbx)
+   377e643ca:	cmp    %dh,(%rbx)
+   377e643cc:	cmp    %esp,0x39(%rcx)
+   377e643cf:	xor    %dh,(%rax)
+   377e643d1:	xor    $0x62,%al
+   377e643d3:	xor    %esi,(%rdi)
+   377e643d5:	ss xor 0x65(%rdi,%rsi,1),%ah
+   377e643da:	xor    %esi,(%rax)
+   377e643dc:	movsxd (%rbx),%esi
+   377e643de:	cmp    %dh,(%rax)
+   377e643e0:	xor    (%rdi),%esi
+   377e643e2:	xor    %cl,(%rdx)
    377e643e4:	(bad)
    377e643e6:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377e643ee:	je     377e64459 <text/template..gobytes.6+0x1>
    377e643f0:	insl   (%dx),%es:(%rdi)
    377e643f1:	gs cmp $0x33323032,%eax
    377e643f7:	sub    $0x302d3630,%eax
    377e643fc:	ss push %rsp
    377e643fe:	xor    (%rbx),%dh
    377e64400:	cmp    (%rdx),%dh
-   377e64402:	xor    %bh,(%rdx)
-   377e64404:	xor    %edi,(%rax)
-   377e64406:	pop    %rdx
-   377e64407:	or     0x75(%rdx),%ah
+   377e64402:	ss cmp (%rbx),%dh
+   377e64405:	cmp    %ebx,0xa(%rdx)
+   377e64408:	(bad)
    377e6440a:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377e64412:	insl   (%dx),%es:(%rdi)
    377e64413:	outsl  %ds:(%rsi),(%dx)
    377e64414:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377e6441c:	(bad)
    377e6441d:	insb   (%dx),%es:(%rdi)
    377e6441e:	jae    377e64485 <crypto/tls._SignatureScheme_index_8+0x1>
@@ -1618725,15 +1618717,15 @@
 	...
 
 0000000377fb7de8 <main.Version.str>:
    377fb7de8:	jbe    377fb7e1a <bufio..stmp_0+0xa>
    377fb7dea:	cs xor %ebp,(%rsi)
    377fb7ded:	xor    %ch,0x68706c61(%rip)        # 3e06bea54 <.debug_line_str+0x67cfea0a>
    377fb7df3:	(bad)
-   377fb7df4:	cs xor (%rax),%eax
+   377fb7df4:	cs xor $0x0,%al
 	...
 
 0000000377fb7e00 <bswapMask>:
    377fb7e00:	femms
    377fb7e02:	or     $0x90a0b0c,%eax
    377fb7e07:	or     %al,(%rdi)
    377fb7e09:	(bad)
@@ -1621886,18 +1621878,16 @@
 0000000377fb9290 <main.Date.str>:
    377fb9290:	xor    (%rax),%dh
    377fb9292:	xor    (%rbx),%dh
    377fb9294:	sub    $0x302d3630,%eax
    377fb9299:	ss push %rsp
    377fb929b:	xor    (%rbx),%dh
    377fb929d:	cmp    (%rdx),%dh
-   377fb929f:	xor    %edi,(%rdx)
-   377fb92a1:	xor    $0x39,%al
-   377fb92a3:	pop    %rdx
-   377fb92a4:	sub    (%rax),%esi
+   377fb929f:	(bad)
+   377fb92a0:	cmp    0x302b5a34(%rip),%dh        # 3a826ecda <.debug_line_str+0x2f8aec90>
    377fb92a6:	xor    %dh,(%rax)
    377fb92a8:	xor    %al,(%rax)
 	...
 
 0000000377fb92c0 <BSWAP_SHUFB_CTL>:
    377fb92c0:	add    (%rdx),%eax
    377fb92c2:	add    %eax,(%rax)
@@ -1626302,27 +1626292,30 @@
 0000000377fbb648 <vendor/golang.org/x/text/unicode/norm..stmp_10>:
    377fbb648:	sub    $0x377f2d5,%eax
    377fbb64d:	add    %al,(%rax)
    377fbb64f:	add    %al,(%rdx)
 	...
 
 0000000377fbb680 <main.Commit.str>:
-   377fbb680:	xor    %esi,(%rdi)
-   377fbb682:	cmp    %edi,(%rax)
-   377fbb684:	xor    $0x37,%al
-   377fbb686:	xor    $0x33643461,%eax
-   377fbb68b:	xor    $0x36663938,%eax
-   377fbb690:	movsxd %gs:(%rcx),%esi
-   377fbb693:	(bad)
-   377fbb695:	xor    %bh,(%rcx)
-   377fbb697:	movsxd (%rsi),%esi
-   377fbb699:	xor    (%rdx),%dh
-   377fbb69b:	xor    %esi,0x35646664(%rip)        # 3ad601d05 <.debug_line_str+0x34c41cbb>
-   377fbb6a1:	xor    $0x33,%al
-   377fbb6a3:	fs xor $0x666166,%eax
+   377fbb680:	gs (bad)
+   377fbb683:	(bad)
+   377fbb684:	ss (bad)
+   377fbb686:	vpminsb 0x198(%rdx){1to8},%ymm3,%ymm12
+   377fbb68d:	xor    %esi,(%rbx)
+   377fbb68f:	cmp    %dh,(%rbx)
+   377fbb691:	cmp    %esp,0x39(%rcx)
+   377fbb694:	xor    %dh,(%rax)
+   377fbb696:	xor    $0x62,%al
+   377fbb698:	xor    %esi,(%rdi)
+   377fbb69a:	ss xor 0x65(%rdi,%rsi,1),%ah
+   377fbb69f:	xor    %esi,(%rax)
+   377fbb6a1:	movsxd (%rbx),%esi
+   377fbb6a3:	cmp    %dh,(%rax)
+   377fbb6a5:	xor    (%rdi),%esi
+   377fbb6a7:	xor    %al,(%rax)
 	...
 
 0000000377fbb6c0 <crypto/ecdsa..dict.nistCurve[*crypto/internal/nistec.P224Point]>:
    377fbb6c0:	and    %ah,%ch
    377fbb6c2:	lret   $0x377
    377fbb6c5:	add    %al,(%rax)
    377fbb6c7:	add    %ah,-0x14(%rax)
@@ -1634910,40 +1634903,41 @@
    377fc1231:	addr32 jae 377fc1271 <runtime.modinfo.str+0x251>
    377fc1234:	and    0x616d2058(%rip),%ch        # 3d9693292 <.debug_line_str+0x60cd3248>
    377fc123a:	imul   $0x73726556,0x2e(%rsi),%ebp
    377fc1241:	imul   $0x2e30763d,0x6e(%rdi),%ebp
    377fc1248:	xor    %ebp,(%rsi)
    377fc124a:	xor    %ch,0x68706c61(%rip)        # 3e06c7eb1 <.debug_line_str+0x67d07e67>
    377fc1250:	(bad)
-   377fc1251:	cs xor (%rax),%esp
+   377fc1251:	cs xor $0x20,%al
    377fc1254:	sub    $0x616d2058,%eax
    377fc1259:	imul   $0x6d6d6f43,0x2e(%rsi),%ebp
-   377fc1260:	imul   $0x34383937,0x31(%rbp,%rdi,1),%esi
+   377fc1260:	imul   $0x36616662,0x65(%rbp,%rdi,1),%esi
    377fc1268:	(bad)
-   377fc1269:	xor    $0x33643461,%eax
-   377fc126e:	xor    $0x36663938,%eax
-   377fc1273:	movsxd %gs:(%rcx),%esi
-   377fc1276:	(bad)
-   377fc1278:	xor    %bh,(%rcx)
-   377fc127a:	movsxd (%rsi),%esi
-   377fc127c:	xor    (%rdx),%dh
-   377fc127e:	xor    %esi,0x35646664(%rip)        # 3ad6078e8 <.debug_line_str+0x34c4789e>
-   377fc1284:	xor    $0x33,%al
-   377fc1286:	fs xor $0x20666166,%eax
+   377fc1269:	vpminsb 0x198(%rdx){1to8},%ymm3,%ymm12
+   377fc1270:	xor    %esi,(%rbx)
+   377fc1272:	cmp    %dh,(%rbx)
+   377fc1274:	cmp    %esp,0x39(%rcx)
+   377fc1277:	xor    %dh,(%rax)
+   377fc1279:	xor    $0x62,%al
+   377fc127b:	xor    %esi,(%rdi)
+   377fc127d:	ss xor 0x65(%rdi,%rsi,1),%ah
+   377fc1282:	xor    %esi,(%rax)
+   377fc1284:	movsxd (%rbx),%esi
+   377fc1286:	cmp    %dh,(%rax)
+   377fc1288:	xor    (%rdi),%esi
+   377fc128a:	xor    %ah,(%rax)
    377fc128c:	sub    $0x616d2058,%eax
    377fc1291:	imul   $0x65746144,0x2e(%rsi),%ebp
    377fc1298:	cmp    $0x33323032,%eax
    377fc129d:	sub    $0x302d3630,%eax
    377fc12a2:	ss push %rsp
    377fc12a4:	xor    (%rbx),%dh
    377fc12a6:	cmp    (%rdx),%dh
-   377fc12a8:	xor    %edi,(%rdx)
-   377fc12aa:	xor    $0x39,%al
-   377fc12ac:	pop    %rdx
-   377fc12ad:	sub    (%rax),%esi
+   377fc12a8:	(bad)
+   377fc12a9:	cmp    0x302b5a34(%rip),%dh        # 3a8276ce3 <.debug_line_str+0x2f8b6c99>
    377fc12af:	xor    %dh,(%rax)
    377fc12b1:	xor    %ah,(%rdx)
    377fc12b3:	or     0x75(%rdx),%ah
    377fc12b6:	imul   $0x6761742d,0x9(%rsp,%riz,2),%ebp
    377fc12be:	jae    377fc12fd <runtime.modinfo.str+0x2dd>
    377fc12c0:	jae    377fc132a <runtime.modinfo.str+0x30a>
    377fc12c2:	(bad)
@@ -1635023,39 +1635017,41 @@
    377fc1382:	or     %esi,0x63(%rsi)
    377fc1385:	jae    377fc13b5 <runtime.modinfo.str+0x395>
    377fc1387:	jb     377fc13ee <runtime.modinfo.str+0x3ce>
    377fc1389:	jbe    377fc13f4 <runtime.modinfo.str+0x3d4>
    377fc138b:	jae    377fc13f6 <runtime.modinfo.str+0x3d6>
    377fc138d:	outsl  %ds:(%rsi),(%dx)
    377fc138e:	outsb  %ds:(%rsi),(%dx)
-   377fc138f:	cmp    $0x38393731,%eax
-   377fc1394:	xor    $0x37,%al
-   377fc1396:	xor    $0x33643461,%eax
-   377fc139b:	xor    $0x36663938,%eax
-   377fc13a0:	movsxd %gs:(%rcx),%esi
-   377fc13a3:	(bad)
-   377fc13a5:	xor    %bh,(%rcx)
-   377fc13a7:	movsxd (%rsi),%esi
-   377fc13a9:	xor    (%rdx),%dh
-   377fc13ab:	xor    %esi,0x35646664(%rip)        # 3ad607a15 <.debug_line_str+0x34c479cb>
-   377fc13b1:	xor    $0x33,%al
-   377fc13b3:	fs xor $0xa666166,%eax
+   377fc138f:	cmp    $0x61666265,%eax
+   377fc1394:	ss (bad)
+   377fc1396:	vpminsb 0x198(%rdx){1to8},%ymm3,%ymm12
+   377fc139d:	xor    %esi,(%rbx)
+   377fc139f:	cmp    %dh,(%rbx)
+   377fc13a1:	cmp    %esp,0x39(%rcx)
+   377fc13a4:	xor    %dh,(%rax)
+   377fc13a6:	xor    $0x62,%al
+   377fc13a8:	xor    %esi,(%rdi)
+   377fc13aa:	ss xor 0x65(%rdi,%rsi,1),%ah
+   377fc13af:	xor    %esi,(%rax)
+   377fc13b1:	movsxd (%rbx),%esi
+   377fc13b3:	cmp    %dh,(%rax)
+   377fc13b5:	xor    (%rdi),%esi
+   377fc13b7:	xor    %cl,(%rdx)
    377fc13b9:	(bad)
    377fc13bb:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377fc13c3:	je     377fc142e <vendor/golang.org/x/sys/cpu..stmp_1+0x26>
    377fc13c5:	insl   (%dx),%es:(%rdi)
    377fc13c6:	gs cmp $0x33323032,%eax
    377fc13cc:	sub    $0x302d3630,%eax
    377fc13d1:	ss push %rsp
    377fc13d3:	xor    (%rbx),%dh
    377fc13d5:	cmp    (%rdx),%dh
-   377fc13d7:	xor    %bh,(%rdx)
-   377fc13d9:	xor    %edi,(%rax)
-   377fc13db:	pop    %rdx
-   377fc13dc:	or     0x75(%rdx),%ah
+   377fc13d7:	ss cmp (%rbx),%dh
+   377fc13da:	cmp    %ebx,0xa(%rdx)
+   377fc13dd:	(bad)
    377fc13df:	imul   $0x2e736376,0x9(%rsp,%riz,2),%ebp
    377fc13e7:	insl   (%dx),%es:(%rdi)
    377fc13e8:	outsl  %ds:(%rsi),(%dx)
    377fc13e9:	imul   $0x663d6465,%fs:0x69(%rsi),%esp
    377fc13f1:	(bad)
    377fc13f2:	insb   (%dx),%es:(%rdi)
    377fc13f3:	jae    377fc145a <vendor/golang.org/x/sys/cpu..stmp_1+0x52>
@@ -4194295,8 +4194291,12 @@
    3786278d4:	add    %al,(%rax)
    3786278d6:	add    %al,(%rax)
    3786278d8:	add    %al,(%rcx)
    3786278da:	add    %dl,0x27(%rcx)
    3786278dd:	add    %al,(%rax)
    3786278df:	add    %al,(%rax)
    3786278e1:	add    %al,(%rax)
-[ Too much input for diff (SHA256: b44027d1d414201cbd30b5451194a3197d7dfa06ec40c0193432993020c11198) ]
+   3786278e3:	add    %bh,(%rdx)
+   3786278e5:	add    %al,(%rax)
+   3786278e7:	add    %al,(%rax)
+   3786278e9:	add    %al,(%rax)
+[ Too much input for diff (SHA256: 3accd5c77d808bba082c026928b009f4de842a12b771b8fd239ec56aaa40a489) ]
```

## sqlite_http/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.3"
+__version__ = "0.1.0-alpha.4"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_http-0.1.0a3.dist-info/METADATA` & `sqlite_http-0.1.0a4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-http
-Version: 0.1.0a3
+Version: 0.1.0a4
 Home-page: https://github.com/asg017/sqlite-http
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-http/issues
 Project-URL: CI, https://github.com/asg017/sqlite-http/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-http/releases
 Requires-Python: >=3.7
```

## Comparing `sqlite_http-0.1.0a3.dist-info/RECORD` & `sqlite_http-0.1.0a4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 noop.cp311-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sqlite_http/__init__.py,sha256=8GXFU1nqrrYru_4gLteImIwxMHtahdb6miVLAy_g-tI,556
-sqlite_http/http0.dll,sha256=kkkn8LRcBo4KctGkMYYzHp9c0-xLGW1V8XP3kB3NW6E,15210365
-sqlite_http/version.py,sha256=Sx7I-AFj7noBhGjqVm3UIa5nn2dzDDf7ogRZFhVIbqA,81
-sqlite_http-0.1.0a3.dist-info/METADATA,sha256=d1vzOsgsH06IXSjcBxmUc1FGRkHZbztCjvDdJjGxv4o,515
-sqlite_http-0.1.0a3.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-sqlite_http-0.1.0a3.dist-info/top_level.txt,sha256=TBYmRyqZs7bPtMoy6C7UI8UkK-JP-yiT-HVEwXG_i_4,17
-sqlite_http-0.1.0a3.dist-info/RECORD,,
+sqlite_http/http0.dll,sha256=ovEYjsmubV69oKhxeHg-s5qGnDMu5QQ6uq-zj65qbII,15210365
+sqlite_http/version.py,sha256=Q5IzSF_n5CfKKas8SfhLSCkb9IvKBgfI1Ol0zdblb8U,81
+sqlite_http-0.1.0a4.dist-info/METADATA,sha256=FFvwBdHItCwF82YFFFV4r2IAYhpFIzWGFa62o3mci5c,515
+sqlite_http-0.1.0a4.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+sqlite_http-0.1.0a4.dist-info/top_level.txt,sha256=TBYmRyqZs7bPtMoy6C7UI8UkK-JP-yiT-HVEwXG_i_4,17
+sqlite_http-0.1.0a4.dist-info/RECORD,,
```

