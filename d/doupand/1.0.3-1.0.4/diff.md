# Comparing `tmp/doupand-1.0.3.tar.gz` & `tmp/doupand-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/doupand-1.0.3.tar", last modified: Tue Apr 11 13:57:19 2023, max compression
+gzip compressed data, was "dist/doupand-1.0.4.tar", last modified: Mon Apr 17 17:04:58 2023, max compression
```

## Comparing `doupand-1.0.3.tar` & `doupand-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-11 13:57:19.000000 doupand-1.0.3/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.3/LICENSE
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/
--rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-08 17:33:37.000000 doupand-1.0.3/doupand/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/utils/
--rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.3/doupand/utils/userauth.py
--rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.3/doupand/utils/__init__.py
--rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.3/doupand/utils/cons.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand/api/
--rw-r--r--   0 tongjun    (501) staff       (20)     3183 2023-04-11 13:54:16.000000 doupand-1.0.3/doupand/api/client.py
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.3/doupand/api/__init__.py
-drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/
--rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/PKG-INFO
--rw-r--r--   0 tongjun    (501) staff       (20)      310 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/SOURCES.txt
--rw-r--r--   0 tongjun    (501) staff       (20)       16 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/requires.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        8 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/top_level.txt
--rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-11 13:57:19.000000 doupand-1.0.3/doupand.egg-info/dependency_links.txt
--rw-r--r--   0 tongjun    (501) staff       (20)     2400 2023-04-11 13:39:22.000000 doupand-1.0.3/setup.py
--rw-r--r--   0 tongjun    (501) staff       (20)       38 2023-04-11 13:57:19.000000 doupand-1.0.3/setup.cfg
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-17 17:04:58.000000 doupand-1.0.4/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-17 17:04:58.000000 doupand-1.0.4/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)     1469 2023-04-07 19:08:40.000000 doupand-1.0.4/LICENSE
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand/
+-rw-r--r--   0 tongjun    (501) staff       (20)      133 2023-04-08 17:33:37.000000 doupand-1.0.4/doupand/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand/utils/
+-rw-r--r--   0 tongjun    (501) staff       (20)      701 2023-04-07 14:51:56.000000 doupand-1.0.4/doupand/utils/userauth.py
+-rw-r--r--   0 tongjun    (501) staff       (20)        0 2023-04-06 17:18:45.000000 doupand-1.0.4/doupand/utils/__init__.py
+-rw-r--r--   0 tongjun    (501) staff       (20)      277 2023-04-08 17:11:54.000000 doupand-1.0.4/doupand/utils/cons.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand/api/
+-rw-r--r--   0 tongjun    (501) staff       (20)     3214 2023-04-17 17:01:44.000000 doupand-1.0.4/doupand/api/client.py
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-06 17:31:40.000000 doupand-1.0.4/doupand/api/__init__.py
+drwxr-xr-x   0 tongjun    (501) staff       (20)        0 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand.egg-info/
+-rw-r--r--   0 tongjun    (501) staff       (20)     2041 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand.egg-info/PKG-INFO
+-rw-r--r--   0 tongjun    (501) staff       (20)      310 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand.egg-info/SOURCES.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)       16 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand.egg-info/requires.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        8 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand.egg-info/top_level.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)        1 2023-04-17 17:04:58.000000 doupand-1.0.4/doupand.egg-info/dependency_links.txt
+-rw-r--r--   0 tongjun    (501) staff       (20)     2400 2023-04-17 17:04:37.000000 doupand-1.0.4/setup.py
+-rw-r--r--   0 tongjun    (501) staff       (20)       38 2023-04-17 17:04:58.000000 doupand-1.0.4/setup.cfg
```

### Comparing `doupand-1.0.3/PKG-INFO` & `doupand-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.3/LICENSE` & `doupand-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doupand-1.0.3/doupand/utils/userauth.py` & `doupand-1.0.4/doupand/utils/userauth.py`

 * *Files identical despite different names*

### Comparing `doupand-1.0.3/doupand/api/client.py` & `doupand-1.0.4/doupand/api/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,38 +52,38 @@
 
             if os.path.exists(fp):
                 df = pd.read_csv(fp)
                 if cur_time < int(df.loc[0]['expire_time']):
                     self.__url_expire_time = int(df.loc[0]['expire_time'])
                     return str(df.loc[0]['http_url'])
 
-            res = requests.post(self.__distribution_url, timeout=10, headers={'Connection': 'close'})
+            req_params = {'token': self.__query_token}
+            res = requests.post(self.__distribution_url, json=req_params, timeout=10, headers={'Connection': 'close'})
             result = res.json()
             if result['status'] == "success":
                 self.__http_url = res.json()['result']
                 self.__url_expire_time = cur_time + 12 * 60 * 60
                 df = pd.DataFrame([[self.__http_url, self.__url_expire_time]], columns=['http_url', 'expire_time'])
                 df.to_csv(fp, index=False)
                 return self.__http_url
             else:
                 raise Exception("初始化请求失败，请重试！")
 
-    def query(self, api_name, fields='', **kwargs):
+    def query(self, api_name, **kwargs):
         """
         请求API
         :param api_name: API名称
         :param fields: 返回字段
         :param kwargs: 参数
         :return:
         """
         req_params = {
             'api_name': api_name,
             'token': self.__query_token,
-            'params': kwargs,
-            'fields': fields
+            'params': kwargs
         }
 
         res = requests.post(self.__query_url, json=req_params, timeout=self.__timeout, headers={'Connection': 'close'})
         result = json.loads(res.text)
         if result['code'] != 0:
             raise Exception(result['msg'])
         data = result['data']
```

### Comparing `doupand-1.0.3/doupand.egg-info/PKG-INFO` & `doupand-1.0.4/doupand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doupand
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple and easy-to-use financial data interface library built for normal investors!
 Home-page: https://doupand.com
 Author: DouBro
 Author-email: doupand@163.com
 License: BSD
 Keywords: Financial Data Interface
 Platform: all
```

### Comparing `doupand-1.0.3/setup.py` & `doupand-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     5331  873305.BJ  873305  ...          BSE         北交所
     5332  873339.BJ  873339  ...          BSE         北交所
     5333  873527.BJ  873527  ...          BSE         北交所
 """
 
 setup(
     name='doupand',
-    version="1.0.3",
+    version="1.0.4",
     description='A simple and easy-to-use financial data interface library built for normal investors!',
     long_description=long_desc,
     author='DouBro',
     author_email='doupand@163.com',
     packages=find_packages(),
     platforms=["all"],
     license='BSD',
```

