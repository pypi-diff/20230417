# Comparing `tmp/network_scanner_kbk-0.0.7.tar.gz` & `tmp/network_scanner_kbk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Brian\2023\Joby\Challenge\network_scanner_kbk\dist\.tmp-awv3ukpi\network_scanner_kbk-0.0.7.tar", last modified: Mon Apr 17 02:47:44 2023, max compression
+gzip compressed data, was "C:\Brian\2023\Joby\Challenge\network_scanner_kbk\dist\.tmp-98ud1c77\network_scanner_kbk-0.0.9.tar", last modified: Mon Apr 17 03:05:17 2023, max compression
```

## Comparing `network_scanner_kbk-0.0.7.tar` & `network_scanner_kbk-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:47:44.824471 network_scanner_kbk-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-04-16 17:12:52.000000 network_scanner_kbk-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      481 2023-04-17 02:47:44.824471 network_scanner_kbk-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      114 2023-04-16 15:31:31.000000 network_scanner_kbk-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 02:47:44.808880 network_scanner_kbk-0.0.7/network_scanner_kbk.egg-info/
--rw-rw-rw-   0        0        0      481 2023-04-17 02:47:44.000000 network_scanner_kbk-0.0.7/network_scanner_kbk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-04-17 02:47:44.000000 network_scanner_kbk-0.0.7/network_scanner_kbk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:47:44.000000 network_scanner_kbk-0.0.7/network_scanner_kbk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-17 02:47:44.000000 network_scanner_kbk-0.0.7/network_scanner_kbk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 02:47:44.824471 network_scanner_kbk-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-04-17 02:35:33.000000 network_scanner_kbk-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:47:44.808880 network_scanner_kbk-0.0.7/src/
--rw-rw-rw-   0        0        0       56 2023-04-17 02:40:09.000000 network_scanner_kbk-0.0.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:47:44.824471 network_scanner_kbk-0.0.7/src/network_scanner_pkg/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:46:12.000000 network_scanner_kbk-0.0.7/src/network_scanner_pkg/__init__.py
--rw-rw-rw-   0        0        0      304 2023-04-15 22:45:38.000000 network_scanner_kbk-0.0.7/src/network_scanner_pkg/example.py
--rw-rw-rw-   0        0        0     7325 2023-04-16 17:15:22.000000 network_scanner_kbk-0.0.7/src/network_scanner_pkg/network_scanner.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:47:44.824471 network_scanner_kbk-0.0.7/test/
--rw-rw-rw-   0        0        0     3408 2023-04-15 20:13:16.000000 network_scanner_kbk-0.0.7/test/test_network_scanner.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:05:17.791445 network_scanner_kbk-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-04-16 17:12:52.000000 network_scanner_kbk-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-04-17 03:05:17.791445 network_scanner_kbk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-16 15:31:31.000000 network_scanner_kbk-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:05:17.791445 network_scanner_kbk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2023-04-17 03:04:27.000000 network_scanner_kbk-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:05:17.760193 network_scanner_kbk-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:05:17.775823 network_scanner_kbk-0.0.9/src/network_scanner_kbk.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-04-17 03:05:17.000000 network_scanner_kbk-0.0.9/src/network_scanner_kbk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-04-17 03:05:17.000000 network_scanner_kbk-0.0.9/src/network_scanner_kbk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:05:17.000000 network_scanner_kbk-0.0.9/src/network_scanner_kbk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 03:05:17.000000 network_scanner_kbk-0.0.9/src/network_scanner_kbk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 03:05:17.775823 network_scanner_kbk-0.0.9/src/network_scanner_pkg/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:46:12.000000 network_scanner_kbk-0.0.9/src/network_scanner_pkg/__init__.py
+-rw-rw-rw-   0        0        0      304 2023-04-15 22:45:38.000000 network_scanner_kbk-0.0.9/src/network_scanner_pkg/example.py
+-rw-rw-rw-   0        0        0     7325 2023-04-16 17:15:22.000000 network_scanner_kbk-0.0.9/src/network_scanner_pkg/network_scanner.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:05:17.791445 network_scanner_kbk-0.0.9/test/
+-rw-rw-rw-   0        0        0     3408 2023-04-15 20:13:16.000000 network_scanner_kbk-0.0.9/test/test_network_scanner.py
```

### Comparing `network_scanner_kbk-0.0.7/LICENSE` & `network_scanner_kbk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `network_scanner_kbk-0.0.7/setup.py` & `network_scanner_kbk-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,20 @@
         long_description = f.read()
 except Exception:
     long_description = ''
 
 setup(
 	# Name of the package 
 	name='network_scanner_kbk',
+    package_dir = {'': 'src'},
 	# Packages to include into the distribution 
-	packages=find_packages('.'),
+	packages=["network_scanner_pkg"],
 	# Start with a small number and increase it with 
 	# every change you make https://semver.org 
-	version='0.0.7',
+	version='0.0.9',
 	# Chose a license from here: https: // 
 	# help.github.com / articles / licensing - a - 
 	# repository. For example: MIT 
 	license='MIT License',
 	# Short description of your library 
 	description='Project to scan and gather connectivity information on small networks',
 	# Long description of your library
```

### Comparing `network_scanner_kbk-0.0.7/src/network_scanner_pkg/network_scanner.py` & `network_scanner_kbk-0.0.9/src/network_scanner_pkg/network_scanner.py`

 * *Files identical despite different names*

### Comparing `network_scanner_kbk-0.0.7/test/test_network_scanner.py` & `network_scanner_kbk-0.0.9/test/test_network_scanner.py`

 * *Files identical despite different names*

