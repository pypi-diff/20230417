# Comparing `tmp/kiui-0.1.3.tar.gz` & `tmp/kiui-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiui-0.1.3.tar", last modified: Mon Apr  3 06:21:05 2023, max compression
+gzip compressed data, was "kiui-0.1.4.tar", last modified: Mon Apr 17 07:12:12 2023, max compression
```

## Comparing `kiui-0.1.3.tar` & `kiui-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:21:05.396114 kiui-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 06:20:48.000000 kiui-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-03 06:21:05.396114 kiui-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-03 06:20:48.000000 kiui-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:21:05.396114 kiui-0.1.3/kiui/
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-03 06:20:48.000000 kiui-0.1.3/kiui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-03 06:20:48.000000 kiui-0.1.3/kiui/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-03 06:20:48.000000 kiui-0.1.3/kiui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-03 06:20:48.000000 kiui-0.1.3/kiui/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:21:05.396114 kiui-0.1.3/kiui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-03 06:21:05.000000 kiui-0.1.3/kiui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-03 06:21:05.000000 kiui-0.1.3/kiui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 06:21:05.000000 kiui-0.1.3/kiui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-03 06:21:05.000000 kiui-0.1.3/kiui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-03 06:21:05.000000 kiui-0.1.3/kiui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 06:21:05.396114 kiui-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-03 06:20:48.000000 kiui-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:12:12.621698 kiui-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 07:11:48.000000 kiui-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 07:12:12.621698 kiui-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-17 07:11:48.000000 kiui-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:12:12.621698 kiui-0.1.4/kiui/
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-17 07:11:48.000000 kiui-0.1.4/kiui/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:12:12.621698 kiui-0.1.4/kiui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 07:12:12.000000 kiui-0.1.4/kiui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 07:12:12.621698 kiui-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-17 07:11:48.000000 kiui-0.1.4/setup.py
```

### Comparing `kiui-0.1.3/LICENSE` & `kiui-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kiui-0.1.3/PKG-INFO` & `kiui-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiui
-Version: 0.1.3
+Version: 0.1.4
 Summary: self-use toolkits
 Home-page: https://github.com/ashawkey/kiuikit
 Author: kiui
 Author-email: ashawkey1999@gmail.com
 Keywords: utility
 Classifier: Programming Language :: Python :: 3 
 Description-Content-Type: text/markdown
-Provides-Extra: full
 License-File: LICENSE
 
 # kiui kit
 
 Utils for self-use.
 
 ### Install
```

### Comparing `kiui-0.1.3/README.md` & `kiui-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kiui-0.1.3/kiui/__init__.py` & `kiui-0.1.4/kiui/__init__.py`

 * *Files identical despite different names*

### Comparing `kiui-0.1.3/kiui/utils.py` & `kiui-0.1.4/kiui/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 import numpy as np
+
 import cv2
 import json
 import varname
 from PIL import Image
 
 from rich.console import Console
-from rich.text import Text
 
 # inspect array like object x and report stats
 def lo(*xs, verbose=0):
 
     console = Console()
 
     def _lo(x, name):
```

### Comparing `kiui-0.1.3/kiui/vis.py` & `kiui-0.1.4/kiui/vis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,120 @@
 import torch
 import numpy as np
 
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 
-import trimesh
 from .utils import lo
 
 def map_color(value, cmap_name='viridis', vmin=None, vmax=None):
     # value: [N], float
     # return: RGB, [N, 3], float in [0, 1]
 
     if vmin is None: vmin = value.min()
     if vmax is None: vmax = value.max()
     value = (value - vmin) / (vmax - vmin) # range in [0, 1]
     cmap = cm.get_cmap(cmap_name) 
     rgb = cmap(value)[:, :3]  # will return rgba, we take only first 3 so we get rgb
     return rgb
 
+# visualize some 2D matrix, different from plot_image, this will keep the original range and plot channel-by-channel
+def plot_matrix(*xs):
+    # x: [B, C, H, W], [C, H, W], or [H, W] torch.Tensor
+    #    [B, H, W, C], [H, W, C], or [H, W] numpy.ndarray
+
+    def _plot_matrix(matrix):
+            
+        if isinstance(matrix, torch.Tensor):
+            if len(matrix.shape) == 3:
+                matrix = matrix.permute(1,2,0).squeeze()
+            matrix = matrix.detach().cpu().numpy()
+
+        lo(matrix)
+
+        if len(matrix.shape) == 3:
+            # per channel
+            for i in range(matrix.shape[-1]):
+                plt.matshow(matrix[..., i])
+                plt.show()
+        else:
+            plt.matshow(matrix)
+            plt.show()
 
-def plot_image(*xs, renormalize=False):
-    # x: [3, H, W] or [1, H, W] or [H, W] torch.Tensor
-    #    [H, W, 3] or [H, W] numpy.ndarray
-
-    def _plot_image(x):
-
-        if isinstance(x, torch.Tensor):
-            if len(x.shape) == 3:
-                x = x.permute(1,2,0).squeeze()
-            x = x.detach().cpu().numpy()
+    for x in xs:
+        if len(x.shape) == 4:
+            for i in range(x.shape[0]):
+                _plot_matrix(x[i])
+        else:
+            _plot_matrix(x)
+  
+# sequentially plot provided images
+def plot_image(*xs, normalize=False):
+    # x: [B, 3, H, W], [3, H, W], [1, H, W] or [H, W] torch.Tensor
+    #    [B, H, W, 3], [H, W, 3], [H, W, 1] or [H, W] numpy.ndarray
+
+    def _plot_image(image):
+
+        if isinstance(image, torch.Tensor):
+            if len(image.shape) == 3:
+                image = image.permute(1,2,0).squeeze()
+            image = image.detach().cpu().numpy()
 
