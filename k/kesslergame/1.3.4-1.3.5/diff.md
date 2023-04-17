# Comparing `tmp/kesslergame-1.3.4.tar.gz` & `tmp/kesslergame-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kesslergame-1.3.4.tar", last modified: Sun Apr 16 23:10:26 2023, max compression
+gzip compressed data, was "kesslergame-1.3.5.tar", last modified: Mon Apr 17 20:05:26 2023, max compression
```

## Comparing `kesslergame-1.3.4.tar` & `kesslergame-1.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 23:10:26.041961 kesslergame-1.3.4/
--rw-rw-rw-   0        0        0    11565 2023-04-16 23:09:55.000000 kesslergame-1.3.4/LICENSE
--rw-rw-rw-   0        0        0       73 2023-04-16 23:09:55.000000 kesslergame-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3330 2023-04-16 23:10:26.041961 kesslergame-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2676 2023-04-16 23:09:55.000000 kesslergame-1.3.4/README.md
--rw-rw-rw-   0        0        0      423 2023-04-16 23:09:55.000000 kesslergame-1.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       23 2023-04-16 23:09:55.000000 kesslergame-1.3.4/requirements.txt
--rw-rw-rw-   0        0        0      882 2023-04-16 23:10:26.041961 kesslergame-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-04-16 23:09:55.000000 kesslergame-1.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 23:10:26.026392 kesslergame-1.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 23:10:26.041961 kesslergame-1.3.4/src/kesslergame/
--rw-rw-rw-   0        0        0      681 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/asteroid.py
--rw-rw-rw-   0        0        0     1524 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/bullet.py
--rw-rw-rw-   0        0        0     1489 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/collisions.py
--rw-rw-rw-   0        0        0     1420 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/controller.py
--rw-rw-rw-   0        0        0     4639 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/controller_gamepad.py
-drwxrwxrwx   0        0        0        0 2023-04-16 23:10:26.041961 kesslergame-1.3.4/src/kesslergame/graphics/
--rw-rw-rw-   0        0        0      380 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/__init__.py
--rw-rw-rw-   0        0        0      720 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/graphics_base.py
--rw-rw-rw-   0        0        0     2433 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/graphics_handler.py
--rw-rw-rw-   0        0        0     5122 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/graphics_plt.py
--rw-rw-rw-   0        0        0     8874 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/graphics_tk.py
--rw-rw-rw-   0        0        0     3992 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/graphics_ue.py
-drwxrwxrwx   0        0        0        0 2023-04-16 23:10:26.041961 kesslergame-1.3.4/src/kesslergame/graphics/images/
--rw-rw-rw-   0        0        0        0 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/images/__init__.py
--rw-rw-rw-   0        0        0     2708 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip1_green.png
--rw-rw-rw-   0        0        0     2578 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip1_orange.png
--rw-rw-rw-   0        0        0     3597 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip2_orange.png
--rw-rw-rw-   0        0        0     2725 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip3_orange.png
--rw-rw-rw-   0        0        0    14596 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/kessler_game.py
--rw-rw-rw-   0        0        0     6486 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/scenario.py
--rw-rw-rw-   0        0        0     2285 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/score.py
--rw-rw-rw-   0        0        0     8363 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/ship.py
--rw-rw-rw-   0        0        0     1506 2023-04-16 23:09:55.000000 kesslergame-1.3.4/src/kesslergame/team.py
-drwxrwxrwx   0        0        0        0 2023-04-16 23:10:26.041961 kesslergame-1.3.4/src/kesslergame.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-04-16 23:10:25.000000 kesslergame-1.3.4/src/kesslergame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1129 2023-04-16 23:10:25.000000 kesslergame-1.3.4/src/kesslergame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 23:10:25.000000 kesslergame-1.3.4/src/kesslergame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-16 23:10:25.000000 kesslergame-1.3.4/src/kesslergame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 23:10:25.000000 kesslergame-1.3.4/src/kesslergame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 23:10:25.000000 kesslergame-1.3.4/src/kesslergame.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:26.327427 kesslergame-1.3.5/
+-rw-rw-rw-   0        0        0    11565 2023-04-17 20:04:59.000000 kesslergame-1.3.5/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-04-17 20:04:59.000000 kesslergame-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3330 2023-04-17 20:05:26.327427 kesslergame-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2676 2023-04-17 20:04:59.000000 kesslergame-1.3.5/README.md
+-rw-rw-rw-   0        0        0      423 2023-04-17 20:04:59.000000 kesslergame-1.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       23 2023-04-17 20:04:59.000000 kesslergame-1.3.5/requirements.txt
+-rw-rw-rw-   0        0        0      882 2023-04-17 20:05:26.327427 kesslergame-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      369 2023-04-17 20:04:59.000000 kesslergame-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:26.311803 kesslergame-1.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:26.311803 kesslergame-1.3.5/src/kesslergame/
+-rw-rw-rw-   0        0        0      681 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/asteroid.py
+-rw-rw-rw-   0        0        0     1524 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/bullet.py
+-rw-rw-rw-   0        0        0     1489 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/collisions.py
+-rw-rw-rw-   0        0        0     1420 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/controller.py
+-rw-rw-rw-   0        0        0     4639 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/controller_gamepad.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:26.327427 kesslergame-1.3.5/src/kesslergame/graphics/
+-rw-rw-rw-   0        0        0      380 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/graphics_base.py
+-rw-rw-rw-   0        0        0     2433 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/graphics_handler.py
+-rw-rw-rw-   0        0        0     5122 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/graphics_plt.py
+-rw-rw-rw-   0        0        0     8874 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/graphics_tk.py
+-rw-rw-rw-   0        0        0     3992 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/graphics_ue.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:26.327427 kesslergame-1.3.5/src/kesslergame/graphics/images/
+-rw-rw-rw-   0        0        0        0 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/images/__init__.py
+-rw-rw-rw-   0        0        0     2708 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip1_green.png
+-rw-rw-rw-   0        0        0     2578 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip1_orange.png
+-rw-rw-rw-   0        0        0     3597 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip2_orange.png
+-rw-rw-rw-   0        0        0     2725 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip3_orange.png
+-rw-rw-rw-   0        0        0    14604 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/kessler_game.py
+-rw-rw-rw-   0        0        0     6486 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/scenario.py
+-rw-rw-rw-   0        0        0     2285 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/score.py
+-rw-rw-rw-   0        0        0     8315 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/ship.py
+-rw-rw-rw-   0        0        0     1506 2023-04-17 20:04:59.000000 kesslergame-1.3.5/src/kesslergame/team.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:05:26.311803 kesslergame-1.3.5/src/kesslergame.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-17 20:05:26.000000 kesslergame-1.3.5/src/kesslergame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1129 2023-04-17 20:05:26.000000 kesslergame-1.3.5/src/kesslergame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:05:26.000000 kesslergame-1.3.5/src/kesslergame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 20:05:26.000000 kesslergame-1.3.5/src/kesslergame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-17 20:05:26.000000 kesslergame-1.3.5/src/kesslergame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 20:05:26.000000 kesslergame-1.3.5/src/kesslergame.egg-info/zip-safe
```

### Comparing `kesslergame-1.3.4/LICENSE` & `kesslergame-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/PKG-INFO` & `kesslergame-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kesslergame
-Version: 1.3.4
+Version: 1.3.5
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zachariah.phillips@us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@psibernetix.com
 License: Apache 2.0 License
