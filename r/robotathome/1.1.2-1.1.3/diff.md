# Comparing `tmp/robotathome-1.1.2.tar.gz` & `tmp/robotathome-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotathome-1.1.2.tar", last modified: Sun Apr  9 20:21:36 2023, max compression
+gzip compressed data, was "robotathome-1.1.3.tar", last modified: Mon Apr 17 07:54:35 2023, max compression
```

## Comparing `robotathome-1.1.2.tar` & `robotathome-1.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.2/LICENSE
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    12789 2023-04-09 20:21:36.207288 robotathome-1.1.2/PKG-INFO
--rw-r--r--   0 lightman  (1000) lightman  (1000)    12065 2023-04-09 20:16:48.000000 robotathome-1.1.2/README.md
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/notebooks/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.2/notebooks/05-Google-colab-drive.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.2/notebooks/10-Download-and-install.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.2/notebooks/20-Before-starting-the-logging-system.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.2/notebooks/30-Getting-started-Framework-data.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.2/notebooks/40-Captured-data.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.2/notebooks/50-RGBD-observations.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.2/notebooks/60-Lsrscan-observations.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.2/notebooks/70-Scenes.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.2/notebooks/80-Characterized-observations.ipynb
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/rh_schema_diagram/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.2/rh_schema_diagram/rh_schema_brief.pdf
--rw-r--r--   0 lightman  (1000) lightman  (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.2/rh_schema_diagram/rh_schema_full.pdf
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/robotathome/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      473 2023-04-09 20:19:37.000000 robotathome-1.1.2/robotathome/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.2/robotathome/_version.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/robotathome/core/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.2/robotathome/core/__init__.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.2/robotathome/core/df.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    46199 2023-04-09 10:57:14.000000 robotathome-1.1.2/robotathome/core/reader.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/robotathome/cv/
--rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.2/robotathome/cv/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.2/robotathome/cv/_greetings.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.2/robotathome/cv/gluoncv.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.2/robotathome/cv/opencv.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.2/robotathome/helpers.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.2/robotathome/log.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/robotathome.egg-info/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    12789 2023-04-09 20:21:36.000000 robotathome-1.1.2/robotathome.egg-info/PKG-INFO
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1103 2023-04-09 20:21:36.000000 robotathome-1.1.2/robotathome.egg-info/SOURCES.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)        1 2023-04-09 20:21:36.000000 robotathome-1.1.2/robotathome.egg-info/dependency_links.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)      226 2023-04-09 20:21:36.000000 robotathome-1.1.2/robotathome.egg-info/requires.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)       16 2023-04-09 20:21:36.000000 robotathome-1.1.2/robotathome.egg-info/top_level.txt
--rw-rw-r--   0 lightman  (1000) lightman  (1000)       38 2023-04-09 20:21:36.207288 robotathome-1.1.2/setup.cfg
--rw-rw-r--   0 lightman  (1000) lightman  (1000)     3306 2023-04-09 11:24:37.000000 robotathome-1.1.2/setup.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/src/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      473 2023-04-09 20:19:37.000000 robotathome-1.1.2/src/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.2/src/_version.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/src/core/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.2/src/core/__init__.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.2/src/core/df.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    46199 2023-04-09 10:57:14.000000 robotathome-1.1.2/src/core/reader.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 20:21:36.207288 robotathome-1.1.2/src/cv/
--rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.2/src/cv/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.2/src/cv/_greetings.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.2/src/cv/gluoncv.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.2/src/cv/opencv.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.2/src/helpers.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.2/src/log.py
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.378348 robotathome-1.1.3/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.3/LICENSE
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)    12791 2023-04-17 07:54:35.378348 robotathome-1.1.3/PKG-INFO
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    12065 2023-04-09 20:16:05.000000 robotathome-1.1.3/README.md
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.374348 robotathome-1.1.3/notebooks/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.3/notebooks/05-Google-colab-drive.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.3/notebooks/10-Download-and-install.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.3/notebooks/20-Before-starting-the-logging-system.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.3/notebooks/30-Getting-started-Framework-data.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.3/notebooks/40-Captured-data.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.3/notebooks/50-RGBD-observations.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.3/notebooks/60-Lsrscan-observations.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.3/notebooks/70-Scenes.ipynb
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.3/notebooks/80-Characterized-observations.ipynb
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.374348 robotathome-1.1.3/rh_schema_diagram/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.3/rh_schema_diagram/rh_schema_brief.pdf
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.3/rh_schema_diagram/rh_schema_full.pdf
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.374348 robotathome-1.1.3/robotathome/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      473 2023-04-16 16:14:35.000000 robotathome-1.1.3/robotathome/__init__.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.3/robotathome/_version.py
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.378348 robotathome-1.1.3/robotathome/core/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.3/robotathome/core/__init__.py
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.3/robotathome/core/df.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    46165 2023-04-16 13:07:22.000000 robotathome-1.1.3/robotathome/core/reader.py
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.378348 robotathome-1.1.3/robotathome/cv/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.3/robotathome/cv/__init__.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.3/robotathome/cv/_greetings.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.3/robotathome/cv/gluoncv.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.3/robotathome/cv/opencv.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.3/robotathome/helpers.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.3/robotathome/log.py
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.378348 robotathome-1.1.3/robotathome.egg-info/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    12791 2023-04-17 07:54:34.000000 robotathome-1.1.3/robotathome.egg-info/PKG-INFO
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     1103 2023-04-17 07:54:35.000000 robotathome-1.1.3/robotathome.egg-info/SOURCES.txt
+-rw-r--r--   0 goyo      (1000) goyo      (1000)        1 2023-04-17 07:54:34.000000 robotathome-1.1.3/robotathome.egg-info/dependency_links.txt
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      226 2023-04-17 07:54:35.000000 robotathome-1.1.3/robotathome.egg-info/requires.txt
+-rw-r--r--   0 goyo      (1000) goyo      (1000)       16 2023-04-17 07:54:35.000000 robotathome-1.1.3/robotathome.egg-info/top_level.txt
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)       38 2023-04-17 07:54:35.378348 robotathome-1.1.3/setup.cfg
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     3306 2023-04-09 11:17:02.000000 robotathome-1.1.3/setup.py
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.378348 robotathome-1.1.3/src/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      473 2023-04-16 16:14:35.000000 robotathome-1.1.3/src/__init__.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.3/src/_version.py
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.378348 robotathome-1.1.3/src/core/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.3/src/core/__init__.py
+-rw-rw-r--   0 goyo      (1000) goyo      (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.3/src/core/df.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    46165 2023-04-16 13:07:22.000000 robotathome-1.1.3/src/core/reader.py
+drwxrwxr-x   0 goyo      (1000) goyo      (1000)        0 2023-04-17 07:54:35.378348 robotathome-1.1.3/src/cv/
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.3/src/cv/__init__.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.3/src/cv/_greetings.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.3/src/cv/gluoncv.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.3/src/cv/opencv.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.3/src/helpers.py
+-rw-r--r--   0 goyo      (1000) goyo      (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.3/src/log.py
```

### Comparing `robotathome-1.1.2/LICENSE` & `robotathome-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/PKG-INFO` & `robotathome-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.2
+Version: 1.1.3
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
@@ -326,7 +326,9 @@
     rh.uncompress('~/Downloads/Robot@Home2_files.tgz', '~/WORKSPACE/files')
 else:
     print('Integrity of Robot@Home2_files.tgz is compromised, please download again')
 ```
 
 
 
+
+
```

### Comparing `robotathome-1.1.2/README.md` & `robotathome-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/05-Google-colab-drive.ipynb` & `robotathome-1.1.3/notebooks/05-Google-colab-drive.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/10-Download-and-install.ipynb` & `robotathome-1.1.3/notebooks/10-Download-and-install.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/20-Before-starting-the-logging-system.ipynb` & `robotathome-1.1.3/notebooks/20-Before-starting-the-logging-system.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/30-Getting-started-Framework-data.ipynb` & `robotathome-1.1.3/notebooks/30-Getting-started-Framework-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/40-Captured-data.ipynb` & `robotathome-1.1.3/notebooks/40-Captured-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/50-RGBD-observations.ipynb` & `robotathome-1.1.3/notebooks/50-RGBD-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/60-Lsrscan-observations.ipynb` & `robotathome-1.1.3/notebooks/60-Lsrscan-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/70-Scenes.ipynb` & `robotathome-1.1.3/notebooks/70-Scenes.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/notebooks/80-Characterized-observations.ipynb` & `robotathome-1.1.3/notebooks/80-Characterized-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/rh_schema_diagram/rh_schema_brief.pdf` & `robotathome-1.1.3/rh_schema_diagram/rh_schema_brief.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/rh_schema_diagram/rh_schema_full.pdf` & `robotathome-1.1.3/rh_schema_diagram/rh_schema_full.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/robotathome/_version.py` & `robotathome-1.1.3/robotathome/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/robotathome/core/df.py` & `robotathome-1.1.3/robotathome/core/df.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/robotathome/core/reader.py` & `robotathome-1.1.3/robotathome/core/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,27 +63,27 @@
             db_filename: file name of the database.
 
         Raises:
             Exception: If the object cannot be instantiated (usually because
                 a database connection could not be done).
 
         Note 1: The default folder structure is:
-            R@H2-2.0.1
-                 │    └── files
-                 │        ├── rgbd
-                 │        └── scene
-                 └─────── rh.db
+         └─── R@H2-2.0.3
+              └── files
+              │   ├── rgbd
+              │   └── scene
+              └── rh.db
 
         Note 2: Example of .rh file
             # This is a default configuration file
             [PATHS]
-            rh_path     = $HOME/R@H2-2.0.1
-            rgbd_path   = ~/R@H2-2.0.1/files/rgbd
+            rh_path     = $HOME/R@H2-2.0.3
+            rgbd_path   = ~/R@H2-2.0.3/files/rgbd
             scene_path  = ~/R@H2-2.0.1/files/scene
-            wspc_path   = ~/R@H2-2.0.1
+            wspc_path   = ~/R@H2-2.0.3
             db_filename = rh.db
 
             Paths strings can content environmental variables such as $HOME or
             a tilde prefix.
         """
         self.__con = None
         self.__aliases = {}
```

### Comparing `robotathome-1.1.2/robotathome/cv/gluoncv.py` & `robotathome-1.1.3/robotathome/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/robotathome/cv/opencv.py` & `robotathome-1.1.3/robotathome/cv/opencv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/robotathome/helpers.py` & `robotathome-1.1.3/robotathome/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/robotathome/log.py` & `robotathome-1.1.3/robotathome/log.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/robotathome.egg-info/PKG-INFO` & `robotathome-1.1.3/robotathome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.2
+Version: 1.1.3
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
@@ -326,7 +326,9 @@
     rh.uncompress('~/Downloads/Robot@Home2_files.tgz', '~/WORKSPACE/files')
 else:
     print('Integrity of Robot@Home2_files.tgz is compromised, please download again')
 ```
 
 
 
+
+
```

### Comparing `robotathome-1.1.2/robotathome.egg-info/SOURCES.txt` & `robotathome-1.1.3/robotathome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/setup.py` & `robotathome-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/src/_version.py` & `robotathome-1.1.3/src/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/src/core/df.py` & `robotathome-1.1.3/src/core/df.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/src/core/reader.py` & `robotathome-1.1.3/src/core/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,27 +63,27 @@
             db_filename: file name of the database.
 
         Raises:
             Exception: If the object cannot be instantiated (usually because
                 a database connection could not be done).
 
         Note 1: The default folder structure is:
-            R@H2-2.0.1
-                 │    └── files
-                 │        ├── rgbd
-                 │        └── scene
-                 └─────── rh.db
+         └─── R@H2-2.0.3
+              └── files
+              │   ├── rgbd
+              │   └── scene
+              └── rh.db
 
         Note 2: Example of .rh file
             # This is a default configuration file
             [PATHS]
-            rh_path     = $HOME/R@H2-2.0.1
-            rgbd_path   = ~/R@H2-2.0.1/files/rgbd
+            rh_path     = $HOME/R@H2-2.0.3
+            rgbd_path   = ~/R@H2-2.0.3/files/rgbd
             scene_path  = ~/R@H2-2.0.1/files/scene
-            wspc_path   = ~/R@H2-2.0.1
+            wspc_path   = ~/R@H2-2.0.3
             db_filename = rh.db
 
             Paths strings can content environmental variables such as $HOME or
             a tilde prefix.
         """
         self.__con = None
         self.__aliases = {}
```

### Comparing `robotathome-1.1.2/src/cv/gluoncv.py` & `robotathome-1.1.3/src/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/src/cv/opencv.py` & `robotathome-1.1.3/src/cv/opencv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/src/helpers.py` & `robotathome-1.1.3/src/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.2/src/log.py` & `robotathome-1.1.3/src/log.py`

 * *Files identical despite different names*

