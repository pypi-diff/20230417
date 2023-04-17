# Comparing `tmp/satdigitalinvoice-3.0.2.tar.gz` & `tmp/satdigitalinvoice-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-3.0.2.tar", last modified: Sun Apr 16 00:16:02 2023, max compression
+gzip compressed data, was "satdigitalinvoice-3.0.3.tar", last modified: Mon Apr 17 06:15:52 2023, max compression
```

## Comparing `satdigitalinvoice-3.0.2.tar` & `satdigitalinvoice-3.0.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    37228 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 00:16:02.000000 satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:16:02.132963 satdigitalinvoice-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-16 00:15:46.000000 satdigitalinvoice-3.0.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34675 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 06:15:52.000000 satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:15:52.418050 satdigitalinvoice-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-17 06:15:36.000000 satdigitalinvoice-3.0.3/tests/test_main.py
```

### Comparing `satdigitalinvoice-3.0.2/PKG-INFO` & `satdigitalinvoice-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.2
+Version: 3.0.3
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/__init__.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import os
 import sys
 from zipfile import ZipFile
 import PySimpleGUI as sg
 
+
+
 SOURCE_DIRECTORY = os.path.dirname(__file__)
 
 DATA_DIRECTORY = ".data"
 ARCHIVOS_DIRECTORY = "archivos"
 TEMPLATES_DIRECTORY = "templates"
 TEMP_DIRECTORY = ".data/temp"
 
@@ -26,28 +28,19 @@
     formatter = logging.Formatter('%(asctime)s - %(message)s')
     fh.setFormatter(formatter)
     logging.root.addHandler(fh)
 
 
 class FacturacionLauncher:
     def __init__(self, cwd=None):
-        app_dir = os.getcwd()
+        self.app_dir = os.getcwd()
         if cwd:
             os.chdir(cwd)
         add_file_handler()
 
