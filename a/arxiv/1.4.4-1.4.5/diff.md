# Comparing `tmp/arxiv-1.4.4.tar.gz` & `tmp/arxiv-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-1.4.4.tar", last modified: Tue Apr 11 01:17:31 2023, max compression
+gzip compressed data, was "arxiv-1.4.5.tar", last modified: Mon Apr 17 00:45:59 2023, max compression
```

## Comparing `arxiv-1.4.4.tar` & `arxiv-1.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.047848 arxiv-1.4.4/
--rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.4/LICENSE.txt
--rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-11 01:17:31.047993 arxiv-1.4.4/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)     7363 2023-03-12 19:09:15.000000 arxiv-1.4.4/README.md
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.040815 arxiv-1.4.4/arxiv/
--rw-r--r--   0 lukas      (501) staff       (20)       35 2022-01-26 03:22:05.000000 arxiv-1.4.4/arxiv/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)    26550 2023-04-11 01:15:41.000000 arxiv-1.4.4/arxiv/arxiv.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.044483 arxiv-1.4.4/arxiv.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      305 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       11 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)        6 2023-04-11 01:17:30.000000 arxiv-1.4.4/arxiv.egg-info/top_level.txt
--rw-r--r--   0 lukas      (501) staff       (20)      146 2023-04-11 01:17:31.048848 arxiv-1.4.4/setup.cfg
--rw-r--r--   0 lukas      (501) staff       (20)      890 2023-04-11 01:15:41.000000 arxiv-1.4.4/setup.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-11 01:17:31.047298 arxiv-1.4.4/tests/
--rw-r--r--   0 lukas      (501) staff       (20)     1008 2021-08-18 02:16:12.000000 arxiv-1.4.4/tests/test_api_bugs.py
--rw-r--r--   0 lukas      (501) staff       (20)     7417 2023-02-01 03:02:02.000000 arxiv-1.4.4/tests/test_client.py
--rw-r--r--   0 lukas      (501) staff       (20)     1213 2022-01-26 03:22:05.000000 arxiv-1.4.4/tests/test_download.py
--rw-r--r--   0 lukas      (501) staff       (20)     4098 2021-08-18 02:16:12.000000 arxiv-1.4.4/tests/test_result.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.443871 arxiv-1.4.5/
+-rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.5/LICENSE.txt
+-rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-17 00:45:59.444040 arxiv-1.4.5/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)     7363 2023-03-12 19:09:15.000000 arxiv-1.4.5/README.md
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.436610 arxiv-1.4.5/arxiv/
+-rw-r--r--   0 lukas      (501) staff       (20)       35 2022-01-26 03:22:05.000000 arxiv-1.4.5/arxiv/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)    26587 2023-04-17 00:44:38.000000 arxiv-1.4.5/arxiv/arxiv.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.440383 arxiv-1.4.5/arxiv.egg-info/
+-rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)      305 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       11 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/requires.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        6 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/top_level.txt
+-rw-r--r--   0 lukas      (501) staff       (20)      146 2023-04-17 00:45:59.444724 arxiv-1.4.5/setup.cfg
+-rw-r--r--   0 lukas      (501) staff       (20)      890 2023-04-17 00:44:38.000000 arxiv-1.4.5/setup.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.443189 arxiv-1.4.5/tests/
+-rw-r--r--   0 lukas      (501) staff       (20)     1008 2021-08-18 02:16:12.000000 arxiv-1.4.5/tests/test_api_bugs.py
+-rw-r--r--   0 lukas      (501) staff       (20)     7417 2023-02-01 03:02:02.000000 arxiv-1.4.5/tests/test_client.py
+-rw-r--r--   0 lukas      (501) staff       (20)     1213 2022-01-26 03:22:05.000000 arxiv-1.4.5/tests/test_download.py
+-rw-r--r--   0 lukas      (501) staff       (20)     4098 2021-08-18 02:16:12.000000 arxiv-1.4.5/tests/test_result.py
```

### Comparing `arxiv-1.4.4/LICENSE.txt` & `arxiv-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.4/PKG-INFO` & `arxiv-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
```

### Comparing `arxiv-1.4.4/README.md` & `arxiv-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.4/arxiv/arxiv.py` & `arxiv-1.4.5/arxiv/arxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """.. include:: ../README.md"""
+from __future__ import annotations
+
 import logging
 import time
 import feedparser
 import re
 import os
 import warnings
 
@@ -31,15 +33,15 @@
     """A url of the form `http://arxiv.org/abs/{id}`."""
     updated: datetime
     """When the result was last updated."""
     published: datetime
     """When the result was originally published."""
     title: str
     """The title of the result."""
-    authors: list
+    authors: List[Author]
     """The result's authors."""
     summary: str
     """The result abstract."""
     comment: str
     """The authors' comment if present."""
     journal_ref: str
     """A journal reference if present."""
