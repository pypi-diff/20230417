# Comparing `tmp/pyportfoliopt-1.5.5.tar.gz` & `tmp/pyportfoliopt-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyportfoliopt-1.5.5.tar", last modified: Mon Apr 17 16:51:04 2023, max compression
+gzip compressed data, was "pyportfoliopt-1.5.6.tar", last modified: Mon Apr 17 17:00:17 2023, max compression
```

## Comparing `pyportfoliopt-1.5.5.tar` & `pyportfoliopt-1.5.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:51:04.363251 pyportfoliopt-1.5.5/
--rw-rw-rw-   0        0        0     1077 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0    20857 2023-04-17 16:51:04.349151 pyportfoliopt-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0    20940 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 16:51:03.710563 pyportfoliopt-1.5.5/pypfopt/
--rw-rw-rw-   0        0        0      767 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/__init__.py
--rw-rw-rw-   0        0        0    24419 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/base_optimizer.py
--rw-rw-rw-   0        0        0    19446 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/black_litterman.py
--rw-rw-rw-   0        0        0    17052 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/cla.py
--rw-rw-rw-   0        0        0    13639 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/discrete_allocation.py
--rw-rw-rw-   0        0        0      675 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/exceptions.py
--rw-rw-rw-   0        0        0    10639 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/expected_returns.py
--rw-rw-rw-   0        0        0     7764 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/hierarchical_portfolio.py
--rw-rw-rw-   0        0        0     8584 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/objective_functions.py
--rw-rw-rw-   0        0        0     9731 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/plotting.py
--rw-rw-rw-   0        0        0    21228 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/pypfopt/risk_models.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:51:04.055257 pyportfoliopt-1.5.5/pyportfoliopt.egg-info/
--rw-rw-rw-   0        0        0    20857 2023-04-17 16:51:02.000000 pyportfoliopt-1.5.5/pyportfoliopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      931 2023-04-17 16:51:02.000000 pyportfoliopt-1.5.5/pyportfoliopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:51:02.000000 pyportfoliopt-1.5.5/pyportfoliopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-17 16:51:02.000000 pyportfoliopt-1.5.5/pyportfoliopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 16:51:02.000000 pyportfoliopt-1.5.5/pyportfoliopt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1790 2023-04-17 16:50:45.000000 pyportfoliopt-1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 16:51:04.363251 pyportfoliopt-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0   120341 2023-04-17 16:50:34.000000 pyportfoliopt-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:51:04.349151 pyportfoliopt-1.5.5/tests/
--rw-rw-rw-   0        0        0    10888 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_base_optimizer.py
--rw-rw-rw-   0        0        0    21361 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_black_litterman.py
--rw-rw-rw-   0        0        0     4727 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_cla.py
--rw-rw-rw-   0        0        0    11209 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_custom_objectives.py
--rw-rw-rw-   0        0        0    13105 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_discrete_allocation.py
--rw-rw-rw-   0        0        0    13318 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_efficient_cdar.py
--rw-rw-rw-   0        0        0    13592 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_efficient_cvar.py
--rw-rw-rw-   0        0        0    42992 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_efficient_frontier.py
--rw-rw-rw-   0        0        0    18697 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_efficient_semivariance.py
--rw-rw-rw-   0        0        0     9787 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_expected_returns.py
--rw-rw-rw-   0        0        0     2429 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_hrp.py
--rw-rw-rw-   0        0        0     1196 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_imports.py
--rw-rw-rw-   0        0        0     4353 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_objective_functions.py
--rw-rw-rw-   0        0        0     8557 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_plotting.py
--rw-rw-rw-   0        0        0    12636 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.5/tests/test_risk_models.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:00:17.462500 pyportfoliopt-1.5.6/
+-rw-rw-rw-   0        0        0     1077 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    20810 2023-04-17 17:00:17.362262 pyportfoliopt-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0    20940 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 17:00:15.459094 pyportfoliopt-1.5.6/pypfopt/
+-rw-rw-rw-   0        0        0      767 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/__init__.py
+-rw-rw-rw-   0        0        0    24419 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/base_optimizer.py
+-rw-rw-rw-   0        0        0    19446 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/black_litterman.py
+-rw-rw-rw-   0        0        0    17052 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/cla.py
+-rw-rw-rw-   0        0        0    13639 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/discrete_allocation.py
+-rw-rw-rw-   0        0        0      675 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/exceptions.py
+-rw-rw-rw-   0        0        0    10639 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/expected_returns.py
+-rw-rw-rw-   0        0        0     7764 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/hierarchical_portfolio.py
+-rw-rw-rw-   0        0        0     8584 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/objective_functions.py
+-rw-rw-rw-   0        0        0     9731 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/plotting.py
+-rw-rw-rw-   0        0        0    21228 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/pypfopt/risk_models.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:00:15.698073 pyportfoliopt-1.5.6/pyportfoliopt.egg-info/
+-rw-rw-rw-   0        0        0    20810 2023-04-17 17:00:14.000000 pyportfoliopt-1.5.6/pyportfoliopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      931 2023-04-17 17:00:14.000000 pyportfoliopt-1.5.6/pyportfoliopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:00:14.000000 pyportfoliopt-1.5.6/pyportfoliopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-17 17:00:14.000000 pyportfoliopt-1.5.6/pyportfoliopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 17:00:14.000000 pyportfoliopt-1.5.6/pyportfoliopt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1790 2023-04-17 16:50:45.000000 pyportfoliopt-1.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:00:17.462500 pyportfoliopt-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0   120294 2023-04-17 16:59:51.000000 pyportfoliopt-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:00:17.335122 pyportfoliopt-1.5.6/tests/
+-rw-rw-rw-   0        0        0    10888 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_base_optimizer.py
+-rw-rw-rw-   0        0        0    21361 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_black_litterman.py
+-rw-rw-rw-   0        0        0     4727 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_cla.py
+-rw-rw-rw-   0        0        0    11209 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_custom_objectives.py
+-rw-rw-rw-   0        0        0    13105 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_discrete_allocation.py
+-rw-rw-rw-   0        0        0    13318 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_efficient_cdar.py
+-rw-rw-rw-   0        0        0    13592 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_efficient_cvar.py
+-rw-rw-rw-   0        0        0    42992 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_efficient_frontier.py
+-rw-rw-rw-   0        0        0    18697 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_efficient_semivariance.py
+-rw-rw-rw-   0        0        0     9787 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_expected_returns.py
+-rw-rw-rw-   0        0        0     2429 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_hrp.py
+-rw-rw-rw-   0        0        0     1196 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_imports.py
+-rw-rw-rw-   0        0        0     4353 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_objective_functions.py
+-rw-rw-rw-   0        0        0     8557 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_plotting.py
+-rw-rw-rw-   0        0        0    12636 2022-12-19 02:22:55.000000 pyportfoliopt-1.5.6/tests/test_risk_models.py
```

### Comparing `pyportfoliopt-1.5.5/LICENSE.txt` & `pyportfoliopt-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/PKG-INFO` & `pyportfoliopt-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyportfoliopt
-Version: 1.5.5
+Version: 1.5.6
 Summary: Financial portfolio optimization in python
