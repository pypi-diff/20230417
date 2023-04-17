# Comparing `tmp/disvide-0.4.2.tar.gz` & `tmp/disvide-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disvide-0.4.2.tar", last modified: Mon Apr 17 14:54:55 2023, max compression
+gzip compressed data, was "disvide-0.5.0.tar", last modified: Mon Apr 17 19:30:51 2023, max compression
```

## Comparing `disvide-0.4.2.tar` & `disvide-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:54:55.047971 disvide-0.4.2/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.4.2/LICENSE
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3180 2023-04-17 14:54:55.047971 disvide-0.4.2/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2771 2023-04-17 14:54:20.000000 disvide-0.4.2/README.rst
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:54:55.047971 disvide-0.4.2/disvide.egg-info/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3180 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       47 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/entry_points.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/requires.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:54:55.000000 disvide-0.4.2/disvide.egg-info/top_level.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:54:55.047971 disvide-0.4.2/setup.cfg
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      789 2023-04-17 14:50:56.000000 disvide-0.4.2/setup.py
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 19:30:51.957975 disvide-0.5.0/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.5.0/LICENSE
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3763 2023-04-17 19:30:51.957975 disvide-0.5.0/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3354 2023-04-17 19:30:09.000000 disvide-0.5.0/README.rst
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 19:30:51.957975 disvide-0.5.0/disvide.egg-info/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3763 2023-04-17 19:30:51.000000 disvide-0.5.0/disvide.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 19:30:51.000000 disvide-0.5.0/disvide.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 19:30:51.000000 disvide-0.5.0/disvide.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       47 2023-04-17 19:30:51.000000 disvide-0.5.0/disvide.egg-info/entry_points.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 19:30:51.000000 disvide-0.5.0/disvide.egg-info/requires.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 19:30:51.000000 disvide-0.5.0/disvide.egg-info/top_level.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 19:30:51.957975 disvide-0.5.0/setup.cfg
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      789 2023-04-17 19:28:51.000000 disvide-0.5.0/setup.py
```

### Comparing `disvide-0.4.2/LICENSE` & `disvide-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `disvide-0.4.2/PKG-INFO` & `disvide-0.5.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,35 @@
-Metadata-Version: 2.1
-Name: disvide
-Version: 0.4.2
-Summary: Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.
-Home-page: https://github.com/Cored-Inc/disvide
-Author: Cored Developments
-Author-email: skyblockmohammed@gmail.com
-License: MIT
-Keywords: discord bot generator beginner
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Disvide 🔧
+===========
 
-# Disvide
+.. image:: https://badge.fury.io/py/disvide.svg
+    :target: https://badge.fury.io/py/disvide
+    :alt: PyPI version
+
+.. image:: https://img.shields.io/discord/983326447970172978.svg?label=Discord&logo=Discord&colorB=7289DA&style=flat
+    :target: https://discord.gg/uqbxCTfxX9
+    :alt: Discord server
 
 Disvide is a Discord bot generator that allows you to create a bot by answering a few questions. This project is created by Cored, Inc and led by FSCYT.
 
-## Prerequisites
+Features
+--------
+
+- Command handler
+- Event handler
+- Slash command handler
+- Sub-commands handler
+- TypeScript and JavaScript support
+- Command categories
+- Easy customizability
+
+Please note that these are the features of the bot that is generated by Disvide, not the features of Disvide itself.
+
+Prerequisites
+-------------
 
 Before using Disvide, make sure you have the following:
 
 - Python 3.6 or higher installed on your system.
 - `pip` package manager installed on your system.
 - A Discord account with access to the developer portal.
 
@@ -26,63 +37,69 @@
 
 - At least 2 GB of RAM.
 - At least 1 GHz CPU.
 - At least 100 MB of free storage space.
 
 Please note that you can run this app with lower-tier hardware, but you may experience performance issues.
 
-## Contents
-
-- [Disvide](#disvide)
-  - [Prerequisites](#prerequisites)
-  - [Contents](#contents)
-  - [Getting Started](#getting-started)
-  - [How to Use](#how-to-use)
-  - [Contributing](#contributing)
-  - [Issues](#issues)
-  - [License](#license)
-
-## Getting Started
+Installation
+------------
 
 To get started with Disvide, follow these steps:
 
 1. Clone this repository to your local machine.
 2. Install the required dependencies by running `pip install -r requirements.txt`.
-3. Create a Discord bot account and obtain the bot token from the Discord Developer Portal.
-4. Run the program by executing `python bot_generator.py` in your terminal.
-5. Answer the following questions to generate your bot:
+
+Getting Started
+---------------
+
+To generate a Discord bot with Disvide, follow these steps:
+
+1. Create a Discord bot account and obtain the bot token from the Discord Developer Portal.
+2. Run the program by executing `python bot_generator.py` in your terminal.
+3. Answer the following questions to generate your bot:
    - What is the username of your bot?
    - What is the token of your bot?
    - What is the client ID of your bot?
    - What is the client secret of your bot?
    - Which programming language do you want to use (TS or JS)?
 
 The program will then generate a Discord bot for you.
 
-## How to Use
+Updates
+-------
 
-To use Disvide, follow the instructions in the [Getting Started](#getting-started) section. Once you have generated your bot, you can customize it by editing the generated code.
+18/04/2023
 
-## Contributing
+- Re-wrote templates for all languages respectively to support all the listed features above.
+- Made huge progress on the command generator part of disvide.
+- Other minor changes...
+
+Contributing
+------------
 
 Contributions to Disvide are welcome! If you would like to contribute, follow these steps:
 
 1. Fork this repository.
 2. Create a new branch with your changes: `git checkout -b my-feature-branch`.
 3. Commit your changes: `git commit -m "Added a new feature"`.
 4. Push to the branch: `git push origin my-feature-branch`.
 5. Create a pull request.
 
-## Issues
+Issues
+------
+
+.. code-block:: md
 
-**We are aware that disvide might not work on windows always and we are working on fixing it.**
+   We are aware that Disvide might not work on Windows natively at the moment and that it works using WSL (only WSL 2 tested for now).
 
-If you encounter any issues while using Disvide, please report them on the [issues page](https://github.com/cored-developments-2023/disvide/issues). To create a new issue, follow these steps:
+If you encounter any issues while using Disvide, please report them on the `issues page <https://github.com/cored-developments-2023/disvide/issues>`_. To create a new issue, follow these steps:
 
 1. Click on the "Issues" tab in the repository.
 2. Click on the "New Issue" button.
 3. Provide a descriptive title and detailed description of the issue.
 4. Click on the "Submit new issue" button.
 
-## License
+License
+-------
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the `LICENSE <LICENSE>`_ file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `disvide-0.4.2/setup.py` & `disvide-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name='disvide',
-    version='0.4.2',
+    version='0.5.0',
     license='MIT',
     author='Cored Developments',
     author_email='skyblockmohammed@gmail.com',
     packages=find_packages(),
     url='https://github.com/Cored-Inc/disvide',
     description='Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.',
     keywords='discord bot generator beginner',
```

