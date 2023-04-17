# Comparing `tmp/gsfarc-1.0.4.zip` & `tmp/gsfarc-2.0.0.dev18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,67 +1,80 @@
-Zip file size: 142216 bytes, number of entries: 65
--rw-rw-rw-  2.0 fat     3233 b- defN 17-Jul-06 09:07 gsfarc-1.0.4/LegalAndCopyrightNotices.txt
--rw-rw-rw-  2.0 fat     1106 b- defN 17-Jul-06 09:49 gsfarc-1.0.4/LICENSE.txt
--rw-rw-rw-  2.0 fat       64 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/MANIFEST.in
--rw-rw-rw-  2.0 fat      247 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/PKG-INFO
--rw-rw-rw-  2.0 fat      138 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/requirements.txt
--rw-rw-rw-  2.0 fat      264 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/setup.cfg
--rw-rw-rw-  2.0 fat     1836 b- defN 17-Jul-06 09:59 gsfarc-1.0.4/setup.py
--rw-rw-rw-  2.0 fat      302 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/api.rst
--rw-rw-rw-  2.0 fat     9791 b- defN 17-Jul-06 12:07 gsfarc-1.0.4/doc/source/conf.py
--rw-rw-rw-  2.0 fat     7812 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/index.rst
--rw-rw-rw-  2.0 fat    14759 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/images/create_tool.png
--rw-rw-rw-  2.0 fat     9729 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/images/create_tool_arcgispro.png
--rw-rw-rw-  2.0 fat    17723 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/images/spectral_index.png
--rw-rw-rw-  2.0 fat     8692 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/images/spectral_index_arcgispro.png
--rw-rw-rw-  2.0 fat    19577 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/images/spectral_index_input.png
--rw-rw-rw-  2.0 fat    10614 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/images/spectral_index_input_arcgispro.png
--rw-rw-rw-  2.0 fat    48131 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/doc/source/images/spectral_index_result.png
--rw-rw-rw-  2.0 fat     4820 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptoolbox.py
--rw-rw-rw-  2.0 fat      977 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/system.py
--rw-rw-rw-  2.0 fat       54 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/__init__.py
--rw-rw-rw-  2.0 fat     2887 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.CreateTool.pyt.xml
--rw-rw-rw-  2.0 fat     3364 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.pyt
--rw-rw-rw-  2.0 fat      954 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.pyt.xml
--rw-rw-rw-  2.0 fat     1887 b- defN 17-Jul-06 09:49 gsfarc-1.0.4/gsfarc/gptool/help.py
--rw-rw-rw-  2.0 fat        0 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/__init__.py
--rw-rw-rw-  2.0 fat     8019 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/builder.py
--rw-rw-rw-  2.0 fat     2206 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/template.py
--rw-rw-rw-  2.0 fat        0 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/__init__.py
--rw-rw-rw-  2.0 fat      964 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/basic.py
--rw-rw-rw-  2.0 fat      589 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/basicarray.py
--rw-rw-rw-  2.0 fat      105 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/bool.py
--rw-rw-rw-  2.0 fat      138 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/boolarray.py
--rw-rw-rw-  2.0 fat      111 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/boolean.py
--rw-rw-rw-  2.0 fat      103 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/byte.py
--rw-rw-rw-  2.0 fat      135 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/bytearray.py
--rw-rw-rw-  2.0 fat      111 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/double.py
--rw-rw-rw-  2.0 fat      136 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/doublearray.py
--rw-rw-rw-  2.0 fat     2977 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviagcrops.py
--rw-rw-rw-  2.0 fat     2982 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviraster.py
--rw-rw-rw-  2.0 fat     1546 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviuri.py
--rw-rw-rw-  2.0 fat     2978 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/envivector.py
--rw-rw-rw-  2.0 fat      109 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/float.py
--rw-rw-rw-  2.0 fat      134 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/floatarray.py
--rw-rw-rw-  2.0 fat      101 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/int.py
--rw-rw-rw-  2.0 fat      133 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/intarray.py
--rw-rw-rw-  2.0 fat      103 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/long.py
--rw-rw-rw-  2.0 fat      107 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/long64.py
--rw-rw-rw-  2.0 fat      132 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/long64array.py
--rw-rw-rw-  2.0 fat      128 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/longarray.py
--rw-rw-rw-  2.0 fat      273 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/string.py
--rw-rw-rw-  2.0 fat      141 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/stringarray.py
--rw-rw-rw-  2.0 fat      103 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/uint.py
--rw-rw-rw-  2.0 fat      128 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/uintarray.py
--rw-rw-rw-  2.0 fat      105 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulong.py
--rw-rw-rw-  2.0 fat      109 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulong64.py
--rw-rw-rw-  2.0 fat      134 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulong64array.py
--rw-rw-rw-  2.0 fat      130 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulongarray.py
--rw-rw-rw-  2.0 fat        0 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/gsfarc/gptool/parameter/templates/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/gsfarc.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/gsfarc.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat      247 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/gsfarc.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       11 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/gsfarc.egg-info/requires.txt
--rw-rw-rw-  2.0 fat     2346 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/gsfarc.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        7 b- defN 17-Jul-13 10:50 gsfarc-1.0.4/gsfarc.egg-info/top_level.txt
--rw-rw-rw-  2.0 fat     1406 b- defN 17-Jul-06 07:40 gsfarc-1.0.4/scripts/creategsftoolbox.py
-65 files, 198151 bytes uncompressed, 130982 bytes compressed:  33.9%
+Zip file size: 46235 bytes, number of entries: 78
+-rw-r--r--  2.0 unx       54 b- defN 23-Apr-17 19:50 gsfarc/__init__.py
+-rw-r--r--  2.0 unx     2010 b- defN 23-Apr-17 19:50 gsfarc/__main__.py
+-rw-r--r--  2.0 unx     4820 b- defN 23-Apr-17 19:50 gsfarc/gptoolbox.py
+-rw-r--r--  2.0 unx      977 b- defN 23-Apr-17 19:50 gsfarc/system.py
+-rw-r--r--  2.0 unx     2887 b- defN 23-Apr-17 19:50 gsfarc/esri/toolboxes/GSF.CreateTool.pyt.xml
+-rw-r--r--  2.0 unx     3290 b- defN 23-Apr-17 19:50 gsfarc/esri/toolboxes/GSF.pyt
+-rw-r--r--  2.0 unx      982 b- defN 23-Apr-17 19:50 gsfarc/esri/toolboxes/GSF.pyt.xml
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 19:50 gsfarc/gptool/__init__.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-Apr-17 19:50 gsfarc/gptool/help.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/__init__.py
+-rw-r--r--  2.0 unx     8019 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/builder.py
+-rw-r--r--  2.0 unx     2206 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/template.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/__init__.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/basic.py
+-rw-r--r--  2.0 unx      589 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/basicarray.py
+-rw-r--r--  2.0 unx      105 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/bool.py
+-rw-r--r--  2.0 unx      138 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/boolarray.py
+-rw-r--r--  2.0 unx      111 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/boolean.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/byte.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/bytearray.py
+-rw-r--r--  2.0 unx      111 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/double.py
+-rw-r--r--  2.0 unx      136 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/doublearray.py
+-rw-r--r--  2.0 unx     2977 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/enviagcrops.py
+-rw-r--r--  2.0 unx     2982 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/enviraster.py
+-rw-r--r--  2.0 unx     1546 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/enviuri.py
+-rw-r--r--  2.0 unx     2978 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/envivector.py
+-rw-r--r--  2.0 unx      109 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/float.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/floatarray.py
+-rw-r--r--  2.0 unx      101 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/int.py
+-rw-r--r--  2.0 unx      133 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/intarray.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/long.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/long64.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/long64array.py
+-rw-r--r--  2.0 unx      128 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/longarray.py
+-rw-r--r--  2.0 unx      273 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/string.py
+-rw-r--r--  2.0 unx      141 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/stringarray.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/uint.py
+-rw-r--r--  2.0 unx      128 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/uintarray.py
+-rw-r--r--  2.0 unx      105 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/ulong.py
+-rw-r--r--  2.0 unx      109 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/ulong64.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/ulong64array.py
+-rw-r--r--  2.0 unx      130 b- defN 23-Apr-17 19:50 gsfarc/gptool/parameter/templates/ulongarray.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 19:50 gsfarc/test/__init__.py
+-rw-r--r--  2.0 unx     3548 b- defN 23-Apr-17 19:50 gsfarc/test/arcgisserver.py
+-rw-r--r--  2.0 unx     4577 b- defN 23-Apr-17 19:50 gsfarc/test/config.py
+-rw-r--r--  2.0 unx      936 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_bool.py
+-rw-r--r--  2.0 unx      794 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_boolarray.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_boolean.py
+-rw-r--r--  2.0 unx     1379 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_byte.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_bytearray.py
+-rw-r--r--  2.0 unx     1032 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_double.py
+-rw-r--r--  2.0 unx      907 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_doublearray.py
+-rw-r--r--  2.0 unx     2071 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_enviraster.py
+-rw-r--r--  2.0 unx     1364 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_enviuri.py
+-rw-r--r--  2.0 unx     1856 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_envivector.py
+-rw-r--r--  2.0 unx     1021 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_float.py
+-rw-r--r--  2.0 unx      919 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_floatarray.py
+-rw-r--r--  2.0 unx     1757 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_int.py
+-rw-r--r--  2.0 unx      812 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_intarray.py
+-rw-r--r--  2.0 unx      950 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_long.py
+-rw-r--r--  2.0 unx     1194 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_long64.py
+-rw-r--r--  2.0 unx      817 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_long64array.py
+-rw-r--r--  2.0 unx      797 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_longarray.py
+-rw-r--r--  2.0 unx     1597 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_string.py
+-rw-r--r--  2.0 unx      803 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_stringarray.py
+-rw-r--r--  2.0 unx      906 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_uint.py
+-rw-r--r--  2.0 unx      800 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_uintarray.py
+-rw-r--r--  2.0 unx     1208 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_ulong.py
+-rw-r--r--  2.0 unx     1193 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_ulong64.py
+-rw-r--r--  2.0 unx      837 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_ulong64array.py
+-rw-r--r--  2.0 unx      812 b- defN 23-Apr-17 19:50 gsfarc/test/test_datatype_ulongarray.py
+-rw-r--r--  2.0 unx     2960 b- defN 23-Apr-17 19:50 gsfarc/test/test_gptoolbox_server.py
+-rw-r--r--  2.0 unx     1106 b- defN 23-Apr-17 19:51 gsfarc-2.0.0.dev18.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      536 b- defN 23-Apr-17 19:51 gsfarc-2.0.0.dev18.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 19:51 gsfarc-2.0.0.dev18.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-17 19:51 gsfarc-2.0.0.dev18.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-17 19:51 gsfarc-2.0.0.dev18.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7288 b- defN 23-Apr-17 19:51 gsfarc-2.0.0.dev18.dist-info/RECORD
+78 files, 90994 bytes uncompressed, 34367 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,196 +1,235 @@
-Filename: gsfarc-1.0.4/LegalAndCopyrightNotices.txt
+Filename: gsfarc/__init__.py
 Comment: 
 
