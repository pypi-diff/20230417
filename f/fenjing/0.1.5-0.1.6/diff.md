# Comparing `tmp/fenjing-0.1.5.tar.gz` & `tmp/fenjing-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.1.5.tar", last modified: Mon Apr 17 05:46:04 2023, max compression
+gzip compressed data, was "fenjing-0.1.6.tar", last modified: Mon Apr 17 05:52:35 2023, max compression
```

## Comparing `fenjing-0.1.5.tar` & `fenjing-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:46:04.311000 fenjing-0.1.5/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.1.5/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 05:46:04.311000 fenjing-0.1.5/PKG-INFO
--rwxr-x---   0 user      (1000) user      (1000)     3553 2023-04-02 06:31:23.000000 fenjing-0.1.5/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:46:04.307000 fenjing-0.1.5/fenjing/
--rwxr-x---   0 user      (1000) user      (1000)      198 2023-04-16 05:52:30.000000 fenjing-0.1.5/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.1.5/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     2476 2023-04-16 05:52:51.000000 fenjing-0.1.5/fenjing/cli.py
--rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.1.5/fenjing/example.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.1.5/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2043 2023-04-17 05:43:42.000000 fenjing-0.1.5/fenjing/form.py
--rwxr-x---   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.1.5/fenjing/int_vars.py
--rwxr-x---   0 user      (1000) user      (1000)    37000 2023-03-31 08:46:50.000000 fenjing-0.1.5/fenjing/pattern.py
--rw-r--r--   0 user      (1000) user      (1000)      853 2023-04-02 05:33:58.000000 fenjing-0.1.5/fenjing/request.py
--rw-r--r--   0 user      (1000) user      (1000)      861 2023-04-17 05:43:42.000000 fenjing-0.1.5/fenjing/scan_url.py
--rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.1.5/fenjing/shell_cmd.py
--rw-r--r--   0 user      (1000) user      (1000)     3864 2023-04-17 05:43:42.000000 fenjing-0.1.5/fenjing/test_form.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:46:04.310000 fenjing-0.1.5/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      412 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-17 05:46:04.311000 fenjing-0.1.5/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.1.5/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:52:35.776000 fenjing-0.1.6/
+-rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.1.6/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 05:52:35.775000 fenjing-0.1.6/PKG-INFO
+-rwxr-x---   0 user      (1000) user      (1000)     3553 2023-04-02 06:31:23.000000 fenjing-0.1.6/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:52:35.771000 fenjing-0.1.6/fenjing/
+-rwxr-x---   0 user      (1000) user      (1000)      198 2023-04-16 05:52:30.000000 fenjing-0.1.6/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.1.6/fenjing/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2476 2023-04-16 05:52:51.000000 fenjing-0.1.6/fenjing/cli.py
+-rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.1.6/fenjing/example.py
+-rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.1.6/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     2053 2023-04-17 05:49:44.000000 fenjing-0.1.6/fenjing/form.py
+-rwxr-x---   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.1.6/fenjing/int_vars.py
+-rwxr-x---   0 user      (1000) user      (1000)    37000 2023-03-31 08:46:50.000000 fenjing-0.1.6/fenjing/pattern.py
+-rw-r--r--   0 user      (1000) user      (1000)      853 2023-04-02 05:33:58.000000 fenjing-0.1.6/fenjing/request.py
+-rw-r--r--   0 user      (1000) user      (1000)      871 2023-04-17 05:49:44.000000 fenjing-0.1.6/fenjing/scan_url.py
+-rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.1.6/fenjing/shell_cmd.py
+-rw-r--r--   0 user      (1000) user      (1000)     3874 2023-04-17 05:49:44.000000 fenjing-0.1.6/fenjing/test_form.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:52:35.775000 fenjing-0.1.6/fenjing.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 05:52:35.000000 fenjing-0.1.6/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      412 2023-04-17 05:52:35.000000 fenjing-0.1.6/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-17 05:52:35.000000 fenjing-0.1.6/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-17 05:52:35.000000 fenjing-0.1.6/fenjing.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-17 05:52:35.000000 fenjing-0.1.6/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-17 05:52:35.776000 fenjing-0.1.6/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.1.6/setup.py
```

### Comparing `fenjing-0.1.5/LICENSE` & `fenjing-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/PKG-INFO` & `fenjing-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.1.5/README.md` & `fenjing-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/fenjing/cli.py` & `fenjing-0.1.6/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/fenjing/example.py` & `fenjing-0.1.6/fenjing/example.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/fenjing/form.py` & `fenjing-0.1.6/fenjing/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     uri = parsed_url[3]
 
     if isinstance(html, str):
         bs = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
         bs = html
     else:
-        raise NotImplemented(f"Unsupported Type: {type(html)=}")
+        raise NotImplemented(f"Unsupported Type: type(html)={type(html)}")
 
     details = []
     for form_element in bs.select("form"):
         form = Form(
             action=form_element.attrs.get("action", uri),
             method=form_element.attrs.get("method", "POST").upper(),
             inputs=[
```

### Comparing `fenjing-0.1.5/fenjing/int_vars.py` & `fenjing-0.1.6/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/fenjing/pattern.py` & `fenjing-0.1.6/fenjing/pattern.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/fenjing/request.py` & `fenjing-0.1.6/fenjing/request.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/fenjing/scan_url.py` & `fenjing-0.1.6/fenjing/scan_url.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def parse_urls(html):
     if isinstance(html, str):
         bs = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
         bs = html
     else:
-        raise NotImplemented(f"Unsupported Type: {type(html)=}")
+        raise NotImplemented(f"Unsupported Type: type(html)={type(html)}")
 
     return [element.attrs["href"] for element in bs.select("a") if "href" in element]
 
 def yield_form(start_url):
     targets = [start_url, ]
     visited = set()
     while targets:
```

### Comparing `fenjing-0.1.5/fenjing/shell_cmd.py` & `fenjing-0.1.6/fenjing/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.5/fenjing/test_form.py` & `fenjing-0.1.6/fenjing/test_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ]
 
 
 def submit_form_input(url: str, form: dict, inputs: dict):
     """
     submit the form inside the url with the inputs
     """
-    logger.info(f"submit {inputs=}")
+    logger.info(f"submit inputs={inputs}")
     if any(len(v) > 2048 for v in inputs.values()) and form["method"] == "GET":
         logger.warning(
             "some inputs are extremely long that the request might fail")
     kwargs = fill_form(url, form, inputs)
     resp = common_request(**kwargs)
     return resp
 
@@ -77,15 +77,15 @@
 def test_form(url, form):
     """
     test whether a form is vulunable,
     if it is, return a function that generate shell command payload.
     """
     cmd = "echo y a  y;"
 
-    logger.info(f"Start testing form, {form=}")
+    logger.info(f"Start testing form, form={form}")
     possible_inputs = get_possible_input(url, form)
     logger.info(f"These inputs might be vulunable: {possible_inputs}")
 
     for possible_input in possible_inputs:
 
         logger.info(f"Tesing: {possible_input}")
```

### Comparing `fenjing-0.1.5/fenjing.egg-info/PKG-INFO` & `fenjing-0.1.6/fenjing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.1.5/setup.py` & `fenjing-0.1.6/setup.py`

 * *Files identical despite different names*

