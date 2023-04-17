# Comparing `tmp/smthforthetest1337-0.0.tar.gz` & `tmp/smthforthetest1337-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smthforthetest1337-0.0.tar", last modified: Mon Apr 17 16:40:28 2023, max compression
+gzip compressed data, was "smthforthetest1337-0.1.tar", last modified: Mon Apr 17 17:40:04 2023, max compression
```

## Comparing `smthforthetest1337-0.0.tar` & `smthforthetest1337-0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:28.358457 smthforthetest1337-0.0/
--rw-rw-rw-   0        0        0      203 2023-04-17 16:40:28.358457 smthforthetest1337-0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-17 16:40:28.358457 smthforthetest1337-0.0/setup.cfg
--rw-rw-rw-   0        0        0      239 2023-04-17 16:28:18.000000 smthforthetest1337-0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:28.327207 smthforthetest1337-0.0/smthforthetest1337/
--rw-rw-rw-   0        0        0       26 2023-04-17 16:36:56.000000 smthforthetest1337-0.0/smthforthetest1337/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:28.358457 smthforthetest1337-0.0/smthforthetest1337.egg-info/
--rw-rw-rw-   0        0        0      203 2023-04-17 16:40:28.000000 smthforthetest1337-0.0/smthforthetest1337.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-17 16:40:28.000000 smthforthetest1337-0.0/smthforthetest1337.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:40:28.000000 smthforthetest1337-0.0/smthforthetest1337.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:40:28.000000 smthforthetest1337-0.0/smthforthetest1337.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-04-17 16:40:28.000000 smthforthetest1337-0.0/smthforthetest1337.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 17:40:04.236821 smthforthetest1337-0.1/
+-rw-rw-rw-   0        0        0      133 2023-04-17 17:40:04.236821 smthforthetest1337-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:40:04.236821 smthforthetest1337-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      239 2023-04-17 17:38:05.000000 smthforthetest1337-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:40:04.205570 smthforthetest1337-0.1/smthforthetest1337/
+-rw-rw-rw-   0        0        0       32 2023-04-17 17:38:05.000000 smthforthetest1337-0.1/smthforthetest1337/_init_.py
+-rw-rw-rw-   0        0        0       26 2023-04-17 17:38:05.000000 smthforthetest1337-0.1/smthforthetest1337/class_files.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:40:04.236821 smthforthetest1337-0.1/smthforthetest1337.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-04-17 17:40:04.000000 smthforthetest1337-0.1/smthforthetest1337.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-17 17:40:04.000000 smthforthetest1337-0.1/smthforthetest1337.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:40:04.000000 smthforthetest1337-0.1/smthforthetest1337.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 16:40:28.000000 smthforthetest1337-0.1/smthforthetest1337.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-04-17 17:40:04.000000 smthforthetest1337-0.1/smthforthetest1337.egg-info/top_level.txt
```

