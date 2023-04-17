# Comparing `tmp/granny-1.3.0.tar.gz` & `tmp/granny-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/granny-1.3.0.tar", last modified: Wed Mar  1 16:09:40 2023, max compression
+gzip compressed data, was "dist/granny-1.4.0.tar", last modified: Mon Apr 17 21:27:08 2023, max compression
```

## Comparing `granny-1.3.0.tar` & `granny-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-03-01 16:09:40.000000 granny-1.3.0/
-drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-03-01 16:09:39.000000 granny-1.3.0/GRANNY/
--rw-------   0 nhan       (501) staff       (20)    36200 2023-03-01 13:43:39.000000 granny-1.3.0/GRANNY/GRANNY.py
--rw-r--r--   0 nhan       (501) staff       (20)      391 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/GRANNY_config.py
-drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-03-01 16:09:40.000000 granny-1.3.0/GRANNY/Mask_RCNN/
--rw-r--r--   0 nhan       (501) staff       (20)        0 2022-12-26 01:39:07.000000 granny-1.3.0/GRANNY/Mask_RCNN/__init__.py
--rw-r--r--   0 nhan       (501) staff       (20)    20789 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/Mask_RCNN/coco.py
--rw-r--r--   0 nhan       (501) staff       (20)     6304 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/Mask_RCNN/config.py
--rw-r--r--   0 nhan       (501) staff       (20)   111990 2022-09-06 07:05:29.000000 granny-1.3.0/GRANNY/Mask_RCNN/model.py
--rw-r--r--   0 nhan       (501) staff       (20)     6859 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/Mask_RCNN/parallel_model.py
--rw-r--r--   0 nhan       (501) staff       (20)     7392 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/Mask_RCNN/shapes.py
--rw-r--r--   0 nhan       (501) staff       (20)    27365 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/Mask_RCNN/utils.py
--rw-r--r--   0 nhan       (501) staff       (20)    16530 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/Mask_RCNN/visualize.py
--rw-r--r--   0 nhan       (501) staff       (20)        0 2022-08-24 06:53:51.000000 granny-1.3.0/GRANNY/__init__.py
--rw-r--r--   0 nhan       (501) staff       (20)     1623 2023-03-01 15:23:41.000000 granny-1.3.0/GRANNY/command.py
--rw-r--r--   0 nhan       (501) staff       (20)      143 2022-11-17 19:17:09.000000 granny-1.3.0/GRANNY/test_perf.py
--rw-r--r--   0 nhan       (501) staff       (20)    35147 2023-01-20 10:38:46.000000 granny-1.3.0/LICENSE.txt
--rw-r--r--   0 nhan       (501) staff       (20)      399 2023-03-01 16:09:40.000000 granny-1.3.0/PKG-INFO
--rw-r--r--   0 nhan       (501) staff       (20)     2034 2023-02-04 05:01:52.000000 granny-1.3.0/README.md
-drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-03-01 16:09:40.000000 granny-1.3.0/granny.egg-info/
--rw-r--r--   0 nhan       (501) staff       (20)      399 2023-03-01 16:09:39.000000 granny-1.3.0/granny.egg-info/PKG-INFO
--rw-r--r--   0 nhan       (501) staff       (20)      685 2023-03-01 16:09:39.000000 granny-1.3.0/granny.egg-info/SOURCES.txt
--rw-r--r--   0 nhan       (501) staff       (20)        1 2023-03-01 16:09:39.000000 granny-1.3.0/granny.egg-info/dependency_links.txt
--rw-r--r--   0 nhan       (501) staff       (20)       47 2023-03-01 16:09:39.000000 granny-1.3.0/granny.egg-info/entry_points.txt
-drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-03-01 16:09:40.000000 granny-1.3.0/granny.egg-info/input_data/
--rw-r--r--   0 nhan       (501) staff       (20)  2230076 2022-11-17 19:17:23.000000 granny-1.3.0/granny.egg-info/input_data/4m_TC-1(3)-2-A.JPG
--rw-r--r--   0 nhan       (501) staff       (20)  2683668 2022-11-17 19:13:36.000000 granny-1.3.0/granny.egg-info/input_data/6moPos_TC-1(3)-2-A.JPG
-drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-03-01 16:09:40.000000 granny-1.3.0/granny.egg-info/input_data/test2_1/
--rw-r--r--   0 nhan       (501) staff       (20)  2230076 2022-11-17 19:20:07.000000 granny-1.3.0/granny.egg-info/input_data/test2_1/4m_TC-1(3)-2-A.JPG
--rw-r--r--   0 nhan       (501) staff       (20)      135 2023-03-01 16:09:39.000000 granny-1.3.0/granny.egg-info/requires.txt
--rw-r--r--   0 nhan       (501) staff       (20)        7 2023-03-01 16:09:39.000000 granny-1.3.0/granny.egg-info/top_level.txt
--rw-r--r--   0 nhan       (501) staff       (20)       38 2023-03-01 16:09:40.000000 granny-1.3.0/setup.cfg
--rw-r--r--   0 nhan       (501) staff       (20)      779 2023-03-01 16:08:55.000000 granny-1.3.0/setup.py
+drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-04-17 21:27:08.000000 granny-1.4.0/
+drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-04-17 21:27:08.000000 granny-1.4.0/GRANNY/
+-rw-r--r--   0 nhan       (501) staff       (20)    37208 2023-04-17 17:52:57.000000 granny-1.4.0/GRANNY/GRANNY.py
+-rw-r--r--   0 nhan       (501) staff       (20)      391 2022-08-24 06:53:51.000000 granny-1.4.0/GRANNY/GRANNY_config.py
+drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-04-17 21:27:08.000000 granny-1.4.0/GRANNY/Mask_RCNN/
+-rw-r--r--   0 nhan       (501) staff       (20)        0 2022-12-26 01:39:07.000000 granny-1.4.0/GRANNY/Mask_RCNN/__init__.py
+-rw-r--r--   0 nhan       (501) staff       (20)    20789 2022-08-24 06:53:51.000000 granny-1.4.0/GRANNY/Mask_RCNN/coco.py
+-rw-r--r--   0 nhan       (501) staff       (20)     6304 2022-08-24 06:53:51.000000 granny-1.4.0/GRANNY/Mask_RCNN/config.py
+-rw-r--r--   0 nhan       (501) staff       (20)   111990 2022-09-06 07:05:29.000000 granny-1.4.0/GRANNY/Mask_RCNN/model.py
+-rw-r--r--   0 nhan       (501) staff       (20)     6859 2022-08-24 06:53:51.000000 granny-1.4.0/GRANNY/Mask_RCNN/parallel_model.py
+-rw-r--r--   0 nhan       (501) staff       (20)     7392 2022-08-24 06:53:51.000000 granny-1.4.0/GRANNY/Mask_RCNN/shapes.py
+-rw-r--r--   0 nhan       (501) staff       (20)    27482 2023-04-11 18:26:14.000000 granny-1.4.0/GRANNY/Mask_RCNN/utils.py
+-rw-r--r--   0 nhan       (501) staff       (20)    16530 2022-08-24 06:53:51.000000 granny-1.4.0/GRANNY/Mask_RCNN/visualize.py
+-rw-r--r--   0 nhan       (501) staff       (20)        0 2022-08-24 06:53:51.000000 granny-1.4.0/GRANNY/__init__.py
+-rw-r--r--   0 nhan       (501) staff       (20)     1625 2023-04-17 17:52:57.000000 granny-1.4.0/GRANNY/command.py
+-rw-r--r--   0 nhan       (501) staff       (20)      143 2022-11-17 19:17:09.000000 granny-1.4.0/GRANNY/test_perf.py
+-rw-r--r--   0 nhan       (501) staff       (20)    35147 2023-01-20 10:38:46.000000 granny-1.4.0/LICENSE.txt
+-rw-r--r--   0 nhan       (501) staff       (20)      399 2023-04-17 21:27:08.000000 granny-1.4.0/PKG-INFO
+-rw-r--r--   0 nhan       (501) staff       (20)     3868 2023-04-12 19:48:47.000000 granny-1.4.0/README.md
+drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/
+-rw-r--r--   0 nhan       (501) staff       (20)      399 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/PKG-INFO
+-rw-r--r--   0 nhan       (501) staff       (20)      685 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/SOURCES.txt
+-rw-r--r--   0 nhan       (501) staff       (20)        1 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/dependency_links.txt
+-rw-r--r--   0 nhan       (501) staff       (20)       47 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/entry_points.txt
+drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/input_data/
+-rw-r--r--   0 nhan       (501) staff       (20)  2230076 2022-11-17 19:17:23.000000 granny-1.4.0/granny.egg-info/input_data/4m_TC-1(3)-2-A.JPG
+-rw-r--r--   0 nhan       (501) staff       (20)  2683668 2022-11-17 19:13:36.000000 granny-1.4.0/granny.egg-info/input_data/6moPos_TC-1(3)-2-A.JPG
+drwxr-xr-x   0 nhan       (501) staff       (20)        0 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/input_data/test2_1/
+-rw-r--r--   0 nhan       (501) staff       (20)  2230076 2022-11-17 19:20:07.000000 granny-1.4.0/granny.egg-info/input_data/test2_1/4m_TC-1(3)-2-A.JPG
+-rw-r--r--   0 nhan       (501) staff       (20)      143 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/requires.txt
+-rw-r--r--   0 nhan       (501) staff       (20)        7 2023-04-17 21:27:08.000000 granny-1.4.0/granny.egg-info/top_level.txt
+-rw-r--r--   0 nhan       (501) staff       (20)       38 2023-04-17 21:27:08.000000 granny-1.4.0/setup.cfg
+-rw-r--r--   0 nhan       (501) staff       (20)      787 2023-04-17 21:24:25.000000 granny-1.4.0/setup.py
```

### Comparing `granny-1.3.0/GRANNY/GRANNY.py` & `granny-1.4.0/GRANNY/GRANNY.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,55 +6,58 @@
 import shutil
 import pathlib
 import tensorflow as tf
 import pandas as pd
 import numpy as np
 import os
 import warnings
