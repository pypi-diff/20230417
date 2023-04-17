# Comparing `tmp/q2report-0.1.25.tar.gz` & `tmp/q2report-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.25.tar", max compression
+gzip compressed data, was "q2report-0.1.26.tar", max compression
```

## Comparing `q2report-0.1.25.tar` & `q2report-0.1.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      472 2023-03-05 20:32:40.557948 q2report-0.1.25/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.25/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.25/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.25/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.25/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.25/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8053 2023-02-19 21:22:41.218242 q2report-0.1.25/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     7798 2023-02-24 09:23:06.744269 q2report-0.1.25/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18203 2023-02-24 12:25:39.270036 q2report-0.1.25/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     5484 2023-02-21 23:03:03.550305 q2report-0.1.25/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20036 2023-02-24 12:27:18.839233 q2report-0.1.25/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8167 2023-02-20 10:32:47.795979 q2report-0.1.25/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    15542 2023-03-05 20:30:05.218241 q2report-0.1.25/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.25/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-03-05 20:32:43.025864 q2report-0.1.25/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.25/README.md
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 q2report-0.1.25/setup.py
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 q2report-0.1.25/PKG-INFO
+-rw-r--r--   0        0        0      475 2023-04-17 10:50:10.817499 q2report-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.26/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.26/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.26/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.26/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.26/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8053 2023-02-19 21:22:41.218242 q2report-0.1.26/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     7798 2023-04-17 10:49:37.697724 q2report-0.1.26/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18203 2023-02-24 12:25:39.270036 q2report-0.1.26/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     5484 2023-02-21 23:03:03.550305 q2report-0.1.26/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20036 2023-02-24 12:27:18.839233 q2report-0.1.26/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8167 2023-02-20 10:32:47.795979 q2report-0.1.26/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    15542 2023-04-17 10:49:55.447800 q2report-0.1.26/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.26/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-04-17 10:50:13.570402 q2report-0.1.26/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.26/README.md
+-rw-r--r--   0        0        0     2131 1970-01-01 00:00:00.000000 q2report-0.1.26/setup.py
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.26/PKG-INFO
```

### Comparing `q2report-0.1.25/q2report/q2printer/docx_parts.py` & `q2report-0.1.26/q2report/q2printer/docx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/q2report/q2printer/q2printer.py` & `q2report-0.1.26/q2report/q2printer/q2printer.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.26/q2report/q2printer/q2printer_docx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/q2report/q2printer/q2printer_html.py` & `q2report-0.1.26/q2report/q2printer/q2printer_html.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.26/q2report/q2printer/q2printer_xlsx.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.26/q2report/q2printer/xlsx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/q2report/q2report.py` & `q2report-0.1.26/q2report/q2report.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/q2report/q2utils.py` & `q2report-0.1.26/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/README.md` & `q2report-0.1.26/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.25/setup.py` & `q2report-0.1.26/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['pillow>=9.4.0,<10.0.0']
 
 setup_kwargs = {
     'name': 'q2report',
-    'version': '0.1.25',
+    'version': '0.1.26',
     'description': '',
     'long_description': '# The light Python report builder.\nConverts data into formatted text (**HTML**, **DOCX**, **XLSX**):\n```python\ndata = {\'data_source1\':[{\'col1\': \'value row1\', ....}, ...],\n        \'data_source2\':[{\'col_1\': \'valie_row1\', ....}, ...],\n        }\n```\nAvailable formatting (styling options):\n```json  \n"style": {\n    "font-family": "Arial",\n    "font-size": "10pt",\n    "font-weight": "normal",\n    "border-width": "0 0 0 0",\n    "padding": "0.05cm 0.05cm 0.05cm 0.05cm",\n    "text-align": "left",\n    "vertical-align": "top"\n  }\n\n```\n## Concept\nThe report definition consists of sections (Report, Pages, Columns, Rows, Cells).  \nEach section inherits style from previous and may override some styling options.  \n*see examples in folder **test_data***\n```python\nReport:  # contains basic style\n    Pages:  # page & margins sizes\n        Columns:  # columns widths - exact, % or autowidth\n            Rows:  # rows heights - auto, exact, min or max\n                   # can be linked to data and then have header, footer and grouping subsections\n                   # \n                Cells  # contains simple text and data links - {col1}\n                       # and aggregate functions - {sum:coll}\n                       # support html formatting with <b> <i> <u> <br>\n                       # cells may be merged (span)\n            Rows:\n                Cells\n            ....\n        Columns:\n            ....\n    Pages:\n        ....\n    ....\n```',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8.1',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `q2report-0.1.25/PKG-INFO` & `q2report-0.1.26/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.25
+Version: 0.1.26
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Description-Content-Type: text/markdown
 
 # The light Python report builder.
```

