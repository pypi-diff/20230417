# Comparing `tmp/heroku3-5.2.0.tar.gz` & `tmp/heroku3-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heroku3-5.2.0.tar", last modified: Thu Jan 19 11:58:55 2023, max compression
+gzip compressed data, was "heroku3-5.2.1.tar", last modified: Mon Apr 17 19:45:49 2023, max compression
```

## Comparing `heroku3-5.2.0.tar` & `heroku3-5.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-01-19 11:58:55.647284 heroku3-5.2.0/
--rw-r--r--   0 marty      (501) staff       (20)      335 2022-08-16 15:09:27.000000 heroku3-5.2.0/AUTHORS.rst
--rw-r--r--   0 marty      (501) staff       (20)      791 2022-08-16 15:09:27.000000 heroku3-5.2.0/HISTORY.rst
--rw-r--r--   0 marty      (501) staff       (20)     1187 2022-08-16 15:09:27.000000 heroku3-5.2.0/LICENSE
--rw-r--r--   0 marty      (501) staff       (20)      102 2022-08-16 15:09:27.000000 heroku3-5.2.0/MANIFEST.in
--rw-r--r--   0 marty      (501) staff       (20)    21637 2023-01-19 11:58:55.647371 heroku3-5.2.0/PKG-INFO
--rw-r--r--   0 marty      (501) staff       (20)    20089 2022-08-16 15:09:27.000000 heroku3-5.2.0/README.rst
-drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-01-19 11:58:55.641621 heroku3-5.2.0/heroku3/
--rw-r--r--   0 marty      (501) staff       (20)      430 2023-01-19 11:52:07.000000 heroku3-5.2.0/heroku3/__init__.py
--rw-r--r--   0 marty      (501) staff       (20)    19158 2022-11-28 16:04:10.000000 heroku3-5.2.0/heroku3/api.py
--rw-r--r--   0 marty      (501) staff       (20)      779 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/core.py
-drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-01-19 11:58:55.642406 heroku3-5.2.0/heroku3/data/
--rw-r--r--   0 marty      (501) staff       (20)   221418 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/data/cacert.pem
--rw-r--r--   0 marty      (501) staff       (20)       47 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/exceptions.py
--rw-r--r--   0 marty      (501) staff       (20)     2902 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/helpers.py
-drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-01-19 11:58:55.646870 heroku3-5.2.0/heroku3/models/
--rw-r--r--   0 marty      (501) staff       (20)     4996 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/__init__.py
-drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-01-19 11:58:55.647141 heroku3-5.2.0/heroku3/models/account/
--rw-r--r--   0 marty      (501) staff       (20)     2319 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/account/__init__.py
--rw-r--r--   0 marty      (501) staff       (20)      799 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/account/feature.py
--rw-r--r--   0 marty      (501) staff       (20)     1052 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/addon.py
--rw-r--r--   0 marty      (501) staff       (20)    21488 2023-01-19 11:45:10.000000 heroku3-5.2.0/heroku3/models/app.py
--rw-r--r--   0 marty      (501) staff       (20)      681 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/app_setup.py
--rw-r--r--   0 marty      (501) staff       (20)      923 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/build.py
--rw-r--r--   0 marty      (501) staff       (20)      262 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/buildpack.py
--rw-r--r--   0 marty      (501) staff       (20)      344 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/buildpack_installation.py
--rw-r--r--   0 marty      (501) staff       (20)      624 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/collaborator.py
--rw-r--r--   0 marty      (501) staff       (20)     3321 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/configvars.py
--rw-r--r--   0 marty      (501) staff       (20)      624 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/domain.py
--rw-r--r--   0 marty      (501) staff       (20)      978 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/dyno.py
--rw-r--r--   0 marty      (501) staff       (20)     1419 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/formation.py
--rw-r--r--   0 marty      (501) staff       (20)      387 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/invoice.py
--rw-r--r--   0 marty      (501) staff       (20)      571 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/key.py
--rw-r--r--   0 marty      (501) staff       (20)      573 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/logdrain.py
--rw-r--r--   0 marty      (501) staff       (20)      763 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/logsession.py
--rw-r--r--   0 marty      (501) staff       (20)     4082 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/oauth.py
--rw-r--r--   0 marty      (501) staff       (20)      385 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/region.py
--rw-r--r--   0 marty      (501) staff       (20)      577 2023-01-19 11:47:45.000000 heroku3-5.2.0/heroku3/models/release.py
--rw-r--r--   0 marty      (501) staff       (20)      451 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/slug.py
--rw-r--r--   0 marty      (501) staff       (20)      497 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/sni_endpoint.py
--rw-r--r--   0 marty      (501) staff       (20)      273 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/sourceblob.py
--rw-r--r--   0 marty      (501) staff       (20)      457 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/models/ssl_cert.py
--rw-r--r--   0 marty      (501) staff       (20)     2567 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/rendezvous.py
--rw-r--r--   0 marty      (501) staff       (20)     3295 2022-08-16 15:09:27.000000 heroku3-5.2.0/heroku3/structures.py
-drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-01-19 11:58:55.642301 heroku3-5.2.0/heroku3.egg-info/
--rw-r--r--   0 marty      (501) staff       (20)    21637 2023-01-19 11:58:55.000000 heroku3-5.2.0/heroku3.egg-info/PKG-INFO
--rw-r--r--   0 marty      (501) staff       (20)     1090 2023-01-19 11:58:55.000000 heroku3-5.2.0/heroku3.egg-info/SOURCES.txt
--rw-r--r--   0 marty      (501) staff       (20)        1 2023-01-19 11:58:55.000000 heroku3-5.2.0/heroku3.egg-info/dependency_links.txt
--rw-r--r--   0 marty      (501) staff       (20)       39 2023-01-19 11:58:55.000000 heroku3-5.2.0/heroku3.egg-info/requires.txt
--rw-r--r--   0 marty      (501) staff       (20)        8 2023-01-19 11:58:55.000000 heroku3-5.2.0/heroku3.egg-info/top_level.txt
--rw-r--r--   0 marty      (501) staff       (20)      185 2022-08-16 15:09:27.000000 heroku3-5.2.0/pyproject.toml
--rw-r--r--   0 marty      (501) staff       (20)      805 2023-01-19 11:58:55.647841 heroku3-5.2.0/setup.cfg
--rwxr-xr-x   0 marty      (501) staff       (20)     1898 2023-01-19 11:52:07.000000 heroku3-5.2.0/setup.py
+drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-04-17 19:45:49.554979 heroku3-5.2.1/
+-rw-r--r--   0 marty      (501) staff       (20)      335 2022-08-16 15:09:27.000000 heroku3-5.2.1/AUTHORS.rst
+-rw-r--r--   0 marty      (501) staff       (20)      791 2022-08-16 15:09:27.000000 heroku3-5.2.1/HISTORY.rst
+-rw-r--r--   0 marty      (501) staff       (20)     1187 2022-08-16 15:09:27.000000 heroku3-5.2.1/LICENSE
+-rw-r--r--   0 marty      (501) staff       (20)      102 2022-08-16 15:09:27.000000 heroku3-5.2.1/MANIFEST.in
+-rw-r--r--   0 marty      (501) staff       (20)    21657 2023-04-17 19:45:49.555056 heroku3-5.2.1/PKG-INFO
+-rw-r--r--   0 marty      (501) staff       (20)    20089 2022-08-16 15:09:27.000000 heroku3-5.2.1/README.rst
+drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-04-17 19:45:49.550101 heroku3-5.2.1/heroku3/
+-rw-r--r--   0 marty      (501) staff       (20)      430 2023-04-17 19:38:52.000000 heroku3-5.2.1/heroku3/__init__.py
+-rw-r--r--   0 marty      (501) staff       (20)    19158 2022-11-28 16:04:10.000000 heroku3-5.2.1/heroku3/api.py
+-rw-r--r--   0 marty      (501) staff       (20)      779 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/core.py
+drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-04-17 19:45:49.551002 heroku3-5.2.1/heroku3/data/
+-rw-r--r--   0 marty      (501) staff       (20)   221418 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/data/cacert.pem
+-rw-r--r--   0 marty      (501) staff       (20)       47 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/exceptions.py
+-rw-r--r--   0 marty      (501) staff       (20)     2902 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/helpers.py
+drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-04-17 19:45:49.554628 heroku3-5.2.1/heroku3/models/
+-rw-r--r--   0 marty      (501) staff       (20)     4996 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/__init__.py
+drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-04-17 19:45:49.554871 heroku3-5.2.1/heroku3/models/account/
+-rw-r--r--   0 marty      (501) staff       (20)     2319 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/account/__init__.py
+-rw-r--r--   0 marty      (501) staff       (20)      799 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/account/feature.py
+-rw-r--r--   0 marty      (501) staff       (20)     1052 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/addon.py
+-rw-r--r--   0 marty      (501) staff       (20)    22088 2023-04-17 19:34:39.000000 heroku3-5.2.1/heroku3/models/app.py
+-rw-r--r--   0 marty      (501) staff       (20)      681 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/app_setup.py
+-rw-r--r--   0 marty      (501) staff       (20)      923 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/build.py
+-rw-r--r--   0 marty      (501) staff       (20)      262 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/buildpack.py
+-rw-r--r--   0 marty      (501) staff       (20)      344 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/buildpack_installation.py
+-rw-r--r--   0 marty      (501) staff       (20)      624 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/collaborator.py
+-rw-r--r--   0 marty      (501) staff       (20)     3321 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/configvars.py
+-rw-r--r--   0 marty      (501) staff       (20)      624 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/domain.py
+-rw-r--r--   0 marty      (501) staff       (20)      978 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/dyno.py
+-rw-r--r--   0 marty      (501) staff       (20)     1419 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/formation.py
+-rw-r--r--   0 marty      (501) staff       (20)      387 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/invoice.py
+-rw-r--r--   0 marty      (501) staff       (20)      571 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/key.py
+-rw-r--r--   0 marty      (501) staff       (20)      573 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/logdrain.py
+-rw-r--r--   0 marty      (501) staff       (20)      763 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/logsession.py
+-rw-r--r--   0 marty      (501) staff       (20)     4082 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/oauth.py
+-rw-r--r--   0 marty      (501) staff       (20)      385 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/region.py
+-rw-r--r--   0 marty      (501) staff       (20)      577 2023-01-19 11:47:45.000000 heroku3-5.2.1/heroku3/models/release.py
+-rw-r--r--   0 marty      (501) staff       (20)      451 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/slug.py
+-rw-r--r--   0 marty      (501) staff       (20)      497 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/sni_endpoint.py
+-rw-r--r--   0 marty      (501) staff       (20)      273 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/sourceblob.py
+-rw-r--r--   0 marty      (501) staff       (20)      457 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/models/ssl_cert.py
+-rw-r--r--   0 marty      (501) staff       (20)     2567 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/rendezvous.py
+-rw-r--r--   0 marty      (501) staff       (20)     3295 2022-08-16 15:09:27.000000 heroku3-5.2.1/heroku3/structures.py
+drwxr-xr-x   0 marty      (501) staff       (20)        0 2023-04-17 19:45:49.550888 heroku3-5.2.1/heroku3.egg-info/
+-rw-r--r--   0 marty      (501) staff       (20)    21657 2023-04-17 19:45:49.000000 heroku3-5.2.1/heroku3.egg-info/PKG-INFO
+-rw-r--r--   0 marty      (501) staff       (20)     1090 2023-04-17 19:45:49.000000 heroku3-5.2.1/heroku3.egg-info/SOURCES.txt
+-rw-r--r--   0 marty      (501) staff       (20)        1 2023-04-17 19:45:49.000000 heroku3-5.2.1/heroku3.egg-info/dependency_links.txt
+-rw-r--r--   0 marty      (501) staff       (20)       39 2023-04-17 19:45:49.000000 heroku3-5.2.1/heroku3.egg-info/requires.txt
+-rw-r--r--   0 marty      (501) staff       (20)        8 2023-04-17 19:45:49.000000 heroku3-5.2.1/heroku3.egg-info/top_level.txt
+-rw-r--r--   0 marty      (501) staff       (20)      185 2022-08-16 15:09:27.000000 heroku3-5.2.1/pyproject.toml
+-rw-r--r--   0 marty      (501) staff       (20)      805 2023-04-17 19:45:49.555404 heroku3-5.2.1/setup.cfg
+-rwxr-xr-x   0 marty      (501) staff       (20)     1898 2023-04-17 19:38:52.000000 heroku3-5.2.1/setup.py
```

### Comparing `heroku3-5.2.0/HISTORY.rst` & `heroku3-5.2.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/LICENSE` & `heroku3-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/PKG-INFO` & `heroku3-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: heroku3
-Version: 5.2.0
+Version: 5.2.1
 Summary: Heroku API Wrapper.
 Home-page: https://github.com/martyzz1/heroku3.py
