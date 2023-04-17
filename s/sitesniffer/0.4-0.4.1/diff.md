# Comparing `tmp/sitesniffer-0.4.tar.gz` & `tmp/sitesniffer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesniffer-0.4.tar", last modified: Mon Apr 17 06:38:46 2023, max compression
+gzip compressed data, was "sitesniffer-0.4.1.tar", last modified: Mon Apr 17 13:17:36 2023, max compression
```

## Comparing `sitesniffer-0.4.tar` & `sitesniffer-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.404198 sitesniffer-0.4/
--rw-r--r--   0 jonahsimon   (501) staff       (20)     1069 2023-04-12 17:27:59.000000 sitesniffer-0.4/LICENCE
--rw-r--r--   0 jonahsimon   (501) staff       (20)     4415 2023-04-17 06:38:46.404003 sitesniffer-0.4/PKG-INFO
--rw-r--r--   0 jonahsimon   (501) staff       (20)     3850 2023-04-12 17:27:59.000000 sitesniffer-0.4/README.md
--rw-r--r--   0 jonahsimon   (501) staff       (20)      477 2023-04-12 17:27:59.000000 sitesniffer-0.4/pyproject.toml
--rw-r--r--   0 jonahsimon   (501) staff       (20)       38 2023-04-17 06:38:46.404268 sitesniffer-0.4/setup.cfg
--rw-r--r--   0 jonahsimon   (501) staff       (20)     1137 2023-04-17 06:35:31.000000 sitesniffer-0.4/setup.py
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.401775 sitesniffer-0.4/sitesniffer.egg-info/
--rw-r--r--   0 jonahsimon   (501) staff       (20)     4415 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/PKG-INFO
--rw-r--r--   0 jonahsimon   (501) staff       (20)      355 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/SOURCES.txt
--rw-r--r--   0 jonahsimon   (501) staff       (20)        1 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/dependency_links.txt
--rw-r--r--   0 jonahsimon   (501) staff       (20)       51 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/requires.txt
--rw-r--r--   0 jonahsimon   (501) staff       (20)       28 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/top_level.txt
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.399443 sitesniffer-0.4/src/
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.403227 sitesniffer-0.4/src/sitesniffer/
--rw-r--r--   0 jonahsimon   (501) staff       (20)      722 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/__init__.py
--rw-r--r--   0 jonahsimon   (501) staff       (20)    12167 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/_sitesniffer.py
--rw-r--r--   0 jonahsimon   (501) staff       (20)     4143 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/data.py
--rw-r--r--   0 jonahsimon   (501) staff       (20)      347 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/exceptions.py
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.403514 sitesniffer-0.4/tests/
--rw-r--r--   0 jonahsimon   (501) staff       (20)     6323 2023-04-12 17:27:59.000000 sitesniffer-0.4/tests/test_sitesniffer.py
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 13:17:36.661108 sitesniffer-0.4.1/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     1069 2023-04-17 13:10:38.000000 sitesniffer-0.4.1/LICENCE
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     4635 2023-04-17 13:17:36.660906 sitesniffer-0.4.1/PKG-INFO
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     4044 2023-04-17 13:10:36.000000 sitesniffer-0.4.1/README.md
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      477 2023-04-17 13:10:37.000000 sitesniffer-0.4.1/pyproject.toml
+-rw-r--r--   0 jonahsimon   (501) staff       (20)       38 2023-04-17 13:17:36.661172 sitesniffer-0.4.1/setup.cfg
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     1169 2023-04-17 13:17:34.000000 sitesniffer-0.4.1/setup.py
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 13:17:36.659898 sitesniffer-0.4.1/sitesniffer.egg-info/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     4635 2023-04-17 13:17:36.000000 sitesniffer-0.4.1/sitesniffer.egg-info/PKG-INFO
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      355 2023-04-17 13:17:36.000000 sitesniffer-0.4.1/sitesniffer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonahsimon   (501) staff       (20)        1 2023-04-17 13:17:36.000000 sitesniffer-0.4.1/sitesniffer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonahsimon   (501) staff       (20)       51 2023-04-17 13:17:36.000000 sitesniffer-0.4.1/sitesniffer.egg-info/requires.txt
+-rw-r--r--   0 jonahsimon   (501) staff       (20)       28 2023-04-17 13:17:36.000000 sitesniffer-0.4.1/sitesniffer.egg-info/top_level.txt
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 13:17:36.658354 sitesniffer-0.4.1/src/
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 13:17:36.660483 sitesniffer-0.4.1/src/sitesniffer/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      724 2023-04-17 13:16:47.000000 sitesniffer-0.4.1/src/sitesniffer/__init__.py
+-rw-r--r--   0 jonahsimon   (501) staff       (20)    12167 2023-04-12 17:27:59.000000 sitesniffer-0.4.1/src/sitesniffer/_sitesniffer.py
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     4143 2023-04-12 17:27:59.000000 sitesniffer-0.4.1/src/sitesniffer/data.py
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      347 2023-04-12 17:27:59.000000 sitesniffer-0.4.1/src/sitesniffer/exceptions.py
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 13:17:36.660625 sitesniffer-0.4.1/tests/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     6323 2023-04-12 17:27:59.000000 sitesniffer-0.4.1/tests/test_sitesniffer.py
```

### Comparing `sitesniffer-0.4/LICENCE` & `sitesniffer-0.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `sitesniffer-0.4/PKG-INFO` & `sitesniffer-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: sitesniffer
-Version: 0.4
+Version: 0.4.1
 Summary: This is a Python script that can extract various information about a website, including its IP address, SSL certificate information, domain information, page load time, and other useful insights.
 Home-page: https://github.com/thisisjsimon/SiteSniffer
 Author: Jonah Simon
 Author-email: thisisjsimon.github@gmail.com
 License: MIT
 Keywords: sniffing,site sniffing,website sniffing,IP address,SSL certificate,domain,website
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 # Site Sniffer in Python 🐽
 
 [![PyPi version](https://img.shields.io/pypi/v/sitesniffer)](https://pypi.org/project/sitesniffer/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![PyPi downloads](https://img.shields.io/pypi/dm/sitesniffer)](https://pypi.org/project/sitesniffer/)
 [![Github commits](https://img.shields.io/github/commit-activity/m/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/commits/main)
 [![Github contributors](https://img.shields.io/github/contributors/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/graphs/contributors)
 [![Code size](https://img.shields.io/github/languages/code-size/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+
 Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.
 
 ## Installation
 
 Install sitesniffer with pip:
 
 ```bash
