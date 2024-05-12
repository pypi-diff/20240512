# Comparing `tmp/ipex_llm-2.1.0b20240510-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240511-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5319557 bytes, number of entries: 189
+Zip file size: 5319448 bytes, number of entries: 189
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3232 b- defN 24-May-07 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,47 +38,47 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-May-10 15:07 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-May-10 15:07 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   470528 b- defN 24-May-10 15:07 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   853504 b- defN 24-May-10 15:07 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856576 b- defN 24-May-10 15:07 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   844288 b- defN 24-May-10 15:07 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-May-10 15:07 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   530432 b- defN 24-May-10 15:07 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   496128 b- defN 24-May-10 15:07 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   471040 b- defN 24-May-10 15:07 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   556032 b- defN 24-May-10 15:07 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   530944 b- defN 24-May-10 15:07 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   549888 b- defN 24-May-10 15:07 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   525312 b- defN 24-May-10 15:07 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   586752 b- defN 24-May-10 15:07 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   561664 b- defN 24-May-10 15:07 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-May-10 15:07 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   524288 b- defN 24-May-10 15:07 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-May-10 15:07 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-May-10 15:07 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-May-10 15:07 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-May-10 15:07 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-May-10 15:07 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   126464 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128512 b- defN 24-May-10 15:07 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-May-10 15:07 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   561152 b- defN 24-May-10 15:07 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-May-11 15:08 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-May-11 15:08 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   470528 b- defN 24-May-11 15:08 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   853504 b- defN 24-May-11 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856576 b- defN 24-May-11 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   844288 b- defN 24-May-11 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-May-11 15:08 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   530432 b- defN 24-May-11 15:08 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   496128 b- defN 24-May-11 15:08 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   471040 b- defN 24-May-11 15:08 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   556032 b- defN 24-May-11 15:08 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   530944 b- defN 24-May-11 15:08 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   549888 b- defN 24-May-11 15:08 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   525312 b- defN 24-May-11 15:08 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   586752 b- defN 24-May-11 15:08 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   561664 b- defN 24-May-11 15:08 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-May-11 15:08 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   524288 b- defN 24-May-11 15:08 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-May-11 15:08 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-May-11 15:08 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-May-11 15:08 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-May-11 15:08 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-May-11 15:08 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   126464 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128512 b- defN 24-May-11 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-May-11 15:08 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   561152 b- defN 24-May-11 15:08 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    18709 b- defN 24-May-07 15:07 ipex_llm/serving/fastchat/ipex_llm_worker.py
@@ -177,15 +177,15 @@
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
 -rw-------  2.0 unx    18514 b- defN 24-Apr-26 15:08 ipex_llm/vllm/ipex_llm_gpu_executor.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
 -rw-------  2.0 unx     5941 b- defN 24-Apr-26 15:08 ipex_llm/vllm/engine/engine.py
 -rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240510.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240510.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     5125 b- defN 24-May-10 15:08 ipex_llm-2.1.0b20240510.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-May-10 15:08 ipex_llm-2.1.0b20240510.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-May-10 15:08 ipex_llm-2.1.0b20240510.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-May-10 15:08 ipex_llm-2.1.0b20240510.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    17921 b- defN 24-May-10 15:08 ipex_llm-2.1.0b20240510.dist-info/RECORD
-189 files, 13004888 bytes uncompressed, 5290925 bytes compressed:  59.3%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240511.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240511.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4013 b- defN 24-May-11 15:08 ipex_llm-2.1.0b20240511.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-May-11 15:08 ipex_llm-2.1.0b20240511.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-May-11 15:08 ipex_llm-2.1.0b20240511.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-May-11 15:08 ipex_llm-2.1.0b20240511.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17921 b- defN 24-May-11 15:08 ipex_llm-2.1.0b20240511.dist-info/RECORD
+189 files, 13003776 bytes uncompressed, 5290816 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -540,29 +540,29 @@
 
 Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240510.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240511.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240510.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240511.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240510.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240511.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240510.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240511.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240510.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240511.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240510.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240511.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240510.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240511.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,17 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	rex (bad)
-   180005636:	ds data16 add %al,(%rax)
+   180005634:	(bad)
+   180005635:	mov    %bh,(%rdi)
+   180005637:	data16 add %al,(%rax)
    18000563a:	add    %al,(%rax)
    18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800551e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055800
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000551e8
@@ -111728,16 +111728,17 @@
    18005e7fa:	add    $0x180,%eax
    18005e7ff:	add    %dh,0x76(%rax)
    18005e802:	add    $0x180,%eax
    18005e807:	add    %bh,0x76(%rax)
    18005e80a:	add    $0x180,%eax
    18005e80f:	add    %al,(%rax)
    18005e811:	add    %al,(%rax)
-   18005e813:	add    %al,0x37(%rax)
-   18005e816:	ds data16 add %al,(%rax)
+   18005e813:	add    %al,%ah
+   18005e815:	mov    %bh,(%rdi)
+   18005e817:	data16 add %al,(%rax)
    18005e81a:	add    %al,(%rax)
    18005e81c:	or     $0x50000000,%eax
    18005e821:	add    (%rax),%eax
    18005e823:	add    %ah,(%rax)
    18005e825:	repnz add $0x5de2000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:29 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,16 +5058,17 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	rex.B (bad)
