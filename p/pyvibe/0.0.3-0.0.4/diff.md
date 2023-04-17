# Comparing `tmp/pyvibe-0.0.3.tar.gz` & `tmp/pyvibe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvibe-0.0.3.tar", last modified: Wed Mar 22 13:47:09 2023, max compression
+gzip compressed data, was "pyvibe-0.0.4.tar", last modified: Mon Apr 17 17:31:39 2023, max compression
```

## Comparing `pyvibe-0.0.3.tar` & `pyvibe-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:47:09.879741 pyvibe-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-22 13:46:53.000000 pyvibe-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-03-22 13:47:09.875741 pyvibe-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-03-22 13:46:53.000000 pyvibe-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-22 13:46:53.000000 pyvibe-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 13:47:09.879741 pyvibe-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:47:09.875741 pyvibe-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:47:09.875741 pyvibe-0.0.3/src/pyvibe/
--rw-r--r--   0 runner    (1001) docker     (123)   111603 2023-03-22 13:46:53.000000 pyvibe-0.0.3/src/pyvibe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-22 13:46:53.000000 pyvibe-0.0.3/src/pyvibe/component_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:47:09.875741 pyvibe-0.0.3/src/pyvibe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-03-22 13:47:09.000000 pyvibe-0.0.3/src/pyvibe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-22 13:47:09.000000 pyvibe-0.0.3/src/pyvibe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:47:09.000000 pyvibe-0.0.3/src/pyvibe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 13:47:09.000000 pyvibe-0.0.3/src/pyvibe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.293241 pyvibe-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 17:31:24.000000 pyvibe-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-17 17:31:39.293241 pyvibe-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-17 17:31:24.000000 pyvibe-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-17 17:31:24.000000 pyvibe-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:31:39.293241 pyvibe-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.289241 pyvibe-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.289241 pyvibe-0.0.4/src/pyvibe/
+-rw-r--r--   0 runner    (1001) docker     (123)   110451 2023-04-17 17:31:24.000000 pyvibe-0.0.4/src/pyvibe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-17 17:31:24.000000 pyvibe-0.0.4/src/pyvibe/component_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:31:39.293241 pyvibe-0.0.4/src/pyvibe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 17:31:39.000000 pyvibe-0.0.4/src/pyvibe.egg-info/top_level.txt
```

### Comparing `pyvibe-0.0.3/LICENSE` & `pyvibe-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvibe-0.0.3/PKG-INFO` & `pyvibe-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvibe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easily create styled web pages with Python
 Author-email: Zain Hoda <zain@pycob.com>
 Project-URL: Homepage, https://github.com/pycob/pyvibe
 Project-URL: Bug Tracker, https://github.com/pycob/pyvibe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyvibe Version: 0.0.3 Summary: Easily create styled
