# Comparing `tmp/notebook-doc-0.1.6.tar.gz` & `tmp/notebook-doc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook-doc-0.1.6.tar", last modified: Tue Mar 21 13:41:03 2023, max compression
+gzip compressed data, was "notebook-doc-0.2.0.tar", last modified: Mon Apr 17 12:07:20 2023, max compression
```

## Comparing `notebook-doc-0.1.6.tar` & `notebook-doc-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 13:41:03.177594 notebook-doc-0.1.6/
--rw-rw-rw-   0        0        0     1089 2023-03-20 12:16:45.000000 notebook-doc-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2043 2023-03-21 13:41:03.177594 notebook-doc-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2023-03-20 15:04:37.000000 notebook-doc-0.1.6/README.md
--rw-rw-rw-   0        0        0     1186 2023-03-21 13:40:33.000000 notebook-doc-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 13:41:03.177594 notebook-doc-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-21 13:41:03.154933 notebook-doc-0.1.6/src/
--rw-rw-rw-   0        0        0       70 2023-03-21 13:40:33.000000 notebook-doc-0.1.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 13:41:03.158457 notebook-doc-0.1.6/src/notebook_doc/
--rw-rw-rw-   0        0        0       84 2023-03-21 13:40:33.000000 notebook-doc-0.1.6/src/notebook_doc/__init__.py
--rw-rw-rw-   0        0        0    12832 2023-03-20 19:05:37.000000 notebook-doc-0.1.6/src/notebook_doc/doc_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-21 13:41:03.176104 notebook-doc-0.1.6/src/notebook_doc.egg-info/
--rw-rw-rw-   0        0        0     2043 2023-03-21 13:41:03.000000 notebook-doc-0.1.6/src/notebook_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-03-21 13:41:03.000000 notebook-doc-0.1.6/src/notebook_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 13:41:03.000000 notebook-doc-0.1.6/src/notebook_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-03-21 13:41:03.000000 notebook-doc-0.1.6/src/notebook_doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-21 13:41:03.000000 notebook-doc-0.1.6/src/notebook_doc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/
+-rw-rw-rw-   0        0        0     1089 2023-03-20 12:16:45.000000 notebook-doc-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2037 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1459 2023-03-21 13:48:14.000000 notebook-doc-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1186 2023-04-17 12:04:44.000000 notebook-doc-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.021616 notebook-doc-0.2.0/src/
+-rw-rw-rw-   0        0        0       53 2023-04-17 12:04:44.000000 notebook-doc-0.2.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.033024 notebook-doc-0.2.0/src/notebook_doc/
+-rw-rw-rw-   0        0        0       88 2023-04-17 12:04:44.000000 notebook-doc-0.2.0/src/notebook_doc/__init__.py
+-rw-rw-rw-   0        0        0    14834 2023-04-17 11:55:40.000000 notebook-doc-0.2.0/src/notebook_doc/doc_functions.py
+-rw-rw-rw-   0        0        0     4827 2023-03-24 10:22:31.000000 notebook-doc-0.2.0/src/notebook_doc/test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:07:20.073508 notebook-doc-0.2.0/src/notebook_doc.egg-info/
+-rw-rw-rw-   0        0        0     2037 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-17 12:07:19.000000 notebook-doc-0.2.0/src/notebook_doc.egg-info/top_level.txt
```

### Comparing `notebook-doc-0.1.6/LICENSE` & `notebook-doc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook-doc-0.1.6/PKG-INFO` & `notebook-doc-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-doc
-Version: 0.1.6
+Version: 0.2.0
 Summary: A package to create documentation for functions in Databricks notebooks
 Author-email: Hiran Hasanka <hiranhasanka@gmail.com>
 Project-URL: Homepage, https://github.com/theSLWayne/notebook-doc
 Project-URL: Bug Tracker, https://github.com/theSLWayne/notebook-doc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,35 +22,35 @@
 
 ## Usage
 
 The package can be used as follows to generate documentation:
 
 1. Install the package (using PyPi - coming soon)
 2. Import the documentation generator function as follows:
