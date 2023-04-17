# Comparing `tmp/imggencli-1.2.3.tar.gz` & `tmp/imggencli-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.2.3.tar", last modified: Mon Apr 17 09:47:28 2023, max compression
+gzip compressed data, was "imggencli-1.2.4.tar", last modified: Mon Apr 17 09:58:48 2023, max compression
```

## Comparing `imggencli-1.2.3.tar` & `imggencli-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:47:28.517896 imggencli-1.2.3/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:47:28.471259 imggencli-1.2.3/Img-gen/
--rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.3/Img-gen/__init__.py
--rw-rw-rw-   0        0        0    10459 2023-04-17 09:46:30.000000 imggencli-1.2.3/Img-gen/cli.py
--rw-rw-rw-   0        0        0     3961 2023-04-17 09:47:28.515425 imggencli-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 09:47:28.510714 imggencli-1.2.3/imggencli.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 09:47:28.520463 imggencli-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-17 09:46:30.000000 imggencli-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:58:48.039231 imggencli-1.2.4/
+drwxrwxrwx   0        0        0        0 2023-04-17 09:58:48.006896 imggencli-1.2.4/Img-gen/
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.4/Img-gen/__init__.py
+-rw-rw-rw-   0        0        0    10478 2023-04-17 09:58:35.000000 imggencli-1.2.4/Img-gen/cli.py
+-rw-rw-rw-   0        0        0     3961 2023-04-17 09:58:48.036307 imggencli-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:58:48.031306 imggencli-1.2.4/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 09:58:47.000000 imggencli-1.2.4/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:58:48.039231 imggencli-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-17 09:58:35.000000 imggencli-1.2.4/setup.py
```

### Comparing `imggencli-1.2.3/Img-gen/cli.py` & `imggencli-1.2.4/Img-gen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,36 +126,36 @@
         "rotate_270": lambda i: i.transpose(Image.ROTATE_270),
     }
     if filter_name in filters:
         return filters[filter_name]
     return image
 
 
-@click.group()
-@click.version_option(version="1.2.3")
+@click.group(name='ImggenCli')
+@click.version_option(version="1.2.4")
 def cli():
     """💠 Use this Open AI api to generate, as well as customize : edit & filter images from the cmd line."""
 
 
 @click.command("img2img")
 @click.argument('input_file')
-@click.option('--n', default=2,type=int, help='Number of variations to generate')
+@click.option('--n', default=2, type=int, help='Number of variations to generate')
 def generate_img(input_file, numVars):
     configure_openai()
     generate_variations(input_file=input_file, n=numVars)
 
 
 @cli.command("generate")
 @click.option(
     "--prompt",
     default="Suprise me",
     prompt=True,
     help="💬 The prompt to generate the image from.",
 )
-@click.option("--size", default="512x512", help="📐 The size of the generated image.")
+@click.option("--size", default="1024x1024", help="📐 The size of the generated image.")
 @click.option(
     "--filter",
     type=click.Choice(
         [
             "grayscale",
             "sepia",
             "blur",
```

### Comparing `imggencli-1.2.3/PKG-INFO` & `imggencli-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.3
+Version: 1.2.4
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.3/README.md` & `imggencli-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `imggencli-1.2.3/imggencli.egg-info/PKG-INFO` & `imggencli-1.2.4/imggencli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.3
+Version: 1.2.4
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.3/setup.py` & `imggencli-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.2.3",
+    version="1.2.4",
     description="A command line application to generate customized images based on the Open AI API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shayan-shaikh/Image-generation-CLI",
     author="Shayan Shaikh",
     license="Open Source",
     author_email="Shaikhshayan1@gmail.com",
```

