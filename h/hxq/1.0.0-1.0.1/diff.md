# Comparing `tmp/hxq-1.0.0.tar.gz` & `tmp/hxq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hxq-1.0.0.tar", last modified: Tue Apr 11 12:38:41 2023, max compression
+gzip compressed data, was "dist\hxq-1.0.1.tar", last modified: Mon Apr 17 15:41:55 2023, max compression
```

## Comparing `hxq-1.0.0.tar` & `hxq-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/
--rw-rw-rw-   0        0        0      169 2023-04-11 12:38:41.000000 hxq-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq/
--rw-rw-rw-   0        0        0      141 2023-04-10 16:33:43.000000 hxq-1.0.0/hxq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq/interface/
--rw-rw-rw-   0        0        0      120 2023-04-10 15:28:34.000000 hxq-1.0.0/hxq/interface/__init__.py
--rw-rw-rw-   0        0        0      490 2023-04-10 16:19:54.000000 hxq-1.0.0/hxq/interface/db_helper.py
--rw-rw-rw-   0        0        0      300 2023-04-10 15:28:44.000000 hxq-1.0.0/hxq/interface/httpx.py
--rw-rw-rw-   0        0        0      117 2023-04-10 15:28:59.000000 hxq-1.0.0/hxq/interface/win32.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq/libs/
--rw-rw-rw-   0        0        0      123 2023-04-10 15:30:35.000000 hxq-1.0.0/hxq/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq/libs/db/
--rw-rw-rw-   0        0        0      120 2023-04-06 15:20:14.000000 hxq-1.0.0/hxq/libs/db/__init__.py
--rw-rw-rw-   0        0        0     4314 2023-04-10 16:30:41.000000 hxq-1.0.0/hxq/libs/db/db_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq/libs/httpx/
--rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.0/hxq/libs/httpx/__init__.py
--rw-rw-rw-   0        0        0      553 2022-08-21 03:37:18.000000 hxq-1.0.0/hxq/libs/httpx/chrome_agent.py
--rw-rw-rw-   0        0        0     8336 2023-04-10 15:29:33.000000 hxq-1.0.0/hxq/libs/httpx/http.py
--rw-rw-rw-   0        0        0     3022 2023-04-10 15:29:39.000000 hxq-1.0.0/hxq/libs/httpx/session.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq/libs/win32/
--rw-rw-rw-   0        0        0      123 2023-04-05 04:51:31.000000 hxq-1.0.0/hxq/libs/win32/__init__.py
--rw-rw-rw-   0        0        0     2024 2023-04-06 13:47:02.000000 hxq-1.0.0/hxq/libs/win32/api.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq/utils/
--rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.0/hxq/utils/__init__.py
--rw-rw-rw-   0        0        0     3362 2023-04-10 15:35:13.000000 hxq-1.0.0/hxq/utils/common.py
--rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.0/hxq/utils/decorator.py
--rw-rw-rw-   0        0        0     1576 2023-04-10 16:12:31.000000 hxq-1.0.0/hxq/utils/encipher.py
--rw-rw-rw-   0        0        0      418 2023-04-10 15:33:03.000000 hxq-1.0.0/hxq/utils/pic_code.py
--rw-rw-rw-   0        0        0      314 2023-04-09 13:39:57.000000 hxq-1.0.0/hxq/utils/ran_func.py
--rw-rw-rw-   0        0        0     3463 2023-04-09 13:39:58.000000 hxq-1.0.0/hxq/utils/threadx.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq.egg-info/
--rw-rw-rw-   0        0        0      169 2023-04-11 12:38:40.000000 hxq-1.0.0/hxq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      635 2023-04-11 12:38:41.000000 hxq-1.0.0/hxq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:38:40.000000 hxq-1.0.0/hxq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-11 12:38:40.000000 hxq-1.0.0/hxq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-11 12:38:40.000000 hxq-1.0.0/hxq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 12:38:41.000000 hxq-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-04-11 12:37:49.000000 hxq-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/
+-rw-rw-rw-   0        0        0      169 2023-04-17 15:41:55.000000 hxq-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/
+-rw-rw-rw-   0        0        0      141 2023-04-17 15:41:39.000000 hxq-1.0.1/hxq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/interface/
+-rw-rw-rw-   0        0        0      777 2023-04-17 15:40:51.000000 hxq-1.0.1/hxq/interface/__init__.py
+-rw-rw-rw-   0        0        0     4230 2023-04-14 14:47:06.000000 hxq-1.0.1/hxq/interface/db_helper.py
+-rw-rw-rw-   0        0        0      300 2023-04-13 13:36:38.000000 hxq-1.0.1/hxq/interface/httpx.py
+-rw-rw-rw-   0        0        0      186 2023-04-13 13:11:19.000000 hxq-1.0.1/hxq/interface/win32.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/
+-rw-rw-rw-   0        0        0      123 2023-04-13 13:04:22.000000 hxq-1.0.1/hxq/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/db/
+-rw-rw-rw-   0        0        0      383 2023-04-13 12:57:46.000000 hxq-1.0.1/hxq/libs/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/httpx/
+-rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.1/hxq/libs/httpx/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-04-13 14:06:06.000000 hxq-1.0.1/hxq/libs/httpx/chrome_agent.py
+-rw-rw-rw-   0        0        0     9128 2023-04-17 15:40:28.000000 hxq-1.0.1/hxq/libs/httpx/http.py
+-rw-rw-rw-   0        0        0     3167 2023-04-16 10:54:55.000000 hxq-1.0.1/hxq/libs/httpx/session.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/libs/win32/
+-rw-rw-rw-   0        0        0     1983 2023-04-13 13:36:03.000000 hxq-1.0.1/hxq/libs/win32/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq/utils/
+-rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.1/hxq/utils/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-04-13 14:08:04.000000 hxq-1.0.1/hxq/utils/common.py
+-rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.1/hxq/utils/decorator.py
+-rw-rw-rw-   0        0        0     1576 2023-04-10 16:12:31.000000 hxq-1.0.1/hxq/utils/encipher.py
+-rw-rw-rw-   0        0        0      418 2023-04-10 15:33:03.000000 hxq-1.0.1/hxq/utils/pic_code.py
+-rw-rw-rw-   0        0        0      314 2023-04-09 13:39:57.000000 hxq-1.0.1/hxq/utils/ran_func.py
+-rw-rw-rw-   0        0        0     3463 2023-04-09 13:39:58.000000 hxq-1.0.1/hxq/utils/threadx.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-17 15:41:55.000000 hxq-1.0.1/hxq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:41:55.000000 hxq-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-04-17 15:41:23.000000 hxq-1.0.1/setup.py
```

### Comparing `hxq-1.0.0/hxq/libs/db/db_helper.py` & `hxq-1.0.1/hxq/interface/db_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2022/5/6 13:09
+# @Time    : 2023/4/6 23:38
 # @Author  : hxq
 # @Software: PyCharm
 # @File    : db_helper.py
