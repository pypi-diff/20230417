# Comparing `tmp/chattychattybangbang-0.0.5.tar.gz` & `tmp/chattychattybangbang-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattychattybangbang-0.0.5.tar", last modified: Tue Apr 11 15:52:20 2023, max compression
+gzip compressed data, was "chattychattybangbang-0.0.6.tar", last modified: Tue Apr 11 21:32:14 2023, max compression
```

## Comparing `chattychattybangbang-0.0.5.tar` & `chattychattybangbang-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/chattychattybangbang/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/castigateuntilvalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/castigateuntilvaluesare.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/castigators.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/jsonutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/openaicredentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/openutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/chattychattybangbang/whereami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 15:52:20.000000 chattychattybangbang-0.0.5/chattychattybangbang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:52:20.353604 chattychattybangbang-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 15:51:48.000000 chattychattybangbang-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:32:14.241613 chattychattybangbang-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-11 21:32:14.241613 chattychattybangbang-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:32:14.241613 chattychattybangbang-0.0.6/chattychattybangbang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/castigateuntilvalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/castigateuntilvaluesare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/castigators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/jsonutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/openaicredentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/openutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/chattychattybangbang/whereami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:32:14.241613 chattychattybangbang-0.0.6/chattychattybangbang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-11 21:32:14.000000 chattychattybangbang-0.0.6/chattychattybangbang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 21:32:14.000000 chattychattybangbang-0.0.6/chattychattybangbang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:32:14.000000 chattychattybangbang-0.0.6/chattychattybangbang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 21:32:14.000000 chattychattybangbang-0.0.6/chattychattybangbang.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 21:32:14.000000 chattychattybangbang-0.0.6/chattychattybangbang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 21:32:14.000000 chattychattybangbang-0.0.6/chattychattybangbang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:32:14.241613 chattychattybangbang-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 21:31:36.000000 chattychattybangbang-0.0.6/setup.py
```

### Comparing `chattychattybangbang-0.0.5/LICENSE` & `chattychattybangbang-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.5/PKG-INFO` & `chattychattybangbang-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattychattybangbang
-Version: 0.0.5
+Version: 0.0.6
 Summary: chat utilities
 Home-page: https://github.com/chattychattybangbang/chattychattybangbang
 Author: chattychattybangbang
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,18 @@
 Utilities for using chatgpt more reliably
 
 
 ### Install
 
     pip install chattychattybangbang
     
+### Set key
+
+    import os
+    os.environ['OPEN_AI_KEY'] = 'getakeyfromopenaisite' 
     
 ### Example
 Asks ChatGPT a question, then calls it again to QA the answer. 
 
 
     from chattychattybangbang.castigateuntilvaluesare import castigate_until_values_are
     question = """
@@ -35,9 +39,11 @@
       Just provide the dict and nothing else in your response, please. 
     """
     d = castigate_until_values_are(question=question, value_description='a color', max_retries=5)
     print(d)
     
     {'AAPL': 'white', 'MSFT': 'red', 'GOOGL': 'green'}
 
