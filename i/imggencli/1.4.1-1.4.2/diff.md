# Comparing `tmp/imggencli-1.4.1.tar.gz` & `tmp/imggencli-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.4.1.tar", last modified: Mon Apr 17 11:18:18 2023, max compression
+gzip compressed data, was "imggencli-1.4.2.tar", last modified: Mon Apr 17 11:27:22 2023, max compression
```

## Comparing `imggencli-1.4.1.tar` & `imggencli-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:18:18.568164 imggencli-1.4.1/
--rw-rw-rw-   0        0        0     1080 2023-03-23 10:19:17.000000 imggencli-1.4.1/License.txt
--rw-rw-rw-   0        0        0     4160 2023-04-17 11:18:18.563485 imggencli-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3699 2023-03-23 09:52:46.000000 imggencli-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 11:18:18.533754 imggencli-1.4.1/imggencli/
--rw-rw-rw-   0        0        0        2 2023-03-23 10:19:28.000000 imggencli-1.4.1/imggencli/__init__.py
--rw-rw-rw-   0        0        0    10536 2023-04-17 11:14:53.000000 imggencli-1.4.1/imggencli/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:18:18.560377 imggencli-1.4.1/imggencli.egg-info/
--rw-rw-rw-   0        0        0     4160 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 11:18:18.568164 imggencli-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-04-17 11:06:26.000000 imggencli-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:27:22.150338 imggencli-1.4.2/
+-rw-rw-rw-   0        0        0     1080 2023-03-23 10:19:17.000000 imggencli-1.4.2/License.txt
+-rw-rw-rw-   0        0        0     4160 2023-04-17 11:27:22.144212 imggencli-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3699 2023-03-23 09:52:46.000000 imggencli-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 11:27:22.120073 imggencli-1.4.2/imggencli/
+-rw-rw-rw-   0        0        0        2 2023-03-23 10:19:28.000000 imggencli-1.4.2/imggencli/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-04-17 11:26:49.000000 imggencli-1.4.2/imggencli/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:27:22.144212 imggencli-1.4.2/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     4160 2023-04-17 11:27:22.000000 imggencli-1.4.2/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-17 11:27:22.000000 imggencli-1.4.2/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:27:22.000000 imggencli-1.4.2/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-17 11:27:22.000000 imggencli-1.4.2/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 11:27:22.000000 imggencli-1.4.2/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 11:27:22.000000 imggencli-1.4.2/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:27:22.150338 imggencli-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-04-17 11:26:49.000000 imggencli-1.4.2/setup.py
```

### Comparing `imggencli-1.4.1/License.txt` & `imggencli-1.4.2/License.txt`

 * *Files identical despite different names*

### Comparing `imggencli-1.4.1/PKG-INFO` & `imggencli-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.4.1
+Version: 1.4.2
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.4.1/README.md` & `imggencli-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `imggencli-1.4.1/imggencli/cli.py` & `imggencli-1.4.2/imggencli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     }
     if filter_name in filters:
         return filters[filter_name]
     return image
 
 
 @click.group()
-@click.version_option(version="1.4.1")
+@click.version_option(version="1.4.2")
 def cli():
     """💠 Use this Open AI api to generate, as well as customize : edit & filter images from the cmd line."""
 
 
 @cli.command("generate")
 @click.option(
     "--prompt",
@@ -181,20 +181,20 @@
 def generate(prompt, size, filter, iterations, save_path):
     """🌸 Generate an image from the OpenAI api"""
     configure_openai()
     generate_image(prompt, size, filter, iterations, save_path)
 
 
 @cli.command("img2img")
-@click.argument("img_path")
+@click.argument("input_file", type=click.Path(exists=True))
 @click.option('--n', default=1, type=int, help='Number of variation images to generate')
-def generate_img(image_path,num):
+def generate_img(input_file, num):
     """Generate an image from an existing image using Open AI api"""
     configure_openai()
-    generate_variations(input_file=image_path, n=num)
+    generate_variations(input_file=input_file, n=num)
 
 
 @cli.command("edit")
 @click.argument("image_path", type=click.Path(exists=True))
 @click.option("--brightness", type=float, help="💡 The brightness of the image")
 @click.option("--contrast", type=float, help="🌈 The contrast of the image")
 @click.option("--sharpness", type=float, help="🔪 The sharpness of the image")
```

### Comparing `imggencli-1.4.1/imggencli.egg-info/PKG-INFO` & `imggencli-1.4.2/imggencli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.4.1
+Version: 1.4.2
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.4.1/setup.py` & `imggencli-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.4.1",
+    version="1.4.2",
     description="A command line application to generate customized images based on the Open AI API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shayan-shaikh/Image-generation-CLI",
     author="Shayan Shaikh",
     license="Open Source",
     author_email="Shaikhshayan1@gmail.com",
```