@@ -34,14 +37,18 @@
 
 ```bash
 pip install git+https://github.com/thisisjsimon/SiteSniffer.git
 ```
 
 ## Usage
 
+ Make sure that you have installed Python 3.11 before proceeding.
+ 
+
+
 To use SiteSniffer, you need to import it first:
 
 ```py
 from sitesniffer import SiteSniffer
 ```
 
 Then, create an instance of the SiteSniffer class by providing the URL of the website you want to analyze:
```

### Comparing `sitesniffer-0.4/README.md` & `sitesniffer-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Site Sniffer in Python 🐽
 
 [![PyPi version](https://img.shields.io/pypi/v/sitesniffer)](https://pypi.org/project/sitesniffer/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![PyPi downloads](https://img.shields.io/pypi/dm/sitesniffer)](https://pypi.org/project/sitesniffer/)
 [![Github commits](https://img.shields.io/github/commit-activity/m/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/commits/main)
 [![Github contributors](https://img.shields.io/github/contributors/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/graphs/contributors)
 [![Code size](https://img.shields.io/github/languages/code-size/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+
 Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.
 
 ## Installation
 
 Install sitesniffer with pip:
 
 ```bash
@@ -21,14 +23,18 @@
 
 ```bash
 pip install git+https://github.com/thisisjsimon/SiteSniffer.git
 ```
 
 ## Usage
 
+ Make sure that you have installed Python 3.11 before proceeding.
+ 
+
+
 To use SiteSniffer, you need to import it first:
 
 ```py
 from sitesniffer import SiteSniffer
 ```
 
 Then, create an instance of the SiteSniffer class by providing the URL of the website you want to analyze:
```

### Comparing `sitesniffer-0.4/setup.py` & `sitesniffer-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description: str = readme.read()
 
 setup(
     name="sitesniffer",
-    version="0.4",
+    version="0.4.1",
     description="This is a Python script that can extract various information about a website, including its IP address, SSL certificate information, domain information, page load time, and other useful insights.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thisisjsimon/SiteSniffer",
     author="Jonah Simon",
     author_email="thisisjsimon.github@gmail.com",
     license="MIT",
@@ -27,8 +27,9 @@
         "site sniffing",
         "website sniffing",
         "IP address",
         "SSL certificate",
         "domain",
         "website",
     ],
+    python_requires=">=3.11",
 )
```

### Comparing `sitesniffer-0.4/sitesniffer.egg-info/PKG-INFO` & `sitesniffer-0.4.1/sitesniffer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: sitesniffer
-Version: 0.4
+Version: 0.4.1
 Summary: This is a Python script that can extract various information about a website, including its IP address, SSL certificate information, domain information, page load time, and other useful insights.
 Home-page: https://github.com/thisisjsimon/SiteSniffer
 Author: Jonah Simon
 Author-email: thisisjsimon.github@gmail.com
 License: MIT
 Keywords: sniffing,site sniffing,website sniffing,IP address,SSL certificate,domain,website
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 # Site Sniffer in Python 🐽
 
 [![PyPi version](https://img.shields.io/pypi/v/sitesniffer)](https://pypi.org/project/sitesniffer/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![PyPi downloads](https://img.shields.io/pypi/dm/sitesniffer)](https://pypi.org/project/sitesniffer/)
 [![Github commits](https://img.shields.io/github/commit-activity/m/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/commits/main)
 [![Github contributors](https://img.shields.io/github/contributors/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/graphs/contributors)
 [![Code size](https://img.shields.io/github/languages/code-size/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+
 Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.
 
 ## Installation
 
 Install sitesniffer with pip:
 
 ```bash
@@ -34,14 +37,18 @@
 
 ```bash
 pip install git+https://github.com/thisisjsimon/SiteSniffer.git
 ```
 
 ## Usage
 
+ Make sure that you have installed Python 3.11 before proceeding.
+ 
+
+
 To use SiteSniffer, you need to import it first:
 
 ```py
 from sitesniffer import SiteSniffer
 ```
 
 Then, create an instance of the SiteSniffer class by providing the URL of the website you want to analyze:
```

### Comparing `sitesniffer-0.4/src/sitesniffer/__init__.py` & `sitesniffer-0.4.1/src/sitesniffer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This module provides a SiteSniffer class that can extract various pieces of information from a given URL. 
 The class can extract the protocol, hostname, path, IP address, domain information, HTTP status code, SSL certificate information, page load time, and URLs on a page.
 """
 from __future__ import annotations
 
 __all__: list[str] = ["SiteSniffer"]
-__version__: str = "0.4"
+__version__: str = "0.4.1"
 __author__: str = "Jonah Simon"
 __email__ = "thisisjsimon.github@gmail.com"
 __title__: str = "sitesniffer"
 __license__: str = "MIT"
 __copyright__: str = "Copyright (c) 2023 thisisjsimon"
 
 from ._sitesniffer import SiteSniffer
```

### Comparing `sitesniffer-0.4/src/sitesniffer/_sitesniffer.py` & `sitesniffer-0.4.1/src/sitesniffer/_sitesniffer.py`

 * *Files identical despite different names*

### Comparing `sitesniffer-0.4/src/sitesniffer/data.py` & `sitesniffer-0.4.1/src/sitesniffer/data.py`

 * *Files identical despite different names*

### Comparing `sitesniffer-0.4/tests/test_sitesniffer.py` & `sitesniffer-0.4.1/tests/test_sitesniffer.py`

 * *Files identical despite different names*

