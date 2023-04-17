# Comparing `tmp/tabcompleter-1.1.0.tar.gz` & `tmp/tabcompleter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabcompleter-1.1.0.tar", last modified: Wed Dec  7 19:11:18 2022, max compression
+gzip compressed data, was "tabcompleter-1.2.0.tar", last modified: Mon Apr 17 17:53:33 2023, max compression
```

## Comparing `tabcompleter-1.1.0.tar` & `tabcompleter-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-07 19:11:18.759354 tabcompleter-1.1.0/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 tabcompleter-1.1.0/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1576 2022-11-28 07:10:47.000000 tabcompleter-1.1.0/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1704 2022-11-28 07:13:14.000000 tabcompleter-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1074 2022-11-28 07:13:28.000000 tabcompleter-1.1.0/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 tabcompleter-1.1.0/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3646 2022-12-07 19:11:18.759410 tabcompleter-1.1.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1480 2022-11-29 01:41:11.000000 tabcompleter-1.1.0/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      327 2022-11-28 07:12:39.000000 tabcompleter-1.1.0/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)      117 2022-12-07 19:11:18.759591 tabcompleter-1.1.0/setup.cfg
--rw-rw-r--   0 michael    (501) staff       (20)     5207 2022-12-07 17:24:51.000000 tabcompleter-1.1.0/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-07 19:11:18.758451 tabcompleter-1.1.0/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       28 2022-11-28 07:23:01.000000 tabcompleter-1.1.0/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-07 19:11:18.759160 tabcompleter-1.1.0/src/tabcompleter.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3646 2022-12-07 19:11:18.000000 tabcompleter-1.1.0/src/tabcompleter.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      341 2022-12-07 19:11:18.000000 tabcompleter-1.1.0/src/tabcompleter.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2022-12-07 19:11:18.000000 tabcompleter-1.1.0/src/tabcompleter.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      144 2022-12-07 19:11:18.000000 tabcompleter-1.1.0/src/tabcompleter.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       13 2022-12-07 19:11:18.000000 tabcompleter-1.1.0/src/tabcompleter.egg-info/top_level.txt
--rw-rw-r--   0 michael    (501) staff       (20)    12516 2022-12-07 17:52:27.000000 tabcompleter-1.1.0/src/tabcompleter.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-17 17:53:33.409340 tabcompleter-1.2.0/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 tabcompleter-1.2.0/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1576 2022-11-28 07:10:47.000000 tabcompleter-1.2.0/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1704 2022-11-28 07:13:14.000000 tabcompleter-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2022-11-28 07:13:28.000000 tabcompleter-1.2.0/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 tabcompleter-1.2.0/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3542 2023-04-17 17:53:33.409390 tabcompleter-1.2.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1480 2022-11-29 01:41:11.000000 tabcompleter-1.2.0/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      327 2022-11-28 07:12:39.000000 tabcompleter-1.2.0/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-17 17:53:33.409557 tabcompleter-1.2.0/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     5239 2023-04-17 17:52:50.000000 tabcompleter-1.2.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-17 17:53:33.408754 tabcompleter-1.2.0/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       28 2022-11-28 07:23:01.000000 tabcompleter-1.2.0/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-17 17:53:33.409243 tabcompleter-1.2.0/src/tabcompleter.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3542 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      341 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       45 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       13 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    12516 2023-01-19 19:17:09.000000 tabcompleter-1.2.0/src/tabcompleter.py
```

### Comparing `tabcompleter-1.1.0/.gitignore` & `tabcompleter-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.1.0/CODE_OF_CONDUCT.md` & `tabcompleter-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.1.0/CONTRIBUTING.md` & `tabcompleter-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.1.0/LICENSE` & `tabcompleter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.1.0/PKG-INFO` & `tabcompleter-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabcompleter
-Version: 1.1.0
+Version: 1.2.0
 Summary: tabcompleter --- Autocompletion in the Python console.
 Home-page: https://github.com/mdmintz/tabcompleter
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/tabcompleter/releases
@@ -23,15 +23,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -39,15 +38,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tabcompleter (📃) [![](https://img.shields.io/pypi/v/tabcompleter.svg)](https://pypi.python.org/pypi/tabcompleter)
 
 <img width="550" alt="tabcompleter" src="https://user-images.githubusercontent.com/6788579/204385233-838cbfbf-6ec7-4b45-812c-d0c2556a82e8.png">
```

### Comparing `tabcompleter-1.1.0/README.md` & `tabcompleter-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.1.0/setup.py` & `tabcompleter-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-"""
-*** tabcompleter ***
+"""*** tabcompleter ***
 Use the TAB key for autocompletion in the Python console.
-(Python 2.7+ and Python 3.6+)
-"""
-
+(Python 3.6+)"""
 from setuptools import setup, find_packages  # noqa
 import os
 import sys
 
 
 this_dir = os.path.abspath(os.path.dirname(__file__))
 long_description = None
@@ -29,42 +26,47 @@
     input_method = input
     if not sys.version_info[0] >= 3:
         input_method = raw_input  # noqa: F821
     confirm_text = ">>> Confirm release PUBLISH to PyPI? (yes/no): "
     reply = str(input_method(confirm_text)).lower().strip()
     if reply == "yes":
         print("\n*** Checking code health with flake8:\n")
-        os.system("python -m pip install 'flake8==5.0.4'")
+        if sys.version_info >= (3, 9):
+            os.system("python -m pip install 'flake8==6.0.0'")
+        else:
+            os.system("python -m pip install 'flake8==5.0.4'")
         flake8_status = os.system("flake8 --exclude=.eggs,temp")
         if flake8_status != 0:
             print("\nWARNING! Fix flake8 issues before publishing to PyPI!\n")
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'build>=0.9.0'")
+        os.system("python -m pip install --upgrade 'build>=0.10.0'")
+        print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'twine>=4.0.1'")
+        os.system("python -m pip install --upgrade 'twine>=4.0.2'")
         print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade tqdm")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
         os.system("python -m twine upload dist/*")  # Requires ~/.pypirc Keys
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="tabcompleter",
-    version="1.1.0",
+    version="1.2.0",
     description="tabcompleter --- Autocompletion in the Python console.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="tab completion console",
     url="https://github.com/mdmintz/tabcompleter",
     project_urls={
         "Changelog": "https://github.com/mdmintz/tabcompleter/releases",
@@ -88,15 +90,14 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
@@ -105,17 +106,16 @@
         "Topic :: Software Development",
         "Topic :: Software Development :: Debuggers",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",  # noqa: E501
+    python_requires=">=3.6",
     install_requires=[
-        'pyreadline;platform_system=="Windows" and python_version<"3.6"',
-        'pyreadline3;platform_system=="Windows" and python_version>="3.6"',
+        'pyreadline3;platform_system=="Windows"',
     ],
     setup_requires=[],
     include_package_data=True,
 )
 
 print("\n*** tabcompleter Installation Complete! ***\n")
```

### Comparing `tabcompleter-1.1.0/src/tabcompleter.egg-info/PKG-INFO` & `tabcompleter-1.2.0/src/tabcompleter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabcompleter
-Version: 1.1.0
+Version: 1.2.0
 Summary: tabcompleter --- Autocompletion in the Python console.
 Home-page: https://github.com/mdmintz/tabcompleter
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/tabcompleter/releases
@@ -23,15 +23,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -39,15 +38,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tabcompleter (📃) [![](https://img.shields.io/pypi/v/tabcompleter.svg)](https://pypi.python.org/pypi/tabcompleter)
 
 <img width="550" alt="tabcompleter" src="https://user-images.githubusercontent.com/6788579/204385233-838cbfbf-6ec7-4b45-812c-d0c2556a82e8.png">
```

### Comparing `tabcompleter-1.1.0/src/tabcompleter.py` & `tabcompleter-1.2.0/src/tabcompleter.py`

 * *Files identical despite different names*