-   1800049d6:	ds data16 add %al,(%rax)
+   1800049d4:	(bad)
+   1800049d5:	mov    %bh,(%rdi)
+   1800049d7:	data16 add %al,(%rax)
    1800049da:	add    %al,(%rax)
    1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c948
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:29 2024
+Time/Date		Sat May 11 15:03:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d200
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c948
@@ -123136,16 +123136,16 @@
    1800660bd:	add    %al,(%rax)
    1800660bf:	add    %bh,0x18005f6(%rax)
    1800660c5:	add    %al,(%rax)
    1800660c7:	add    %al,%al
    1800660c9:	testb  $0x0,0x180(%rip)        # 0x180066250
    1800660d0:	add    %al,(%rax)
    1800660d2:	add    %al,(%rax)
-   1800660d4:	rex.B (bad)
-   1800660d6:	ds data16 add %al,(%rax)
+   1800660d4:	(bad)
+   1800660d7:	data16 add %al,(%rax)
    1800660da:	add    %al,(%rax)
    1800660dc:	or     $0x50000000,%eax
    1800660e1:	add    (%rax),%eax
    1800660e3:	add    %al,0x53040006(,%rbp,2)
    1800660ea:	(bad)
 	...
    1800660ff:	add    %bh,0x70(%rax)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b148
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:02:37 2024
+Time/Date		Sat May 11 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b600
 SizeOfInitializedData	00000000000bf800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b148
@@ -117188,15 +117188,15 @@
    18006472a:	add    $0x180,%eax
    18006472f:	add    %dh,-0x2a(%rax)
    180064732:	add    $0x180,%eax
    180064737:	add    %bh,-0x2a(%rax)
    18006473a:	add    $0x180,%eax
    18006473f:	add    %al,(%rax)
    180064741:	add    %al,(%rax)
-   180064743:	add    %cl,0x663e37(%rip)        # 0x1806c8580
+   180064743:	add    %dl,0x663f88(%rcx)
    180064749:	add    %al,(%rax)
    18006474b:	add    %cl,0x50000000(%rip)        # 0x1d0064751
    180064751:	add    (%rax),%eax
    180064753:	add    %ah,(%rax)
    180064755:	push   %rcx
    180064756:	(bad)
    180064757:	add    %ah,(%rax)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800553f8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:04:36 2024
+Time/Date		Sat May 11 15:04:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055a00
 SizeOfInitializedData	00000000000bf200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000553f8
@@ -111831,15 +111831,17 @@
    18005e7da:	add    $0x180,%eax
    18005e7df:	add    %dh,0x76(%rax)
    18005e7e2:	add    $0x180,%eax
    18005e7e7:	add    %bh,0x76(%rax)
    18005e7ea:	add    $0x180,%eax
    18005e7ef:	add    %al,(%rax)
    18005e7f1:	add    %al,(%rax)