-Download-URL: https://github.com/martyzz1/heroku3.py/tarball/v5.2.0
 Author: Martin Moss
 Author-email: martin_moss@btinternet.com
 License: MIT
+Download-URL: https://github.com/martyzz1/heroku3.py/tarball/v5.2.1
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
@@ -738,7 +739,9 @@
 * Used in production on https://www.migreat.com & https://www.migreat.co.uk since 2013-10-01
 
 3.0.0 (2013-08-28)
 ------------------
 * Rewrite to support V3 API
 
 * Initial release.
+
+
```

### Comparing `heroku3-5.2.0/README.rst` & `heroku3-5.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/api.py` & `heroku3-5.2.1/heroku3/api.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/core.py` & `heroku3-5.2.1/heroku3/core.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/data/cacert.pem` & `heroku3-5.2.1/heroku3/data/cacert.pem`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/helpers.py` & `heroku3-5.2.1/heroku3/helpers.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/__init__.py` & `heroku3-5.2.1/heroku3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/account/__init__.py` & `heroku3-5.2.1/heroku3/models/account/__init__.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/account/feature.py` & `heroku3-5.2.1/heroku3/models/account/feature.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/addon.py` & `heroku3-5.2.1/heroku3/models/addon.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/app.py` & `heroku3-5.2.1/heroku3/models/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 class App(BaseResource):
     """Heroku App."""
 
     _strs = ["buildpack_provided_description", "git_url", "id", "name", "web_url"]
     _ints = ["slug_size", "repo_size"]
-    _bools = ["maintenance"]
+    _bools = ["maintenance", "acm"]
     _dates = ["archived_at", "created_at", "released_at", "updated_at"]
     _map = {"region": Region, "owner": User, "stack": Stack,
             "organization": Organization, "team": Team, "space": Space}
     _pks = ["name", "id"]
 
     def __init__(self):
         super(App, self).__init__()
@@ -157,14 +157,41 @@
         item = self._h._resource_deserialize(r.content.decode("utf-8"))
         return ConfigVars.new_from_dict(item, h=self._h, app=self)
 
     def sni_endpoints(self, **kwargs):
         """The SNI (SSL) endpoints for this app."""
         return self._h._get_resources(resource=("apps", self.id, "sni-endpoints"), obj=SNIEndpoint, app=self)
 
+    def enable_acm(self):
+        r = self._h._http_resource(
+            method="POST",
+            resource=("apps", self.id, "acm")
+        )
+
+        r.raise_for_status()
+        return r.ok
+
+    def disable_acm(self):
+        r = self._h._http_resource(
+            method="DELETE",
+            resource=("apps", self.id, "acm")
+        )
+
+        r.raise_for_status()
+        return r.ok
+
+    def refresh_acm(self):
+        r = self._h._http_resource(
+            method="PATCH",
+            resource=("apps", self.id, "acm")
+        )
+
+        r.raise_for_status()
+        return r.ok
+
     def add_sni_endpoint(self, certificate_chain, private_key):
         r = self._h._http_resource(
             method="POST",
             resource=("apps", self.id, "sni-endpoints"),
             data=self._h._resource_serialize({
                 "certificate_chain": certificate_chain,
                 "private_key": private_key,
```

