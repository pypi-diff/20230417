# Comparing `tmp/glview-1.5.0.tar.gz` & `tmp/glview-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glview-1.5.0.tar", last modified: Fri Apr 14 14:05:09 2023, max compression
+gzip compressed data, was "glview-1.5.1.tar", last modified: Mon Apr 17 10:00:01 2023, max compression
```

## Comparing `glview-1.5.0.tar` & `glview-1.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-14 14:05:09.602748 glview-1.5.0/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.0/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.0/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-14 14:05:09.602748 glview-1.5.0/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      361 2023-03-13 15:45:56.000000 glview-1.5.0/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-14 14:05:09.598748 glview-1.5.0/glview/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.0/glview/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.0/glview/argv.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11494 2023-04-14 14:01:57.000000 glview-1.5.0/glview/glrenderer.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     9035 2023-04-14 08:09:07.000000 glview-1.5.0/glview/glview.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     6950 2023-03-13 15:45:56.000000 glview-1.5.0/glview/imageprovider.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      285 2023-03-13 15:45:56.000000 glview-1.5.0/glview/panzoom.vs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17213 2023-04-14 13:56:12.000000 glview-1.5.0/glview/pygletui.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4478 2023-04-14 11:24:45.000000 glview-1.5.0/glview/texture.fs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-03-16 09:59:41.000000 glview-1.5.0/glview/version.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-14 14:05:09.602748 glview-1.5.0/glview.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/zip-safe
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      163 2023-03-14 15:45:52.000000 glview-1.5.0/requirements.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-04-14 14:05:09.602748 glview-1.5.0/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.0/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-17 10:00:01.560995 glview-1.5.1/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.1/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.1/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-17 10:00:01.560995 glview-1.5.1/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      361 2023-03-13 15:45:56.000000 glview-1.5.1/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-17 10:00:01.560995 glview-1.5.1/glview/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.1/glview/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.1/glview/argv.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11563 2023-04-17 09:59:15.000000 glview-1.5.1/glview/glrenderer.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     8958 2023-04-17 09:53:29.000000 glview-1.5.1/glview/glview.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     6950 2023-03-13 15:45:56.000000 glview-1.5.1/glview/imageprovider.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      285 2023-03-13 15:45:56.000000 glview-1.5.1/glview/panzoom.vs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17381 2023-04-17 09:54:42.000000 glview-1.5.1/glview/pygletui.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4478 2023-04-14 11:24:45.000000 glview-1.5.1/glview/texture.fs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-04-17 09:55:11.000000 glview-1.5.1/glview/version.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-17 10:00:01.560995 glview-1.5.1/glview.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-17 10:00:01.000000 glview-1.5.1/glview.egg-info/zip-safe
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      163 2023-03-14 15:45:52.000000 glview-1.5.1/requirements.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-04-17 10:00:01.560995 glview-1.5.1/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.1/setup.py
```

### Comparing `glview-1.5.0/LICENSE` & `glview-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glview-1.5.0/PKG-INFO` & `glview-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.0
+Version: 1.5.1
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glview-1.5.0/glview/argv.py` & `glview-1.5.1/glview/argv.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.0/glview/glrenderer.py` & `glview-1.5.1/glview/glrenderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             self.prog['mousepos'].value = tuple(self.ui.mousepos)
             self.prog['orientation'].value = orientation
             self.prog['aspect'].value = self._get_aspect_ratio(vpw, vph, texw, texh)
             self.prog['scale'].value = self.ui.scale
             self.prog['grayscale'].value = (texture.components == 1)
             self.prog['gamma'].value = self.ui.gamma
             self.prog['ev'].value = self.ui.ev
