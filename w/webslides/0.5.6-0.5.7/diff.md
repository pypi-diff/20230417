# Comparing `tmp/webslides-0.5.6.tar.gz` & `tmp/webslides-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webslides-0.5.6.tar", last modified: Sun Apr 16 19:12:19 2023, max compression
+gzip compressed data, was "webslides-0.5.7.tar", last modified: Mon Apr 17 05:57:44 2023, max compression
```

## Comparing `webslides-0.5.6.tar` & `webslides-0.5.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.534754 webslides-0.5.6/
--rw-rw-rw-   0        0        0      193 2023-04-16 18:43:46.000000 webslides-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6621 2023-04-16 19:12:19.532754 webslides-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     6275 2023-04-16 18:40:55.000000 webslides-0.5.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 19:12:19.535756 webslides-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      537 2023-04-16 19:12:16.000000 webslides-0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.463756 webslides-0.5.6/webslides/
--rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.5.6/webslides/__init__.py
--rw-rw-rw-   0        0        0     5017 2023-04-16 18:37:59.000000 webslides-0.5.6/webslides/main.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.521757 webslides-0.5.6/webslides/modules/
--rw-rw-rw-   0        0        0     9881 2023-04-16 19:12:16.000000 webslides-0.5.6/webslides/modules/demo.py
--rw-rw-rw-   0        0        0     3800 2023-04-15 17:59:58.000000 webslides-0.5.6/webslides/modules/generate.py
--rw-rw-rw-   0        0        0     2383 2023-04-16 15:35:26.000000 webslides-0.5.6/webslides/modules/hello_world.py
--rw-rw-rw-   0        0        0     2824 2023-04-16 17:57:26.000000 webslides-0.5.6/webslides/modules/input_validations.py
--rw-rw-rw-   0        0        0     1724 2023-04-16 16:39:50.000000 webslides-0.5.6/webslides/modules/other.py
--rw-rw-rw-   0        0        0     2998 2023-04-16 18:40:55.000000 webslides-0.5.6/webslides/modules/pagination.py
--rw-rw-rw-   0        0        0     7774 2023-04-16 18:40:55.000000 webslides-0.5.6/webslides/modules/tohtml.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:12:19.495757 webslides-0.5.6/webslides.egg-info/
--rw-rw-rw-   0        0        0     6621 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 19:12:19.000000 webslides-0.5.6/webslides.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 05:57:44.105495 webslides-0.5.7/
+-rw-rw-rw-   0        0        0      193 2023-04-16 18:43:46.000000 webslides-0.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6763 2023-04-17 05:57:44.103495 webslides-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6421 2023-04-17 05:53:40.000000 webslides-0.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 05:57:44.105495 webslides-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      537 2023-04-17 05:46:17.000000 webslides-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 05:57:44.047496 webslides-0.5.7/webslides/
+-rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.5.7/webslides/__init__.py
+-rw-rw-rw-   0        0        0     5046 2023-04-17 05:57:42.000000 webslides-0.5.7/webslides/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 05:57:44.100500 webslides-0.5.7/webslides/modules/
+-rw-rw-rw-   0        0        0     9881 2023-04-16 19:12:16.000000 webslides-0.5.7/webslides/modules/demo.py
+-rw-rw-rw-   0        0        0     3800 2023-04-15 17:59:58.000000 webslides-0.5.7/webslides/modules/generate.py
+-rw-rw-rw-   0        0        0     2383 2023-04-16 15:35:26.000000 webslides-0.5.7/webslides/modules/hello_world.py
+-rw-rw-rw-   0        0        0     2824 2023-04-16 17:57:26.000000 webslides-0.5.7/webslides/modules/input_validations.py
+-rw-rw-rw-   0        0        0     1724 2023-04-16 16:39:50.000000 webslides-0.5.7/webslides/modules/other.py
+-rw-rw-rw-   0        0        0     2998 2023-04-16 18:40:55.000000 webslides-0.5.7/webslides/modules/pagination.py
+-rw-rw-rw-   0        0        0     7774 2023-04-16 18:40:55.000000 webslides-0.5.7/webslides/modules/tohtml.py
+drwxrwxrwx   0        0        0        0 2023-04-17 05:57:44.074496 webslides-0.5.7/webslides.egg-info/
+-rw-rw-rw-   0        0        0     6763 2023-04-17 05:57:43.000000 webslides-0.5.7/webslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-17 05:57:43.000000 webslides-0.5.7/webslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 05:57:43.000000 webslides-0.5.7/webslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 05:57:43.000000 webslides-0.5.7/webslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 05:57:43.000000 webslides-0.5.7/webslides.egg-info/top_level.txt
```

### Comparing `webslides-0.5.6/PKG-INFO` & `webslides-0.5.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.5.6
+Version: 0.5.7
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
+## Live demo
+Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
+
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
 - Allows for clickable content, like internal links for page navigation and external links to sources
 - Tooltips can be used
 - Allows interactivity with plotly figures
 - Allows interactivity with other elements, such as folium geographical maps
 - Can be shared by attachment in email
 - Very compact file size (no images)