+import json
+import sys
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 pd.options.mode.chained_assignment = None
 tf.autograph.set_verbosity(3)
 tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
 
 
 class GrannyBaseClass(object):
     """ 
         Implementation for semantic segmentation of instances and superficial scald rating in "Granny Smith" apples
     """
 
-    def __init__(self, action = "", fname = "", num_instances = 1, verbose = 0 ):
+    def __init__(self, action = "", fname = "", num_instances = 1, verbose = 0):
         # current directory
         self.ROOT_DIR = pathlib.Path(__file__).parent.resolve()
 
         # logs
         self.MODEL_DIR = os.path.join(os.path.curdir, "logs")
 
         # new directory of the rotated input images
         self.NEW_DATA_DIR = "input_data" + os.sep
 
         # directory of the pretrained we
         self.PRETRAINED_MODEL = os.path.join(
-            self.ROOT_DIR, "mask_rcnn_balloon.h5")
-
-        # initialize default parameters
-        self.VERBOSE = verbose
-        self.ACTION = action
-        self.FILE_NAME = fname
-        self.FOLDER_NAME = fname
-        self.OLD_DATA_DIR = fname
-        self.NUM_INSTANCES = num_instances
-
+            self.ROOT_DIR, "mask_rcnn_starch_cross_section.h5")
+        
         # accepted file extensions
         self.FILE_EXTENSION = (
             ".JPG", ".JPG".lower(),
             ".PNG", ".PNG".lower(),
             ".JPEG", ".JPEG".lower(),
             ".TIFF", ".TIFF".lower(),
         )
 
