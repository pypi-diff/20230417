# Comparing `tmp/thinks_dash_components-0.3.4.tar.gz` & `tmp/thinks_dash_components-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinks_dash_components-0.3.4.tar", last modified: Fri Apr 14 08:37:02 2023, max compression
+gzip compressed data, was "thinks_dash_components-0.3.5.tar", last modified: Mon Apr 17 08:01:55 2023, max compression
```

## Comparing `thinks_dash_components-0.3.4.tar` & `thinks_dash_components-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:37:02.236989 thinks_dash_components-0.3.4/
--rw-rw-rw-   0        0        0        0 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      464 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4087 2023-04-14 08:37:02.236989 thinks_dash_components-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/README.md
--rw-rw-rw-   0        0        0     2320 2023-04-14 08:36:38.000000 thinks_dash_components-0.3.4/package.json
--rw-rw-rw-   0        0        0       42 2023-04-14 08:37:02.236989 thinks_dash_components-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-02-22 05:19:29.000000 thinks_dash_components-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:37:02.232001 thinks_dash_components-0.3.4/thinks_dash_components/
--rw-rw-rw-   0        0        0     1857 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/Alert.py
--rw-rw-rw-   0        0        0     1700 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/DesignableRadioItems.py
--rw-rw-rw-   0        0        0     2183 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/IndexedDB.py
--rw-rw-rw-   0        0        0     1088 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/InputNumber.py
--rw-rw-rw-   0        0        0     1092 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/IosScrollWrapper.py
--rw-rw-rw-   0        0        0     1913 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/LoadingWrapper.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/MobileDropdown.py
--rw-rw-rw-   0        0        0     2192 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/Notice.py
--rw-rw-rw-   0        0        0     1352 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/OperationObserver.py
--rw-rw-rw-   0        0        0     1388 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/Rotate.py
--rw-rw-rw-   0        0        0     1613 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/SelectableBox.py
--rw-rw-rw-   0        0        0     1343 2023-04-06 01:49:20.000000 thinks_dash_components-0.3.4/thinks_dash_components/StorageObserver.py
--rw-rw-rw-   0        0        0     1878 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/TouchableComponent.py
--rw-rw-rw-   0        0        0      999 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/UrlObserver.py
--rw-rw-rw-   0        0        0     1598 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/_ComponentTemplate.py
--rw-rw-rw-   0        0        0     2360 2023-02-22 05:17:07.000000 thinks_dash_components-0.3.4/thinks_dash_components/__init__.py
--rw-rw-rw-   0        0        0      899 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/_imports_.py
--rw-rw-rw-   0        0        0    44306 2023-04-14 08:36:52.000000 thinks_dash_components-0.3.4/thinks_dash_components/metadata.json
--rw-rw-rw-   0        0        0     2320 2023-04-14 08:36:51.000000 thinks_dash_components-0.3.4/thinks_dash_components/package-info.json
--rw-rw-rw-   0        0        0   124231 2023-04-14 08:36:50.000000 thinks_dash_components-0.3.4/thinks_dash_components/thinks_dash_components.min.js
--rw-rw-rw-   0        0        0      106 2023-04-14 08:36:50.000000 thinks_dash_components-0.3.4/thinks_dash_components/thinks_dash_components.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-14 08:37:02.235992 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/
--rw-rw-rw-   0        0        0     4087 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-14 08:37:02.000000 thinks_dash_components-0.3.4/thinks_dash_components.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 08:01:55.109531 thinks_dash_components-0.3.5/
+-rw-rw-rw-   0        0        0        0 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      453 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4087 2023-04-17 08:01:55.109531 thinks_dash_components-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2023-04-17 07:43:57.000000 thinks_dash_components-0.3.5/README.md
+-rw-rw-rw-   0        0        0     2309 2023-04-17 07:59:14.000000 thinks_dash_components-0.3.5/package.json
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:01:55.110532 thinks_dash_components-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:01:55.102530 thinks_dash_components-0.3.5/thinks_dash_components/
+-rw-rw-rw-   0        0        0     1857 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/Alert.py
+-rw-rw-rw-   0        0        0     1700 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/DesignableRadioItems.py
+-rw-rw-rw-   0        0        0     2183 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/IndexedDB.py
+-rw-rw-rw-   0        0        0     1088 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/InputNumber.py
+-rw-rw-rw-   0        0        0     1092 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/IosScrollWrapper.py
+-rw-rw-rw-   0        0        0     1913 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/LoadingWrapper.py
+-rw-rw-rw-   0        0        0     1458 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/MobileDropdown.py
+-rw-rw-rw-   0        0        0     2192 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/Notice.py
+-rw-rw-rw-   0        0        0     1352 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/OperationObserver.py
+-rw-rw-rw-   0        0        0     1388 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/Rotate.py
+-rw-rw-rw-   0        0        0     1613 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/SelectableBox.py
+-rw-rw-rw-   0        0        0     1304 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.5/thinks_dash_components/StorageObserver.py
+-rw-rw-rw-   0        0        0     1878 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/TouchableComponent.py
+-rw-rw-rw-   0        0        0      999 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/UrlObserver.py
+-rw-rw-rw-   0        0        0     1598 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/_ComponentTemplate.py
+-rw-rw-rw-   0        0        0     2273 2023-04-17 07:43:58.000000 thinks_dash_components-0.3.5/thinks_dash_components/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/_imports_.py
+-rw-rw-rw-   0        0        0    44448 2023-04-17 08:01:36.000000 thinks_dash_components-0.3.5/thinks_dash_components/metadata.json
+-rw-rw-rw-   0        0        0     2309 2023-04-17 08:01:35.000000 thinks_dash_components-0.3.5/thinks_dash_components/package-info.json
+-rw-rw-rw-   0        0        0   124273 2023-04-17 08:01:34.000000 thinks_dash_components-0.3.5/thinks_dash_components/thinks_dash_components.min.js
+-rw-rw-rw-   0        0        0      106 2023-04-17 08:01:34.000000 thinks_dash_components-0.3.5/thinks_dash_components/thinks_dash_components.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-17 08:01:55.108531 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/
+-rw-rw-rw-   0        0        0     4087 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-17 08:01:55.000000 thinks_dash_components-0.3.5/thinks_dash_components.egg-info/top_level.txt
```

### Comparing `thinks_dash_components-0.3.4/PKG-INFO` & `thinks_dash_components-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinks_dash_components
-Version: 0.3.4
+Version: 0.3.5
 Summary: Dash Extension Components for Smartphones
 Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
 License: MIT
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `thinks_dash_components-0.3.4/README.md` & `thinks_dash_components-0.3.5/thinks_dash_components.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: thinks-dash-components
+Version: 0.3.5
+Summary: Dash Extension Components for Smartphones
+Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
+License: MIT
+Classifier: Framework :: Dash
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Thinks Dash Components
 
 Thinks Dash Components is a Dash component library.
 
 Get started with:
 1. Install Dash and its dependencies: https://dash.plotly.com/installation
 2. Run `python usage.py`
```

