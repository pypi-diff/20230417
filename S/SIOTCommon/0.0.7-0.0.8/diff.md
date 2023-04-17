# Comparing `tmp/SIOTCommon-0.0.7.tar.gz` & `tmp/SIOTCommon-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.7.tar", last modified: Wed Apr 12 16:56:22 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.8.tar", last modified: Mon Apr 17 13:06:17 2023, max compression
```

## Comparing `SIOTCommon-0.0.7.tar` & `SIOTCommon-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 16:56:22.249489 SIOTCommon-0.0.7/
--rw-rw-rw-   0        0        0      339 2023-04-12 16:56:22.248487 SIOTCommon-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 16:56:22.219486 SIOTCommon-0.0.7/SIOTC/
--rw-rw-rw-   0        0        0     1654 2023-04-11 17:33:40.000000 SIOTCommon-0.0.7/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6805 2023-04-12 00:41:58.000000 SIOTCommon-0.0.7/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.7/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-04-12 16:52:19.000000 SIOTCommon-0.0.7/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-12 16:56:22.246489 SIOTCommon-0.0.7/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      339 2023-04-12 16:56:22.000000 SIOTCommon-0.0.7/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-12 16:56:22.000000 SIOTCommon-0.0.7/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 16:56:22.000000 SIOTCommon-0.0.7/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-04-12 16:56:22.000000 SIOTCommon-0.0.7/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 16:56:22.000000 SIOTCommon-0.0.7/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 16:56:22.249489 SIOTCommon-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-04-12 16:56:19.000000 SIOTCommon-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:06:17.350705 SIOTCommon-0.0.8/
+-rw-rw-rw-   0        0        0      339 2023-04-17 13:06:17.350705 SIOTCommon-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:06:17.326725 SIOTCommon-0.0.8/SIOTC/
+-rw-rw-rw-   0        0        0     1653 2023-04-17 13:05:56.000000 SIOTCommon-0.0.8/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6805 2023-04-16 14:42:03.000000 SIOTCommon-0.0.8/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.8/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-04-12 16:52:19.000000 SIOTCommon-0.0.8/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:06:17.348706 SIOTCommon-0.0.8/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-04-17 13:06:17.000000 SIOTCommon-0.0.8/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-17 13:06:17.000000 SIOTCommon-0.0.8/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:06:17.000000 SIOTCommon-0.0.8/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-04-17 13:06:17.000000 SIOTCommon-0.0.8/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 13:06:17.000000 SIOTCommon-0.0.8/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:06:17.350705 SIOTCommon-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-04-17 13:06:13.000000 SIOTCommon-0.0.8/setup.py
```

### Comparing `SIOTCommon-0.0.7/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.8/SIOTC/DatabaseLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy import create_engine, Table
 from sqlalchemy.orm import sessionmaker, scoped_session
 
 def GetSession():
     Base = automap_base()
-    engine = create_engine('postgresql://postgres:postgres@localhost:5432/SweIoTdb', echo=True)
+    engine = create_engine('postgresql://postgres:3485780@localhost:5432/SweIoTdb', echo=True)
     Base.prepare(engine, reflect=True, schema='public')
     session_factory = sessionmaker(bind=engine)
     session = scoped_session(session_factory)
     return session, Base
 
 def GetModel(table_name):
     session, Base = GetSession()
```

### Comparing `SIOTCommon-0.0.7/SIOTC/Operations.py` & `SIOTCommon-0.0.8/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.7/SIOTC/helperhttps.py` & `SIOTCommon-0.0.8/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.7/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.0.8/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.7/setup.py` & `SIOTCommon-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

