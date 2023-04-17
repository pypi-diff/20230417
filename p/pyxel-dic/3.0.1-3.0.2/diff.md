# Comparing `tmp/pyxel-dic-3.0.1.tar.gz` & `tmp/pyxel-dic-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel-dic-3.0.1.tar", last modified: Fri Apr  7 10:12:41 2023, max compression
+gzip compressed data, was "pyxel-dic-3.0.2.tar", last modified: Mon Apr 17 15:15:22 2023, max compression
```

## Comparing `pyxel-dic-3.0.1.tar` & `pyxel-dic-3.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 10:12:41.683986 pyxel-dic-3.0.1/
--rw-rw-rw-   0        0        0     4675 2023-04-07 10:12:41.683986 pyxel-dic-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3998 2023-04-03 06:25:37.000000 pyxel-dic-3.0.1/README.md
--rw-rw-rw-   0        0        0      777 2023-04-07 10:08:59.000000 pyxel-dic-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      898 2023-04-07 10:12:41.688019 pyxel-dic-3.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 10:12:41.500924 pyxel-dic-3.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 10:12:41.640253 pyxel-dic-3.0.1/src/pyxel/
--rw-rw-rw-   0        0        0      323 2023-04-07 09:22:53.000000 pyxel-dic-3.0.1/src/pyxel/__init__.py
--rw-rw-rw-   0        0        0    30095 2023-04-07 09:47:16.000000 pyxel-dic-3.0.1/src/pyxel/camera.py
--rw-rw-rw-   0        0        0    24473 2023-04-07 09:40:44.000000 pyxel-dic-3.0.1/src/pyxel/dic.py
--rw-rw-rw-   0        0        0     2317 2023-04-07 09:22:53.000000 pyxel-dic-3.0.1/src/pyxel/exportpixmap.py
--rw-rw-rw-   0        0        0    11341 2023-04-07 09:26:23.000000 pyxel-dic-3.0.1/src/pyxel/image.py
--rw-rw-rw-   0        0        0     9658 2023-04-07 09:22:53.000000 pyxel-dic-3.0.1/src/pyxel/levelset.py
--rw-rw-rw-   0        0        0     3293 2023-04-07 09:46:08.000000 pyxel-dic-3.0.1/src/pyxel/material.py
--rw-rw-rw-   0        0        0   115237 2023-04-07 09:45:00.000000 pyxel-dic-3.0.1/src/pyxel/mesh.py
--rw-rw-rw-   0        0        0    17624 2023-04-07 09:22:53.000000 pyxel-dic-3.0.1/src/pyxel/mesher.py
--rw-rw-rw-   0        0        0     6859 2023-04-07 09:22:53.000000 pyxel-dic-3.0.1/src/pyxel/meshparser.py
--rw-rw-rw-   0        0        0     4746 2023-04-07 09:22:53.000000 pyxel-dic-3.0.1/src/pyxel/utils.py
--rw-rw-rw-   0        0        0    15965 2023-04-07 09:22:53.000000 pyxel-dic-3.0.1/src/pyxel/vtktools.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:12:41.679814 pyxel-dic-3.0.1/src/pyxel_dic.egg-info/
--rw-rw-rw-   0        0        0     4675 2023-04-07 10:12:41.000000 pyxel-dic-3.0.1/src/pyxel_dic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-04-07 10:12:41.000000 pyxel-dic-3.0.1/src/pyxel_dic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 10:12:41.000000 pyxel-dic-3.0.1/src/pyxel_dic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-07 10:12:41.000000 pyxel-dic-3.0.1/src/pyxel_dic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-07 10:12:41.000000 pyxel-dic-3.0.1/src/pyxel_dic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.737573 pyxel-dic-3.0.2/
+-rw-rw-rw-   0        0        0     4930 2023-04-17 15:15:22.737573 pyxel-dic-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4250 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/README.md
+-rw-rw-rw-   0        0        0      745 2023-04-17 15:14:03.000000 pyxel-dic-3.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      898 2023-04-17 15:15:22.743204 pyxel-dic-3.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.535867 pyxel-dic-3.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.695455 pyxel-dic-3.0.2/src/pyxel/
+-rw-rw-rw-   0        0        0      332 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/__init__.py
+-rw-rw-rw-   0        0        0    31183 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/camera.py
+-rw-rw-rw-   0        0        0    24473 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/dic.py
+-rw-rw-rw-   0        0        0     2317 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/exportpixmap.py
+-rw-rw-rw-   0        0        0    13368 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/image.py
+-rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/levelset.py
+-rw-rw-rw-   0        0        0     3293 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/material.py
+-rw-rw-rw-   0        0        0   124883 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/mesh.py
+-rw-rw-rw-   0        0        0    17624 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/mesher.py
+-rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/meshparser.py
+-rw-rw-rw-   0        0        0     3245 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/utils.py
+-rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/vtktools.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.730933 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/
+-rw-rw-rw-   0        0        0     4930 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/top_level.txt
```

### Comparing `pyxel-dic-3.0.1/PKG-INFO` & `pyxel-dic-3.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.0.1
+Version: 3.0.2
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: CeCILL
 Project-URL: Homepage, https://github.com/jcpassieux/pyxel
 Project-URL: Bug Tracker, https://github.com/jcpassieux/pyxel/issues
@@ -19,68 +19,72 @@
 **pyxel** is an open-source Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics application. It is freely available for research and teaching.
 
 <p align="center">
   <img src="https://github.com/jcpassieux/pyxel/blob/master/pyxel.png" width="150" title="hover text">
 </p>
 
 In its present form, it is restricted to 2D-DIC and 3D-DVC. Stereo (SDIC) will be updated later. 
-The gray level conservation problem is written in the physical space. It relies on camera models (which must be calibrated) and on a dedicated quadrature rule in the FE mesh space. Considering front-parallel camera settings, the implemented camera model is a simplified pinhole model (including only 4 parameters 2D: 2 translations, 1 rotation and the focal length and 7 parameters in 3D: focal length, 3 rotations, 3 translations) . More complex camera models (including distorsions) could easily be implemented within this framework (next update?). The library natively includes linear and quadratic triangles, quadrilateral, tetraedral, hexaedral elements. The library also exports the results in different format such that the measurements can be post-processed ether with MatPlotLib or using Paraview.
+The gray level conservation problem is written in the physical space. It relies on camera models (which must be calibrated) and on a dedicated quadrature rule in the FE mesh space. Considering front-parallel camera settings, the implemented camera model is a simplified pinhole model (including only 4 parameters 2D: 2 translations, 1 rotation and the focal length and 7 parameters in 3D: focal length, 3 rotations, 3 translations). More complex camera models (including distorsions) could easily be implemented within this framework (next update?). The library natively includes linear and quadratic triangles, quadrilateral, tetraedral, hexaedral elements. The library also exports the results in different format such that the measurements can be post-processed ether with MatPlotLib or using Paraview.
+
+<p align="center">
+  <img src="https://github.com/jcpassieux/pyxel/blob/master/pyxel-figs.png" height="200" title="hover text">
+</p>
 
 1. SCRIPT FILE
     - pyxel is a library. For each testcase, a script file must be written.
-    - a set of sample scripts named `example_#.py` is provided in the `./data` folder
+    - a set of sample scripts named `example_#.py` is provided in the `./test` folder
      to understand the main functionnalities of the library.
 
 2. ABOUT MESHES
