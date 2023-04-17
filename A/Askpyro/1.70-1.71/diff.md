# Comparing `tmp/Askpyro-1.70.tar.gz` & `tmp/Askpyro-1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Askpyro-1.70.tar", last modified: Mon Apr 17 04:24:10 2023, max compression
+gzip compressed data, was "Askpyro-1.71.tar", last modified: Mon Apr 17 05:42:17 2023, max compression
```

## Comparing `Askpyro-1.70.tar` & `Askpyro-1.71.tar`

### file list

```diff
@@ -1,26 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.336058 Askpyro-1.70/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.332059 Askpyro-1.70/Askpyro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 04:19:08.000000 Askpyro-1.70/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 04:24:10.336058 Askpyro-1.70/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1933 2023-04-17 04:19:08.000000 Askpyro-1.70/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.332059 Askpyro-1.70/askpyro/
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5553 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/conversation.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.332059 Askpyro-1.70/askpyro/helpers/
--rw-r--r--   0 root         (0) root         (0)      814 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.336058 Askpyro-1.70/examples/
--rw-r--r--   0 root         (0) root         (0)      161 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/buttons.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/callback.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/filters.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/start.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 04:24:10.336058 Askpyro-1.70/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3252 2023-04-17 04:24:06.000000 Askpyro-1.70/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:42:17.739234 Askpyro-1.71/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:42:17.739234 Askpyro-1.71/Askpyro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 05:41:57.000000 Askpyro-1.71/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 05:42:17.739234 Askpyro-1.71/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-04-17 05:41:57.000000 Askpyro-1.71/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 05:42:17.739234 Askpyro-1.71/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-04-17 05:41:57.000000 Askpyro-1.71/setup.py
```

### Comparing `Askpyro-1.70/Askpyro.egg-info/PKG-INFO` & `Askpyro-1.71/Askpyro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.70
+Version: 1.71
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.70 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.71 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
 telegram chat messenger mtproto api client library python Platform: UNKNOWN
```

### Comparing `Askpyro-1.70/LICENSE` & `Askpyro-1.71/LICENSE`

 * *Files identical despite different names*

### Comparing `Askpyro-1.70/PKG-INFO` & `Askpyro-1.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.70
+Version: 1.71
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.70 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.71 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
 telegram chat messenger mtproto api client library python Platform: UNKNOWN
```

### Comparing `Askpyro-1.70/README.md` & `Askpyro-1.71/README.md`

 * *Files identical despite different names*

### Comparing `Askpyro-1.70/setup.py` & `Askpyro-1.71/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import re
 from sys import argv
 
 from setuptools import setup, find_packages
 
 
 
-with open("requirements.txt", encoding="utf-8") as r:
-    requires = [i.strip() for i in r]
+#with open("requirements.txt", encoding="utf-8") as r:
+    #requires = [i.strip() for i in r]
 
 with open("askpyro/__init__.py", encoding="utf-8") as f:
     version = re.findall(r"__version__ = \"(.+)\"", f.read())[0]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
@@ -72,14 +72,8 @@
     project_urls={
         "Tracker": "https://github.com/Abishnoi69/Askpyro/issues",
         "Community": "https://t.me/AbishnoiMF",
         "Source": "https://github.com/Abishnoi69/Askpyro",
         "Documentation": "https://github.com/Abishnoi69/askpyro/wiki",
     },
     python_requires="~=3.7",
-    package_data={
-        "Askpyro": ["py.typed"],
-    },
-    packages=find_packages(exclude=["compiler*", "tests*"]),
-    zip_safe=False,
-    install_requires=requires
 )
```

