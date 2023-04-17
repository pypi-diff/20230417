# Comparing `tmp/shunting-yard-1.0.7.tar.gz` & `tmp/shunting-yard-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shunting-yard-1.0.7.tar", last modified: Mon Mar 13 12:52:40 2023, max compression
+gzip compressed data, was "shunting-yard-1.0.8.tar", last modified: Mon Apr 17 09:00:10 2023, max compression
```

## Comparing `shunting-yard-1.0.7.tar` & `shunting-yard-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/
--rw-rw-rw-   0        0        0     1097 2023-02-28 15:01:14.000000 shunting-yard-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3634 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3257 2023-03-09 09:38:54.000000 shunting-yard-1.0.7/README.md
--rw-rw-rw-   0        0        0      110 2023-02-28 15:21:46.000000 shunting-yard-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-03-13 12:51:34.000000 shunting-yard-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/shunting_yard/
--rw-rw-rw-   0        0        0      898 2023-03-02 08:03:42.000000 shunting-yard-1.0.7/shunting_yard/__init__.py
--rw-rw-rw-   0        0        0      517 2023-03-13 08:45:42.000000 shunting-yard-1.0.7/shunting_yard/__main__.py
--rw-rw-rw-   0        0        0      398 2023-03-13 12:44:14.000000 shunting-yard-1.0.7/shunting_yard/constants.py
--rw-rw-rw-   0        0        0     3288 2023-03-13 08:41:38.000000 shunting-yard-1.0.7/shunting_yard/rpn.py
--rw-rw-rw-   0        0        0     4385 2023-03-13 12:50:44.000000 shunting-yard-1.0.7/shunting_yard/shunting_yard.py
--rw-rw-rw-   0        0        0     1616 2023-03-13 12:48:44.000000 shunting-yard-1.0.7/shunting_yard/tokenize.py
-drwxrwxrwx   0        0        0        0 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/shunting_yard.egg-info/
--rw-rw-rw-   0        0        0     3634 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/shunting_yard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/shunting_yard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/shunting_yard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/shunting_yard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-13 12:52:40.000000 shunting-yard-1.0.7/tests/
--rw-rw-rw-   0        0        0     1879 2023-03-01 14:58:52.000000 shunting-yard-1.0.7/tests/test_rpn.py
--rw-rw-rw-   0        0        0     3081 2023-03-13 12:45:18.000000 shunting-yard-1.0.7/tests/test_shunting_yard.py
--rw-rw-rw-   0        0        0     3825 2023-03-13 12:50:12.000000 shunting-yard-1.0.7/tests/test_tokenize.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.137452 shunting-yard-1.0.8/
+-rw-rw-rw-   0        0        0     1097 2023-02-28 14:01:14.000000 shunting-yard-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3870 2023-04-17 09:00:10.138452 shunting-yard-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3493 2023-04-17 08:55:23.000000 shunting-yard-1.0.8/README.md
+-rw-rw-rw-   0        0        0      110 2023-02-28 14:21:46.000000 shunting-yard-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-17 09:00:10.140452 shunting-yard-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-04-17 08:51:19.000000 shunting-yard-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.119933 shunting-yard-1.0.8/shunting_yard/
+-rw-rw-rw-   0        0        0      898 2023-03-02 07:03:42.000000 shunting-yard-1.0.8/shunting_yard/__init__.py
+-rw-rw-rw-   0        0        0      517 2023-03-13 07:45:42.000000 shunting-yard-1.0.8/shunting_yard/__main__.py
+-rw-rw-rw-   0        0        0      398 2023-03-13 11:44:14.000000 shunting-yard-1.0.8/shunting_yard/constants.py
+-rw-rw-rw-   0        0        0     3288 2023-04-17 08:39:24.000000 shunting-yard-1.0.8/shunting_yard/rpn.py
+-rw-rw-rw-   0        0        0     4360 2023-04-17 08:46:39.000000 shunting-yard-1.0.8/shunting_yard/shunting_yard.py
+-rw-rw-rw-   0        0        0     2653 2023-04-17 08:51:05.000000 shunting-yard-1.0.8/shunting_yard/tokenize.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.131453 shunting-yard-1.0.8/shunting_yard.egg-info/
+-rw-rw-rw-   0        0        0     3870 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 09:00:10.000000 shunting-yard-1.0.8/shunting_yard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 09:00:10.136452 shunting-yard-1.0.8/tests/
+-rw-rw-rw-   0        0        0     1879 2023-03-01 13:58:52.000000 shunting-yard-1.0.8/tests/test_rpn.py
+-rw-rw-rw-   0        0        0     3081 2023-04-17 08:46:41.000000 shunting-yard-1.0.8/tests/test_shunting_yard.py
+-rw-rw-rw-   0        0        0     6926 2023-04-17 08:56:27.000000 shunting-yard-1.0.8/tests/test_tokenize.py
```

### Comparing `shunting-yard-1.0.7/LICENSE` & `shunting-yard-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.7/PKG-INFO` & `shunting-yard-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: shunting-yard
-Version: 1.0.7
-Summary: Compute any math expression
-Home-page: https://www.github.com/charon25/ShuntingYard
-Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.7.tar.gz
-Author: Paul 'charon25' Kern
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shuting-yard algorithm
 
 This repo is a Python (>= 3.9) module containing an implementation of the [Shunting-yard algorithm](https://en.wikipedia.org/wiki/Shunting_yard_algorithm), which converts any "regular" mathematical expression into its [Reverse Polish Notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation) equivalent, and then can evaluate it.
 
 # Installation
 
 To install it, just run :
@@ -62,15 +50,15 @@
 ```
 
 ## Allowed functions
 
 By default, the module can process the 5 basic operations (`+`, `-`, `*`, `/`, `^`) as well as those functions :
  - sqrt
  - sin, cos, tan
- - min, max (with 2 arguments)
+ - min, max (with 2, 3 or 4 arguments)
  - abs
 
 As well as the constants `pi` and `e`.
 
 These operations and functions can be mixed however you want.
 
 Furthermore, you can add more functions with the optional parameters `additional_functions` of the `sy.compute` function. It should be a dictionary whose keys are string, and values are a tuple containing first the number of expected argument to the function, and then the function itself. For example :
@@ -88,14 +76,24 @@
 
 The `sy.compute` (and `sy.shuting_yard`) also have extra parameters :
  - `case_sensitive` (bool, defaults to `True`) : if `True`, will consider `sin` and `SIN` different functions.
  - `variable` (str, optional) : if defined, will consider any token matching it as a number. This is useful in expression such as `min(x, 1)` to get `x` to behave as a number.
 
 ## Additional features
 
+### Implicit multiplication
+
+This program supports implicit multiplication (when the `*` symbol is omitted). They can have multiple forms, such as :
+- `(1+2)(2+3)`
+- `2sin(pi)`
+- `(1+2)3`
+- `sin(pi)10`
+
+### Functions
+
 Instead of just calling the `sy.compute` function, you can break it into its parts :
  - `sy.shunting_yard` will return the RPN equivalent expression of the given mathematical expression ;
  - `sy.compute_rpn` will use this expression and compute its value (use the `additional_functions` parameters here).
 
 Furthermore, you can just use the `sy.tokenize` function to transform a mathematical expression into its base components (returns a generator).
 
 Examples :
```

### Comparing `shunting-yard-1.0.7/README.md` & `shunting-yard-1.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: shunting-yard
+Version: 1.0.8
+Summary: Compute any math expression
+Home-page: https://www.github.com/charon25/ShuntingYard
+Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.8.tar.gz
+Author: Paul 'charon25' Kern
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Shuting-yard algorithm
 
 This repo is a Python (>= 3.9) module containing an implementation of the [Shunting-yard algorithm](https://en.wikipedia.org/wiki/Shunting_yard_algorithm), which converts any "regular" mathematical expression into its [Reverse Polish Notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation) equivalent, and then can evaluate it.
 
 # Installation
 
 To install it, just run :
@@ -50,15 +62,15 @@
 ```
 
 ## Allowed functions
 
 By default, the module can process the 5 basic operations (`+`, `-`, `*`, `/`, `^`) as well as those functions :
  - sqrt
  - sin, cos, tan
- - min, max (with 2 arguments)
+ - min, max (with 2, 3 or 4 arguments)
  - abs
 
 As well as the constants `pi` and `e`.
 
 These operations and functions can be mixed however you want.
 
 Furthermore, you can add more functions with the optional parameters `additional_functions` of the `sy.compute` function. It should be a dictionary whose keys are string, and values are a tuple containing first the number of expected argument to the function, and then the function itself. For example :
@@ -76,14 +88,24 @@
 
 The `sy.compute` (and `sy.shuting_yard`) also have extra parameters :
  - `case_sensitive` (bool, defaults to `True`) : if `True`, will consider `sin` and `SIN` different functions.
  - `variable` (str, optional) : if defined, will consider any token matching it as a number. This is useful in expression such as `min(x, 1)` to get `x` to behave as a number.
 
 ## Additional features
 
+### Implicit multiplication
+
+This program supports implicit multiplication (when the `*` symbol is omitted). They can have multiple forms, such as :
+- `(1+2)(2+3)`
+- `2sin(pi)`
+- `(1+2)3`
+- `sin(pi)10`
+
+### Functions
+
 Instead of just calling the `sy.compute` function, you can break it into its parts :
  - `sy.shunting_yard` will return the RPN equivalent expression of the given mathematical expression ;
  - `sy.compute_rpn` will use this expression and compute its value (use the `additional_functions` parameters here).
 
 Furthermore, you can just use the `sy.tokenize` function to transform a mathematical expression into its base components (returns a generator).
 
 Examples :
```

### Comparing `shunting-yard-1.0.7/setup.py` & `shunting-yard-1.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fi:
     long_description = fi.read()
 
 setuptools.setup(
 	name="shunting-yard",
-	version="1.0.7",
+	version="1.0.8",
 	author="Paul 'charon25' Kern",
 	description="Compute any math expression",
 	long_description=long_description,
     long_description_content_type='text/markdown',
 	python_requires=">=3.9",
 	url="https://www.github.com/charon25/ShuntingYard",
 	license="MIT",
 	packages=['shunting_yard'],
-	download_url="https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.7.tar.gz"
+	download_url="https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.8.tar.gz"
 )
```

### Comparing `shunting-yard-1.0.7/shunting_yard/__init__.py` & `shunting-yard-1.0.8/shunting_yard/__init__.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.7/shunting_yard/__main__.py` & `shunting-yard-1.0.8/shunting_yard/__main__.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.7/shunting_yard/rpn.py` & `shunting-yard-1.0.8/shunting_yard/rpn.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import math
 from operator import add, mul, neg, pos, sub, truediv
 from typing import Any, Callable, Optional, Union
+import math
 
 from shunting_yard.constants import NUMBER_CHARS
 
 
 class WrongExpressionError(Exception):
     pass
```

### Comparing `shunting-yard-1.0.7/shunting_yard/shunting_yard.py` & `shunting-yard-1.0.8/shunting_yard/shunting_yard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from string import ascii_lowercase
-import math
 from enum import Enum
 from typing import Optional
+import math
+import re
 
 from shunting_yard.tokenize import tokenize
 from shunting_yard.constants import BASE_OPERATORS, NUMBER_CHARS, FUNCTION_CHARS, SEPARATORS, SEPARATORS_NO_CLOSING_BRACKET, UNARY_OPERATORS_SYMBOLS
 
 
 class MismatchedBracketsError(Exception):
     pass
```

### Comparing `shunting-yard-1.0.7/shunting_yard.egg-info/PKG-INFO` & `shunting-yard-1.0.8/shunting_yard.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shunting-yard
-Version: 1.0.7
+Version: 1.0.8
 Summary: Compute any math expression
 Home-page: https://www.github.com/charon25/ShuntingYard
-Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.7.tar.gz
+Download-URL: https://github.com/charon25/ShuntingYard/archive/refs/tags/v1.0.8.tar.gz
 Author: Paul 'charon25' Kern
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shuting-yard algorithm
@@ -62,15 +62,15 @@
 ```
 
 ## Allowed functions
 
 By default, the module can process the 5 basic operations (`+`, `-`, `*`, `/`, `^`) as well as those functions :
  - sqrt
  - sin, cos, tan
- - min, max (with 2 arguments)
+ - min, max (with 2, 3 or 4 arguments)
  - abs
 
 As well as the constants `pi` and `e`.
 
 These operations and functions can be mixed however you want.
 
 Furthermore, you can add more functions with the optional parameters `additional_functions` of the `sy.compute` function. It should be a dictionary whose keys are string, and values are a tuple containing first the number of expected argument to the function, and then the function itself. For example :
@@ -88,14 +88,24 @@
 
 The `sy.compute` (and `sy.shuting_yard`) also have extra parameters :
  - `case_sensitive` (bool, defaults to `True`) : if `True`, will consider `sin` and `SIN` different functions.
  - `variable` (str, optional) : if defined, will consider any token matching it as a number. This is useful in expression such as `min(x, 1)` to get `x` to behave as a number.
 
 ## Additional features
 
+### Implicit multiplication
+
+This program supports implicit multiplication (when the `*` symbol is omitted). They can have multiple forms, such as :
+- `(1+2)(2+3)`
+- `2sin(pi)`
+- `(1+2)3`
+- `sin(pi)10`
+
+### Functions
+
 Instead of just calling the `sy.compute` function, you can break it into its parts :
  - `sy.shunting_yard` will return the RPN equivalent expression of the given mathematical expression ;
  - `sy.compute_rpn` will use this expression and compute its value (use the `additional_functions` parameters here).
 
 Furthermore, you can just use the `sy.tokenize` function to transform a mathematical expression into its base components (returns a generator).
 
 Examples :
```

### Comparing `shunting-yard-1.0.7/tests/test_rpn.py` & `shunting-yard-1.0.8/tests/test_rpn.py`

 * *Files identical despite different names*

### Comparing `shunting-yard-1.0.7/tests/test_shunting_yard.py` & `shunting-yard-1.0.8/tests/test_shunting_yard.py`

 * *Files identical despite different names*

