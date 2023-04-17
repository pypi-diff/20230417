# Comparing `tmp/hledger_lots-0.1.3.tar.gz` & `tmp/hledger_lots-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_lots-0.1.3.tar", last modified: Thu Apr  6 19:34:54 2023, max compression
+gzip compressed data, was "hledger_lots-0.1.4.tar", last modified: Mon Apr 17 20:53:21 2023, max compression
```

## Comparing `hledger_lots-0.1.3.tar` & `hledger_lots-0.1.4.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-06 19:34:54.676165 hledger_lots-0.1.3/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4823 2023-04-06 19:34:54.676165 hledger_lots-0.1.3/PKG-INFO
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-06 19:34:54.670165 hledger_lots-0.1.3/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4483 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-06 19:34:54.672165 hledger_lots-0.1.3/hledger_lots/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/hledger_lots/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/hledger_lots/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2833 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/hledger_lots/avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2525 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/hledger_lots/avg_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/hledger_lots/checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    11421 2023-04-06 19:30:34.000000 hledger_lots-0.1.3/hledger_lots/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3626 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/hledger_lots/fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3040 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/hledger_lots/fifo_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      969 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/hledger_lots/files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-06 18:16:59.000000 hledger_lots-0.1.3/hledger_lots/hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4143 2023-04-06 17:59:15.000000 hledger_lots-0.1.3/hledger_lots/info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1856 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/hledger_lots/lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-06 19:34:54.673165 hledger_lots-0.1.3/hledger_lots.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4823 2023-04-06 19:34:54.000000 hledger_lots-0.1.3/hledger_lots.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      974 2023-04-06 19:34:54.000000 hledger_lots-0.1.3/hledger_lots.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-06 19:34:54.000000 hledger_lots-0.1.3/hledger_lots.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-06 19:34:54.000000 hledger_lots-0.1.3/hledger_lots.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       33 2023-04-06 19:34:54.000000 hledger_lots-0.1.3/hledger_lots.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-04-06 19:34:54.000000 hledger_lots-0.1.3/hledger_lots.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1174 2023-04-06 19:32:12.000000 hledger_lots-0.1.3/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-06 19:34:54.676165 hledger_lots-0.1.3/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-06 19:34:54.674165 hledger_lots-0.1.3/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-03-30 00:36:22.000000 hledger_lots-0.1.3/tests/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/tests/lots_data.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/tests/test__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4537 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/tests/test_avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/tests/test_checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2544 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/tests/test_fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2305 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/tests/test_files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/tests/test_hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-06 18:17:55.000000 hledger_lots-0.1.3/tests/test_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-03 16:53:21.000000 hledger_lots-0.1.3/tests/test_lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-06 19:34:54.670165 hledger_lots-0.1.3/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-06 19:34:54.676165 hledger_lots-0.1.3/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-03-29 00:01:39.000000 hledger_lots-0.1.3/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/PKG-INFO
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.203704 hledger_lots-0.1.4/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4733 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.205704 hledger_lots-0.1.4/hledger_lots/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3001 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2525 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/avg_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    12828 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3776 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3040 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/fifo_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      969 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/hledger_lots/hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4313 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2780 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3770 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/hledger_lots/prices_yahoo.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.207704 hledger_lots-0.1.4/hledger_lots.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1003 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       33 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       53 2023-04-17 20:53:21.000000 hledger_lots-0.1.4/hledger_lots.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1174 2023-04-17 20:49:44.000000 hledger_lots-0.1.4/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.210704 hledger_lots-0.1.4/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-03-30 00:36:22.000000 hledger_lots-0.1.4/tests/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/lots_data.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4601 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/tests/test_avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2612 2023-04-17 20:48:23.000000 hledger_lots-0.1.4/tests/test_fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2305 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-14 13:21:43.000000 hledger_lots-0.1.4/tests/test_lib.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.202704 hledger_lots-0.1.4/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-17 20:53:21.214704 hledger_lots-0.1.4/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-14 14:58:40.000000 hledger_lots-0.1.4/venv/bin/rstpep2html.py
```

### Comparing `hledger_lots-0.1.3/PKG-INFO` & `hledger_lots-0.1.4/hledger_lots.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hledger_lots
-Version: 0.1.3
+Name: hledger-lots
+Version: 0.1.4
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,15 @@
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
 This package create a sale transaction according to information provided by the user and traverse the journal file to determine what quantity and lot prices should be used and generate a valid hledger transaction to be appended to the journal with additional helpful calculations as comment tags.
 
 When using this package, you don't need to create lots as subaccounts or tag, just add a purchase transaction as usual and when there is a sale, *hledger-lots* will generate the correct postings adding the cost for you, so you don't need to bother looking for this information.
 
