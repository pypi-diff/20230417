# Comparing `tmp/coco_loader-0.0.2.tar.gz` & `tmp/coco_loader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coco_loader-0.0.2.tar", max compression
+gzip compressed data, was "coco_loader-0.0.3.tar", max compression
```

## Comparing `coco_loader-0.0.2.tar` & `coco_loader-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-04-17 05:29:43.361653 coco_loader-0.0.2/LICENSE
--rw-r--r--   0        0        0     2406 2023-04-17 05:30:05.766619 coco_loader-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-06 01:21:23.643490 coco_loader-0.0.2/coco_loader/__init__.py
--rw-r--r--   0        0        0      638 2023-04-17 05:28:44.651914 coco_loader-0.0.2/coco_loader/bases.py
--rw-r--r--   0        0        0     1149 2023-04-17 05:44:03.178835 coco_loader-0.0.2/coco_loader/common.py
--rw-r--r--   0        0        0      391 2023-04-17 05:28:24.536399 coco_loader-0.0.2/coco_loader/imagecaptioning.py
--rw-r--r--   0        0        0      698 2023-04-17 05:28:24.536419 coco_loader-0.0.2/coco_loader/keypointdetection.py
--rw-r--r--   0        0        0      691 2023-04-17 05:28:24.536453 coco_loader-0.0.2/coco_loader/objectdetection.py
--rw-r--r--   0        0        0      832 2023-04-17 05:28:24.516831 coco_loader-0.0.2/coco_loader/panopticsegmentation.py
--rw-r--r--   0        0        0      627 2023-04-17 05:44:52.654775 coco_loader-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 coco_loader-0.0.2/setup.py
--rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 coco_loader-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-17 05:29:43.361653 coco_loader-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2406 2023-04-17 05:30:05.766619 coco_loader-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 01:21:23.643490 coco_loader-0.0.3/coco_loader/__init__.py
+-rw-r--r--   0        0        0      638 2023-04-17 05:28:44.651914 coco_loader-0.0.3/coco_loader/bases.py
+-rw-r--r--   0        0        0     1149 2023-04-17 05:44:03.178835 coco_loader-0.0.3/coco_loader/common.py
+-rw-r--r--   0        0        0      391 2023-04-17 05:28:24.536399 coco_loader-0.0.3/coco_loader/imagecaptioning.py
+-rw-r--r--   0        0        0      698 2023-04-17 05:28:24.536419 coco_loader-0.0.3/coco_loader/keypointdetection.py
+-rw-r--r--   0        0        0      691 2023-04-17 05:28:24.536453 coco_loader-0.0.3/coco_loader/objectdetection.py
+-rw-r--r--   0        0        0      832 2023-04-17 05:28:24.516831 coco_loader-0.0.3/coco_loader/panopticsegmentation.py
+-rw-r--r--   0        0        0      627 2023-04-17 05:49:36.771323 coco_loader-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 coco_loader-0.0.3/setup.py
+-rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 coco_loader-0.0.3/PKG-INFO
```

### Comparing `coco_loader-0.0.2/LICENSE` & `coco_loader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.2/README.md` & `coco_loader-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.2/coco_loader/bases.py` & `coco_loader-0.0.3/coco_loader/bases.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.2/coco_loader/common.py` & `coco_loader-0.0.3/coco_loader/common.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.2/coco_loader/keypointdetection.py` & `coco_loader-0.0.3/coco_loader/keypointdetection.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.2/coco_loader/objectdetection.py` & `coco_loader-0.0.3/coco_loader/objectdetection.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.2/coco_loader/panopticsegmentation.py` & `coco_loader-0.0.3/coco_loader/panopticsegmentation.py`

 * *Files identical despite different names*

### Comparing `coco_loader-0.0.2/pyproject.toml` & `coco_loader-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coco-loader"
-version = "0.0.2"
+version = "0.0.3"
 description = "COCO dataset loader."
 license = "MIT"
 authors = ["Jinhyuck Cha <jhcha@superb-ai.com>"]
 maintainers = ["Jinhyuck Cha <jhcha@superb-ai.com>"]
 readme = "README.md"
 homepage = "https://github.com/jinhyuckcha/coco-loader"
 repository = "https://github.com/jinhyuckcha/coco-loader"
