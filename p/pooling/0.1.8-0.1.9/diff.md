# Comparing `tmp/pooling-0.1.8.tar.gz` & `tmp/pooling-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pooling-0.1.8.tar", last modified: Wed Dec 14 01:22:13 2022, max compression
+gzip compressed data, was "pooling-0.1.9.tar", last modified: Mon Apr 17 14:54:08 2023, max compression
```

## Comparing `pooling-0.1.8.tar` & `pooling-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-12-14 01:22:13.459194 pooling-0.1.8/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-03-09 15:46:28.000000 pooling-0.1.8/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      144 2022-03-09 15:46:28.000000 pooling-0.1.8/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     4847 2022-12-14 01:22:13.458961 pooling-0.1.8/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     4258 2022-12-13 09:14:22.000000 pooling-0.1.8/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-12-14 01:22:13.457606 pooling-0.1.8/pooling/
--rw-r--r--   0 test       (501) staff       (20)      191 2022-11-24 09:56:55.000000 pooling-0.1.8/pooling/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     7263 2022-12-13 09:13:59.000000 pooling-0.1.8/pooling/base.py
--rw-r--r--   0 test       (501) staff       (20)     5289 2022-11-24 08:21:55.000000 pooling-0.1.8/pooling/mysql.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2022-12-14 01:22:13.458538 pooling-0.1.8/pooling.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     4847 2022-12-14 01:22:13.000000 pooling-0.1.8/pooling.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      292 2022-12-14 01:22:13.000000 pooling-0.1.8/pooling.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-12-14 01:22:13.000000 pooling-0.1.8/pooling.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2022-12-14 01:22:13.000000 pooling-0.1.8/pooling.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       23 2022-12-14 01:22:13.000000 pooling-0.1.8/pooling.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)        8 2022-12-14 01:22:13.000000 pooling-0.1.8/pooling.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       23 2022-11-24 12:37:28.000000 pooling-0.1.8/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2022-12-14 01:22:13.459243 pooling-0.1.8/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1376 2022-12-13 09:14:28.000000 pooling-0.1.8/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-17 14:54:08.936163 pooling-0.1.9/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2022-03-09 15:46:28.000000 pooling-0.1.9/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      144 2022-03-09 15:46:28.000000 pooling-0.1.9/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     5054 2023-04-17 14:54:08.936025 pooling-0.1.9/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     4504 2023-04-17 14:47:27.000000 pooling-0.1.9/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-17 14:54:08.934965 pooling-0.1.9/pooling/
+-rw-r--r--   0 test       (501) staff       (20)      191 2022-11-24 09:56:55.000000 pooling-0.1.9/pooling/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     7263 2023-04-17 06:30:58.000000 pooling-0.1.9/pooling/base.py
+-rw-r--r--   0 test       (501) staff       (20)     6093 2023-04-17 06:34:35.000000 pooling-0.1.9/pooling/mysql.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-17 14:54:08.935738 pooling-0.1.9/pooling.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     5054 2023-04-17 14:54:08.000000 pooling-0.1.9/pooling.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      292 2023-04-17 14:54:08.000000 pooling-0.1.9/pooling.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-17 14:54:08.000000 pooling-0.1.9/pooling.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-17 14:54:08.000000 pooling-0.1.9/pooling.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       23 2023-04-17 14:54:08.000000 pooling-0.1.9/pooling.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)        8 2023-04-17 14:54:08.000000 pooling-0.1.9/pooling.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       23 2022-11-24 12:37:28.000000 pooling-0.1.9/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-04-17 14:54:08.936213 pooling-0.1.9/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1376 2023-04-16 00:03:09.000000 pooling-0.1.9/setup.py
```

### Comparing `pooling-0.1.8/LICENSE` & `pooling-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pooling-0.1.8/PKG-INFO` & `pooling-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pooling
-Version: 0.1.8
+Version: 0.1.9
 Summary: pooling anything.
-Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: pooling
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -146,14 +144,15 @@
 
 * Call pool.get_session() returns a proxied connection instance.
 * The returned proxied connection instance is a proxy instance of the real connection.
 * When the returned proxied connection is being deleted, the real connection will be returned to the pool so that the real connection can be used again.
 * A simple mysql connection pool can be imported by doing `from pooling.mysql import MysqlConnectionPool`. Compare with the `MysqlConnectionPool` implemented in `Usage Example 1`, it add ping() test and errors handler in get_session() method.
 * The `pooling.mysql` module depends on `mysqlclient`, but `pooling` is NOT, so that `mysqlclient` is not auto installed after `pooling` installed. You should do `pip install mysqlclient` by yourself if you want to use `MysqlConnectionPool`.
 * If you want to use `MysqlConnectorPool`, you need to install package `mysql-connector-python` by yourself.
+* If you want to use `PyMySQLConnectionPool`, you need to install package `PyMySQL` by yourself.
 
 ## Releases
 
 ### v0.1.0
 
 - First release.
 
@@ -181,8 +180,11 @@
 
 - Unit test passed.
 
 ### v0.1.8
 
 - Add _pooling_is_connection_closed test.
 
+### v0.1.9
 
+- Fix doing useless time.sleep problem in pooling.mysql.MysqlConnectionPoolBase.get_session.
+- Add pooling.mysql.PyMySQLConnectionPool.
```

### Comparing `pooling-0.1.8/README.md` & `pooling-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
 * Call pool.get_session() returns a proxied connection instance.
 * The returned proxied connection instance is a proxy instance of the real connection.
 * When the returned proxied connection is being deleted, the real connection will be returned to the pool so that the real connection can be used again.
 * A simple mysql connection pool can be imported by doing `from pooling.mysql import MysqlConnectionPool`. Compare with the `MysqlConnectionPool` implemented in `Usage Example 1`, it add ping() test and errors handler in get_session() method.
 * The `pooling.mysql` module depends on `mysqlclient`, but `pooling` is NOT, so that `mysqlclient` is not auto installed after `pooling` installed. You should do `pip install mysqlclient` by yourself if you want to use `MysqlConnectionPool`.
 * If you want to use `MysqlConnectorPool`, you need to install package `mysql-connector-python` by yourself.
+* If you want to use `PyMySQLConnectionPool`, you need to install package `PyMySQL` by yourself.
 
 ## Releases
 
 ### v0.1.0
 
 - First release.
 
@@ -161,7 +162,12 @@
 ### v0.1.7
 
 - Unit test passed.
 
 ### v0.1.8
 
 - Add _pooling_is_connection_closed test.
+
+### v0.1.9
+
+- Fix doing useless time.sleep problem in pooling.mysql.MysqlConnectionPoolBase.get_session.
+- Add pooling.mysql.PyMySQLConnectionPool.
```

### Comparing `pooling-0.1.8/pooling/base.py` & `pooling-0.1.9/pooling/base.py`

 * *Files identical despite different names*

### Comparing `pooling-0.1.8/pooling/mysql.py` & `pooling-0.1.9/pooling/mysql.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,49 +24,54 @@
     MAX_RECONNECT_SLEEP_TIME = 5
     RECONNECT_SLEEP_TIME_DELTA = 0.1
 
     def do_session_create(self, *args, **kwargs):
         raise NotImplementedError()
 
     def do_session_destory(self, real_session):
-        real_session.close()
-
+        try:
+            real_session.close()
+        except Exception as error:
+            _logger.exception("MysqlConnectionPool.do_session_destory calling real_session.close() failed: error={error}...".format(error=error))
+    
     def get_cursor(self, conn):
         return conn.cursor()
 
     def get_session(self, timeout=None):
         last_error = Exception("Too short time to get a connection...")
         stime = time.time()
         sleep_time = 0.0
         while True:
             ntime = time.time()
             if timeout:
                 if ntime - stime > timeout:
                     break
+            session = None
             try:
                 session = PoolBase.get_session(self, timeout=timeout)
             except Exception as error:
                 _logger.exception("MysqlConnectionPool.get_session calling PoolBase.get_session() failed: error={error}...".format(error=error))
                 last_error = error
