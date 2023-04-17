# Comparing `tmp/glinux-homedir-helper-0.0.1.tar.gz` & `tmp/glinux-homedir-helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glinux-homedir-helper-0.0.1.tar", last modified: Mon Apr 17 00:28:03 2023, max compression
+gzip compressed data, was "glinux-homedir-helper-0.0.2.tar", last modified: Mon Apr 17 01:46:16 2023, max compression
```

## Comparing `glinux-homedir-helper-0.0.1.tar` & `glinux-homedir-helper-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 00:28:03.115332 glinux-homedir-helper-0.0.1/
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      748 2023-04-17 00:28:03.115332 glinux-homedir-helper-0.0.1/PKG-INFO
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       63 2023-04-17 00:20:24.973022 glinux-homedir-helper-0.0.1/setup.cfg
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1582 2023-04-17 00:27:59.623269 glinux-homedir-helper-0.0.1/setup.py
+drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 01:46:16.623371 glinux-homedir-helper-0.0.2/
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      530 2023-04-17 01:46:16.623371 glinux-homedir-helper-0.0.2/PKG-INFO
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       33 2023-04-17 01:41:00.442723 glinux-homedir-helper-0.0.2/setup.cfg
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1097 2023-04-17 01:46:15.591356 glinux-homedir-helper-0.0.2/setup.py
```

### Comparing `glinux-homedir-helper-0.0.1/setup.py` & `glinux-homedir-helper-0.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from distutils.core import setup
 setup(
   name = 'glinux-homedir-helper',         # How you named your package folder (MyLib)
   packages = ['glinux-homedir-helper'],   # Chose the same as "name"
-  version = '0.0.1',      # Start with a small number and increase it with every change you make
-  license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
-  author = 'YOUR NAME',                   # Type in your name
-  author_email = 'your.email@domain.com',      # Type in your E-Mail
-  url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
+  version = '0.0.2',      # Start with a small number and increase it with every change you make
+  license='Proprietary',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
+  description = 'None',   # Give a short description about your library
+  author = 'Jarrah Bloomfield',                   # Type in your name
+  author_email = 'jarrahb@google.com',      # Type in your E-Mail
+  url = 'https://google.com',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
-  keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
+  keywords = [],
   install_requires=[     
       ],
   classifiers=[
-    'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-    'Intended Audience :: Developers',      # Define that your audience are developers
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',   # Again, pick a license
-    'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
+    'Development Status :: 7 - Inactive',
+    'Intended Audience :: Other Audience', 
+    'Topic :: Other/Nonlisted Topic',
+    'License :: Other/Proprietary License',
+    'Programming Language :: Python :: 3',
   ],
 )
```

