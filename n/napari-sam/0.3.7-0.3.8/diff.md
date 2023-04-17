# Comparing `tmp/napari-sam-0.3.7.tar.gz` & `tmp/napari-sam-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.7.tar", last modified: Fri Apr 14 17:31:26 2023, max compression
+gzip compressed data, was "napari-sam-0.3.8.tar", last modified: Mon Apr 17 14:11:09 2023, max compression
```

## Comparing `napari-sam-0.3.7.tar` & `napari-sam-0.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.302404 napari-sam-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 17:31:10.000000 napari-sam-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 17:31:10.000000 napari-sam-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-14 17:31:26.302404 napari-sam-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-14 17:31:10.000000 napari-sam-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 17:31:10.000000 napari-sam-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-14 17:31:26.302404 napari-sam-0.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.298404 napari-sam-0.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.302404 napari-sam-0.3.7/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39447 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.302404 napari-sam-0.3.7/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.857162 napari-sam-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 14:10:51.000000 napari-sam-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 14:10:51.000000 napari-sam-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-17 14:11:09.857162 napari-sam-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-17 14:10:51.000000 napari-sam-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 14:10:51.000000 napari-sam-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-17 14:11:09.857162 napari-sam-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.853162 napari-sam-0.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.857162 napari-sam-0.3.8/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39534 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-17 14:10:51.000000 napari-sam-0.3.8/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:11:09.857162 napari-sam-0.3.8/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 14:11:09.000000 napari-sam-0.3.8/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.7/LICENSE` & `napari-sam-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.7/PKG-INFO` & `napari-sam-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.7
+Version: 0.3.8
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.7 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.8 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.7/README.md` & `napari-sam-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.7/setup.cfg` & `napari-sam-0.3.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.7/src/napari_sam/_widget.py` & `napari-sam-0.3.8/src/napari_sam/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,15 @@
         self.sam_model.to(self.device)
         self.sam_predictor = SamPredictor(self.sam_model)
         self.sam_anything_predictor = SamAutomaticMaskGenerator(self.sam_model)
         self.is_model_loaded = True
         self._check_activate_btn()
 
     def _activate(self):
+        self.btn_activate.setEnabled(False)
         if not self.is_active:
             self.is_active = True
             self.btn_activate.setText("Deactivate")
             self.btn_load_model.setEnabled(False)
             self.cb_model_type.setEnabled(False)
             self.cb_image_layers.setEnabled(False)
             self.cb_label_layers.setEnabled(False)
@@ -415,14 +416,15 @@
                 image = image[..., :3]  # Remove a potential alpha channel
                 records = self.sam_anything_predictor.generate(image)
                 masks = np.asarray([record["segmentation"] for record in records])
                 prediction = np.argmax(masks, axis=0)
                 self.label_layer.data = prediction
         else:
             self._deactivate()
+        self.btn_activate.setEnabled(True)
 
     def _deactivate(self):
         self.is_active = False
         self.btn_activate.setText("Activate")
         self.btn_load_model.setEnabled(True)
         self.cb_model_type.setEnabled(True)
         self.cb_image_layers.setEnabled(True)
```

### Comparing `napari-sam-0.3.7/src/napari_sam/utils.py` & `napari-sam-0.3.8/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.7/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.8/src/napari_sam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.7
+Version: 0.3.8
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.7 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.8 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

