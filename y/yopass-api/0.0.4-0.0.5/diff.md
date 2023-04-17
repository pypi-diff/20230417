# Comparing `tmp/yopass_api-0.0.4.tar.gz` & `tmp/yopass_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopass_api-0.0.4.tar", last modified: Sun Apr 16 16:29:04 2023, max compression
+gzip compressed data, was "yopass_api-0.0.5.tar", max compression
```

## Comparing `yopass_api-0.0.4.tar` & `yopass_api-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-16 16:29:04.119362 yopass_api-0.0.4/
--rw-rw-r--   0 xstl      (1000) xstl      (1000)     1075 2023-04-15 19:39:08.000000 yopass_api-0.0.4/LICENSE
--rw-rw-r--   0 xstl      (1000) xstl      (1000)     1383 2023-04-16 16:29:04.119362 yopass_api-0.0.4/PKG-INFO
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      821 2023-04-16 16:23:08.000000 yopass_api-0.0.4/README.md
--rw-rw-r--   0 xstl      (1000) xstl      (1000)       38 2023-04-16 16:29:04.131363 yopass_api-0.0.4/setup.cfg
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      955 2023-04-16 16:20:36.000000 yopass_api-0.0.4/setup.py
-drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-16 16:29:04.067362 yopass_api-0.0.4/yopass_api/
--rw-rw-r--   0 xstl      (1000) xstl      (1000)       26 2023-04-16 15:40:52.000000 yopass_api-0.0.4/yopass_api/__init__.py
--rw-rw-r--   0 xstl      (1000) xstl      (1000)     4912 2023-04-16 15:10:07.000000 yopass_api-0.0.4/yopass_api/yopass_api.py
-drwxrwxr-x   0 xstl      (1000) xstl      (1000)        0 2023-04-16 16:29:04.115363 yopass_api-0.0.4/yopass_api.egg-info/
--rw-rw-r--   0 xstl      (1000) xstl      (1000)     1383 2023-04-16 16:29:03.000000 yopass_api-0.0.4/yopass_api.egg-info/PKG-INFO
--rw-rw-r--   0 xstl      (1000) xstl      (1000)      253 2023-04-16 16:29:03.000000 yopass_api-0.0.4/yopass_api.egg-info/SOURCES.txt
--rw-rw-r--   0 xstl      (1000) xstl      (1000)        1 2023-04-16 16:29:03.000000 yopass_api-0.0.4/yopass_api.egg-info/dependency_links.txt
--rw-rw-r--   0 xstl      (1000) xstl      (1000)       29 2023-04-16 16:29:03.000000 yopass_api-0.0.4/yopass_api.egg-info/requires.txt
--rw-rw-r--   0 xstl      (1000) xstl      (1000)       11 2023-04-16 16:29:03.000000 yopass_api-0.0.4/yopass_api.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1096 2023-04-17 04:26:33.237964 yopass_api-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1039 2023-04-17 19:48:01.884801 yopass_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1018 2023-04-17 19:35:57.769174 yopass_api-0.0.5/README.md
+-rw-r--r--   0        0        0       27 2023-04-17 04:26:33.238965 yopass_api-0.0.5/yopass_api/__init__.py
+-rw-r--r--   0        0        0     5048 2023-04-17 17:57:13.344021 yopass_api-0.0.5/yopass_api/yopass_api.py
+-rw-r--r--   0        0        0     2071 1970-01-01 00:00:00.000000 yopass_api-0.0.5/PKG-INFO
```

### Comparing `yopass_api-0.0.4/LICENSE` & `yopass_api-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Sergey Ilyashevich
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Sergey Ilyashevich
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `yopass_api-0.0.4/PKG-INFO` & `yopass_api-0.0.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,34 @@
-Metadata-Version: 2.1
-Name: yopass_api
-Version: 0.0.4
-Summary: This module will allow you to use Python and Yopass in automation projects
-Home-page: https://github.com/silyashevich/yopass_api
-Author: Sergey Ilyashevich
-Author-email: silyashevich@gmail.com
-License: UNKNOWN
-Keywords: yopass,api,cryptography
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# yopass_api
-
-This is a module to work with a (the) [Yopass](https://github.com/jhaals/yopass) backend created by [Johan Haals](https://github.com/jhaals).
-This module will allow you to use Python and Yopass in automation projects.
-
-## Installing
-
-```py
-pip install yopass_api
-```
-
-## Basic Example
-
-This is a basic example of store secret, get link and fetch secret:
-
-```py
-from yopass_api import Yopass
-
-yopass = Yopass(api="http://your.yopass.backend:1024")
-secret_password = yopass.generate_passphrase(length=5)
-secret_id = yopass.store(
-    message="test",
-    password=secret_password,
-    expiration="1w",
-    one_time=False,
-)
-secret_url = yopass.secret_url(secret_id=secret_id, password=secret_password)
-print(secret_url)
-message = yopass.fetch(secret_id=secret_id, password=secret_password)
-print(message)
-
-```
-
-
+[![codecov](https://codecov.io/github/silyashevich/yopass_api/branch/main/graph/badge.svg?token=YDY235VL6Q)](https://codecov.io/github/silyashevich/yopass_api)
+
+# yopass_api
+
+This is a module to work with a (the) [Yopass](https://github.com/jhaals/yopass) backend created by [Johan Haals](https://github.com/jhaals).
+This module will allow you to use Python and self-hosted Yopass in automation projects.
+
+## Installing
+
+```py
+pip install yopass_api
+```
+
+## Basic Example
+
+This is a basic example of store secret, get link and fetch secret:
+
+```py
+from yopass_api import Yopass
+
+yopass = Yopass(api="https://api.yopass.se")
+secret_password = yopass.generate_passphrase(length=5)
+secret_id = yopass.store(
+    message="test",
+    password=secret_password,
+    expiration="1w",
+    one_time=False,
+)
+secret_url = yopass.secret_url(secret_id=secret_id, password=secret_password)
+print(secret_url)
+message = yopass.fetch(secret_id=secret_id, password=secret_password)
+print(message)
+
+```
```

