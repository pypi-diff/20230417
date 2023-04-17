# Comparing `tmp/flashcam-1.3.22.tar.gz` & `tmp/flashcam-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.3.22.tar", last modified: Mon Apr 17 11:15:50 2023, max compression
+gzip compressed data, was "flashcam-1.3.4.tar", last modified: Wed Mar  1 18:44:42 2023, max compression
```

## Comparing `flashcam-1.3.22.tar` & `flashcam-1.3.4.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-17 11:15:50.326171 flashcam-1.3.22/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      851 2023-04-17 11:15:50.326171 flashcam-1.3.22/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 11:15:47.000000 flashcam-1.3.22/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-17 11:15:50.318172 flashcam-1.3.22/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    26132 2023-04-17 11:13:59.000000 flashcam-1.3.22/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.3.22/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.3.22/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 11:13:16.000000 flashcam-1.3.22/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-17 11:15:50.322172 flashcam-1.3.22/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.3.22/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.3.22/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-02-01 13:41:33.000000 flashcam-1.3.22/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-17 11:15:50.326171 flashcam-1.3.22/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/c120.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/c270_orig.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/cameras.org
--rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/cameras.pdf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/cameras.tex
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-02-14 15:48:37.000000 flashcam-1.3.22/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/f100.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/f100_orig.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/data/vf0770.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-02-14 15:48:37.000000 flashcam-1.3.22/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.3.22/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.3.22/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-03-06 14:36:24.000000 flashcam-1.3.22/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    45483 2023-04-17 11:13:16.000000 flashcam-1.3.22/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35226 2023-04-17 11:13:16.000000 flashcam-1.3.22/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   100516 2023-03-06 14:36:24.000000 flashcam-1.3.22/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 11:13:16.000000 flashcam-1.3.22/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27417 2022-11-16 13:28:21.000000 flashcam-1.3.22/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       21 2023-04-17 11:15:49.000000 flashcam-1.3.22/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29933 2023-04-17 11:13:16.000000 flashcam-1.3.22/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-17 11:15:50.322172 flashcam-1.3.22/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      851 2023-04-17 11:15:50.000000 flashcam-1.3.22/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      913 2023-04-17 11:15:50.000000 flashcam-1.3.22/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-17 11:15:50.000000 flashcam-1.3.22/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-04-17 11:15:50.000000 flashcam-1.3.22/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-04-17 11:15:50.000000 flashcam-1.3.22/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-17 11:15:50.326171 flashcam-1.3.22/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1796 2023-03-06 14:36:24.000000 flashcam-1.3.22/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.243785 flashcam-1.3.4/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    10122 2023-03-01 18:44:42.243785 flashcam-1.3.4/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     7670 2023-03-01 18:44:38.000000 flashcam-1.3.4/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.239785 flashcam-1.3.4/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    26096 2023-02-15 18:20:42.000000 flashcam-1.3.4/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.3.4/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.3.4/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      447 2022-06-10 13:50:42.000000 flashcam-1.3.4/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.239785 flashcam-1.3.4/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.3.4/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.3.4/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-02-01 13:41:33.000000 flashcam-1.3.4/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.243785 flashcam-1.3.4/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/c120.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/c270_orig.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/cameras.org
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/cameras.pdf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/cameras.tex
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/f100.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/f100_orig.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/data/vf0770.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.3.4/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.3.4/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4176 2023-03-01 15:27:12.000000 flashcam-1.3.4/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    45014 2023-03-01 15:27:12.000000 flashcam-1.3.4/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35197 2023-02-14 15:48:37.000000 flashcam-1.3.4/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    97755 2023-03-01 18:42:49.000000 flashcam-1.3.4/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11293 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27417 2022-11-16 13:28:21.000000 flashcam-1.3.4/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-03-01 18:44:41.000000 flashcam-1.3.4/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29797 2023-02-15 17:29:21.000000 flashcam-1.3.4/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-03-01 18:44:42.239785 flashcam-1.3.4/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    10122 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      854 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-03-01 18:44:42.000000 flashcam-1.3.4/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-03-01 18:44:42.243785 flashcam-1.3.4/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1687 2023-03-01 15:27:12.000000 flashcam-1.3.4/setup.py
```

### Comparing `flashcam-1.3.22/bin/flashcam` & `flashcam-1.3.4/bin/flashcam`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 
 import flashcam.config as config
 
 try:
     import flashcam.uniwrec as uniwrec
 except:
     print("X... cannot import uniwrec ... ?problem with pynput and Xserver")
-    print(" ... i go on... anyway")
 
 import os #  for exit
 
 import numpy as np
 
 import datetime as dt
```