-        # loading the sample.zip
-        try:
-            with ZipFile(os.path.join(app_dir, 'sample.zip'), 'r') as zf:
-                for member in zf.infolist():
-                    if not os.path.exists(member.filename):
-                        zf.extract(member)
-        except FileNotFoundError:
-            pass
-
         # layout
         layout = [
             [sg.Column([[
                 sg.Image(source=os.path.join(SOURCE_DIRECTORY, "images", "logo.png"), pad=2),
             ]], justification='center', pad=0, background_color='black')],
             [
                 sg.Multiline(
@@ -78,22 +71,39 @@
         )
 
     @staticmethod
     def read_config():
         from satdigitalinvoice.file_data_managers import ConfigManager
         return ConfigManager()
 
+    def load_sample_files(self):
+        # loading the sample.zip
+        try:
+            with ZipFile(os.path.join(self.app_dir, 'sample.zip'), 'r') as zf:
+                for member in zf.infolist():
+                    if not os.path.exists(member.filename):
+                        zf.extract(member)
+        except FileNotFoundError:
+            pass
+
     def run(self):
         self.window.finalize()
         self.window.read(timeout=0)
 
         try:
+            # check if another directory is configured
+            from satdigitalinvoice.file_data_managers import InitManager
+            if cwd := InitManager().get('cwd'):
+                os.chdir(cwd)
+            self.load_sample_files()
+
             from satdigitalinvoice.facturacion import FacturacionGUI
-            config = self.read_config()
-            app = FacturacionGUI(config)
+            app = FacturacionGUI(
+                config=self.read_config()
+            )
         except Exception as ex:
             logging.exception(ex)
             self.window['console'].update(
                 f"Error al cargar la aplicación. {ex.__class__.__name__}: {ex}",
                 text_color='red4',
             )
             self.window.read()
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/__version__.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/environments.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/environments.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import jinja2
 from jinja2 import Environment, Undefined
 from jinja2.filters import do_mark_safe
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import iterate as h_iterate
+from satdigitalinvoice.formatting_functions.common import pesos, num_letras
 
 from . import TEMPLATES_DIRECTORY
 
 
 class FacturacionEnvironment(Environment):
     @property
     def filter(self):
@@ -41,16 +42,28 @@
             if isinstance(v, Undefined):
                 return v
             return h_iterate(v)
 
         @self.filter
         def bold(k):
             return do_mark_safe(
-                tag(html_escape(k), "b")
+                tag(html_escape(str(k)), "b")
             )
 
+        @self.filter
+        def moneda_nacional(k):
+            return pesos(k)
+
+        @self.filter
+        def numero(k):
+            return str(k) + ' (' + num_letras(k) + ')'
+
+        @self.filter
+        def porcentaje(k):
+            return str(k) + '% (' + num_letras(k) + ' POR CIENTO)'
+
 
 def tag(text, tag):
     return '<' + tag + '>' + text + '</' + tag + '>'
 
 
 facturacion_environment = FacturacionEnvironment()
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/facturacion.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 
 from . import __version__, PPD, PUE, TEMP_DIRECTORY
 from .client_validation import validar_client
 from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
-from .formatting_functions.common import fecha, pesos, porcentaje
+from .formatting_functions.common import fecha
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, archivos_filename, mf_pago_fmt, archivos_folder, period_desc, ajustes_directory, find_ajustes, \
     format_concepto_desc, generate_pdf_template, periodicidad_desc, parse_fecha_pago, parse_importe_pago, preview_cfdis
 from .layout import make_layout, ActionButtonManager
 from .localdb import LocalDBSatCFDI, LiquidatedState
 from .log_tools import cfdi_header, header_line, print_yaml
 from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder
 from .utils import random_string, parse_date_period, load_certificate, to_int, cert_info, add_month, clear_directory, find_best_match, months_between
@@ -59,30 +59,30 @@
         self.serie = config['serie']
         self.csd_signer = load_certificate(config.get('csd')) if 'csd' in config else None
         self.fiel_signer = load_certificate(config.get('fiel')) if 'fiel' in config else None
 
         self.sat_service = SAT(signer=self.fiel_signer)
         self.rfc_prediales = config['rfc_prediales']
 
-        self.window = PySimpleGUI.Window(
-            f"Facturación Mensual CFDI 4.0 {self.csd_signer.rfc}",
-            make_layout(bool(self.fiel_signer)),
-            size=(1280, 800),
-            resizable=True,
-            font=("Courier New", 10, "bold"),
-        )
-
         self.all_invoices = None
         self.local_db = LocalDBSatCFDI(
             enviar_a_partir=config['enviar_a_partir'],
             pagar_a_partir=config['pagar_a_partir']
         )
         # noinspection PyTypeChecker
         self.selected_satcfdi = None  # type: MyCFDI
 
+        self.window = PySimpleGUI.Window(
+            f"Facturación Mensual CFDI 4.0 {self.csd_signer.rfc}",
+            make_layout(bool(self.fiel_signer), self.local_db),
+            size=(1280, 800),
+            resizable=True,
+            font=("Courier New", 10, "bold"),
+        )
+
         self.action_button_manager = ActionButtonManager(self.window["crear_facturas"])
         self.console = self.window["console"]
 
         MyCFDI.local_db = self.local_db
 
     def run(self):
         self.window.finalize()
@@ -97,14 +97,20 @@
         self.window['emitidas_search'].bind("<Return>", "_enter")
 
         self.window['facturas_table'].bind('<Double-Button-1>', '_double_click')
         self.window['clientes_table'].bind('<Double-Button-1>', '_double_click')
         self.window['emitidas_table'].bind('<Double-Button-1>', '_double_click')
         self.window['ajustes_table'].bind('<Double-Button-1>', '_double_click')
 
+        self.window['facturas_table'].bind('<Control-KeyPress-a>', '+select_all')
+        self.window['clientes_table'].bind('<Control-KeyPress-a>', '+select_all')
+        self.window['emitidas_table'].bind('<Control-KeyPress-a>', '+select_all')
+        self.window['correos_table'].bind('<Control-KeyPress-a>', '+select_all')
+        self.window['ajustes_table'].bind('<Control-KeyPress-a>', '+select_all')
+
         # Add logging to the window
         h = logging.StreamHandler(self.window['console'])
         h.setLevel(logging.ERROR)
         logging.root.addHandler(h)
 
         self.main_loop()
         self.window.close()
@@ -190,64 +196,97 @@
 
     def _read(self, timeout=0):
         event, values = self.window.read(timeout=timeout)
         if event in ("Exit", PySimpleGUI.WIN_CLOSED):
             exit(0)
 
     def action_button(self, action_name, action_items):
-        if action_name == 'facturas':
-            self.all_invoices = None
-            for invoice in action_items:
-                cfdi = self.generate_invoice(invoice=invoice)
-                if cfdi is None:
-                    break
-                print_yaml({
-                    "FacturaGenerada": cfdi_header(cfdi),
-                })
-                self._read()
-        elif action_name == 'correos':
-            clients = ClientsManager()
-            emisor_cif = clients[self.csd_signer.rfc]
-            with self.email_manager.sender as s:
-                for receptor, notify_invoices, pendientes_meses_anteriores in action_items:
-                    def attachments():
-                        for ni in notify_invoices:
-                            yield ni.filename + ".xml"
-                            yield ni.filename + ".pdf"
-
-                    subject = f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}"
-
-                    s.send_email(
-                        subject=subject,
-                        to_addrs=receptor["Email"],
-                        html=facturacion_environment.get_template('mail_facturas_template.html').render(
-                            facturas=notify_invoices,
-                            pendientes_meses_anteriores=pendientes_meses_anteriores,
-                            emisor=emisor_cif,
-                        ),
-                        file_attachments=attachments()
-                    )
-                    for r in notify_invoices:
-                        self.local_db.notified_set(r.uuid, True)
+        match action_name:
+            case 'facturas':
+                self.all_invoices = None
+                for invoice in action_items:
+                    cfdi = self.generate_invoice(invoice=invoice)
+                    if cfdi is None:
+                        break
                     print_yaml({
-                        "correo": subject,
-                        "para": receptor["Email"]
+                        "FacturaGenerada": cfdi_header(cfdi),
                     })
                     self._read()
-        elif action_name == 'clientes':
-            for client in action_items:
-                print(f"Validando: {client['Rfc']}")
-                validar_client(client)
-                self._read()
-        else:
-            raise ValueError(f"Invalid action: {action_name}")
+
+            case 'correos':
+                clients = ClientsManager()
+                emisor_cif = clients[self.csd_signer.rfc]
+                with self.email_manager.sender as s:
+                    for receptor, notify_invoices, pendientes_meses_anteriores in action_items:
+                        def attachments():
+                            for ni in notify_invoices:
+                                yield ni.filename + ".xml"
+                                yield ni.filename + ".pdf"
+
+                        subject = f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}"
+
+                        s.send_email(
+                            subject=subject,
+                            to_addrs=receptor["Email"],
+                            html=facturacion_environment.get_template('mail_facturas_template.html').render(
+                                facturas=notify_invoices,
+                                pendientes_meses_anteriores=pendientes_meses_anteriores,
+                                emisor=emisor_cif,
+                            ),
+                            file_attachments=attachments()
+                        )
+                        for r in notify_invoices:
+                            self.local_db.notified_set(r.uuid, True)
+                        print_yaml({
+                            "correo": subject,
+                            "para": receptor["Email"]
+                        })
+                        self._read()
+
+            case 'ajustes':
+                clients = ClientsManager()
+                emisor_cif = clients[self.csd_signer.rfc]
+                with self.email_manager.sender as s:
+                    for data in action_items:
+                        receptor = data['receptor']
+                        file_name = data['file_name']
+                        subject = f"Ajuste Renta {receptor['RazonSocial']} - {receptor['Rfc']}"
+
+                        if not data['ajuste_porcentaje']:
+                            print(f"NO HAY {subject}")
+                            continue
+
+                        s.send_email(
+                            subject=subject,
+                            to_addrs=receptor["Email"],
+                            html=facturacion_environment.get_template('mail_ajustes_template.html').render(
+                                emisor=emisor_cif,
+                            ),
+                            file_attachments=[file_name]
+                        )
+                        print_yaml({
+                            "correo": subject,
+                            "para": receptor["Email"]
+                        })
+                        self._read()
+
+            case 'clientes':
+                for client in action_items:
+                    print(f"Validando: {client['Rfc']}")
+                    validar_client(client)
+                    self._read()
+
+            case _:
+                raise ValueError(f"Invalid action: {action_name}")
+
         print("FIN")
 