### Comparing `heroku3-5.2.0/heroku3/models/app_setup.py` & `heroku3-5.2.1/heroku3/models/app_setup.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/build.py` & `heroku3-5.2.1/heroku3/models/build.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/collaborator.py` & `heroku3-5.2.1/heroku3/models/collaborator.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/configvars.py` & `heroku3-5.2.1/heroku3/models/configvars.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/domain.py` & `heroku3-5.2.1/heroku3/models/domain.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/dyno.py` & `heroku3-5.2.1/heroku3/models/dyno.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/formation.py` & `heroku3-5.2.1/heroku3/models/formation.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/key.py` & `heroku3-5.2.1/heroku3/models/key.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/logdrain.py` & `heroku3-5.2.1/heroku3/models/logdrain.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/logsession.py` & `heroku3-5.2.1/heroku3/models/logsession.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/oauth.py` & `heroku3-5.2.1/heroku3/models/oauth.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/models/release.py` & `heroku3-5.2.1/heroku3/models/release.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/rendezvous.py` & `heroku3-5.2.1/heroku3/rendezvous.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3/structures.py` & `heroku3-5.2.1/heroku3/structures.py`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/heroku3.egg-info/PKG-INFO` & `heroku3-5.2.1/heroku3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: heroku3
-Version: 5.2.0
+Version: 5.2.1
 Summary: Heroku API Wrapper.
 Home-page: https://github.com/martyzz1/heroku3.py
