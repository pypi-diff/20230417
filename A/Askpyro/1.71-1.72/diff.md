# Comparing `tmp/Askpyro-1.71.tar.gz` & `tmp/Askpyro-1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Askpyro-1.71.tar", last modified: Mon Apr 17 05:42:17 2023, max compression
+gzip compressed data, was "Askpyro-1.72.tar", last modified: Mon Apr 17 06:08:00 2023, max compression
```

## Comparing `Askpyro-1.71.tar` & `Askpyro-1.72.tar`

### file list

```diff
@@ -1,11 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:42:17.739234 Askpyro-1.71/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 05:42:17.739234 Askpyro-1.71/Askpyro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 05:42:17.000000 Askpyro-1.71/Askpyro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 05:41:57.000000 Askpyro-1.71/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 05:42:17.739234 Askpyro-1.71/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1933 2023-04-17 05:41:57.000000 Askpyro-1.71/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 05:42:17.739234 Askpyro-1.71/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3084 2023-04-17 05:41:57.000000 Askpyro-1.71/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.071849 Askpyro-1.72/Askpyro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 06:07:59.000000 Askpyro-1.72/Askpyro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      367 2023-04-17 06:08:00.000000 Askpyro-1.72/Askpyro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 06:07:59.000000 Askpyro-1.72/Askpyro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 06:07:59.000000 Askpyro-1.72/Askpyro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 06:07:36.000000 Askpyro-1.72/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 06:08:00.075849 Askpyro-1.72/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-04-17 06:07:36.000000 Askpyro-1.72/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/askpyro/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5553 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/askpyro/helpers/
+-rw-r--r--   0 root         (0) root         (0)      814 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/examples/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/buttons.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/callback.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/filters.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/start.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 06:08:00.075849 Askpyro-1.72/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-04-17 06:07:36.000000 Askpyro-1.72/setup.py
```

### Comparing `Askpyro-1.71/Askpyro.egg-info/PKG-INFO` & `Askpyro-1.72/Askpyro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.71
+Version: 1.72
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
-Metadata-Version: 2.1 Name: Askpyro Version: 1.71 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.72 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
 telegram chat messenger mtproto api client library python Platform: UNKNOWN
```

### Comparing `Askpyro-1.71/LICENSE` & `Askpyro-1.72/LICENSE`

 * *Files identical despite different names*

### Comparing `Askpyro-1.71/PKG-INFO` & `Askpyro-1.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.71
+Version: 1.72
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
-Metadata-Version: 2.1 Name: Askpyro Version: 1.71 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.72 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
 telegram chat messenger mtproto api client library python Platform: UNKNOWN
```

### Comparing `Askpyro-1.71/README.md` & `Askpyro-1.72/README.md`

 * *Files identical despite different names*

### Comparing `Askpyro-1.71/setup.py` & `Askpyro-1.72/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,35 +14,30 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Askpyro.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
 from sys import argv
-
+import setuptools
 from setuptools import setup, find_packages
 
 
 
-#with open("requirements.txt", encoding="utf-8") as r:
-    #requires = [i.strip() for i in r]
-
-with open("askpyro/__init__.py", encoding="utf-8") as f:
-    version = re.findall(r"__version__ = \"(.+)\"", f.read())[0]
-
-with open("README.md", encoding="utf-8") as f:
-    readme = f.read()
+with open("README.md", encoding="utf8") as readme:
+    long_description = readme.read()
 
 
 
-setup(
+setuptools.setup(
     name="Askpyro",
-    version=version,
+    packages=setuptools.find_packages(),
+    version="1.72",
     description="Easy conversation handler for pyrogram",
-    long_description=readme,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Askpyro/releases/latest",
     author="Abishnoi",
     author_email="abishnoi@askpyro.org",
     license="LGPLv3",
     classifiers=[
```