-
-# import pymysql
-# import pymssql
 import contextlib
 import re
 import json
 import importlib
-import datetime
-from json import JSONEncoder
-from dbutils.pooled_db import PooledDB
+from typing import Union
 
+from hxq.libs.db import DateTimeEncoder
+from dbutils.pooled_db import PooledDB, PooledDedicatedDBConnection
 
-class DateTimeEncoder(JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, (datetime.date, datetime.datetime)):
-            return obj.isoformat(sep=" ")
-        return super().default(obj)
+__all__ = [
+    "DBHelper",
+]
 
 
 class DBHelper:
     """简单的数据库连接池助手"""
 
     def __init__(self, config):
         self.config = self.import_config(config)
@@ -49,15 +44,15 @@
             database=self.config.setdefault('SQL_DATABASE', None),
             charset=self.config.setdefault('SQL_CHARSET', 'utf8mb4')
         )
 
     """导入配置"""
 
     @staticmethod
-    def import_config(obj):
+    def import_config(obj) -> dict:
         """
         导入字典or类对象中的配置信息
         """
         config = dict()
         if isinstance(obj, dict):
             [config.update({k.upper(): v}) for k, v in obj.items()]
         elif hasattr(obj, '__dict__'):
@@ -65,56 +60,56 @@
         else:
             raise ValueError('请导入正确的config对象!')
         return config
 
     """列表类型转字典"""
 
     @staticmethod
