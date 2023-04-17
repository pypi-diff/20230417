# Comparing `tmp/mop_utils-1.7.tar.gz` & `tmp/mop_utils-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mop_utils-1.7.tar", last modified: Fri Mar 31 08:28:20 2023, max compression
+gzip compressed data, was "mop_utils-1.8.tar", last modified: Mon Apr 17 06:46:56 2023, max compression
```

## Comparing `mop_utils-1.7.tar` & `mop_utils-1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 08:28:20.991842 mop_utils-1.7/
--rw-rw-rw-   0        0        0      108 2023-03-31 08:28:20.991842 mop_utils-1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-31 08:28:20.960451 mop_utils-1.7/mop_utils/
--rw-rw-rw-   0        0        0       89 2023-02-13 07:03:05.000000 mop_utils-1.7/mop_utils/__init__.py
--rw-rw-rw-   0        0        0     4181 2023-02-16 02:07:15.000000 mop_utils-1.7/mop_utils/base_model_wrapper.py
--rw-rw-rw-   0        0        0       39 2023-02-16 07:10:11.000000 mop_utils-1.7/mop_utils/constant.py
-drwxrwxrwx   0        0        0        0 2023-03-31 08:28:20.990835 mop_utils-1.7/mop_utils.egg-info/
--rw-rw-rw-   0        0        0      108 2023-03-31 08:28:20.000000 mop_utils-1.7/mop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-03-31 08:28:20.000000 mop_utils-1.7/mop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 08:28:20.000000 mop_utils-1.7/mop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-03-31 08:28:20.000000 mop_utils-1.7/mop_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-31 08:28:20.000000 mop_utils-1.7/mop_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 08:28:20.992846 mop_utils-1.7/setup.cfg
--rw-rw-rw-   0        0        0      345 2023-03-31 08:28:10.000000 mop_utils-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:46:56.875088 mop_utils-1.8/
+-rw-rw-rw-   0        0        0      108 2023-04-17 06:46:56.874088 mop_utils-1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 06:46:56.822549 mop_utils-1.8/mop_utils/
+-rw-rw-rw-   0        0        0       89 2023-02-13 07:03:05.000000 mop_utils-1.8/mop_utils/__init__.py
+-rw-rw-rw-   0        0        0     4529 2023-04-13 06:22:23.000000 mop_utils-1.8/mop_utils/base_model_wrapper.py
+-rw-rw-rw-   0        0        0       39 2023-02-16 07:10:11.000000 mop_utils-1.8/mop_utils/constant.py
+-rw-rw-rw-   0        0        0     6264 2023-03-31 08:33:06.000000 mop_utils-1.8/mop_utils/inference_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:46:56.873089 mop_utils-1.8/mop_utils.egg-info/
+-rw-rw-rw-   0        0        0      108 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 06:46:56.876088 mop_utils-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      345 2023-04-17 06:44:13.000000 mop_utils-1.8/setup.py
```

### Comparing `mop_utils-1.7/mop_utils/base_model_wrapper.py` & `mop_utils-1.8/mop_utils/base_model_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from abc import ABC, abstractmethod
 from typing import List, Dict, Optional, Any
 
 
 class MopInferenceInput:
     def __init__(self, text: Optional[str] = None, image: Optional[str] = None,
                  width: Optional[int] = None,
-                 height: Optional[int] = None) -> None:
+                 height: Optional[int] = None,
+                 images: Optional[List] = None) -> None:
         self.__text__ = text
         self.__image__ = image
         self.__width__ = width
         self.__height__ = height
+        self.__images__ = images
 
     def from_dict(self, input_dict: Dict) -> Any:
         self.__text__ = input_dict.get('text', None)
         self.__image__ = input_dict.get('image', None)
         self.__width__ = input_dict.get('width', None)
         self.__height__ = input_dict.get('height', None)
-        if self.__text__ is None and self.__image__ is None:
+        self.__images__ = input_dict.get('images', None)
+        if self.__text__ is None and self.__image__ is None and self.__images__ is None:
             raise ValueError('Either text or image must be provided')
         return self
 
     def __str__(self) -> str:
         return str(vars(self))
 
     def __repr__(self) -> str:
@@ -54,14 +57,22 @@
     def height(self) -> int:
         return self.__height__
 
     @height.setter
     def height(self, height: int) -> None:
         self.__height__ = height
 
+    @property
+    def images(self) -> str:
+        return self.__images__
+
+    @images.setter
+    def images(self, images: str) -> None:
+        self.__images__ = images
+
 
 class InferenceInput(MopInferenceInput):
     '''this is a subclass to be compatible with old version'''
 
 
 class MopInferenceOutput:
     def __init__(self, confidence_scores: Optional[Dict] = None, predicted_labels: Optional[Dict] = None) -> None:
```

