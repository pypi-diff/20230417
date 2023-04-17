# Comparing `tmp/optimyzer_api_client-0.5.0.tar.gz` & `tmp/optimyzer_api_client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimyzer_api_client-0.5.0.tar", last modified: Sat Apr 15 16:10:50 2023, max compression
+gzip compressed data, was "optimyzer_api_client-0.5.1.tar", last modified: Mon Apr 17 12:40:48 2023, max compression
```

## Comparing `optimyzer_api_client-0.5.0.tar` & `optimyzer_api_client-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:10:50.392681 optimyzer_api_client-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-15 16:10:50.392681 optimyzer_api_client-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-15 16:10:50.393681 optimyzer_api_client-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1741 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:10:50.386680 optimyzer_api_client-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:10:50.390680 optimyzer_api_client-0.5.0/src/optimyzer_api_client/
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4870 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client/api_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4624 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     7635 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client/machine.py
--rw-rw-rw-   0 root         (0) root         (0)    10504 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-04-15 16:10:29.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client/secret_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 16:10:50.391680 optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-15 16:10:50.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      524 2023-04-15 16:10:50.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 16:10:50.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-15 16:10:50.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-15 16:10:50.000000 optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:40:48.196428 optimyzer_api_client-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-04-17 12:40:48.196428 optimyzer_api_client-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-17 12:40:48.197428 optimyzer_api_client-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1741 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:40:48.190427 optimyzer_api_client-0.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:40:48.194427 optimyzer_api_client-0.5.1/src/optimyzer_api_client/
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4870 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client/api_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4624 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7635 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client/machine.py
+-rw-rw-rw-   0 root         (0) root         (0)    10504 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-04-17 12:40:28.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client/secret_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:40:48.195428 optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-04-17 12:40:48.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2023-04-17 12:40:48.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 12:40:48.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-17 12:40:48.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 12:40:48.000000 optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/top_level.txt
```

### Comparing `optimyzer_api_client-0.5.0/LICENSE` & `optimyzer_api_client-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimyzer_api_client-0.5.0/PKG-INFO` & `optimyzer_api_client-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimyzer_api_client
-Version: 0.5.0
+Version: 0.5.1
 Summary: An API Client for Optimyzer
 Home-page: https://gitlab.com/gauss-ml-open/optimyzer-api-client
 Author: Gauss Machine Learning GmbH
 Author-email: info@gauss-ml.com
 License: UNKNOWN
 Keywords: parameter optimization,machine learning,artificial intelligence,neural networks
 Platform: UNKNOWN
@@ -38,32 +38,32 @@
 
 Installing the `Optimyzer API Client` is very easy, just run `pip install optimyzer_api_client`
 in your favorite Python environment and you're done. If you like it, you might want to add
 `optimyzer_api_client` to your project's dependencies.
 
 ## Optimyzer Usage
 
-`Optimyzer` has been built to be included in any kind of workflow as easily as possible. 
+`OptimyzerClient` has been built to be included in any kind of workflow as easily as possible. 
 
 First you have to import it:
 
 ```python
-from optimyzer_api_client import Optimyzer
+from optimyzer_api_client import OptimyzerClient
 ```
 
 Then you need to create an instance using your `Optimyzer` username and password.
 
 ```python
-oac = Optimyzer(username="your@email.com", password="AVery$ecureP@ssw0rd!")
+oac = OptimyzerClient.from_login(username="your@email.com", password="AVery$ecureP@ssw0rd!")
 ```
 
 You can also use a credentials file.
 
 ```python
-oac = Optimyzer.from_credentials("/path/to/credentials_file.json")
+oac = OptimyzerClient.from_credentials("/path/to/credentials_file.json")
 ```
 
 Once you have an `Optimyzer API Client` instance, you can start creating machines, optimizations,
 and runing them.
 Check out the `notebooks` on this repository for examples on how to get started.
```

### Comparing `optimyzer_api_client-0.5.0/README.md` & `optimyzer_api_client-0.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 Installing the `Optimyzer API Client` is very easy, just run `pip install optimyzer_api_client`
 in your favorite Python environment and you're done. If you like it, you might want to add
 `optimyzer_api_client` to your project's dependencies.
 
 ## Optimyzer Usage
 