-Filename: gsfarc-1.0.4/LICENSE.txt
+Filename: gsfarc/__main__.py
 Comment: 
 
-Filename: gsfarc-1.0.4/MANIFEST.in
+Filename: gsfarc/gptoolbox.py
 Comment: 
 
-Filename: gsfarc-1.0.4/PKG-INFO
+Filename: gsfarc/system.py
 Comment: 
 
-Filename: gsfarc-1.0.4/requirements.txt
+Filename: gsfarc/esri/toolboxes/GSF.CreateTool.pyt.xml
 Comment: 
 
-Filename: gsfarc-1.0.4/setup.cfg
+Filename: gsfarc/esri/toolboxes/GSF.pyt
 Comment: 
 
-Filename: gsfarc-1.0.4/setup.py
+Filename: gsfarc/esri/toolboxes/GSF.pyt.xml
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/api.rst
+Filename: gsfarc/gptool/__init__.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/conf.py
+Filename: gsfarc/gptool/help.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/index.rst
+Filename: gsfarc/gptool/parameter/__init__.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/images/create_tool.png
+Filename: gsfarc/gptool/parameter/builder.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/images/create_tool_arcgispro.png
+Filename: gsfarc/gptool/parameter/template.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/images/spectral_index.png
+Filename: gsfarc/gptool/parameter/templates/__init__.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/images/spectral_index_arcgispro.png
+Filename: gsfarc/gptool/parameter/templates/basic.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/images/spectral_index_input.png
+Filename: gsfarc/gptool/parameter/templates/basicarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/images/spectral_index_input_arcgispro.png
+Filename: gsfarc/gptool/parameter/templates/bool.py
 Comment: 
 
