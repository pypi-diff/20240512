# Comparing `tmp/soar_sml-9.6.2a1-cp39-cp39-win_amd64.whl.zip` & `tmp/soar_sml-9.6.2a42-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1847655 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat  3599360 b- defN 24-May-02 16:35 soar_sml/Soar.dll
--rw-rw-rw-  2.0 fat   535216 b- defN 24-May-02 16:35 soar_sml/Soar.lib
--rw-rw-rw-  2.0 fat   775168 b- defN 24-May-02 16:35 soar_sml/_Python_sml_ClientInterface.pyd
--rw-rw-rw-  2.0 fat   158424 b- defN 24-May-02 16:27 soar_sml/__init__.py
--rw-rw-rw-  2.0 fat     4463 b- defN 24-May-02 16:34 soar_sml-9.6.2a1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 24-May-02 16:34 soar_sml-9.6.2a1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-02 16:34 soar_sml-9.6.2a1.dist-info/entry_points.txt
-?rw-------  2.0 fat      642 b- stor 85-Oct-26 08:21 soar_sml-9.6.2a1.dist-info/RECORD
-8 files, 5073371 bytes uncompressed, 1846551 bytes compressed:  63.6%
+Zip file size: 1848018 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat  3599360 b- defN 24-May-12 13:44 soar_sml/Soar.dll
+-rw-rw-rw-  2.0 fat   535216 b- defN 24-May-12 13:44 soar_sml/Soar.lib
+-rw-rw-rw-  2.0 fat   775168 b- defN 24-May-12 13:44 soar_sml/_Python_sml_ClientInterface.pyd
+-rw-rw-rw-  2.0 fat   158424 b- defN 24-May-12 13:43 soar_sml/__init__.py
+-rw-rw-rw-  2.0 fat     5165 b- defN 24-May-12 13:44 soar_sml-9.6.2a42.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 24-May-12 13:44 soar_sml-9.6.2a42.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-12 13:44 soar_sml-9.6.2a42.dist-info/entry_points.txt
+?rw-------  2.0 fat      646 b- stor 85-Oct-26 08:21 soar_sml-9.6.2a42.dist-info/RECORD
+8 files, 5074077 bytes uncompressed, 1846906 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: soar_sml/_Python_sml_ClientInterface.pyd
 Comment: 
 
 Filename: soar_sml/__init__.py
 Comment: 
 
-Filename: soar_sml-9.6.2a1.dist-info/METADATA
+Filename: soar_sml-9.6.2a42.dist-info/METADATA
 Comment: 
 
-Filename: soar_sml-9.6.2a1.dist-info/WHEEL
+Filename: soar_sml-9.6.2a42.dist-info/WHEEL
 Comment: 
 
-Filename: soar_sml-9.6.2a1.dist-info/entry_points.txt
+Filename: soar_sml-9.6.2a42.dist-info/entry_points.txt
 Comment: 
 
-Filename: soar_sml-9.6.2a1.dist-info/RECORD
+Filename: soar_sml-9.6.2a42.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## soar_sml/Soar.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018027acd8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu May  2 16:35:05 2024
+Time/Date		Sun May 12 13:44:28 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	38
 SizeOfCode		0000000000282600
 SizeOfInitializedData	00000000000f2600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000027acd8
@@ -873707,23 +873707,24 @@
    1802b941f:	(bad)
    1802b9420:	cmp    %ch,(%rcx,%rbp,1)
    1802b9423:	addb   $0x0,(%rcx)
    1802b9426:	add    %al,(%rax)
    1802b9428:	pop    %rax
    1802b9429:	mov    $0x18028,%esp
    1802b942e:	add    %al,(%rax)
-   1802b9430:	xor    %esi,(%rsi)
-   1802b9432:	cmp    (%rbx),%dh
-   1802b9434:	xor    $0x3a,%al
-   1802b9436:	xor    $0x37,%eax
+   1802b9430:	xor    %esi,(%rbx)
+   1802b9432:	cmp    (%rsp,%rsi,1),%dh
+   1802b9435:	cmp    (%rdx),%dh
+   1802b9437:	xor    %al,(%rax)
+   1802b9439:	add    %al,(%rax)
    1802b943b:	add    %al,(%rax)
    1802b943d:	add    %al,(%rax)
    1802b943f:	add    %cl,0x61(%rbp)
    1802b9442:	jns    0x1802b9464
-   1802b9444:	and    %dh,(%rdx)
+   1802b9444:	xor    %esi,(%rdx)
    1802b9446:	and    %dh,(%rdx)
    1802b9448:	xor    %dh,(%rdx)
    1802b944a:	xor    $0x0,%al
    1802b944c:	add    %al,(%rax)
    1802b944e:	add    %al,(%rax)
    1802b9450:	push   $0x1803005
    1802b9455:	add    %al,(%rax)
@@ -969099,15 +969100,15 @@
    1802f5bc9:	rex.WXB sub %al,0x1(%r8)
    1802f5bd0:	push   $0x180284b
    1802f5bd5:	add    %al,(%rax)
    1802f5bd7:	add    %dh,0x4b(%rax)
    1802f5bda:	sub    %al,0x1(%rax)
    1802f5be0:	add    %al,(%rax)
    1802f5be2:	add    %al,(%rax)
-   1802f5be4:	mov    $0x6633c0,%ecx
+   1802f5be4:	mov    $0x6640c7,%esp
    1802f5be9:	add    %al,(%rax)
    1802f5beb:	add    %cl,0x3c000000(%rip)        # 0x1bc2f5bf1
    1802f5bf1:	add    (%rax),%eax
    1802f5bf3:	add    %dh,%ah
    1802f5bf5:	rex.WXB xor %al,(%r8)
    1802f5bf8:	hlt
    1802f5bf9:	xor    $0x30,%eax
```

## Comparing `soar_sml-9.6.2a1.dist-info/METADATA` & `soar_sml-9.6.2a42.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: soar-sml
-Version: 9.6.2a1
-Summary: Raw SML Bindings to the SOAR Cognitive Architecture
-Requires-Python: >=3.8,<3.12
+Version: 9.6.2a42
+Summary: Raw SML Bindings to the Soar Cognitive Architecture
+Requires-Python: >=3.8
 License: BSD
-Author: 
-Keywords: soar
+Author: John E. Laird, Allen Newell, Paul Rosenbloom, A. Deschamps, A. Mininger, A. Nickels, A. Nuxoll, A. Turner, B. Stearns, C. Dettmering, D. Pearson, D. Ray, I. Hines, J. Boggs, J. Crossman, J. Kirk, J. Li, J. Voigt, J. Xu, K. Coulter, L. Goeddel, M. Assanie, M. Bloch, M. Lanting, M. Schmidt, M. Tinkerhess, N. Derbinsky, N. Glenn, N. Gorski, N. Timpko, R. Marinier, R. Wray, S. Jones, S. Lathrop, S. Mohan, S. Nason, S. Wallace, S. Wintermute, Y. Wang
+Maintainer-email: Nathan Glenn <garfieldnate@gmail.com>, Center for Integrated Cognition
+Keywords: soar,sml,cog-arch,cognitive architecture,cognitive,soar-sml,ai
 Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://soar.eecs.umich.edu/
+Project-URL: Repository, https://github.com/SoarGroup/Soar
 Provides-Extra: compat
 Requires-Dist: soar-compat; extra == 'compat'
 Description-Content-Type: text/markdown
 
 
 # Soar
```

