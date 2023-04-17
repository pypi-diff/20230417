# Comparing `tmp/colabtunnel-0.0.1.tar.gz` & `tmp/colabtunnel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colabtunnel-0.0.1.tar", last modified: Mon Apr 17 20:28:29 2023, max compression
+gzip compressed data, was "colabtunnel-0.0.2.tar", last modified: Mon Apr 17 20:31:50 2023, max compression
```

## Comparing `colabtunnel-0.0.1.tar` & `colabtunnel-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 root         (0) root         (0)        0 2023-04-17 20:28:29.000000 colabtunnel-0.0.1/
--rw-------   0 root         (0) root         (0)     1071 2023-04-17 19:55:48.000000 colabtunnel-0.0.1/LICENSE
--rw-------   0 root         (0) root         (0)      612 2023-04-17 20:28:29.000000 colabtunnel-0.0.1/PKG-INFO
--rw-------   0 root         (0) root         (0)        0 2023-04-17 20:06:07.000000 colabtunnel-0.0.1/README.md
-drwx------   0 root         (0) root         (0)        0 2023-04-17 20:28:29.000000 colabtunnel-0.0.1/colabtunnel/
--rw-------   0 root         (0) root         (0)       59 2023-04-17 20:00:23.000000 colabtunnel-0.0.1/colabtunnel/__init__.py
--rw-------   0 root         (0) root         (0)     1647 2023-04-17 20:06:00.000000 colabtunnel-0.0.1/colabtunnel/colabtunnel.py
-drwx------   0 root         (0) root         (0)        0 2023-04-17 20:28:29.000000 colabtunnel-0.0.1/colabtunnel.egg-info/
--rw-------   0 root         (0) root         (0)      612 2023-04-17 20:28:28.000000 colabtunnel-0.0.1/colabtunnel.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      217 2023-04-17 20:28:28.000000 colabtunnel-0.0.1/colabtunnel.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2023-04-17 20:28:28.000000 colabtunnel-0.0.1/colabtunnel.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)       12 2023-04-17 20:28:28.000000 colabtunnel-0.0.1/colabtunnel.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2023-04-17 20:28:29.000000 colabtunnel-0.0.1/setup.cfg
--rw-------   0 root         (0) root         (0)      749 2023-04-17 20:06:19.000000 colabtunnel-0.0.1/setup.py
+drwx------   0 root         (0) root         (0)        0 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/
+-rw-------   0 root         (0) root         (0)     1071 2023-04-17 19:55:48.000000 colabtunnel-0.0.2/LICENSE
+-rw-------   0 root         (0) root         (0)      598 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/PKG-INFO
+-rw-------   0 root         (0) root         (0)        0 2023-04-17 20:06:07.000000 colabtunnel-0.0.2/README.md
+drwx------   0 root         (0) root         (0)        0 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel/
+-rw-------   0 root         (0) root         (0)       59 2023-04-17 20:31:31.000000 colabtunnel-0.0.2/colabtunnel/__init__.py
+-rw-------   0 root         (0) root         (0)     1647 2023-04-17 20:06:00.000000 colabtunnel-0.0.2/colabtunnel/colabtunnel.py
+drwx------   0 root         (0) root         (0)        0 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/
+-rw-------   0 root         (0) root         (0)      598 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      217 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)       12 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/colabtunnel.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)       38 2023-04-17 20:31:50.000000 colabtunnel-0.0.2/setup.cfg
+-rw-------   0 root         (0) root         (0)      735 2023-04-17 20:31:26.000000 colabtunnel-0.0.2/setup.py
```

### Comparing `colabtunnel-0.0.1/LICENSE` & `colabtunnel-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.1/colabtunnel/colabtunnel.py` & `colabtunnel-0.0.2/colabtunnel/colabtunnel.py`

 * *Files identical despite different names*

### Comparing `colabtunnel-0.0.1/setup.py` & `colabtunnel-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="colabtunnel",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
-    description="Run code-server on Google Colab with persistence of settings and code.",
+    description="Connect to Google Colab VM from your local VSCode Editor",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

