# Comparing `tmp/ansible_aisnippet-0.1.1.tar.gz` & `tmp/ansible_aisnippet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_aisnippet-0.1.1.tar", max compression
+gzip compressed data, was "ansible_aisnippet-0.1.2.tar", max compression
```

## Comparing `ansible_aisnippet-0.1.1.tar` & `ansible_aisnippet-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-17 07:46:59.777856 ansible_aisnippet-0.1.1/LICENSE
--rw-r--r--   0        0        0     6367 2023-04-17 07:29:55.142141 ansible_aisnippet-0.1.1/README.md
--rw-r--r--   0        0        0       83 2023-04-11 08:44:07.947618 ansible_aisnippet-0.1.1/ansible_aisnippet/__init__.py
--rw-r--r--   0        0        0     3972 2023-04-17 07:13:11.832041 ansible_aisnippet-0.1.1/ansible_aisnippet/aisnippet.py
--rw-r--r--   0        0        0     1157 2023-04-17 06:00:51.121775 ansible_aisnippet-0.1.1/ansible_aisnippet/helpers.py
--rw-r--r--   0        0        0     2680 2023-04-17 06:52:47.622249 ansible_aisnippet-0.1.1/ansible_aisnippet/main.py
--rw-r--r--   0        0        0    46019 2023-04-17 06:31:12.350668 ansible_aisnippet-0.1.1/ansible_aisnippet/snippets.json
--rw-r--r--   0        0        0      908 2023-04-17 09:01:43.790253 ansible_aisnippet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7273 1970-01-01 00:00:00.000000 ansible_aisnippet-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6367 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/README.md
+-rw-r--r--   0        0        0       83 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/ansible_aisnippet/__init__.py
+-rw-r--r--   0        0        0     3972 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/ansible_aisnippet/aisnippet.py
+-rw-r--r--   0        0        0     1157 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/ansible_aisnippet/helpers.py
+-rw-r--r--   0        0        0     2680 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/ansible_aisnippet/main.py
+-rw-r--r--   0        0        0    46019 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/ansible_aisnippet/snippets.json
+-rw-r--r--   0        0        0      908 2023-04-17 09:05:14.485315 ansible_aisnippet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7273 1970-01-01 00:00:00.000000 ansible_aisnippet-0.1.2/PKG-INFO
```

### Comparing `ansible_aisnippet-0.1.1/LICENSE` & `ansible_aisnippet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_aisnippet-0.1.1/README.md` & `ansible_aisnippet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ansible_aisnippet-0.1.1/ansible_aisnippet/aisnippet.py` & `ansible_aisnippet-0.1.2/ansible_aisnippet/aisnippet.py`

 * *Files identical despite different names*

### Comparing `ansible_aisnippet-0.1.1/ansible_aisnippet/helpers.py` & `ansible_aisnippet-0.1.2/ansible_aisnippet/helpers.py`

 * *Files identical despite different names*

### Comparing `ansible_aisnippet-0.1.1/ansible_aisnippet/main.py` & `ansible_aisnippet-0.1.2/ansible_aisnippet/main.py`

 * *Files identical despite different names*

### Comparing `ansible_aisnippet-0.1.1/ansible_aisnippet/snippets.json` & `ansible_aisnippet-0.1.2/ansible_aisnippet/snippets.json`

 * *Files identical despite different names*

### Comparing `ansible_aisnippet-0.1.1/pyproject.toml` & `ansible_aisnippet-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ansible-aisnippet"
-version = "0.1.1"
+version = "0.1.2"
 description = "Ansible-aisnippet Generate ansible tasks with ChatGPT."
 authors = ["Stephane ROBERT <robert.stephane.28@gmail.com>"]
 readme = "README.md"
 include = [
     "LICENSE",
 ]
 homepage = "https://blog.stephane-robert.info/"
```

### Comparing `ansible_aisnippet-0.1.1/PKG-INFO` & `ansible_aisnippet-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-aisnippet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ansible-aisnippet Generate ansible tasks with ChatGPT.
 Home-page: https://blog.stephane-robert.info/
 Keywords: ansible,module,ChatGPT
 Author: Stephane ROBERT
 Author-email: robert.stephane.28@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

