# Comparing `tmp/squad-sagemaker-db-connector-0.1.tar.gz` & `tmp/squad-sagemaker-db-connector-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squad-sagemaker-db-connector-0.1.tar", last modified: Mon Apr 17 08:30:26 2023, max compression
+gzip compressed data, was "squad-sagemaker-db-connector-0.2.tar", last modified: Mon Apr 17 09:30:14 2023, max compression
```

## Comparing `squad-sagemaker-db-connector-0.1.tar` & `squad-sagemaker-db-connector-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ujjwal     (501) staff       (20)        0 2023-04-17 08:30:26.880888 squad-sagemaker-db-connector-0.1/
--rw-r--r--   0 ujjwal     (501) staff       (20)     1482 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/LICENSE
--rw-r--r--   0 ujjwal     (501) staff       (20)       61 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/MANIFEST.in
--rw-r--r--   0 ujjwal     (501) staff       (20)     7827 2023-04-17 08:30:26.880985 squad-sagemaker-db-connector-0.1/PKG-INFO
--rw-r--r--   0 ujjwal     (501) staff       (20)     6935 2023-04-14 08:56:26.000000 squad-sagemaker-db-connector-0.1/README.rst
-drwxr-xr-x   0 ujjwal     (501) staff       (20)        0 2023-04-17 08:30:26.879155 squad-sagemaker-db-connector-0.1/auctm_database_connector/
--rw-r--r--   0 ujjwal     (501) staff       (20)       56 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/auctm_database_connector/__init__.py
--rw-r--r--   0 ujjwal     (501) staff       (20)      842 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/auctm_database_connector/bifrost.py
--rw-r--r--   0 ujjwal     (501) staff       (20)     1070 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/auctm_database_connector/decision_science.py
--rw-r--r--   0 ujjwal     (501) staff       (20)     1257 2023-04-17 07:08:41.000000 squad-sagemaker-db-connector-0.1/auctm_database_connector/sagemaker.py
--rw-r--r--   0 ujjwal     (501) staff       (20)     1268 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/auctm_database_connector/squadiq.py
--rw-r--r--   0 ujjwal     (501) staff       (20)      999 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/auctm_database_connector/substrate.py
--rw-r--r--   0 ujjwal     (501) staff       (20)     2801 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.1/auctm_database_connector/utils.py
--rw-r--r--   0 ujjwal     (501) staff       (20)      832 2023-04-17 08:30:26.881376 squad-sagemaker-db-connector-0.1/setup.cfg
--rw-r--r--   0 ujjwal     (501) staff       (20)     1552 2023-04-17 08:30:24.000000 squad-sagemaker-db-connector-0.1/setup.py
-drwxr-xr-x   0 ujjwal     (501) staff       (20)        0 2023-04-17 08:30:26.880697 squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/
--rw-r--r--   0 ujjwal     (501) staff       (20)     7827 2023-04-17 08:30:26.000000 squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/PKG-INFO
--rw-r--r--   0 ujjwal     (501) staff       (20)      623 2023-04-17 08:30:26.000000 squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/SOURCES.txt
--rw-r--r--   0 ujjwal     (501) staff       (20)        1 2023-04-17 08:30:26.000000 squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/dependency_links.txt
--rw-r--r--   0 ujjwal     (501) staff       (20)        1 2023-04-17 08:07:26.000000 squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/not-zip-safe
--rw-r--r--   0 ujjwal     (501) staff       (20)       57 2023-04-17 08:30:26.000000 squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/requires.txt
--rw-r--r--   0 ujjwal     (501) staff       (20)       25 2023-04-17 08:30:26.000000 squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/top_level.txt
+drwxr-xr-x   0 ujjwal     (501) staff       (20)        0 2023-04-17 09:30:14.262370 squad-sagemaker-db-connector-0.2/
+-rw-r--r--   0 ujjwal     (501) staff       (20)     1482 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/LICENSE
+-rw-r--r--   0 ujjwal     (501) staff       (20)       61 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/MANIFEST.in
+-rw-r--r--   0 ujjwal     (501) staff       (20)     7821 2023-04-17 09:30:14.262442 squad-sagemaker-db-connector-0.2/PKG-INFO
+-rw-r--r--   0 ujjwal     (501) staff       (20)     6929 2023-04-17 09:27:08.000000 squad-sagemaker-db-connector-0.2/README.rst
+drwxr-xr-x   0 ujjwal     (501) staff       (20)        0 2023-04-17 09:30:14.261129 squad-sagemaker-db-connector-0.2/database_connector/
+-rw-r--r--   0 ujjwal     (501) staff       (20)       56 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/database_connector/__init__.py
+-rw-r--r--   0 ujjwal     (501) staff       (20)      842 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/database_connector/bifrost.py
+-rw-r--r--   0 ujjwal     (501) staff       (20)     1070 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/database_connector/decision_science.py
+-rw-r--r--   0 ujjwal     (501) staff       (20)     1257 2023-04-17 07:08:41.000000 squad-sagemaker-db-connector-0.2/database_connector/sagemaker.py
+-rw-r--r--   0 ujjwal     (501) staff       (20)     1268 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/database_connector/squadiq.py
+-rw-r--r--   0 ujjwal     (501) staff       (20)      999 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/database_connector/substrate.py
+-rw-r--r--   0 ujjwal     (501) staff       (20)     2801 2023-04-14 08:40:00.000000 squad-sagemaker-db-connector-0.2/database_connector/utils.py
+-rw-r--r--   0 ujjwal     (501) staff       (20)      832 2023-04-17 09:30:14.262726 squad-sagemaker-db-connector-0.2/setup.cfg
+-rw-r--r--   0 ujjwal     (501) staff       (20)     1565 2023-04-17 09:30:12.000000 squad-sagemaker-db-connector-0.2/setup.py
+drwxr-xr-x   0 ujjwal     (501) staff       (20)        0 2023-04-17 09:30:14.262244 squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/
+-rw-r--r--   0 ujjwal     (501) staff       (20)     7821 2023-04-17 09:30:14.000000 squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/PKG-INFO
+-rw-r--r--   0 ujjwal     (501) staff       (20)      581 2023-04-17 09:30:14.000000 squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 ujjwal     (501) staff       (20)        1 2023-04-17 09:30:14.000000 squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 ujjwal     (501) staff       (20)        1 2023-04-17 08:07:26.000000 squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/not-zip-safe
+-rw-r--r--   0 ujjwal     (501) staff       (20)       57 2023-04-17 09:30:14.000000 squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/requires.txt
+-rw-r--r--   0 ujjwal     (501) staff       (20)       19 2023-04-17 09:30:14.000000 squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/top_level.txt
```

### Comparing `squad-sagemaker-db-connector-0.1/LICENSE` & `squad-sagemaker-db-connector-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/PKG-INFO` & `squad-sagemaker-db-connector-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squad-sagemaker-db-connector
-Version: 0.1
+Version: 0.2
 Summary: A pluggable connector that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://github.com/squadrun/auctm-database-connector
 Author: Ujjwal Gupta
 Author-email: ujjwal.gupta@squadstack.com
 License: MIT
 Keywords: Db connector
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,15 +60,15 @@
 This module provides the database connection for the SquadIQ database. It provides **read-only** access to the database.
 
 Usage
 ------
 
 .. code-block:: python
 
