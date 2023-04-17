# Comparing `tmp/gofigr-0.10.5.tar.gz` & `tmp/gofigr-0.10.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofigr-0.10.5.tar", last modified: Thu Apr  6 16:46:32 2023, max compression
+gzip compressed data, was "gofigr-0.10.6.tar", last modified: Sun Apr 16 22:56:38 2023, max compression
```

## Comparing `gofigr-0.10.5.tar` & `gofigr-0.10.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 16:46:32.178324 gofigr-0.10.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-04-06 16:28:46.000000 gofigr-0.10.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-04-06 16:28:46.000000 gofigr-0.10.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-04-06 16:46:32.178324 gofigr-0.10.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-04-06 16:28:46.000000 gofigr-0.10.5/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 16:46:32.170324 gofigr-0.10.5/gofigr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12625 2023-04-06 16:28:46.000000 gofigr-0.10.5/gofigr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-04-06 16:28:46.000000 gofigr-0.10.5/gofigr/gfconfig.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17897 2023-04-06 16:28:46.000000 gofigr-0.10.5/gofigr/jupyter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41221 2023-04-06 16:28:46.000000 gofigr-0.10.5/gofigr/models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 16:46:32.174324 gofigr-0.10.5/gofigr/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-04-06 16:28:46.000000 gofigr-0.10.5/gofigr/resources/FreeMono.ttf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-04-06 16:28:46.000000 gofigr-0.10.5/gofigr/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2023-04-06 16:28:46.000000 gofigr-0.10.5/gofigr/watermarks.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 16:46:32.174324 gofigr-0.10.5/gofigr.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-04-06 16:46:32.000000 gofigr-0.10.5/gofigr.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      447 2023-04-06 16:46:32.000000 gofigr-0.10.5/gofigr.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-06 16:46:32.000000 gofigr-0.10.5/gofigr.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-06 16:46:32.000000 gofigr-0.10.5/gofigr.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2023-04-06 16:46:32.000000 gofigr-0.10.5/gofigr.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-04-06 16:46:32.000000 gofigr-0.10.5/gofigr.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1522 2023-04-06 16:28:46.000000 gofigr-0.10.5/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-06 16:46:32.178324 gofigr-0.10.5/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-06 16:46:32.178324 gofigr-0.10.5/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40678 2023-04-06 16:28:46.000000 gofigr-0.10.5/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-04-06 16:28:46.000000 gofigr-0.10.5/tests/test_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-04-06 16:28:46.000000 gofigr-0.10.5/tests/test_watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.213648 gofigr-0.10.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-04-16 22:39:06.000000 gofigr-0.10.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-04-16 22:39:06.000000 gofigr-0.10.6/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-04-16 22:56:38.213648 gofigr-0.10.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-04-16 22:39:06.000000 gofigr-0.10.6/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.209648 gofigr-0.10.6/gofigr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12625 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/gfconfig.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18297 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/jupyter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41605 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.213648 gofigr-0.10.6/gofigr/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/resources/FreeMono.ttf
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.209648 gofigr-0.10.6/gofigr.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      447 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-04-16 22:39:06.000000 gofigr-0.10.6/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-16 22:56:38.213648 gofigr-0.10.6/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.213648 gofigr-0.10.6/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40797 2023-04-16 22:39:06.000000 gofigr-0.10.6/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-04-16 22:39:06.000000 gofigr-0.10.6/tests/test_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-04-16 22:39:06.000000 gofigr-0.10.6/tests/test_watermarks.py
```

### Comparing `gofigr-0.10.5/LICENSE` & `gofigr-0.10.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.5/PKG-INFO` & `gofigr-0.10.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.10.5
+Version: 0.10.6
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/10.0.4/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.10.6/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.10.5)
+GoFigr - Python Client (0.10.6)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.10.5/README.rst` & `gofigr-0.10.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.10.5)
+GoFigr - Python Client (0.10.6)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.10.5/gofigr/__init__.py` & `gofigr-0.10.6/gofigr/__init__.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.5/gofigr/gfconfig.py` & `gofigr-0.10.6/gofigr/gfconfig.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.5/gofigr/jupyter.py` & `gofigr-0.10.6/gofigr/jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,19 +296,28 @@
             fig = plt.figure(num)
             if not getattr(fig, '_gf_is_published', False):
                 self.publish(fig=fig)
 
     @staticmethod
     def _resolve_target(gf, fig, target):
         if target is None:
-            cell_id = _GF_EXTENSION.cell.cell_id
-            if cell_id is None:
-                cell_id = "Unknown"
+            # Try to get the figure's title
+            suptitle = getattr(fig, "_suptitle", "")
+            title = fig.axes[0].get_title() if len(fig.axes) > 0 else None
+            if suptitle is not None and suptitle.strip() != "":
+                fig_name = suptitle
+            elif title is not None and title.strip() != "":
+                fig_name = title
+            else:
+                cell_id = _GF_EXTENSION.cell.cell_id
+                if cell_id is None:
+                    cell_id = "Unknown"
+
+                fig_name = f"Cell {cell_id}, Figure #{fig.number}"
 
-            fig_name = f"Cell {cell_id}, Figure #{fig.number}"
             return _GF_EXTENSION.analysis.get_figure(fig_name, create=True)
         else:
             return parse_model_instance(gf.Figure,
                                         target,
                                         lambda search: _GF_EXTENSION.analysis.get_figure(name=search.name,
                                                                                          description=search.description,
                                                                                          create=search.create))
```

### Comparing `gofigr-0.10.5/gofigr/models.py` & `gofigr-0.10.6/gofigr/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -814,14 +814,16 @@
         analyses = [self._gf.Analysis(**datum) for datum in data.get("analyses", [])]
         figures = [self._gf.Figure(**datum) for datum in data.get("figures", [])]
         return Recents(analyses, figures)
 
 
 class gf_Analysis(ShareableModelMixin):
     """Represents an analysis"""
+    # pylint: disable=protected-access
+
     fields = ["api_id",
               "name",
               "description",
               LinkedEntityField("workspace", lambda gf: gf.Workspace, lazy=True, many=False),
               LinkedEntityField("figures", lambda gf: gf.Figure, lazy=True, many=True, derived=True,
                                 backlink_property='analysis')] + TIMESTAMP_FIELDS + CHILD_TIMESTAMP_FIELDS
     endpoint = "analysis/"
