# Comparing `tmp/docx_word_instance_generator-0.7.0-py3-none-any.whl.zip` & `tmp/docx_word_instance_generator-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 4644 bytes, number of entries: 10
+Zip file size: 5061 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat     1534 b- defN 23-Apr-14 14:39 docx_word_instance_generator/WordGenerator.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-14 08:21 docx_word_instance_generator/__init__.py
--rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-17 07:50 docx_word_instance_generator/version.py
--rw-rw-rw-  2.0 fat     1065 b- defN 23-Apr-17 07:50 docx_word_instance_generator-0.7.0.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat      904 b- defN 23-Apr-17 07:50 docx_word_instance_generator-0.7.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 07:50 docx_word_instance_generator-0.7.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       34 b- defN 23-Apr-17 07:50 docx_word_instance_generator-0.7.0.dist-info/requirements.txt
--rw-rw-rw-  2.0 fat      804 b- defN 23-Apr-17 07:50 docx_word_instance_generator-0.7.0.dist-info/setup.py
--rw-rw-rw-  2.0 fat       29 b- defN 23-Apr-17 07:50 docx_word_instance_generator-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1008 b- defN 23-Apr-17 07:50 docx_word_instance_generator-0.7.0.dist-info/RECORD
-10 files, 5487 bytes uncompressed, 2852 bytes compressed:  48.0%
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-17 07:59 docx_word_instance_generator/version.py
+-rw-rw-rw-  2.0 fat     1065 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      172 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/README.md
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       34 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/requirements.txt
+-rw-rw-rw-  2.0 fat      804 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/setup.py
+-rw-rw-rw-  2.0 fat       29 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1119 b- defN 23-Apr-17 07:59 docx_word_instance_generator-0.8.0.dist-info/RECORD
+11 files, 5955 bytes uncompressed, 3085 bytes compressed:  48.2%
```

## zipnote {}

```diff
@@ -3,29 +3,32 @@
 
 Filename: docx_word_instance_generator/__init__.py
 Comment: 
 
 Filename: docx_word_instance_generator/version.py
 Comment: 
 
-Filename: docx_word_instance_generator-0.7.0.dist-info/LICENSE.md
+Filename: docx_word_instance_generator-0.8.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: docx_word_instance_generator-0.7.0.dist-info/METADATA
+Filename: docx_word_instance_generator-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: docx_word_instance_generator-0.7.0.dist-info/WHEEL
+Filename: docx_word_instance_generator-0.8.0.dist-info/README.md
 Comment: 
 
-Filename: docx_word_instance_generator-0.7.0.dist-info/requirements.txt
+Filename: docx_word_instance_generator-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: docx_word_instance_generator-0.7.0.dist-info/setup.py
+Filename: docx_word_instance_generator-0.8.0.dist-info/requirements.txt
 Comment: 
 
-Filename: docx_word_instance_generator-0.7.0.dist-info/top_level.txt
+Filename: docx_word_instance_generator-0.8.0.dist-info/setup.py
 Comment: 
 
-Filename: docx_word_instance_generator-0.7.0.dist-info/RECORD
+Filename: docx_word_instance_generator-0.8.0.dist-info/top_level.txt
+Comment: 
+
+Filename: docx_word_instance_generator-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docx_word_instance_generator/version.py

```diff
@@ -1 +1 @@
-VERSION = "0.7.0"
+VERSION = "0.8.0"
```

## Comparing `docx_word_instance_generator-0.7.0.dist-info/LICENSE.md` & `docx_word_instance_generator-0.8.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `docx_word_instance_generator-0.7.0.dist-info/METADATA` & `docx_word_instance_generator-0.8.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: docx-word-instance-generator
-Version: 0.7.0
+Version: 0.8.0
 Summary: Generates docx from docs Jinja2 templates
 Home-page: https://github.com/Koldar/django-koldar-common-apps
 Author: Massimo Bono
 Author-email: massimobono1@gmail.com
 License: MIT
 Keywords: docx,template,jinja2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
