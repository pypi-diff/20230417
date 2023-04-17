# Comparing `tmp/read_rapidpe-0.1.0.tar.gz` & `tmp/read_rapidpe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_rapidpe-0.1.0.tar", max compression
+gzip compressed data, was "read_rapidpe-0.1.1.tar", max compression
```

## Comparing `read_rapidpe-0.1.0.tar` & `read_rapidpe-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2014 2022-11-12 06:32:47.036245 read_rapidpe-0.1.0/README.md
--rw-r--r--   0        0        0      404 2023-04-17 05:48:14.277945 read_rapidpe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      353 2023-04-16 13:12:20.078578 read_rapidpe-0.1.0/read_rapidpe/__init__.py
--rw-r--r--   0        0        0     8095 2022-12-12 05:47:03.434185 read_rapidpe-0.1.0/read_rapidpe/grid_point.py
--rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.1.0/read_rapidpe/p_astro.py
--rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.1.0/read_rapidpe/parser.py
--rw-r--r--   0        0        0     1474 2023-04-16 14:05:36.413685 read_rapidpe-0.1.0/read_rapidpe/plot.py
--rw-r--r--   0        0        0    18461 2023-04-17 05:43:56.585212 read_rapidpe-0.1.0/read_rapidpe/result.py
--rw-r--r--   0        0        0     2200 2022-11-25 08:05:18.514011 read_rapidpe-0.1.0/read_rapidpe/transform.py
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 read_rapidpe-0.1.0/setup.py
--rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 read_rapidpe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2014 2022-11-12 06:32:47.036245 read_rapidpe-0.1.1/README.md
+-rw-r--r--   0        0        0      423 2023-04-17 12:28:20.926528 read_rapidpe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-04-16 13:12:20.078578 read_rapidpe-0.1.1/read_rapidpe/__init__.py
+-rw-r--r--   0        0        0     8095 2022-12-12 05:47:03.434185 read_rapidpe-0.1.1/read_rapidpe/grid_point.py
+-rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.1.1/read_rapidpe/p_astro.py
+-rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.1.1/read_rapidpe/parser.py
+-rw-r--r--   0        0        0     1474 2023-04-16 14:05:36.413685 read_rapidpe-0.1.1/read_rapidpe/plot.py
+-rw-r--r--   0        0        0    18461 2023-04-17 05:43:56.585212 read_rapidpe-0.1.1/read_rapidpe/result.py
+-rw-r--r--   0        0        0     2200 2022-11-25 08:05:18.514011 read_rapidpe-0.1.1/read_rapidpe/transform.py
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 read_rapidpe-0.1.1/setup.py
+-rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 read_rapidpe-0.1.1/PKG-INFO
```

### Comparing `read_rapidpe-0.1.0/README.md` & `read_rapidpe-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.0/read_rapidpe/grid_point.py` & `read_rapidpe-0.1.1/read_rapidpe/grid_point.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.0/read_rapidpe/p_astro.py` & `read_rapidpe-0.1.1/read_rapidpe/p_astro.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.0/read_rapidpe/parser.py` & `read_rapidpe-0.1.1/read_rapidpe/parser.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.0/read_rapidpe/plot.py` & `read_rapidpe-0.1.1/read_rapidpe/plot.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.0/read_rapidpe/result.py` & `read_rapidpe-0.1.1/read_rapidpe/result.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.0/read_rapidpe/transform.py` & `read_rapidpe-0.1.1/read_rapidpe/transform.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.0/setup.py` & `read_rapidpe-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 ['read_rapidpe']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['joblib>=1.2.0,<2.0.0',
+ 'lalsuite>=7.14,<8.0',
  'matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.23.4,<2.0.0',
  'python-ligo-lw>=1.8.3,<2.0.0',
  'scipy>=1.9.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'read-rapidpe',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': 'Read Rapid-PE\n===\n\nThis is a package to read Rapid-PE outputs.\n\n# Install (dev mode)\n```\ngit clone git@git.ligo.org:yu-kuang.chu/read-rapidpe.git\ncd read-rapidpe\npip install -e . \n```\n\n# Example Usage\n\n## Plot marginalized log-likelihood on m1-m2 grid points\n```python\nfrom read_rapidpe import RapidPE_result\nimport matplotlib.pyplot as plt\nimport glob\n\n\nresults_dir = "path/to/results"\nresult_xml_files = glob.glob(results_dir+"*.xml.gz")\nresult = RapidPE_result.from_xml_array(result_xml_files)\n\n\n# Plot marginalized-log-likelihood over intrinsic parameter (mass_1/mass_2) grid points\nplt.scatter(result.mass_1, result.mass_2, c=result.marg_log_likelihood )\nplt.xlabel("$m_1$")\nplt.ylabel("$m_2$")\nplt.colorbar(label="$\\ln(L_{marg})$")\n```\n\n## Plot interpolated likelihood\n```python\nfrom read_rapidpe import RapidPE_result\nimport matplotlib.pyplot as plt\nimport glob\nimport numpy as np\n\n\nresults_dir = "path/to/results"\nresult_xml_files = glob.glob(results_dir+"*.xml.gz")\nresult = RapidPE_result.from_xml_array(result_xml_files)\n\n\n# Create Random m1, m2 samples\nm1 = np.random.random(10000)*5\nm2 = np.random.random(10000)*5\n\n\n# After calling result.do_interpolate_marg_log_likelihood_m1m2(), \n# the method result.log_likelihood(m1, m2) will be avalible.\nresult.do_interpolate_marg_log_likelihood_m1m2()\n\n# Calculate interpolated log_likelihood\nlog_likelihood = result.log_likelihood(m1, m2)\n\n\n# =============== Plotting ===============\n# Plot interpolated likelihood \nplt.scatter(m1, m2, c=np.exp(log_likelihood), marker=".", s=3, alpha=0.1)\n\n# Plot marginalized likelihood on grid points\nplt.scatter(result.mass_1, result.mass_2, c=np.exp(result.marg_log_likelihood), marker="+", vmin=0)\n\nplt.xlabel("$m_1$")\nplt.ylabel("$m_2$")\nplt.colorbar(label=r"$\\mathcal{L}$")\n```\n\n\n## Convert to Pandas DataFrame\n\n```python\nimport pandas as pd\nfrom read_rapidpe import RapidPE_grid_point\n\n\ngrid_point = RapidPE_grid_point.from_xml("ILE_iteration_xxxxxxxxxx.samples.xml.gz")\npd.DataFrame(grid_point.extrinsic_table)\n```\n\n',
     'author': 'Cory Chu',
     'author_email': 'cory@gwlab.page',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `read_rapidpe-0.1.0/PKG-INFO` & `read_rapidpe-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: read-rapidpe
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Cory Chu
 Author-email: cory@gwlab.page
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
+Requires-Dist: lalsuite (>=7.14,<8.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: python-ligo-lw (>=1.8.3,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 Read Rapid-PE
```