-Download-URL: https://github.com/martyzz1/heroku3.py/tarball/v5.2.0
 Author: Martin Moss
 Author-email: martin_moss@btinternet.com
 License: MIT
+Download-URL: https://github.com/martyzz1/heroku3.py/tarball/v5.2.1
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
@@ -738,7 +739,9 @@
 * Used in production on https://www.migreat.com & https://www.migreat.co.uk since 2013-10-01
 
 3.0.0 (2013-08-28)
 ------------------
 * Rewrite to support V3 API
 
 * Initial release.
+
+
```

### Comparing `heroku3-5.2.0/heroku3.egg-info/SOURCES.txt` & `heroku3-5.2.1/heroku3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heroku3-5.2.0/setup.cfg` & `heroku3-5.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 5.2.0
+current_version = 5.2.1
 commit = True
 tag = True
 
 [bumpversion:file:heroku3/__init__.py]
 
 [bumpversion:file:setup.py]
 search = https://github.com/martyzz1/heroku3.py/tarball/v{current_version}
```

### Comparing `heroku3-5.2.0/setup.py` & `heroku3-5.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     version=version,
     description="Heroku API Wrapper.",
     long_description=open("README.rst").read() + "\n\n" + open("HISTORY.rst").read(),
     # long_description_content_type="text/x-rst",
     author="Martin Moss",
     author_email="martin_moss@btinternet.com",
     url="https://github.com/martyzz1/heroku3.py",
-    download_url="https://github.com/martyzz1/heroku3.py/tarball/v5.2.0",
+    download_url="https://github.com/martyzz1/heroku3.py/tarball/v5.2.1",
     packages=["heroku3"],
     package_data={
         "": [
             "LICENSE",
         ]
     },
     include_package_data=True,
```