-                continue
-            try:
-                session.ping()
-            except Exception as error:
-                _logger.exception("MysqlConnectionPool.get_session calling session.ping() failed: error={error}...".format(error=error))
-                last_error = error
-                session._pooling_destory_session()
-                continue
-            sleep_time = self.get_session_sleep(sleep_time)
-            if sleep_time:
-                time.sleep(sleep_time)
-            return session
+            if session:
+                try:
+                    session.ping()
+                except Exception as error:
+                    _logger.exception("MysqlConnectionPool.get_session calling session.ping() failed: error={error}...".format(error=error))
+                    last_error = error
+                    session._pooling_destory_session()
+                    session = None
+            if not session:
+                sleep_time = self.get_session_sleep(sleep_time)
+                if sleep_time:
+                    time.sleep(sleep_time)
+            else:
+                return session
         raise last_error
 
     def get_session_sleep(self, sleep_time):
-        time.sleep(sleep_time)
         sleep_time += self.RECONNECT_SLEEP_TIME_DELTA
         if sleep_time >= self.MAX_RECONNECT_SLEEP_TIME:
             sleep_time = 0.0
         return sleep_time
 
     def query(self, *args, **kwargs):
         """Execute a SELECT SQL and get all the results.
@@ -154,9 +159,24 @@
         kwargs.setdefault("charset", "utf8mb4")
         kwargs.setdefault("collation", "utf8mb4_unicode_ci")
         return mysql.connector.connect(*args, **kwargs)
 
     def get_cursor(self, conn):
         return conn.cursor(dictionary=True, buffered=True)
 
+class PyMySQLConnectionPool(MysqlConnectionPoolBase):
+    """Mysql connection pool using `pymysql` adaptor.
+
+    Default settings:
+        cursorclass: pymysql.cursors.DictCursor
+    """
+
+    def do_session_create(self, *args, **kwargs):
+        import pymysql
+        import pymysql.cursors
+        kwargs.setdefault("cursorclass", pymysql.cursors.DictCursor)
+        if "collation" in kwargs:
+            del kwargs["collation"]
+        connection = pymysql.connect(*args, **kwargs)
+        return connection
 
 MysqlConnectionPool = MysqlclientConnectionPool # by default we use mysqlclient adaptor
```

### Comparing `pooling-0.1.8/pooling.egg-info/PKG-INFO` & `pooling-0.1.9/pooling.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pooling
-Version: 0.1.8
+Version: 0.1.9
 Summary: pooling anything.
-Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: pooling
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -146,14 +144,15 @@
 
 * Call pool.get_session() returns a proxied connection instance.
 * The returned proxied connection instance is a proxy instance of the real connection.
 * When the returned proxied connection is being deleted, the real connection will be returned to the pool so that the real connection can be used again.
 * A simple mysql connection pool can be imported by doing `from pooling.mysql import MysqlConnectionPool`. Compare with the `MysqlConnectionPool` implemented in `Usage Example 1`, it add ping() test and errors handler in get_session() method.
 * The `pooling.mysql` module depends on `mysqlclient`, but `pooling` is NOT, so that `mysqlclient` is not auto installed after `pooling` installed. You should do `pip install mysqlclient` by yourself if you want to use `MysqlConnectionPool`.
 * If you want to use `MysqlConnectorPool`, you need to install package `mysql-connector-python` by yourself.
+* If you want to use `PyMySQLConnectionPool`, you need to install package `PyMySQL` by yourself.
 
 ## Releases
 
 ### v0.1.0
 
 - First release.
 
@@ -181,8 +180,11 @@
 
 - Unit test passed.
 
 ### v0.1.8
 
 - Add _pooling_is_connection_closed test.
 
+### v0.1.9
 
+- Fix doing useless time.sleep problem in pooling.mysql.MysqlConnectionPoolBase.get_session.
+- Add pooling.mysql.PyMySQLConnectionPool.
```

### Comparing `pooling-0.1.8/setup.py` & `pooling-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, 'requirements.txt'), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="pooling",
-    version="0.1.8",
+    version="0.1.9",
     description="pooling anything.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     license_files=("LICENSE",),
```