+        # initialize default parameters
+        self.VERBOSE = verbose
+        self.ACTION = action
+        self.FILE_NAME = fname if fname.endswith(self.FILE_EXTENSION) else ""
+        self.FOLDER_NAME = fname if not fname.endswith(self.FILE_EXTENSION) else os.sep.join(fname.split(os.sep)[0:-1])
+        self.FOLDER_NAME = self.FOLDER_NAME + os.sep if not self.FOLDER_NAME.endswith(os.sep) else self.FOLDER_NAME
+        self.OLD_DATA_DIR = self.FOLDER_NAME
+        self.INPUT_FNAME = fname
+        self.NUM_INSTANCES = num_instances
         self.RESULT_DIR = "results" + os.sep
 
         # location where masked apple trays will be saved
         self.FULLMASK_DIR = self.RESULT_DIR + "full_masked_images" + os.sep
 
         # location where segmented/individual instances will be saved
         self.SEGMENTED_DIR = self.RESULT_DIR + "segmented_images" + os.sep
@@ -96,16 +99,16 @@
                         (list) file_name: all files inside data_dir
         """
         file_name = []
         folder_name = []
 
         # if data_dir is a file
         if data_dir.endswith(self.FILE_EXTENSION):
-            file_name.append(data_dir.split(os.sep)[-1])
-            folder_name.append(data_dir.replace(data_dir.split(os.sep)[-1], os.path.curdir))
+            file_name.append(data_dir)
+            folder_name.append(data_dir.replace(data_dir.split(os.sep)[-1], ""))
             return folder_name, file_name
 
         # list all folders and files in data_dir
         for root, dirs, files in os.walk(data_dir):
 
             # append the files to the list
             for file in files:
@@ -133,17 +136,19 @@
         for ext in self.FILE_EXTENSION:
             fname = re.sub(ext, "", fname)
         return fname
 
 
 class GrannyExtractInstances(GrannyBaseClass): 
     def __init__(self, action, fname, num_instances, verbose):
+        num_instances = 18 if num_instances == None else num_instances
+        verbose = 1 if verbose == 1 else 0
         super(GrannyExtractInstances, self).__init__(action, fname, num_instances, verbose)
 
-    def load_model(self, verbose=1):
+    def load_model(self, verbose=0):
         """ 
                 Load pretrained model, download if the model does not exist
 
                 Args: 
                         (int) verbose: specify 0 to turn off model display
 
                 Returns: 
