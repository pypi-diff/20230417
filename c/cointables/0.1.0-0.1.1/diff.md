# Comparing `tmp/cointables-0.1.0.tar.gz` & `tmp/cointables-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cointables-0.1.0.tar", max compression
+gzip compressed data, was "cointables-0.1.1.tar", max compression
```

## Comparing `cointables-0.1.0.tar` & `cointables-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2023-04-16 05:54:06.882290 cointables-0.1.0/LICENSE
--rw-r--r--   0        0        0      862 2023-04-16 07:26:03.560087 cointables-0.1.0/README.md
--rw-r--r--   0        0        0       29 2023-04-16 06:13:34.050997 cointables-0.1.0/cointables/__init__.py
--rw-r--r--   0        0        0     8310 2023-04-16 07:24:17.483851 cointables-0.1.0/cointables/main.py
--rw-r--r--   0        0        0      325 2023-04-16 07:24:28.887875 cointables-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 cointables-0.1.0/setup.py
--rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 cointables-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-16 05:54:06.882290 cointables-0.1.1/LICENSE
+-rw-r--r--   0        0        0      862 2023-04-16 17:41:58.241167 cointables-0.1.1/README.md
+-rw-r--r--   0        0        0       29 2023-04-16 06:13:34.050997 cointables-0.1.1/cointables/__init__.py
+-rw-r--r--   0        0        0     8544 2023-04-16 17:39:27.618964 cointables-0.1.1/cointables/main.py
+-rw-r--r--   0        0        0      325 2023-04-16 17:57:00.866267 cointables-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 cointables-0.1.1/setup.py
+-rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 cointables-0.1.1/PKG-INFO
```

### Comparing `cointables-0.1.0/LICENSE` & `cointables-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cointables-0.1.0/README.md` & `cointables-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cointables-0.1.0/cointables/main.py` & `cointables-0.1.1/cointables/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,31 @@
         coin : str
             Ticker name of quote currency (default: 'BTC')
         market : str
             Ticker name of base currency (default: 'USDT')
         candles : str
             Time interval for candles (default: '30m')
             Valid intervals are: '1m', '3m', '5m', '15m', '30m', '1h', '2h', '4h', '6h', '8h', '12h', '1d', '3d', '1w', '1M'
+
+        Attributes
+        ----------------
         dataframe : <pandas.DataFrame object>
-            Financial data of price activity loaded from above information
+            A DataFrame object containing the financial data of price activity loaded from above information.
         message : str
-            Any message from an external function to store on Chart class (for easy migration across modules)
+            Any message from an external function to store on Chart class (for easy migration across modules).
+        sampled_epoch : int or None
+            The epoch timestamp (either randomly sampled or set by user) see: `get_data_random` method. 
         """
         self.client = client        # client binance object API key api secret
         self.coin = coin
         self.market = market
         self.candles = candles
-        self.dataframe = []
+        self.dataframe = pd.DataFrame()
         self.message = ''
+        self.sampled_epoch = None
 
     def get_data(self, time_diff=2419200000, num_candles=500):
         """
         Retrieve historical market data from the Binance API and return it as a Pandas DataFrame object.
 
         Parameters
         ---------------------------
@@ -100,17 +106,15 @@
         self.dataframe = df
 
         return df
         
 
     def coinGET_custom(self,GET_METHOD):
         """
-        Returns OHLC data of the quote cryptocurrency with the base currency (i.e., 'market') for custom GET_METHOD.
-        
-        Note: The base currency for alts must be either USDT or BTC.
+        Returns OHLC data of the quote cryptocurrency with the base currency (i.e., 'market') for custom GET_METHOD. Note: The base currency for alts must be either USDT or BTC.
         
         Parameters
         -------------------
         GET_METHOD: method or function
             A custom GET_METHOD that returns the OHLC data for a specific cryptocurrency market.
             
             Example:
@@ -149,17 +153,15 @@
         # Save the OHLC data as a dataframe and return it
         self.dataframe = df
         return df
 
 
     def coinGET(self,time_diff=2419200000, num_candles=500):
         """
-        Returns OHLC data of the quote cryptocurrency with the base currency (i.e., 'market').
-        
-        Note: The base currency for alts must be either USDT or BTC.
+        Returns OHLC data of the quote cryptocurrency with the base currency (i.e., 'market'). Note: The base currency for alts must be either USDT or BTC.
         
         Parameters
         -------------------
         time_diff : int, optional
             An integer representing the time difference in seconds between the current time and the starting time of the historical data to retrieve. The default value is 2419200 seconds, which is equivalent to 28 days.
         num_candles : int, optional
             An integer representing the number of historical candles to retrieve. The default value is 500. If this parameter is provided, it takes priority over the `time_diff` parameter.
```

### Comparing `cointables-0.1.0/setup.py` & `cointables-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['datetime>=5.1,<6.0', 'numpy>=1.24.2,<2.0.0', 'pandas>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'cointables',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# cointables\n\nCointables is a Python package that provides a simple and convenient framework to extract historical Open-High-Low-Close (OHLC) data for various cryptocurrencies from Binance. Cointables supports different sampling methods and GET approaches, allowing users to customize their data extraction process. This is a fork from `andrewrgarcia/bitcharts`\n\n\n## Installation\n\nCointables can be installed using pip:\n\n```\npip install cointables\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```\nvirtualenv venv\nsource venv/bin/activate\npip install cointables\n```\n\nTo exit the virtual environment, simply type deactivate. To access it at any other time again, enter with the above source `venv...` command.',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cointables-0.1.0/PKG-INFO` & `cointables-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cointables
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