-   ```{python}
+   ```python
    from notebook_doc import render_documentation
    ```
 3. Make sure that you have executed all cells that contain function definitions.
 4. Execute `render_documentation` function and provide the globals() dictionary to generate documentation as a HTML script.
 
 ### Example (in Databricks)
 
 Databricks `displayHTML` function can be directly used to display the HTML document returned by the `render_documentation` function.
 
-```{python}
+```python
 from notebook_doc import render_documentation
 
 displayHTML(render_documentation(globals(), module_name='Dummy Module'))
 ```
 
 ### Example (in other notebooks)
 
 HTML output from `render_documentation` function can be written on a local HTML file so that documentation can be displayed as a HTML file.
 
-```{python}
+```python
 from notebook_doc import render_documentation
 
 html_output = render_documentation(globals(), module_name='Dummy Module')
 
 with open('dummy_doc.html', 'w') as f:
     f.write(html_output)
 ```
```

### Comparing `notebook-doc-0.1.6/README.md` & `notebook-doc-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 ## Usage
 
 The package can be used as follows to generate documentation:
 
 1. Install the package (using PyPi - coming soon)
 2. Import the documentation generator function as follows:
-   ```{python}
+   ```python
    from notebook_doc import render_documentation
    ```
 3. Make sure that you have executed all cells that contain function definitions.
 4. Execute `render_documentation` function and provide the globals() dictionary to generate documentation as a HTML script.
 
 ### Example (in Databricks)
 
 Databricks `displayHTML` function can be directly used to display the HTML document returned by the `render_documentation` function.
 
-```{python}
+```python
 from notebook_doc import render_documentation
 
 displayHTML(render_documentation(globals(), module_name='Dummy Module'))
 ```
 
 ### Example (in other notebooks)
 
 HTML output from `render_documentation` function can be written on a local HTML file so that documentation can be displayed as a HTML file.
 
-```{python}
+```python
 from notebook_doc import render_documentation
 
 html_output = render_documentation(globals(), module_name='Dummy Module')
 
 with open('dummy_doc.html', 'w') as f:
     f.write(html_output)
 ```
```

### Comparing `notebook-doc-0.1.6/pyproject.toml` & `notebook-doc-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "Jinja2>=3.1.0", "docstring_parser>=0.15"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notebook-doc"
-version = "0.1.6"
+version = "0.2.0"
 dependencies = [
   "Jinja2>=3.1.0",
   "docstring_parser>=0.15"
 ]
 authors = [
   { name="Hiran Hasanka", email="hiranhasanka@gmail.com" },
 ]
@@ -22,15 +22,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/theSLWayne/notebook-doc"
 "Bug Tracker" = "https://github.com/theSLWayne/notebook-doc/issues"
 
 [tool.bumpver]