```

### Comparing `coco_loader-0.0.2/setup.py` & `coco_loader-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['dataclasses-json>=0.5.4,<0.6.0']
 
 setup_kwargs = {
     'name': 'coco-loader',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'COCO dataset loader.',
     'long_description': "# coco-loader\n\nCOCO dataset loader.\nProvides serializable native Python bindings for several COCO dataset formats.\n\nSupported bindings and their corresponding modules:\n\n- Object Detection: `objectdetection`\n- Keypoint Detection: `keypointdetection`\n- Panoptic Segmentation: `panopticsegmentation`\n- Image Captioning: `imagecaptioning`\n\n## Installation\n\n`coco-loader` is available on PyPI:\n\n```bash\npip install coco-loader\n```\n\n## Usage\n\n### Creating a dataset (Object Detection)\n\n```python\n>>> from coco_loader.common import Info, Image, License\n>>> from coco_loader.objectdetection import ObjectDetectionAnnotation, \\\n...                                      ObjectDetectionCategory, \\\n...                                      ObjectDetectionDataset\n>>> from datetime import datetime\n>>> info = Info(  # Describe the dataset\n...    year=datetime.now().year,\n...    version='1.0',\n...    description='This is a test dataset',\n...    contributor='Test',\n...    url='https://test',\n...    date_created=datetime.now()\n... )\n>>> mit_license = License(  # Set the license\n...     id=0,\n...     name='MIT',\n...     url='https://opensource.org/licenses/MIT'\n... )\n>>> images = [  # Describe the images\n...     Image(\n...         id=0,\n...         width=640, height=480,\n...         file_name='test.jpg',\n...         license=mit_license.id,\n...         flickr_url='',\n...         coco_url='',\n...         date_captured=datetime.now()\n...     ),\n...     ...\n... ]\n>>> categories = [  # Describe the categories\n...     ObjectDetectionCategory(\n...         id=0,\n...         name='pedestrian',\n...         supercategory=''\n...     ),\n...     ...\n... ]\n>>> annotations = [  # Describe the annotations\n...     ObjectDetectionAnnotation(\n...         id=0,\n...         image_id=0,\n...         category_id=0,\n...         segmentation=[],\n...         area=800.0,\n...         bbox=[300.0, 100.0, 20.0, 40.0],\n...         is_crowd=0\n...     ),\n...     ...\n... ]\n>>> dataset = ObjectDetectionDataset(  # Create the dataset\n...     info=info,\n...     images=images,\n...     licenses=[mit_license],\n...     categories=categories,\n...     annotations=annotations\n... )\n>>> dataset.save('test_dataset.json', indent=2)  # Save the dataset\n```\n\n### Loading a dataset\n\n```python\n>>> from coco_loader.objectdetection import ObjectDetectionDataset\n>>> dataset = ObjectDetectionDataset.load('test_dataset.json')  # Load the dataset\n```\n",
     'author': 'Jinhyuck Cha',
     'author_email': 'jhcha@superb-ai.com',
     'maintainer': 'Jinhyuck Cha',
     'maintainer_email': 'jhcha@superb-ai.com',
     'url': 'https://github.com/jinhyuckcha/coco-loader',
```

### Comparing `coco_loader-0.0.2/PKG-INFO` & `coco_loader-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coco-loader
-Version: 0.0.2
+Version: 0.0.3
 Summary: COCO dataset loader.
 Home-page: https://github.com/jinhyuckcha/coco-loader
 License: MIT
 Author: Jinhyuck Cha
 Author-email: jhcha@superb-ai.com
 Maintainer: Jinhyuck Cha
 Maintainer-email: jhcha@superb-ai.com
```