-    def set_selected_satcfdi(self, factura):
-        i = factura
+    def set_selected_satcfdis(self, cfdis: list):
+        i = cfdis[0] if len(cfdis) == 1 else None
+
         self.selected_satcfdi = i
         if i:
             estado = self.local_db.status_sat(i).get('Estado', 'Vigente')
             self.window["status_sat"].update(
                 estado.center(10),
                 disabled=False,
                 button_color="red4" if estado != "Vigente" else "green",
@@ -318,59 +357,43 @@
                         and (
                         i.name == search_text
                         or i["Receptor"]["Rfc"] == search_text
                         or search_text in i["Receptor"].get("Nombre", "")
                 ):
                     yield i
 
-        cfdis = list(fact_iter())
-        self.emitidas_show(cfdis)
+        self.window['emitidas_table'].update(
+            values=list(fact_iter()),
+        )
 
     def facturas_pendientes(self):
         self.window["emitidas_text"].update("Facturas Pendientes de Pago")
 
         def fact_iter():
             for i in self.get_all_invoices().values():
                 if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                         and self.local_db.liquidated_state(i) == LiquidatedState.NO:
                     yield i
 
-        cfdis = list(fact_iter())
-        self.emitidas_show(cfdis)
+        self.window['emitidas_table'].update(
+            values=list(fact_iter()),
+        )
 
     def facturas_emitidas(self, dp):
         self.window["emitidas_text"].update("Facturas Emitidas en " + str(dp))
 
         def fact_iter():
             for i in self.get_all_invoices().values():
                 if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                         and i["Fecha"] == dp:
                     yield i
 
-        cfdis = list(fact_iter())
-        self.emitidas_show(cfdis)
-
-    def emitidas_show(self, cfdis):
-        rows = [
-            [
-                i,
-                cfdi['Receptor'].get('Nombre', '')[0:36],
-                cfdi['Receptor']['Rfc'],
-                cfdi.name,
-                cfdi["Fecha"].strftime("%Y-%m-%d"),
-                cfdi["Total"],
-                self.local_db.liquidated_state(cfdi),
-                mf_pago_fmt(cfdi)
-            ]
-            for i, cfdi in enumerate(cfdis, start=1)
-        ]
         self.window['emitidas_table'].update(
-            values=rows,
+            values=list(fact_iter()),
         )
-        self.window['emitidas_table'].metadata = cfdis
 
     def main_loop(self):
         while True:
             event, values = self.window.read()
             try:
                 if event in ("Exit", PySimpleGUI.WIN_CLOSED):
                     return
@@ -443,55 +466,26 @@
                             self.console.update("")
                             cfdis = generate_ingresos(
                                 clients=ClientsManager(),
                                 facturas=FacturasManager(dp)["Facturas"],
                                 dp=dp,
                                 emisor_rfc=self.csd_signer.rfc
                             )
-                            if cfdis is None:
+                            if cfdis:
+                                self.window['facturas_table'].update(
+                                    values=cfdis,
+                                )
+                            else:
                                 self.window['console_tab'].select()
                                 continue
 
-                            rows = [[
-                                i,
-                                cfdi['Emisor']['RegimenFiscal'].code,
-                                cfdi['Receptor']['Nombre'][0:36],
-                                cfdi['Receptor']['Rfc'],
-                                mf_pago_fmt(cfdi),
-                                cfdi['SubTotal'],
-                                cfdi['Total'],
-                            ]
-                                for i, cfdi in enumerate(cfdis, start=1)
-                            ]
-                            self.window['facturas_table'].update(
-                                values=rows,
-                            )
-                            self.window['facturas_table'].metadata = cfdis
-                            self.action_button_manager.set_items('facturas', cfdis)
-
                         if values['main_tab_group'] == 'clients_tab':
-                            self.window['clientes_table'].update(values=[])
-                            clients = list(ClientsManager().values())
-                            facturas = FacturasManager(dp)["Facturas"]
-                            rows = [
-                                [
-                                    i,
-                                    client["RazonSocial"][:36],
-                                    client["Rfc"],
-                                    client["RegimenFiscal"].code,
-                                    client["CodigoPostal"],
-                                    sum(1 for f in facturas if f["Receptor"] == client["Rfc"]) or "",
-                                ]
-                                for i, client in enumerate(clients, start=1)
-                            ]
                             self.window['clientes_table'].update(
-                                values=rows,
+                                values=list(ClientsManager().values()),
                             )
-                            self.window['clientes_table'].metadata = clients
-                            self.action_button_manager.set_items('clientes', clients)
 
                         if values['main_tab_group'] == 'emitidas_tab':
                             self.action_button_manager.clear()
                             self.facturas_pendientes()
 
                         if values['main_tab_group'] == 'correos_tab':
                             now = date.today()
@@ -521,174 +515,134 @@
                                 fac_pen = sorted(
                                     fac_pen_iter(),
                                     key=lambda r: r["Fecha"]
                                 )
                                 receptor = clients[receptor_rfc]
                                 cfdi_correos.append((receptor, notify_invoices, fac_pen))
 
-                            rows = [
-                                [
-                                    i,
-                                    receptor["RazonSocial"][0:36],
-                                    receptor["Rfc"],
-                                    ",".join(n.name for n in notify_invoices),
-                                    ",".join(n.name for n in facturas_pendientes)
-                                ] for i, (receptor, notify_invoices, facturas_pendientes) in enumerate(cfdi_correos, start=1)
-                            ]
                             self.window['correos_table'].update(
-                                values=rows,
+                                values=cfdi_correos,
                             )
-                            self.window['correos_table'].metadata = cfdi_correos
-                            self.action_button_manager.set_items('correos', cfdi_correos)
 
                         if values['main_tab_group'] == 'ajustes_tab':
+                            self.window['ajustes_table'].update(values=[])
                             if dp is None or dp.month is None:
                                 self.window['preparar_ajustes_text'].update("Periodo no válido")
-                                self.window['ajustes_table'].update(values=[])
                                 continue
 
                             dp_effective = add_month(dp, 1)
                             self.window['preparar_ajustes_text'].update(f"Ajustes Efectivos Al: {period_desc(dp_effective)}")
 
                             # clear directory
                             ajustes_dir = ajustes_directory(DatePeriod(dp.year, dp.month))
                             clear_directory(ajustes_dir)
                             emisor_rfc = self.csd_signer.rfc
 
                             clients = ClientsManager()
                             facturas = FacturasManager(None)["Facturas"]
 
                             def ajustes_iter():
-                                for i, (rfc, concepto) in enumerate(find_ajustes(facturas, dp_effective.month)):
-                                    receptor = clients[rfc]  # type: dict
+                                for i, (receptor_rfc, concepto) in enumerate(find_ajustes(facturas, dp_effective.month)):
                                     valor_unitario_raw = concepto["ValorUnitario"]
 
                                     if isinstance(valor_unitario_raw, dict):
-                                        vud, vu = find_best_match(valor_unitario_raw, dp)
-                                        vund, vun = find_best_match(valor_unitario_raw, dp_effective)
-                                        meses = months_between(vund, vud)
+                                        vu_eff, vu = find_best_match(valor_unitario_raw, dp)
+                                        vun_eff, vun = find_best_match(valor_unitario_raw, dp_effective)
+                                        if vu_eff == vun_eff:
+                                            vun = None
+                                            num_meses = None
+                                        else:
+                                            num_meses = months_between(vun_eff, vu_eff)
+
                                         if vun and vu:
-                                            ajuste_porcentaje = (vun / vu - 1)
+                                            ajuste_porcentaje = round((vun / vu - 1) * 100, 2)
                                         else:
                                             ajuste_porcentaje = None
                                     else:
                                         vu = valor_unitario_raw
                                         vun = None
-                                        meses = None
+                                        num_meses = None
                                         ajuste_porcentaje = None
 
                                     concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
-                                    file_name = os.path.join(ajustes_dir, f'AjusteRenta_{rfc}_{i}.pdf')
+                                    file_name = os.path.join(ajustes_dir, f'AjusteRenta_{receptor_rfc}_{i}.pdf')
 
+                                    client_receptor = clients[receptor_rfc]  # type: dict
                                     data = {
-                                        "receptor": receptor,
+                                        "receptor": client_receptor,
                                         "emisor": clients[emisor_rfc],
                                         "concepto": concepto,
-                                        "valor_unitario": pesos(vu) if vu else "",
-                                        "valor_unitario_nuevo": pesos(vun) if vun else "",
-                                        "ajuste_porcentaje": porcentaje(ajuste_porcentaje, 2) if ajuste_porcentaje is not None else "",
-                                        "ajuste_periodo": f"{meses} MESES",
+                                        "valor_unitario": vu,
+                                        "valor_unitario_nuevo": vun or '',
+                                        "ajuste_porcentaje": ajuste_porcentaje or "",
+                                        "meses": num_meses or '',
                                         "efectivo_periodo_desc": periodicidad_desc(dp_effective, concepto['_periodo_mes_ajuste'], concepto.get('_desfase_mes')),
                                         "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
                                         "fecha_hoy": fecha(date.today()),
                                         'file_name': file_name
                                     }
-                                    if ajuste_porcentaje is not None:
+
+                                    if ajuste_porcentaje:
                                         res = generate_pdf_template(
                                             template_name='incremento_template.md',
                                             fields=data
                                         )
                                         with open(file_name, 'wb') as f:
                                             f.write(res)
                                     yield data
 
-                            ajustes_iter = list(ajustes_iter())
-                            rows = [
-                                [
-                                    i,
-                                    ajuste["receptor"]["RazonSocial"][:36],
-                                    ajuste["receptor"]["Rfc"],
-                                    ajuste["valor_unitario"].split(' ')[0],
-                                    ajuste["valor_unitario_nuevo"].split(' ')[0],
-                                    ajuste["ajuste_porcentaje"].split(' ')[0],
-                                    ajuste["periodo"],
-                                    ajuste["ajuste_periodo"],
-                                    ajuste["efectivo_periodo_desc"]
-                                ]
-                                for i, ajuste in enumerate(ajustes_iter, start=1)
-                            ]
                             self.window['ajustes_table'].update(
-                                values=rows,
+                                values=list(ajustes_iter()),
                             )
-                            self.window['ajustes_table'].metadata = ajustes_iter
-                            self.action_button_manager.set_items('ajustes', ajustes_iter)
 
                     case "facturas_pendientes":
                         self.facturas_pendientes()
 
                     case "facturas_emitidas":
                         self.facturas_emitidas(dp)
 
                     case 'facturas_table_double_click':
-                        items = self.window["facturas_table"].metadata
-                        selection = values["facturas_table"]
-                        s_items = [items[i] for i in selection] if selection else items
+                        # noinspection PyUnresolvedReferences
+                        s_items = self.window["facturas_table"].selected_items()
                         preview_cfdis(s_items)
 
                     case 'clientes_table_double_click':
-                        items = self.window["clientes_table"].metadata
-                        selection = values["clientes_table"]
-                        s_items = [items[i] for i in selection] if selection else items
-
-                        if s_items:
-                            client = s_items[0]
+                        # noinspection PyUnresolvedReferences
+                        for client in self.window["clientes_table"].selected_items():
                             url = csf.url(rfc=client["Rfc"], id_cif=client["IdCIF"])
                             os.startfile(url)
 
                     case 'emitidas_table_double_click':
-                        items = self.window["emitidas_table"].metadata
-                        selection = values["emitidas_table"]
-                        s_items = [items[i] for i in selection] if selection else items
-
-                        if s_items:
-                            cfdi = s_items[0]  # type: MyCFDI
-                            os.startfile(
-                                os.path.abspath(cfdi.filename + ".pdf")
-                            )
+                        # noinspection PyUnresolvedReferences
+                        s_items = self.window["emitidas_table"].selected_items()
+                        preview_cfdis(s_items)
 
                     case 'ajustes_table_double_click':
-                        items = self.window["ajustes_table"].metadata
-                        selection = values["ajustes_table"]
-                        s_items = [items[i] for i in selection] if selection else items
-
-                        if s_items:
-                            ajuste = s_items[0]
+                        # noinspection PyUnresolvedReferences
+                        for ajuste in self.window["ajustes_table"].selected_items():
                             os.startfile(
                                 os.path.abspath(ajuste['file_name'])
                             )
 
                     case "facturas_table" | "clientes_table" | "correos_table" | "ajustes_table" | "emitidas_table":
-                        items = self.window[event].metadata
-                        selection = values[event]
+                        # noinspection PyUnresolvedReferences
+                        s_items = self.window[event].selected_items()
                         if event == "emitidas_table":
-                            if selection:
-                                self.set_selected_satcfdi(
-                                    items[selection[0]]
-                                )
-                            else:
-                                self.set_selected_satcfdi([])
+                            self.set_selected_satcfdis(s_items)
                         else:
-                            s_items = [items[i] for i in selection] if selection else items
                             self.action_button_manager.set_items(event.split("_")[0], s_items)
 
+                    case "facturas_table+select_all" | "clientes_table+select_all" | "correos_table+select_all" | "ajustes_table+select_all" | "emitidas_table+select_all":
+                        # noinspection PyUnresolvedReferences
+                        self.window[event.split("+")[0]].select_all()
+
                     case "prepare_pago" | "importe_pago_enter" | "fecha_pago_enter" | "forma_pago_enter" | "ver_html_pago":
                         if i := self.selected_satcfdi:
                             fecha_pago = parse_fecha_pago(values["fecha_pago"])
-                            importe_pago = parse_importe_pago(values["importe_pago"])
-                            importe_pago = importe_pago or i.saldo_pendiente
+                            importe_pago = parse_importe_pago(values["importe_pago"]) or i.saldo_pendiente
                             self.window["importe_pago"].update(importe_pago)
 
                             cfdi = pago_factura(
                                 factura_pagar=i,
                                 fecha_pago=fecha_pago,
                                 forma_pago=values["forma_pago"],
                                 importe_pago=importe_pago,
@@ -696,30 +650,30 @@
                             self.action_button_manager.set_items('facturas', [cfdi])
                             if event == "ver_html_pago":
                                 preview_cfdis([cfdi])
 
                     case "status_sat":
                         if i := self.selected_satcfdi:
                             self.local_db.status_sat(i, update=True)
-                            self.set_selected_satcfdi(i)
+                            self.set_selected_satcfdis([i])
 
                     case "pendiente_pago":
                         if i := self.selected_satcfdi:
                             self.local_db.liquidated_flip(i)
-                            self.set_selected_satcfdi(i)
+                            self.set_selected_satcfdis([i])
 
                     case "email_notificada":
                         if i := self.selected_satcfdi:
                             self.local_db.notified_flip(i)
-                            self.set_selected_satcfdi(i)
+                            self.set_selected_satcfdis([i])
 
                     case "crear_facturas":
                         action_text = self.action_button_manager.text()
                         res = PySimpleGUI.popup(
-                            f"{action_text}?",
+                            f"Estas seguro que quieres '{action_text}'?",
                             title="Confirmar",
                             button_type=POPUP_BUTTONS_OK_CANCEL,
                         )
                         if res == "OK":
                             self.header(action_text.upper())
                             self.window['console_tab'].select()
                             self._read()
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/file_data_managers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import collections.abc
 import json
 import logging
 import os
+import re
 from decimal import Decimal
 
 import jsonschema as jsonschema
 import yaml
 from satcfdi import Code, DatePeriod
 from satcfdi.pacs import sat
 # noinspection PyUnresolvedReferences
@@ -19,15 +20,15 @@
 
 REGIMEN_FISCAL = CATALOGS['{http://www.sat.gob.mx/sitio_internet/cfd/catalogos}c_RegimenFiscal']
 
 logger = logging.getLogger(__name__)
 sat_manager = sat.SAT()
 
 
-class DuplicateKeySafeLoader(yaml.CSafeLoader):
+class DuplicateKeySafeLoader(SafeLoader):
     def construct_mapping(self, node, deep=False):
         if isinstance(node, MappingNode):
             self.flatten_mapping(node)
 
         if not isinstance(node, MappingNode):
             raise ConstructorError(None, None,
                                    "expected a mapping node, but found %s" % node.id,
@@ -42,14 +43,25 @@
             if key in mapping:
                 raise ConstructorError("while constructing a mapping", node.start_mark,
                                        "found duplicate key (%s)" % key, key_node.start_mark)
             mapping[key] = value
         return mapping
 
 
+decimal_regex = re.compile(r'[-+]?[0-9_]*\.[0-9_]*', re.X)
+for ch in '-+0123456789.':
+    DuplicateKeySafeLoader.yaml_implicit_resolvers[ch].insert(
+        0,
+        (
+            '!decimal',
+            decimal_regex
+        )
+    )
+
+
 def load_validator(schema_file):
     with open(os.path.join(SOURCE_DIRECTORY, 'schemas', schema_file), "r", encoding="utf-8") as fs:
         schema = yaml.load(fs, SafeLoader)
         validator = jsonschema.validators.validator_for(schema)
         validator.check_schema(schema)
         return validator(schema)
 
@@ -69,14 +81,24 @@
         super().__init__(self._raw())
 
     def _raw(self):
         with open(self.file_source, "r", encoding="utf-8") as fs:
             return yaml.load(fs, DuplicateKeySafeLoader)
 
 
+class InitManager(LocalData):
+    file_source = "init.yaml"
+
+    def __init__(self):
+        try:
+            super().__init__()
+        except FileNotFoundError:
+            pass
+
+
 class ConfigManager(LocalData):
     file_source = "config.yaml"
 
     def __init__(self):
         super().__init__()
         if error := jsonschema.exceptions.best_match(config_validator.iter_errors(self)):
             raise error
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/gui_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from weasyprint import HTML, CSS
 from xlsxwriter.exceptions import FileCreateError
 
 from . import SOURCE_DIRECTORY, ARCHIVOS_DIRECTORY, TEMP_DIRECTORY
 from .environments import facturacion_environment
+from .formatting_functions.common import fecha_mes
 from .utils import add_month
 
 logger = logging.getLogger(__name__)
 logger.level = logging.INFO
 
 sat_manager = sat.SAT()
 
@@ -120,15 +121,15 @@
             print(f"{factura_details['Receptor']}: FormaPago '{factura_details['FormaPago']}' is invalid, expected '99' for PPD")
             is_valid = False
 
     return is_valid
 
 
 def period_desc(dp: DatePeriod):
-    return format_date(date(year=dp.year, month=dp.month, day=1), locale='es_MX', format="'Mes de' MMMM 'del' y").upper()
+    return fecha_mes(date(year=dp.year, month=dp.month, day=1))
 
 
 def periodicidad_desc(dp: DatePeriod, periodo_mes_ajuste, offset):
     periodo_meses, mes_ajuste = parse_periodo_mes_ajuste(periodo_mes_ajuste)
 
     if (dp.month - mes_ajuste) % periodo_meses == 0:
         if offset:
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-3.0.3/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/layout.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/layout.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import date, datetime
 
 import PySimpleGUI as sg
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
+from satdigitalinvoice.gui_functions import mf_pago_fmt
 
 from .log_tools import *
 
 FORMA_PAGO = CATALOGS['{http://www.sat.gob.mx/sitio_internet/cfd/catalogos}c_FormaPago']
 TEXT_PADDING = ((5, 0), 3)
 
 # 24 x 24
@@ -56,15 +57,64 @@
 EDIT_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAAA10lEQVR4nO3UPUpDQRSG4cfCQgn" \
             "+LSPLSCcEC1u3EXdgEXdg3EC2IXYS0N4itZWWGkGvDHyBkE45Npq3usyB95tz5s6w4ZfZwwQveMIFtqvkB5jhDZe4xmdCyuQdxivrk3RSIl/gAe84Ta118oytCvkQPdwmZJxxXVXJl/TSSZd6O/hvs4+7yE" \
             "/Wasd4xT2ONvIl/3gsuys3dLRWGyZ0ll/2RwwiX2SnZ5XyxnkerD5uEjKqkjemmOe7H3FXJW885rGaR9xVyg/xkZBpxjXIwZewU7VTf4ovf6VSMafchm4AAAAASUVORK5CYII="
 
 BUTTON_COLOR = (sg.theme_background_color(), sg.theme_background_color())
 
 
-def make_layout(has_fiel):
+class MyTable(sg.Table):
+    def __init__(self, key, headings, row_fn):
+        super().__init__(
+            values=[],
+            key=key,
+            headings=headings,
+            expand_x=True,
+            expand_y=True,
+            select_mode=sg.TABLE_SELECT_MODE_EXTENDED,
+            enable_events=True,
+            text_color="black",
+            background_color="white",
+            # headings=HEADINGS,
+            # values=[],
+            # auto_size_columns=False,
+            # col_widths=COL_WIDTHS,
+            # justification="center",
+            # num_rows=20,
+            alternating_row_color="grey95", #"aliceblue",
+            # row_height=ROW_HEIGHT,
+            # header_text_color="white",
+            # header_background_color="darkblue",
+            # font=FONT,
+            # bind_return_key=True,
+            tooltip="Doble click para ver factura",
+            # right_click_menu=RIGHT_CLICK_MENU
+            metadata=[]
+        )
+        self.row_fn = row_fn
+
+    def selected_items(self):
+        return [self.metadata[i] for i in self.SelectedRows]
+
+    def select_all(self):
+        self.update(
+            select_rows=list(range(len(self.metadata)))
+        )
+
+    def update(self, values=None, **kwargs):
+        super().update(
+            values=[
+                self.row_fn(i, item)
+                for i, item in enumerate(values, start=1)
+            ],
+            **kwargs
+        )
+        self.metadata = values
+
+
+def make_layout(has_fiel, local_db):
     # LAYOUT
     button_column = [
         sg.Button(image_data=CONFIG_ICON, key="ver_config", border_width=0, button_color=BUTTON_COLOR),
         sg.Text("Periodo:", pad=TEXT_PADDING),
         sg.Input(date.today().strftime('%Y-%m'), size=(11, 1), key="periodo"),
         sg.Button(image_data=FOLDER_ICON, key="ver_carpeta", border_width=0, button_color=BUTTON_COLOR),
         sg.Button(image_data=EXCEL_ICON, key="ver_excel", border_width=0, button_color=BUTTON_COLOR),
@@ -106,64 +156,64 @@
                         [
                             [
                                 sg.Button("Refrescar", key="refresh_clientes", border_width=0),
                                 sg.Push(),
                                 sg.Button(image_data=EDIT_ICON, key="editar_clientes", border_width=0, button_color=BUTTON_COLOR),
                             ],
                             [
-                                sg.Table(
-                                    values=[],
+                                MyTable(
+                                    key="clientes_table",
                                     headings=[
                                         "#",
                                         "Razon Social",
                                         "Rfc",
                                         "Reg",
-                                        "CP",
-                                        "Facturas",
+                                        "CP"
                                     ],
-                                    key="clientes_table",
-                                    expand_x=True,
-                                    expand_y=True,
-                                    select_mode=sg.TABLE_SELECT_MODE_EXTENDED,
-                                    enable_events=True,
-                                    text_color="black",
-                                    background_color="white",
-                                    def_col_width=10,
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r["RazonSocial"],
+                                        r["Rfc"],
+                                        r["RegimenFiscal"].code,
+                                        r["CodigoPostal"]
+                                    ]
                                 )
                             ]],
                         key='clients_tab',
                     ),
                     sg.Tab(
                         'Facturas'.center(13),
                         [
                             [
                                 sg.Button("Refrescar", key="refresh_facturas", border_width=0, ),
                                 sg.Text("", pad=TEXT_PADDING, key="preparar_facturas_text"),
                                 sg.Push(),
                                 sg.Button(image_data=EDIT_ICON, key="editar_facturas", border_width=0, button_color=BUTTON_COLOR),
                             ],
                             [
-                                sg.Table(
-                                    values=[],
+                                MyTable(
+                                    key="facturas_table",
                                     headings=[
                                         '#',
                                         'EReg',
                                         'Receptor Razon Social',
                                         'Recep. Rfc',
                                         "Tipo",
                                         "Subtotal",
                                         "Total"
                                     ],
-                                    key="facturas_table",
-                                    expand_x=True,
-                                    expand_y=True,
-                                    select_mode=sg.TABLE_SELECT_MODE_EXTENDED,
-                                    enable_events=True,
-                                    text_color="black",
-                                    background_color="white",
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r['Emisor']['RegimenFiscal'].code,
+                                        r['Receptor']['Nombre'],
+                                        r['Receptor']['Rfc'],
+                                        mf_pago_fmt(r),
+                                        r['SubTotal'],
+                                        r['Total']
+                                    ]
                                 )
                             ]],
                         key='facturas_tab',
                     ),
                     sg.Tab(
                         'Emitidas'.center(13),
                         [
@@ -190,96 +240,99 @@
                                     sg.Text("ImpPagado:", pad=TEXT_PADDING, key="imp_pagado_text", border_width=0),
                                     sg.Input("", size=(12, 1), key="importe_pago", border_width=0),
                                     sg.Button("Comprobante Pago", key="prepare_pago", border_width=0),
                                     sg.Button(image_data=PREVIEW_ICON, key="ver_html_pago", border_width=0, button_color=BUTTON_COLOR),
                                 ]], visible=False, key="ppd_action_items"),
                             ],
                             [
-                                sg.Table(
-                                    values=[],
+                                MyTable(
+                                    key="emitidas_table",
                                     headings=[
                                         '#',
                                         'Receptor Razon Social',
                                         'Recep. Rfc',
                                         'Factura',
                                         "Fecha",
                                         "Total",
                                         "Pagada",
                                         "Tipo",
                                     ],
-                                    key="emitidas_table",
-                                    expand_x=True,
-                                    expand_y=True,
-                                    select_mode=sg.TABLE_SELECT_MODE_BROWSE,
-                                    enable_events=True,
-                                    text_color="black",
-                                    background_color="white",
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r['Receptor'].get('Nombre', ''),
+                                        r['Receptor']['Rfc'],
+                                        r.name,
+                                        r["Fecha"].strftime("%Y-%m-%d"),
+                                        r["Total"],
+                                        local_db.liquidated_state(r),
+                                        mf_pago_fmt(r)
+                                    ]
                                 )
                             ]],
                         key='emitidas_tab',
