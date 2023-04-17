# Comparing `tmp/robotathome-1.1.4.tar.gz` & `tmp/robotathome-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotathome-1.1.4.tar", last modified: Mon Apr 17 18:50:23 2023, max compression
+gzip compressed data, was "robotathome-1.1.5.tar", last modified: Mon Apr 17 19:32:41 2023, max compression
```

## Comparing `robotathome-1.1.4.tar` & `robotathome-1.1.5.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.384211 robotathome-1.1.4/
--rw-r--r--   0 goyo      (1000) goyo      (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.4/LICENSE
--rw-rw-r--   0 goyo      (1000) goyo      (1000)    12789 2023-04-17 18:50:23.380211 robotathome-1.1.4/PKG-INFO
--rw-r--r--   0 goyo      (1000) goyo      (1000)    12065 2023-04-09 20:16:05.000000 robotathome-1.1.4/README.md
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.344212 robotathome-1.1.4/notebooks/
--rw-r--r--   0 goyo      (1000) goyo      (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.4/notebooks/05-Google-colab-drive.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.4/notebooks/10-Download-and-install.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.4/notebooks/20-Before-starting-the-logging-system.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.4/notebooks/30-Getting-started-Framework-data.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.4/notebooks/40-Captured-data.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.4/notebooks/50-RGBD-observations.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.4/notebooks/60-Lsrscan-observations.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.4/notebooks/70-Scenes.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.4/notebooks/80-Characterized-observations.ipynb
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.348212 robotathome-1.1.4/rh_schema_diagram/
--rw-r--r--   0 goyo      (1000) goyo      (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.4/rh_schema_diagram/rh_schema_brief.pdf
--rw-r--r--   0 goyo      (1000) goyo      (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.4/rh_schema_diagram/rh_schema_full.pdf
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.356212 robotathome-1.1.4/robotathome/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      473 2023-04-17 18:47:30.000000 robotathome-1.1.4/robotathome/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.4/robotathome/_version.py
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.364212 robotathome-1.1.4/robotathome/core/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.4/robotathome/core/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.4/robotathome/core/df.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    46165 2023-04-16 13:07:22.000000 robotathome-1.1.4/robotathome/core/reader.py
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.372212 robotathome-1.1.4/robotathome/cv/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.4/robotathome/cv/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.4/robotathome/cv/_greetings.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.4/robotathome/cv/gluoncv.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.4/robotathome/cv/opencv.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.4/robotathome/helpers.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.4/robotathome/log.py
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.360212 robotathome-1.1.4/robotathome.egg-info/
--rw-r--r--   0 goyo      (1000) goyo      (1000)    12789 2023-04-17 18:50:23.000000 robotathome-1.1.4/robotathome.egg-info/PKG-INFO
--rw-r--r--   0 goyo      (1000) goyo      (1000)     1103 2023-04-17 18:50:23.000000 robotathome-1.1.4/robotathome.egg-info/SOURCES.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)        1 2023-04-17 18:50:23.000000 robotathome-1.1.4/robotathome.egg-info/dependency_links.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)      226 2023-04-17 18:50:23.000000 robotathome-1.1.4/robotathome.egg-info/requires.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)       16 2023-04-17 18:50:23.000000 robotathome-1.1.4/robotathome.egg-info/top_level.txt
--rw-rw-r--   0 goyo      (1000) goyo      (1000)       38 2023-04-17 18:50:23.384211 robotathome-1.1.4/setup.cfg
--rw-r--r--   0 goyo      (1000) goyo      (1000)     3306 2023-04-09 11:17:02.000000 robotathome-1.1.4/setup.py
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.372212 robotathome-1.1.4/src/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      473 2023-04-17 18:47:30.000000 robotathome-1.1.4/src/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.4/src/_version.py
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.376212 robotathome-1.1.4/src/core/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.4/src/core/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.4/src/core/df.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    46165 2023-04-16 13:07:22.000000 robotathome-1.1.4/src/core/reader.py
-drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 18:50:23.380211 robotathome-1.1.4/src/cv/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.4/src/cv/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.4/src/cv/_greetings.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.4/src/cv/gluoncv.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.4/src/cv/opencv.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.4/src/helpers.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.4/src/log.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.5/LICENSE
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    12789 2023-04-17 19:32:41.494285 robotathome-1.1.5/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12065 2023-04-09 20:16:48.000000 robotathome-1.1.5/README.md
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/notebooks/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.5/notebooks/05-Google-colab-drive.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.5/notebooks/10-Download-and-install.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   774981 2023-04-17 18:44:46.000000 robotathome-1.1.5/notebooks/100-Iterating-over-RGBD-images.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12082 2023-04-17 18:45:03.000000 robotathome-1.1.5/notebooks/110-Concatenating-images-from-multiple-cameras.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    37648 2023-04-17 18:38:58.000000 robotathome-1.1.5/notebooks/120-Making-a-video.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    26523 2023-04-17 18:45:32.000000 robotathome-1.1.5/notebooks/130-Processing-images-with-YOLO.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.5/notebooks/20-Before-starting-the-logging-system.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.5/notebooks/30-Getting-started-Framework-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.5/notebooks/40-Captured-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.5/notebooks/50-RGBD-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.5/notebooks/60-Lsrscan-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.5/notebooks/70-Scenes.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.5/notebooks/80-Characterized-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13884 2023-04-17 06:32:58.000000 robotathome-1.1.5/notebooks/90-The-config-file.ipynb
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/rh_schema_diagram/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.5/rh_schema_diagram/rh_schema_brief.pdf
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.5/rh_schema_diagram/rh_schema_full.pdf
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/robotathome/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      473 2023-04-17 19:29:55.000000 robotathome-1.1.5/robotathome/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.5/robotathome/_version.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/robotathome/core/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.5/robotathome/core/__init__.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.5/robotathome/core/df.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    46165 2023-04-16 16:14:10.000000 robotathome-1.1.5/robotathome/core/reader.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/robotathome/cv/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.5/robotathome/cv/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.5/robotathome/cv/_greetings.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.5/robotathome/cv/gluoncv.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.5/robotathome/cv/opencv.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.5/robotathome/helpers.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.5/robotathome/log.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/robotathome.egg-info/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12789 2023-04-17 19:32:41.000000 robotathome-1.1.5/robotathome.egg-info/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1331 2023-04-17 19:32:41.000000 robotathome-1.1.5/robotathome.egg-info/SOURCES.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)        1 2023-04-17 19:32:41.000000 robotathome-1.1.5/robotathome.egg-info/dependency_links.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      226 2023-04-17 19:32:41.000000 robotathome-1.1.5/robotathome.egg-info/requires.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)       16 2023-04-17 19:32:41.000000 robotathome-1.1.5/robotathome.egg-info/top_level.txt
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)       38 2023-04-17 19:32:41.494285 robotathome-1.1.5/setup.cfg
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     3599 2023-04-17 19:27:59.000000 robotathome-1.1.5/setup.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/src/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      473 2023-04-17 19:29:55.000000 robotathome-1.1.5/src/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.5/src/_version.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/src/core/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.5/src/core/__init__.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.5/src/core/df.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    46165 2023-04-16 16:14:10.000000 robotathome-1.1.5/src/core/reader.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-17 19:32:41.494285 robotathome-1.1.5/src/cv/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.5/src/cv/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.5/src/cv/_greetings.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.5/src/cv/gluoncv.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.5/src/cv/opencv.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.5/src/helpers.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.5/src/log.py
```

### Comparing `robotathome-1.1.4/LICENSE` & `robotathome-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/PKG-INFO` & `robotathome-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.4
+Version: 1.1.5
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
```

### Comparing `robotathome-1.1.4/README.md` & `robotathome-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/05-Google-colab-drive.ipynb` & `robotathome-1.1.5/notebooks/05-Google-colab-drive.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/10-Download-and-install.ipynb` & `robotathome-1.1.5/notebooks/10-Download-and-install.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/20-Before-starting-the-logging-system.ipynb` & `robotathome-1.1.5/notebooks/20-Before-starting-the-logging-system.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/30-Getting-started-Framework-data.ipynb` & `robotathome-1.1.5/notebooks/30-Getting-started-Framework-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/40-Captured-data.ipynb` & `robotathome-1.1.5/notebooks/40-Captured-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/50-RGBD-observations.ipynb` & `robotathome-1.1.5/notebooks/50-RGBD-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/60-Lsrscan-observations.ipynb` & `robotathome-1.1.5/notebooks/60-Lsrscan-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/70-Scenes.ipynb` & `robotathome-1.1.5/notebooks/70-Scenes.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/notebooks/80-Characterized-observations.ipynb` & `robotathome-1.1.5/notebooks/80-Characterized-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/rh_schema_diagram/rh_schema_brief.pdf` & `robotathome-1.1.5/rh_schema_diagram/rh_schema_brief.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/rh_schema_diagram/rh_schema_full.pdf` & `robotathome-1.1.5/rh_schema_diagram/rh_schema_full.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome/_version.py` & `robotathome-1.1.5/robotathome/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome/core/df.py` & `robotathome-1.1.5/robotathome/core/df.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome/core/reader.py` & `robotathome-1.1.5/robotathome/core/reader.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome/cv/gluoncv.py` & `robotathome-1.1.5/robotathome/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome/cv/opencv.py` & `robotathome-1.1.5/robotathome/cv/opencv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome/helpers.py` & `robotathome-1.1.5/robotathome/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome/log.py` & `robotathome-1.1.5/robotathome/log.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/robotathome.egg-info/PKG-INFO` & `robotathome-1.1.5/robotathome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.4
+Version: 1.1.5
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
```

### Comparing `robotathome-1.1.4/robotathome.egg-info/SOURCES.txt` & `robotathome-1.1.5/robotathome.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 LICENSE
 README.md
 setup.py
 notebooks/05-Google-colab-drive.ipynb
 notebooks/10-Download-and-install.ipynb
