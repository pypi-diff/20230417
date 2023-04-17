# Comparing `tmp/disvide-0.4.1.tar.gz` & `tmp/disvide-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disvide-0.4.1.tar", last modified: Mon Apr 17 14:44:05 2023, max compression
+gzip compressed data, was "disvide-0.4.2.tar", last modified: Mon Apr 17 14:54:55 2023, max compression
```

## Comparing `disvide-0.4.1.tar` & `disvide-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:44:05.057975 disvide-0.4.1/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.4.1/LICENSE
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3083 2023-04-17 14:44:05.057975 disvide-0.4.1/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2674 2023-04-17 12:38:38.000000 disvide-0.4.1/README.rst
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:44:05.057975 disvide-0.4.1/disvide.egg-info/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3083 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       47 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/entry_points.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/requires.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/top_level.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:44:05.057975 disvide-0.4.1/setup.cfg
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      789 2023-04-17 14:44:00.000000 disvide-0.4.1/setup.py
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:54:55.047971 disvide-0.4.2/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.4.2/LICENSE
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3180 2023-04-17 14:54:55.047971 disvide-0.4.2/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2771 2023-04-17 14:54:20.000000 disvide-0.4.2/README.rst
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:54:55.047971 disvide-0.4.2/disvide.egg-info/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3180 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       47 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/entry_points.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/requires.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/top_level.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:54:55.047971 disvide-0.4.2/setup.cfg
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      789 2023-04-17 14:50:56.000000 disvide-0.4.2/setup.py
```

### Comparing `disvide-0.4.1/LICENSE` & `disvide-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `disvide-0.4.1/PKG-INFO` & `disvide-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disvide
-Version: 0.4.1
+Version: 0.4.2
 Summary: Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.
 Home-page: https://github.com/Cored-Inc/disvide
 Author: Cored Developments
 Author-email: skyblockmohammed@gmail.com
 License: MIT
 Keywords: discord bot generator beginner
 Description-Content-Type: text/markdown
@@ -70,14 +70,16 @@
 2. Create a new branch with your changes: `git checkout -b my-feature-branch`.
 3. Commit your changes: `git commit -m "Added a new feature"`.
 4. Push to the branch: `git push origin my-feature-branch`.
 5. Create a pull request.
 
 ## Issues
 
+**We are aware that disvide might not work on windows always and we are working on fixing it.**
+
 If you encounter any issues while using Disvide, please report them on the [issues page](https://github.com/cored-developments-2023/disvide/issues). To create a new issue, follow these steps:
 
 1. Click on the "Issues" tab in the repository.
 2. Click on the "New Issue" button.
 3. Provide a descriptive title and detailed description of the issue.
 4. Click on the "Submit new issue" button.
```

### Comparing `disvide-0.4.1/README.rst` & `disvide-0.4.2/disvide.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: disvide
+Version: 0.4.2
+Summary: Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.
+Home-page: https://github.com/Cored-Inc/disvide
+Author: Cored Developments
+Author-email: skyblockmohammed@gmail.com
+License: MIT
+Keywords: discord bot generator beginner
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Disvide
 
 Disvide is a Discord bot generator that allows you to create a bot by answering a few questions. This project is created by Cored, Inc and led by FSCYT.
 
 ## Prerequisites
 
 Before using Disvide, make sure you have the following:
@@ -58,17 +70,19 @@
 2. Create a new branch with your changes: `git checkout -b my-feature-branch`.
 3. Commit your changes: `git commit -m "Added a new feature"`.
 4. Push to the branch: `git push origin my-feature-branch`.
 5. Create a pull request.
 
 ## Issues
 
+**We are aware that disvide might not work on windows always and we are working on fixing it.**
+
 If you encounter any issues while using Disvide, please report them on the [issues page](https://github.com/cored-developments-2023/disvide/issues). To create a new issue, follow these steps:
 
 1. Click on the "Issues" tab in the repository.
 2. Click on the "New Issue" button.
 3. Provide a descriptive title and detailed description of the issue.
 4. Click on the "Submit new issue" button.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `disvide-0.4.1/disvide.egg-info/PKG-INFO` & `disvide-0.4.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: disvide
-Version: 0.4.1
-Summary: Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.
-Home-page: https://github.com/Cored-Inc/disvide
-Author: Cored Developments
-Author-email: skyblockmohammed@gmail.com
-License: MIT
-Keywords: discord bot generator beginner
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Disvide
 
 Disvide is a Discord bot generator that allows you to create a bot by answering a few questions. This project is created by Cored, Inc and led by FSCYT.
 
 ## Prerequisites
 
 Before using Disvide, make sure you have the following:
@@ -70,17 +58,19 @@
 2. Create a new branch with your changes: `git checkout -b my-feature-branch`.
 3. Commit your changes: `git commit -m "Added a new feature"`.
 4. Push to the branch: `git push origin my-feature-branch`.
 5. Create a pull request.
 
 ## Issues
 
+**We are aware that disvide might not work on windows always and we are working on fixing it.**
+
 If you encounter any issues while using Disvide, please report them on the [issues page](https://github.com/cored-developments-2023/disvide/issues). To create a new issue, follow these steps:
 
 1. Click on the "Issues" tab in the repository.
 2. Click on the "New Issue" button.
 3. Provide a descriptive title and detailed description of the issue.
 4. Click on the "Submit new issue" button.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `disvide-0.4.1/setup.py` & `disvide-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name='disvide',
-    version='0.4.1',
+    version='0.4.2',
     license='MIT',
     author='Cored Developments',
     author_email='skyblockmohammed@gmail.com',
     packages=find_packages(),
     url='https://github.com/Cored-Inc/disvide',
     description='Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.',
     keywords='discord bot generator beginner',
```