+See [examples](https://github.com/microprediction/chattychattybangbang/tree/main/examples) for presidential poetry appreciation, etc. 
+
 ### Article
 See [Reliably getting answers out of chatgpt](https://medium.com/@mike.roweprediger/reliably-getting-answers-out-of-chatgpt-by-forcing-it-to-qa-itself-feb1f56782b9) on medium. Thanks to Michael Rowe.
```

### Comparing `chattychattybangbang-0.0.5/README.md` & `chattychattybangbang-0.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 Utilities for using chatgpt more reliably
 
 
 ### Install
 
     pip install chattychattybangbang
     
+### Set key
+
+    import os
+    os.environ['OPEN_AI_KEY'] = 'getakeyfromopenaisite' 
     
 ### Example
 Asks ChatGPT a question, then calls it again to QA the answer. 
 
 
     from chattychattybangbang.castigateuntilvaluesare import castigate_until_values_are
     question = """
@@ -19,9 +23,11 @@
       Just provide the dict and nothing else in your response, please. 
     """
     d = castigate_until_values_are(question=question, value_description='a color', max_retries=5)
     print(d)
     
     {'AAPL': 'white', 'MSFT': 'red', 'GOOGL': 'green'}
 
+See [examples](https://github.com/microprediction/chattychattybangbang/tree/main/examples) for presidential poetry appreciation, etc. 
+
 ### Article
 See [Reliably getting answers out of chatgpt](https://medium.com/@mike.roweprediger/reliably-getting-answers-out-of-chatgpt-by-forcing-it-to-qa-itself-feb1f56782b9) on medium. Thanks to Michael Rowe.
```

### Comparing `chattychattybangbang-0.0.5/chattychattybangbang/castigateuntilvalid.py` & `chattychattybangbang-0.0.6/chattychattybangbang/castigateuntilvaluesare.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-from chattychattybangbang.openaicredentials import set_credentials
-from chattychattybangbang.validators import default_validator, validate_numeric_dict
-from chattychattybangbang.jsonutil import json_or_none
-from chattychattybangbang.castigators import default_castigator
-from chattychattybangbang.openutil import ask_gpt
-
+from chattychattybangbang.castigateuntilvalid import castigate_until_valid
+from chattychattybangbang.validators import validate_yes_or_no
 
 DEFAULT_MAX_RETRIES = 3
+DEFAULT_N_CHECK = 5
 
 
-def castigate_until_valid(question:str, validator=None, castigator=None, max_retries:int=DEFAULT_MAX_RETRIES):
+def values_isa_validator(parsed_response: dict, value_description:str,
+                         max_retries=DEFAULT_MAX_RETRIES, n_check=DEFAULT_N_CHECK):
+    """ For each value in a dictionary, ask ChatGPT if it meets value_description
+        Short-circuit
+    :param value_description:  'is a president'
+    :param n_check:            How many to check
+    :return:
     """
-    :param question:
-    :param validator:     Function taking dict --> bool
-    :param castigator:    Function taking castigator(question, response) --> str
+    n_checked = 0
+    for k, v in parsed_response.items():
+        validation_question = 'Please answer the following as a yes or no question only, returning a single word please. Is ' + str(
+            v) + ' ' + value_description + ' ?'
+        yes_or_no_dict = castigate_until_valid(question=validation_question,
+                                          validator=validate_yes_or_no,
+                                          max_retries=max_retries)
+        if yes_or_no_dict is None:
+            return False
+        else:
+            yes_or_no_values = list(yes_or_no_dict.values())[0]
+            if not isinstance(yes_or_no_values, str) or (('no' in yes_or_no_values.lower()) and ('yes' not in yes_or_no_values.lower())):
+                return False
+            else:
+                n_checked+=1
+                if n_checked>=n_check:
+                    break
+    return True
+
+
+def castigate_until_values_are(question:str, value_description:str,
+                               castigator=None, max_retries=DEFAULT_MAX_RETRIES,
+                               n_check=5):
+    """ Retry until we get a dict whose values are 'value_description'
+    :param question:   'Please provide a dictionary length 3 where
+    :param value_description:  'is a color'
+    :param castigator:
     :param max_retries:
     :return:
     """
-    if validator is None:
-        validator = default_validator
-    if castigator is None:
-        castigator = default_castigator
-
-    retries = 0
-
-    while retries < max_retries:
-        response = ask_gpt(question)
-        parsed_response = json_or_none(response)
-
-        if parsed_response and validator(parsed_response):
-            break
-
-        question = castigator(question, response)
-        retries += 1
-
-    if retries == max_retries:
-        return None
-    else:
-        return parsed_response
-
-
-def castigate_until_numeric_dict(question:str, castigator=None, max_retries=DEFAULT_MAX_RETRIES):
-    return castigate_until_valid(question=question, validator=validate_numeric_dict, max_retries=max_retries)
+    def _validator(parsed_response):
+         return values_isa_validator(parsed_response=parsed_response,
+                                     value_description=value_description,
+                                     n_check=n_check)
+
+    return castigate_until_valid(question=question,
+                                validator=_validator,
+                                  castigator=castigator,
+                                max_retries=max_retries)
 
 
 if __name__=='__main__':
     question = """
-      I would like you to create a dictionary by choosing three tickers from companies
-      that were in the sp500 index in 2011 and returning a dictionary with keys given by
-      the tickers and values equal to a text description of the colors of the companies
-      in question. 
+      I would like you to pick three companies from the sp500 index. 
+      Return a dictionary containing the main color in their logo (pick one only)
+      The keys of the dictionary should be the company tickers. 
+      Just provide the dict and nothing else in your response, please. 
     """
-    d = castigate_until_valid(question=question)
+    d = castigate_until_values_are(question=question, value_description='a color')
+    print(d)
```

### Comparing `chattychattybangbang-0.0.5/chattychattybangbang/openaicredentials.py` & `chattychattybangbang-0.0.6/chattychattybangbang/openaicredentials.py`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.5/chattychattybangbang/validators.py` & `chattychattybangbang-0.0.6/chattychattybangbang/validators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from hypothesis import given
 from hypothesis.strategies import dictionaries, text
+from typing import Dict, List, Union, KeysView, Any
 
 # Example validators
 
 
 def validate_text_dict(parsed_response:dict):
     return isinstance(parsed_response,dict)
 
@@ -13,14 +14,40 @@
         for k,v in parsed_response.items():
             v_float = float(v)
         return True
     except Exception as e:
         return False
 
 
+STR_KEYS_TYPE = Union[List[str], Dict[str, Any], KeysView[str]]
+
+
+def validate_numeric_dict_with_known_keys(parsed_response: dict,
+                                          valid_keys:STR_KEYS_TYPE,
+                                          case_insensitive=True):
+
+    def _is_in(s: str, string_set: set) -> bool:
+        # Case-insensitive membership
+        s_lower = s.lower()
+        lower_set = {item.lower() for item in list(string_set)}
+        return s_lower in lower_set
+
+    try:
+        for k, v in parsed_response.items():
+            v_float = float(v)
+            if case_insensitive:
+                assert _is_in(k, valid_keys)
+            else:
+                assert k in valid_keys
+
+        return True
+    except Exception as e:
+        return False
+
+
 def validate_yes_or_no(parsed_response:dict):
     value = list(parsed_response.values())[0]
     return isinstance(value,str) and (('yes' in value.lower()) or ('no' in value.lower()))
 
 
 default_validator = validate_text_dict
```

### Comparing `chattychattybangbang-0.0.5/chattychattybangbang.egg-info/PKG-INFO` & `chattychattybangbang-0.0.6/chattychattybangbang.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattychattybangbang
-Version: 0.0.5
+Version: 0.0.6
 Summary: chat utilities
 Home-page: https://github.com/chattychattybangbang/chattychattybangbang
 Author: chattychattybangbang
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,18 @@
 Utilities for using chatgpt more reliably
 
 
 ### Install
 
     pip install chattychattybangbang
     
+### Set key
+
+    import os
+    os.environ['OPEN_AI_KEY'] = 'getakeyfromopenaisite' 
     
 ### Example
 Asks ChatGPT a question, then calls it again to QA the answer. 
 
 
     from chattychattybangbang.castigateuntilvaluesare import castigate_until_values_are
     question = """
@@ -35,9 +39,11 @@
       Just provide the dict and nothing else in your response, please. 
     """
     d = castigate_until_values_are(question=question, value_description='a color', max_retries=5)
     print(d)
     
     {'AAPL': 'white', 'MSFT': 'red', 'GOOGL': 'green'}
 
+See [examples](https://github.com/microprediction/chattychattybangbang/tree/main/examples) for presidential poetry appreciation, etc. 
+
 ### Article
 See [Reliably getting answers out of chatgpt](https://medium.com/@mike.roweprediger/reliably-getting-answers-out-of-chatgpt-by-forcing-it-to-qa-itself-feb1f56782b9) on medium. Thanks to Michael Rowe.
```

### Comparing `chattychattybangbang-0.0.5/chattychattybangbang.egg-info/SOURCES.txt` & `chattychattybangbang-0.0.6/chattychattybangbang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.5/setup.py` & `chattychattybangbang-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="chattychattybangbang",
-    version="0.0.5",
+    version="0.0.6",
     description="chat utilities",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/chattychattybangbang/chattychattybangbang",
     author="chattychattybangbang",
     author_email="pcotton@intechinvestments.com",
     license="MIT",
```

