# Comparing `tmp/sgex-0.6.2.tar.gz` & `tmp/sgex-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgex-0.6.2.tar", last modified: Wed Mar  1 16:50:51 2023, max compression
+gzip compressed data, was "sgex-0.6.3.tar", last modified: Mon Apr 17 11:41:22 2023, max compression
```

## Comparing `sgex-0.6.2.tar` & `sgex-0.6.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-01 16:50:51.654697 sgex-0.6.2/
--rw-r--r--   0 user      (1000) user      (1000)     1520 2022-01-17 07:52:33.000000 sgex-0.6.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    25389 2023-03-01 16:50:51.654697 sgex-0.6.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    22622 2023-03-01 16:33:51.000000 sgex-0.6.2/README.md
--rw-r--r--   0 user      (1000) user      (1000)     1365 2023-03-01 16:50:21.000000 sgex-0.6.2/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-03-01 16:50:51.654697 sgex-0.6.2/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-01 16:50:51.650697 sgex-0.6.2/sgex/
--rw-r--r--   0 user      (1000) user      (1000)      448 2023-03-01 16:50:21.000000 sgex-0.6.2/sgex/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    23488 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/_call.py
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-03-01 16:50:21.000000 sgex-0.6.2/sgex/_version.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-01 16:50:51.653697 sgex-0.6.2/sgex/call/
--rw-r--r--   0 user      (1000) user      (1000)       99 2023-03-01 16:50:21.000000 sgex-0.6.2/sgex/call/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3893 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/call/call.py
--rw-r--r--   0 user      (1000) user      (1000)     1591 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/call/hook.py
--rw-r--r--   0 user      (1000) user      (1000)     6346 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/call/job.py
--rw-r--r--   0 user      (1000) user      (1000)     4517 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/call/package.py
--rw-r--r--   0 user      (1000) user      (1000)     2515 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/call/query.py
--rw-r--r--   0 user      (1000) user      (1000)     3891 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/call/type.py
--rw-r--r--   0 user      (1000) user      (1000)     2427 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/config.py
--rw-r--r--   0 user      (1000) user      (1000)     3901 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/io.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-01 16:50:51.654697 sgex-0.6.2/sgex/parse/
--rw-r--r--   0 user      (1000) user      (1000)       89 2023-03-01 16:50:21.000000 sgex-0.6.2/sgex/parse/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2133 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/parse/corp_info.py
--rw-r--r--   0 user      (1000) user      (1000)     2519 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/parse/freqs.py
--rw-r--r--   0 user      (1000) user      (1000)     1039 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/parse/wordlist.py
--rw-r--r--   0 user      (1000) user      (1000)      874 2023-02-28 16:55:51.000000 sgex-0.6.2/sgex/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-03-01 16:50:51.651697 sgex-0.6.2/sgex.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    25389 2023-03-01 16:50:51.000000 sgex-0.6.2/sgex.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      481 2023-03-01 16:50:51.000000 sgex-0.6.2/sgex.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-03-01 16:50:51.000000 sgex-0.6.2/sgex.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       88 2023-03-01 16:50:51.000000 sgex-0.6.2/sgex.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        5 2023-03-01 16:50:51.000000 sgex-0.6.2/sgex.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 11:41:22.209772 sgex-0.6.3/
+-rw-r--r--   0 user      (1000) user      (1000)     1520 2022-01-17 07:52:33.000000 sgex-0.6.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    25433 2023-04-17 11:41:22.209772 sgex-0.6.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    22666 2023-04-17 11:35:35.000000 sgex-0.6.3/README.md
+-rw-r--r--   0 user      (1000) user      (1000)     1365 2023-04-17 11:35:35.000000 sgex-0.6.3/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-17 11:41:22.209772 sgex-0.6.3/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 11:41:22.205772 sgex-0.6.3/sgex/
+-rw-r--r--   0 user      (1000) user      (1000)      448 2023-03-01 16:50:21.000000 sgex-0.6.3/sgex/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    23488 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/_call.py
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-04-17 11:35:35.000000 sgex-0.6.3/sgex/_version.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 11:41:22.208773 sgex-0.6.3/sgex/call/
+-rw-r--r--   0 user      (1000) user      (1000)       99 2023-03-01 16:50:21.000000 sgex-0.6.3/sgex/call/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3893 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/call/call.py
+-rw-r--r--   0 user      (1000) user      (1000)     1591 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/call/hook.py
+-rw-r--r--   0 user      (1000) user      (1000)     6353 2023-04-17 11:35:35.000000 sgex-0.6.3/sgex/call/job.py
+-rw-r--r--   0 user      (1000) user      (1000)     4703 2023-04-17 11:35:35.000000 sgex-0.6.3/sgex/call/package.py
+-rw-r--r--   0 user      (1000) user      (1000)     3170 2023-04-17 11:35:35.000000 sgex-0.6.3/sgex/call/query.py
+-rw-r--r--   0 user      (1000) user      (1000)     3891 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/call/type.py
+-rw-r--r--   0 user      (1000) user      (1000)     2427 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/config.py
+-rw-r--r--   0 user      (1000) user      (1000)     3901 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/io.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 11:41:22.208773 sgex-0.6.3/sgex/parse/
+-rw-r--r--   0 user      (1000) user      (1000)       89 2023-03-01 16:50:21.000000 sgex-0.6.3/sgex/parse/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2133 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/parse/corp_info.py
+-rw-r--r--   0 user      (1000) user      (1000)     2521 2023-04-17 11:35:35.000000 sgex-0.6.3/sgex/parse/freqs.py
+-rw-r--r--   0 user      (1000) user      (1000)     1039 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/parse/wordlist.py
+-rw-r--r--   0 user      (1000) user      (1000)      874 2023-02-28 16:55:51.000000 sgex-0.6.3/sgex/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 11:41:22.206772 sgex-0.6.3/sgex.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    25433 2023-04-17 11:41:22.000000 sgex-0.6.3/sgex.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      481 2023-04-17 11:41:22.000000 sgex-0.6.3/sgex.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-17 11:41:22.000000 sgex-0.6.3/sgex.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       88 2023-04-17 11:41:22.000000 sgex-0.6.3/sgex.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        5 2023-04-17 11:41:22.000000 sgex-0.6.3/sgex.egg-info/top_level.txt
```

### Comparing `sgex-0.6.2/LICENSE` & `sgex-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/PKG-INFO` & `sgex-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgex
-Version: 0.6.2
+Version: 0.6.3
 Summary: Sketch Grammar Explorer (Sketch Engine API wrapper)
 Author-email: Loryn Isaacs <50170623+engisalor@users.noreply.github.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Loryn Isaacs
         All rights reserved.
         