### Comparing `flashcam-1.3.22/flashcam/base_camera2.py` & `flashcam-1.3.4/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/config.py` & `flashcam-1.3.4/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.3.4/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.3.4/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/DET_NRDY.jpg` & `flashcam-1.3.4/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/DET_RDY_.jpg` & `flashcam-1.3.4/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/c120.jpg` & `flashcam-1.3.4/flashcam/data/c120.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/c270_orig.png` & `flashcam-1.3.4/flashcam/data/c270_orig.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/cameras.org` & `flashcam-1.3.4/flashcam/data/cameras.org`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/cameras.pdf` & `flashcam-1.3.4/flashcam/data/cameras.pdf`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/cameras.tex` & `flashcam-1.3.4/flashcam/data/cameras.tex`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/f100.jpg` & `flashcam-1.3.4/flashcam/data/f100.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/f100_orig.jpg` & `flashcam-1.3.4/flashcam/data/f100_orig.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/monoskop.jpg` & `flashcam-1.3.4/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/data/vf0770.jpg` & `flashcam-1.3.4/flashcam/data/vf0770.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/direct.py` & `flashcam-1.3.4/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/izmq_receiver.py` & `flashcam-1.3.4/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/mmapwr.py` & `flashcam-1.3.4/flashcam/mmapwr.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 
 def mmread_n_clear(  filename = MMAPFILE ):
     """
     read and clear  filename
     """
-    # print("D... MMRC")
+    print("D... MMRC")
     if os.path.exists(filename):
         file_size = os.path.getsize( MMAPFILE )
         if int(file_size) != int(MMAPSIZE):
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
```

### Comparing `flashcam-1.3.22/flashcam/real_camera.py` & `flashcam-1.3.4/flashcam/real_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
 # -----------------------------------------------------------------
 
 class Camera(BaseCamera):
 
     video_source = 0
     histomean = 50