-   18005e7f3:	add    %al,0x663e(%rdi,%rsi,1)
+   18005e7f3:	add    %al,(%rsi)
+   18005e7f5:	mov    %edi,(%rdi)
+   18005e7f7:	data16 add %al,(%rax)
    18005e7fa:	add    %al,(%rax)
    18005e7fc:	or     $0x50000000,%eax
    18005e801:	add    (%rax),%eax
    18005e803:	add    %ah,(%rax)
    18005e805:	repnz add $0x5e02000,%eax
 	...
    18005e87f:	add    %dl,0x18005f5(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062938
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:02:37 2024
+Time/Date		Sat May 11 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c6800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062938
@@ -128639,17 +128639,19 @@
    18006bff7:	add    %al,%al
    18006bff9:	push   %rsi
    18006bffa:	(bad)
    18006bffb:	addb   $0x0,(%rcx)
    18006bffe:	add    %al,(%rax)
    18006c000:	add    %al,(%rax)
    18006c002:	add    %al,(%rax)
-   18006c004:	or     $0x663e37,%eax
-   18006c009:	add    %al,(%rax)
-   18006c00b:	add    %cl,0x50000000(%rip)        # 0x1d006c011
+   18006c004:	xchg   %eax,%ecx
+   18006c005:	mov    %bh,(%rdi)
+   18006c007:	data16 add %al,(%rax)
+   18006c00a:	add    %al,(%rax)
+   18006c00c:	or     $0x50000000,%eax
    18006c011:	add    (%rax),%eax
    18006c013:	add    %al,-0x4d7bfffa(%rsp,%rcx,8)
    18006c01a:	(bad)
 	...
    18006c07f:	add    %bh,%al
    18006c081:	iret
    18006c082:	(bad)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005cb58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:04:37 2024
+Time/Date		Sat May 11 15:04:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005d400
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005cb58
@@ -123256,16 +123256,17 @@
    18006609d:	add    %al,(%rax)
    18006609f:	add    %bh,0x18005f6(%rax)
    1800660a5:	add    %al,(%rax)
    1800660a7:	add    %al,%al
    1800660a9:	testb  $0x0,0x180(%rip)        # 0x180066230
    1800660b0:	add    %al,(%rax)
    1800660b2:	add    %al,(%rax)
-   1800660b4:	test   %esi,(%rdi)
-   1800660b6:	ds data16 add %al,(%rax)
+   1800660b4:	(bad)
+   1800660b5:	mov    %edi,(%rdi)
+   1800660b7:	data16 add %al,(%rax)
    1800660ba:	add    %al,(%rax)
    1800660bc:	or     $0x50000000,%eax
    1800660c1:	add    (%rax),%eax
    1800660c3:	add    %al,0x55040006(,%rbp,2)
    1800660ca:	(bad)
 	...
    1800660ff:	add    %bh,0x70(%rax)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180061648
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:02:37 2024
+Time/Date		Sat May 11 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061e00
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000061648
@@ -127298,17 +127298,19 @@
    18006a0d6:	add    %al,(%rax)
    18006a0d8:	shlb   $1,(%rsi)
    18006a0da:	(bad)
    18006a0db:	addb   $0x0,(%rcx)
    18006a0de:	add    %al,(%rax)
    18006a0e0:	add    %al,(%rax)
    18006a0e2:	add    %al,(%rax)
-   18006a0e4:	or     $0x663e37,%eax
-   18006a0e9:	add    %al,(%rax)
-   18006a0eb:	add    %cl,0x50000000(%rip)        # 0x1d006a0f1
+   18006a0e4:	xchg   %eax,%ecx
+   18006a0e5:	mov    %bh,(%rdi)
+   18006a0e7:	data16 add %al,(%rax)
+   18006a0ea:	add    %al,(%rax)
+   18006a0ec:	or     $0x50000000,%eax
    18006a0f1:	add    (%rax),%eax
    18006a0f3:	add    %al,(%rax)
    18006a0f5:	lods   %ds:(%rsi),%eax
    18006a0f6:	(bad)
    18006a0f7:	add    %al,(%rax)
    18006a0f9:	lahf
    18006a0fa:	(bad)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b868
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:04:36 2024
+Time/Date		Sat May 11 15:04:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c000
 SizeOfInitializedData	00000000000c6200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b868
@@ -121930,15 +121930,17 @@
    180064181:	(bad)
    180064182:	add    $0x180,%eax
    180064187:	add    %dl,%al
    180064189:	(bad)
    18006418a:	add    $0x180,%eax
    18006418f:	add    %al,(%rax)
    180064191:	add    %al,(%rax)
-   180064193:	add    %al,0x663e(%rdi,%rsi,1)
+   180064193:	add    %al,(%rsi)
+   180064195:	mov    %edi,(%rdi)
+   180064197:	data16 add %al,(%rax)
    18006419a:	add    %al,(%rax)
    18006419c:	or     $0x50000000,%eax
    1800641a1:	add    (%rax),%eax
    1800641a3:	add    %al,(%rax)
    1800641a5:	rex.WRX (bad)
    1800641a7:	add    %al,(%rax)
    1800641a9:	rex.X (bad)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180068aa8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:02:37 2024
+Time/Date		Sat May 11 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000069000
 SizeOfInitializedData	00000000000c8200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000068aa8
@@ -137914,17 +137914,19 @@
    180071c27:	add    %al,%al
    180071c29:	cmpsb  %es:(%rdi),%ds:(%rsi)
    180071c2a:	(bad)
    180071c2b:	addb   $0x0,(%rcx)
    180071c2e:	add    %al,(%rax)
    180071c30:	add    %al,(%rax)
    180071c32:	add    %al,(%rax)
-   180071c34:	or     $0x663e37,%eax
-   180071c39:	add    %al,(%rax)
-   180071c3b:	add    %cl,0x50000000(%rip)        # 0x1d0071c41
+   180071c34:	xchg   %eax,%ecx
+   180071c35:	mov    %bh,(%rdi)
+   180071c37:	data16 add %al,(%rax)
+   180071c3a:	add    %al,(%rax)
+   180071c3c:	or     $0x50000000,%eax
    180071c41:	add    (%rax),%eax
    180071c43:	add    %dl,%al
    180071c45:	sub    $0x21d00007,%eax
    180071c4a:	(bad)
 	...
    180071c7f:	add    %al,0x31(%rax)
    180071c82:	(bad)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062d58
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:04:36 2024
+Time/Date		Sat May 11 15:04:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063400
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062d58
@@ -132533,16 +132533,17 @@
    18006ccf7:	add    %al,%al
    18006ccf9:	push   %rsi
    18006ccfa:	(bad)
    18006ccfb:	addb   $0x0,(%rcx)
    18006ccfe:	add    %al,(%rax)
    18006cd00:	add    %al,(%rax)
    18006cd02:	add    %al,(%rax)
-   18006cd04:	test   %dh,(%rdi)
-   18006cd06:	ds data16 add %al,(%rax)
+   18006cd04:	(bad)
+   18006cd05:	mov    %edi,(%rdi)
+   18006cd07:	data16 add %al,(%rax)
    18006cd0a:	add    %al,(%rax)
    18006cd0c:	or     $0x50000000,%eax
    18006cd11:	add    (%rax),%eax
    18006cd13:	add    %dl,%al
    18006cd15:	fiadds (%rsi)
    18006cd17:	add    %dl,%al
    18006cd19:	movb   $0x0,(%rsi)
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,16 +5355,17 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	rex (bad)
-   180004a36:	ds data16 add %al,(%rax)
+   180004a34:	(bad)
+   180004a35:	mov    %bh,(%rdi)
+   180004a37:	data16 add %al,(%rax)
    180004a3a:	add    %al,(%rax)
    180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b658
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:29 2024
+Time/Date		Sat May 11 15:03:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005be00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b658
@@ -121795,16 +121795,17 @@
    1800641a1:	(bad)
    1800641a2:	add    $0x180,%eax
    1800641a7:	add    %dl,%al
    1800641a9:	(bad)
    1800641aa:	add    $0x180,%eax
    1800641af:	add    %al,(%rax)
    1800641b1:	add    %al,(%rax)
-   1800641b3:	add    %al,0x37(%rcx)
-   1800641b6:	ds data16 add %al,(%rax)
+   1800641b3:	add    %al,%ch
+   1800641b5:	mov    %bh,(%rdi)
+   1800641b7:	data16 add %al,(%rax)
    1800641ba:	add    %al,(%rax)
    1800641bc:	or     $0x50000000,%eax
    1800641c1:	add    (%rax),%eax
    1800641c3:	add    %al,(%rax)
    1800641c5:	rex.WRX (bad)
    1800641c7:	add    %al,(%rax)
    1800641c9:	rex (bad)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,16 +25509,17 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	rex (bad)
-   140014ac6:	ds data16 add %al,(%rax)
+   140014ac4:	(bad)
+   140014ac5:	mov    %bh,(%rdi)
+   140014ac7:	data16 add %al,(%rax)
    140014aca:	add    %al,(%rax)
    140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:05:02 2024
+Time/Date		Sat May 11 15:05:05 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189047,17 +189047,19 @@
    140093ee5:	add    %al,(%rax)
    140093ee7:	add    %al,(%rax)
    140093ee9:	cltd
    140093eea:	or     %al,0x1(%rax)
    140093eed:	add    %al,(%rax)
    140093eef:	add    %al,(%rax)
    140093ef1:	add    %al,(%rax)
-   140093ef3:	add    %bl,0x663e37(%rsi)
-   140093ef9:	add    %al,(%rax)
-   140093efb:	add    %cl,-0x34000000(%rip)        # 0x10c093f01
+   140093ef3:	add    %ah,(%rcx)
+   140093ef5:	mov    %edi,(%rdi)
+   140093ef7:	data16 add %al,(%rax)
+   140093efa:	add    %al,(%rax)
+   140093efc:	or     $0xcc000000,%eax
    140093f01:	add    (%rax),%eax
    140093f03:	add    %dl,-0x6ffff68d(%rax)
    140093f09:	movsxd (%rcx),%ecx
 	...
    140093f7f:	add    %al,0x1400977(%rax)
    140093f85:	add    %al,(%rax)
    140093f87:	add    %al,-0x61(%rbp)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:29 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,16 +24136,17 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	rex.B (bad)
-   140013ef6:	ds data16 add %al,(%rax)
+   140013ef4:	(bad)
+   140013ef5:	mov    %bh,(%rdi)
+   140013ef7:	data16 add %al,(%rax)
    140013efa:	add    %al,(%rax)
    140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,16 +24679,17 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	rex (bad)
-   140013fc6:	ds data16 add %al,(%rax)
+   140013fc4:	(bad)
+   140013fc5:	mov    %bh,(%rdi)
+   140013fc7:	data16 add %al,(%rax)
    140013fca:	add    %al,(%rax)
    140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,16 +40341,17 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %al,0x37(%rax)
-   14001f126:	ds data16 add %al,(%rax)
+   14001f123:	add    %al,%ah
+   14001f125:	mov    %bh,(%rdi)
+   14001f127:	data16 add %al,(%rax)
    14001f12a:	add    %al,(%rax)
    14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32229,16 +32229,17 @@
    1400191e5:	add    %al,(%rax)
    1400191e7:	add    %al,(%rax)
    1400191e9:	push   %rbp
    1400191ea:	add    %eax,0x1(%rax)
    1400191ed:	add    %al,(%rax)
    1400191ef:	add    %al,(%rax)
    1400191f1:	add    %al,(%rax)
-   1400191f3:	add    %al,0x37(%rax)
-   1400191f6:	ds data16 add %al,(%rax)
+   1400191f3:	add    %al,%ah
+   1400191f5:	mov    %bh,(%rdi)
+   1400191f7:	data16 add %al,(%rax)
    1400191fa:	add    %al,(%rax)
    1400191fc:	or     $0x20000000,%eax
    140019201:	add    (%rax),%eax
    140019203:	add    %dh,%al
    140019205:	movabs 0x18ff00001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:04:36 2024
+Time/Date		Sat May 11 15:04:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32355,15 +32355,17 @@
    1400191c5:	add    %al,(%rax)
    1400191c7:	add    %al,(%rax)
    1400191c9:	push   %rbp
    1400191ca:	add    %eax,0x1(%rax)
    1400191cd:	add    %al,(%rax)
    1400191cf:	add    %al,(%rax)
    1400191d1:	add    %al,(%rax)
-   1400191d3:	add    %al,0x663e(%rdi,%rsi,1)
+   1400191d3:	add    %al,(%rsi)
+   1400191d5:	mov    %edi,(%rdi)
+   1400191d7:	data16 add %al,(%rax)
    1400191da:	add    %al,(%rax)
    1400191dc:	or     $0x20000000,%eax
    1400191e1:	add    (%rax),%eax
    1400191e3:	add    %dh,-0x5f(%rax)
    1400191e6:	add    %eax,(%rax)
    1400191e8:	jo     0x14001917b
    1400191ea:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:27 2024
+Time/Date		Sat May 11 15:03:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27178,17 +27178,17 @@
    140015fe0:	push   $0x1400123
    140015fe5:	add    %al,(%rax)
    140015fe7:	add    %dh,0x23(%rax)
    140015fea:	add    %eax,0x1(%rax)
    140015fed:	add    %al,(%rax)
    140015fef:	add    %al,(%rax)
    140015ff1:	add    %al,(%rax)
-   140015ff3:	add    %bh,(%rdi)
-   140015ff5:	(bad)
-   140015ff6:	ds data16 add %al,(%rax)
+   140015ff3:	add    %al,%bl
+   140015ff5:	mov    %bh,(%rdi)
+   140015ff7:	data16 add %al,(%rax)
    140015ffa:	add    %al,(%rax)
    140015ffc:	or     $0x90000000,%eax
    140016001:	add    (%rax),%eax
    140016003:	add    %ch,%al
    140016005:	add    %eax,%gs:(%rax)
    140016008:	call   0x140016160
 	...
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:04:35 2024
+Time/Date		Sat May 11 15:04:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27305,15 +27305,15 @@
    140015fc0:	push   $0x1400123
    140015fc5:	add    %al,(%rax)
    140015fc7:	add    %dh,0x23(%rax)
    140015fca:	add    %eax,0x1(%rax)
    140015fcd:	add    %al,(%rax)
    140015fcf:	add    %al,(%rax)
    140015fd1:	add    %al,(%rax)
-   140015fd3:	add    %al,0x663e37(%rbx)
+   140015fd3:	add    %al,0x663f89(%rip)        # 0x140679f62
    140015fd9:	add    %al,(%rax)
    140015fdb:	add    %cl,-0x70000000(%rip)        # 0xd0015fe1
    140015fe1:	add    (%rax),%eax
    140015fe3:	add    %ch,0x65(%rax)
    140015fe6:	add    %eax,(%rax)
    140015fe8:	push   $0x155
 	...
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:27 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28462,17 +28462,17 @@
    1400170cd:	add    %al,(%rax)
    1400170cf:	add    %cl,0x1400133(%rax)
    1400170d5:	add    %al,(%rax)
    1400170d7:	add    %dl,0x1400133(%rax)
    1400170dd:	add    %al,(%rax)
    1400170df:	add    %al,(%rax)
    1400170e1:	add    %al,(%rax)
-   1400170e3:	add    %bh,(%rdi)
-   1400170e5:	(bad)
-   1400170e6:	ds data16 add %al,(%rax)
+   1400170e3:	add    %al,%ah
+   1400170e5:	mov    %bh,(%rdi)
+   1400170e7:	data16 add %al,(%rax)
    1400170ea:	add    %al,(%rax)
    1400170ec:	or     $0x90000000,%eax
    1400170f1:	add    (%rax),%eax
    1400170f3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170f7:	add    %ch,0x1(%rdx,%riz,2)
    1400170fb:	add    %al,(%rax)
    1400170fd:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:04:35 2024
+Time/Date		Sat May 11 15:04:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28607,15 +28607,15 @@
    1400170ad:	add    %al,(%rax)
    1400170af:	add    %cl,0x1400133(%rax)
    1400170b5:	add    %al,(%rax)
    1400170b7:	add    %dl,0x1400133(%rax)
    1400170bd:	add    %al,(%rax)
    1400170bf:	add    %al,(%rax)
    1400170c1:	add    %al,(%rax)
-   1400170c3:	add    %al,0x663e37(%rbx)
+   1400170c3:	add    %al,0x663f89(%rip)        # 0x14067b052
    1400170c9:	add    %al,(%rax)
    1400170cb:	add    %cl,-0x70000000(%rip)        # 0xd00170d1
    1400170d1:	add    (%rax),%eax
    1400170d3:	add    %ch,0x1(%rsi,%rsi,2)
    1400170d7:	add    %ch,0x1(%rsi,%riz,2)
 	...
    1400170ff:	add    %ah,(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32576,16 +32576,17 @@
    140019305:	add    %al,(%rax)
    140019307:	add    %al,(%rax)
    140019309:	push   %rbp
    14001930a:	add    %eax,0x1(%rax)
    14001930d:	add    %al,(%rax)
    14001930f:	add    %al,(%rax)
    140019311:	add    %al,(%rax)
-   140019313:	add    %al,0x37(%rax)
-   140019316:	ds data16 add %al,(%rax)
+   140019313:	add    %al,%ah
+   140019315:	mov    %bh,(%rdi)
+   140019317:	data16 add %al,(%rax)
    14001931a:	add    %al,(%rax)
    14001931c:	or     $0x20000000,%eax
    140019321:	add    (%rax),%eax
    140019323:	add    %bh,%ah
    140019325:	movabs %al,0x192fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Fri May 10 15:04:36 2024
+Time/Date		Sat May 11 15:04:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32701,15 +32701,17 @@
    1400192e5:	add    %al,(%rax)
    1400192e7:	add    %al,(%rax)
    1400192e9:	push   %rbp
    1400192ea:	add    %eax,0x1(%rax)
    1400192ed:	add    %al,(%rax)
    1400192ef:	add    %al,(%rax)
    1400192f1:	add    %al,(%rax)
-   1400192f3:	add    %al,0x663e(%rdi,%rsi,1)
+   1400192f3:	add    %al,(%rsi)
+   1400192f5:	mov    %edi,(%rdi)
+   1400192f7:	data16 add %al,(%rax)
    1400192fa:	add    %al,(%rax)
    1400192fc:	or     $0x20000000,%eax
    140019301:	add    (%rax),%eax
    140019303:	add    %bh,%ah
    140019305:	movabs %al,0x194fc0001
 	...
    14001937e:	add    %al,(%rax)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,16 +4028,17 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	rex (bad)
-   180004606:	ds data16 add %al,(%rax)
+   180004604:	(bad)
+   180004605:	mov    %bh,(%rdi)
+   180004607:	data16 add %al,(%rax)
    18000460a:	add    %al,(%rax)
    18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180062b48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri May 10 15:03:28 2024
+Time/Date		Sat May 11 15:03:32 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000063200
 SizeOfInitializedData	00000000000c7c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000062b48
@@ -132428,16 +132428,17 @@
    18006cd17:	add    %al,%al
    18006cd19:	push   %rsi
    18006cd1a:	(bad)
    18006cd1b:	addb   $0x0,(%rcx)
    18006cd1e:	add    %al,(%rax)
    18006cd20:	add    %al,(%rax)
    18006cd22:	add    %al,(%rax)
-   18006cd24:	rex (bad)
-   18006cd26:	ds data16 add %al,(%rax)
+   18006cd24:	(bad)
+   18006cd25:	mov    %bh,(%rdi)
+   18006cd27:	data16 add %al,(%rax)
    18006cd2a:	add    %al,(%rax)
    18006cd2c:	or     $0x50000000,%eax
    18006cd31:	add    (%rax),%eax
    18006cd33:	add    %dl,%al
    18006cd35:	fiadds (%rsi)
    18006cd37:	add    %dl,%al
    18006cd39:	(bad)
```

## Comparing `ipex_llm-2.1.0b20240510.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240511.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240510.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240511.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240510.dist-info/METADATA` & `ipex_llm-2.1.0b20240511.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240510
+Version: 2.1.0b20240511
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240510) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240511) ; extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
 Requires-Dist: numpy (==1.26.4) ; extra == 'llama-index'
 Requires-Dist: sentencepiece ; extra == 'llama-index'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'llama-index'
