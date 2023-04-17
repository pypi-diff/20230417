# Comparing `tmp/PrSpiders-0.2.9.tar.gz` & `tmp/PrSpiders-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.2.9.tar", last modified: Mon Apr 17 02:59:42 2023, max compression
+gzip compressed data, was "PrSpiders-0.3.0.tar", last modified: Mon Apr 17 09:57:56 2023, max compression
```

## Comparing `PrSpiders-0.2.9.tar` & `PrSpiders-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:42.018781 PrSpiders-0.2.9/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0     4465 2023-04-17 02:59:42.017781 PrSpiders-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.843785 PrSpiders-0.2.9/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.2.9/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.2.9/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11166 2023-04-17 02:59:19.000000 PrSpiders-0.2.9/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3995 2023-04-07 07:28:46.000000 PrSpiders-0.2.9/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.9/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.880778 PrSpiders-0.2.9/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4465 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3953 2023-04-12 08:30:03.000000 PrSpiders-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.890780 PrSpiders-0.2.9/pkg/
--rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.2.9/pkg/__init.py
--rw-rw-rw-   0        0        0        0 2023-04-12 08:12:31.000000 PrSpiders-0.2.9/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.924789 PrSpiders-0.2.9/pkg/prspider/
--rw-rw-rw-   0        0        0     1161 2023-04-12 08:15:15.000000 PrSpiders-0.2.9/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      259 2023-03-31 06:17:29.000000 PrSpiders-0.2.9/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.2.9/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      490 2023-04-12 08:17:20.000000 PrSpiders-0.2.9/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.986785 PrSpiders-0.2.9/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.2.9/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.2.9/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.2.9/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.9/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-04-17 02:59:42.019782 PrSpiders-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:19.000000 PrSpiders-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:42.004783 PrSpiders-0.2.9/table_parse/
--rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.2.9/table_parse/T.py
--rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.2.9/table_parse/__init__.py
--rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.2.9/table_parse/tb_parse.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:57:56.715401 PrSpiders-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4465 2023-04-17 09:57:56.712405 PrSpiders-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 09:57:56.641397 PrSpiders-0.3.0/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.0/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.0/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11166 2023-04-17 02:59:19.000000 PrSpiders-0.3.0/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4196 2023-04-17 09:57:49.000000 PrSpiders-0.3.0/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.0/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:57:56.662397 PrSpiders-0.3.0/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4465 2023-04-17 09:57:56.000000 PrSpiders-0.3.0/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-04-17 09:57:56.000000 PrSpiders-0.3.0/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:57:56.000000 PrSpiders-0.3.0/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-17 09:57:56.000000 PrSpiders-0.3.0/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-17 09:57:56.000000 PrSpiders-0.3.0/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-17 09:57:56.000000 PrSpiders-0.3.0/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3953 2023-04-12 08:30:03.000000 PrSpiders-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:57:56.671403 PrSpiders-0.3.0/pkg/
+-rw-rw-rw-   0        0        0        0 2023-04-17 09:57:16.000000 PrSpiders-0.3.0/pkg/__init.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 09:57:16.000000 PrSpiders-0.3.0/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:57:56.683398 PrSpiders-0.3.0/pkg/prspider/
+-rw-rw-rw-   0        0        0        0 2023-04-17 09:57:16.000000 PrSpiders-0.3.0/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 09:57:16.000000 PrSpiders-0.3.0/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 09:57:16.000000 PrSpiders-0.3.0/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 09:57:16.000000 PrSpiders-0.3.0/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:57:56.697400 PrSpiders-0.3.0/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.3.0/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.3.0/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.3.0/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.0/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:57:56.715401 PrSpiders-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-04-17 09:57:49.000000 PrSpiders-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:57:56.708398 PrSpiders-0.3.0/table_parse/
+-rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.3.0/table_parse/T.py
+-rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.3.0/table_parse/__init__.py
+-rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.3.0/table_parse/tb_parse.py
```

### Comparing `PrSpiders-0.2.9/LICENSE.txt` & `PrSpiders-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/PKG-INFO` & `PrSpiders-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.9
+Version: 0.3.0
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.2.9/PrSpider/PrSpiders.py` & `PrSpiders-0.3.0/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/PrSpider/pxpath.py` & `PrSpiders-0.3.0/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/PrSpider/requestXpath.py` & `PrSpiders-0.3.0/PrSpider/requestXpath.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,30 +58,34 @@
         self.current_time = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         header = self.header
         self.method = method.upper()
         self.retry_time = retry_time
         self.retry_interval = retry_interval
         self.meta_ = meta
         if headers and isinstance(headers, dict):
+            if headers.get('user-agent') or headers.get('User-Agent'):
+                header = {}
             header.update(headers)
+            print(header)
         while True:
             try:
                 self.response = requests.request(
                     url=url, headers=header, timeout=timeout, method=self.method, *args, **kwargs)
                 self.response.encoding = encoding
-                if self.response.status_code == 200:
+                if self.response.ok:
                     return self
                 else:
                     raise Exception(f'Respider {self.retry_interval}s')
             except Exception as e:
                 logging.error('%s [ERRORS] [Url] %s [Msg] %s' % (self.current_time, url, e))
-                logging.info('[Retry Url] %s [Interval] %ss' % (url, retry_interval))
+                if settion.retry:
+                    logging.info('[Retry Url] %s [Interval] %ss' % (url, retry_interval))
                 retry_time -= 1
                 if retry_time <= 0 or settion.retry is False:
-                    self.response.status_code = 405
+                    self.response.status_code = 410 if not self.response.status_code else self.response.status_code
                     return self
                 time.sleep(retry_interval)
 
     @property
     def text(self):
         return self.response.text
 
@@ -131,8 +135,8 @@
     def meta(self):
         return self.meta_
 
     def close(self):
         self.response.close()
 
     def __str__(self) -> str:
-        return f"<{type(self).__name__} code={self.code} len={self.get_len}>"
+        return f"<Request Code={self.code} Len={self.get_len}>"
```

### Comparing `PrSpiders-0.2.9/PrSpider/useragent.py` & `PrSpiders-0.3.0/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.3.0/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.9
+Version: 0.3.0
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.2.9/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.3.0/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/README.md` & `PrSpiders-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/requestXpath/__init__.py` & `PrSpiders-0.3.0/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/requestXpath/pxpath.py` & `PrSpiders-0.3.0/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/requestXpath/requestXpath.py` & `PrSpiders-0.3.0/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/requestXpath/useragent.py` & `PrSpiders-0.3.0/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/setup.py` & `PrSpiders-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
-__version__ = '0.2.9'
+__version__ = '0.3.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

### Comparing `PrSpiders-0.2.9/table_parse/T.py` & `PrSpiders-0.3.0/table_parse/T.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.9/table_parse/tb_parse.py` & `PrSpiders-0.3.0/table_parse/tb_parse.py`

 * *Files identical despite different names*

