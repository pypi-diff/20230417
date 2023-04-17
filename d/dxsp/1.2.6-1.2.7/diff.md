# Comparing `tmp/dxsp-1.2.6.tar.gz` & `tmp/dxsp-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.2.6.tar", max compression
+gzip compressed data, was "dxsp-1.2.7.tar", max compression
```

## Comparing `dxsp-1.2.6.tar` & `dxsp-1.2.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-17 15:31:59.195254 dxsp-1.2.6/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-17 15:31:59.195254 dxsp-1.2.6/README.md
--rw-r--r--   0        0        0      136 2023-04-17 15:31:59.923259 dxsp-1.2.6/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-17 15:31:59.199254 dxsp-1.2.6/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-17 15:31:59.199254 dxsp-1.2.6/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    27986 2023-04-17 15:31:59.199254 dxsp-1.2.6/dxsp/main.py
--rw-r--r--   0        0        0      960 2023-04-17 15:31:59.923259 dxsp-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 15:39:23.100213 dxsp-1.2.7/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-17 15:39:23.100213 dxsp-1.2.7/README.md
+-rw-r--r--   0        0        0      136 2023-04-17 15:39:23.760220 dxsp-1.2.7/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-17 15:39:23.100213 dxsp-1.2.7/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-17 15:39:23.100213 dxsp-1.2.7/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    27987 2023-04-17 15:39:23.100213 dxsp-1.2.7/dxsp/main.py
+-rw-r--r--   0        0        0      960 2023-04-17 15:39:23.760220 dxsp-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.7/PKG-INFO
```

### Comparing `dxsp-1.2.6/LICENSE` & `dxsp-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.6/README.md` & `dxsp-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.6/dxsp/assets/blockchains.py` & `dxsp-1.2.7/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.6/dxsp/main.py` & `dxsp-1.2.7/dxsp/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 or self.dex_exchange != blockchain["uniswap_v3"]
             ):
                 self.router = blockchain["uniswap_v2"]
             else:
                 self.router = blockchain["uniswap_v3"]
         self.logger.debug(f"self.router {self.router}")
 
-        self.logger.debug(f"self.name {self.name}")        
+        #self.logger.debug(f"self.name {self.name}")        
 
         self.base_trading_symbol = base_trading_symbol
         if self.base_trading_symbol is None:
             self.base_trading_symbol= 'USDC'
         self.logger.debug(f"self.base_trading_symbol {self.base_trading_symbol}")
 
         self.amount_trading_option = amount_trading_option
```

### Comparing `dxsp-1.2.6/pyproject.toml` & `dxsp-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.2.6"
+version = "1.2.7"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.2.6/PKG-INFO` & `dxsp-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.2.6
+Version: 1.2.7
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

