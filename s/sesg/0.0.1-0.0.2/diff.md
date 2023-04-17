# Comparing `tmp/sesg-0.0.1.tar.gz` & `tmp/sesg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesg-0.0.1.tar", max compression
+gzip compressed data, was "sesg-0.0.2.tar", max compression
```

## Comparing `sesg-0.0.1.tar` & `sesg-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.1/LICENSE
--rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.1/README.md
--rw-r--r--   0        0        0     3014 2023-04-17 17:40:49.328811 sesg-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.1/src/sesg/__init__.py
--rw-r--r--   0        0        0     8118 2023-04-17 15:25:34.200852 sesg-0.0.1/src/sesg/graph.py
--rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.1/src/sesg/metrics.py
--rw-r--r--   0        0        0    16870 2023-04-16 16:49:33.237266 sesg-0.0.1/src/sesg/scopus_client.py
--rw-r--r--   0        0        0    13843 2023-04-17 14:58:16.710757 sesg-0.0.1/src/sesg/search_string.py
--rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.1/src/sesg/snowballing.py
--rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.1/src/sesg/topic_extraction.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.2/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.2/README.md
+-rw-r--r--   0        0        0     3014 2023-04-17 21:18:26.339911 sesg-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.2/src/sesg/__init__.py
+-rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.2/src/sesg/graph.py
+-rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.2/src/sesg/metrics.py
+-rw-r--r--   0        0        0    16870 2023-04-16 16:49:33.237266 sesg-0.0.2/src/sesg/scopus_client.py
+-rw-r--r--   0        0        0    13843 2023-04-17 14:58:16.710757 sesg-0.0.2/src/sesg/search_string.py
+-rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.2/src/sesg/snowballing.py
+-rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.2/src/sesg/topic_extraction.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.2/PKG-INFO
```

### Comparing `sesg-0.0.1/LICENSE` & `sesg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sesg-0.0.1/pyproject.toml` & `sesg-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sesg"
-version = "0.0.1"
+version = "0.0.2"
 description = "SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string."
 authors = ["Demetrius Panovitch <demetrius.mp789@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
   {include = "sesg", from = "src"}
 ]
```

### Comparing `sesg-0.0.1/src/sesg/graph.py` & `sesg-0.0.2/src/sesg/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     Examples:
         >>> adjacency_list = {
         ...     1: [2],
         ...     2: [3, 4],
         ...     4: [5, 6]
         ... }
-        >>> breadth_first_search(adjacency_list=adjacency_list, starting_node=2)
+        >>> _breadth_first_search(adjacency_list=adjacency_list, starting_node=2)
         [2, 4, 6, 5, 3]
     """  # noqa: E501
     reachable_nodes: List[int] = []
     q: deque[int] = deque()
     visited: Mapping[int, bool] = defaultdict(lambda: False)
 
     s = starting_node
@@ -206,15 +206,15 @@
     def format_node(node_id: int) -> str:
         return str(node_id).zfill(node_padding)
 
     # adding nodes
     # all nodes will be created as "not found" (with dashed style)
     for node, tooltip in tooltips.items():
         graph.node(
-            str(node),
+            format_node(node),
             tooltip=tooltip,
             style="dashed",
         )
 
     # adding edges
     for node, neighbors in adjacency_list.items():
         for neighbor in neighbors:
```

### Comparing `sesg-0.0.1/src/sesg/metrics.py` & `sesg-0.0.2/src/sesg/metrics.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.1/src/sesg/scopus_client.py` & `sesg-0.0.2/src/sesg/scopus_client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.1/src/sesg/search_string.py` & `sesg-0.0.2/src/sesg/search_string.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.1/src/sesg/snowballing.py` & `sesg-0.0.2/src/sesg/snowballing.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.1/src/sesg/topic_extraction.py` & `sesg-0.0.2/src/sesg/topic_extraction.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.1/PKG-INFO` & `sesg-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesg
-Version: 0.0.1
+Version: 0.0.2
 Summary: SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string.
 License: GPL-3.0-only
 Author: Demetrius Panovitch
 Author-email: demetrius.mp789@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

