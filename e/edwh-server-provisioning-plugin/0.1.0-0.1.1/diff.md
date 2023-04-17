# Comparing `tmp/edwh_server_provisioning_plugin-0.1.0.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.1.1.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.1.0.tar` & `edwh_server_provisioning_plugin-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/.dcignore
--rw-r--r--   0        0        0    13500 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/requirements.txt
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/setup.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    45349 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/readme.md
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/.dcignore
+-rw-r--r--   0        0        0    13732 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/old_documentation_in_dutch.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/src/edwh_server_provisioning_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/src/edwh_server_provisioning_plugin/__init__.py
+-rw-r--r--   0        0        0    45349 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/readme.md
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.1/PKG-INFO
```

### Comparing `edwh_server_provisioning_plugin-0.1.0/.dcignore` & `edwh_server_provisioning_plugin-0.1.1/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.0/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.1.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.1 (2023-04-17)
+### Documentation
+* **readme:** New plugin docs, keep old (Dutch) readme for reference ([`fe2e8da`](https://github.com/educationwarehouse/server_provisioning/commit/fe2e8daec6ca758cc3997fc5ce95de9f3735ad52))
+
 ## v0.1.0 (2023-04-17)
 ### Feature
 * **server_provisioning:** Rewrote to edwh plugin structure ([`632a604`](https://github.com/educationwarehouse/server_provisioning/commit/632a604182aa35b06b1fbfdab1a5f9cf9766a1fe))
 * **connect-postgres:** Allow selecting 'omgeving' from which to use postgres with the -o flag ([`ecdf807`](https://github.com/educationwarehouse/server_provisioning/commit/ecdf8078ab5f5192bd9d7056a7543c9514dc11a0))
 * **ungit:** Finished ungit via npx + port forwarding ([`93b6972`](https://github.com/educationwarehouse/server_provisioning/commit/93b69726e74e125dc4c64b0fb706b7c06e1b8ff3))
 * **ungit:** Ungit werkte maar nog niet goed in de achtergrond :( ([`fc85368`](https://github.com/educationwarehouse/server_provisioning/commit/fc8536836183efbde97745ec86cfc389949ad8fe))
 * Setup.sh toegevoegd ([`948dd4c`](https://github.com/educationwarehouse/server_provisioning/commit/948dd4c237357d1dacdea189d862cda0c2f940fe))
```

### Comparing `edwh_server_provisioning_plugin-0.1.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.1.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.0/LICENSE.txt` & `edwh_server_provisioning_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.0/pyproject.toml` & `edwh_server_provisioning_plugin-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.0/readme.md` & `edwh_server_provisioning_plugin-0.1.1/old_documentation_in_dutch.md`

 * *Files identical despite different names*

