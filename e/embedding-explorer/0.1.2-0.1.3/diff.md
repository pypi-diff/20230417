# Comparing `tmp/embedding_explorer-0.1.2.tar.gz` & `tmp/embedding_explorer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding_explorer-0.1.2.tar", max compression
+gzip compressed data, was "embedding_explorer-0.1.3.tar", max compression
```

## Comparing `embedding_explorer-0.1.2.tar` & `embedding_explorer-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.1.2/LICENSE
--rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.1.2/README.md
--rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.1.2/embedding_explorer/__init__.py
--rw-r--r--   0        0        0     4578 2023-04-11 10:33:13.278666 embedding_explorer-0.1.2/embedding_explorer/app.py
--rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.1.2/embedding_explorer/assets/favicon.ico
--rw-r--r--   0        0        0     2170 2023-04-11 10:30:36.606316 embedding_explorer-0.1.2/embedding_explorer/blueprints/dashboard.py
--rw-r--r--   0        0        0     3250 2023-04-11 10:30:00.242235 embedding_explorer-0.1.2/embedding_explorer/blueprints/explorer.py
--rw-r--r--   0        0        0     2277 2023-03-27 13:27:51.091877 embedding_explorer-0.1.2/embedding_explorer/components/model_card.py
--rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.1.2/embedding_explorer/components/network.py
--rw-r--r--   0        0        0     1106 2023-03-17 13:45:00.203784 embedding_explorer-0.1.2/embedding_explorer/components/slider.py
--rw-r--r--   0        0        0     3239 2023-04-11 10:28:39.678054 embedding_explorer-0.1.2/embedding_explorer/components/word_selector.py
--rw-r--r--   0        0        0      853 2023-03-27 13:36:18.356965 embedding_explorer-0.1.2/embedding_explorer/model.py
--rw-r--r--   0        0        0     4907 2023-03-20 14:01:46.998402 embedding_explorer-0.1.2/embedding_explorer/plots/network.py
--rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.1.2/embedding_explorer/prepare/semkern.py
--rw-r--r--   0        0        0     1125 2023-03-27 14:47:02.041747 embedding_explorer-0.1.2/embedding_explorer/prepare/thumbnails.py
--rw-r--r--   0        0        0      684 2023-04-11 10:36:05.899051 embedding_explorer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.1.2/setup.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-03-13 11:52:25.053838 embedding_explorer-0.1.3/LICENSE
+-rw-r--r--   0        0        0       95 2023-03-13 11:52:25.057838 embedding_explorer-0.1.3/README.md
+-rw-r--r--   0        0        0      142 2023-03-27 13:50:12.710655 embedding_explorer-0.1.3/embedding_explorer/__init__.py
+-rw-r--r--   0        0        0     4732 2023-04-17 11:46:15.047242 embedding_explorer-0.1.3/embedding_explorer/app.py
+-rw-r--r--   0        0        0    16170 2023-03-21 14:13:23.726074 embedding_explorer-0.1.3/embedding_explorer/assets/favicon.ico
+-rw-r--r--   0        0        0     2041 2023-04-17 11:40:06.279827 embedding_explorer-0.1.3/embedding_explorer/blueprints/dashboard.py
+-rw-r--r--   0        0        0     3250 2023-04-11 10:30:00.242235 embedding_explorer-0.1.3/embedding_explorer/blueprints/explorer.py
+-rw-r--r--   0        0        0     2277 2023-03-27 13:27:51.091877 embedding_explorer-0.1.3/embedding_explorer/components/model_card.py
+-rw-r--r--   0        0        0     2000 2023-03-27 13:28:01.367900 embedding_explorer-0.1.3/embedding_explorer/components/network.py
+-rw-r--r--   0        0        0     1106 2023-03-17 13:45:00.203784 embedding_explorer-0.1.3/embedding_explorer/components/slider.py
+-rw-r--r--   0        0        0     3239 2023-04-11 10:28:39.678054 embedding_explorer-0.1.3/embedding_explorer/components/word_selector.py
+-rw-r--r--   0        0        0      853 2023-03-27 13:36:18.356965 embedding_explorer-0.1.3/embedding_explorer/model.py
+-rw-r--r--   0        0        0     4907 2023-03-20 14:01:46.998402 embedding_explorer-0.1.3/embedding_explorer/plots/network.py
+-rw-r--r--   0        0        0     5843 2023-03-27 14:42:08.501085 embedding_explorer-0.1.3/embedding_explorer/prepare/semkern.py
+-rw-r--r--   0        0        0     1125 2023-03-27 14:47:02.041747 embedding_explorer-0.1.3/embedding_explorer/prepare/thumbnails.py
+-rw-r--r--   0        0        0      684 2023-04-17 11:48:58.442963 embedding_explorer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 embedding_explorer-0.1.3/setup.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 embedding_explorer-0.1.3/PKG-INFO
```

### Comparing `embedding_explorer-0.1.2/LICENSE` & `embedding_explorer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/app.py` & `embedding_explorer-0.1.3/embedding_explorer/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 from dash_extensions.enrich import Dash, DashBlueprint
 
 from embedding_explorer.blueprints.dashboard import create_dashboard
 from embedding_explorer.blueprints.explorer import create_explorer
 from embedding_explorer.model import Model
 
 