-Description-Content-Type: text/plain
+Description-Content-Type: text/markdown
 License-File: LICENSE.md
+License-File: README.md
 License-File: requirements.txt
 License-File: setup.py
 Requires-Dist: Jinja2 (>=3.1.2)
 Requires-Dist: MarkupSafe (>=2.1.2)
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme ; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: mock ; extra == 'test'
 
-<no readme found>
+
+Introduction
+============
+
+Allows you to generate new word docx extended documents generated 
+from a docx template. The template uses Jinja2 template engine by default.
```

## Comparing `docx_word_instance_generator-0.7.0.dist-info/setup.py` & `docx_word_instance_generator-0.8.0.dist-info/setup.py`

 * *Files identical despite different names*

## Comparing `docx_word_instance_generator-0.7.0.dist-info/RECORD` & `docx_word_instance_generator-0.8.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 docx_word_instance_generator/WordGenerator.py,sha256=o6a-t8eDQSwKaGp0CV3PHqeDipCq9jVZ_8IJ5B9xkXE,1534
 docx_word_instance_generator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docx_word_instance_generator/version.py,sha256=eKj5kuF3R_LOr_-Iq2-HpF7MH76xReur9yN39Kky7ho,17
-docx_word_instance_generator-0.7.0.dist-info/LICENSE.md,sha256=4GTsQqtffGQX2TQ1XIcZW9W9Q1Bh7E33NK89pXibeVQ,1065
-docx_word_instance_generator-0.7.0.dist-info/METADATA,sha256=_Zu6pwGujzH8AOmmCNs1M0uikMS99gNzOn6mrmKpNSw,904
-docx_word_instance_generator-0.7.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-docx_word_instance_generator-0.7.0.dist-info/requirements.txt,sha256=RnWM0qpgrSqDU3T3Vpv57W8GfbCXqyQvtpULqV65etk,34
-docx_word_instance_generator-0.7.0.dist-info/setup.py,sha256=UqrHk1kurcXWHG-gFvLO90OoYdW0FlPyYDASpP9R43U,804
-docx_word_instance_generator-0.7.0.dist-info/top_level.txt,sha256=kUeS5yk5dWKeWqje5djxLmPv-o0L-bdkeknXZ75-mKk,29
-docx_word_instance_generator-0.7.0.dist-info/RECORD,,
+docx_word_instance_generator/version.py,sha256=QnEtO8Bvd4VVrcq-tLf2Az_cVyZ9QVyRUhORPzPhizY,17
+docx_word_instance_generator-0.8.0.dist-info/LICENSE.md,sha256=4GTsQqtffGQX2TQ1XIcZW9W9Q1Bh7E33NK89pXibeVQ,1065
+docx_word_instance_generator-0.8.0.dist-info/METADATA,sha256=LyunXV9VO5nGXMZCHF-LCAb5SSLbORH8A9Lt5Gv5G9o,1089
+docx_word_instance_generator-0.8.0.dist-info/README.md,sha256=YYqblskLZzykbh2A7LWAAANA-4LMzVxJ9mFnQw8Rf0Y,172
+docx_word_instance_generator-0.8.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+docx_word_instance_generator-0.8.0.dist-info/requirements.txt,sha256=RnWM0qpgrSqDU3T3Vpv57W8GfbCXqyQvtpULqV65etk,34
+docx_word_instance_generator-0.8.0.dist-info/setup.py,sha256=UqrHk1kurcXWHG-gFvLO90OoYdW0FlPyYDASpP9R43U,804
+docx_word_instance_generator-0.8.0.dist-info/top_level.txt,sha256=kUeS5yk5dWKeWqje5djxLmPv-o0L-bdkeknXZ75-mKk,29
+docx_word_instance_generator-0.8.0.dist-info/RECORD,,
```

