# Comparing `tmp/selenextra-1.0.tar.gz` & `tmp/selenextra-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-1.0.tar", last modified: Sat Apr 15 06:29:10 2023, max compression
+gzip compressed data, was "selenextra-1.0.2.tar", last modified: Mon Apr 17 06:35:59 2023, max compression
```

## Comparing `selenextra-1.0.tar` & `selenextra-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 06:29:10.658282 selenextra-1.0/
--rw-rw-rw-   0        0        0    35823 2023-04-15 06:25:51.000000 selenextra-1.0/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-15 06:29:10.657273 selenextra-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-15 06:25:51.000000 selenextra-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 06:29:10.651290 selenextra-1.0/selenextra/
--rw-rw-rw-   0        0        0     4629 2023-04-15 06:25:51.000000 selenextra-1.0/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-15 06:25:51.000000 selenextra-1.0/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-15 06:25:51.000000 selenextra-1.0/selenextra/patcher.py
-drwxrwxrwx   0        0        0        0 2023-04-15 06:29:10.656276 selenextra-1.0/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-15 06:29:10.000000 selenextra-1.0/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 06:29:10.658282 selenextra-1.0/setup.cfg
--rw-rw-rw-   0        0        0      780 2023-04-15 06:28:31.000000 selenextra-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:35:59.346557 selenextra-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-17 06:11:14.000000 selenextra-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      627 2023-04-17 06:35:59.345559 selenextra-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-17 06:11:14.000000 selenextra-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 06:35:59.339575 selenextra-1.0.2/selenextra/
+-rw-rw-rw-   0        0        0     4630 2023-04-17 06:35:09.000000 selenextra-1.0.2/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-17 06:11:14.000000 selenextra-1.0.2/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-17 06:11:14.000000 selenextra-1.0.2/selenextra/patcher.py
+drwxrwxrwx   0        0        0        0 2023-04-17 06:35:59.344560 selenextra-1.0.2/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      627 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 06:35:59.000000 selenextra-1.0.2/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 06:35:59.346557 selenextra-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-04-17 06:35:20.000000 selenextra-1.0.2/setup.py
```

### Comparing `selenextra-1.0/LICENSE` & `selenextra-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-1.0/PKG-INFO` & `selenextra-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 1.0
+Version: 1.0.2
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-1.0/selenextra/__init__.py` & `selenextra-1.0.2/selenextra/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from urllib.parse import urlparse
 from undetected_chromedriver import ChromeOptions
 from seleniumwire.undetected_chromedriver import Chrome
 from selenium.common.exceptions import TimeoutException
 from seleniumwire.request import Request, Response
 from typing import Union, Callable, Any, List, Tuple
 from .patcher import CustomPatcher
 from .exceptions import *
 
-import requests
+import json
 import re
 import random as rnd
 import time
 
 
 class ChromeDriver(Chrome):
     CONNECTION_TIMEOUT = 30
@@ -40,14 +41,29 @@
         return self.execute_script('return navigator.userAgent')
 
     def get_cookie_string(self) -> str:
         cookies = self.get_cookies()
         cookies = [f'{item["name"]}={item["value"]}' for item in cookies]
 
         return '; '.join(cookies) + ';'
+    
+    def get_browser_ip(self) -> str:
+        url = 'https://httpbin.org/ip'
+
+        try:
+            self.get(url)
+            
+            request = self.wait_for_request('/ip')
+            body = request.response.body.decode('utf-8')
+            data = json.loads(body)
+            ip = data['origin']
+        except:
+            raise RequestException(f"Error retrieving IP address from {url}")
+        
+        return ip
 
     def callback_with_timeout(self, callback: Callable[[Tuple], Any], params: tuple, timeout: Union[int, float] = 30) -> Any:
         end_time = time.time() + timeout
 
         while time.time() < end_time:
             result = callback(*params)
 
@@ -102,37 +118,20 @@
                 continue
 
             return callback(request) if callback else request
 
     def find_first_matching_request(self, paths: List[Tuple[str, Callable[[Request], Any]]], timeout: Union[int, float] = 30) -> Any:
         return self.callback_with_timeout(self._find_first_matching_request, (paths, ), timeout)
 
-    def add_proxy(self, proxy: str) -> Tuple[bool, str]:
-        proxy_dict = {}
-        proxy_type = proxy.split(':')[0]
-
-        if proxy_type == 'http':
-            proxy_dict['http'] = proxy
-            proxy_dict['https'] = proxy
-        elif proxy_type == 'https':
-            proxy_dict['http'] = f'{proxy.replace("https", "http")}'
-            proxy_dict['https'] = proxy
-
-        proxy_dict['no_proxy'] = 'localhost,127.0.0.1'
-
-        result = (False, None)
-
-        try:
-            resp = requests.get('https://httpbin.org/ip', proxies=proxy_dict)
-            if not resp.status_code == 200:
-                return result
-        except:
-            return result
-
-        self.proxy = proxy_dict
-        data = resp.json()
-
-        return True, data['origin']
+    def add_proxy(self, proxy: str) -> None:
+        scheme = urlparse(proxy).scheme
+        http_proxy = f'{proxy.replace("https", "http") if scheme == "https" else proxy}'
+
+        self.proxy = {
+            'http': http_proxy,
+            'https': proxy,
+            'no_proxy': 'localhost,127.0.0.1'
+        }
 
     def quit(self) -> None:
         super().quit()
         self.custom_patcher = None
```

### Comparing `selenextra-1.0/selenextra/patcher.py` & `selenextra-1.0.2/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-1.0/selenextra.egg-info/PKG-INFO` & `selenextra-1.0.2/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 1.0
+Version: 1.0.2
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

