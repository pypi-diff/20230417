# Comparing `tmp/kornia_moons-0.2.4.tar.gz` & `tmp/kornia_moons-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kornia_moons-0.2.4.tar", last modified: Mon Mar 20 12:58:00 2023, max compression
+gzip compressed data, was "kornia_moons-0.2.5.tar", last modified: Mon Apr 17 12:10:11 2023, max compression
```

## Comparing `kornia_moons-0.2.4.tar` & `kornia_moons-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-03-20 12:58:00.890737 kornia_moons-0.2.4/
--rw-r--r--   0 oldufo     (501) staff       (20)     2348 2021-06-15 15:28:17.000000 kornia_moons-0.2.4/CONTRIBUTING.md
--rw-r--r--   0 oldufo     (501) staff       (20)    11357 2021-06-15 15:28:17.000000 kornia_moons-0.2.4/LICENSE
--rw-r--r--   0 oldufo     (501) staff       (20)      111 2021-06-15 15:28:17.000000 kornia_moons-0.2.4/MANIFEST.in
--rw-r--r--   0 oldufo     (501) staff       (20)     2205 2023-03-20 12:58:00.890613 kornia_moons-0.2.4/PKG-INFO
--rw-r--r--   0 oldufo     (501) staff       (20)     1414 2022-08-24 14:54:58.000000 kornia_moons-0.2.4/README.md
-drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-03-20 12:58:00.889476 kornia_moons-0.2.4/kornia_moons/
--rw-r--r--   0 oldufo     (501) staff       (20)       22 2023-03-20 11:05:58.000000 kornia_moons-0.2.4/kornia_moons/__init__.py
--rw-r--r--   0 oldufo     (501) staff       (20)     1358 2023-03-20 11:05:58.000000 kornia_moons-0.2.4/kornia_moons/_nbdev.py
--rw-r--r--   0 oldufo     (501) staff       (20)    22143 2023-03-20 11:05:58.000000 kornia_moons-0.2.4/kornia_moons/feature.py
-drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-03-20 12:58:00.890444 kornia_moons-0.2.4/kornia_moons.egg-info/
--rw-r--r--   0 oldufo     (501) staff       (20)     2205 2023-03-20 12:58:00.000000 kornia_moons-0.2.4/kornia_moons.egg-info/PKG-INFO
--rw-r--r--   0 oldufo     (501) staff       (20)      353 2023-03-20 12:58:00.000000 kornia_moons-0.2.4/kornia_moons.egg-info/SOURCES.txt
--rw-r--r--   0 oldufo     (501) staff       (20)        1 2023-03-20 12:58:00.000000 kornia_moons-0.2.4/kornia_moons.egg-info/dependency_links.txt
--rw-r--r--   0 oldufo     (501) staff       (20)        1 2021-06-15 15:53:30.000000 kornia_moons-0.2.4/kornia_moons.egg-info/not-zip-safe
--rw-r--r--   0 oldufo     (501) staff       (20)       38 2023-03-20 12:58:00.000000 kornia_moons-0.2.4/kornia_moons.egg-info/requires.txt
--rw-r--r--   0 oldufo     (501) staff       (20)       13 2023-03-20 12:58:00.000000 kornia_moons-0.2.4/kornia_moons.egg-info/top_level.txt
--rw-r--r--   0 oldufo     (501) staff       (20)     2420 2023-03-20 12:56:41.000000 kornia_moons-0.2.4/settings.ini
--rw-r--r--   0 oldufo     (501) staff       (20)       38 2023-03-20 12:58:00.890773 kornia_moons-0.2.4/setup.cfg
--rw-r--r--   0 oldufo     (501) staff       (20)     2856 2022-08-24 14:56:24.000000 kornia_moons-0.2.4/setup.py
+drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-17 12:10:11.869689 kornia_moons-0.2.5/
+-rw-r--r--   0 oldufo     (501) staff       (20)     2348 2023-04-17 09:31:17.000000 kornia_moons-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0 oldufo     (501) staff       (20)    11357 2023-04-17 09:31:17.000000 kornia_moons-0.2.5/LICENSE
+-rw-r--r--   0 oldufo     (501) staff       (20)      111 2023-04-17 09:31:17.000000 kornia_moons-0.2.5/MANIFEST.in
+-rw-r--r--   0 oldufo     (501) staff       (20)     2158 2023-04-17 12:10:11.869561 kornia_moons-0.2.5/PKG-INFO
+-rw-r--r--   0 oldufo     (501) staff       (20)     1296 2023-04-17 11:47:08.000000 kornia_moons-0.2.5/README.md
+drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-17 12:10:11.868114 kornia_moons-0.2.5/kornia_moons/
+-rw-r--r--   0 oldufo     (501) staff       (20)       22 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/__init__.py
+-rw-r--r--   0 oldufo     (501) staff       (20)     6858 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/_modidx.py
+-rw-r--r--   0 oldufo     (501) staff       (20)     1358 2023-04-17 09:31:18.000000 kornia_moons-0.2.5/kornia_moons/_nbdev.py
+-rw-r--r--   0 oldufo     (501) staff       (20)     8614 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/feature.py
+-rw-r--r--   0 oldufo     (501) staff       (20)    18988 2023-04-17 12:08:39.000000 kornia_moons-0.2.5/kornia_moons/viz.py
+drwxr-xr-x   0 oldufo     (501) staff       (20)        0 2023-04-17 12:10:11.869395 kornia_moons-0.2.5/kornia_moons.egg-info/
+-rw-r--r--   0 oldufo     (501) staff       (20)     2158 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/PKG-INFO
+-rw-r--r--   0 oldufo     (501) staff       (20)      436 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/SOURCES.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)        1 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/dependency_links.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)       46 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/entry_points.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)        1 2021-06-15 15:53:30.000000 kornia_moons-0.2.5/kornia_moons.egg-info/not-zip-safe
+-rw-r--r--   0 oldufo     (501) staff       (20)       45 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/requires.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)       13 2023-04-17 12:10:11.000000 kornia_moons-0.2.5/kornia_moons.egg-info/top_level.txt
+-rw-r--r--   0 oldufo     (501) staff       (20)     2433 2023-04-17 12:06:09.000000 kornia_moons-0.2.5/settings.ini
+-rw-r--r--   0 oldufo     (501) staff       (20)       38 2023-04-17 12:10:11.869726 kornia_moons-0.2.5/setup.cfg
+-rw-r--r--   0 oldufo     (501) staff       (20)     2596 2023-04-17 09:31:18.000000 kornia_moons-0.2.5/setup.py
```

### Comparing `kornia_moons-0.2.4/CONTRIBUTING.md` & `kornia_moons-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.4/LICENSE` & `kornia_moons-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.4/kornia_moons/_nbdev.py` & `kornia_moons-0.2.5/kornia_moons/_nbdev.py`

 * *Files identical despite different names*

### Comparing `kornia_moons-0.2.4/settings.ini` & `kornia_moons-0.2.5/settings.ini`

 * *Files 7% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 user = ducha-aiki
 description = Conversions between kornia and other computer vision libraries formats
 keywords = kornia, python, pytorch, deep learning, computer vision
 author = Dmytro Mishkin
 author_email = ducha.aiki@gmail.com
 copyright = Dmytro Mishkin
 branch = master
-version = 0.2.4
-min_python = 3.6
+version = 0.2.5
+min_python = 3.7
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
 # From 1-7: Planning Pre-Alpha Alpha Beta Production Mature Inactive
 status = 1
 
 # Optional. Same format as setuptools requirements
-requirements = kornia torch matplotlib
+requirements = kornia torch matplotlib opencv-python
 # Optional. Same format as setuptools console_scripts
 # console_scripts = 
 # Optional. Same format as setuptools dependency-links
 # dep_links = 
 
 ###
 # You probably won't need to change anything under here,
 #   unless you have some special requirements
 ###
 
 # Change to, e.g. "nbs", to put your notebooks in nbs dir instead of repo root
-nbs_path = nbs
-doc_path = docs
+nbs_path = .
+doc_path = _docs
 
 # Anything shown as '%(...)s' is substituted with that setting automatically
 doc_host =  https://%(user)s.github.io
 #For Enterprise Git pages use:  
 #doc_host = https://pages.github.%(company_name)s.com.
```