-    def _tuple2dict(results, cursor):
+    def _tuple2dict(results, cursor) -> dict:
         result = [dict(zip([desc[0] for desc in cursor.description], item)) for item in results]
         return json.loads(DateTimeEncoder().encode(result))
 
     """执行增删改查sql语句"""
 
-    def execute(self, sql_statement: str):
+    def execute(self, sql_statement: str) -> Union[dict, int]:
         with self.connect() as conn:
             cursor = conn.cursor()
             row_count = cursor.execute(sql_statement)
             # 匹配对大小写不敏感
             if re.search(r"SELECT", sql_statement, re.I):
                 result = cursor.fetchall()
                 return self._tuple2dict(result, cursor)
 
             cursor.connection.commit()
             return row_count if row_count else 0
 
     """查询一条数据"""
 
-    def first(self, sql_statement):
+    def first(self, sql_statement) -> dict:
         with self.connect() as conn:
             cursor = conn.cursor()
             cursor.execute(sql_statement)
             result = cursor.fetchone()
 
         return self._tuple2dict([result], cursor)
 
     """查询所有数据"""
 
-    def all(self, sql_statement):
+    def all(self, sql_statement) -> dict:
         with self.connect() as conn:
             cursor = conn.cursor()
             cursor.execute(sql_statement)
             result = cursor.fetchall()
 
         return self._tuple2dict(result, cursor)
 
     """创建连接"""
 
     @contextlib.contextmanager
-    def connect(self):
+    def connect(self) -> PooledDedicatedDBConnection:
         conn = self.pool.connection()  # 创建连接
         yield conn  # 游标
         self.close(conn)
 
     """关闭连接"""
 
     @staticmethod
```

### Comparing `hxq-1.0.0/hxq/libs/httpx/chrome_agent.py` & `hxq-1.0.1/hxq/libs/httpx/chrome_agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/5/7 22:17
 # @Author  : hertx
 # @Software: PyCharm
 # @File    : chrome_agent.py
 import random
 
-version_list = ['85.0.4183.83', '85.0.4183.87', '86.0.4240.22', '87.0.4280.20', '87.0.4280.88',
-                '88.0.4324.96', '89.0.4389.23', '90.0.4430.24', '91.0.4472.19', '90.0.4430.212']
-user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{} Safari/537.36 '
 
-
-def random_chrome_version():
+def random_version():
+    version_list = ['85.0.4183.83', '85.0.4183.87', '86.0.4240.22', '87.0.4280.20', '87.0.4280.88',
+                    '88.0.4324.96', '89.0.4389.23', '90.0.4430.24', '91.0.4472.19', '90.0.4430.212']
+    user_agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{} ' \
+                 'Safari/537.36'
     return user_agent.format(random.choice(version_list))
+
+
+if __name__ == '__main__':
+    print(random_version())
```

### Comparing `hxq-1.0.0/hxq/libs/httpx/http.py` & `hxq-1.0.1/hxq/libs/httpx/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/5/7 22:22
 # @Author  : hxq
 # @Software: PyCharm
 # @File    : http.py
+import contextlib
 import importlib
 import sys
 import json
+from asyncio import sleep
 from functools import wraps
 from typing import Union, List
+
+import aiofiles
 from lxml import etree, html
 from requests.packages import urllib3
 from requests import Session, Response, exceptions
-from hxq.libs.httpx.chrome_agent import random_chrome_version
 from requests.cookies import cookiejar_from_dict, RequestsCookieJar
 
+from hxq.utils.common import run_event_loop
+
 if sys.version_info >= (3,):
     from urllib.parse import urlencode
     from urllib import parse
 else:
     from urllib import urlencode, parse
 # 关闭错误提示
 urllib3.disable_warnings()
 
 