-            self.prog['gamut.compress'].value = self.ui.gamut_fit
+            self.prog['gamut.compress'].value = (self.ui.gamut_fit != 0)
             self.prog['gamut.power'].value = self.ui.gamut_pow
             self.prog['gamut.thr'].value = self.ui.gamut_thr
             self.prog['gamut.scale'].value = self._gamut(imgidx)
             self.prog['debug'].value = self.ui.debug_mode
             self.vao.render(moderngl.TRIANGLE_STRIP)
         self.ctx.finish()
         elapsed = (time.time() - t0) * 1000
@@ -96,20 +96,20 @@
         self.tprev = time.time()
         self._vprint(f"rendering {w} x {h} pixels took {elapsed:.1f} ms, frame-to-frame interval was {interval:.1f} ms", log_level=2)
         return elapsed
 
     def _gamut(self, imgidx):
         """
         Calculate per-color-channel scale factors as required by the shader for gamut
-        compression. The calculation is based on a user-defined 'power' controlling the
-        curve slope, and 'thr' and 'limit' values that are currently hardcoded at 0.8
-        and 1.2, respectively. Gamut distance values are compressed from [thr, lim] to
-        [thr, 1].
+        compression. The calculation is based on three user-defined parameters (power,
+        limit, and threshold) that control the shape of the compression curve. Per-image
+        control of the 'limit' parameter is supported, but not currently used.
         """