```

### Comparing `kesslergame-1.3.4/README.md` & `kesslergame-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/setup.cfg` & `kesslergame-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/__init__.py` & `kesslergame-1.3.5/src/kesslergame/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .scenario import Scenario
 from .score import Score
 from .graphics import GraphicsType, KesslerGraphics
 
 
 __all__ = ['KesslerGame', 'TrainerEnvironment', 'KesslerController', 'Scenario', 'Score', 'GraphicsType',
            'KesslerGraphics', 'GamepadController']
-__version__ = '1.3.4'
+__version__ = '1.3.5'
```

### Comparing `kesslergame-1.3.4/src/kesslergame/asteroid.py` & `kesslergame-1.3.5/src/kesslergame/asteroid.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/bullet.py` & `kesslergame-1.3.5/src/kesslergame/bullet.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/collisions.py` & `kesslergame-1.3.5/src/kesslergame/collisions.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/controller.py` & `kesslergame-1.3.5/src/kesslergame/controller.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/controller_gamepad.py` & `kesslergame-1.3.5/src/kesslergame/controller_gamepad.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/graphics_base.py` & `kesslergame-1.3.5/src/kesslergame/graphics/graphics_base.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/graphics_handler.py` & `kesslergame-1.3.5/src/kesslergame/graphics/graphics_handler.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/graphics_plt.py` & `kesslergame-1.3.5/src/kesslergame/graphics/graphics_plt.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/graphics_tk.py` & `kesslergame-1.3.5/src/kesslergame/graphics/graphics_tk.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/graphics_ue.py` & `kesslergame-1.3.5/src/kesslergame/graphics/graphics_ue.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip1_green.png` & `kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip1_green.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip1_orange.png` & `kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip1_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip2_orange.png` & `kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip2_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/graphics/images/playerShip3_orange.png` & `kesslergame-1.3.5/src/kesslergame/graphics/images/playerShip3_orange.png`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/kessler_game.py` & `kesslergame-1.3.5/src/kesslergame/kessler_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,16 @@
 
             # --- Check ship-ship collisions ---
             for ship1 in liveships:
                 for ship2 in liveships:
                     if (ship1 is not ship2) and (not ship2.is_respawning) and (not ship1.is_respawning):
                         dist = np.sqrt(sum([(pos1 - pos2) ** 2 for pos1, pos2 in zip(ship1.position, ship2.position)]))
                         if dist < ship1.radius + ship2.radius:
-                            ship1.destruct(map_size=scenario.map_size) # Only destroy one ship. Other ship gets destructed in its loop
+                            ship1.destruct(map_size=scenario.map_size)
+                            ship2.destruct(map_size=scenario.map_size)
             # Cull ships that are not alive
             liveships = [ship for ship in liveships if ship.alive]
 
             # Update performance tracker with collisions timing
             if self.perf_tracker:
                 perf_dict['collisions_check'] = time.perf_counter() - prev
                 prev = time.perf_counter()
```