### Comparing `yopass_api-0.0.4/yopass_api/yopass_api.py` & `yopass_api-0.0.5/yopass_api/yopass_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 from string import ascii_letters, digits
 from urllib.parse import urljoin
 
 import pgpy
 import requests
 from cryptography.utils import CryptographyDeprecationWarning
 
-warnings.filterwarnings("ignore", category=CryptographyDeprecationWarning)
-
 
 class Yopass:
     """Base class used by bound module functions."""
 
     def __init__(self, api: str, timeout=None):
         """Initialize an instance.
 
         Args:
             api (str): Yopass URL
             timeout: optional, see https://requests.readthedocs.io/en/latest/user/advanced/#timeouts
         """
+        warnings.filterwarnings("ignore", category=CryptographyDeprecationWarning)
         self.api = api
         self.timeout = timeout
 
     @property
     def api(self):
         """Сontains Yopass URL
 
@@ -59,24 +58,25 @@
         Returns:
             timeout, see https://requests.readthedocs.io/en/latest/user/advanced/#timeouts
         """
         return self._timeout
 
     @timeout.setter
     def timeout(self, value):
-        if not isinstance(
+        if not value or isinstance(
             value,
             (
                 int,
                 float,
                 tuple,
             ),
         ):
-            self._timeout = None
-        self._timeout = value
+            self._timeout = value
+        else:
+            raise ValueError("Invalid value: int/float/tuple expected")
 
     def generate_passphrase(self, length: int) -> str:
         """Simple password string generation (ASCII letters and digits)
 
         Args:
             length (int):
 
@@ -93,15 +93,19 @@
         Args:
             secret_id (str): secret identifier
             password (str): secret password
 
         Returns:
             str: URL
         """
-        return urljoin(self._api, f"/#/s/{secret_id}/{password}")
+        return (
+            urljoin(self._api, f"/#/s/{secret_id}/{password}")
+            if secret_id is not None
+            else None
+        )
 
     def store(self, message: str, password: str, expiration: str, one_time=True) -> str:
         """Store secret in Yopass
 
         Args:
             message (str): secret
             password (str): password
@@ -130,17 +134,17 @@
             response = requests.post(
                 urljoin(self._api, "/secret"),
                 data=payload,
                 headers=headers,
                 timeout=self.timeout,
             )
             response.raise_for_status()
-            return json.loads(response.text)["message"]
+            return response.json()["message"]
         except requests.exceptions.RequestException as _:
-            return None
+            return ""
 
     def fetch(self, secret_id: str, password: str) -> str:
         """Fetch secret from Yopass
 
         Args:
             secret_id (str): secret identifier
             password (str): password
@@ -155,13 +159,13 @@
         try:
             response = requests.get(
                 urljoin(self._api, f"/secret/{secret_id}"),
                 headers=headers,
                 timeout=self.timeout,
             )
             response.raise_for_status()
-            secret = pgpy.PGPMessage.from_blob(
-                json.loads(response.text)["message"]
-            ).decrypt(passphrase=password)
+            secret = pgpy.PGPMessage.from_blob(response.json()["message"]).decrypt(
+                passphrase=password
+            )
             return secret.message
         except requests.exceptions.RequestException as _:
-            return None
+            return ""
```

