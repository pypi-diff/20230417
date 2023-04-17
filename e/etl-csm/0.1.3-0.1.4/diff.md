# Comparing `tmp/etl_csm-0.1.3.tar.gz` & `tmp/etl_csm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.1.3.tar", last modified: Fri Apr 14 17:05:08 2023, max compression
+gzip compressed data, was "etl_csm-0.1.4.tar", last modified: Mon Apr 17 14:48:33 2023, max compression
```

## Comparing `etl_csm-0.1.3.tar` & `etl_csm-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 17:05:08.090532 etl_csm-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-14 17:05:08.085532 etl_csm-0.1.3/Etl/
--rw-rw-rw-   0        0        0     3379 2023-04-14 17:04:18.000000 etl_csm-0.1.3/Etl/Execute.py
--rw-rw-rw-   0        0        0     1543 2023-04-14 17:04:18.000000 etl_csm-0.1.3/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/Helper.py
--rw-rw-rw-   0        0        0     1753 2023-04-14 17:04:18.000000 etl_csm-0.1.3/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.3/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      526 2023-04-14 17:05:08.089533 etl_csm-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 17:05:08.088532 etl_csm-0.1.3/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 17:05:08.090532 etl_csm-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      911 2023-04-14 17:04:42.000000 etl_csm-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:48:33.068051 etl_csm-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-17 14:48:33.063049 etl_csm-0.1.4/Etl/
+-rw-rw-rw-   0        0        0     3379 2023-04-17 14:37:44.000000 etl_csm-0.1.4/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1547 2023-04-17 14:38:05.000000 etl_csm-0.1.4/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1761 2023-04-17 14:38:26.000000 etl_csm-0.1.4/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.4/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      526 2023-04-17 14:48:33.067052 etl_csm-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 14:48:33.066049 etl_csm-0.1.4/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:48:33.068051 etl_csm-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      911 2023-04-17 14:48:31.000000 etl_csm-0.1.4/setup.py
```

### Comparing `etl_csm-0.1.3/Etl/Execute.py` & `etl_csm-0.1.4/Etl/Execute.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/Etl/Extrator.py` & `etl_csm-0.1.4/Etl/Extrator.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         ARGS
         query = Query a ser feita
     """
     try:
         engine = psycopg2.connect(
             database = 'postgres',
             user = 'tracking',
-            password = environ['SQL_PASSWORD'],
+            password = environ['SQL_PRD_PASSWORD'],
             host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
             port = '5432',
         )
     except (Exception,psycopg2.Error) as error:
         print(f'''
             Erro na conexão
             {error}
```

### Comparing `etl_csm-0.1.3/Etl/Helper.py` & `etl_csm-0.1.4/Etl/Helper.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/Etl/Loader.py` & `etl_csm-0.1.4/Etl/Loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from .Helper import psql_insert_copy,timing
 
 @timing
 def load_cloud(df:Type,bot:str) -> None:
     """
     Ira fazer o processo de carregamento para o RDS depois de processado.
     """
-    engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PASSWORD']}@prd-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
+    engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PRD_PASSWORD']}@prd-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
     tries = 10
     for _ in range(tries):
         try:
             df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',method = psql_insert_copy,index = False,chunksize = 10000)
             break
         except (Exception,psycopg2.Error) as error:
             warning("Fazendo novo conexao com a clean data para adicionar coluna!")
             engine = psycopg2.connect(
                 database = 'clean_data',
                 user = 'tracking',
-                password = environ['SQL_PASSWORD'],
+                password = environ['SQL_PRD_PASSWORD'],
                 host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
                 port = '5432',
             )
             cursor = engine.cursor()
             column = findall('"(.*?)"',str(error))[0]
             warning(f"Tive que acrescentar mais uma coluna ao seu dataframe ja existente a coluna foi {column}")
             query = f"""
```

### Comparing `etl_csm-0.1.3/Etl/Treatment_extras.py` & `etl_csm-0.1.4/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/Etl/Treatment_tracking.py` & `etl_csm-0.1.4/Etl/Treatment_tracking.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/Etl/Treatment_tracking_pme.py` & `etl_csm-0.1.4/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/Etl/__init__.py` & `etl_csm-0.1.4/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/LICENSE` & `etl_csm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/PKG-INFO` & `etl_csm-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.3/README.md` & `etl_csm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.3/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.4/etl_csm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.3/setup.py` & `etl_csm-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
```

