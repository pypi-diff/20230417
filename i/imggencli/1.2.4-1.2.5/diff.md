# Comparing `tmp/imggencli-1.2.4.tar.gz` & `tmp/imggencli-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.2.4.tar", last modified: Mon Apr 17 09:58:48 2023, max compression
+gzip compressed data, was "imggencli-1.2.5.tar", last modified: Mon Apr 17 10:08:10 2023, max compression
```

## Comparing `imggencli-1.2.4.tar` & `imggencli-1.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:58:48.039231 imggencli-1.2.4/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:58:48.006896 imggencli-1.2.4/Img-gen/
--rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.4/Img-gen/__init__.py
--rw-rw-rw-   0        0        0    10478 2023-04-17 09:58:35.000000 imggencli-1.2.4/Img-gen/cli.py
--rw-rw-rw-   0        0        0     3961 2023-04-17 09:58:48.036307 imggencli-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 09:58:48.031306 imggencli-1.2.4/imggencli.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 09:58:48.039231 imggencli-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-17 09:58:35.000000 imggencli-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:08:10.066930 imggencli-1.2.5/
+drwxrwxrwx   0        0        0        0 2023-04-17 10:08:10.037463 imggencli-1.2.5/Img-gen/
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.5/Img-gen/__init__.py
+-rw-rw-rw-   0        0        0    10478 2023-04-17 09:58:35.000000 imggencli-1.2.5/Img-gen/cli.py
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:08:10.063867 imggencli-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:08:10.059410 imggencli-1.2.5/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-17 10:08:10.000000 imggencli-1.2.5/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:08:09.000000 imggencli-1.2.5/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:08:10.066930 imggencli-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-04-17 10:07:48.000000 imggencli-1.2.5/setup.py
```

### Comparing `imggencli-1.2.4/Img-gen/cli.py` & `imggencli-1.2.5/Img-gen/cli.py`

 * *Files identical despite different names*

### Comparing `imggencli-1.2.4/PKG-INFO` & `imggencli-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.4
+Version: 1.2.5
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.4/README.md` & `imggencli-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `imggencli-1.2.4/imggencli.egg-info/PKG-INFO` & `imggencli-1.2.5/imggencli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.4
+Version: 1.2.5
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.4/setup.py` & `imggencli-1.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.2.4",
+    version="1.2.5",
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
-    entry_points={"console_scripts": ["dallecli=dallecli.cli:cli"]},
+    entry_points={"console_scripts": ["imggencli=imggencli.cli:cli"]},
 )
```

