# Comparing `tmp/atmoswing-vigicrues-0.9.2.tar.gz` & `tmp/atmoswing-vigicrues-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-0.9.2.tar", last modified: Fri Dec 16 19:25:01 2022, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.0.0.tar", last modified: Mon Apr 17 10:05:39 2023, max compression
```

## Comparing `atmoswing-vigicrues-0.9.2.tar` & `atmoswing-vigicrues-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:25:01.907522 atmoswing-vigicrues-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-16 19:25:01.907522 atmoswing-vigicrues-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      376 2022-12-16 19:25:01.911522 atmoswing-vigicrues-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:25:01.903522 atmoswing-vigicrues-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:25:01.907522 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:25:01.907522 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/disseminations/transfer_sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:25:01.907522 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:25:01.907522 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2022-12-16 19:24:44.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:25:01.907522 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-16 19:25:01.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-16 19:25:01.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 19:25:01.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-16 19:25:01.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-16 19:25:01.000000 atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.674262 atmoswing-vigicrues-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.674262 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.682263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.682263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.682263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.678263 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 10:05:39.000000 atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:05:39.686263 atmoswing-vigicrues-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-17 10:05:14.000000 atmoswing-vigicrues-1.0.0/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-0.9.2/LICENSE` & `atmoswing-vigicrues-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/pyproject.toml` & `atmoswing-vigicrues-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "0.9.2"
+version = "1.0.0"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,21 +16,22 @@
     has_eccodes = True
 
 from .controller import Controller
 from .options import Options
 from .exceptions import (ConfigError, Error, FilePathError, OptionError,
                          PathError)
 from .preactions.download_gfs import DownloadGfsData
+from .preactions.transfer_sftp_in import TransferSftpIn
 from .preactions.transform_gfs import TransformGfsData
 from .preactions.transform_ecmwf import TransformEcmwfData
 from .postactions.export_bdapbp import ExportBdApBp
 from .postactions.export_prv import ExportPrv
-from .disseminations.transfer_sftp import TransferSftp
+from .disseminations.transfer_sftp_out import TransferSftpOut
 from .utils import file_exists, check_dir_exists, check_file_exists, \
     build_date_dir_structure
 
 
 __all__ = ('Error', 'OptionError', 'ConfigError', 'PathError', 'FilePathError',
-           'Controller', 'Options', 'ExportBdApBp', 'ExportPrv', 'TransferSftp',
+           'Controller', 'Options', 'ExportBdApBp', 'ExportPrv', 'TransferSftpOut',
            'DownloadGfsData', 'TransformGfsData', 'TransformEcmwfData', 'file_exists',
            'check_file_exists', 'check_dir_exists', 'build_date_dir_structure',
-           'Dataset', 'eccodes')
+           'Dataset', 'eccodes', 'TransferSftpIn')
```

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import argparse
+from datetime import datetime
 
 from atmoswing_vigicrues.controller import Controller
 
 
 def main() -> int:
     parser = argparse.ArgumentParser(
         description="Traite les prévisions et les exportations d'AtmoSwing pour "
                     "le réseau Vigicrues.")
     parser.add_argument(
         '--config-file', type=str, required=False,
-        help="fichier de configuration du présent module.")
+        help="Fichier de configuration du présent module.")
+    parser.add_argument(
+        '--date', type=str, required=False,
+        help="Date pour laquelle émettre une prévision (YYYYMMDDHH).")
 
     args = parser.parse_args()
 
     controller = Controller(args)
 
+    if args.date:
+        date = datetime.strptime(args.date, '%Y%m%d%H')
+        return controller.run(date)
+
     return controller.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         ----------
         cli_options : object
             Options passées en lignes de commandes à la fonction main()
         """
         self.options = asv.Options(cli_options)
         self.verbose = True
         self.max_attempts = 8
-        self.time_increment = 24
+        self.time_increment = 6
         self.date = datetime.datetime.utcnow()
         self.pre_actions = []
         self.post_actions = []
         self.disseminations = []
         self._register_pre_actions()
         self._register_post_actions()
         self._register_disseminations()
```

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/disseminations/transfer_sftp.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import paramiko, socks
 
 import atmoswing_vigicrues as asv
 
 from .dissemination import Dissemination
 
 
-class TransferSftp(Dissemination):
+class TransferSftpOut(Dissemination):
     """
     Transfer des résultats par SFTP.
 
     Parameters
     ----------
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
@@ -112,13 +112,14 @@
         except paramiko.ssh_exception.SSHException as e:
             print(f"SFTP SSHException {e}")
         except FileNotFoundError as e:
             print(f"SFTP FileNotFoundError {e}")
         except Exception as e:
             print(f"La diffusion SFTP a échoué ({e}).")
 
-    def _chdir_or_mkdir(self, dir, sftp):
+    @staticmethod
+    def _chdir_or_mkdir(dir_path, sftp):
         try:
-            sftp.chdir(dir)
+            sftp.chdir(dir_path)
         except IOError:
-            sftp.mkdir(dir)
-            sftp.chdir(dir)
+            sftp.mkdir(dir_path)
+            sftp.chdir(dir_path)
```

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-0.9.2/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.0.0/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