@@ -51,15 +53,15 @@
     Taxonomy](https://arxiv.org/category_taxonomy).
     """
     categories: List[str]
     """
     All of the result's categories. See [arXiv: Category
     Taxonomy](https://arxiv.org/category_taxonomy).
     """
-    links: list
+    links: List[Link]
     """Up to three URLs associated with this result."""
     pdf_url: str
     """The URL of a PDF version of this result if present among links."""
     _raw: feedparser.FeedParserDict
     """
     The raw feedparser result object if this Result was constructed with
     Result._from_feed_entry.
@@ -67,22 +69,22 @@
 
     def __init__(
         self,
         entry_id: str,
         updated: datetime = _DEFAULT_TIME,
         published: datetime = _DEFAULT_TIME,
         title: str = "",
-        authors: List['Result.Author'] = [],
+        authors: List[Author] = [],
         summary: str = "",
         comment: str = "",
         journal_ref: str = "",
         doi: str = "",
         primary_category: str = "",
         categories: List[str] = [],
-        links: List['Result.Link'] = [],
+        links: List[Link] = [],
         _raw: feedparser.FeedParserDict = None,
     ):
         """
         Constructs an arXiv search result item.
 
         In most cases, prefer using `Result._from_feed_entry` to parsing and
         constructing `Result`s yourself.
@@ -100,15 +102,15 @@
         self.categories = categories
         self.links = links
         # Calculated members
         self.pdf_url = Result._get_pdf_url(links)
         # Debugging
         self._raw = _raw
 
-    def _from_feed_entry(entry: feedparser.FeedParserDict) -> 'Result':
+    def _from_feed_entry(entry: feedparser.FeedParserDict) -> Result:
         """
         Converts a feedparser entry for an arXiv search result feed into a
         Result object.
         """
         if not hasattr(entry, "id"):
             raise Result.MissingFieldError("id")
         # Title attribute may be absent for certain titles. Defaulting to "0" as
@@ -217,15 +219,15 @@
             filename = self._get_default_filename('tar.gz')
         path = os.path.join(dirpath, filename)
         # Bodge: construct the source URL from the PDF URL.
         source_url = self.pdf_url.replace('/pdf/', '/src/')
         written_path, _ = urlretrieve(source_url, path)
         return written_path
 
-    def _get_pdf_url(links: list) -> str:
+    def _get_pdf_url(links: List[Link]) -> str:
         """
         Finds the PDF link among a result's links and returns its URL.
 
         Should only be called once for a given `Result`, in its constructor.
         After construction, the URL should be available in `Result.pdf_url`.
         """
         pdf_urls = [link.href for link in links if link.title == 'pdf']
@@ -262,15 +264,15 @@
             In most cases, prefer using `Author._from_feed_author` to parsing
             and constructing `Author`s yourself.
             """
             self.name = name
 
         def _from_feed_author(
             feed_author: feedparser.FeedParserDict
-        ) -> 'Result.Author':
+        ) -> Result.Author:
             """
             Constructs an `Author` with the name specified in an author object
             from a feed entry.
 
             See usage in `Result._from_feed_entry`.
             """
             return Result.Author(feed_author.name)
@@ -316,15 +318,15 @@
             self.href = href
             self.title = title
             self.rel = rel
             self.content_type = content_type
 
         def _from_feed_link(
             feed_link: feedparser.FeedParserDict
-        ) -> 'Result.Link':
+        ) -> Result.Link:
             """
             Constructs a `Link` with link metadata specified in a link object
             from a feed entry.
 
             See usage in `Result._from_feed_entry`.
             """
             return Result.Link(
@@ -412,15 +414,15 @@
 
     This should be unencoded. Use `au:del_maestro AND ti:checkerboard`, not
     `au:del_maestro+AND+ti:checkerboard`.
 
     See [the arXiv API User's Manual: Details of Query
     Construction](https://arxiv.org/help/api/user-manual#query_details).
     """
-    id_list: list
+    id_list: List[str]
     """
     A list of arXiv article IDs to which to limit the search.
 
     See [the arXiv API User's
     Manual](https://arxiv.org/help/api/user-manual#search_query_and_id_list)
     for documentation of the interaction between `query` and `id_list`.
     """
```

### Comparing `arxiv-1.4.4/arxiv.egg-info/PKG-INFO` & `arxiv-1.4.5/arxiv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
```

### Comparing `arxiv-1.4.4/setup.py` & `arxiv-1.4.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.4.4'
+version = '1.4.5'
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='arxiv',
     version=version,
```

### Comparing `arxiv-1.4.4/tests/test_api_bugs.py` & `arxiv-1.4.5/tests/test_api_bugs.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.4/tests/test_client.py` & `arxiv-1.4.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.4/tests/test_download.py` & `arxiv-1.4.5/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.4/tests/test_result.py` & `arxiv-1.4.5/tests/test_result.py`

 * *Files identical despite different names*