-def get_dash_app(blueprint: DashBlueprint, use_pages: bool) -> Dash:
+def get_dash_app(blueprint: DashBlueprint, **kwargs) -> Dash:
     """Returns app based on a blueprint with
     tailwindcss and font awesome added."""
+    additional_scripts = kwargs.get("external_scripts", [])
+    use_pages = kwargs.get("use_pages", False)
+    pages_folder = "" if use_pages else "pages"
     app = Dash(
-        __name__,
         blueprint=blueprint,
-        title="embedding-explorer",
+        title=kwargs.get("title", "embedding-explorer"),
         external_scripts=[
             {
                 "src": "https://cdn.tailwindcss.com",
             },
             {
                 "src": "https://kit.fontawesome.com/9640e5cd85.js",
                 "crossorigin": "anonymous",
             },
+            *additional_scripts,
         ],
         prevent_initial_callbacks=True,
-        use_pages=use_pages,
-        pages_folder="" if use_pages else "pages",
+        pages_folder=pages_folder,
+        **kwargs,
     )
     return app
 
 
 def is_notebook() -> bool:
     return "ipykernel" in sys.modules
 
@@ -152,9 +155,9 @@
         If the app runs in a Jupyter notebook, work goes on on
         a background thread, this thread is returned.
     """
     blueprint, register_pages = create_dashboard(
         models=models, fuzzy_search=fuzzy_search
     )
     app = get_dash_app(blueprint=blueprint, use_pages=True)
-    register_pages(app)
+    register_pages()
     return run_app(app, port=port)
```

### Comparing `embedding_explorer-0.1.2/embedding_explorer/assets/favicon.ico` & `embedding_explorer-0.1.3/embedding_explorer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/blueprints/dashboard.py` & `embedding_explorer-0.1.3/embedding_explorer/blueprints/dashboard.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,20 +48,17 @@
         ]
     )
 
     main_blueprint = DashBlueprint()
     main_blueprint.layout = html.Div(dash.page_container)
     dashboard.register_callbacks(main_blueprint)
 
-    def register_pages(app: Dash) -> None:
-        print("Registering pages")
+    def register_pages():
         dash.register_page(
             "home", path="/", layout=dashboard.layout, redirect_from=["/home"]
         )
         for model_name, layout in pages.items():
             dash.register_page(
                 quote(model_name), "/" + quote(model_name), layout=layout
             )
-        print("Done registering pages")
 
-    print("Done creating dashbaord")
     return main_blueprint, register_pages
```

### Comparing `embedding_explorer-0.1.2/embedding_explorer/blueprints/explorer.py` & `embedding_explorer-0.1.3/embedding_explorer/blueprints/explorer.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/components/model_card.py` & `embedding_explorer-0.1.3/embedding_explorer/components/model_card.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/components/network.py` & `embedding_explorer-0.1.3/embedding_explorer/components/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/components/slider.py` & `embedding_explorer-0.1.3/embedding_explorer/components/slider.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/components/word_selector.py` & `embedding_explorer-0.1.3/embedding_explorer/components/word_selector.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/model.py` & `embedding_explorer-0.1.3/embedding_explorer/model.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/plots/network.py` & `embedding_explorer-0.1.3/embedding_explorer/plots/network.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/prepare/semkern.py` & `embedding_explorer-0.1.3/embedding_explorer/prepare/semkern.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/embedding_explorer/prepare/thumbnails.py` & `embedding_explorer-0.1.3/embedding_explorer/prepare/thumbnails.py`

 * *Files identical despite different names*

### Comparing `embedding_explorer-0.1.2/pyproject.toml` & `embedding_explorer-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length=79
 
 [tool.ruff]
 line-length=79
 
 [tool.poetry]
 name = "embedding-explorer"
-version = "0.1.2"
+version = "0.1.3"
 description = "Tools for interactive visual inspection of static word embedding models."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "embedding_explorer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `embedding_explorer-0.1.2/setup.py` & `embedding_explorer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'numpy>=1.23.0',
  'pandas>=1.5.2,<1.6.0',
  'scikit-learn>=1.1.0,<1.2.0',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'embedding-explorer',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Tools for interactive visual inspection of static word embedding models.',
     'long_description': '# embedding-explorer\nTools for interactive visual exploration of static word embedding models.\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `embedding_explorer-0.1.2/PKG-INFO` & `embedding_explorer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedding-explorer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for interactive visual inspection of static word embedding models.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

