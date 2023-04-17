# Comparing `tmp/datadir-1.0.0-2.tar.gz` & `tmp/datadir-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadir-1.0.0.tar", last modified: Thu Mar  9 16:08:24 2023, max compression
+gzip compressed data, was "datadir-1.0.1.tar", last modified: Mon Apr 17 21:28:18 2023, max compression
```

## Comparing `datadir-1.0.0-2.tar` & `datadir-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 16:08:24.215443 datadir-1.0.0/
--rw-rw-rw-   0        0        0     1089 2023-02-18 15:25:33.000000 datadir-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       43 2023-03-09 15:48:19.000000 datadir-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      968 2023-03-09 16:08:24.215443 datadir-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-03-09 16:04:05.000000 datadir-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 16:08:24.204930 datadir-1.0.0/datadir/
--rw-rw-rw-   0        0        0      369 2023-02-18 16:13:52.000000 datadir-1.0.0/datadir/__init__.py
--rw-rw-rw-   0        0        0     4371 2023-03-09 15:29:25.000000 datadir-1.0.0/datadir/datadirectory.py
-drwxrwxrwx   0        0        0        0 2023-03-09 16:08:24.214443 datadir-1.0.0/datadir.egg-info/
--rw-rw-rw-   0        0        0      968 2023-03-09 16:08:24.000000 datadir-1.0.0/datadir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-03-09 16:08:24.000000 datadir-1.0.0/datadir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 16:08:24.000000 datadir-1.0.0/datadir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-03-09 16:08:24.000000 datadir-1.0.0/datadir.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-09 16:08:24.000000 datadir-1.0.0/datadir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-03-09 15:44:30.000000 datadir-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       47 2023-03-09 15:33:37.000000 datadir-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-09 16:08:24.215443 datadir-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1648 2023-03-09 16:04:15.000000 datadir-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 16:08:24.214443 datadir-1.0.0/tests/
--rw-rw-rw-   0        0        0    14051 2023-03-09 15:29:15.000000 datadir-1.0.0/tests/test_DataDirectory.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:28:18.471205 datadir-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2023-02-18 15:25:33.000000 datadir-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-03-09 15:48:19.000000 datadir-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      968 2023-04-17 21:28:18.471205 datadir-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-03-09 16:04:05.000000 datadir-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:28:18.458692 datadir-1.0.1/datadir/
+-rw-rw-rw-   0        0        0      369 2023-04-17 21:24:43.000000 datadir-1.0.1/datadir/__init__.py
+-rw-rw-rw-   0        0        0     4438 2023-04-17 21:20:10.000000 datadir-1.0.1/datadir/datadirectory.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:28:18.470203 datadir-1.0.1/datadir.egg-info/
+-rw-rw-rw-   0        0        0      968 2023-04-17 21:28:18.000000 datadir-1.0.1/datadir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-04-17 21:28:18.000000 datadir-1.0.1/datadir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:28:18.000000 datadir-1.0.1/datadir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-17 21:28:18.000000 datadir-1.0.1/datadir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 21:28:18.000000 datadir-1.0.1/datadir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-03-09 15:44:30.000000 datadir-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2023-03-09 15:33:37.000000 datadir-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:28:18.471205 datadir-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1648 2023-03-09 16:04:15.000000 datadir-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:28:18.470203 datadir-1.0.1/tests/
+-rw-rw-rw-   0        0        0    14208 2023-04-17 21:23:38.000000 datadir-1.0.1/tests/test_DataDirectory.py
```

### Comparing `datadir-1.0.0/LICENSE` & `datadir-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datadir-1.0.0/PKG-INFO` & `datadir-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadir
-Version: 1.0.0
+Version: 1.0.1
 Summary: A data directory helper Python package
 Home-page: https://github.com/hboueix/datadir
 Author: Hugo Boueix
 License: MIT
 Project-URL: Issue tracker, https://github.com/hboueix/datadir/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datadir-1.0.0/datadir/datadirectory.py` & `datadir-1.0.1/datadir/datadirectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,7 +99,10 @@
             )
         
     def get_obj(self, file_path: str, **kwargs: Any) -> Any:
         return pkl.load(open(os.path.join(self.basedir_path, file_path), 'rb'), **kwargs)
 
     def save_obj(self, file_path: str, obj: Any, **kwargs: Any) -> None:
         pkl.dump(obj, open(os.path.join(self.basedir_path, file_path), 'wb'), **kwargs)
+
+    def __str__(self) -> str:
+        return self.basedir_path
```

### Comparing `datadir-1.0.0/datadir.egg-info/PKG-INFO` & `datadir-1.0.1/datadir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadir
-Version: 1.0.0
+Version: 1.0.1
 Summary: A data directory helper Python package
 Home-page: https://github.com/hboueix/datadir
 Author: Hugo Boueix
 License: MIT
 Project-URL: Issue tracker, https://github.com/hboueix/datadir/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datadir-1.0.0/setup.py` & `datadir-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `datadir-1.0.0/tests/test_DataDirectory.py` & `datadir-1.0.1/tests/test_DataDirectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,19 @@
         os.makedirs(TestDataDirectory.basedir, exist_ok=False)
 
     def teardown_method(self, method: Any) -> None:
         shutil.rmtree(TestDataDirectory.basedir)
         if os.path.exists(TestDataDirectory.not_existing_dir):
             shutil.rmtree(TestDataDirectory.not_existing_dir)
 
+    def test_str(self) -> None:
+        data_dir = DataDirectory(TestDataDirectory.basedir)
+
+        assert str(data_dir) == TestDataDirectory.basedir
+
     def test_create_basedir_if_not_exists(self) -> None:
         _ = DataDirectory(TestDataDirectory.not_existing_dir)
 
         assert os.path.isdir(TestDataDirectory.not_existing_dir)
 
     def test_create_basedir_if_exists(self) -> None:
         _ = DataDirectory(TestDataDirectory.basedir)
```

