# Comparing `tmp/cmip-0.0.4.tar.gz` & `tmp/cmip-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmip-0.0.4.tar", last modified: Fri Apr 14 09:56:29 2023, max compression
+gzip compressed data, was "cmip-0.0.5.tar", last modified: Mon Apr 17 02:48:33 2023, max compression
```

## Comparing `cmip-0.0.4.tar` & `cmip-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.783858 cmip-0.0.4/
--rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      493 2023-04-14 09:56:29.782848 cmip-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      113 2022-12-15 09:05:59.000000 cmip-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.739760 cmip-0.0.4/cmip/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.753844 cmip-0.0.4/cmip/data/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/data/ad.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/data/chinese_frequency.tsv
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/data/letter_mapping.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/data/pinyin.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.756849 cmip-0.0.4/cmip/gibberish/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/gibberish/__init__.py
--rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/gibberish/gibberish.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.757845 cmip-0.0.4/cmip/image/
--rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.765846 cmip-0.0.4/cmip/text/
--rw-rw-rw-   0        0        0     2882 2023-04-14 09:40:30.000000 cmip-0.0.4/cmip/text/__init__.py
--rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.4/cmip/text/ac_automation.py
--rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/text/normalize.py
--rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/text/similarity.py
--rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.4/cmip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.773845 cmip-0.0.4/cmip/web/
--rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.4/cmip/web/__init__.py
--rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.4/cmip/web/html.py
--rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/web/simhash_utils.py
--rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/web/utils.py
--rw-rw-rw-   0        0        0     3331 2023-04-14 09:54:31.000000 cmip-0.0.4/cmip/web/web_scraping.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.777849 cmip-0.0.4/cmip/word_discover/
--rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/word_discover/__init__.py
--rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/word_discover/ngram.py
--rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.4/cmip/word_discover/word_discover.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.748757 cmip-0.0.4/cmip.egg-info/
--rw-rw-rw-   0        0        0      493 2023-04-14 09:56:29.000000 cmip-0.0.4/cmip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-04-14 09:56:29.000000 cmip-0.0.4/cmip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:56:29.000000 cmip-0.0.4/cmip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-14 09:56:29.000000 cmip-0.0.4/cmip.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 09:56:29.000000 cmip-0.0.4/cmip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 09:56:29.783858 cmip-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-14 09:56:01.000000 cmip-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:56:29.780847 cmip-0.0.4/test/
--rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.4/test/__init__.py
--rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.4/test/test_ac_automation.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.547712 cmip-0.0.5/
+-rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1128 2023-04-17 02:48:33.545710 cmip-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-04-17 02:44:31.000000 cmip-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.509003 cmip-0.0.5/cmip/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.519984 cmip-0.0.5/cmip/data/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/ad.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/chinese_frequency.tsv
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/letter_mapping.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/data/pinyin.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.521971 cmip-0.0.5/cmip/gibberish/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/gibberish/__init__.py
+-rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/gibberish/gibberish.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.523972 cmip-0.0.5/cmip/image/
+-rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.529977 cmip-0.0.5/cmip/text/
+-rw-rw-rw-   0        0        0     2882 2023-04-14 09:40:30.000000 cmip-0.0.5/cmip/text/__init__.py
+-rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.5/cmip/text/ac_automation.py
+-rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/text/normalize.py
+-rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/text/similarity.py
+-rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.5/cmip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.537704 cmip-0.0.5/cmip/web/
+-rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.5/cmip/web/__init__.py
+-rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.5/cmip/web/html.py
+-rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/web/simhash_utils.py
+-rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/web/utils.py
+-rw-rw-rw-   0        0        0     3445 2023-04-17 02:42:39.000000 cmip-0.0.5/cmip/web/web_scraping.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.540705 cmip-0.0.5/cmip/word_discover/
+-rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/word_discover/__init__.py
+-rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/word_discover/ngram.py
+-rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.5/cmip/word_discover/word_discover.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.515975 cmip-0.0.5/cmip.egg-info/
+-rw-rw-rw-   0        0        0     1128 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 02:48:33.000000 cmip-0.0.5/cmip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 02:48:33.547712 cmip-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-17 02:45:11.000000 cmip-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:48:33.542705 cmip-0.0.5/test/
+-rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.5/test/__init__.py
+-rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.5/test/test_ac_automation.py
```

### Comparing `cmip-0.0.4/LICENSE` & `cmip-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/gibberish/gibberish.py` & `cmip-0.0.5/cmip/gibberish/gibberish.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/image/__init__.py` & `cmip-0.0.5/cmip/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/text/__init__.py` & `cmip-0.0.5/cmip/text/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/text/ac_automation.py` & `cmip-0.0.5/cmip/text/ac_automation.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/text/normalize.py` & `cmip-0.0.5/cmip/text/normalize.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/text/similarity.py` & `cmip-0.0.5/cmip/text/similarity.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/utils.py` & `cmip-0.0.5/cmip/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/web/html.py` & `cmip-0.0.5/cmip/web/html.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/web/simhash_utils.py` & `cmip-0.0.5/cmip/web/simhash_utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/web/utils.py` & `cmip-0.0.5/cmip/web/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/web/web_scraping.py` & `cmip-0.0.5/cmip/web/web_scraping.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,83 +4,81 @@
 import aiofiles
 from io import BytesIO
 from PIL import Image
 from tqdm.asyncio import tqdm
 from cmip.web.utils import url2domain, decode_image
 
 
