# Comparing `tmp/sitesniffer-0.3.2.tar.gz` & `tmp/sitesniffer-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesniffer-0.3.2.tar", last modified: Sat Apr  1 17:51:44 2023, max compression
+gzip compressed data, was "sitesniffer-0.4.tar", last modified: Mon Apr 17 06:38:46 2023, max compression
```

## Comparing `sitesniffer-0.3.2.tar` & `sitesniffer-0.4.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-01 17:51:44.435123 sitesniffer-0.3.2/
--rw-r--r--   0 jonahsimon   (501) staff       (20)     1095 2023-03-31 18:52:33.000000 sitesniffer-0.3.2/LICENCE
--rw-r--r--   0 jonahsimon   (501) staff       (20)     3825 2023-04-01 17:51:44.434933 sitesniffer-0.3.2/PKG-INFO
--rw-r--r--   0 jonahsimon   (501) staff       (20)     3350 2023-04-01 11:01:09.000000 sitesniffer-0.3.2/README.md
--rw-r--r--   0 jonahsimon   (501) staff       (20)      458 2023-04-01 16:30:07.000000 sitesniffer-0.3.2/pyproject.toml
--rw-r--r--   0 jonahsimon   (501) staff       (20)       38 2023-04-01 17:51:44.435197 sitesniffer-0.3.2/setup.cfg
--rw-r--r--   0 jonahsimon   (501) staff       (20)      922 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/setup.py
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-01 17:51:44.431454 sitesniffer-0.3.2/sitesniffer/
--rw-r--r--   0 jonahsimon   (501) staff       (20)       42 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/sitesniffer/__init__.py
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-01 17:51:44.434184 sitesniffer-0.3.2/sitesniffer/src/
--rw-r--r--   0 jonahsimon   (501) staff       (20)      796 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/sitesniffer/src/__init__.py
--rw-r--r--   0 jonahsimon   (501) staff       (20)     9073 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/sitesniffer/src/_sitesniffer.py
--rw-r--r--   0 jonahsimon   (501) staff       (20)      740 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/sitesniffer/src/data.py
--rw-r--r--   0 jonahsimon   (501) staff       (20)      324 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/sitesniffer/src/exceptions.py
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-01 17:51:44.434649 sitesniffer-0.3.2/sitesniffer/tests/
--rw-r--r--   0 jonahsimon   (501) staff       (20)        0 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/sitesniffer/tests/__init__.py
--rw-r--r--   0 jonahsimon   (501) staff       (20)        0 2023-04-01 17:34:21.000000 sitesniffer-0.3.2/sitesniffer/tests/test_sitesniffer.py
-drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-01 17:51:44.432942 sitesniffer-0.3.2/sitesniffer.egg-info/
--rw-r--r--   0 jonahsimon   (501) staff       (20)     3825 2023-04-01 17:51:44.000000 sitesniffer-0.3.2/sitesniffer.egg-info/PKG-INFO
--rw-r--r--   0 jonahsimon   (501) staff       (20)      421 2023-04-01 17:51:44.000000 sitesniffer-0.3.2/sitesniffer.egg-info/SOURCES.txt
--rw-r--r--   0 jonahsimon   (501) staff       (20)        1 2023-04-01 17:51:44.000000 sitesniffer-0.3.2/sitesniffer.egg-info/dependency_links.txt
--rw-r--r--   0 jonahsimon   (501) staff       (20)       44 2023-04-01 17:51:44.000000 sitesniffer-0.3.2/sitesniffer.egg-info/requires.txt
--rw-r--r--   0 jonahsimon   (501) staff       (20)       12 2023-04-01 17:51:44.000000 sitesniffer-0.3.2/sitesniffer.egg-info/top_level.txt
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.404198 sitesniffer-0.4/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     1069 2023-04-12 17:27:59.000000 sitesniffer-0.4/LICENCE
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     4415 2023-04-17 06:38:46.404003 sitesniffer-0.4/PKG-INFO
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     3850 2023-04-12 17:27:59.000000 sitesniffer-0.4/README.md
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      477 2023-04-12 17:27:59.000000 sitesniffer-0.4/pyproject.toml
+-rw-r--r--   0 jonahsimon   (501) staff       (20)       38 2023-04-17 06:38:46.404268 sitesniffer-0.4/setup.cfg
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     1137 2023-04-17 06:35:31.000000 sitesniffer-0.4/setup.py
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.401775 sitesniffer-0.4/sitesniffer.egg-info/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     4415 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/PKG-INFO
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      355 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonahsimon   (501) staff       (20)        1 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonahsimon   (501) staff       (20)       51 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/requires.txt
+-rw-r--r--   0 jonahsimon   (501) staff       (20)       28 2023-04-17 06:38:46.000000 sitesniffer-0.4/sitesniffer.egg-info/top_level.txt
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.399443 sitesniffer-0.4/src/
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.403227 sitesniffer-0.4/src/sitesniffer/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      722 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/__init__.py
+-rw-r--r--   0 jonahsimon   (501) staff       (20)    12167 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/_sitesniffer.py
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     4143 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/data.py
+-rw-r--r--   0 jonahsimon   (501) staff       (20)      347 2023-04-12 17:27:59.000000 sitesniffer-0.4/src/sitesniffer/exceptions.py
+drwxr-xr-x   0 jonahsimon   (501) staff       (20)        0 2023-04-17 06:38:46.403514 sitesniffer-0.4/tests/
+-rw-r--r--   0 jonahsimon   (501) staff       (20)     6323 2023-04-12 17:27:59.000000 sitesniffer-0.4/tests/test_sitesniffer.py
```

### Comparing `sitesniffer-0.3.2/LICENCE` & `sitesniffer-0.4/LICENCE`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MIT License
 
 Copyright (c) 2023 thisisjsimon
-Copyright (c) 2023 shouzy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sitesniffer-0.3.2/PKG-INFO` & `sitesniffer-0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,122 @@
 Metadata-Version: 2.1
 Name: sitesniffer
-Version: 0.3.2
+Version: 0.4
 Summary: This is a Python script that can extract various information about a website, including its IP address, SSL certificate information, domain information, page load time, and other useful insights.
 Home-page: https://github.com/thisisjsimon/SiteSniffer
 Author: Jonah Simon
 Author-email: thisisjsimon.github@gmail.com
 License: MIT
+Keywords: sniffing,site sniffing,website sniffing,IP address,SSL certificate,domain,website
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 # Site Sniffer in Python 🐽
 
-Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.
+[![PyPi version](https://img.shields.io/pypi/v/sitesniffer)](https://pypi.org/project/sitesniffer/)
+[![PyPi downloads](https://img.shields.io/pypi/dm/sitesniffer)](https://pypi.org/project/sitesniffer/)
+[![Github commits](https://img.shields.io/github/commit-activity/m/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/commits/main)
+[![Github contributors](https://img.shields.io/github/contributors/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/graphs/contributors)
+[![Code size](https://img.shields.io/github/languages/code-size/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-#
+Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.
 
 ## Installation
 
-Install sitesniffer with pip
+Install sitesniffer with pip:
+
+```bash
+pip install sitesniffer
+```
+
+Alternativly:
 
 ```bash
