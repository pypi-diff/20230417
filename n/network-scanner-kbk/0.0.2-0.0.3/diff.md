# Comparing `tmp/network_scanner_kbk-0.0.2.tar.gz` & `tmp/network_scanner_kbk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Brian\2023\Joby\Challenge\network_scanner_kbk\dist\.tmp-nyn1ndau\network_scanner_kbk-0.0.2.tar", last modified: Sun Apr 16 21:43:36 2023, max compression
+gzip compressed data, was "C:\Brian\2023\Joby\Challenge\network_scanner_kbk\dist\.tmp-vytq6a7m\network_scanner_kbk-0.0.3.tar", last modified: Sun Apr 16 22:22:16 2023, max compression
```

## Comparing `network_scanner_kbk-0.0.2.tar` & `network_scanner_kbk-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.687541 network_scanner_kbk-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-16 17:12:52.000000 network_scanner_kbk-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      285 2023-04-16 21:43:36.685548 network_scanner_kbk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      114 2023-04-16 15:31:31.000000 network_scanner_kbk-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.657204 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/
--rw-rw-rw-   0        0        0      285 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-16 21:43:36.000000 network_scanner_kbk-0.0.2/network_scanner_kbk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 21:43:36.687541 network_scanner_kbk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      371 2023-04-16 21:30:39.000000 network_scanner_kbk-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.677542 network_scanner_kbk-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-04-16 15:33:58.000000 network_scanner_kbk-0.0.2/src/__init__.py
--rw-rw-rw-   0        0        0      304 2023-04-15 22:45:38.000000 network_scanner_kbk-0.0.2/src/example.py
--rw-rw-rw-   0        0        0     7325 2023-04-16 17:15:22.000000 network_scanner_kbk-0.0.2/src/network_scanner.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:43:36.682540 network_scanner_kbk-0.0.2/test/
--rw-rw-rw-   0        0        0     3408 2023-04-15 20:13:16.000000 network_scanner_kbk-0.0.2/test/test_network_scanner.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:22:16.511551 network_scanner_kbk-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-16 17:12:52.000000 network_scanner_kbk-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-04-16 22:22:16.511551 network_scanner_kbk-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-16 15:31:31.000000 network_scanner_kbk-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 22:22:16.495914 network_scanner_kbk-0.0.3/network_scanner_kbk.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-04-16 22:22:16.000000 network_scanner_kbk-0.0.3/network_scanner_kbk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-16 22:22:16.000000 network_scanner_kbk-0.0.3/network_scanner_kbk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 22:22:16.000000 network_scanner_kbk-0.0.3/network_scanner_kbk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-16 22:22:16.000000 network_scanner_kbk-0.0.3/network_scanner_kbk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 22:22:16.511551 network_scanner_kbk-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-04-16 22:16:44.000000 network_scanner_kbk-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:22:16.495914 network_scanner_kbk-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-04-16 15:33:58.000000 network_scanner_kbk-0.0.3/src/__init__.py
+-rw-rw-rw-   0        0        0      304 2023-04-15 22:45:38.000000 network_scanner_kbk-0.0.3/src/example.py
+-rw-rw-rw-   0        0        0     7325 2023-04-16 17:15:22.000000 network_scanner_kbk-0.0.3/src/network_scanner.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:22:16.511551 network_scanner_kbk-0.0.3/test/
+-rw-rw-rw-   0        0        0     3408 2023-04-15 20:13:16.000000 network_scanner_kbk-0.0.3/test/test_network_scanner.py
```

### Comparing `network_scanner_kbk-0.0.2/LICENSE` & `network_scanner_kbk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `network_scanner_kbk-0.0.2/src/network_scanner.py` & `network_scanner_kbk-0.0.3/src/network_scanner.py`

 * *Files identical despite different names*

### Comparing `network_scanner_kbk-0.0.2/test/test_network_scanner.py` & `network_scanner_kbk-0.0.3/test/test_network_scanner.py`

 * *Files identical despite different names*