### Comparing `thinks_dash_components-0.3.4/package.json` & `thinks_dash_components-0.3.5/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333332%*

 * *Differences: {"'dependencies'": "{'react-is': '^18.2.0', 'yaml': '^2.2.1'}", "'version'": "'0.3.5'"}*

```diff
@@ -1,14 +1,16 @@
 {
     "author": "thinkup-sol <s_matsumoto@thinkup-sol.co.jp>",
     "dependencies": {
         "async": "^3.2.4",
         "ramda": "^0.26.1",
         "react-icons": "^4.7.1",
-        "styled-components": "^5.3.6"
+        "react-is": "^18.2.0",
+        "styled-components": "^5.3.6",
+        "yaml": "^2.2.1"
     },
     "description": "Dash Extension Components for Smartphones",
     "devDependencies": {
         "@babel/core": "^7.5.4",
         "@babel/plugin-proposal-object-rest-spread": "^7.5.4",
         "@babel/preset-env": "^7.5.4",
         "@babel/preset-react": "^7.0.0",
@@ -54,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.4"
+    "version": "0.3.5"
 }
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/Alert.py` & `thinks_dash_components-0.3.5/thinks_dash_components/Alert.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/DesignableRadioItems.py` & `thinks_dash_components-0.3.5/thinks_dash_components/DesignableRadioItems.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/IndexedDB.py` & `thinks_dash_components-0.3.5/thinks_dash_components/IndexedDB.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/InputNumber.py` & `thinks_dash_components-0.3.5/thinks_dash_components/InputNumber.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/IosScrollWrapper.py` & `thinks_dash_components-0.3.5/thinks_dash_components/IosScrollWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/LoadingWrapper.py` & `thinks_dash_components-0.3.5/thinks_dash_components/LoadingWrapper.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/MobileDropdown.py` & `thinks_dash_components-0.3.5/thinks_dash_components/MobileDropdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 
 - id (string; optional)
 
 - className (string; optional)
 
 - clearable (boolean; default True)
 
+- disable (boolean; optional)
+
 - notfoundMsg (string; optional)
 
 - options (list; optional)
 
 - value (string | number; optional)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'thinks_dash_components'
     _type = 'MobileDropdown'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, options=Component.UNDEFINED, value=Component.UNDEFINED, notfoundMsg=Component.UNDEFINED, clearable=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'className', 'clearable', 'notfoundMsg', 'options', 'value']
+    def __init__(self, id=Component.UNDEFINED, className=Component.UNDEFINED, options=Component.UNDEFINED, value=Component.UNDEFINED, notfoundMsg=Component.UNDEFINED, clearable=Component.UNDEFINED, disable=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'className', 'clearable', 'disable', 'notfoundMsg', 'options', 'value']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'className', 'clearable', 'notfoundMsg', 'options', 'value']
+        self.available_properties = ['id', 'className', 'clearable', 'disable', 'notfoundMsg', 'options', 'value']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(MobileDropdown, self).__init__(**args)
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/Notice.py` & `thinks_dash_components-0.3.5/thinks_dash_components/Notice.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/OperationObserver.py` & `thinks_dash_components-0.3.5/thinks_dash_components/OperationObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/Rotate.py` & `thinks_dash_components-0.3.5/thinks_dash_components/Rotate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/SelectableBox.py` & `thinks_dash_components-0.3.5/thinks_dash_components/SelectableBox.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/StorageObserver.py` & `thinks_dash_components-0.3.5/thinks_dash_components/StorageObserver.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# AUTO GENERATED FILE - DO NOT EDIT
-
-from dash.development.base_component import Component, _explicitize_args
-
-
-class StorageObserver(Component):
-    """A StorageObserver component.
-
-
-Keyword arguments:
-
-- id (string; optional)
-
-- clear (boolean; default False)
-
-- interval (number; default 10000)
-
-- limit (number; required)"""
-    _children_props = []
-    _base_nodes = ['children']
-    _namespace = 'thinks_dash_components'
-    _type = 'StorageObserver'
-    @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, limit=Component.REQUIRED, interval=Component.UNDEFINED, clear=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'clear', 'interval', 'limit']
-        self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'clear', 'interval', 'limit']
-        self.available_wildcard_properties =            []
-        _explicit_args = kwargs.pop('_explicit_args')
-        _locals = locals()
-        _locals.update(kwargs)  # For wildcard attrs and excess named props
-        args = {k: _locals[k] for k in _explicit_args}
-
-        for k in ['limit']:
-            if k not in args:
-                raise TypeError(
-                    'Required argument `' + k + '` was not specified.')
-
-        super(StorageObserver, self).__init__(**args)
+# AUTO GENERATED FILE - DO NOT EDIT
+
+from dash.development.base_component import Component, _explicitize_args
+
+
+class StorageObserver(Component):
+    """A StorageObserver component.
+
+
+Keyword arguments:
+
+- id (string; optional)
+
+- clear (boolean; default False)
+
+- interval (number; default 10000)
+
+- limit (number; required)"""
+    _children_props = []
+    _base_nodes = ['children']
+    _namespace = 'thinks_dash_components'
+    _type = 'StorageObserver'
+    @_explicitize_args
+    def __init__(self, id=Component.UNDEFINED, limit=Component.REQUIRED, interval=Component.UNDEFINED, clear=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'clear', 'interval', 'limit']
+        self._valid_wildcard_attributes =            []
+        self.available_properties = ['id', 'clear', 'interval', 'limit']
+        self.available_wildcard_properties =            []
+        _explicit_args = kwargs.pop('_explicit_args')
+        _locals = locals()
+        _locals.update(kwargs)  # For wildcard attrs and excess named props
+        args = {k: _locals[k] for k in _explicit_args}
+
+        for k in ['limit']:
+            if k not in args:
+                raise TypeError(
+                    'Required argument `' + k + '` was not specified.')
+
+        super(StorageObserver, self).__init__(**args)
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/TouchableComponent.py` & `thinks_dash_components-0.3.5/thinks_dash_components/TouchableComponent.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/UrlObserver.py` & `thinks_dash_components-0.3.5/thinks_dash_components/UrlObserver.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/_ComponentTemplate.py` & `thinks_dash_components-0.3.5/thinks_dash_components/_ComponentTemplate.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/__init__.py` & `thinks_dash_components-0.3.5/thinks_dash_components/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from __future__ import print_function as _
-
-import os as _os
-import sys as _sys
-import json
-
-import dash as _dash
-
-# noinspection PyUnresolvedReferences
-from ._imports_ import *
-from ._imports_ import __all__
-
-if not hasattr(_dash, '__plotly_dash') and not hasattr(_dash, 'development'):
-    print('Dash was not successfully imported. '
-          'Make sure you don\'t have a file '
-          'named \n"dash.py" in your current directory.', file=_sys.stderr)
-    _sys.exit(1)
-
-_basepath = _os.path.dirname(__file__)
-_filepath = _os.path.abspath(_os.path.join(_basepath, 'package-info.json'))
-with open(_filepath) as f:
-    package = json.load(f)
-
-package_name = package['name'].replace(' ', '_').replace('-', '_')
-__version__ = package['version']
-
-_current_path = _os.path.dirname(_os.path.abspath(__file__))
-
-_this_module = _sys.modules[__name__]
-
-async_resources = []
-
-_js_dist = []
-
-_js_dist.extend(
-    [
-        {
-            "relative_package_path": "async-{}.js".format(async_resource),
-            "external_url": (
-                "https://unpkg.com/{0}@{2}"
-                "/{1}/async-{3}.js"
-            ).format(package_name, __name__, __version__, async_resource),
-            "namespace": package_name,
-            "async": True,
-        }
-        for async_resource in async_resources
-    ]
-)
-
-# TODO: Figure out if unpkg link works
-_js_dist.extend(
-    [
-        {
-            "relative_package_path": "async-{}.js.map".format(async_resource),
-            "external_url": (
-                "https://unpkg.com/{0}@{2}"
-                "/{1}/async-{3}.js.map"
-            ).format(package_name, __name__, __version__, async_resource),
-            "namespace": package_name,
-            "dynamic": True,
-        }
-        for async_resource in async_resources
-    ]
-)
-
-_js_dist.extend(
-    [
-        {
-            'relative_package_path': 'thinks_dash_components.min.js',
-    
-            'namespace': package_name
-        },
-        {
-            'relative_package_path': 'thinks_dash_components.min.js.map',
-    
-            'namespace': package_name,
-            'dynamic': True
-        }
-    ]
-)
-
-_css_dist = []
-
-
-for _component in __all__:
-    setattr(locals()[_component], '_js_dist', _js_dist)
-    setattr(locals()[_component], '_css_dist', _css_dist)
+from __future__ import print_function as _
+
+import os as _os
+import sys as _sys
+import json
+
+import dash as _dash
+
+# noinspection PyUnresolvedReferences
+from ._imports_ import *
+from ._imports_ import __all__
+
+if not hasattr(_dash, '__plotly_dash') and not hasattr(_dash, 'development'):
+    print('Dash was not successfully imported. '
+          'Make sure you don\'t have a file '
+          'named \n"dash.py" in your current directory.', file=_sys.stderr)
+    _sys.exit(1)
+
+_basepath = _os.path.dirname(__file__)
+_filepath = _os.path.abspath(_os.path.join(_basepath, 'package-info.json'))
+with open(_filepath) as f:
+    package = json.load(f)
+
+package_name = package['name'].replace(' ', '_').replace('-', '_')
+__version__ = package['version']
+
+_current_path = _os.path.dirname(_os.path.abspath(__file__))
+
+_this_module = _sys.modules[__name__]
+
+async_resources = []
+
+_js_dist = []
+
+_js_dist.extend(
+    [
+        {
+            "relative_package_path": "async-{}.js".format(async_resource),
+            "external_url": (
+                "https://unpkg.com/{0}@{2}"
+                "/{1}/async-{3}.js"
+            ).format(package_name, __name__, __version__, async_resource),
+            "namespace": package_name,
+            "async": True,
+        }
+        for async_resource in async_resources
+    ]
+)
+
+# TODO: Figure out if unpkg link works
+_js_dist.extend(
+    [
+        {
+            "relative_package_path": "async-{}.js.map".format(async_resource),
+            "external_url": (
+                "https://unpkg.com/{0}@{2}"
+                "/{1}/async-{3}.js.map"
+            ).format(package_name, __name__, __version__, async_resource),
+            "namespace": package_name,
+            "dynamic": True,
+        }
+        for async_resource in async_resources
+    ]
+)
+
+_js_dist.extend(
+    [
+        {
+            'relative_package_path': 'thinks_dash_components.min.js',
+    
+            'namespace': package_name
+        },
+        {
+            'relative_package_path': 'thinks_dash_components.min.js.map',
+    
+            'namespace': package_name,
+            'dynamic': True
+        }
+    ]
+)
+
+_css_dist = []
+
+
+for _component in __all__:
+    setattr(locals()[_component], '_js_dist', _js_dist)
+    setattr(locals()[_component], '_css_dist', _css_dist)
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/_imports_.py` & `thinks_dash_components-0.3.5/thinks_dash_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/metadata.json` & `thinks_dash_components-0.3.5/thinks_dash_components/metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994419642857143%*

 * *Differences: {"'src/lib/components/MobileDropdown.react.js'": "{'props': {'disable': OrderedDict([('type', "*

 * *                                                 "OrderedDict([('name', 'bool')])), ('required', "*

 * *                                                 "False), ('description', '')])}}"}*

```diff
@@ -992,14 +992,21 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "bool"
                 }
             },