-    - a mesh is entierly defined by two variables:
-        (1) a python dictionnary for the elements (the key is the element type and the value is a numpy array of size NE * NN (NN being the number of nodes of this element type and NE the number of elements). The element type label (according to gmsh numbering). 
+    - A Finite Element mesh is required for the displacement measurement. In pyxel, a mesh is entierly defined by two variables:<br>
+        (1) a python dictionary for the elements (the key is the element type and the value is a numpy array of size NE * NN (NN being the number of nodes of this element type and NE the number of elements). The element type label (according to gmsh numbering). 
         example:
         ```python
 	  e = dict()
        e[3] = np.array([[n0, n1, n2, n3]])
         ```
         (2) a numpy array n for the node coordinates, example:
         ```python
         n = np.array([[x0, y0], [x1, y1], ...])
         ```
     - There is an home made mesher for parallelipedic domains, given the approximate elements size in each direction (see examples). We recommand to use external meshers like, for instance, `gmsh`
-    - To read/write the meshes, we rely on the library `meshio`. 
+    - To read/write the meshes, we use the usefull library `meshio`. 
 
-3. USING THE LIBRARY FOR A 2D ANALYSIS
-    - Open the mesh: 
+3. MINIMAL SAMPLE CODE
+    - to run a simple 2D-DIC analysis:
       ```python
-      m = px.ReadMesh('mesh.msh')
+      f = px.Image('img-0.tif').Load()
+      g = px.Image('img-1.tif').Load()
+      roi = np.array([[ 100,   100], [ 500,  500]])
+      m, cam = px.MeshFromROI(roi, 50, f, typel=3)
+      U, res = px.Correlate(f, g, m, cam)
       ```
-    - Open the image:
-      ```python
-      f = px.Image('image.tif').Load()
-      ```
-    - Connectivity, quadrature, Interpolation:
-      ```python
-      m.Connectivity()
-      m.DICIntegration(cam)
-      ```      
-    - Compute DIC approx. Hessian H and right hand side b:
+    - A multiscale initialization is usually required
       ```python
-      dic = px.DICEngine()
-      H = dic.ComputeLHS(f, m, cam)
-      b, res = dic.ComputeRHS(g, m, cam, U)
+      U = px.MultiscaleInit(f, g, m, cam, scales=[3, 2, 1], l0=30)
       ```
 4. OUTPUT FILES
     - It is possible to post-process the results directly using matplotlib.
-       	but a more convenient way is to use Paraview www.paraview.org 
-    - The library exports VTK files written in `./vtk` directory 
-    - `*.vtu` files are generated, but it is also possible to generate 
-      `*.pvd` files for use in paraview.
-
+      ```python
+      m.PlotContourDispl(U, s=30)
+      ```
+    - but a more convenient way (especially in DVC) is to use Paraview www.paraview.org 
+      ```python
+      m.VTKSol('vtufile', U)
+      ```    
 5. TERM OF USE. 
     This program is a free software: you can redistribute it/or modify it. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY.
     **pyxel** is distributed under the terms of CeCILL which is a french free software license agreement in the spirit of GNU GPL
 
 6. DEPENDANCIES 
     `numpy`, `scipy`, `matplotlib`, `opencv-python`, `scikit-image`, `meshio`, `gmsh`
 
+7. INSTALL
+    - It is possible to clone the git repository, or simply install it using PyPI:
+      ```python
+      pip install pyxel-dic
+      ```
 # References
 
 Jean-Charles Passieux, Robin Bouclier. **Classic and Inverse Compositional Gauss-Newton in Global DIC**. *International Journal for Numerical Methods in Engineering*, 119(6), p.453-468, 2019.
 
 Jean-Charles Passieux. **pyxel, an open-source FE-DIC library**. *Zenodo*. http://doi.org/10.5281/zenodo.4654018
```

### Comparing `pyxel-dic-3.0.1/README.md` & `pyxel-dic-3.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,68 +4,72 @@
 **pyxel** is an open-source Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics application. It is freely available for research and teaching.
 
 <p align="center">
   <img src="https://github.com/jcpassieux/pyxel/blob/master/pyxel.png" width="150" title="hover text">
 </p>
 
 In its present form, it is restricted to 2D-DIC and 3D-DVC. Stereo (SDIC) will be updated later. 
-The gray level conservation problem is written in the physical space. It relies on camera models (which must be calibrated) and on a dedicated quadrature rule in the FE mesh space. Considering front-parallel camera settings, the implemented camera model is a simplified pinhole model (including only 4 parameters 2D: 2 translations, 1 rotation and the focal length and 7 parameters in 3D: focal length, 3 rotations, 3 translations) . More complex camera models (including distorsions) could easily be implemented within this framework (next update?). The library natively includes linear and quadratic triangles, quadrilateral, tetraedral, hexaedral elements. The library also exports the results in different format such that the measurements can be post-processed ether with MatPlotLib or using Paraview.
+The gray level conservation problem is written in the physical space. It relies on camera models (which must be calibrated) and on a dedicated quadrature rule in the FE mesh space. Considering front-parallel camera settings, the implemented camera model is a simplified pinhole model (including only 4 parameters 2D: 2 translations, 1 rotation and the focal length and 7 parameters in 3D: focal length, 3 rotations, 3 translations). More complex camera models (including distorsions) could easily be implemented within this framework (next update?). The library natively includes linear and quadratic triangles, quadrilateral, tetraedral, hexaedral elements. The library also exports the results in different format such that the measurements can be post-processed ether with MatPlotLib or using Paraview.
+
+<p align="center">
+  <img src="https://github.com/jcpassieux/pyxel/blob/master/pyxel-figs.png" height="200" title="hover text">
+</p>
 
 1. SCRIPT FILE
     - pyxel is a library. For each testcase, a script file must be written.
-    - a set of sample scripts named `example_#.py` is provided in the `./data` folder
+    - a set of sample scripts named `example_#.py` is provided in the `./test` folder
      to understand the main functionnalities of the library.
 
 2. ABOUT MESHES
-    - a mesh is entierly defined by two variables:
-        (1) a python dictionnary for the elements (the key is the element type and the value is a numpy array of size NE * NN (NN being the number of nodes of this element type and NE the number of elements). The element type label (according to gmsh numbering). 
+    - A Finite Element mesh is required for the displacement measurement. In pyxel, a mesh is entierly defined by two variables:<br>
+        (1) a python dictionary for the elements (the key is the element type and the value is a numpy array of size NE * NN (NN being the number of nodes of this element type and NE the number of elements). The element type label (according to gmsh numbering). 
         example:
         ```python
 	  e = dict()
        e[3] = np.array([[n0, n1, n2, n3]])
         ```
         (2) a numpy array n for the node coordinates, example:
         ```python
         n = np.array([[x0, y0], [x1, y1], ...])
         ```
     - There is an home made mesher for parallelipedic domains, given the approximate elements size in each direction (see examples). We recommand to use external meshers like, for instance, `gmsh`
-    - To read/write the meshes, we rely on the library `meshio`. 
+    - To read/write the meshes, we use the usefull library `meshio`. 
 
-3. USING THE LIBRARY FOR A 2D ANALYSIS
-    - Open the mesh: 
+3. MINIMAL SAMPLE CODE
+    - to run a simple 2D-DIC analysis:
       ```python
-      m = px.ReadMesh('mesh.msh')
+      f = px.Image('img-0.tif').Load()
+      g = px.Image('img-1.tif').Load()
+      roi = np.array([[ 100,   100], [ 500,  500]])
+      m, cam = px.MeshFromROI(roi, 50, f, typel=3)
+      U, res = px.Correlate(f, g, m, cam)
       ```
-    - Open the image:
-      ```python
-      f = px.Image('image.tif').Load()
-      ```
-    - Connectivity, quadrature, Interpolation:
-      ```python
-      m.Connectivity()
-      m.DICIntegration(cam)
-      ```      
-    - Compute DIC approx. Hessian H and right hand side b:
+    - A multiscale initialization is usually required
       ```python
-      dic = px.DICEngine()
-      H = dic.ComputeLHS(f, m, cam)
-      b, res = dic.ComputeRHS(g, m, cam, U)
+      U = px.MultiscaleInit(f, g, m, cam, scales=[3, 2, 1], l0=30)
       ```
 4. OUTPUT FILES
     - It is possible to post-process the results directly using matplotlib.
-       	but a more convenient way is to use Paraview www.paraview.org 
-    - The library exports VTK files written in `./vtk` directory 
-    - `*.vtu` files are generated, but it is also possible to generate 
-      `*.pvd` files for use in paraview.
-
+      ```python
+      m.PlotContourDispl(U, s=30)
+      ```
+    - but a more convenient way (especially in DVC) is to use Paraview www.paraview.org 
+      ```python
+      m.VTKSol('vtufile', U)
+      ```    
 5. TERM OF USE. 
     This program is a free software: you can redistribute it/or modify it. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY.
     **pyxel** is distributed under the terms of CeCILL which is a french free software license agreement in the spirit of GNU GPL
 
 6. DEPENDANCIES 
     `numpy`, `scipy`, `matplotlib`, `opencv-python`, `scikit-image`, `meshio`, `gmsh`
 
+7. INSTALL
+    - It is possible to clone the git repository, or simply install it using PyPI:
+      ```python
+      pip install pyxel-dic
+      ```
 # References
 
 Jean-Charles Passieux, Robin Bouclier. **Classic and Inverse Compositional Gauss-Newton in Global DIC**. *International Journal for Numerical Methods in Engineering*, 119(6), p.453-468, 2019.
 
-Jean-Charles Passieux. **pyxel, an open-source FE-DIC library**. *Zenodo*. http://doi.org/10.5281/zenodo.4654018
+Jean-Charles Passieux. **pyxel, an open-source FE-DIC library**. *Zenodo*. http://doi.org/10.5281/zenodo.4654018
```

### Comparing `pyxel-dic-3.0.1/pyproject.toml` & `pyxel-dic-3.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-[build-system]
-requires = [
-    "setuptools>=42",
-    "wheel",
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pyxel-dic"
-version = "3.0.1"
-authors = [
-  { name="JC Passieux", email="jc.passieux@gmail.com" },
-]
-description = "Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "numpy",
-    "scipy",
-    "matplotlib",
-    "meshio",
-    "opencv-python",
-    "gmsh",
-    "scikit-image",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/jcpassieux/pyxel"
+[build-system]
+requires = [
+    "setuptools>=42",
+    "wheel",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pyxel-dic"
+version = "3.0.2"
+authors = [
+  { name="JC Passieux", email="jc.passieux@gmail.com" },
+]
+description = "Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "numpy",
+    "scipy",
+    "matplotlib",
+    "meshio",
+    "opencv-python",
+    "gmsh",
+    "scikit-image",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/jcpassieux/pyxel"
 "Bug Tracker" = "https://github.com/jcpassieux/pyxel/issues"
```

### Comparing `pyxel-dic-3.0.1/setup.cfg` & `pyxel-dic-3.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.1/src/pyxel/camera.py` & `pyxel-dic-3.0.2/src/pyxel/camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -573,14 +573,17 @@
 # print(sp.pycode(w.diff(tx, 1)))
 # print(sp.pycode(w.diff(ty, 1)))
 # print(sp.pycode(w.diff(tz, 1)))
 # print(sp.pycode(w.diff(rx, 1)))
 # print(sp.pycode(w.diff(ry, 1)))
 # print(sp.pycode(w.diff(rz, 1)))
 
+
+
+
 class CameraVol:
     def __init__(self, p):
         self.set_p(p)
 
     def set_p(self, p):
         """
         Set manually the camera parameters.
@@ -673,15 +676,34 @@
         v = X*(-f*np.sin(rx)*np.sin(ry)*np.cos(rz) + f*np.sin(rz)*np.cos(ry)) + \
             Y*f*np.cos(rx)*np.cos(rz) + Z*(-f*np.sin(rx)*np.cos(ry)*np.cos(rz) - \
                                                f*np.sin(ry)*np.sin(rz)) + f*ty
         w = X*f*np.sin(ry)*np.cos(rx) + Y*f*np.sin(rx) + \
             Z*f*np.cos(rx)*np.cos(ry) + f*tz
         return u, v, w
 
-    def PinvNL(self, u, v, w):
+    # import sympy as sp
+    # dPxdX, dPxdY, dPxdZ, dPydX, dPydY, dPydZ, dPzdX, dPzdY, dPzdZ = \
+    #    sp.symbols('dPxdX, dPxdY, dPxdZ, dPydX, dPydY, dPydZ, dPzdX, dPzdY, dPzdZ')    
+    # J = sp.Matrix([[dPxdX, dPxdY, dPxdZ],
+    #                [dPydX, dPydY, dPydZ],
+    #                [dPzdX, dPzdY, dPzdZ]])
+    # detJ = sp.det(J)
+    # print(sp.pycode(detJ))
+    # Jinv = J.inv()*detJ
+    # print(Jinv[0,0])
+    # print(Jinv[0,1])
+    # print(Jinv[0,2])
+    # print(Jinv[1,0])
+    # print(Jinv[1,1])
+    # print(Jinv[1,2])    
+    # print(Jinv[2,0])
+    # print(Jinv[2,1])
+    # print(Jinv[2,2])
+
+    def Pinv(self, u, v, w):
         """
         Inverse of the Camera model. Maps a point in the image to a point
         in the mesh coordinate sys.
         (General version for any possibly NL camera models)
 
         Parameters
         ----------
@@ -698,33 +720,41 @@
             X coordinate of the corresponding position in the mesh system
         Y : 1D NUMPY.ARRAY
             Y coordinate of the corresponding position in the mesh system
         Z : 1D NUMPY.ARRAY
             Z coordinate of the corresponding position in the mesh system
 
         """
-        X = np.zeros(len(u))
-        Y = np.zeros(len(u))
-        Z = np.zeros(len(u))
+        X = np.zeros_like(u)
+        Y = np.zeros_like(u)
+        Z = np.zeros_like(u)
         for ii in range(10):
             pnx, pny, pnz = self.P(X, Y, Z)
             resx = u - pnx
             resy = v - pny
             resz = w - pnz
-            raise Exception("PinvNL for CameraVol not implemented yet... TODO!")
             dPxdX, dPxdY, dPxdZ, dPydX, dPydY, dPydZ, dPzdX, dPzdY, dPzdZ = self.dPdX(X, Y, Z)
-            detJ = dPxdX * dPydY - dPxdY * dPydX
-            dX = dPydY / detJ * resx - dPxdY / detJ * resy
-            dY = -dPydX / detJ * resx + dPxdX / detJ * resy
+            detJ = dPxdX*dPydY*dPzdZ - dPxdX*dPydZ*dPzdY - dPxdY*dPydX*dPzdZ + \
+                dPxdY*dPydZ*dPzdX + dPxdZ*dPydX*dPzdY - dPxdZ*dPydY*dPzdX
+            dX = ((dPydY*dPzdZ - dPydZ*dPzdY) * resx + \
+                (-dPxdY*dPzdZ + dPxdZ*dPzdY) * resy + \
+                 (dPxdY*dPydZ - dPxdZ*dPydY) * resz) / detJ
+            dY = ((-dPydX*dPzdZ + dPydZ*dPzdX) * resx + \
+                   (dPxdX*dPzdZ - dPxdZ*dPzdX) * resy + \
+                  (-dPxdX*dPydZ + dPxdZ*dPydX) * resz ) / detJ
+            dZ = ((dPydX*dPzdY - dPydY*dPzdX) * resx + \
+                 (-dPxdX*dPzdY + dPxdY*dPzdX) * resy + \
+                  (dPxdX*dPydY - dPxdY*dPydX) * resz ) / detJ
             X += dX
             Y += dY
-            res = np.linalg.norm(dX) + np.linalg.norm(dY)
+            Z += dZ
+            res = np.linalg.norm(dX) + np.linalg.norm(dY) + np.linalg.norm(dZ)
             if res < 1e-4:
                 break
-        return X, Y
+        return X, Y, Z
 
     def dPdX(self, X, Y, Z):
         """
         Derivative of the Camera model wrt physical position X, Y
 
         Parameters
         ----------
```

### Comparing `pyxel-dic-3.0.1/src/pyxel/dic.py` & `pyxel-dic-3.0.2/src/pyxel/dic.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.1/src/pyxel/exportpixmap.py` & `pyxel-dic-3.0.2/src/pyxel/exportpixmap.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.1/src/pyxel/image.py` & `pyxel-dic-3.0.2/src/pyxel/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,57 +10,74 @@
 
 """
 import os
 import numpy as np
 import scipy.interpolate as spi
 import matplotlib.pyplot as plt
 from .utils import PlotMeshImage
-from .vtktools import VTIWriter
+from .vtktools import VTIWriter, PVDFile
 import cv2
 from skimage import io
+from warnings import warn
 
 class Image:
     def __init__(self, fname):
         """Contructor"""
         self.fname = fname
+        self.x0 = 0
+        self.y0 = 0
         
     def LoadPIL(self):
         import PIL.Image as image
         """Load image data using Pillow"""
         if os.path.isfile(self.fname):
             if self.fname.split(".")[-1] == "npy":
-                self.pix = np.load(self.fname)
+                self.pix = np.load(self.fname, allow_pickle=False)
+            elif self.fname.split(".")[-1] == "npz":
+                fnpz = np.load(self.fname, allow_pickle=False)
+                # Only one array
+                self.pix = fnpz[fnpz.files[0]]
+                if len(fnpz.files) > 0:
+                    warn("Took the first dataset in file "+self.fname)
             else:
                 self.pix = np.asarray(image.open(self.fname)).astype(float)
-                # self.pix = image.imread(self.fname).astype(float)
             if len(self.pix.shape) == 3:
                 self.ToGray()
         else:
             raise Exception("File "+self.fname+" not in directory "+os.getcwd())
         return self
 
     def Load(self, bw=True):
         """Load image data"""
         if os.path.isfile(self.fname):
             if self.fname.split(".")[-1] == "npy":
-                self.pix = np.load(self.fname)
+                self.pix = np.load(self.fname, allow_pickle=False)
+            elif self.fname.split(".")[-1] == "npz":
+                fnpz = np.load(self.fname, allow_pickle=False)
+                # Only one array
+                self.pix = fnpz[fnpz.files[0]]
+                if len(fnpz.files) > 0:
+                    warn("Took the first dataset in file "+self.fname)
             else:
                 self.pix = cv2.imread(self.fname).astype(float)
-                if len(self.pix.shape) == 3 and bw:
-                    self.ToGray()
             if len(self.pix.shape) == 3 and bw:
                 self.ToGray()
         else:
-            print("File "+self.fname+" not in directory "+os.getcwd())
+            raise Exception("File "+self.fname+" not in directory "+os.getcwd())
         return self
 
+    def SetOrigin(self, x0, y0):
+        self.x0 = x0
+        self.y0 = y0
+
     def Copy(self):
         """Image Copy"""
         newimg = Image("Copy")
         newimg.pix = self.pix.copy()
+        newimg.SetOrigin(self.x0, self.y0)
         return newimg
 
     def Save(self, fname):
         """Image Save"""
         f = np.round(self.pix).astype("uint8")
         cv2.imwrite(fname,f)
 
@@ -70,23 +87,23 @@
         y = np.arange(0, self.pix.shape[1])
         self.tck = spi.RectBivariateSpline(x, y, self.pix)
 
     def Interp(self, x, y):
         """evaluate interpolator at non-integer pixel position x, y"""
         if not hasattr(self,'tck'):
             self.BuildInterp()
-        return self.tck.ev(x, y)
+        return self.tck.ev(x-self.x0, y-self.y0)
 
     def InterpGrad(self, x, y):
         """evaluate gradient of the interpolator at non-integer pixel position x, y"""
-        return self.tck.ev(x, y, 1, 0), self.tck.ev(x, y, 0, 1)
+        return self.tck.ev(x-self.x0, y-self.y0, 1, 0), self.tck.ev(x-self.x0, y-self.y0, 0, 1)
 
     def InterpHess(self, x, y):
         """evaluate Hessian of the interpolator at non-integer pixel position x, y"""
-        return self.tck.ev(x, y, 2, 0), self.tck.ev(x, y, 0, 2), self.tck.ev(x, y, 1, 1)
+        return self.tck.ev(x-self.x0, y-self.y0, 2, 0), self.tck.ev(x-self.x0, y-self.y0, 0, 2), self.tck.ev(x-self.x0, y-self.y0, 1, 1)
 
     def Plot(self):
         """Plot Image"""
         plt.imshow(self.pix, cmap="gray", interpolation="none", origin="upper")
         # plt.axis('off')
         # plt.colorbar()
 
@@ -122,14 +139,15 @@
         )
         nn[0] = nn[0] // scale
         im0 = np.mean(
             im0.reshape(nn[1], nn[0]).T.reshape(np.prod(nn) // scale, scale), axis=1
         )
         nn[1] = nn[1] // scale
         self.pix = im0.reshape(nn)
+        self.SetOrigin(self.x0/scale, self.y0/scale)
 
     def ToGray(self, type="lum"):
         """Convert RGB to Grayscale :
 
         Parameters
         ----------
         type : string
@@ -171,17 +189,17 @@
         if title is None:
             if n < 0:
                 plt.title("Select some points... and press enter")
             else:
                 plt.title("Select " + str(n) + " points... and press enter")
         else:
             plt.title(title)
-        pts1 = np.array(plt.ginput(n, timeout=0))
+        pts1 = np.array(plt.ginput(n, timeout=0)) - np.array([[self.x0, self.y0]])
         plt.close()
-        return pts1
+        return pts1 
 
     def SelectROI(self, m=None, cam=None):
         """Select a Region of Interest within the image. 
         
         Parameters
         ----------
         m : pyxel.Mesh object (OPTIONNAL)
@@ -202,21 +220,20 @@
             self.Plot()
 
         def line_select_callback(eclick, erelease):
             x1, y1 = eclick.xdata, eclick.ydata
             x2, y2 = erelease.xdata, erelease.ydata
             print(
                 "roi = np.array([[%4d, %4d], [%4d, %4d]])"
-                % (int(x1), int(y1), int(x2), int(y2))
+                % (int(x1+self.x0), int(y1+self.y0), int(x2+self.x0), int(y2+self.y0))
             )
 
         rs = RectangleSelector(
             ax,
             line_select_callback,
-            drawtype="box",
             useblit=False,
             button=[1],
             minspanx=5,
             minspany=5,
             spancoords="pixels",
             interactive=True,
         )
@@ -225,72 +242,99 @@
 
 #%%
 
 class Volume:
     def __init__(self, fname):
         """Contructor"""
         self.fname = fname
+        self.x0 = 0
+        self.y0 = 0
+        self.z0 = 0
 
     def Load(self):
         """Load image data"""
         if os.path.isfile(self.fname):
             if self.fname.split(".")[-1] == "mat":
                 import scipy.io as spio
                 matf = spio.loadmat(self.fname)
                 print(matf.keys())
                 for k in matf.keys():
                     if type(matf[k]) == np.ndarray:
                         print('Opened %s in *.mat file' % (k,))
                         self.pix  = matf[k].astype('double')
                         break
             elif self.fname.split(".")[-1] == "npy":
-                self.pix = np.load(self.fname)
+                self.pix = np.load(self.fname, allow_pickle=False)
+            elif self.fname.split(".")[-1] == "npz":
+                fnpz = np.load(self.fname, allow_pickle=False)
+                # Only one array
+                self.pix = fnpz[fnpz.files[0]]
+                if len(fnpz.files) > 0:
+                    warn("Took the first dataset in file "+self.fname)
             else:
                 self.pix = io.imread(self.fname).astype('double')
         else:
             raise Exception("File "+self.fname+" not in directory "+os.getcwd())
         return self
 
+    def SetOrigin(self, x0, y0, z0):
+        self.x0 = x0
+        self.y0 = y0
+        self.z0 = z0
+
     def Copy(self):
         """Image Copy"""
         newimg = Volume("Copy")
         newimg.pix = self.pix.copy()
+        newimg.SetOrigin(self.x0, self.y0, self.z0)
         return newimg
 
     def Save(self, fname='SavedVolume.tiff'):
         """Image Save"""
         f = np.round(self.pix).astype("uint8")
         io.imsave(fname, f)
 
-    def VTKImage(self, fname='SavedVolume'):
+    def VTKImage(self, fname='SavedVolume', sx=0, sy=0, sz=0):
         """Image Save"""
         fpix = np.round(self.pix).astype("uint8")
-        vtk = VTIWriter(self.pix.shape[0], self.pix.shape[1], self.pix.shape[2])
+        vtk = VTIWriter(self.pix.shape[0], self.pix.shape[1], self.pix.shape[2], sx, sy, sz)
         vtk.addCellData('f', 1, fpix.T.ravel())
         dir0, filename = os.path.split(fname)
         if not os.path.isdir(os.path.join("vtk", dir0)):
             os.makedirs(os.path.join("vtk", dir0))
         vtk.VTIWriter(os.path.join("vtk", dir0, filename))
+
+    def VTKSlice(self, fname='SavedSlice'):
+        """Image Save"""
+        nx, ny, nz = self.pix.shape
+        fs = self.Copy()
+        fs.pix = self.pix[[nx//2], :, :]
+        fs.VTKImage(fname+'_0_0', nx//2, 0, 0)
+        fs.pix = self.pix[:, [ny//2], :]
+        fs.VTKImage(fname+'_1_0', 0, ny//2, 0)
+        fs.pix = self.pix[:, :, [nz//2]]
+        fs.VTKImage(fname+'_2_0', 0, 0, nz//2)
+        PVDFile(os.path.join('vtk', fname),'vti',3,1)
         
     def BuildInterp(self):
         """build trilinear interp"""
         x = np.arange(self.pix.shape[0])
         y = np.arange(self.pix.shape[1])
         z = np.arange(self.pix.shape[2])
         self.interp = spi.RegularGridInterpolator((x,y,z), self.pix, method='linear', bounds_error=True, fill_value=None)
 
     def Interp(self, x, y, z):
         """Evaluate the continuous representation of the voxels """
         if not hasattr(self,'interp'):
             self.BuildInterp()
-        return self.interp(np.vstack((x, y, z)).T) 
+        return self.interp(np.vstack((x-self.x0, y-self.y0, z-self.z0)).T)
 
     def InterpGrad(self, x, y, z, eps = 1.e-7):
         """Evaluate the gradient of the continuous representation of the voxels """
-        P_coords = np.vstack((x,y,z)).T
+        P_coords = np.vstack((x-self.x0, y-self.y0, z-self.z0)).T
         df_dP = []
         for xi in range(3):
             P_coords_xi_p_dxi = P_coords.copy()
             P_coords_xi_p_dxi[:, xi] = P_coords_xi_p_dxi[:, xi] + eps/2
             P_coords_xi_m_dxi = P_coords.copy()
             P_coords_xi_m_dxi[:, xi] = P_coords_xi_m_dxi[:, xi] - eps/2
             df_dP.append( (self.interp(P_coords_xi_p_dxi) - self.interp(P_coords_xi_m_dxi))/(eps))
@@ -335,7 +379,8 @@
         plt.show()
 
     def SubSample(self, n):
         """Image copy with subsampling for multiscale initialization"""
         from skimage.transform import downscale_local_mean
         scale = 2**n
         self.pix = downscale_local_mean(self.pix, (scale, scale, scale))
+        self.SetOrigin(self.x0/scale, self.y0/scale, self.z0/scale)
```

### Comparing `pyxel-dic-3.0.1/src/pyxel/levelset.py` & `pyxel-dic-3.0.2/src/pyxel/levelset.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.1/src/pyxel/material.py` & `pyxel-dic-3.0.2/src/pyxel/material.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.1/src/pyxel/mesh.py` & `pyxel-dic-3.0.2/src/pyxel/mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import scipy as sp
 from mpl_toolkits.mplot3d import Axes3D
 from mpl_toolkits.mplot3d import art3d
 import matplotlib.pyplot as plt
 import matplotlib.collections as cols
 import matplotlib.animation as animation
 #from numba import njit # uncomment for just in time compilation
-from .utils import meshgrid, isInBox, PVDFile
+from .utils import meshgrid, isInBox
+from .vtktools import PVDFile
 import meshio
 
 def ElTypes():
     """
     Returns a dictionnary of GMSH element types which some of them are used in the library.
     """
     return {
@@ -639,31 +640,237 @@
             one = np.ones(len(x))
             return np.concatenate((-one, zer, zer, one)).reshape((4, len(x))).T
         xg = 0.25 * np.array([1])
         yg = 0.25 * np.array([1])
         zg = 0.25 * np.array([1])
         wg = np.array([0.1666666666666666])
         return xg, yg, zg, wg, N, dN_xi, dN_eta, dN_zeta
-    # elif eltype == 11:
-    #     """
-    #     #############
-    #         Tet10
-    #     #############
-    #     """
-    #     xg = 0.25 * np.array([1])
-    #     yg = 0.25 * np.array([1])
-    #     zg = 0.25 * np.array([1])
-    #     wg = np.array([0.1666666666666666])
-    # x = np.ones((4, 4))*0.13819660 @ np.array([0, 1, 0, 0])
-    # y = np.ones((4, 4))*0.13819660 @ np.array([0, 0, 1, 0])
-    # z = np.ones((4, 4))*0.13819660 @ np.array([0, 0, 0, 1])
+    elif eltype == 11:
+        """
+        #############
+            Tet10
+        #############
+        """
+        def N(x, y, z):
+            return np.concatenate(((1-x-y-z)*(1-2*x-2*y-2*z),
+                                    x*(2*x-1),
+                                    y*(2*y-1),
+                                    z*(2*z-1),
+                                    4*z*(1-x-y-z),
+                                    4*x*y,
+                                    4*y*z,
+                                    4*y*(1-x-y-z),
+                                    4*x*z,
+                                    4*x*(1-x-y-z),
+                                    )).reshape((10, len(x))).T
+        def dN_xi(x, y, z):
+            zer = np.zeros(len(x))
+            return np.concatenate((-3+4*x+4*y+4*z,
+                                   4*x-1,
+                                   zer, 
+                                   zer,
+                                   -4*z,
+                                   4*y,
+                                   zer,
+                                   -4*y,
+                                   4*z,
+                                   4*(1-2*x-y-z),
+                                   )).reshape((10, len(x))).T
+        def dN_eta(x, y, z):
+            zer = np.zeros(len(x))
+            return np.concatenate((-3+4*x+4*y+4*z, 
+                                   zer, 
+                                   4*y-1, 
+                                   zer,
+                                   -4*z,
+                                   4*x,
+                                   4*z,
+                                   4*(1-x-2*y-z),                                   
+                                   zer,
+                                   -4*x,
+                                   )).reshape((10, len(x))).T
+        def dN_zeta(x, y, z):
+            zer = np.zeros(len(x))
+            return np.concatenate((-3+4*x+4*y+4*z, 
+                                   zer, 
+                                   zer, 
+                                   4*z-1,
+                                   4*(1-x-y-2*z),
+                                   zer,
+                                   4*y,
+                                   -4*y,
+                                   4*x,
+                                   -4*x,
+                                   )).reshape((10, len(x))).T
+
+        ### 4 Gauss points
+        c = 0.585410196624968
+        b = 0.138196601125010
+        xg = np.array([b,b,b,c])
+        yg = np.array([b,b,c,b])
+        zg = np.array([b,c,b,b])
+        wg = np.array([1,1,1,1]) * 0.25
+        
+        ### 15 Gauss points
+        # a = 0.25
+        # b1 = (7+np.sqrt(15))/34
+        # b2 = (7-np.sqrt(15))/34
+        # c1 = (13-3*np.sqrt(15))/34
+        # c2 = (13+3*np.sqrt(15))/34
+        # d = (5-np.sqrt(15))/20
+        # e = (5+np.sqrt(15))/20
+        # w1 = 8/405
+        # w2 = (2665-14*np.sqrt(15))/226800
+        # w3 = (2665+14*np.sqrt(15))/226800
+        # w4 = 5/567
+        # xg = np.array([a,b1,b1,b1,c1,b2,b2,b2,c2,d,d,e,d,e,e])
+        # yg = np.array([a,b1,b1,c1,b1,b2,b2,c2,b2,d,e,d,e,d,e])
+        # zg = np.array([a,b1,c1,b1,b1,b2,c2,b2,b2,e,d,d,e,e,d])
+        # wg = np.array([w1,w2,w2,w2,w2,w3,w3,w3,w3,w4,w4,w4,w4,w4,w4])
+        
+        return xg, yg, zg, wg, N, dN_xi, dN_eta, dN_zeta
+    elif eltype == 17:
+        """
+        #############
+            Hex20
+        #############
+        """
+        # import sympy as sp
+        # x, y, z = sp.symbols('x, y, z')
+        # f = [(1-x)*(1-y)*(1-z)*(-2-x-y-z),
+        #                 (1+x)*(1-y)*(1-z)*(-2+x-y-z),
+        #                 (1+x)*(1+y)*(1-z)*(-2+x+y-z),
+        #                 (1-x)*(1+y)*(1-z)*(-2-x+y-z),
+        #                 (1-x)*(1-y)*(1+z)*(-2-x-y+z),
+        #                 (1+x)*(1-y)*(1+z)*(-2+x-y+z),
+        #                 (1+x)*(1+y)*(1+z)*(-2+x+y+z),
+        #                 (1-x)*(1+y)*(1+z)*(-2-x+y+z),
+        #                 2*(1-x**2)*(1-y)*(1-z),
+        #                 2*(1+x)*(1-y**2)*(1-z),
+        #                 2*(1-x**2)*(1+y)*(1-z),
+        #                 2*(1-x)*(1-y**2)*(1-z),
+        #                 2*(1-x**2)*(1-y)*(1+z),
+        #                 2*(1+x)*(1-y**2)*(1+z),
+        #                 2*(1-x**2)*(1+y)*(1+z),
+        #                 2*(1-x)*(1-y**2)*(1+z),
+        #                 2*(1-x)*(1-y)*(1-z**2),
+        #                 2*(1+x)*(1-y)*(1-z**2),
+        #                 2*(1+x)*(1+y)*(1-z**2),
+        #                 2*(1-x)*(1+y)*(1-z**2)]
+        # for fi in f:
+        #     print(sp.pycode(sp.diff(fi, x)))
+        # for fi in f:
+        #     print(sp.pycode(sp.diff(fi, y)))
+        # for fi in f:
+        #     print(sp.pycode(sp.diff(fi, z)))
+        def N(x, y, z):
+            return 0.125 * np.concatenate(((1-x)*(1-y)*(1-z)*(-2-x-y-z),
+                                           (1+x)*(1-y)*(1-z)*(-2+x-y-z),
+                                           (1+x)*(1+y)*(1-z)*(-2+x+y-z),
+                                           (1-x)*(1+y)*(1-z)*(-2-x+y-z),
+                                           (1-x)*(1-y)*(1+z)*(-2-x-y+z),
+                                           (1+x)*(1-y)*(1+z)*(-2+x-y+z),
+                                           (1+x)*(1+y)*(1+z)*(-2+x+y+z),
+                                           (1-x)*(1+y)*(1+z)*(-2-x+y+z),
+                                           2*(1-x**2)*(1-y)*(1-z),
+                                           2*(1+x)*(1-y**2)*(1-z),
+                                           2*(1-x**2)*(1+y)*(1-z),
+                                           2*(1-x)*(1-y**2)*(1-z),
+                                           2*(1-x**2)*(1-y)*(1+z),
+                                           2*(1+x)*(1-y**2)*(1+z),
+                                           2*(1-x**2)*(1+y)*(1+z),
+                                           2*(1-x)*(1-y**2)*(1+z),
+                                           2*(1-x)*(1-y)*(1-z**2),
+                                           2*(1+x)*(1-y)*(1-z**2),
+                                           2*(1+x)*(1+y)*(1-z**2),
+                                           2*(1-x)*(1+y)*(1-z**2))).reshape((20, len(x))).T
+        def dN_xi(x, y, z):
+            return 0.125 * np.concatenate((
+            -(1 - x)*(1 - y)*(1 - z) - (1 - y)*(1 - z)*(-x - y - z - 2),
+            (1 - y)*(1 - z)*(x + 1) + (1 - y)*(1 - z)*(x - y - z - 2),
+            (1 - z)*(x + 1)*(y + 1) + (1 - z)*(y + 1)*(x + y - z - 2),
+            -(1 - x)*(1 - z)*(y + 1) - (1 - z)*(y + 1)*(-x + y - z - 2),
+            -(1 - x)*(1 - y)*(z + 1) - (1 - y)*(z + 1)*(-x - y + z - 2),
+            (1 - y)*(x + 1)*(z + 1) + (1 - y)*(z + 1)*(x - y + z - 2),
+            (x + 1)*(y + 1)*(z + 1) + (y + 1)*(z + 1)*(x + y + z - 2),
+            -(1 - x)*(y + 1)*(z + 1) - (y + 1)*(z + 1)*(-x + y + z - 2),
+            -4*x*(1 - y)*(1 - z),
+            2*(1 - y**2)*(1 - z),
+            -4*x*(1 - z)*(y + 1),
+            -2*(1 - y**2)*(1 - z),
+            -4*x*(1 - y)*(z + 1),
+            2*(1 - y**2)*(z + 1),
+            -4*x*(y + 1)*(z + 1),
+            -2*(1 - y**2)*(z + 1),
+            -2*(1 - y)*(1 - z**2),
+            2*(1 - y)*(1 - z**2),
+            2*(1 - z**2)*(y + 1),
+            -2*(1 - z**2)*(y + 1)
+            )).reshape((20, len(x))).T
+        def dN_eta(x, y, z):
+            return 0.125 * np.concatenate((
+            -(1 - x)*(1 - y)*(1 - z) - (1 - x)*(1 - z)*(-x - y - z - 2),
+            -(1 - y)*(1 - z)*(x + 1) - (1 - z)*(x + 1)*(x - y - z - 2),
+            (1 - z)*(x + 1)*(y + 1) + (1 - z)*(x + 1)*(x + y - z - 2),
+            (1 - x)*(1 - z)*(y + 1) + (1 - x)*(1 - z)*(-x + y - z - 2),
+            -(1 - x)*(1 - y)*(z + 1) - (1 - x)*(z + 1)*(-x - y + z - 2),
+            -(1 - y)*(x + 1)*(z + 1) - (x + 1)*(z + 1)*(x - y + z - 2),
+            (x + 1)*(y + 1)*(z + 1) + (x + 1)*(z + 1)*(x + y + z - 2),
+            (1 - x)*(y + 1)*(z + 1) + (1 - x)*(z + 1)*(-x + y + z - 2),
+            -(1 - z)*(2 - 2*x**2),
+            -2*y*(1 - z)*(2*x + 2),
+            (1 - z)*(2 - 2*x**2),
+            -2*y*(1 - z)*(2 - 2*x),
+            -(2 - 2*x**2)*(z + 1),
+            -2*y*(2*x + 2)*(z + 1),
+            (2 - 2*x**2)*(z + 1),
+            -2*y*(2 - 2*x)*(z + 1),
+            -(1 - z**2)*(2 - 2*x),
+            -(1 - z**2)*(2*x + 2),
+            (1 - z**2)*(2*x + 2),
+            (1 - z**2)*(2 - 2*x)
+            )).reshape((20, len(x))).T
+        def dN_zeta(x, y, z):
+            return 0.125 * np.concatenate((
+            -(1 - x)*(1 - y)*(1 - z) - (1 - x)*(1 - y)*(-x - y - z - 2),
+            -(1 - y)*(1 - z)*(x + 1) - (1 - y)*(x + 1)*(x - y - z - 2),
+            -(1 - z)*(x + 1)*(y + 1) - (x + 1)*(y + 1)*(x + y - z - 2),
+            -(1 - x)*(1 - z)*(y + 1) - (1 - x)*(y + 1)*(-x + y - z - 2),
+            (1 - x)*(1 - y)*(z + 1) + (1 - x)*(1 - y)*(-x - y + z - 2),
+            (1 - y)*(x + 1)*(z + 1) + (1 - y)*(x + 1)*(x - y + z - 2),
+            (x + 1)*(y + 1)*(z + 1) + (x + 1)*(y + 1)*(x + y + z - 2),
+            (1 - x)*(y + 1)*(z + 1) + (1 - x)*(y + 1)*(-x + y + z - 2),
+            -(1 - y)*(2 - 2*x**2),
+            -(1 - y**2)*(2*x + 2),
+            -(2 - 2*x**2)*(y + 1),
+            -(1 - y**2)*(2 - 2*x),
+            (1 - y)*(2 - 2*x**2),
+            (1 - y**2)*(2*x + 2),
+            (2 - 2*x**2)*(y + 1),
+            (1 - y**2)*(2 - 2*x),
+            -2*z*(1 - y)*(2 - 2*x),
+            -2*z*(1 - y)*(2*x + 2),
+            -2*z*(2*x + 2)*(y + 1),
+            -2*z*(2 - 2*x)*(y + 1),
+            )).reshape((20, len(x))).T
 
+        # 8 gauss points
+        xg = np.sqrt(3) / 3 * np.array([-1, 1, -1, 1, -1, 1, -1, 1])
+        yg = np.sqrt(3) / 3 * np.array([-1, -1, 1, 1, -1, -1, 1, 1])
+        zg = np.sqrt(3) / 3 * np.array([-1, -1, -1, -1, 1, 1, 1, 1])
+        wg = np.ones(8)
         
-    #     0.58541020
-    #     return xg, yg, zg, wg, N, dN_xi, dN_eta, dN_zeta
+        # 27 gauss points
+        # xi = np.array([-np.sqrt(3/5), 0, np.sqrt(3/5)])
+        # xg, yg, zg = np.meshgrid(xi, xi, xi)
+        # wi = np.array([0.5555555555555556, 0.8888888888888888, 0.5555555555555556])
+        # wx, wy, wz = np.meshgrid(wi, wi, wi)
+        # wg = wy*wx*wz
+        return xg.ravel(), yg.ravel(), zg.ravel(), wg.ravel(), N, dN_xi, dN_eta, dN_zeta
+
 
 
 #%% 
 class Mesh:
     def __init__(self, e, n, dim=2):
         """Contructor from elems and node arrays"""
         self.e = e
@@ -1732,15 +1939,15 @@
         UU is a (ndof x nstep) Numpy array containing the displacement dofs
          where ndof is the numer of dofs
          ans   nstep the number of time steps
         """
         for ig in range(UU.shape[1]):
             fname = filename + "_0_" + str(ig)
             self.VTKSol(fname, UU[:, ig])
-        PVDFile(filename, "vtu", 1, UU.shape[1])
+        PVDFile(os.path.join('vtk',filename), "vtu", 1, UU.shape[1])
 
     def Write(self, filename, point_data={}, cell_data={}):
         """
         Export a meshfile using meshio.
         mesh format depends on the chosen extension.
         Abaqus (.inp), ANSYS msh (.msh), AVS-UCD (.avs), CGNS (.cgns), 
         DOLFIN XML (.xml), Exodus (.e, .exo), FLAC3D (.f3grid), H5M (.h5m), 
@@ -2540,15 +2747,15 @@
 
     def KeepVolElems(self):
         """
         Removes every but volume (or 3D) elements.
         """
         newe = dict()
         for je in self.e.keys():
-            if je in [4, 5, 10, 11, 12]:
+            if je in [4, 5, 11, 12, 14, 17]:
                 newe[je] = self.e[je]
         self.e = newe
 
     def RemoveElemsOutsideRoi(self, roi, cam=None):
         """
         Removes all the elements whose center lie in the Region of Interest of
         an image f.
```

### Comparing `pyxel-dic-3.0.1/src/pyxel/mesher.py` & `pyxel-dic-3.0.2/src/pyxel/mesher.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.1/src/pyxel/meshparser.py` & `pyxel-dic-3.0.2/src/pyxel/meshparser.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.1/src/pyxel/vtktools.py` & `pyxel-dic-3.0.2/src/pyxel/vtktools.py`

 * *Files 3% similar despite different names*

```diff
@@ -293,19 +293,22 @@
         # Write to file and exit
         outFile = open(fileName, 'w')
         doc.writexml(outFile, newl='\n')
         print("VTK: "+ fileName +".vtr written")
         outFile.close()
 
 class VTIWriter():
-    def __init__(self, nx, ny, nz):
+    def __init__(self, nx, ny, nz, sx=0, sy=0, sz=0):
         self.clearData()
         self.nx = nx
         self.ny = ny
         self.nz = nz
+        self.sx = sx
+        self.sy = sy
+        self.sz = sz
     def addCellData(self, varName, numb, data):
         cdnew = VTKData(varName, numb, data)
         self.cd = np.append(self.cd, cdnew)
     def addPointData(self, varName, numb, data):
         pdnew = VTKData(varName, numb, data)
         self.pd = np.append(self.pd, pdnew)
     def clearData(self):
@@ -319,15 +322,15 @@
         root_element.setAttribute("type", "ImageData")
         root_element.setAttribute("version", "0.1")
         root_element.setAttribute("byte_order", "LittleEndian")
         doc.appendChild(root_element)
     
         # ImageData element
         ImageData = doc.createElementNS("VTK", "ImageData")
-        extent=np.array([0, self.nx, 0, self.ny, 0, self.nz])
+        extent=np.array([self.sx, self.sx+self.nx, self.sy, self.sy+self.ny, self.sz, self.sz+self.nz])
         ImageData.setAttribute("WholeExtent", array2string(extent))
         ImageData.setAttribute("Origin", "-0.5 -0.5 -0.5")
         ImageData.setAttribute("Spacing", "1 1 1")
         root_element.appendChild(ImageData)
     
         # Piece 0 (only one)
         piece = doc.createElementNS("VTK", "Piece")
@@ -364,22 +367,37 @@
     
         # Write to file and exit
         fileName += '.vti'
         outFile = open(fileName, 'w')
         doc.writexml(outFile, newl='\n')
         print("VTI: "+ fileName +" written")
         outFile.close()
-    
-def PVDFile(fileName,ext,npart,nstep):    
-    """ Write PVD file
+
+def PVDFile(fileName,ext,npart,nstep):
+    """
+    Write PVD file
     Usage: writePVD("toto","vtu",npart,nstep) 
     generated file: "toto.pvd" 
-    vtk files must be formated as follows:
-    npart=2  and nstep=5  =>  toto_5_2.*  (starts from zero)    """   
-    rep,fname=os.path.split(fileName)
+    
+    VTK files must be named as follows:
+    npart=2  and nstep=5  =>  toto_5_2.*  (starts from zero)
+    
+    Parameters
+    ----------
+    fileName : STRING
+        mesh files without numbers and extension
+    ext : STRING
+        extension (vtu, vtk, vtr, vti)
+    npart : INT
+        Number of parts to plot together
+    nstep : INT
+        Number of time steps.
+
+    """
+    rep, fname = os.path.split(fileName)
     import xml.dom.minidom
     pvd = xml.dom.minidom.Document()
     pvd_root = pvd.createElementNS("VTK", "VTKFile")
     pvd_root.setAttribute("type", "Collection")
     pvd_root.setAttribute("version", "0.1")
     pvd_root.setAttribute("byte_order", "LittleEndian")
     pvd.appendChild(pvd_root)
```

### Comparing `pyxel-dic-3.0.1/src/pyxel_dic.egg-info/PKG-INFO` & `pyxel-dic-3.0.2/src/pyxel_dic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.0.1
+Version: 3.0.2
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: CeCILL
 Project-URL: Homepage, https://github.com/jcpassieux/pyxel
 Project-URL: Bug Tracker, https://github.com/jcpassieux/pyxel/issues
@@ -19,68 +19,72 @@
 **pyxel** is an open-source Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics application. It is freely available for research and teaching.
 
 <p align="center">
   <img src="https://github.com/jcpassieux/pyxel/blob/master/pyxel.png" width="150" title="hover text">
 </p>
 
 In its present form, it is restricted to 2D-DIC and 3D-DVC. Stereo (SDIC) will be updated later. 
-The gray level conservation problem is written in the physical space. It relies on camera models (which must be calibrated) and on a dedicated quadrature rule in the FE mesh space. Considering front-parallel camera settings, the implemented camera model is a simplified pinhole model (including only 4 parameters 2D: 2 translations, 1 rotation and the focal length and 7 parameters in 3D: focal length, 3 rotations, 3 translations) . More complex camera models (including distorsions) could easily be implemented within this framework (next update?). The library natively includes linear and quadratic triangles, quadrilateral, tetraedral, hexaedral elements. The library also exports the results in different format such that the measurements can be post-processed ether with MatPlotLib or using Paraview.
+The gray level conservation problem is written in the physical space. It relies on camera models (which must be calibrated) and on a dedicated quadrature rule in the FE mesh space. Considering front-parallel camera settings, the implemented camera model is a simplified pinhole model (including only 4 parameters 2D: 2 translations, 1 rotation and the focal length and 7 parameters in 3D: focal length, 3 rotations, 3 translations). More complex camera models (including distorsions) could easily be implemented within this framework (next update?). The library natively includes linear and quadratic triangles, quadrilateral, tetraedral, hexaedral elements. The library also exports the results in different format such that the measurements can be post-processed ether with MatPlotLib or using Paraview.
+
+<p align="center">
+  <img src="https://github.com/jcpassieux/pyxel/blob/master/pyxel-figs.png" height="200" title="hover text">
+</p>
 
 1. SCRIPT FILE
     - pyxel is a library. For each testcase, a script file must be written.
-    - a set of sample scripts named `example_#.py` is provided in the `./data` folder
+    - a set of sample scripts named `example_#.py` is provided in the `./test` folder
      to understand the main functionnalities of the library.
 
 2. ABOUT MESHES
-    - a mesh is entierly defined by two variables:
-        (1) a python dictionnary for the elements (the key is the element type and the value is a numpy array of size NE * NN (NN being the number of nodes of this element type and NE the number of elements). The element type label (according to gmsh numbering). 
+    - A Finite Element mesh is required for the displacement measurement. In pyxel, a mesh is entierly defined by two variables:<br>
+        (1) a python dictionary for the elements (the key is the element type and the value is a numpy array of size NE * NN (NN being the number of nodes of this element type and NE the number of elements). The element type label (according to gmsh numbering). 
         example:
         ```python
 	  e = dict()
        e[3] = np.array([[n0, n1, n2, n3]])
         ```
         (2) a numpy array n for the node coordinates, example:
         ```python
         n = np.array([[x0, y0], [x1, y1], ...])
         ```
     - There is an home made mesher for parallelipedic domains, given the approximate elements size in each direction (see examples). We recommand to use external meshers like, for instance, `gmsh`
-    - To read/write the meshes, we rely on the library `meshio`. 
+    - To read/write the meshes, we use the usefull library `meshio`. 
 
-3. USING THE LIBRARY FOR A 2D ANALYSIS
-    - Open the mesh: 
+3. MINIMAL SAMPLE CODE
+    - to run a simple 2D-DIC analysis:
       ```python
-      m = px.ReadMesh('mesh.msh')
+      f = px.Image('img-0.tif').Load()
+      g = px.Image('img-1.tif').Load()
+      roi = np.array([[ 100,   100], [ 500,  500]])
+      m, cam = px.MeshFromROI(roi, 50, f, typel=3)
+      U, res = px.Correlate(f, g, m, cam)
       ```
-    - Open the image:
-      ```python
-      f = px.Image('image.tif').Load()
-      ```
-    - Connectivity, quadrature, Interpolation:
-      ```python
-      m.Connectivity()
-      m.DICIntegration(cam)
-      ```      
-    - Compute DIC approx. Hessian H and right hand side b:
+    - A multiscale initialization is usually required
       ```python
-      dic = px.DICEngine()
-      H = dic.ComputeLHS(f, m, cam)
-      b, res = dic.ComputeRHS(g, m, cam, U)
+      U = px.MultiscaleInit(f, g, m, cam, scales=[3, 2, 1], l0=30)
       ```
 4. OUTPUT FILES
     - It is possible to post-process the results directly using matplotlib.
-       	but a more convenient way is to use Paraview www.paraview.org 
-    - The library exports VTK files written in `./vtk` directory 
-    - `*.vtu` files are generated, but it is also possible to generate 
-      `*.pvd` files for use in paraview.
-
+      ```python
+      m.PlotContourDispl(U, s=30)
+      ```
+    - but a more convenient way (especially in DVC) is to use Paraview www.paraview.org 
+      ```python
+      m.VTKSol('vtufile', U)
+      ```    
 5. TERM OF USE. 
     This program is a free software: you can redistribute it/or modify it. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY.
     **pyxel** is distributed under the terms of CeCILL which is a french free software license agreement in the spirit of GNU GPL
 
 6. DEPENDANCIES 
     `numpy`, `scipy`, `matplotlib`, `opencv-python`, `scikit-image`, `meshio`, `gmsh`
 
+7. INSTALL
+    - It is possible to clone the git repository, or simply install it using PyPI:
+      ```python
+      pip install pyxel-dic
+      ```
 # References
 
 Jean-Charles Passieux, Robin Bouclier. **Classic and Inverse Compositional Gauss-Newton in Global DIC**. *International Journal for Numerical Methods in Engineering*, 119(6), p.453-468, 2019.
 
 Jean-Charles Passieux. **pyxel, an open-source FE-DIC library**. *Zenodo*. http://doi.org/10.5281/zenodo.4654018
```