### Comparing `kornia_moons-0.2.4/setup.py` & `kornia_moons-0.2.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,57 @@
 from pkg_resources import parse_version
-from pkg_resources import DistributionNotFound, get_distribution
 from configparser import ConfigParser
-import re
-import setuptools
+import setuptools, shlex
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
-
-# Taken from https://github.com/albumentations-team/albumentations/blob/1.0.0/setup.py
-def choose_requirement(mains, secondary):
-    """If some version version of main requirement installed, return main,
-    else return secondary.
-    """
-    chosen = secondary
-    for main in mains:
-        try:
-            name = re.split(r"[!<>=]", main)[0]
-            get_distribution(name)
-            chosen = main
-            break
-        except DistributionNotFound as e:
-            pass
-    return str(chosen)
-
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
+config.read('settings.ini', encoding='utf-8')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
 licenses = {
     'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8'.split()
+py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
 
-requirements = cfg.get('requirements','').split()
-lic = licenses[cfg['license']]
+requirements = shlex.split(cfg.get('requirements', ''))
+if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
 min_python = cfg['min_python']
-
-# Taken from https://github.com/albumentations-team/albumentations/blob/1.0.0/setup.py
-# If none of packages in first installed, install second package
-CHOOSE_INSTALL_REQUIRES = [
-        ("opencv-python", "opencv-contrib-python", "opencv-contrib-python-headless"),
-        "opencv-python-headless"]
-
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+dev_requirements = (cfg.get('dev_requirements') or '').split()
 
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
     classifiers = [
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
-        'License :: ' + lic[1],
         'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]],
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
-    install_requires = requirements + [choose_requirement(*CHOOSE_INSTALL_REQUIRES)],
+    install_requires = requirements,
+    extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
+    long_description = open('README.md', encoding='utf-8').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
-    entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
     **setup_cfg)
 
+
```

