# Comparing `tmp/imggencli-1.3.3.tar.gz` & `tmp/imggencli-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.3.3.tar", last modified: Mon Apr 17 10:26:08 2023, max compression
+gzip compressed data, was "imggencli-1.4.1.tar", last modified: Mon Apr 17 11:18:18 2023, max compression
```

## Comparing `imggencli-1.3.3.tar` & `imggencli-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:08.230372 imggencli-1.3.3/
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:26:08.228942 imggencli-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:08.196437 imggencli-1.3.3/dalleci/
--rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.3.3/dalleci/__init__.py
--rw-rw-rw-   0        0        0    10533 2023-04-17 10:24:07.000000 imggencli-1.3.3/dalleci/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:08.221238 imggencli-1.3.3/imggencli.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:26:08.000000 imggencli-1.3.3/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:26:08.230372 imggencli-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-17 10:25:59.000000 imggencli-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:18:18.568164 imggencli-1.4.1/
+-rw-rw-rw-   0        0        0     1080 2023-03-23 10:19:17.000000 imggencli-1.4.1/License.txt
+-rw-rw-rw-   0        0        0     4160 2023-04-17 11:18:18.563485 imggencli-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3699 2023-03-23 09:52:46.000000 imggencli-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 11:18:18.533754 imggencli-1.4.1/imggencli/
+-rw-rw-rw-   0        0        0        2 2023-03-23 10:19:28.000000 imggencli-1.4.1/imggencli/__init__.py
+-rw-rw-rw-   0        0        0    10536 2023-04-17 11:14:53.000000 imggencli-1.4.1/imggencli/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:18:18.560377 imggencli-1.4.1/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     4160 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 11:18:18.000000 imggencli-1.4.1/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:18:18.568164 imggencli-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-04-17 11:06:26.000000 imggencli-1.4.1/setup.py
```

### Comparing `imggencli-1.3.3/PKG-INFO` & `imggencli-1.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.3.3
+Version: 1.4.1
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
 Description-Content-Type: text/markdown
+License-File: License.txt
 
 # ImgGenCli 💠
 
 `imggencli` is a community-maintained cli designed to provide users with the ability to generate, edit and filter images using the DALL-E 2 API provided by OpenAI, all from the command line.
 
 The tool provides three main commands, generate, edit, and filter.
 
@@ -93,8 +94,18 @@
   --filter [grayscale|sepia|blur|contour|detail|edge_enhance|edge_enhance_more|emboss|find_edges|sharpen|smooth|smooth_more|outline|posterize|solarize|invert|flip]
                                   🎨 The filter to apply to the image
   --save-path PATH                The directory to save the filtered image.
                                   Defaults to the current directory.
   --help                          Show this message and exit.
 ```
 
-### Updates / Changes / Future Scope : Implementing img2img in the same cli application
+**```update```**
+```console
+Usage: imggencli update [OPTIONS]
+
+  🔐 Update the OpenAI API key.
+
+Options:
+  --help  Show this message and exit.
+```
+
+Please feel to create issues or request for features. There will be many features added to the cli.
```

### Comparing `imggencli-1.3.3/README.md` & `imggencli-1.4.1/imggencli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: imggencli
+Version: 1.4.1
+Summary: A command line application to generate customized images based on the Open AI API.
+Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
+Author: Shayan Shaikh
+Author-email: Shaikhshayan1@gmail.com
+License: Open Source
+Keywords: cli,developer tools,productivity,openai,generative art,ai
+Requires-Python: >3.5
+Description-Content-Type: text/markdown
+License-File: License.txt
+
 # ImgGenCli 💠
 
 `imggencli` is a community-maintained cli designed to provide users with the ability to generate, edit and filter images using the DALL-E 2 API provided by OpenAI, all from the command line.
 
 The tool provides three main commands, generate, edit, and filter.
 
 The `generate` command allows the user to generate an image using a prompt, with the option to apply a filter, specify the size, and choose the number of times to generate the image. The generated image can also be saved to a specified file path.
@@ -81,8 +94,18 @@
   --filter [grayscale|sepia|blur|contour|detail|edge_enhance|edge_enhance_more|emboss|find_edges|sharpen|smooth|smooth_more|outline|posterize|solarize|invert|flip]
                                   🎨 The filter to apply to the image
   --save-path PATH                The directory to save the filtered image.
                                   Defaults to the current directory.
   --help                          Show this message and exit.
 ```
 
-### Updates / Changes / Future Scope : Implementing img2img in the same cli application
+**```update```**
+```console
+Usage: imggencli update [OPTIONS]
+
+  🔐 Update the OpenAI API key.
+
+Options:
+  --help  Show this message and exit.
+```
+
+Please feel to create issues or request for features. There will be many features added to the cli.
```