+Metadata-Version: 2.1 Name: pyvibe Version: 0.0.4 Summary: Easily create styled
 web pages with Python Author-email: Zain Hoda
 pycob.com> Project-URL: Homepage, https://github.com/pycob/pyvibe Project-URL:
 Bug Tracker, https://github.com/pycob/pyvibe/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # PyVibe https://
 www.pyvibe.com/ | [Examples](https://www.pyvibe.com/gallery.html) | [Use With
```

### Comparing `pyvibe-0.0.3/README.md` & `pyvibe-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyvibe-0.0.3/src/pyvibe/__init__.py` & `pyvibe-0.0.4/src/pyvibe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -897,35 +897,36 @@
 
   def to_html(self):
     return '''<hr class="my-5 border-gray-300 w-full">'''
 
 class Footer(Component):
   """Renders a footer
   """
-  def __init__(self, title: str = '', subtitle: str = '', logo: str = '', components: list = None):    
+  def __init__(self, title: str = '', subtitle: str = '', logo: str = '', link: str = '', components: list = None):    
     self.title = title
     self.subtitle = subtitle
     self.logo = logo
+    self.link = link
     # https://stackoverflow.com/questions/4841782/python-constructor-and-default-value
     self.components = components or []
     
 
   def __enter__(self):
     return self
 
   def __exit__(self, exc_type, exc_value, traceback):
     pass
 
   def to_html(self):
     return '''<footer class="text-gray-600 body-font">
     <div class="container px-5 mx-auto flex md:items-center lg:items-start md:flex-row md:flex-nowrap flex-wrap flex-col">
-        <div class="w-64 flex-shrink-0 md:mx-0 mx-auto text-center md:text-left">
-            <a class="flex title-font font-medium items-center md:justify-start justify-center text-gray-900 dark:text-white"><img class="object-scale-down h-10" src="''' + self.logo + '''"><span class="ml-3 text-xl">''' + self.title + '''</span></a>
+        <a href="''' + self.link + '''" class="w-64 flex-shrink-0 md:mx-0 mx-auto text-center md:text-left">
+            <span class="flex title-font font-medium items-center md:justify-start justify-center text-gray-900 dark:text-white"><img class="object-scale-down h-10" src="''' + self.logo + '''"><span class="ml-3 text-xl">''' + self.title + '''</span></span>
             <p class="mt-2 text-sm text-gray-500">''' + self.subtitle + '''</p>
-        </div>
+        </a>
         <div class="flex-grow flex flex-wrap md:pl-20 -mb-10 md:mt-0 mt-10 md:text-left text-center">
             ''' + '\n'.join(map(lambda x: x.to_html(), self.components)) + ''' 
         </div>
     </div>
 </footer>'''
 
   def add(self, component):
@@ -1601,27 +1602,20 @@
     ''' + self.svg + '''
     ''' + self.value + '''
 </li>'''
 
 class Navbar(Component):
   """Renders a navbar
   """
-  def __init__(self, title: str, logo: str = 'https://cdn.pycob.com/pyvibe.png', button_label: str = 'Sign In', button_url: str = '/auth/login', button_svg: str = '', components: list = None):    
+  def __init__(self, title: str, logo: str = 'https://cdn.pycob.com/pyvibe.png', components: list = None):    
     self.title = title
     self.logo = logo
-    self.button_label = button_label
-    self.button_url = button_url
-    self.button_svg = button_svg
     # https://stackoverflow.com/questions/4841782/python-constructor-and-default-value
     self.components = components or []
-    if button_label == "Sign In" and button_svg == "":
-        self.button_svg = '<svg fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="ml-1 h-4 w-4" viewBox="0 0 24 24"><path d="M5 12h14M12 5l7 7-7 7"></path></svg>'
     
-    if button_svg == "":
-        self.button_svg = '<svg fill="none" stroke="currentColor" stroke-width="1.5" class="ml-1 h-4 w-4" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true"><path stroke-linecap="round" stroke-linejoin="round" d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z"></path></svg>'
 
   def __enter__(self):
     return self
 
   def __exit__(self, exc_type, exc_value, traceback):
     pass
 
@@ -1642,18 +1636,15 @@
         <img src="''' + self.logo + '''" class="mr-3 h-6 sm:h-9" alt="Logo" />
         <span class="self-center whitespace-nowrap md:text-4xl font-semibold text-white">''' + self.title + '''</span>
       </a>
       <div class="flex md:order-2">
         <button onclick="toggleDarkMode()" type="button" class="mx-3 px-3 py-2 text-xs font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800 bg-gradient-to-br from-purple-600 to-blue-500 group-hover:from-purple-600 group-hover:to-blue-500">
             <svg id="sun" data-toggle-icon="sun" class="w-4 h-4" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M10 2a1 1 0 011 1v1a1 1 0 11-2 0V3a1 1 0 011-1zm4 8a4 4 0 11-8 0 4 4 0 018 0zm-.464 4.95l.707.707a1 1 0 001.414-1.414l-.707-.707a1 1 0 00-1.414 1.414zm2.12-10.607a1 1 0 010 1.414l-.706.707a1 1 0 11-1.414-1.414l.707-.707a1 1 0 011.414 0zM17 11a1 1 0 100-2h-1a1 1 0 100 2h1zm-7 4a1 1 0 011 1v1a1 1 0 11-2 0v-1a1 1 0 011-1zM5.05 6.464A1 1 0 106.465 5.05l-.708-.707a1 1 0 00-1.414 1.414l.707.707zm1.414 8.486l-.707.707a1 1 0 01-1.414-1.414l.707-.707a1 1 0 011.414 1.414zM4 11a1 1 0 100-2H3a1 1 0 000 2h1z" fill-rule="evenodd" clip-rule="evenodd"></path></svg>
             <svg id="moon" data-toggle-icon="moon" class="w-4 h-4 hidden" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M17.293 13.293A8 8 0 016.707 2.707a8.001 8.001 0 1010.586 10.586z"></path></svg>        </button>
-        <a type="button" href="''' + self.button_url + '''" id="pycob-login-button" class="mr-3 inline-flex items-center rounded-lg bg-blue-700 px-2 py-1 text-center text-xs font-medium text-white hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 md:mr-0">
-          ''' + self.button_label + '''
-          ''' + self.button_svg + '''
-        </a>
+
         <button onclick="toggleNav()" data-collapse-toggle="navbar-sticky" type="button" class="inline-flex items-center rounded-lg p-2 text-sm text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-white dark:hover:bg-gray-700 dark:focus:ring-gray-600 md:hidden" aria-controls="navbar-sticky" aria-expanded="true">
           <span class="sr-only">Open main menu</span>
           <svg class="h-6 w-6" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
         </button>
       </div>
       <div class="w-full items-center justify-between md:order-1 md:flex md:w-auto hidden" id="navbar-sticky">
         <ul class="mt-4 flex flex-col rounded-lg md:mt-0 md:flex-row md:space-x-8 md:border-0 md:text-sm md:font-medium">
@@ -1735,15 +1726,15 @@
 
   def to_html(self):
     return '''<a class="block rounded-lg py-2 pl-3 pr-4 text-white hover:bg-blue-800 md:p-2 ''' + self.classes + '''" href="''' + self.url + '''">''' + self.text + '''</a>'''
 
 class Page(Component):
   """A page is the top level component of a website. It contains the navbar, the main content, and the footer.
   """
-  def __init__(self, title: str = '', description: str = '', image: str = '', additional_head: str = '', navbar: Navbar = Navbar(title='PyVibe App'), footer: Footer = Footer(title='Made with PyVibe', logo='https://cdn.pycob.com/pyvibe.png'), sidebar: Sidebar = None, components: list = None):    
+  def __init__(self, title: str = '', description: str = '', image: str = '', additional_head: str = '', navbar: Navbar = Navbar(title='PyVibe App'), footer: Footer = Footer(title='Made with PyVibe', logo='https://cdn.pycob.com/pyvibe.png', link='https://www.pyvibe.com'), sidebar: Sidebar = None, components: list = None):    
     self.title = title
     self.description = description
     self.image = image
     self.additional_head = additional_head
     self.navbar = navbar
     self.footer = footer
     self.sidebar = sidebar
```

### Comparing `pyvibe-0.0.3/src/pyvibe.egg-info/PKG-INFO` & `pyvibe-0.0.4/src/pyvibe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvibe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easily create styled web pages with Python
 Author-email: Zain Hoda <zain@pycob.com>
 Project-URL: Homepage, https://github.com/pycob/pyvibe
 Project-URL: Bug Tracker, https://github.com/pycob/pyvibe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyvibe Version: 0.0.3 Summary: Easily create styled
+Metadata-Version: 2.1 Name: pyvibe Version: 0.0.4 Summary: Easily create styled
 web pages with Python Author-email: Zain Hoda
 pycob.com> Project-URL: Homepage, https://github.com/pycob/pyvibe Project-URL:
 Bug Tracker, https://github.com/pycob/pyvibe/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # PyVibe https://
 www.pyvibe.com/ | [Examples](https://www.pyvibe.com/gallery.html) | [Use With
```