@@ -226,15 +231,15 @@
                 rows += 1
         df["rows"].iloc[-1] = rows
 
         # sort apple/pear in each row using their x-center coordinates
         # if the first row has 5 apples/pears
         df_list = []
         if len(df[df["rows"] == 1]) == 5:
-            apple_id = 18
+            apple_id = self.NUM_INSTANCES
             for i in range(1, 5):
                 dfx = df[df["rows"] == i].sort_values(
                     "xcenter", ascending=False, inplace=False, ignore_index=True)
                 for id in range(0, len(dfx)):
                     dfx["apple_id"].iloc[id] = apple_id
                     apple_id -= 1
                 df_list.append(dfx)
@@ -267,15 +272,15 @@
         # convert to DataFrame
         df = pd.DataFrame(box)
 
         # label each column
         df.columns = ["y1", "x1", "y2", "x2"]
 
         # take first 18 rows (18 apples)
-        df = df.iloc[0:18]
+        df = df.iloc[0:self.NUM_INSTANCES]
 
         # calculate centers for each apples
         df["ycenter"] = ((df["y1"]+df["y2"])/2).astype(int)
         df["xcenter"] = ((df["x1"]+df["x2"])/2).astype(int)
 
         # initialize columns
         df["rows"] = 0
@@ -360,15 +365,15 @@
                         None
         """
         try:
             # load model
             model = self.load_model(verbose=self.VERBOSE)
 
             # list all folders and files
-            data_dirs, file_names = self.list_all(self.OLD_DATA_DIR)
+            data_dirs, file_names = self.list_all(self.INPUT_FNAME)
 
             # check and create a new "results" directory to store the results
             for data_dir in data_dirs:
                 self.check_path(data_dir.replace(
                     self.OLD_DATA_DIR, self.FULLMASK_DIR))
                 self.check_path(data_dir.replace(
                     self.OLD_DATA_DIR, self.SEGMENTED_DIR))
@@ -396,62 +401,42 @@
                 mask, box = self.create_fullmask_image(
                     model=model,
                     im=img,
                     fname=file_name.replace(
                         self.OLD_DATA_DIR, self.FULLMASK_DIR)
                 )
 
-                # when NUM_INSTANCES = 18 (18 apples/pears) or NUM_INSTANCES not specified
-                if self.NUM_INSTANCES == 1 or self.NUM_INSTANCES == 18:
-
-                    # sort all instances using the convention in demo/18_apples_tray_convention.pdf
-                    sorted_ar = self.sort_instances(box)
+                # if there are more instances than NUM_INSTANCES
+                if self.NUM_INSTANCES > len(box):
+                    print(
+                        f"Only {len(box)} instances is detected.")
+                    box = box
 
-                    # extract the images
-                    self.extract_image(sorted_arr=sorted_ar, mask=mask, im=img, fname=file_name.replace(
-                        self.OLD_DATA_DIR, self.SEGMENTED_DIR))
-
-                # when NUM_INSTANCES != 18
+                # if there are less instances than NUM_INSTANCES
                 else:
+                    box = box[0:self.NUM_INSTANCES, :]
+
+                # sort all instances using the convention in demo/18_apples_tray_convention.pdf
+                sorted_ar = self.sort_instances(box)
 
-                    # the instances will not be sorted
-                    warnings.warn(
-                        "this is not a regular tray, the instances will not be sorted.")
-
-                    # if there are more instances than NUM_INSTANCES
-                    if self.NUM_INSTANCES > len(box):
-                        print(
-                            f"Only {len(box)} instances is detected.")
-                        box = box
-
-                    # if there are less instances than NUM_INSTANCES
-                    else:
-                        box = box[0:self.NUM_INSTANCES, :]
-
-                    # concatenate the location array information
-                    box = np.array(np.concatenate((box, np.array(
-                        np.arange(1, len(box) + 1, dtype=int), ndmin=2).T, np.array(
-                        np.arange(0, len(box), dtype=int), ndmin=2).T), axis=1))
-
-                    # increase the dimensions to 2D
-                    box = box[:, np.newaxis, :]
-
-                    # extract the images
-                    self.extract_image(sorted_arr=box, mask=mask, im=img, fname=file_name.replace(
-                        self.OLD_DATA_DIR, self.SEGMENTED_DIR))
+                # extract the images
+                self.extract_image(sorted_arr=sorted_ar, mask=mask, im=img, fname=file_name.replace(
+                    self.OLD_DATA_DIR, self.SEGMENTED_DIR))
 
                 # for debugging purpose
                 print(
-                    f"\t- {name} extracted. Check \"results/\" for output. - \n")
+                    f"\t- {name} done. Check \"results/\" for output. - \n")
         except FileNotFoundError:
             print(f"\t- Folder/File Does Not Exist -")
 
 
 class GrannySuperficialScald(GrannyBaseClass): 
     def __init__(self, action, fname, num_instances, verbose):
+        num_instances = 1 if num_instances == None else num_instances
+        verbose = 0 if verbose == None else 1
         super(GrannySuperficialScald, self).__init__(action, fname, num_instances, verbose)
 
     def remove_purple(self, img):
         """
                 Remove the surrounding purple from the individual apples using YCrCb color space. 
                 This function helps remove the unwanted regions for more precise calculation of the scald area. 
 
