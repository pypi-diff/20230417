# Comparing `tmp/PrSpiders-0.2.8.tar.gz` & `tmp/PrSpiders-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.2.8.tar", last modified: Wed Apr 12 08:13:45 2023, max compression
+gzip compressed data, was "PrSpiders-0.2.9.tar", last modified: Mon Apr 17 02:59:42 2023, max compression
```

## Comparing `PrSpiders-0.2.8.tar` & `PrSpiders-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.125501 PrSpiders-0.2.8/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4469 2023-04-12 08:13:45.123929 PrSpiders-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 08:13:44.966773 PrSpiders-0.2.8/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.2.8/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.2.8/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    10988 2023-04-07 07:28:46.000000 PrSpiders-0.2.8/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3995 2023-04-07 07:28:46.000000 PrSpiders-0.2.8/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.8/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:13:44.997774 PrSpiders-0.2.8/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4469 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-12 08:13:44.000000 PrSpiders-0.2.8/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3957 2023-04-10 01:15:21.000000 PrSpiders-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.003774 PrSpiders-0.2.8/pkg/
--rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.2.8/pkg/__init.py
--rw-rw-rw-   0        0        0        0 2023-04-12 08:12:31.000000 PrSpiders-0.2.8/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.018772 PrSpiders-0.2.8/pkg/prspider/
--rw-rw-rw-   0        0        0     1160 2023-04-12 08:12:59.000000 PrSpiders-0.2.8/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      259 2023-03-31 06:17:29.000000 PrSpiders-0.2.8/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.2.8/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      492 2023-03-31 06:15:13.000000 PrSpiders-0.2.8/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.093775 PrSpiders-0.2.8/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.2.8/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.2.8/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.2.8/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.8/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-04-12 08:13:45.126520 PrSpiders-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-04-12 08:12:59.000000 PrSpiders-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:13:45.109776 PrSpiders-0.2.8/table_parse/
--rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.2.8/table_parse/T.py
--rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.2.8/table_parse/__init__.py
--rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.2.8/table_parse/tb_parse.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:59:42.018781 PrSpiders-0.2.9/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4465 2023-04-17 02:59:42.017781 PrSpiders-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.843785 PrSpiders-0.2.9/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.2.9/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.2.9/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11166 2023-04-17 02:59:19.000000 PrSpiders-0.2.9/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3995 2023-04-07 07:28:46.000000 PrSpiders-0.2.9/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.9/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.880778 PrSpiders-0.2.9/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4465 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-17 02:59:41.000000 PrSpiders-0.2.9/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3953 2023-04-12 08:30:03.000000 PrSpiders-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.890780 PrSpiders-0.2.9/pkg/
+-rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.2.9/pkg/__init.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 08:12:31.000000 PrSpiders-0.2.9/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.924789 PrSpiders-0.2.9/pkg/prspider/
+-rw-rw-rw-   0        0        0     1161 2023-04-12 08:15:15.000000 PrSpiders-0.2.9/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      259 2023-03-31 06:17:29.000000 PrSpiders-0.2.9/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.2.9/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-04-12 08:17:20.000000 PrSpiders-0.2.9/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:59:41.986785 PrSpiders-0.2.9/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.2.9/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.2.9/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.2.9/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.2.9/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 02:59:42.019782 PrSpiders-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:19.000000 PrSpiders-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:59:42.004783 PrSpiders-0.2.9/table_parse/
+-rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.2.9/table_parse/T.py
+-rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.2.9/table_parse/__init__.py
+-rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.2.9/table_parse/tb_parse.py
```

### Comparing `PrSpiders-0.2.8/LICENSE.txt` & `PrSpiders-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/PKG-INFO` & `PrSpiders-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.8
+Version: 0.2.9
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,16 +33,14 @@
 | `data`           | `Type: dict or string`                          | `Request parameters`            |
 | `encoding`       | `Default: "utf-8" Type: string`                 | `Request Encoding`              |
 | `retry_time`     | `Default: 3 Type: int`                          | `Retry Count`                   |
 | `retry_interval` | `Default: 1 Type: int`                          | `Retry Interval`                |
 | `timeout`        | `Default: 3 Type: int`                          | `Request timeout`               |
 | `others`         | `*args or **kwargs`                             | `Follow Requests`               | 
 
-
-
 ## *Get started*
 
 Install Package: pip install requestXpath
 Make a request:
 
     from requestXpath import prequests
     url = 'https://gitee.com/'
```

### Comparing `PrSpiders-0.2.8/PrSpider/PrSpiders.py` & `PrSpiders-0.2.9/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/PrSpider/pxpath.py` & `PrSpiders-0.2.9/PrSpider/pxpath.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             return None
 
 
 class prxpath():
 
     def __init__(self, xp=None, xp_rule=None):
         self.xp = xp