-- **Update by rerun of Python code ðŸ¥³**
+- **Easy to update by rerun of Python code**
 
 ## Potential drawbacks
 
 Let's be honest, potential drawbacks may be:
 
 - Python is required to create presentations
 - Recipients cannot easily alter the presentation
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `webslides-0.5.6/README.md` & `webslides-0.5.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
+## Live demo
+Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
+
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
 - Allows for clickable content, like internal links for page navigation and external links to sources
 - Tooltips can be used
 - Allows interactivity with plotly figures
 - Allows interactivity with other elements, such as folium geographical maps
 - Can be shared by attachment in email
 - Very compact file size (no images)
-- **Update by rerun of Python code 🥳**
+- **Easy to update by rerun of Python code**
 
 ## Potential drawbacks
 
 Let's be honest, potential drawbacks may be:
 
 - Python is required to create presentations
 - Recipients cannot easily alter the presentation
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `webslides-0.5.6/setup.py` & `webslides-0.5.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="webslides",
-    version="0.5.6",
+    version="0.5.7",
     author="Derk-Jan Woltjer",
     author_email="derkjan.woltjer@gmail.com",
     description="Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     licence="MIT License",
     packages=find_packages(),
```

### Comparing `webslides-0.5.6/webslides/main.py` & `webslides-0.5.7/webslides/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import codecs
 import webbrowser
 
 from webslides.modules.tohtml import *
 from webslides.modules.generate import *
 from webslides.modules.pagination import *
 from webslides.modules.input_validations import *
@@ -120,16 +121,16 @@
         html = html.replace('<span></span></div>', '</div><span></span>')
 
     ###################
     ## HANDLE OUTPUT ##
     ###################
 
     # create output directory 'out' if not present