@@ -705,43 +690,42 @@
                         w.writelines("\n")
                     print(f"\t- Done. Check \"results/\" for output. - \n")
             except FileNotFoundError:
                 print(f"\t- Folder/File Does Not Exist or Wrong NUM_INSTANCES Values.-")
 
 
 class GrannyPeelColor(GrannyBaseClass): 
-    def __init__(self, action, fname, num_instances, verbose): 
+    def __init__(self, action, fname, num_instances, rgb = 0, verbose = 0): 
         super(GrannyPeelColor, self).__init__(action, fname, num_instances, verbose)
         self.MEAN_VALUES_L = [50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50]
         self.MEAN_VALUES_A = [
-            -22.73535185450301,
-            -35.856673734593976,
-            -14.839191848288477,
-            -38.33945889256972,
-            -38.35401900977177,
-            -25.183705217005663,
-            -37.46455193845067,
-            -18.57975296251061,
-            -20.153556829155015,
-            -28.66620337913712,
-            -15.422998269835011
+            -37.431935692331884,
+            -38.293360653725784,
+            -35.82872139214024,
+            -28.65441389649031,
+            -20.132066117704923,
+            -25.194905219214903,
+            -22.755906449379097,
+            -18.56182827236788,
+            -15.454144111751553,
+            -14.824498082241526
         ]
         self.MEAN_VALUES_B = [
-            84.36038598038662,
-            72.21634388774689,
-            91.21422051166374,
-            60.41978876347979,
-            60.40667779362334,
-            81.7513027496333,
-            58.068541555881474,
-            86.95338287223824,
-            78.30049344632643,
-            77.42875637928557,
-            92.37148315325989
+            58.106332924284644,
+            60.495161874167344,
+            72.19300566542566,
+            77.41069574523988,
+            78.2944440629932,
+            81.71376220418327,
+            84.27577503150619,
+            86.90495332877367,
+            92.36555388970727,
+            91.26334782696254,
         ]