+            "disable": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
             "id": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/package-info.json` & `thinks_dash_components-0.3.5/thinks_dash_components/package-info.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333332%*

 * *Differences: {"'dependencies'": "{'react-is': '^18.2.0', 'yaml': '^2.2.1'}", "'version'": "'0.3.5'"}*

```diff
@@ -1,14 +1,16 @@
 {
     "author": "thinkup-sol <s_matsumoto@thinkup-sol.co.jp>",
     "dependencies": {
         "async": "^3.2.4",
         "ramda": "^0.26.1",
         "react-icons": "^4.7.1",
-        "styled-components": "^5.3.6"
+        "react-is": "^18.2.0",
+        "styled-components": "^5.3.6",
+        "yaml": "^2.2.1"
     },
     "description": "Dash Extension Components for Smartphones",
     "devDependencies": {
         "@babel/core": "^7.5.4",
         "@babel/plugin-proposal-object-rest-spread": "^7.5.4",
         "@babel/preset-env": "^7.5.4",
         "@babel/preset-react": "^7.0.0",
@@ -54,9 +56,9 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "pug": "pug --out ./doc/reference --watch ./doc/reference/src --pretty",
         "start": "webpack-serve --host localhost --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.3.4"
+    "version": "0.3.5"
 }
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components/thinks_dash_components.min.js` & `thinks_dash_components-0.3.5/thinks_dash_components/thinks_dash_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(o()),
                 r = i(e);
             if (!t) return r;
             var n = r.split("/"),
                 a = n.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_3_4m1681461408"), n.splice(-1, 1, a.join(".")), n.join("/")
+            return a.splice(1, 0, "v0_3_5m1681718492"), n.splice(-1, 1, a.join(".")), n.join("/")
         }
     }
     return r(r.s = 13)
 }([function(e, t) {
     e.exports = window.PropTypes
 }, function(e, t) {
     e.exports = window.React
@@ -3755,18 +3755,20 @@
                 }, t.wrapRef = h.a.createRef(), t.listRef = h.a.createRef(), t.valueRef = h.a.createRef(), t.options = t.props.options, t.isScroll = !1, t.isTouch = !1, t.interval = 300, t.pos = 1, t.id = Math.random().toString(32).substring(2), t.closeStyle = {
                     display: "none"
                 }, t.toggle = t.toggle.bind(Ye(t)), t.select = t.select.bind(Ye(t)), t.clear = t.clear.bind(Ye(t)), t.close = t.close.bind(Ye(t)), t.scroll = t.scroll.bind(Ye(t)), t.touchStart = t.touchStart.bind(Ye(t)), t.touchEnd = t.touchEnd.bind(Ye(t)), t
             }
             return t = i, (r = [{
                 key: "toggle",
                 value: function() {
-                    var e = getComputedStyle(this.listRef.current).maxHeight;
-                    Number(e.replace("px", "")) <= 0 || (this.setState({
-                        open: !this.state.open
-                    }), this.setListPos(!this.state.open))
+                    if (!this.props.disable) {
+                        var e = getComputedStyle(this.listRef.current).maxHeight;
+                        Number(e.replace("px", "")) <= 0 || (this.setState({
+                            open: !this.state.open
+                        }), this.setListPos(!this.state.open))
+                    }
                 }
             }, {
                 key: "select",
                 value: function(e) {
                     var t = e.currentTarget.dataset;
                     console.log("-- MOBILE DROPDOWN SELECT", JSON.stringify(t)), this.setState({
                         open: !1,
@@ -4099,15 +4101,16 @@
     }, ft.propTypes = {
         id: p.a.string,
         className: p.a.string,
         options: p.a.array,
         value: p.a.oneOfType([p.a.string, p.a.number]),
         notfoundMsg: p.a.string,
         clearable: p.a.bool,
-        setProps: p.a.func
+        setProps: p.a.func,
+        disable: p.a.bool
     };
     var Et = y.a.div(Je || (Je = Ot(["\n    position: fixed;\n    top: 0;\n    left: 0;\n    width: 100%;\n    height: 100%;\n"]))),
         Pt = y.a.div.attrs((function(e) {
             return {
                 iconColor: e.iconColor
             }
         }))(Ke || (Ke = Ot(["\n    width: 30px;\n    height: 30px;\n    position: relative;\n\n    svg {\n        width: 100%;\n        height: 100%;\n        color: ", ";\n    }\n"])), (function(e) {
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components.egg-info/PKG-INFO` & `thinks_dash_components-0.3.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,106 +1,96 @@
-Metadata-Version: 2.1
-Name: thinks-dash-components
-Version: 0.3.4
-Summary: Dash Extension Components for Smartphones
-Author: thinkup-sol <s_matsumoto@thinkup-sol.co.jp>
-License: MIT
-Classifier: Framework :: Dash
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Thinks Dash Components
-
-Thinks Dash Components is a Dash component library.
-
-Get started with:
-1. Install Dash and its dependencies: https://dash.plotly.com/installation
-2. Run `python usage.py`
-3. Visit http://localhost:8050 in your web browser
-
-## Contributing
-
-See [CONTRIBUTING.md](./CONTRIBUTING.md)
-
-### Install dependencies
-
-If you have selected install_dependencies during the prompt, you can skip this part.
-
-1. Install npm packages
-    ```
-    $ npm install
-    ```
-2. Create a virtual env and activate.
-    ```
-    $ virtualenv venv
-    $ . venv/bin/activate
-    ```
-    _Note: venv\Scripts\activate for windows_
-
-3. Install python packages required to build components.
-    ```
-    $ pip install -r requirements.txt
-    ```
-4. Install the python packages for testing (optional)
-    ```
-    $ pip install -r tests/requirements.txt
-    ```
-
-### Write your component code in `src/lib/components/ThinksDashComponents.react.js`.
-
-- The demo app is in `src/demo` and you will import your example component code into your demo app.
-- Test your code in a Python environment:
-    1. Build your code
-        ```
-        $ npm run build
-        ```
-    2. Run and modify the `usage.py` sample dash app:
-        ```
-        $ python usage.py
-        ```
-- Write tests for your component.
-    - A sample test is available in `tests/test_usage.py`, it will load `usage.py` and you can then automate interactions with selenium.
-    - Run the tests with `$ pytest tests`.
-    - The Dash team uses these types of integration tests extensively. Browse the Dash component code on GitHub for more examples of testing (e.g. https://github.com/plotly/dash-core-components)
-- Add custom styles to your component by putting your custom CSS files into your distribution folder (`thinks_dash_components`).
-    - Make sure that they are referenced in `MANIFEST.in` so that they get properly included when you're ready to publish your component.
-    - Make sure the stylesheets are added to the `_css_dist` dict in `thinks_dash_components/__init__.py` so dash will serve them automatically when the component suite is requested.
-- [Review your code](./review_checklist.md)
-
-### Create a production build and publish:
-
-1. Build your code:
-    ```
-    $ npm run build
-    ```
-2. Create a Python distribution
-    ```
-    $ python setup.py sdist bdist_wheel
-    ```
-    This will create source and wheel distribution in the generated the `dist/` folder.
-    See [PyPA](https://packaging.python.org/guides/distributing-packages-using-setuptools/#packaging-your-project)
-    for more information.
-
-3. Test your tarball by copying it into a new environment and installing it locally:
-    ```
-    $ pip install thinks_dash_components-0.0.1.tar.gz
-    ```
-
-4. If it works, then you can publish the component to NPM and PyPI:
-    1. Publish on PyPI
-        ```
-        $ twine upload dist/*
-        ```
-    2. Cleanup the dist folder (optional)
-        ```
-        $ rm -rf dist
-        ```
-    3. Publish on NPM (Optional if chosen False in `publish_on_npm`)
-        ```
-        $ npm publish
-        ```
-        _Publishing your component to NPM will make the JavaScript bundles available on the unpkg CDN. By default, Dash serves the component library's CSS and JS locally, but if you choose to publish the package to NPM you can set `serve_locally` to `False` and you may see faster load times._
-
-5. Share your component with the community! https://community.plotly.com/c/dash
-    1. Publish this repository to GitHub
-    2. Tag your GitHub repository with the plotly-dash tag so that it appears here: https://github.com/topics/plotly-dash
-    3. Create a post in the Dash community forum: https://community.plotly.com/c/dash
+# Thinks Dash Components
+
+Thinks Dash Components is a Dash component library.
+
+Get started with:
+1. Install Dash and its dependencies: https://dash.plotly.com/installation
+2. Run `python usage.py`
+3. Visit http://localhost:8050 in your web browser
+
+## Contributing
+
+See [CONTRIBUTING.md](./CONTRIBUTING.md)
+
+### Install dependencies
+
+If you have selected install_dependencies during the prompt, you can skip this part.
+
+1. Install npm packages
+    ```
+    $ npm install
+    ```
+2. Create a virtual env and activate.
+    ```
+    $ virtualenv venv
+    $ . venv/bin/activate
+    ```
+    _Note: venv\Scripts\activate for windows_
+
+3. Install python packages required to build components.
+    ```
+    $ pip install -r requirements.txt
+    ```
+4. Install the python packages for testing (optional)
+    ```
+    $ pip install -r tests/requirements.txt
+    ```
+
+### Write your component code in `src/lib/components/ThinksDashComponents.react.js`.
+
+- The demo app is in `src/demo` and you will import your example component code into your demo app.
+- Test your code in a Python environment:
+    1. Build your code
+        ```
+        $ npm run build
+        ```
+    2. Run and modify the `usage.py` sample dash app:
+        ```
+        $ python usage.py
+        ```
+- Write tests for your component.
+    - A sample test is available in `tests/test_usage.py`, it will load `usage.py` and you can then automate interactions with selenium.
+    - Run the tests with `$ pytest tests`.
+    - The Dash team uses these types of integration tests extensively. Browse the Dash component code on GitHub for more examples of testing (e.g. https://github.com/plotly/dash-core-components)
+- Add custom styles to your component by putting your custom CSS files into your distribution folder (`thinks_dash_components`).
+    - Make sure that they are referenced in `MANIFEST.in` so that they get properly included when you're ready to publish your component.
+    - Make sure the stylesheets are added to the `_css_dist` dict in `thinks_dash_components/__init__.py` so dash will serve them automatically when the component suite is requested.
+- [Review your code](./review_checklist.md)
+
+### Create a production build and publish:
+
+1. Build your code:
+    ```
+    $ npm run build
+    ```
+2. Create a Python distribution
+    ```
+    $ python setup.py sdist bdist_wheel
+    ```
+    This will create source and wheel distribution in the generated the `dist/` folder.
+    See [PyPA](https://packaging.python.org/guides/distributing-packages-using-setuptools/#packaging-your-project)
+    for more information.
+
+3. Test your tarball by copying it into a new environment and installing it locally:
+    ```
+    $ pip install thinks_dash_components-0.0.1.tar.gz
+    ```
+
+4. If it works, then you can publish the component to NPM and PyPI:
+    1. Publish on PyPI
+        ```
+        $ twine upload dist/*
+        ```
+    2. Cleanup the dist folder (optional)
+        ```
+        $ rm -rf dist
+        ```
+    3. Publish on NPM (Optional if chosen False in `publish_on_npm`)
+        ```
+        $ npm publish
+        ```
+        _Publishing your component to NPM will make the JavaScript bundles available on the unpkg CDN. By default, Dash serves the component library's CSS and JS locally, but if you choose to publish the package to NPM you can set `serve_locally` to `False` and you may see faster load times._
+
+5. Share your component with the community! https://community.plotly.com/c/dash
+    1. Publish this repository to GitHub
+    2. Tag your GitHub repository with the plotly-dash tag so that it appears here: https://github.com/topics/plotly-dash
+    3. Create a post in the Dash community forum: https://community.plotly.com/c/dash
```

### Comparing `thinks_dash_components-0.3.4/thinks_dash_components.egg-info/SOURCES.txt` & `thinks_dash_components-0.3.5/thinks_dash_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