-    #nfrm = 0 # number frame.... nonono
     capdevice = None # global
 
     @staticmethod
     def init_cam(  ):
         """
         should return videocapture device
         but also sould set Camerare.video_source
@@ -135,18 +134,18 @@
             ret = False
         else:
             print(f"i... frame {BaseCamera.nframes:8d}   ", end="\r" )
             try: #----this catches errors of libjpeg with cv2.CAP_V4L2
                 ret, frame = cap.read()
                 BaseCamera.nframes+=1
                 #wname = f"res {frame.shape[1]}x{frame.shape[0]}"
-                # nfrm+=1
+                nfrm+=1
                 #print(f"D... got frame (frames iter)   ret={ret}  {frame.shape}")
             except Exception as ex:
-                print("D... SOME OTHER EXCEPTION ON RECV (realc)...", ex)
+                print("D... SOME OTHER EXCEPTION ON RECV...", ex)
                 config.CONFIG["camera_on"] = False
        # --- camera probably works ret True
         if not ret:
             time.sleep(0.5)
             config.CONFIG["camera_on"] = False
             print("i... ??? cap didnt go ok, graying... trying to acquire new cap")
             cap = Camera.init_cam( ) # WHAT IS THIS? the same?<= static?
@@ -194,15 +193,15 @@
                 scale_percent = 50
                 width = int(image.shape[1] * scale_percent / 100)
                 height = int(image.shape[0] * scale_percent / 100)
                 # dsize
                 dsize = (width, height)
                 # resize image
                 frame = cv2.resize(image, dsize)
-                time.sleep(0.3) # from 85%cpu to 20% ??????
+                time.sleep(0.1) # from 85%cpu to 20% ??????
                 return "image", frame, cap # repeat cap==image
 
             elif cap.find("clock.jpg")==0:
                 height, width = 480, 640
                 blank_image = np.zeros((height,width,3), np.uint8)
                 blank_image[:,0:width//2] = (20,20,20)      # (B, G, R)
                 blank_image[:,width//2:width] = (25,25,25)
@@ -216,15 +215,15 @@
                 draw = ImageDraw.Draw(img_pil)
                 drtext = dt.datetime.now().strftime("%H:%M:%S.%f")[:-5]
 
                 #draw.text( position,  "国庆节/中秋节 快乐!", font = font, fill = (b, g, r, a))
                 b,g,r,a = 0,255,0,200
                 draw.text( position,  drtext, font = font, fill = (b, g, r, a))
                 frame = np.array(img_pil)
-                time.sleep(0.3) # from 85%cpu to 20% with 0.1;
+                time.sleep(0.1) # from 85%cpu to 20%
                 # cv2.putText(
                 #     blank_image, #numpy array on which text is written
                 #     drtext, #text
                 #     position, #position at which writing has to start
                 #     #cv2.FONT_HERSHEY_SIMPLEX, #font family
                 #     font,
                 #     4, #font size
@@ -237,15 +236,15 @@
                 #print("i... static image mode")
                 capfull = os.path.expanduser( f"~/.config/flashcam/{cap}" )
                 if  os.path.exists(capfull):
                     fullpath_fixed_image =  capfull
                 else:
                     print("X... image doesnt exist", cap, "using monoskop")
 
-                time.sleep(0.3) # from 85%cpu to 20% with 0.1
+                time.sleep(0.1) # from 85%cpu to 20%
                 return "image", cv2.imread( fullpath_fixed_image), cap # repeat cap==image
         else:
             #print("i...  camera mode")
             if cap is None and vidnum is None:
                 print("X... camera not accessible")
                 time.sleep(0.2)
                 return "image",  cv2.imread( fullpath_fixed_image), cap # repeat cap==image
@@ -674,15 +673,15 @@
                     # ------------- COMMANDS COMMING FROM WEB.PY----------------
                     #  expressions
                     # ------------- commands comming from web.py----------------
                     #           -------------- or from seread (fixed_image ...)
                     expression,value = mmread_n_clear( )
 
                     if expression[:5] != "xxxxx":
-                        #print(f"i...  *  EXPR: {expression} == {value}")
+                        print(f"i...  *  EXPR: {expression} == {value}")
                         print(f"i...  *  EXPR: {expression} == {value}")
                         print(f"i...  *  EXPR: {expression} == {value}")
 
                         # -------------------- conversions without eval inf float bool, string
                         if is_int(value):
                             print("i... ",value, 'can be safely converted to an integer.')
                             value = int(float(value)) # 1.0 => int crashes
@@ -704,20 +703,14 @@
                             # eval makes float float and int int
                             #print("o... evaluating")
                             globals()[expression] = value  #was  eval(value)
                             print("i... evaluated")
                         except:
                             print("X... globals expression FAIL",expression,value)
 
-                        # I need a crosscheck here on screen
-                        if expression=="pausedMOTION":
-                            if value is True:
-                                print("===================== DM RUNNING ====================")
-                            if value is False:
-                                print("--------------------- DM on standby -----------------")
 
                     # THIs - I think - Is for send telegram via web interface
                     # it is rather DEBUG tool than a real use
                     # NOT TESTED
                     #senh.telegram_send_image()
 
                     # telegramnow = dt.datetime.now()
```

### Comparing `flashcam-1.3.22/flashcam/stream_enhancer.py` & `flashcam-1.3.4/flashcam/stream_enhancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,15 +827,15 @@
                 print(f"fCAMERA {self.zmqrpi_name} ")
                 print(f"fCAMERA {self.zmqrpi_name} {telegramnow.strftime('%a %H:%M:%S')}")
                 y = threading.Thread(target=telegram.bot_send, args=("ALERT", f"CAMERA {self.zmqrpi_name} {telegramnow.strftime('%a %H:%M:%S')}", self.frame))
                 y.start()
                 print("i.. telegram SENT============")
                 self.telegramlast=telegramnow
             else:
-                print("i.. telegram not allowed due time", (telegramnow-self.telegramlast).total_seconds()," block time=",TELEGRAMBLOCK)
+                print("i.. telegram not allowed due time", (telegramnow-self.telegramlast).total_seconds())
         #else:
         #    print(f"X...  jtele=={self.jtelegram}, token")
         return
 
 
 
 # --------------------------------------------------------save avi ------------
```

### Comparing `flashcam-1.3.22/flashcam/uniwrec.py` & `flashcam-1.3.4/flashcam/uniwrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,14 @@
        * with remote flashcam server """
 
 
 
 
 
 def rotate_image(image, angle):