-`Optimyzer` has been built to be included in any kind of workflow as easily as possible. 
+`OptimyzerClient` has been built to be included in any kind of workflow as easily as possible. 
 
 First you have to import it:
 
 ```python
-from optimyzer_api_client import Optimyzer
+from optimyzer_api_client import OptimyzerClient
 ```
 
 Then you need to create an instance using your `Optimyzer` username and password.
 
 ```python
-oac = Optimyzer(username="your@email.com", password="AVery$ecureP@ssw0rd!")
+oac = OptimyzerClient.from_login(username="your@email.com", password="AVery$ecureP@ssw0rd!")
 ```
 
 You can also use a credentials file.
 
 ```python
-oac = Optimyzer.from_credentials("/path/to/credentials_file.json")
+oac = OptimyzerClient.from_credentials("/path/to/credentials_file.json")
 ```
 
 Once you have an `Optimyzer API Client` instance, you can start creating machines, optimizations,
 and runing them.
 Check out the `notebooks` on this repository for examples on how to get started.
```

### Comparing `optimyzer_api_client-0.5.0/setup.py` & `optimyzer_api_client-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `optimyzer_api_client-0.5.0/src/optimyzer_api_client/api_connection.py` & `optimyzer_api_client-0.5.1/src/optimyzer_api_client/api_connection.py`

 * *Files identical despite different names*

### Comparing `optimyzer_api_client-0.5.0/src/optimyzer_api_client/client.py` & `optimyzer_api_client-0.5.1/src/optimyzer_api_client/client.py`

 * *Files identical despite different names*

### Comparing `optimyzer_api_client-0.5.0/src/optimyzer_api_client/machine.py` & `optimyzer_api_client-0.5.1/src/optimyzer_api_client/machine.py`

 * *Files identical despite different names*

### Comparing `optimyzer_api_client-0.5.0/src/optimyzer_api_client/optimization.py` & `optimyzer_api_client-0.5.1/src/optimyzer_api_client/optimization.py`

 * *Files identical despite different names*

### Comparing `optimyzer_api_client-0.5.0/src/optimyzer_api_client/secret_loader.py` & `optimyzer_api_client-0.5.1/src/optimyzer_api_client/secret_loader.py`

 * *Files identical despite different names*

### Comparing `optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/PKG-INFO` & `optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimyzer-api-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: An API Client for Optimyzer
 Home-page: https://gitlab.com/gauss-ml-open/optimyzer-api-client
 Author: Gauss Machine Learning GmbH
 Author-email: info@gauss-ml.com
 License: UNKNOWN
 Keywords: parameter optimization,machine learning,artificial intelligence,neural networks
 Platform: UNKNOWN
@@ -38,32 +38,32 @@
 
 Installing the `Optimyzer API Client` is very easy, just run `pip install optimyzer_api_client`
 in your favorite Python environment and you're done. If you like it, you might want to add
 `optimyzer_api_client` to your project's dependencies.
 
 ## Optimyzer Usage
 
-`Optimyzer` has been built to be included in any kind of workflow as easily as possible. 
+`OptimyzerClient` has been built to be included in any kind of workflow as easily as possible. 
 
 First you have to import it:
 
 ```python
-from optimyzer_api_client import Optimyzer
+from optimyzer_api_client import OptimyzerClient
 ```
 
 Then you need to create an instance using your `Optimyzer` username and password.
 
 ```python
-oac = Optimyzer(username="your@email.com", password="AVery$ecureP@ssw0rd!")
+oac = OptimyzerClient.from_login(username="your@email.com", password="AVery$ecureP@ssw0rd!")
 ```
 
 You can also use a credentials file.
 
 ```python
-oac = Optimyzer.from_credentials("/path/to/credentials_file.json")
+oac = OptimyzerClient.from_credentials("/path/to/credentials_file.json")
 ```
 
 Once you have an `Optimyzer API Client` instance, you can start creating machines, optimizations,
 and runing them.
 Check out the `notebooks` on this repository for examples on how to get started.
```

### Comparing `optimyzer_api_client-0.5.0/src/optimyzer_api_client.egg-info/SOURCES.txt` & `optimyzer_api_client-0.5.1/src/optimyzer_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

