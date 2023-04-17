# Comparing `tmp/imggencli-1.2.5.tar.gz` & `tmp/imggencli-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.2.5.tar", last modified: Mon Apr 17 10:08:10 2023, max compression
+gzip compressed data, was "imggencli-1.2.6.tar", last modified: Mon Apr 17 10:11:42 2023, max compression
```

## Comparing `imggencli-1.2.5.tar` & `imggencli-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:08:10.066930 imggencli-1.2.5/
-drwxrwxrwx   0        0        0        0 2023-04-17 10:08:10.037463 imggencli-1.2.5/Img-gen/
--rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.5/Img-gen/__init__.py
--rw-rw-rw-   0        0        0    10478 2023-04-17 09:58:35.000000 imggencli-1.2.5/Img-gen/cli.py
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:08:10.063867 imggencli-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:08:10.059410 imggencli-1.2.5/imggencli.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-17 10:08:10.000000 imggencli-1.2.5/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:08:10.066930 imggencli-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-04-17 10:07:48.000000 imggencli-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:11:42.019096 imggencli-1.2.6/
+drwxrwxrwx   0        0        0        0 2023-04-17 10:11:41.984921 imggencli-1.2.6/Img-gen/
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.6/Img-gen/__init__.py
+-rw-rw-rw-   0        0        0    10478 2023-04-17 09:58:35.000000 imggencli-1.2.6/Img-gen/cli.py
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:11:42.016489 imggencli-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:11:42.011104 imggencli-1.2.6/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:11:41.000000 imggencli-1.2.6/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-17 10:11:41.000000 imggencli-1.2.6/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:11:41.000000 imggencli-1.2.6/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 10:11:41.000000 imggencli-1.2.6/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 10:11:41.000000 imggencli-1.2.6/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:11:41.000000 imggencli-1.2.6/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:11:42.019096 imggencli-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2023-04-17 10:11:32.000000 imggencli-1.2.6/setup.py
```

### Comparing `imggencli-1.2.5/Img-gen/cli.py` & `imggencli-1.2.6/Img-gen/cli.py`

 * *Files identical despite different names*

### Comparing `imggencli-1.2.5/PKG-INFO` & `imggencli-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.5
+Version: 1.2.6
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.5/README.md` & `imggencli-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `imggencli-1.2.5/imggencli.egg-info/PKG-INFO` & `imggencli-1.2.6/imggencli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.5
+Version: 1.2.6
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.5/setup.py` & `imggencli-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.2.5",
+    version="1.2.6",
     description="A command line application to generate customized images based on the Open AI API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shayan-shaikh/Image-generation-CLI",
     author="Shayan Shaikh",
     license="Open Source",
     author_email="Shaikhshayan1@gmail.com",
     keywords=["cli", "developer tools", "productivity", "openai", "generative art", "ai"],
     packages=find_packages(),
     install_requires=["click==8.1.3", "openai==0.27.2", "rich==13.3.1", "idna", "pillow"],
-    entry_points={"console_scripts": ["imggencli=imggencli.cli:cli"]},
+    entry_points={"console_scripts": ["imggencli=dallecli.cli:cli"]},
 )
```

