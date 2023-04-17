# Comparing `tmp/to-pip-1.7.tar.gz` & `tmp/to-pip-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-pip-1.7.tar", last modified: Fri Apr  7 16:27:11 2023, max compression
+gzip compressed data, was "to-pip-1.9.2.tar", last modified: Mon Apr 17 00:21:36 2023, max compression
```

## Comparing `to-pip-1.7.tar` & `to-pip-1.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-07 16:27:11.806573 to-pip-1.7/
--rw-rw-r--   0 root         (0) root         (0)     2136 2023-04-07 16:27:11.806274 to-pip-1.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1974 2023-04-07 16:27:07.000000 to-pip-1.7/README.md
--rw-rw-r--   0 root         (0) root         (0)       38 2023-04-07 16:27:11.806646 to-pip-1.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      486 2023-04-07 16:27:07.000000 to-pip-1.7/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-07 16:27:11.805553 to-pip-1.7/to_pip.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2136 2023-04-07 16:27:11.000000 to-pip-1.7/to_pip.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      210 2023-04-07 16:27:11.000000 to-pip-1.7/to_pip.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-07 16:27:11.000000 to-pip-1.7/to_pip.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       40 2023-04-07 16:27:11.000000 to-pip-1.7/to_pip.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       56 2023-04-07 16:27:11.000000 to-pip-1.7/to_pip.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        7 2023-04-07 16:27:11.000000 to-pip-1.7/to_pip.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)     4471 2023-04-07 16:27:06.000000 to-pip-1.7/to_pip.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:21:36.230825 to-pip-1.9.2/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-04-17 00:21:36.230419 to-pip-1.9.2/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-04-17 00:21:36.000000 to-pip-1.9.2/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 00:21:36.230861 to-pip-1.9.2/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      488 2023-04-17 00:21:36.000000 to-pip-1.9.2/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:21:36.230278 to-pip-1.9.2/to_pip.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-04-17 00:21:36.000000 to-pip-1.9.2/to_pip.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      210 2023-04-17 00:21:36.000000 to-pip-1.9.2/to_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 00:21:36.000000 to-pip-1.9.2/to_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       40 2023-04-17 00:21:36.000000 to-pip-1.9.2/to_pip.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-04-17 00:21:36.000000 to-pip-1.9.2/to_pip.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        7 2023-04-17 00:21:36.000000 to-pip-1.9.2/to_pip.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4471 2023-04-17 00:21:36.000000 to-pip-1.9.2/to_pip.py
```

### Comparing `to-pip-1.7/PKG-INFO` & `to-pip-1.9.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
-Name: to-pip
-Version: 1.7
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # to-pip
 
 `to-pip` is a tool that makes it easy to convert a set of Python files into a Python package that can be uploaded to PyPI. It can also upload the package to PyPI for you, if you provide your PyPI credentials. 
 
 ## Usage
 
 ### Web Interface
 
+Github:
+[https://github.com/bohachu/to_pip](https://github.com/bohachu/to_pip)
+
+Web interface:
+[http://to-pip.falra.net](http://to-pip.falra.net)
+
 You can use the web interface of `to-pip` [here](https://to-pip-jqvkl3xr3a-uc.a.run.app). Simply upload your Python files, enter your package name and version, and click "Create Package". If you provide your PyPI credentials, you can also choose to upload the package to PyPI directly from the web interface.
 
 ### Command Line Interface
 
 You can also use the `to-pip` command-line tool to create a package from your Python files. To use it, simply install the `to-pip` package using pip:
 
 ```
@@ -52,9 +49,7 @@
 ### Example
 
 Let's say you have two Python files, `hello.py` and `world.py`, that you want to package into a package called `helloworld` with version `1.0.0`. Here's how you would use `to-pip` to create the package:
 
 ```
 python -m to_pip -n helloworld -v 1.0.0 hello.py world.py
 ```
-
-
```

### Comparing `to-pip-1.7/README.md` & `to-pip-1.9.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,30 @@
+Metadata-Version: 2.1
+Name: to-pip
+Version: 1.9.2
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # to-pip
 
 `to-pip` is a tool that makes it easy to convert a set of Python files into a Python package that can be uploaded to PyPI. It can also upload the package to PyPI for you, if you provide your PyPI credentials. 
 
 ## Usage
 
 ### Web Interface
 
+Github:
+[https://github.com/bohachu/to_pip](https://github.com/bohachu/to_pip)
+
+Web interface:
+[http://to-pip.falra.net](http://to-pip.falra.net)
+
 You can use the web interface of `to-pip` [here](https://to-pip-jqvkl3xr3a-uc.a.run.app). Simply upload your Python files, enter your package name and version, and click "Create Package". If you provide your PyPI credentials, you can also choose to upload the package to PyPI directly from the web interface.
 
 ### Command Line Interface
 
 You can also use the `to-pip` command-line tool to create a package from your Python files. To use it, simply install the `to-pip` package using pip:
 
 ```
@@ -43,7 +58,9 @@
 ### Example
 
 Let's say you have two Python files, `hello.py` and `world.py`, that you want to package into a package called `helloworld` with version `1.0.0`. Here's how you would use `to-pip` to create the package:
 
 ```
 python -m to_pip -n helloworld -v 1.0.0 hello.py world.py
 ```
+
+
```

### Comparing `to-pip-1.7/to_pip.egg-info/PKG-INFO` & `to-pip-1.9.2/to_pip.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 1.7
+Version: 1.9.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
 
 `to-pip` is a tool that makes it easy to convert a set of Python files into a Python package that can be uploaded to PyPI. It can also upload the package to PyPI for you, if you provide your PyPI credentials. 
 
 ## Usage
 
 ### Web Interface
 
+Github:
+[https://github.com/bohachu/to_pip](https://github.com/bohachu/to_pip)
+
+Web interface:
+[http://to-pip.falra.net](http://to-pip.falra.net)
+
 You can use the web interface of `to-pip` [here](https://to-pip-jqvkl3xr3a-uc.a.run.app). Simply upload your Python files, enter your package name and version, and click "Create Package". If you provide your PyPI credentials, you can also choose to upload the package to PyPI directly from the web interface.
 
 ### Command Line Interface
 
 You can also use the `to-pip` command-line tool to create a package from your Python files. To use it, simply install the `to-pip` package using pip:
 
 ```
```

### Comparing `to-pip-1.7/to_pip.py` & `to-pip-1.9.2/to_pip.py`

 * *Files identical despite different names*