-    if angle is None:     return image
-    if abs(angle)<0.1:     return image
     image_center = tuple(np.array(image.shape[1::-1]) / 2)
     # print( "rotate", image_center, angle )
     rot_mat = cv2.getRotationMatrix2D(image_center, angle, 1.0)
     #print(rot_mat)
     result = cv2.warpAffine(image, rot_mat, image.shape[1::-1], flags=cv2.INTER_LINEAR)
     #print("rotated by ", angle)
     return result
@@ -1243,38 +1241,28 @@
                             else:
                                 row.append(wide)
                         # -----
                         # -----
                         row.append(order)
                         row = sorted(row)
                         row = row[::-1]  # revert - we want Big to small
-                        # print( "TICKS... max:", row[0]  )
-
-                        base = 10**math.floor( math.log10( row[0]) )
-                        if row[0]/base<4:
-                            base = 10**math.floor( math.log10( row[0]/4) )
-
-                        minors = np.arange( base, row[0], base)
-                        minors = minors[::-1]
-                        #print(minors)
-                        if len(row) <= 2:
+                        if len(row) <= 4:
                             in0 = row[0] / 2
-                            row.append(in0)
                             in1 =  row[0] / 4
+                            in2 = row[0] / 4 *3
+                            in3 = row[0] / 5
+                            #in2 = row[-1]/10
+                            row.append(in0)
                             row.append(in1)
-                        #     in2 = row[0] / 4 *3
-                        #     in3 = row[0] / 5
-                        #     #in2 = row[-1]/10
-                        #     row.append(in2)
-                        #     # row.append( in2 )
+                            row.append(in2)
+                            # row.append( in2 )
                             # print("   > ",row)
-                        return row,minors  # Big to small
-
+                        return row  # Big to small
 
-                    def one_mark(dist=1.7, wide=[1, 2], speed=0, dispnumb = True):
+                    def one_mark(dist=1.7, wide=[1, 2], speed=0):
                         #  wide ...  # Big to small
                         # h,w = frame.shape[0], frame.shape[1]
                         # pixel distance of halfwidth
 
                         # alpha = pixwid * radians_per_pixel2
                         # dist = wide/math.tan( alpha)
                         # I need to calculate 1m
@@ -1301,79 +1289,58 @@
 
                             mY = mY + level * step
 
                             yA, yB = mY, mY
 
                             xA = mX
                             xB = mX + int(pixwid)
-
-                            yC = mY - int(pixwid) # up
-
                             color = (0, 255, 0)  # BGR
                             color = (55, 0, 255)  # BGR same as the red cross
                             colos = (255, 0, 55)  # BGR same as the red cross
                             if level == 0:
-                                # line - horiznotal
+                                # line
                                 cv2.line(
                                     frame,
                                     (int(xA), int(yA)),
                                     (int(xB), int(yB)),
                                     color,
                                     1,
                                 )
-                                cv2.line( # left
+                                cv2.line(
                                     frame,
                                     (int(xA), int(yA)),
                                     (int(2*xA-xB), int(yB)),
-                                    color,
+                                    colos,
                                     1,
                                 )
 
-
-                                cv2.line( # probably central  mark
+                                cv2.line( # probably 1st mark
                                     frame,
                                     (int(xA), int(yA + 8)),
                                     (int(xA), int(yA - 8)),
                                     color,
                                     1,
                                 )
 
-                            # vert bars on horiz axis
-                            cv2.line(  # ticks right
+                            # vert bars -
+                            cv2.line(
                                 frame,
-                                (int(xB), int(yB + 3)),
-                                (int(xB), int(yB - 3)),
+                                (int(xB), int(yB + 2)),
+                                (int(xB), int(yB - 2)),
                                 color,
                                 1,
                             )
-                            cv2.line( # ticks left
+                            cv2.line(
                                 frame,
-                                (int(2*xA-xB), int(yB + 3)),
-                                (int(2*xA-xB), int(yB - 3)),
-                                color,
+                                (int(2*xA-xB), int(yB + 2)),
+                                (int(2*xA-xB), int(yB - 2)),
+                                colos,
                                 1,
                             )
 
-                            if yC>0:
-                                # horz bars on vertic axis
-                                cv2.line( # up
-                                    frame,
-                                    (int(xA), int(yA)),
-                                    (int(xA), int(yC)),
-                                    color,
-                                    1,
-                                )
-                                cv2.line(
-                                    frame,
-                                    (int(xA-3), int(yC )),
-                                    (int(xA+3), int(yC )),
-                                    color,
-                                    1,
-                                )
-
                             unit = "m"
                             # --- check the biggest to set the unit [0] is biggest
                             if wide[0] <= 0.001:
                                 iwide = round(iwide * 1000 * 1000) / 1000
                                 unit = "mm"
                             elif wide[0] <= 0.01:
                                 iwide = round(iwide * 100 * 1000) / 1000
@@ -1403,60 +1370,34 @@
                             if level > 0:
                                 unit = ""  # no unit during the scale
                             unit2 = "m"
 
                             if str(iwide)[:2] == "0.":
                                 iwide = str(iwide)[1:]
 
-                            if dispnumb:
-                                # width on scale - scale values
-                                cv2.putText(
-                                    frame,
-                                    f"{iwide}",
-                                    (int(xB - 10), int(mY - 7)),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-                                cv2.putText(
-                                    frame,
-                                    f"{iwide}",
-                                    (int(2*xA-xB - 10), int(mY - 7)),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-
-                                cv2.putText(  # up
-                                    frame,
-                                    f"{iwide}{unit}",
-                                    (int(xA + 10), int(yC)),  # little rightx a bit up y
-                                    cv2.FONT_HERSHEY_SIMPLEX,
-                                    0.35,
-                                    color,
-                                    1,
-                                )
-
-
+                            # width on scale - scale values
+                            cv2.putText(
+                                frame,
+                                f"{iwide}{unit}",
+                                (int(xB - 10), int(mY - 7)),  # little rightx a bit up y
+                                cv2.FONT_HERSHEY_SIMPLEX,
+                                0.35,
+                                color,
+                                1,
+                            )
+                            cv2.putText(
+                                frame,
+                                f"{iwide}{unit}",
+                                (int(2*xA-xB - 10), int(mY - 7)),  # little rightx a bit up y
+                                cv2.FONT_HERSHEY_SIMPLEX,
+                                0.35,
+                                colos,
+                                1,
+                            )
 
-                                if level==0 and unit!="":
-                                    cv2.putText(
-                                        frame,
-                                        f"  unit ... {unit}",
-                                        (
-                                            int(xA - 130),
-                                            int(mY - 5 -40),
-                                        ),  # little rightx a bit up y
-                                        cv2.FONT_HERSHEY_SIMPLEX,
-                                        0.35,
-                                        color,
-                                        1,
-                                    )
 
 
                             if level >= 0:
                                 # distance - only at first mark
                                 cv2.putText(
                                     frame,
                                     f"  at {dist} {unit2}",
@@ -1494,18 +1435,15 @@
                                         0.35,
                                         color,
                                         1,
                                     )
                             level += 1
 
                     # main part of the ruler making---------------
-
-                    order,minorticks = get_order(dist=measure)
-                    # print(minorticks)
-
+                    order = get_order(dist=measure)
                     # speed computation
                     if not (tracker1 is None) and len(tracker_list) > 2:
                         b = tracker_list[-1]
                         try:
                             v_from = -2
                             a = tracker_list[v_from]
                             while True:
@@ -1522,15 +1460,14 @@
                         c = ((b[0] - a[0]) ** 2 + (b[1] - a[1]) ** 2) ** 0.5
                         v = c / dt * radians_per_pixel2
                         v = round(100 * math.tan(v) * measure) / 100
                         # print(f"i... speed = {v} m/s  {dt:.2}==dt " )
                     else:
                         v = 0
                     # plot ruler
-                    one_mark(dist=measure, wide=minorticks, speed=v, dispnumb = False)
                     one_mark(dist=measure, wide=order, speed=v)
 
                     # ----------- THERE IS A MISTAKE countdown_s not known here
                 #                 if "countdown" in locals() and len(countdown) > 0:
                 #                     now = datetime.datetime.now()
                 #                     delta = now - datetime.datetime(1970, 1, 1)
                 #                     if delta < countdown_s:
@@ -1823,15 +1760,15 @@
                     (measure > 0)
                     and (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("N"))
                 ):
                     print("N PRESSED! - measure distance - far")
                     measure_prev_tmp = measure
-                    measure = round(10 * measure / 1.2) / 10
+                    measure = round(10 * measure / 1.15) / 10
                     if measure_prev_tmp == measure:
                         measure = measure/2
                     if measure < 0.1:
                         measure = 0.1
 
                 if (
                     (measure > 0)
```

### Comparing `flashcam-1.3.22/flashcam/usbcheck.py` & `flashcam-1.3.4/flashcam/usbcheck.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                 #wname = f"res {frame.shape[1]}x{frame.shape[0]}"
                 nfrm+=1
                 print("D... got frame",nfrm, "ret=", ret)
     #        except TimeoutError:
     #            timeoutok = True
     #            nfrm = 0
             except Exception as ex:
-                print("D... SOME OTHER EXCEPTION ON RECV (usbchk)...", ex)
+                print("D... SOME OTHER EXCEPTION ON RECV...", ex)
 
 #        if  timeoutok:
 #            print("X... timout")
 
         if not ret:
             time.sleep(0.5)
             print("D... trying to recommend")
```

### Comparing `flashcam-1.3.22/flashcam/v4lc.py` & `flashcam-1.3.4/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.3.22/flashcam/web.py` & `flashcam-1.3.4/flashcam/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,23 +503,23 @@
             if request.form.get('left2') == 'LEFT2':
                 print("<-")
                 if (pantilthat.get_pan()+8)<=90:
                     pantilthat.pan( pantilthat.get_pan()+8 )
 
         if  request.form.get('external_signal') is not None:
             excommand = str( request.form.get('external_signal') )
-            #print(f"**** external signal == {excommand} *****")
-            #print(f"**** external signal == {excommand} *****")
-            #print(f"**** external signal == {excommand} *****")
+            print(f"**** external signal == {excommand} *****")
+            print(f"**** external signal == {excommand} *****")
+            print(f"**** external signal == {excommand} *****")
             print(f"**** external signal == {excommand} *****")
             if excommand == "pausedmON":
-                print("i... unpause   - Detect Motion         unpause   - Detect Motion ")
+                print("i... unpause   - Detect Motion")
                 mmwrite(f"pausedMOTION False" )
             if excommand == "pausedmOF":
-                print("i... pause - NO Detect Motion              pause - NO Detect Motion")
+                print("i... pause - NO Detect Motion NOW")
                 mmwrite(f"pausedMOTION True" )
 
 
         if  request.form.get('crosson') == 'CROSSON':
             print("green cross ON")
             cross_on = True
         elif  request.form.get('crossoff') == 'CROSSOFF':
@@ -571,16 +571,14 @@
     return render_template_string(index_page, url=url, url_bg  = url_bg, url_fg  = url_fg)
 
 
 
 
 @auth.verify_password
 def verify_password(username, password):
-    global remote_ip
-    remote_ip=request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
 #    user = User.query.filter_by(username = username).first()
 #    if not user or not user.verify_password(password):
 #        return False
 #    g.user = user
     # config.load_config() # IMPLIES THAT ALL changes in 'bin flask500' are lost
     # config.show_config()
     u = config.CONFIG["user"]
@@ -591,19 +589,20 @@
     #     with open( os.path.expanduser("~/.pycamfw_pass") ) as f:
     #         print("YES---> FILE  ","~/.pycamfw_pass")
     #         p=f.readlines()[0].strip()
     # except:
     #     print("NO FILE  ","~/.pycamfw_pass")
 
     if (username==u) and (password==p):
-        # logthis( "   TRUE  checking userpass (client)"+username+"/"+password+"/")
-        logthis( f" TRUE  PASS {request.remote_addr:15s} {remote_ip:15s}: /{u}/{p}/")
+        logthis( "   TRUE  checking userpass (client)"+username+"/"+password+"/")
+        logthis( "   TRUE  checking userpass (real  )"+u+"/"+p+"/")
         return True
     else:
-        logthis( f" FALSE PASS {request.remote_addr:15s} {remote_ip:15s}: /{username}/{password}/")
+        logthis( "   FALSE checking userpass (client)"+username+"/"+password+"/")
+        logthis( "   FALSE checking userpass (real  )"+u+"/"+p+"/")
         return False
 
 
 
 
 @app.route('/')
 @auth.login_required
```

### Comparing `flashcam-1.3.22/flashcam.egg-info/SOURCES.txt` & `flashcam-1.3.4/flashcam.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,13 +27,11 @@
 flashcam/data/DET_NRDY.jpg
 flashcam/data/DET_RDY_.jpg
 flashcam/data/c120.jpg
 flashcam/data/c270_orig.png
 flashcam/data/cameras.org
 flashcam/data/cameras.pdf
 flashcam/data/cameras.tex
-flashcam/data/digital-7.mono.ttf
 flashcam/data/f100.jpg
 flashcam/data/f100_orig.jpg
 flashcam/data/monoskop.jpg
-flashcam/data/vf0770.jpg
-flashcam/data/windows.jpg
+flashcam/data/vf0770.jpg
```

### Comparing `flashcam-1.3.22/setup.py` & `flashcam-1.3.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,14 @@
     license="GPL2",
     version=get_version("flashcam/version.py"),
     packages=['flashcam'],
     package_data={'flashcam': ['data/BEAM_OFF.jpg',
                                'data/BEAM_ON_.jpg',
                                'data/DET_NRDY.jpg',
                                'data/DET_RDY_.jpg',
-                               'data/windows.jpg',
-                               'data/digital-7.mono.ttf',
                                'data/monoskop.jpg'
     ]},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/flashcam','bin/flashcamg','bin/flashcam_join','bin/flashcam_rep'],
     install_requires = ['fire','v4l2py','flask_httpauth','gunicorn','numpy','imutils','pandas','matplotlib','psutil','pyserial-asyncio', 'imagezmq','notifator','pyautogui','importlib_resources','requests','pynput'],
 )
```

