# Comparing `tmp/odoo_models_connect-0.1.1.tar.gz` & `tmp/odoo_models_connect-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_models_connect-0.1.1.tar", last modified: Sun Apr 16 15:03:50 2023, max compression
+gzip compressed data, was "odoo_models_connect-0.1.2.tar", last modified: Sun Apr 16 15:28:03 2023, max compression
```

## Comparing `odoo_models_connect-0.1.1.tar` & `odoo_models_connect-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:03:50.476564 odoo_models_connect-0.1.1/
--rw-rw-rw-   0        0        0     2955 2023-04-16 15:03:50.476564 odoo_models_connect-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2577 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 15:03:50.442640 odoo_models_connect-0.1.1/odoo_models_connect/
--rw-rw-rw-   0        0        0       39 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.1/odoo_models_connect/__init__.py
--rw-rw-rw-   0        0        0     5905 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.1/odoo_models_connect/connect_odoo.py
--rw-rw-rw-   0        0        0      686 2023-04-12 01:41:36.000000 odoo_models_connect-0.1.1/odoo_models_connect/fields.py
--rw-rw-rw-   0        0        0     3306 2023-04-16 15:03:16.000000 odoo_models_connect-0.1.1/odoo_models_connect/models.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:03:50.467354 odoo_models_connect-0.1.1/odoo_models_connect.egg-info/
--rw-rw-rw-   0        0        0     2955 2023-04-16 15:03:50.000000 odoo_models_connect-0.1.1/odoo_models_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-16 15:03:50.000000 odoo_models_connect-0.1.1/odoo_models_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:03:50.000000 odoo_models_connect-0.1.1/odoo_models_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 15:03:50.000000 odoo_models_connect-0.1.1/odoo_models_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-16 15:03:50.000000 odoo_models_connect-0.1.1/odoo_models_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:03:50.478692 odoo_models_connect-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-04-16 15:03:31.000000 odoo_models_connect-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:03.219671 odoo_models_connect-0.1.2/
+-rw-rw-rw-   0        0        0     2955 2023-04-16 15:28:03.218160 odoo_models_connect-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2577 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:03.174268 odoo_models_connect-0.1.2/odoo_models_connect/
+-rw-rw-rw-   0        0        0       39 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.2/odoo_models_connect/__init__.py
+-rw-rw-rw-   0        0        0     5905 2023-04-12 01:10:18.000000 odoo_models_connect-0.1.2/odoo_models_connect/connect_odoo.py
+-rw-rw-rw-   0        0        0      686 2023-04-12 01:41:36.000000 odoo_models_connect-0.1.2/odoo_models_connect/fields.py
+-rw-rw-rw-   0        0        0     4429 2023-04-16 15:27:28.000000 odoo_models_connect-0.1.2/odoo_models_connect/models.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:28:03.211099 odoo_models_connect-0.1.2/odoo_models_connect.egg-info/
+-rw-rw-rw-   0        0        0     2955 2023-04-16 15:28:02.000000 odoo_models_connect-0.1.2/odoo_models_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-16 15:28:02.000000 odoo_models_connect-0.1.2/odoo_models_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:28:02.000000 odoo_models_connect-0.1.2/odoo_models_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 15:28:02.000000 odoo_models_connect-0.1.2/odoo_models_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-16 15:28:02.000000 odoo_models_connect-0.1.2/odoo_models_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:28:03.219671 odoo_models_connect-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-04-16 15:27:37.000000 odoo_models_connect-0.1.2/setup.py
```

### Comparing `odoo_models_connect-0.1.1/PKG-INFO` & `odoo_models_connect-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_models_connect
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.1.1/README.md` & `odoo_models_connect-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.1/odoo_models_connect/connect_odoo.py` & `odoo_models_connect-0.1.2/odoo_models_connect/connect_odoo.py`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.1/odoo_models_connect/fields.py` & `odoo_models_connect-0.1.2/odoo_models_connect/fields.py`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.1/odoo_models_connect/models.py` & `odoo_models_connect-0.1.2/odoo_models_connect/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,54 @@
 import xmlrpc.client
 from xmlrpc.client import Error
 from .fields import OdooField
 from dotenv import dotenv_values
 from abc import ABC, abstractmethod
+import os
+from dotenv import load_dotenv
 
 
-config = dict(dotenv_values())
+def load_env_vars():
+    """
+    Carga las variables de entorno desde el archivo .env en el directorio actual
+    """
+    # Obtenemos la ruta del archivo actual que está siendo ejecutado
+    current_file_path = os.path.abspath(__file__)
+
+    # Obtenemos el directorio donde se encuentra el archivo actual
+    current_dir_path = os.path.dirname(current_file_path)
+
+    # Construimos la ruta completa al archivo .env
+    env_path = os.path.join(current_dir_path, '.env')
+
+    # Cargamos las variables de entorno desde el archivo .env
+    load_dotenv(env_path)
+
+def check_env_vars():
+    """
+    Verifica que se hayan definido correctamente las variables de entorno necesarias
+    """
+    required_env_vars = ['DATABASE', 'USERNAME', 'PASSWORD', 'URL']
+    for env_var in required_env_vars:
+        if not os.getenv(env_var):
+            raise Exception(f'La variable de entorno {env_var} no está definida')
+
+# Cargamos las variables de entorno desde el archivo .env
+load_env_vars()
+
+# Verificamos que se hayan definido correctamente las variables de entorno necesarias
+check_env_vars()
 
 
 class OdooModel(object):
     # Configuración de conexión a la instancia de Odoo
-    DATABASE = config.get('DATABASE')
-    USERNAME = config.get('USERNAME')
-    PASSWORD = config.get('PASSWORD')
-    URL = config.get('URL')
+    DATABASE = os.getenv('DATABASE')
+    USERNAME = os.getenv('USERNAME')
+    PASSWORD = os.getenv('PASSWORD')
+    URL = os.getenv('URL')
 
     COMMON = '/xmlrpc/2/common'
     OBJECTS = '/xmlrpc/2/object'
 
     UUID = None
     MODELS = None
```

### Comparing `odoo_models_connect-0.1.1/odoo_models_connect.egg-info/PKG-INFO` & `odoo_models_connect-0.1.2/odoo_models_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-models-connect
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.1.1/setup.py` & `odoo_models_connect-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.1'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.1.2'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 # Debe coincidir con el nombre de la carpeta
 PACKAGE_NAME = 'odoo_models_connect'
 AUTHOR = 'Deiver Jose Vazquez Moreno'  # Modificar con vuestros datos
 AUTHOR_EMAIL = 'estudiandovazmore@gmail.com'  # Modificar con vuestros datos
 # Modificar con vuestros datos
 URL = 'https://github.com/DeijoseDevelop/odoo_models_connect'
```