-        gamut_lim = self.files.metadata[imgidx]['gamut_bounds']  # per-channel limits
+        if (gamut_lim := self.ui.gamut_lim) is None:  # use global limits by default
+            gamut_lim = self.files.metadata[imgidx]['gamut_bounds']  # per-image limit
         gamut_lim = np.clip(gamut_lim, 1.01, np.inf)  # >1.01 to ensure no overflows
         scale = self._gamut_curve(self.ui.gamut_pow, self.ui.gamut_thr, gamut_lim)
         return scale
 
     def _gamut_curve(self, power, thr, lim):
         """
         Calculate a curve shaping scale factor for each color channel, based on the given
```

### Comparing `glview-1.5.0/glview/glview.py` & `glview-1.5.1/glview/glview.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,15 @@
         print("    w                       write current tile(s) to a PNG")
         print("    h                       reset zoom/pan/exposure to initial state")
         print("    f                       toggle fullscreen <-> windowed")
         print("    t                       toggle nearest <-> linear filtering")
         print("    g                       toggle sRGB gamma correction on/off")
         print("    e                       slide exposure from -2EV to +2EV & back")
         print("    b                       toggle between HDR/LDR exposure control")
-        print("    k                       toggle gamut compression on/off")
-        print("    c                       adjust gamut compression strength")
+        print("    k                       toggle gamut compression strength")
         print("    i                       print image information (EXIF)")
         print("    d                       drop the currently shown image")
         print("    del                     delete the currently shown image")
         print("    space                   toggle debug rendering on/off")
         print("    q / esc / ctrl+c        terminate")
         print()
         print("  supported file types:")
```

### Comparing `glview-1.5.0/glview/imageprovider.py` & `glview-1.5.1/glview/imageprovider.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.0/glview/pygletui.py` & `glview-1.5.1/glview/pygletui.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,19 @@
         self.renderer = None
         self.texture_filter = "NEAREST"
         self.img_per_tile = [0, 1, 2, 3]
         self.gamma = False
         self.ev_range = 2
         self.ev_linear = 0.0
         self.ev = 0.0
-        self.gamut_fit = False  # on/off toggle
-        self.gamut_lin = 0.0  # adjusted dynamically
-        self.gamut_pow = np.ones(3)  # derived from self.gamut_lin
-        self.gamut_thr = np.ones(3) * 0.8  # hardcoded preset
+        self.gamut_fit = 0  # 0|1|2...
+        self.gamut_lim = np.ones(3) * 1.1
+        self.gamut_pow = np.ones(3) * 1.5
+        self.gamut_thr = np.ones(3) * 0.8
+        self.gamut_lin = 0.0
 
     def start(self, renderer):
         """ Start the UI thread. """
         self._vprint(f"spawning {self.thread_name}...")
         self.renderer = renderer
         self.running = True
         self.ui_thread = threading.Thread(target=lambda: self._try(self._pyglet_runner), name=self.thread_name)
@@ -178,30 +179,34 @@
     def _smooth_exposure(self):
         # this is invoked 50 times per second, so exposure control is pretty fast
         keys = pyglet.window.key
         self.ev_linear += 0.005 * self.key_state[keys.E]
         self.ev = self._triangle_wave(self.ev_linear, self.ev_range)
         self.need_redraw = True
 
-    def _smooth_gamut_fit(self):
-        # this is invoked 50 times per second, so gamut fit control is pretty fast
-        keys = pyglet.window.key
-        self.gamut_lin += 0.005 * self.key_state[keys.C]
-        power = self._triangle_wave(self.gamut_lin, 2) + 3  # [0, 1] => [-2, 2] => [1, 5]
-        self.gamut_pow = np.ones(3) * power
-        self.need_redraw = True
+    def _switch_gamut_curve(self):
+        # cycle through a predefined selection of gamut compression modes:
+        #  0 - off
+        #  1 - steep curve, almost like clipping
+        #  2 - shallow curve, strong desaturation
+        presets = [None, (10.0, 1.1, 0.8), (3.0, 1.2, 0.8)]
+        self.gamut_fit = (self.gamut_fit + 1) % len(presets)
+        if (selection := presets[self.gamut_fit]) is not None:
+            power, limit, threshold = selection
+            self.gamut_pow = np.ones(3) * power
+            self.gamut_lim = np.ones(3) * limit
+            self.gamut_thr = np.ones(3) * threshold
 
     def _setup_events(self):
         self._vprint("setting up Pyglet window event handlers...")
 
         @self.window.event
         def on_draw():
             self._keyboard_zoom_pan()
             self._smooth_exposure()
-            self._smooth_gamut_fit()
             if self.need_redraw:
                 self.renderer.redraw()
                 self.window.set_caption(self._caption())
                 self.window.flip()
                 if self.was_resized:
                     # ensure that both buffers (back & front) are filled
                     # with the same image after a resize event, or else
@@ -267,24 +272,24 @@
                     self.window.set_mouse_visible(not self.fullscreen)
                     self.need_redraw = True
                 if symbol == keys.H:  # reset exposure + zoom & pan ("home")
                     self.scale = 1.0
                     self.mousepos = np.zeros(2)
                     self.ev_linear = 0.0
                     self.gamut_lin = 0.0
-                    self.gamut_fit = False
+                    self.gamut_fit = 0
                     self.need_redraw = True
                 if symbol == keys.G:  # gamma
                     self.gamma = not self.gamma
                     self.need_redraw = True
                 if symbol == keys.B:  # toggle between narrow/wide (LDR/HDR) exposure control
                     self.ev_range = (self.ev_range + 6) % 12
                     self.need_redraw = True
-                if symbol == keys.K: # toggle gamut compression on/off
-                    self.gamut_fit = not self.gamut_fit
+                if symbol == keys.K: # cycle through gamut compression modes (off/hi/lo)
+                    self._switch_gamut_curve()
                     self.need_redraw = True
                 if symbol == keys.T:  # texture filtering
                     self.texture_filter = "LINEAR" if self.texture_filter == "NEAREST" else "NEAREST"
                     self.need_redraw = True
                 if symbol == keys.S:  # split
                     self.numtiles = (self.numtiles % 4) + 1
                     self.tileidx = min(self.tileidx, self.numtiles - 1)
```

### Comparing `glview-1.5.0/glview/texture.fs` & `glview-1.5.1/glview/texture.fs`

 * *Files identical despite different names*

### Comparing `glview-1.5.0/glview.egg-info/PKG-INFO` & `glview-1.5.1/glview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.0
+Version: 1.5.1
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glview-1.5.0/setup.py` & `glview-1.5.1/setup.py`

 * *Files identical despite different names*