-current_version = "0.1.6"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `notebook-doc-0.1.6/src/notebook_doc/doc_functions.py` & `notebook-doc-0.2.0/src/notebook_doc/doc_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from docstring_parser import parse
 from jinja2 import Template
 import os
 import inspect
 from typing import get_type_hints, Union, get_origin, get_args
 
-
 def get_functions(globals_dict: dict) -> dict:
     """Get names and details of all functions executed in the given notebook
 
     Returns:
         Dictionary of function names and their details, indexed by function names.
     """
 
@@ -51,15 +50,18 @@
                     if get_origin(type_hints[param_name]) is Union:
                         types = [
                             type_hint.__name__
                             for type_hint in list(get_args(type_hints[param_name]))
                         ]
                         names_types[param_name] = " or ".join(types)
                     else:
-                        names_types[param_name] = type_hints[param_name].__name__
+                        try:
+                            names_types[param_name] = type_hints[param_name].__name__
+                        except AttributeError:
+                            names_types[param_name] = None
                 else:
                     names_types[param_name] = None
             func_type_list.append(names_types)
         else:
             # If not, add None
             func_type_list.append(None)
 
@@ -113,67 +115,81 @@
         # Parse docstring
         parsed_docstring = parse(docstring)
         # Create detailed profile for the function
         func_details = {
             "name": func_name,
             "head": func_head,
             "short_description": parsed_docstring.short_description,
-            "long_description": parsed_docstring.long_description,
+            "long_description": parsed_docstring.long_description.replace(
+                "\n", "<br>"
+            ).replace("\t", "&nbsp;&nbsp;&nbsp;&nbsp;")
+            if parsed_docstring.long_description
+            else parsed_docstring.long_description,
             "args": [
                 {
                     "arg_name": arg.arg_name,
                     "arg_type": types[arg.arg_name]
-                    if arg.arg_name in types 
+                    if arg.arg_name in types
                     else arg.type_name,
                     "is_optional": arg.is_optional,
                     "default": arg.default,
                     "description": arg.description,
                 }
                 for arg in parsed_docstring.params
             ]
             if parsed_docstring.params is not None
             else None,
             "raises": [
-                {"type": raises.type_name, "description": raises.description}
+                {
+                    "type": raises.type_name,
+                    "description": raises.description.replace("\n", "<br>").replace(
+                        "\t", "&nbsp;&nbsp;&nbsp;&nbsp;"
+                    ),
+                }
                 for raises in parsed_docstring.raises
             ]
             if parsed_docstring.raises is not None
             else None,
             "returns": {
                 "name": parsed_docstring.returns.return_name,
                 "type": ret_type
                 if ret_type is not None
                 else parsed_docstring.returns.type_name,
-                "description": parsed_docstring.returns.description,
+                "description": parsed_docstring.returns.description.replace(
+                    "\n", "<br>"
+                ).replace("\t", "&nbsp;&nbsp;&nbsp;&nbsp;"),
             }
             if parsed_docstring.returns is not None
             else None,
             "examples": [
                 {
-                    "description": example.description.replace("\n", "<br>"),
+                    "description": example.description.replace("\n", "<br>").replace(
+                        "\t", "&nbsp;&nbsp;&nbsp;&nbsp;"
+                    ),
                     "snippet": example.snippet,
                 }
                 for example in parsed_docstring.examples
             ]
             if parsed_docstring.examples is not None
             else None,
         }
         funcs.append(func_details)
 
     return funcs
 
 
-def generate_html(docstrings: list, title: str) -> str:
+def generate_html(docstrings: list, title: str, enable_links:bool) -> str:
     """Generate HTML file documenting the functions
 
     Generate HTML code that displays the functions and their docstrings as documentation.
 
     Args:
         docstrings: The list that includes details about each function
         title: Title of the module or the notebook
+        enable_links: Whether to enable links in the generated HTML document
 
     Returns:
         Rendered HTML document as a string.
     """
 
     # Create HTML template to display the documentation as a HTML file
     template = Template(
@@ -196,25 +212,39 @@
                     <h3 class="display-5"> {{ title }} - Documentation </h3>
                 </span>
             </div>
         </nav>
         <div class="container bg-light">
         <div class="row">
             <div class="col-3">
-                <div class="container sticky-top">
-                    <br>
-                    <h5>Functions List</h5>
-                    <div class="card" style="width: 18rem;">
-                        <ul class="list-group list-group-flush">
-                        {% for docstring in docstrings %}
-                            <li class="list-group-item">{{ docstring.name }}</a>
-                        {% endfor %}
-                        </ul>
+                {% if links %}
+                    <div class="container sticky-top">
+                        <br>
+                        <h5>Functions List</h5>
+                        <div class="card">
+                            <ul class="list-group list-group-flush">
+                            {% for docstring in docstrings %}
+                                <a href="#{{ docstring.name }}" style="text-decoration: none; color: black;"><li class="list-group-item">{{ docstring.name }}</li></a>
+                            {% endfor %}
+                            </ul>
+                        </div>
                     </div>
-                </div>
+                {% else %}
+                    <div class="container sticky-top">
+                        <br>
+                        <h5>Functions List</h5>
+                        <div class="card">
+                            <ul class="list-group list-group-flush">
+                            {% for docstring in docstrings %}
+                                <li class="list-group-item">{{ docstring.name }}</li>
+                            {% endfor %}
+                            </ul>
+                        </div>
+                    </div>
+                {% endif %}
             </div>
             <div class="col">
             <h5 class="display-6">Functions</h4>
             {% for docstring in docstrings %}
                 <div id="{{ docstring.name }}">
                 <p class="h3"> {{ docstring.name }} </p>
                 <div class="card">
@@ -259,15 +289,15 @@
                         {% if docstring.examples|length > 0 %}
                             <b>Examples:</b>
                             <ul class="list-group list-group-flush">
                                 {% for example in docstring.examples %}
                                 <li class="list-group-item">
                                     <div class="card">
                                         <div class="card-header">
-                                            {{ example.description }}
+                                            {{ example.description | safe }}
                                         </div>
                                     </div>
                                 </li>
                             {% endfor %}
                             </ul>
                         {% endif %}
                     </div>
@@ -287,27 +317,30 @@
     </body>
 
     </html>
     """
     )
 
     # Render the HTML template with function details
-    html = template.render({"docstrings": docstrings, "title": title})
+    html = template.render({"docstrings": docstrings, "title": title, "links": enable_links})
 
     return html
 
 
-def render_documentation(globals_dict: dict, module_name: str = None) -> str:
+def render_documentation(globals_dict: dict, module_name: str = None, enable_links: bool = False) -> str:
     """Render documentation for a given notebook.
 
     Entry point to all functions - this should be invoked inside of the notebook to generate documentation for a notebook.
 
     Args:
         globals_dict: globels() object
         module_name: Name of the module that is being documented. Optional. Will use 'Notebook' if not provided.
+        enable_links: Whether to enable links in the generated HTML document. This will include links for each function
+                    documentation on the left side of the HTML page. Recommended only if you are writing HTML documentation
+                    into a HTML file. These links will not work with Databricks generateHTML method. Optional. Defaulted to False.
 
     Returns:
         Documentation as HTML script
 
     Examples:
         Run the function as following with the name of the module:
 
@@ -321,10 +354,11 @@
     """
 
     docstrings = get_functions(globals_dict)
     parsed_docstrings = parse_docstrings(docstrings)
     html_docs = generate_html(
         docstrings=parsed_docstrings,
         title=module_name if module_name is not None else "Notebook",
+        enable_links=enable_links
     )
 
     return html_docs
```

