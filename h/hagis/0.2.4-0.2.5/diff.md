# Comparing `tmp/hagis-0.2.4.tar.gz` & `tmp/hagis-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.4.tar", last modified: Mon Apr 17 13:06:02 2023, max compression
+gzip compressed data, was "hagis-0.2.5.tar", last modified: Mon Apr 17 13:26:53 2023, max compression
```

## Comparing `hagis-0.2.4.tar` & `hagis-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:06:02.324439 hagis-0.2.4/
--rw-rw-rw-   0        0        0      941 2023-04-17 13:06:02.322452 hagis-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 13:06:02.309262 hagis-0.2.4/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.4/hagis/__init__.py
--rw-rw-rw-   0        0        0     9714 2023-04-17 13:05:10.000000 hagis-0.2.4/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:06:02.318442 hagis-0.2.4/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-17 13:05:17.000000 hagis-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 13:06:02.325441 hagis-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:26:53.284656 hagis-0.2.5/
+-rw-rw-rw-   0        0        0      941 2023-04-17 13:26:53.283656 hagis-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 13:26:53.271105 hagis-0.2.5/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.5/hagis/__init__.py
+-rw-rw-rw-   0        0        0     9657 2023-04-17 13:24:45.000000 hagis-0.2.5/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:26:53.281645 hagis-0.2.5/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 13:26:53.000000 hagis-0.2.5/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-17 13:24:55.000000 hagis-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:26:53.284656 hagis-0.2.5/setup.cfg
```

### Comparing `hagis-0.2.4/PKG-INFO` & `hagis-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.4
+Version: 0.2.5
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.4/hagis/hagis.py` & `hagis-0.2.5/hagis/hagis.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,23 +62,22 @@
         key = generate_token_url, md5(dumps(parameters).encode("utf-8")).hexdigest()
 
         def generate_token() -> str:
             if key not in Layer._token_cache:
                 Layer._token_cache[key] = "", 0
 
             # Get the cached token and its expiry.
-            token, cachcurrent_expiration_seconds = Layer._token_cache[key];
+            token, expiration_seconds = Layer._token_cache[key];
 
             # Renew if less than a minute left.
-            if cachcurrent_expiration_seconds - time() < 60:
+            if expiration_seconds - time() < 60:
                 response = post(generate_token_url, data = parameters)
                 dictionary = loads(response.content)
-                token = dictionary["token"]
-                current_expiration_seconds = dictionary["expires"] / 1000
-                Layer._token_cache[key] = token, current_expiration_seconds
+                token, expiration_seconds = dictionary["token"], dictionary["expires"] / 1000
+                Layer._token_cache[key] = token, expiration_seconds
 
             return token
         
         self.generate_token = generate_token;
 
     def query(self, where_clause: str = "1=1", **kwargs: Any) -> Iterable[T]:
         if self._is_dynamic:
```

### Comparing `hagis-0.2.4/hagis.egg-info/PKG-INFO` & `hagis-0.2.5/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.4
+Version: 0.2.5
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.4/pyproject.toml` & `hagis-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