+@run_event_loop
+async def iter_write_file(file_path: str, r: Response):
+    async with aiofiles.open(file_path, 'wb') as file:
+        for chunk in r.iter_content(1024 * 10):
+            await file.write(chunk)
+
+
 def requests_catch_exception(func):
     """
     requests异常捕获装饰器
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> Union[HTTPResponse, HTTPError]:
@@ -146,68 +158,90 @@
         if len(json_str.keys()) > 1:
             json_str = {'root': json_str}
 
         xml_to_dict = importlib.import_module('xmltodict')
         _unparse = getattr(xml_to_dict, 'unparse')
         return _unparse(json_str, pretty=1)
 
+    def close(self):
+        # print('链接关闭')
+        self.res.close()
+
     def __str__(self):
         return "{}:{}".format(self.__response, self.encoding)
 
 
 class HTTPError:
     """请求错误"""
 
-    def __init__(self, code, reason=None):
+    def __init__(self, code, error_reason=None):
         """
         :param code: http状态码
-        :param reason: http状态原因
+        :param error_reason: http状态原因
         """
         self.ok = False
         self.code = code
-        self.reason = reason
+        self.error_reason = error_reason
 
     def __str__(self):
-        return "HTTP {}: {}".format(self.code, self.reason)
+        return "HTTP {}: {}".format(self.code, self.error_reason)
 
 
 class HTTPRequest:
 
     @classmethod
-    def get(cls, url, params=None, timeout=None, proxies=None, **kwargs):
+    def get(cls, url, params=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         GET请求
         """
         kwargs.setdefault('allow_redirects', True)
-        return cls.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs)
+        with cls.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs) as r:
+            return r
 
     @classmethod
-    def post(cls, url, data=None, timeout=None, proxies=None, **kwargs):
+    def post(cls, url, data=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         POST请求
         """
-        return cls.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs)
+        with cls.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs) as r:
+            return r
+
+    @classmethod
+    def download(cls, url, file_path, params=None, data=None, **kwargs):
+        """
+        下载文件
+        """
+        kwargs.setdefault('method', 'GET')
+        kwargs['stream'] = True
+        with cls.request(kwargs['method'].upper(), url, params=params, data=data, **kwargs) as r:
+            if not r.ok:
+                return r.error_reason
+            iter_write_file(file_path, r.res)
 
     @staticmethod
+    @contextlib.contextmanager
     @requests_catch_exception
     def request(method, url, **kwargs):
         """
         :param method: 大小不敏感，在Session内部upper统一转化为大写
         :param url: 地址
         :param kwargs:
         :return:
         """
+
         kwargs.setdefault('ignore_status', True)
         ignore_status = kwargs.pop('ignore_status')
-        kwargs.setdefault('headers', {"User-Agent": random_chrome_version()})
-        with Session().request(method, url, **kwargs) as r:
-            results = HTTPResponse(r)
+        ua = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 " \
+             "Safari/537.36"
+        kwargs.setdefault('headers', {"User-Agent": ua})
+        results = HTTPResponse(Session().request(method, url, **kwargs))
         if not ignore_status and results.code != 200:
-            return HTTPError(results.code, '请求状态错异常!')
-        return results
+            yield HTTPError(results.code, '请求状态错异常!')
+        yield results
+        results.close()
 
     @staticmethod
     def cookiejar2dict(cookiejar: RequestsCookieJar) -> dict:
         """
         CookieJar转dict
         """
         return (lambda ck: [[ck.update({k: v}) for k, v in cookiejar.items()], ck][1])(dict())
@@ -220,23 +254,14 @@
         return cookiejar_from_dict(cookie_dict)
 
     @staticmethod
     def _raw_headers_to_dict(this_headers_str: str) -> dict:
         """
         抓包raw字符串解析为headers
         """
-        """
-        results = {}
-        for item in this_headers_str.strip().split('\n'):
-            if not item.strip():
-                continue
-            items = item.strip().split(':')
-            results[items[0]] = ':'.join(items[1:]).strip()
-        return results
-        """
         # lambda
         return (lambda x: [[(lambda xx: (
             lambda items: [xx.update({items[0].strip(): ':'.join(items[1:]).strip()}), xx][1]))(x)(
             item.strip().split(':')) for item in this_headers_str.strip().split('\n') if item.strip()], x])(dict())[1]
 
     @staticmethod
     def dict2url(dict_params) -> str:
```

### Comparing `hxq-1.0.0/hxq/libs/httpx/session.py` & `hxq-1.0.1/hxq/libs/httpx/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/5/7 22:35
 # @Author  : hxq
 # @Software: PyCharm
 # @File    : session.py
+import contextlib
+from typing import Union
+
 from requests import Session
 from requests.structures import CaseInsensitiveDict
 from requests.utils import default_headers
 
 from hxq.libs.httpx.http import HTTPRequest, requests_catch_exception, HTTPResponse, HTTPError
-from hxq.libs.httpx.chrome_agent import random_chrome_version
+from hxq.libs.httpx.chrome_agent import random_version
 
 
 class SessionRequest(HTTPRequest):
     """基于requests 方便日常使用的简单二次封装"""
 
     def __init__(self, ignore_status=True):
         """
         :param ignore_status: 是否忽略错误状态码
         """
         self.__http = Session()
-        self.headers = {"User-Agent": random_chrome_version()}
+        self.headers = {"User-Agent": random_version()}
         self.ignore_status = ignore_status
 
-    def get(self, url, params=None, timeout=None, proxies=None, **kwargs):
+    def get(self, url, params=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         GET请求
         """
         kwargs.setdefault('allow_redirects', True)
-        return self.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs)
+        with self.request('GET', url, params=params, timeout=timeout, proxies=proxies, **kwargs) as r:
+            return r
 