-    current_dir = os.path.dirname(os.path.abspath(__file__))
-    fpath = os.path.join(current_dir, '../wsout')
+    current_working_dir = os.path.dirname(os.path.abspath(sys.argv[0]))
+    fpath = os.path.join(current_working_dir, '/wsout')
 
     if not os.path.exists(fpath):
         os.makedirs(fpath)
 
     with codecs.open(f"{fpath}/{fname}", "w", encoding='utf-8') as f:
         f.write(html)
         print(f'output saved as {fname}')
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-import os import codecs import webbrowser from webslides.modules.tohtml import
-* from webslides.modules.generate import * from webslides.modules.pagination
-import * from webslides.modules.input_validations import * def create
-(content=None , title_page=None , fname='output.html' , open_in_browser=True ,
-show_index_page=False , show_highlights_page=False , show_topcat=True ,
-show_subcat=True , show_highlights_only=False): """ param pd (pagedata): list
-of lists with html strings or plotly fig objects ie. [[titlepage],
-[hl_page_title,hl_page_content], [index_page_title,index_page_content],
+import os import sys import codecs import webbrowser from
+webslides.modules.tohtml import * from webslides.modules.generate import * from
+webslides.modules.pagination import * from webslides.modules.input_validations
+import * def create(content=None , title_page=None , fname='output.html' ,
+open_in_browser=True , show_index_page=False , show_highlights_page=False ,
+show_topcat=True , show_subcat=True , show_highlights_only=False): """ param pd
+(pagedata): list of lists with html strings or plotly fig objects ie. [
+[titlepage],[hl_page_title,hl_page_content],
+[index_page_title,index_page_content],
 [content_page1_title,content_page1_comments,content_page1_fig],
 [content_page2_title,content_page2_comments,content_page2_fig]] param fname:
 str filename for output file. If not provided defaults to 'output.html') param
 write: bool, False will only output to screen, True will write file AND output
 to screen return: str html code """ # INPUT VALIDATIONS if title_page:
 title_error = validate_title_page(title_page) if title_error: print
 (title_error) return if content: content_error = validate_content(content) if
@@ -42,14 +43,14 @@
 html.replace('', '
 ') # insert content html html = content_to_html(html, page,
 show_topcat=show_topcat, show_subcat=show_subcat,
 show_index_page=show_index_page, show_highlights_page=show_highlights_page,
 show_navi=True) # close page html = html.replace('
 ', '
 ') ################### ## HANDLE OUTPUT ## ################### # create output
-directory 'out' if not present current_dir = os.path.dirname(os.path.abspath
-(__file__)) fpath = os.path.join(current_dir, '../wsout') if not os.path.exists
-(fpath): os.makedirs(fpath) with codecs.open(f"{fpath}/{fname}", "w",
-encoding='utf-8') as f: f.write(html) print(f'output saved as {fname}') if
-open_in_browser: # open in browser to check result htmlfile = f"{fpath}/
-{fname}" webbrowser.open(htmlfile) print(f'opened in browser {fname}') return
-None
+directory 'out' if not present current_working_dir = os.path.dirname
+(os.path.abspath(sys.argv[0])) fpath = os.path.join(current_working_dir, '/
+wsout') if not os.path.exists(fpath): os.makedirs(fpath) with codecs.open(f"
+{fpath}/{fname}", "w", encoding='utf-8') as f: f.write(html) print(f'output
+saved as {fname}') if open_in_browser: # open in browser to check result
+htmlfile = f"{fpath}/{fname}" webbrowser.open(htmlfile) print(f'opened in
+browser {fname}') return None
```

### Comparing `webslides-0.5.6/webslides/modules/demo.py` & `webslides-0.5.7/webslides/modules/demo.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.6/webslides/modules/generate.py` & `webslides-0.5.7/webslides/modules/generate.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.6/webslides/modules/hello_world.py` & `webslides-0.5.7/webslides/modules/hello_world.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.6/webslides/modules/input_validations.py` & `webslides-0.5.7/webslides/modules/input_validations.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.6/webslides/modules/other.py` & `webslides-0.5.7/webslides/modules/other.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.6/webslides/modules/pagination.py` & `webslides-0.5.7/webslides/modules/pagination.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.6/webslides/modules/tohtml.py` & `webslides-0.5.7/webslides/modules/tohtml.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.6/webslides.egg-info/PKG-INFO` & `webslides-0.5.7/webslides.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.5.6
+Version: 0.5.7
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
+## Live demo
+Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
+
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
 - Allows for clickable content, like internal links for page navigation and external links to sources
 - Tooltips can be used
 - Allows interactivity with plotly figures
 - Allows interactivity with other elements, such as folium geographical maps
 - Can be shared by attachment in email
 - Very compact file size (no images)
-- **Update by rerun of Python code ðŸ¥³**
+- **Easy to update by rerun of Python code**
 
 ## Potential drawbacks
 
 Let's be honest, potential drawbacks may be:
 
 - Python is required to create presentations
 - Recipients cannot easily alter the presentation
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