@@ -98,36 +98,36 @@
 
 Dependencies:
 - required: `pandas pyyaml requests requests-cache`
 - optional: `keyring openpyxl defusedxml`
 
 ## TL;DR
 
-An abbreviated example of SGEX usage.
+An abbreviated example of SGEX for making calls to Sketch Engine.
 
 ```python
 import sgex
 
 # add API credentials to the server configuration
-config = {"ske": {**sgex.config.default["ske"], **{"username": "J. Doe", "api_key": "1234"}}}
+sgex.config.default["ske"] |= {"username": "J. Doe", "api_key": "1234"}
 
 # define API calls
 calls = [
     # the first freqs call is complete (has all the needed parameters)
     sgex.Freqs({
         "format": "csv",
         "q": 'alemma,"eat"',
         "corpname": "preloaded/susanne",
         "fcrit": "doc.file 0",
         }),
     # successive freqs calls will reuse previous parameters
     sgex.Freqs({"q": 'alemma,"sleep"'})]
 
 # package calls
-package = sgex.Package(calls, "ske", config)
+package = sgex.Package(calls, "ske")
 
 # send requests
 package.send_requests()
 
 # access response data
 print(package.responses[0].text)
 "corpus","preloaded/susanne"
@@ -181,17 +181,15 @@
     'wait': {
       '0': 1, # wait 0 seconds for 1 call
       '2': 99, # wait 2 seconds for 2-99 calls
       '5': 899, # wait 5 seconds for 100-899 calls
       '45': None}}} # wait 45 seconds for 900+ calls
 
 # add your API credentials for making calls to the "ske" server
-config = sgex.config.default
-config["ske"]["username"] = "J. Doe"
-config["ske"]["api_key"] = "1234"
+sgex.config.default["ske"] |= {"username": "J. Doe", "api_key": "1234"}
 ```
 
 ### 2. Making a `corp_info` API call
 
 Each type of API call has its own Python class (e.g., `CorpInfo`), which is a child of the generic `Call` class. To make API calls, start by creating `Call` objects.
 
 Calls are added to a `Package` class, which prepares requests and manages their execution. A `Package` can be inspected to make sure everything looks good before sending calls. Packages also expose other settings for more advanced usage.