-Filename: gsfarc-1.0.4/doc/source/images/spectral_index_result.png
+Filename: gsfarc/gptool/parameter/templates/boolarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptoolbox.py
+Filename: gsfarc/gptool/parameter/templates/boolean.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/system.py
+Filename: gsfarc/gptool/parameter/templates/byte.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/__init__.py
+Filename: gsfarc/gptool/parameter/templates/bytearray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.CreateTool.pyt.xml
+Filename: gsfarc/gptool/parameter/templates/double.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.pyt
+Filename: gsfarc/gptool/parameter/templates/doublearray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.pyt.xml
+Filename: gsfarc/gptool/parameter/templates/enviagcrops.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/help.py
+Filename: gsfarc/gptool/parameter/templates/enviraster.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/__init__.py
+Filename: gsfarc/gptool/parameter/templates/enviuri.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/builder.py
+Filename: gsfarc/gptool/parameter/templates/envivector.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/template.py
+Filename: gsfarc/gptool/parameter/templates/float.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/__init__.py
+Filename: gsfarc/gptool/parameter/templates/floatarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/basic.py
+Filename: gsfarc/gptool/parameter/templates/int.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/basicarray.py
+Filename: gsfarc/gptool/parameter/templates/intarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/bool.py
+Filename: gsfarc/gptool/parameter/templates/long.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/boolarray.py
+Filename: gsfarc/gptool/parameter/templates/long64.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/boolean.py
+Filename: gsfarc/gptool/parameter/templates/long64array.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/byte.py
+Filename: gsfarc/gptool/parameter/templates/longarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/bytearray.py
+Filename: gsfarc/gptool/parameter/templates/string.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/double.py
+Filename: gsfarc/gptool/parameter/templates/stringarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/doublearray.py
+Filename: gsfarc/gptool/parameter/templates/uint.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviagcrops.py
+Filename: gsfarc/gptool/parameter/templates/uintarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviraster.py
+Filename: gsfarc/gptool/parameter/templates/ulong.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviuri.py
+Filename: gsfarc/gptool/parameter/templates/ulong64.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/envivector.py
+Filename: gsfarc/gptool/parameter/templates/ulong64array.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/float.py
+Filename: gsfarc/gptool/parameter/templates/ulongarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/floatarray.py
+Filename: gsfarc/test/__init__.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/int.py
+Filename: gsfarc/test/arcgisserver.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/intarray.py
+Filename: gsfarc/test/config.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/long.py
+Filename: gsfarc/test/test_datatype_bool.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/long64.py
+Filename: gsfarc/test/test_datatype_boolarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/long64array.py
+Filename: gsfarc/test/test_datatype_boolean.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/longarray.py
+Filename: gsfarc/test/test_datatype_byte.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/string.py
+Filename: gsfarc/test/test_datatype_bytearray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/stringarray.py
+Filename: gsfarc/test/test_datatype_double.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/uint.py
+Filename: gsfarc/test/test_datatype_doublearray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/uintarray.py
+Filename: gsfarc/test/test_datatype_enviraster.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulong.py
+Filename: gsfarc/test/test_datatype_enviuri.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulong64.py
+Filename: gsfarc/test/test_datatype_envivector.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulong64array.py
+Filename: gsfarc/test/test_datatype_float.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/ulongarray.py
+Filename: gsfarc/test/test_datatype_floatarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc/gptool/parameter/templates/__init__.py
+Filename: gsfarc/test/test_datatype_int.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc.egg-info/dependency_links.txt
+Filename: gsfarc/test/test_datatype_intarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc.egg-info/not-zip-safe
+Filename: gsfarc/test/test_datatype_long.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc.egg-info/PKG-INFO
+Filename: gsfarc/test/test_datatype_long64.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc.egg-info/requires.txt
+Filename: gsfarc/test/test_datatype_long64array.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc.egg-info/SOURCES.txt
+Filename: gsfarc/test/test_datatype_longarray.py
 Comment: 
 