-
                     ),
                     sg.Tab(
                         'Correos'.center(13),
                         [
                             [
                                 sg.Button("Refrescar", key="refresh_correos", border_width=0, ),
                             ],
                             [
-                                sg.Table(
-                                    values=[],
+                                MyTable(
+                                    key="correos_table",
                                     headings=[
                                         '#',
                                         'Receptor Razon Social',
                                         'Recep. Rfc',
                                         'Facturas',
                                         'Pendientes Emitidas Meses Anteriores'
                                     ],
-                                    key="correos_table",
-                                    expand_x=True,
-                                    expand_y=True,
-                                    select_mode=sg.TABLE_SELECT_MODE_EXTENDED,
-                                    enable_events=True,
-                                    text_color="black",
-                                    background_color="white",
-                                    def_col_width=10,
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r[0]["RazonSocial"][0:36],
+                                        r[0]["Rfc"],
+                                        ",".join(n.name for n in r[1]),
+                                        ",".join(n.name for n in r[2])
+                                    ]
                                 )
                             ]],
                         key='correos_tab',
                     ),
                     sg.Tab(
                         'Ajustes'.center(13),
                         [
                             [
                                 sg.Button("Refrescar", key="refresh_ajustes", border_width=0, ),
                                 sg.Text("", pad=TEXT_PADDING, key="preparar_ajustes_text"),
                             ],
                             [
-                                sg.Table(
-                                    values=[],
+                                MyTable(
+                                    key="ajustes_table",
                                     headings=[
                                         "#",
                                         "Receptor Razon Social",
                                         "Recep. Rfc",
                                         "Actual",
                                         "Nuevo",
                                         "Ajuste %",
                                         "Periodo",
-                                        "Ajuste Periodo",
+                                        "Meses",
                                         "Ajuste Efectivo"
                                     ],
-                                    key="ajustes_table",
-                                    expand_x=True,
-                                    expand_y=True,
-                                    right_click_selects=True,
-                                    select_mode=sg.TABLE_SELECT_MODE_EXTENDED,
-                                    enable_events=True,
-                                    text_color="black",
-                                    background_color="white",
-                                    def_col_width=10,
+                                    row_fn=lambda i, r: [
+                                        i,
+                                        r["receptor"]["RazonSocial"],
+                                        r["receptor"]["Rfc"],
+                                        r["valor_unitario"],
+                                        r["valor_unitario_nuevo"],
+                                        r["ajuste_porcentaje"],
+                                        r["periodo"],
+                                        r["meses"],
+                                        r["efectivo_periodo_desc"]
+                                    ]
                                 )
                             ]],
                         key='ajustes_tab'
                     ),
                     sg.Tab(
                         'Recuperar'.center(13),
                         [
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/localdb.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-3.0.3/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-3.0.3/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice/utils.py` & `satdigitalinvoice-3.0.3/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.2
+Version: 3.0.3
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.2/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-3.0.3/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 satdigitalinvoice/formatting_functions/common.py
 satdigitalinvoice/images/logo.png
 satdigitalinvoice/markdown_styles/markdown6.css
 satdigitalinvoice/schemas/cliente.yaml
 satdigitalinvoice/schemas/config.yaml
 satdigitalinvoice/schemas/factura.yaml
 tests/test_clients.py
+tests/test_common.py
 tests/test_crear_facturas.py
 tests/test_localdb.py
 tests/test_main.py
```

### Comparing `satdigitalinvoice-3.0.2/setup.py` & `satdigitalinvoice-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/tests/test_crear_facturas.py` & `satdigitalinvoice-3.0.3/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/tests/test_localdb.py` & `satdigitalinvoice-3.0.3/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.2/tests/test_main.py` & `satdigitalinvoice-3.0.3/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def test_layout_unique_keys():
     try:
         import _tkinter
     except ImportError:
         return
 
-    layout = make_layout(has_fiel=True)
+    layout = make_layout(has_fiel=True, local_db=None)
 
     def elements(layout):
         for e in layout:
             if isinstance(e, list):
                 yield from elements(e)
             else:
                 yield e
```

