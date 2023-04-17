# Comparing `tmp/customvalidator-0.3.tar.gz` & `tmp/customvalidator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customvalidator-0.3.tar", last modified: Mon Apr 17 11:27:25 2023, max compression
+gzip compressed data, was "customvalidator-0.4.tar", last modified: Mon Apr 17 11:34:01 2023, max compression
```

## Comparing `customvalidator-0.3.tar` & `customvalidator-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:27:25.556010 customvalidator-0.3/
--rw-rw-rw-   0        0        0       60 2023-04-17 11:27:25.556010 customvalidator-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 11:27:25.543333 customvalidator-0.3/customdbcred/
--rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customvalidator-0.3/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:27:25.544332 customvalidator-0.3/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customvalidator-0.3/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:27:25.545332 customvalidator-0.3/customvalidator/
--rw-rw-rw-   0        0        0      926 2023-03-25 03:37:23.000000 customvalidator-0.3/customvalidator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:27:25.555008 customvalidator-0.3/customvalidator.egg-info/
--rw-rw-rw-   0        0        0       60 2023-04-17 11:27:25.000000 customvalidator-0.3/customvalidator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-17 11:27:25.000000 customvalidator-0.3/customvalidator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:27:25.000000 customvalidator-0.3/customvalidator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 11:27:25.000000 customvalidator-0.3/customvalidator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 11:27:25.557361 customvalidator-0.3/setup.cfg
--rw-rw-rw-   0        0        0      204 2023-04-17 11:08:54.000000 customvalidator-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.503602 customvalidator-0.4/
+-rw-rw-rw-   0        0        0       60 2023-04-17 11:34:01.502602 customvalidator-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.484307 customvalidator-0.4/customdbcred/
+-rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customvalidator-0.4/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.486358 customvalidator-0.4/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customvalidator-0.4/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.487307 customvalidator-0.4/customvalidator/
+-rw-rw-rw-   0        0        0      926 2023-03-25 03:37:23.000000 customvalidator-0.4/customvalidator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.501588 customvalidator-0.4/customvalidator.egg-info/
+-rw-rw-rw-   0        0        0       60 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:34:01.503602 customvalidator-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      204 2023-04-17 11:33:48.000000 customvalidator-0.4/setup.py
```

### Comparing `customvalidator-0.3/customdbcred/__init__.py` & `customvalidator-0.4/customdbcred/__init__.py`

 * *Files identical despite different names*

### Comparing `customvalidator-0.3/customstatuscodes/__init__.py` & `customvalidator-0.4/customstatuscodes/__init__.py`

 * *Files identical despite different names*

### Comparing `customvalidator-0.3/customvalidator/__init__.py` & `customvalidator-0.4/customvalidator/__init__.py`

 * *Files identical despite different names*