### Comparing `notebook-doc-0.1.6/src/notebook_doc.egg-info/PKG-INFO` & `notebook-doc-0.2.0/src/notebook_doc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-doc
-Version: 0.1.6
+Version: 0.2.0
 Summary: A package to create documentation for functions in Databricks notebooks
 Author-email: Hiran Hasanka <hiranhasanka@gmail.com>
 Project-URL: Homepage, https://github.com/theSLWayne/notebook-doc
 Project-URL: Bug Tracker, https://github.com/theSLWayne/notebook-doc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,35 +22,35 @@
 
 ## Usage
 
 The package can be used as follows to generate documentation:
 
 1. Install the package (using PyPi - coming soon)
 2. Import the documentation generator function as follows:
-   ```{python}
+   ```python
    from notebook_doc import render_documentation
    ```
 3. Make sure that you have executed all cells that contain function definitions.
 4. Execute `render_documentation` function and provide the globals() dictionary to generate documentation as a HTML script.
 
 ### Example (in Databricks)
 
 Databricks `displayHTML` function can be directly used to display the HTML document returned by the `render_documentation` function.
 
-```{python}
+```python
 from notebook_doc import render_documentation
 
 displayHTML(render_documentation(globals(), module_name='Dummy Module'))
 ```
 
 ### Example (in other notebooks)
 
 HTML output from `render_documentation` function can be written on a local HTML file so that documentation can be displayed as a HTML file.
 
-```{python}
+```python
 from notebook_doc import render_documentation
 
 html_output = render_documentation(globals(), module_name='Dummy Module')
 
 with open('dummy_doc.html', 'w') as f:
     f.write(html_output)
 ```
```