@@ -835,14 +837,24 @@
         :param kwargs: parameters to Figure (e.g. description) if it needs to be created
         :return: Figure instance
 
         """
         return self.figures.find_or_create(name=name,
                                            default_obj=self._gf.Figure(name=name, **kwargs) if create else None)
 
+    def get_logs(self):
+        """\
+        Retrieves the activity log.
+
+        :return: list of LogItem objects.
+        """
+        response = self._gf._get(urljoin(self.endpoint, f'{self.api_id}/log/'),
+                                 expected_status=HTTPStatus.OK)
+        return [LogItem.from_json(datum) for datum in response.json()]
+
 
 class gf_Figure(ShareableModelMixin):
     """Represents a figure"""
     fields = ["api_id",
               "name",
               "description",
               LinkedEntityField("analysis", lambda gf: gf.Analysis, lazy=True, many=False),
```

### Comparing `gofigr-0.10.5/gofigr/resources/FreeMono.ttf` & `gofigr-0.10.6/gofigr/resources/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.5/gofigr/watermarks.py` & `gofigr-0.10.6/gofigr/watermarks.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.5/gofigr.egg-info/PKG-INFO` & `gofigr-0.10.6/gofigr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.10.5
+Version: 0.10.6
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/10.0.4/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.10.6/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.10.5)
+GoFigr - Python Client (0.10.6)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.10.5/pyproject.toml` & `gofigr-0.10.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gofigr"
-version = "0.10.5"
+version = "0.10.6"
 description = "GoFigr client library"
 readme = "README.rst"
 authors = [{ name = "Maciej Pacula", email = "maciej@gofigr.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,25 +20,25 @@
 dependencies = [
     "numpy", "pandas", "pyqrcode", "pillow", "matplotlib", "dateutils",
     "python-dateutil", "ipython", "requests", "pypng", "ipynbname"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
-dev = ["pip-tools", "bumpver", "build", "twine", "pylint", "flake8", "sphinx", "sphinx_rtd_theme"]
+dev = ["pip-tools", "bumpver", "build", "twine", "pylint", "flake8", "sphinx", "sphinx_rtd_theme", "sphinxcontrib-jquery"]
 
 [project.urls]
 Homepage = "https://www.gofigr.io"
-Documentation = "https://gofigr.io/docs/gofigr-python/10.0.4/"
+Documentation = "https://gofigr.io/docs/gofigr-python/0.10.6/"
 
 [project.scripts]
 gfconfig = "gofigr.gfconfig:main"
 
 [tool.bumpver]
-current_version = "0.10.5"
+current_version = "0.10.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gofigr-0.10.5/tests/test_client.py` & `gofigr-0.10.6/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -780,14 +780,16 @@
 
             # Even though the object is shared, the user it's shared with should not be able to view who else
             # it's shared with.
             self.assertRaises(UnauthorizedError, lambda: self.clone_gf_object(obj, other_client).get_sharing_users())
 
             # Unshare
             obj.unshare(other_client.username)
+            time.sleep(2)
+
             self.assertRaises(UnauthorizedError,
                               lambda: self.clone_gf_object(obj, other_client, bare=True).fetch())
             self.assertEqual(len(obj.get_sharing_users()), 0)
 
             # Double unshare
             obj.unshare(other_client.username)
             self.assertRaises(UnauthorizedError,
@@ -799,25 +801,28 @@
             shared_obj = self.clone_gf_object(obj, other_client, bare=True).fetch()
             self.assertEqual(obj, shared_obj)
             self.assertEqual(len(obj.get_sharing_users()), 0)
             self.assertRaises(UnauthorizedError, lambda: self.clone_gf_object(obj, other_client).get_sharing_users())
 
             # Turn off link sharing
             obj.set_link_sharing(False)
+            time.sleep(2)
+
             self.assertRaises(UnauthorizedError,
                               lambda: self.clone_gf_object(obj, other_client, bare=True).fetch())
             self.assertEqual(len(obj.get_sharing_users()), 0)
 
         for client, other_client in self.client_pairs:
             for obj in self.list_all_objects(client):
                 if not isinstance(obj, ShareableModelMixin):
                     continue
 
                 for _ in range(2):  # Sharing/unsharing cycles are indempotent
                     _check_one(other_client, obj)
+                    time.sleep(2)
 
                 # Sharing with a non-existent user
                 self.assertRaises(RuntimeError, lambda: obj.share("no_such_user_exists"))
                 self.assertRaises(RuntimeError, lambda: obj.unshare("no_such_user_exists"))
 
         # Nothing should be shared now
         self.assert_exclusivity()
@@ -911,14 +916,16 @@
                 # Still, should not be able to remove original OWNER
                 self.assertRaises(RuntimeError, lambda: workspace_ref.change_membership(client.username,
                                                                                         WorkspaceMembership.ADMIN))
 
                 # User should be able to downgrade themselves
                 workspace_ref.change_membership(other_client.username, WorkspaceMembership.VIEWER)
 
+                time.sleep(2)
+
                 self.assertRaises(UnauthorizedError, lambda: workspace_ref.change_membership(other_client.username,
                                                                                              WorkspaceMembership.ADMIN))
 
     def test_membership_validation(self):
         for client, other_client in self.client_pairs:
             for workspace in client.workspaces:
                 self.assertRaises(RuntimeError,
```

### Comparing `gofigr-0.10.5/tests/test_models.py` & `gofigr-0.10.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.5/tests/test_watermarks.py` & `gofigr-0.10.6/tests/test_watermarks.py`

 * *Files identical despite different names*

