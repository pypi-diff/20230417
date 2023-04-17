# Comparing `tmp/TCFile-2023.4.tar.gz` & `tmp/TCFile-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCFile-2023.4.tar", last modified: Tue Apr  4 15:05:53 2023, max compression
+gzip compressed data, was "TCFile-2023.4.1.tar", last modified: Mon Apr 17 02:00:25 2023, max compression
```

## Comparing `TCFile-2023.4.tar` & `TCFile-2023.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       42 2023-04-04 15:05:45.921389 TCFile-2023.4/.gitattributes
--rw-r--r--   0        0        0      689 2023-04-04 15:05:45.921389 TCFile-2023.4/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      241 2023-04-04 15:05:45.921389 TCFile-2023.4/.gitignore
--rw-r--r--   0        0        0     1069 2023-04-04 15:05:45.921389 TCFile-2023.4/LICENSE
--rw-r--r--   0        0        0      819 2023-04-04 15:05:45.921389 TCFile-2023.4/README.md
--rw-r--r--   0        0        0      929 2023-04-04 15:05:45.921389 TCFile-2023.4/TCFile-tests/TCFhandler.py
--rw-r--r--   0        0        0      134 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile-tests/test_snapshot.TCF
--rw-r--r--   0        0        0     3406 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile/TCFhandler/TCFile.py
--rw-r--r--   0        0        0       26 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile/TCFhandler/__init__.py
--rw-r--r--   0        0        0       25 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile/__init__.py
--rw-r--r--   0        0        0     1956 2023-04-04 15:05:45.997389 TCFile-2023.4/docs/structure_TCF.md
--rw-r--r--   0        0        0     1049 2023-04-04 15:05:45.997389 TCFile-2023.4/pyproject.toml
--rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 TCFile-2023.4/PKG-INFO
+-rw-r--r--   0        0        0       42 2023-04-17 02:00:15.316127 TCFile-2023.4.1/.gitattributes
+-rw-r--r--   0        0        0      689 2023-04-17 02:00:15.316127 TCFile-2023.4.1/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      241 2023-04-17 02:00:15.316127 TCFile-2023.4.1/.gitignore
+-rw-r--r--   0        0        0     1069 2023-04-17 02:00:15.316127 TCFile-2023.4.1/LICENSE
+-rw-r--r--   0        0        0      856 2023-04-17 02:00:15.316127 TCFile-2023.4.1/README.md
+-rw-r--r--   0        0        0     3594 2023-04-17 02:00:15.316127 TCFile-2023.4.1/TCFile/TCFile_class.py
+-rw-r--r--   0        0        0       27 2023-04-17 02:00:15.316127 TCFile-2023.4.1/TCFile/__init__.py
+-rw-r--r--   0        0        0     1956 2023-04-17 02:00:15.316127 TCFile-2023.4.1/docs/structure_TCF.md
+-rw-r--r--   0        0        0      807 2023-04-17 02:00:15.316127 TCFile-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-17 02:00:15.316127 TCFile-2023.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      134 2023-04-17 02:00:15.420127 TCFile-2023.4.1/tests/sample.TCF
+-rw-r--r--   0        0        0      822 2023-04-17 02:00:15.420127 TCFile-2023.4.1/tests/test_TCFile_class.py
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 TCFile-2023.4.1/PKG-INFO
```

### Comparing `TCFile-2023.4/.github/workflows/deploy.yml` & `TCFile-2023.4.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `TCFile-2023.4/LICENSE` & `TCFile-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TCFile-2023.4/README.md` & `TCFile-2023.4.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,49 @@
-## TCFile python package
+# TCFile python package
 
-Basic image processing tools of tomocube data.
+A basic image processing tool of tomocube data.
 
 ## Installation
 
-After downloading the repository, execute the following command in the repository;
-
 ```bash
-pip install .
+pip install TCFile
 ```
 
-## Note
-
-It is not for normal users, and API is not fixed. 
-Please use this package with full understanding.
-Any suggestions and comments are welcome! 
-
 ## Use case
 
 ```python
 
-from ..TCFile import *
+from TCFile import TCFile
 
-tcfile = TCFile('test.TCF','3D') # for now, it only read 3D RI data
+tcfile = TCFile('test.TCF','3D') # ready for return 3D RI images
 print(f"number of snapshots : {len(tcfile)}")
 
