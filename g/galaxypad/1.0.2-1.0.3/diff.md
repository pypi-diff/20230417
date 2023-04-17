# Comparing `tmp/galaxypad-1.0.2-py3-none-any.whl.zip` & `tmp/galaxypad-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7753 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-10 23:34 galaxypad/__init__.py
+Zip file size: 7815 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-17 15:54 galaxypad/__init__.py
 -rw-rw-rw-  2.0 fat     1517 b- defN 23-Apr-10 17:18 galaxypad/__main__.py
--rw-rw-rw-  2.0 fat    13205 b- defN 23-Apr-10 23:33 galaxypad/pad.py
--rw-rw-rw-  2.0 fat     4575 b- defN 23-Apr-10 23:36 galaxypad-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 23:36 galaxypad-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-10 23:36 galaxypad-1.0.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-10 23:36 galaxypad-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      631 b- defN 23-Apr-10 23:36 galaxypad-1.0.2.dist-info/RECORD
-8 files, 20151 bytes uncompressed, 6651 bytes compressed:  67.0%
+-rw-rw-rw-  2.0 fat    13660 b- defN 23-Apr-17 15:55 galaxypad/pad.py
+-rw-rw-rw-  2.0 fat     4575 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      631 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/RECORD
+8 files, 20606 bytes uncompressed, 6713 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: galaxypad/__main__.py
 Comment: 
 
 Filename: galaxypad/pad.py
 Comment: 
 
-Filename: galaxypad-1.0.2.dist-info/METADATA
+Filename: galaxypad-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: galaxypad-1.0.2.dist-info/WHEEL
+Filename: galaxypad-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: galaxypad-1.0.2.dist-info/entry_points.txt
+Filename: galaxypad-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: galaxypad-1.0.2.dist-info/top_level.txt
+Filename: galaxypad-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: galaxypad-1.0.2.dist-info/RECORD
+Filename: galaxypad-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## galaxypad/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "Aurum"
 
 from .pad import *
```

## galaxypad/pad.py

```diff
@@ -49,42 +49,54 @@
     Reads and returns the game's ID name from Dolphin's emulated game memory.
 
     :return: the game's ID name.
     """
     return dolphin_memory_engine.read_bytes(0, 4).decode("ascii")
 
 
+@validate_ptr("s32*")
+def dolphin_read_s32(ptr: int) -> int:
+    """
+    Reads a signed 32-bit integer at the specified address in Dolphin's emulated game memory and returns it.
+
+    :param ptr: the pointer to the signed 32-bit integer.
+    :return: the value read.
+    """
+    return dolphin_memory_engine.read_word(ptr)
+
+
 @validate_ptr("u32*")
 def dolphin_read_u32(ptr: int) -> int:
     """
     Reads an unsigned 32-bit integer at the specified address in Dolphin's emulated game memory and returns it.
 
     :param ptr: the pointer to the unsigned 32-bit integer.
     :return: the value read.
     """
     return dolphin_memory_engine.read_word(ptr) & 0xFFFFFFFF
 
 
 @validate_ptr("char*")
-def dolphin_read_cstring(ptr: int) -> str:
+def dolphin_read_cstring(ptr: int, encoding: str = "ascii") -> str:
     """
     Reads a C-string at the specified address in Dolphin's emulated game memory and returns it.
 
     :param ptr: the pointer to the C-string.
+    :param encoding: the string's encoding.
     :return: the value read.
     """
     chars = bytearray()
     while True:
         char = dolphin_memory_engine.read_byte(ptr)
         ptr += 1
         if char == 0:
             break
         else:
             chars.append(char)
-    return chars.decode("ascii")
+    return chars.decode(encoding)
 
 
 @validate_ptr("PadRecorderInfo*")
 def dolphin_read_update_frame(pad_recorder_info_ptr: int) -> int:
     """
     Reads the update frame number associated with the PadRecordInfo in Dolphin's emulated game memory and returns it.
 
@@ -98,15 +110,15 @@
 def dolphin_read_recorder_mode(pad_recorder_info_ptr: int) -> int:
     """
     Reads the recorder mode associated with the PadRecordInfo in Dolphin's emulated game memory and returns it.
 
     :param pad_recorder_info_ptr: the pointer to PadRecordInfo.
     :return: the value read.
     """
-    return dolphin_read_u32(pad_recorder_info_ptr + OFFSET_RECORDER_MODE)
+    return dolphin_read_s32(pad_recorder_info_ptr + OFFSET_RECORDER_MODE)
 
 
 @validate_ptr("PadRecorderInfo*")
 def dolphin_read_stage_name(pad_recorder_info_ptr: int) -> str | None:
     """
     Reads the stage's name associated with the PadRecordInfo in Dolphin's emulated game memory and returns it.
 
@@ -121,15 +133,15 @@
 def dolphin_read_restart_id(pad_recorder_info_ptr: int) -> int:
     """
     Reads the spawn ID associated with the PadRecordInfo in Dolphin's emulated game memory and returns it.
 
     :param pad_recorder_info_ptr: the pointer to PadRecordInfo.
     :return: the value read.
     """
-    return dolphin_read_u32(pad_recorder_info_ptr + OFFSET_RESTART_ID)
+    return dolphin_read_s32(pad_recorder_info_ptr + OFFSET_RESTART_ID)
 
 
 @validate_ptr("PadRecorderInfo*")
 def dolphin_read_kpad_statuses(pad_recorder_info_ptr: int) -> list[bytes]:
     """
     Reads the KPADStatus structs associated with the PadRecordInfo in Dolphin's emulated game memory and returns them.
 
@@ -338,14 +350,15 @@
             # Get current update frame
             current_frame = dolphin_read_update_frame(pad_recorder_info_ptr)
 
             if current_frame == ((next_frame - 1) & 0xFFFFFFFF):
                 continue
             elif current_frame != next_frame:
                 print("Aborted recording due to a synchronization error!")
+                dolphin_memory_engine.un_hook()
                 return
 
             next_frame = (current_frame + 1) & 0xFFFFFFFF
 
             # Still recording?
             recorder_state = dolphin_read_recorder_mode(pad_recorder_info_ptr)
```

## Comparing `galaxypad-1.0.2.dist-info/METADATA` & `galaxypad-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxypad
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python tool to record PAD playback for Super Mario Galaxy 2
 Home-page: https://github.com/SunakazeKun/galaxypad
 Author: Aurum
 License: gpl-3.0
 Keywords: nintendo,super-mario-galaxy-2,pad,dolphin,modding
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