-    def post(self, url, data=None, timeout=None, proxies=None, **kwargs):
+    def post(self, url, data=None, timeout=None, proxies=None, **kwargs) -> Union[HTTPResponse, HTTPError]:
         """
         POST请求
         """
-        return self.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs)
+        with self.request('POST', url, data=data, timeout=timeout, proxies=proxies, **kwargs) as r:
+            return r
 
+    @contextlib.contextmanager
     @requests_catch_exception
     def request(self, method, url, **kwargs):
         """
         :param method: 大小不敏感，在Session内部upper统一转化为大写
         :param url: 地址
         :param kwargs:
         :return:
         """
-        with self.__http.request(method, url, **kwargs) as r:
-            results = HTTPResponse(r)
+        # with self.__http.request(method, url, **kwargs) as r:
+        results = HTTPResponse(self.__http.request(method, url, **kwargs))
         if not self.ignore_status and results.code != 200:
-            return HTTPError(results.code, '请求状态错异常!')
-        return results
+            yield HTTPError(results.code, '请求状态错异常!')
+        yield results
+        results.close()
 
     @property
     def cookies(self) -> dict:
         """
         读取cookies
-        # _cookies = {}
-        # [_cookies.update({k: v}) for k, v in self.__http.cookies.items()]
         """
         return self.cookiejar2dict(self.__http.cookies)
 
     @cookies.setter
     def cookies(self, cookie: dict):
         """
         设置cookies
```

### Comparing `hxq-1.0.0/hxq/libs/win32/api.py` & `hxq-1.0.1/hxq/libs/win32/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/4/5 12:51
+# @Time    : 2022/4/5 12:51
 # @Author  : hxq
 # @Software: PyCharm
-# @File    : api.py
+# @File    : __init__.py.py
 import os
+import importlib
 import getpass
-import winshell
 
+winshell = importlib.import_module("winshell")
 
-class API:
+
+class Client:
     def __init__(self):
-        pass
+        ...
 
     @property
     def desktop(self):
         """
         桌面路径
         """
-        return winshell.desktop()
+        return getattr(winshell, 'desktop')()
 
     @property
     def username(self):
         """
         系统用户名
         """
         return getpass.getuser()
@@ -30,15 +32,15 @@
     def start_file(path):
         """
         启动文件/应用
         """
         os.startfile(path)
 
     @property
-    def startup_path(self):
+    def startup_path(self) -> str:
         """
         自启动目录
         """
         startup_path = r"AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup"
         return os.path.join(os.getenv("SystemDrive"), r"\users", self.username, startup_path)
 
     @staticmethod
@@ -49,27 +51,21 @@
         :param shortcut_name: 需要创建快捷方式的路径
         :param desc: 描述，鼠标放在图标上面会有提示
         :return:
         """
         if not shortcut_name.endswith('.lnk'):
             shortcut_name = shortcut_name + ".lnk"
         try:
-            winshell.CreateShortcut(
+            getattr(winshell, 'CreateShortcut')(
                 Path=shortcut_name,
                 Target=exe_path,
                 Icon=(exe_path, 0),
                 Description=desc
             )
             return True
         except ImportError as err:
             print("'winshell' lib may not available on current os")
             print("error detail %s" % str(err))
         return False
 
-
-if __name__ == '__main__':
-    api = API()
-    print(api.startup_path)
-    print(api.start_file(api.startup_path))
-    # bin_path = r"D:\InstallData\日常软件\XQ工具\XQ工具.exe"
-    # link_path = api.startup_path + "\\tools"
-    # api.create_shortcut(bin_path, link_path, "小工具")
+    def create_startup(self, exe_path: str, lnk_name: str, desc: str):
+        return self.create_shortcut(exe_path, os.path.join(self.startup_path, lnk_name), desc)
```

### Comparing `hxq-1.0.0/hxq/utils/common.py` & `hxq-1.0.1/hxq/utils/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/7/10 20:42
 # @Author  : hxq
 # @Software: PyCharm
 # @File    : common.py
-
+import asyncio
 import os
 import sys
 import pkgutil
 import socket
 import subprocess
+from functools import wraps
+
 from hxq.utils.decorator import except_desc, func_run_times
 
 
 # 生成资源文件目录访问路径
 def resource_path(relative_path=''):
     if getattr(sys, 'frozen', False):  # 是否Bundle Resource
         base_path = getattr(sys, '_MEIPASS')
     else:
         base_path = os.path.abspath(".")  # 获取当前工作路径,
     return os.path.join(base_path, relative_path)
 
 
+def run_event_loop(func):
+    @wraps(func)
+    def wrapped(*args, **kwargs):
+        return asyncio.get_event_loop().run_until_complete(func(*args, **kwargs))
+
+    return wrapped
+
+
 @except_desc
 def url2ip(url):
     socket_list = socket.getaddrinfo(url, None, 0, socket.SOCK_STREAM)
     ip_info = socket_list[0][4][0]
     print('【{}】 IP地址：{}'.format(url, ip_info))
     return ip_info
```

### Comparing `hxq-1.0.0/hxq/utils/decorator.py` & `hxq-1.0.1/hxq/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.0/hxq/utils/encipher.py` & `hxq-1.0.1/hxq/utils/encipher.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.0/hxq/utils/threadx.py` & `hxq-1.0.1/hxq/utils/threadx.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.0/hxq.egg-info/SOURCES.txt` & `hxq-1.0.1/hxq.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 hxq.egg-info/top_level.txt
 hxq/interface/__init__.py
 hxq/interface/db_helper.py
 hxq/interface/httpx.py
 hxq/interface/win32.py
 hxq/libs/__init__.py
 hxq/libs/db/__init__.py
-hxq/libs/db/db_helper.py
 hxq/libs/httpx/__init__.py
 hxq/libs/httpx/chrome_agent.py
 hxq/libs/httpx/http.py
 hxq/libs/httpx/session.py
 hxq/libs/win32/__init__.py
-hxq/libs/win32/api.py
 hxq/utils/__init__.py
 hxq/utils/common.py
 hxq/utils/decorator.py
 hxq/utils/encipher.py
 hxq/utils/pic_code.py
 hxq/utils/ran_func.py
 hxq/utils/threadx.py
```

### Comparing `hxq-1.0.0/setup.py` & `hxq-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import find_packages, setup
 
 setup(name='hxq',
       author='hxq',
-      version='1.0.0',
+      version='1.0.1',
       packages=find_packages(exclude=["*.demo", "*.demo.*", "tests", "demos"]),
       author_email='337168530@qq.com',
       description="这是一个python工具包",
       license="GPL",
       # 而 extras_require 这里仅表示该模块会依赖这些包,深度使用模块时，才会用到，这里需要你手动安装
       extras_require={
           'HTML': ["bs4>=0.0.1", "xmltodict>=1.2"],
       },
       # install_requires 在安装模块时会自动安装依赖包
       install_requires=[
           'requests>=2.24.0',
           'lxml>=4.9.2',
+          'pymysql~=1.0.3',
+          'DBUtils~=3.0.2',
       ]
       )
```

