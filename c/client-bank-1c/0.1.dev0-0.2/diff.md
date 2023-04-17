# Comparing `tmp/client_bank_1c-0.1.dev0.tar.gz` & `tmp/client_bank_1c-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_bank_1c-0.1.dev0.tar", max compression
+gzip compressed data, was "client_bank_1c-0.2.tar", max compression
```

## Comparing `client_bank_1c-0.1.dev0.tar` & `client_bank_1c-0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.1.dev0/LICENSE
--rw-r--r--   0        0        0     4296 2023-04-15 22:58:47.352673 client_bank_1c-0.1.dev0/client_bank_1c.py
--rw-r--r--   0        0        0      890 2023-04-15 23:14:58.886400 client_bank_1c-0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 client_bank_1c-0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.2/LICENSE
+-rw-r--r--   0        0        0     4355 2023-04-17 12:26:54.666496 client_bank_1c-0.2/client_bank_1c.py
+-rw-r--r--   0        0        0      886 2023-04-17 12:34:45.188023 client_bank_1c-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 client_bank_1c-0.2/PKG-INFO
```

### Comparing `client_bank_1c-0.1.dev0/LICENSE` & `client_bank_1c-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `client_bank_1c-0.1.dev0/client_bank_1c.py` & `client_bank_1c-0.2/client_bank_1c.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
             'РасчСчет': [],
             'Документ': [],
         }
         documents = []
         accounts = []
         section = 'info'
         for line in stream:
+            if not line.strip():
+                continue
+
             key, value = self._parse_line(line)
 
             if key == 'СекцияРасчСчет':
                 assert section == 'info'
                 section = key
                 section_values = {}
```

### Comparing `client_bank_1c-0.1.dev0/pyproject.toml` & `client_bank_1c-0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "client-bank-1c"
-version = "0.1-dev"
+version = "0.2"
 description = "1C Client Bank Exchange Format"
 authors = ["Dmitry Voronin <dimka665@gmail.com>"]
 
 repository = "https://github.com/odoo-ru/client-bank-1c"
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `client_bank_1c-0.1.dev0/PKG-INFO` & `client_bank_1c-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: client-bank-1c
-Version: 0.1.dev0
+Version: 0.2
 Summary: 1C Client Bank Exchange Format
 Home-page: https://github.com/odoo-ru/client-bank-1c
 License: MIT
 Author: Dmitry Voronin
 Author-email: dimka665@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Intended Audience :: Developers
```

