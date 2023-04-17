# Comparing `tmp/UniTok-3.0.12.tar.gz` & `tmp/UniTok-3.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.0.12.tar", last modified: Tue Mar 28 09:44:29 2023, max compression
+gzip compressed data, was "UniTok-3.0.13.tar", last modified: Mon Apr 17 08:15:56 2023, max compression
```

## Comparing `UniTok-3.0.12.tar` & `UniTok-3.0.13.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-03-28 09:44:29.567077 UniTok-3.0.12/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6585 2023-03-28 09:44:29.566969 UniTok-3.0.12/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.0.12/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-03-28 09:44:29.563498 UniTok-3.0.12/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.0.12/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-03-28 09:44:29.564786 UniTok-3.0.12/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.0.12/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.0.12/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.0.12/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.0.12/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3525 2023-03-28 08:59:34.000000 UniTok-3.0.12/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.0.12/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4388 2023-03-28 09:39:29.000000 UniTok-3.0.12/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-03-28 09:44:29.566695 UniTok-3.0.12/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.0.12/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-03-26 10:24:07.000000 UniTok-3.0.12/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.0.12/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.0.12/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.0.12/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.0.12/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.0.12/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.0.12/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8664 2023-03-28 09:40:52.000000 UniTok-3.0.12/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6267 2023-03-28 08:56:34.000000 UniTok-3.0.12/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8273 2023-03-28 09:20:14.000000 UniTok-3.0.12/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-03-28 09:20:42.000000 UniTok-3.0.12/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-03-28 09:44:29.564108 UniTok-3.0.12/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6585 2023-03-28 09:44:29.000000 UniTok-3.0.12/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-03-28 09:44:29.000000 UniTok-3.0.12/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-03-28 09:44:29.000000 UniTok-3.0.12/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-03-28 09:44:29.000000 UniTok-3.0.12/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-03-28 09:44:29.000000 UniTok-3.0.12/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-03-28 09:44:29.567105 UniTok-3.0.12/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      725 2023-03-28 09:44:18.000000 UniTok-3.0.12/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.539966 UniTok-3.0.13/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6585 2023-04-17 08:15:56.539869 UniTok-3.0.13/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.0.13/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.536402 UniTok-3.0.13/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.0.13/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.537639 UniTok-3.0.13/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.0.13/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.0.13/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.0.13/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.0.13/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3519 2023-04-17 08:08:49.000000 UniTok-3.0.13/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.0.13/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4388 2023-03-28 09:39:29.000000 UniTok-3.0.13/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.539590 UniTok-3.0.13/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.0.13/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-03-26 10:24:07.000000 UniTok-3.0.13/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.0.13/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.0.13/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.0.13/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.0.13/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.0.13/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.0.13/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8664 2023-03-28 09:40:52.000000 UniTok-3.0.13/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6267 2023-03-28 08:56:34.000000 UniTok-3.0.13/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8382 2023-04-14 07:07:55.000000 UniTok-3.0.13/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-03-28 09:20:42.000000 UniTok-3.0.13/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-17 08:15:56.537038 UniTok-3.0.13/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6585 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-17 08:15:56.000000 UniTok-3.0.13/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-17 08:15:56.539996 UniTok-3.0.13/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      725 2023-04-17 08:09:02.000000 UniTok-3.0.13/setup.py
```

### Comparing `UniTok-3.0.12/PKG-INFO` & `UniTok-3.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.0.12
+Version: 3.0.13
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.0.12/README.md` & `UniTok-3.0.13/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/analysis/lengths.py` & `UniTok-3.0.13/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/analysis/plot.py` & `UniTok-3.0.13/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/column.py` & `UniTok-3.0.13/UniTok/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,8 +111,8 @@
             max_length=max_length,
             padding=padding,
         )
 
 
 class IndexColumn(Column):
     def __init__(self, name='index'):
-        super().__init__(name, tok=IdTok(name=name))
+        super().__init__(tok=IdTok(name=name))
```

### Comparing `UniTok-3.0.12/UniTok/meta.py` & `UniTok-3.0.13/UniTok/meta.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/tok/bert_tok.py` & `UniTok-3.0.13/UniTok/tok/bert_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/tok/number_tok.py` & `UniTok-3.0.13/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/tok/split_tok.py` & `UniTok-3.0.13/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/tok/tok.py` & `UniTok-3.0.13/UniTok/tok/tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/unidep.py` & `UniTok-3.0.13/UniTok/unidep.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/unitok.py` & `UniTok-3.0.13/UniTok/unitok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok/vocab.py` & `UniTok-3.0.13/UniTok/vocab.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,36 +188,40 @@
         self._counter = {}
         self._oov_token = oov_token or self._oov_token
         return self
 
     def trim(self, min_count=None, min_frequency=1):
         """
         trim vocab by min frequency
-        :return:
+        :return: trimmed tokens
         """
+        _trimmed = []
+
         if min_count is None:
             warnings.warn('vocab.min_frequency is deprecated, '
                           'use vocab.min_count instead (will be removed in 4.x version)', DeprecationWarning)
             min_count = min_frequency
 
         vocabs = []
         for index in self._counter:
             if self._counter[index] >= min_count:
                 vocabs.append(self.i2o[index])
+            else:
+                _trimmed.append(self.i2o[index])
 
         self.i2o = dict()
         self.o2i = dict()
 
         self.set_count_mode(False)
         if self.reserved_tokens is not None:
             self.reserve(self.reserved_tokens)
         self.extend(vocabs)
 
         self._stable_mode = True
-        return self
+        return _trimmed
 
     def summarize(self, base=10):
         """
         summarize vocab by frequency
         :param base: display base, default 10
         :return: counts of clustered bounds, e.g., { (1, 2): 100, (2, 3): 200, ... }
         """
```

### Comparing `UniTok-3.0.12/UniTok/vocabs.py` & `UniTok-3.0.13/UniTok/vocabs.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/UniTok.egg-info/PKG-INFO` & `UniTok-3.0.13/UniTok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.0.12
+Version: 3.0.13
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.0.12/UniTok.egg-info/SOURCES.txt` & `UniTok-3.0.13/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UniTok-3.0.12/setup.py` & `UniTok-3.0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='UniTok',
-    version='3.0.12',
+    version='3.0.13',
     keywords=['token', 'tokenizer', 'bert'],
     description='Unified Tokenizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/UnifiedTokenizer',
     author='Jyonn Liu',
```

