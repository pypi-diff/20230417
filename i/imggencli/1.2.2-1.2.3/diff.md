# Comparing `tmp/imggencli-1.2.2.tar.gz` & `tmp/imggencli-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imggencli-1.2.2.tar", last modified: Mon Apr 17 09:34:36 2023, max compression
+gzip compressed data, was "imggencli-1.2.3.tar", last modified: Mon Apr 17 09:47:28 2023, max compression
```

## Comparing `imggencli-1.2.2.tar` & `imggencli-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:34:36.153106 imggencli-1.2.2/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:34:36.121394 imggencli-1.2.2/Img-gen/
--rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.2/Img-gen/__init__.py
--rw-rw-rw-   0        0        0    10325 2023-04-17 09:34:22.000000 imggencli-1.2.2/Img-gen/cli.py
--rw-rw-rw-   0        0        0     3961 2023-04-17 09:34:36.151295 imggencli-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 09:34:36.146661 imggencli-1.2.2/imggencli.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 09:34:36.000000 imggencli-1.2.2/imggencli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 09:34:36.153106 imggencli-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-17 09:33:00.000000 imggencli-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:47:28.517896 imggencli-1.2.3/
+drwxrwxrwx   0        0        0        0 2023-04-17 09:47:28.471259 imggencli-1.2.3/Img-gen/
+-rw-rw-rw-   0        0        0        2 2023-04-17 08:01:17.000000 imggencli-1.2.3/Img-gen/__init__.py
+-rw-rw-rw-   0        0        0    10459 2023-04-17 09:46:30.000000 imggencli-1.2.3/Img-gen/cli.py
+-rw-rw-rw-   0        0        0     3961 2023-04-17 09:47:28.515425 imggencli-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2023-04-17 08:01:17.000000 imggencli-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:47:28.510714 imggencli-1.2.3/imggencli.egg-info/
+-rw-rw-rw-   0        0        0     3961 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 09:47:28.000000 imggencli-1.2.3/imggencli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:47:28.520463 imggencli-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-17 09:46:30.000000 imggencli-1.2.3/setup.py
```

### Comparing `imggencli-1.2.2/Img-gen/cli.py` & `imggencli-1.2.3/Img-gen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,37 @@
                     image.save(save_path)
     except openai.error.AuthenticationError:
         print("🔒 Authentication Failed. Try with a fresh API key.")
     except Exception:
         print("❌ Failed to generate image. Please try again with a different prompt.")
 
 
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
+
+
 def edit_image(image, brightness=None, contrast=None, sharpness=None):
     if brightness is not None:
         image = ImageEnhance.Brightness(image).enhance(brightness)
     if contrast is not None:
         image = ImageEnhance.Contrast(image).enhance(contrast)
     if sharpness is not None:
         image = ImageEnhance.Sharpness(image).enhance(sharpness)
@@ -104,43 +127,25 @@
     }
     if filter_name in filters:
         return filters[filter_name]
     return image
 
 
 @click.group()
-@click.version_option(version="1.2.0")
+@click.version_option(version="1.2.3")
 def cli():
     """💠 Use this Open AI api to generate, as well as customize : edit & filter images from the cmd line."""
 
 
 @click.command("img2img")
 @click.argument('input_file')
-@click.option('--n', default=2, help='Number of variations to generate')
-def generate_variations(input_file, n, save_path=None):
-    try:
-        with console.status("Generating image...", spinner="dots8Bit"):
-            response = openai.Image.create_variation(
-                image=open(input_file, "rb"),
-                n=n,
-                size="1024x1024"
-            )
-            image_data = requests.get(
-                response.get("data")[0]["url"], timeout=300
-            ).content
-            image = Image.open(BytesIO(image_data))
-            image.show()
-            if save_path is not None:
-                if not path.exists(path.dirname(save_path)):
-                    makedirs(path.dirname(save_path))
-                image.save(save_path)
-    except openai.error.AuthenticationError:
-        print("🔒 Authentication Failed. Try with a fresh API key.")
-    except Exception:
-        print("❌ Failed to generate image. Please try again with a different prompt.")
+@click.option('--n', default=2,type=int, help='Number of variations to generate')
+def generate_img(input_file, numVars):
+    configure_openai()
+    generate_variations(input_file=input_file, n=numVars)
 
 
 @cli.command("generate")
 @click.option(
     "--prompt",
     default="Suprise me",
     prompt=True,
@@ -286,8 +291,7 @@
 def get_unique_filename(filename):
     name, ext = path.splitext(filename)
     i = 1
     while path.exists(filename):
         filename = f"{name}_{i}{ext}"
         i += 1
     return filename
-
```

### Comparing `imggencli-1.2.2/PKG-INFO` & `imggencli-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.2
+Version: 1.2.3
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.2/README.md` & `imggencli-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `imggencli-1.2.2/imggencli.egg-info/PKG-INFO` & `imggencli-1.2.3/imggencli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imggencli
-Version: 1.2.2
+Version: 1.2.3
 Summary: A command line application to generate customized images based on the Open AI API.
 Home-page: https://github.com/shayan-shaikh/Image-generation-CLI
 Author: Shayan Shaikh
 Author-email: Shaikhshayan1@gmail.com
 License: Open Source
 Keywords: cli,developer tools,productivity,openai,generative art,ai
 Requires-Python: >3.5
```

### Comparing `imggencli-1.2.2/setup.py` & `imggencli-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = file.read()
 
 
 setup(
     name="imggencli",
     python_requires=">3.5",
     options={"bdist_wheel": {"universal": "1"}},
-    version="1.2.2",
+    version="1.2.3",
     description="A command line application to generate customized images based on the Open AI API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shayan-shaikh/Image-generation-CLI",
     author="Shayan Shaikh",
     license="Open Source",
     author_email="Shaikhshayan1@gmail.com",
```

