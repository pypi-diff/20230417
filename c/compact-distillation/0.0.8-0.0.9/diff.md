# Comparing `tmp/compact-distillation-0.0.8.tar.gz` & `tmp/compact-distillation-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/compact-distillation-0.0.8.tar", last modified: Thu Dec 17 12:08:14 2020, max compression
+gzip compressed data, was "dist/compact-distillation-0.0.9.tar", last modified: Thu Dec 17 12:34:29 2020, max compression
```

## Comparing `compact-distillation-0.0.8.tar` & `compact-distillation-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adines    (1000) adines    (1000)        0 2020-12-17 12:08:14.000000 compact-distillation-0.0.8/
--rw-r--r--   0 adines    (1000) adines    (1000)      653 2020-12-17 12:08:14.000000 compact-distillation-0.0.8/PKG-INFO
--rw-r--r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 compact-distillation-0.0.8/LICENSE.txt
--rw-r--r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 compact-distillation-0.0.8/README.rst
--rw-r--r--   0 adines    (1000) adines    (1000)     8444 2020-12-17 12:08:09.000000 compact-distillation-0.0.8/setup.py
--rw-r--r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 compact-distillation-0.0.8/MANIFEST.in
-drwxr-xr-x   0 adines    (1000) adines    (1000)        0 2020-12-17 12:08:14.000000 compact-distillation-0.0.8/compact_distillation.egg-info/
--rw-r--r--   0 adines    (1000) adines    (1000)      653 2020-12-17 12:08:13.000000 compact-distillation-0.0.8/compact_distillation.egg-info/PKG-INFO
--rw-r--r--   0 adines    (1000) adines    (1000)      739 2020-12-17 12:08:13.000000 compact-distillation-0.0.8/compact_distillation.egg-info/requires.txt
--rw-r--r--   0 adines    (1000) adines    (1000)        1 2020-12-17 12:08:13.000000 compact-distillation-0.0.8/compact_distillation.egg-info/dependency_links.txt
--rw-r--r--   0 adines    (1000) adines    (1000)      350 2020-12-17 12:08:13.000000 compact-distillation-0.0.8/compact_distillation.egg-info/SOURCES.txt
--rw-r--r--   0 adines    (1000) adines    (1000)       13 2020-12-17 12:08:13.000000 compact-distillation-0.0.8/compact_distillation.egg-info/top_level.txt
--rw-r--r--   0 adines    (1000) adines    (1000)       67 2020-12-17 12:08:14.000000 compact-distillation-0.0.8/setup.cfg
-drwxr-xr-x   0 adines    (1000) adines    (1000)        0 2020-12-17 12:08:14.000000 compact-distillation-0.0.8/distillation/
--rw-r--r--   0 adines    (1000) adines    (1000)     8003 2020-12-17 12:08:09.000000 compact-distillation-0.0.8/distillation/semiSupervised.py
--rw-r--r--   0 adines    (1000) adines    (1000)      313 2020-12-16 17:48:57.000000 compact-distillation-0.0.8/distillation/__init__.py
--rw-r--r--   0 adines    (1000) adines    (1000)     9499 2020-12-16 16:37:39.000000 compact-distillation-0.0.8/distillation/utils.py
+drwxr-xr-x   0 adines    (1000) adines    (1000)        0 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/
+-rw-r--r--   0 adines    (1000) adines    (1000)      653 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/PKG-INFO
+-rw-r--r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 compact-distillation-0.0.9/LICENSE.txt
+-rw-r--r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 compact-distillation-0.0.9/README.rst
+-rw-r--r--   0 adines    (1000) adines    (1000)     8444 2020-12-17 12:34:27.000000 compact-distillation-0.0.9/setup.py
+-rw-r--r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 compact-distillation-0.0.9/MANIFEST.in
+drwxr-xr-x   0 adines    (1000) adines    (1000)        0 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/compact_distillation.egg-info/
+-rw-r--r--   0 adines    (1000) adines    (1000)      653 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/compact_distillation.egg-info/PKG-INFO
+-rw-r--r--   0 adines    (1000) adines    (1000)      739 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/compact_distillation.egg-info/requires.txt
+-rw-r--r--   0 adines    (1000) adines    (1000)        1 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/compact_distillation.egg-info/dependency_links.txt
+-rw-r--r--   0 adines    (1000) adines    (1000)      350 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/compact_distillation.egg-info/SOURCES.txt
+-rw-r--r--   0 adines    (1000) adines    (1000)       13 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/compact_distillation.egg-info/top_level.txt
+-rw-r--r--   0 adines    (1000) adines    (1000)       67 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/setup.cfg
+drwxr-xr-x   0 adines    (1000) adines    (1000)        0 2020-12-17 12:34:29.000000 compact-distillation-0.0.9/distillation/
+-rw-r--r--   0 adines    (1000) adines    (1000)     8027 2020-12-17 12:34:27.000000 compact-distillation-0.0.9/distillation/semiSupervised.py
+-rw-r--r--   0 adines    (1000) adines    (1000)      313 2020-12-16 17:48:57.000000 compact-distillation-0.0.9/distillation/__init__.py
+-rw-r--r--   0 adines    (1000) adines    (1000)     9499 2020-12-16 16:37:39.000000 compact-distillation-0.0.9/distillation/utils.py
```

### Comparing `compact-distillation-0.0.8/PKG-INFO` & `compact-distillation-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: compact-distillation
-Version: 0.0.8
+Version: 0.0.9
 Summary: API that provides methods to construct deep compact classification models using semi-supervised methods.
 Home-page: https://github.com/adines/SOTA-tinyML
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: classification,compact networks,deep learning,semi-supervised
```

### Comparing `compact-distillation-0.0.8/LICENSE.txt` & `compact-distillation-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compact-distillation-0.0.8/README.rst` & `compact-distillation-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `compact-distillation-0.0.8/setup.py` & `compact-distillation-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.8',  # Required
+    version='0.0.9',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='API that provides methods to construct deep compact classification models using semi-supervised methods.',  # Required
 
     # This is an optional longer description of your project that represents
```

