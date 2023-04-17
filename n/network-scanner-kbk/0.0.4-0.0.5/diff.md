# Comparing `tmp/network_scanner_kbk-0.0.4.tar.gz` & `tmp/network_scanner_kbk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Brian\2023\Joby\Challenge\network_scanner_kbk\dist\.tmp-gyds0ci1\network_scanner_kbk-0.0.4.tar", last modified: Sun Apr 16 22:36:55 2023, max compression
+gzip compressed data, was "C:\Brian\2023\Joby\Challenge\network_scanner_kbk\dist\.tmp-k7063hho\network_scanner_kbk-0.0.5.tar", last modified: Mon Apr 17 01:20:28 2023, max compression
```

## Comparing `network_scanner_kbk-0.0.4.tar` & `network_scanner_kbk-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 22:36:55.369254 network_scanner_kbk-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-16 17:12:52.000000 network_scanner_kbk-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      481 2023-04-16 22:36:55.369254 network_scanner_kbk-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      114 2023-04-16 15:31:31.000000 network_scanner_kbk-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 22:36:55.369254 network_scanner_kbk-0.0.4/network_scanner_kbk.egg-info/
--rw-rw-rw-   0        0        0      481 2023-04-16 22:36:55.000000 network_scanner_kbk-0.0.4/network_scanner_kbk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-16 22:36:55.000000 network_scanner_kbk-0.0.4/network_scanner_kbk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 22:36:55.000000 network_scanner_kbk-0.0.4/network_scanner_kbk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-16 22:36:55.000000 network_scanner_kbk-0.0.4/network_scanner_kbk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 22:36:55.369254 network_scanner_kbk-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-04-16 22:32:22.000000 network_scanner_kbk-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:36:55.369254 network_scanner_kbk-0.0.4/src/
--rw-rw-rw-   0        0        0        0 2023-04-16 15:33:58.000000 network_scanner_kbk-0.0.4/src/__init__.py
--rw-rw-rw-   0        0        0      304 2023-04-15 22:45:38.000000 network_scanner_kbk-0.0.4/src/example.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:36:55.369254 network_scanner_kbk-0.0.4/src/network_scanner/
--rw-rw-rw-   0        0        0        0 2023-04-16 15:33:58.000000 network_scanner_kbk-0.0.4/src/network_scanner/__init__.py
--rw-rw-rw-   0        0        0     7325 2023-04-16 17:15:22.000000 network_scanner_kbk-0.0.4/src/network_scanner/network_scanner.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:36:55.369254 network_scanner_kbk-0.0.4/test/
--rw-rw-rw-   0        0        0     3408 2023-04-15 20:13:16.000000 network_scanner_kbk-0.0.4/test/test_network_scanner.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:20:28.248050 network_scanner_kbk-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-16 17:12:52.000000 network_scanner_kbk-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-04-17 01:20:28.248050 network_scanner_kbk-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-16 15:31:31.000000 network_scanner_kbk-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 01:20:28.248050 network_scanner_kbk-0.0.5/network_scanner_kbk.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-04-17 01:20:28.000000 network_scanner_kbk-0.0.5/network_scanner_kbk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-17 01:20:28.000000 network_scanner_kbk-0.0.5/network_scanner_kbk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:20:28.000000 network_scanner_kbk-0.0.5/network_scanner_kbk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:20:28.000000 network_scanner_kbk-0.0.5/network_scanner_kbk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 01:20:28.248050 network_scanner_kbk-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-04-17 01:19:22.000000 network_scanner_kbk-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:20:28.248050 network_scanner_kbk-0.0.5/test/
+-rw-rw-rw-   0        0        0     3408 2023-04-15 20:13:16.000000 network_scanner_kbk-0.0.5/test/test_network_scanner.py
```

### Comparing `network_scanner_kbk-0.0.4/LICENSE` & `network_scanner_kbk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `network_scanner_kbk-0.0.4/setup.py` & `network_scanner_kbk-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 setup(
 	# Name of the package 
 	name='network_scanner_kbk',
 	# Packages to include into the distribution 
 	packages=find_packages('.'),
 	# Start with a small number and increase it with 
 	# every change you make https://semver.org 
-	version='0.0.4',
+	version='0.0.5',
 	# Chose a license from here: https: // 
 	# help.github.com / articles / licensing - a - 
 	# repository. For example: MIT 
 	license='MIT License',
 	# Short description of your library 
 	description='Project to scan and gather connectivity information on small networks',
 	# Long description of your library
```

### Comparing `network_scanner_kbk-0.0.4/test/test_network_scanner.py` & `network_scanner_kbk-0.0.5/test/test_network_scanner.py`

 * *Files identical despite different names*