+notebooks/100-Iterating-over-RGBD-images.ipynb
+notebooks/110-Concatenating-images-from-multiple-cameras.ipynb
+notebooks/120-Making-a-video.ipynb
+notebooks/130-Processing-images-with-YOLO.ipynb
 notebooks/20-Before-starting-the-logging-system.ipynb
 notebooks/30-Getting-started-Framework-data.ipynb
 notebooks/40-Captured-data.ipynb
 notebooks/50-RGBD-observations.ipynb
 notebooks/60-Lsrscan-observations.ipynb
 notebooks/70-Scenes.ipynb
 notebooks/80-Characterized-observations.ipynb
+notebooks/90-The-config-file.ipynb
 rh_schema_diagram/rh_schema_brief.pdf
 rh_schema_diagram/rh_schema_full.pdf
 robotathome/__init__.py
 robotathome/_version.py
 robotathome/helpers.py
 robotathome/log.py
 robotathome.egg-info/PKG-INFO
```

### Comparing `robotathome-1.1.4/setup.py` & `robotathome-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,15 +93,20 @@
           'notebooks/10-Download-and-install.ipynb',
           'notebooks/20-Before-starting-the-logging-system.ipynb',
           'notebooks/30-Getting-started-Framework-data.ipynb',
           'notebooks/40-Captured-data.ipynb',
           'notebooks/50-RGBD-observations.ipynb',
           'notebooks/60-Lsrscan-observations.ipynb',
           'notebooks/70-Scenes.ipynb',
