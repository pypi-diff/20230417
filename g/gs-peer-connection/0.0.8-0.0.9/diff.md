# Comparing `tmp/gs-peer-connection-0.0.8.tar.gz` & `tmp/gs-peer-connection-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gs-peer-connection-0.0.8.tar", last modified: Fri Apr 29 08:45:02 2022, max compression
+gzip compressed data, was "dist\gs-peer-connection-0.0.9.tar", last modified: Fri Apr 29 10:43:36 2022, max compression
```

## Comparing `gs-peer-connection-0.0.8.tar` & `gs-peer-connection-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/
--rw-rw-rw-   0        0        0      698 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gs_peer_connection.egg-info/
--rw-rw-rw-   0        0        0      698 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gs_peer_connection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gs_peer_connection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gs_peer_connection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gs_peer_connection.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gs_peer_connection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gs_peer_connection.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/gspeerconnection/
--rw-rw-rw-   0        0        0     6702 2022-04-29 08:43:42.000000 gs-peer-connection-0.0.8/gspeerconnection/gspeerconnectionbroadcaster.py
--rw-rw-rw-   0        0        0     3587 2022-03-16 10:19:42.000000 gs-peer-connection-0.0.8/gspeerconnection/gspeerconnectionwatcher.py
--rw-rw-rw-   0        0        0       42 2022-04-29 08:45:02.000000 gs-peer-connection-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1074 2022-04-29 08:45:00.000000 gs-peer-connection-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/
+-rw-rw-rw-   0        0        0      698 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gs_peer_connection.egg-info/
+-rw-rw-rw-   0        0        0      698 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gs_peer_connection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gs_peer_connection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gs_peer_connection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gs_peer_connection.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gs_peer_connection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gs_peer_connection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/gspeerconnection/
+-rw-rw-rw-   0        0        0     5171 2022-04-29 10:43:19.000000 gs-peer-connection-0.0.9/gspeerconnection/gspeerconnectionbroadcaster.py
+-rw-rw-rw-   0        0        0     3587 2022-03-16 10:19:42.000000 gs-peer-connection-0.0.9/gspeerconnection/gspeerconnectionwatcher.py
+-rw-rw-rw-   0        0        0       42 2022-04-29 10:43:36.000000 gs-peer-connection-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1074 2022-04-29 10:43:19.000000 gs-peer-connection-0.0.9/setup.py
```

### Comparing `gs-peer-connection-0.0.8/PKG-INFO` & `gs-peer-connection-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-peer-connection
-Version: 0.0.8
+Version: 0.0.9
 Summary: python peer connection adapter
 Home-page: https://glass-sphere-ai.de
 Author: Glass Sphere Software
 Author-email: 
 License: MIT
 Description: # GS Peer connection adapter
```

### Comparing `gs-peer-connection-0.0.8/gs_peer_connection.egg-info/PKG-INFO` & `gs-peer-connection-0.0.9/gs_peer_connection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-peer-connection
-Version: 0.0.8
+Version: 0.0.9
 Summary: python peer connection adapter
 Home-page: https://glass-sphere-ai.de
 Author: Glass Sphere Software
 Author-email: 
 License: MIT
 Description: # GS Peer connection adapter
```

### Comparing `gs-peer-connection-0.0.8/gspeerconnection/gspeerconnectionbroadcaster.py` & `gs-peer-connection-0.0.9/gspeerconnection/gspeerconnectionbroadcaster.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,42 +13,14 @@
 webcam = None
 camera = None
 videotrack = None
 
 
 class GSPeerConnectionBroadcaster:
 
-    def create_local_tracks(self, device, transcode=True):
-        global relay, webcam
-        if relay is None:
-            if platform.system() == "Darwin":
-                options = {
-                    "video_size": f"{str(self.gsdbs.credentials['hres'])}x{str(self.gsdbs.credentials['vres'])}",
-                    "preset": "veryfast",
-                    "framerate": str(self.gsdbs.credentials["framerate"]),
-                    "c:v": "h264_v4l2m2m",
-                    "input_format": "h264",
-                    "pixelformat": "H264"
-                }
-                webcam = MediaPlayer("default:none", format="avfoundation", options=options)
-            elif platform.system() == "Windows":
-                webcam = MediaPlayer(f"video={device}", format="dshow")
-            else:
-                options = {
-                    "video_size": f"{str(self.gsdbs.credentials['hres'])}x{str(self.gsdbs.credentials['vres'])}",
-                    "preset": "veryfast",
-                    "framerate": str(self.gsdbs.credentials["framerate"]),
-                    "c:v": "h264_v4l2m2m",
-                    "input_format": "h264",
-                    "pixelformat": "H264"
-                }
-                webcam = MediaPlayer(device, format="v4l2", options=options)
-            relay = MediaRelay()
-        return relay.subscribe(webcam.video, buffered=False)
-
     def create_local_tracks_new(self, play_from, decode):
         global relay, webcam
 
         if play_from:
             player = MediaPlayer(play_from, decode=decode)
             return player.audio, player.video
         else:
@@ -97,23 +69,17 @@
                 RTCIceServer(self.gsdbs.credentials["turnserver"],
                              self.gsdbs.credentials["turnuser"],
                              self.gsdbs.credentials["turnpw"]),
             ]))
             self.peerConnections[id] = pc
 
             audio, video = self.create_local_tracks_new(
-                None, decode=True
+                None, decode=self.gsdbs.credentials["decode"]
             )
-            channel = pc.createDataChannel("message")
-
-            # def send_data():
-            #     channel.send("test123")
-            # channel.on("open", send_data)
-
-            video_codec = "video/H264"
+            video_codec = self.gsdbs.credentials["videocodec"]
 
             if audio:
                 pc.addTrack(audio)
             if video:
                 video_sender = pc.addTrack(video)
                 if video_codec:
                     # only allow the specified video codec
```

### Comparing `gs-peer-connection-0.0.8/gspeerconnection/gspeerconnectionwatcher.py` & `gs-peer-connection-0.0.9/gspeerconnection/gspeerconnectionwatcher.py`

 * *Files identical despite different names*

### Comparing `gs-peer-connection-0.0.8/setup.py` & `gs-peer-connection-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="gs-peer-connection",
-    version="0.0.8",
+    version="0.0.9",
     description="python peer connection adapter",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://glass-sphere-ai.de",
     author="Glass Sphere Software",
     author_email="",
     license="MIT",
```