### Comparing `kesslergame-1.3.4/src/kesslergame/scenario.py` & `kesslergame-1.3.5/src/kesslergame/scenario.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/score.py` & `kesslergame-1.3.5/src/kesslergame/score.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame/ship.py` & `kesslergame-1.3.5/src/kesslergame/ship.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,20 +191,19 @@
 
     def destruct(self, map_size):
         """
         Called by the game when a ship collides with something and dies. Handles life decrementing and triggers respawn
         """
         self.lives -= 1
         self.deaths +=1
-        if self.lives > 0:
-            # spawn_position = [map_size[0] / 2,
-            #                   map_size[1] / 2]
-            spawn_position = self.position
-            spawn_heading = self.heading
-            self.respawn(spawn_position, spawn_heading)
+        # spawn_position = [map_size[0] / 2,
+        #                   map_size[1] / 2]
+        spawn_position = self.position
+        spawn_heading = self.heading
+        self.respawn(spawn_position, spawn_heading)
 
     def respawn(self, position: List[float], heading: float = 90.0) -> None:
         """
         Called when we die and need to make a new ship.
         'respawning' is an invulnerability timer.
         """
         # If we are in the middle of respawning, this is non-zero.
```

### Comparing `kesslergame-1.3.4/src/kesslergame/team.py` & `kesslergame-1.3.5/src/kesslergame/team.py`

 * *Files identical despite different names*

### Comparing `kesslergame-1.3.4/src/kesslergame.egg-info/PKG-INFO` & `kesslergame-1.3.5/src/kesslergame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kesslergame
-Version: 1.3.4
+Version: 1.3.5
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zachariah.phillips@us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@psibernetix.com
 License: Apache 2.0 License
```

### Comparing `kesslergame-1.3.4/src/kesslergame.egg-info/SOURCES.txt` & `kesslergame-1.3.5/src/kesslergame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