-Home-page: https://github.com/robertmartin8/PyPortfolioOpt
+Home-page: 
 Author: Robert Andrew Martin
 Author-email: martin.robertandrew@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyportfolioopt.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/robertmartin8/PyPortfolioOpt/issues
 Project-URL: Personal website, https://reasonabledeviations.com
 Keywords: portfolio finance optimization quant trading investing
```

### Comparing `pyportfoliopt-1.5.5/README.md` & `pyportfoliopt-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/__init__.py` & `pyportfoliopt-1.5.6/pypfopt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/base_optimizer.py` & `pyportfoliopt-1.5.6/pypfopt/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/black_litterman.py` & `pyportfoliopt-1.5.6/pypfopt/black_litterman.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/cla.py` & `pyportfoliopt-1.5.6/pypfopt/cla.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/discrete_allocation.py` & `pyportfoliopt-1.5.6/pypfopt/discrete_allocation.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/exceptions.py` & `pyportfoliopt-1.5.6/pypfopt/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/expected_returns.py` & `pyportfoliopt-1.5.6/pypfopt/expected_returns.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/hierarchical_portfolio.py` & `pyportfoliopt-1.5.6/pypfopt/hierarchical_portfolio.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/objective_functions.py` & `pyportfoliopt-1.5.6/pypfopt/objective_functions.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/plotting.py` & `pyportfoliopt-1.5.6/pypfopt/plotting.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pypfopt/risk_models.py` & `pyportfoliopt-1.5.6/pypfopt/risk_models.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pyportfoliopt.egg-info/PKG-INFO` & `pyportfoliopt-1.5.6/pyportfoliopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyportfoliopt
-Version: 1.5.5
+Version: 1.5.6
 Summary: Financial portfolio optimization in python