-async def event_handler_save_images(response, folder) -> None:
+async def event_handler_save_images(response, folder, min_img_size=200) -> None:
     try:
         content_type = response.headers.get("content-type", "")
         if content_type.startswith("image") and not content_type.startswith("image/svg"):
             image = await response.body()
             url = response.request.url
-            if len(image) > 200:
-                file_hash = hash(os.path.basename(url))
-                _path = os.path.join(folder, f"{file_hash}-{len(image)}.jpg")
+            if len(image) > min_img_size:
+                file_hash: int = hash(os.path.basename(url))
+                _path: str = os.path.join(folder, f"{file_hash}={len(image)}.jpg")
                 if url.endswith("webp"):
                     byte_stream = BytesIO(image)
                     im = Image.open(byte_stream)
                     im = im.convert("RGB")
                     im.save(_path)
                 else:
                     async with aiofiles.open(_path, 'wb') as f:
                         await f.write(image)
     except Exception as e:
         print(f"Error saving image: {response.request.url}, {e}")
 
 
-async def fetch_url(semaphore, url, folder, save_images=True):
+async def fetch_url(semaphore, browser, url, folder, save_image=True, min_img_size=200):
     async with semaphore:
-        async with async_playwright() as p:
-            browser = await p.chromium.launch()
-            context = await browser.new_context()
-            page = await context.new_page()
-            if save_images:
-                page.on("response", lambda response: asyncio.create_task(
-                    event_handler_save_images(response, folder)))
-            try:
-                await page.goto(url, wait_until="networkidle")
-                content = await page.content()
-
-                async with aiofiles.open(f"{folder}/dynamic.html", "w", encoding="utf-8") as f:
-                    await f.write(content)
-
-                images = await page.query_selector_all('img')
-                for idx, src in enumerate(
-                        set([await page.evaluate('(element) => element.src', image) for image in images])):
-                    if src.startswith("data:image"):
-                        async with aiofiles.open(os.path.join(folder, f"{idx}.jpg"), 'wb') as f:
-                            await f.write(decode_image(src))
-
-            except Exception as e:
-                print(f"Error fetching URL: {url}, {e}")
-
-            finally:
-                await page.close()
-                await context.close()
-                await browser.close()
+        context = await browser.new_context()
+        page = await context.new_page()
+        if save_image:
+            page.on("response", lambda response: asyncio.create_task(
+                event_handler_save_images(response, folder, min_img_size)))
+        try:
+            await page.goto(url, wait_until="networkidle")
+            content = await page.content()
+
+            async with aiofiles.open(os.path.join(folder, "dynamic.html"), "w", encoding="utf-8") as f:
+                await f.write(content)
+
+            images = await page.query_selector_all('img')
+            for idx, src in enumerate(
+                    set([await page.evaluate('(element) => element.src', image) for image in images])):
+                if src.startswith("data:image"):
+                    async with aiofiles.open(os.path.join(folder, f"{idx}.jpg"), 'wb') as f:
+                        await f.write(decode_image(src))
+
+        except Exception as e:
+            print(f"Error fetching URL: {url}, {e}")
+
+        finally:
+            await page.close()
+            await context.close()
 
 
-async def web_scraping(urls, output_path="output", max_concurrent_tasks=10):
+async def web_scraping(urls, output_path="output", max_concurrent_tasks=10, save_image=True, min_img_size=200):
     semaphore = asyncio.Semaphore(max_concurrent_tasks)
-
-    tasks = []
-    for i, url in enumerate(urls):
-        folder = f"{output_path}/{url2domain(url)}"
-        os.makedirs(folder, exist_ok=True)
-        tasks.append(fetch_url(semaphore, url, folder))
-
-    try:
-        for result in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Fetching URLs"):
-            await result
-    except Exception as e:
-        print(f"Error in main: {e}")
-    finally:
-        await semaphore.acquire()
+    async with async_playwright() as p:
+        browser = await p.chromium.launch()
+        tasks = []
+        for i, url in enumerate(urls):
+            folder = os.path.join(output_path, url2domain(url))
+            os.makedirs(folder, exist_ok=True)
+            tasks.append(fetch_url(semaphore, browser, url, folder, save_image, min_img_size))
+        try:
+            for result in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Fetching URLs"):
+                await result
+        except Exception as e:
+            print(f"Error in main: {e}")
+        finally:
+            await semaphore.acquire()
+            await browser.close()
 
 
 if __name__ == "__main__":
     urls = [
         "https://baidu.com",
         "https://qq.com",
         # ...更多的URL
```

### Comparing `cmip-0.0.4/cmip/word_discover/ngram.py` & `cmip-0.0.5/cmip/word_discover/ngram.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip/word_discover/word_discover.py` & `cmip-0.0.5/cmip/word_discover/word_discover.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/cmip.egg-info/SOURCES.txt` & `cmip-0.0.5/cmip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmip-0.0.4/setup.py` & `cmip-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cmip",
-    version="0.0.4",
+    version="0.0.5",
     author="geb",
     author_email="853934146@qq.com",
     description="An efficient information processing program.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikuh/cmip",
     packages=setuptools.find_packages(),
```

### Comparing `cmip-0.0.4/test/test_ac_automation.py` & `cmip-0.0.5/test/test_ac_automation.py`

 * *Files identical despite different names*