### Comparing `compact-distillation-0.0.8/compact_distillation.egg-info/PKG-INFO` & `compact-distillation-0.0.9/compact_distillation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: compact-distillation
-Version: 0.0.8
+Version: 0.0.9
 Summary: API that provides methods to construct deep compact classification models using semi-supervised methods.
 Home-page: https://github.com/adines/SOTA-tinyML
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: classification,compact networks,deep learning,semi-supervised
```

### Comparing `compact-distillation-0.0.8/compact_distillation.egg-info/requires.txt` & `compact-distillation-0.0.9/compact_distillation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `compact-distillation-0.0.8/distillation/semiSupervised.py` & `compact-distillation-0.0.9/distillation/semiSupervised.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         save = SaveModelCallback(monitor='accuracy', fname='model-'+baseModel)
         early = EarlyStoppingCallback(monitor='accuracy', patience=8)
         learn = Learner(dls, bModel, splitter=default_split, metrics=[accuracy], cbs=[early, save])
 
         # Train base learner
         learn.fine_tune(50, freeze_epochs=2)
         learn.save(baseModel)
-        shutil.copy('models'+os.sep+'model-'+baseModel+'.pth',outputPath)
+        shutil.copy(path+os.sep+'models'+os.sep+'model-'+baseModel+'.pth',outputPath)
 
         # supervised method
         plainSupervised(path,pathUnlabelled,learn,confidence)
 
         # Load new images
         dls2 = ImageDataLoaders.from_folder(path+'_tmp', batch_tfms=aug_transforms(), item_tfms=Resize(size), bs=bs)
 
@@ -42,15 +42,15 @@
         save2 = SaveModelCallback(monitor='accuracy', fname='model-' + targetModel)
         early2 = EarlyStoppingCallback(monitor='accuracy', patience=8)
         learn2 = Learner(dls2, tModel, splitter=default_split, metrics=[accuracy], cbs=[early2, save2])
 
         # Train base learner
         learn2.fine_tune(50, freeze_epochs=2)
         learn2.save(outputPath+os.sep+targetModel)
-        shutil.copy('models' + os.sep + 'model-' + targetModel + '.pth', outputPath)
+        shutil.copy(path+os.sep+'models' + os.sep + 'model-' + targetModel + '.pth', outputPath)
         shutil.rmtree(path+'_tmp')
 
 
 
 def dataDistillation(baseModel, targetModel, transforms, path, pathUnlabelled, outputPath, bs=32, size=224, confidence=0.8):
     if not testNameModel(baseModel):
         print("The base model selected is not valid")
```

### Comparing `compact-distillation-0.0.8/distillation/utils.py` & `compact-distillation-0.0.9/distillation/utils.py`

 * *Files identical despite different names*