-Home-page: https://github.com/robertmartin8/PyPortfolioOpt
+Home-page: 
 Author: Robert Andrew Martin
 Author-email: martin.robertandrew@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyportfolioopt.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/robertmartin8/PyPortfolioOpt/issues
 Project-URL: Personal website, https://reasonabledeviations.com
 Keywords: portfolio finance optimization quant trading investing
```

### Comparing `pyportfoliopt-1.5.5/pyportfoliopt.egg-info/SOURCES.txt` & `pyportfoliopt-1.5.6/pyportfoliopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/pyproject.toml` & `pyportfoliopt-1.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/setup.py` & `pyportfoliopt-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,19 +142,19 @@
     desc = f.read()
     desc = desc.split("<!-- content -->")[-1]
     desc = re.sub("<[^<]+?>", "", desc)  # Remove html
 
 
 setup(
     name="pyportfoliopt",
-    version="1.5.5",
+    version="1.5.6",
     description="Financial portfolio optimization in python",
     long_description=desc,
     long_description_content_type="text/markdown",
-    url="https://github.com/robertmartin8/PyPortfolioOpt",
+    url="",
     author="Robert Andrew Martin",
     author_email="martin.robertandrew@gmail.com",
     license="MIT",
     packages=["pypfopt"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
```

### Comparing `pyportfoliopt-1.5.5/tests/test_base_optimizer.py` & `pyportfoliopt-1.5.6/tests/test_base_optimizer.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_black_litterman.py` & `pyportfoliopt-1.5.6/tests/test_black_litterman.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_cla.py` & `pyportfoliopt-1.5.6/tests/test_cla.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_custom_objectives.py` & `pyportfoliopt-1.5.6/tests/test_custom_objectives.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_discrete_allocation.py` & `pyportfoliopt-1.5.6/tests/test_discrete_allocation.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_efficient_cdar.py` & `pyportfoliopt-1.5.6/tests/test_efficient_cdar.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_efficient_cvar.py` & `pyportfoliopt-1.5.6/tests/test_efficient_cvar.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_efficient_frontier.py` & `pyportfoliopt-1.5.6/tests/test_efficient_frontier.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_efficient_semivariance.py` & `pyportfoliopt-1.5.6/tests/test_efficient_semivariance.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_expected_returns.py` & `pyportfoliopt-1.5.6/tests/test_expected_returns.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_hrp.py` & `pyportfoliopt-1.5.6/tests/test_hrp.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_imports.py` & `pyportfoliopt-1.5.6/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_objective_functions.py` & `pyportfoliopt-1.5.6/tests/test_objective_functions.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_plotting.py` & `pyportfoliopt-1.5.6/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pyportfoliopt-1.5.5/tests/test_risk_models.py` & `pyportfoliopt-1.5.6/tests/test_risk_models.py`

 * *Files identical despite different names*