+        self.rgb = 0 
 
     def remove_purple(self, img):
         """
                 Remove the surrounding purple from the individual apples using YCrCb color space. 
                 This function helps remove the unwanted regions for more precise calculation of the scald area. 
 
                 Args: 
@@ -828,15 +812,15 @@
         mean_l = np.sum(lab_img[:,:,0])/np.count_nonzero(threshold_1) * 100/255
         mean_a = np.sum(lab_img[:,:,1]*threshold_2)/np.count_nonzero(threshold_2) - 128
         mean_b = np.sum(lab_img[:,:,2]*threshold_3)/np.count_nonzero(threshold_3) - 128
 
         # normalize by shifting point in the spherical coordinates
         radius = np.sqrt(mean_l**2 + mean_a**2 + mean_b**2)
         scaled_l = 50
-        scaled_a = np.sign(mean_a)*np.sqrt((radius**2 - scaled_l**2)/(1 + (mean_b/mean_a)**2))
+        scaled_a = np.sign(mean_a)*np.sqrt(np.abs(radius**2 - scaled_l**2)/(1 + (mean_b/mean_a)**2))
         scaled_b = np.sign(mean_b)*mean_b/mean_a*scaled_a
 
         return scaled_l, scaled_a, scaled_b
     
     def calculate_bin_distance(self, color_list, method = "Euclidean"): 
         """
             Calculate the Euclidean distance from normalized image's LAB to each bin color. 
