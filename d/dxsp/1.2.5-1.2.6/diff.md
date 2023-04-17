# Comparing `tmp/dxsp-1.2.5.tar.gz` & `tmp/dxsp-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.2.5.tar", max compression
+gzip compressed data, was "dxsp-1.2.6.tar", max compression
```

## Comparing `dxsp-1.2.5.tar` & `dxsp-1.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-17 14:44:22.605823 dxsp-1.2.5/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-17 14:44:22.605823 dxsp-1.2.5/README.md
--rw-r--r--   0        0        0      136 2023-04-17 14:44:23.249821 dxsp-1.2.5/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-17 14:44:22.605823 dxsp-1.2.5/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-17 14:44:22.605823 dxsp-1.2.5/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    27976 2023-04-17 14:44:22.605823 dxsp-1.2.5/dxsp/main.py
--rw-r--r--   0        0        0      960 2023-04-17 14:44:23.249821 dxsp-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 15:31:59.195254 dxsp-1.2.6/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-17 15:31:59.195254 dxsp-1.2.6/README.md
+-rw-r--r--   0        0        0      136 2023-04-17 15:31:59.923259 dxsp-1.2.6/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-17 15:31:59.199254 dxsp-1.2.6/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-17 15:31:59.199254 dxsp-1.2.6/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    27986 2023-04-17 15:31:59.199254 dxsp-1.2.6/dxsp/main.py
+-rw-r--r--   0        0        0      960 2023-04-17 15:31:59.923259 dxsp-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.6/PKG-INFO
```

### Comparing `dxsp-1.2.5/LICENSE` & `dxsp-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.5/README.md` & `dxsp-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.5/dxsp/assets/blockchains.py` & `dxsp-1.2.6/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.5/dxsp/main.py` & `dxsp-1.2.6/dxsp/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.w3 = w3
         if self.w3 is None:
             self.w3 = Web3(Web3.HTTPProvider(self.rpc))
             try:
                 self.w3.net.listening
                 self.logger.info(msg=f"connected to {self.rpc} with w3 {self.w3}")
             except Exception as e:
-                logger.error(msg=f"connectivity failed using {rpc}")
+                self.logger.error(msg=f"connectivity failed using {self.rpc}")
                 return
         self.logger.debug(f"self.w3 {self.w3}")
         self.logger.info(msg=f"connected")
 
         self.protocol_type = protocol_type
         if self.protocol_type is None:
             if self.protocol_type == "0x":
```

### Comparing `dxsp-1.2.5/pyproject.toml` & `dxsp-1.2.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.2.5"
+version = "1.2.6"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.2.5/PKG-INFO` & `dxsp-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.2.5
+Version: 1.2.6
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

