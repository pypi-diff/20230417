# Comparing `tmp/avsos-0.0.1.tar.gz` & `tmp/avsos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsos-0.0.1.tar", last modified: Mon Apr 17 21:48:39 2023, max compression
+gzip compressed data, was "avsos-0.0.2.tar", last modified: Mon Apr 17 21:51:43 2023, max compression
```

## Comparing `avsos-0.0.1.tar` & `avsos-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:48:39.289475 avsos-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 21:48:39.289475 avsos-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1469 2023-04-17 20:18:08.000000 avsos-0.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:48:39.289475 avsos-0.0.1/avsos/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.1/avsos/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)    17220 2023-04-17 20:49:03.000000 avsos-0.0.1/avsos/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5574 2023-04-17 20:49:19.000000 avsos-0.0.1/avsos/portscan.py
--rw-r--r--   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.1/avsos/setup.py
--rw-r--r--   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.1/avsos/start_zap.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5521 2023-04-17 20:49:09.000000 avsos-0.0.1/avsos/zapscan.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:48:39.289475 avsos-0.0.1/avsos.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 21:48:39.000000 avsos-0.0.1/avsos.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-04-17 21:48:39.000000 avsos-0.0.1/avsos.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-17 21:48:39.000000 avsos-0.0.1/avsos.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-17 21:48:39.000000 avsos-0.0.1/avsos.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      116 2023-04-17 21:48:39.000000 avsos-0.0.1/avsos.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-17 21:48:39.000000 avsos-0.0.1/avsos.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-17 21:48:39.289475 avsos-0.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      349 2023-04-17 21:47:25.000000 avsos-0.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:51:43.825697 avsos-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 21:51:43.825697 avsos-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1469 2023-04-17 20:18:08.000000 avsos-0.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:51:43.821695 avsos-0.0.2/avsos/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.2/avsos/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1308 2023-04-17 10:40:51.000000 avsos-0.0.2/avsos/config.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.2/avsos/encryption.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    17220 2023-04-17 20:20:28.000000 avsos-0.0.2/avsos/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5753 2023-04-14 19:31:26.000000 avsos-0.0.2/avsos/osint.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5574 2023-04-17 10:41:29.000000 avsos-0.0.2/avsos/portscan.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.2/avsos/setup.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.2/avsos/start_zap.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.2/avsos/utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5521 2023-04-17 20:22:12.000000 avsos-0.0.2/avsos/zapscan.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 21:51:43.825697 avsos-0.0.2/avsos.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      361 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      108 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-17 21:51:43.000000 avsos-0.0.2/avsos.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-17 21:51:43.825697 avsos-0.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      349 2023-04-17 21:51:37.000000 avsos-0.0.2/setup.py
```

### Comparing `avsos-0.0.1/README.md` & `avsos-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `avsos-0.0.1/avsos/main.py` & `avsos-0.0.2/avsos/main.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.1/avsos/portscan.py` & `avsos-0.0.2/avsos/portscan.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.1/avsos/zapscan.py` & `avsos-0.0.2/avsos/zapscan.py`

 * *Files identical despite different names*

