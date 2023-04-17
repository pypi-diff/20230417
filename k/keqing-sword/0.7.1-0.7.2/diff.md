# Comparing `tmp/keqing_sword-0.7.1.tar.gz` & `tmp/keqing_sword-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keqing_sword-0.7.1.tar", max compression
+gzip compressed data, was "keqing_sword-0.7.2.tar", max compression
```

## Comparing `keqing_sword-0.7.1.tar` & `keqing_sword-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/LICENSE
--rw-r--r--   0        0        0     1930 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/README.md
--rw-r--r--   0        0        0      686 2023-02-04 05:02:57.543067 keqing_sword-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/__init__.py
--rw-r--r--   0        0        0       89 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/global_const.py
--rw-r--r--   0        0        0     1689 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_diff.py
--rw-r--r--   0        0        0     2211 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_getosm.py
--rw-r--r--   0        0        0     1071 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_getosm.py.LICENSE
--rw-r--r--   0        0        0      137 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_getosm.py.METADATA
--rw-r--r--   0        0        0      514 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_network.py
--rw-r--r--   0        0        0      329 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_parse.py
--rw-r--r--   0        0        0     1686 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_query.py
--rw-r--r--   0        0        0       10 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_stream_read.py
--rw-r--r--   0        0        0        0 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/method_stream_write.py
--rw-r--r--   0        0        0     3093 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/model_basic.py
--rw-r--r--   0        0        0     1789 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/type_constraint.py
--rw-r--r--   0        0        0      498 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/type_data.py
--rw-r--r--   0        0        0     5417 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/type_element.py
--rw-r--r--   0        0        0    14006 2023-02-04 05:00:03.591530 keqing_sword-0.7.1/src/kqs/waifu.py
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 keqing_sword-0.7.1/setup.py
--rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 keqing_sword-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 07:01:30.054163 keqing_sword-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3764 2023-04-17 07:01:30.054163 keqing_sword-0.7.2/README.md
+-rw-r--r--   0        0        0      704 2023-04-17 07:03:03.466672 keqing_sword-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/__init__.py
+-rw-r--r--   0        0        0       89 2023-04-17 07:02:45.882558 keqing_sword-0.7.2/src/kqs/global_const.py
+-rw-r--r--   0        0        0     1689 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_diff.py
+-rw-r--r--   0        0        0     2211 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_getosm.py
+-rw-r--r--   0        0        0     1071 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_getosm.py.LICENSE
+-rw-r--r--   0        0        0      137 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_getosm.py.METADATA
+-rw-r--r--   0        0        0      514 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_network.py
+-rw-r--r--   0        0        0     1130 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_parse.py
+-rw-r--r--   0        0        0     1686 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_query.py
+-rw-r--r--   0        0        0       10 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_stream_read.py
+-rw-r--r--   0        0        0        0 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_stream_write.py
+-rw-r--r--   0        0        0     3093 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/model_basic.py
+-rw-r--r--   0        0        0     1789 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/type_constraint.py
+-rw-r--r--   0        0        0      498 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/type_data.py
+-rw-r--r--   0        0        0     5417 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/type_element.py
+-rw-r--r--   0        0        0    14429 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/waifu.py
+-rw-r--r--   0        0        0     4396 1970-01-01 00:00:00.000000 keqing_sword-0.7.2/PKG-INFO
```

### Comparing `keqing_sword-0.7.1/LICENSE` & `keqing_sword-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/pyproject.toml` & `keqing_sword-0.7.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "Keqing_Sword"
-version = "0.7.1"
+version = "0.7.2"
 description = "A non-database Python base OSM data parser, with SQL operation simulated."
 authors = ["快乐的老鼠宝宝 <keaitianxinmail@qq.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "src/kqs"}]
+packages = [
+    {include = "kqs", from = "src"},
+]
+
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
 
 [tool.poetry.group.prod.dependencies]
 python = ">=3.8,<4"
```

### Comparing `keqing_sword-0.7.1/src/kqs/method_diff.py` & `keqing_sword-0.7.2/src/kqs/method_diff.py`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/method_getosm.py` & `keqing_sword-0.7.2/src/kqs/method_getosm.py`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/method_getosm.py.LICENSE` & `keqing_sword-0.7.2/src/kqs/method_getosm.py.LICENSE`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/method_network.py` & `keqing_sword-0.7.2/src/kqs/method_network.py`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/method_query.py` & `keqing_sword-0.7.2/src/kqs/method_query.py`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/model_basic.py` & `keqing_sword-0.7.2/src/kqs/model_basic.py`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/type_constraint.py` & `keqing_sword-0.7.2/src/kqs/type_constraint.py`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/type_element.py` & `keqing_sword-0.7.2/src/kqs/type_element.py`

 * *Files identical despite different names*

### Comparing `keqing_sword-0.7.1/src/kqs/waifu.py` & `keqing_sword-0.7.2/src/kqs/waifu.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,26 +94,39 @@
                 self.bounds_list.append(Bounds(element.attrib))
             else:
                 # raise TypeError('Unexpected element tag type: ' + element.tag)
                 pass
 
     def meow(self):
         import logging
-        logging.info(str(
-        ("==============================\n")
-        +("Keqing load successful!\n")
-        +("==============================\n")
-        +(
-            str(len(self.node_dict))
-            +str(len(self.way_dict))
-            +str(len(self.relation_dict))
-            +str(len(self.bounds_list))
+
+        logging.basicConfig(level=logging.INFO)
+        logging.info(
+            str(
+                "\n"
+                + "==============================\n"
+                + "Keqing load successful!\n"
+                + "==============================\n"
+                + (
+                    "node    : "
+                    + str(len(self.node_dict))
+                    + "\n"
+                    + "way     : "
+                    + str(len(self.way_dict))
+                    + "\n"
+                    + "relation: "
+                    + str(len(self.relation_dict))
+                    + "\n"
+                    + "bounds  : "
+                    + str(len(self.bounds_list))
+                    + "\n"
+                )
+                + "=============================="
+            )
         )
-        +("\n==============================")
-        ))
 
     def read(self, mode=None, file_path="", text="", url="", fpath=""):
         def pre_read_warn(mode: str, file_path: str, text: str, url: str):
             if url != "" and (mode != "network" and mode != "n"):
                 if ("http://" in url) or ("https://" in url):
                     print(
                         "WARN:You may intent to request from network, but you enter another mode."
```

