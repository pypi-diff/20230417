# Comparing `tmp/Alpha_Rabbit-1.3.6.tar.gz` & `tmp/Alpha_Rabbit-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.3.6.tar", last modified: Mon Apr 17 05:59:42 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.3.7.tar", last modified: Mon Apr 17 06:11:23 2023, max compression
```

## Comparing `Alpha_Rabbit-1.3.6.tar` & `Alpha_Rabbit-1.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 05:59:42.711609 Alpha_Rabbit-1.3.6/
-drwxrwxrwx   0        0        0        0 2023-04-17 05:59:42.704625 Alpha_Rabbit-1.3.6/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    25090 2023-04-17 05:59:09.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22640 2023-03-24 01:41:23.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-04-17 05:59:42.710406 Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-04-17 05:59:42.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-04-17 05:59:42.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 05:59:42.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-17 05:59:42.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 05:59:42.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-04-17 05:59:42.712650 Alpha_Rabbit-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.6/README.md
--rw-rw-rw-   0        0        0       85 2023-04-17 05:59:42.712650 Alpha_Rabbit-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-04-17 05:59:38.000000 Alpha_Rabbit-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:11:23.640563 Alpha_Rabbit-1.3.7/
+drwxrwxrwx   0        0        0        0 2023-04-17 06:11:23.635571 Alpha_Rabbit-1.3.7/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    25924 2023-04-17 06:09:48.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22640 2023-03-24 01:41:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:11:23.640563 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 06:11:23.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-04-17 06:11:23.640563 Alpha_Rabbit-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.3.7/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-17 06:11:23.641556 Alpha_Rabbit-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-04-17 06:11:15.000000 Alpha_Rabbit-1.3.7/setup.py
```

### Comparing `Alpha_Rabbit-1.3.6/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.3.7/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files 4% similar despite different names*

```diff
@@ -475,14 +475,37 @@
                         cmap="YlGnBu",
                         annot=True,
                         mask=mask,
                         )
         plt.savefig(savedir)
         plt.show()
 
+    def combine_imgs_pdf(folder_path, pdf_file_path,idstname):
+        import os
+        from PIL import Image
+        """
+        合成文件夹下的所有图片为pdf
+        Args:
+            folder_path (str): 源文件夹
+            pdf_file_path (str): 输出路径
+        """
+        files = os.listdir(folder_path)
+        png_files = []
+        sources = []
+        for file in files:
+            if 'png' in file or 'jpg' in file:
+                png_files.append(folder_path + file)
+        png_files.sort()
+    
+        for file in png_files:
+            png_file = Image.open(file)
+            png_file = png_file.convert("RGB")
+            sources.append(png_file)
+        sources[0].save(pdf_file_path+'{}.pdf'.format(idstname), "pdf", save_all=True, append_images=sources[1:],quality = 95)
+
 class mate_alphalens(object):
     def __init__(self) -> None:
         pass
 
     def index_mate(self,factordata,price):
         fcdf = factordata.reset_index()
         fcdf['date'] = pd.to_datetime(fcdf['date'])
```

### Comparing `Alpha_Rabbit-1.3.6/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Calculator.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.6/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.3.7/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.6/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.3.7/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.6/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.3.7/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha-Rabbit
-Version: 1.3.6
+Version: 1.3.7
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.3.6/LICENSE.txt` & `Alpha_Rabbit-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.3.6/PKG-INFO` & `Alpha_Rabbit-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha_Rabbit
-Version: 1.3.6
+Version: 1.3.7
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.3.6/setup.py` & `Alpha_Rabbit-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.3.6",
+    version="1.3.7",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```

