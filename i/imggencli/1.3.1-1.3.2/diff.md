# Comparing `tmp/imggencli-1.3.1.tar.gz` & `tmp/imggencli-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.3.1.tar", last modified: Mon Apr 17 10:16:15 2023, max compression
+gzip compressed data, was "imggencli-1.3.2.tar", last modified: Mon Apr 17 10:19:54 2023, max compression
```

## Comparing `imggencli-1.3.1.tar` & `imggencli-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:16:15.155325 imggencli-1.3.1/
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:16:15.151436 imggencli-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:16:15.125841 imggencli-1.3.1/dalleci/
--rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.3.1/dalleci/__init__.py
--rw-rw-rw-   0        0        0    10462 2023-04-17 10:14:42.000000 imggencli-1.3.1/dalleci/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:16:15.148924 imggencli-1.3.1/imggencli.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:16:15.000000 imggencli-1.3.1/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-17 10:16:15.000000 imggencli-1.3.1/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:16:15.000000 imggencli-1.3.1/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 10:16:15.000000 imggencli-1.3.1/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 10:16:15.000000 imggencli-1.3.1/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:16:15.000000 imggencli-1.3.1/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:16:15.155325 imggencli-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-17 10:15:53.000000 imggencli-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:19:54.745621 imggencli-1.3.2/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:19:54.742796 imggencli-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:19:54.716910 imggencli-1.3.2/dalleci/
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.3.2/dalleci/__init__.py
+-rw-rw-rw-   0        0        0    10533 2023-04-17 10:19:10.000000 imggencli-1.3.2/dalleci/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:19:54.740634 imggencli-1.3.2/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:19:54.000000 imggencli-1.3.2/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:19:54.748223 imggencli-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-17 10:19:43.000000 imggencli-1.3.2/setup.py
```

### Comparing `imggencli-1.3.1/PKG-INFO` & `imggencli-1.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: imggencli
-Version: 1.3.1
-Summary: A command line application to generate customized images based on the Open AI API.
-Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
-Author: Shayan Shaikh
-Author-email: Shaikhshayan1@gmail.com
-License: Open Source
-Keywords: cli,developer tools,productivity,openai,generative art,ai
-Requires-Python: >3.5
-Description-Content-Type: text/markdown
-
 # ImgGenCli 💠
 
 `imggencli` is a community-maintained cli designed to provide users with the ability to generate, edit and filter images using the DALL-E 2 API provided by OpenAI, all from the command line.
 
 The tool provides three main commands, generate, edit, and filter.
 
 The `generate` command allows the user to generate an image using a prompt, with the option to apply a filter, specify the size, and choose the number of times to generate the image. The generated image can also be saved to a specified file path.
```

### Comparing `imggencli-1.3.1/README.md` & `imggencli-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: imggencli
+Version: 1.3.2
+Summary: A command line application to generate customized images based on the Open AI API.
+Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
+Author: Shayan Shaikh
+Author-email: Shaikhshayan1@gmail.com
+License: Open Source
+Keywords: cli,developer tools,productivity,openai,generative art,ai
+Requires-Python: >3.5
+Description-Content-Type: text/markdown
+
 # ImgGenCli 💠
 
 `imggencli` is a community-maintained cli designed to provide users with the ability to generate, edit and filter images using the DALL-E 2 API provided by OpenAI, all from the command line.
 
 The tool provides three main commands, generate, edit, and filter.
 
 The `generate` command allows the user to generate an image using a prompt, with the option to apply a filter, specify the size, and choose the number of times to generate the image. The generated image can also be saved to a specified file path.
```

### Comparing `imggencli-1.3.1/dalleci/cli.py` & `imggencli-1.3.2/dalleci/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     """💠 Use this Open AI api to generate, as well as customize : edit & filter images from the cmd line."""
 
 
 @click.command("img2img")
 @click.argument('input_file')
 @click.option('--n', default=2, type=int, help='Number of variations to generate')
 def generate_img(input_file, numVars):
+    """🌸 Generate an image from an existing image using Open Ai"""
     configure_openai()
     generate_variations(input_file=input_file, n=numVars)
 
 
 @cli.command("generate")
 @click.option(
     "--prompt",
```

### Comparing `imggencli-1.3.1/imggencli.egg-info/PKG-INFO` & `imggencli-1.3.2/imggencli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.3.1
+Version: 1.3.2
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.3.1/setup.py` & `imggencli-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.3.1",
+    version="1.3.2",
     description="A command line application to generate customized images based on the Open AI API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shayan-shaikh/Image-generation-CLI",
     author="Shayan Shaikh",
     license="Open Source",
     author_email="Shaikhshayan1@gmail.com",
```

