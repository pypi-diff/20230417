# Comparing `tmp/p-ttauto-crawler-0.0.7.tar.gz` & `tmp/p-ttauto-crawler-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.0.7.tar", last modified: Mon Apr 17 01:30:41 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.0.8.tar", last modified: Mon Apr 17 03:39:14 2023, max compression
```

## Comparing `p-ttauto-crawler-0.0.7.tar` & `p-ttauto-crawler-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.103883 p-ttauto-crawler-0.0.7/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      397 2023-04-17 01:30:41.103883 p-ttauto-crawler-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.098883 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-17 01:30:41.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 01:30:40.000000 p-ttauto-crawler-0.0.7/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 01:30:41.103883 p-ttauto-crawler-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-04-17 01:30:36.000000 p-ttauto-crawler-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.100884 p-ttauto-crawler-0.0.7/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 01:30:41.102883 p-ttauto-crawler-0.0.7/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0    16746 2023-04-17 01:30:28.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0    10719 2023-04-14 06:00:31.000000 p-ttauto-crawler-0.0.7/ttauto_crawler/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.230369 p-ttauto-crawler-0.0.8/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-04-17 03:39:14.230369 p-ttauto-crawler-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.225368 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 03:39:14.000000 p-ttauto-crawler-0.0.8/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:39:14.231369 p-ttauto-crawler-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-04-17 03:38:05.000000 p-ttauto-crawler-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.228368 p-ttauto-crawler-0.0.8/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:39:14.229371 p-ttauto-crawler-0.0.8/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0    16746 2023-04-17 03:39:11.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0    10733 2023-04-17 03:37:59.000000 p-ttauto-crawler-0.0.8/ttauto_crawler/utils.py
```

### Comparing `p-ttauto-crawler-0.0.7/LICENSE` & `p-ttauto-crawler-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.0.7/setup.py` & `p-ttauto-crawler-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.0.7",
+    version="0.0.8",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-ttauto-crawler-0.0.7/ttauto_crawler/main.py` & `p-ttauto-crawler-0.0.8/ttauto_crawler/main.py`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.0.7/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.0.8/ttauto_crawler/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,10 +277,10 @@
 
     s = deepFtpUpload3(file, ftp, "")
     ftp.quit()
     return s
 
 def ftpUpload(file):
     try:
-        ftpUpload50(file)
+        return ftpUpload50(file)
     except:
-        ftpUpload3(file)
+        return ftpUpload3(file)
```