-Filename: gsfarc-1.0.4/gsfarc.egg-info/top_level.txt
+Filename: gsfarc/test/test_datatype_string.py
 Comment: 
 
-Filename: gsfarc-1.0.4/scripts/creategsftoolbox.py
+Filename: gsfarc/test/test_datatype_stringarray.py
+Comment: 
+
+Filename: gsfarc/test/test_datatype_uint.py
+Comment: 
+
+Filename: gsfarc/test/test_datatype_uintarray.py
+Comment: 
+
+Filename: gsfarc/test/test_datatype_ulong.py
+Comment: 
+
+Filename: gsfarc/test/test_datatype_ulong64.py
+Comment: 
+
+Filename: gsfarc/test/test_datatype_ulong64array.py
+Comment: 
+
+Filename: gsfarc/test/test_datatype_ulongarray.py
+Comment: 
+
+Filename: gsfarc/test/test_gptoolbox_server.py
+Comment: 
+
+Filename: gsfarc-2.0.0.dev18.dist-info/LICENSE.txt
+Comment: 
+
+Filename: gsfarc-2.0.0.dev18.dist-info/METADATA
+Comment: 
+
+Filename: gsfarc-2.0.0.dev18.dist-info/WHEEL
+Comment: 
+
+Filename: gsfarc-2.0.0.dev18.dist-info/entry_points.txt
+Comment: 
+
+Filename: gsfarc-2.0.0.dev18.dist-info/top_level.txt
+Comment: 
+
+Filename: gsfarc-2.0.0.dev18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gsfarc-1.0.4/LICENSE.txt` & `gsfarc-2.0.0.dev18.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptoolbox.py` & `gsfarc/gptoolbox.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/system.py` & `gsfarc/system.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.CreateTool.pyt.xml` & `gsfarc/esri/toolboxes/GSF.CreateTool.pyt.xml`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.pyt` & `gsfarc/esri/toolboxes/GSF.pyt`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 Toolbox for creating gptools from an ese task endpoint.
 """
 import os.path
 import arcpy
 from gsf import Server
 from gsfarc.gptoolbox import GPToolbox
 
-# Python 3
-try:
-    from urllib.parse import urlparse
-except ImportError:
-    from urlparse import urlparse
+from urllib.parse import urlparse
 
 
 class Toolbox(object):
     def __init__(self):
         """Define the toolbox (the name of the toolbox is the name of the
         .pyt file)."""
         self.label = "GSF"
@@ -82,20 +78,20 @@
         # Get task name, service name, etc.
         parsed_url = urlparse(parameters[0].valueAsText)
         parsed_netloc = parsed_url.netloc.split(':')
         host = parsed_netloc[0]
         port = parsed_netloc[1] if len(parsed_netloc) > 1 else '9191'
 
         split_path = parsed_url.path.split('/')
-        if len(split_path) < 5:
+        if len(split_path) < 4:
             messages.addErrorMessage('Task name not found in url.')
             raise arcpy.ExecuteError
 
         task_name = split_path[4]
-        service_name = split_path[3]
+        service_name = split_path[2]
 
         #  Messaging.
         messages.AddMessage('toolbox path: ' + toolbox_path)
         messages.AddMessage('service name: ' + service_name)
         messages.AddMessage('task name: ' + task_name)
 
         # Create toolbox.
```

## Comparing `gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.pyt.xml` & `gsfarc/esri/toolboxes/GSF.pyt.xml`

 * *Files 16% similar despite different names*

### Comparing `gsfarc-1.0.4/gsfarc/esri/toolboxes/GSF.pyt.xml` & `gsfarc/esri/toolboxes/GSF.pyt.xml`

```diff
@@ -1,24 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata xml:lang="en">
   <Esri>
     <CreaDate>20160506</CreaDate>
     <CreaTime>09242000</CreaTime>
     <ArcGISFormat>1.0</ArcGISFormat>
     <SyncOnce>TRUE</SyncOnce>
-    <ModDate>20160629</ModDate>
-    <ModTime>7580600</ModTime>
+    <ModDate>20230413</ModDate>
+    <ModTime>141243</ModTime>
     <scaleRange>
       <minScale>150000000</minScale>
       <maxScale>5000</maxScale>
     </scaleRange>
     <ArcGISProfile>ItemDescription</ArcGISProfile>
   </Esri>
   <toolbox name="GSF" alias="gsf">
-    <arcToolboxHelpPath>c:\program files (x86)\arcgis\desktop10.2\Help\gp</arcToolboxHelpPath>
+    <arcToolboxHelpPath>c:\program files\arcgis\pro\Resources\Help\gp</arcToolboxHelpPath>
+    <toolsets/>
   </toolbox>
   <dataIdInfo>
     <idCitation>
       <resTitle>GSF</resTitle>
     </idCitation>
     <idAbs>&lt;DIV STYLE=&quot;text-align:Left;&quot;&gt;&lt;DIV&gt;&lt;DIV&gt;&lt;P&gt;&lt;SPAN&gt;The Geospatial Services Framework toolbox allows you to create tools from GSF task endpoints.&lt;/SPAN&gt;&lt;/P&gt;&lt;/DIV&gt;&lt;/DIV&gt;&lt;/DIV&gt;</idAbs>
   </dataIdInfo>
```

## Comparing `gsfarc-1.0.4/gsfarc/gptool/help.py` & `gsfarc/gptool/help.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/builder.py` & `gsfarc/gptool/parameter/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             raise UnknownDataTypeError('Unable to map task datatype: ' + data_type + '.  A template must be created.')
 
         gp_param['name'] = task_param['name']
         gp_param['displayName'] = task_param['display_name']
         gp_param['direction'] = _DIRECTION_MAP[task_param['direction']]
         gp_param['paramType'] = 'Required' if task_param['required'] else 'Optional'
         # GSF output type translates to a derived output type in Arc
-        if gp_param['direction'] is 'Output':
+        if gp_param['direction'] == 'Output':
             gp_param['paramType'] = 'Derived'
 
         gp_param['multiValue'] = True if 'dimensions' in task_param else False
 
         # Substitute values into the template
         gp_params.append(parameter_map[data_type].get_parameter(task_param).substitute(gp_param))
```

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/template.py` & `gsfarc/gptool/parameter/template.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/templates/basic.py` & `gsfarc/gptool/parameter/templates/basic.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/templates/basicarray.py` & `gsfarc/gptool/parameter/templates/basicarray.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviagcrops.py` & `gsfarc/gptool/parameter/templates/enviagcrops.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviraster.py` & `gsfarc/gptool/parameter/templates/enviraster.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/templates/enviuri.py` & `gsfarc/gptool/parameter/templates/enviuri.py`

 * *Files identical despite different names*

## Comparing `gsfarc-1.0.4/gsfarc/gptool/parameter/templates/envivector.py` & `gsfarc/gptool/parameter/templates/envivector.py`

 * *Files identical despite different names*

