# Comparing `tmp/arcanum-newspaper-segmentation-client-1.6.5.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.5.tar", last modified: Fri Apr 14 14:45:37 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.6.tar", last modified: Mon Apr 17 15:59:58 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.6.5.tar` & `arcanum-newspaper-segmentation-client-1.6.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.5/LICENSE
--rw-rw-rw-   0        0        0      675 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.5/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-14 14:44:59.000000 arcanum-newspaper-segmentation-client-1.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.747778 arcanum-newspaper-segmentation-client-1.6.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    13433 2023-04-14 10:21:05.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     3203 2023-04-14 10:21:05.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      756 2023-04-14 14:44:20.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.781078 arcanum-newspaper-segmentation-client-1.6.6/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.6/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-04-17 15:59:58.780080 arcanum-newspaper-segmentation-client-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.6/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:59:58.781078 arcanum-newspaper-segmentation-client-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-17 15:59:41.000000 arcanum-newspaper-segmentation-client-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.736198 arcanum-newspaper-segmentation-client-1.6.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.757141 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-17 15:59:58.000000 arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 15:59:58.780080 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    13521 2023-04-17 15:58:20.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     3203 2023-04-14 10:21:05.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      756 2023-04-14 14:44:20.000000 arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/LICENSE` & `arcanum-newspaper-segmentation-client-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.5
+Version: 1.6.6
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/setup.py` & `arcanum-newspaper-segmentation-client-1.6.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.6.5",
+    version="1.6.6",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.5
+Version: 1.6.6
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.6.6/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,14 +268,16 @@
 def add_ocr_blocks(segmented_page: dict, textract_response: dict) -> None:
     ocr_blocks_by_id = {ocr_block["Id"]: ocr_block for ocr_block in textract_response["Blocks"]}
 
     for article in segmented_page["articles"]:
         for block in article["blocks"]:
             ocr_blocks = []
             for ocr_block_id in block["ocr_blocks"]:
+                if ocr_block_id not in ocr_blocks_by_id:
+                    continue
                 ocr_blocks.append(ocr_blocks_by_id[ocr_block_id])
             block["ocr_blocks"] = ocr_blocks
 
 
 def run_newspaper_segmentation_on_image(image: Image, textract_response: dict, api_key: str) -> dict:
     image.thumbnail((1024, 1024))
     request_data = {"textract_response": textract_response}
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/pdf.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.6.6/src/newspaper_segmentation_client/text.py`

 * *Files identical despite different names*

