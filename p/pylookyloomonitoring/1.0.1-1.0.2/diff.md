# Comparing `tmp/pylookyloomonitoring-1.0.1.tar.gz` & `tmp/pylookyloomonitoring-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylookyloomonitoring-1.0.1.tar", max compression
+gzip compressed data, was "pylookyloomonitoring-1.0.2.tar", max compression
```

## Comparing `pylookyloomonitoring-1.0.1.tar` & `pylookyloomonitoring-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.1/LICENSE
--rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.0.1/README.md
--rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.0.1/pylookyloomonitoring/__init__.py
--rw-r--r--   0        0        0     6159 2023-03-30 11:12:42.787394 pylookyloomonitoring-1.0.1/pylookyloomonitoring/api.py
--rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.1/pylookyloomonitoring/py.typed
--rw-r--r--   0        0        0     1461 2023-03-30 11:13:45.555804 pylookyloomonitoring-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.2/LICENSE
+-rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.0.2/README.md
+-rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.0.2/pylookyloomonitoring/__init__.py
+-rw-r--r--   0        0        0     6376 2023-04-17 12:01:59.260660 pylookyloomonitoring-1.0.2/pylookyloomonitoring/api.py
+-rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.2/pylookyloomonitoring/py.typed
+-rw-r--r--   0        0        0     1461 2023-04-17 12:03:18.353656 pylookyloomonitoring-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.0.2/PKG-INFO
```

### Comparing `pylookyloomonitoring-1.0.1/LICENSE` & `pylookyloomonitoring-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.1/README.md` & `pylookyloomonitoring-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.1/pylookyloomonitoring/__init__.py` & `pylookyloomonitoring-1.0.2/pylookyloomonitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.1/pylookyloomonitoring/api.py` & `pylookyloomonitoring-1.0.2/pylookyloomonitoring/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import logging
+
 from importlib.metadata import version
-from datetime import datetime
+from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Dict, Optional, List, Any, Union, TypedDict
 from urllib.parse import urljoin, urlparse
 
 import requests
 
 
@@ -76,14 +78,15 @@
 
         if not urlparse(self.root_url).scheme:
             self.root_url = 'http://' + self.root_url
         if not self.root_url.endswith('/'):
             self.root_url += '/'
         self.session = requests.session()
         self.session.headers['user-agent'] = useragent if useragent else f'PyLookylooMonitoring / {version("pylookyloomonitoring")}'
+        self.logger = logging.getLogger(f'{self.__class__.__name__}')
 
     @property
     def is_up(self) -> bool:
         '''Test if the given instance is accessible'''
         try:
             r = self.session.head(self.root_url)
         except requests.exceptions.ConnectionError:
@@ -159,15 +162,16 @@
         if expire_at:
             if isinstance(expire_at, (str, int, float)):
                 _expire = float(expire_at)
             if isinstance(expire_at, datetime):
                 _expire = expire_at.timestamp()
             if _expire < datetime.now().timestamp():
                 # The expiration time is in the past.
-                raise TimeError('Expiration time in the past.')
+                self.logger.warning(f'Expiration time in the past ({expire_at}), forcing it to tomorrow.')
+                _expire = (datetime.now() + timedelta(hours=24)).timestamp()
             to_post['expire_at'] = _expire
         if collection:
             to_post['collection'] = collection
 
         if compare_settings:
             to_post['compare_settings'] = compare_settings
```

### Comparing `pylookyloomonitoring-1.0.1/pyproject.toml` & `pylookyloomonitoring-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylookyloomonitoring"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python API to connect to lookyloo monitoring"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PyLookylooMonitoring"
 documentation = "https://pylookyloomonitoring.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
@@ -36,16 +36,16 @@
 requests = "^2.28.2"
 Sphinx = { version = "^6.1.3", optional = true }
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^2.17.1"
-mypy = "^1.1.1"
+pylint = "^2.17.2"
+mypy = "^1.2.0"
 types-requests = "^2.28.11.17"
-ipython = "^8.11.0"
-pytest = "^7.2.2"
+ipython = "^8.12.0"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pylookyloomonitoring-1.0.1/PKG-INFO` & `pylookyloomonitoring-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookyloomonitoring
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API to connect to lookyloo monitoring
 Home-page: https://github.com/Lookyloo/PyLookylooMonitoring
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