@@ -204,15 +202,18 @@
 # indicate which server to use
 server = "ske"
 
 # define a call
 call = sgex.CorpInfo({"corpname": "preloaded/susanne"})
 
 # package the call
-package = sgex.Package(call, server, config)
+package = sgex.Package(call, server)
+
+# config dicts can also be passed explicitly
+# package = sgex.Package(call, server, config_dict)
 
 # inspect the package details
 print(package.calls)
 [CORP_INFO(2a8c0b24) {'api_key': '1234', 'username': 'J. Doe', 'corpname': 'preloaded/susanne'}]
 
 print(package.calls[0].request)
 <Request [GET]>
@@ -445,15 +446,15 @@
 Package.server: str  # server to call
 Package.halt: bool   # whether to stop a job on error
 Package.errors: set  # errors encountered
 Package.loglevel: str  # logging level
 Package.max_workers: int  # threads for asynchronous calls
 Package.responses: list  # call responses
 Package.max_responses: int  # max items to store in `Package.responses` (for large jobs)
-Package.session_params: dict(  # parameters for the `request-cache` session
+Package.session_params: dict(  # parameters for the `requests-cache` session
     cache_name="data",
     serializer="json",
     backend="filesystem",
     ignored_parameters=credential_parameters,
     key_fn=call.create_custom_key,
 )
 Package.config: dict  # server configuration
@@ -475,18 +476,18 @@
 These classes combine multiple API calls, parsing methods, etc., to execute larger jobs with a single command.
 
 **Text type analysis**
 
 `TTypeAnalysis` automates the steps for generating a DataFrame describing the corpus's composition.
 
 ```python
-from sgex.call import TTypeAnalysis
+from sgex.call.job import TTypeAnalysis
 
 # prepare the job
-ttypes = TTypeAnalysis("susanne", <server>, <config>)
+ttypes = TTypeAnalysis("susanne", <server>)
 
 # run the job
 ttypes.run()
 
 # view the results
 print(ttypes.df.head(3))
     str  frq  relfreq  attribute
@@ -496,18 +497,18 @@
 ```
 
 **Simple frequency query**
 
 `SimpleFreqsQuery` automates making a `freqs` call with Simple Query syntax and processing JSON data into a DataFrame.
 
 ```python
-from sgex.call import SimpleFreqsQuery
+from sgex.call.job import SimpleFreqsQuery
 
 # prepare the job
-query = SimpleFreqsQuery("sleep", "susanne", "noske", ".config.yml")
+query = SimpleFreqsQuery("sleep", "susanne", "noske")
 
 # run the job
 query.run()
 
 # view the results (each row is a corpus attribute/text type)
 print(query.df.head(3))
    frq         rel        reltt  ...  total_fpm total_size fmaxitems
```

### Comparing `sgex-0.6.2/README.md` & `sgex-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,36 +45,36 @@
 
 Dependencies:
 - required: `pandas pyyaml requests requests-cache`
 - optional: `keyring openpyxl defusedxml`
 
 ## TL;DR
 
-An abbreviated example of SGEX usage.
+An abbreviated example of SGEX for making calls to Sketch Engine.
 
 ```python
 import sgex
 
 # add API credentials to the server configuration
-config = {"ske": {**sgex.config.default["ske"], **{"username": "J. Doe", "api_key": "1234"}}}
+sgex.config.default["ske"] |= {"username": "J. Doe", "api_key": "1234"}
 
 # define API calls
 calls = [
     # the first freqs call is complete (has all the needed parameters)
     sgex.Freqs({
         "format": "csv",
         "q": 'alemma,"eat"',
         "corpname": "preloaded/susanne",
         "fcrit": "doc.file 0",
         }),
     # successive freqs calls will reuse previous parameters
     sgex.Freqs({"q": 'alemma,"sleep"'})]
 
 # package calls
-package = sgex.Package(calls, "ske", config)
+package = sgex.Package(calls, "ske")
 
 # send requests
 package.send_requests()
 
 # access response data
 print(package.responses[0].text)
 "corpus","preloaded/susanne"
@@ -128,17 +128,15 @@
     'wait': {
       '0': 1, # wait 0 seconds for 1 call
       '2': 99, # wait 2 seconds for 2-99 calls
       '5': 899, # wait 5 seconds for 100-899 calls
       '45': None}}} # wait 45 seconds for 900+ calls
 
 # add your API credentials for making calls to the "ske" server
-config = sgex.config.default
-config["ske"]["username"] = "J. Doe"
-config["ske"]["api_key"] = "1234"
+sgex.config.default["ske"] |= {"username": "J. Doe", "api_key": "1234"}
 ```
 
 ### 2. Making a `corp_info` API call
 
 Each type of API call has its own Python class (e.g., `CorpInfo`), which is a child of the generic `Call` class. To make API calls, start by creating `Call` objects.
 
 Calls are added to a `Package` class, which prepares requests and manages their execution. A `Package` can be inspected to make sure everything looks good before sending calls. Packages also expose other settings for more advanced usage.
@@ -151,15 +149,18 @@
 # indicate which server to use
 server = "ske"
 
 # define a call
 call = sgex.CorpInfo({"corpname": "preloaded/susanne"})
 
 # package the call
-package = sgex.Package(call, server, config)
+package = sgex.Package(call, server)
+
+# config dicts can also be passed explicitly
+# package = sgex.Package(call, server, config_dict)
 
 # inspect the package details
 print(package.calls)
 [CORP_INFO(2a8c0b24) {'api_key': '1234', 'username': 'J. Doe', 'corpname': 'preloaded/susanne'}]
 
 print(package.calls[0].request)
 <Request [GET]>
@@ -392,15 +393,15 @@
 Package.server: str  # server to call
 Package.halt: bool   # whether to stop a job on error
 Package.errors: set  # errors encountered
 Package.loglevel: str  # logging level
 Package.max_workers: int  # threads for asynchronous calls
 Package.responses: list  # call responses
 Package.max_responses: int  # max items to store in `Package.responses` (for large jobs)
-Package.session_params: dict(  # parameters for the `request-cache` session
+Package.session_params: dict(  # parameters for the `requests-cache` session
     cache_name="data",
     serializer="json",
     backend="filesystem",
     ignored_parameters=credential_parameters,
     key_fn=call.create_custom_key,
 )
 Package.config: dict  # server configuration
@@ -422,18 +423,18 @@
 These classes combine multiple API calls, parsing methods, etc., to execute larger jobs with a single command.
 
 **Text type analysis**
 
 `TTypeAnalysis` automates the steps for generating a DataFrame describing the corpus's composition.
 
 ```python
-from sgex.call import TTypeAnalysis
+from sgex.call.job import TTypeAnalysis
 
 # prepare the job
-ttypes = TTypeAnalysis("susanne", <server>, <config>)
+ttypes = TTypeAnalysis("susanne", <server>)
 
 # run the job
 ttypes.run()
 
 # view the results
 print(ttypes.df.head(3))
     str  frq  relfreq  attribute
@@ -443,18 +444,18 @@
 ```
 
 **Simple frequency query**
 
 `SimpleFreqsQuery` automates making a `freqs` call with Simple Query syntax and processing JSON data into a DataFrame.
 
 ```python
-from sgex.call import SimpleFreqsQuery
+from sgex.call.job import SimpleFreqsQuery
 
 # prepare the job
-query = SimpleFreqsQuery("sleep", "susanne", "noske", ".config.yml")
+query = SimpleFreqsQuery("sleep", "susanne", "noske")
 
 # run the job
 query.run()
 
 # view the results (each row is a corpus attribute/text type)
 print(query.df.head(3))
    frq         rel        reltt  ...  total_fpm total_size fmaxitems
```

### Comparing `sgex-0.6.2/pyproject.toml` & `sgex-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sgex"
-version = "0.6.2"  # x-release-please-version
+version = "0.6.3"  # x-release-please-version
 requires-python = ">=3.8"
 authors = [{name="Loryn Isaacs", email="50170623+engisalor@users.noreply.github.com"}]
 description = "Sketch Grammar Explorer (Sketch Engine API wrapper)"
 keywords = [
     "sketch engine",
     "api wrapper",
     "corpus linguistics",
```

### Comparing `sgex-0.6.2/sgex/_call.py` & `sgex-0.6.3/sgex/_call.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/call/call.py` & `sgex-0.6.3/sgex/call/call.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/call/hook.py` & `sgex-0.6.3/sgex/call/hook.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/call/job.py` & `sgex-0.6.3/sgex/call/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Classes to execute specific API jobs."""
 import pandas as pd
 
 from sgex.call.package import Package
 from sgex.call.query import simple_query
 from sgex.call.type import CorpInfo, Freqs, Wordlist
+from sgex.config import default
 from sgex.parse import corp_info, freqs, wordlist
 
 
 class TTypeAnalysis:
     """Collects frequency data about a corpus's text types (attributes).
 
     Args:
         corpname: Corpus.
         server: Server.
-        config: Configuration.
+        config: Configuration dict.
 
     Methods:
         get_corp_info: Makes a preliminary corp_info call.
         get_ttypes: Runs Wordlist calls for each attribute.
         make_df: Makes a DataFrame of results.
         run: Executes job.
 
@@ -66,15 +67,15 @@
 
     def run(self):
         """Executes the job."""
         self.get_corp_info()
         self.get_ttypes()
         self.make_df()
 
-    def __init__(self, corpname: str, server: str, config: dict) -> None:
+    def __init__(self, corpname: str, server: str, config: dict = default) -> None:
         self.corpname = corpname
         self.server = server
         self.config = config
         self.corp_info_params = {
             "corpname": corpname,
             "struct_attr_stats": 1,
         }
@@ -98,15 +99,15 @@
 
 class SimpleFreqsQuery:
     """Collects data for a freqs query using simple query syntax.
 
     Args:
         corpname: Corpus.
         server: Server.
-        config: Configuration.
+        config: Configuration dict.
         fcrit: Attributes to query.
         fcrit_limit: Limit attributes to those with fewer than N values.
 
     Methods:
         get_corp_info: Makes a preliminary corp_info call.
         set_fcrit: Determines which attributes to include in ``fcrit``.
         get_freqs: Runs the freqs API call.
@@ -160,24 +161,23 @@
         self.df = freqs.freqs_json(self.package.responses[0])
 
     def __init__(
         self,
         query: str,
         corpname: str,
         server: str,
-        config: dict,
+        config: dict = default,
         fcrit=None,
         fcrit_limit: int = 0,
     ):
         self.query = query
         self.corpname = corpname
         self.server = server
         self.config = config
         self.fcrit_limit = fcrit_limit
-        self.corp_info_params = {"corpname": corpname}
         self.corp_info_params = {
             "corpname": corpname,
             "struct_attr_stats": 1,
         }
         q = simple_query(query)
         self.freqs_params = {
             "q": q,
```

### Comparing `sgex-0.6.2/sgex/call/package.py` & `sgex-0.6.3/sgex/call/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.parse import parse_qs, urlparse
 
 from requests import Response
 from requests_cache import CachedSession
 
 from sgex.call import call, hook
 from sgex.call.type import Call
-from sgex.config import credential_parameters
+from sgex.config import credential_parameters, default
 from sgex.config import load as load_config
 
 
 class Package:
     """Class for organizing and executing API calls."""
 
     def send_requests(self) -> None:
@@ -52,14 +52,17 @@
     def _manage_response(self, response: Response, t0: float) -> None:
         self._add_response_to_instance(response)
         self._handle_errors(response)
 
     def _add_response_to_instance(self, response: Response) -> None:
         if self.max_responses >= len(self.responses):
             self.responses.append(response)
+            if self.max_responses == len(self.responses):
+                m = f"reached max_responses ({self.max_responses})"
+                logging.warning(m)
 
     def _handle_errors(self, response: Response) -> None:
         error = None
         # HTTP errors
         response.raise_for_status()
         # Sketch Engine errors
         # TODO include other formats (CSV, etc.)
@@ -70,15 +73,15 @@
             dt = {k: v for k, v in query.items() if k not in credential_parameters}
             host = response.url.split("?")[0]
             self.errors.add((error, host, str(dt)))
             logging.warning(f"{error} - {host} - {dt}")
         if error and self.halt:
             raise Warning(f"requests halted with error: {error}")
 
-    def __init__(self, calls: list, server: str, config, **kwargs):
+    def __init__(self, calls: list, server: str, config: dict = default, **kwargs):
         if isinstance(calls, Call):
             calls = [calls]
         self.calls = calls
         self.server = server
         self.halt = True
         self.errors = set()
         self.loglevel = "warning"
```

### Comparing `sgex-0.6.2/sgex/call/query.py` & `sgex-0.6.3/sgex/call/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 """Functions for assembling CQL rules from query strings."""
 import re
 
+escape_symbols = {
+    '"': r'\\"',
+    "$": r"\$",
+    "(": r"\(",
+    ")": r"\)",
+    "+": r"\+",
+    "[": r"\[",
+    "]": r"\]",
+    "^": r"\^",
+    "{": r"\{",
+    "}": r"\}",
+    "\\": "\\\\\\\\",
+}
+
 
 def query_to_cql(query: str):
     """Converts a word/phrase into a ``lc`` and ``lemma_lc`` CQL rule."""
     words = [x for x in query.split() if x]
     return " ".join([f'[lc="{w.strip()}" | lemma_lc="{w.strip()}"]' for w in words])
 
 
@@ -57,16 +71,28 @@
                 queries[x][y] = [q[y], if_atomic(q[y], atomic_hyphens)]
             else:
                 queries[x][y] = [q[y]]
             queries[x][y] = [a for a in queries[x][y] if a]
     return queries
 
 
+def query_escape(query: str):
+    """Escapes special CQL characters in a string.
+
+    Note:
+        Single backslashes are converted to four backslashes, which is needed to query
+        this literal character in current CQL behavior. Querying a single backslash in
+        SkE's simple query returns strings in angled brackets, not backslashes.
+    """
+    return "".join([escape_symbols.get(c, c) for c in query])
+
+
 def simple_query(query: str, atomic_hyphens=True):
     """Converts a query string into a CQL rule following SkE ``simple`` behavior."""
+    query = query_escape(query)
     queries = query_to_dict(query, atomic_hyphens)
     dt = queries.copy()
     all = []
     for v in dt.values():
         ls = []
         for c in v.keys():
             v[c] = [query_to_cql(phrase) for phrase in v[c]]
```

### Comparing `sgex-0.6.2/sgex/call/type.py` & `sgex-0.6.3/sgex/call/type.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/config.py` & `sgex-0.6.3/sgex/config.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/io.py` & `sgex-0.6.3/sgex/io.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/parse/corp_info.py` & `sgex-0.6.3/sgex/parse/corp_info.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/parse/freqs.py` & `sgex-0.6.3/sgex/parse/freqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
             del dt["Word"]
             b.append(dt)
         clean.append(b)
     return clean
 
 
 def clean_heads(heads) -> list:
-    """Extracts each block's fcrit attribute: ``head[0]["n"]``."""
+    """Extracts each block's fcrit attribute: ``head[0]["id"]``."""
     if len([x for x in heads if x]):
-        return [head[0].get("n") for head in heads]
+        return [head[0].get("id") for head in heads]
     else:
         return None
 
 
 def freqs_json(response: Response) -> pd.DataFrame:
     """Converts a single-/multi-block freqs JSON response to a DataFrame.
```

### Comparing `sgex-0.6.2/sgex/parse/wordlist.py` & `sgex-0.6.3/sgex/parse/wordlist.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex/util.py` & `sgex-0.6.3/sgex/util.py`

 * *Files identical despite different names*

### Comparing `sgex-0.6.2/sgex.egg-info/PKG-INFO` & `sgex-0.6.3/sgex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgex
-Version: 0.6.2
+Version: 0.6.3
 Summary: Sketch Grammar Explorer (Sketch Engine API wrapper)
 Author-email: Loryn Isaacs <50170623+engisalor@users.noreply.github.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Loryn Isaacs
         All rights reserved.
         
@@ -98,36 +98,36 @@
 
 Dependencies:
 - required: `pandas pyyaml requests requests-cache`
 - optional: `keyring openpyxl defusedxml`
 
 ## TL;DR
 
-An abbreviated example of SGEX usage.
+An abbreviated example of SGEX for making calls to Sketch Engine.
 
 ```python
 import sgex
 
 # add API credentials to the server configuration
-config = {"ske": {**sgex.config.default["ske"], **{"username": "J. Doe", "api_key": "1234"}}}
+sgex.config.default["ske"] |= {"username": "J. Doe", "api_key": "1234"}
 
 # define API calls
 calls = [
     # the first freqs call is complete (has all the needed parameters)
     sgex.Freqs({
         "format": "csv",
         "q": 'alemma,"eat"',
         "corpname": "preloaded/susanne",
         "fcrit": "doc.file 0",
         }),
     # successive freqs calls will reuse previous parameters
     sgex.Freqs({"q": 'alemma,"sleep"'})]
 
 # package calls
-package = sgex.Package(calls, "ske", config)
+package = sgex.Package(calls, "ske")
 
 # send requests
 package.send_requests()
 
 # access response data
 print(package.responses[0].text)
 "corpus","preloaded/susanne"
@@ -181,17 +181,15 @@
     'wait': {
       '0': 1, # wait 0 seconds for 1 call
       '2': 99, # wait 2 seconds for 2-99 calls
       '5': 899, # wait 5 seconds for 100-899 calls
       '45': None}}} # wait 45 seconds for 900+ calls
 
 # add your API credentials for making calls to the "ske" server
-config = sgex.config.default
-config["ske"]["username"] = "J. Doe"
-config["ske"]["api_key"] = "1234"
+sgex.config.default["ske"] |= {"username": "J. Doe", "api_key": "1234"}
 ```
 
 ### 2. Making a `corp_info` API call
 
 Each type of API call has its own Python class (e.g., `CorpInfo`), which is a child of the generic `Call` class. To make API calls, start by creating `Call` objects.
 
 Calls are added to a `Package` class, which prepares requests and manages their execution. A `Package` can be inspected to make sure everything looks good before sending calls. Packages also expose other settings for more advanced usage.
@@ -204,15 +202,18 @@
 # indicate which server to use
 server = "ske"
 
 # define a call
 call = sgex.CorpInfo({"corpname": "preloaded/susanne"})
 
 # package the call
-package = sgex.Package(call, server, config)
+package = sgex.Package(call, server)
+
+# config dicts can also be passed explicitly
+# package = sgex.Package(call, server, config_dict)
 
 # inspect the package details
 print(package.calls)
 [CORP_INFO(2a8c0b24) {'api_key': '1234', 'username': 'J. Doe', 'corpname': 'preloaded/susanne'}]
 
 print(package.calls[0].request)
 <Request [GET]>
@@ -445,15 +446,15 @@
 Package.server: str  # server to call
 Package.halt: bool   # whether to stop a job on error
 Package.errors: set  # errors encountered
 Package.loglevel: str  # logging level
 Package.max_workers: int  # threads for asynchronous calls
 Package.responses: list  # call responses
 Package.max_responses: int  # max items to store in `Package.responses` (for large jobs)
-Package.session_params: dict(  # parameters for the `request-cache` session
+Package.session_params: dict(  # parameters for the `requests-cache` session
     cache_name="data",
     serializer="json",
     backend="filesystem",
     ignored_parameters=credential_parameters,
     key_fn=call.create_custom_key,
 )
 Package.config: dict  # server configuration
@@ -475,18 +476,18 @@
 These classes combine multiple API calls, parsing methods, etc., to execute larger jobs with a single command.
 
 **Text type analysis**
 
 `TTypeAnalysis` automates the steps for generating a DataFrame describing the corpus's composition.
 
 ```python
-from sgex.call import TTypeAnalysis
+from sgex.call.job import TTypeAnalysis
 
 # prepare the job
-ttypes = TTypeAnalysis("susanne", <server>, <config>)
+ttypes = TTypeAnalysis("susanne", <server>)
 
 # run the job
 ttypes.run()
 
 # view the results
 print(ttypes.df.head(3))
     str  frq  relfreq  attribute
@@ -496,18 +497,18 @@
 ```
 
 **Simple frequency query**
 
 `SimpleFreqsQuery` automates making a `freqs` call with Simple Query syntax and processing JSON data into a DataFrame.
 
 ```python
-from sgex.call import SimpleFreqsQuery
+from sgex.call.job import SimpleFreqsQuery
 
 # prepare the job
-query = SimpleFreqsQuery("sleep", "susanne", "noske", ".config.yml")
+query = SimpleFreqsQuery("sleep", "susanne", "noske")
 
 # run the job
 query.run()
 
 # view the results (each row is a corpus attribute/text type)
 print(query.df.head(3))
    frq         rel        reltt  ...  total_fpm total_size fmaxitems
```