@@ -847,22 +831,33 @@
 
             Returns: 
                     
         """
         bin_num = 0 
         dist = 0
         if method == "Euclidean": 
-            dist = np.sqrt((color_list[1] - np.array(self.MEAN_VALUES_A))**2, (color_list[2] - np.array(self.MEAN_VALUES_B))**2) 
-            bin_num = np.argmin(dist)
-        
+            dist_a = color_list[1] - np.array(self.MEAN_VALUES_A)
+            dist_b = color_list[2] - np.array(self.MEAN_VALUES_B)
+            dist = np.sqrt((dist_a/np.linalg.norm(dist_a))**2 + (dist_b/np.linalg.norm(dist_b))**2) 
+            bin_num = np.argmin(dist) + 1
         return bin_num, dist
     
+    def get_distance_from_rgb(self, img): 
+        r = np.mean(img[:,:,0])
+        g = np.mean(img[:,:,1])
+        b = np.mean(img[:,:,2])
+        return 
+    
     def sort_peel_color(self): 
+        """ 
+
+        """
         # create "results" directory to save the results
         self.check_path(self.BIN_COLOR)
+
         if self.NUM_INSTANCES == 1: 
             try:
                 # create "results" directory to save the results
                 self.check_path(self.RESULT_DIR)
 
                 # read image 
                 file_name = self.FILE_NAME
@@ -874,43 +869,56 @@
 
                 # image smoothing
                 img = cv2.GaussianBlur(img, (3, 3), sigmaX=0, sigmaY=0)
 
                 # get image values
                 l, a, b = self.get_green_yellow_values(img)
 
+                if self.rgb == "":
                 # calculate distance to each bin 
-                bin_num, distances = self.calculate_bin_distance([l, a, b])
+                    bin_num, distance = self.calculate_bin_distance([l, a, b])
+                else: 
+                    distance = self.get_distance_from_rgb(img)
 
                 # convert to string
                 string_dist = ""
-                for dist in distances: 
-                    string_dist += dist + ","
+                for dist in distance: 
+                    string_dist += str(dist) + ","
+
+                color_info = {}
+                color_info["bin_num"] = bin_num.tolist()
+                color_info["distances"] = distance.tolist()
+                color_info["LAB_pixels"] = [l, a, b]
 
                 # save the scores to results/rating.csv
                 with open(self.BIN_COLOR + os.sep + "peel_colors.csv", "w") as w:
-                    w.writelines(f"{self.clean_name(file_name)},{bin_num},{string_dist}")
+                    w.writelines(f"{self.clean_name(file_name.split(os.sep)[-1])},{bin_num},{string_dist},{l},{a},{b}")
                     w.writelines("\n")
+
+                with open(self.BIN_COLOR + os.sep + "peel_colors.json", "w") as w:
+                    json.dump({file_name.split(os.sep)[-1]:color_info}, w)
                 print(f"\t- Done. Check \"results/\" for output. - \n")
 
-            except:
+            except FileNotFoundError:
                 print(f"\t- Folder/File Does Not Exist or Wrong NUM_INSTANCES Values. -")
         
         else: 
             try: 
                 # list all files and folders in the folder
                 folders, files = self.list_all(self.FOLDER_NAME)
 
                 # create "results" directory to save the results
                 for folder in folders:
                     self.check_path(folder.replace(
                         self.FOLDER_NAME, self.BIN_COLOR))
-                
+
                 bin_nums = []
                 distances = []
+                channels_values = []
+                color_infos = {} 
                 for file_name in files: 
                     img = skimage.io.imread(file_name)
 
                     # remove surrounding purple
                     img = self.remove_purple(img)
                     nopurple_img = img 
 
@@ -922,25 +930,36 @@
 
                     # calculate distance to each bin 
                     bin_num, distance = self.calculate_bin_distance([l, a, b])
 
                     # convert to string
                     string_dist = ""
                     for dist in distance: 
-                        string_dist += dist + ","
+                        string_dist += str(dist) + ","
                     
                     bin_nums.append(bin_num)
                     distances.append(string_dist)
+                    channels_values.append(str(l) + "," + str(a) + "," + str(b))
+                    color_info = {}
+                    color_info["bin_num"] = bin_num.tolist()
+                    color_info["distances"] = distance.tolist()
+                    color_info["LAB_pixels"] = [l, a, b]
+                    image_data = {}
+                    image_data[file_name.split(os.sep)[-1]] = color_info
+                    color_infos.update(image_data)
 
                 with open(self.BIN_COLOR + os.sep + "peel_colors.csv", "w") as w: 
-                    for i in len(bin_nums): 
-                        w.writelines(f"{self.clean_name(files[i])},{bin_nums[i]},{string_dist[i]}")
+                    for i in range(len(bin_nums)): 
+                        w.writelines(f"{self.clean_name(files[i].split(os.sep)[-1])},{bin_nums[i]},{distances[i]}{channels_values[i]}")
                         w.writelines("\n")
-                    print(f"\t- Done. Check \"results/\" for output. - \n")
-            except: 
+
+                with open(self.BIN_COLOR + os.sep + "peel_colors.json", "w") as w: 
+                    json.dump(color_infos, w)
+                print(f"\t- Done. Check \"results/\" for output. - \n")
+            except FileNotFoundError: 
                 print(f"\t- Folder/File Does Not Exist or Wrong NUM_INSTANCES Values. -")
 
 
 class GrannyStarchIndex(GrannyBaseClass): 
     def __init__(self, action, fname, num_instances, verbose): 
         super(GrannyBaseClass).__init__(self, action, fname, num_instances, verbose)
```

### Comparing `granny-1.3.0/GRANNY/Mask_RCNN/coco.py` & `granny-1.4.0/GRANNY/Mask_RCNN/coco.py`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/GRANNY/Mask_RCNN/config.py` & `granny-1.4.0/GRANNY/Mask_RCNN/config.py`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/GRANNY/Mask_RCNN/model.py` & `granny-1.4.0/GRANNY/Mask_RCNN/model.py`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/GRANNY/Mask_RCNN/parallel_model.py` & `granny-1.4.0/GRANNY/Mask_RCNN/parallel_model.py`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/GRANNY/Mask_RCNN/shapes.py` & `granny-1.4.0/GRANNY/Mask_RCNN/shapes.py`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/GRANNY/Mask_RCNN/utils.py` & `granny-1.4.0/GRANNY/Mask_RCNN/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 import shutil
 import PIL
 from PIL import Image
 tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
 
 # URL from which to download the latest COCO trained weights
 # COCO_MODEL_URL = "https://github.com/matterport/Mask_RCNN/releases/download/v2.0/mask_rcnn_coco.h5"
-COCO_MODEL_URL = "https://github.com/matterport/Mask_RCNN/releases/download/v2.1/mask_rcnn_balloon.h5"
+# COCO_MODEL_URL = "https://github.com/matterport/Mask_RCNN/releases/download/v2.1/mask_rcnn_balloon.h5"
+COCO_MODEL_URL = "https://github.com/SystemsGenetics/granny/raw/master/GRANNY/mask_rcnn_starch_cross_section.h5"
+
+
 
 ############################################################
 #  Bounding Boxes
 ############################################################
 
 def extract_bboxes(mask):
     """Compute bounding boxes from masks.