-    from auctm_database_connector import bifrost, substrate, decision_science, squadiq, sagemaker
+    from database_connector import bifrost, substrate, decision_science, squadiq, sagemaker
 
     bifrost_engine = bifrost.engine
     substrate_engine = substrate.engine
     ds_engine = decision_science.engine
     iq_engine = squadiq.engine
     ds_sagemaker_engine = sagemaker.engine
```

### Comparing `squad-sagemaker-db-connector-0.1/README.rst` & `squad-sagemaker-db-connector-0.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 This module provides the database connection for the SquadIQ database. It provides **read-only** access to the database.
 
 Usage
 ------
 
 .. code-block:: python
 
-    from auctm_database_connector import bifrost, substrate, decision_science, squadiq, sagemaker
+    from database_connector import bifrost, substrate, decision_science, squadiq, sagemaker
 
     bifrost_engine = bifrost.engine
     substrate_engine = substrate.engine
     ds_engine = decision_science.engine
     iq_engine = squadiq.engine
     ds_sagemaker_engine = sagemaker.engine
```

### Comparing `squad-sagemaker-db-connector-0.1/auctm_database_connector/bifrost.py` & `squad-sagemaker-db-connector-0.2/database_connector/bifrost.py`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/auctm_database_connector/decision_science.py` & `squad-sagemaker-db-connector-0.2/database_connector/decision_science.py`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/auctm_database_connector/sagemaker.py` & `squad-sagemaker-db-connector-0.2/database_connector/sagemaker.py`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/auctm_database_connector/squadiq.py` & `squad-sagemaker-db-connector-0.2/database_connector/squadiq.py`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/auctm_database_connector/substrate.py` & `squad-sagemaker-db-connector-0.2/database_connector/substrate.py`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/auctm_database_connector/utils.py` & `squad-sagemaker-db-connector-0.2/database_connector/utils.py`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/setup.cfg` & `squad-sagemaker-db-connector-0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `squad-sagemaker-db-connector-0.1/setup.py` & `squad-sagemaker-db-connector-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="squad-sagemaker-db-connector",
+    version="0.2",
     author="Ujjwal Gupta",
     author_email="ujjwal.gupta@squadstack.com",
     description=("A pluggable connector that allows users (admins) to execute SQL,"
                  " view, and export the results."),
     license="MIT",
     keywords="Db connector",
     url="https://github.com/squadrun/auctm-database-connector",
-    packages=['auctm_database_connector'],
+    packages=['database_connector'],
     long_description=read('README.rst'),
     long_description_content_type='text/plain',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Topic :: Utilities',
```