@@ -51,47 +51,31 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240510) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240510) ; extra == 'xpu'
-Provides-Extra: xpu-2-0
-Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
-Requires-Dist: protobuf ; extra == 'xpu-2-0'
-Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
-Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
-Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
-Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
-Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
-Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
-Requires-Dist: tabulate ; extra == 'xpu-2-0'
-Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
-Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240510) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240510) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240511) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240511) ; extra == 'xpu'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240510) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240510) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240511) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240511) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240510.dist-info/RECORD` & `ipex_llm-2.1.0b20240511.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -38,46 +38,46 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=8PY59_2g5AERU7lWR1z7Uaaay9B3HcV4wgJ8d972_6s,36352
-ipex_llm/libs/bloom.dll,sha256=YOFjBUPo9vU7Hy0bErhLr637rKPFlNl3C1ACKZEhJy8,470528
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=bWyK6dmae8UXEyc7e1caUh5BdYNfd795Q1DPrGZsjCo,853504
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=-O0LBen7L_hZ7rKkNQ9Y0j3ph3rE0qiHYAIW5Ly9ecQ,856576
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=3V_XE2D-GzTqAW1cj31Yc3i54kMzJsN2YXUyQZeR300,844288
-ipex_llm/libs/gptneox-api.dll,sha256=ABvrp4bMOy-BszF66IdMZGHCiW9A28kQPwU15C56oGY,24576
-ipex_llm/libs/gptneox.dll,sha256=nA3IXv6aSmNWJzd04KWFTi0NjpzEcyMRPG5nPkvdTXI,530432
-ipex_llm/libs/libbloom_avx.dll,sha256=w5V85QNxt7PqEwOPlsJ9p6iau4J29cDmpQz421GdQdY,496128
-ipex_llm/libs/libbloom_vnni.dll,sha256=B1ODA0kdmGvVEvC_Mjlpk1RWXv0phzvGnORqS1EVxUI,471040
-ipex_llm/libs/libgptneox_avx.dll,sha256=0D6w1pFRmvDtJFDKSAeQ16ZTqgDpgvpXQbTsDI20-bs,556032
-ipex_llm/libs/libgptneox_vnni.dll,sha256=SFxJb_0UlA9P16mZ6ufWObBRmP3HzC6POfvgl12Ewpk,530944
-ipex_llm/libs/libllama_avx.dll,sha256=9Ss5eh-OJkf9bL2_lR1ZZT8xLg_RTsK0BCrFWJ1S4Jg,549888
-ipex_llm/libs/libllama_vnni.dll,sha256=82pGSkuKEHH-HerztjdPyORs6BrJYoHT78-fNc7QqhM,525312
-ipex_llm/libs/libstarcoder_avx.dll,sha256=icgYnsBWXTdkGMBs6xyBiHKxvR4O1_qPxDDXk2eBTGE,586752
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=O_APNY81LnjwY-fWTzuxH_38TgcBXSI_6g8t6nLcdVk,561664
-ipex_llm/libs/llama-api.dll,sha256=lo_UGSJvt1wcDei3mhqaOdxyiB_0YBB4EY_v_o70khU,25088
-ipex_llm/libs/llama.dll,sha256=kDE6p-Dme9ZlJOTNqQwmR43Xmasx-u9luOnegthyCBU,524288
-ipex_llm/libs/main-bloom.exe,sha256=M25BRZzWnHsd2rIVlozSuQP8Z3PSsyKHvzlH-OexRn8,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=ZeJA_3q_2tN9RhKJlstso7G4KJ9hDENwv1DK1EQ7b-s,726016
-ipex_llm/libs/main-gptneox.exe,sha256=ZVllvfBc3tY6Q9INSkckYy6soNUGx26enOgq9Av5D48,98816
-ipex_llm/libs/main-llama.exe,sha256=XTfGDNyV97jWVqNqMx804VYix2SIgcYRd20ZmX64zlQ,99840
-ipex_llm/libs/main-starcoder.exe,sha256=iWyOHF8Ow16PmLKkeJGUJjgfisMF95Gub7JVTUUw5Yc,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=u6DBGyhJSlrfXgpK_mM8y6bAaQoqufEhmor5JnvmJ2Y,126464
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=wDY7YxL5Nh7MRY_VYUCZvCDetm9A3Z5EQVDhAjjaeOQ,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=biF5UBYDD_htRqUlb0bl0kb_ghwIzuLklUo-ATayopQ,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=wByktOVcOZus7ZEnFvX0RYrggNKebO6-Z7OXX_YWVRA,104448
-ipex_llm/libs/quantize-llama.exe,sha256=Ocs-0POZ81Z3kGEtwzYONV8lwQc2EpbdIR2dKL8Hzqk,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=TC-4yZRqkTn7Jg4tnzdObekGVKOeiC89V4pNne6pQls,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=UB1IPePfBrzWSqY4U73KodN-t_D7Q1IO9yaTejeQktQ,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=k1LGSRBhBl7OWb11U03Suc3LuBu64FCLSoSoacPWYxI,128512
-ipex_llm/libs/starcoder-api.dll,sha256=2IjVy0Ka2F1-IdvrBtyyImQ4y00018F2ffjrP8M-vt0,21504
-ipex_llm/libs/starcoder.dll,sha256=uA5TEAA9AxibUEiyXwose4RZ-LWNNDfpXmtHUd5JP2I,561152
+ipex_llm/libs/bloom-api.dll,sha256=VQ0VR24P6z_eX_i9KUhBDh58IpcTij0ldbH9DPAi17s,36352
+ipex_llm/libs/bloom.dll,sha256=Jvz-B85i32VA6sZpsy3n8Uzy4LwwBNDac1M9mg1y0Ss,470528
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=sj9u1K-HwCHrePrtYfFA9Ji224ENbYjLnnGRPPr29iA,853504
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=hcPmjPMh3C-_DVErARC93PeXEAC5-HmOKnXwUsjU-ZU,856576
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=QuEttYuEM75URFbH2VvcX4gwfdOfgfUO3xX5bcOK-Xo,844288
+ipex_llm/libs/gptneox-api.dll,sha256=tftEfqhtpgZcPA0wsOzX6fGcjPHtHJihQeUCNYpwJrg,24576
+ipex_llm/libs/gptneox.dll,sha256=Mws1r4KX-bE8kZoqsCOGZbf3mJGdF9l4JOs-4suwlTE,530432
+ipex_llm/libs/libbloom_avx.dll,sha256=PsubnRd3rmhDmpCPCJQ_TyfRqIgtyZoq0p21fdNyOlo,496128
+ipex_llm/libs/libbloom_vnni.dll,sha256=uA-S5NBdm4V8GtJcKwWxQZvnfm7MDu79mao5V5t8O0Y,471040
+ipex_llm/libs/libgptneox_avx.dll,sha256=muOqrjtlJ7Pcb7iE72G41GVUGQGOWf9nJlUDPtqTXok,556032
+ipex_llm/libs/libgptneox_vnni.dll,sha256=gpjdeoRfdFTCbGaBFwEWFKyrqhQ7AMmWbhWZVrpJKBU,530944
+ipex_llm/libs/libllama_avx.dll,sha256=xSmWbK5uLaiUbU-ExlQ-6f3SKd6GWIM6zo4TgtrcFH4,549888
+ipex_llm/libs/libllama_vnni.dll,sha256=zdKkrnB1JDbbO6LFCvQIeJjcRlvLfQBL8cVpjqzuGv0,525312
+ipex_llm/libs/libstarcoder_avx.dll,sha256=MgsUmeaOfItSPDbTOx_egaIx3A3guVGp3Er0JcOyvsI,586752
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=80ss7_Pccxiexx3ulceH8-TSjK2fAolQGij0E2_nBPY,561664
+ipex_llm/libs/llama-api.dll,sha256=gefEj2JlMnP-a2t_USa7A6DVK_1TLdtyVhMR212cbXc,25088
+ipex_llm/libs/llama.dll,sha256=5ElGQXtoiJiWpyv0Nqr_HUCv0rIbezmW0Ahy-eFpb_U,524288
+ipex_llm/libs/main-bloom.exe,sha256=RRjbu6lbg4H-zQPErRnmOTc158HbAbFCmjU8ONIK-Wg,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=vCCF_5GRrkeSu5MyOIa4inbVH0hHY7KhssTTkIhJ10g,726016
+ipex_llm/libs/main-gptneox.exe,sha256=ALC1TKnMn8HCBMa0QjxHZ88KUGV6kLTTiwxmuYq-vJw,98816
+ipex_llm/libs/main-llama.exe,sha256=Fw2rcYBrRwO-JrYDbymdtew4iVIIjwR0Me_XYaQ9n2Q,99840
+ipex_llm/libs/main-starcoder.exe,sha256=ekMx5hwErixJs6-E8XCwYXwArs3dqVWicht-wej7x5s,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=p3eqSoTMm6QamNoXlMKJ-2f-QxzIphWg3IGYfKXq3Zg,126464
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=zZCNoO2xsgCBlV49MU30IwD8B2_pYBJKN4NP7HGXJIU,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=FEKDAx1dC9q0ppbXTJqOLUBREf1mMCnKEhPR_-jHIyY,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=4-3m7COWVIezVBzJZybqLh1-FrZIG2Nx_61LwkS4GHg,104448
+ipex_llm/libs/quantize-llama.exe,sha256=X6CexqJrCTIDsmap5594OZEdbdbxKwZ2i72ZeoJJK4Y,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=5hwQ3XTDLmXPlaXJCZH9LE8RRilnKaaR6sYV8kfUUhQ,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=RMaNPjf0nUJ6a9i98gFycD11Dnj2gfh6SUK1zQf8b5A,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=gxEm52iSMqb_RNRsFBOzO9w37gcCqV45B7PhB1oniD0,128512
+ipex_llm/libs/starcoder-api.dll,sha256=tY4VGM9-uPwY8y2lDyGlk6MfHut0M4wxm8Jrl_v1rTs,21504
+ipex_llm/libs/starcoder.dll,sha256=lVukA6yZ5jz64Q8MB7qzgFs4TvdcVyDk1tvYU6cuDOg,561152
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=cxg-L4hPIUPr9tQ5TVwCdH2nt7IdcAmPmkKcK13vI7s,18709
@@ -176,14 +176,14 @@
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
 ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/ipex_llm_gpu_executor.py,sha256=pY-8XxRRX1_9MTW0TUTidxHmjmXKGsvs1AIIVWU21yM,18514
 ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/engine/engine.py,sha256=mVuCyoTcCX7KnK819-8fL_rNAu05WF_gql6jEcZ9bn8,5941
 ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
-ipex_llm-2.1.0b20240510.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240510.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240510.dist-info/METADATA,sha256=1CNJQN3MUzGf1F1yCspNXDz2dfkF6YRL1WJt70zW-2A,5125
-ipex_llm-2.1.0b20240510.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240510.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240510.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240510.dist-info/RECORD,,
+ipex_llm-2.1.0b20240511.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240511.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240511.dist-info/METADATA,sha256=nyPWMsFM6hDL5DqnDvSwWp_0LFIDrBIxolz2Zx1ed3s,4013
+ipex_llm-2.1.0b20240511.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240511.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240511.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240511.dist-info/RECORD,,
```