+
         self._expr = xp_rule
 
     def getall(self):
         if isinstance(self.xp, list):
             self.xp = [prxpath(_, self._expr) for _ in self.xp]
         return self.xp
 
@@ -153,20 +154,20 @@
                 self.result = [f'{warps}'.join([replace(i) for i in _]) for _ in self.result] if repl is True else [
                     f'{warps}'.join(_) for _ in self.result]
                 self.result = [replace(_) for _ in self.result]
                 self.result = [_ for _ in self.result if _ != '']
                 self.result = f'{warps}'.join(self.result) if len(self.result) == 1 else self.result
             else:
                 self.result = [f'{warps}'.join(_) for _ in self.result]
+                self.result = [replace(_) for _ in self.result] if repl else self.result
 
         else:
             self.result = self.xp.xpath(text_xpath)
             if lists is False:
-                if repl is True:
-                    self.result = [replace(_) for _ in self.result]
+                self.result = [replace(_) for _ in self.result] if repl else self.result
                 self.result = f'{warps}'.join(self.result)
 
         return self.result
 
     def date(self):
         text = self.text()
         if isinstance(text, str):
@@ -254,16 +255,17 @@
             result_time = minutes_ago
 
         elif u'秒前' in s_time:
             second = re.findall(u'(\d+)秒前', s_time)[0]
             second_ago = (datetime.now() - timedelta(seconds=int(second))).strftime("%Y-%m-%d %H:%M:%S")
             result_time = second_ago
 
-        # 06-29
-        elif re.findall(r'\d{1,2}-\d{1,2}', s_time) and len(s_time) <= 5:
+        # 06-29 1月12日
+        elif re.findall(r'\d{1,2}-\d{1,2}|\d{1,2}月\d{1,2}日', s_time) and len(s_time) <= 5:
+            s_time = s_time.replace('月', '-').replace('日', '')
             now_year = str(datetime.now().year)
             _time = now_year + '-' + s_time
             result_time = time.strftime("%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d"))
 
         # 1小时前
         elif u'小时前' in s_time:
             hours = re.findall(u'(\d+|半)小时前', s_time)[0]
```

### Comparing `PrSpiders-0.2.8/PrSpider/requestXpath.py` & `PrSpiders-0.2.9/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/PrSpider/useragent.py` & `PrSpiders-0.2.9/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.2.9/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.2.8
+Version: 0.2.9
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,16 +33,14 @@
 | `data`           | `Type: dict or string`                          | `Request parameters`            |
 | `encoding`       | `Default: "utf-8" Type: string`                 | `Request Encoding`              |
 | `retry_time`     | `Default: 3 Type: int`                          | `Retry Count`                   |
 | `retry_interval` | `Default: 1 Type: int`                          | `Retry Interval`                |
 | `timeout`        | `Default: 3 Type: int`                          | `Request timeout`               |
 | `others`         | `*args or **kwargs`                             | `Follow Requests`               | 
 
-
-
 ## *Get started*
 
 Install Package: pip install requestXpath
 Make a request:
 
     from requestXpath import prequests
     url = 'https://gitee.com/'
```

### Comparing `PrSpiders-0.2.8/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.2.9/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/README.md` & `PrSpiders-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 | `data`           | `Type: dict or string`                          | `Request parameters`            |
 | `encoding`       | `Default: "utf-8" Type: string`                 | `Request Encoding`              |
 | `retry_time`     | `Default: 3 Type: int`                          | `Retry Count`                   |
 | `retry_interval` | `Default: 1 Type: int`                          | `Retry Interval`                |
 | `timeout`        | `Default: 3 Type: int`                          | `Request timeout`               |
 | `others`         | `*args or **kwargs`                             | `Follow Requests`               | 
 
-
-
 ## *Get started*
 
 Install Package: pip install requestXpath
 Make a request:
 
     from requestXpath import prequests
     url = 'https://gitee.com/'
```

### Comparing `PrSpiders-0.2.8/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.2.9/pkg/prspider/PrSpider_CMD.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # encoding:utf-8
 
 __version__ = "v0.1.0"
 
 import argparse
 
-from start import start_code
+from .start import start_code
 
 
 def get_version():
     return "0.2.8"
 
 
 def main():
```

### Comparing `PrSpiders-0.2.8/requestXpath/__init__.py` & `PrSpiders-0.2.9/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/requestXpath/pxpath.py` & `PrSpiders-0.2.9/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/requestXpath/requestXpath.py` & `PrSpiders-0.2.9/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/requestXpath/useragent.py` & `PrSpiders-0.2.9/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/setup.py` & `PrSpiders-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

### Comparing `PrSpiders-0.2.8/table_parse/T.py` & `PrSpiders-0.2.9/table_parse/T.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.2.8/table_parse/tb_parse.py` & `PrSpiders-0.2.9/table_parse/tb_parse.py`

 * *Files identical despite different names*

