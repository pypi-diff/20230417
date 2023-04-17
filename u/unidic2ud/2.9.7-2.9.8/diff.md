# Comparing `tmp/unidic2ud-2.9.7.tar.gz` & `tmp/unidic2ud-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidic2ud-2.9.7.tar", last modified: Wed Dec 28 01:20:17 2022, max compression
+gzip compressed data, was "unidic2ud-2.9.8.tar", last modified: Mon Apr 17 14:55:57 2023, max compression
```

## Comparing `unidic2ud-2.9.7.tar` & `unidic2ud-2.9.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2022-12-28 01:20:17.867853 unidic2ud-2.9.7/
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    15547 2022-12-28 01:20:17.867853 unidic2ud-2.9.7/PKG-INFO
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    12486 2022-04-24 14:48:41.000000 unidic2ud-2.9.7/README.md
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       38 2022-12-28 01:20:17.867853 unidic2ud-2.9.7/setup.cfg
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     1902 2022-12-28 01:19:59.000000 unidic2ud-2.9.7/setup.py
-drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2022-12-28 01:20:17.851853 unidic2ud-2.9.7/unidic2ud/
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      182 2019-11-22 08:08:05.000000 unidic2ud-2.9.7/unidic2ud/__init__.py
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      579 2019-11-14 15:01:21.000000 unidic2ud-2.9.7/unidic2ud/__main__.py
-drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2022-12-28 01:20:17.855853 unidic2ud-2.9.7/unidic2ud/cabocha/
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      134 2020-05-01 08:10:03.000000 unidic2ud-2.9.7/unidic2ud/cabocha/__init__.py
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     2334 2020-07-02 02:46:43.000000 unidic2ud-2.9.7/unidic2ud/cabocha/cli.py
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     7461 2020-08-14 03:26:22.000000 unidic2ud-2.9.7/unidic2ud/cabocha/unidic2cabocha.py
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     1937 2020-01-14 14:43:33.000000 unidic2ud-2.9.7/unidic2ud/cli.py
-drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2022-12-28 01:20:17.855853 unidic2ud-2.9.7/unidic2ud/download/
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001) 10039018 2021-01-27 23:08:05.000000 unidic2ud-2.9.7/unidic2ud/download/japanese-modern.udpipe
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       20 2020-07-07 12:47:44.000000 unidic2ud-2.9.7/unidic2ud/mecabrc
-drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2022-12-28 01:20:17.867853 unidic2ud-2.9.7/unidic2ud/spacy/
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       99 2021-01-03 06:56:03.000000 unidic2ud-2.9.7/unidic2ud/spacy/__init__.py
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     6632 2021-02-20 00:35:59.000000 unidic2ud-2.9.7/unidic2ud/spacy/unidic2spacy.py
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    16231 2022-04-24 13:45:19.000000 unidic2ud-2.9.7/unidic2ud/unidic2ud.py
-drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2022-12-28 01:20:17.855853 unidic2ud-2.9.7/unidic2ud.egg-info/
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    15547 2022-12-28 01:20:17.000000 unidic2ud-2.9.7/unidic2ud.egg-info/PKG-INFO
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      513 2022-12-28 01:20:17.000000 unidic2ud-2.9.7/unidic2ud.egg-info/SOURCES.txt
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)        1 2022-12-28 01:20:17.000000 unidic2ud-2.9.7/unidic2ud.egg-info/dependency_links.txt
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       89 2022-12-28 01:20:17.000000 unidic2ud-2.9.7/unidic2ud.egg-info/entry_points.txt
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       51 2022-12-28 01:20:17.000000 unidic2ud-2.9.7/unidic2ud.egg-info/requires.txt
--rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       10 2022-12-28 01:20:17.000000 unidic2ud-2.9.7/unidic2ud.egg-info/top_level.txt
+drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2023-04-17 14:55:57.317874 unidic2ud-2.9.8/
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    15547 2023-04-17 14:55:57.317874 unidic2ud-2.9.8/PKG-INFO
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    12486 2022-04-24 14:48:41.000000 unidic2ud-2.9.8/README.md
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       38 2023-04-17 14:55:57.317874 unidic2ud-2.9.8/setup.cfg
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     1902 2023-04-17 14:55:26.000000 unidic2ud-2.9.8/setup.py
+drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2023-04-17 14:55:57.305874 unidic2ud-2.9.8/unidic2ud/
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      182 2019-11-22 08:08:05.000000 unidic2ud-2.9.8/unidic2ud/__init__.py
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      579 2019-11-14 15:01:21.000000 unidic2ud-2.9.8/unidic2ud/__main__.py
+drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2023-04-17 14:55:57.305874 unidic2ud-2.9.8/unidic2ud/cabocha/
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      134 2020-05-01 08:10:03.000000 unidic2ud-2.9.8/unidic2ud/cabocha/__init__.py
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     2334 2020-07-02 02:46:43.000000 unidic2ud-2.9.8/unidic2ud/cabocha/cli.py
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     7461 2020-08-14 03:26:22.000000 unidic2ud-2.9.8/unidic2ud/cabocha/unidic2cabocha.py
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     1937 2020-01-14 14:43:33.000000 unidic2ud-2.9.8/unidic2ud/cli.py
+drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2023-04-17 14:55:57.305874 unidic2ud-2.9.8/unidic2ud/download/
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001) 10039018 2021-01-27 23:08:05.000000 unidic2ud-2.9.8/unidic2ud/download/japanese-modern.udpipe
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       20 2020-07-07 12:47:44.000000 unidic2ud-2.9.8/unidic2ud/mecabrc
+drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2023-04-17 14:55:57.317874 unidic2ud-2.9.8/unidic2ud/spacy/
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       99 2021-01-03 06:56:03.000000 unidic2ud-2.9.8/unidic2ud/spacy/__init__.py
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)     6632 2021-02-20 00:35:59.000000 unidic2ud-2.9.8/unidic2ud/spacy/unidic2spacy.py
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    16231 2023-04-17 14:52:21.000000 unidic2ud-2.9.8/unidic2ud/unidic2ud.py
+drwxr-xr-x   0 yasuoka   (1001) yasuoka   (1001)        0 2023-04-17 14:55:57.305874 unidic2ud-2.9.8/unidic2ud.egg-info/
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)    15547 2023-04-17 14:55:57.000000 unidic2ud-2.9.8/unidic2ud.egg-info/PKG-INFO
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)      513 2023-04-17 14:55:57.000000 unidic2ud-2.9.8/unidic2ud.egg-info/SOURCES.txt
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)        1 2023-04-17 14:55:57.000000 unidic2ud-2.9.8/unidic2ud.egg-info/dependency_links.txt
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       89 2023-04-17 14:55:57.000000 unidic2ud-2.9.8/unidic2ud.egg-info/entry_points.txt
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       51 2023-04-17 14:55:57.000000 unidic2ud-2.9.8/unidic2ud.egg-info/requires.txt
+-rw-r--r--   0 yasuoka   (1001) yasuoka   (1001)       10 2023-04-17 14:55:57.000000 unidic2ud-2.9.8/unidic2ud.egg-info/top_level.txt
```

### Comparing `unidic2ud-2.9.7/PKG-INFO` & `unidic2ud-2.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidic2ud
-Version: 2.9.7
+Version: 2.9.8
 Summary: Tokenizer POS-tagger Lemmatizer and Dependency-parser for modern and contemporary Japanese
 Home-page: https://github.com/KoichiYasuoka/UniDic2UD
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: japanese-modern, https://github.com/UniversalDependencies/UD_Japanese-Modern
 Project-URL: ud-ja-kanbun, https://corpus.kanji.zinbun.kyoto-u.ac.jp/gitlab/Kanbun/ud-ja-kanbun