-  pip install sitesniffer
+pip install git+https://github.com/thisisjsimon/SiteSniffer.git
 ```
 
 ## Usage
+
 To use SiteSniffer, you need to import it first:
-```bash
-  from sitesniffer import SiteSniffer
+
+```py
+from sitesniffer import SiteSniffer
 ```
 
 Then, create an instance of the SiteSniffer class by providing the URL of the website you want to analyze:
-```bash
-  sniffer = SiteSniffer('https://example.com')
+
+```py
+sniffer = SiteSniffer('https://example.com')
 ```
 
 You can then call the methods of the SiteSniffer object to get various details about the website:
-```bash
-  print(sniffer.ip_address())
-  print(sniffer.domain_info())
-  print(sniffer.status_code())
-  # See docs for full list
+
+```py
+print(sniffer.ip_address())
+print(sniffer.domain_info())
+print(sniffer.status_code())
+# See docs for full list
 ```
 
 Each of the methods in this package returns the corresponding detail of the website. For example, get_ip_address() returns the IP address of the website.
 
 ## Example
 
-```bash
-  from sitesniffer import SiteSniffer
+```py
+from sitesniffer import SiteSniffer
 
-  sniffer = SiteSniffer('https://google.com')
-  print(sniffer.ip_address())
+sniffer = SiteSniffer('https://google.com')
+print(sniffer.ip_address())
 ```
-## Output
-```bash
-  142.250.185.110
+
+### Output
+
+```py
+'142.250.185.110'
 ```
