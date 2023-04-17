# Comparing `tmp/processpiper-0.1.0.tar.gz` & `tmp/processpiper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processpiper-0.1.0.tar", last modified: Sun Apr 16 03:06:28 2023, max compression
+gzip compressed data, was "processpiper-0.2.0.tar", last modified: Mon Apr 17 09:22:21 2023, max compression
```

## Comparing `processpiper-0.1.0.tar` & `processpiper-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 03:06:28.864277 processpiper-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6067 2023-04-16 03:06:28.864277 processpiper-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5512 2023-04-16 03:05:50.000000 processpiper-0.1.0/README.md
--rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 03:06:28.864277 processpiper-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 03:06:28.830269 processpiper-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 03:06:28.846273 processpiper-0.1.0/src/processpiper/
--rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.1.0/src/processpiper/__init__.py
--rw-rw-rw-   0        0        0     2090 2023-04-09 09:57:23.000000 processpiper-0.1.0/src/processpiper/activity.py
--rw-rw-rw-   0        0        0    11680 2023-04-16 00:20:15.000000 processpiper-0.1.0/src/processpiper/colourtheme.py
--rw-rw-rw-   0        0        0     1752 2023-04-10 02:30:30.000000 processpiper-0.1.0/src/processpiper/constants.py
--rw-rw-rw-   0        0        0     4978 2023-04-16 00:55:33.000000 processpiper-0.1.0/src/processpiper/event.py
--rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.1.0/src/processpiper/footer.py
--rw-rw-rw-   0        0        0     2800 2023-04-09 09:10:50.000000 processpiper-0.1.0/src/processpiper/gateway.py
--rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.1.0/src/processpiper/helper.py
--rw-rw-rw-   0        0        0    10601 2023-04-10 09:12:37.000000 processpiper-0.1.0/src/processpiper/lane.py
--rw-rw-rw-   0        0        0    35774 2023-04-16 00:46:46.000000 processpiper-0.1.0/src/processpiper/painter.py
--rw-rw-rw-   0        0        0     5071 2023-04-10 03:09:02.000000 processpiper-0.1.0/src/processpiper/pool.py
--rw-rw-rw-   0        0        0    17739 2023-04-16 00:50:43.000000 processpiper-0.1.0/src/processpiper/processmap.py
--rw-rw-rw-   0        0        0    18671 2023-04-10 08:48:17.000000 processpiper-0.1.0/src/processpiper/shape.py
--rw-rw-rw-   0        0        0     5424 2023-04-16 02:56:17.000000 processpiper-0.1.0/src/processpiper/text2diagram.py
--rw-rw-rw-   0        0        0     2267 2023-04-09 09:14:12.000000 processpiper-0.1.0/src/processpiper/title.py
--rw-rw-rw-   0        0        0     1189 2023-04-09 08:43:43.000000 processpiper-0.1.0/src/processpiper/version.py
-drwxrwxrwx   0        0        0        0 2023-04-16 03:06:28.861276 processpiper-0.1.0/src/processpiper.egg-info/
--rw-rw-rw-   0        0        0     6067 2023-04-16 03:06:28.000000 processpiper-0.1.0/src/processpiper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-04-16 03:06:28.000000 processpiper-0.1.0/src/processpiper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 03:06:28.000000 processpiper-0.1.0/src/processpiper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 03:06:28.000000 processpiper-0.1.0/src/processpiper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 03:06:28.000000 processpiper-0.1.0/src/processpiper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 03:06:28.863277 processpiper-0.1.0/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.1.0/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-04-10 04:22:15.000000 processpiper-0.1.0/src/tests/github_action_test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.723548 processpiper-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6655 2023-04-17 09:22:21.722547 processpiper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6100 2023-04-17 09:21:44.000000 processpiper-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:22:21.723548 processpiper-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.684538 processpiper-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.704543 processpiper-0.2.0/src/processpiper/
+-rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.2.0/src/processpiper/__init__.py
+-rw-rw-rw-   0        0        0     2090 2023-04-09 09:57:23.000000 processpiper-0.2.0/src/processpiper/activity.py
+-rw-rw-rw-   0        0        0    11673 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/colourtheme.py
+-rw-rw-rw-   0        0        0     1752 2023-04-10 02:30:30.000000 processpiper-0.2.0/src/processpiper/constants.py
+-rw-rw-rw-   0        0        0     4978 2023-04-16 00:55:33.000000 processpiper-0.2.0/src/processpiper/event.py
+-rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.2.0/src/processpiper/footer.py
+-rw-rw-rw-   0        0        0     2800 2023-04-09 09:10:50.000000 processpiper-0.2.0/src/processpiper/gateway.py
+-rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.2.0/src/processpiper/helper.py
+-rw-rw-rw-   0        0        0    10507 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/lane.py
+-rw-rw-rw-   0        0        0    35774 2023-04-16 00:46:46.000000 processpiper-0.2.0/src/processpiper/painter.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/pool.py
+-rw-rw-rw-   0        0        0    17603 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/processmap.py
+-rw-rw-rw-   0        0        0    18609 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/shape.py
+-rw-rw-rw-   0        0        0     6829 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/text2diagram.py
+-rw-rw-rw-   0        0        0     2267 2023-04-09 09:14:12.000000 processpiper-0.2.0/src/processpiper/title.py
+-rw-rw-rw-   0        0        0     1189 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/processpiper/version.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.719547 processpiper-0.2.0/src/processpiper.egg-info/
+-rw-rw-rw-   0        0        0     6655 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-17 09:22:21.000000 processpiper-0.2.0/src/processpiper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 09:22:21.720547 processpiper-0.2.0/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.2.0/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.2.0/src/tests/github_action_test.py
```

### Comparing `processpiper-0.1.0/LICENSE` & `processpiper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/PKG-INFO` & `processpiper-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-Metadata-Version: 2.1
-Name: processpiper
-Version: 0.1.0
-Summary: Processpiper. An open source python library to generate business process diagram using code.
-Author: CS Goh
-Project-URL: Homepage, https://github.com/csgoh/processpiper
-Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
+![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
+![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
+![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
+![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
+![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
+[![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
 
 # ProcessPiper (Business Process Diagram as Code)
 A python library to generate business process diagram using code. 
 
 ## Why ProcessPiper?
 1. Generate professional business process diagrams with Python code, eliminating the need for manual drawing and complex tools.
 2. Improve teamwork by utilising source code repositories for change monitoring, collaboration, and diagram history.
@@ -52,14 +44,19 @@
 
 ### Python version requirements:
 * Python 3.10, 3.11
   
 ### Library Dependencies
 * Pillow 9.4.0
 
+### Supported Platforms
+* Windows
+* Ubuntu
+* MacOS
+
 ## Documentation
 Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this RaC library.
 
 ## Examples
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
```

### Comparing `processpiper-0.1.0/README.md` & `processpiper-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,30 @@
+Metadata-Version: 2.1
+Name: processpiper
+Version: 0.2.0
+Summary: Processpiper. An open source python library to generate business process diagram using code.
+Author: CS Goh
+Project-URL: Homepage, https://github.com/csgoh/processpiper
+Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
+![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
+![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
+![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
+![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
+[![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
 
 # ProcessPiper (Business Process Diagram as Code)
 A python library to generate business process diagram using code. 
 
 ## Why ProcessPiper?
 1. Generate professional business process diagrams with Python code, eliminating the need for manual drawing and complex tools.
 2. Improve teamwork by utilising source code repositories for change monitoring, collaboration, and diagram history.
@@ -38,14 +58,19 @@
 
 ### Python version requirements:
 * Python 3.10, 3.11
   
 ### Library Dependencies
 * Pillow 9.4.0
 
+### Supported Platforms
+* Windows
+* Ubuntu
+* MacOS
+
 ## Documentation
 Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this RaC library.
 
 ## Examples
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
```

### Comparing `processpiper-0.1.0/pyproject.toml` & `processpiper-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/activity.py` & `processpiper-0.2.0/src/processpiper/activity.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/colourtheme.py` & `processpiper-0.2.0/src/processpiper/colourtheme.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 
 
 DEFAULT_FONT = "Arial"
 DEFAULT_TITLE_FONT_SIZE = 26
 DEFAULT_POOL_FONT_SIZE = 18
 DEFAULT_LANE_FONT_SIZE = 18
 DEFAULT_ELEMENT_FONT_SIZE = 14
```

### Comparing `processpiper-0.1.0/src/processpiper/constants.py` & `processpiper-0.2.0/src/processpiper/constants.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/event.py` & `processpiper-0.2.0/src/processpiper/event.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/footer.py` & `processpiper-0.2.0/src/processpiper/footer.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/gateway.py` & `processpiper-0.2.0/src/processpiper/gateway.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/helper.py` & `processpiper-0.2.0/src/processpiper/helper.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/lane.py` & `processpiper-0.2.0/src/processpiper/lane.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from itertools import count
 from .shape import Shape
 from .painter import Painter
 from .event import Event, Start, End, Timer, Intermediate
 from .activity import Activity, Task, Subprocess
 from .gateway import Gateway, Exclusive, Parallel, Inclusive
 from .constants import Configs
-from .helper import Helper
+#from .helper import Helper
 
 
 class EventType:
     """Event types"""
 
     START = "Start"
     END = "End"
@@ -251,23 +251,21 @@
         ### Set own shape position
         if shape.lane_name == self.name:
             shape_x, shape_y, shape_w, shape_h = shape.set_draw_position(
                 x,
                 (y + Configs.LANE_SHAPE_TOP_MARGIN),
                 painter,
             )
-            next_x = shape_x + shape_w + Configs.HSPACE_BETWEEN_SHAPES
-
+            
             #### Mark for removal
             # shape.draw_position_set = True
 
             shape.x_pos_traversed = True
 
             ### Set next elements' position
-            this_lane = self.name
             for index, next_shape in enumerate(shape.connection_to.target):
 
                 ### Check whether the position has been set, if yes, skipped.
                 ### This is needed to avoid infinite recursion
                 if next_shape.traversed == True:
                     continue
```

### Comparing `processpiper-0.1.0/src/processpiper/painter.py` & `processpiper-0.2.0/src/processpiper/painter.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/pool.py` & `processpiper-0.2.0/src/processpiper/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from dataclasses import dataclass, field
 from .painter import Painter
 from .lane import Lane
 from .constants import Configs
-from .helper import Helper
 
 
 @dataclass
 class Pool:
     """A pool is a collection of lanes."""
 
     name: str = field(init=True)
```

### Comparing `processpiper-0.1.0/src/processpiper/processmap.py` & `processpiper-0.2.0/src/processpiper/processmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,19 +193,19 @@
                 for shape in lane.shapes:
                     ### If the shape has no connection_from, it is the start shape
                     Helper.printc(f"{shape.name} - {len(shape.connection_from)}")
                     if len(shape.connection_from) == 0:
                         return shape
         return None
 
-    def get_lane_by_id(self, id: int) -> Lane:
+    def get_lane_by_id(self, lane_id: int) -> Lane:
         """Get a lane by its id"""
         for pool in self._pools:
             for lane in pool._lanes:
-                if lane.id == id:
+                if lane.id == lane_id:
                     return lane
         return None
 
     def get_pool_by_name(self, name: str) -> Pool:
         """Get a pool by its name"""
         for pool in self._pools:
             if pool.name == name:
@@ -221,25 +221,24 @@
     ):
         """Set the x position for the shape"""
         current_lane = self.get_lane_by_id(current_shape.lane_id)
         Helper.printc(
             f"set_shape_x_position: {current_lane.name}, {current_shape.name}", "34"
         )
         if index == 0:
-            current_pool = self.get_pool_by_name(current_shape.pool_name)
+            
             if previous_shape is not None:
                 if previous_shape.pool_name == current_shape.pool_name:
                     if previous_shape.lane_id == current_shape.lane_id:
                         current_shape.x = self.get_next_x_position()
                         Helper.printc(f"          same pool same lane")
                     else:
                         current_shape.x = self.get_next_x_position()
                         Helper.printc(f"          same pool diff lane")
                 else:
-                    previous_pool = self.get_pool_by_name(previous_shape.pool_name)
                     current_shape.x = self.get_next_x_position()
                     Helper.printc(f"          diff pool")
             else:
                 current_shape.x = self.get_next_x_position()
                 Helper.printc(f"          previous = none")
         else:
             ### If previous shape is connecting to multiple shapes,
```

### Comparing `processpiper-0.1.0/src/processpiper/shape.py` & `processpiper-0.2.0/src/processpiper/shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 # SOFTWARE.
 from dataclasses import dataclass, field
 import math
 from itertools import count
 from .painter import Painter
 from .helper import Helper
 
-# from .connection import Connection
+
 from typing import TypeVar
-from .helper import Helper
+
 
 ### This is to allow the connect method to return the same type of shape
 TShape = TypeVar("TShape", bound="Shape")
 
 BOX_WIDTH = 100
 BOX_HEIGHT = 60
 CIRCLE_RADIUS = 20
```

### Comparing `processpiper-0.1.0/src/processpiper/title.py` & `processpiper-0.2.0/src/processpiper/title.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/processpiper/version.py` & `processpiper-0.2.0/src/processpiper/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Version information for processpiper."""
-__version__ = "v0.1.0"
+__version__ = "v0.2.0"
```

### Comparing `processpiper-0.1.0/src/processpiper.egg-info/PKG-INFO` & `processpiper-0.2.0/src/processpiper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.1.0
+Version: 0.2.0
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
+![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
+![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
+![python version](https://img.shields.io/pypi/pyversions/processpiper?style=plastic)
+![stars](https://img.shields.io/github/stars/csgoh/processpiper?style=plastic)
+[![Twitter Follow](https://img.shields.io/twitter/follow/CSGohNZ?style=social)](https://twitter.com/CSGohNZ)
 
 # ProcessPiper (Business Process Diagram as Code)
 A python library to generate business process diagram using code. 
 
 ## Why ProcessPiper?
 1. Generate professional business process diagrams with Python code, eliminating the need for manual drawing and complex tools.
 2. Improve teamwork by utilising source code repositories for change monitoring, collaboration, and diagram history.
@@ -52,14 +58,19 @@
 
 ### Python version requirements:
 * Python 3.10, 3.11
   
 ### Library Dependencies
 * Pillow 9.4.0
 
+### Supported Platforms
+* Windows
+* Ubuntu
+* MacOS
+
 ## Documentation
 Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this RaC library.
 
 ## Examples
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
```

### Comparing `processpiper-0.1.0/src/processpiper.egg-info/SOURCES.txt` & `processpiper-0.2.0/src/processpiper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processpiper-0.1.0/src/tests/github_action_test.py` & `processpiper-0.2.0/src/tests/github_action_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import inspect
 import os.path
-import time
 
 
 from src.processpiper import ProcessMap, EventType, ActivityType, GatewayType
 
 
 def prep_for_test(filename: str):
     path = os.path.join("images", "test")
```

