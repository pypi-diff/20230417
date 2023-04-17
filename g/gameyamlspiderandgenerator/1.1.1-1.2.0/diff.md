# Comparing `tmp/gameyamlspiderandgenerator-1.1.1.tar.gz` & `tmp/gameyamlspiderandgenerator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.1.1.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.2.0.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.1.1.tar` & `gameyamlspiderandgenerator-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2023-04-14 04:39:09.582935 gameyamlspiderandgenerator-1.1.1/LICENSE
--rwxr-xr-x   0        0        0      809 2023-04-14 04:39:09.583123 gameyamlspiderandgenerator-1.1.1/README.md
--rwxr-xr-x   0        0        0      610 2023-04-14 04:39:09.583410 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0      980 2023-04-14 04:39:09.583612 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-04-14 04:39:09.583800 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-04-14 04:39:09.584087 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-04-14 04:39:09.584282 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     2365 2023-04-16 02:41:59.202807 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0       56 2023-04-14 04:39:09.584827 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2406 2023-04-14 04:39:09.585063 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     6406 2023-04-16 03:52:20.134307 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7531 2023-04-16 03:03:23.223332 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-04-14 04:39:09.585883 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1132 2023-04-16 04:31:11.710886 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1187 2023-04-16 02:34:35.339573 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1706 2023-04-16 02:46:20.126317 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-04-16 02:40:43.137333 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-04-16 02:40:42.901945 gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      617 2023-04-16 04:31:41.930635 gameyamlspiderandgenerator-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-14 04:39:09.582935 gameyamlspiderandgenerator-1.2.0/LICENSE
+-rwxr-xr-x   0        0        0      809 2023-04-14 04:39:09.583123 gameyamlspiderandgenerator-1.2.0/README.md
+-rwxr-xr-x   0        0        0      610 2023-04-14 04:39:09.583410 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0      980 2023-04-14 04:39:09.583612 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-04-14 04:39:09.583800 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-04-14 04:39:09.584087 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      194 2023-04-14 04:39:09.584282 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     2365 2023-04-16 02:41:59.202807 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0       56 2023-04-14 04:39:09.584827 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2406 2023-04-14 04:39:09.585063 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     6985 2023-04-17 07:30:56.959305 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7561 2023-04-17 06:48:24.156686 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-04-14 04:39:09.585883 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1133 2023-04-17 06:52:34.054978 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1447 2023-04-17 07:29:28.159875 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1908 2023-04-17 06:46:51.090830 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-04-16 02:40:43.137333 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-04-16 02:40:42.901945 gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      617 2023-04-17 07:35:59.555205 gameyamlspiderandgenerator-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.2.0/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.1.1/LICENSE` & `gameyamlspiderandgenerator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/README.md` & `gameyamlspiderandgenerator-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,18 @@
             ]
             if "name" in ii
         ][0]
         self.more_info = self.get_more_info()
         self.tag = self.get_tags()
 
     def get_thumbnail(self):
-        return self.soup.select_one("#header > img").attrs["src"]
+        th = self.soup.select_one("#header > img")
+        if th is None:
+            return None
+        return th.attrs["src"]
 
     def get_brief_desc(self):
         return (
             pss_dedent(self.data["aggregateRating"]["description"])
             if "description" in self.data["aggregateRating"]
             else None
         )
@@ -54,26 +57,26 @@
         temp = self.soup.select_one("div.columns > div.right_col.column > div.screenshot_list").select('a')
         return [i.attrs['href'] for i in temp]
 
     def get_desc(self):
         return pss_dedent(self.remove_query(html2text(
             str(self.soup.select_one("div.formatted_description.user_formatted")),
             bodywidth=0,
-        )).strip())
+        )).replace("\n"*4, "\n").strip())
 
     def get_platforms(self):
         repl = {
             "Windows": "windows",
             "macOS": "macos",
             "Linux": "linux",
             "Android": "android",
             "HTML5": "web",
             "iOS": "ios",
         }
-        platforms = self.more_info["Platforms"][0].split(",")
+        platforms = self.more_info["Platforms"][0].split(",") if "Platforms" in self.more_info else ["Windows"]
         return [repl[i.strip()] for i in platforms]
 
     def get_authors(self) -> list[dict]:
         temp = self.more_info["Author"]
         return [{"name": i, "role": "developer"} for i in temp]
 
     def get_tags(self) -> list[str]:
@@ -108,21 +111,31 @@
         return list(set(ret))
 
     def get_langs(self) -> list[str]:
         temp = self.more_info["Languages"] if "Languages" in self.more_info else ["English"]
         return list(set(find(i).language for i in temp))
 
     def get_links(self) -> list[dict]:
-        link = [i.attrs["href"] for i in self.soup.select("a[href]")]
-        data = list(set(link))
-        return [
-            {"name": p["prefix"], "uri": sub(p["match"], p["replace"], i)}
-            for i, p in itertools.product(data, fgi_dict)
-            if match(p["match"], i)
-        ]
+        link = [i.attrs["href"] for i in self.soup.select_one("div.left_col.column > div.formatted_description.user_formatted").select("a[href]")]
+        data = [{"url": i, "processed": False} for i in list(set(link))]
+        processed_data = []
+        for i in data:
+            for p in fgi_dict:
+                if re.match(p["match"], i["url"]):
+                    processed_data.append(
+                        {
+                            "name": p["prefix"],
+                            "uri": re.sub(p["match"], p["replace"], i["url"]),
+                        }
+                    )
+                    i["processed"] = True
+        for i in data:
+            if not i["processed"]:
+                processed_data.append({"name": ".website", "uri": i["url"]})
+        return processed_data
 
     def get_more_info(self):
         d = {}
         for i in range(1, 18):
             with suppress(Exception):
                 cache = self.soup.select_one(
                     f"div.info_panel_wrapper > div > table > tbody > tr:nth-child({str(i)})"
@@ -136,16 +149,14 @@
 
         temp = data.copy()
         for _ in pkg["hook"].values():
             temp = pkg["hook"].Search(self.get_name()).setup(temp)
         return temp
 
     def to_yaml(self) -> YamlData:
-        if type(self.data) == int:
-            return self.data
         ret = {
             "name": self.get_name(),
             "brief-description": self.get_brief_desc(),
             "description": self.get_desc(),
             "description-format": "markdown",
             "authors": self.get_authors(),
             "tags": {
```

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             self.remove_query(
                 (
                     html2text(
                         self.data[str(self.id)]["data"]["detailed_description"],
                         bodywidth=0,
                     )
                 )
-            )
+            ).replace("\n"*4, "\n").strip()
         )
 
     def get_brief_desc(self):
         return pss_dedent(
             html2text(self.data[str(self.id)]["data"]["short_description"], bodywidth=0)
         )
```

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         # Compatibility with the old version
         return self.__getattribute__(item)
 
     def __setitem__(self, key, value):
         # Compatibility with the old version
         self.__setattr__(key, value)
 
+
     def load(self, file_data: str | dict | None):
         if type(file_data) is dict:
             self.__dict__.update(file_data)
             return
         if file_data is None:
             self.__dict__.update(default_config)
             return
```

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,24 @@
         "replace": "discord:\\g<1>",
     },
     {
         "match": "https://www.facebook.com/(.+)/",
         "prefix": ".facebook",
         "replace": "facebook:\\g<1>",
     },
+    {
+        "match": "https://www.furaffinity.net/user/(.+)/",
+        "prefix": ".furaffinity",
+        "replace": "furaffinity:\\g<1>",
+    },
+    {
+        "match": "(https://weibo.com/.+)",
+        "prefix": ".weibo",
+        "replace": "\\g<1>",
+    },
 ]
 default_config = {'api': {'apple': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90',
                           'google-play': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90'},
                   'gitToken': 'your token',
                   'hook': ['search'],
                   'plugin': ['steam', 'itchio'],
                   'proxy': {}}
```

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
+import re
 import zipfile
 from io import BytesIO
 from textwrap import dedent
-from typing import AnyStr
 
 from PIL import Image
 from loguru import logger
 from ruamel.yaml import YAML
 from ruamel.yaml.scalarstring import PreservedScalarString
 
 
-def pss_dedent(x: AnyStr) -> PreservedScalarString:
+def pss_dedent(x: str) -> PreservedScalarString:
     return PreservedScalarString(dedent(x))
 
 
 fgi = YAML(typ=["rt", "string"])
 fgi.indent(sequence=4, offset=2)
 fgi.preserve_quotes = True
 fgi.width = 4096
 
 
-def dump_to_yaml(data: dict) -> AnyStr:
+def dump_to_yaml(data: dict) -> str:
     temp = fgi.dump_to_string(data)
     for i in list(data.keys())[1:]:
         temp = temp.replace("\n" + i, "\n\n" + i)
     return temp
 
 
 def process_thumbnail(img_byte: bytes):
     img = Image.open(BytesIO(img_byte))
-    if img.size[0] % 360 == img.size[1] % 168 == 0:
+    if img.size[0] % 360 == img.size[1] % 168:
         img_resize = img.resize((360, 168))
         ret_byte = BytesIO()
         img_resize.save(ret_byte, format="PNG", optimize=True, quality=85)
         return ret_byte.getvalue()
     logger.warning("Thumbnails cannot be scaled down.")
     return img_byte
 
@@ -45,15 +45,21 @@
 
     def __str__(self):
         return dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'})
 
     def __bytes__(self):
         from ..util.spider import get_bytes
         _io = BytesIO()
-        img = get_bytes(self.raw_dict["thumbnail"])
         zip_data = zipfile.ZipFile(_io, 'w', zipfile.ZIP_STORED)
-        zip_data.writestr('thumbnail.png', process_thumbnail(img))
-
-        zip_data.writestr(self.raw_dict['name'] + ".yaml",
+        if self.raw_dict["thumbnail"] is not None:
+            img = get_bytes(self.raw_dict["thumbnail"])
+            zip_data.writestr('thumbnail.png', process_thumbnail(img))
+            logger.info("thumbnail exists")
+        zip_data.writestr(get_valid_filename(self.raw_dict['name']) + ".yaml",
                           dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'}))
         zip_data.close()
         return _io.getvalue()
+
+
+def get_valid_filename(s):
+    s = s.strip().replace(' ', '_')
+    return re.sub(r'(?u)[^-\w.]', '_', s)
```

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.2.0/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.1.1/pyproject.toml` & `gameyamlspiderandgenerator-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.1.1"
+version = "1.2.0"
 description = ""
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.1.1/PKG-INFO` & `gameyamlspiderandgenerator-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.1.1
+Version: 1.2.0
 Summary: 
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

