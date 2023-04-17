# Comparing `tmp/imggencli-1.2.1.tar.gz` & `tmp/imggencli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.2.1.tar", last modified: Thu Mar 23 10:40:36 2023, max compression
+gzip compressed data, was "imggencli-1.2.2.tar", last modified: Mon Apr 17 09:34:36 2023, max compression
```

## Comparing `imggencli-1.2.1.tar` & `imggencli-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 10:40:36.458644 imggencli-1.2.1/
--rw-rw-rw-   0        0        0     1080 2023-03-23 10:19:17.000000 imggencli-1.2.1/License.txt
--rw-rw-rw-   0        0        0     4160 2023-03-23 10:40:36.458644 imggencli-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3699 2023-03-23 09:52:46.000000 imggencli-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 10:40:36.429067 imggencli-1.2.1/imggencli/
--rw-rw-rw-   0        0        0        2 2023-03-23 10:19:28.000000 imggencli-1.2.1/imggencli/__init__.py
--rw-rw-rw-   0        0        0     9222 2023-03-23 10:20:46.000000 imggencli-1.2.1/imggencli/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-23 10:40:36.458644 imggencli-1.2.1/imggencli.egg-info/
--rw-rw-rw-   0        0        0     4160 2023-03-23 10:40:36.000000 imggencli-1.2.1/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-03-23 10:40:36.000000 imggencli-1.2.1/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 10:40:36.000000 imggencli-1.2.1/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-23 10:40:36.000000 imggencli-1.2.1/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-03-23 10:40:36.000000 imggencli-1.2.1/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-23 10:40:36.000000 imggencli-1.2.1/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 10:40:36.469232 imggencli-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-03-23 10:40:09.000000 imggencli-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:34:36.153106 imggencli-1.2.2/
+drwxrwxrwx   0        0        0        0 2023-04-17 09:34:36.121394 imggencli-1.2.2/Img-gen/
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.2/Img-gen/__init__.py
+-rw-rw-rw-   0        0        0    10325 2023-04-17 09:34:22.000000 imggencli-1.2.2/Img-gen/cli.py
+-rw-rw-rw-   0        0        0     3961 2023-04-17 09:34:36.151295 imggencli-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:34:36.146661 imggencli-1.2.2/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:34:36.153106 imggencli-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-17 09:33:00.000000 imggencli-1.2.2/setup.py
```

### Comparing `imggencli-1.2.1/PKG-INFO` & `imggencli-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: imggencli
-Version: 1.2.1
-Summary: A command line application to generate customized images based on the Open AI API.
-Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
-Author: Shayan Shaikh
-Author-email: Shaikhshayan1@gmail.com
-License: Open Source
-Keywords: cli,developer tools,productivity,openai,generative art,ai
-Requires-Python: >3.5
-Description-Content-Type: text/markdown
-License-File: License.txt
-
 # ImgGenCli 💠
 
 `imggencli` is a community-maintained cli designed to provide users with the ability to generate, edit and filter images using the DALL-E 2 API provided by OpenAI, all from the command line.
 
 The tool provides three main commands, generate, edit, and filter.
 
 The `generate` command allows the user to generate an image using a prompt, with the option to apply a filter, specify the size, and choose the number of times to generate the image. The generated image can also be saved to a specified file path.
@@ -94,18 +81,8 @@
   --filter [grayscale|sepia|blur|contour|detail|edge_enhance|edge_enhance_more|emboss|find_edges|sharpen|smooth|smooth_more|outline|posterize|solarize|invert|flip]
                                   🎨 The filter to apply to the image
   --save-path PATH                The directory to save the filtered image.
                                   Defaults to the current directory.
   --help                          Show this message and exit.
 ```
 
-**```update```**
-```console
-Usage: imggencli update [OPTIONS]
-
-  🔐 Update the OpenAI API key.
-
-Options:
-  --help  Show this message and exit.
-```
-
-Please feel to create issues or request for features. There will be many features added to the cli.
+### Updates / Changes / Future Scope : Implementing img2img in the same cli application
```

