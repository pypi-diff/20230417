# Comparing `tmp/felixlib-0.0.8.tar.gz` & `tmp/felixlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felixlib-0.0.8.tar", last modified: Tue Feb 18 11:19:06 2020, max compression
+gzip compressed data, was "felixlib-0.0.9.tar", last modified: Tue Feb 18 14:09:50 2020, max compression
```

## Comparing `felixlib-0.0.8.tar` & `felixlib-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       22 2020-02-18 09:42:36.788713 felixlib-0.0.8/felixlib/__init__.py
--rw-r--r--   0        0        0    27648 2020-02-18 11:18:12.252836 felixlib-0.0.8/felixlib/__main__.cp37-win32.pyd
--rw-r--r--   0        0        0    34816 2020-02-18 11:16:18.148364 felixlib-0.0.8/felixlib/__main__.cp37-win_amd64.pyd
--rw-r--r--   0        0        0   189440 2020-02-18 11:18:16.555811 felixlib-0.0.8/felixlib/ansys.cp37-win32.pyd
--rw-r--r--   0        0        0   208384 2020-02-18 11:16:22.271188 felixlib-0.0.8/felixlib/ansys.cp37-win_amd64.pyd
--rw-r--r--   0        0        0    24576 2020-02-18 11:18:16.986567 felixlib-0.0.8/felixlib/const.cp37-win32.pyd
--rw-r--r--   0        0        0    30208 2020-02-18 11:16:22.709047 felixlib-0.0.8/felixlib/const.cp37-win_amd64.pyd
--rw-r--r--   0        0        0    94208 2020-02-18 11:18:17.825793 felixlib-0.0.8/felixlib/cython_build.cp37-win32.pyd
--rw-r--r--   0        0        0   109056 2020-02-18 11:16:23.623566 felixlib-0.0.8/felixlib/cython_build.cp37-win_amd64.pyd
--rw-r--r--   0        0        0    33280 2020-02-18 11:18:18.247978 felixlib-0.0.8/felixlib/data_analysis.cp37-win32.pyd
--rw-r--r--   0        0        0    41984 2020-02-18 11:16:24.076352 felixlib-0.0.8/felixlib/data_analysis.cp37-win_amd64.pyd
--rw-r--r--   0        0        0    99328 2020-02-18 11:18:19.052312 felixlib-0.0.8/felixlib/flask_common.cp37-win32.pyd
--rw-r--r--   0        0        0   117760 2020-02-18 11:16:25.096620 felixlib-0.0.8/felixlib/flask_common.cp37-win_amd64.pyd
--rw-r--r--   0        0        0   266752 2020-02-18 11:18:20.968298 felixlib-0.0.8/felixlib/general.cp37-win32.pyd
--rw-r--r--   0        0        0   306688 2020-02-18 11:16:28.092594 felixlib-0.0.8/felixlib/general.cp37-win_amd64.pyd
--rw-r--r--   0        0        0   124416 2020-02-18 11:18:22.089440 felixlib-0.0.8/felixlib/inventor.cp37-win32.pyd
--rw-r--r--   0        0        0   142848 2020-02-18 11:16:29.320306 felixlib-0.0.8/felixlib/inventor.cp37-win_amd64.pyd
--rw-r--r--   0        0        0   154112 2020-02-18 11:18:25.666897 felixlib-0.0.8/felixlib/pyi_build.cp37-win32.pyd
--rw-r--r--   0        0        0   173056 2020-02-18 11:16:32.354202 felixlib-0.0.8/felixlib/pyi_build.cp37-win_amd64.pyd
--rw-r--r--   0        0        0   100864 2020-02-18 11:18:27.612688 felixlib-0.0.8/felixlib/sg_common.cp37-win32.pyd
--rw-r--r--   0        0        0   113664 2020-02-18 11:16:34.309208 felixlib-0.0.8/felixlib/sg_common.cp37-win_amd64.pyd
--rw-r--r--   0        0        0       49 2019-11-15 13:20:34.000000 felixlib-0.0.8/LICENSE
--rw-r--r--   0        0        0      620 2020-02-18 11:16:08.699616 felixlib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       10 2019-11-11 13:51:08.000000 felixlib-0.0.8/README.md
--rw-r--r--   0        0        0      840 2020-02-18 11:19:06.801066 felixlib-0.0.8/setup.py
--rw-r--r--   0        0        0      770 2020-02-18 11:19:06.801066 felixlib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-18 09:42:36.000000 felixlib-0.0.9/felixlib/__init__.py
+-rw-r--r--   0        0        0    27648 2020-02-18 14:01:24.585785 felixlib-0.0.9/felixlib/__main__.cp37-win32.pyd
+-rw-r--r--   0        0        0    34816 2020-02-18 13:59:48.319356 felixlib-0.0.9/felixlib/__main__.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0   189440 2020-02-18 14:01:29.155825 felixlib-0.0.9/felixlib/ansys.cp37-win32.pyd
+-rw-r--r--   0        0        0   208384 2020-02-18 13:59:52.919759 felixlib-0.0.9/felixlib/ansys.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0    24576 2020-02-18 14:01:29.615394 felixlib-0.0.9/felixlib/const.cp37-win32.pyd
+-rw-r--r--   0        0        0    30208 2020-02-18 13:59:53.386481 felixlib-0.0.9/felixlib/const.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0    94208 2020-02-18 14:01:30.630402 felixlib-0.0.9/felixlib/cython_build.cp37-win32.pyd
+-rw-r--r--   0        0        0   109056 2020-02-18 13:59:54.413090 felixlib-0.0.9/felixlib/cython_build.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0    33280 2020-02-18 14:01:31.086214 felixlib-0.0.9/felixlib/data_analysis.cp37-win32.pyd
+-rw-r--r--   0        0        0    41984 2020-02-18 13:59:54.843598 felixlib-0.0.9/felixlib/data_analysis.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0    99328 2020-02-18 14:01:31.985412 felixlib-0.0.9/felixlib/flask_common.cp37-win32.pyd
+-rw-r--r--   0        0        0   117760 2020-02-18 13:59:55.812378 felixlib-0.0.9/felixlib/flask_common.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0   269824 2020-02-18 14:01:34.347860 felixlib-0.0.9/felixlib/general.cp37-win32.pyd
+-rw-r--r--   0        0        0   310272 2020-02-18 13:59:58.709995 felixlib-0.0.9/felixlib/general.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0   124416 2020-02-18 14:01:35.706016 felixlib-0.0.9/felixlib/inventor.cp37-win32.pyd
+-rw-r--r--   0        0        0   142848 2020-02-18 14:00:00.153064 felixlib-0.0.9/felixlib/inventor.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0   155136 2020-02-18 14:01:39.827575 felixlib-0.0.9/felixlib/pyi_build.cp37-win32.pyd
+-rw-r--r--   0        0        0   174592 2020-02-18 14:00:03.626345 felixlib-0.0.9/felixlib/pyi_build.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0   100864 2020-02-18 14:01:41.876240 felixlib-0.0.9/felixlib/sg_common.cp37-win32.pyd
+-rw-r--r--   0        0        0   113664 2020-02-18 14:00:05.814001 felixlib-0.0.9/felixlib/sg_common.cp37-win_amd64.pyd
+-rw-r--r--   0        0        0       49 2019-11-15 13:20:34.450387 felixlib-0.0.9/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-18 14:08:03.219089 felixlib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       10 2019-11-11 13:51:08.027886 felixlib-0.0.9/README.md
+-rw-r--r--   0        0        0      578 2020-02-18 14:09:51.255357 felixlib-0.0.9/setup.py
+-rw-r--r--   0        0        0      418 2020-02-18 14:09:51.255357 felixlib-0.0.9/PKG-INFO
```

### Comparing `felixlib-0.0.8/setup.py` & `felixlib-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,38 +3,24 @@
 
 packages = \
 ['felixlib']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['colorama>=0.4.1,<0.5.0',
- 'flask>=1.1,<2.0',
- 'numpy>=1.17,<2.0',
- 'psutil>=5.6,<6.0',
- 'pysimplegui>=4.14,<5.0',
- 'pywebview>=3.1,<4.0',
- 'pywin32>=225,<226',
- 'pywinauto>=0.6.8,<0.7.0',
- 'send2trash>=1.5,<2.0',
- 'wtforms>=2.2,<3.0',
- 'xlwings>=0.16.0,<0.17.0']
-
 setup_kwargs = {
     'name': 'felixlib',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'felixlib',
     'long_description': 'felixlib\n',
     'author': 'spectereye',
     'author_email': 'spectereye@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.7, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*',
 }
 
 
 setup(**setup_kwargs)
```

