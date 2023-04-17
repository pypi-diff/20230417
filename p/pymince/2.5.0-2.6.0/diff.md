# Comparing `tmp/pymince-2.5.0.tar.gz` & `tmp/pymince-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymince-2.5.0.tar", last modified: Fri Feb 17 14:52:02 2023, max compression
+gzip compressed data, was "pymince-2.6.0.tar", last modified: Mon Apr 17 09:52:29 2023, max compression
```

## Comparing `pymince-2.5.0.tar` & `pymince-2.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:52:02.444614 pymince-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-17 14:51:46.000000 pymince-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36445 2023-02-17 14:52:02.444614 pymince-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35622 2023-02-17 14:51:46.000000 pymince-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:52:02.444614 pymince-2.5.0/pymince/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/std.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-17 14:51:46.000000 pymince-2.5.0/pymince/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:52:02.444614 pymince-2.5.0/pymince.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36445 2023-02-17 14:52:02.000000 pymince-2.5.0/pymince.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-02-17 14:52:02.000000 pymince-2.5.0/pymince.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:52:02.000000 pymince-2.5.0/pymince.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:52:02.000000 pymince-2.5.0/pymince.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-17 14:52:02.000000 pymince-2.5.0/pymince.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-02-17 14:51:46.000000 pymince-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 14:52:02.444614 pymince-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-02-17 14:51:46.000000 pymince-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:29.263609 pymince-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-17 09:52:11.000000 pymince-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37583 2023-04-17 09:52:29.263609 pymince-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36760 2023-04-17 09:52:11.000000 pymince-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:29.259609 pymince-2.6.0/pymince/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 09:52:11.000000 pymince-2.6.0/pymince/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:29.263609 pymince-2.6.0/pymince.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37583 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 09:52:29.000000 pymince-2.6.0/pymince.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-17 09:52:11.000000 pymince-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:52:29.263609 pymince-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 09:52:11.000000 pymince-2.6.0/setup.py
```

### Comparing `pymince-2.5.0/LICENSE` & `pymince-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/PKG-INFO` & `pymince-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymince
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python shredded utilities
 Home-page: https://github.com/rmoralespp/pymince
 Author: rmoralespp
 Author-email: rmoralespp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,21 +52,21 @@
 ### Usage
 | PyModules  | Tools  |
 | :--------  | :----- |
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
-| **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
+| **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
-| **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*has_only_one*](#has_only_one), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
-| **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
+| **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
 
 ##### fibonacci
 ```
@@ -342,14 +342,24 @@
 :param bool cleaning:
     If "cleaning" is True and a directory already exists,
     this directory and the files contained in it will be deleted.
 
     If "cleaning" is True and a file already exists,
     this file will be deleted.
 ```
+##### get_valid_filename
+```
+get_valid_filename(s)
+
+Returns a valid filename for the given string.
+
+- Remove leading/trailing spaces
+- Change spaces to underscores
+- Remove anything that is not an alphanumeric, dash, underscore, or dot
+```
 ##### is_empty_directory
 ```
 is_empty_directory(path)
 
 Check if the given path is an empty directory.
 ```
 ##### match_from_zip
@@ -648,30 +658,14 @@
 
 Examples:
     from pymince.iterator import grouper
 
     groups = grouper([1, 2, 3, 4, 5], 2)
     list(list(g) for g in groups) # --> [[1, 2], [3, 4], [5]]
 ```
-##### has_only_one
-```
-has_only_one(iterable)
-
-Check if given iterable has only one element.
-
-:param iterable:
-:rtype: bool
-
-Examples:
-    from pymince.iterator import has_only_one
-
-    has_only_one([1]) # --> True
-    has_only_one([1, 2]) # --> False
-    has_only_one([]) # --> False
-```
 ##### ibool
 ```
 ibool(iterable)
 
 Iterator class supporting ´__bool__´.
 
 Examples:
@@ -740,14 +734,30 @@
 mul(iterable, start=1)
 
 Return the multiplication of a 'start' value (default: 1)
 plus an iterable of numbers.
 
 When the iterable is empty, return the start value.
 ```
+##### only_one
+```
+only_one(iterable)
+
+Check if given iterable has only one element.
+
+:param iterable:
+:rtype: bool
+
+Examples:
+    from pymince.iterator import only_one
+
+    only_one([1]) # --> True
+    only_one([1, 2]) # --> False
+    only_one([]) # --> False
+```
 ##### pad_end
 ```
 pad_end(iterable, length, fill_value=None)
 
 The function adds "fill_value" at the finishing of the iterable,
 until it reaches the specified length.
 If the value of the "length" param is less than the length of
@@ -782,14 +792,27 @@
  Examples:
     from pymince.iterator import pad_start
 
     pad_start(("a", "b"), 3, fill_value="1") # --> "1" "a" "b"
     pad_start(("a", "b"), 3) # --> None "a" "b"
     pad_start(("a", "b", "c"), 3) # --> "a" "b" "c"
 ```
+##### partition
+```
+partition(predicate, iterable)
+
+Split the iterable into two lists, based on the boolean return-value
+of the predicate.
+
+Examples:
+    from pymince.iterator import partition
+
+    is_odd = lambda x: x % 2 != 0
+    even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
+```
 ##### replacer
 ```
 replacer(iterable, matcher, new_value, count=-1)
 
 Make a generator that yields all occurrences of the old "iterable"
 replaced by "new_value".
 
@@ -925,14 +948,28 @@
 Dump JSON into the zip archive under the name arcname.
 
 Examples:
     from pymince.json import dump_into_zip
 
     dump_into_zip("archive.zip", "foo.json", {"key": "value"})
 ```
+##### idump_into
+```
+idump_into(filename, iterable, encoding='utf-8', **kwargs)
+
+Dump an iterable incrementally into a JSON file
+using the "utf-8" encoding.
+The result will always be an array with the elements of the iterable.
+
+Examples:
+    from pymince.json import idump_into
+
+    it = iter([{"key": "foo"}, {"key": "bar"}])
+    dump_into("foo.json", it)
+```
 ##### load_from
 ```
 load_from(filename, encoding='utf-8')
 
 Load JSON from a file using "utf-8" encoding.
 
 Examples:
@@ -982,15 +1019,15 @@
     {"timestamp":"2022-06-17 18:37:48,789","level":"DEBUG","payload":{"string":"value1","number":1}}
     {"timestamp":"2022-06-17 18:37:48,789","level":"DEBUG","payload":{"string":"value2","number":2}}
 ```
 ##### timed_block
 ```
 timed_block(name, logger=None)
 
-Logger the duration of the handled context.
+Log the duration of the handled context.
 
 Examples:
     import logging
     from pymince.logging import timed_block
 
     logging.basicConfig(level=logging.DEBUG)
     with timed_block("sleeping"):
@@ -1203,14 +1240,20 @@
     mapping = (("abc", "123"), ("def", "456"))
     replace = multireplacer(mapping)
 
     replace("...def...")  # --> "...456..."
     replace("...abc...")  # --> "...123..."
     replace("...abc...def...")  # --> "...123...456..."
 ```
+##### normalize_newlines
+```
+normalize_newlines(s)
+
+Normalize CRLF and CR newlines to just LF.
+```
 ##### remove_decimal_zeros
 ```
 remove_decimal_zeros(value, decimal_sep='.', min_decimals=None)
 
 Removes non-significant decimal zeros from a formatted text number.
 
 Examples:
```

### Comparing `pymince-2.5.0/README.md` & `pymince-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 ### Usage
 | PyModules  | Tools  |
 | :--------  | :----- |
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
-| **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
+| **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
-| **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*has_only_one*](#has_only_one), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
-| **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
+| **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
 
 ##### fibonacci
 ```
@@ -319,14 +319,24 @@
 :param bool cleaning:
     If "cleaning" is True and a directory already exists,
     this directory and the files contained in it will be deleted.
 
     If "cleaning" is True and a file already exists,
     this file will be deleted.
 ```
+##### get_valid_filename
+```
+get_valid_filename(s)
+
+Returns a valid filename for the given string.
+
+- Remove leading/trailing spaces
+- Change spaces to underscores
+- Remove anything that is not an alphanumeric, dash, underscore, or dot
+```
 ##### is_empty_directory
 ```
 is_empty_directory(path)
 
 Check if the given path is an empty directory.
 ```
 ##### match_from_zip
@@ -625,30 +635,14 @@
 
 Examples:
     from pymince.iterator import grouper
 
     groups = grouper([1, 2, 3, 4, 5], 2)
     list(list(g) for g in groups) # --> [[1, 2], [3, 4], [5]]
 ```
-##### has_only_one
-```
-has_only_one(iterable)
-
-Check if given iterable has only one element.
-
-:param iterable:
-:rtype: bool
-
-Examples:
-    from pymince.iterator import has_only_one
-
-    has_only_one([1]) # --> True
-    has_only_one([1, 2]) # --> False
-    has_only_one([]) # --> False
-```
 ##### ibool
 ```
 ibool(iterable)
 
 Iterator class supporting ´__bool__´.
 
 Examples:
@@ -717,14 +711,30 @@
 mul(iterable, start=1)
 
 Return the multiplication of a 'start' value (default: 1)
 plus an iterable of numbers.
 
 When the iterable is empty, return the start value.
 ```
+##### only_one
+```
+only_one(iterable)
+
+Check if given iterable has only one element.
+
+:param iterable:
+:rtype: bool
+
+Examples:
+    from pymince.iterator import only_one
+
+    only_one([1]) # --> True
+    only_one([1, 2]) # --> False
+    only_one([]) # --> False
+```
 ##### pad_end
 ```
 pad_end(iterable, length, fill_value=None)
 
 The function adds "fill_value" at the finishing of the iterable,
 until it reaches the specified length.
 If the value of the "length" param is less than the length of
@@ -759,14 +769,27 @@
  Examples:
     from pymince.iterator import pad_start
 
     pad_start(("a", "b"), 3, fill_value="1") # --> "1" "a" "b"
     pad_start(("a", "b"), 3) # --> None "a" "b"
     pad_start(("a", "b", "c"), 3) # --> "a" "b" "c"
 ```
+##### partition
+```
+partition(predicate, iterable)
+
+Split the iterable into two lists, based on the boolean return-value
+of the predicate.
+
+Examples:
+    from pymince.iterator import partition
+
+    is_odd = lambda x: x % 2 != 0
+    even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
+```
 ##### replacer
 ```
 replacer(iterable, matcher, new_value, count=-1)
 
 Make a generator that yields all occurrences of the old "iterable"
 replaced by "new_value".
 
@@ -902,14 +925,28 @@
 Dump JSON into the zip archive under the name arcname.
 
 Examples:
     from pymince.json import dump_into_zip
 
     dump_into_zip("archive.zip", "foo.json", {"key": "value"})
 ```
+##### idump_into
+```
+idump_into(filename, iterable, encoding='utf-8', **kwargs)
+
+Dump an iterable incrementally into a JSON file
+using the "utf-8" encoding.
+The result will always be an array with the elements of the iterable.
+
+Examples:
+    from pymince.json import idump_into
+
+    it = iter([{"key": "foo"}, {"key": "bar"}])
+    dump_into("foo.json", it)
+```
 ##### load_from
 ```
 load_from(filename, encoding='utf-8')
 
 Load JSON from a file using "utf-8" encoding.
 
 Examples:
@@ -959,15 +996,15 @@
     {"timestamp":"2022-06-17 18:37:48,789","level":"DEBUG","payload":{"string":"value1","number":1}}
     {"timestamp":"2022-06-17 18:37:48,789","level":"DEBUG","payload":{"string":"value2","number":2}}
 ```
 ##### timed_block
 ```
 timed_block(name, logger=None)
 
-Logger the duration of the handled context.
+Log the duration of the handled context.
 
 Examples:
     import logging
     from pymince.logging import timed_block
 
     logging.basicConfig(level=logging.DEBUG)
     with timed_block("sleeping"):
@@ -1180,14 +1217,20 @@
     mapping = (("abc", "123"), ("def", "456"))
     replace = multireplacer(mapping)
 
     replace("...def...")  # --> "...456..."
     replace("...abc...")  # --> "...123..."
     replace("...abc...def...")  # --> "...123...456..."
 ```
+##### normalize_newlines
+```
+normalize_newlines(s)
+
+Normalize CRLF and CR newlines to just LF.
+```
 ##### remove_decimal_zeros
 ```
 remove_decimal_zeros(value, decimal_sep='.', min_decimals=None)
 
 Removes non-significant decimal zeros from a formatted text number.
 
 Examples:
```

### Comparing `pymince-2.5.0/pymince/algorithm.py` & `pymince-2.6.0/pymince/algorithm.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince/boolean.py` & `pymince-2.6.0/pymince/boolean.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince/dates.py` & `pymince-2.6.0/pymince/dates.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince/dictionary.py` & `pymince-2.6.0/pymince/dictionary.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince/file.py` & `pymince-2.6.0/pymince/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,7 +111,22 @@
         decompress("/foo/src.txt.gz", "/baz/dst.txt")  # --> "/baz/dst.txt"
     """
 
     with gzip.open(src_path) as src, open(dst_path, mode="wb") as dst:
         lines = iter(functools.partial(src.read, size), b"")
         dst.writelines(lines)
     return dst_path
+
+
+def get_valid_filename(s):
+    """
+    Returns a valid filename for the given string.
+
+    - Remove leading/trailing spaces
+    - Change spaces to underscores
+    - Remove anything that is not an alphanumeric, dash, underscore, or dot
+    """
+
+    filename = re.sub(r"(?u)[^-\w.]", "", s.strip().replace(" ", "_"))
+    if filename in ("", ".", ".."):
+        raise ValueError(filename)
+    return filename
```

### Comparing `pymince-2.5.0/pymince/functional.py` & `pymince-2.6.0/pymince/functional.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince/iterator.py` & `pymince-2.6.0/pymince/iterator.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         from pymince.iterator import all_equal
 
         all_equal([1, 1]) # --> True
         all_equal([1, 2]) # --> False
     """
 
     grouped = itertools.groupby(iterable, key=key)
-    return has_only_one(grouped)
+    return only_one(grouped)
 
 
 def all_distinct(iterable, key=None):
     """
     Check if all the elements of a key-based iterable are distinct.
 
     :param iterable:
@@ -200,36 +200,57 @@
         from pymince.iterator import all_distinct
 
         all_distinct([1, 1]) # --> False
         all_distinct([1, 2]) # --> True
     """
 
     grouped = itertools.groupby(iterable, key=key)
-    return all(has_only_one(group) for _, group in grouped)
+    return all(only_one(group) for _, group in grouped)
 
 
-def has_only_one(iterable):
+def only_one(iterable):
     """
     Check if given iterable has only one element.
 
     :param iterable:
     :rtype: bool
 
     Examples:
-        from pymince.iterator import has_only_one
+        from pymince.iterator import only_one
 
-        has_only_one([1]) # --> True
-        has_only_one([1, 2]) # --> False
-        has_only_one([]) # --> False
+        only_one([1]) # --> True
+        only_one([1, 2]) # --> False
+        only_one([]) # --> False
     """
 
     it = iter(iterable)
     return next(it, empty) is not empty and next(it, empty) is empty
 
 
+def partition(predicate, iterable):
+    """
+    Split the iterable into two lists, based on the boolean return-value
+    of the predicate.
+
+    Examples:
+        from pymince.iterator import partition
+
+        is_odd = lambda x: x % 2 != 0
+        even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
+    """
+
+    if predicate is None:
+        predicate = bool
+
+    results = ([], [])
+    for n in iter(iterable):
+        results[predicate(n)].append(n)
+    return results
+
+
 def splitter(iterable, sep, key=None, maxsplit=-1, container=None):
     """
     Splits an iterable based on a separator.
     A separator will never appear in the output.
 
     :param iterable:
     :param sep: The delimiter to split the iterable.
```

### Comparing `pymince-2.5.0/pymince/json.py` & `pymince-2.6.0/pymince/json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 """Useful functions for working with JSONs."""
+
 import csv
 import dataclasses
 import datetime
 import decimal
 import functools
 import itertools
 import json
 import operator
+import textwrap
 import uuid
 import zipfile
 
 dumps = functools.partial(json.dumps, ensure_ascii=False)
 dump = functools.partial(json.dump, ensure_ascii=False)
 ENCODING = "utf-8"
 
@@ -112,14 +114,47 @@
 
         data = itertools.islice(read(), start, stop)
         pool = tuple(data)
 
     dump_into(json_path, pool, encoding=encoding, **kwargs)
 
 
+def idump_into(filename, iterable, encoding=ENCODING, **kwargs):
+    """
+    Dump an iterable incrementally into a JSON file
+    using the "utf-8" encoding.
+    The result will always be an array with the elements of the iterable.
+
+    Examples:
+        from pymince.json import idump_into
+
+        it = iter([{"key": "foo"}, {"key": "bar"}])
+        dump_into("foo.json", it)
+    """
+
+    def worker(items):
+        encode = functools.partial(dumps, **kwargs)
+        indent = kwargs.get("indent")
+        prefix = " " * indent if indent else ""
+        yield "[\n"
+        obj = next(items, None)
+        if obj is not None:
+            yield textwrap.indent(encode(obj), prefix)
+        for obj in items:
+            yield ",\n"
+            yield textwrap.indent(encode(obj), prefix)
+
+        yield "\n"
+        yield "]"
+
+    it = iter(iterable)
+    with open(filename, mode="w", encoding=encoding) as f:
+        f.writelines(worker(it))
+
+
 class JSONEncoder(json.JSONEncoder):
     """
     JSON encoder that handles additional types compared
     to `json.JSONEncoder`
 
     - `datetime` and `date` are serialized to strings according to the isoformat.
     - `decimal.Decimal` is serialized to a string.
```

### Comparing `pymince-2.5.0/pymince/logging.py` & `pymince-2.6.0/pymince/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import time
 
 
 @contextlib.contextmanager
 def timed_block(name, logger=None):
     """
-    Logger the duration of the handled context.
+    Log the duration of the handled context.
 
     Examples:
         import logging
         from pymince.logging import timed_block
 
         logging.basicConfig(level=logging.DEBUG)
         with timed_block("sleeping"):
```

### Comparing `pymince-2.5.0/pymince/std.py` & `pymince-2.6.0/pymince/std.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince/text.py` & `pymince-2.6.0/pymince/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 _int_regexp_any = re.compile(r"^[-+]?[1-9]\d*\.?[0]*$")
 _int_regexp_pos = re.compile(r"^[+]?[1-9]\d*\.?[0]*$")
 _int_regexp_neg = re.compile(r"^-[1-9]\d*\.?[0]*$")
 _bin_regexp_not = re.compile(r"[^01]")
 _percentage_regexp = re.compile(r"^(?:0|[1-9]\d*)(?:\.\d+)?(?:\s)?%$")
 _email_address_regexp = re.compile(r"^\S+@\S+$")
 _roman_regex = re.compile(r"^M{0,3}(CM|CD|D?C{0,3})(XC|XL|L?X{0,3})(IX|IV|V?I{0,3})$")
+_re_newlines = re.compile(r"\r\n|\r")  # used in normalize_newlines
 
 
 def get_random_string(length, alphabet=string.ascii_letters):
     """Generate random string."""
 
     return "".join(random.choice(alphabet) for _ in range(length))
 
@@ -33,14 +34,20 @@
     Generate a cryptographically secure random string.
     Useful for creating temporary passwords.
     """
 
     return "".join(secrets.choice(alphabet) for _ in range(length))
 
 
+def normalize_newlines(s):
+    """Normalize CRLF and CR newlines to just LF."""
+
+    return _re_newlines.sub("\n", s)
+
+
 def remove_number_commas(s):
     """
     Removes commas from a formatted text number having commas
     as group separator.
 
     :param str s:
     :rtype str
```

### Comparing `pymince-2.5.0/pymince/warnings.py` & `pymince-2.6.0/pymince/warnings.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince/xml.py` & `pymince-2.6.0/pymince/xml.py`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/pymince.egg-info/PKG-INFO` & `pymince-2.6.0/pymince.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymince
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python shredded utilities
 Home-page: https://github.com/rmoralespp/pymince
 Author: rmoralespp
 Author-email: rmoralespp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -52,21 +52,21 @@
 ### Usage
 | PyModules  | Tools  |
 | :--------  | :----- |
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict)|
-| **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
+| **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
-| **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*has_only_one*](#has_only_one), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
-| **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
+| **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
 
 ##### fibonacci
 ```
@@ -342,14 +342,24 @@
 :param bool cleaning:
     If "cleaning" is True and a directory already exists,
     this directory and the files contained in it will be deleted.
 
     If "cleaning" is True and a file already exists,
     this file will be deleted.
 ```
+##### get_valid_filename
+```
+get_valid_filename(s)
+
+Returns a valid filename for the given string.
+
+- Remove leading/trailing spaces
+- Change spaces to underscores
+- Remove anything that is not an alphanumeric, dash, underscore, or dot
+```
 ##### is_empty_directory
 ```
 is_empty_directory(path)
 
 Check if the given path is an empty directory.
 ```
 ##### match_from_zip
@@ -648,30 +658,14 @@
 
 Examples:
     from pymince.iterator import grouper
 
     groups = grouper([1, 2, 3, 4, 5], 2)
     list(list(g) for g in groups) # --> [[1, 2], [3, 4], [5]]
 ```
-##### has_only_one
-```
-has_only_one(iterable)
-
-Check if given iterable has only one element.
-
-:param iterable:
-:rtype: bool
-
-Examples:
-    from pymince.iterator import has_only_one
-
-    has_only_one([1]) # --> True
-    has_only_one([1, 2]) # --> False
-    has_only_one([]) # --> False
-```
 ##### ibool
 ```
 ibool(iterable)
 
 Iterator class supporting ´__bool__´.
 
 Examples:
@@ -740,14 +734,30 @@
 mul(iterable, start=1)
 
 Return the multiplication of a 'start' value (default: 1)
 plus an iterable of numbers.
 
 When the iterable is empty, return the start value.
 ```
+##### only_one
+```
+only_one(iterable)
+
+Check if given iterable has only one element.
+
+:param iterable:
+:rtype: bool
+
+Examples:
+    from pymince.iterator import only_one
+
+    only_one([1]) # --> True
+    only_one([1, 2]) # --> False
+    only_one([]) # --> False
+```
 ##### pad_end
 ```
 pad_end(iterable, length, fill_value=None)
 
 The function adds "fill_value" at the finishing of the iterable,
 until it reaches the specified length.
 If the value of the "length" param is less than the length of
@@ -782,14 +792,27 @@
  Examples:
     from pymince.iterator import pad_start
 
     pad_start(("a", "b"), 3, fill_value="1") # --> "1" "a" "b"
     pad_start(("a", "b"), 3) # --> None "a" "b"
     pad_start(("a", "b", "c"), 3) # --> "a" "b" "c"
 ```
+##### partition
+```
+partition(predicate, iterable)
+
+Split the iterable into two lists, based on the boolean return-value
+of the predicate.
+
+Examples:
+    from pymince.iterator import partition
+
+    is_odd = lambda x: x % 2 != 0
+    even_items, odd_items = partition(is_odd, range(10))  # ([0, 2, 4, 6, 8], [1, 3, 5, 7, 9])
+```
 ##### replacer
 ```
 replacer(iterable, matcher, new_value, count=-1)
 
 Make a generator that yields all occurrences of the old "iterable"
 replaced by "new_value".
 
@@ -925,14 +948,28 @@
 Dump JSON into the zip archive under the name arcname.
 
 Examples:
     from pymince.json import dump_into_zip
 
     dump_into_zip("archive.zip", "foo.json", {"key": "value"})
 ```
+##### idump_into
+```
+idump_into(filename, iterable, encoding='utf-8', **kwargs)
+
+Dump an iterable incrementally into a JSON file
+using the "utf-8" encoding.
+The result will always be an array with the elements of the iterable.
+
+Examples:
+    from pymince.json import idump_into
+
+    it = iter([{"key": "foo"}, {"key": "bar"}])
+    dump_into("foo.json", it)
+```
 ##### load_from
 ```
 load_from(filename, encoding='utf-8')
 
 Load JSON from a file using "utf-8" encoding.
 
 Examples:
@@ -982,15 +1019,15 @@
     {"timestamp":"2022-06-17 18:37:48,789","level":"DEBUG","payload":{"string":"value1","number":1}}
     {"timestamp":"2022-06-17 18:37:48,789","level":"DEBUG","payload":{"string":"value2","number":2}}
 ```
 ##### timed_block
 ```
 timed_block(name, logger=None)
 
-Logger the duration of the handled context.
+Log the duration of the handled context.
 
 Examples:
     import logging
     from pymince.logging import timed_block
 
     logging.basicConfig(level=logging.DEBUG)
     with timed_block("sleeping"):
@@ -1203,14 +1240,20 @@
     mapping = (("abc", "123"), ("def", "456"))
     replace = multireplacer(mapping)
 
     replace("...def...")  # --> "...456..."
     replace("...abc...")  # --> "...123..."
     replace("...abc...def...")  # --> "...123...456..."
 ```
+##### normalize_newlines
+```
+normalize_newlines(s)
+
+Normalize CRLF and CR newlines to just LF.
+```
 ##### remove_decimal_zeros
 ```
 remove_decimal_zeros(value, decimal_sep='.', min_decimals=None)
 
 Removes non-significant decimal zeros from a formatted text number.
 
 Examples:
```

### Comparing `pymince-2.5.0/pyproject.toml` & `pymince-2.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymince-2.5.0/setup.py` & `pymince-2.6.0/setup.py`

 * *Files identical despite different names*