-#
 
 ## Essential Python Libraries for Web Scraping and HTTP Requests
 
-The following Python libraries are essential for working with the Site Sniffer package:
-
-* requests: used for sending HTTP requests and receiving responses.
-* socket, ssl, and idna: used for working with IP addresses and SSL certificates.
-* whois: used for querying WHOIS information for a domain.
-* re: used for working with regular expressions.
-* time: used for timing how long it takes to load a webpage.
-* BeautifulSoup: used for parsing HTML.
+The following Python libraries are essential for working with the ``sitesniffer`` package:
 
+```py
+# standard library
+import re
+import socket
+import ssl
+import time
+import typing
+import urllib.parse
+import dataclasses
+
+# third party
+import bs4
+import idna
+import requests
+import whois
+```
 
+## Docs
 
-## The defined functions included (docs):
+### The defined functions included in ``SiteSniffer``
 
 | Function Name  | Function Description |
 | ------------- | ------------- |
-| SiteSniffer | A class for extracting information about a website, such as its IP address, SSL certificate information, and load time. |
-| extract_protocol | Extracts the protocol from the URL. |
-| extract_hostname | Extracts the hostname from the URL. |
-| extract_path | Extracts the path from the URL. |
-| ip_address | Returns the IP address of the domain. |
-| domain_info | Returns the domain information for the website. |
-| status_code | Returns the HTTP status code of the website. |
-| ssl_info | Returns the SSL certificate information for the website. |
-| load_time | Returns the website's load time. |
-| links | Returns a list of links found on the website. |
-| is_mobile_friendly | Checks if the website is mobile-friendly. |
-| has_responsive_design | Checks if the website has a responsive design. |
-| has_cookies | Checks if the website uses cookies. |
-| has_google_analytics | Checks if the website has Google Analytics installed. |
-| page_meta_description | Returns the website's meta description. |
-| has_meta_description | Checks if the website has a meta description. |
-| page_keywords | Returns the website's keywords. |
-| has_keywords | Checks if the website has keywords. |
-
-#
-[![License: MIT](https://img.shields.io/badge/License-MIT-darkgrey.svg)](https://opensource.org/licenses/MIT)
+| ``extract_protocol`` | Extracts the protocol from the URL. |
+| ``extract_hostname`` | Extracts the hostname from the URL. |
+| ``extract_path`` | Extracts the path from the URL. |
+| ``ip_address`` | Returns the IP address of the domain. |
+| ``domain_info`` | Returns the domain information for the website. |
+| ``status_code`` | Returns the HTTP status code of the website. |
+| ``ssl_info`` | Returns the SSL certificate information for the website. |
+| ``load_time`` | Returns the website's load time. |
+| ``links`` | Returns a list of links found on the website. |
+| ``is_mobile_friendly`` | Checks if the website is mobile-friendly. |
+| ``has_responsive_design`` | Checks if the website has a responsive design. |
+| ``has_cookies`` | Checks if the website uses cookies. |
+| ``has_google_analytics`` | Checks if the website has Google Analytics installed. |
+| ``page_meta_description`` | Returns the website's meta description. |
+| ``has_meta_description`` | Checks if the website has a meta description. |
+| ``page_keywords`` | Returns the website's keywords. |
+| ``has_keywords`` | Checks if the website has keywords. |
```

### Comparing `sitesniffer-0.3.2/setup.py` & `sitesniffer-0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,34 @@
+#!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 from __future__ import annotations
 
-from setuptools import find_packages, setup
+from setuptools import setup
 
-from sitesniffer.src import __author__, __license__, __title__, __version__
-
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description: str = f.read()
+with open("README.md", "r", encoding="utf-8") as readme:
+    long_description: str = readme.read()
 
 setup(
-    name=__title__,
-    version=__version__,
+    name="sitesniffer",
+    version="0.4",
     description="This is a Python script that can extract various information about a website, including its IP address, SSL certificate information, domain information, page load time, and other useful insights.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thisisjsimon/SiteSniffer",
-    author=__author__,
+    author="Jonah Simon",
     author_email="thisisjsimon.github@gmail.com",
-    license=__license__,
-    packages=find_packages(),
-    install_requires=["whois", "bs4", "idna", "requests"],
+    license="MIT",
+    packages=["sitesniffer"],
+    package_dir={"sitesniffer": "src/sitesniffer"},
+    py_modules=["exceptions", "data"],
+    install_requires=["python-whois", "bs4", "idna", "requests"],
     extras_require={"dev": ["pytest", "twine"]},
+    keywords=[
+        "sniffing",
+        "site sniffing",
+        "website sniffing",
+        "IP address",
+        "SSL certificate",
+        "domain",
+        "website",
+    ],
 )
```

### Comparing `sitesniffer-0.3.2/sitesniffer/src/__init__.py` & `sitesniffer-0.4/src/sitesniffer/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+#!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 """SiteSniffer - A tool to extract various information from a given URL
 
 This module provides a SiteSniffer class that can extract various pieces of information from a given URL. 
 The class can extract the protocol, hostname, path, IP address, domain information, HTTP status code, SSL certificate information, page load time, and URLs on a page.
 """
 from __future__ import annotations
 
-__all__: list[str] = ["SiteSniffer", "DomainInfo", "SiteSnifferException"]
-__version__: str = "0.3.2"
+__all__: list[str] = ["SiteSniffer"]
+__version__: str = "0.4"
 __author__: str = "Jonah Simon"
+__email__ = "thisisjsimon.github@gmail.com"
 __title__: str = "sitesniffer"
 __license__: str = "MIT"
-__copyright__: str = "Copyright (c) 2023 thisisjsimon\nCopyright (c) 2023 shouzy"
+__copyright__: str = "Copyright (c) 2023 thisisjsimon"
 
 from ._sitesniffer import SiteSniffer
-from .data import DomainInfo
-from .exceptions import SiteSnifferException
```

### Comparing `sitesniffer-0.3.2/sitesniffer.egg-info/PKG-INFO` & `sitesniffer-0.4/sitesniffer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,122 @@
 Metadata-Version: 2.1
 Name: sitesniffer
-Version: 0.3.2
+Version: 0.4
 Summary: This is a Python script that can extract various information about a website, including its IP address, SSL certificate information, domain information, page load time, and other useful insights.
 Home-page: https://github.com/thisisjsimon/SiteSniffer
 Author: Jonah Simon
 Author-email: thisisjsimon.github@gmail.com
 License: MIT
+Keywords: sniffing,site sniffing,website sniffing,IP address,SSL certificate,domain,website
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 # Site Sniffer in Python 🐽
 
-Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.
+[![PyPi version](https://img.shields.io/pypi/v/sitesniffer)](https://pypi.org/project/sitesniffer/)
+[![PyPi downloads](https://img.shields.io/pypi/dm/sitesniffer)](https://pypi.org/project/sitesniffer/)
+[![Github commits](https://img.shields.io/github/commit-activity/m/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/commits/main)
+[![Github contributors](https://img.shields.io/github/contributors/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer/graphs/contributors)
+[![Code size](https://img.shields.io/github/languages/code-size/thisisjsimon/SiteSniffer)](https://github.com/thisisjsimon/SiteSniffer)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-#
+Site Sniffer is a Python package designed to extract information about a website by providing its URL. It is useful for individuals who need to perform website analysis, including web developers, SEO specialists, and website owners. The package extracts various details such as the IP address, HTTP status code, SSL certificate information, domain registration details, load time, meta description, keywords, and a list of links on the page.
 
 ## Installation
 
-Install sitesniffer with pip
+Install sitesniffer with pip:
+
+```bash
+pip install sitesniffer
+```
+
+Alternativly:
 
 ```bash
-  pip install sitesniffer
+pip install git+https://github.com/thisisjsimon/SiteSniffer.git
 ```
 
 ## Usage
+
 To use SiteSniffer, you need to import it first:
-```bash
-  from sitesniffer import SiteSniffer
+
+```py
+from sitesniffer import SiteSniffer
 ```
 
 Then, create an instance of the SiteSniffer class by providing the URL of the website you want to analyze:
-```bash
-  sniffer = SiteSniffer('https://example.com')
+
+```py
+sniffer = SiteSniffer('https://example.com')
 ```
 
 You can then call the methods of the SiteSniffer object to get various details about the website:
-```bash
-  print(sniffer.ip_address())
-  print(sniffer.domain_info())
-  print(sniffer.status_code())
-  # See docs for full list
+
+```py
+print(sniffer.ip_address())
+print(sniffer.domain_info())
+print(sniffer.status_code())
+# See docs for full list
 ```
 
 Each of the methods in this package returns the corresponding detail of the website. For example, get_ip_address() returns the IP address of the website.
 
 ## Example
 
-```bash
-  from sitesniffer import SiteSniffer
+```py
+from sitesniffer import SiteSniffer
 
-  sniffer = SiteSniffer('https://google.com')
-  print(sniffer.ip_address())
+sniffer = SiteSniffer('https://google.com')
+print(sniffer.ip_address())
 ```
-## Output
-```bash
-  142.250.185.110
+
+### Output
+
+```py
+'142.250.185.110'
 ```
-#
 
 ## Essential Python Libraries for Web Scraping and HTTP Requests
 
-The following Python libraries are essential for working with the Site Sniffer package:
-
-* requests: used for sending HTTP requests and receiving responses.
-* socket, ssl, and idna: used for working with IP addresses and SSL certificates.
-* whois: used for querying WHOIS information for a domain.
-* re: used for working with regular expressions.
-* time: used for timing how long it takes to load a webpage.
-* BeautifulSoup: used for parsing HTML.
+The following Python libraries are essential for working with the ``sitesniffer`` package:
 
+```py
+# standard library
+import re
+import socket
+import ssl
+import time
+import typing
+import urllib.parse
+import dataclasses
+
+# third party
+import bs4
+import idna
+import requests
+import whois
+```
 
+## Docs
 
-## The defined functions included (docs):
+### The defined functions included in ``SiteSniffer``
 
 | Function Name  | Function Description |
 | ------------- | ------------- |
-| SiteSniffer | A class for extracting information about a website, such as its IP address, SSL certificate information, and load time. |
-| extract_protocol | Extracts the protocol from the URL. |
-| extract_hostname | Extracts the hostname from the URL. |
-| extract_path | Extracts the path from the URL. |
-| ip_address | Returns the IP address of the domain. |
-| domain_info | Returns the domain information for the website. |
-| status_code | Returns the HTTP status code of the website. |
-| ssl_info | Returns the SSL certificate information for the website. |
-| load_time | Returns the website's load time. |
-| links | Returns a list of links found on the website. |
-| is_mobile_friendly | Checks if the website is mobile-friendly. |
-| has_responsive_design | Checks if the website has a responsive design. |
-| has_cookies | Checks if the website uses cookies. |
-| has_google_analytics | Checks if the website has Google Analytics installed. |
-| page_meta_description | Returns the website's meta description. |
-| has_meta_description | Checks if the website has a meta description. |
-| page_keywords | Returns the website's keywords. |
-| has_keywords | Checks if the website has keywords. |
-
-#
-[![License: MIT](https://img.shields.io/badge/License-MIT-darkgrey.svg)](https://opensource.org/licenses/MIT)
+| ``extract_protocol`` | Extracts the protocol from the URL. |
+| ``extract_hostname`` | Extracts the hostname from the URL. |
+| ``extract_path`` | Extracts the path from the URL. |
+| ``ip_address`` | Returns the IP address of the domain. |
+| ``domain_info`` | Returns the domain information for the website. |
+| ``status_code`` | Returns the HTTP status code of the website. |
+| ``ssl_info`` | Returns the SSL certificate information for the website. |
+| ``load_time`` | Returns the website's load time. |
+| ``links`` | Returns a list of links found on the website. |
+| ``is_mobile_friendly`` | Checks if the website is mobile-friendly. |
+| ``has_responsive_design`` | Checks if the website has a responsive design. |
+| ``has_cookies`` | Checks if the website uses cookies. |
+| ``has_google_analytics`` | Checks if the website has Google Analytics installed. |
+| ``page_meta_description`` | Returns the website's meta description. |
+| ``has_meta_description`` | Checks if the website has a meta description. |
+| ``page_keywords`` | Returns the website's keywords. |
+| ``has_keywords`` | Checks if the website has keywords. |
```