-## Usage 1: handling a data for each snapshot
+## Usage 1: handling each snapshots (or data)
 data = tcfile[0]
 print(f"shape of data : {data.shape}")
 # or
 for data in tcfile:
     # do some operations on the data ...
     pass
 ```
 
-## Test (for development and contribution)
+## TODO
+
+- [ ] fluorescence data reader
+- [ ] TCFile compressor/decompressor for portability
+- [ ] rich documentation
+- [ ] rigorous tests
+- [ ] TCFile writer ?
+- [ ] TCFile converter ?
+
+Any suggestions and comments are welcome!
+
+## Test
 
 ```bash
-conda install PIL h5py numpy
-pytest TCFile-tests/TCFhandler.py
+# install this package in editable mode
+git clone https://github.com/ehgus/TCFile.git
+cd TCFile
+pip install -e .
+# execute pytest
+pytest
 ```
```

### Comparing `TCFile-2023.4/TCFile/TCFhandler/TCFile.py` & `TCFile-2023.4.1/TCFile/TCFile_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import h5py
 
 class TCFile(Sequence):
     '''
     interface class to TCF files.
     This class returns data as if list containg multiple data.
     Preview of the data is stored in attributes.
-    * Note: It can read 3D, 2DMIP, BF.
+    * Note: It can read 3D, 2DMIP, BF. 
 
     Attributes
     ----------
     length : int
         time series length of the TCF file
     dataShape : numpy.array[int]
         shape of single shot data
@@ -68,15 +68,17 @@
         self.imgtype = imgtype
     
     def __getitem__ (self, key:int) -> np.ndarray:
         '''
         Return
         ------
         data : numpy.ndarray[uint8]
-            raw data of refractive index mutliplided by 1e4.
+            return a single image.
+            When choosing 2DMIP or 3D data as a output, it returns refractive index map,
+            and a RGB image for bright field image.
 
         Raises
         ------
         TypeError
             If key is not int
         IndexError
             If key is out of bound
@@ -97,9 +99,12 @@
             data /= 1e4
         elif 'BF' == self.imgtype:
             data = Image.fromarray(data, mode = 'RGB')
 
         return data
 
     def __len__(self):
+        '''
+        Return the number of images available. 
+        '''
         return self.length
```

### Comparing `TCFile-2023.4/docs/structure_TCF.md` & `TCFile-2023.4.1/docs/structure_TCF.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## structure of TCF
+# structure of TCF
 
 ```bash
 HDF5.File
 ├─ CreateDate
 ├─ DataID
 ├─ Description
 ├─ DeviceHost
@@ -78,8 +78,8 @@
    │  ├─ Wavelength
    │  ├─ ZP
    │  ├─ ZP2
    │  └─ ZP3
    └─ Imaging
       ├─ CameraGain
       └─ CameraShutter
-```
+```
```

### Comparing `TCFile-2023.4/pyproject.toml` & `TCFile-2023.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "TCFile"
-version = "2023.4"
+version = "2023.4.1"
 description = "Python package for handling TCF data. It works with Tomcube data"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.7,<4"
 license = {file = "LICENSE"}
 authors = [{name = "Dohyeon Lee", email = "dleh428@kaist.ac.kr"}]
+maintainers = [{name = "Dohyeon Lee", email = "dleh428@kaist.ac.kr"}]
 
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Operating System :: Microsoft :: Windows",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Scientific/Engineering :: Image Processing"
+    "Topic :: Scientific/Engineering"
 ]
 
 dependencies = [
-    "numpy>=1.18.5",
-    "scipy>=1.7.0",
-    "scikit-image>0.18.2",
-    "h5py>=3.2.0",
-    "multimethod>=1.4",
-    "matplotlib>=3.4.0",
-    "opencv-python>=4.5.0",
-    "pytest>=6.2"
+    "numpy>=1.18.5,<2",
+    "h5py>=3.2.0,<4",
+    "pillow>=9.5.0,<10"
 ]
 
-[tool.setuptools.packages.find]
-where = ["TCFile"]
-exclude = ["tests"]
+[project.urls]
+repository = "https://github.com/ehgus/TCFile"
+
+[tool.flit.sdist]
+include = ["TCFile/"]
```

