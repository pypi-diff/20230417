# Comparing `tmp/hopara-1.9.0.tar.gz` & `tmp/hopara-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopara-1.9.0.tar", last modified: Thu Nov 10 23:21:03 2022, max compression
+gzip compressed data, was "hopara-1.9.1.tar", last modified: Tue Dec  6 22:35:37 2022, max compression
```

## Comparing `hopara-1.9.0.tar` & `hopara-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-10 23:21:03.779144 hopara-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1263 2022-11-10 23:21:03.779144 hopara-1.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1121 2022-11-10 23:20:53.000000 hopara-1.9.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-10 23:21:03.779144 hopara-1.9.0/hopara/
--rw-rw-rw-   0 root         (0) root         (0)      581 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2470 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1319 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     1725 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/from_pandas.py
--rw-rw-rw-   0 root         (0) root         (0)     3940 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/hopara.py
--rw-rw-rw-   0 root         (0) root         (0)     1860 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/request.py
--rw-rw-rw-   0 root         (0) root         (0)     3026 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/table.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/type.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2022-11-10 23:20:53.000000 hopara-1.9.0/hopara/view.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-10 23:21:03.779144 hopara-1.9.0/hopara.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1263 2022-11-10 23:21:03.000000 hopara-1.9.0/hopara.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      333 2022-11-10 23:21:03.000000 hopara-1.9.0/hopara.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-11-10 23:21:03.000000 hopara-1.9.0/hopara.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-11-10 23:21:03.000000 hopara-1.9.0/hopara.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-11-10 23:21:03.000000 hopara-1.9.0/hopara.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      177 2022-11-10 23:21:03.783144 hopara-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      590 2022-11-10 23:20:53.000000 hopara-1.9.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-06 22:35:37.068453 hopara-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2022-12-06 22:35:37.068453 hopara-1.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2022-12-06 22:35:26.000000 hopara-1.9.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-06 22:35:37.064453 hopara-1.9.1/hopara/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2454 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1725 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/from_pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/hopara.py
+-rw-rw-rw-   0 root         (0) root         (0)     1860 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3026 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2022-12-06 22:35:26.000000 hopara-1.9.1/hopara/view.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-06 22:35:37.064453 hopara-1.9.1/hopara.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2022-12-06 22:35:37.000000 hopara-1.9.1/hopara.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      333 2022-12-06 22:35:37.000000 hopara-1.9.1/hopara.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2022-12-06 22:35:37.000000 hopara-1.9.1/hopara.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-12-06 22:35:37.000000 hopara-1.9.1/hopara.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-12-06 22:35:37.000000 hopara-1.9.1/hopara.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      177 2022-12-06 22:35:37.068453 hopara-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      590 2022-12-06 22:35:26.000000 hopara-1.9.1/setup.py
```

### Comparing `hopara-1.9.0/PKG-INFO` & `hopara-1.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopara
-Version: 1.9.0
+Version: 1.9.1
 Summary: Hopara Python Library
 Author: Hopara Inc
 Description-Content-Type: text/markdown
 
 # Pyhopara
 
 Pyhopara is the Hopara Python SDK. It's main purpose is to ingest data from Python/Pandas.
```

### Comparing `hopara-1.9.0/README.md` & `hopara-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara/__init__.py` & `hopara-1.9.1/hopara/__init__.py`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara/config.py` & `hopara-1.9.1/hopara/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 
     def get_dataset_url(self) -> str:
         dataset_url = os.getenv("HOPARA_DATASET_URL")
         if dataset_url is None and self.__config:
             dataset_url = self.get_value('datasetEndpoint')
         return dataset_url
 
-    def get_bff_url(self) -> str:
-        dataset_url = os.getenv("HOPARA_BFF_URL")
-        if dataset_url is None and self.__config:
-            dataset_url = self.get_value('bffEndpoint')
-        return dataset_url
+    def get_app_url(self) -> str:
+        app_url = os.getenv("HOPARA_APP_URL")
+        if app_url is None and self.__config:
+            app_url = self.get_value('appEndpoint')
+        return app_url
 
     def get_email(self) -> str:
         email = os.getenv("HOPARA_EMAIL")
         if email is None and self.__config:
             email = self.get_value('email')
         return email
```

### Comparing `hopara-1.9.0/hopara/filter.py` & `hopara-1.9.1/hopara/filter.py`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara/from_pandas.py` & `hopara-1.9.1/hopara/from_pandas.py`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara/hopara.py` & `hopara-1.9.1/hopara/hopara.py`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara/request.py` & `hopara-1.9.1/hopara/request.py`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara/table.py` & `hopara-1.9.1/hopara/table.py`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara/type.py` & `hopara-1.9.1/hopara/type.py`

 * *Files identical despite different names*

### Comparing `hopara-1.9.0/hopara.egg-info/PKG-INFO` & `hopara-1.9.1/hopara.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopara
-Version: 1.9.0
+Version: 1.9.1
 Summary: Hopara Python Library
 Author: Hopara Inc
 Description-Content-Type: text/markdown
 
 # Pyhopara
 
 Pyhopara is the Hopara Python SDK. It's main purpose is to ingest data from Python/Pandas.
```

### Comparing `hopara-1.9.0/setup.py` & `hopara-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 with open(os.path.join(current_dir, 'README.md')) as fp:
     long_description = fp.read()
 
 setup(
     name='hopara',
     packages=find_packages(include=['hopara']),
-    version='1.9.0',
+    version='1.9.1',
     description='Hopara Python Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Hopara Inc',
     install_requires=requires
 )
```