-It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction.
+It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction, including market performance from *prices directives*, which can be automatically downloaded from [Yahoo Finance](https://finance.yahoo.com/).
 
 To verify your transaction, this package can also check if your past sale has the correct cost.
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
@@ -43,15 +43,15 @@
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
 1. Add purchase transaction as normal. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/test2022.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-fifo will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
+2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
    
 
 ## Reports
 
 To get information about the commodities, there is more 2 commands:
@@ -59,15 +59,15 @@
 | command | description                                          |
 |---------|------------------------------------------------------|
 | view    | Get the lots and indicators for a specific commodity |
 | list   | Get the indicators for all commodities as a table    |
 
 
 
-If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail.
+If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail and [market prices](market_prices) to download the prices from [Yahoo Finance](https://finance.yahoo.com/).
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
```

### Comparing `hledger_lots-0.1.3/docs/README.md` & `hledger_lots-0.1.4/docs/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
 This package create a sale transaction according to information provided by the user and traverse the journal file to determine what quantity and lot prices should be used and generate a valid hledger transaction to be appended to the journal with additional helpful calculations as comment tags.
 
 When using this package, you don't need to create lots as subaccounts or tag, just add a purchase transaction as usual and when there is a sale, *hledger-lots* will generate the correct postings adding the cost for you, so you don't need to bother looking for this information.
 
-It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction.
+It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction, including market performance from *prices directives*, which can be automatically downloaded from [Yahoo Finance](https://finance.yahoo.com/).
 
 To verify your transaction, this package can also check if your past sale has the correct cost.
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
@@ -33,15 +33,15 @@
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
 1. Add purchase transaction as normal. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/test2022.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-fifo will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
+2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
    
 
 ## Reports
 
 To get information about the commodities, there is more 2 commands:
@@ -49,15 +49,15 @@
 | command | description                                          |
 |---------|------------------------------------------------------|
 | view    | Get the lots and indicators for a specific commodity |
 | list   | Get the indicators for all commodities as a table    |
 
 
 
-If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail.
+If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail and [market prices](market_prices) to download the prices from [Yahoo Finance](https://finance.yahoo.com/).
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
```

### Comparing `hledger_lots-0.1.3/hledger_lots/avg.py` & `hledger_lots-0.1.4/hledger_lots/avg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import subprocess
 from dataclasses import dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from typing import List, Optional
 
+from hledger_lots.hl import adjust_txn
+
 from . import checks
-from .lib import AdjustedTxn, CostMethodError, get_xirr
+from .lib import AdjustedTxn, CostMethodError, adjust_commodity, get_xirr
 
 
 @dataclass
 class AvgCost:
     date: str
     total_qtty: float = 0
     total_amount: float = 0
@@ -73,32 +75,35 @@
     qtty: float,
     cur: str,
     cash_account: str,
     revenue_account: str,
     comm_account: str,
     value: float,
     check: bool,
+    sell_cmd: str,
 ):
+    adj_comm = adjust_commodity(cur)
     checks.check_short_sell_current(txns, qtty)
     checks.check_base_currency(txns)
     checks.check_available(txns, comm_account, qtty)
 
     sell_date = datetime.strptime(date, "%Y-%m-%d").date()
     avg_cost = get_avg_cost(txns, check)
     cost = avg_cost[-1].avg_cost
 
     base_curr = txns[0].base_cur
     price = value / qtty
     xirr = get_xirr(price, sell_date, txns) or 0 * 100
 
-    txn_hl = f"""{date} Sold {cur}
+    txn_hl = f"""{date} Sold {cur}  ; cost_method:avg_cost
     ; commodity:{cur}, qtty:{qtty:,.2f}, price:{price:,.2f}
     ; xirr:{xirr:.2f}% annual percent rate 30/360US
+    ; command:{sell_cmd}
     {cash_account}    {value:.2f} {base_curr}
-    {comm_account}    {qtty * -1} {cur} @ {cost} {base_curr}
+    {comm_account}    {qtty * -1} {adj_comm} @ {cost} {base_curr}
     {revenue_account}"""
 
     comm = ["hledger", "-f-", "print", "--explicit"]
     txn_proc = subprocess.run(comm, input=txn_hl.encode(), capture_output=True)
 
     txn_print: str = txn_proc.stdout.decode("utf8")
     return txn_print
```

### Comparing `hledger_lots-0.1.3/hledger_lots/avg_info.py` & `hledger_lots-0.1.4/hledger_lots/avg_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/hledger_lots/checks.py` & `hledger_lots-0.1.4/hledger_lots/checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/hledger_lots/cli.py` & `hledger_lots-0.1.4/hledger_lots/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,37 @@
+import functools
 import os
+from pathlib import Path
 from typing import Literal, Tuple
 
 import rich_click as click
 
 from .avg import avg_sell, get_avg_cost
 from .avg_info import AllAvgInfo, AvgInfo
 from .fifo import get_lots, get_sell_lots, txn2hl
 from .fifo_info import AllFifoInfo, FifoInfo
 from .files import get_default_file, get_file_path
 from .hl import hledger2txn
-from .info import AllInfo
-from .lib import default_fn_bool, dt_list2table
+from .info import AllInfo, get_commodities
+from .lib import default_fn_bool, dt_list2table, get_sell_comm
+from .prices_yahoo import get_hledger_prices
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 click.rich_click.USE_MARKDOWN = True
 click.rich_click.SHOW_ARGUMENTS = True
 click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
 click.rich_click.MAX_WIDTH = 80
 click.rich_click.SHOW_METAVARS_COLUMN = False
 click.rich_click.APPEND_METAVARS_HELP = True
 click.rich_click.STYLE_ERRORS_SUGGESTION = "magenta italic"
 click.rich_click.ERRORS_SUGGESTION = (
     "Try running the '--help' flag for more information."
 )
-click.rich_click.ERRORS_EPILOGUE = "To find out more, visit [link=https://github.com/edkedk99/hledger-fifo]https://github.com/edkedk99/hledger-fifo[/link]"
+click.rich_click.ERRORS_EPILOGUE = "To find out more, visit [link=https://github.com/edkedk99/hledger-lots]https://github.com/edkedk99/hledger-lots[/link]"
 click.rich_click.STYLE_OPTIONS_TABLE_LEADING = 1
 click.rich_click.STYLE_OPTIONS_TABLE_BOX = "SIMPLE"
 click.rich_click.STYLE_OPTIONS_PANEL_BORDER = "dim"  # Possibly conceal
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 @click.option(
@@ -41,15 +44,15 @@
     help="Inform the journal file path. If \"-\", read from stdin. Without this flag read from $LEDGER_FILE or ~/.hledger.journal in this order  or '-f-'.",
 )
 @click.version_option()
 def cli(file: str):  # pyright:ignore
     """
     Commands to apply FIFO(first-in-first-out) or AVERAGE COST accounting principles without manual management of lots. Useful for transactions involving buying and selling foreign currencies or stocks.
 
-    To find out more, visit [https://github.com/edkedk99/hledger-fifo](https://github.com/edkedk99/hledger-fifo)
+    To find out more, visit [https://github.com/edkedk99/hledger-lots](https://github.com/edkedk99/hledger-lots)
     """
 
 
 @click.command()
 @click.option(
     "-f",
     "--file",
@@ -80,36 +83,50 @@
     default=lambda: os.environ.get("HLEDGER_LOTS_NO_DESC", None),
     prompt=False,
     help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
 )
 @click.option(
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
-    help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=tru|false. Default to false. Inthe future it will default to true",
+    help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. Inthe future it will default to true",
+)
+# TODO: fill help
+@click.option(
+    "-p",
+    "--append-prices-to",
+    type=click.Path(),
+    default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
+    prompt=False,
+    required=False,
+    help="Download market price and append to this option file value. Check the doc for info on how to set it up. Can be set with env HLEDGER_APPEND_PRICES_TO",
 )
 def view(
     file: Tuple[str, ...],
     avg_cost: bool,
     commodity: str,
     no_desc: str,
     check: bool,
+    append_prices_to: Path,
 ):
     """
     Report lots for a commodity.\r
 
     Show a report with lots for a commodity considering eventual past sale using FIFO or AVERAGE COST accounting principles.
 
     Also show some indicators about the lots and performance if there is prices in the journal after the last purchase. See the docs for details
 
     All flags, except '--file' will be interactively prompted if absent, much like 'hledger-add'.
     """
 
     journals = file or get_default_file()
     adj_txn = hledger2txn(journals, commodity, no_desc)
 
+    if append_prices_to:
+        get_hledger_prices(file, append_prices_to)
+
     if avg_cost:
         buy_lots = get_avg_cost(adj_txn, check)
         table = dt_list2table(buy_lots)
         click.echo(table)
         avg_info = AvgInfo(journals, commodity, check)
         click.echo(avg_info.info_txt)
 
@@ -232,39 +249,55 @@
     All flags, except '--file' will be interactively prompted if absent, much like 'hledger-add'.
     """
 
     journals = file or get_default_file()
     adj_txns = hledger2txn(journals, commodity, no_desc)
     value = quantity * price
 
+    sell_comm_fn = functools.partial(
+        get_sell_comm,
+        commodity,
+        no_desc,
+        commodity_account,
+        cash_account,
+        revenue_account,
+        date,
+        quantity,
+        price,
+    )
+
     if avg_cost and not commodity_account:
         commodity_account = input("Commodity account: ")
 
     if avg_cost:
+        sell_cmd = sell_comm_fn(True)
         sell_avg = avg_sell(
             txns=adj_txns,
             date=date,
             qtty=quantity,
             cur=commodity,
             cash_account=cash_account,
             revenue_account=revenue_account,
             comm_account=commodity_account,
             value=value,
             check=check,
+            sell_cmd=sell_cmd,
         )
         click.echo(sell_avg)
     else:
         sell_fifo = get_sell_lots(adj_txns, date, quantity, check)
+        sell_cmd = sell_comm_fn(False)
         txn_print = txn2hl(
             txns=sell_fifo,
             date=date,
             cur=commodity,
             cash_account=cash_account,
             revenue_account=revenue_account,
             value=value,
+            sell_cmd=sell_cmd,
         )
         click.echo(txn_print)
 
 
 @click.command(name="list")
 @click.option(
     "-f",
@@ -298,30 +331,43 @@
     help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
 )
 @click.option(
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
     help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=tru|false. Default to false. Inthe future it will default to true",
 )
+@click.option(
+    "-p",
+    "--append-prices-to",
+    type=click.Path(),
+    default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
+    prompt=False,
+    required=False,
+    help="Download market price and append to this option file value. Check the doc for info on how to set it up. Can be set with env HLEDGER_LOTS_APPEND_PRICES_TO",
+)
 def list_commodities(
     file: Tuple[str, ...],
     avg_cost: bool,
     output_format: str,
     no_desc: Literal["plain", "pretty", "csv"],
     check: bool,
+    append_prices_to: Path,
 ):
     """
     List indicators for all your commodities in a tabular format sorted from higher to lower **XIRR**. It is advised to use full-screen of the terminal. See the docs for a list of indicators and output examples.
 
     It can output in three formats: *plain, pretty and csv*.
     """
 
     journals = file or get_default_file()
     lots_info = AllInfo(journals, no_desc)
 
+    if append_prices_to:
+        get_hledger_prices(file, append_prices_to)
+
     lots_info = (
         AllAvgInfo(file, no_desc, check)
         if avg_cost
         else AllFifoInfo(file, no_desc, check)
     )
 
     if output_format == "pretty":
```

### Comparing `hledger_lots-0.1.3/hledger_lots/fifo.py` & `hledger_lots-0.1.4/hledger_lots/fifo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import subprocess
 from datetime import datetime
 from typing import List
 
 from . import checks
-from .lib import AdjustedTxn, CostMethodError, get_avg_fifo, get_xirr
+from .lib import AdjustedTxn, CostMethodError, adjust_commodity, get_avg_fifo, get_xirr
 
 
 def check_sell(sell: AdjustedTxn, previous_buys: List[AdjustedTxn], check: bool):
     if not check:
         return
 
     diff_zero = [
@@ -87,30 +87,37 @@
 def txn2hl(
     txns: List[AdjustedTxn],
     date: str,
     cur: str,
     cash_account: str,
     revenue_account: str,
     value: float,
+    sell_cmd: str,
 ):
+    adj_comm = adjust_commodity(cur)
     base_curr = txns[0].base_cur
     avg_cost = get_avg_fifo(txns)
     sum_qtty = sum(txn.qtty for txn in txns)
     price = value / sum_qtty
     dt = datetime.strptime(date, "%Y-%m-%d").date()
     xirr = get_xirr(price, dt, txns) or 0 * 100
 
     txn_hl = f"""
-{date} Sold {cur}
+{date} Sold {cur}  ; cost_method:fifo
     ; commodity:{cur}, qtty:{sum_qtty:,.2f}, price:{price:,.2f}
-    ; avg_fifo_cost:{avg_cost:,.4f}, xirr:{xirr:.2f}% annual percent rate 30/360US
+    ; avg_cost:{avg_cost:,.4f}, xirr:{xirr:.2f}% annual percent rate 30/360US
+    ; command:{sell_cmd}
     {cash_account}  {value:.2f} {base_curr}
 """
 
     for txn in txns:
-        txn_hl += f"    {txn.acct}    {txn.qtty * -1} {cur} @ {txn.price} {base_curr}  ; buy_date:{txn.date}, base_cur:{txn.base_cur}\n"
+        txn_hl += f"    {txn.acct}    {txn.qtty * -1} {adj_comm} @ {txn.price} {base_curr}  ; buy_date:{txn.date}, base_cur:{txn.base_cur}\n"
 
     txn_hl += f"    {revenue_account}   "
     comm = ["hledger", "-f-", "print", "--explicit"]
-    txn_proc = subprocess.run(comm, input=txn_hl.encode(), capture_output=True)
+    txn_proc = subprocess.run(
+        comm,
+        input=txn_hl.encode(),
+        capture_output=True,
+    )
     txn_print: str = txn_proc.stdout.decode("utf8")
     return txn_print
```

### Comparing `hledger_lots-0.1.3/hledger_lots/fifo_info.py` & `hledger_lots-0.1.4/hledger_lots/fifo_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/hledger_lots/files.py` & `hledger_lots-0.1.4/hledger_lots/files.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/hledger_lots/hl.py` & `hledger_lots-0.1.4/hledger_lots/hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/hledger_lots/info.py` & `hledger_lots-0.1.4/hledger_lots/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import csv
 import re
 import subprocess
+from dataclasses import dataclass
 from datetime import date, datetime
 from io import StringIO
 from typing import List, Optional, Tuple, TypedDict
 
 from tabulate import tabulate
 
 from .files import get_files_comm
 from .hl import hledger2txn
-from .lib import get_xirr
+from .lib import adjust_commodity, get_xirr
 
 
 class LotsInfo(TypedDict):
     comm: str
     cur: str
     qtty: str
     amount: str
@@ -21,57 +22,77 @@
     mkt_price: Optional[str]
     mkt_amount: Optional[str]
     mkt_profit: Optional[str]
     mkt_date: Optional[str]
     xirr: Optional[str]
 
 
+@dataclass
+class Price:
+    date: date
+    comm: str
+    price: float
+    cur: str
+
+
+def get_last_price(files_comm: List[str], commodity: str):
+    prices_comm = [
+        "hledger",
+        *files_comm,
+        "prices",
+        f"cur:{commodity}",
+        "--infer-reverse-prices",
+    ]
+    prices_proc = subprocess.run(prices_comm, capture_output=True)
+    prices_str = prices_proc.stdout.decode("utf8")
+
+    if prices_str == "":
+        return (None, None)
+
+    prices_list = [row.split(" ", 3) for row in prices_str.split("\n") if row != ""]
+
+    date_list = [
+        (row[1], re.sub(r"[a-zA-Z]|\,|\s", "", row[3]))
+        for row in prices_list
+        if row[2] == adjust_commodity(commodity)
+    ]
+
+    if len(date_list) == 0:
+        return (None, None)
+
+    last_date_str = date_list[-1][0]
+    last_date = datetime.strptime(last_date_str, "%Y-%m-%d").date()
+    last_price = float(date_list[-1][1])
+    return (last_date, last_price)
+
+
+def get_commodities(journals: Tuple[str, ...]):
+    files_comm = get_files_comm(journals)
+    comm = ["hledger", *files_comm, "commodities"]
+    commodities_proc = subprocess.run(comm, capture_output=True)
+    commodities_str = commodities_proc.stdout.decode("utf8")
+
+    commodities_list = [com for com in commodities_str.split("\n")]
+    return commodities_list
+
+
 class Info:
     def __init__(
         self, journals: Tuple[str, ...], commodity: str, no_desc: Optional[str] = None
     ) -> None:
         self.journals = journals
         self.files_comm = get_files_comm(journals)
         self.commodity = commodity
         self.txns = hledger2txn(journals, commodity, no_desc)
 
         self.has_txn = len(self.txns) > 0
 
-        self.market_date, self.market_price = self.last_price
+        self.last_price = get_last_price(self.files_comm, commodity)
 
-    @property
-    def last_price(self):
-        prices_comm = [
-            "hledger",
-            *self.files_comm,
-            "prices",
-            f"cur:{self.commodity}",
-            "--infer-reverse-prices",
-        ]
-        prices_proc = subprocess.run(prices_comm, capture_output=True)
-        prices_str = prices_proc.stdout.decode("utf8")
-
-        if prices_str == "":
-            return (None, None)
-
-        prices_list = [row.split(" ", 3) for row in prices_str.split("\n") if row != ""]
-
-        date_list = [
-            (row[1], re.sub(r"[a-zA-Z]|\,|\s", "", row[3]))
-            for row in prices_list
-            if row[2] == self.commodity
-        ]
-
-        if len(date_list) == 0:
-            return (None, None)
-
-        last_date_str = date_list[-1][0]
-        last_date = datetime.strptime(last_date_str, "%Y-%m-%d").date()
-        last_price = float(date_list[-1][1])
-        return (last_date, last_price)
+        self.market_date, self.market_price = self.last_price
 
     def get_lots_xirr(self, last_buy_date: date):
         if self.market_date and self.market_price and self.market_date >= last_buy_date:
             xirr = get_xirr(self.market_price, self.market_date, self.txns)
             return xirr
 
     def get_info_txt(self, info: LotsInfo):
@@ -98,24 +119,15 @@
         return info_txt
 
 
 class AllInfo:
     def __init__(self, journals: Tuple[str, ...], no_desc: str) -> None:
         self.journals = journals
         self.no_desc = no_desc
-
-    @property
-    def commodities(self):
-        files_comm = get_files_comm(self.journals)
-        comm = ["hledger", *files_comm, "commodities"]
-        commodities_proc = subprocess.run(comm, capture_output=True)
-        commodities_str = commodities_proc.stdout.decode("utf8")
-
-        commodities_list = [com for com in commodities_str.split("\n")]
-        return commodities_list
+        self.commodities = get_commodities(journals)
 
     def get_infos_table(self, infos: List[LotsInfo], output_format: str):
         infos_list = [info for info in infos]
         infos_sorted = sorted(
             infos_list, key=lambda info: info["xirr"] or "", reverse=True
         )
         table = tabulate(
```

### Comparing `hledger_lots-0.1.3/hledger_lots.egg-info/PKG-INFO` & `hledger_lots-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hledger-lots
-Version: 0.1.3
+Name: hledger_lots
+Version: 0.1.4
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-lots
 Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
 Project-URL: repository, https://github.com/edkedk99/hledger-lots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,15 @@
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
 This package create a sale transaction according to information provided by the user and traverse the journal file to determine what quantity and lot prices should be used and generate a valid hledger transaction to be appended to the journal with additional helpful calculations as comment tags.
 
 When using this package, you don't need to create lots as subaccounts or tag, just add a purchase transaction as usual and when there is a sale, *hledger-lots* will generate the correct postings adding the cost for you, so you don't need to bother looking for this information.
 
-It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction.
+It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction, including market performance from *prices directives*, which can be automatically downloaded from [Yahoo Finance](https://finance.yahoo.com/).
 
 To verify your transaction, this package can also check if your past sale has the correct cost.
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
@@ -43,15 +43,15 @@
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
 1. Add purchase transaction as normal. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/test2022.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-fifo will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
+2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
    
 
 ## Reports
 
 To get information about the commodities, there is more 2 commands:
@@ -59,15 +59,15 @@
 | command | description                                          |
 |---------|------------------------------------------------------|
 | view    | Get the lots and indicators for a specific commodity |
 | list   | Get the indicators for all commodities as a table    |
 
 
 
-If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail.
+If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail and [market prices](market_prices) to download the prices from [Yahoo Finance](https://finance.yahoo.com/).
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
```

### Comparing `hledger_lots-0.1.3/hledger_lots.egg-info/SOURCES.txt` & `hledger_lots-0.1.4/hledger_lots.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 hledger_lots/cli.py
 hledger_lots/fifo.py
 hledger_lots/fifo_info.py
 hledger_lots/files.py
 hledger_lots/hl.py
 hledger_lots/info.py
 hledger_lots/lib.py
+hledger_lots/prices_yahoo.py
 hledger_lots.egg-info/PKG-INFO
 hledger_lots.egg-info/SOURCES.txt
 hledger_lots.egg-info/dependency_links.txt
 hledger_lots.egg-info/entry_points.txt
 hledger_lots.egg-info/requires.txt
 hledger_lots.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `hledger_lots-0.1.3/pyproject.toml` & `hledger_lots-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting", "lots"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_lots"
-version = "0.1.3"
+version = "0.1.4"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "tabulate",
```

### Comparing `hledger_lots-0.1.3/tests/lots_data.py` & `hledger_lots-0.1.4/tests/lots_data.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/tests/test_avg.py` & `hledger_lots-0.1.4/tests/test_avg.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,20 +130,22 @@
             date="2022-02-01",
             qtty=50,
             cur="AAPL",
             cash_account="Asset:Bank",
             revenue_account="Revenue:Capital Gain",
             comm_account="Acct1",
             value=1000,
-            check=False
+            check=False,
+            sell_cmd=""
         )
 
-        expected = """2022-02-01 Sold AAPL
+        expected = """2022-02-01 Sold AAPL  ; cost_method:avg_cost
     ; commodity:AAPL, qtty:50.00, price:20.00
     ; xirr:3.56% annual percent rate 30/360US
+    ; command:
     Asset:Bank                                    1000.00 USD
     Acct1                   -50 AAPL @ 17.848837209302324 USD
     Revenue:Capital Gain               -107.5581395348838 USD
 
 """
 
         assert test == expected
```

### Comparing `hledger_lots-0.1.3/tests/test_checks.py` & `hledger_lots-0.1.4/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/tests/test_fifo.py` & `hledger_lots-0.1.4/tests/test_fifo.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,38 +48,40 @@
     date = "2022-02-01"
     cash_account = "Bank"
     revenue_account = "Revenue"
 
     def test_txn2hl_profit(self):
         cur = "USD"
         test = fifo.txn2hl(
-            self.txns, self.date, cur, self.cash_account, self.revenue_account, 160
+            self.txns, self.date, cur, self.cash_account, self.revenue_account, 160, ""
         )
 
-        expected = """2022-02-01 Sold USD
+        expected = """2022-02-01 Sold USD  ; cost_method:fifo
     ; commodity:USD, qtty:5.00, price:32.00
-    ; avg_fifo_cost:26.0000, xirr:61.42% annual percent rate 30/360US
+    ; avg_cost:26.0000, xirr:61.42% annual percent rate 30/360US
+    ; command:
     Bank                 160.00 USD
     Acct1      -2.00 USD @ 35.0 USD  ; buy_date:2022-01-12, base_cur:USD
     Acct1      -3.00 USD @ 20.0 USD  ; buy_date:2022-01-14, base_cur:USD
     Revenue              -30.00 USD
 
 """
 
         assert test == expected
 
     def test_txn2hl_loss(self):
         cur = "USD"
         test = fifo.txn2hl(
-            self.txns, self.date, cur, self.cash_account, self.revenue_account, 80
+            self.txns, self.date, cur, self.cash_account, self.revenue_account, 80, ""
         )
 
-        expected = """2022-02-01 Sold USD
+        expected = """2022-02-01 Sold USD  ; cost_method:fifo
     ; commodity:USD, qtty:5.00, price:16.00
-    ; avg_fifo_cost:26.0000, xirr:-1.00% annual percent rate 30/360US
+    ; avg_cost:26.0000, xirr:-1.00% annual percent rate 30/360US
+    ; command:
     Bank                  80.00 USD
     Acct1      -2.00 USD @ 35.0 USD  ; buy_date:2022-01-12, base_cur:USD
     Acct1      -3.00 USD @ 20.0 USD  ; buy_date:2022-01-14, base_cur:USD
     Revenue               50.00 USD
 
 """
```

### Comparing `hledger_lots-0.1.3/tests/test_files.py` & `hledger_lots-0.1.4/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/tests/test_hl.py` & `hledger_lots-0.1.4/tests/test_hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/tests/test_info.py` & `hledger_lots-0.1.4/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/tests/test_lib.py` & `hledger_lots-0.1.4/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.3/venv/bin/rst2html.py` & `hledger_lots-0.1.4/venv/bin/rst2html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # $Id: rst2html.py 8927 2022-01-03 23:50:05Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML.
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2html4.py` & `hledger_lots-0.1.4/venv/bin/rst2html4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # $Id: rst2html4.py 8927 2022-01-03 23:50:05Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing (X)HTML.
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2html5.py` & `hledger_lots-0.1.4/venv/bin/rst2html5.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 # :Copyright: © 2015 Günter Milde.
 # :License: Released under the terms of the `2-Clause BSD license`_, in short:
 #
 #    Copying and distribution of this file, with or without modification,
 #    are permitted in any medium without royalty provided the copyright
 #    notice and this notice are preserved.
 #    This file is offered as-is, without any warranty.
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2latex.py` & `hledger_lots-0.1.4/venv/bin/rst2latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # $Id: rst2latex.py 8956 2022-01-20 10:11:44Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing LaTeX.
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2man.py` & `hledger_lots-0.1.4/venv/bin/rst2man.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # Author:
 # Contact: grubert@users.sf.net
 # Copyright: This module has been placed in the public domain.
 
 """
 man.py
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2odt.py` & `hledger_lots-0.1.4/venv/bin/rst2odt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # $Id: rst2odt.py 8994 2022-01-29 16:28:17Z milde $
 # Author: Dave Kuhlman <dkuhlman@rexx.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 A front end to the Docutils Publisher, producing OpenOffice documents.
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2odt_prepstyles.py` & `hledger_lots-0.1.4/venv/bin/rst2odt_prepstyles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # $Id: rst2odt_prepstyles.py 8932 2022-01-05 14:59:31Z milde $
 # Author: Dave Kuhlman <dkuhlman@rexx.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 Fix a word-processor-generated styles.odt for odtwriter use: Drop page size
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2pseudoxml.py` & `hledger_lots-0.1.4/venv/bin/rst2xml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
-# $Id: rst2pseudoxml.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2xml.py 8927 2022-01-03 23:50:05Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
-A minimal front end to the Docutils Publisher, producing pseudo-XML.
+A minimal front end to the Docutils Publisher, producing Docutils XML.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
 except:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
-description = ('Generates pseudo-XML from standalone reStructuredText '
-               'sources (for testing purposes).  ' + default_description)
+description = ('Generates Docutils-native XML from standalone '
+               'reStructuredText sources.  ' + default_description)
 
-publish_cmdline(description=description)
+publish_cmdline(writer_name='xml', description=description)
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2s5.py` & `hledger_lots-0.1.4/venv/bin/rst2s5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # $Id: rst2s5.py 8927 2022-01-03 23:50:05Z milde $
 # Author: Chris Liechti <cliechti@gmx.net>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML slides using
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2xetex.py` & `hledger_lots-0.1.4/venv/bin/rst2xetex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
 # $Id: rst2xetex.py 8956 2022-01-20 10:11:44Z milde $
 # Author: Guenter Milde
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing Lua/XeLaTeX code.
```

### Comparing `hledger_lots-0.1.3/venv/bin/rst2xml.py` & `hledger_lots-0.1.4/venv/bin/rstpep2html.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
-# $Id: rst2xml.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rstpep2html.py 8927 2022-01-03 23:50:05Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
-A minimal front end to the Docutils Publisher, producing Docutils XML.
+A minimal front end to the Docutils Publisher, producing HTML from PEP
+(Python Enhancement Proposal) documents.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
 except:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
-description = ('Generates Docutils-native XML from standalone '
-               'reStructuredText sources.  ' + default_description)
+description = ('Generates (X)HTML from reStructuredText-format PEP files.  '
+               + default_description)
 
-publish_cmdline(writer_name='xml', description=description)
+publish_cmdline(reader_name='pep', writer_name='pep_html',
+                description=description)
```

### Comparing `hledger_lots-0.1.3/venv/bin/rstpep2html.py` & `hledger_lots-0.1.4/venv/bin/rst2pseudoxml.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-#!/home/eduardo/projects/hledger-fifo/venv/bin/python
+#!/home/eduardo/projects/hledger-lots/venv/bin/python
 
-# $Id: rstpep2html.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2pseudoxml.py 8927 2022-01-03 23:50:05Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
-A minimal front end to the Docutils Publisher, producing HTML from PEP
-(Python Enhancement Proposal) documents.
+A minimal front end to the Docutils Publisher, producing pseudo-XML.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
 except:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
-description = ('Generates (X)HTML from reStructuredText-format PEP files.  '
-               + default_description)
+description = ('Generates pseudo-XML from standalone reStructuredText '
+               'sources (for testing purposes).  ' + default_description)
 
-publish_cmdline(reader_name='pep', writer_name='pep_html',
-                description=description)
+publish_cmdline(description=description)
```