```

### Comparing `granny-1.3.0/GRANNY/Mask_RCNN/visualize.py` & `granny-1.4.0/GRANNY/Mask_RCNN/visualize.py`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/GRANNY/command.py` & `granny-1.4.0/GRANNY/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     required = True, help = "Required. Specify an action to perform.")
 
     parser.add_argument("-d", "--image_dir", dest = "dir", type = str, nargs = "?", 
     required = True, help = "Required. Specify a directory or a file.")
 
     parser.add_argument("-n", "--num_instances", dest = "num_instances", type = int, nargs = "?", 
     required = False, help = "Optional, default is 18. The number of instances on each image.")
-    
+
     parser.add_argument("-v", "--verbose", dest = "verbose", type = int, nargs = "?", 
     default = 0, required = False, help = "Optional. Specify 1 to turn on model display.")
-    
+
     args = parser.parse_args()
 
     if args.action == "extract": 
         granny.GrannyExtractInstances(args.action, args.dir, args.num_instances, args.verbose).mask_extract_image()
     elif args.action == "scald": 
         granny.GrannySuperficialScald(args.action, args.dir, args.num_instances, args.verbose).rate_binarize_image()
-    elif args.action == "pear": 
-        granny.GrannyPeelColor(args.action, args.dir, args.num_instances, args.verbose).sort_peel_color()
+    elif args.action == "peel": 
+        granny.GrannyPeelColor(args.action, args.dir, args.num_instances, args.rgb, args.verbose).sort_peel_color()
     elif args.action == "starch": 
         granny.GrannyStarchIndex(args.action, args.dir, args.num_instances, args.verbose).main()
     else: 
         print("\t- Invalid Action. -")
```

### Comparing `granny-1.3.0/LICENSE.txt` & `granny-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/granny.egg-info/SOURCES.txt` & `granny-1.4.0/granny.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/granny.egg-info/input_data/4m_TC-1(3)-2-A.JPG` & `granny-1.4.0/granny.egg-info/input_data/4m_TC-1(3)-2-A.JPG`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/granny.egg-info/input_data/6moPos_TC-1(3)-2-A.JPG` & `granny-1.4.0/granny.egg-info/input_data/6moPos_TC-1(3)-2-A.JPG`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/granny.egg-info/input_data/test2_1/4m_TC-1(3)-2-A.JPG` & `granny-1.4.0/granny.egg-info/input_data/test2_1/4m_TC-1(3)-2-A.JPG`

 * *Files identical despite different names*

### Comparing `granny-1.3.0/setup.py` & `granny-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 requirements = """pandas
 ipython
 ipykernel
 numpy
 opencv-python
 matplotlib>=3.5
 h5py<3.0.0
-scikit-image
+scikit-image==0.16.2
 tensorflow<=1.15
 pillow
 protobuf<=3.20
 keras==2.3
 """.split()
 
 
 setuptools.setup(
     name='granny',
     packages=setuptools.find_packages(),
     url="https://github.com/SystemsGenetics/granny",
-    version='1.3.0',
+    version='1.4.0',
     description='GRANNY is an implementation of Mask-RCNN and image processing techniques,\
         developed by the Ficklin Research Program, to rate disorder severity in "Granny Smith" apple.',
     author='Nhan H. Nguyen',
     license='GNU General Public License v3.0',
     python_requires='<3.8',
     install_requires=[
         requirements,
```

