# Comparing `tmp/oauthAPImojang-0.3.1.tar.gz` & `tmp/oauthAPImojang-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthAPImojang-0.3.1.tar", last modified: Sun Apr 16 22:40:38 2023, max compression
+gzip compressed data, was "oauthAPImojang-0.3.2.tar", last modified: Sun Apr 16 23:48:07 2023, max compression
```

## Comparing `oauthAPImojang-0.3.1.tar` & `oauthAPImojang-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/
--rw-rw-rw-   0        0        0       61 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang/
--rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 oauthAPImojang-0.3.1/oauthAPImojang/__init__.py
--rw-rw-rw-   0        0        0    35440 2023-04-16 22:18:16.000000 oauthAPImojang-0.3.1/oauthAPImojang/minecraftTHEapi.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/
--rw-rw-rw-   0        0        0       61 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/oauthAPImojang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 22:40:40.000000 oauthAPImojang-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-04-16 22:19:26.000000 oauthAPImojang-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/
+-rw-rw-rw-   0        0        0       61 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/oauthAPImojang/
+-rw-rw-rw-   0        0        0    35440 2023-04-16 22:18:16.000000 oauthAPImojang-0.3.2/oauthAPImojang/SkyBlockAPI.py
+-rw-rw-rw-   0        0        0       97 2023-04-16 23:47:12.000000 oauthAPImojang-0.3.2/oauthAPImojang/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/oauthAPImojang.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/oauthAPImojang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/oauthAPImojang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/oauthAPImojang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/oauthAPImojang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/oauthAPImojang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 23:48:08.000000 oauthAPImojang-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-04-16 23:47:48.000000 oauthAPImojang-0.3.2/setup.py
```

### Comparing `oauthAPImojang-0.3.1/oauthAPImojang/minecraftTHEapi.py` & `oauthAPImojang-0.3.2/oauthAPImojang/SkyBlockAPI.py`

 * *Files identical despite different names*