-          'notebooks/80-Characterized-observations.ipynb']
+          'notebooks/80-Characterized-observations.ipynb',
+          'notebooks/90-The-config-file.ipynb',
+          'notebooks/100-Iterating-over-RGBD-images.ipynb',
+          'notebooks/110-Concatenating-images-from-multiple-cameras.ipynb',
+          'notebooks/120-Making-a-video.ipynb',
+          'notebooks/130-Processing-images-with-YOLO.ipynb']
          )
     ],
     # sql files from robotathome package will be included in the installation package
     # located at ~/<anaconda-dir>/envs/<env-name>/lib/<python>/site-packages/robotathome
     package_data={'robotathome': ['*.sql']},
 
 )
```

### Comparing `robotathome-1.1.4/src/_version.py` & `robotathome-1.1.5/src/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/src/core/df.py` & `robotathome-1.1.5/src/core/df.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/src/core/reader.py` & `robotathome-1.1.5/src/core/reader.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/src/cv/gluoncv.py` & `robotathome-1.1.5/src/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/src/cv/opencv.py` & `robotathome-1.1.5/src/cv/opencv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/src/helpers.py` & `robotathome-1.1.5/src/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.4/src/log.py` & `robotathome-1.1.5/src/log.py`

 * *Files identical despite different names*