### Comparing `imggencli-1.2.1/README.md` & `imggencli-1.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: imggencli
+Version: 1.2.2
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
@@ -81,18 +93,8 @@
   --filter [grayscale|sepia|blur|contour|detail|edge_enhance|edge_enhance_more|emboss|find_edges|sharpen|smooth|smooth_more|outline|posterize|solarize|invert|flip]
                                   🎨 The filter to apply to the image
   --save-path PATH                The directory to save the filtered image.
                                   Defaults to the current directory.
   --help                          Show this message and exit.
 ```
 
-**```update```**
-```console
-Usage: imggencli update [OPTIONS]
-
-  🔐 Update the OpenAI API key.
-
-Options:
-  --help  Show this message and exit.
-```
-
-Please feel to create issues or request for features. There will be many features added to the cli.
+### Updates / Changes / Future Scope : Implementing img2img in the same cli application
```

### Comparing `imggencli-1.2.1/imggencli/cli.py` & `imggencli-1.2.2/Img-gen/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,15 +106,41 @@
         return filters[filter_name]
     return image
 
 
 @click.group()
 @click.version_option(version="1.2.0")
 def cli():
-    """💠 Use the Dall.E 2 api to generate, edit & filter images from the cmd line."""
+    """💠 Use this Open AI api to generate, as well as customize : edit & filter images from the cmd line."""
+
+
+@click.command("img2img")
+@click.argument('input_file')
+@click.option('--n', default=2, help='Number of variations to generate')
+def generate_variations(input_file, n, save_path=None):
+    try:
+        with console.status("Generating image...", spinner="dots8Bit"):
+            response = openai.Image.create_variation(
+                image=open(input_file, "rb"),
+                n=n,
+                size="1024x1024"
+            )
+            image_data = requests.get(
+                response.get("data")[0]["url"], timeout=300
+            ).content
+            image = Image.open(BytesIO(image_data))
+            image.show()
+            if save_path is not None:
+                if not path.exists(path.dirname(save_path)):
+                    makedirs(path.dirname(save_path))
+                image.save(save_path)
+    except openai.error.AuthenticationError:
+        print("🔒 Authentication Failed. Try with a fresh API key.")
+    except Exception:
+        print("❌ Failed to generate image. Please try again with a different prompt.")
 
 
 @cli.command("generate")
 @click.option(
     "--prompt",
     default="Suprise me",
     prompt=True,
@@ -260,7 +286,8 @@
 def get_unique_filename(filename):
     name, ext = path.splitext(filename)
     i = 1
     while path.exists(filename):
         filename = f"{name}_{i}{ext}"
         i += 1
     return filename
+
```

### Comparing `imggencli-1.2.1/imggencli.egg-info/PKG-INFO` & `imggencli-1.2.2/imggencli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.1
+Version: 1.2.2
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
 Description-Content-Type: text/markdown
-License-File: License.txt
 
 # ImgGenCli 💠
 
 `imggencli` is a community-maintained cli designed to provide users with the ability to generate, edit and filter images using the DALL-E 2 API provided by OpenAI, all from the command line.
 
 The tool provides three main commands, generate, edit, and filter.
 
@@ -94,18 +93,8 @@
   --filter [grayscale|sepia|blur|contour|detail|edge_enhance|edge_enhance_more|emboss|find_edges|sharpen|smooth|smooth_more|outline|posterize|solarize|invert|flip]
                                   🎨 The filter to apply to the image
   --save-path PATH                The directory to save the filtered image.
                                   Defaults to the current directory.
   --help                          Show this message and exit.
 ```
 
-**```update```**
-```console
-Usage: imggencli update [OPTIONS]
-
-  🔐 Update the OpenAI API key.
-
-Options:
-  --help  Show this message and exit.
-```
-
-Please feel to create issues or request for features. There will be many features added to the cli.
+### Updates / Changes / Future Scope : Implementing img2img in the same cli application
```

### Comparing `imggencli-1.2.1/setup.py` & `imggencli-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.2.1",
+    version="1.2.2",
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
+    entry_points={"console_scripts": ["dallecli=dallecli.cli:cli"]},
 )
```