### Comparing `squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/PKG-INFO` & `squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squad-sagemaker-db-connector
-Version: 0.1
+Version: 0.2
 Summary: A pluggable connector that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://github.com/squadrun/auctm-database-connector
 Author: Ujjwal Gupta
 Author-email: ujjwal.gupta@squadstack.com
 License: MIT
 Keywords: Db connector
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,15 +60,15 @@
 This module provides the database connection for the SquadIQ database. It provides **read-only** access to the database.
 
 Usage
 ------
 
 .. code-block:: python
 
-    from auctm_database_connector import bifrost, substrate, decision_science, squadiq, sagemaker
+    from database_connector import bifrost, substrate, decision_science, squadiq, sagemaker
 
     bifrost_engine = bifrost.engine
     substrate_engine = substrate.engine
     ds_engine = decision_science.engine
     iq_engine = squadiq.engine
     ds_sagemaker_engine = sagemaker.engine
```

### Comparing `squad-sagemaker-db-connector-0.1/squad_sagemaker_db_connector.egg-info/SOURCES.txt` & `squad-sagemaker-db-connector-0.2/squad_sagemaker_db_connector.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-auctm_database_connector/__init__.py
-auctm_database_connector/bifrost.py
-auctm_database_connector/decision_science.py
-auctm_database_connector/sagemaker.py
-auctm_database_connector/squadiq.py
-auctm_database_connector/substrate.py
-auctm_database_connector/utils.py
+database_connector/__init__.py
+database_connector/bifrost.py
+database_connector/decision_science.py
+database_connector/sagemaker.py
+database_connector/squadiq.py
+database_connector/substrate.py
+database_connector/utils.py
 squad_sagemaker_db_connector.egg-info/PKG-INFO
 squad_sagemaker_db_connector.egg-info/SOURCES.txt
 squad_sagemaker_db_connector.egg-info/dependency_links.txt
 squad_sagemaker_db_connector.egg-info/not-zip-safe
 squad_sagemaker_db_connector.egg-info/requires.txt
 squad_sagemaker_db_connector.egg-info/top_level.txt
```

