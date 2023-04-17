# Comparing `tmp/imggencli-1.3.2.tar.gz` & `tmp/imggencli-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.3.2.tar", last modified: Mon Apr 17 10:19:54 2023, max compression
+gzip compressed data, was "imggencli-1.3.3.tar", last modified: Mon Apr 17 10:26:08 2023, max compression
```

## Comparing `imggencli-1.3.2.tar` & `imggencli-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:19:54.745621 imggencli-1.3.2/
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:19:54.742796 imggencli-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:19:54.716910 imggencli-1.3.2/dalleci/
--rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.3.2/dalleci/__init__.py
--rw-rw-rw-   0        0        0    10533 2023-04-17 10:19:10.000000 imggencli-1.3.2/dalleci/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:19:54.740634 imggencli-1.3.2/imggencli.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:19:54.748223 imggencli-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-17 10:19:43.000000 imggencli-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:08.230372 imggencli-1.3.3/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:26:08.228942 imggencli-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:08.196437 imggencli-1.3.3/dalleci/
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.3.3/dalleci/__init__.py
+-rw-rw-rw-   0        0        0    10533 2023-04-17 10:24:07.000000 imggencli-1.3.3/dalleci/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:08.221238 imggencli-1.3.3/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:26:08.230372 imggencli-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-17 10:25:59.000000 imggencli-1.3.3/setup.py
```

### Comparing `imggencli-1.3.2/PKG-INFO` & `imggencli-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.3.2
+Version: 1.3.3
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.3.2/README.md` & `imggencli-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `imggencli-1.3.2/dalleci/cli.py` & `imggencli-1.3.3/dalleci/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     }
     if filter_name in filters:
         return filters[filter_name]
     return image
 
 
 @click.group()
-@click.version_option(version="1.3.1")
+@click.version_option(version="1.3.2")
 def cli():
     """💠 Use this Open AI api to generate, as well as customize : edit & filter images from the cmd line."""
 
 
 @click.command("img2img")
 @click.argument('input_file')
 @click.option('--n', default=2, type=int, help='Number of variations to generate')
```

### Comparing `imggencli-1.3.2/imggencli.egg-info/PKG-INFO` & `imggencli-1.3.3/imggencli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.3.2
+Version: 1.3.3
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.3.2/setup.py` & `imggencli-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.3.2",
+    version="1.3.3",
     description="A command line application to generate customized images based on the Open AI API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shayan-shaikh/Image-generation-CLI",
     author="Shayan Shaikh",
     license="Open Source",
     author_email="Shaikhshayan1@gmail.com",
```

