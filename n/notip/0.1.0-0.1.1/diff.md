# Comparing `tmp/notip-0.1.0.tar.gz` & `tmp/notip-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notip-0.1.0.tar", last modified: Mon Apr 17 10:07:27 2023, max compression
+gzip compressed data, was "notip-0.1.1.tar", last modified: Mon Apr 17 12:51:03 2023, max compression
```

## Comparing `notip-0.1.0.tar` & `notip-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 10:07:27.414547 notip-0.1.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1585 2023-04-17 10:07:27.414547 notip-0.1.0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      848 2023-04-17 09:55:41.000000 notip-0.1.0/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 10:07:27.414547 notip-0.1.0/notip.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1585 2023-04-17 10:07:27.000000 notip-0.1.0/notip.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      172 2023-04-17 10:07:27.000000 notip-0.1.0/notip.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 10:07:27.000000 notip-0.1.0/notip.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       60 2023-04-17 10:07:27.000000 notip-0.1.0/notip.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 10:07:27.000000 notip-0.1.0/notip.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-04-17 10:07:27.418547 notip-0.1.0/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      838 2023-04-17 09:53:49.000000 notip-0.1.0/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 12:51:03.134465 notip-0.1.1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1325 2023-04-17 12:51:03.134465 notip-0.1.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      848 2023-04-17 09:55:41.000000 notip-0.1.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 12:51:03.134465 notip-0.1.1/notip/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 12:46:44.000000 notip-0.1.1/notip/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26544 2022-07-01 17:10:03.000000 notip-0.1.1/notip/posthoc_fmri.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 12:51:03.134465 notip-0.1.1/notip.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1325 2023-04-17 12:51:03.000000 notip-0.1.1/notip.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-04-17 12:51:03.000000 notip-0.1.1/notip.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 12:51:03.000000 notip-0.1.1/notip.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       60 2023-04-17 12:51:03.000000 notip-0.1.1/notip.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-04-17 12:51:03.000000 notip-0.1.1/notip.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-04-17 12:51:03.134465 notip-0.1.1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      858 2023-04-17 12:50:38.000000 notip-0.1.1/setup.py
```

### Comparing `notip-0.1.0/README.md` & `notip-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `notip-0.1.0/setup.py` & `notip-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     readme = readme_file.read()
 
 requirements = ["numpy>=1.15.0", "scipy>=1.0.0",
                 "joblib>=1.0.1", "scikit-learn>=0.22"]
 
 setup(
     name="notip",
-    version="0.1.0",
+    version="0.1.1",
     author="Alexandre Blain",
     author_email="alexandre.blain@inria.fr",
     description="Nonparametric TDP control for brain imaging",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/alexblnn/Notip",
-    download_url="https://github.com/alexblnn/Notip/archive/refs/tags/0.1.0.tar.gz",
+    download_url="https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v1/notip-0.1.0.tar.gz",
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 )
```

