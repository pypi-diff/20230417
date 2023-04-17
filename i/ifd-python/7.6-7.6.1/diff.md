# Comparing `tmp/ifd_python-7.6.tar.gz` & `tmp/ifd_python-7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.6.tar", max compression
+gzip compressed data, was "ifd_python-7.6.1.tar", max compression
```

## Comparing `ifd_python-7.6.tar` & `ifd_python-7.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.6/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2045 2023-04-14 12:09:37.448293 ifd_python-7.6/ifd/entities/Image.py
--rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6/ifd/entities/Modele.py
--rw-r--r--   0        0        0      666 2023-04-14 14:33:26.310964 ifd_python-7.6/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/repository/__init__.py
--rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.6/ifd/spec.py
--rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 14:33:55.090755 ifd_python-7.6/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      327 2023-04-14 14:34:13.294623 ifd_python-7.6/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.6/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.1/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.1/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2045 2023-04-14 12:09:37.448293 ifd_python-7.6.1/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      666 2023-04-14 14:33:26.310964 ifd_python-7.6.1/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.1/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.1/ifd/spec.py
+-rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.1/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:38:02.412258 ifd_python-7.6.1/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-17 07:38:11.740163 ifd_python-7.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.1/PKG-INFO
```

### Comparing `ifd_python-7.6/LICENSE` & `ifd_python-7.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/README.md` & `ifd_python-7.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.6.1/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/Classification.py` & `ifd_python-7.6.1/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/Detection.py` & `ifd_python-7.6.1/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/Image.py` & `ifd_python-7.6.1/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/LogResult.py` & `ifd_python-7.6.1/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/OCR.py` & `ifd_python-7.6.1/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.6.1/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/entities/bbox.py` & `ifd_python-7.6.1/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.6.1/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/ifd/tools.py` & `ifd_python-7.6.1/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6/PKG-INFO` & `ifd_python-7.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.6
+Version: 7.6.1
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

