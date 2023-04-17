# Comparing `tmp/markdownlit-0.0.6.tar.gz` & `tmp/markdownlit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownlit-0.0.6.tar", last modified: Fri Apr  7 13:11:15 2023, max compression
+gzip compressed data, was "markdownlit-0.0.7.tar", last modified: Mon Apr 17 21:19:08 2023, max compression
```

## Comparing `markdownlit-0.0.6.tar` & `markdownlit-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:11:15.823478 markdownlit-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-07 13:10:57.000000 markdownlit-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-04-07 13:11:15.823478 markdownlit-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-07 13:10:57.000000 markdownlit-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:11:15.823478 markdownlit-0.0.6/markdownlit/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-07 13:10:57.000000 markdownlit-0.0.6/markdownlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:11:15.823478 markdownlit-0.0.6/markdownlit/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-07 13:10:57.000000 markdownlit-0.0.6/markdownlit/extensions/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-07 13:10:57.000000 markdownlit-0.0.6/markdownlit/extensions/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-07 13:10:57.000000 markdownlit-0.0.6/markdownlit/extensions/at_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-07 13:10:57.000000 markdownlit-0.0.6/markdownlit/extensions/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-07 13:10:57.000000 markdownlit-0.0.6/markdownlit/extensions/double_dash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:11:15.823478 markdownlit-0.0.6/markdownlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-04-07 13:11:15.000000 markdownlit-0.0.6/markdownlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 13:11:15.000000 markdownlit-0.0.6/markdownlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 13:11:15.000000 markdownlit-0.0.6/markdownlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-07 13:11:15.000000 markdownlit-0.0.6/markdownlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 13:11:15.000000 markdownlit-0.0.6/markdownlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-07 13:10:57.000000 markdownlit-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 13:11:15.823478 markdownlit-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:19:08.562228 markdownlit-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 21:18:46.000000 markdownlit-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-04-17 21:19:08.562228 markdownlit-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-17 21:18:46.000000 markdownlit-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:19:08.558228 markdownlit-0.0.7/markdownlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-17 21:18:46.000000 markdownlit-0.0.7/markdownlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:19:08.562228 markdownlit-0.0.7/markdownlit/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-17 21:18:46.000000 markdownlit-0.0.7/markdownlit/extensions/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 21:18:46.000000 markdownlit-0.0.7/markdownlit/extensions/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-17 21:18:46.000000 markdownlit-0.0.7/markdownlit/extensions/at_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-17 21:18:46.000000 markdownlit-0.0.7/markdownlit/extensions/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-17 21:18:46.000000 markdownlit-0.0.7/markdownlit/extensions/double_dash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:19:08.558228 markdownlit-0.0.7/markdownlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-04-17 21:19:08.000000 markdownlit-0.0.7/markdownlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 21:19:08.000000 markdownlit-0.0.7/markdownlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:19:08.000000 markdownlit-0.0.7/markdownlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-17 21:19:08.000000 markdownlit-0.0.7/markdownlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 21:19:08.000000 markdownlit-0.0.7/markdownlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 21:18:46.000000 markdownlit-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:19:08.562228 markdownlit-0.0.7/setup.cfg
```

### Comparing `markdownlit-0.0.6/LICENSE` & `markdownlit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownlit-0.0.6/PKG-INFO` & `markdownlit-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownlit
-Version: 0.0.6
+Version: 0.0.7
 Summary: markdownlit adds a couple of lit Markdown capabilities to your Streamlit apps
 Author-email: Arnaud Miribel <arnaudmiribel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `markdownlit-0.0.6/README.md` & `markdownlit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `markdownlit-0.0.6/markdownlit/__init__.py` & `markdownlit-0.0.7/markdownlit/__init__.py`

 * *Files identical despite different names*

### Comparing `markdownlit-0.0.6/markdownlit/extensions/align.py` & `markdownlit-0.0.7/markdownlit/extensions/align.py`

 * *Files identical despite different names*

### Comparing `markdownlit-0.0.6/markdownlit/extensions/arrow.py` & `markdownlit-0.0.7/markdownlit/extensions/arrow.py`

 * *Files identical despite different names*

### Comparing `markdownlit-0.0.6/markdownlit/extensions/at_sign.py` & `markdownlit-0.0.7/markdownlit/extensions/at_sign.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,21 +65,21 @@
         if html.find("</style>") != -1:
             html = html[html.find("</style>") + len("</style>") :]
         el = ET.ElementTree(ET.fromstring(str(html))).getroot()
         el.set("style", "display: inline; color:inherit; text-decoration:inherit;")
         return el, m.start(0), m.end(0)
 
     @staticmethod
-    @st.cache_data
+    @cache_data
     def _get_favicon(url: str) -> str:
         favicons = favicon.get(url, timeout=2)
         return favicons[0].url
 
     @staticmethod
-    @st.cache_data
+    @cache_data
     def _get_page_title(url: str) -> str:
         n = requests.get(url)
         al = n.text
         return al[al.find("<title>") + 7 : al.find("</title>")]
 
     def _guess_icon_and_label(self, url: str) -> Tuple[str, str]:
         """Find out plausible icon and label from URL alone
```

### Comparing `markdownlit-0.0.6/markdownlit/extensions/color.py` & `markdownlit-0.0.7/markdownlit/extensions/color.py`

 * *Files identical despite different names*

### Comparing `markdownlit-0.0.6/markdownlit/extensions/double_dash.py` & `markdownlit-0.0.7/markdownlit/extensions/double_dash.py`

 * *Files identical despite different names*

### Comparing `markdownlit-0.0.6/markdownlit.egg-info/PKG-INFO` & `markdownlit-0.0.7/markdownlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownlit
-Version: 0.0.6
+Version: 0.0.7
 Summary: markdownlit adds a couple of lit Markdown capabilities to your Streamlit apps
 Author-email: Arnaud Miribel <arnaudmiribel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `markdownlit-0.0.6/pyproject.toml` & `markdownlit-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "markdownlit"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Arnaud Miribel", email="arnaudmiribel@gmail.com" },
 ]
 description = "markdownlit adds a couple of lit Markdown capabilities to your Streamlit apps"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