### Comparing `imggencli-1.3.3/dalleci/cli.py` & `imggencli-1.4.1/imggencli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         print("🔒 Authentication Failed. Try with a fresh API key.")
     except Exception:
         print("❌ Failed to generate image. Please try again with a different prompt.")
 
 
 def generate_variations(input_file, n, save_path=None):
     try:
-        with console.status("Generating image...", spinner="dots8Bit"):
+        with console.status("Generating image from given input...", spinner="dots8Bit"):
             response = openai.Image.create_variation(
                 image=open(input_file, "rb"),
                 n=n,
                 size="1024x1024"
             )
             image_data = requests.get(
                 response.get("data")[0]["url"], timeout=300
@@ -127,28 +127,19 @@
     }
     if filter_name in filters:
         return filters[filter_name]
     return image
 
 
 @click.group()
-@click.version_option(version="1.3.2")
+@click.version_option(version="1.4.1")
 def cli():
     """💠 Use this Open AI api to generate, as well as customize : edit & filter images from the cmd line."""
 
 
-@click.command("img2img")
-@click.argument('input_file')
-@click.option('--n', default=2, type=int, help='Number of variations to generate')
-def generate_img(input_file, numVars):
-    """🌸 Generate an image from an existing image using Open Ai"""
-    configure_openai()
-    generate_variations(input_file=input_file, n=numVars)
-
-
 @cli.command("generate")
 @click.option(
     "--prompt",
     default="Suprise me",
     prompt=True,
     help="💬 The prompt to generate the image from.",
 )
@@ -184,19 +175,28 @@
 @click.option(
     "--save-path",
     type=click.Path(dir_okay=False, writable=True),
     help="💾 Save the generated image to the specified file path",
     default="images/output.png",
 )
 def generate(prompt, size, filter, iterations, save_path):
-    """🌸 Generate an image from the OpenAI Dalle api"""
+    """🌸 Generate an image from the OpenAI api"""
     configure_openai()
     generate_image(prompt, size, filter, iterations, save_path)
 
 
+@cli.command("img2img")
+@click.argument("img_path")
+@click.option('--n', default=1, type=int, help='Number of variation images to generate')
+def generate_img(image_path,num):
+    """Generate an image from an existing image using Open AI api"""
+    configure_openai()
+    generate_variations(input_file=image_path, n=num)
+
+
 @cli.command("edit")
 @click.argument("image_path", type=click.Path(exists=True))
 @click.option("--brightness", type=float, help="💡 The brightness of the image")
 @click.option("--contrast", type=float, help="🌈 The contrast of the image")
 @click.option("--sharpness", type=float, help="🔪 The sharpness of the image")
 def edit(image_path, brightness, contrast, sharpness):
     """🎴 Change the brightness, contrast and sharpness of an image."""
```

### Comparing `imggencli-1.3.3/imggencli.egg-info/PKG-INFO` & `imggencli-1.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: imggencli
-Version: 1.3.3
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
@@ -93,8 +81,18 @@
   --filter [grayscale|sepia|blur|contour|detail|edge_enhance|edge_enhance_more|emboss|find_edges|sharpen|smooth|smooth_more|outline|posterize|solarize|invert|flip]
                                   🎨 The filter to apply to the image
   --save-path PATH                The directory to save the filtered image.
                                   Defaults to the current directory.
   --help                          Show this message and exit.
 ```
 
-### Updates / Changes / Future Scope : Implementing img2img in the same cli application
+**```update```**
+```console
+Usage: imggencli update [OPTIONS]
+
+  🔐 Update the OpenAI API key.
+
+Options:
+  --help  Show this message and exit.
+```
+
+Please feel to create issues or request for features. There will be many features added to the cli.
```

### Comparing `imggencli-1.3.3/setup.py` & `imggencli-1.4.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.3.3",
+    version="1.4.1",
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
-    entry_points={"console_scripts": ["imggencli = dallecli.cli:cli"]},
+    entry_points={"console_scripts": ["imggencli=imggencli.cli:cli"]},
 )
```