-        lo(x)
+        lo(image)
 
-        x = x.astype(np.float32)
+        image = image.astype(np.float32)
         
-        # renormalize
-        if renormalize:
-            x = (x - x.min(axis=0, keepdims=True)) / (x.max(axis=0, keepdims=True) - x.min(axis=0, keepdims=True) + 1e-8)
+        # normalize
+        if normalize:
+            image = (image - image.min(axis=0, keepdims=True)) / (image.max(axis=0, keepdims=True) - image.min(axis=0, keepdims=True) + 1e-8)
 
-        plt.imshow(x)
+        plt.imshow(image)
         plt.show()
     
     for x in xs:
-        _plot_image(x)
+        if len(x.shape) == 4:
+            for i in range(x.shape[0]):
+                _plot_image(x[i])
+        else:
+            _plot_image(x)
 
 
 def plot_pointcloud(pc, color=None):
     # pc: [N, 3]
     # color: [N, 3/4]
 
     lo(pc)
 
-    # import open3d as o3d
-    # pcd = o3d.geometry.PointCloud()
-    # pcd.points = o3d.utility.Vector3dVector(pc)
-    # if color is not None:
-    #     pcd.colors = o3d.utility.Vector3dVector(color)
-    # o3d.visualization.draw_geometries([pcd])
-
-    pc = trimesh.PointCloud(pc, color)
-    # axis
-    axes = trimesh.creation.axis(axis_length=4)
-    # sphere
-    box = trimesh.primitives.Box(extents=(2, 2, 2)).as_outline()
-    box.colors = np.array([[128, 128, 128]] * len(box.entities))
+    if color is None or color.shape[-1] == 3:
+        # use o3d as it's better to control
+        import open3d as o3d
+        pcd = o3d.geometry.PointCloud()
+        pcd.points = o3d.utility.Vector3dVector(pc)
+        if color is not None:
+            pcd.colors = o3d.utility.Vector3dVector(color)
+        o3d.visualization.draw_geometries([pcd])
+
+    else:
+        import trimesh
+        pc = trimesh.PointCloud(pc, color)
+        # axis
+        axes = trimesh.creation.axis(axis_length=4)
+        # sphere
+        box = trimesh.primitives.Box(extents=(2, 2, 2)).as_outline()
+        box.colors = np.array([[128, 128, 128]] * len(box.entities))
 
-    trimesh.Scene([pc, axes, box]).show()
+        trimesh.Scene([pc, axes, box]).show()
     
 
-def plot_poses(poses, size=0.05, bound=1, points=None):
+def plot_poses(poses, size=0.05, bound=1, points=None, mesh=None):
     # poses: [B, 4, 4]
 
     lo(poses)
 
+    import trimesh
     axes = trimesh.creation.axis(axis_length=4)
     box = trimesh.primitives.Box(extents=[2*bound]*3).as_outline()
     box.colors = np.array([[128, 128, 128]] * len(box.entities))
     objects = [axes, box]
 
     if bound > 1:
         unit_box = trimesh.primitives.Box(extents=[2]*3).as_outline()
@@ -96,20 +134,21 @@
         o = pos + dir * 3
 
         segs = np.array([[pos, a], [pos, b], [pos, c], [pos, d], [a, b], [b, c], [c, d], [d, a], [pos, o]])
         segs = trimesh.load_path(segs)
         objects.append(segs)
 
     if points is not None:
-        print('[visualize points]', points.shape, points.dtype, points.min(0), points.max(0))
+
+        lo(points)
+
         colors = np.zeros((points.shape[0], 4), dtype=np.uint8)
         colors[:, 2] = 255 # blue
         colors[:, 3] = 30 # transparent
         objects.append(trimesh.PointCloud(points, colors))
 
-    # tmp: verify mesh matches the points
-    # mesh = trimesh.load('trial_garden_colmap/mesh_stage0/mesh.ply')
-    # objects.append(mesh)
+    if mesh is not None:
+        objects.append(mesh)
 
     scene = trimesh.Scene(objects)
     scene.set_camera(distance=bound, center=[0, 0, 0])
     scene.show()
```

### Comparing `kiui-0.1.3/kiui.egg-info/PKG-INFO` & `kiui-0.1.4/kiui.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiui
-Version: 0.1.3
+Version: 0.1.4
 Summary: self-use toolkits
 Home-page: https://github.com/ashawkey/kiuikit
 Author: kiui
 Author-email: ashawkey1999@gmail.com
 Keywords: utility
 Classifier: Programming Language :: Python :: 3 
 Description-Content-Type: text/markdown
-Provides-Extra: full
 License-File: LICENSE
 
 # kiui kit
 
 Utils for self-use.
 
 ### Install
```

### Comparing `kiui-0.1.3/setup.py` & `kiui-0.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == '__main__':
     setup(
         name="kiui",
-        version='0.1.3',
+        version='0.1.4',
         description="self-use toolkits",
         long_description=open('README.md', encoding='utf-8').read(),
         long_description_content_type='text/markdown',
         url='https://github.com/ashawkey/kiuikit',
         author='kiui',
         author_email='ashawkey1999@gmail.com',
         packages=['kiui'],
@@ -15,17 +15,15 @@
         classifiers=[
             'Programming Language :: Python :: 3 ',
         ],
         keywords='utility',
         install_requires=[
             'varname',
             'rich',
+            'trimesh',
+            'numpy',
+            'torch',
+            'tqdm',
+            'matplotlib',
+            'opencv-python',
         ],
-        extras_require={
-            'full': [
-                'tqdm',
-                'numpy',
-                'matplotlib',
-                'opencv-python',
-            ],
-        },
     )
```

