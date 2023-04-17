# Comparing `tmp/abch_tree_sitter_solidity-1.0.6-py3-none-win_amd64.whl.zip` & `tmp/abch_tree_sitter_solidity-1.0.7-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 54365 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       44 b- defN 23-Apr-17 14:22 tree_sitter_solidity/__init__.py
--rw-rw-rw-  2.0 fat      396 b- defN 23-Apr-17 14:22 tree_sitter_solidity/core.py
--rw-rw-rw-  2.0 fat   438272 b- defN 23-Apr-17 14:23 tree_sitter_solidity/solidity.dll
--rw-rw-rw-  2.0 fat     1060 b- defN 23-Apr-17 14:25 abch_tree_sitter_solidity-1.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2055 b- defN 23-Apr-17 14:25 abch_tree_sitter_solidity-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-Apr-17 14:25 abch_tree_sitter_solidity-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-17 14:25 abch_tree_sitter_solidity-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      739 b- defN 23-Apr-17 14:25 abch_tree_sitter_solidity-1.0.6.dist-info/RECORD
-8 files, 442685 bytes uncompressed, 53051 bytes compressed:  88.0%
+Zip file size: 54363 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       44 b- defN 23-Apr-17 19:14 tree_sitter_solidity/__init__.py
+-rw-rw-rw-  2.0 fat      396 b- defN 23-Apr-17 19:14 tree_sitter_solidity/core.py
+-rw-rw-rw-  2.0 fat   438272 b- defN 23-Apr-17 19:15 tree_sitter_solidity/solidity.dll
+-rw-rw-rw-  2.0 fat     1060 b- defN 23-Apr-17 19:17 abch_tree_sitter_solidity-1.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2055 b- defN 23-Apr-17 19:17 abch_tree_sitter_solidity-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Apr-17 19:17 abch_tree_sitter_solidity-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-17 19:17 abch_tree_sitter_solidity-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      739 b- defN 23-Apr-17 19:17 abch_tree_sitter_solidity-1.0.7.dist-info/RECORD
+8 files, 442685 bytes uncompressed, 53049 bytes compressed:  88.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: tree_sitter_solidity/core.py
 Comment: 
 
 Filename: tree_sitter_solidity/solidity.dll
 Comment: 
 
-Filename: abch_tree_sitter_solidity-1.0.6.dist-info/LICENSE
+Filename: abch_tree_sitter_solidity-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: abch_tree_sitter_solidity-1.0.6.dist-info/METADATA
+Filename: abch_tree_sitter_solidity-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: abch_tree_sitter_solidity-1.0.6.dist-info/WHEEL
+Filename: abch_tree_sitter_solidity-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: abch_tree_sitter_solidity-1.0.6.dist-info/top_level.txt
+Filename: abch_tree_sitter_solidity-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: abch_tree_sitter_solidity-1.0.6.dist-info/RECORD
+Filename: abch_tree_sitter_solidity-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tree_sitter_solidity/solidity.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000c2f0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 17 14:23:35 2023
+Time/Date		Mon Apr 17 19:15:52 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	34
 SizeOfCode		000000000000be00
 SizeOfInitializedData	000000000005f400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000c2f0
@@ -80955,16 +80955,16 @@
    18006a88a:	add    %al,0x1(%rax)
    18006a890:	sbb    %dl,%cl
    18006a892:	add    %al,0x1(%rax)
    18006a898:	and    %dl,%cl
    18006a89a:	add    %al,0x1(%rax)
    18006a8a0:	add    %al,(%rax)
    18006a8a2:	add    %al,(%rax)
-   18006a8a4:	addr32 push %rsi
-   18006a8a6:	cmp    $0x64,%eax
+   18006a8a4:	call   0x1806ae643
+   18006a8a9:	add    %al,(%rax)
    18006a8ab:	add    %cl,0x58000000(%rip)        # 0x1d806a8b1
    18006a8b1:	add    (%rax),%al
    18006a8b3:	add    %ah,0x6(%rcx,%rbp,4)
    18006a8b7:	add    %ah,0x6(%rbx,%rbx,4)
 	...
    18006a8ff:	add    %bl,(%rax)
    18006a901:	add    %al,(%rax)
```

## Comparing `abch_tree_sitter_solidity-1.0.6.dist-info/LICENSE` & `abch_tree_sitter_solidity-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `abch_tree_sitter_solidity-1.0.6.dist-info/METADATA` & `abch_tree_sitter_solidity-1.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abch-tree-sitter-solidity
-Version: 1.0.6
+Version: 1.0.7
 Summary: Solidity grammar for the Tree-sitter parsing library
 Home-page: https://github.com/Ackee-Blockchain/tree-sitter-solidity
 Author: Ackee Blockchain
 License: MIT
 Project-URL: Source, https://github.com/Ackee-Blockchain/tree-sitter-solidity
 Platform: any
 Requires-Python: >=3.7
```

## Comparing `abch_tree_sitter_solidity-1.0.6.dist-info/RECORD` & `abch_tree_sitter_solidity-1.0.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 tree_sitter_solidity/__init__.py,sha256=dBy830gvSzEAaxSaIuSnit8rJ1h7R_0vl0qX5ivDwFY,44
 tree_sitter_solidity/core.py,sha256=mhyS4mR-Z_1BITJMpCfeU1u-oIe6YbsJlARjQ67ufSY,396
-tree_sitter_solidity/solidity.dll,sha256=4xtslSCQjkAFLNAv1KFm8pZ-OFGn081wIxoiO-Lg9Is,438272
-abch_tree_sitter_solidity-1.0.6.dist-info/LICENSE,sha256=GPd7_hXjRWKN4WvgAGyM6Yd588MLzpuAQjjJRCwTq8w,1060
-abch_tree_sitter_solidity-1.0.6.dist-info/METADATA,sha256=kmr_jMHdZj2cd3bSRDRa6mCLue_UeHplr9tUpZhfVwo,2055
-abch_tree_sitter_solidity-1.0.6.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-abch_tree_sitter_solidity-1.0.6.dist-info/top_level.txt,sha256=ZDlLIOwRGN8Kb_Im4c8b9DybPg9ShmIDze61oVAmXaQ,21
-abch_tree_sitter_solidity-1.0.6.dist-info/RECORD,,
+tree_sitter_solidity/solidity.dll,sha256=z3_gpvboIZ07OplocdsHnEGnnnRlZNik2EwQR7GWYII,438272
+abch_tree_sitter_solidity-1.0.7.dist-info/LICENSE,sha256=GPd7_hXjRWKN4WvgAGyM6Yd588MLzpuAQjjJRCwTq8w,1060
+abch_tree_sitter_solidity-1.0.7.dist-info/METADATA,sha256=reZdOYoNCKT168NkSoPFCJLJHsyEixRGiKhCCBN8wWc,2055
+abch_tree_sitter_solidity-1.0.7.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+abch_tree_sitter_solidity-1.0.7.dist-info/top_level.txt,sha256=ZDlLIOwRGN8Kb_Im4c8b9DybPg9ShmIDze61oVAmXaQ,21
+abch_tree_sitter_solidity-1.0.7.dist-info/RECORD,,
```