```

### Comparing `unidic2ud-2.9.7/README.md` & `unidic2ud-2.9.8/README.md`

 * *Files identical despite different names*

### Comparing `unidic2ud-2.9.7/setup.py` & `unidic2ud-2.9.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 with open("README.md","r",encoding="utf-8") as r:
   long_description=r.read()
 URL="https://github.com/KoichiYasuoka/UniDic2UD"
 
 pl=platform.platform()
 if pl.startswith("CYGWIN"):
-  install_requires=["ufal.udpipe>=1.2.0","mecab-cygwin>=0.5.0","deplacy>=2.0.3"]
+  install_requires=["ufal.udpipe>=1.2.0","mecab-cygwin>=0.5.0","deplacy>=2.0.5"]
 else:
   import sys
   useFugashi=(sys.version_info.major==3)and(sys.version_info.minor>4)
   try:
     d=subprocess.check_output(["mecab-config","--libs-only-L"])
   except:
     import os
     useFugashi&=(os.name=="nt")
   if useFugashi:
-    install_requires=["ufal.udpipe>=1.2.0.3","fugashi>=1.0.5","deplacy>=2.0.3"]
+    install_requires=["ufal.udpipe>=1.2.0.3","fugashi>=1.0.5","deplacy>=2.0.5"]
   else:
-    install_requires=["ufal.udpipe>=1.2.0","mecab-python3>=0.996.5","deplacy>=2.0.3"]
+    install_requires=["ufal.udpipe>=1.2.0","mecab-python3>=0.996.5","deplacy>=2.0.5"]
 
 setuptools.setup(
   name="unidic2ud",
-  version="2.9.7",
+  version="2.9.8",
   description="Tokenizer POS-tagger Lemmatizer and Dependency-parser for modern and contemporary Japanese",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url=URL,
   author="Koichi Yasuoka",
   author_email="yasuoka@kanji.zinbun.kyoto-u.ac.jp",
   license="MIT",
```

### Comparing `unidic2ud-2.9.7/unidic2ud/__main__.py` & `unidic2ud-2.9.8/unidic2ud/__main__.py`

 * *Files identical despite different names*

### Comparing `unidic2ud-2.9.7/unidic2ud/cabocha/cli.py` & `unidic2ud-2.9.8/unidic2ud/cabocha/cli.py`

 * *Files identical despite different names*

### Comparing `unidic2ud-2.9.7/unidic2ud/cabocha/unidic2cabocha.py` & `unidic2ud-2.9.8/unidic2ud/cabocha/unidic2cabocha.py`

 * *Files identical despite different names*

### Comparing `unidic2ud-2.9.7/unidic2ud/cli.py` & `unidic2ud-2.9.8/unidic2ud/cli.py`

 * *Files identical despite different names*

### Comparing `unidic2ud-2.9.7/unidic2ud/download/japanese-modern.udpipe` & `unidic2ud-2.9.8/unidic2ud/download/japanese-modern.udpipe`

 * *Files identical despite different names*

### Comparing `unidic2ud-2.9.7/unidic2ud/spacy/unidic2spacy.py` & `unidic2ud-2.9.8/unidic2ud/spacy/unidic2spacy.py`

 * *Files identical despite different names*

### Comparing `unidic2ud-2.9.7/unidic2ud/unidic2ud.py` & `unidic2ud-2.9.8/unidic2ud/unidic2ud.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 PACKAGE_DIR=os.path.abspath(os.path.dirname(__file__))
 DOWNLOAD_DIR=os.path.join(PACKAGE_DIR,"download")
 import time
 tm=time.time()
 
 UNIDIC_URL="https://clrd.ninjal.ac.jp/unidic_archive/"
 UNIDIC_URLS={
-  "gendai":UNIDIC_URL+"cwj/3.1.0/unidic-cwj-3.1.0.zip",
-  "spoken":UNIDIC_URL+"csj/3.1.0/unidic-csj-3.1.0.zip",
+  "gendai":UNIDIC_URL+"cwj/3.1.1/unidic-cwj-3.1.1.zip",
+  "spoken":UNIDIC_URL+"csj/3.1.1/unidic-csj-3.1.1.zip",
   "qkana":UNIDIC_URL+"2203/UniDic-202203_60b_qkana.zip",
   "kindai":UNIDIC_URL+"2203/UniDic-202203_60a_kindai-bungo.zip",
   "kinsei":UNIDIC_URL+"2203/UniDic-202203_50c_kinsei-edo.zip",
   "kyogen":UNIDIC_URL+"2203/UniDic-202203_40_chusei-kougo.zip",
   "wakan":UNIDIC_URL+"2203/UniDic-202203_30_chusei-bungo.zip",
   "wabun":UNIDIC_URL+"2203/UniDic-202203_20_chuko.zip",
   "manyo":UNIDIC_URL+"2203/UniDic-202203_10_jodai.zip"
```

### Comparing `unidic2ud-2.9.7/unidic2ud.egg-info/PKG-INFO` & `unidic2ud-2.9.8/unidic2ud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidic2ud
-Version: 2.9.7
+Version: 2.9.8
 Summary: Tokenizer POS-tagger Lemmatizer and Dependency-parser for modern and contemporary Japanese
 Home-page: https://github.com/KoichiYasuoka/UniDic2UD
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: japanese-modern, https://github.com/UniversalDependencies/UD_Japanese-Modern
 Project-URL: ud-ja-kanbun, https://corpus.kanji.zinbun.kyoto-u.ac.jp/gitlab/Kanbun/ud-ja-kanbun
```

### Comparing `unidic2ud-2.9.7/unidic2ud.egg-info/SOURCES.txt` & `unidic2ud-2.9.8/unidic2ud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

