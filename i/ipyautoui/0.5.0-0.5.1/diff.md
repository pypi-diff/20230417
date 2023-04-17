# Comparing `tmp/ipyautoui-0.5.0.tar.gz` & `tmp/ipyautoui-0.5.1.tar.gz`

## Comparing `ipyautoui-0.5.0.tar` & `ipyautoui-0.5.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    31400 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    40881 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25164 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/LICENSE
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/README.md
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    40881 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25164 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/README.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/PKG-INFO
```

### Comparing `ipyautoui-0.5.0/src/ipyautoui/__init__.py` & `ipyautoui-0.5.1/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/_dev_sys_path_append.py` & `ipyautoui-0.5.1/src/ipyautoui/_dev_sys_path_append.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/_utils.py` & `ipyautoui-0.5.1/src/ipyautoui/_utils.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.1/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/_version.py` & `ipyautoui-0.5.1/src/ipyautoui/_version.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.1/src/ipyautoui/autodisplay.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     KWARGS_OPENPREVIEW,
     KWARGS_OPENFILE,
     KWARGS_OPENFOLDER,
     KWARGS_DISPLAY_ALL_FILES,
     KWARGS_COLLAPSE_ALL_FILES,
     KWARGS_HOME_DISPLAY_FILES,
 )
-
+from wcmatch import fnmatch
 import requests
 
 # from mf library
 # try:
 #     from xlsxtemplater import from_excel
 # except:
 #     pass
@@ -615,14 +615,15 @@
 
     d = DisplayObject.from_path(path1, renderers=user_file_renderers)
     d.order = ORDER_DEFAULT
     display(d)
 
 # +
 
+
 class AutoDisplay(tr.HasTraits):
     """
     displays the contents of a file in the notebook.
     comes with the following default renderers:
     DEFAULT_FILE_RENDERERS = {
         '.csv': csv_prev,
         '.json': json_prev,
@@ -643,14 +644,15 @@
         '.pdf': pdf_prev,
     }
     user_file_renderers can be passed to class provided they have the correct
     dict format: user_file_renderers = {'.ext': myrenderer}
     notice that the class allows for "compound" filetypes, especially useful for .json files
     if you want to display the data in a specific way.
     """
+
     def __init__(
         self,
         display_objects_actions: ty.List[DisplayObjectActions],
         patterns: ty.Union[
             str, ty.List, None
         ] = None,  # TODO: add pattern matching. currently only works with paths
         title: ty.Union[str, None] = None,
```

### Comparing `ipyautoui-0.5.0/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.1/src/ipyautoui/autodisplay_renderers.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.1/src/ipyautoui/autoipywidget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.1/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/autoui.py` & `ipyautoui-0.5.1/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.1/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.1/src/ipyautoui/autowidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.1/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/constants.py` & `ipyautoui-0.5.1/src/ipyautoui/constants.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo.py` & `ipyautoui-0.5.1/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/env.py` & `ipyautoui-0.5.1/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.1/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.1/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.1/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/autogrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/editgrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.1/src/ipyautoui/custom/workingdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/.gitignore` & `ipyautoui-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/LICENSE` & `ipyautoui-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/README.md` & `ipyautoui-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.0/pyproject.toml` & `ipyautoui-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "numpy",
     "openpyxl",            # for excel fiel viewer
     "pandas",
     "pydantic",
     "pytest",
     "PyYAML",
     "stringcase",
-    "traitlets",
     "wcmatch",
     "maplocal==0.1.1",
 ]
 
 [project.urls]
 Homepage = "https://github.com/maxfordham/ipyautoui"
```

### Comparing `ipyautoui-0.5.0/PKG-INFO` & `ipyautoui-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.5.0
+Version: 0.5.1
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,14 @@
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pydantic
 Requires-Dist: pytest
 Requires-Dist: pyyaml
 Requires-Dist: stringcase
-Requires-Dist: traitlets
 Requires-Dist: wcmatch
 Description-Content-Type: text/markdown
 
 # ipyautoui
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/maxfordham/ipyautoui/HEAD) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![PyPI version](https://badge.fury.io/py/ipyautoui.svg)](https://badge.fury.io/py/ipyautoui)
```

