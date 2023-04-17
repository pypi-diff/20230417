# Comparing `tmp/SimpleIDML-1.1.3.tar.gz` & `tmp/SimpleIDML-1.1.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleIDML-1.1.3.tar", last modified: Tue Jan 18 09:40:51 2022, max compression
+gzip compressed data, was "dist/SimpleIDML-1.1.6a1.tar", last modified: Mon Apr 17 14:18:51 2023, max compression
```

## Comparing `SimpleIDML-1.1.3.tar` & `SimpleIDML-1.1.6a1.tar`

### file list

```diff
@@ -1,171 +1,147 @@
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.304486 SimpleIDML-1.1.3/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       36 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/AUTHORS
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1424 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/LICENSE
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      199 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/MANIFEST.in
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    23513 2022-01-18 09:40:51.304046 SimpleIDML-1.1.3/PKG-INFO
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    22502 2022-01-18 09:40:07.000000 SimpleIDML-1.1.3/README.rst
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       38 2022-01-18 09:40:51.304612 SimpleIDML-1.1.3/setup.cfg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1783 2022-01-18 09:35:39.000000 SimpleIDML-1.1.3/setup.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.166648 SimpleIDML-1.1.3/src/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.172356 SimpleIDML-1.1.3/src/SimpleIDML.egg-info/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    23513 2022-01-18 09:40:50.000000 SimpleIDML-1.1.3/src/SimpleIDML.egg-info/PKG-INFO
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     7940 2022-01-18 09:40:50.000000 SimpleIDML-1.1.3/src/SimpleIDML.egg-info/SOURCES.txt
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        1 2022-01-18 09:40:50.000000 SimpleIDML-1.1.3/src/SimpleIDML.egg-info/dependency_links.txt
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       14 2022-01-18 09:40:50.000000 SimpleIDML-1.1.3/src/SimpleIDML.egg-info/requires.txt
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       12 2022-01-18 09:40:50.000000 SimpleIDML-1.1.3/src/SimpleIDML.egg-info/top_level.txt
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.173551 SimpleIDML-1.1.3/src/scripts/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      618 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/scripts/simpleidml_create_package_from_dir.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      682 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/scripts/simpleidml_indesign_close_all_documents.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     3732 2020-12-04 14:34:01.000000 SimpleIDML-1.1.3/src/scripts/simpleidml_indesign_save_as.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.179801 SimpleIDML-1.1.3/src/simple_idml/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      320 2020-12-04 14:34:01.000000 SimpleIDML-1.1.3/src/simple_idml/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2353 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/commands.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    37735 2020-05-27 07:40:19.000000 SimpleIDML-1.1.3/src/simple_idml/components.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2168 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/decorators.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      254 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/exceptions.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      685 2020-06-09 15:50:28.000000 SimpleIDML-1.1.3/src/simple_idml/extras.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     6826 2020-12-04 14:34:01.000000 SimpleIDML-1.1.3/src/simple_idml/ftp.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1795 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/id_package.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    49978 2020-06-30 07:14:18.000000 SimpleIDML-1.1.3/src/simple_idml/idml.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.180527 SimpleIDML-1.1.3/src/simple_idml/indesign/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/indesign/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    11540 2020-12-04 14:34:01.000000 SimpleIDML-1.1.3/src/simple_idml/indesign/indesign.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.182374 SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      126 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/close_all_documents.jsx
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    12733 2022-01-18 09:35:17.000000 SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/export.jsx
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      285 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/list_profiles.jsx
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1190 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/package_to_print.jsx
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      636 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/save_as.jsx
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4486 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/test.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     3436 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/src/simple_idml/utils.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.185114 SimpleIDML-1.1.3/tests/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      262 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/Makefile
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.186125 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.187204 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/META-INF/
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)      253 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/META-INF/container.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)    25750 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/META-INF/metadata.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.187893 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/MasterSpreads/
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)     2622 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/MasterSpreads/MasterSpread_ua5.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.189893 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)    15600 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Fonts.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)     7501 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Graphic.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)    73533 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Preferences.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)    36650 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Styles.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.190378 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Spreads/
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)    19391 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Spreads/Spread_myprefixud8.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.191552 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)     1399 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/Story_myprefixu10d.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)      999 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/Story_myprefixue1.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)     3145 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/Story_myprefixuf7.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.192637 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/XML/
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)      785 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/XML/BackingStory.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)      491 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/XML/Mapping.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)     1565 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/XML/Tags.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)    16258 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/designmap.xml
--rw-rw-r--   0 guerrastanislas   (501) staff       (20)       43 2020-06-08 10:38:32.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/mimetype
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   207919 2020-06-08 12:38:50.000000 SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       62 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/coveragerc
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.196658 SimpleIDML-1.1.3/tests/regressiontests/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.256476 SimpleIDML-1.1.3/tests/regressiontests/IDML/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    40088 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-0photo.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   364544 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-0photo.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    46702 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   860160 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    45371 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   864256 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    40775 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages-layers-with-guides.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   360448 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages-layers-with-guides.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    37291 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   466944 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages.indd
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.260012 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.260861 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/META-INF/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      253 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/META-INF/container.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    25538 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.261892 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/MasterSpreads/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2608 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.264038 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Resources/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    15342 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     7221 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    73611 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    35821 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.264681 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Spreads/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    19082 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.266425 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Stories/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      940 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2320 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1315 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.267854 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/XML/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      732 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      274 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/XML/Mapping.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1302 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/XML/Tags.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    16154 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/designmap.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       43 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/mimetype
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   575266 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo-package.zip
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    35520 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo-with-attributes.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   389120 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo-with-attributes.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    40175 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   569344 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    40093 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_import-xml.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   372736 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_import-xml.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    36554 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    36272 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-xml.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-xml.indd
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.292593 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   271361 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   278787 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   282004 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   278792 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   205722 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   206957 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   205708 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   205726 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   207343 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   208277 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   206817 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   208159 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   204178 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    49511 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-bloc-notes.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)  1966080 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-bloc-notes.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    47823 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   585728 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    45235 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   675840 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    42578 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-edito.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   655360 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-edito.indd
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    30910 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-template.idml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.295997 SimpleIDML-1.1.3/tests/regressiontests/IDML/media/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    37435 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   103166 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/media/bouboune.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    27644 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/media/default.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   190741 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/media/default2.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   140777 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/module1.pdf
--rw-r--r--   0 guerrastanislas   (501) staff       (20)  1303348 2020-11-24 09:03:39.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/package-pirate.zip
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    41657 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/page-9modules.idml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)  1015808 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/IDML/page-9modules.indd
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.297496 SimpleIDML-1.1.3/tests/regressiontests/SOAP/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     7916 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/SOAP/indesign-service.xml
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-01-18 09:40:51.303208 SimpleIDML-1.1.3/tests/regressiontests/XML/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1105 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1073 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1074 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1259 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1279 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      947 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1030 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1071 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1041 2020-06-30 07:14:18.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1007 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1041 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml.xml
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    25869 2020-05-27 07:40:19.000000 SimpleIDML-1.1.3/tests/regressiontests/components.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2067 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/extras.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     7138 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/id_package.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   219693 2020-06-30 07:14:18.000000 SimpleIDML-1.1.3/tests/regressiontests/idml.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     6984 2020-12-04 14:34:01.000000 SimpleIDML-1.1.3/tests/regressiontests/indesign.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     9296 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/regressiontests/utils.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1715 2020-05-21 11:29:53.000000 SimpleIDML-1.1.3/tests/runtests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    29332 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1424 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/LICENSE
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       36 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/AUTHORS
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      278 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a1/tests/Makefile
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       62 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/coveragerc
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2067 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/extras.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6984 2020-12-04 14:34:01.000000 SimpleIDML-1.1.6a1/tests/regressiontests/indesign.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/__init__.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/SOAP/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7916 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/SOAP/indesign-service.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1259 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1007 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1071 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1279 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1041 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1073 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1105 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1074 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      947 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1104 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1041 2020-06-30 07:14:18.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1030 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     9296 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7138 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/id_package.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   219693 2020-06-30 07:14:18.000000 SimpleIDML-1.1.6a1/tests/regressiontests/idml.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    25869 2020-05-27 07:40:19.000000 SimpleIDML-1.1.6a1/tests/regressiontests/components.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    36272 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    45235 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   675840 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1303348 2020-11-24 09:03:39.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/package-pirate.zip
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    46702 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   466944 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   860160 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37291 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.idml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   282004 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   207343 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205726 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   204178 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205708 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206957 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   278792 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   271361 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   208277 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206817 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   278787 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   208159 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206617 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   205722 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    41657 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   585728 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1015808 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    47823 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   335872 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35520 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   389120 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    36554 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7221 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35821 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    15342 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    73611 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    16154 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/designmap.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      253 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/container.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    25538 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       43 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/mimetype
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      732 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      274 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/Mapping.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1302 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/Tags.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1315 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2320 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      940 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Spreads/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19082 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/MasterSpreads/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2608 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   360448 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   575266 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-package.zip
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40775 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   864256 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)  1966080 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    45371 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    49511 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   140777 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/module1.pdf
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   372736 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    30910 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-template.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40093 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   569344 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   364544 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40088 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    40175 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.idml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   655360 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.indd
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    42578 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.idml
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37435 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   103166 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/bouboune.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   190741 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default2.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    27644 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1632 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a1/tests/runtests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      198 2022-03-14 13:09:46.000000 SimpleIDML-1.1.6a1/MANIFEST.in
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1785 2023-04-17 14:17:50.000000 SimpleIDML-1.1.6a1/setup.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    22600 2023-04-17 06:31:13.000000 SimpleIDML-1.1.6a1/README.rst
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    29332 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6585 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       14 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       12 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/top_level.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/dependency_links.txt
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/simple_idml/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      681 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/extras.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      322 2023-04-17 14:17:50.000000 SimpleIDML-1.1.6a1/src/simple_idml/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4486 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/test.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3436 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1795 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/id_package.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    11609 2023-02-20 07:55:47.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/indesign.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/__init__.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      285 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/list_profiles.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      126 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/close_all_documents.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      636 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/save_as.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12733 2022-01-18 09:35:17.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/export.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1190 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/package_to_print.jsx
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    50966 2023-04-17 12:02:50.000000 SimpleIDML-1.1.6a1/src/simple_idml/idml.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      247 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/exceptions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    37323 2023-04-17 12:05:26.000000 SimpleIDML-1.1.6a1/src/simple_idml/components.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6906 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/ftp.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2369 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/simple_idml/commands.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2211 2023-04-17 11:58:25.000000 SimpleIDML-1.1.6a1/src/simple_idml/decorators.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-17 14:18:15.000000 SimpleIDML-1.1.6a1/src/scripts/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      682 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_close_all_documents.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      618 2020-05-21 11:29:53.000000 SimpleIDML-1.1.6a1/src/scripts/simpleidml_create_package_from_dir.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3653 2023-02-20 07:55:46.000000 SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_save_as.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `SimpleIDML-1.1.3/LICENSE` & `SimpleIDML-1.1.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/PKG-INFO` & `SimpleIDML-1.1.6a1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,25 @@
-Metadata-Version: 2.1
-Name: SimpleIDML
-Version: 1.1.3
-Summary: A library to manipulate Adobe(r) IDML(r) files.
-Home-page: https://github.com/Starou/SimpleIDML
-Author: Stanislas Guerra
-Author-email: stanislas.guerra@gmail.com
-License: BSD Licence
-Project-URL: Source Code, https://github.com/Starou/SimpleIDML
-Project-URL: Issue Tracker, https://github.com/Starou/SimpleIDML/issues
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Printing
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
-License-File: AUTHORS
-
 ==========
 SimpleIDML
 ==========
 
-.. image:: https://coveralls.io/repos/Starou/SimpleIDML/badge.png
-  :target: https://coveralls.io/r/Starou/SimpleIDML
-
 .. image:: https://img.shields.io/pypi/v/simpleidml.svg
   :target: https://pypi.python.org/pypi/SimpleIDML
 
 .. image:: https://img.shields.io/pypi/pyversions/simpleidml.svg
     :target: https://pypi.python.org/pypi/SimpleIDML/
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/l/simpleidml.svg
     :target: https://pypi.python.org/pypi/SimpleIDML/
     :alt: License
 
-.. image:: https://travis-ci.org/Starou/SimpleIDML.svg
-    :target: https://travis-ci.org/Starou/SimpleIDML
-    :alt: Travis C.I.
+.. image:: https://coveralls.io/repos/github/Starou/SimpleIDML/badge.svg?branch=master
+    :target: https://coveralls.io/github/Starou/SimpleIDML?branch=master
+
 
 Installation
 ============
 
 Use ``pip``:
 
 .. code-block:: bash
@@ -482,14 +453,25 @@
 
 A script (``simpleidml_indesign_save_as.py``) that wraps these functions is
 installed in your PATH.
 
 Revisions
 =========
 
+1.1.5
+-----
+
+- Add a ``page_number`` parameter to ``IDMLPackage.import_pdf()`` so that you
+  can choose which page from the PDF file to display.
+
+1.1.4
+-----
+
+- PyLint refactorisation.
+
 1.1.3
 -----
 
 - Catch and log exceptions to the InDesign Server when setting options in
   export.jsx. Thanks to @kylehodgson for the contribution.
 
 1.1.2
@@ -731,9 +713,7 @@
 Bugfixes
 ''''''''
 
 Tickets #19, #21 (orphan layers), #23 (AssertXMLEqual), #24 (import_xml() failure).
 
 
 .. _XPath: http://en.wikipedia.org/wiki/XPath
-
-
```

### Comparing `SimpleIDML-1.1.3/README.rst` & `SimpleIDML-1.1.6a1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,711 +1,743 @@
-==========
-SimpleIDML
-==========
-
-.. image:: https://coveralls.io/repos/Starou/SimpleIDML/badge.png
-  :target: https://coveralls.io/r/Starou/SimpleIDML
-
-.. image:: https://img.shields.io/pypi/v/simpleidml.svg
-  :target: https://pypi.python.org/pypi/SimpleIDML
-
-.. image:: https://img.shields.io/pypi/pyversions/simpleidml.svg
-    :target: https://pypi.python.org/pypi/SimpleIDML/
-    :alt: Supported Python versions
-
-.. image:: https://img.shields.io/pypi/l/simpleidml.svg
-    :target: https://pypi.python.org/pypi/SimpleIDML/
-    :alt: License
-
-.. image:: https://travis-ci.org/Starou/SimpleIDML.svg
-    :target: https://travis-ci.org/Starou/SimpleIDML
-    :alt: Travis C.I.
-
-Installation
-============
-
-Use ``pip``:
-
-.. code-block:: bash
-
-    pip install SimpleIDML
-
-Or:
-
-.. code-block:: bash
-
-    python setup.py build
-    sudo python setup.py install
-
-Python support
---------------
-
-- Python 3: 3.6+
-
-Any questions?
---------------
-
-https://groups.google.com/forum/#!forum/simpleidml-users
-
-Developers
-----------
-
-.. code-block:: bash
-
-    vagrant up
-    vagrant ssh
-    cd tests
-    python runtests.py
-
-What is SimpleIDML?
-===================
-
-SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML file. The main purpose being
-the ability to compose IDML files together and produce complex documents from simple pieces and
-to separate the data from the structure.
-
-The philosophy behind SimpleIDML is to keep separated the content and the structure and to use XML
-files to feed your documents by using the XML Structure in InDesign.
-Keeping this isolation is important to ease the debugging and to keep track of what is going on.
-
-I urge you to take a look in the *regressiontests* directory for real-world examples.
-
-Uses cases - success story(ies)
-===============================
-
-Le Figaro - FigaroClassifieds
------------------------------
-
-SimpleIDML is used in production at *Le Figaro* aside in-house tools managing the content of
-Classifieds Ads magazines like *Propriétés de France* or *Belles Maisons à louer*.
-These tools produces XML files describing the page layout (which IDML templates and sub-templates
-to use) and the page content.
-The XML files feed another tool - the one using SimpleIDML - that compose the final page.
-
-The steps of the (simplified) process of composition are:
-
-1. Get the main IDML template (the page) ;
-2. Ad the sub-templates (the ads) into the page template ;
-3. Import the content into the final IDML file ;
-4. Edit the file in InDesign ;
-5. Push the changesets back to the content management application and update the database.
-
-There is a lot of cool features in this application. You can update a part of a page already or
-partially composed for example.
-
-Architecture
-''''''''''''
-
-These applications are web-applications. The communication is done by web-services feeding a task
-queue (RabbitMQ/Celery).
-
-The performances are quite good. Composing a document require a fraction of a second.
-
-What are IDML files?
-====================
-
-IDML (*InDesign Markup Language*) files are a Zip archives (Adobe calls them packages) storing
-essentially XML files. Adobe made a descent job because those files can completely express the
-content of the native (binary) documents.
-This is a small revolution in the print world when it comes to automatically process files in both
-ways from templates and database (Round-trip) without using proprietary server-edition of
-Publishing Software.
-
-What does SimpleIDML do?
-========================
-
-Package exploration
--------------------
-
-You can discover the structure of your IDML files:
-
-.. code-block:: python
-
-    >>> from simple_idml import idml
-    >>> my_idml_package = idml.IDMLPackage("/path/to/my_main_document.idml")
-    >>> my_idml_package.spreads
-    [u'Spreads/Spread_ub6.xml', u'Spreads/Spread_ubc.xml', u'Spreads/Spread_uc3.xml']
-    >>> my_idml_package.stories
-    [u'Stories/Story_u139.xml', u'Stories/Story_u11b.xml',
-     u'Stories/Story_u102.xml', u'Stories/Story_ue4.xml']
-
-Some attributes are *lxml.etree* Elements or Documents:
-
-.. code-block:: python
-
-    >>> my_package.font_families
-    [<Element FontFamily at 0x1010048c0>,
-     <Element FontFamily at 0x101004a50>,
-     <Element FontFamily at 0x101004aa0>,
-        <Element FontFamily at 0x101004af0>]
-    >>> [e.get("Name") for e in my_package.font_families]
-    ['Minion Pro', 'Myriad Pro', 'Kozuka Mincho Pro', 'Vollkorn']
-
-    >>> my_package.xml_structure
-    <Element Root at 0x101004910>
-    >>> from lxml import etree
-    >>> # print my_package.xml_structure_pretty() is a shortcut for:
-    >>> print etree.tostring(my_package.xml_structure, pretty_print=True)
-    <Root Self="di2">
-      <article XMLContent="u102" Self="di2i3">
-        <Story XMLContent="ue4" Self="di2i3i1">
-          <title Self="di2i3i1i1"/>
-          <subtitle Self="di2i3i1i2"/>
-        </Story>
-        <content XMLContent="u11b" Self="di2i3i2"/>
-        <illustration XMLContent="u135" Self="di2i3i3"/>
-        <description XMLContent="u139" Self="di2i3i4"/>
-      </article>
-      <article XMLContent="udb" Self="di2i4"/>
-      <article XMLContent="udd" Self="di2i5"/>
-      <advertise XMLContent="udf" Self="di2i6"/>
-    </Root>
-
-
-``xml_structure`` attribute is a representation of the XML Structure of your InDesign XML-ready
-document (The one you want to use to populate the content with data from an external XML file
-having the same structure).
-
-
-Build package
--------------
-
-There is a convenient script to create a IDML package from a flat directory called
-*simpleidml_create_package_from_dir.py* which should be in your PATH.
-
-
-Compose document
-----------------
-
-**Important**: You should always use a ``with`` context when using side-effect methods on
-``IDMLPackage`` instances returning new instances.
-
-
-For example, the following is bad because ``my_doc`` initial instance reference is lost and
-the associated file cannot be properly closed. This may rise an exception on Windows platform
-if you try to ``os.unlink()`` an unclosed file.
-
-.. code-block:: python
-
-    from simple_idml import idml
-    my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
-    my_doc = my_doc.prefix("main")
-
-Instead, use:
-
-.. code-block:: python
-
-    from simple_idml import idml
-    my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
-    with my_doc.prefix("main") as f:
-        # some code.
-
-Insert elements
-'''''''''''''''
-
-Using the XML Structure you can ask SimpleIDML to insert into a document at a XML tag the content
-of another XML tag from another document. The tag paths are expressed using XPath_ syntax.
-Note that you should always make a copy of your idml files before altering them with
-``shutil.copy2(src, dst)`` for instance and prefix your document before using ``insert_idml()``
-to avoid reference collisions.
-
-.. code-block:: python
-
-    >>> from simple_idml import idml
-    >>> idml_main = idml.IDMLPackage("/path/to/my_main_document.idml")
-    >>> idml_module = idml.IDMLPackage("/path/to/my_small_document.idml")
-
-    >>> with idml_main.prefix("main") as p_idml_main, \
-    >>>      idml_module.prefix("article") as p_idml_article:
-
-    >>>     with p_idml_main.insert_idml(p_idml_article, at="/Root/article[3]",
-                                         only="/Root/module[1]") as f:
-    >>>         f.stories
-    ['Stories/Story_article1u188.xml', 'Stories/Story_article1u19f.xml',
-     'Stories/Story_article1u1db.xml', 'Stories/Story_mainu102.xml',
-     'Stories/Story_mainu11b.xml', 'Stories/Story_mainu139.xml',
-     'Stories/Story_mainue4.xml']
-
-
-    >>>         print f.xml_structure_pretty()
-    <Root Self="maindi2">
-      <article XMLContent="mainu102" Self="maindi2i3">
-        <Story XMLContent="mainue4" Self="maindi2i3i1">
-          <title Self="maindi2i3i1i1"/>
-          <subtitle Self="maindi2i3i1i2"/>
-        </Story>
-        <content XMLContent="mainu11b" Self="maindi2i3i2"/>
-        <illustration XMLContent="mainu135" Self="maindi2i3i3"/>
-        <description XMLContent="mainu139" Self="maindi2i3i4"/>
-      </article>
-      <article XMLContent="mainudb" Self="maindi2i4"/>
-      <article Self="maindi2i5">
-        <module XMLContent="article1u1db" Self="article1di3i12">
-          <main_picture XMLContent="article1u182" Self="article1di3i12i1"/>
-          <headline XMLContent="article1u188" Self="article1di3i12i2"/>
-          <Story XMLContent="article1u19f" Self="article1di3i12i3">
-            <article Self="article1di3i12i3i2"/>
-            <informations Self="article1di3i12i3i1"/>
-          </Story>
-        </module>
-      </article>
-      <advertise XMLContent="mainudf" Self="maindi2i6"/>
-    </Root>
-
-
-Combine pages
-'''''''''''''
-
-You may need to gather pages from severals documents into a single one:
-
-.. code-block:: python
-
-    >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
-    >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
-
-    >>> # Always start by prefixing packages to avoid collision.
-    >>> with edito_idml_file.prefix("edito") as p_edito,\
-    >>>      courrier_idml_file.prefix("courrier") as p_courrier:
-    >>>     len(edito_idml_file.pages)
-    2
-
-    >>>     new_idml = p_edito.add_page_from_idml(p_courrier,
-    ...                                           page_number=1,
-    ...                                           at="/Root",
-    ...                                           only="/Root/page[1]")
-    >>>     len(new_idml.pages)
-    3
-
-    # The XML Structure has integrated the new file.
-    >>>     print etree.tostring(new_idml.xml_structure, pretty_print=True)
-    <Root Self="editodi2">
-      <page Self="editodi2ib">
-        <article Self="editodi2ibif">
-          <Story XMLContent="editoue4" Self="editodi2ibifi1f">
-            <title Self="editodi2ibifi1fi1"/>
-            <subtitle Self="editodi2ibifi1fi2"/>
-          </Story>
-          <content XMLContent="editou11b" Self="editodi2ibifi1e"/>
-        </article>
-      </page>
-      <page Self="editodi2i10">
-        <advertise XMLContent="editou1de" Self="editodi2i10i23"/>
-      </page>
-      <page Self="courrierdi2ib">
-        <title XMLContent="courrieru1b2" Self="courrierdi2ibi34"/>
-        <article XMLContent="courrieru1c9" Self="courrierdi2ibi33"/>
-        <article XMLContent="courrieru1e0" Self="courrierdi2ibi32"/>
-        <article XMLContent="courrieru1fb" Self="courrierdi2ibi31"/>
-        <article XMLContent="courrieru212" Self="courrierdi2ibi30"/>
-      </page>
-    </Root>
-
-
-There is a convenient method to add several pages at once:
-
-.. code-block:: python
-
-    >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
-    >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
-    >>> bloc_notes_idml_file = IDMLPackage("magazineA-bloc-notes.idml")
-
-    >>> with edito_idml_file.prefix("edito") as p_edito,\
-    >>>      courrier_idml_file.prefix("courrier") as p_courrier,\
-    >>>      bloc_notes_idml_file.prefix("blocnotes") as p_bloc_notes:
-
-    >>>     packages_to_add = [
-    ...         (p_courrier, 1, "/Root", "/Root/page[1]"),
-    ...         (p_bloc_notes, 1, "/Root", "/Root/page[1]"),
-    ...     ]
-
-    >>>     new_idml = p_edito.add_pages_from_idml(packages_to_add)
-    >>>     len(new_idml.pages)
-    4
-    >>>     new_idml.spreads
-    ['Spreads/Spread_editoub6.xml',
-     'Spreads/Spread_editoubc.xml',
-     'Spreads/Spread_editoubd.xml']
-
-
-Import/Export XML
------------------
-
-Exporting as XML:
-
-.. code-block:: python
-
-    >>> idml_file = IDMLPackage("path/to/file.idml")
-    >>> print idml_file.export_xml()
-    <Root>
-        <module>
-            <main_picture/>
-            <headline>Hello world!</headline>
-            <Story>
-                <article>Lorem ipsum dolor sit amet, ...</article>
-                <informations>Lorem ipsum dolor sit amet,</informations>
-            </Story>
-        </module>
-    </Root>
-
-You can as well import XML file into your InDesign® documents. The following rules applies:
-
-- A node having the attribute ``simpleidml-setcontent="false"`` will not update the content of the
-  corresponding element into the idml document (but its children will be updated).
-- A node having the attribute ``simpleidml-ignorecontent"true"`` will not update the content of the
-  corresponding element into the idml document **and** its children.
-- A node having the attribute ``simpleidml-setcontent="delete"`` will remove the corresponding
-  element into the idml document (Story and Spread elements).
-- A node having the attribute ``simpleidml-setcontent="remove-previous-br"`` will remove the new-line
-  characters before the element.
-- You can mix several flags using a comma (i.e.: ``simpleidml-setcontent="delete,remove-previous-br"``)
-- In a *ignorecontent* context the content of a child node can be turned on with the
-  ``simpleidml-forcecontent="true"`` flag.
-- Images references are passed by the *href* attribute. An empty value will remove the
-  corresponding page items into the document.
-- Nested tag will be created if they are mapped with a *character-style*.
-- The style applied to the newly created tag is a combinaison of the parent character-styles and
-  the mapped one.
-
-Please take a look into the tests for in-depth examples.
-
-Import PDF
-----------
-
-A block can be used as a placeholder for a PDF file:
-
-.. code-block:: python
-
-    >>> with IDMLPackage("my_package.idml") as idml_file:
-    >>>     with idml_file.import_pdf("file:/path/to/file.pdf", at="/Root/modules/module[2]", crop="PDFCrop") as f:
-    >>>         f.export_xml()
-
-The ``crop`` parameter should be one of the ``PDFCrop_EnumValue`` from the IDML Specification
-(``"CropArt"``, ``"CropPDF"``, ``"CropTrim"``, ``"CropBleed"``, ``"CropMedia"``,
-``"CropContentVisibleLayers"``, ``"CropContentAllLayers"``, ``"CropContent"``).
-It defaults to ``CropContentVisibleLayers````
-
-Use InDesign server SOAP interface to convert a file
-----------------------------------------------------
-
-This require an *InDesign Server* and a readable/writable working directory.
-The same directory must be accessible by the client either by the filesystem or
-over FTP.
-
-The ``formats`` parameter is a list (of dicts) of formats and parameters you want
-your file to be exported into.
-The supported output formats are ``jpeg``, ``idml``, ``pdf``, ``indd`` and
-``zip`` (a zipped InDesign Package).
-
-Export parameters are provided using the ``params`` key. Use
-``simpleidml_indesign_save_as.py --help`` for a list of supported parameters.
-
-The response is a list of binary strings matching ``formats`` provided:
-
-.. code-block:: python
-
-    from simple_idml.indesign import indesign
-
-    response = indesign.save_as("/path_to_file.idml", [{"fmt": "indd"}],
-                                "http://url-to-indesign-server:port",
-                                "/path/to/client/workdir",
-                                "/path/to/indesign-server/workdir")[0]
-    with open("my_file.indd", "wb+") as f:
-        f.write(response)
-
-    response = indesign.save_as("/path_to_file.indd", [{"fmt": "idml"}],
-                                "http://url-to-indesign-server:port",
-                                "/path/to/client/workdir",
-                                "/path/to/indesign-server/workdir")[0]
-    with open("my_file.idml", "wb+") as f:
-        f.write(response)
-
-    response = indesign.save_as("/path_to_file.indd", [{
-                                    "fmt": "pdf",
-                                    "params": {"colorSpace": "CMYK"},
-                                }],
-                                "http://url-to-indesign-server:port",
-                                "/path/to/client/workdir",
-                                "/path/to/indesign-server/workdir")[0]
-    with open("my_file.pdf", "wb+") as f:
-        f.write(response)
-
-    pdf_response, jpeg_response, zip_response = indesign.save_as(
-                                    "/path_to_file.indd",
-                                    [{"fmt": "pdf"}, {"fmt": "jpeg"}, {"fmt": "zip"}],
-                                    "http://url-to-indesign-server:port",
-                                    "/path/to/client/workdir",
-                                    "/path/to/indesign-server/workdir")
-
-To convert an InDesign Package, use ``indesign.export_package_as()`` instead.
-
-If the InDesign Server instance runs on a Windows machine, set the
-``indesign_server_path_style`` parameter to ``"windows"``.
-
-If the client access to the working directory *via* FTP, you must specify that
-in the ``ftp_params`` parameter:
-
-.. code-block:: python
-
-    {
-        'auth': ("ftp://ftp.foo.org", "user_account", "s3cret-pa55word"),
-        'passive': False,
-        'keepalive': True,         # False by default (optional)
-        'keepalive_interval': 30,  # set socket.TCP_KEEPINTVL (optional)
-        'keepalive_idle': 45,      # set socket.TCP_KEEPIDLE  (optional)
-        'polite': False,           # Unilaterally close ftp connection (optional)
-    }
-
-A script (``simpleidml_indesign_save_as.py``) that wraps these functions is
-installed in your PATH.
-
-Revisions
-=========
-
-1.1.3
------
-
-- Catch and log exceptions to the InDesign Server when setting options in
-  export.jsx. Thanks to @kylehodgson for the contribution.
-
-1.1.2
------
-
-New features
-''''''''''''
-
-- Add ``indesign.export_package_as()`` to convert an InDesign Package.
-
-1.1.1
------
-
-New features
-''''''''''''
-
-- Add the possiblity to remove new-line characters when importing XML by using the flag
-  ``simpleidml-setcontent="remove-previous-br"``.
-
-1.1.0
------
-
-Removed Python 2 support.
-
-New features
-''''''''''''
-
-- Add the possiblity to remove elements when importing XML by using the flag
-  ``simpleidml-setcontent="delete"``.
-- The ``PDFCrop`` attribute is now parametrable when using ``import_pdf()``.
-- ``IDMLPackage.add_note(note, author, at=path)`` added.
-
-1.0.5
------
-
-Bug fixes
-'''''''''
-
-- Fixed ``indesign.save_as()`` in Python 3 where the jsx file was opened
-  in text mode instead of binary.
-
-1.0.3
------
-
-- Use setuptools instead of distutils for a better integration with Pypi.
-
-1.0.0
------
-
-New features
-''''''''''''
-
-- Added support for Python 3
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- Removed support for Python 2.6
-
-0.92.9
-------
-
-New features
-''''''''''''
-
-- Added ``simpleidml_indesign_profiles.py`` script to list the available joboptions
-  files on the InDesign Server using the SOAP interface.
-
-Bug fixes
-'''''''''
-
-- Fix working directory cleaning of the SOAP server when an exception is raised.
-  ``indesign.save_as()`` may be backward incompatible since the returned list
-  may contains some ``None`` (instead of raising an exception before returning
-  anything).
-- Give the list of available profiles (joboptions files) on the InDesign Server
-  if the given 'pdfExportPresetName' is not found.
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- ``indesign.close_all_documents()`` has been replace the ``CloseAllDocuments`` class
-  and its ``.execute()`` method.
-- Some util functions that wrap the basic file manipulations to manage the case of
-  a ftp access to those files have been moved from indesign.py to a new ftp.py module.
-
-0.92.8
-------
-
-New features
-''''''''''''
-
-- Added ``IDMLPackage.import_pdf()`` method.
-
-
-Bug fixes
-'''''''''
-
-- Fix ``bleedMarks`` in export.jsx.
-
-0.92.7
-------
-
-Bug fixes
-'''''''''
-
-- FillTint wasn't managed.
-- Force ``lxml < 4`` in dependencies.
-
-0.92.6
-------
-
-Bug fixes
-'''''''''
-
-- Catch errors when InDesign SOAP server fails to complete a task and raise
-  an exception.
-
-0.92.5
-------
-
-Bug fixes
-'''''''''
-
-- Handle <PDF> in `IDMLPackage._get_item_translation_for_insert()`
-
-0.92.4
-------
-
-Bug fixes
-'''''''''
-
-- Fix issue #11: Parent CharacterStyle not applied in import_xml() in some cases.
-
-0.92.2
-------
-
-New features
-''''''''''''
-
-- More ftp parameters for `indesign.save_as()` function. Hardcoded socket parameters are now
-  modifiable. And you can set the flag `polite` to `False` if you encounter hanging problem
-  on `ftp.quit()` as I do. Being unpolite calls an unilateral and rude `ftp.close()`.
-  Please upgrade your code with explicite values if you rely on the previous default
-  behavior.
-
-0.92.1
-------
-
-Bug fixes
-'''''''''
-
-- ``indesign.save_as()`` uses a dedicated temporary working directory to avoid
-  concurrent access on files.
-- Added a logger to ``indesign.save_as()`` ('simpleidml.indesign') and some debug messages.
-- Fixed hanging ``ftp.retrbinary()`` in ``indesign.save_as()`` calls by tuning the socket.
-
-0.91.8
-------
-
-New features
-''''''''''''
-
-- Added support for PDF export presets in ``indesign.save_as()``.
-
-0.91.7
-------
-
-New features
-''''''''''''
-
-- Added ``IMDLPackage.merge_layers(with_name)`` (Refs#7).
-- Added a new script ``simpleidml_indesign_close_all_documents.py``.
-
-Bug fixes
-'''''''''
-
-- In ``IDMLPackage.insert_idml()``, Elements from the same layer (but not tagged in the structure)
-  are now added in the Spread of the document of destination.
-- Better support for Windows platform.
-- Fixed character style mapping with tag when using insert_idml.
-- Fixed Export XML in some edge case.
-- Added parameters to ``simpleidml_indesign_save_as`` when exporting to PDF.
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- ``indesign.save_as()`` formats parameters is now a list of dictionaries.
-
-0.91.6
-------
-
-New features
-''''''''''''
-
-- Add the ``simpleidml-ignorecontent`` and ``simpleidml-forcecontent`` tags (XML attributes)
-  allowing one to carefully exclude a node and its children during the import XML process.
-- ``indesign.save_as()`` now works with a client working directory over a FTP.
-  This require ``wget`` to be on your system if you want to create zip packages.
-
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- ``indesign.save_as()`` require both a client workdir and a server workdir parameter.
-
-0.91.5.5
---------
-
-Bugfixes
-''''''''
-
-- <EPS> elements in Spread weren't handled correctly.
-- All spread elements were added in the destination package when using ``insert_idml()``.
-
-
-0.91.3
-------
-
-New features
-''''''''''''
-
-Add a SOAP client to call a InDesign server to get INDD file and export in various
-formats.
-
-0.91.2
-------
-
-New features
-''''''''''''
-
-- Ticket #20 - Suffix layers.
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- Ticket #22 - IDMLPackage.import_xml() parameter is a XML string and not a file object.
-
-Bugfixes
-''''''''
-
-Tickets #19, #21 (orphan layers), #23 (AssertXMLEqual), #24 (import_xml() failure).
-
-
-.. _XPath: http://en.wikipedia.org/wiki/XPath
+Metadata-Version: 1.1
+Name: SimpleIDML
+Version: 1.1.6a1
+Summary: A library to manipulate Adobe(r) IDML(r) files.
+Home-page: https://github.com/Starou/SimpleIDML
+Author: Stanislas Guerra
+Author-email: stanislas.guerra@gmail.com
+License: BSD Licence
+Project-URL: Source Code, https://github.com/Starou/SimpleIDML
+Project-URL: Issue Tracker, https://github.com/Starou/SimpleIDML/issues
+Description: ==========
+        SimpleIDML
+        ==========
+        
+        .. image:: https://img.shields.io/pypi/v/simpleidml.svg
+          :target: https://pypi.python.org/pypi/SimpleIDML
+        
+        .. image:: https://img.shields.io/pypi/pyversions/simpleidml.svg
+            :target: https://pypi.python.org/pypi/SimpleIDML/
+            :alt: Supported Python versions
+        
+        .. image:: https://img.shields.io/pypi/l/simpleidml.svg
+            :target: https://pypi.python.org/pypi/SimpleIDML/
+            :alt: License
+        
+        .. image:: https://coveralls.io/repos/github/Starou/SimpleIDML/badge.svg?branch=master
+            :target: https://coveralls.io/github/Starou/SimpleIDML?branch=master
+        
+        
+        Installation
+        ============
+        
+        Use ``pip``:
+        
+        .. code-block:: bash
+        
+            pip install SimpleIDML
+        
+        Or:
+        
+        .. code-block:: bash
+        
+            python setup.py build
+            sudo python setup.py install
+        
+        Python support
+        --------------
+        
+        - Python 3: 3.6+
+        
+        Any questions?
+        --------------
+        
+        https://groups.google.com/forum/#!forum/simpleidml-users
+        
+        Developers
+        ----------
+        
+        .. code-block:: bash
+        
+            vagrant up
+            vagrant ssh
+            cd tests
+            python runtests.py
+        
+        What is SimpleIDML?
+        ===================
+        
+        SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML file. The main purpose being
+        the ability to compose IDML files together and produce complex documents from simple pieces and
+        to separate the data from the structure.
+        
+        The philosophy behind SimpleIDML is to keep separated the content and the structure and to use XML
+        files to feed your documents by using the XML Structure in InDesign.
+        Keeping this isolation is important to ease the debugging and to keep track of what is going on.
+        
+        I urge you to take a look in the *regressiontests* directory for real-world examples.
+        
+        Uses cases - success story(ies)
+        ===============================
+        
+        Le Figaro - FigaroClassifieds
+        -----------------------------
+        
+        SimpleIDML is used in production at *Le Figaro* aside in-house tools managing the content of
+        Classifieds Ads magazines like *Propriétés de France* or *Belles Maisons à louer*.
+        These tools produces XML files describing the page layout (which IDML templates and sub-templates
+        to use) and the page content.
+        The XML files feed another tool - the one using SimpleIDML - that compose the final page.
+        
+        The steps of the (simplified) process of composition are:
+        
+        1. Get the main IDML template (the page) ;
+        2. Ad the sub-templates (the ads) into the page template ;
+        3. Import the content into the final IDML file ;
+        4. Edit the file in InDesign ;
+        5. Push the changesets back to the content management application and update the database.
+        
+        There is a lot of cool features in this application. You can update a part of a page already or
+        partially composed for example.
+        
+        Architecture
+        ''''''''''''
+        
+        These applications are web-applications. The communication is done by web-services feeding a task
+        queue (RabbitMQ/Celery).
+        
+        The performances are quite good. Composing a document require a fraction of a second.
+        
+        What are IDML files?
+        ====================
+        
+        IDML (*InDesign Markup Language*) files are a Zip archives (Adobe calls them packages) storing
+        essentially XML files. Adobe made a descent job because those files can completely express the
+        content of the native (binary) documents.
+        This is a small revolution in the print world when it comes to automatically process files in both
+        ways from templates and database (Round-trip) without using proprietary server-edition of
+        Publishing Software.
+        
+        What does SimpleIDML do?
+        ========================
+        
+        Package exploration
+        -------------------
+        
+        You can discover the structure of your IDML files:
+        
+        .. code-block:: python
+        
+            >>> from simple_idml import idml
+            >>> my_idml_package = idml.IDMLPackage("/path/to/my_main_document.idml")
+            >>> my_idml_package.spreads
+            [u'Spreads/Spread_ub6.xml', u'Spreads/Spread_ubc.xml', u'Spreads/Spread_uc3.xml']
+            >>> my_idml_package.stories
+            [u'Stories/Story_u139.xml', u'Stories/Story_u11b.xml',
+             u'Stories/Story_u102.xml', u'Stories/Story_ue4.xml']
+        
+        Some attributes are *lxml.etree* Elements or Documents:
+        
+        .. code-block:: python
+        
+            >>> my_package.font_families
+            [<Element FontFamily at 0x1010048c0>,
+             <Element FontFamily at 0x101004a50>,
+             <Element FontFamily at 0x101004aa0>,
+                <Element FontFamily at 0x101004af0>]
+            >>> [e.get("Name") for e in my_package.font_families]
+            ['Minion Pro', 'Myriad Pro', 'Kozuka Mincho Pro', 'Vollkorn']
+        
+            >>> my_package.xml_structure
+            <Element Root at 0x101004910>
+            >>> from lxml import etree
+            >>> # print my_package.xml_structure_pretty() is a shortcut for:
+            >>> print etree.tostring(my_package.xml_structure, pretty_print=True)
+            <Root Self="di2">
+              <article XMLContent="u102" Self="di2i3">
+                <Story XMLContent="ue4" Self="di2i3i1">
+                  <title Self="di2i3i1i1"/>
+                  <subtitle Self="di2i3i1i2"/>
+                </Story>
+                <content XMLContent="u11b" Self="di2i3i2"/>
+                <illustration XMLContent="u135" Self="di2i3i3"/>
+                <description XMLContent="u139" Self="di2i3i4"/>
+              </article>
+              <article XMLContent="udb" Self="di2i4"/>
+              <article XMLContent="udd" Self="di2i5"/>
+              <advertise XMLContent="udf" Self="di2i6"/>
+            </Root>
+        
+        
+        ``xml_structure`` attribute is a representation of the XML Structure of your InDesign XML-ready
+        document (The one you want to use to populate the content with data from an external XML file
+        having the same structure).
+        
+        
+        Build package
+        -------------
+        
+        There is a convenient script to create a IDML package from a flat directory called
+        *simpleidml_create_package_from_dir.py* which should be in your PATH.
+        
+        
+        Compose document
+        ----------------
+        
+        **Important**: You should always use a ``with`` context when using side-effect methods on
+        ``IDMLPackage`` instances returning new instances.
+        
+        
+        For example, the following is bad because ``my_doc`` initial instance reference is lost and
+        the associated file cannot be properly closed. This may rise an exception on Windows platform
+        if you try to ``os.unlink()`` an unclosed file.
+        
+        .. code-block:: python
+        
+            from simple_idml import idml
+            my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
+            my_doc = my_doc.prefix("main")
+        
+        Instead, use:
+        
+        .. code-block:: python
+        
+            from simple_idml import idml
+            my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
+            with my_doc.prefix("main") as f:
+                # some code.
+        
+        Insert elements
+        '''''''''''''''
+        
+        Using the XML Structure you can ask SimpleIDML to insert into a document at a XML tag the content
+        of another XML tag from another document. The tag paths are expressed using XPath_ syntax.
+        Note that you should always make a copy of your idml files before altering them with
+        ``shutil.copy2(src, dst)`` for instance and prefix your document before using ``insert_idml()``
+        to avoid reference collisions.
+        
+        .. code-block:: python
+        
+            >>> from simple_idml import idml
+            >>> idml_main = idml.IDMLPackage("/path/to/my_main_document.idml")
+            >>> idml_module = idml.IDMLPackage("/path/to/my_small_document.idml")
+        
+            >>> with idml_main.prefix("main") as p_idml_main, \
+            >>>      idml_module.prefix("article") as p_idml_article:
+        
+            >>>     with p_idml_main.insert_idml(p_idml_article, at="/Root/article[3]",
+                                                 only="/Root/module[1]") as f:
+            >>>         f.stories
+            ['Stories/Story_article1u188.xml', 'Stories/Story_article1u19f.xml',
+             'Stories/Story_article1u1db.xml', 'Stories/Story_mainu102.xml',
+             'Stories/Story_mainu11b.xml', 'Stories/Story_mainu139.xml',
+             'Stories/Story_mainue4.xml']
+        
+        
+            >>>         print f.xml_structure_pretty()
+            <Root Self="maindi2">
+              <article XMLContent="mainu102" Self="maindi2i3">
+                <Story XMLContent="mainue4" Self="maindi2i3i1">
+                  <title Self="maindi2i3i1i1"/>
+                  <subtitle Self="maindi2i3i1i2"/>
+                </Story>
+                <content XMLContent="mainu11b" Self="maindi2i3i2"/>
+                <illustration XMLContent="mainu135" Self="maindi2i3i3"/>
+                <description XMLContent="mainu139" Self="maindi2i3i4"/>
+              </article>
+              <article XMLContent="mainudb" Self="maindi2i4"/>
+              <article Self="maindi2i5">
+                <module XMLContent="article1u1db" Self="article1di3i12">
+                  <main_picture XMLContent="article1u182" Self="article1di3i12i1"/>
+                  <headline XMLContent="article1u188" Self="article1di3i12i2"/>
+                  <Story XMLContent="article1u19f" Self="article1di3i12i3">
+                    <article Self="article1di3i12i3i2"/>
+                    <informations Self="article1di3i12i3i1"/>
+                  </Story>
+                </module>
+              </article>
+              <advertise XMLContent="mainudf" Self="maindi2i6"/>
+            </Root>
+        
+        
+        Combine pages
+        '''''''''''''
+        
+        You may need to gather pages from severals documents into a single one:
+        
+        .. code-block:: python
+        
+            >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
+            >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
+        
+            >>> # Always start by prefixing packages to avoid collision.
+            >>> with edito_idml_file.prefix("edito") as p_edito,\
+            >>>      courrier_idml_file.prefix("courrier") as p_courrier:
+            >>>     len(edito_idml_file.pages)
+            2
+        
+            >>>     new_idml = p_edito.add_page_from_idml(p_courrier,
+            ...                                           page_number=1,
+            ...                                           at="/Root",
+            ...                                           only="/Root/page[1]")
+            >>>     len(new_idml.pages)
+            3
+        
+            # The XML Structure has integrated the new file.
+            >>>     print etree.tostring(new_idml.xml_structure, pretty_print=True)
+            <Root Self="editodi2">
+              <page Self="editodi2ib">
+                <article Self="editodi2ibif">
+                  <Story XMLContent="editoue4" Self="editodi2ibifi1f">
+                    <title Self="editodi2ibifi1fi1"/>
+                    <subtitle Self="editodi2ibifi1fi2"/>
+                  </Story>
+                  <content XMLContent="editou11b" Self="editodi2ibifi1e"/>
+                </article>
+              </page>
+              <page Self="editodi2i10">
+                <advertise XMLContent="editou1de" Self="editodi2i10i23"/>
+              </page>
+              <page Self="courrierdi2ib">
+                <title XMLContent="courrieru1b2" Self="courrierdi2ibi34"/>
+                <article XMLContent="courrieru1c9" Self="courrierdi2ibi33"/>
+                <article XMLContent="courrieru1e0" Self="courrierdi2ibi32"/>
+                <article XMLContent="courrieru1fb" Self="courrierdi2ibi31"/>
+                <article XMLContent="courrieru212" Self="courrierdi2ibi30"/>
+              </page>
+            </Root>
+        
+        
+        There is a convenient method to add several pages at once:
+        
+        .. code-block:: python
+        
+            >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
+            >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
+            >>> bloc_notes_idml_file = IDMLPackage("magazineA-bloc-notes.idml")
+        
+            >>> with edito_idml_file.prefix("edito") as p_edito,\
+            >>>      courrier_idml_file.prefix("courrier") as p_courrier,\
+            >>>      bloc_notes_idml_file.prefix("blocnotes") as p_bloc_notes:
+        
+            >>>     packages_to_add = [
+            ...         (p_courrier, 1, "/Root", "/Root/page[1]"),
+            ...         (p_bloc_notes, 1, "/Root", "/Root/page[1]"),
+            ...     ]
+        
+            >>>     new_idml = p_edito.add_pages_from_idml(packages_to_add)
+            >>>     len(new_idml.pages)
+            4
+            >>>     new_idml.spreads
+            ['Spreads/Spread_editoub6.xml',
+             'Spreads/Spread_editoubc.xml',
+             'Spreads/Spread_editoubd.xml']
+        
+        
+        Import/Export XML
+        -----------------
+        
+        Exporting as XML:
+        
+        .. code-block:: python
+        
+            >>> idml_file = IDMLPackage("path/to/file.idml")
+            >>> print idml_file.export_xml()
+            <Root>
+                <module>
+                    <main_picture/>
+                    <headline>Hello world!</headline>
+                    <Story>
+                        <article>Lorem ipsum dolor sit amet, ...</article>
+                        <informations>Lorem ipsum dolor sit amet,</informations>
+                    </Story>
+                </module>
+            </Root>
+        
+        You can as well import XML file into your InDesign® documents. The following rules applies:
+        
+        - A node having the attribute ``simpleidml-setcontent="false"`` will not update the content of the
+          corresponding element into the idml document (but its children will be updated).
+        - A node having the attribute ``simpleidml-ignorecontent"true"`` will not update the content of the
+          corresponding element into the idml document **and** its children.
+        - A node having the attribute ``simpleidml-setcontent="delete"`` will remove the corresponding
+          element into the idml document (Story and Spread elements).
+        - A node having the attribute ``simpleidml-setcontent="remove-previous-br"`` will remove the new-line
+          characters before the element.
+        - You can mix several flags using a comma (i.e.: ``simpleidml-setcontent="delete,remove-previous-br"``)
+        - In a *ignorecontent* context the content of a child node can be turned on with the
+          ``simpleidml-forcecontent="true"`` flag.
+        - Images references are passed by the *href* attribute. An empty value will remove the
+          corresponding page items into the document.
+        - Nested tag will be created if they are mapped with a *character-style*.
+        - The style applied to the newly created tag is a combinaison of the parent character-styles and
+          the mapped one.
+        
+        Please take a look into the tests for in-depth examples.
+        
+        Import PDF
+        ----------
+        
+        A block can be used as a placeholder for a PDF file:
+        
+        .. code-block:: python
+        
+            >>> with IDMLPackage("my_package.idml") as idml_file:
+            >>>     with idml_file.import_pdf("file:/path/to/file.pdf", at="/Root/modules/module[2]", crop="PDFCrop") as f:
+            >>>         f.export_xml()
+        
+        The ``crop`` parameter should be one of the ``PDFCrop_EnumValue`` from the IDML Specification
+        (``"CropArt"``, ``"CropPDF"``, ``"CropTrim"``, ``"CropBleed"``, ``"CropMedia"``,
+        ``"CropContentVisibleLayers"``, ``"CropContentAllLayers"``, ``"CropContent"``).
+        It defaults to ``CropContentVisibleLayers````
+        
+        Use InDesign server SOAP interface to convert a file
+        ----------------------------------------------------
+        
+        This require an *InDesign Server* and a readable/writable working directory.
+        The same directory must be accessible by the client either by the filesystem or
+        over FTP.
+        
+        The ``formats`` parameter is a list (of dicts) of formats and parameters you want
+        your file to be exported into.
+        The supported output formats are ``jpeg``, ``idml``, ``pdf``, ``indd`` and
+        ``zip`` (a zipped InDesign Package).
+        
+        Export parameters are provided using the ``params`` key. Use
+        ``simpleidml_indesign_save_as.py --help`` for a list of supported parameters.
+        
+        The response is a list of binary strings matching ``formats`` provided:
+        
+        .. code-block:: python
+        
+            from simple_idml.indesign import indesign
+        
+            response = indesign.save_as("/path_to_file.idml", [{"fmt": "indd"}],
+                                        "http://url-to-indesign-server:port",
+                                        "/path/to/client/workdir",
+                                        "/path/to/indesign-server/workdir")[0]
+            with open("my_file.indd", "wb+") as f:
+                f.write(response)
+        
+            response = indesign.save_as("/path_to_file.indd", [{"fmt": "idml"}],
+                                        "http://url-to-indesign-server:port",
+                                        "/path/to/client/workdir",
+                                        "/path/to/indesign-server/workdir")[0]
+            with open("my_file.idml", "wb+") as f:
+                f.write(response)
+        
+            response = indesign.save_as("/path_to_file.indd", [{
+                                            "fmt": "pdf",
+                                            "params": {"colorSpace": "CMYK"},
+                                        }],
+                                        "http://url-to-indesign-server:port",
+                                        "/path/to/client/workdir",
+                                        "/path/to/indesign-server/workdir")[0]
+            with open("my_file.pdf", "wb+") as f:
+                f.write(response)
+        
+            pdf_response, jpeg_response, zip_response = indesign.save_as(
+                                            "/path_to_file.indd",
+                                            [{"fmt": "pdf"}, {"fmt": "jpeg"}, {"fmt": "zip"}],
+                                            "http://url-to-indesign-server:port",
+                                            "/path/to/client/workdir",
+                                            "/path/to/indesign-server/workdir")
+        
+        To convert an InDesign Package, use ``indesign.export_package_as()`` instead.
+        
+        If the InDesign Server instance runs on a Windows machine, set the
+        ``indesign_server_path_style`` parameter to ``"windows"``.
+        
+        If the client access to the working directory *via* FTP, you must specify that
+        in the ``ftp_params`` parameter:
+        
+        .. code-block:: python
+        
+            {
+                'auth': ("ftp://ftp.foo.org", "user_account", "s3cret-pa55word"),
+                'passive': False,
+                'keepalive': True,         # False by default (optional)
+                'keepalive_interval': 30,  # set socket.TCP_KEEPINTVL (optional)
+                'keepalive_idle': 45,      # set socket.TCP_KEEPIDLE  (optional)
+                'polite': False,           # Unilaterally close ftp connection (optional)
+            }
+        
+        A script (``simpleidml_indesign_save_as.py``) that wraps these functions is
+        installed in your PATH.
+        
+        Revisions
+        =========
+        
+        1.1.5
+        -----
+        
+        - Add a ``page_number`` parameter to ``IDMLPackage.import_pdf()`` so that you
+          can choose which page from the PDF file to display.
+        
+        1.1.4
+        -----
+        
+        - PyLint refactorisation.
+        
+        1.1.3
+        -----
+        
+        - Catch and log exceptions to the InDesign Server when setting options in
+          export.jsx. Thanks to @kylehodgson for the contribution.
+        
+        1.1.2
+        -----
+        
+        New features
+        ''''''''''''
+        
+        - Add ``indesign.export_package_as()`` to convert an InDesign Package.
+        
+        1.1.1
+        -----
+        
+        New features
+        ''''''''''''
+        
+        - Add the possiblity to remove new-line characters when importing XML by using the flag
+          ``simpleidml-setcontent="remove-previous-br"``.
+        
+        1.1.0
+        -----
+        
+        Removed Python 2 support.
+        
+        New features
+        ''''''''''''
+        
+        - Add the possiblity to remove elements when importing XML by using the flag
+          ``simpleidml-setcontent="delete"``.
+        - The ``PDFCrop`` attribute is now parametrable when using ``import_pdf()``.
+        - ``IDMLPackage.add_note(note, author, at=path)`` added.
+        
+        1.0.5
+        -----
+        
+        Bug fixes
+        '''''''''
+        
+        - Fixed ``indesign.save_as()`` in Python 3 where the jsx file was opened
+          in text mode instead of binary.
+        
+        1.0.3
+        -----
+        
+        - Use setuptools instead of distutils for a better integration with Pypi.
+        
+        1.0.0
+        -----
+        
+        New features
+        ''''''''''''
+        
+        - Added support for Python 3
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - Removed support for Python 2.6
+        
+        0.92.9
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added ``simpleidml_indesign_profiles.py`` script to list the available joboptions
+          files on the InDesign Server using the SOAP interface.
+        
+        Bug fixes
+        '''''''''
+        
+        - Fix working directory cleaning of the SOAP server when an exception is raised.
+          ``indesign.save_as()`` may be backward incompatible since the returned list
+          may contains some ``None`` (instead of raising an exception before returning
+          anything).
+        - Give the list of available profiles (joboptions files) on the InDesign Server
+          if the given 'pdfExportPresetName' is not found.
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - ``indesign.close_all_documents()`` has been replace the ``CloseAllDocuments`` class
+          and its ``.execute()`` method.
+        - Some util functions that wrap the basic file manipulations to manage the case of
+          a ftp access to those files have been moved from indesign.py to a new ftp.py module.
+        
+        0.92.8
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added ``IDMLPackage.import_pdf()`` method.
+        
+        
+        Bug fixes
+        '''''''''
+        
+        - Fix ``bleedMarks`` in export.jsx.
+        
+        0.92.7
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - FillTint wasn't managed.
+        - Force ``lxml < 4`` in dependencies.
+        
+        0.92.6
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - Catch errors when InDesign SOAP server fails to complete a task and raise
+          an exception.
+        
+        0.92.5
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - Handle <PDF> in `IDMLPackage._get_item_translation_for_insert()`
+        
+        0.92.4
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - Fix issue #11: Parent CharacterStyle not applied in import_xml() in some cases.
+        
+        0.92.2
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - More ftp parameters for `indesign.save_as()` function. Hardcoded socket parameters are now
+          modifiable. And you can set the flag `polite` to `False` if you encounter hanging problem
+          on `ftp.quit()` as I do. Being unpolite calls an unilateral and rude `ftp.close()`.
+          Please upgrade your code with explicite values if you rely on the previous default
+          behavior.
+        
+        0.92.1
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - ``indesign.save_as()`` uses a dedicated temporary working directory to avoid
+          concurrent access on files.
+        - Added a logger to ``indesign.save_as()`` ('simpleidml.indesign') and some debug messages.
+        - Fixed hanging ``ftp.retrbinary()`` in ``indesign.save_as()`` calls by tuning the socket.
+        
+        0.91.8
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added support for PDF export presets in ``indesign.save_as()``.
+        
+        0.91.7
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added ``IMDLPackage.merge_layers(with_name)`` (Refs#7).
+        - Added a new script ``simpleidml_indesign_close_all_documents.py``.
+        
+        Bug fixes
+        '''''''''
+        
+        - In ``IDMLPackage.insert_idml()``, Elements from the same layer (but not tagged in the structure)
+          are now added in the Spread of the document of destination.
+        - Better support for Windows platform.
+        - Fixed character style mapping with tag when using insert_idml.
+        - Fixed Export XML in some edge case.
+        - Added parameters to ``simpleidml_indesign_save_as`` when exporting to PDF.
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - ``indesign.save_as()`` formats parameters is now a list of dictionaries.
+        
+        0.91.6
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Add the ``simpleidml-ignorecontent`` and ``simpleidml-forcecontent`` tags (XML attributes)
+          allowing one to carefully exclude a node and its children during the import XML process.
+        - ``indesign.save_as()`` now works with a client working directory over a FTP.
+          This require ``wget`` to be on your system if you want to create zip packages.
+        
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - ``indesign.save_as()`` require both a client workdir and a server workdir parameter.
+        
+        0.91.5.5
+        --------
+        
+        Bugfixes
+        ''''''''
+        
+        - <EPS> elements in Spread weren't handled correctly.
+        - All spread elements were added in the destination package when using ``insert_idml()``.
+        
+        
+        0.91.3
+        ------
+        
+        New features
+        ''''''''''''
+        
+        Add a SOAP client to call a InDesign server to get INDD file and export in various
+        formats.
+        
+        0.91.2
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Ticket #20 - Suffix layers.
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - Ticket #22 - IDMLPackage.import_xml() parameter is a XML string and not a file object.
+        
+        Bugfixes
+        ''''''''
+        
+        Tickets #19, #21 (orphan layers), #23 (AssertXMLEqual), #24 (import_xml() failure).
+        
+        
+        .. _XPath: http://en.wikipedia.org/wiki/XPath
+        
+Platform: UNKNOWN
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Printing
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `SimpleIDML-1.1.3/setup.py` & `SimpleIDML-1.1.6a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="SimpleIDML",
-    version="1.1.3",
+    version="1.1.6a1",
     license='BSD Licence',
     author='Stanislas Guerra',
     author_email='stanislas.guerra@gmail.com',
     description='A library to manipulate Adobe(r) IDML(r) files.',
     long_description=README,
     url='https://github.com/Starou/SimpleIDML',
     project_urls={
```

### Comparing `SimpleIDML-1.1.3/src/SimpleIDML.egg-info/PKG-INFO` & `SimpleIDML-1.1.6a1/src/SimpleIDML.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,739 +1,743 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: SimpleIDML
-Version: 1.1.3
+Version: 1.1.6a1
 Summary: A library to manipulate Adobe(r) IDML(r) files.
 Home-page: https://github.com/Starou/SimpleIDML
 Author: Stanislas Guerra
 Author-email: stanislas.guerra@gmail.com
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/SimpleIDML
 Project-URL: Issue Tracker, https://github.com/Starou/SimpleIDML/issues
+Description: ==========
+        SimpleIDML
+        ==========
+        
+        .. image:: https://img.shields.io/pypi/v/simpleidml.svg
+          :target: https://pypi.python.org/pypi/SimpleIDML
+        
+        .. image:: https://img.shields.io/pypi/pyversions/simpleidml.svg
+            :target: https://pypi.python.org/pypi/SimpleIDML/
+            :alt: Supported Python versions
+        
+        .. image:: https://img.shields.io/pypi/l/simpleidml.svg
+            :target: https://pypi.python.org/pypi/SimpleIDML/
+            :alt: License
+        
+        .. image:: https://coveralls.io/repos/github/Starou/SimpleIDML/badge.svg?branch=master
+            :target: https://coveralls.io/github/Starou/SimpleIDML?branch=master
+        
+        
+        Installation
+        ============
+        
+        Use ``pip``:
+        
+        .. code-block:: bash
+        
+            pip install SimpleIDML
+        
+        Or:
+        
+        .. code-block:: bash
+        
+            python setup.py build
+            sudo python setup.py install
+        
+        Python support
+        --------------
+        
+        - Python 3: 3.6+
+        
+        Any questions?
+        --------------
+        
+        https://groups.google.com/forum/#!forum/simpleidml-users
+        
+        Developers
+        ----------
+        
+        .. code-block:: bash
+        
+            vagrant up
+            vagrant ssh
+            cd tests
+            python runtests.py
+        
+        What is SimpleIDML?
+        ===================
+        
+        SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML file. The main purpose being
+        the ability to compose IDML files together and produce complex documents from simple pieces and
+        to separate the data from the structure.
+        
+        The philosophy behind SimpleIDML is to keep separated the content and the structure and to use XML
+        files to feed your documents by using the XML Structure in InDesign.
+        Keeping this isolation is important to ease the debugging and to keep track of what is going on.
+        
+        I urge you to take a look in the *regressiontests* directory for real-world examples.
+        
+        Uses cases - success story(ies)
+        ===============================
+        
+        Le Figaro - FigaroClassifieds
+        -----------------------------
+        
+        SimpleIDML is used in production at *Le Figaro* aside in-house tools managing the content of
+        Classifieds Ads magazines like *Propriétés de France* or *Belles Maisons à louer*.
+        These tools produces XML files describing the page layout (which IDML templates and sub-templates
+        to use) and the page content.
+        The XML files feed another tool - the one using SimpleIDML - that compose the final page.
+        
+        The steps of the (simplified) process of composition are:
+        
+        1. Get the main IDML template (the page) ;
+        2. Ad the sub-templates (the ads) into the page template ;
+        3. Import the content into the final IDML file ;
+        4. Edit the file in InDesign ;
+        5. Push the changesets back to the content management application and update the database.
+        
+        There is a lot of cool features in this application. You can update a part of a page already or
+        partially composed for example.
+        
+        Architecture
+        ''''''''''''
+        
+        These applications are web-applications. The communication is done by web-services feeding a task
+        queue (RabbitMQ/Celery).
+        
+        The performances are quite good. Composing a document require a fraction of a second.
+        
+        What are IDML files?
+        ====================
+        
+        IDML (*InDesign Markup Language*) files are a Zip archives (Adobe calls them packages) storing
+        essentially XML files. Adobe made a descent job because those files can completely express the
+        content of the native (binary) documents.
+        This is a small revolution in the print world when it comes to automatically process files in both
+        ways from templates and database (Round-trip) without using proprietary server-edition of
+        Publishing Software.
+        
+        What does SimpleIDML do?
+        ========================
+        
+        Package exploration
+        -------------------
+        
+        You can discover the structure of your IDML files:
+        
+        .. code-block:: python
+        
+            >>> from simple_idml import idml
+            >>> my_idml_package = idml.IDMLPackage("/path/to/my_main_document.idml")
+            >>> my_idml_package.spreads
+            [u'Spreads/Spread_ub6.xml', u'Spreads/Spread_ubc.xml', u'Spreads/Spread_uc3.xml']
+            >>> my_idml_package.stories
+            [u'Stories/Story_u139.xml', u'Stories/Story_u11b.xml',
+             u'Stories/Story_u102.xml', u'Stories/Story_ue4.xml']
+        
+        Some attributes are *lxml.etree* Elements or Documents:
+        
+        .. code-block:: python
+        
+            >>> my_package.font_families
+            [<Element FontFamily at 0x1010048c0>,
+             <Element FontFamily at 0x101004a50>,
+             <Element FontFamily at 0x101004aa0>,
+                <Element FontFamily at 0x101004af0>]
+            >>> [e.get("Name") for e in my_package.font_families]
+            ['Minion Pro', 'Myriad Pro', 'Kozuka Mincho Pro', 'Vollkorn']
+        
+            >>> my_package.xml_structure
+            <Element Root at 0x101004910>
+            >>> from lxml import etree
+            >>> # print my_package.xml_structure_pretty() is a shortcut for:
+            >>> print etree.tostring(my_package.xml_structure, pretty_print=True)
+            <Root Self="di2">
+              <article XMLContent="u102" Self="di2i3">
+                <Story XMLContent="ue4" Self="di2i3i1">
+                  <title Self="di2i3i1i1"/>
+                  <subtitle Self="di2i3i1i2"/>
+                </Story>
+                <content XMLContent="u11b" Self="di2i3i2"/>
+                <illustration XMLContent="u135" Self="di2i3i3"/>
+                <description XMLContent="u139" Self="di2i3i4"/>
+              </article>
+              <article XMLContent="udb" Self="di2i4"/>
+              <article XMLContent="udd" Self="di2i5"/>
+              <advertise XMLContent="udf" Self="di2i6"/>
+            </Root>
+        
+        
+        ``xml_structure`` attribute is a representation of the XML Structure of your InDesign XML-ready
+        document (The one you want to use to populate the content with data from an external XML file
+        having the same structure).
+        
+        
+        Build package
+        -------------
+        
+        There is a convenient script to create a IDML package from a flat directory called
+        *simpleidml_create_package_from_dir.py* which should be in your PATH.
+        
+        
+        Compose document
+        ----------------
+        
+        **Important**: You should always use a ``with`` context when using side-effect methods on
+        ``IDMLPackage`` instances returning new instances.
+        
+        
+        For example, the following is bad because ``my_doc`` initial instance reference is lost and
+        the associated file cannot be properly closed. This may rise an exception on Windows platform
+        if you try to ``os.unlink()`` an unclosed file.
+        
+        .. code-block:: python
+        
+            from simple_idml import idml
+            my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
+            my_doc = my_doc.prefix("main")
+        
+        Instead, use:
+        
+        .. code-block:: python
+        
+            from simple_idml import idml
+            my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
+            with my_doc.prefix("main") as f:
+                # some code.
+        
+        Insert elements
+        '''''''''''''''
+        
+        Using the XML Structure you can ask SimpleIDML to insert into a document at a XML tag the content
+        of another XML tag from another document. The tag paths are expressed using XPath_ syntax.
+        Note that you should always make a copy of your idml files before altering them with
+        ``shutil.copy2(src, dst)`` for instance and prefix your document before using ``insert_idml()``
+        to avoid reference collisions.
+        
+        .. code-block:: python
+        
+            >>> from simple_idml import idml
+            >>> idml_main = idml.IDMLPackage("/path/to/my_main_document.idml")
+            >>> idml_module = idml.IDMLPackage("/path/to/my_small_document.idml")
+        
+            >>> with idml_main.prefix("main") as p_idml_main, \
+            >>>      idml_module.prefix("article") as p_idml_article:
+        
+            >>>     with p_idml_main.insert_idml(p_idml_article, at="/Root/article[3]",
+                                                 only="/Root/module[1]") as f:
+            >>>         f.stories
+            ['Stories/Story_article1u188.xml', 'Stories/Story_article1u19f.xml',
+             'Stories/Story_article1u1db.xml', 'Stories/Story_mainu102.xml',
+             'Stories/Story_mainu11b.xml', 'Stories/Story_mainu139.xml',
+             'Stories/Story_mainue4.xml']
+        
+        
+            >>>         print f.xml_structure_pretty()
+            <Root Self="maindi2">
+              <article XMLContent="mainu102" Self="maindi2i3">
+                <Story XMLContent="mainue4" Self="maindi2i3i1">
+                  <title Self="maindi2i3i1i1"/>
+                  <subtitle Self="maindi2i3i1i2"/>
+                </Story>
+                <content XMLContent="mainu11b" Self="maindi2i3i2"/>
+                <illustration XMLContent="mainu135" Self="maindi2i3i3"/>
+                <description XMLContent="mainu139" Self="maindi2i3i4"/>
+              </article>
+              <article XMLContent="mainudb" Self="maindi2i4"/>
+              <article Self="maindi2i5">
+                <module XMLContent="article1u1db" Self="article1di3i12">
+                  <main_picture XMLContent="article1u182" Self="article1di3i12i1"/>
+                  <headline XMLContent="article1u188" Self="article1di3i12i2"/>
+                  <Story XMLContent="article1u19f" Self="article1di3i12i3">
+                    <article Self="article1di3i12i3i2"/>
+                    <informations Self="article1di3i12i3i1"/>
+                  </Story>
+                </module>
+              </article>
+              <advertise XMLContent="mainudf" Self="maindi2i6"/>
+            </Root>
+        
+        
+        Combine pages
+        '''''''''''''
+        
+        You may need to gather pages from severals documents into a single one:
+        
+        .. code-block:: python
+        
+            >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
+            >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
+        
+            >>> # Always start by prefixing packages to avoid collision.
+            >>> with edito_idml_file.prefix("edito") as p_edito,\
+            >>>      courrier_idml_file.prefix("courrier") as p_courrier:
+            >>>     len(edito_idml_file.pages)
+            2
+        
+            >>>     new_idml = p_edito.add_page_from_idml(p_courrier,
+            ...                                           page_number=1,
+            ...                                           at="/Root",
+            ...                                           only="/Root/page[1]")
+            >>>     len(new_idml.pages)
+            3
+        
+            # The XML Structure has integrated the new file.
+            >>>     print etree.tostring(new_idml.xml_structure, pretty_print=True)
+            <Root Self="editodi2">
+              <page Self="editodi2ib">
+                <article Self="editodi2ibif">
+                  <Story XMLContent="editoue4" Self="editodi2ibifi1f">
+                    <title Self="editodi2ibifi1fi1"/>
+                    <subtitle Self="editodi2ibifi1fi2"/>
+                  </Story>
+                  <content XMLContent="editou11b" Self="editodi2ibifi1e"/>
+                </article>
+              </page>
+              <page Self="editodi2i10">
+                <advertise XMLContent="editou1de" Self="editodi2i10i23"/>
+              </page>
+              <page Self="courrierdi2ib">
+                <title XMLContent="courrieru1b2" Self="courrierdi2ibi34"/>
+                <article XMLContent="courrieru1c9" Self="courrierdi2ibi33"/>
+                <article XMLContent="courrieru1e0" Self="courrierdi2ibi32"/>
+                <article XMLContent="courrieru1fb" Self="courrierdi2ibi31"/>
+                <article XMLContent="courrieru212" Self="courrierdi2ibi30"/>
+              </page>
+            </Root>
+        
+        
+        There is a convenient method to add several pages at once:
+        
+        .. code-block:: python
+        
+            >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
+            >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
+            >>> bloc_notes_idml_file = IDMLPackage("magazineA-bloc-notes.idml")
+        
+            >>> with edito_idml_file.prefix("edito") as p_edito,\
+            >>>      courrier_idml_file.prefix("courrier") as p_courrier,\
+            >>>      bloc_notes_idml_file.prefix("blocnotes") as p_bloc_notes:
+        
+            >>>     packages_to_add = [
+            ...         (p_courrier, 1, "/Root", "/Root/page[1]"),
+            ...         (p_bloc_notes, 1, "/Root", "/Root/page[1]"),
+            ...     ]
+        
+            >>>     new_idml = p_edito.add_pages_from_idml(packages_to_add)
+            >>>     len(new_idml.pages)
+            4
+            >>>     new_idml.spreads
+            ['Spreads/Spread_editoub6.xml',
+             'Spreads/Spread_editoubc.xml',
+             'Spreads/Spread_editoubd.xml']
+        
+        
+        Import/Export XML
+        -----------------
+        
+        Exporting as XML:
+        
+        .. code-block:: python
+        
+            >>> idml_file = IDMLPackage("path/to/file.idml")
+            >>> print idml_file.export_xml()
+            <Root>
+                <module>
+                    <main_picture/>
+                    <headline>Hello world!</headline>
+                    <Story>
+                        <article>Lorem ipsum dolor sit amet, ...</article>
+                        <informations>Lorem ipsum dolor sit amet,</informations>
+                    </Story>
+                </module>
+            </Root>
+        
+        You can as well import XML file into your InDesign® documents. The following rules applies:
+        
+        - A node having the attribute ``simpleidml-setcontent="false"`` will not update the content of the
+          corresponding element into the idml document (but its children will be updated).
+        - A node having the attribute ``simpleidml-ignorecontent"true"`` will not update the content of the
+          corresponding element into the idml document **and** its children.
+        - A node having the attribute ``simpleidml-setcontent="delete"`` will remove the corresponding
+          element into the idml document (Story and Spread elements).
+        - A node having the attribute ``simpleidml-setcontent="remove-previous-br"`` will remove the new-line
+          characters before the element.
+        - You can mix several flags using a comma (i.e.: ``simpleidml-setcontent="delete,remove-previous-br"``)
+        - In a *ignorecontent* context the content of a child node can be turned on with the
+          ``simpleidml-forcecontent="true"`` flag.
+        - Images references are passed by the *href* attribute. An empty value will remove the
+          corresponding page items into the document.
+        - Nested tag will be created if they are mapped with a *character-style*.
+        - The style applied to the newly created tag is a combinaison of the parent character-styles and
+          the mapped one.
+        
+        Please take a look into the tests for in-depth examples.
+        
+        Import PDF
+        ----------
+        
+        A block can be used as a placeholder for a PDF file:
+        
+        .. code-block:: python
+        
+            >>> with IDMLPackage("my_package.idml") as idml_file:
+            >>>     with idml_file.import_pdf("file:/path/to/file.pdf", at="/Root/modules/module[2]", crop="PDFCrop") as f:
+            >>>         f.export_xml()
+        
+        The ``crop`` parameter should be one of the ``PDFCrop_EnumValue`` from the IDML Specification
+        (``"CropArt"``, ``"CropPDF"``, ``"CropTrim"``, ``"CropBleed"``, ``"CropMedia"``,
+        ``"CropContentVisibleLayers"``, ``"CropContentAllLayers"``, ``"CropContent"``).
+        It defaults to ``CropContentVisibleLayers````
+        
+        Use InDesign server SOAP interface to convert a file
+        ----------------------------------------------------
+        
+        This require an *InDesign Server* and a readable/writable working directory.
+        The same directory must be accessible by the client either by the filesystem or
+        over FTP.
+        
+        The ``formats`` parameter is a list (of dicts) of formats and parameters you want
+        your file to be exported into.
+        The supported output formats are ``jpeg``, ``idml``, ``pdf``, ``indd`` and
+        ``zip`` (a zipped InDesign Package).
+        
+        Export parameters are provided using the ``params`` key. Use
+        ``simpleidml_indesign_save_as.py --help`` for a list of supported parameters.
+        
+        The response is a list of binary strings matching ``formats`` provided:
+        
+        .. code-block:: python
+        
+            from simple_idml.indesign import indesign
+        
+            response = indesign.save_as("/path_to_file.idml", [{"fmt": "indd"}],
+                                        "http://url-to-indesign-server:port",
+                                        "/path/to/client/workdir",
+                                        "/path/to/indesign-server/workdir")[0]
+            with open("my_file.indd", "wb+") as f:
+                f.write(response)
+        
+            response = indesign.save_as("/path_to_file.indd", [{"fmt": "idml"}],
+                                        "http://url-to-indesign-server:port",
+                                        "/path/to/client/workdir",
+                                        "/path/to/indesign-server/workdir")[0]
+            with open("my_file.idml", "wb+") as f:
+                f.write(response)
+        
+            response = indesign.save_as("/path_to_file.indd", [{
+                                            "fmt": "pdf",
+                                            "params": {"colorSpace": "CMYK"},
+                                        }],
+                                        "http://url-to-indesign-server:port",
+                                        "/path/to/client/workdir",
+                                        "/path/to/indesign-server/workdir")[0]
+            with open("my_file.pdf", "wb+") as f:
+                f.write(response)
+        
+            pdf_response, jpeg_response, zip_response = indesign.save_as(
+                                            "/path_to_file.indd",
+                                            [{"fmt": "pdf"}, {"fmt": "jpeg"}, {"fmt": "zip"}],
+                                            "http://url-to-indesign-server:port",
+                                            "/path/to/client/workdir",
+                                            "/path/to/indesign-server/workdir")
+        
+        To convert an InDesign Package, use ``indesign.export_package_as()`` instead.
+        
+        If the InDesign Server instance runs on a Windows machine, set the
+        ``indesign_server_path_style`` parameter to ``"windows"``.
+        
+        If the client access to the working directory *via* FTP, you must specify that
+        in the ``ftp_params`` parameter:
+        
+        .. code-block:: python
+        
+            {
+                'auth': ("ftp://ftp.foo.org", "user_account", "s3cret-pa55word"),
+                'passive': False,
+                'keepalive': True,         # False by default (optional)
+                'keepalive_interval': 30,  # set socket.TCP_KEEPINTVL (optional)
+                'keepalive_idle': 45,      # set socket.TCP_KEEPIDLE  (optional)
+                'polite': False,           # Unilaterally close ftp connection (optional)
+            }
+        
+        A script (``simpleidml_indesign_save_as.py``) that wraps these functions is
+        installed in your PATH.
+        
+        Revisions
+        =========
+        
+        1.1.5
+        -----
+        
+        - Add a ``page_number`` parameter to ``IDMLPackage.import_pdf()`` so that you
+          can choose which page from the PDF file to display.
+        
+        1.1.4
+        -----
+        
+        - PyLint refactorisation.
+        
+        1.1.3
+        -----
+        
+        - Catch and log exceptions to the InDesign Server when setting options in
+          export.jsx. Thanks to @kylehodgson for the contribution.
+        
+        1.1.2
+        -----
+        
+        New features
+        ''''''''''''
+        
+        - Add ``indesign.export_package_as()`` to convert an InDesign Package.
+        
+        1.1.1
+        -----
+        
+        New features
+        ''''''''''''
+        
+        - Add the possiblity to remove new-line characters when importing XML by using the flag
+          ``simpleidml-setcontent="remove-previous-br"``.
+        
+        1.1.0
+        -----
+        
+        Removed Python 2 support.
+        
+        New features
+        ''''''''''''
+        
+        - Add the possiblity to remove elements when importing XML by using the flag
+          ``simpleidml-setcontent="delete"``.
+        - The ``PDFCrop`` attribute is now parametrable when using ``import_pdf()``.
+        - ``IDMLPackage.add_note(note, author, at=path)`` added.
+        
+        1.0.5
+        -----
+        
+        Bug fixes
+        '''''''''
+        
+        - Fixed ``indesign.save_as()`` in Python 3 where the jsx file was opened
+          in text mode instead of binary.
+        
+        1.0.3
+        -----
+        
+        - Use setuptools instead of distutils for a better integration with Pypi.
+        
+        1.0.0
+        -----
+        
+        New features
+        ''''''''''''
+        
+        - Added support for Python 3
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - Removed support for Python 2.6
+        
+        0.92.9
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added ``simpleidml_indesign_profiles.py`` script to list the available joboptions
+          files on the InDesign Server using the SOAP interface.
+        
+        Bug fixes
+        '''''''''
+        
+        - Fix working directory cleaning of the SOAP server when an exception is raised.
+          ``indesign.save_as()`` may be backward incompatible since the returned list
+          may contains some ``None`` (instead of raising an exception before returning
+          anything).
+        - Give the list of available profiles (joboptions files) on the InDesign Server
+          if the given 'pdfExportPresetName' is not found.
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - ``indesign.close_all_documents()`` has been replace the ``CloseAllDocuments`` class
+          and its ``.execute()`` method.
+        - Some util functions that wrap the basic file manipulations to manage the case of
+          a ftp access to those files have been moved from indesign.py to a new ftp.py module.
+        
+        0.92.8
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added ``IDMLPackage.import_pdf()`` method.
+        
+        
+        Bug fixes
+        '''''''''
+        
+        - Fix ``bleedMarks`` in export.jsx.
+        
+        0.92.7
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - FillTint wasn't managed.
+        - Force ``lxml < 4`` in dependencies.
+        
+        0.92.6
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - Catch errors when InDesign SOAP server fails to complete a task and raise
+          an exception.
+        
+        0.92.5
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - Handle <PDF> in `IDMLPackage._get_item_translation_for_insert()`
+        
+        0.92.4
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - Fix issue #11: Parent CharacterStyle not applied in import_xml() in some cases.
+        
+        0.92.2
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - More ftp parameters for `indesign.save_as()` function. Hardcoded socket parameters are now
+          modifiable. And you can set the flag `polite` to `False` if you encounter hanging problem
+          on `ftp.quit()` as I do. Being unpolite calls an unilateral and rude `ftp.close()`.
+          Please upgrade your code with explicite values if you rely on the previous default
+          behavior.
+        
+        0.92.1
+        ------
+        
+        Bug fixes
+        '''''''''
+        
+        - ``indesign.save_as()`` uses a dedicated temporary working directory to avoid
+          concurrent access on files.
+        - Added a logger to ``indesign.save_as()`` ('simpleidml.indesign') and some debug messages.
+        - Fixed hanging ``ftp.retrbinary()`` in ``indesign.save_as()`` calls by tuning the socket.
+        
+        0.91.8
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added support for PDF export presets in ``indesign.save_as()``.
+        
+        0.91.7
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Added ``IMDLPackage.merge_layers(with_name)`` (Refs#7).
+        - Added a new script ``simpleidml_indesign_close_all_documents.py``.
+        
+        Bug fixes
+        '''''''''
+        
+        - In ``IDMLPackage.insert_idml()``, Elements from the same layer (but not tagged in the structure)
+          are now added in the Spread of the document of destination.
+        - Better support for Windows platform.
+        - Fixed character style mapping with tag when using insert_idml.
+        - Fixed Export XML in some edge case.
+        - Added parameters to ``simpleidml_indesign_save_as`` when exporting to PDF.
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - ``indesign.save_as()`` formats parameters is now a list of dictionaries.
+        
+        0.91.6
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Add the ``simpleidml-ignorecontent`` and ``simpleidml-forcecontent`` tags (XML attributes)
+          allowing one to carefully exclude a node and its children during the import XML process.
+        - ``indesign.save_as()`` now works with a client working directory over a FTP.
+          This require ``wget`` to be on your system if you want to create zip packages.
+        
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - ``indesign.save_as()`` require both a client workdir and a server workdir parameter.
+        
+        0.91.5.5
+        --------
+        
+        Bugfixes
+        ''''''''
+        
+        - <EPS> elements in Spread weren't handled correctly.
+        - All spread elements were added in the destination package when using ``insert_idml()``.
+        
+        
+        0.91.3
+        ------
+        
+        New features
+        ''''''''''''
+        
+        Add a SOAP client to call a InDesign server to get INDD file and export in various
+        formats.
+        
+        0.91.2
+        ------
+        
+        New features
+        ''''''''''''
+        
+        - Ticket #20 - Suffix layers.
+        
+        Backward incompatibilities
+        ''''''''''''''''''''''''''
+        
+        - Ticket #22 - IDMLPackage.import_xml() parameter is a XML string and not a file object.
+        
+        Bugfixes
+        ''''''''
+        
+        Tickets #19, #21 (orphan layers), #23 (AssertXMLEqual), #24 (import_xml() failure).
+        
+        
+        .. _XPath: http://en.wikipedia.org/wiki/XPath
+        
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Printing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
-License-File: AUTHORS
-
-==========
-SimpleIDML
-==========
-
-.. image:: https://coveralls.io/repos/Starou/SimpleIDML/badge.png
-  :target: https://coveralls.io/r/Starou/SimpleIDML
-
-.. image:: https://img.shields.io/pypi/v/simpleidml.svg
-  :target: https://pypi.python.org/pypi/SimpleIDML
-
-.. image:: https://img.shields.io/pypi/pyversions/simpleidml.svg
-    :target: https://pypi.python.org/pypi/SimpleIDML/
-    :alt: Supported Python versions
-
-.. image:: https://img.shields.io/pypi/l/simpleidml.svg
-    :target: https://pypi.python.org/pypi/SimpleIDML/
-    :alt: License
-
-.. image:: https://travis-ci.org/Starou/SimpleIDML.svg
-    :target: https://travis-ci.org/Starou/SimpleIDML
-    :alt: Travis C.I.
-
-Installation
-============
-
-Use ``pip``:
-
-.. code-block:: bash
-
-    pip install SimpleIDML
-
-Or:
-
-.. code-block:: bash
-
-    python setup.py build
-    sudo python setup.py install
-
-Python support
---------------
-
-- Python 3: 3.6+
-
-Any questions?
---------------
-
-https://groups.google.com/forum/#!forum/simpleidml-users
-
-Developers
-----------
-
-.. code-block:: bash
-
-    vagrant up
-    vagrant ssh
-    cd tests
-    python runtests.py
-
-What is SimpleIDML?
-===================
-
-SimpleIDML is a Python library to manipulate Adobe® InDesign® IDML file. The main purpose being
-the ability to compose IDML files together and produce complex documents from simple pieces and
-to separate the data from the structure.
-
-The philosophy behind SimpleIDML is to keep separated the content and the structure and to use XML
-files to feed your documents by using the XML Structure in InDesign.
-Keeping this isolation is important to ease the debugging and to keep track of what is going on.
-
-I urge you to take a look in the *regressiontests* directory for real-world examples.
-
-Uses cases - success story(ies)
-===============================
-
-Le Figaro - FigaroClassifieds
------------------------------
-
-SimpleIDML is used in production at *Le Figaro* aside in-house tools managing the content of
-Classifieds Ads magazines like *Propriétés de France* or *Belles Maisons à louer*.
-These tools produces XML files describing the page layout (which IDML templates and sub-templates
-to use) and the page content.
-The XML files feed another tool - the one using SimpleIDML - that compose the final page.
-
-The steps of the (simplified) process of composition are:
-
-1. Get the main IDML template (the page) ;
-2. Ad the sub-templates (the ads) into the page template ;
-3. Import the content into the final IDML file ;
-4. Edit the file in InDesign ;
-5. Push the changesets back to the content management application and update the database.
-
-There is a lot of cool features in this application. You can update a part of a page already or
-partially composed for example.
-
-Architecture
-''''''''''''
-
-These applications are web-applications. The communication is done by web-services feeding a task
-queue (RabbitMQ/Celery).
-
-The performances are quite good. Composing a document require a fraction of a second.
-
-What are IDML files?
-====================
-
-IDML (*InDesign Markup Language*) files are a Zip archives (Adobe calls them packages) storing
-essentially XML files. Adobe made a descent job because those files can completely express the
-content of the native (binary) documents.
-This is a small revolution in the print world when it comes to automatically process files in both
-ways from templates and database (Round-trip) without using proprietary server-edition of
-Publishing Software.
-
-What does SimpleIDML do?
-========================
-
-Package exploration
--------------------
-
-You can discover the structure of your IDML files:
-
-.. code-block:: python
-
-    >>> from simple_idml import idml
-    >>> my_idml_package = idml.IDMLPackage("/path/to/my_main_document.idml")
-    >>> my_idml_package.spreads
-    [u'Spreads/Spread_ub6.xml', u'Spreads/Spread_ubc.xml', u'Spreads/Spread_uc3.xml']
-    >>> my_idml_package.stories
-    [u'Stories/Story_u139.xml', u'Stories/Story_u11b.xml',
-     u'Stories/Story_u102.xml', u'Stories/Story_ue4.xml']
-
-Some attributes are *lxml.etree* Elements or Documents:
-
-.. code-block:: python
-
-    >>> my_package.font_families
-    [<Element FontFamily at 0x1010048c0>,
-     <Element FontFamily at 0x101004a50>,
-     <Element FontFamily at 0x101004aa0>,
-        <Element FontFamily at 0x101004af0>]
-    >>> [e.get("Name") for e in my_package.font_families]
-    ['Minion Pro', 'Myriad Pro', 'Kozuka Mincho Pro', 'Vollkorn']
-
-    >>> my_package.xml_structure
-    <Element Root at 0x101004910>
-    >>> from lxml import etree
-    >>> # print my_package.xml_structure_pretty() is a shortcut for:
-    >>> print etree.tostring(my_package.xml_structure, pretty_print=True)
-    <Root Self="di2">
-      <article XMLContent="u102" Self="di2i3">
-        <Story XMLContent="ue4" Self="di2i3i1">
-          <title Self="di2i3i1i1"/>
-          <subtitle Self="di2i3i1i2"/>
-        </Story>
-        <content XMLContent="u11b" Self="di2i3i2"/>
-        <illustration XMLContent="u135" Self="di2i3i3"/>
-        <description XMLContent="u139" Self="di2i3i4"/>
-      </article>
-      <article XMLContent="udb" Self="di2i4"/>
-      <article XMLContent="udd" Self="di2i5"/>
-      <advertise XMLContent="udf" Self="di2i6"/>
-    </Root>
-
-
-``xml_structure`` attribute is a representation of the XML Structure of your InDesign XML-ready
-document (The one you want to use to populate the content with data from an external XML file
-having the same structure).
-
-
-Build package
--------------
-
-There is a convenient script to create a IDML package from a flat directory called
-*simpleidml_create_package_from_dir.py* which should be in your PATH.
-
-
-Compose document
-----------------
-
-**Important**: You should always use a ``with`` context when using side-effect methods on
-``IDMLPackage`` instances returning new instances.
-
-
-For example, the following is bad because ``my_doc`` initial instance reference is lost and
-the associated file cannot be properly closed. This may rise an exception on Windows platform
-if you try to ``os.unlink()`` an unclosed file.
-
-.. code-block:: python
-
-    from simple_idml import idml
-    my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
-    my_doc = my_doc.prefix("main")
-
-Instead, use:
-
-.. code-block:: python
-
-    from simple_idml import idml
-    my_doc = idml.IDMLPackage("/path/to/my_main_document.idml")
-    with my_doc.prefix("main") as f:
-        # some code.
-
-Insert elements
-'''''''''''''''
-
-Using the XML Structure you can ask SimpleIDML to insert into a document at a XML tag the content
-of another XML tag from another document. The tag paths are expressed using XPath_ syntax.
-Note that you should always make a copy of your idml files before altering them with
-``shutil.copy2(src, dst)`` for instance and prefix your document before using ``insert_idml()``
-to avoid reference collisions.
-
-.. code-block:: python
-
-    >>> from simple_idml import idml
-    >>> idml_main = idml.IDMLPackage("/path/to/my_main_document.idml")
-    >>> idml_module = idml.IDMLPackage("/path/to/my_small_document.idml")
-
-    >>> with idml_main.prefix("main") as p_idml_main, \
-    >>>      idml_module.prefix("article") as p_idml_article:
-
-    >>>     with p_idml_main.insert_idml(p_idml_article, at="/Root/article[3]",
-                                         only="/Root/module[1]") as f:
-    >>>         f.stories
-    ['Stories/Story_article1u188.xml', 'Stories/Story_article1u19f.xml',
-     'Stories/Story_article1u1db.xml', 'Stories/Story_mainu102.xml',
-     'Stories/Story_mainu11b.xml', 'Stories/Story_mainu139.xml',
-     'Stories/Story_mainue4.xml']
-
-
-    >>>         print f.xml_structure_pretty()
-    <Root Self="maindi2">
-      <article XMLContent="mainu102" Self="maindi2i3">
-        <Story XMLContent="mainue4" Self="maindi2i3i1">
-          <title Self="maindi2i3i1i1"/>
-          <subtitle Self="maindi2i3i1i2"/>
-        </Story>
-        <content XMLContent="mainu11b" Self="maindi2i3i2"/>
-        <illustration XMLContent="mainu135" Self="maindi2i3i3"/>
-        <description XMLContent="mainu139" Self="maindi2i3i4"/>
-      </article>
-      <article XMLContent="mainudb" Self="maindi2i4"/>
-      <article Self="maindi2i5">
-        <module XMLContent="article1u1db" Self="article1di3i12">
-          <main_picture XMLContent="article1u182" Self="article1di3i12i1"/>
-          <headline XMLContent="article1u188" Self="article1di3i12i2"/>
-          <Story XMLContent="article1u19f" Self="article1di3i12i3">
-            <article Self="article1di3i12i3i2"/>
-            <informations Self="article1di3i12i3i1"/>
-          </Story>
-        </module>
-      </article>
-      <advertise XMLContent="mainudf" Self="maindi2i6"/>
-    </Root>
-
-
-Combine pages
-'''''''''''''
-
-You may need to gather pages from severals documents into a single one:
-
-.. code-block:: python
-
-    >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
-    >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
-
-    >>> # Always start by prefixing packages to avoid collision.
-    >>> with edito_idml_file.prefix("edito") as p_edito,\
-    >>>      courrier_idml_file.prefix("courrier") as p_courrier:
-    >>>     len(edito_idml_file.pages)
-    2
-
-    >>>     new_idml = p_edito.add_page_from_idml(p_courrier,
-    ...                                           page_number=1,
-    ...                                           at="/Root",
-    ...                                           only="/Root/page[1]")
-    >>>     len(new_idml.pages)
-    3
-
-    # The XML Structure has integrated the new file.
-    >>>     print etree.tostring(new_idml.xml_structure, pretty_print=True)
-    <Root Self="editodi2">
-      <page Self="editodi2ib">
-        <article Self="editodi2ibif">
-          <Story XMLContent="editoue4" Self="editodi2ibifi1f">
-            <title Self="editodi2ibifi1fi1"/>
-            <subtitle Self="editodi2ibifi1fi2"/>
-          </Story>
-          <content XMLContent="editou11b" Self="editodi2ibifi1e"/>
-        </article>
-      </page>
-      <page Self="editodi2i10">
-        <advertise XMLContent="editou1de" Self="editodi2i10i23"/>
-      </page>
-      <page Self="courrierdi2ib">
-        <title XMLContent="courrieru1b2" Self="courrierdi2ibi34"/>
-        <article XMLContent="courrieru1c9" Self="courrierdi2ibi33"/>
-        <article XMLContent="courrieru1e0" Self="courrierdi2ibi32"/>
-        <article XMLContent="courrieru1fb" Self="courrierdi2ibi31"/>
-        <article XMLContent="courrieru212" Self="courrierdi2ibi30"/>
-      </page>
-    </Root>
-
-
-There is a convenient method to add several pages at once:
-
-.. code-block:: python
-
-    >>> edito_idml_file = IDMLPackage("magazineA-edito.idml")
-    >>> courrier_idml_file = IDMLPackage("magazineA-courrier-des-lecteurs.idml")
-    >>> bloc_notes_idml_file = IDMLPackage("magazineA-bloc-notes.idml")
-
-    >>> with edito_idml_file.prefix("edito") as p_edito,\
-    >>>      courrier_idml_file.prefix("courrier") as p_courrier,\
-    >>>      bloc_notes_idml_file.prefix("blocnotes") as p_bloc_notes:
-
-    >>>     packages_to_add = [
-    ...         (p_courrier, 1, "/Root", "/Root/page[1]"),
-    ...         (p_bloc_notes, 1, "/Root", "/Root/page[1]"),
-    ...     ]
-
-    >>>     new_idml = p_edito.add_pages_from_idml(packages_to_add)
-    >>>     len(new_idml.pages)
-    4
-    >>>     new_idml.spreads
-    ['Spreads/Spread_editoub6.xml',
-     'Spreads/Spread_editoubc.xml',
-     'Spreads/Spread_editoubd.xml']
-
-
-Import/Export XML
------------------
-
-Exporting as XML:
-
-.. code-block:: python
-
-    >>> idml_file = IDMLPackage("path/to/file.idml")
-    >>> print idml_file.export_xml()
-    <Root>
-        <module>
-            <main_picture/>
-            <headline>Hello world!</headline>
-            <Story>
-                <article>Lorem ipsum dolor sit amet, ...</article>
-                <informations>Lorem ipsum dolor sit amet,</informations>
-            </Story>
-        </module>
-    </Root>
-
-You can as well import XML file into your InDesign® documents. The following rules applies:
-
-- A node having the attribute ``simpleidml-setcontent="false"`` will not update the content of the
-  corresponding element into the idml document (but its children will be updated).
-- A node having the attribute ``simpleidml-ignorecontent"true"`` will not update the content of the
-  corresponding element into the idml document **and** its children.
-- A node having the attribute ``simpleidml-setcontent="delete"`` will remove the corresponding
-  element into the idml document (Story and Spread elements).
-- A node having the attribute ``simpleidml-setcontent="remove-previous-br"`` will remove the new-line
-  characters before the element.
-- You can mix several flags using a comma (i.e.: ``simpleidml-setcontent="delete,remove-previous-br"``)
-- In a *ignorecontent* context the content of a child node can be turned on with the
-  ``simpleidml-forcecontent="true"`` flag.
-- Images references are passed by the *href* attribute. An empty value will remove the
-  corresponding page items into the document.
-- Nested tag will be created if they are mapped with a *character-style*.
-- The style applied to the newly created tag is a combinaison of the parent character-styles and
-  the mapped one.
-
-Please take a look into the tests for in-depth examples.
-
-Import PDF
-----------
-
-A block can be used as a placeholder for a PDF file:
-
-.. code-block:: python
-
-    >>> with IDMLPackage("my_package.idml") as idml_file:
-    >>>     with idml_file.import_pdf("file:/path/to/file.pdf", at="/Root/modules/module[2]", crop="PDFCrop") as f:
-    >>>         f.export_xml()
-
-The ``crop`` parameter should be one of the ``PDFCrop_EnumValue`` from the IDML Specification
-(``"CropArt"``, ``"CropPDF"``, ``"CropTrim"``, ``"CropBleed"``, ``"CropMedia"``,
-``"CropContentVisibleLayers"``, ``"CropContentAllLayers"``, ``"CropContent"``).
-It defaults to ``CropContentVisibleLayers````
-
-Use InDesign server SOAP interface to convert a file
-----------------------------------------------------
-
-This require an *InDesign Server* and a readable/writable working directory.
-The same directory must be accessible by the client either by the filesystem or
-over FTP.
-
-The ``formats`` parameter is a list (of dicts) of formats and parameters you want
-your file to be exported into.
-The supported output formats are ``jpeg``, ``idml``, ``pdf``, ``indd`` and
-``zip`` (a zipped InDesign Package).
-
-Export parameters are provided using the ``params`` key. Use
-``simpleidml_indesign_save_as.py --help`` for a list of supported parameters.
-
-The response is a list of binary strings matching ``formats`` provided:
-
-.. code-block:: python
-
-    from simple_idml.indesign import indesign
-
-    response = indesign.save_as("/path_to_file.idml", [{"fmt": "indd"}],
-                                "http://url-to-indesign-server:port",
-                                "/path/to/client/workdir",
-                                "/path/to/indesign-server/workdir")[0]
-    with open("my_file.indd", "wb+") as f:
-        f.write(response)
-
-    response = indesign.save_as("/path_to_file.indd", [{"fmt": "idml"}],
-                                "http://url-to-indesign-server:port",
-                                "/path/to/client/workdir",
-                                "/path/to/indesign-server/workdir")[0]
-    with open("my_file.idml", "wb+") as f:
-        f.write(response)
-
-    response = indesign.save_as("/path_to_file.indd", [{
-                                    "fmt": "pdf",
-                                    "params": {"colorSpace": "CMYK"},
-                                }],
-                                "http://url-to-indesign-server:port",
-                                "/path/to/client/workdir",
-                                "/path/to/indesign-server/workdir")[0]
-    with open("my_file.pdf", "wb+") as f:
-        f.write(response)
-
-    pdf_response, jpeg_response, zip_response = indesign.save_as(
-                                    "/path_to_file.indd",
-                                    [{"fmt": "pdf"}, {"fmt": "jpeg"}, {"fmt": "zip"}],
-                                    "http://url-to-indesign-server:port",
-                                    "/path/to/client/workdir",
-                                    "/path/to/indesign-server/workdir")
-
-To convert an InDesign Package, use ``indesign.export_package_as()`` instead.
-
-If the InDesign Server instance runs on a Windows machine, set the
-``indesign_server_path_style`` parameter to ``"windows"``.
-
-If the client access to the working directory *via* FTP, you must specify that
-in the ``ftp_params`` parameter:
-
-.. code-block:: python
-
-    {
-        'auth': ("ftp://ftp.foo.org", "user_account", "s3cret-pa55word"),
-        'passive': False,
-        'keepalive': True,         # False by default (optional)
-        'keepalive_interval': 30,  # set socket.TCP_KEEPINTVL (optional)
-        'keepalive_idle': 45,      # set socket.TCP_KEEPIDLE  (optional)
-        'polite': False,           # Unilaterally close ftp connection (optional)
-    }
-
-A script (``simpleidml_indesign_save_as.py``) that wraps these functions is
-installed in your PATH.
-
-Revisions
-=========
-
-1.1.3
------
-
-- Catch and log exceptions to the InDesign Server when setting options in
-  export.jsx. Thanks to @kylehodgson for the contribution.
-
-1.1.2
------
-
-New features
-''''''''''''
-
-- Add ``indesign.export_package_as()`` to convert an InDesign Package.
-
-1.1.1
------
-
-New features
-''''''''''''
-
-- Add the possiblity to remove new-line characters when importing XML by using the flag
-  ``simpleidml-setcontent="remove-previous-br"``.
-
-1.1.0
------
-
-Removed Python 2 support.
-
-New features
-''''''''''''
-
-- Add the possiblity to remove elements when importing XML by using the flag
-  ``simpleidml-setcontent="delete"``.
-- The ``PDFCrop`` attribute is now parametrable when using ``import_pdf()``.
-- ``IDMLPackage.add_note(note, author, at=path)`` added.
-
-1.0.5
------
-
-Bug fixes
-'''''''''
-
-- Fixed ``indesign.save_as()`` in Python 3 where the jsx file was opened
-  in text mode instead of binary.
-
-1.0.3
------
-
-- Use setuptools instead of distutils for a better integration with Pypi.
-
-1.0.0
------
-
-New features
-''''''''''''
-
-- Added support for Python 3
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- Removed support for Python 2.6
-
-0.92.9
-------
-
-New features
-''''''''''''
-
-- Added ``simpleidml_indesign_profiles.py`` script to list the available joboptions
-  files on the InDesign Server using the SOAP interface.
-
-Bug fixes
-'''''''''
-
-- Fix working directory cleaning of the SOAP server when an exception is raised.
-  ``indesign.save_as()`` may be backward incompatible since the returned list
-  may contains some ``None`` (instead of raising an exception before returning
-  anything).
-- Give the list of available profiles (joboptions files) on the InDesign Server
-  if the given 'pdfExportPresetName' is not found.
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- ``indesign.close_all_documents()`` has been replace the ``CloseAllDocuments`` class
-  and its ``.execute()`` method.
-- Some util functions that wrap the basic file manipulations to manage the case of
-  a ftp access to those files have been moved from indesign.py to a new ftp.py module.
-
-0.92.8
-------
-
-New features
-''''''''''''
-
-- Added ``IDMLPackage.import_pdf()`` method.
-
-
-Bug fixes
-'''''''''
-
-- Fix ``bleedMarks`` in export.jsx.
-
-0.92.7
-------
-
-Bug fixes
-'''''''''
-
-- FillTint wasn't managed.
-- Force ``lxml < 4`` in dependencies.
-
-0.92.6
-------
-
-Bug fixes
-'''''''''
-
-- Catch errors when InDesign SOAP server fails to complete a task and raise
-  an exception.
-
-0.92.5
-------
-
-Bug fixes
-'''''''''
-
-- Handle <PDF> in `IDMLPackage._get_item_translation_for_insert()`
-
-0.92.4
-------
-
-Bug fixes
-'''''''''
-
-- Fix issue #11: Parent CharacterStyle not applied in import_xml() in some cases.
-
-0.92.2
-------
-
-New features
-''''''''''''
-
-- More ftp parameters for `indesign.save_as()` function. Hardcoded socket parameters are now
-  modifiable. And you can set the flag `polite` to `False` if you encounter hanging problem
-  on `ftp.quit()` as I do. Being unpolite calls an unilateral and rude `ftp.close()`.
-  Please upgrade your code with explicite values if you rely on the previous default
-  behavior.
-
-0.92.1
-------
-
-Bug fixes
-'''''''''
-
-- ``indesign.save_as()`` uses a dedicated temporary working directory to avoid
-  concurrent access on files.
-- Added a logger to ``indesign.save_as()`` ('simpleidml.indesign') and some debug messages.
-- Fixed hanging ``ftp.retrbinary()`` in ``indesign.save_as()`` calls by tuning the socket.
-
-0.91.8
-------
-
-New features
-''''''''''''
-
-- Added support for PDF export presets in ``indesign.save_as()``.
-
-0.91.7
-------
-
-New features
-''''''''''''
-
-- Added ``IMDLPackage.merge_layers(with_name)`` (Refs#7).
-- Added a new script ``simpleidml_indesign_close_all_documents.py``.
-
-Bug fixes
-'''''''''
-
-- In ``IDMLPackage.insert_idml()``, Elements from the same layer (but not tagged in the structure)
-  are now added in the Spread of the document of destination.
-- Better support for Windows platform.
-- Fixed character style mapping with tag when using insert_idml.
-- Fixed Export XML in some edge case.
-- Added parameters to ``simpleidml_indesign_save_as`` when exporting to PDF.
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- ``indesign.save_as()`` formats parameters is now a list of dictionaries.
-
-0.91.6
-------
-
-New features
-''''''''''''
-
-- Add the ``simpleidml-ignorecontent`` and ``simpleidml-forcecontent`` tags (XML attributes)
-  allowing one to carefully exclude a node and its children during the import XML process.
-- ``indesign.save_as()`` now works with a client working directory over a FTP.
-  This require ``wget`` to be on your system if you want to create zip packages.
-
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- ``indesign.save_as()`` require both a client workdir and a server workdir parameter.
-
-0.91.5.5
---------
-
-Bugfixes
-''''''''
-
-- <EPS> elements in Spread weren't handled correctly.
-- All spread elements were added in the destination package when using ``insert_idml()``.
-
-
-0.91.3
-------
-
-New features
-''''''''''''
-
-Add a SOAP client to call a InDesign server to get INDD file and export in various
-formats.
-
-0.91.2
-------
-
-New features
-''''''''''''
-
-- Ticket #20 - Suffix layers.
-
-Backward incompatibilities
-''''''''''''''''''''''''''
-
-- Ticket #22 - IDMLPackage.import_xml() parameter is a XML string and not a file object.
-
-Bugfixes
-''''''''
-
-Tickets #19, #21 (orphan layers), #23 (AssertXMLEqual), #24 (import_xml() failure).
-
-
-.. _XPath: http://en.wikipedia.org/wiki/XPath
-
-
```

### Comparing `SimpleIDML-1.1.3/src/scripts/simpleidml_create_package_from_dir.py` & `SimpleIDML-1.1.6a1/src/scripts/simpleidml_create_package_from_dir.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/src/scripts/simpleidml_indesign_close_all_documents.py` & `SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_close_all_documents.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/src/scripts/simpleidml_indesign_save_as.py` & `SimpleIDML-1.1.6a1/src/scripts/simpleidml_indesign_save_as.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from builtins import map
 import os
 from simple_idml.indesign import indesign
 from simple_idml.commands import InDesignSoapCommand
 
 
 class InDesignSaveAsCommand(InDesignSoapCommand):
     description = """SOAP call to an InDesign Server to save a file in other formats.
@@ -47,20 +46,20 @@
        - monochromeBitmapSamplingDPI: [9 to 2400]
 
     Example:
         "path/to/out.pdf|colorBars=1,cropMarks=1,monochromeBitmapCompression=CCIT3"
        """
 
     def __init__(self):
-        super(InDesignSaveAsCommand, self).__init__()
+        super().__init__()
         self.parser.add_argument('source', metavar='SOURCE', help="path/to/file.{indd|zip}")
         self.parser.add_argument('destinations', metavar='DESTINATIONS', help="file1|opt1=a,opt2=b;file2|opt1=c")
 
     def execute(self):
-        super(InDesignSaveAsCommand, self).execute()
+        super().execute()
         destinations = self.args.destinations.split(";")
         formats = map(self.parse_destination_arg, destinations)
         if os.path.splitext(self.args.source)[1] == ".zip":
             func = indesign.export_package_as
         else:
             func = indesign.save_as
         responses = func(self.args.source, formats, self.args.url, self.args.client_workdir,
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/commands.py` & `SimpleIDML-1.1.6a1/src/simple_idml/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 # -*- coding: utf-8 -*-
 
-from builtins import object
 import argparse
 import logging
 
 
-class InDesignSoapCommand(object):
+class InDesignSoapCommand():
+    description = ""
+
     def __init__(self):
         self.parser = argparse.ArgumentParser(description=self.description,
-                                             formatter_class=argparse.RawDescriptionHelpFormatter)
-        self.parser.add_argument("-u", "--url", default="http://127.0.0.1:8082", help=u"InDesign Server SOAP url")
+                                              formatter_class=argparse.RawDescriptionHelpFormatter)
+        self.parser.add_argument("-u", "--url", default="http://127.0.0.1:8082", help="InDesign Server SOAP url")
         self.parser.add_argument("--client-workdir", default="/tmp",
                                  help=("Directory where temporary files are written, as seen by the SOAP client."
-                                     " This could be a FTP path."))
+                                       " This could be a FTP path."))
         self.parser.add_argument("--server-workdir", default="/tmp",
                                  help="Directory where temporary files are written, as seen by the InDesign server.")
         self.parser.add_argument("--server-path-style", default="posix",
                                  choices=['posix', 'windows'], help="The OS type running InDesign Server")
         self.parser.add_argument("--no-clean-workdir", action="store_true", default=False,
                                  help="Do not clean the working directory when finished")
         self.parser.add_argument("--ftp-url",
                                  help="The FTP server for the workdir. It must be on the filesystem of the InDesign Server.")
         self.parser.add_argument("--ftp-user", default="")
         self.parser.add_argument("--ftp-password", default="")
         self.parser.add_argument("--ftp-passive", action="store_true", default=False)
         self.parser.add_argument("-v", "--verbose", action="store_true", default=False)
 
+        self.ftp_params = None
+        self.args = None
+
     def execute(self):
         self.parse_options()
         self.set_ftp_params()
         self.set_suds_logging()
 
     def parse_options(self):
         self.args = self.parser.parse_args()
 
     def set_ftp_params(self):
-        self.ftp_params = None
         if self.args.ftp_url:
             self.ftp_params = {
                 'auth': (self.args.ftp_url, self.args.ftp_user, self.args.ftp_password),
                 'passive': self.args.ftp_passive,
             }
 
     def set_suds_logging(self):
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/components.py` & `SimpleIDML-1.1.6a1/src/simple_idml/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import copy
 import datetime
 import os
 import re
 from decimal import Decimal
 from lxml import etree
 from simple_idml import IdPkgNS, BACKINGSTORY
-from simple_idml.utils import increment_xmltag_id, prefix_content_filename
+from simple_idml.utils import increment_xmltag_id, prefix_content_filename, deepcopy_element_as
 from simple_idml.utils import Proxy
 
 RECTO = "recto"
 VERSO = "verso"
 
 rx_node_name_from_xml_name = re.compile(r"[\w]+/[\w]+_([\w]+)\.xml")
 
 
-class IDMLXMLFile(object):
+class IDMLXMLFile():
     """Abstract class for various XML files found in IDML Packages. """
     name = None
     doctype = None
     excluded_tags_for_prefix = (
         "Document",
         "Language",
         "NumberingList",
@@ -44,25 +44,26 @@
         "AppliedCharacterStyle",
         "AppliedParagraphStyle",
         "AppliedObjectStyle",
         "NextStyle",
         "FillColor",
         "StrokeColor",
         "ItemLayer",
+        "NextTextFrame",
+        "PreviousTextFrame",
     )
 
     def __init__(self, idml_package, working_copy_path=None):
         self.idml_package = idml_package
         self.working_copy_path = working_copy_path
         self._fobj = None
         self._dom = None
 
     def __repr__(self):
-        return "<%s object %s at %s>" % (self.__class__.__name__,
-                                         self.name, hex(id(self)))
+        return f"<{self.__class__.__name__} object {self.name} at {hex(id(self))}>"
 
     @property
     def fobj(self):
         if self._fobj is None:
             if self.working_copy_path:
                 filename = os.path.join(self.working_copy_path, self.name)
                 fobj = open(filename, mode="rb+")
@@ -90,40 +91,39 @@
     def tostring(self):
         kwargs = {"xml_declaration": True,
                   "encoding": "UTF-8",
                   "standalone": True,
                   "pretty_print": True}
 
         if etree.LXML_VERSION < (2, 3):
-            s = etree.tostring(self.dom, **kwargs)
+            strn = etree.tostring(self.dom, **kwargs)
             if self.doctype:
-                lines = s.splitlines()
+                lines = strn.splitlines()
                 lines.insert(1, self.doctype)
-                s = "\n".join(line.decode("utf-8") for line in lines)
-                s += "\n"
-                s = s.encode("utf-8")
+                strn = "\n".join(line.decode("utf-8") for line in lines)
+                strn += "\n"
+                strn = strn.encode("utf-8")
         else:
             kwargs["doctype"] = self.doctype
-            s = etree.tostring(self.dom, **kwargs)
-        return s
+            strn = etree.tostring(self.dom, **kwargs)
+        return strn
 
     def synchronize(self):
         # Explicit initialization of dom from self._fobj before reset
         # because in tostring() we get the dom from this file if None.
-        self.dom
+        self.dom  # pylint: disable=pointless-statement
         self.fobj.close()
         self._fobj = None
 
         # Must instanciate with a working_copy to use this.
-        fobj = open(os.path.join(self.working_copy_path, self.name), mode="wb+")
-        fobj.write(self.tostring())
-        fobj.close()
+        with open(os.path.join(self.working_copy_path, self.name), mode="wb+") as fobj:
+            fobj.write(self.tostring())
 
     def get_element_by_id(self, value, tag="XMLElement", attr="Self"):
-        elem = self.dom.xpath("//%s[@%s='%s']" % (tag, attr, value))
+        elem = self.dom.xpath(f"//{tag}[@{attr}='{value}']")
         # etree FutureWarning when trying to simply do: elem = len(elem) and elem[0] or None
         if len(elem):
             elem = elem[0]
             if elem.tag == "XMLElement":
                 elem = XMLElement(elem)
         else:
             elem = None
@@ -139,29 +139,30 @@
         # <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]"
         #  PointSize="10" />
         for elt in self.dom.iter():
             if elt.tag in self.excluded_tags_for_prefix:
                 continue
             for attr in self.prefixable_attrs:
                 if elt.get(attr):
-                    elt.set(attr, "%s%s" % (prefix, elt.get(attr)))
+                    if attr in ['NextTextFrame', 'PreviousTextFrame'] and elt.get(attr) == 'n':
+                        continue
+                    elt.set(attr, f"{prefix}{elt.get(attr)}")
 
         # <idPkg:Spread src="Spreads/Spread_ub6.xml"/>
         # <idPkg:Story src="Stories/Story_u139.xml"/>
         for elt in self.dom.xpath(".//idPkg:Spread | .//idPkg:Story",
                                   namespaces={'idPkg': IdPkgNS}):
             if elt.get("src"):
                 elt.set("src", prefix_content_filename(elt.get("src"), prefix, "ref"))
 
         # <Document xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging"...
         # StoryList="ue4 u102 u11b u139 u9c"...>
         elt = self.dom.xpath("/Document")
         if elt and elt[0].get("StoryList"):
-            elt[0].set("StoryList", " ".join(["%s%s" % (prefix, s)
-                                              for s in elt[0].get("StoryList").split(" ")]))
+            elt[0].set("StoryList", " ".join([f"{prefix}{s}" for s in elt[0].get("StoryList").split(" ")]))
 
     def set_element_resource_path(self, element_id, resource_path, synchronize=False):
         """ For Spread and Story subclasses only (this comment is a call for a Mixin). """
         # the element may not be an <XMLElement> (so tag="*").
         elt = self.get_element_by_id(element_id, tag="*")
         if elt is None:
             return
@@ -174,23 +175,23 @@
     def remove_xml_element_page_items(self, element_id, synchronize=False):
         """Page items are sometimes in Stories rather in Spread. """
         elt = self.get_element_by_id(element_id)
         if elt.get("NoTextMarker"):
             elt.attrib.pop("NoTextMarker")
         if elt.get("XMLContent"):
             elt.attrib.pop("XMLContent")
-        for c in elt.iterchildren():
-            elt.remove(c)
+        for child in elt.iterchildren():
+            elt.remove(child)
         if synchronize:
             self.synchronize()
 
 
 class MasterSpread(IDMLXMLFile):
     def __init__(self, idml_package, name, working_copy_path=None):
-        super(MasterSpread, self).__init__(idml_package, working_copy_path)
+        super().__init__(idml_package, working_copy_path)
         self.name = name
 
 
 class Spread(IDMLXMLFile):
     """
 
         Spread coordinates system
@@ -213,15 +214,15 @@
       |                 |                  |
       |_________________|__________________|
                         |
                         ˇ +Y
     """
 
     def __init__(self, idml_package, name, working_copy_path=None):
-        super(Spread, self).__init__(idml_package, working_copy_path)
+        super().__init__(idml_package, working_copy_path)
         self.name = name
         self._pages = None
         self._node = None
 
     @property
     def pages(self):
         if self._pages is None:
@@ -263,52 +264,51 @@
         last_page.page_items = [item for item in last_page.page_items
                                 if item.get("Self") in items_references]
         last_page.set_face(face_required)
 
     def clear(self):
         items = list(self.node.items())
         self.node.clear()
-        for k, v in items:
-            self.node.set(k, v)
+        for k, value in items:
+            self.node.set(k, value)
 
         self._pages = None
 
     def get_node_name_from_xml_name(self):
         return rx_node_name_from_xml_name.match(self.name).groups()[0]
 
     def set_layer_references(self, layer_id):
         for elt in self.dom.iter():
             if elt.get("ItemLayer"):
                 elt.set("ItemLayer", layer_id)
         self.synchronize()
 
     def has_any_item_on_layer(self, layer_id):
         # The page Guide are not page items.
-        return bool(len(self.node.xpath(".//*[not(self::Guide)][@ItemLayer='%s']" % layer_id)))
+        return bool(len(self.node.xpath(f".//*[not(self::Guide)][@ItemLayer='{layer_id}']")))
 
     def has_any_guide_on_layer(self, layer_id):
-        return bool(len(self.node.xpath(".//Guide[@ItemLayer='%s']" % layer_id)))
+        return bool(len(self.node.xpath(f".//Guide[@ItemLayer='{layer_id}']")))
 
     def remove_guides_on_layer(self, layer_id, synchronize=False):
-        for guide in self.node.xpath(".//Guide[@ItemLayer='%s']" % layer_id):
+        for guide in self.node.xpath(f".//Guide[@ItemLayer='{layer_id}']"):
             guide.getparent().remove(guide)
         if synchronize:
             self.synchronize()
 
     def remove_page_item(self, item_id, synchronize=False):
         # etree FutureWarning when trying to simply do: elt = foo() or bar().
         elt = self.get_element_by_id(item_id, tag="*")
         if elt is None:
             elt = self.get_element_by_id(item_id, tag="*", attr="ParentStory")
         elt.getparent().remove(elt)
         if synchronize:
             self.synchronize()
 
     def rectangle_to_textframe(self, rectangle):
-        from simple_idml.utils import deepcopy_element_as
         textframe = deepcopy_element_as(rectangle, "TextFrame")
         textframe.set("ContentType", "TextType")
         textframe.set("PreviousTextFrame", "n")
         textframe.set("NextTextFrame", "n")
         # These attributes and subelements must be removed.
         del textframe.attrib["StoryTitle"]  # Suppose it is always present.
         for sub_elt_name in ("InCopyExportOption", "FrameFittingOption", "ObjectExportOption"):
@@ -322,25 +322,25 @@
 
 
 STORIES_DIRNAME = "Stories"
 
 
 class Story(IDMLXMLFile):
     def __init__(self, idml_package, name, working_copy_path=None):
-        super(Story, self).__init__(idml_package, working_copy_path)
+        super().__init__(idml_package, working_copy_path)
         self.name = name
         self.node_name = "Story"
         self._node = None
 
     @classmethod
     def create(cls, idml_package, story_id, xml_element_id, xml_element_tag, working_copy_path):
         dirname = os.path.join(working_copy_path, STORIES_DIRNAME)
         if not os.path.exists(dirname):
             os.mkdir(dirname)
-        story_name = "%s/Story_%s.xml" % (STORIES_DIRNAME, story_id)
+        story_name = f"{STORIES_DIRNAME}/Story_{story_id}.xml"
         story = Story(idml_package, story_name, working_copy_path)
 
         # Difficult to do it in .fobj() because we don't always need
         # to create a unexisting file.
         filename = os.path.join(working_copy_path, story_name)
         story._fobj = open(filename, mode="w+")
         story.fobj.write(
@@ -394,16 +394,16 @@
         xml_element.addnext(local_style)
 
     def clear_element_content(self, element_id):
         element = self.get_element_by_id(element_id)
         # We remove all `CharacterStyleRange' containers except the first.
         # FIXME: This should handle ./ParagraphStyleRange/CharacterStyleRange too.
         children = element.xpath("./CharacterStyleRange")[1:]
-        for c in children:
-            element.remove(c)
+        for child in children:
+            element.remove(child)
         for content_node in self.get_element_content_nodes(element):
             content_node.text = ""
 
     def get_element_content_nodes(self, element):
         return element.xpath(("./ParagraphStyleRange/CharacterStyleRange/Content | "
                               "./CharacterStyleRange/Content | "
                               "./XMLElement/CharacterStyleRange/Content | "
@@ -415,20 +415,20 @@
                               "./ParagraphStyleRange/CharacterStyleRange/XMLElement | "
                               "./CharacterStyleRange/XMLElement | "
                               "./ParagraphStyleRange/XMLElement | "
                               "./XMLElement | "
                               "./Content"))
 
     def set_element_id(self, element):
-        ref_element = [e for e in element.itersiblings(tag="XMLElement", preceding=True)]
+        ref_element = list(element.itersiblings(tag="XMLElement", preceding=True))
         if ref_element:
             ref_element = ref_element[0]
             position = "sibling"
         else:
-            ref_element = [e for e in element.iterancestors(tag="XMLElement")]
+            ref_element = list(element.iterancestors(tag="XMLElement"))
             if ref_element:
                 ref_element = ref_element[0]
             else:
                 raise NotImplementedError
             position = "child"
         element.set("Self", increment_xmltag_id(ref_element.get("Self"), position))
 
@@ -467,28 +467,28 @@
                                             </ParagraphStyleRange>
                                         </Note>""")
         element.insert(0, note_node)
 
 
 class BackingStory(Story):
     def __init__(self, idml_package, name=BACKINGSTORY, working_copy_path=None):
-        super(BackingStory, self).__init__(idml_package, name, working_copy_path)
+        super().__init__(idml_package, name, working_copy_path)
         self.node_name = "XmlStory"
 
     def get_root(self):
         return XMLElement(self.dom.find("*//XMLElement"))
 
 
 class Designmap(IDMLXMLFile):
     name = "designmap.xml"
     doctype = '<?aid style="50" type="document" readerVersion="6.0" featureSet="257" product="7.5(142)" ?>'
     page_start_attr = "PageStart"
 
     def __init__(self, idml_package, working_copy_path):
-        super(Designmap, self).__init__(idml_package, working_copy_path)
+        super().__init__(idml_package, working_copy_path)
         self._spread_nodes = None
         self._style_mapping_node = None
         self._section_node = None
         self._layer_nodes = None
         self._active_layer = None
 
     @property
@@ -551,34 +551,34 @@
             )
 
     def prefix(self, prefix):
         self.prefix_active_layer(prefix)
         self.prefix_page_start(prefix)
 
     def prefix_active_layer(self, prefix):
-        self.active_layer = "%s%s" % (prefix, self.active_layer)
+        self.active_layer = f"{prefix}{self.active_layer}"
 
     def prefix_page_start(self, prefix):
         section_node = self.section_node
         current_page_start = section_node.get(self.page_start_attr)
-        section_node.set(self.page_start_attr, "%s%s" % (prefix, current_page_start))
+        section_node.set(self.page_start_attr, f"{prefix}{current_page_start}")
 
     def add_stories(self, stories):
         # Add stories in StoryList.
         elt = self.dom.xpath("/Document")[0]
         current_stories = elt.get("StoryList").split(" ")
         elt.set("StoryList", " ".join(current_stories + stories))
 
         # Add <idPkg:Story src="Stories/Story_[name].xml"/> elements.
         for story in stories:
             elt.append(etree.Element("{http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging}Story",
-                                     src="Stories/Story_%s.xml" % story))
+                                     src=f"Stories/Story_{story}.xml"))
 
     def add_layer_nodes(self, layer_nodes):
-        current_layers_ids = [l.get("Self") for l in self.layer_nodes]
+        current_layers_ids = [layer.get("Self") for layer in self.layer_nodes]
         for layer in reversed(layer_nodes):
             # If a similar layer is already present, we do not add it.
             if layer.get("Self") not in current_layers_ids:
                 self.layer_nodes[-1].addnext(copy.deepcopy(layer))
         self._layer_nodes = None
 
     def remove_layer(self, layer_id, synchronize=False):
@@ -591,43 +591,40 @@
             if len(self.layer_nodes):
                 self.active_layer = self.layer_nodes[0].get("Self")
         if synchronize:
             self.synchronize()
 
     def suffix_layers(self, suffix):
         for layer in self.layer_nodes:
-            layer.set("Name", "%s%s" % (layer.get("Name"), suffix))
+            layer.set("Name", f"{layer.get('Name')}{suffix}")
 
     def merge_layers(self, with_name=None):
         layer_0 = self.layer_nodes.pop(0)
         if with_name:
             layer_0.set("Name", with_name)
-        for l in self.layer_nodes:
-            l.getparent().remove(l)
+        for layer in self.layer_nodes:
+            layer.getparent().remove(layer)
         self._layer_nodes = None
         self.active_layer = layer_0.get("Self")
         self.synchronize()
 
     def get_layer_id_by_name(self, layer_name):
-        layer_node = self.dom.xpath(".//Layer[@Name='%s']" % layer_name)[0]
+        layer_node = self.dom.xpath(f".//Layer[@Name='{layer_name}']")[0]
         return layer_node.get("Self")
 
     def get_active_layer_name(self):
-        layer_node = self.dom.xpath(".//Layer[@Self='%s']" % self.active_layer)[0]
+        layer_node = self.dom.xpath(f".//Layer[@Self='{self.active_layer}']")[0]
         return layer_node.get("Name")
 
 
 class Style(IDMLXMLFile):
     name = "Resources/Styles.xml"
 
-    def __init__(self, idml_package, working_copy_path=None):
-        super(Style, self).__init__(idml_package, working_copy_path)
-
     def get_style_node_by_name(self, style_name):
-        return self.dom.xpath(".//CharacterStyle[@Self='%s']" % style_name)[0]
+        return self.dom.xpath(f".//CharacterStyle[@Self='{style_name}']")[0]
 
     def style_groups(self):
         """ Groups are `RootCharacterStyleGroup', `RootParagraphStyleGroup' etc. """
         return [elt for elt in self.dom.xpath("/idPkg:Styles/*", namespaces={'idPkg': IdPkgNS})
                 if re.match(r"^.+Group$", elt.tag)]
 
     def get_root(self):
@@ -638,32 +635,32 @@
     name = "XML/Mapping.xml"
     initial_dom = ("<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"yes\"?>\
                    <idPkg:Mapping xmlns:idPkg=\"http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging\"\
                    DOMVersion=\"7.5\">\
                    </idPkg:Mapping>")
 
     def __init__(self, idml_package, working_copy_path=None):
-        super(StyleMapping, self).__init__(idml_package, working_copy_path)
+        super().__init__(idml_package, working_copy_path)
         self._character_style_mapping = None
 
     @property
     def fobj(self):
         """Overriden because it may not exists in the package. """
         try:
-            super(StyleMapping, self).fobj
+            super().fobj
         except (KeyError, IOError):
             if self.working_copy_path:
                 self._initialize_fobj()
         return self._fobj
 
     @property
     def dom(self):
         """Overriden because it may not exists in the package. """
         try:
-            super(StyleMapping, self).dom
+            super().dom
         except AttributeError:
             self._dom = etree.fromstring(self.initial_dom.encode("utf-8"))
         return self._dom
 
     @property
     def character_style_mapping(self):
         if self._character_style_mapping is None:
@@ -679,16 +676,16 @@
         filename = os.path.join(self.working_copy_path, self.name)
         fobj = open(filename, mode="w+")
         fobj.write(self.initial_dom)
         fobj.seek(0)
         self._fobj = fobj
 
     def iter_stylenode(self):
-        for n in self.dom.xpath("//XMLImportMap"):
-            yield n
+        for node in self.dom.xpath("//XMLImportMap"):
+            yield node
 
     def add_stylenode(self, node):
         self.dom.append(copy.deepcopy(node))
         self._character_style_mapping = None
 
 
 class Graphic(IDMLXMLFile):
@@ -715,15 +712,15 @@
     def fonts(self):
         return self.dom.xpath("//FontFamily")
 
     def get_root(self):
         return self.dom.xpath("/idPkg:Fonts", namespaces={'idPkg': IdPkgNS})[0]
 
 
-class Page(object):
+class Page():
     """
         Coordinate system
         -----------------
 
         The <Page> position in the <Spread> is expressed by 2 attributes :
 
             - `GeometricBounds' (y1 x1 y2 x2) where (x1, y1) is the position of the upper-left
@@ -761,16 +758,15 @@
             self._is_recto = is_recto
         return self._is_recto
 
     @property
     def face(self):
         if self.is_recto:
             return RECTO
-        else:
-            return VERSO
+        return VERSO
 
     @property
     def geometric_bounds(self):
         return [Decimal(c) for c in self.node.get("GeometricBounds").split(" ")]
 
     @geometric_bounds.setter
     def geometric_bounds(self, matrix):
@@ -817,50 +813,48 @@
             return True
         else:
             return False
 
     def set_face(self, face):
         if self.face == face:
             return
-        else:
-            item_transform = self.item_transform
-            item_transform_x_origin = item_transform[4]
+        item_transform = self.item_transform
+        item_transform_x_origin = item_transform[4]
 
-            if face == RECTO:
-                item_transform[4] = Decimal("0")
-            elif face == VERSO:
-                item_transform[4] = - self.geometric_bounds[3]
-
-            item_transform_x = item_transform[4] - item_transform_x_origin
-            self.item_transform = item_transform
-
-            # All page items are moved according to item_transform_x.
-            for item in self.page_items:
-                item_transform = [Decimal(c) for c in item.get("ItemTransform").split(" ")]
-                item_transform[4] = item_transform[4] + item_transform_x
-                item.set("ItemTransform", " ".join([str(v) for v in item_transform]))
+        if face == RECTO:
+            item_transform[4] = Decimal("0")
+        elif face == VERSO:
+            item_transform[4] = - self.geometric_bounds[3]
+
+        item_transform_x = item_transform[4] - item_transform_x_origin
+        self.item_transform = item_transform
+
+        # All page items are moved according to item_transform_x.
+        for item in self.page_items:
+            item_transform = [Decimal(c) for c in item.get("ItemTransform").split(" ")]
+            item_transform[4] = item_transform[4] + item_transform_x
+            item.set("ItemTransform", " ".join([str(v) for v in item_transform]))
 
-            self._is_recto = None
-            self._coordinates = None
+        self._is_recto = None
+        self._coordinates = None
 
 
 class XMLElement(Proxy):
     """A proxy over the etree.Element to represent XMLElement nodes in Story files. """
     def __repr__(self):
         if self.element is not None:
             return "%s {%s}" % (repr(self.element), ", ".join(["%s: %s" % (k, v) for k, v in self.element.items()]))
-        else:
-            return "XMLElement (no element)"
+        return "XMLElement (no element)"
 
     def __init__(self, element=None, tag=None):
         if element is not None:
             self.element = element
         else:
-            self.element = etree.Element("XMLElement", MarkupTag="XMLTag/%s" % tag)
-        super(XMLElement, self).__init__(target=self.element)
+            self.element = etree.Element("XMLElement", MarkupTag=f"XMLTag/{tag}")
+        super().__init__(target=self.element)
 
     def add_content(self, content, parent=None, style_range_node=None):
         content_element = etree.Element("Content")
         content_element.text = content
         if style_range_node is None:
             style_range_node = parent.clone_style_range()
         style_range_node.append(content_element)
@@ -909,39 +903,36 @@
         ]
 
         for attr in attrs:
             if style_node.get(attr) is not None:
                 style_range_node.set(attr, style_node.get(attr))
 
         for attr in ("Leading", "AppliedFont"):
-            path = "Properties/%s" % attr
+            path = f"Properties/{attr}"
             attr_node = style_node.find(path)
             if attr_node is not None:
                 properties_node.append(copy.deepcopy(attr_node))
         return style_range_node
 
     def get_attribute(self, name):
         attr_node = self._get_attribute_node(name)
-        return (attr_node is not None and
-                attr_node.get("Value") or None)
+        return attr_node.get("Value") if attr_node is not None else None
 
     def _get_attribute_node(self, name):
-        attr_node = self.xpath("./XMLAttribute[@Name='%s']" % name)
+        attr_node = self.xpath(f"./XMLAttribute[@Name='{name}']")
         if len(attr_node):
             return attr_node[0]
 
     def get_attributes(self):
-        return dict([(node.get("Name"), node.get("Value"))
-                     for node in self.xpath("./XMLAttribute")])
+        return {node.get("Name"): node.get("Value") for node in self.xpath("./XMLAttribute")}
 
     def set_attribute(self, name, value):
         attr_node = self._get_attribute_node(name)
         if attr_node is None:
-            attr_node = etree.Element("XMLAttribute", Name=name,
-                                      Self="%sXMLAttributen%s" % (self.get("Self"), name))
+            attr_node = etree.Element("XMLAttribute", Name=name, Self=f"{self.get('Self')}XMLAttributen{name}")
             self.append(attr_node)
         attr_node.set("Value", value)
 
     def set_attributes(self, attributes):
         for name, value in attributes.items():
             self.set_attribute(name, value)
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/decorators.py` & `SimpleIDML-1.1.6a1/src/simple_idml/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,28 +36,28 @@
             # Catch any exception to reset working_copy_path.
             try:
                 idml_package = view_func(idml_package, *args, **kwargs)
             except BaseException as err:
                 idml_package.working_copy_path = None
                 raise err
 
-        from simple_idml.idml import IDMLPackage
+        from simple_idml.idml import IDMLPackage  # pylint: disable=import-outside-toplevel
         # Create a new archive from the extracted one.
-        tmp_package = IDMLPackage("%s.idml" % tmp_filename, mode="w")
+        tmp_package = IDMLPackage(f"{tmp_filename}.idml", mode="w")
         for root, dirs, filenames in os.walk(tmp_filename):
             for filename in filenames:
                 filename = os.path.join(root, filename)
                 arcname = filename.replace(tmp_filename, "")
                 tmp_package.write(filename, arcname)
         tmp_package.close()
 
         # swap working_copy with initial IDML Package.
         new_filename = idml_package.filename
         idml_package.close()
         os.unlink(idml_package.filename)
-        os.rename(tmp_package.filename, new_filename)
+        shutil.move(tmp_package.filename, new_filename)
         shutil.rmtree(tmp_filename)
         idml_package.working_copy_path = None
 
         return IDMLPackage(new_filename)
 
     return new_func
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/extras.py` & `SimpleIDML-1.1.6a1/src/simple_idml/extras.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import os
 from simple_idml.idml import IDMLPackage
 
 
 def create_idml_package_from_dir(src_dir, destination):
     if not os.path.exists(src_dir):
-        raise IOError("%s does not exist." % src_dir)
+        raise IOError(f"{src_dir} does not exist.")
     if os.path.exists(destination):
-        raise IOError("%s already exist." % destination)
+        raise IOError(f"{destination} already exist.")
 
     with IDMLPackage(destination, mode="w") as package:
         for root, dirs, filenames in os.walk(src_dir):
             for filename in filenames:
                 if filename in ['.DS_Store']:
                     continue
                 package.write(os.path.join(root, filename),
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/ftp.py` & `SimpleIDML-1.1.6a1/src/simple_idml/ftp.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 
 def copy(src_filename, dst_filename, ftp_params=None, src_open_mode="rb"):
     if not ftp_params:
         shutil.copy(src_filename, dst_filename)
         return
 
-    with open(src_filename, src_open_mode) as f:
+    with open(src_filename, src_open_mode) as fobj:
         ftp = get_ftp(ftp_params)
         command = f'STOR {dst_filename}'
         try:
             if "b" in src_open_mode:
-                ftp.storbinary(command, f)
+                ftp.storbinary(command, fobj)
             else:  # python2 only. storlines in Python 3 requires binary mode as well.
-                ftp.storlines(command, f)
+                ftp.storlines(command, fobj)
         except:
             print(f'Cannot {command}')
             raise
         finally:
             close_ftp_conn(ftp, ftp_params)
 
 
@@ -88,23 +88,23 @@
     close_ftp_conn(ftp, ftp_params)
 
 
 def read(filename, ftp_params=None):
     response = ""
 
     if not ftp_params:
-        with open(filename, "rb") as f:
-            response = f.read()
+        with open(filename, "rb") as fobj:
+            response = fobj.read()
     else:
-        with BytesIO() as r:
+        with BytesIO() as buf:
             ftp = get_ftp(ftp_params)
-            ftp.retrbinary('RETR %s' % filename, r.write)
+            ftp.retrbinary(f'RETR {filename}', buf.write)
             close_ftp_conn(ftp, ftp_params)
-            r.seek(0)
-            response = r.read()
+            buf.seek(0)
+            response = buf.read()
 
     return response
 
 
 def zip_dir(dirname, zip_filename, ftp_params=None):
     if ftp_params:
         # Work locally in a temporary directory.
@@ -116,74 +116,74 @@
             'user': ftp_params['auth'][1],
             'passwd': ftp_params['auth'][2],
             'url': ftp_params['auth'][0],
             'no_passive': ftp_params['passive'] and "" or "--no-passive-ftp",
             'dirname': dirname,
             'dst': tmp_dirname
         }
-        p = subprocess.Popen(shlex.split(cmd))
-        p.wait()
+        proc = subprocess.Popen(shlex.split(cmd))
+        proc.wait()
 
         zip_tree(os.path.join(tmp_dirname, dirname), tmp_zip_filename)
         copy(tmp_zip_filename, zip_filename, ftp_params)
         shutil.rmtree(tmp_dirname)
         rmtree(dirname, ftp_params)
     else:
         zip_tree(dirname, zip_filename)
         shutil.rmtree(dirname)
 
 
 def zip_tree(tree, destination):
-    #http://stackoverflow.com/a/17080988/113036
+    # http://stackoverflow.com/a/17080988/113036
     relroot = os.path.abspath(os.path.join(tree, os.pardir))
-    with zipfile.ZipFile(destination, "w", zipfile.ZIP_DEFLATED) as zip:
+    with zipfile.ZipFile(destination, "w", zipfile.ZIP_DEFLATED) as zfile:
         for root, dirs, files in os.walk(tree):
             # add directory (needed for empty dirs)
-            zip.write(root, os.path.relpath(root, relroot))
+            zfile.write(root, os.path.relpath(root, relroot))
             for file in files:
                 filename = os.path.join(root, file)
                 if os.path.isfile(filename):  # regular files only
                     arcname = os.path.join(os.path.relpath(root, relroot), file)
-                    zip.write(filename, arcname)
+                    zfile.write(filename, arcname)
 
 
 # https://gist.github.com/Starou/beb8bde114bf7a20cf80
 def rmtree_ftp(ftp, path):
     """Recursively delete a directory tree on a remote server."""
-    wd = ftp.pwd()
+    working_dir = ftp.pwd()
 
     try:
         names = ftp.nlst(path)
-    except ftplib.all_errors as e:
+    except ftplib.all_errors as exc:
         # some FTP servers complain when you try and list non-existent paths
-        #_log.debug('FtpRmTree: Could not remove {0}: {1}'.format(path, e))
+        #_log.debug('FtpRmTree: Could not remove {0}: {1}'.format(path, exc))
         return
 
     for name in names:
         if os.path.split(name)[1] in ('.', '..'):
             continue
 
         try:
             ftp.cwd(name)  # if we can cwd to it, it's a folder
-            ftp.cwd(wd)  # don't try a nuke a folder we're in
+            ftp.cwd(working_dir)  # don't try a nuke a folder we're in
             rmtree_ftp(ftp, name)
         except ftplib.all_errors:
             ftp.delete(name)
 
     try:
         ftp.rmd(path)
-    except ftplib.all_errors as e:
-        raise e
+    except ftplib.all_errors as exc:
+        raise exc
 
 
-def mkdir_unique(dir, ftp_params=None):
+def mkdir_unique(directory, ftp_params=None):
     if not ftp_params:
-        unique_path = tempfile.mkdtemp(dir=dir)
+        unique_path = tempfile.mkdtemp(dir=directory)
     else:
-        unique_path = os.path.join(dir, uuid.uuid1().hex)
+        unique_path = os.path.join(directory, uuid.uuid1().hex)
         ftp = get_ftp(ftp_params)
         ftp.mkd(unique_path)
         close_ftp_conn(ftp, ftp_params)
     return unique_path
 
 
 def close_ftp_conn(ftp, ftp_params=None):
@@ -195,16 +195,16 @@
         ftp.quit()
 
 
 def get_ftp(ftp_params):
     ftp = ftplib.FTP(*ftp_params["auth"])
     ftp.set_pasv(ftp_params["passive"])
 
-    #https://bbs.archlinux.org/viewtopic.php?id=134529
-    #https://github.com/keepitsimple/pyFTPclient/blob/master/pyftpclient.py
+    # https://bbs.archlinux.org/viewtopic.php?id=134529
+    # https://github.com/keepitsimple/pyFTPclient/blob/master/pyftpclient.py
     if ftp_params.get('keepalive', False) is True:
         ftp.sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
     if 'keepalive_interval' in ftp_params and hasattr(socket, "TCP_KEEPINTVL"):
         ftp.sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPINTVL,
                             ftp_params['keepalive_interval'])
     if 'keepalive_idle' in ftp_params and hasattr(socket, "TCP_KEEPIDLE"):
         ftp.sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPIDLE,
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/id_package.py` & `SimpleIDML-1.1.6a1/src/simple_idml/id_package.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/src/simple_idml/idml.py` & `SimpleIDML-1.1.6a1/src/simple_idml/idml.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,15 @@
     def __init__(self, *args, **kwargs):
         kwargs["compression"] = zipfile.ZIP_STORED
         zipfile.ZipFile.__init__(self, *args, **kwargs)
         self.working_copy_path = None
         self.init_lazy_references()
 
     def __repr__(self):
-        return "<idml.IDMLPackage instance of '%s' at %s>" % (
-            os.path.basename(self.filename),
-            hex(id(self))
-        )
+        return f"<idml.IDMLPackage instance of '{os.path.basename(self.filename)}' at {hex(id(self))}>"
 
     def init_lazy_references(self):
         self._xml_structure = None
         self._xml_structure_tree = None
         self._designmap = None
         self._tags = None
         self._font_families = None
@@ -51,25 +48,24 @@
         self._stories = None
         self._story_ids = None
         self._referenced_layers = None
 
     def namelist(self):
         if not self.working_copy_path:
             return zipfile.ZipFile.namelist(self)
-        else:
-            namelist = []
-            for root, dirs, filenames in os.walk(self.working_copy_path):
-                rel_root = root.replace(self.working_copy_path, "")[1:]
-                for filename in filenames:
-                    namelist.append("%(rel_root)s%(sep)s%(filename)s" % {
-                        'rel_root': rel_root,
-                        'sep': rel_root and "/" or "",
-                        'filename': filename
-                    })
-            return namelist
+        namelist = []
+        for root, dirs, filenames in os.walk(self.working_copy_path):
+            rel_root = root.replace(self.working_copy_path, "")[1:]
+            for filename in filenames:
+                namelist.append("%(rel_root)s%(sep)s%(filename)s" % {
+                    'rel_root': rel_root,
+                    'sep': rel_root and "/" or "",
+                    'filename': filename
+                })
+        return namelist
 
     def contentfile_namelist(self):
         """Namelist filtered on Spreads and Stories. """
         return [f for f in self.namelist() if os.path.dirname(f) in ("Spreads", "Stories")]
 
     @property
     def xml_structure(self):
@@ -91,28 +87,28 @@
                     if not elt.get("MarkupTag"):
                         continue
                     elt = XMLElement(elt)
                     new_destination_node = elt.to_xml_structure_element()
                     destination_node.append(new_destination_node)
                     if elt.get("XMLContent"):
                         xml_content_value = elt.get("XMLContent")
-                        story_name = "Stories/Story_%s.xml" % xml_content_value
+                        story_name = f"Stories/Story_{xml_content_value}.xml"
                         story = Story(self, name=story_name)
                         try:
                             new_source_node = story.get_element_by_id(elt.get("Self"))
                         # The story does not exists.
                         except KeyError:
                             continue
                         else:
                             append_childs(new_source_node, new_destination_node)
                     else:
                         append_childs(elt, new_destination_node)
 
             append_childs(source_node, structure)
-            self._xml_structure = structure
+            self._xml_structure = structure  # pylint: disable=attribute-defined-outside-init
         return self._xml_structure
 
     def xml_structure_pretty(self):
         return etree.tostring(self.xml_structure, pretty_print=True)
 
     @property
     def xml_structure_tree(self):
@@ -121,116 +117,116 @@
             self._xml_structure_tree = xml_structure_tree
         return self._xml_structure_tree
 
     @property
     def designmap(self):
         if self._designmap is None:
             designmap = Designmap(self, working_copy_path=self.working_copy_path)
-            self._designmap = designmap
+            self._designmap = designmap  # pylint: disable=attribute-defined-outside-init
         return self._designmap
 
     @property
     def tags(self):
         if self._tags is None:
             tags = [copy.deepcopy(elt) for elt in Tags(self).tags()]
-            self._tags = tags
+            self._tags = tags  # pylint: disable=attribute-defined-outside-init
         return self._tags
 
     @property
     def font_families(self):
         if self._font_families is None:
             font_families = [copy.deepcopy(elt) for elt in Fonts(self).fonts()]
-            self._font_families = font_families
+            self._font_families = font_families  # pylint: disable=attribute-defined-outside-init
         return self._font_families
 
     @property
     def style_groups(self):
         if self._style_groups is None:
             style_groups = [copy.deepcopy(elt) for elt in Style(self).style_groups()]
-            self._style_groups = style_groups
+            self._style_groups = style_groups  # pylint: disable=attribute-defined-outside-init
         return self._style_groups
 
     @property
     def style(self):
         if self._style is None:
             style = Style(self, self.working_copy_path)
-            self._style = style
+            self._style = style  # pylint: disable=attribute-defined-outside-init
         return self._style
 
     @property
     def style_mapping(self):
         """The style mapping file may not be present in the archive and is created in that case. """
         if self._style_mapping is None:
             style_mapping = StyleMapping(self, self.working_copy_path)
-            self._style_mapping = style_mapping
+            self._style_mapping = style_mapping  # pylint: disable=attribute-defined-outside-init
         return self._style_mapping
 
     @property
     def graphic(self):
         if self._graphic is None:
             graphic = Graphic(self, self.working_copy_path)
-            self._graphic = graphic
+            self._graphic = graphic  # pylint: disable=attribute-defined-outside-init
         return self._graphic
 
     @property
     def spreads(self):
         if self._spreads is None:
             spreads = [elt for elt in self.namelist() if re.match("^Spreads/*", elt)]
-            self._spreads = spreads
+            self._spreads = spreads  # pylint: disable=attribute-defined-outside-init
         return self._spreads
 
     @property
     def spreads_objects(self):
         if self._spreads_objects is None:
             spreads_objects = [Spread(self, s, self.working_copy_path) for s in self.spreads]
-            self._spreads_objects = spreads_objects
+            self._spreads_objects = spreads_objects  # pylint: disable=attribute-defined-outside-init
         return self._spreads_objects
 
     @property
     def last_spread(self):
         if self._last_spread is None:
             src = self.designmap.spread_nodes[-1].get("src")
-            self._last_spread = Spread(self, src, self.working_copy_path)
+            self._last_spread = Spread(self, src, self.working_copy_path)  # pylint: disable=attribute-defined-outside-init
         return self._last_spread
 
     @property
     def pages(self):
         if self._pages is None:
             pages = []
             for spread in self.spreads_objects:
                 pages += spread.pages
-            self._pages = pages
+            self._pages = pages  # pylint: disable=attribute-defined-outside-init
         return self._pages
 
     @property
     def backing_story(self):
         """The style mapping file may not be present in the archive and is created in that case. """
         if self._backing_story is None:
             backing_story = BackingStory(self, working_copy_path=self.working_copy_path)
-            self._backing_story = backing_story
+            self._backing_story = backing_story  # pylint: disable=attribute-defined-outside-init
         return self._backing_story
 
     @property
     def stories(self):
         if self._stories is None:
             stories = [elt for elt in self.namelist()
-                       if re.match("^%s/*" % STORIES_DIRNAME, elt)]
-            self._stories = stories
+                       if re.match(f"^{STORIES_DIRNAME}/*", elt)]
+            self._stories = stories  # pylint: disable=attribute-defined-outside-init
         return self._stories
 
     def stories_for_node(self, node_path):
-        return ["%s/Story_%s.xml" % (STORIES_DIRNAME, child.get("XMLContent"))
+        return [f"{STORIES_DIRNAME}/Story_{child.get('XMLContent')}.xml"
                 for child in self.xml_structure.xpath(node_path)[0].iter()
                 if child.get("XMLContent") in self.story_ids]
 
     @property
     def story_ids(self):
         """ extract  `ID' from `Stories/Story_ID.xml'. """
         if self._story_ids is None:
-            self._story_ids = self._get_story_ids_for_stories(self.stories)
+            self._story_ids = self._get_story_ids_for_stories(self.stories)  # pylint: disable=attribute-defined-outside-init
         return self._story_ids
 
     def story_ids_for_node(self, node_path):
         return self._get_story_ids_for_stories(self.stories_for_node(node_path))
 
     def _get_story_ids_for_stories(self, stories):
         rx_story_id = re.compile(r"%s/Story_([\w]+)\.xml" % STORIES_DIRNAME)
@@ -241,15 +237,15 @@
         if self._referenced_layers is None:
             referenced_layers = []
             for layer in self.designmap.layer_nodes:
                 layer_id = layer.get("Self")
                 for spread in self.spreads_objects:
                     if spread.has_any_item_on_layer(layer_id):
                         referenced_layers.append(layer_id)
-            self._referenced_layers = referenced_layers
+            self._referenced_layers = referenced_layers  # pylint: disable=attribute-defined-outside-init
         return self._referenced_layers
 
     @use_working_copy
     def import_xml(self, xml, at):
         """ Reproduce the action «Import XML» on a XML Element in InDesign® Structure. """
 
         # Python 3 strictly require a bytestring.
@@ -270,15 +266,15 @@
                     value_to_apply = style_to_apply_node.get(attr)
                     applied_value = style_range_node.get(attr) or applied_style_node.get(attr)
                     if attr == "FontStyle":
                         style_range_node.set(attr, _merge_font_style(applied_value, value_to_apply))
                     else:
                         style_range_node.set(attr, style_to_apply_node.get(attr))
             # TODO
-            #for attr in ("Leading", "AppliedFont"):
+            # for attr in ("Leading", "AppliedFont"):
             #    path = "Properties/%s" % attr
             #    source_attr_node = source_style_node.find(path)
             #    attr_node = (style_node is not None and style_node.find(path) is not None)
             #    if attr_node is None and source_attr_node is not None:
             #        properties_element.append(copy.deepcopy(source_attr_node))
 
         mergeable_font_styles = {
@@ -305,15 +301,15 @@
             """Use the more distant parent as base style and then apply its children styles until the new tag itself.
 
             Returns:
              o new_style_range_node: unbound element.
              o root_style_node
             """
             nested_styles = []
-            while(xml_structure_node is not None):
+            while xml_structure_node is not None :
                 style_name = self.style_mapping.character_style_mapping.get(xml_structure_node.tag)
                 if style_name:
                     style_node = self.style.get_style_node_by_name(style_name)
                     nested_styles.insert(0, style_node)
                 xml_structure_node = xml_structure_node.getparent()
 
             # Merge the styles starting from the top parent like in a HTML document.
@@ -335,17 +331,17 @@
             # If the parent specify a font face, a font style or a font size and the style_node don't, it is added.
             for attr in ("PointSize", "FontStyle", "HorizontalScale", "Tracking",
                          "FillColor", "FillTint", "Capitalization", "Position"):
                 if parent_style_node.get(attr) is not None and (applied_style_node is None or not applied_style_node.get(attr)):
                     style_range_node.set(attr, parent_style_node.get(attr))
 
             for attr in ("Leading", "AppliedFont"):
-                path = "Properties/%s" % attr
+                path = f"Properties/{attr}"
                 parent_attr_node = parent_style_node.find(path)
-                attr_node = (applied_style_node is not None and applied_style_node.find(path) is not None) or None
+                attr_node = applied_style_node.find(path) is not None if applied_style_node is not None else None
                 if attr_node is None and parent_attr_node is not None:
                     properties_element.append(copy.deepcopy(parent_attr_node))
 
         def _move_siblings_content(at, element_id):
             """ When new XML elements are inserted, the siblings of the initial <content> (<BR> etc) are
                 repositionned after the last <content> created.
             """
@@ -353,24 +349,24 @@
             element = story.get_element_by_id(element_id)
             content_nodes = element.get_element_content_nodes()
             if len(content_nodes) < 2:
                 return
 
             first_content_node = content_nodes[0]
             last_content_node = content_nodes[-1]
-            siblings = [s for s in first_content_node.itersiblings()]
+            siblings = list(first_content_node.itersiblings())
             if not len(siblings):
                 return
 
             for sibling in siblings:
                 last_content_node.addnext(sibling)
             story.synchronize()
 
         def _import_new_node(source_node, at=None, element_id=None, story=None):
-            xml_structure_parent_node = self.xml_structure.find("*//*[@Self='%s']" % element_id)
+            xml_structure_parent_node = self.xml_structure.find(f"*//*[@Self='{element_id}']")
             xml_structure_new_node = etree.Element(source_node.tag)
             # We cannot force the self._xml_structure reset by setting it at None.
             xml_structure_parent_node.append(xml_structure_new_node)
 
             style_range_node, applied_style_node = _get_nested_style_range_node(xml_structure_new_node)
             story = story or self.get_story_object_by_xpath(at)
             parent = story.get_element_by_id(element_id)
@@ -382,15 +378,15 @@
 
             xml_structure_new_node.set("Self", new_xml_element.get("Self"))
 
             # Source may also contains some children.
             source_node_children = source_node.getchildren()
             if len(source_node_children):
                 story.synchronize()
-                for j, source_node_child in enumerate(source_node_children):
+                for source_node_child in source_node_children:
                     _import_new_node(source_node_child,
                                      element_id=new_xml_element.get("Self"),
                                      story=story)
 
             if source_node.tail:
                 story.add_content_to_element(element_id, source_node.tail, parent)
             story.synchronize()
@@ -406,15 +402,15 @@
                 content_flags = items.get(SETCONTENT_TAG, "").split(',')
                 if "remove-previous-br" in content_flags:
                     local_story = story or self.get_story_object_by_xpath(at)
                     elt = local_story.get_element_by_id(element_id).element
                     for _elt in reversed(elt.xpath("preceding::*")):
                         if _elt.tag == "XMLElement":
                             break
-                        elif _elt.tag == "Br":
+                        if _elt.tag == "Br":
                             _elt.getparent().remove(_elt)
                             continue
                     local_story.synchronize()
                 if "delete" in content_flags:
                     local_story = story or self.get_story_object_by_xpath(at)
                     local_story.remove_element(element_id, synchronize=True)
                     spread = self.get_spread_object_by_xpath(at)
@@ -438,15 +434,15 @@
                     for s, d in zip(source_node_children, [self.xml_structure_tree.getpath(c) for c in
                                                            destination_node.iterchildren()]):
                         _import_node(s, at=d, ignorecontent_parent_flag=ignorecontent)
 
                 # Step-by-step iteration.
                 else:
                     destination_node_child = next(destination_node_children, None)
-                    for i, source_child in enumerate(source_node_children):
+                    for source_child in source_node_children:
                         # Source and destination match.
                         if destination_node_child is not None and source_child.tag == destination_node_child.tag:
                             _import_node(source_child, at=self.xml_structure_tree.getpath(destination_node_child),
                                          ignorecontent_parent_flag=ignorecontent)
                             destination_node_child = next(destination_node_children, None)
                         # Source does not match destination. It is added, but only if the tag is mapped to a style.
                         elif not ignorecontent and source_child.tag in self.style_mapping.character_style_mapping.keys():
@@ -454,32 +450,32 @@
 
                     _move_siblings_content(at, element_id)
 
         _import_node(source_node, at)
         return self
 
     @use_working_copy
-    def import_pdf(self, pdf_path, at, crop="CropContentVisibleLayers"):
-        self.set_attributes(at, {'href': "%s" % pdf_path})
+    def import_pdf(self, pdf_path, at, crop="CropContentVisibleLayers", page_number=1):
+        self.set_attributes(at, {'href': pdf_path})
         spread = self.get_spread_object_by_xpath(at)
 
         # spread_elt is a <Rectangle> that will host the <PDF>.
         # The <PDF> element get the id of the <Rectangle>.
         spread_elt = self.get_spread_elem_by_xpath(at)
         element_id = self.get_element_content_id_by_xpath(at)
-        spread_elt.set("Self", "%s-old" % element_id)
+        spread_elt.set("Self", f"{element_id}-old")
         x, y = self.get_elem_point_position(spread_elt)
         pdf_node = etree.fromstring(f"""<PDF Self="{element_id}" GrayVectorPolicy="IgnoreAll" RGBVectorPolicy="IgnoreAll" CMYKVectorPolicy="IgnoreAll" OverriddenPageItemProps="" LocalDisplaySetting="Default" ImageTypeName="$ID/Adobe Portable Document Format (PDF)" AppliedObjectStyle="ObjectStyle/$ID/[None]" ItemTransform="1 0 0 1 {x} {y}" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" Visible="true" Name="$ID/">
         <TextWrapPreference Inverse="false" ApplyToMasterPageOnly="false" TextWrapSide="BothSides" TextWrapMode="None">
             <Properties>
                 <TextWrapOffset Top="0" Left="0" Bottom="0" Right="0" />
             </Properties>
             <ContourOption ContourType="SameAsClipping" IncludeInsideEdges="false" ContourPathName="$ID/" />
         </TextWrapPreference>
-        <PDFAttribute PageNumber="1" PDFCrop="{crop}" TransparentBackground="true" />
+        <PDFAttribute PageNumber="{page_number}" PDFCrop="{crop}" TransparentBackground="true" />
         <MetadataPacketPreference>
         </MetadataPacketPreference>
         <Link Self="{element_id}-link" AssetURL="$ID/" AssetID="$ID/" LinkResourceURI="{pdf_path}" LinkResourceFormat="$ID/Adobe Portable Document Format (PDF)" StoredState="Normal" LinkResourceModified="false" LinkObjectModified="false" ShowInUI="true" CanEmbed="true" CanUnembed="true" CanPackage="true" ImportPolicy="NoAutoImport" ExportPolicy="NoAutoExport" />
         <ClippingPathSettings ClippingType="None" InvertPath="false" IncludeInsideEdges="false" RestrictToFrame="false" UseHighResolutionImage="true" Threshold="25" Tolerance="2" InsetFrame="0" AppliedPathName="$ID/" Index="-1" />
         <GraphicLayerOption UpdateLinkOption="KeepOverrides" />
     </PDF>""")
 
@@ -616,26 +612,26 @@
     def suffix_layers(self, suffix):
         self.designmap.suffix_layers(suffix)
         self.designmap.synchronize()
         return self
 
     @use_working_copy
     def insert_idml(self, idml_package, at, only):
-        t = self._get_item_translation_for_insert(idml_package, at, only)
+        trans = self._get_item_translation_for_insert(idml_package, at, only)
         self.remove_content(at)
         self._add_font_families_from_idml(idml_package)
         self._add_styles_from_idml(idml_package)
         self._add_mapped_styles_from_idml(idml_package)
         self._add_graphics_from_idml(idml_package)
         self._add_tags_from_idml(idml_package)
-        self._add_spread_elements_from_idml(idml_package, at, only, t)
+        self._add_spread_elements_from_idml(idml_package, at, only, trans)
         self._add_stories_from_idml(idml_package, at, only)
         self._add_layers_from_idml(idml_package, at, only)
         self.remove_orphan_layers()
-        self._xml_structure = None
+        self._xml_structure = None  # pylint: disable=attribute-defined-outside-init
         return self
 
     @use_working_copy
     def remove_content(self, under):
         """Recursively reach the leafs to remove the content. """
         def _remove_content(node):
             if len(node.getchildren()):
@@ -651,16 +647,17 @@
 
             spread = self.get_spread_object_by_xpath(xpath)
             if spread:
                 spread.remove_page_item(element_content_id, synchronize=True)
 
         try:
             node = self.xml_structure.xpath(under)[0]
-        except IndexError:
-            raise IndexError("Cannot remove content under path '%s'. Are you sure the path exists ?" % under)
+        except IndexError as exc:
+            raise IndexError(f"Cannot remove content under path '{under}'."
+                             " Are you sure the path exists?") from exc
 
         for child in node.iterchildren():
             _remove_content(child)
         # `under' node may have a reference to its first children in his story.
         story = self.get_story_object_by_xpath(under)
         story.remove_children(node.get("Self"), synchronize=True)
 
@@ -733,15 +730,15 @@
         self.graphic.synchronize()
 
     def _add_tags_from_idml(self, idml_package):
         tags = Tags(self)
         tags.working_copy_path = self.working_copy_path
         tags_root_elt = tags.get_root()
         for tag in idml_package.tags:
-            if not tags_root_elt.xpath("//XMLTag[@Self='%s']" % (tag.get("Self"))):
+            if not tags_root_elt.xpath(f"//XMLTag[@Self='{tag.get('Self')}']"):
                 tags_root_elt.append(copy.deepcopy(tag))
         tags.synchronize()
 
     def _get_item_translation_for_insert(self, idml_package, at, only):
         """ Compute the ItemTransform shift to apply to the elements in idml_package to insert. """
 
         at_elem = self.get_spread_elem_by_xpath(at)
@@ -781,22 +778,24 @@
         # Add spread elements on the same layer. We start by that because the order in the
         # Spread file is the z-position on the Layer.
         only_layer = idml_package.get_structure_element_layer_id(only_node)
         spread_elts_to_add = idml_package.get_spread_elements_by_layer(layer_id=only_layer,
                                                                        excluded_tags=["Guide"])
 
         # Then add the tagged elements that may be on others layers.
+        all_elts_to_add = [elt for lst in [elt.findall('*') for elt in spread_elts_to_add]
+                           for elt in lst] + spread_elts_to_add
         for node in only_node.iter():
             if node.get("XMLContent") is None:
                 continue
             spread_elt = idml_package.get_spread_elem_by_id(node.get("XMLContent"))
             # Image and EPS element are included in a Rectangle.
             if spread_elt.tag in ["Image", "EPS"]:
                 spread_elt = spread_elt.getparent()
-            if spread_elt not in spread_elts_to_add:
+            if spread_elt not in all_elts_to_add:
                 spread_elts_to_add.append(spread_elt)
 
         def _add_spread_element(spread_dest_elt, spread_elt):
             spread_elt_copy = copy.deepcopy(spread_elt)
             self.apply_translation_to_element(spread_elt_copy, translation)
             spread_dest_elt.append(spread_elt_copy)
 
@@ -873,17 +872,16 @@
 
         # Add Story files.
         # `Stories' directory may not be present in the destination package.
         stories_dirname = os.path.join(self.working_copy_path, STORIES_DIRNAME)
         if not os.path.exists(stories_dirname):
             os.mkdir(stories_dirname)
         for filename in idml_package.stories_for_node(only):
-            story_cp = open(os.path.join(self.working_copy_path, filename), mode="wb+")
-            story_cp.write(idml_package.open(filename, mode="r").read())
-            story_cp.close()
+            with open(os.path.join(self.working_copy_path, filename), mode="wb+") as story_cp:
+                story_cp.write(idml_package.open(filename, mode="r").read())
 
         # Update designmap.xml.
         self.designmap.add_stories(idml_package.story_ids_for_node(only))
         self.designmap.synchronize()
         # BackingStory.xml ??
         self.init_lazy_references()
 
@@ -944,15 +942,15 @@
 
     @use_working_copy
     def xml_element_leaf_to_node(self, xpath, xml_content_ref):
         spread = self.get_spread_object_by_xpath(xpath)
         page_item = spread.get_element_by_id(xml_content_ref, tag="*", attr="Self")
 
         page_item.set("ParentStory", xml_content_ref)
-        page_item.set("Self", "%sToNode" % xml_content_ref)
+        page_item.set("Self", f"{xml_content_ref}ToNode")
 
         # To be a node, a Rectangle must be converted into a TextFrame.
         # There is not simple way to change the tag of a XMLElement so
         # a new copy is created.
         if page_item.tag == "Rectangle":
             spread.rectangle_to_textframe(page_item)
         spread.synchronize()
@@ -964,17 +962,17 @@
         # TODO : make sure the filename does not exists.
         new_spread_name = increment_filename(self.last_spread.name)
         new_spread_wc_path = os.path.join(working_copy_path, new_spread_name)
         shutil.copy2(
             os.path.join(working_copy_path, self.last_spread.name),
             new_spread_wc_path
         )
-        self._spreads = None
-        self._spreads_objects = None
-        self._last_spread = None
+        self._spreads = None  # pylint: disable=attribute-defined-outside-init
+        self._spreads_objects = None  # pylint: disable=attribute-defined-outside-init
+        self._last_spread = None  # pylint: disable=attribute-defined-outside-init
 
         new_spread = Spread(self, new_spread_name, working_copy_path)
         new_spread.clear()
         new_spread.node.set("Self", new_spread.get_node_name_from_xml_name())
 
         self.designmap.add_spread(new_spread)
         self.designmap.synchronize()
@@ -985,15 +983,15 @@
     def get_spread_elements_by_layer(self, layer_name=None, layer_id=None, excluded_tags=[]):
         layer_id = layer_id or self.get_layer_id_by_name(layer_name)
 
         spread_elements = []
         for spread_object in self.spreads_objects:
             spread_elements.extend(spread_object.dom.xpath(
                 ".//*%(excluded_tags)s[@ItemLayer='%(layer_id)s']" % {
-                    'excluded_tags': "".join(["[not(self::%s)]" % e for e in excluded_tags]),
+                    'excluded_tags': "".join([f"[not(self::{e})]" for e in excluded_tags]),
                     'layer_id': layer_id}))
 
         return spread_elements
 
     def get_spread_object_by_name(self, name):
         """ - name : 'Spreads/Spread_mainub6.xml' """
         return next(filter(lambda s: s.name == name, self.spreads_objects))
@@ -1034,15 +1032,15 @@
         elt = spread.get_element_by_id(elt_id, tag="*")
         if elt is None:
             elt = spread.get_element_by_id(elt_id, tag="*", attr="ParentStory")
         return elt
 
     def get_spread_by_xpath(self, xpath):
         spread = self.get_spread_object_by_xpath(xpath)
-        return spread and spread.name or None
+        return spread.name if spread else None
 
     def get_layer_id_by_name(self, layer_name):
         return self.designmap.get_layer_id_by_name(layer_name)
 
     def get_active_layer_name(self):
         return self.designmap.get_active_layer_name()
 
@@ -1057,39 +1055,37 @@
     def get_story_object_by_xpath(self, xpath):
         xml_element = self.xml_structure.xpath(xpath)[0]
 
         def get_story_name(xml_element):
             ref = xml_element.get("XMLContent")
             if ref:
                 return ref
-            else:
-                parent = xml_element.getparent()
-                if parent is not None:
-                    return get_story_name(xml_element.getparent())
-                else:
-                    return BACKINGSTORY
+            parent = xml_element.getparent()
+            if parent is not None:
+                return get_story_name(xml_element.getparent())
+            return BACKINGSTORY
 
         story_name = get_story_name(xml_element)
 
         # Some XMLElement store a reference which is not a Story.
         # In that case, the Story is the parent's Story.
         if (story_name not in self.story_ids) and (story_name is not BACKINGSTORY):
             xpath = self.xml_structure_tree.getpath(xml_element.getparent())
             story = self.get_story_object_by_xpath(xpath)
         else:
             if story_name == BACKINGSTORY:
                 story = BackingStory(self)
             else:
-                story = Story(self, "%s/Story_%s.xml" % (STORIES_DIRNAME, story_name))
+                story = Story(self, f"{STORIES_DIRNAME}/Story_{story_name}.xml")
         story.working_copy_path = self.working_copy_path
         return story
 
     def get_story_by_xpath(self, xpath):
         story = self.get_story_object_by_xpath(xpath)
-        return story and story.name or None
+        return story.name if story else None
 
     def get_element_content_id_by_xpath(self, xpath):
         return self.xml_structure.xpath(xpath)[0].get("XMLContent")
 
     def get_elem_point_position(self, elem, point_index=0):
         point = elem.xpath("Properties/PathGeometry/GeometryPathType/PathPointArray/PathPointType")[point_index]
         x, y = point.get("Anchor").split(" ")
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/indesign/indesign.py` & `SimpleIDML-1.1.6a1/src/simple_idml/indesign/indesign.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # -*- coding: utf-8 -*-
 
-from builtins import object
 import logging
 import ntpath
 import os
+
+from xml.sax import SAXParseException
+from zipfile import ZipFile
+
+from suds.client import Client
+
 from simple_idml import exceptions
 from simple_idml import ftp
 from simple_idml.decorators import simple_decorator
-from suds.client import Client
-from xml.sax import SAXParseException
-from zipfile import ZipFile
 
 CURRENT_DIR = os.path.abspath(os.path.split(__file__)[0])
 SCRIPTS_DIR = os.path.join(CURRENT_DIR, "scripts")
 
 
 class InDesignSoapScript(object):
+    javascript_basename = None
+
     def __init__(self, server_url, client_workdir, server_workdir, server_path_style="posix",
                  ftp_params=None, clean_workdir=True, logger=None, logger_extra=None):
+        self.client = None
+        self.javascript_client_copy_filename = None
+        self.javascript_server_copy_filename = None
+        self.params = None
+
         self.server_url = server_url
         self.client_workdir = client_workdir
         self.server_workdir = server_workdir
         self.ftp_params = ftp_params
         self.clean_workdir = clean_workdir
 
         if not logger:
@@ -31,15 +40,15 @@
         self.logger_extra = logger_extra or {}
 
         self.server_path_mod = ntpath if server_path_style == "windows" else os.path
 
     def execute(self):
         self.copy_script_on_working_directory()
 
-        self.client = Client("%s/service?wsdl" % self.server_url)
+        self.client = Client(f"{self.server_url}/service?wsdl")
         self.client.set_options(location=self.server_url)
         self.set_params()
         return self.runscript()
 
     def copy_script_on_working_directory(self):
         javascript_master_filename = os.path.join(SCRIPTS_DIR, self.javascript_basename)
         self.javascript_client_copy_filename = os.path.join(self.client_workdir, self.javascript_basename)
@@ -50,27 +59,27 @@
 
     def set_params(self):
         self.params = self.client.factory.create("ns0:RunScriptParameters")
         self.params.scriptLanguage = 'javascript'
         self.params.scriptFile = self.javascript_server_copy_filename
 
     def runscript(self):
-        self.logger.debug('Calling SOAP "RunScript" service (params: %s)' % self.params, extra=self.logger_extra)
+        self.logger.debug('Calling SOAP "RunScript" service (params: %s)', self.params, extra=self.logger_extra)
         try:
             response = self.client.service.RunScript(self.params)
-        except SAXParseException as e:
+        except SAXParseException as exc:
             response = None
-            self.logger.error('SAXParseException: %s' % e.getMessage(), extra=self.logger_extra)
+            self.logger.error('SAXParseException: %s', exc.getMessage(), extra=self.logger_extra)
         else:
             if response.errorNumber:
-                self.logger.error("SOAP response: %s\nSOAP RunScript params: %s" % (response, self.params),
+                self.logger.error("SOAP response: %s\nSOAP RunScript params: %s", response, self.params,
                                   extra=self.logger_extra)
                 raise exceptions.InDesignSoapException(self.params, response)
 
-            self.logger.debug('"RunScript" successful! Response: %s' % response, extra=self.logger_extra)
+            self.logger.debug('"RunScript" successful! Response: %s', response, extra=self.logger_extra)
         finally:
             if self.clean_workdir:
                 ftp.unlink(self.javascript_client_copy_filename, self.ftp_params)
 
         response = self.runscript_extra(response)
         return response
 
@@ -85,30 +94,30 @@
 class CloseAllDocuments(InDesignSoapScript):
     javascript_basename = "close_all_documents.jsx"
 
 
 class SaveAsBase(InDesignSoapScript):
     def __init__(self, src_name, dst_format, js_params, server_url, client_workdir, server_workdir,
                  server_path_style="posix", ftp_params=None, clean_workdir=True, logger=None, logger_extra=None):
-        super(SaveAsBase, self).__init__(server_url, client_workdir, server_workdir, server_path_style,
-                                         ftp_params, clean_workdir, logger, logger_extra)
+        super().__init__(server_url, client_workdir, server_workdir, server_path_style,
+                         ftp_params, clean_workdir, logger, logger_extra)
         self.js_params = js_params
         self.dst_format = dst_format
 
         self.src_name = src_name
         src_rootname = os.path.splitext(self.src_name)[0]
         self.set_dst_basename(src_rootname)
 
         self.response_client_copy_filename = os.path.join(self.client_workdir, self.dst_basename)
 
     def set_dst_basename(self, src_rootname):
-        self.dst_basename = "%sTMP.%s" % (src_rootname, self.dst_format)
+        self.dst_basename = f"{src_rootname}TMP.{self.dst_format}"
 
     def set_params(self):
-        super(SaveAsBase, self).set_params()
+        super().set_params()
 
         src_server_copy_filename = self.server_path_mod.join(self.server_workdir, self.src_name)
         src = self.client.factory.create("ns0:IDSP-ScriptArg")
         src.name = "source"
         src.value = src_server_copy_filename
 
         response_server_copy_filename = self.server_path_mod.join(self.server_workdir, self.dst_basename)
@@ -116,23 +125,23 @@
         dst.name = "destination"
         dst.value = response_server_copy_filename
 
         self.params.scriptArgs = [src, dst]
 
         # Extra parameters
         extra_params = []
-        for k, v in self.js_params.items():
+        for k, value in self.js_params.items():
             param = self.client.factory.create("ns0:IDSP-ScriptArg")
             param.name = k
-            param.value = v
+            param.value = value
             extra_params.append(param)
         self.params.scriptArgs.extend(extra_params)
 
     def runscript_extra(self, response):
-        response = super(SaveAsBase, self).runscript_extra(response)
+        response = super().runscript_extra(response)
         if response:
             response = ftp.read(self.response_client_copy_filename, self.ftp_params)
             if self.clean_workdir:
                 ftp.unlink(self.response_client_copy_filename, self.ftp_params)
         return response
 
 
@@ -140,15 +149,15 @@
     javascript_basename = "save_as.jsx"
 
 
 class Export(SaveAsBase):
     javascript_basename = "export.jsx"
 
     def set_params(self):
-        super(Export, self).set_params()
+        super().set_params()
         fmt = self.client.factory.create("ns0:IDSP-ScriptArg")
         fmt.name = "format"
         fmt.value = self.dst_format
         self.params.scriptArgs.append(fmt)
 
 
 class PackageForPrint(SaveAsBase):
@@ -156,19 +165,19 @@
 
     def set_dst_basename(self, src_rootname):
         self.dst_basename = src_rootname  # A directory
 
     def runscript_extra(self, response):
         # Zip the tree generated in response_client_copy_filename and
         # make that variable point on that zip file.
-        zip_filename = "%s.zip" % self.response_client_copy_filename
+        zip_filename = f"{self.response_client_copy_filename}.zip"
         ftp.zip_dir(self.response_client_copy_filename, zip_filename, self.ftp_params)
         self.response_client_copy_filename = zip_filename
 
-        return super(PackageForPrint, self).runscript_extra(response)
+        return super().runscript_extra(response)
 
 
 @simple_decorator
 def use_dedicated_working_directory(view_func):
     def new_func(src_path, formats_options, indesign_server_url, indesign_client_workdir,
                  indesign_server_workdir, indesign_server_path_style="posix",
                  clean_workdir=True, ftp_params=None, logger=None, logger_extra=None):
@@ -185,16 +194,16 @@
         indesign_server_workdir = server_path_mod.join(indesign_server_workdir, os.path.basename(working_dir))
 
         try:
             response = view_func(src_path, formats_options, indesign_server_url,
                                  indesign_client_workdir, indesign_server_workdir,
                                  indesign_server_path_style, clean_workdir, ftp_params,
                                  logger, logger_extra)
-        except BaseException as e:
-            raise e
+        except BaseException as exc:
+            raise exc
         finally:
             if clean_workdir:
                 ftp.rmtree(working_dir, ftp_params)
         return response
     return new_func
```

### Comparing `SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/export.jsx` & `SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/export.jsx`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/package_to_print.jsx` & `SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/package_to_print.jsx`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/src/simple_idml/indesign/scripts/save_as.jsx` & `SimpleIDML-1.1.6a1/src/simple_idml/indesign/scripts/save_as.jsx`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/src/simple_idml/test.py` & `SimpleIDML-1.1.6a1/src/simple_idml/test.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/src/simple_idml/utils.py` & `SimpleIDML-1.1.6a1/src/simple_idml/utils.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/MasterSpreads/MasterSpread_ua5.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml`

 * *Files 5% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/MasterSpreads/MasterSpread_ua5.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/MasterSpreads/MasterSpread_ua5.xml`

```diff
@@ -1,25 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:MasterSpread xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
   <MasterSpread Self="ua5" ItemTransform="1 0 0 1 0 0" OverriddenPageItemProps="" Name="A-Master" NamePrefix="A" BaseName="Master" ShowMasterItems="true" PageCount="2" PrimaryTextFrame="n">
     <Properties>
       <PageColor type="enumeration">UseMasterColor</PageColor>
     </Properties>
-    <Page Self="myprefixuaa" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 -566.9291338582677 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
+    <Page Self="uaa" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 -566.9291338582677 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
       <Properties>
         <PageColor type="enumeration">UseMasterColor</PageColor>
       </Properties>
       <MarginPreference ColumnCount="1" ColumnGutter="12" Top="36" Bottom="36" Left="36" Right="36" ColumnDirection="Horizontal" ColumnsPositions="0 494.92913385826773"/>
       <GridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100" LineAlignment="LeftOrTopLineJustify" GridAlignment="AlignEmCenter" CharacterAlignment="AlignEmCenter">
         <Properties>
           <AppliedFont type="string">Minion Pro</AppliedFont>
         </Properties>
       </GridDataInformation>
     </Page>
-    <Page Self="myprefixuab" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
+    <Page Self="uab" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
       <Properties>
         <PageColor type="enumeration">UseMasterColor</PageColor>
       </Properties>
       <MarginPreference ColumnCount="1" ColumnGutter="12" Top="36" Bottom="36" Left="36" Right="36" ColumnDirection="Horizontal" ColumnsPositions="0 494.92913385826773"/>
       <GridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100" LineAlignment="LeftOrTopLineJustify" GridAlignment="AlignEmCenter" CharacterAlignment="AlignEmCenter">
         <Properties>
           <AppliedFont type="string">Minion Pro</AppliedFont>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Fonts.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml`

 * *Files 9% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Fonts.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Fonts.xml`

```diff
@@ -1,67 +1,67 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Fonts xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <FontFamily Self="myprefixdi38" Name="Minion Pro">
-    <Font Self="myprefixdi38FontnMinion Pro Bold Cond" FontFamily="Minion Pro" Name="Minion Pro Bold Cond" PostScriptName="MinionPro-BoldCn" Status="Installed" FontStyleName="Bold Cond" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond" FullNameNative="Minion Pro Bold Cond" FontStyleNameNative="Bold Cond" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Bold Cond Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Cond Italic" PostScriptName="MinionPro-BoldCnIt" Status="Installed" FontStyleName="Bold Cond Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond Italic" FullNameNative="Minion Pro Bold Cond Italic" FontStyleNameNative="Bold Cond Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Regular" FontFamily="Minion Pro" Name="Minion Pro Regular" PostScriptName="MinionPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro" FullNameNative="Minion Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Italic" FontFamily="Minion Pro" Name="Minion Pro Italic" PostScriptName="MinionPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Italic" FullNameNative="Minion Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Medium" FontFamily="Minion Pro" Name="Minion Pro Medium" PostScriptName="MinionPro-Medium" Status="Installed" FontStyleName="Medium" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium" FullNameNative="Minion Pro Medium" FontStyleNameNative="Medium" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Medium Italic" FontFamily="Minion Pro" Name="Minion Pro Medium Italic" PostScriptName="MinionPro-MediumIt" Status="Installed" FontStyleName="Medium Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium Italic" FullNameNative="Minion Pro Medium Italic" FontStyleNameNative="Medium Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Semibold" FontFamily="Minion Pro" Name="Minion Pro Semibold" PostScriptName="MinionPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold" FullNameNative="Minion Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Semibold Italic" FontFamily="Minion Pro" Name="Minion Pro Semibold Italic" PostScriptName="MinionPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold Italic" FullNameNative="Minion Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Bold" FontFamily="Minion Pro" Name="Minion Pro Bold" PostScriptName="MinionPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold" FullNameNative="Minion Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Bold Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Italic" PostScriptName="MinionPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Italic" FullNameNative="Minion Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+  <FontFamily Self="di38" Name="Minion Pro">
+    <Font Self="di38FontnMinion Pro Bold Cond" FontFamily="Minion Pro" Name="Minion Pro Bold Cond" PostScriptName="MinionPro-BoldCn" Status="Installed" FontStyleName="Bold Cond" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond" FullNameNative="Minion Pro Bold Cond" FontStyleNameNative="Bold Cond" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Bold Cond Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Cond Italic" PostScriptName="MinionPro-BoldCnIt" Status="Installed" FontStyleName="Bold Cond Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond Italic" FullNameNative="Minion Pro Bold Cond Italic" FontStyleNameNative="Bold Cond Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Regular" FontFamily="Minion Pro" Name="Minion Pro Regular" PostScriptName="MinionPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro" FullNameNative="Minion Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Italic" FontFamily="Minion Pro" Name="Minion Pro Italic" PostScriptName="MinionPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Italic" FullNameNative="Minion Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Medium" FontFamily="Minion Pro" Name="Minion Pro Medium" PostScriptName="MinionPro-Medium" Status="Installed" FontStyleName="Medium" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium" FullNameNative="Minion Pro Medium" FontStyleNameNative="Medium" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Medium Italic" FontFamily="Minion Pro" Name="Minion Pro Medium Italic" PostScriptName="MinionPro-MediumIt" Status="Installed" FontStyleName="Medium Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium Italic" FullNameNative="Minion Pro Medium Italic" FontStyleNameNative="Medium Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Semibold" FontFamily="Minion Pro" Name="Minion Pro Semibold" PostScriptName="MinionPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold" FullNameNative="Minion Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Semibold Italic" FontFamily="Minion Pro" Name="Minion Pro Semibold Italic" PostScriptName="MinionPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold Italic" FullNameNative="Minion Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Bold" FontFamily="Minion Pro" Name="Minion Pro Bold" PostScriptName="MinionPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold" FullNameNative="Minion Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Bold Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Italic" PostScriptName="MinionPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Italic" FullNameNative="Minion Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
   </FontFamily>
-  <FontFamily Self="myprefixdi79" Name="Myriad Pro">
-    <Font Self="myprefixdi79FontnMyriad Pro Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Condensed" PostScriptName="MyriadPro-Cond" Status="Installed" FontStyleName="Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed" FullNameNative="Myriad Pro Condensed" FontStyleNameNative="Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Condensed Italic" PostScriptName="MyriadPro-CondIt" Status="Installed" FontStyleName="Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed Italic" FullNameNative="Myriad Pro Condensed Italic" FontStyleNameNative="Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed" PostScriptName="MyriadPro-BoldCond" Status="Installed" FontStyleName="Bold Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed" FullNameNative="Myriad Pro Bold Condensed" FontStyleNameNative="Bold Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed Italic" PostScriptName="MyriadPro-BoldCondIt" Status="Installed" FontStyleName="Bold Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed Italic" FullNameNative="Myriad Pro Bold Condensed Italic" FontStyleNameNative="Bold Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Regular" FontFamily="Myriad Pro" Name="Myriad Pro Regular" PostScriptName="MyriadPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro" FullNameNative="Myriad Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Italic" FontFamily="Myriad Pro" Name="Myriad Pro Italic" PostScriptName="MyriadPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Italic" FullNameNative="Myriad Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Semibold" FontFamily="Myriad Pro" Name="Myriad Pro Semibold" PostScriptName="MyriadPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold" FullNameNative="Myriad Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Semibold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Semibold Italic" PostScriptName="MyriadPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold Italic" FullNameNative="Myriad Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold" FontFamily="Myriad Pro" Name="Myriad Pro Bold" PostScriptName="MyriadPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold" FullNameNative="Myriad Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Italic" PostScriptName="MyriadPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Italic" FullNameNative="Myriad Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+  <FontFamily Self="di79" Name="Myriad Pro">
+    <Font Self="di79FontnMyriad Pro Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Condensed" PostScriptName="MyriadPro-Cond" Status="Installed" FontStyleName="Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed" FullNameNative="Myriad Pro Condensed" FontStyleNameNative="Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Condensed Italic" PostScriptName="MyriadPro-CondIt" Status="Installed" FontStyleName="Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed Italic" FullNameNative="Myriad Pro Condensed Italic" FontStyleNameNative="Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed" PostScriptName="MyriadPro-BoldCond" Status="Installed" FontStyleName="Bold Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed" FullNameNative="Myriad Pro Bold Condensed" FontStyleNameNative="Bold Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed Italic" PostScriptName="MyriadPro-BoldCondIt" Status="Installed" FontStyleName="Bold Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed Italic" FullNameNative="Myriad Pro Bold Condensed Italic" FontStyleNameNative="Bold Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Regular" FontFamily="Myriad Pro" Name="Myriad Pro Regular" PostScriptName="MyriadPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro" FullNameNative="Myriad Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Italic" FontFamily="Myriad Pro" Name="Myriad Pro Italic" PostScriptName="MyriadPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Italic" FullNameNative="Myriad Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Semibold" FontFamily="Myriad Pro" Name="Myriad Pro Semibold" PostScriptName="MyriadPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold" FullNameNative="Myriad Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Semibold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Semibold Italic" PostScriptName="MyriadPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold Italic" FullNameNative="Myriad Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold" FontFamily="Myriad Pro" Name="Myriad Pro Bold" PostScriptName="MyriadPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold" FullNameNative="Myriad Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Italic" PostScriptName="MyriadPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Italic" FullNameNative="Myriad Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
   </FontFamily>
-  <FontFamily Self="myprefixdi7d" Name="Kozuka Mincho Pro">
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro EL" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro EL" PostScriptName="KozMinPro-ExtraLight" Status="Installed" FontStyleName="EL" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro EL" FullNameNative="小塚明朝 Pro EL" FontStyleNameNative="EL" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro L" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro L" PostScriptName="KozMinPro-Light" Status="Installed" FontStyleName="L" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro L" FullNameNative="小塚明朝 Pro L" FontStyleNameNative="L" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro R" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro R" PostScriptName="KozMinPro-Regular" Status="Installed" FontStyleName="R" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro R" FullNameNative="小塚明朝 Pro R" FontStyleNameNative="R" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro M" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro M" PostScriptName="KozMinPro-Medium" Status="Installed" FontStyleName="M" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro M" FullNameNative="小塚明朝 Pro M" FontStyleNameNative="M" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro B" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro B" PostScriptName="KozMinPro-Bold" Status="Installed" FontStyleName="B" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro B" FullNameNative="小塚明朝 Pro B" FontStyleNameNative="B" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro H" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro H" PostScriptName="KozMinPro-Heavy" Status="Installed" FontStyleName="H" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro H" FullNameNative="小塚明朝 Pro H" FontStyleNameNative="H" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+  <FontFamily Self="di7d" Name="Kozuka Mincho Pro">
+    <Font Self="di7dFontnKozuka Mincho Pro EL" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro EL" PostScriptName="KozMinPro-ExtraLight" Status="Installed" FontStyleName="EL" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro EL" FullNameNative="小塚明朝 Pro EL" FontStyleNameNative="EL" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro L" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro L" PostScriptName="KozMinPro-Light" Status="Installed" FontStyleName="L" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro L" FullNameNative="小塚明朝 Pro L" FontStyleNameNative="L" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro R" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro R" PostScriptName="KozMinPro-Regular" Status="Installed" FontStyleName="R" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro R" FullNameNative="小塚明朝 Pro R" FontStyleNameNative="R" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro M" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro M" PostScriptName="KozMinPro-Medium" Status="Installed" FontStyleName="M" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro M" FullNameNative="小塚明朝 Pro M" FontStyleNameNative="M" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro B" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro B" PostScriptName="KozMinPro-Bold" Status="Installed" FontStyleName="B" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro B" FullNameNative="小塚明朝 Pro B" FontStyleNameNative="B" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro H" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro H" PostScriptName="KozMinPro-Heavy" Status="Installed" FontStyleName="H" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro H" FullNameNative="小塚明朝 Pro H" FontStyleNameNative="H" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
   </FontFamily>
-  <CompositeFont Self="myprefixCompositeFont/$ID/[No composite font]" Name="$ID/[No composite font]">
-    <CompositeFontEntry Self="myprefixu7c" Name="$ID/Kanji" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" Locked="true" ScaleOption="true" BaselineShift="0">
+  <CompositeFont Self="CompositeFont/$ID/[No composite font]" Name="$ID/[No composite font]">
+    <CompositeFontEntry Self="u7c" Name="$ID/Kanji" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu7e" Name="$ID/Kana" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="ぁあぃいぅうぇえぉおかがきぎくぐけげこごさざしじすずせぜそぞただちぢっつづてでとどなにぬねのはばぱひびぴふぶぷへべぺほぼぽまみむめもゃやゅゆょよらりるれろゎわゐゑをんゔゕゖゝゞァアィイゥウェエォオカガキギクグケゲコゴサザシジスズセゼソゾタダチヂッツヅテデトドナニヌネノハバパヒビピフブプヘベペホボポマミムメモャヤュユョヨラリルレロヮワヰヱヲンヴヵヶヷヸヹヺーヽヾ" Locked="true" ScaleOption="true" BaselineShift="0">
+    <CompositeFontEntry Self="u7e" Name="$ID/Kana" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="ぁあぃいぅうぇえぉおかがきぎくぐけげこごさざしじすずせぜそぞただちぢっつづてでとどなにぬねのはばぱひびぴふぶぷへべぺほぼぽまみむめもゃやゅゆょよらりるれろゎわゐゑをんゔゕゖゝゞァアィイゥウェエォオカガキギクグケゲコゴサザシジスズセゼソゾタダチヂッツヅテデトドナニヌネノハバパヒビピフブプヘベペホボポマミムメモャヤュユョヨラリルレロヮワヰヱヲンヴヵヶヷヸヹヺーヽヾ" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu7f" Name="$ID/Punctuation" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="—―‖‘’“”‥…′″∥、。〈〉《》「」『』【】〔〕〜・！（），．／：；？［］｛｝～" Locked="true" ScaleOption="true" BaselineShift="0">
+    <CompositeFontEntry Self="u7f" Name="$ID/Punctuation" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="—―‖‘’“”‥…′″∥、。〈〉《》「」『』【】〔〕〜・！（），．／：；？［］｛｝～" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu80" Name="$ID/Symbols" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="¢£§¨¬°±´¶×÷ΑΒΓΔΕΖΗΘΙΚΛΜΝΞΟΠΡΣΤΥΦΧΨΩαβγδεζηθικλμνξοπρστυφχψωЁАБВГДЕЖЗИЙКЛМНОПРСТУФХЦЧШЩЪЫЬЭЮЯабвгдежзийклмнопрстуфхцчшщъыьэюяё‐†‡‰※℃Å←↑→↓⇒⇔∀∂∃∇∈∋−√∝∞∠∧∨∩∪∫∬∴∵∽≒≠≡≦≧≪≫⊂⊃⊆⊇⊥⌒■□▲△▼▽◆◇○◎●◯★☆♀♂♪♭♯〃〆〇〒〓゛゜＃＄％＆＊＋－０１２３４５６７８９＜＝＞＠ＡＢＣＤＥＦＧＨＩＪＫＬＭＮＯＰＱＲＳＴＵＶＷＸＹＺ＼＾＿｀ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ｜￠￡￢￣￥" Locked="true" ScaleOption="true" BaselineShift="0">
+    <CompositeFontEntry Self="u80" Name="$ID/Symbols" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="¢£§¨¬°±´¶×÷ΑΒΓΔΕΖΗΘΙΚΛΜΝΞΟΠΡΣΤΥΦΧΨΩαβγδεζηθικλμνξοπρστυφχψωЁАБВГДЕЖЗИЙКЛМНОПРСТУФХЦЧШЩЪЫЬЭЮЯабвгдежзийклмнопрстуфхцчшщъыьэюяё‐†‡‰※℃Å←↑→↓⇒⇔∀∂∃∇∈∋−√∝∞∠∧∨∩∪∫∬∴∵∽≒≠≡≦≧≪≫⊂⊃⊆⊇⊥⌒■□▲△▼▽◆◇○◎●◯★☆♀♂♪♭♯〃〆〇〒〓゛゜＃＄％＆＊＋－０１２３４５６７８９＜＝＞＠ＡＢＣＤＥＦＧＨＩＪＫＬＭＮＯＰＱＲＳＴＵＶＷＸＹＺ＼＾＿｀ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ｜￠￡￢￣￥" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu81" Name="$ID/Alphabetic" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters=" !&quot;#$%&amp;'()*+,-./:;&lt;=&gt;?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~ ¡¤¥¦©ª«­®¯²³µ·¸¹º»¼½¾¿ÀÁÂÃÄÅÆÇÈÉÊËÌÍÎÏÐÑÒÓÔÕÖØÙÚÛÜÝÞßàáâãäåæçèéêëìíîïðñòóôõöøùúûüýþÿıŒœŠšŸŽžƒˆˇ˘˙˚˛˜˝–‚„•‹›⁄€™∆∏∑≈≤≥◊ﬀﬁﬂﬃﬄﬅﬆ" Locked="true" ScaleOption="false" BaselineShift="0">
+    <CompositeFontEntry Self="u81" Name="$ID/Alphabetic" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters=" !&quot;#$%&amp;'()*+,-./:;&lt;=&gt;?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~ ¡¤¥¦©ª«­®¯²³µ·¸¹º»¼½¾¿ÀÁÂÃÄÅÆÇÈÉÊËÌÍÎÏÐÑÒÓÔÕÖØÙÚÛÜÝÞßàáâãäåæçèéêëìíîïðñòóôõöøùúûüýþÿıŒœŠšŸŽžƒˆˇ˘˙˚˛˜˝–‚„•‹›⁄€™∆∏∑≈≤≥◊ﬀﬁﬂﬃﬄﬅﬆ" Locked="true" ScaleOption="false" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Minion Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu82" Name="$ID/Numbers" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="0123456789" Locked="true" ScaleOption="false" BaselineShift="0">
+    <CompositeFontEntry Self="u82" Name="$ID/Numbers" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="0123456789" Locked="true" ScaleOption="false" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Minion Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
   </CompositeFont>
 </idPkg:Fonts>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Graphic.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml`

 * *Files 18% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Graphic.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Graphic.xml`

```diff
@@ -1,50 +1,50 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Graphic xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Color Self="myprefixColor/Black" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Specialblack" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Black" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=0 M=0 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=0 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=0 M=100 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=100 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=100 M=0 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=0 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=100 M=90 Y=10 K=0" Model="Process" Space="CMYK" ColorValue="100 90 10 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=90 Y=10 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=15 M=100 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="15 100 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=15 M=100 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=75 M=5 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="75 5 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=75 M=5 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Cyan" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Cyan" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Magenta" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Magenta" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Paper" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Specialpaper" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Paper" ColorEditable="true" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Registration" Model="Registration" Space="CMYK" ColorValue="100 100 100 100" ColorOverride="Specialregistration" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Registration" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Yellow" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Yellow" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/u70" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/u72" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/uba" Model="Process" Space="CMYK" ColorValue="11 95 100 2" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
-  <Ink Self="myprefixInk/$ID/Process Cyan" Name="$ID/Process Cyan" Angle="75" ConvertToProcess="false" Frequency="70" NeutralDensity="0.61" PrintInk="true" TrapOrder="1" InkType="Normal"/>
-  <Ink Self="myprefixInk/$ID/Process Magenta" Name="$ID/Process Magenta" Angle="15" ConvertToProcess="false" Frequency="70" NeutralDensity="0.76" PrintInk="true" TrapOrder="2" InkType="Normal"/>
-  <Ink Self="myprefixInk/$ID/Process Yellow" Name="$ID/Process Yellow" Angle="0" ConvertToProcess="false" Frequency="70" NeutralDensity="0.16" PrintInk="true" TrapOrder="3" InkType="Normal"/>
-  <Ink Self="myprefixInk/$ID/Process Black" Name="$ID/Process Black" Angle="45" ConvertToProcess="false" Frequency="70" NeutralDensity="1.7" PrintInk="true" TrapOrder="4" InkType="Normal"/>
-  <PastedSmoothShade Self="myprefixPastedSmoothShade/u6f" ContentsVersion="0" ContentsType="ConstantShade" SpotColorList="" ContentsEncoding="Ascii64Encoding" ContentsMatrix="1 0 0 1 0 0" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
+  <Color Self="Color/Black" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Specialblack" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Black" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=0 M=0 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=0 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=0 M=100 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=100 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=100 M=0 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=0 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=100 M=90 Y=10 K=0" Model="Process" Space="CMYK" ColorValue="100 90 10 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=90 Y=10 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=15 M=100 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="15 100 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=15 M=100 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=75 M=5 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="75 5 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=75 M=5 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/Cyan" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Cyan" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/Magenta" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Magenta" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/Paper" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Specialpaper" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Paper" ColorEditable="true" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/Registration" Model="Registration" Space="CMYK" ColorValue="100 100 100 100" ColorOverride="Specialregistration" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Registration" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/Yellow" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Yellow" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/u70" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/u72" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/u1b4" Model="Process" Space="CMYK" ColorValue="11 95 100 2" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
+  <Ink Self="Ink/$ID/Process Cyan" Name="$ID/Process Cyan" Angle="75" ConvertToProcess="false" Frequency="70" NeutralDensity="0.61" PrintInk="true" TrapOrder="1" InkType="Normal"/>
+  <Ink Self="Ink/$ID/Process Magenta" Name="$ID/Process Magenta" Angle="15" ConvertToProcess="false" Frequency="70" NeutralDensity="0.76" PrintInk="true" TrapOrder="2" InkType="Normal"/>
+  <Ink Self="Ink/$ID/Process Yellow" Name="$ID/Process Yellow" Angle="0" ConvertToProcess="false" Frequency="70" NeutralDensity="0.16" PrintInk="true" TrapOrder="3" InkType="Normal"/>
+  <Ink Self="Ink/$ID/Process Black" Name="$ID/Process Black" Angle="45" ConvertToProcess="false" Frequency="70" NeutralDensity="1.7" PrintInk="true" TrapOrder="4" InkType="Normal"/>
+  <PastedSmoothShade Self="PastedSmoothShade/u6f" ContentsVersion="0" ContentsType="ConstantShade" SpotColorList="" ContentsEncoding="Ascii64Encoding" ContentsMatrix="1 0 0 1 0 0" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
     <Properties>
-      <Contents>AAAAAUBv4AAAAAAAAAAAAAAAAAAAAAAAAAAAAA==</Contents>
+      <Contents><![CDATA[AAAAAUBv4AAAAAAAAAAAAAAAAAAAAAAAAAAAAA==]]></Contents>
     </Properties>
   </PastedSmoothShade>
-  <Swatch Self="myprefixSwatch/None" Name="None" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Gradient Self="myprefixGradient/u71" Type="Linear" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
-    <GradientStop Self="myprefixu71GradientStop0" StopColor="Color/u70" Location="0"/>
-    <GradientStop Self="myprefixu71GradientStop1" StopColor="Color/Black" Location="100" Midpoint="50"/>
+  <Swatch Self="Swatch/None" Name="None" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Gradient Self="Gradient/u71" Type="Linear" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
+    <GradientStop Self="u71GradientStop0" StopColor="Color/u70" Location="0"/>
+    <GradientStop Self="u71GradientStop1" StopColor="Color/Black" Location="100" Midpoint="50"/>
   </Gradient>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Triple_Stroke" Name="$ID/Triple_Stroke"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThickThinThick" Name="$ID/ThickThinThick"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThinThickThin" Name="$ID/ThinThickThin"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThickThick" Name="$ID/ThickThick"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThickThin" Name="$ID/ThickThin"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThinThick" Name="$ID/ThinThick"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThinThin" Name="$ID/ThinThin"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Japanese Dots" Name="$ID/Japanese Dots"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/White Diamond" Name="$ID/White Diamond"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Left Slant Hash" Name="$ID/Left Slant Hash"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Right Slant Hash" Name="$ID/Right Slant Hash"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Straight Hash" Name="$ID/Straight Hash"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Wavy" Name="$ID/Wavy"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Canned Dotted" Name="$ID/Canned Dotted"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Canned Dashed 3x2" Name="$ID/Canned Dashed 3x2"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Canned Dashed 4x4" Name="$ID/Canned Dashed 4x4"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Dashed" Name="$ID/Dashed"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Solid" Name="$ID/Solid"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Triple_Stroke" Name="$ID/Triple_Stroke"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThickThinThick" Name="$ID/ThickThinThick"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThinThickThin" Name="$ID/ThinThickThin"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThickThick" Name="$ID/ThickThick"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThickThin" Name="$ID/ThickThin"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThinThick" Name="$ID/ThinThick"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThinThin" Name="$ID/ThinThin"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Japanese Dots" Name="$ID/Japanese Dots"/>
+  <StrokeStyle Self="StrokeStyle/$ID/White Diamond" Name="$ID/White Diamond"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Left Slant Hash" Name="$ID/Left Slant Hash"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Right Slant Hash" Name="$ID/Right Slant Hash"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Straight Hash" Name="$ID/Straight Hash"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Wavy" Name="$ID/Wavy"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Canned Dotted" Name="$ID/Canned Dotted"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Canned Dashed 3x2" Name="$ID/Canned Dashed 3x2"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Canned Dashed 4x4" Name="$ID/Canned Dashed 4x4"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Dashed" Name="$ID/Dashed"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Solid" Name="$ID/Solid"/>
 </idPkg:Graphic>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Preferences.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml`

 * *Files 9% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Preferences.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Preferences.xml`

```diff
@@ -79,15 +79,15 @@
         <ListItem type="unit">0</ListItem>
         <ListItem type="unit">0</ListItem>
         <ListItem type="unit">0</ListItem>
       </InsetSpacing>
     </Properties>
   </TextFramePreference>
   <TextPreference TypographersQuotes="true" HighlightHjViolations="false" HighlightKeeps="false" HighlightSubstitutedGlyphs="false" HighlightCustomSpacing="false" HighlightSubstitutedFonts="true" UseOpticalSize="true" UseParagraphLeading="false" SuperscriptSize="58.3" SuperscriptPosition="33.3" SubscriptSize="58.3" SubscriptPosition="33.3" SmallCap="70" LeadingKeyIncrement="2" BaselineShiftKeyIncrement="2" KerningKeyIncrement="20" ShowInvisibles="false" JustifyTextWraps="false" AbutTextToTextWrap="true" ZOrderTextWrap="false" LinkTextFilesWhenImporting="false" HighlightKinsoku="false" QuoteCharactersRotatedInVertical="false" UseNewVerticalScaling="false" UseCidMojikumi="false" EnableStylePreviewMode="false" SmartTextReflow="true" AddPages="EndOfStory" LimitToMasterTextFrames="true" PreserveFacingPageSpreads="false" DeleteEmptyPages="false"/>
-  <TextDefault FontStyle="Italic" PointSize="12" KerningMethod="$ID/Metrics" Tracking="0" Capitalization="Normal" Position="Superscript" Underline="false" StrikeThru="false" Ligatures="true" NoBreak="false" HorizontalScale="100" VerticalScale="100" BaselineShift="0" Skew="0" FillTint="-1" StrokeTint="-1" StrokeWeight="1" OverprintStroke="false" OverprintFill="false" OTFFigureStyle="Default" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" OTFContextualAlternate="true" OTFSwash="false" UnderlineTint="-1" UnderlineGapTint="-1" UnderlineOverprint="false" UnderlineGapOverprint="false" UnderlineOffset="-9999" UnderlineWeight="-9999" StrikeThroughTint="-1" StrikeThroughGapTint="-1" StrikeThroughOverprint="false" StrikeThroughGapOverprint="false" StrikeThroughOffset="-9999" StrikeThroughWeight="-9999" FillColor="myprefixColor/Black" StrokeColor="myprefixSwatch/None" AppliedLanguage="$ID/English: UK" ParagraphKashidaWidth="2" FirstLineIndent="0" LeftIndent="0" RightIndent="0" SpaceBefore="0" SpaceAfter="0" Justification="LeftAlign" SingleWordJustification="FullyJustified" AutoLeading="120" DropCapLines="0" DropCapCharacters="0" KeepLinesTogether="false" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" StartParagraph="Anywhere" Composer="HL Composer" MinimumWordSpacing="80" MaximumWordSpacing="133" DesiredWordSpacing="100" MinimumLetterSpacing="0" MaximumLetterSpacing="0" DesiredLetterSpacing="0" MinimumGlyphScaling="100" MaximumGlyphScaling="100" DesiredGlyphScaling="100" RuleAbove="false" RuleAboveOverprint="false" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelow="false" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleBelowGapTint="-1" HyphenateCapitalizedWords="true" Hyphenation="true" HyphenateBeforeLast="2" HyphenateAfterFirst="2" HyphenateWordsLongerThan="5" HyphenateLadderLimit="3" HyphenationZone="36" HyphenWeight="5" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" AppliedCharacterStyle="myprefixCharacterStyle/sup" LastLineIndent="0" HyphenateLastWord="true" OTFSlashedZero="false" OTFHistorical="false" OTFStylisticSets="0" GradientFillLength="-1" GradientFillAngle="0" GradientStrokeLength="-1" GradientStrokeAngle="0" GradientFillStart="0 0" GradientStrokeStart="0 0" KeepWithPrevious="false" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" RuleBelowOverprint="false" RuleBelowGapOverprint="false" DropcapDetail="1" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFMark="true" OTFLocale="true" PositionalForm="None" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" CharacterDirection="DefaultDirection" KeyboardDirection="DefaultDirection" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" XOffsetDiacritic="0" YOffsetDiacritic="0" ParagraphBreakType="Anywhere" PageNumberType="AutoPageNumber" AppliedNamedGrid="n" GridAlignFirstLineOnly="false" GridAlignment="None" GridGyoudori="0" AutoTcy="0" AutoTcyIncludeRoman="false" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" Rensuuji="true" RotateSingleByteCharacters="false" LeadingModel="LeadingModelAkiBelow" CharacterAlignment="AlignEmCenter" Tsume="0" LeadingAki="-1" TrailingAki="-1" CharacterRotation="0" Jidori="0" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustRotation="false" ShataiAdjustTsume="true" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" KentenTint="-1" KentenStrokeTint="-1" KentenWeight="-1" KentenOverprintFill="Auto" KentenOverprintStroke="Auto" KentenKind="None" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" RubyTint="-1" RubyWeight="-1" RubyOverprintFill="Auto" RubyOverprintStroke="Auto" RubyStrokeTint="-1" RubyFontSize="-1" RubyOpenTypePro="true" RubyXScale="100" RubyYScale="100" RubyType="PerCharacterRuby" RubyAlignment="RubyJIS" RubyPosition="AboveRight" RubyXOffset="0" RubyYOffset="0" RubyParentSpacing="RubyParent121Aki" RubyAutoAlign="true" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyParentOverhangAmount="RubyOverhangOneRuby" Warichu="false" WarichuSize="50" WarichuLines="2" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsAfterBreak="2" WarichuCharsBeforeBreak="2" OTFProportionalMetrics="false" OTFHVKana="false" OTFRomanItalics="false" ScaleAffectsLineHeight="false" CjkGridTracking="false" GlyphForm="None" ParagraphGyoudori="false" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingExpression="^#.^t" BulletsTextAfter="^t" NumberingLevel="1" NumberingContinue="true" NumberingStartAt="1" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign">
+  <TextDefault FontStyle="Bold" PointSize="12" KerningMethod="$ID/Metrics" Tracking="0" Capitalization="Normal" Position="Normal" Underline="false" StrikeThru="false" Ligatures="true" NoBreak="false" HorizontalScale="100" VerticalScale="100" BaselineShift="0" Skew="0" FillTint="-1" StrokeTint="-1" StrokeWeight="1" OverprintStroke="false" OverprintFill="false" OTFFigureStyle="Default" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" OTFContextualAlternate="true" OTFSwash="false" UnderlineTint="-1" UnderlineGapTint="-1" UnderlineOverprint="false" UnderlineGapOverprint="false" UnderlineOffset="-9999" UnderlineWeight="-9999" StrikeThroughTint="-1" StrikeThroughGapTint="-1" StrikeThroughOverprint="false" StrikeThroughGapOverprint="false" StrikeThroughOffset="-9999" StrikeThroughWeight="-9999" FillColor="Color/Black" StrokeColor="Swatch/None" AppliedLanguage="$ID/English: UK" ParagraphKashidaWidth="2" FirstLineIndent="0" LeftIndent="0" RightIndent="0" SpaceBefore="0" SpaceAfter="0" Justification="LeftAlign" SingleWordJustification="FullyJustified" AutoLeading="120" DropCapLines="0" DropCapCharacters="0" KeepLinesTogether="false" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" StartParagraph="Anywhere" Composer="HL Composer" MinimumWordSpacing="80" MaximumWordSpacing="133" DesiredWordSpacing="100" MinimumLetterSpacing="0" MaximumLetterSpacing="0" DesiredLetterSpacing="0" MinimumGlyphScaling="100" MaximumGlyphScaling="100" DesiredGlyphScaling="100" RuleAbove="false" RuleAboveOverprint="false" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelow="false" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleBelowGapTint="-1" HyphenateCapitalizedWords="true" Hyphenation="true" HyphenateBeforeLast="2" HyphenateAfterFirst="2" HyphenateWordsLongerThan="5" HyphenateLadderLimit="3" HyphenationZone="36" HyphenWeight="5" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" AppliedCharacterStyle="CharacterStyle/MyBoldStyle" LastLineIndent="0" HyphenateLastWord="true" OTFSlashedZero="false" OTFHistorical="false" OTFStylisticSets="0" GradientFillLength="-1" GradientFillAngle="0" GradientStrokeLength="-1" GradientStrokeAngle="0" GradientFillStart="0 0" GradientStrokeStart="0 0" KeepWithPrevious="false" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" RuleBelowOverprint="false" RuleBelowGapOverprint="false" DropcapDetail="1" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFMark="true" OTFLocale="true" PositionalForm="None" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" CharacterDirection="DefaultDirection" KeyboardDirection="DefaultDirection" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" XOffsetDiacritic="0" YOffsetDiacritic="0" ParagraphBreakType="Anywhere" PageNumberType="AutoPageNumber" AppliedNamedGrid="n" GridAlignFirstLineOnly="false" GridAlignment="None" GridGyoudori="0" AutoTcy="0" AutoTcyIncludeRoman="false" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" Rensuuji="true" RotateSingleByteCharacters="false" LeadingModel="LeadingModelAkiBelow" CharacterAlignment="AlignEmCenter" Tsume="0" LeadingAki="-1" TrailingAki="-1" CharacterRotation="0" Jidori="0" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustRotation="false" ShataiAdjustTsume="true" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" KentenTint="-1" KentenStrokeTint="-1" KentenWeight="-1" KentenOverprintFill="Auto" KentenOverprintStroke="Auto" KentenKind="None" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" RubyTint="-1" RubyWeight="-1" RubyOverprintFill="Auto" RubyOverprintStroke="Auto" RubyStrokeTint="-1" RubyFontSize="-1" RubyOpenTypePro="true" RubyXScale="100" RubyYScale="100" RubyType="PerCharacterRuby" RubyAlignment="RubyJIS" RubyPosition="AboveRight" RubyXOffset="0" RubyYOffset="0" RubyParentSpacing="RubyParent121Aki" RubyAutoAlign="true" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyParentOverhangAmount="RubyOverhangOneRuby" Warichu="false" WarichuSize="50" WarichuLines="2" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsAfterBreak="2" WarichuCharsBeforeBreak="2" OTFProportionalMetrics="false" OTFHVKana="false" OTFRomanItalics="false" ScaleAffectsLineHeight="false" CjkGridTracking="false" GlyphForm="None" ParagraphGyoudori="false" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingExpression="^#.^t" BulletsTextAfter="^t" NumberingLevel="1" NumberingContinue="true" NumberingStartAt="1" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign">
     <Properties>
       <AppliedFont type="string">Minion Pro</AppliedFont>
       <Leading type="enumeration">Auto</Leading>
       <UnderlineColor type="string">Text Color</UnderlineColor>
       <UnderlineGapColor type="object">Swatch/None</UnderlineGapColor>
       <UnderlineType type="object">StrokeStyle/$ID/Solid</UnderlineType>
       <StrikeThroughColor type="string">Text Color</StrikeThroughColor>
@@ -647,20 +647,20 @@
             <SectionHeaderType SortingHeaderString="$ID/Y" DocumentHeaderString="$ID/" UIHeaderString="$ID/kIndexSection_Y" Language="256"/>
             <SectionHeaderType SortingHeaderString="$ID/Z" DocumentHeaderString="$ID/" UIHeaderString="$ID/kIndexSection_Z" Language="256"/>
           </SectionHeaderArray>
         </IndexHeaderGroupType>
       </ListOfIndexHeaderGroup>
     </Properties>
   </IndexHeaderSetting>
-  <PageItemDefault TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" AppliedGraphicObjectStyle="ObjectStyle/$ID/[Normal Graphics Frame]" AppliedTextObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" AppliedGridObjectStyle="ObjectStyle/$ID/[Normal Grid]" CornerOption="None" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GradientFillAngle="0" GradientStrokeAngle="0" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false"/>
+  <PageItemDefault TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" AppliedGraphicObjectStyle="ObjectStyle/$ID/[Normal Graphics Frame]" AppliedTextObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" AppliedGridObjectStyle="ObjectStyle/$ID/[Normal Grid]" CornerOption="None" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GradientFillAngle="0" GradientStrokeAngle="0" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false"/>
   <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
   <ButtonPreference Name=""/>
   <TinDocumentDataObject>
     <Properties>
-      <GaijiRefMaps>/////wAAAAAAAAAA</GaijiRefMaps>
+      <GaijiRefMaps><![CDATA[/////wAAAAAAAAAA]]></GaijiRefMaps>
     </Properties>
   </TinDocumentDataObject>
   <LayoutGridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100">
     <Properties>
       <AppliedFont type="string">Minion Pro</AppliedFont>
     </Properties>
   </LayoutGridDataInformation>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Styles.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml`

 * *Files 10% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Resources/Styles.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Resources/Styles.xml`

```diff
@@ -1,32 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Styles xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <RootCharacterStyleGroup Self="myprefixu65">
-    <CharacterStyle Self="myprefixCharacterStyle/$ID/[No character style]" Imported="false" Name="$ID/[No character style]"/>
-    <CharacterStyle Self="myprefixCharacterStyle/bold" Imported="false" KeyboardShortcut="0 0" Name="bold" FontStyle="Bold">
-      <Properties>
-        <BasedOn type="string">$ID/[No character style]</BasedOn>
-        <PreviewColor type="enumeration">Nothing</PreviewColor>
-      </Properties>
-    </CharacterStyle>
-    <CharacterStyle Self="myprefixCharacterStyle/italique" Imported="false" KeyboardShortcut="0 0" Name="italique" FontStyle="Italic">
-      <Properties>
-        <BasedOn type="string">$ID/[No character style]</BasedOn>
-        <PreviewColor type="enumeration">Nothing</PreviewColor>
-      </Properties>
-    </CharacterStyle>
-    <CharacterStyle Self="myprefixCharacterStyle/sup" Imported="false" KeyboardShortcut="0 0" Name="sup" Position="Superscript">
+  <RootCharacterStyleGroup Self="u65">
+    <CharacterStyle Self="CharacterStyle/$ID/[No character style]" Imported="false" Name="$ID/[No character style]"/>
+    <CharacterStyle Self="CharacterStyle/MyBoldStyle" Imported="false" KeyboardShortcut="0 0" Name="MyBoldStyle" FontStyle="Bold">
       <Properties>
         <BasedOn type="string">$ID/[No character style]</BasedOn>
         <PreviewColor type="enumeration">Nothing</PreviewColor>
       </Properties>
     </CharacterStyle>
   </RootCharacterStyleGroup>
-  <RootParagraphStyleGroup Self="myprefixu64">
-    <ParagraphStyle Self="myprefixParagraphStyle/$ID/[No paragraph style]" Name="$ID/[No paragraph style]" Imported="false" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" FillColor="myprefixColor/Black" FontStyle="Regular" PointSize="12" HorizontalScale="100" KerningMethod="$ID/Metrics" Ligatures="true" PageNumberType="AutoPageNumber" StrokeWeight="1" Tracking="0" Composer="HL Composer" DropCapCharacters="0" DropCapLines="0" BaselineShift="0" Capitalization="Normal" StrokeColor="myprefixSwatch/None" HyphenateLadderLimit="3" VerticalScale="100" LeftIndent="0" RightIndent="0" FirstLineIndent="0" AutoLeading="120" AppliedLanguage="$ID/English: UK" Hyphenation="true" HyphenateAfterFirst="2" HyphenateBeforeLast="2" HyphenateCapitalizedWords="true" HyphenateWordsLongerThan="5" NoBreak="false" HyphenationZone="36" SpaceBefore="0" SpaceAfter="0" Underline="false" OTFFigureStyle="Default" DesiredWordSpacing="100" MaximumWordSpacing="133" MinimumWordSpacing="80" DesiredLetterSpacing="0" MaximumLetterSpacing="0" MinimumLetterSpacing="0" DesiredGlyphScaling="100" MaximumGlyphScaling="100" MinimumGlyphScaling="100" StartParagraph="Anywhere" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" Position="Normal" StrikeThru="false" CharacterAlignment="AlignEmCenter" KeepLinesTogether="false" StrokeTint="-1" FillTint="-1" OverprintStroke="false" OverprintFill="false" GradientStrokeAngle="0" GradientFillAngle="0" GradientStrokeLength="-1" GradientFillLength="-1" GradientStrokeStart="0 0" GradientFillStart="0 0" Skew="0" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleAboveOverprint="false" RuleBelowOverprint="false" RuleAbove="false" RuleBelow="false" LastLineIndent="0" HyphenateLastWord="true" ParagraphBreakType="Anywhere" SingleWordJustification="FullyJustified" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelowGapTint="-1" RuleBelowGapOverprint="false" Justification="LeftAlign" DropcapDetail="1" PositionalForm="None" OTFMark="true" HyphenWeight="5" OTFLocale="true" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFSlashedZero="false" OTFStylisticSets="0" OTFHistorical="false" OTFContextualAlternate="true" UnderlineGapOverprint="false" UnderlineGapTint="-1" UnderlineOffset="-9999" UnderlineOverprint="false" UnderlineTint="-1" UnderlineWeight="-9999" StrikeThroughGapOverprint="false" StrikeThroughGapTint="-1" StrikeThroughOffset="-9999" StrikeThroughOverprint="false" StrikeThroughTint="-1" StrikeThroughWeight="-9999" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" KeepWithPrevious="false" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" OTFSwash="false" Tsume="0" LeadingAki="-1" TrailingAki="-1" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" RubyOpenTypePro="true" RubyFontSize="-1" RubyAlignment="RubyJIS" RubyType="PerCharacterRuby" RubyParentSpacing="RubyParent121Aki" RubyXScale="100" RubyYScale="100" RubyXOffset="0" RubyYOffset="0" RubyPosition="AboveRight" RubyAutoAlign="true" RubyParentOverhangAmount="RubyOverhangOneRuby" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyTint="-1" RubyOverprintFill="Auto" RubyStrokeTint="-1" RubyOverprintStroke="Auto" RubyWeight="-1" KentenKind="None" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" KentenTint="-1" KentenOverprintFill="Auto" KentenStrokeTint="-1" KentenOverprintStroke="Auto" KentenWeight="-1" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" AutoTcy="0" AutoTcyIncludeRoman="false" Jidori="0" GridGyoudori="0" GridAlignFirstLineOnly="false" GridAlignment="None" CharacterRotation="0" RotateSingleByteCharacters="false" Rensuuji="true" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustTsume="true" ShataiAdjustRotation="false" Warichu="false" WarichuLines="2" WarichuSize="50" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsBeforeBreak="2" WarichuCharsAfterBreak="2" OTFHVKana="false" OTFProportionalMetrics="false" OTFRomanItalics="false" LeadingModel="LeadingModelAkiBelow" ScaleAffectsLineHeight="false" ParagraphGyoudori="false" CjkGridTracking="false" GlyphForm="None" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingStartAt="1" NumberingLevel="1" NumberingContinue="true" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign" NumberingExpression="^#.^t" BulletsTextAfter="^t" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" CharacterDirection="DefaultDirection" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" ParagraphKashidaWidth="2" XOffsetDiacritic="0" YOffsetDiacritic="0" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" KeyboardDirection="DefaultDirection">
+  <RootParagraphStyleGroup Self="u64">
+    <ParagraphStyle Self="ParagraphStyle/$ID/[No paragraph style]" Name="$ID/[No paragraph style]" Imported="false" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" FillColor="Color/Black" FontStyle="Regular" PointSize="12" HorizontalScale="100" KerningMethod="$ID/Metrics" Ligatures="true" PageNumberType="AutoPageNumber" StrokeWeight="1" Tracking="0" Composer="HL Composer" DropCapCharacters="0" DropCapLines="0" BaselineShift="0" Capitalization="Normal" StrokeColor="Swatch/None" HyphenateLadderLimit="3" VerticalScale="100" LeftIndent="0" RightIndent="0" FirstLineIndent="0" AutoLeading="120" AppliedLanguage="$ID/English: UK" Hyphenation="true" HyphenateAfterFirst="2" HyphenateBeforeLast="2" HyphenateCapitalizedWords="true" HyphenateWordsLongerThan="5" NoBreak="false" HyphenationZone="36" SpaceBefore="0" SpaceAfter="0" Underline="false" OTFFigureStyle="Default" DesiredWordSpacing="100" MaximumWordSpacing="133" MinimumWordSpacing="80" DesiredLetterSpacing="0" MaximumLetterSpacing="0" MinimumLetterSpacing="0" DesiredGlyphScaling="100" MaximumGlyphScaling="100" MinimumGlyphScaling="100" StartParagraph="Anywhere" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" Position="Normal" StrikeThru="false" CharacterAlignment="AlignEmCenter" KeepLinesTogether="false" StrokeTint="-1" FillTint="-1" OverprintStroke="false" OverprintFill="false" GradientStrokeAngle="0" GradientFillAngle="0" GradientStrokeLength="-1" GradientFillLength="-1" GradientStrokeStart="0 0" GradientFillStart="0 0" Skew="0" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleAboveOverprint="false" RuleBelowOverprint="false" RuleAbove="false" RuleBelow="false" LastLineIndent="0" HyphenateLastWord="true" ParagraphBreakType="Anywhere" SingleWordJustification="FullyJustified" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelowGapTint="-1" RuleBelowGapOverprint="false" Justification="LeftAlign" DropcapDetail="1" PositionalForm="None" OTFMark="true" HyphenWeight="5" OTFLocale="true" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFSlashedZero="false" OTFStylisticSets="0" OTFHistorical="false" OTFContextualAlternate="true" UnderlineGapOverprint="false" UnderlineGapTint="-1" UnderlineOffset="-9999" UnderlineOverprint="false" UnderlineTint="-1" UnderlineWeight="-9999" StrikeThroughGapOverprint="false" StrikeThroughGapTint="-1" StrikeThroughOffset="-9999" StrikeThroughOverprint="false" StrikeThroughTint="-1" StrikeThroughWeight="-9999" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" KeepWithPrevious="false" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" OTFSwash="false" Tsume="0" LeadingAki="-1" TrailingAki="-1" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" RubyOpenTypePro="true" RubyFontSize="-1" RubyAlignment="RubyJIS" RubyType="PerCharacterRuby" RubyParentSpacing="RubyParent121Aki" RubyXScale="100" RubyYScale="100" RubyXOffset="0" RubyYOffset="0" RubyPosition="AboveRight" RubyAutoAlign="true" RubyParentOverhangAmount="RubyOverhangOneRuby" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyTint="-1" RubyOverprintFill="Auto" RubyStrokeTint="-1" RubyOverprintStroke="Auto" RubyWeight="-1" KentenKind="None" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" KentenTint="-1" KentenOverprintFill="Auto" KentenStrokeTint="-1" KentenOverprintStroke="Auto" KentenWeight="-1" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" AutoTcy="0" AutoTcyIncludeRoman="false" Jidori="0" GridGyoudori="0" GridAlignFirstLineOnly="false" GridAlignment="None" CharacterRotation="0" RotateSingleByteCharacters="false" Rensuuji="true" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustTsume="true" ShataiAdjustRotation="false" Warichu="false" WarichuLines="2" WarichuSize="50" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsBeforeBreak="2" WarichuCharsAfterBreak="2" OTFHVKana="false" OTFProportionalMetrics="false" OTFRomanItalics="false" LeadingModel="LeadingModelAkiBelow" ScaleAffectsLineHeight="false" ParagraphGyoudori="false" CjkGridTracking="false" GlyphForm="None" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingStartAt="1" NumberingLevel="1" NumberingContinue="true" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign" NumberingExpression="^#.^t" BulletsTextAfter="^t" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" CharacterDirection="DefaultDirection" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" ParagraphKashidaWidth="2" XOffsetDiacritic="0" YOffsetDiacritic="0" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" KeyboardDirection="DefaultDirection">
       <Properties>
         <Leading type="enumeration">Auto</Leading>
         <TabList type="list"/>
         <AppliedFont type="string">Minion Pro</AppliedFont>
         <RuleAboveColor type="string">Text Color</RuleAboveColor>
         <RuleBelowColor type="string">Text Color</RuleBelowColor>
         <RuleAboveType type="object">StrokeStyle/$ID/Solid</RuleAboveType>
@@ -57,35 +45,35 @@
         <BulletsFontStyle type="enumeration">Nothing</BulletsFontStyle>
         <AppliedNumberingList type="object">NumberingList/$ID/[Default]</AppliedNumberingList>
         <NumberingRestartPolicies RestartPolicy="AnyPreviousLevel" LowerLevel="0" UpperLevel="0"/>
         <BulletsCharacterStyle type="object">CharacterStyle/$ID/[No character style]</BulletsCharacterStyle>
         <NumberingCharacterStyle type="object">CharacterStyle/$ID/[No character style]</NumberingCharacterStyle>
       </Properties>
     </ParagraphStyle>
-    <ParagraphStyle Self="myprefixParagraphStyle/$ID/NormalParagraphStyle" Name="$ID/NormalParagraphStyle" Imported="false" NextStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" KeyboardShortcut="0 0">
+    <ParagraphStyle Self="ParagraphStyle/$ID/NormalParagraphStyle" Name="$ID/NormalParagraphStyle" Imported="false" NextStyle="ParagraphStyle/$ID/NormalParagraphStyle" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" KeyboardShortcut="0 0">
       <Properties>
         <BasedOn type="string">$ID/[No paragraph style]</BasedOn>
         <PreviewColor type="enumeration">Nothing</PreviewColor>
       </Properties>
     </ParagraphStyle>
   </RootParagraphStyleGroup>
-  <TOCStyle Self="myprefixTOCStyle/$ID/DefaultTOCStyleName" TitleStyle="ParagraphStyle/$ID/[No paragraph style]" Title="Contents" Name="$ID/DefaultTOCStyleName" RunIn="false" IncludeHidden="false" IncludeBookDocuments="false" CreateBookmarks="true" SetStoryDirection="Horizontal" NumberedParagraphs="IncludeFullParagraph" MakeAnchor="false"/>
-  <RootCellStyleGroup Self="myprefixu6a">
-    <CellStyle Self="myprefixCellStyle/$ID/[None]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/[No paragraph style]" Name="$ID/[None]"/>
+  <TOCStyle Self="TOCStyle/$ID/DefaultTOCStyleName" TitleStyle="ParagraphStyle/$ID/[No paragraph style]" Title="Contents" Name="$ID/DefaultTOCStyleName" RunIn="false" IncludeHidden="false" IncludeBookDocuments="false" CreateBookmarks="true" SetStoryDirection="Horizontal" NumberedParagraphs="IncludeFullParagraph" MakeAnchor="false"/>
+  <RootCellStyleGroup Self="u6a">
+    <CellStyle Self="CellStyle/$ID/[None]" AppliedParagraphStyle="ParagraphStyle/$ID/[No paragraph style]" Name="$ID/[None]"/>
   </RootCellStyleGroup>
-  <RootTableStyleGroup Self="myprefixu6c">
-    <TableStyle Self="myprefixTableStyle/$ID/[No table style]" Name="$ID/[No table style]" StrokeOrder="BestJoins" TopBorderStrokeWeight="1" TopBorderStrokeType="StrokeStyle/$ID/Solid" TopBorderStrokeColor="Color/Black" TopBorderStrokeTint="100" TopBorderStrokeOverprint="false" TopBorderStrokeGapColor="Color/Paper" TopBorderStrokeGapTint="100" TopBorderStrokeGapOverprint="false" LeftBorderStrokeWeight="1" LeftBorderStrokeType="StrokeStyle/$ID/Solid" LeftBorderStrokeColor="Color/Black" LeftBorderStrokeTint="100" LeftBorderStrokeOverprint="false" LeftBorderStrokeGapColor="Color/Paper" LeftBorderStrokeGapTint="100" LeftBorderStrokeGapOverprint="false" BottomBorderStrokeWeight="1" BottomBorderStrokeType="StrokeStyle/$ID/Solid" BottomBorderStrokeColor="Color/Black" BottomBorderStrokeTint="100" BottomBorderStrokeOverprint="false" BottomBorderStrokeGapColor="Color/Paper" BottomBorderStrokeGapTint="100" BottomBorderStrokeGapOverprint="false" RightBorderStrokeWeight="1" RightBorderStrokeType="StrokeStyle/$ID/Solid" RightBorderStrokeColor="Color/Black" RightBorderStrokeTint="100" RightBorderStrokeOverprint="false" RightBorderStrokeGapColor="Color/Paper" RightBorderStrokeGapTint="100" RightBorderStrokeGapOverprint="false" SpaceBefore="4" SpaceAfter="-4" SkipFirstAlternatingStrokeRows="0" SkipLastAlternatingStrokeRows="0" StartRowStrokeCount="0" StartRowStrokeColor="Color/Black" StartRowStrokeWeight="1" StartRowStrokeType="StrokeStyle/$ID/Solid" StartRowStrokeTint="100" StartRowStrokeGapOverprint="false" StartRowStrokeGapColor="Color/Paper" StartRowStrokeGapTint="100" StartRowStrokeOverprint="false" EndRowStrokeCount="0" EndRowStrokeColor="Color/Black" EndRowStrokeWeight="0.25" EndRowStrokeType="StrokeStyle/$ID/Solid" EndRowStrokeTint="100" EndRowStrokeOverprint="false" EndRowStrokeGapColor="Color/Paper" EndRowStrokeGapTint="100" EndRowStrokeGapOverprint="false" SkipFirstAlternatingStrokeColumns="0" SkipLastAlternatingStrokeColumns="0" StartColumnStrokeCount="0" StartColumnStrokeColor="Color/Black" StartColumnStrokeWeight="1" StartColumnStrokeType="StrokeStyle/$ID/Solid" StartColumnStrokeTint="100" StartColumnStrokeOverprint="false" StartColumnStrokeGapColor="Color/Paper" StartColumnStrokeGapTint="100" StartColumnStrokeGapOverprint="false" EndColumnStrokeCount="0" EndColumnStrokeColor="Color/Black" EndColumnStrokeWeight="0.25" EndColumnLineStyle="StrokeStyle/$ID/Solid" EndColumnStrokeTint="100" EndColumnStrokeOverprint="false" EndColumnStrokeGapColor="Color/Paper" EndColumnStrokeGapTint="100" EndColumnStrokeGapOverprint="false" ColumnFillsPriority="false" SkipFirstAlternatingFillRows="0" SkipLastAlternatingFillRows="0" StartRowFillColor="Color/Black" StartRowFillCount="0" StartRowFillTint="20" StartRowFillOverprint="false" EndRowFillCount="0" EndRowFillColor="Swatch/None" EndRowFillTint="100" EndRowFillOverprint="false" SkipFirstAlternatingFillColumns="0" SkipLastAlternatingFillColumns="0" StartColumnFillCount="0" StartColumnFillColor="Color/Black" StartColumnFillTint="20" StartColumnFillOverprint="false" EndColumnFillCount="0" EndColumnFillColor="Swatch/None" EndColumnFillTint="100" EndColumnFillOverprint="false" HeaderRegionSameAsBodyRegion="true" FooterRegionSameAsBodyRegion="true" LeftColumnRegionSameAsBodyRegion="true" RightColumnRegionSameAsBodyRegion="true" HeaderRegionCellStyle="n" FooterRegionCellStyle="n" LeftColumnRegionCellStyle="n" RightColumnRegionCellStyle="n" BodyRegionCellStyle="CellStyle/$ID/[None]"/>
-    <TableStyle Self="myprefixTableStyle/$ID/[Basic Table]" Name="$ID/[Basic Table]" KeyboardShortcut="0 0">
+  <RootTableStyleGroup Self="u6c">
+    <TableStyle Self="TableStyle/$ID/[No table style]" Name="$ID/[No table style]" StrokeOrder="BestJoins" TopBorderStrokeWeight="1" TopBorderStrokeType="StrokeStyle/$ID/Solid" TopBorderStrokeColor="Color/Black" TopBorderStrokeTint="100" TopBorderStrokeOverprint="false" TopBorderStrokeGapColor="Color/Paper" TopBorderStrokeGapTint="100" TopBorderStrokeGapOverprint="false" LeftBorderStrokeWeight="1" LeftBorderStrokeType="StrokeStyle/$ID/Solid" LeftBorderStrokeColor="Color/Black" LeftBorderStrokeTint="100" LeftBorderStrokeOverprint="false" LeftBorderStrokeGapColor="Color/Paper" LeftBorderStrokeGapTint="100" LeftBorderStrokeGapOverprint="false" BottomBorderStrokeWeight="1" BottomBorderStrokeType="StrokeStyle/$ID/Solid" BottomBorderStrokeColor="Color/Black" BottomBorderStrokeTint="100" BottomBorderStrokeOverprint="false" BottomBorderStrokeGapColor="Color/Paper" BottomBorderStrokeGapTint="100" BottomBorderStrokeGapOverprint="false" RightBorderStrokeWeight="1" RightBorderStrokeType="StrokeStyle/$ID/Solid" RightBorderStrokeColor="Color/Black" RightBorderStrokeTint="100" RightBorderStrokeOverprint="false" RightBorderStrokeGapColor="Color/Paper" RightBorderStrokeGapTint="100" RightBorderStrokeGapOverprint="false" SpaceBefore="4" SpaceAfter="-4" SkipFirstAlternatingStrokeRows="0" SkipLastAlternatingStrokeRows="0" StartRowStrokeCount="0" StartRowStrokeColor="Color/Black" StartRowStrokeWeight="1" StartRowStrokeType="StrokeStyle/$ID/Solid" StartRowStrokeTint="100" StartRowStrokeGapOverprint="false" StartRowStrokeGapColor="Color/Paper" StartRowStrokeGapTint="100" StartRowStrokeOverprint="false" EndRowStrokeCount="0" EndRowStrokeColor="Color/Black" EndRowStrokeWeight="0.25" EndRowStrokeType="StrokeStyle/$ID/Solid" EndRowStrokeTint="100" EndRowStrokeOverprint="false" EndRowStrokeGapColor="Color/Paper" EndRowStrokeGapTint="100" EndRowStrokeGapOverprint="false" SkipFirstAlternatingStrokeColumns="0" SkipLastAlternatingStrokeColumns="0" StartColumnStrokeCount="0" StartColumnStrokeColor="Color/Black" StartColumnStrokeWeight="1" StartColumnStrokeType="StrokeStyle/$ID/Solid" StartColumnStrokeTint="100" StartColumnStrokeOverprint="false" StartColumnStrokeGapColor="Color/Paper" StartColumnStrokeGapTint="100" StartColumnStrokeGapOverprint="false" EndColumnStrokeCount="0" EndColumnStrokeColor="Color/Black" EndColumnStrokeWeight="0.25" EndColumnLineStyle="StrokeStyle/$ID/Solid" EndColumnStrokeTint="100" EndColumnStrokeOverprint="false" EndColumnStrokeGapColor="Color/Paper" EndColumnStrokeGapTint="100" EndColumnStrokeGapOverprint="false" ColumnFillsPriority="false" SkipFirstAlternatingFillRows="0" SkipLastAlternatingFillRows="0" StartRowFillColor="Color/Black" StartRowFillCount="0" StartRowFillTint="20" StartRowFillOverprint="false" EndRowFillCount="0" EndRowFillColor="Swatch/None" EndRowFillTint="100" EndRowFillOverprint="false" SkipFirstAlternatingFillColumns="0" SkipLastAlternatingFillColumns="0" StartColumnFillCount="0" StartColumnFillColor="Color/Black" StartColumnFillTint="20" StartColumnFillOverprint="false" EndColumnFillCount="0" EndColumnFillColor="Swatch/None" EndColumnFillTint="100" EndColumnFillOverprint="false" HeaderRegionSameAsBodyRegion="true" FooterRegionSameAsBodyRegion="true" LeftColumnRegionSameAsBodyRegion="true" RightColumnRegionSameAsBodyRegion="true" HeaderRegionCellStyle="n" FooterRegionCellStyle="n" LeftColumnRegionCellStyle="n" RightColumnRegionCellStyle="n" BodyRegionCellStyle="CellStyle/$ID/[None]"/>
+    <TableStyle Self="TableStyle/$ID/[Basic Table]" Name="$ID/[Basic Table]" KeyboardShortcut="0 0">
       <Properties>
         <BasedOn type="string">$ID/[No table style]</BasedOn>
       </Properties>
     </TableStyle>
   </RootTableStyleGroup>
-  <RootObjectStyleGroup Self="myprefixu75">
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[None]" Name="$ID/[None]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/[No paragraph style]" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" CornerOption="None">
+  <RootObjectStyleGroup Self="u75">
+    <ObjectStyle Self="ObjectStyle/$ID/[None]" Name="$ID/[None]" AppliedParagraphStyle="ParagraphStyle/$ID/[No paragraph style]" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" CornerOption="None">
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
       <TextFramePreference TextColumnCount="1" TextColumnGutter="12" TextColumnFixedWidth="144" UseFixedColumnWidth="false" FirstBaselineOffset="AscentOffset" MinimumFirstBaselineOffset="0" VerticalJustification="TopAlign" VerticalThreshold="0" IgnoreWrap="false" UseFlexibleColumnWidth="false" TextColumnMaxWidth="0" AutoSizingType="Off" AutoSizingReferencePoint="CenterPoint" UseMinimumHeightForAutoSizing="false" MinimumHeightForAutoSizing="0" UseMinimumWidthForAutoSizing="false" MinimumWidthForAutoSizing="0" UseNoLineBreaksForAutoSizing="false" VerticalBalanceColumns="false">
@@ -109,15 +97,15 @@
           <TextWrapOffset Top="0" Left="0" Bottom="0" Right="0"/>
         </Properties>
         <ContourOption ContourType="SameAsClipping" IncludeInsideEdges="false" ContourPathName="$ID/"/>
       </TextWrapPreference>
       <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
     </ObjectStyle>
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[Normal Graphics Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Graphics Frame]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/[No paragraph style]" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="false" EnableTextFrameBaselineOptions="false" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixColor/Black" StrokeTint="-1" OverprintStroke="false" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
+    <ObjectStyle Self="ObjectStyle/$ID/[Normal Graphics Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Graphics Frame]" AppliedParagraphStyle="ParagraphStyle/$ID/[No paragraph style]" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="false" EnableTextFrameBaselineOptions="false" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Color/Black" StrokeTint="-1" OverprintStroke="false" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
       <Properties>
         <BasedOn type="string">$ID/[None]</BasedOn>
       </Properties>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
@@ -148,15 +136,15 @@
       <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="Unknown" StoryOrientation="Unknown" StoryDirection="UnknownDirection"/>
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
       <ObjectStyleObjectEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleStrokeEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleFillEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleContentEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
     </ObjectStyle>
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[Normal Text Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Text Frame]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
+    <ObjectStyle Self="ObjectStyle/$ID/[Normal Text Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Text Frame]" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
       <Properties>
         <BasedOn type="string">$ID/[None]</BasedOn>
       </Properties>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
@@ -187,15 +175,15 @@
       <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Unknown" StoryDirection="LeftToRightDirection"/>
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
       <ObjectStyleObjectEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleStrokeEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleFillEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleContentEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
     </ObjectStyle>
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[Normal Grid]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Grid]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="true" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
+    <ObjectStyle Self="ObjectStyle/$ID/[Normal Grid]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Grid]" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="true" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
       <Properties>
         <BasedOn type="string">$ID/[None]</BasedOn>
       </Properties>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
@@ -227,10 +215,10 @@
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
       <ObjectStyleObjectEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleStrokeEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleFillEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleContentEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
     </ObjectStyle>
   </RootObjectStyleGroup>
-  <TrapPreset Self="myprefixTrapPreset/$ID/k[No Trap Preset]" Name="$ID/k[No Trap Preset]" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
-  <TrapPreset Self="myprefixTrapPreset/$ID/kDefaultTrapStyleName" Name="$ID/kDefaultTrapStyleName" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
+  <TrapPreset Self="TrapPreset/$ID/k[No Trap Preset]" Name="$ID/k[No Trap Preset]" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
+  <TrapPreset Self="TrapPreset/$ID/kDefaultTrapStyleName" Name="$ID/kDefaultTrapStyleName" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
 </idPkg:Styles>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Spreads/Spread_myprefixud8.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml`

 * *Files 10% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Spreads/Spread_myprefixud8.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Spreads/Spread_ud6.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Spread xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Spread Self="myprefixud8" FlattenerOverride="Default" AllowPageShuffle="true" ItemTransform="1 0 0 1 0 0" ShowMasterItems="true" PageCount="1" BindingLocation="0" PageTransitionType="None" PageTransitionDirection="NotApplicable" PageTransitionDuration="Medium">
+  <Spread Self="ud6" FlattenerOverride="Default" AllowPageShuffle="true" ItemTransform="1 0 0 1 0 0" ShowMasterItems="true" PageCount="1" BindingLocation="0" PageTransitionType="None" PageTransitionDirection="NotApplicable" PageTransitionDuration="Medium">
     <FlattenerPreference LineArtAndTextResolution="300" GradientAndMeshResolution="150" ClipComplexRegions="false" ConvertAllStrokesToOutlines="false" ConvertAllTextToOutlines="false">
       <Properties>
         <RasterVectorBalance type="double">50</RasterVectorBalance>
       </Properties>
     </FlattenerPreference>
-    <Page Self="myprefixudd" AppliedAlternateLayout="u9b" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="1" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="ua5" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
+    <Page Self="udb" AppliedAlternateLayout="u9b" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="1" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="ua5" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
       <Properties>
         <Descriptor type="list">
           <ListItem type="string"/>
           <ListItem type="enumeration">Arabic</ListItem>
           <ListItem type="boolean">true</ListItem>
           <ListItem type="boolean">false</ListItem>
           <ListItem type="long">1</ListItem>
@@ -21,15 +21,15 @@
       <MarginPreference ColumnCount="1" ColumnGutter="12" Top="36" Bottom="36" Left="36" Right="36" ColumnDirection="Horizontal" ColumnsPositions="0 494.92913385826773"/>
       <GridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100" LineAlignment="LeftOrTopLineJustify" GridAlignment="AlignEmCenter" CharacterAlignment="AlignEmCenter">
         <Properties>
           <AppliedFont type="string">Minion Pro</AppliedFont>
         </Properties>
       </GridDataInformation>
     </Page>
-    <Rectangle Self="myprefixudf" ContentType="GraphicType" StoryTitle="$ID/" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 17.763779527559194 -391.27559055118115">
+    <Rectangle Self="u182" ContentType="GraphicType" StoryTitle="$ID/" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 17.763779527559194 -391.27559055118115">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="144.56692913385828 58.582677165354326" LeftDirection="144.56692913385828 58.582677165354326" RightDirection="144.56692913385828 58.582677165354326"/>
               <PathPointType Anchor="144.56692913385828 199.46456692913392" LeftDirection="144.56692913385828 199.46456692913392" RightDirection="144.56692913385828 199.46456692913392"/>
               <PathPointType Anchor="403.46456692913387 199.46456692913392" LeftDirection="403.46456692913387 199.46456692913392" RightDirection="403.46456692913387 199.46456692913392"/>
@@ -41,70 +41,70 @@
       <TextWrapPreference Inverse="false" ApplyToMasterPageOnly="false" TextWrapSide="BothSides" TextWrapMode="None">
         <Properties>
           <TextWrapOffset Top="0" Left="0" Bottom="0" Right="0"/>
         </Properties>
         <ContourOption ContourType="SameAsClipping" IncludeInsideEdges="false" ContourPathName="$ID/"/>
       </TextWrapPreference>
       <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
-      <FrameFittingOption RightCrop="44.102362204724386" BottomCrop="219.1181102362204"/>
+      <FrameFittingOption FittingOnEmptyFrame="FillProportionally"/>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
-      <Image Self="myprefixu14a" Space="$ID/#Links_RGB" ActualPpi="72 72" EffectivePpi="72 72" ImageRenderingIntent="UseColorSettings" OverriddenPageItemProps="" LocalDisplaySetting="Default" ImageTypeName="$ID/JPEG" AppliedObjectStyle="myprefixObjectStyle/$ID/[None]" ItemTransform="1 0 0 1 144.56692913385825 58.58267716535431" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" Visible="true" Name="$ID/">
+      <Image Self="u216" Space="$ID/#Links_RGB" ActualPpi="72 72" EffectivePpi="84 84" ImageRenderingIntent="UseColorSettings" OverriddenPageItemProps="" LocalDisplaySetting="Default" ImageTypeName="$ID/JPEG" AppliedObjectStyle="ObjectStyle/$ID/[None]" ItemTransform="0.8544476494893585 0 0 0.8544476494893584 144.56692913385828 58.582677165354326" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" Visible="true" Name="$ID/">
         <Properties>
           <Profile type="string">$ID/None</Profile>
           <GraphicBounds Left="0" Top="0" Right="303" Bottom="360"/>
         </Properties>
         <TextWrapPreference Inverse="false" ApplyToMasterPageOnly="false" TextWrapSide="BothSides" TextWrapMode="None">
           <Properties>
             <TextWrapOffset Top="0" Left="0" Bottom="0" Right="0"/>
           </Properties>
           <ContourOption ContourType="SameAsClipping" IncludeInsideEdges="false" ContourPathName="$ID/"/>
         </TextWrapPreference>
         <MetadataPacketPreference>
           <Properties>
-            <Contents>&lt;?xpacket begin=&quot;﻿&quot; id=&quot;W5M0MpCehiHzreSzNTczkc9d&quot;?&gt;
-&lt;x:xmpmeta xmlns:x=&quot;adobe:ns:meta/&quot; x:xmptk=&quot;Adobe XMP Core 5.6-c011 79.156289, 2014/03/31-23:39:12        &quot;&gt;
-   &lt;rdf:RDF xmlns:rdf=&quot;http://www.w3.org/1999/02/22-rdf-syntax-ns#&quot;&gt;
-      &lt;rdf:Description rdf:about=&quot;&quot;
-            xmlns:tiff=&quot;http://ns.adobe.com/tiff/1.0/&quot;
-            xmlns:exif=&quot;http://ns.adobe.com/exif/1.0/&quot;&gt;
-         &lt;tiff:XResolution&gt;72/1&lt;/tiff:XResolution&gt;
-         &lt;tiff:YResolution&gt;72/1&lt;/tiff:YResolution&gt;
-         &lt;tiff:ResolutionUnit&gt;2&lt;/tiff:ResolutionUnit&gt;
-         &lt;tiff:YCbCrPositioning&gt;1&lt;/tiff:YCbCrPositioning&gt;
-         &lt;exif:ColorSpace&gt;1&lt;/exif:ColorSpace&gt;
-         &lt;exif:PixelXDimension&gt;360&lt;/exif:PixelXDimension&gt;
-         &lt;exif:PixelYDimension&gt;303&lt;/exif:PixelYDimension&gt;
-         &lt;exif:SceneCaptureType&gt;0&lt;/exif:SceneCaptureType&gt;
-         &lt;exif:ExifVersion&gt;0221&lt;/exif:ExifVersion&gt;
-         &lt;exif:FlashpixVersion&gt;0100&lt;/exif:FlashpixVersion&gt;
-         &lt;exif:ComponentsConfiguration&gt;
-            &lt;rdf:Seq&gt;
-               &lt;rdf:li&gt;1&lt;/rdf:li&gt;
-               &lt;rdf:li&gt;2&lt;/rdf:li&gt;
-               &lt;rdf:li&gt;3&lt;/rdf:li&gt;
-               &lt;rdf:li&gt;0&lt;/rdf:li&gt;
-            &lt;/rdf:Seq&gt;
-         &lt;/exif:ComponentsConfiguration&gt;
-      &lt;/rdf:Description&gt;
-   &lt;/rdf:RDF&gt;
-&lt;/x:xmpmeta&gt;
-&lt;?xpacket end=&quot;r&quot;?&gt;</Contents>
+            <Contents><![CDATA[<?xpacket begin="﻿" id="W5M0MpCehiHzreSzNTczkc9d"?>
+<x:xmpmeta xmlns:x="adobe:ns:meta/" x:xmptk="Adobe XMP Core 5.6-c011 79.156289, 2014/03/31-23:39:12        ">
+   <rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#">
+      <rdf:Description rdf:about=""
+            xmlns:tiff="http://ns.adobe.com/tiff/1.0/"
+            xmlns:exif="http://ns.adobe.com/exif/1.0/">
+         <tiff:XResolution>72/1</tiff:XResolution>
+         <tiff:YResolution>72/1</tiff:YResolution>
+         <tiff:ResolutionUnit>2</tiff:ResolutionUnit>
+         <tiff:YCbCrPositioning>1</tiff:YCbCrPositioning>
+         <exif:ColorSpace>1</exif:ColorSpace>
+         <exif:PixelXDimension>360</exif:PixelXDimension>
+         <exif:PixelYDimension>303</exif:PixelYDimension>
+         <exif:SceneCaptureType>0</exif:SceneCaptureType>
+         <exif:ExifVersion>0221</exif:ExifVersion>
+         <exif:FlashpixVersion>0100</exif:FlashpixVersion>
+         <exif:ComponentsConfiguration>
+            <rdf:Seq>
+               <rdf:li>1</rdf:li>
+               <rdf:li>2</rdf:li>
+               <rdf:li>3</rdf:li>
+               <rdf:li>0</rdf:li>
+            </rdf:Seq>
+         </exif:ComponentsConfiguration>
+      </rdf:Description>
+   </rdf:RDF>
+</x:xmpmeta>
+<?xpacket end="r"?>]]></Contents>
           </Properties>
         </MetadataPacketPreference>
-        <Link Self="myprefixu14e" AssetURL="$ID/" AssetID="$ID/" LinkResourceURI="file:/Users/stan/Dropbox/Projets/Slashdev/SimpleIDML/repos/git/simpleidml/tests/regressiontests/IDML/media/default.jpg" LinkResourceFormat="$ID/JPEG" StoredState="Normal" LinkClassID="35906" LinkClientID="257" LinkResourceModified="false" LinkObjectModified="false" ShowInUI="true" CanEmbed="true" CanUnembed="true" CanPackage="true" ImportPolicy="NoAutoImport" ExportPolicy="NoAutoExport" LinkImportStamp="file 129767622980000000 27644" LinkImportModificationTime="2012-03-21T01:11:38" LinkImportTime="2014-09-24T14:59:30" LinkResourceSize="0~6bfc"/>
+        <Link Self="u21a" AssetURL="$ID/" AssetID="$ID/" LinkResourceURI="file:/Users/stan/Dropbox/Projets/Slashdev/SimpleIDML/repos/git/simpleidml/tests/regressiontests/IDML/media/default.jpg" LinkResourceFormat="$ID/JPEG" StoredState="Normal" LinkClassID="35906" LinkClientID="257" LinkResourceModified="false" LinkObjectModified="false" ShowInUI="true" CanEmbed="true" CanUnembed="true" CanPackage="true" ImportPolicy="NoAutoImport" ExportPolicy="NoAutoExport" LinkImportStamp="file 129767622980000000 27644" LinkImportModificationTime="2012-03-21T01:11:38" LinkImportTime="2014-09-24T14:47:22" LinkResourceSize="0~6bfc"/>
         <ClippingPathSettings ClippingType="None" InvertPath="false" IncludeInsideEdges="false" RestrictToFrame="false" UseHighResolutionImage="true" Threshold="25" Tolerance="2" InsetFrame="0" AppliedPathName="$ID/" Index="-1"/>
         <ImageIOPreference ApplyPhotoshopClippingPath="true" AllowAutoEmbedding="true" AlphaChannelName="$ID/"/>
       </Image>
     </Rectangle>
-    <TextFrame Self="myprefixuf3" ParentStory="myprefixue1" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 237.82677165354335 -166.29921259842524">
+    <TextFrame Self="u185" ParentStory="u188" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 237.82677165354335 -166.29921259842524">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="-76.06299212598424 -19.842519685039377" LeftDirection="-76.06299212598424 -19.842519685039377" RightDirection="-76.06299212598424 -19.842519685039377"/>
               <PathPointType Anchor="-76.06299212598424 -0.9448818897638205" LeftDirection="-76.06299212598424 -0.9448818897638205" RightDirection="-76.06299212598424 -0.9448818897638205"/>
               <PathPointType Anchor="182.83464566929132 -0.9448818897638205" LeftDirection="182.83464566929132 -0.9448818897638205" RightDirection="182.83464566929132 -0.9448818897638205"/>
@@ -122,15 +122,15 @@
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
     </TextFrame>
-    <TextFrame Self="myprefixu109" ParentStory="myprefixuf7" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 298.77165354330714 -98.26771653543307">
+    <TextFrame Self="u19c" ParentStory="u19f" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 298.77165354330714 -98.26771653543307">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="-137.00787401574803 -64.25196850393701" LeftDirection="-137.00787401574803 -64.25196850393701" RightDirection="-137.00787401574803 -64.25196850393701"/>
               <PathPointType Anchor="-137.00787401574803 51.968503937007945" LeftDirection="-137.00787401574803 51.968503937007945" RightDirection="-137.00787401574803 51.968503937007945"/>
               <PathPointType Anchor="121.88976377952753 51.968503937007945" LeftDirection="121.88976377952753 51.968503937007945" RightDirection="121.88976377952753 51.968503937007945"/>
@@ -148,15 +148,15 @@
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
     </TextFrame>
-    <TextFrame Self="myprefixu11f" ParentStory="myprefixu10d" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 16.062992125984294 -357.16535433070874">
+    <TextFrame Self="u1d4" ParentStory="u1db" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 16.062992125984294 -357.16535433070874">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="141.73228346456693 19.84251968503935" LeftDirection="141.73228346456693 19.84251968503935" RightDirection="141.73228346456693 19.84251968503935"/>
               <PathPointType Anchor="141.73228346456693 310.8661417322836" LeftDirection="141.73228346456693 310.8661417322836" RightDirection="141.73228346456693 310.8661417322836"/>
               <PathPointType Anchor="409.13385826771633 310.8661417322836" LeftDirection="409.13385826771633 310.8661417322836" RightDirection="409.13385826771633 310.8661417322836"/>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/Story_myprefixu10d.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml`

 * *Files 20% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/Story_myprefixu10d.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u1db.xml`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Story Self="myprefixu10d" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
+  <Story Self="u1db" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
-    <XMLElement Self="myprefixdi3i4" MarkupTag="XMLTag/module" XMLContent="myprefixu10d">
-      <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
-        <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]">
-          <XMLElement Self="myprefixdi3i4i1" MarkupTag="XMLTag/main_picture" XMLContent="myprefixu14a">
-            <XMLAttribute Self="myprefixdi3i4i1XMLAttributenhref" Name="href" Value="file:///Users/stan/Dropbox/Projets/Slashdev/SimpleIDML/repos/git/simpleidml/tests/regressiontests/IDML/media/default.jpg"/>
+    <XMLElement Self="di3i12" MarkupTag="XMLTag/module" XMLContent="u1db">
+      <ParagraphStyleRange AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle">
+        <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]">
+          <XMLElement Self="di3i12i1" MarkupTag="XMLTag/main_picture" XMLContent="u216">
+            <XMLAttribute Self="di3i12i1XMLAttributenhref" Name="href" Value="file:///Users/stan/Dropbox/Projets/Slashdev/SimpleIDML/repos/git/simpleidml/tests/regressiontests/IDML/media/default.jpg"/>
           </XMLElement>
-          <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1"/>
-          <XMLElement Self="myprefixdi3i4i3" MarkupTag="XMLTag/Story" XMLContent="myprefixuf7"/>
+          <XMLElement Self="di3i12i2" MarkupTag="XMLTag/headline" XMLContent="u188"/>
+          <XMLElement Self="di3i12i3" MarkupTag="XMLTag/Story" XMLContent="u19f"/>
         </CharacterStyleRange>
       </ParagraphStyleRange>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/Story_myprefixue1.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml`

 * *Files 25% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/Stories/Story_myprefixue1.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/BackingStory.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
-<idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Story Self="myprefixue1" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
-    <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
-    <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
-    <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1">
-      <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
-        <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" FillColor="myprefixColor/uba" FontStyle="Bold">
-          <Content>The Life Aquatic with Steve Zissou</Content>
-        </CharacterStyleRange>
-      </ParagraphStyleRange>
-    </XMLElement>
-  </Story>
-</idPkg:Story>
+<idPkg:BackingStory xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
+  <XmlStory Self="u83" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
+    <ParagraphStyleRange AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle">
+      <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]">
+        <Content>﻿</Content>
+        <XMLElement Self="di3" MarkupTag="XMLTag/Root">
+          <XMLElement Self="di3i12" MarkupTag="XMLTag/module" XMLContent="u1db"/>
+        </XMLElement>
+        <Content>﻿﻿</Content>
+      </CharacterStyleRange>
+    </ParagraphStyleRange>
+  </XmlStory>
+</idPkg:BackingStory>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/XML/Tags.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/Tags.xml`

 * *Files 7% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/XML/Tags.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/XML/Tags.xml`

```diff
@@ -1,53 +1,43 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Tags xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
   <XMLTag Self="XMLTag/article" Name="article">
     <Properties>
       <TagColor type="enumeration">Blue</TagColor>
     </Properties>
   </XMLTag>
-  <XMLTag Self="XMLTag/bold" Name="bold">
-    <Properties>
-      <TagColor type="enumeration">LightBlue</TagColor>
-    </Properties>
-  </XMLTag>
   <XMLTag Self="XMLTag/headline" Name="headline">
     <Properties>
       <TagColor type="enumeration">Green</TagColor>
     </Properties>
   </XMLTag>
   <XMLTag Self="XMLTag/informations" Name="informations">
     <Properties>
       <TagColor type="enumeration">GridOrange</TagColor>
     </Properties>
   </XMLTag>
-  <XMLTag Self="XMLTag/italique" Name="italique">
-    <Properties>
-      <TagColor type="enumeration">LightBlue</TagColor>
-    </Properties>
-  </XMLTag>
   <XMLTag Self="XMLTag/main_picture" Name="main_picture">
     <Properties>
       <TagColor type="enumeration">Red</TagColor>
     </Properties>
   </XMLTag>
   <XMLTag Self="XMLTag/module" Name="module">
     <Properties>
       <TagColor type="enumeration">LightGray</TagColor>
     </Properties>
   </XMLTag>
-  <XMLTag Self="XMLTag/Root" Name="Root">
+  <XMLTag Self="XMLTag/MyBoldTag" Name="MyBoldTag">
     <Properties>
       <TagColor type="enumeration">LightBlue</TagColor>
     </Properties>
   </XMLTag>
-  <XMLTag Self="XMLTag/Story" Name="Story">
+  <XMLTag Self="XMLTag/Root" Name="Root">
     <Properties>
-      <TagColor type="enumeration">BrickRed</TagColor>
+      <TagColor type="enumeration">LightBlue</TagColor>
     </Properties>
   </XMLTag>
-  <XMLTag Self="XMLTag/sup" Name="sup">
+  <XMLTag Self="XMLTag/Story" Name="Story">
     <Properties>
-      <TagColor type="enumeration">Red</TagColor>
+      <TagColor type="enumeration">BrickRed</TagColor>
     </Properties>
   </XMLTag>
 </idPkg:Tags>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/designmap.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/designmap.xml`

 * *Files 18% similar despite different names*

#### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br/designmap.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/designmap.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<?aid style="50" type="document" readerVersion="6.0" featureSet="257" product="7.5(142)" ?>
-<Document xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0" Self="d" StoryList="myprefixue1 myprefixuf7 myprefixu10d myprefixu83" ZeroPoint="0 0" ActiveLayer="myprefixua4" CMYKProfile="$ID/" RGBProfile="$ID/" SolidColorIntent="UseColorSettings" AfterBlendingIntent="UseColorSettings" DefaultImageIntent="UseColorSettings" RGBPolicy="ColorPolicyOff" CMYKPolicy="ColorPolicyOff" AccurateLABSpots="false">
+<?aid style="50" type="document" readerVersion="6.0" featureSet="257" product="10.0(70)" ?>
+<Document xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0" Self="d" StoryList="u188 u19f u1db u83" ZeroPoint="0 0" ActiveLayer="ua4" CMYKProfile="$ID/" RGBProfile="$ID/" SolidColorIntent="UseColorSettings" AfterBlendingIntent="UseColorSettings" DefaultImageIntent="UseColorSettings" RGBPolicy="ColorPolicyOff" CMYKPolicy="ColorPolicyOff" AccurateLABSpots="false">
   <Language Self="Language/$ID/French" Name="$ID/French" SingleQuotes="‘’" DoubleQuotes="«»" PrimaryLanguageName="$ID/French" SublanguageName="$ID/" Id="274" HyphenationVendor="Proximity" SpellingVendor="Proximity"/>
   <Language Self="Language/$ID/English%3a UK" Name="$ID/English: UK" SingleQuotes="‘’" DoubleQuotes="“”" PrimaryLanguageName="$ID/English" SublanguageName="$ID/UK" Id="525" HyphenationVendor="Proximity" SpellingVendor="Proximity"/>
   <idPkg:Graphic src="Resources/Graphic.xml"/>
   <idPkg:Fonts src="Resources/Fonts.xml"/>
   <idPkg:Styles src="Resources/Styles.xml"/>
   <NumberingList Self="NumberingList/$ID/[Default]" Name="$ID/[Default]" ContinueNumbersAcrossStories="false" ContinueNumbersAcrossDocuments="false"/>
   <NamedGrid Self="NamedGrid/$ID/[Page Grid]" Name="$ID/[Page Grid]">
@@ -44,110 +44,110 @@
   <TextVariable Self="dTextVariablenModification Date" Name="Modification Date" VariableType="ModificationDateType">
     <DateVariablePreference TextBefore="" Format="d MMMM yyyy h:mm aa" TextAfter=""/>
   </TextVariable>
   <TextVariable Self="dTextVariablenOutput Date" Name="Output Date" VariableType="OutputDateType">
     <DateVariablePreference TextBefore="" Format="dd/MM/yy" TextAfter=""/>
   </TextVariable>
   <TextVariable Self="dTextVariablenRunning Header" Name="Running Header" VariableType="MatchParagraphStyleType">
-    <MatchParagraphStylePreference TextBefore="" TextAfter="" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" SearchStrategy="FirstOnPage" ChangeCase="None" DeleteEndPunctuation="false"/>
+    <MatchParagraphStylePreference TextBefore="" TextAfter="" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" SearchStrategy="FirstOnPage" ChangeCase="None" DeleteEndPunctuation="false"/>
   </TextVariable>
   <idPkg:Tags src="XML/Tags.xml"/>
-  <Layer Self="myprefixua4" Name="Layer 1" Visible="true" Locked="false" IgnoreWrap="false" ShowGuides="true" LockGuides="false" UI="true" Expendable="true" Printable="true">
+  <Layer Self="ua4" Name="Layer 1" Visible="true" Locked="false" IgnoreWrap="false" ShowGuides="true" LockGuides="false" UI="true" Expendable="true" Printable="true">
     <Properties>
       <LayerColor type="enumeration">LightBlue</LayerColor>
     </Properties>
   </Layer>
   <idPkg:MasterSpread src="MasterSpreads/MasterSpread_ua5.xml"/>
-  <idPkg:Spread src="Spreads/Spread_myprefixud8.xml"/>
-  <Section Self="u9b" Length="1" AlternateLayoutLength="1" AlternateLayout="Personnalisées V" Name="" ContinueNumbering="true" IncludeSectionPrefix="false" Marker="" PageStart="myprefixudd" SectionPrefix="">
+  <idPkg:Spread src="Spreads/Spread_ud6.xml"/>
+  <Section Self="u9b" Length="1" AlternateLayoutLength="1" AlternateLayout="Personnalisées V" Name="" ContinueNumbering="true" IncludeSectionPrefix="false" Marker="" PageStart="udb" SectionPrefix="">
     <Properties>
       <PageNumberStyle type="enumeration">Arabic</PageNumberStyle>
     </Properties>
   </Section>
   <DocumentUser Self="dDocumentUser0" UserName="$ID/Unknown User Name">
     <Properties>
       <UserColor type="enumeration">Gold</UserColor>
     </Properties>
   </DocumentUser>
   <DocumentUser Self="dDocumentUser1" UserName="$ID/Unknown User Name">
     <Properties>
       <UserColor type="enumeration">Gold</UserColor>
     </Properties>
   </DocumentUser>
-  <CrossReferenceFormat Self="u122" Name="Full Paragraph &amp; Page Number" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u122BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u122BuildingBlock1" BlockType="FullParagraphBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u122BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot; on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u122BuildingBlock3" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u123" Name="Full Paragraph" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u123BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u123BuildingBlock1" BlockType="FullParagraphBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u123BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u124" Name="Paragraph Text &amp; Page Number" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u124BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u124BuildingBlock1" BlockType="ParagraphTextBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u124BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot; on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u124BuildingBlock3" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u125" Name="Paragraph Text" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u125BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u125BuildingBlock1" BlockType="ParagraphTextBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u125BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u126" Name="Paragraph Number &amp; Page Number" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u126BuildingBlock0" BlockType="ParagraphNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u126BuildingBlock1" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText=" on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u126BuildingBlock2" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u127" Name="Paragraph Number" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u127BuildingBlock0" BlockType="ParagraphNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u128" Name="Text Anchor Name &amp; Page Number" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u128BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u128BuildingBlock1" BlockType="BookmarkNameBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u128BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot; on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u128BuildingBlock3" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u129" Name="Text Anchor Name" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u129BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u129BuildingBlock1" BlockType="BookmarkNameBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u129BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-  </CrossReferenceFormat>
-  <CrossReferenceFormat Self="u12a" Name="Page Number" AppliedCharacterStyle="n">
-    <BuildingBlock Self="u12aBuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
-    <BuildingBlock Self="u12aBuildingBlock1" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  <CrossReferenceFormat Self="u10c" Name="Full Paragraph &amp; Page Number" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u10cBuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10cBuildingBlock1" BlockType="FullParagraphBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10cBuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot; on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10cBuildingBlock3" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u10d" Name="Full Paragraph" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u10dBuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10dBuildingBlock1" BlockType="FullParagraphBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10dBuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u10e" Name="Paragraph Text &amp; Page Number" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u10eBuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10eBuildingBlock1" BlockType="ParagraphTextBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10eBuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot; on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10eBuildingBlock3" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u10f" Name="Paragraph Text" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u10fBuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10fBuildingBlock1" BlockType="ParagraphTextBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u10fBuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u110" Name="Paragraph Number &amp; Page Number" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u110BuildingBlock0" BlockType="ParagraphNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u110BuildingBlock1" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText=" on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u110BuildingBlock2" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u111" Name="Paragraph Number" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u111BuildingBlock0" BlockType="ParagraphNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u112" Name="Text Anchor Name &amp; Page Number" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u112BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u112BuildingBlock1" BlockType="BookmarkNameBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u112BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot; on page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u112BuildingBlock3" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u113" Name="Text Anchor Name" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u113BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u113BuildingBlock1" BlockType="BookmarkNameBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u113BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+  </CrossReferenceFormat>
+  <CrossReferenceFormat Self="u114" Name="Page Number" AppliedCharacterStyle="n">
+    <BuildingBlock Self="u114BuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
+    <BuildingBlock Self="u114BuildingBlock1" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
   </CrossReferenceFormat>
   <idPkg:BackingStory src="XML/BackingStory.xml"/>
-  <idPkg:Story src="Stories/Story_myprefixu10d.xml"/>
-  <idPkg:Story src="Stories/Story_myprefixuf7.xml"/>
-  <idPkg:Story src="Stories/Story_myprefixue1.xml"/>
+  <idPkg:Story src="Stories/Story_u1db.xml"/>
+  <idPkg:Story src="Stories/Story_u19f.xml"/>
+  <idPkg:Story src="Stories/Story_u188.xml"/>
   <idPkg:Mapping src="XML/Mapping.xml"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Symbol" Name="$ID/kIndexGroup_Symbol" Include="true" Priority="0" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Alphabet" Name="$ID/kIndexGroup_Alphabet" Include="true" Priority="1" HeaderType="BasicLatin"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Numeric" Name="$ID/kIndexGroup_Numeric" Include="false" Priority="2" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_GreekAlphabet" Name="$ID/kWRIndexGroup_GreekAlphabet" Include="false" Priority="3" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_CyrillicAlphabet" Name="$ID/kWRIndexGroup_CyrillicAlphabet" Include="false" Priority="4" HeaderType="Russian"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Kana" Name="$ID/kIndexGroup_Kana" Include="false" Priority="5" HeaderType="HiraganaAll"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Chinese" Name="$ID/kIndexGroup_Chinese" Include="false" Priority="6" HeaderType="ChinesePinyin"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Korean" Name="$ID/kIndexGroup_Korean" Include="false" Priority="7" HeaderType="KoreanConsonant"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_ArabicAlphabet" Name="$ID/kWRIndexGroup_ArabicAlphabet" Include="false" Priority="8" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_HebrewAlphabet" Name="$ID/kWRIndexGroup_HebrewAlphabet" Include="false" Priority="9" HeaderType="Nothing"/>
-  <ColorGroup Self="myprefixu143" Name="[Root Color Group]" IsRootColorGroup="true">
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch0" SwatchItemRef="Swatch/None"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch1" SwatchItemRef="Color/Registration"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch2" SwatchItemRef="Color/Paper"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch3" SwatchItemRef="Color/Black"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch4" SwatchItemRef="Color/C=0 M=0 Y=100 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch5" SwatchItemRef="Color/C=0 M=100 Y=0 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch6" SwatchItemRef="Color/C=100 M=0 Y=0 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch7" SwatchItemRef="Color/C=100 M=90 Y=10 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch8" SwatchItemRef="Color/C=15 M=100 Y=100 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch9" SwatchItemRef="Color/C=75 M=5 Y=100 K=0"/>
+  <ColorGroup Self="u207" Name="[Root Color Group]" IsRootColorGroup="true">
+    <ColorGroupSwatch Self="u207ColorGroupSwatch0" SwatchItemRef="Swatch/None"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch1" SwatchItemRef="Color/Registration"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch2" SwatchItemRef="Color/Paper"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch3" SwatchItemRef="Color/Black"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch4" SwatchItemRef="Color/C=0 M=0 Y=100 K=0"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch5" SwatchItemRef="Color/C=0 M=100 Y=0 K=0"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch6" SwatchItemRef="Color/C=100 M=0 Y=0 K=0"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch7" SwatchItemRef="Color/C=100 M=90 Y=10 K=0"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch8" SwatchItemRef="Color/C=15 M=100 Y=100 K=0"/>
+    <ColorGroupSwatch Self="u207ColorGroupSwatch9" SwatchItemRef="Color/C=75 M=5 Y=100 K=0"/>
   </ColorGroup>
   <ABullet Self="dABullet0" CharacterType="UnicodeOnly" CharacterValue="8226">
     <Properties>
       <BulletsFont type="string">$ID/</BulletsFont>
       <BulletsFontStyle type="string">$ID/</BulletsFontStyle>
     </Properties>
   </ABullet>
```

### Comparing `SimpleIDML-1.1.3/tests/article-1photo_import-xml-with-setcontent-remove-br.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml`

 * *Files 0% similar despite different names*

#### zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 207919 bytes, number of entries: 16
--rw-rw-r--  2.0 unx    16258 b- stor 20-Jun-08 12:38 designmap.xml
--rw-rw-r--  2.0 unx       43 b- stor 20-Jun-08 12:38 mimetype
--rw-rw-r--  2.0 unx     1399 b- stor 20-Jun-08 12:38 Stories/Story_myprefixu10d.xml
--rw-rw-r--  2.0 unx     3145 b- stor 20-Jun-08 12:38 Stories/Story_myprefixuf7.xml
--rw-rw-r--  2.0 unx      999 b- stor 20-Jun-08 12:38 Stories/Story_myprefixue1.xml
--rw-rw-r--  2.0 unx    19391 b- stor 20-Jun-08 12:38 Spreads/Spread_myprefixud8.xml
--rw-rw-r--  2.0 unx     7501 b- stor 20-Jun-08 12:38 Resources/Graphic.xml
--rw-rw-r--  2.0 unx    36650 b- stor 20-Jun-08 12:38 Resources/Styles.xml
--rw-rw-r--  2.0 unx    73533 b- stor 20-Jun-08 12:38 Resources/Preferences.xml
--rw-rw-r--  2.0 unx    15600 b- stor 20-Jun-08 12:38 Resources/Fonts.xml
--rw-rw-r--  2.0 unx      253 b- stor 20-Jun-08 12:38 META-INF/container.xml
--rw-rw-r--  2.0 unx    25750 b- stor 20-Jun-08 12:38 META-INF/metadata.xml
--rw-rw-r--  2.0 unx     2622 b- stor 20-Jun-08 12:38 MasterSpreads/MasterSpread_ua5.xml
--rw-rw-r--  2.0 unx      785 b- stor 20-Jun-08 12:38 XML/BackingStory.xml
--rw-rw-r--  2.0 unx      491 b- stor 20-Jun-08 12:38 XML/Mapping.xml
--rw-rw-r--  2.0 unx     1565 b- stor 20-Jun-08 12:38 XML/Tags.xml
-16 files, 205985 bytes uncompressed, 205985 bytes compressed:  0.0%
+Zip file size: 208159 bytes, number of entries: 16
+-rw-r--r--  2.0 unx    16250 b- stor 14-Sep-24 15:18 designmap.xml
+-rw-r--r--  2.0 unx       43 b- stor 14-Sep-24 15:18 mimetype
+-rw-r--r--  2.0 unx     2622 b- stor 14-Sep-24 15:18 MasterSpreads/MasterSpread_ua5.xml
+-rw-r--r--  2.0 unx      253 b- stor 14-Sep-24 15:18 META-INF/container.xml
+-rw-r--r--  2.0 unx    25750 b- stor 14-Sep-24 15:18 META-INF/metadata.xml
+-rw-r--r--  2.0 unx    15600 b- stor 14-Sep-24 15:18 Resources/Fonts.xml
+-rw-r--r--  2.0 unx     7501 b- stor 14-Sep-24 15:18 Resources/Graphic.xml
+-rw-r--r--  2.0 unx    73533 b- stor 14-Sep-24 15:18 Resources/Preferences.xml
+-rw-r--r--  2.0 unx    36650 b- stor 14-Sep-24 15:18 Resources/Styles.xml
+-rw-r--r--  2.0 unx    19307 b- stor 14-Sep-24 15:18 Spreads/Spread_myprefixud8.xml
+-rw-r--r--  2.0 unx     1313 b- stor 14-Sep-24 15:18 Stories/Story_myprefixu10d.xml
+-rw-r--r--  2.0 unx     1097 b- stor 14-Sep-24 15:18 Stories/Story_myprefixue1.xml
+-rw-r--r--  2.0 unx     3465 b- stor 14-Sep-24 15:18 Stories/Story_myprefixuf7.xml
+-rw-r--r--  2.0 unx      785 b- stor 14-Sep-24 15:18 XML/BackingStory.xml
+-rw-r--r--  2.0 unx      491 b- stor 14-Sep-24 15:18 XML/Mapping.xml
+-rw-r--r--  2.0 unx     1565 b- stor 14-Sep-24 15:18 XML/Tags.xml
+16 files, 206225 bytes uncompressed, 206225 bytes compressed:  0.0%
```

#### zipnote «TEMP»/diffoscope_nwk2mihn_/tmp6zlnlnb0_.zip

```diff
@@ -1,44 +1,44 @@
 Filename: designmap.xml
 Comment: 
 
 Filename: mimetype
 Comment: 
 
-Filename: Stories/Story_myprefixu10d.xml
+Filename: MasterSpreads/MasterSpread_ua5.xml
 Comment: 
 
-Filename: Stories/Story_myprefixuf7.xml
+Filename: META-INF/container.xml
 Comment: 
 
-Filename: Stories/Story_myprefixue1.xml
+Filename: META-INF/metadata.xml
 Comment: 
 
-Filename: Spreads/Spread_myprefixud8.xml
+Filename: Resources/Fonts.xml
 Comment: 
 
 Filename: Resources/Graphic.xml
 Comment: 
 
-Filename: Resources/Styles.xml
+Filename: Resources/Preferences.xml
 Comment: 
 
-Filename: Resources/Preferences.xml
+Filename: Resources/Styles.xml
 Comment: 
 
-Filename: Resources/Fonts.xml
+Filename: Spreads/Spread_myprefixud8.xml
 Comment: 
 
-Filename: META-INF/container.xml
+Filename: Stories/Story_myprefixu10d.xml
 Comment: 
 
-Filename: META-INF/metadata.xml
+Filename: Stories/Story_myprefixue1.xml
 Comment: 
 
-Filename: MasterSpreads/MasterSpread_ua5.xml
+Filename: Stories/Story_myprefixuf7.xml
 Comment: 
 
 Filename: XML/BackingStory.xml
 Comment: 
 
 Filename: XML/Mapping.xml
 Comment:
```

#### designmap.xml

##### designmap.xml

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <?aid style="50" type="document" readerVersion="6.0" featureSet="257" product="7.5(142)" ?>
-<Document xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0" Self="d" StoryList="myprefixue1 myprefixuf7 myprefixu10d myprefixu83" ZeroPoint="0 0" ActiveLayer="myprefixua4" CMYKProfile="$ID/" RGBProfile="$ID/" SolidColorIntent="UseColorSettings" AfterBlendingIntent="UseColorSettings" DefaultImageIntent="UseColorSettings" RGBPolicy="ColorPolicyOff" CMYKPolicy="ColorPolicyOff" AccurateLABSpots="false">
+<Document xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0" Self="d" StoryList="myprefixue1 myprefixuf7 myprefixu10d myprefixu83" ZeroPoint="0 0" ActiveLayer="ua4" CMYKProfile="$ID/" RGBProfile="$ID/" SolidColorIntent="UseColorSettings" AfterBlendingIntent="UseColorSettings" DefaultImageIntent="UseColorSettings" RGBPolicy="ColorPolicyOff" CMYKPolicy="ColorPolicyOff" AccurateLABSpots="false">
   <Language Self="Language/$ID/French" Name="$ID/French" SingleQuotes="‘’" DoubleQuotes="«»" PrimaryLanguageName="$ID/French" SublanguageName="$ID/" Id="274" HyphenationVendor="Proximity" SpellingVendor="Proximity"/>
   <Language Self="Language/$ID/English%3a UK" Name="$ID/English: UK" SingleQuotes="‘’" DoubleQuotes="“”" PrimaryLanguageName="$ID/English" SublanguageName="$ID/UK" Id="525" HyphenationVendor="Proximity" SpellingVendor="Proximity"/>
   <idPkg:Graphic src="Resources/Graphic.xml"/>
   <idPkg:Fonts src="Resources/Fonts.xml"/>
   <idPkg:Styles src="Resources/Styles.xml"/>
   <NumberingList Self="NumberingList/$ID/[Default]" Name="$ID/[Default]" ContinueNumbersAcrossStories="false" ContinueNumbersAcrossDocuments="false"/>
   <NamedGrid Self="NamedGrid/$ID/[Page Grid]" Name="$ID/[Page Grid]">
```

#### Stories/Story_myprefixu10d.xml

##### Stories/Story_myprefixu10d.xml

```diff
@@ -3,15 +3,15 @@
   <Story Self="myprefixu10d" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
     <XMLElement Self="myprefixdi3i4" MarkupTag="XMLTag/module" XMLContent="myprefixu10d">
       <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
         <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]">
           <XMLElement Self="myprefixdi3i4i1" MarkupTag="XMLTag/main_picture" XMLContent="myprefixu14a">
-            <XMLAttribute Self="myprefixdi3i4i1XMLAttributenhref" Name="href" Value="file:///Users/stan/Dropbox/Projets/Slashdev/SimpleIDML/repos/git/simpleidml/tests/regressiontests/IDML/media/default.jpg"/>
+            <XMLAttribute Self="myprefixdi3i4i1XMLAttributenhref" Name="href" Value="file:../../IDML/media/bouboune.jpg"/>
           </XMLElement>
           <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1"/>
           <XMLElement Self="myprefixdi3i4i3" MarkupTag="XMLTag/Story" XMLContent="myprefixuf7"/>
         </CharacterStyleRange>
       </ParagraphStyleRange>
     </XMLElement>
   </Story>
```

#### Stories/Story_myprefixuf7.xml

##### Stories/Story_myprefixuf7.xml

```diff
@@ -9,23 +9,21 @@
         <XMLElement Self="myprefixdi3i4i3i1" MarkupTag="XMLTag/article">
           <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10">
             <Content>While oceanographer and documentarian</Content>
           </CharacterStyleRange>
           <XMLElement MarkupTag="XMLTag/bold" Self="myprefixdi3i4i3i1i1">
             <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/bold" PointSize="10">
               <Properties/>
-              <Content>Steve Zissou (Bill Murray) is working on his latest documentary at sea,
-            his best friend Esteban du Plantier (Seymour Cassel)</Content>
+              <Content>Steve Zissou (Bill Murray) is working on his latest documentary at sea, his best friend Esteban du Plantier (Seymour Cassel)</Content>
             </CharacterStyleRange>
           </XMLElement>
           <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10">
             <Properties/>
-            <Content>is eaten by a creature Zissou describes as a &quot;Jaguar shark.&quot;
-            For his next project, Zissou is determined to document the shark's destruction.
-                The crew aboard Zissou's research vessel</Content>
+            <Content>is eaten by a creature Zissou describes as a &quot;Jaguar shark.&quot; For his next project, Zissou is determined to document the shark's destruction.
+            The crew aboard Zissou's research vessel</Content>
           </CharacterStyleRange>
           <XMLElement MarkupTag="XMLTag/italique" Self="myprefixdi3i4i3i1i2">
             <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/italique" PointSize="10">
               <Properties/>
               <Content>Belafonte</Content>
             </CharacterStyleRange>
           </XMLElement>
@@ -37,20 +35,23 @@
             <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/italique" PointSize="10">
               <Properties/>
               <Content>Pelé dos Santos (Seu Jorge)</Content>
             </CharacterStyleRange>
           </XMLElement>
           <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10">
             <Properties/>
-            <Content>,
-                    a safety expert and Brazilian musician who sings David Bowie songs in Portuguese, and Klaus Daimler (Willem Dafoe),
-                    the German second-in-command who viewed Zissou and Esteban as father figures.</Content>
+            <Content>, a safety expert and Brazilian musician who sings David Bowie songs in Portuguese, and Klaus Daimler (Willem Dafoe), the German second-in-command who viewed Zissou and Esteban as father figures</Content>
           </CharacterStyleRange>
         </XMLElement>
         <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]">
           <Br/>
           <Br/>
         </CharacterStyleRange>
+        <XMLElement Self="myprefixdi3i4i3i2" MarkupTag="XMLTag/informations">
+          <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" FontStyle="Italic" PointSize="10">
+            <Content>The Life Aquatic with Steve Zissou is an American comedy-drama film directed, written, and co-produced by Wes Anderson.</Content>
+          </CharacterStyleRange>
+        </XMLElement>
       </ParagraphStyleRange>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

#### Stories/Story_myprefixue1.xml

##### Stories/Story_myprefixue1.xml

```diff
@@ -2,13 +2,14 @@
 <idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
   <Story Self="myprefixue1" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
     <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1">
       <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
         <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" FillColor="myprefixColor/uba" FontStyle="Bold">
-          <Content>The Life Aquatic with Steve Zissou</Content>
+          <Content>THE HEADLINE HERE</Content>
         </CharacterStyleRange>
       </ParagraphStyleRange>
+      <XMLAttribute Name="simpleidml-setcontent" Self="myprefixdi3i4i2XMLAttributensimpleidml-setcontent" Value="false"/>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

#### Spreads/Spread_myprefixud8.xml

##### Spreads/Spread_myprefixud8.xml

```diff
@@ -91,15 +91,15 @@
          &lt;/exif:ComponentsConfiguration&gt;
       &lt;/rdf:Description&gt;
    &lt;/rdf:RDF&gt;
 &lt;/x:xmpmeta&gt;
 &lt;?xpacket end=&quot;r&quot;?&gt;</Contents>
           </Properties>
         </MetadataPacketPreference>
-        <Link Self="myprefixu14e" AssetURL="$ID/" AssetID="$ID/" LinkResourceURI="file:/Users/stan/Dropbox/Projets/Slashdev/SimpleIDML/repos/git/simpleidml/tests/regressiontests/IDML/media/default.jpg" LinkResourceFormat="$ID/JPEG" StoredState="Normal" LinkClassID="35906" LinkClientID="257" LinkResourceModified="false" LinkObjectModified="false" ShowInUI="true" CanEmbed="true" CanUnembed="true" CanPackage="true" ImportPolicy="NoAutoImport" ExportPolicy="NoAutoExport" LinkImportStamp="file 129767622980000000 27644" LinkImportModificationTime="2012-03-21T01:11:38" LinkImportTime="2014-09-24T14:59:30" LinkResourceSize="0~6bfc"/>
+        <Link Self="myprefixu14e" AssetURL="$ID/" AssetID="$ID/" LinkResourceURI="file:../../IDML/media/bouboune.jpg" LinkResourceFormat="$ID/JPEG" StoredState="Normal" LinkClassID="35906" LinkClientID="257" LinkResourceModified="false" LinkObjectModified="false" ShowInUI="true" CanEmbed="true" CanUnembed="true" CanPackage="true" ImportPolicy="NoAutoImport" ExportPolicy="NoAutoExport" LinkImportStamp="file 129767622980000000 27644" LinkImportModificationTime="2012-03-21T01:11:38" LinkImportTime="2014-09-24T14:59:30" LinkResourceSize="0~6bfc"/>
         <ClippingPathSettings ClippingType="None" InvertPath="false" IncludeInsideEdges="false" RestrictToFrame="false" UseHighResolutionImage="true" Threshold="25" Tolerance="2" InsetFrame="0" AppliedPathName="$ID/" Index="-1"/>
         <ImageIOPreference ApplyPhotoshopClippingPath="true" AllowAutoEmbedding="true" AlphaChannelName="$ID/"/>
       </Image>
     </Rectangle>
     <TextFrame Self="myprefixuf3" ParentStory="myprefixue1" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 237.82677165354335 -166.29921259842524">
       <Properties>
         <PathGeometry>
```

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-0photo.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-0photo.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-0photo.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo-elts-same-layer.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/2articles-1photo.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/2articles-1photo.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages-layers-with-guides.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages-layers-with-guides.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages-layers-with-guides.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/4-pages.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/4-pages.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/META-INF/metadata.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u188.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo/Stories/Story_u19f.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo-package.zip` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-package.zip`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo-with-attributes.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo-with-attributes.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo-with-attributes.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_import-xml.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_import-xml.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_import-xml.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-nested-xml.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-xml.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/article-1photo_imported-xml.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/article-1photo_imported-xml.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-0-photo-complex.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-complex.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo-elts-same-layer.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/4-pages-insert-article-1-photo.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent2.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-forcecontent3.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-ignorecontent.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-nested-tags.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2-prefixed.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-extra-nodes2.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-with-setcontent-false.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 208159 bytes, number of entries: 16
--rw-r--r--  2.0 unx    16250 b- stor 14-Sep-24 15:18 designmap.xml
--rw-r--r--  2.0 unx       43 b- stor 14-Sep-24 15:18 mimetype
--rw-r--r--  2.0 unx     2622 b- stor 14-Sep-24 15:18 MasterSpreads/MasterSpread_ua5.xml
--rw-r--r--  2.0 unx      253 b- stor 14-Sep-24 15:18 META-INF/container.xml
--rw-r--r--  2.0 unx    25750 b- stor 14-Sep-24 15:18 META-INF/metadata.xml
--rw-r--r--  2.0 unx    15600 b- stor 14-Sep-24 15:18 Resources/Fonts.xml
--rw-r--r--  2.0 unx     7501 b- stor 14-Sep-24 15:18 Resources/Graphic.xml
--rw-r--r--  2.0 unx    73533 b- stor 14-Sep-24 15:18 Resources/Preferences.xml
--rw-r--r--  2.0 unx    36650 b- stor 14-Sep-24 15:18 Resources/Styles.xml
--rw-r--r--  2.0 unx    19307 b- stor 14-Sep-24 15:18 Spreads/Spread_myprefixud8.xml
--rw-r--r--  2.0 unx     1313 b- stor 14-Sep-24 15:18 Stories/Story_myprefixu10d.xml
--rw-r--r--  2.0 unx     1097 b- stor 14-Sep-24 15:18 Stories/Story_myprefixue1.xml
--rw-r--r--  2.0 unx     3465 b- stor 14-Sep-24 15:18 Stories/Story_myprefixuf7.xml
--rw-r--r--  2.0 unx      785 b- stor 14-Sep-24 15:18 XML/BackingStory.xml
--rw-r--r--  2.0 unx      491 b- stor 14-Sep-24 15:18 XML/Mapping.xml
--rw-r--r--  2.0 unx     1565 b- stor 14-Sep-24 15:18 XML/Tags.xml
-16 files, 206225 bytes uncompressed, 206225 bytes compressed:  0.0%
+Zip file size: 204178 bytes, number of entries: 16
+-rw-r--r--  2.0 unx    16250 b- stor 14-Sep-24 15:19 designmap.xml
+-rw-r--r--  2.0 unx       43 b- stor 14-Sep-24 15:19 mimetype
+-rw-r--r--  2.0 unx     2622 b- stor 14-Sep-24 15:19 MasterSpreads/MasterSpread_ua5.xml
+-rw-r--r--  2.0 unx      253 b- stor 14-Sep-24 15:19 META-INF/container.xml
+-rw-r--r--  2.0 unx    25750 b- stor 14-Sep-24 15:19 META-INF/metadata.xml
+-rw-r--r--  2.0 unx    15600 b- stor 14-Sep-24 15:19 Resources/Fonts.xml
+-rw-r--r--  2.0 unx     7501 b- stor 14-Sep-24 15:19 Resources/Graphic.xml
+-rw-r--r--  2.0 unx    73533 b- stor 14-Sep-24 15:19 Resources/Preferences.xml
+-rw-r--r--  2.0 unx    36650 b- stor 14-Sep-24 15:19 Resources/Styles.xml
+-rw-r--r--  2.0 unx    15566 b- stor 14-Sep-24 15:19 Spreads/Spread_myprefixud8.xml
+-rw-r--r--  2.0 unx     1171 b- stor 14-Sep-24 15:19 Stories/Story_myprefixu10d.xml
+-rw-r--r--  2.0 unx      999 b- stor 14-Sep-24 15:19 Stories/Story_myprefixue1.xml
+-rw-r--r--  2.0 unx     3465 b- stor 14-Sep-24 15:19 Stories/Story_myprefixuf7.xml
+-rw-r--r--  2.0 unx      785 b- stor 14-Sep-24 15:19 XML/BackingStory.xml
+-rw-r--r--  2.0 unx      491 b- stor 14-Sep-24 15:19 XML/Mapping.xml
+-rw-r--r--  2.0 unx     1565 b- stor 14-Sep-24 15:19 XML/Tags.xml
+16 files, 202244 bytes uncompressed, 202244 bytes compressed:  0.0%
```

#### Spreads/Spread_myprefixud8.xml

##### Spreads/Spread_myprefixud8.xml

```diff
@@ -48,61 +48,14 @@
       <FrameFittingOption RightCrop="44.102362204724386" BottomCrop="219.1181102362204"/>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
-      <Image Self="myprefixu14a" Space="$ID/#Links_RGB" ActualPpi="72 72" EffectivePpi="72 72" ImageRenderingIntent="UseColorSettings" OverriddenPageItemProps="" LocalDisplaySetting="Default" ImageTypeName="$ID/JPEG" AppliedObjectStyle="myprefixObjectStyle/$ID/[None]" ItemTransform="1 0 0 1 144.56692913385825 58.58267716535431" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" Visible="true" Name="$ID/">
-        <Properties>
-          <Profile type="string">$ID/None</Profile>
-          <GraphicBounds Left="0" Top="0" Right="303" Bottom="360"/>
-        </Properties>
-        <TextWrapPreference Inverse="false" ApplyToMasterPageOnly="false" TextWrapSide="BothSides" TextWrapMode="None">
-          <Properties>
-            <TextWrapOffset Top="0" Left="0" Bottom="0" Right="0"/>
-          </Properties>
-          <ContourOption ContourType="SameAsClipping" IncludeInsideEdges="false" ContourPathName="$ID/"/>
-        </TextWrapPreference>
-        <MetadataPacketPreference>
-          <Properties>
-            <Contents>&lt;?xpacket begin=&quot;﻿&quot; id=&quot;W5M0MpCehiHzreSzNTczkc9d&quot;?&gt;
-&lt;x:xmpmeta xmlns:x=&quot;adobe:ns:meta/&quot; x:xmptk=&quot;Adobe XMP Core 5.6-c011 79.156289, 2014/03/31-23:39:12        &quot;&gt;
-   &lt;rdf:RDF xmlns:rdf=&quot;http://www.w3.org/1999/02/22-rdf-syntax-ns#&quot;&gt;
-      &lt;rdf:Description rdf:about=&quot;&quot;
-            xmlns:tiff=&quot;http://ns.adobe.com/tiff/1.0/&quot;
-            xmlns:exif=&quot;http://ns.adobe.com/exif/1.0/&quot;&gt;
-         &lt;tiff:XResolution&gt;72/1&lt;/tiff:XResolution&gt;
-         &lt;tiff:YResolution&gt;72/1&lt;/tiff:YResolution&gt;
-         &lt;tiff:ResolutionUnit&gt;2&lt;/tiff:ResolutionUnit&gt;
-         &lt;tiff:YCbCrPositioning&gt;1&lt;/tiff:YCbCrPositioning&gt;
-         &lt;exif:ColorSpace&gt;1&lt;/exif:ColorSpace&gt;
-         &lt;exif:PixelXDimension&gt;360&lt;/exif:PixelXDimension&gt;
-         &lt;exif:PixelYDimension&gt;303&lt;/exif:PixelYDimension&gt;
-         &lt;exif:SceneCaptureType&gt;0&lt;/exif:SceneCaptureType&gt;
-         &lt;exif:ExifVersion&gt;0221&lt;/exif:ExifVersion&gt;
-         &lt;exif:FlashpixVersion&gt;0100&lt;/exif:FlashpixVersion&gt;
-         &lt;exif:ComponentsConfiguration&gt;
-            &lt;rdf:Seq&gt;
-               &lt;rdf:li&gt;1&lt;/rdf:li&gt;
-               &lt;rdf:li&gt;2&lt;/rdf:li&gt;
-               &lt;rdf:li&gt;3&lt;/rdf:li&gt;
-               &lt;rdf:li&gt;0&lt;/rdf:li&gt;
-            &lt;/rdf:Seq&gt;
-         &lt;/exif:ComponentsConfiguration&gt;
-      &lt;/rdf:Description&gt;
-   &lt;/rdf:RDF&gt;
-&lt;/x:xmpmeta&gt;
-&lt;?xpacket end=&quot;r&quot;?&gt;</Contents>
-          </Properties>
-        </MetadataPacketPreference>
-        <Link Self="myprefixu14e" AssetURL="$ID/" AssetID="$ID/" LinkResourceURI="file:../../IDML/media/bouboune.jpg" LinkResourceFormat="$ID/JPEG" StoredState="Normal" LinkClassID="35906" LinkClientID="257" LinkResourceModified="false" LinkObjectModified="false" ShowInUI="true" CanEmbed="true" CanUnembed="true" CanPackage="true" ImportPolicy="NoAutoImport" ExportPolicy="NoAutoExport" LinkImportStamp="file 129767622980000000 27644" LinkImportModificationTime="2012-03-21T01:11:38" LinkImportTime="2014-09-24T14:59:30" LinkResourceSize="0~6bfc"/>
-        <ClippingPathSettings ClippingType="None" InvertPath="false" IncludeInsideEdges="false" RestrictToFrame="false" UseHighResolutionImage="true" Threshold="25" Tolerance="2" InsetFrame="0" AppliedPathName="$ID/" Index="-1"/>
-        <ImageIOPreference ApplyPhotoshopClippingPath="true" AllowAutoEmbedding="true" AlphaChannelName="$ID/"/>
-      </Image>
     </Rectangle>
     <TextFrame Self="myprefixuf3" ParentStory="myprefixue1" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 237.82677165354335 -166.29921259842524">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="-76.06299212598424 -19.842519685039377" LeftDirection="-76.06299212598424 -19.842519685039377" RightDirection="-76.06299212598424 -19.842519685039377"/>
```

#### Stories/Story_myprefixu10d.xml

##### Stories/Story_myprefixu10d.xml

```diff
@@ -2,17 +2,15 @@
 <idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
   <Story Self="myprefixu10d" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
     <XMLElement Self="myprefixdi3i4" MarkupTag="XMLTag/module" XMLContent="myprefixu10d">
       <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
         <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]">
-          <XMLElement Self="myprefixdi3i4i1" MarkupTag="XMLTag/main_picture" XMLContent="myprefixu14a">
-            <XMLAttribute Self="myprefixdi3i4i1XMLAttributenhref" Name="href" Value="file:../../IDML/media/bouboune.jpg"/>
-          </XMLElement>
+          <XMLElement Self="myprefixdi3i4i1" MarkupTag="XMLTag/main_picture"/>
           <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1"/>
           <XMLElement Self="myprefixdi3i4i3" MarkupTag="XMLTag/Story" XMLContent="myprefixuf7"/>
         </CharacterStyleRange>
       </ParagraphStyleRange>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

#### Stories/Story_myprefixue1.xml

##### Stories/Story_myprefixue1.xml

```diff
@@ -2,14 +2,13 @@
 <idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
   <Story Self="myprefixue1" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
     <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1">
       <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
         <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" FillColor="myprefixColor/uba" FontStyle="Bold">
-          <Content>THE HEADLINE HERE</Content>
+          <Content>The Life Aquatic with Steve Zissou</Content>
         </CharacterStyleRange>
       </ParagraphStyleRange>
-      <XMLAttribute Name="simpleidml-setcontent" Self="myprefixdi3i4i2XMLAttributensimpleidml-setcontent" Value="false"/>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/expected/article-1photo_import-xml-without-picture.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/expected/article-1photo_import-xml.idml`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 204178 bytes, number of entries: 16
--rw-r--r--  2.0 unx    16250 b- stor 14-Sep-24 15:19 designmap.xml
--rw-r--r--  2.0 unx       43 b- stor 14-Sep-24 15:19 mimetype
--rw-r--r--  2.0 unx     2622 b- stor 14-Sep-24 15:19 MasterSpreads/MasterSpread_ua5.xml
--rw-r--r--  2.0 unx      253 b- stor 14-Sep-24 15:19 META-INF/container.xml
--rw-r--r--  2.0 unx    25750 b- stor 14-Sep-24 15:19 META-INF/metadata.xml
--rw-r--r--  2.0 unx    15600 b- stor 14-Sep-24 15:19 Resources/Fonts.xml
--rw-r--r--  2.0 unx     7501 b- stor 14-Sep-24 15:19 Resources/Graphic.xml
--rw-r--r--  2.0 unx    73533 b- stor 14-Sep-24 15:19 Resources/Preferences.xml
--rw-r--r--  2.0 unx    36650 b- stor 14-Sep-24 15:19 Resources/Styles.xml
--rw-r--r--  2.0 unx    15566 b- stor 14-Sep-24 15:19 Spreads/Spread_myprefixud8.xml
--rw-r--r--  2.0 unx     1171 b- stor 14-Sep-24 15:19 Stories/Story_myprefixu10d.xml
--rw-r--r--  2.0 unx      999 b- stor 14-Sep-24 15:19 Stories/Story_myprefixue1.xml
--rw-r--r--  2.0 unx     3465 b- stor 14-Sep-24 15:19 Stories/Story_myprefixuf7.xml
--rw-r--r--  2.0 unx      785 b- stor 14-Sep-24 15:19 XML/BackingStory.xml
--rw-r--r--  2.0 unx      491 b- stor 14-Sep-24 15:19 XML/Mapping.xml
--rw-r--r--  2.0 unx     1565 b- stor 14-Sep-24 15:19 XML/Tags.xml
-16 files, 202244 bytes uncompressed, 202244 bytes compressed:  0.0%
+Zip file size: 206617 bytes, number of entries: 16
+-rw-r--r--  2.0 unx    16150 b- stor 14-Sep-24 15:01 designmap.xml
+-rw-r--r--  2.0 unx       43 b- stor 14-Sep-24 15:01 mimetype
+-rw-r--r--  2.0 unx     2608 b- stor 14-Sep-24 15:01 MasterSpreads/MasterSpread_ua5.xml
+-rw-r--r--  2.0 unx      253 b- stor 14-Sep-24 15:01 META-INF/container.xml
+-rw-r--r--  2.0 unx    25750 b- stor 14-Sep-24 15:01 META-INF/metadata.xml
+-rw-r--r--  2.0 unx    15342 b- stor 14-Sep-24 15:01 Resources/Fonts.xml
+-rw-r--r--  2.0 unx     7216 b- stor 14-Sep-24 15:01 Resources/Graphic.xml
+-rw-r--r--  2.0 unx    73610 b- stor 14-Sep-24 15:01 Resources/Preferences.xml
+-rw-r--r--  2.0 unx    36401 b- stor 14-Sep-24 15:01 Resources/Styles.xml
+-rw-r--r--  2.0 unx    19147 b- stor 14-Sep-24 15:01 Spreads/Spread_ud8.xml
+-rw-r--r--  2.0 unx     1217 b- stor 14-Sep-24 15:01 Stories/Story_u10d.xml
+-rw-r--r--  2.0 unx      951 b- stor 14-Sep-24 15:01 Stories/Story_ue1.xml
+-rw-r--r--  2.0 unx     3313 b- stor 14-Sep-24 15:01 Stories/Story_uf7.xml
+-rw-r--r--  2.0 unx      737 b- stor 14-Sep-24 15:01 XML/BackingStory.xml
+-rw-r--r--  2.0 unx      445 b- stor 14-Sep-24 15:01 XML/Mapping.xml
+-rw-r--r--  2.0 unx     1564 b- stor 14-Sep-24 15:01 XML/Tags.xml
+16 files, 204747 bytes uncompressed, 204747 bytes compressed:  0.0%
```

#### zipnote «TEMP»/diffoscope_nwk2mihn_/tmptpgy26d1_.zip

```diff
@@ -21,24 +21,24 @@
 
 Filename: Resources/Preferences.xml
 Comment: 
 
 Filename: Resources/Styles.xml
 Comment: 
 
-Filename: Spreads/Spread_myprefixud8.xml
+Filename: Spreads/Spread_ud8.xml
 Comment: 
 
-Filename: Stories/Story_myprefixu10d.xml
+Filename: Stories/Story_u10d.xml
 Comment: 
 
-Filename: Stories/Story_myprefixue1.xml
+Filename: Stories/Story_ue1.xml
 Comment: 
 
-Filename: Stories/Story_myprefixuf7.xml
+Filename: Stories/Story_uf7.xml
 Comment: 
 
 Filename: XML/BackingStory.xml
 Comment: 
 
 Filename: XML/Mapping.xml
 Comment:
```

#### designmap.xml

##### designmap.xml

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<?aid style="50" type="document" readerVersion="6.0" featureSet="257" product="7.5(142)" ?>
-<Document xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0" Self="d" StoryList="myprefixue1 myprefixuf7 myprefixu10d myprefixu83" ZeroPoint="0 0" ActiveLayer="ua4" CMYKProfile="$ID/" RGBProfile="$ID/" SolidColorIntent="UseColorSettings" AfterBlendingIntent="UseColorSettings" DefaultImageIntent="UseColorSettings" RGBPolicy="ColorPolicyOff" CMYKPolicy="ColorPolicyOff" AccurateLABSpots="false">
+<?aid style="50" type="document" readerVersion="6.0" featureSet="257" product="10.0(70)" ?>
+<Document xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0" Self="d" StoryList="ue1 uf7 u10d u83" ZeroPoint="0 0" ActiveLayer="ua4" CMYKProfile="$ID/" RGBProfile="$ID/" SolidColorIntent="UseColorSettings" AfterBlendingIntent="UseColorSettings" DefaultImageIntent="UseColorSettings" RGBPolicy="ColorPolicyOff" CMYKPolicy="ColorPolicyOff" AccurateLABSpots="false">
   <Language Self="Language/$ID/French" Name="$ID/French" SingleQuotes="‘’" DoubleQuotes="«»" PrimaryLanguageName="$ID/French" SublanguageName="$ID/" Id="274" HyphenationVendor="Proximity" SpellingVendor="Proximity"/>
   <Language Self="Language/$ID/English%3a UK" Name="$ID/English: UK" SingleQuotes="‘’" DoubleQuotes="“”" PrimaryLanguageName="$ID/English" SublanguageName="$ID/UK" Id="525" HyphenationVendor="Proximity" SpellingVendor="Proximity"/>
   <idPkg:Graphic src="Resources/Graphic.xml"/>
   <idPkg:Fonts src="Resources/Fonts.xml"/>
   <idPkg:Styles src="Resources/Styles.xml"/>
   <NumberingList Self="NumberingList/$ID/[Default]" Name="$ID/[Default]" ContinueNumbersAcrossStories="false" ContinueNumbersAcrossDocuments="false"/>
   <NamedGrid Self="NamedGrid/$ID/[Page Grid]" Name="$ID/[Page Grid]">
@@ -44,25 +44,25 @@
   <TextVariable Self="dTextVariablenModification Date" Name="Modification Date" VariableType="ModificationDateType">
     <DateVariablePreference TextBefore="" Format="d MMMM yyyy h:mm aa" TextAfter=""/>
   </TextVariable>
   <TextVariable Self="dTextVariablenOutput Date" Name="Output Date" VariableType="OutputDateType">
     <DateVariablePreference TextBefore="" Format="dd/MM/yy" TextAfter=""/>
   </TextVariable>
   <TextVariable Self="dTextVariablenRunning Header" Name="Running Header" VariableType="MatchParagraphStyleType">
-    <MatchParagraphStylePreference TextBefore="" TextAfter="" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" SearchStrategy="FirstOnPage" ChangeCase="None" DeleteEndPunctuation="false"/>
+    <MatchParagraphStylePreference TextBefore="" TextAfter="" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" SearchStrategy="FirstOnPage" ChangeCase="None" DeleteEndPunctuation="false"/>
   </TextVariable>
   <idPkg:Tags src="XML/Tags.xml"/>
-  <Layer Self="myprefixua4" Name="Layer 1" Visible="true" Locked="false" IgnoreWrap="false" ShowGuides="true" LockGuides="false" UI="true" Expendable="true" Printable="true">
+  <Layer Self="ua4" Name="Layer 1" Visible="true" Locked="false" IgnoreWrap="false" ShowGuides="true" LockGuides="false" UI="true" Expendable="true" Printable="true">
     <Properties>
       <LayerColor type="enumeration">LightBlue</LayerColor>
     </Properties>
   </Layer>
   <idPkg:MasterSpread src="MasterSpreads/MasterSpread_ua5.xml"/>
-  <idPkg:Spread src="Spreads/Spread_myprefixud8.xml"/>
-  <Section Self="u9b" Length="1" AlternateLayoutLength="1" AlternateLayout="Personnalisées V" Name="" ContinueNumbering="true" IncludeSectionPrefix="false" Marker="" PageStart="myprefixudd" SectionPrefix="">
+  <idPkg:Spread src="Spreads/Spread_ud8.xml"/>
+  <Section Self="u9b" Length="1" AlternateLayoutLength="1" AlternateLayout="Personnalisées V" Name="" ContinueNumbering="true" IncludeSectionPrefix="false" Marker="" PageStart="udd" SectionPrefix="">
     <Properties>
       <PageNumberStyle type="enumeration">Arabic</PageNumberStyle>
     </Properties>
   </Section>
   <DocumentUser Self="dDocumentUser0" UserName="$ID/Unknown User Name">
     <Properties>
       <UserColor type="enumeration">Gold</UserColor>
@@ -115,39 +115,39 @@
     <BuildingBlock Self="u129BuildingBlock2" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="&quot;" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
   </CrossReferenceFormat>
   <CrossReferenceFormat Self="u12a" Name="Page Number" AppliedCharacterStyle="n">
     <BuildingBlock Self="u12aBuildingBlock0" BlockType="CustomStringBuildingBlock" AppliedCharacterStyle="n" CustomText="page " AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
     <BuildingBlock Self="u12aBuildingBlock1" BlockType="PageNumberBuildingBlock" AppliedCharacterStyle="n" CustomText="$ID/" AppliedDelimiter="$ID/" IncludeDelimiter="false"/>
   </CrossReferenceFormat>
   <idPkg:BackingStory src="XML/BackingStory.xml"/>
-  <idPkg:Story src="Stories/Story_myprefixu10d.xml"/>
-  <idPkg:Story src="Stories/Story_myprefixuf7.xml"/>
-  <idPkg:Story src="Stories/Story_myprefixue1.xml"/>
+  <idPkg:Story src="Stories/Story_u10d.xml"/>
+  <idPkg:Story src="Stories/Story_uf7.xml"/>
+  <idPkg:Story src="Stories/Story_ue1.xml"/>
   <idPkg:Mapping src="XML/Mapping.xml"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Symbol" Name="$ID/kIndexGroup_Symbol" Include="true" Priority="0" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Alphabet" Name="$ID/kIndexGroup_Alphabet" Include="true" Priority="1" HeaderType="BasicLatin"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Numeric" Name="$ID/kIndexGroup_Numeric" Include="false" Priority="2" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_GreekAlphabet" Name="$ID/kWRIndexGroup_GreekAlphabet" Include="false" Priority="3" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_CyrillicAlphabet" Name="$ID/kWRIndexGroup_CyrillicAlphabet" Include="false" Priority="4" HeaderType="Russian"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Kana" Name="$ID/kIndexGroup_Kana" Include="false" Priority="5" HeaderType="HiraganaAll"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Chinese" Name="$ID/kIndexGroup_Chinese" Include="false" Priority="6" HeaderType="ChinesePinyin"/>
   <IndexingSortOption Self="dIndexingSortOptionnkIndexGroup_Korean" Name="$ID/kIndexGroup_Korean" Include="false" Priority="7" HeaderType="KoreanConsonant"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_ArabicAlphabet" Name="$ID/kWRIndexGroup_ArabicAlphabet" Include="false" Priority="8" HeaderType="Nothing"/>
   <IndexingSortOption Self="dIndexingSortOptionnkWRIndexGroup_HebrewAlphabet" Name="$ID/kWRIndexGroup_HebrewAlphabet" Include="false" Priority="9" HeaderType="Nothing"/>
-  <ColorGroup Self="myprefixu143" Name="[Root Color Group]" IsRootColorGroup="true">
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch0" SwatchItemRef="Swatch/None"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch1" SwatchItemRef="Color/Registration"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch2" SwatchItemRef="Color/Paper"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch3" SwatchItemRef="Color/Black"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch4" SwatchItemRef="Color/C=0 M=0 Y=100 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch5" SwatchItemRef="Color/C=0 M=100 Y=0 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch6" SwatchItemRef="Color/C=100 M=0 Y=0 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch7" SwatchItemRef="Color/C=100 M=90 Y=10 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch8" SwatchItemRef="Color/C=15 M=100 Y=100 K=0"/>
-    <ColorGroupSwatch Self="myprefixu143ColorGroupSwatch9" SwatchItemRef="Color/C=75 M=5 Y=100 K=0"/>
+  <ColorGroup Self="u143" Name="[Root Color Group]" IsRootColorGroup="true">
+    <ColorGroupSwatch Self="u143ColorGroupSwatch0" SwatchItemRef="Swatch/None"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch1" SwatchItemRef="Color/Registration"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch2" SwatchItemRef="Color/Paper"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch3" SwatchItemRef="Color/Black"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch4" SwatchItemRef="Color/C=0 M=0 Y=100 K=0"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch5" SwatchItemRef="Color/C=0 M=100 Y=0 K=0"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch6" SwatchItemRef="Color/C=100 M=0 Y=0 K=0"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch7" SwatchItemRef="Color/C=100 M=90 Y=10 K=0"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch8" SwatchItemRef="Color/C=15 M=100 Y=100 K=0"/>
+    <ColorGroupSwatch Self="u143ColorGroupSwatch9" SwatchItemRef="Color/C=75 M=5 Y=100 K=0"/>
   </ColorGroup>
   <ABullet Self="dABullet0" CharacterType="UnicodeOnly" CharacterValue="8226">
     <Properties>
       <BulletsFont type="string">$ID/</BulletsFont>
       <BulletsFontStyle type="string">$ID/</BulletsFontStyle>
     </Properties>
   </ABullet>
```

#### MasterSpreads/MasterSpread_ua5.xml

##### MasterSpreads/MasterSpread_ua5.xml

```diff
@@ -1,25 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:MasterSpread xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
   <MasterSpread Self="ua5" ItemTransform="1 0 0 1 0 0" OverriddenPageItemProps="" Name="A-Master" NamePrefix="A" BaseName="Master" ShowMasterItems="true" PageCount="2" PrimaryTextFrame="n">
     <Properties>
       <PageColor type="enumeration">UseMasterColor</PageColor>
     </Properties>
-    <Page Self="myprefixuaa" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 -566.9291338582677 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
+    <Page Self="uaa" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 -566.9291338582677 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
       <Properties>
         <PageColor type="enumeration">UseMasterColor</PageColor>
       </Properties>
       <MarginPreference ColumnCount="1" ColumnGutter="12" Top="36" Bottom="36" Left="36" Right="36" ColumnDirection="Horizontal" ColumnsPositions="0 494.92913385826773"/>
       <GridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100" LineAlignment="LeftOrTopLineJustify" GridAlignment="AlignEmCenter" CharacterAlignment="AlignEmCenter">
         <Properties>
           <AppliedFont type="string">Minion Pro</AppliedFont>
         </Properties>
       </GridDataInformation>
     </Page>
-    <Page Self="myprefixuab" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
+    <Page Self="uab" AppliedAlternateLayout="n" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="A" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="n" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
       <Properties>
         <PageColor type="enumeration">UseMasterColor</PageColor>
       </Properties>
       <MarginPreference ColumnCount="1" ColumnGutter="12" Top="36" Bottom="36" Left="36" Right="36" ColumnDirection="Horizontal" ColumnsPositions="0 494.92913385826773"/>
       <GridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100" LineAlignment="LeftOrTopLineJustify" GridAlignment="AlignEmCenter" CharacterAlignment="AlignEmCenter">
         <Properties>
           <AppliedFont type="string">Minion Pro</AppliedFont>
```

#### Resources/Fonts.xml

##### Resources/Fonts.xml

```diff
@@ -1,67 +1,67 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Fonts xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <FontFamily Self="myprefixdi38" Name="Minion Pro">
-    <Font Self="myprefixdi38FontnMinion Pro Bold Cond" FontFamily="Minion Pro" Name="Minion Pro Bold Cond" PostScriptName="MinionPro-BoldCn" Status="Installed" FontStyleName="Bold Cond" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond" FullNameNative="Minion Pro Bold Cond" FontStyleNameNative="Bold Cond" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Bold Cond Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Cond Italic" PostScriptName="MinionPro-BoldCnIt" Status="Installed" FontStyleName="Bold Cond Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond Italic" FullNameNative="Minion Pro Bold Cond Italic" FontStyleNameNative="Bold Cond Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Regular" FontFamily="Minion Pro" Name="Minion Pro Regular" PostScriptName="MinionPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro" FullNameNative="Minion Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Italic" FontFamily="Minion Pro" Name="Minion Pro Italic" PostScriptName="MinionPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Italic" FullNameNative="Minion Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Medium" FontFamily="Minion Pro" Name="Minion Pro Medium" PostScriptName="MinionPro-Medium" Status="Installed" FontStyleName="Medium" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium" FullNameNative="Minion Pro Medium" FontStyleNameNative="Medium" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Medium Italic" FontFamily="Minion Pro" Name="Minion Pro Medium Italic" PostScriptName="MinionPro-MediumIt" Status="Installed" FontStyleName="Medium Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium Italic" FullNameNative="Minion Pro Medium Italic" FontStyleNameNative="Medium Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Semibold" FontFamily="Minion Pro" Name="Minion Pro Semibold" PostScriptName="MinionPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold" FullNameNative="Minion Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Semibold Italic" FontFamily="Minion Pro" Name="Minion Pro Semibold Italic" PostScriptName="MinionPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold Italic" FullNameNative="Minion Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Bold" FontFamily="Minion Pro" Name="Minion Pro Bold" PostScriptName="MinionPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold" FullNameNative="Minion Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi38FontnMinion Pro Bold Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Italic" PostScriptName="MinionPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Italic" FullNameNative="Minion Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+  <FontFamily Self="di38" Name="Minion Pro">
+    <Font Self="di38FontnMinion Pro Bold Cond" FontFamily="Minion Pro" Name="Minion Pro Bold Cond" PostScriptName="MinionPro-BoldCn" Status="Installed" FontStyleName="Bold Cond" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond" FullNameNative="Minion Pro Bold Cond" FontStyleNameNative="Bold Cond" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Bold Cond Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Cond Italic" PostScriptName="MinionPro-BoldCnIt" Status="Installed" FontStyleName="Bold Cond Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Cond Italic" FullNameNative="Minion Pro Bold Cond Italic" FontStyleNameNative="Bold Cond Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Regular" FontFamily="Minion Pro" Name="Minion Pro Regular" PostScriptName="MinionPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro" FullNameNative="Minion Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Italic" FontFamily="Minion Pro" Name="Minion Pro Italic" PostScriptName="MinionPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Italic" FullNameNative="Minion Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Medium" FontFamily="Minion Pro" Name="Minion Pro Medium" PostScriptName="MinionPro-Medium" Status="Installed" FontStyleName="Medium" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium" FullNameNative="Minion Pro Medium" FontStyleNameNative="Medium" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Medium Italic" FontFamily="Minion Pro" Name="Minion Pro Medium Italic" PostScriptName="MinionPro-MediumIt" Status="Installed" FontStyleName="Medium Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Medium Italic" FullNameNative="Minion Pro Medium Italic" FontStyleNameNative="Medium Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Semibold" FontFamily="Minion Pro" Name="Minion Pro Semibold" PostScriptName="MinionPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold" FullNameNative="Minion Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Semibold Italic" FontFamily="Minion Pro" Name="Minion Pro Semibold Italic" PostScriptName="MinionPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Semibold Italic" FullNameNative="Minion Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Bold" FontFamily="Minion Pro" Name="Minion Pro Bold" PostScriptName="MinionPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold" FullNameNative="Minion Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di38FontnMinion Pro Bold Italic" FontFamily="Minion Pro" Name="Minion Pro Bold Italic" PostScriptName="MinionPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Minion Pro Bold Italic" FullNameNative="Minion Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.068;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
   </FontFamily>
-  <FontFamily Self="myprefixdi79" Name="Myriad Pro">
-    <Font Self="myprefixdi79FontnMyriad Pro Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Condensed" PostScriptName="MyriadPro-Cond" Status="Installed" FontStyleName="Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed" FullNameNative="Myriad Pro Condensed" FontStyleNameNative="Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Condensed Italic" PostScriptName="MyriadPro-CondIt" Status="Installed" FontStyleName="Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed Italic" FullNameNative="Myriad Pro Condensed Italic" FontStyleNameNative="Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed" PostScriptName="MyriadPro-BoldCond" Status="Installed" FontStyleName="Bold Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed" FullNameNative="Myriad Pro Bold Condensed" FontStyleNameNative="Bold Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed Italic" PostScriptName="MyriadPro-BoldCondIt" Status="Installed" FontStyleName="Bold Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed Italic" FullNameNative="Myriad Pro Bold Condensed Italic" FontStyleNameNative="Bold Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Regular" FontFamily="Myriad Pro" Name="Myriad Pro Regular" PostScriptName="MyriadPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro" FullNameNative="Myriad Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Italic" FontFamily="Myriad Pro" Name="Myriad Pro Italic" PostScriptName="MyriadPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Italic" FullNameNative="Myriad Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Semibold" FontFamily="Myriad Pro" Name="Myriad Pro Semibold" PostScriptName="MyriadPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold" FullNameNative="Myriad Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Semibold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Semibold Italic" PostScriptName="MyriadPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold Italic" FullNameNative="Myriad Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold" FontFamily="Myriad Pro" Name="Myriad Pro Bold" PostScriptName="MyriadPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold" FullNameNative="Myriad Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi79FontnMyriad Pro Bold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Italic" PostScriptName="MyriadPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Italic" FullNameNative="Myriad Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+  <FontFamily Self="di79" Name="Myriad Pro">
+    <Font Self="di79FontnMyriad Pro Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Condensed" PostScriptName="MyriadPro-Cond" Status="Installed" FontStyleName="Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed" FullNameNative="Myriad Pro Condensed" FontStyleNameNative="Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Condensed Italic" PostScriptName="MyriadPro-CondIt" Status="Installed" FontStyleName="Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Condensed Italic" FullNameNative="Myriad Pro Condensed Italic" FontStyleNameNative="Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold Condensed" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed" PostScriptName="MyriadPro-BoldCond" Status="Installed" FontStyleName="Bold Condensed" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed" FullNameNative="Myriad Pro Bold Condensed" FontStyleNameNative="Bold Condensed" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold Condensed Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Condensed Italic" PostScriptName="MyriadPro-BoldCondIt" Status="Installed" FontStyleName="Bold Condensed Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Condensed Italic" FullNameNative="Myriad Pro Bold Condensed Italic" FontStyleNameNative="Bold Condensed Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Regular" FontFamily="Myriad Pro" Name="Myriad Pro Regular" PostScriptName="MyriadPro-Regular" Status="Installed" FontStyleName="Regular" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro" FullNameNative="Myriad Pro" FontStyleNameNative="Regular" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Italic" FontFamily="Myriad Pro" Name="Myriad Pro Italic" PostScriptName="MyriadPro-It" Status="Installed" FontStyleName="Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Italic" FullNameNative="Myriad Pro Italic" FontStyleNameNative="Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Semibold" FontFamily="Myriad Pro" Name="Myriad Pro Semibold" PostScriptName="MyriadPro-Semibold" Status="Installed" FontStyleName="Semibold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold" FullNameNative="Myriad Pro Semibold" FontStyleNameNative="Semibold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Semibold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Semibold Italic" PostScriptName="MyriadPro-SemiboldIt" Status="Installed" FontStyleName="Semibold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Semibold Italic" FullNameNative="Myriad Pro Semibold Italic" FontStyleNameNative="Semibold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold" FontFamily="Myriad Pro" Name="Myriad Pro Bold" PostScriptName="MyriadPro-Bold" Status="Installed" FontStyleName="Bold" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold" FullNameNative="Myriad Pro Bold" FontStyleNameNative="Bold" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di79FontnMyriad Pro Bold Italic" FontFamily="Myriad Pro" Name="Myriad Pro Bold Italic" PostScriptName="MyriadPro-BoldIt" Status="Installed" FontStyleName="Bold Italic" FontType="OpenTypeCFF" WritingScript="0" FullName="Myriad Pro Bold Italic" FullNameNative="Myriad Pro Bold Italic" FontStyleNameNative="Bold Italic" PlatformName="$ID/" Version="Version 2.062;PS 2.000;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
   </FontFamily>
-  <FontFamily Self="myprefixdi7d" Name="Kozuka Mincho Pro">
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro EL" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro EL" PostScriptName="KozMinPro-ExtraLight" Status="Installed" FontStyleName="EL" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro EL" FullNameNative="小塚明朝 Pro EL" FontStyleNameNative="EL" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro L" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro L" PostScriptName="KozMinPro-Light" Status="Installed" FontStyleName="L" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro L" FullNameNative="小塚明朝 Pro L" FontStyleNameNative="L" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro R" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro R" PostScriptName="KozMinPro-Regular" Status="Installed" FontStyleName="R" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro R" FullNameNative="小塚明朝 Pro R" FontStyleNameNative="R" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro M" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro M" PostScriptName="KozMinPro-Medium" Status="Installed" FontStyleName="M" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro M" FullNameNative="小塚明朝 Pro M" FontStyleNameNative="M" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro B" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro B" PostScriptName="KozMinPro-Bold" Status="Installed" FontStyleName="B" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro B" FullNameNative="小塚明朝 Pro B" FontStyleNameNative="B" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
-    <Font Self="myprefixdi7dFontnKozuka Mincho Pro H" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro H" PostScriptName="KozMinPro-Heavy" Status="Installed" FontStyleName="H" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro H" FullNameNative="小塚明朝 Pro H" FontStyleNameNative="H" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+  <FontFamily Self="di7d" Name="Kozuka Mincho Pro">
+    <Font Self="di7dFontnKozuka Mincho Pro EL" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro EL" PostScriptName="KozMinPro-ExtraLight" Status="Installed" FontStyleName="EL" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro EL" FullNameNative="小塚明朝 Pro EL" FontStyleNameNative="EL" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro L" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro L" PostScriptName="KozMinPro-Light" Status="Installed" FontStyleName="L" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro L" FullNameNative="小塚明朝 Pro L" FontStyleNameNative="L" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro R" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro R" PostScriptName="KozMinPro-Regular" Status="Installed" FontStyleName="R" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro R" FullNameNative="小塚明朝 Pro R" FontStyleNameNative="R" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro M" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro M" PostScriptName="KozMinPro-Medium" Status="Installed" FontStyleName="M" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro M" FullNameNative="小塚明朝 Pro M" FontStyleNameNative="M" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro B" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro B" PostScriptName="KozMinPro-Bold" Status="Installed" FontStyleName="B" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro B" FullNameNative="小塚明朝 Pro B" FontStyleNameNative="B" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
+    <Font Self="di7dFontnKozuka Mincho Pro H" FontFamily="Kozuka Mincho Pro" Name="Kozuka Mincho Pro H" PostScriptName="KozMinPro-Heavy" Status="Installed" FontStyleName="H" FontType="OpenTypeCID" WritingScript="1" FullName="Kozuka Mincho Pro H" FullNameNative="小塚明朝 Pro H" FontStyleNameNative="H" PlatformName="$ID/" Version="Version 4.005;PS 4.003;hotconv 1.0.57;makeotf.lib2.0.21895" TypekitID="$ID/"/>
   </FontFamily>
-  <CompositeFont Self="myprefixCompositeFont/$ID/[No composite font]" Name="$ID/[No composite font]">
-    <CompositeFontEntry Self="myprefixu7c" Name="$ID/Kanji" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" Locked="true" ScaleOption="true" BaselineShift="0">
+  <CompositeFont Self="CompositeFont/$ID/[No composite font]" Name="$ID/[No composite font]">
+    <CompositeFontEntry Self="u7c" Name="$ID/Kanji" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu7e" Name="$ID/Kana" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="ぁあぃいぅうぇえぉおかがきぎくぐけげこごさざしじすずせぜそぞただちぢっつづてでとどなにぬねのはばぱひびぴふぶぷへべぺほぼぽまみむめもゃやゅゆょよらりるれろゎわゐゑをんゔゕゖゝゞァアィイゥウェエォオカガキギクグケゲコゴサザシジスズセゼソゾタダチヂッツヅテデトドナニヌネノハバパヒビピフブプヘベペホボポマミムメモャヤュユョヨラリルレロヮワヰヱヲンヴヵヶヷヸヹヺーヽヾ" Locked="true" ScaleOption="true" BaselineShift="0">
+    <CompositeFontEntry Self="u7e" Name="$ID/Kana" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="ぁあぃいぅうぇえぉおかがきぎくぐけげこごさざしじすずせぜそぞただちぢっつづてでとどなにぬねのはばぱひびぴふぶぷへべぺほぼぽまみむめもゃやゅゆょよらりるれろゎわゐゑをんゔゕゖゝゞァアィイゥウェエォオカガキギクグケゲコゴサザシジスズセゼソゾタダチヂッツヅテデトドナニヌネノハバパヒビピフブプヘベペホボポマミムメモャヤュユョヨラリルレロヮワヰヱヲンヴヵヶヷヸヹヺーヽヾ" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu7f" Name="$ID/Punctuation" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="—―‖‘’“”‥…′″∥、。〈〉《》「」『』【】〔〕〜・！（），．／：；？［］｛｝～" Locked="true" ScaleOption="true" BaselineShift="0">
+    <CompositeFontEntry Self="u7f" Name="$ID/Punctuation" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="—―‖‘’“”‥…′″∥、。〈〉《》「」『』【】〔〕〜・！（），．／：；？［］｛｝～" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu80" Name="$ID/Symbols" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="¢£§¨¬°±´¶×÷ΑΒΓΔΕΖΗΘΙΚΛΜΝΞΟΠΡΣΤΥΦΧΨΩαβγδεζηθικλμνξοπρστυφχψωЁАБВГДЕЖЗИЙКЛМНОПРСТУФХЦЧШЩЪЫЬЭЮЯабвгдежзийклмнопрстуфхцчшщъыьэюяё‐†‡‰※℃Å←↑→↓⇒⇔∀∂∃∇∈∋−√∝∞∠∧∨∩∪∫∬∴∵∽≒≠≡≦≧≪≫⊂⊃⊆⊇⊥⌒■□▲△▼▽◆◇○◎●◯★☆♀♂♪♭♯〃〆〇〒〓゛゜＃＄％＆＊＋－０１２３４５６７８９＜＝＞＠ＡＢＣＤＥＦＧＨＩＪＫＬＭＮＯＰＱＲＳＴＵＶＷＸＹＺ＼＾＿｀ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ｜￠￡￢￣￥" Locked="true" ScaleOption="true" BaselineShift="0">
+    <CompositeFontEntry Self="u80" Name="$ID/Symbols" FontStyle="$ID/R" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="¢£§¨¬°±´¶×÷ΑΒΓΔΕΖΗΘΙΚΛΜΝΞΟΠΡΣΤΥΦΧΨΩαβγδεζηθικλμνξοπρστυφχψωЁАБВГДЕЖЗИЙКЛМНОПРСТУФХЦЧШЩЪЫЬЭЮЯабвгдежзийклмнопрстуфхцчшщъыьэюяё‐†‡‰※℃Å←↑→↓⇒⇔∀∂∃∇∈∋−√∝∞∠∧∨∩∪∫∬∴∵∽≒≠≡≦≧≪≫⊂⊃⊆⊇⊥⌒■□▲△▼▽◆◇○◎●◯★☆♀♂♪♭♯〃〆〇〒〓゛゜＃＄％＆＊＋－０１２３４５６７８９＜＝＞＠ＡＢＣＤＥＦＧＨＩＪＫＬＭＮＯＰＱＲＳＴＵＶＷＸＹＺ＼＾＿｀ａｂｃｄｅｆｇｈｉｊｋｌｍｎｏｐｑｒｓｔｕｖｗｘｙｚ｜￠￡￢￣￥" Locked="true" ScaleOption="true" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Kozuka Mincho Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu81" Name="$ID/Alphabetic" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters=" !&quot;#$%&amp;'()*+,-./:;&lt;=&gt;?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~ ¡¤¥¦©ª«­®¯²³µ·¸¹º»¼½¾¿ÀÁÂÃÄÅÆÇÈÉÊËÌÍÎÏÐÑÒÓÔÕÖØÙÚÛÜÝÞßàáâãäåæçèéêëìíîïðñòóôõöøùúûüýþÿıŒœŠšŸŽžƒˆˇ˘˙˚˛˜˝–‚„•‹›⁄€™∆∏∑≈≤≥◊ﬀﬁﬂﬃﬄﬅﬆ" Locked="true" ScaleOption="false" BaselineShift="0">
+    <CompositeFontEntry Self="u81" Name="$ID/Alphabetic" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters=" !&quot;#$%&amp;'()*+,-./:;&lt;=&gt;?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~ ¡¤¥¦©ª«­®¯²³µ·¸¹º»¼½¾¿ÀÁÂÃÄÅÆÇÈÉÊËÌÍÎÏÐÑÒÓÔÕÖØÙÚÛÜÝÞßàáâãäåæçèéêëìíîïðñòóôõöøùúûüýþÿıŒœŠšŸŽžƒˆˇ˘˙˚˛˜˝–‚„•‹›⁄€™∆∏∑≈≤≥◊ﬀﬁﬂﬃﬄﬅﬆ" Locked="true" ScaleOption="false" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Minion Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
-    <CompositeFontEntry Self="myprefixu82" Name="$ID/Numbers" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="0123456789" Locked="true" ScaleOption="false" BaselineShift="0">
+    <CompositeFontEntry Self="u82" Name="$ID/Numbers" FontStyle="$ID/Regular" RelativeSize="100" HorizontalScale="100" VerticalScale="100" CustomCharacters="0123456789" Locked="true" ScaleOption="false" BaselineShift="0">
       <Properties>
         <AppliedFont type="string">Minion Pro</AppliedFont>
       </Properties>
     </CompositeFontEntry>
   </CompositeFont>
 </idPkg:Fonts>
```

#### Resources/Graphic.xml

##### Resources/Graphic.xml

```diff
@@ -1,50 +1,50 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Graphic xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Color Self="myprefixColor/Black" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Specialblack" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Black" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=0 M=0 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=0 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=0 M=100 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=100 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=100 M=0 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=0 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=100 M=90 Y=10 K=0" Model="Process" Space="CMYK" ColorValue="100 90 10 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=90 Y=10 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=15 M=100 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="15 100 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=15 M=100 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/C=75 M=5 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="75 5 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=75 M=5 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Cyan" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Cyan" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Magenta" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Magenta" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Paper" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Specialpaper" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Paper" ColorEditable="true" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Registration" Model="Registration" Space="CMYK" ColorValue="100 100 100 100" ColorOverride="Specialregistration" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Registration" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/Yellow" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Yellow" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/u70" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/u72" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
-  <Color Self="myprefixColor/uba" Model="Process" Space="CMYK" ColorValue="11 95 100 2" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
-  <Ink Self="myprefixInk/$ID/Process Cyan" Name="$ID/Process Cyan" Angle="75" ConvertToProcess="false" Frequency="70" NeutralDensity="0.61" PrintInk="true" TrapOrder="1" InkType="Normal"/>
-  <Ink Self="myprefixInk/$ID/Process Magenta" Name="$ID/Process Magenta" Angle="15" ConvertToProcess="false" Frequency="70" NeutralDensity="0.76" PrintInk="true" TrapOrder="2" InkType="Normal"/>
-  <Ink Self="myprefixInk/$ID/Process Yellow" Name="$ID/Process Yellow" Angle="0" ConvertToProcess="false" Frequency="70" NeutralDensity="0.16" PrintInk="true" TrapOrder="3" InkType="Normal"/>
-  <Ink Self="myprefixInk/$ID/Process Black" Name="$ID/Process Black" Angle="45" ConvertToProcess="false" Frequency="70" NeutralDensity="1.7" PrintInk="true" TrapOrder="4" InkType="Normal"/>
-  <PastedSmoothShade Self="myprefixPastedSmoothShade/u6f" ContentsVersion="0" ContentsType="ConstantShade" SpotColorList="" ContentsEncoding="Ascii64Encoding" ContentsMatrix="1 0 0 1 0 0" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
+  <Color Self="Color/Black" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Specialblack" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Black" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=0 M=0 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=0 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=0 M=100 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=0 M=100 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=100 M=0 Y=0 K=0" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=0 Y=0 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=100 M=90 Y=10 K=0" Model="Process" Space="CMYK" ColorValue="100 90 10 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=100 M=90 Y=10 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=15 M=100 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="15 100 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=15 M=100 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/C=75 M=5 Y=100 K=0" Model="Process" Space="CMYK" ColorValue="75 5 100 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="C=75 M=5 Y=100 K=0" ColorEditable="true" ColorRemovable="true" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/Cyan" Model="Process" Space="CMYK" ColorValue="100 0 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Cyan" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/Magenta" Model="Process" Space="CMYK" ColorValue="0 100 0 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Magenta" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/Paper" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Specialpaper" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Paper" ColorEditable="true" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/Registration" Model="Registration" Space="CMYK" ColorValue="100 100 100 100" ColorOverride="Specialregistration" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Registration" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Color Self="Color/Yellow" Model="Process" Space="CMYK" ColorValue="0 0 100 0" ColorOverride="Hiddenreserved" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="Yellow" ColorEditable="false" ColorRemovable="false" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/u70" Model="Process" Space="CMYK" ColorValue="0 0 0 0" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/u72" Model="Process" Space="CMYK" ColorValue="0 0 0 100" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
+  <Color Self="Color/uba" Model="Process" Space="CMYK" ColorValue="11 95 100 2" ColorOverride="Normal" AlternateSpace="NoAlternateColor" AlternateColorValue="" Name="" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937"/>
+  <Ink Self="Ink/$ID/Process Cyan" Name="$ID/Process Cyan" Angle="75" ConvertToProcess="false" Frequency="70" NeutralDensity="0.61" PrintInk="true" TrapOrder="1" InkType="Normal"/>
+  <Ink Self="Ink/$ID/Process Magenta" Name="$ID/Process Magenta" Angle="15" ConvertToProcess="false" Frequency="70" NeutralDensity="0.76" PrintInk="true" TrapOrder="2" InkType="Normal"/>
+  <Ink Self="Ink/$ID/Process Yellow" Name="$ID/Process Yellow" Angle="0" ConvertToProcess="false" Frequency="70" NeutralDensity="0.16" PrintInk="true" TrapOrder="3" InkType="Normal"/>
+  <Ink Self="Ink/$ID/Process Black" Name="$ID/Process Black" Angle="45" ConvertToProcess="false" Frequency="70" NeutralDensity="1.7" PrintInk="true" TrapOrder="4" InkType="Normal"/>
+  <PastedSmoothShade Self="PastedSmoothShade/u6f" ContentsVersion="0" ContentsType="ConstantShade" SpotColorList="" ContentsEncoding="Ascii64Encoding" ContentsMatrix="1 0 0 1 0 0" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
     <Properties>
-      <Contents>AAAAAUBv4AAAAAAAAAAAAAAAAAAAAAAAAAAAAA==</Contents>
+      <Contents><![CDATA[AAAAAUBv4AAAAAAAAAAAAAAAAAAAAAAAAAAAAA==]]></Contents>
     </Properties>
   </PastedSmoothShade>
-  <Swatch Self="myprefixSwatch/None" Name="None" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
-  <Gradient Self="myprefixGradient/u71" Type="Linear" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
-    <GradientStop Self="myprefixu71GradientStop0" StopColor="Color/u70" Location="0"/>
-    <GradientStop Self="myprefixu71GradientStop1" StopColor="Color/Black" Location="100" Midpoint="50"/>
+  <Swatch Self="Swatch/None" Name="None" ColorEditable="false" ColorRemovable="false" Visible="true" SwatchCreatorID="7937"/>
+  <Gradient Self="Gradient/u71" Type="Linear" Name="$ID/" ColorEditable="true" ColorRemovable="true" Visible="false" SwatchCreatorID="7937">
+    <GradientStop Self="u71GradientStop0" StopColor="Color/u70" Location="0"/>
+    <GradientStop Self="u71GradientStop1" StopColor="Color/Black" Location="100" Midpoint="50"/>
   </Gradient>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Triple_Stroke" Name="$ID/Triple_Stroke"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThickThinThick" Name="$ID/ThickThinThick"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThinThickThin" Name="$ID/ThinThickThin"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThickThick" Name="$ID/ThickThick"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThickThin" Name="$ID/ThickThin"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThinThick" Name="$ID/ThinThick"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/ThinThin" Name="$ID/ThinThin"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Japanese Dots" Name="$ID/Japanese Dots"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/White Diamond" Name="$ID/White Diamond"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Left Slant Hash" Name="$ID/Left Slant Hash"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Right Slant Hash" Name="$ID/Right Slant Hash"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Straight Hash" Name="$ID/Straight Hash"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Wavy" Name="$ID/Wavy"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Canned Dotted" Name="$ID/Canned Dotted"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Canned Dashed 3x2" Name="$ID/Canned Dashed 3x2"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Canned Dashed 4x4" Name="$ID/Canned Dashed 4x4"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Dashed" Name="$ID/Dashed"/>
-  <StrokeStyle Self="myprefixStrokeStyle/$ID/Solid" Name="$ID/Solid"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Triple_Stroke" Name="$ID/Triple_Stroke"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThickThinThick" Name="$ID/ThickThinThick"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThinThickThin" Name="$ID/ThinThickThin"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThickThick" Name="$ID/ThickThick"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThickThin" Name="$ID/ThickThin"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThinThick" Name="$ID/ThinThick"/>
+  <StrokeStyle Self="StrokeStyle/$ID/ThinThin" Name="$ID/ThinThin"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Japanese Dots" Name="$ID/Japanese Dots"/>
+  <StrokeStyle Self="StrokeStyle/$ID/White Diamond" Name="$ID/White Diamond"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Left Slant Hash" Name="$ID/Left Slant Hash"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Right Slant Hash" Name="$ID/Right Slant Hash"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Straight Hash" Name="$ID/Straight Hash"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Wavy" Name="$ID/Wavy"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Canned Dotted" Name="$ID/Canned Dotted"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Canned Dashed 3x2" Name="$ID/Canned Dashed 3x2"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Canned Dashed 4x4" Name="$ID/Canned Dashed 4x4"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Dashed" Name="$ID/Dashed"/>
+  <StrokeStyle Self="StrokeStyle/$ID/Solid" Name="$ID/Solid"/>
 </idPkg:Graphic>
```

#### Resources/Preferences.xml

##### Resources/Preferences.xml

```diff
@@ -79,15 +79,15 @@
         <ListItem type="unit">0</ListItem>
         <ListItem type="unit">0</ListItem>
         <ListItem type="unit">0</ListItem>
       </InsetSpacing>
     </Properties>
   </TextFramePreference>
   <TextPreference TypographersQuotes="true" HighlightHjViolations="false" HighlightKeeps="false" HighlightSubstitutedGlyphs="false" HighlightCustomSpacing="false" HighlightSubstitutedFonts="true" UseOpticalSize="true" UseParagraphLeading="false" SuperscriptSize="58.3" SuperscriptPosition="33.3" SubscriptSize="58.3" SubscriptPosition="33.3" SmallCap="70" LeadingKeyIncrement="2" BaselineShiftKeyIncrement="2" KerningKeyIncrement="20" ShowInvisibles="false" JustifyTextWraps="false" AbutTextToTextWrap="true" ZOrderTextWrap="false" LinkTextFilesWhenImporting="false" HighlightKinsoku="false" QuoteCharactersRotatedInVertical="false" UseNewVerticalScaling="false" UseCidMojikumi="false" EnableStylePreviewMode="false" SmartTextReflow="true" AddPages="EndOfStory" LimitToMasterTextFrames="true" PreserveFacingPageSpreads="false" DeleteEmptyPages="false"/>
-  <TextDefault FontStyle="Italic" PointSize="12" KerningMethod="$ID/Metrics" Tracking="0" Capitalization="Normal" Position="Superscript" Underline="false" StrikeThru="false" Ligatures="true" NoBreak="false" HorizontalScale="100" VerticalScale="100" BaselineShift="0" Skew="0" FillTint="-1" StrokeTint="-1" StrokeWeight="1" OverprintStroke="false" OverprintFill="false" OTFFigureStyle="Default" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" OTFContextualAlternate="true" OTFSwash="false" UnderlineTint="-1" UnderlineGapTint="-1" UnderlineOverprint="false" UnderlineGapOverprint="false" UnderlineOffset="-9999" UnderlineWeight="-9999" StrikeThroughTint="-1" StrikeThroughGapTint="-1" StrikeThroughOverprint="false" StrikeThroughGapOverprint="false" StrikeThroughOffset="-9999" StrikeThroughWeight="-9999" FillColor="myprefixColor/Black" StrokeColor="myprefixSwatch/None" AppliedLanguage="$ID/English: UK" ParagraphKashidaWidth="2" FirstLineIndent="0" LeftIndent="0" RightIndent="0" SpaceBefore="0" SpaceAfter="0" Justification="LeftAlign" SingleWordJustification="FullyJustified" AutoLeading="120" DropCapLines="0" DropCapCharacters="0" KeepLinesTogether="false" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" StartParagraph="Anywhere" Composer="HL Composer" MinimumWordSpacing="80" MaximumWordSpacing="133" DesiredWordSpacing="100" MinimumLetterSpacing="0" MaximumLetterSpacing="0" DesiredLetterSpacing="0" MinimumGlyphScaling="100" MaximumGlyphScaling="100" DesiredGlyphScaling="100" RuleAbove="false" RuleAboveOverprint="false" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelow="false" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleBelowGapTint="-1" HyphenateCapitalizedWords="true" Hyphenation="true" HyphenateBeforeLast="2" HyphenateAfterFirst="2" HyphenateWordsLongerThan="5" HyphenateLadderLimit="3" HyphenationZone="36" HyphenWeight="5" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" AppliedCharacterStyle="myprefixCharacterStyle/sup" LastLineIndent="0" HyphenateLastWord="true" OTFSlashedZero="false" OTFHistorical="false" OTFStylisticSets="0" GradientFillLength="-1" GradientFillAngle="0" GradientStrokeLength="-1" GradientStrokeAngle="0" GradientFillStart="0 0" GradientStrokeStart="0 0" KeepWithPrevious="false" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" RuleBelowOverprint="false" RuleBelowGapOverprint="false" DropcapDetail="1" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFMark="true" OTFLocale="true" PositionalForm="None" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" CharacterDirection="DefaultDirection" KeyboardDirection="DefaultDirection" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" XOffsetDiacritic="0" YOffsetDiacritic="0" ParagraphBreakType="Anywhere" PageNumberType="AutoPageNumber" AppliedNamedGrid="n" GridAlignFirstLineOnly="false" GridAlignment="None" GridGyoudori="0" AutoTcy="0" AutoTcyIncludeRoman="false" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" Rensuuji="true" RotateSingleByteCharacters="false" LeadingModel="LeadingModelAkiBelow" CharacterAlignment="AlignEmCenter" Tsume="0" LeadingAki="-1" TrailingAki="-1" CharacterRotation="0" Jidori="0" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustRotation="false" ShataiAdjustTsume="true" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" KentenTint="-1" KentenStrokeTint="-1" KentenWeight="-1" KentenOverprintFill="Auto" KentenOverprintStroke="Auto" KentenKind="None" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" RubyTint="-1" RubyWeight="-1" RubyOverprintFill="Auto" RubyOverprintStroke="Auto" RubyStrokeTint="-1" RubyFontSize="-1" RubyOpenTypePro="true" RubyXScale="100" RubyYScale="100" RubyType="PerCharacterRuby" RubyAlignment="RubyJIS" RubyPosition="AboveRight" RubyXOffset="0" RubyYOffset="0" RubyParentSpacing="RubyParent121Aki" RubyAutoAlign="true" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyParentOverhangAmount="RubyOverhangOneRuby" Warichu="false" WarichuSize="50" WarichuLines="2" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsAfterBreak="2" WarichuCharsBeforeBreak="2" OTFProportionalMetrics="false" OTFHVKana="false" OTFRomanItalics="false" ScaleAffectsLineHeight="false" CjkGridTracking="false" GlyphForm="None" ParagraphGyoudori="false" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingExpression="^#.^t" BulletsTextAfter="^t" NumberingLevel="1" NumberingContinue="true" NumberingStartAt="1" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign">
+  <TextDefault FontStyle="Italic" PointSize="12" KerningMethod="$ID/Metrics" Tracking="0" Capitalization="Normal" Position="Superscript" Underline="false" StrikeThru="false" Ligatures="true" NoBreak="false" HorizontalScale="100" VerticalScale="100" BaselineShift="0" Skew="0" FillTint="-1" StrokeTint="-1" StrokeWeight="1" OverprintStroke="false" OverprintFill="false" OTFFigureStyle="Default" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" OTFContextualAlternate="true" OTFSwash="false" UnderlineTint="-1" UnderlineGapTint="-1" UnderlineOverprint="false" UnderlineGapOverprint="false" UnderlineOffset="-9999" UnderlineWeight="-9999" StrikeThroughTint="-1" StrikeThroughGapTint="-1" StrikeThroughOverprint="false" StrikeThroughGapOverprint="false" StrikeThroughOffset="-9999" StrikeThroughWeight="-9999" FillColor="Color/Black" StrokeColor="Swatch/None" AppliedLanguage="$ID/English: UK" ParagraphKashidaWidth="2" FirstLineIndent="0" LeftIndent="0" RightIndent="0" SpaceBefore="0" SpaceAfter="0" Justification="LeftAlign" SingleWordJustification="FullyJustified" AutoLeading="120" DropCapLines="0" DropCapCharacters="0" KeepLinesTogether="false" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" StartParagraph="Anywhere" Composer="HL Composer" MinimumWordSpacing="80" MaximumWordSpacing="133" DesiredWordSpacing="100" MinimumLetterSpacing="0" MaximumLetterSpacing="0" DesiredLetterSpacing="0" MinimumGlyphScaling="100" MaximumGlyphScaling="100" DesiredGlyphScaling="100" RuleAbove="false" RuleAboveOverprint="false" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelow="false" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleBelowGapTint="-1" HyphenateCapitalizedWords="true" Hyphenation="true" HyphenateBeforeLast="2" HyphenateAfterFirst="2" HyphenateWordsLongerThan="5" HyphenateLadderLimit="3" HyphenationZone="36" HyphenWeight="5" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" AppliedCharacterStyle="CharacterStyle/sup" LastLineIndent="0" HyphenateLastWord="true" OTFSlashedZero="false" OTFHistorical="false" OTFStylisticSets="0" GradientFillLength="-1" GradientFillAngle="0" GradientStrokeLength="-1" GradientStrokeAngle="0" GradientFillStart="0 0" GradientStrokeStart="0 0" KeepWithPrevious="false" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" RuleBelowOverprint="false" RuleBelowGapOverprint="false" DropcapDetail="1" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFMark="true" OTFLocale="true" PositionalForm="None" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" CharacterDirection="DefaultDirection" KeyboardDirection="DefaultDirection" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" XOffsetDiacritic="0" YOffsetDiacritic="0" ParagraphBreakType="Anywhere" PageNumberType="AutoPageNumber" AppliedNamedGrid="n" GridAlignFirstLineOnly="false" GridAlignment="None" GridGyoudori="0" AutoTcy="0" AutoTcyIncludeRoman="false" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" Rensuuji="true" RotateSingleByteCharacters="false" LeadingModel="LeadingModelAkiBelow" CharacterAlignment="AlignEmCenter" Tsume="0" LeadingAki="-1" TrailingAki="-1" CharacterRotation="0" Jidori="0" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustRotation="false" ShataiAdjustTsume="true" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" KentenTint="-1" KentenStrokeTint="-1" KentenWeight="-1" KentenOverprintFill="Auto" KentenOverprintStroke="Auto" KentenKind="None" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" RubyTint="-1" RubyWeight="-1" RubyOverprintFill="Auto" RubyOverprintStroke="Auto" RubyStrokeTint="-1" RubyFontSize="-1" RubyOpenTypePro="true" RubyXScale="100" RubyYScale="100" RubyType="PerCharacterRuby" RubyAlignment="RubyJIS" RubyPosition="AboveRight" RubyXOffset="0" RubyYOffset="0" RubyParentSpacing="RubyParent121Aki" RubyAutoAlign="true" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyParentOverhangAmount="RubyOverhangOneRuby" Warichu="false" WarichuSize="50" WarichuLines="2" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsAfterBreak="2" WarichuCharsBeforeBreak="2" OTFProportionalMetrics="false" OTFHVKana="false" OTFRomanItalics="false" ScaleAffectsLineHeight="false" CjkGridTracking="false" GlyphForm="None" ParagraphGyoudori="false" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingExpression="^#.^t" BulletsTextAfter="^t" NumberingLevel="1" NumberingContinue="true" NumberingStartAt="1" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign">
     <Properties>
       <AppliedFont type="string">Minion Pro</AppliedFont>
       <Leading type="enumeration">Auto</Leading>
       <UnderlineColor type="string">Text Color</UnderlineColor>
       <UnderlineGapColor type="object">Swatch/None</UnderlineGapColor>
       <UnderlineType type="object">StrokeStyle/$ID/Solid</UnderlineType>
       <StrikeThroughColor type="string">Text Color</StrikeThroughColor>
@@ -647,20 +647,20 @@
             <SectionHeaderType SortingHeaderString="$ID/Y" DocumentHeaderString="$ID/" UIHeaderString="$ID/kIndexSection_Y" Language="256"/>
             <SectionHeaderType SortingHeaderString="$ID/Z" DocumentHeaderString="$ID/" UIHeaderString="$ID/kIndexSection_Z" Language="256"/>
           </SectionHeaderArray>
         </IndexHeaderGroupType>
       </ListOfIndexHeaderGroup>
     </Properties>
   </IndexHeaderSetting>
-  <PageItemDefault TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" AppliedGraphicObjectStyle="ObjectStyle/$ID/[Normal Graphics Frame]" AppliedTextObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" AppliedGridObjectStyle="ObjectStyle/$ID/[Normal Grid]" CornerOption="None" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GradientFillAngle="0" GradientStrokeAngle="0" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false"/>
+  <PageItemDefault TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" AppliedGraphicObjectStyle="ObjectStyle/$ID/[Normal Graphics Frame]" AppliedTextObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" AppliedGridObjectStyle="ObjectStyle/$ID/[Normal Grid]" CornerOption="None" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GradientFillAngle="0" GradientStrokeAngle="0" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false"/>
   <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
   <ButtonPreference Name=""/>
   <TinDocumentDataObject>
     <Properties>
-      <GaijiRefMaps>/////wAAAAAAAAAA</GaijiRefMaps>
+      <GaijiRefMaps><![CDATA[/////wAAAAAAAAAA]]></GaijiRefMaps>
     </Properties>
   </TinDocumentDataObject>
   <LayoutGridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100">
     <Properties>
       <AppliedFont type="string">Minion Pro</AppliedFont>
     </Properties>
   </LayoutGridDataInformation>
```

#### Resources/Styles.xml

##### Resources/Styles.xml

```diff
@@ -1,32 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Styles xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <RootCharacterStyleGroup Self="myprefixu65">
-    <CharacterStyle Self="myprefixCharacterStyle/$ID/[No character style]" Imported="false" Name="$ID/[No character style]"/>
-    <CharacterStyle Self="myprefixCharacterStyle/bold" Imported="false" KeyboardShortcut="0 0" Name="bold" FontStyle="Bold">
+  <RootCharacterStyleGroup Self="u65">
+    <CharacterStyle Self="CharacterStyle/$ID/[No character style]" Imported="false" Name="$ID/[No character style]"/>
+    <CharacterStyle Self="CharacterStyle/bold" Imported="false" KeyboardShortcut="0 0" Name="bold" FontStyle="Bold">
       <Properties>
         <BasedOn type="string">$ID/[No character style]</BasedOn>
         <PreviewColor type="enumeration">Nothing</PreviewColor>
       </Properties>
     </CharacterStyle>
-    <CharacterStyle Self="myprefixCharacterStyle/italique" Imported="false" KeyboardShortcut="0 0" Name="italique" FontStyle="Italic">
+    <CharacterStyle Self="CharacterStyle/italique" Imported="false" KeyboardShortcut="0 0" Name="italique" FontStyle="Italic">
       <Properties>
         <BasedOn type="string">$ID/[No character style]</BasedOn>
         <PreviewColor type="enumeration">Nothing</PreviewColor>
       </Properties>
     </CharacterStyle>
-    <CharacterStyle Self="myprefixCharacterStyle/sup" Imported="false" KeyboardShortcut="0 0" Name="sup" Position="Superscript">
+    <CharacterStyle Self="CharacterStyle/sup" Imported="false" KeyboardShortcut="0 0" Name="sup" Position="Superscript">
       <Properties>
         <BasedOn type="string">$ID/[No character style]</BasedOn>
         <PreviewColor type="enumeration">Nothing</PreviewColor>
       </Properties>
     </CharacterStyle>
   </RootCharacterStyleGroup>
-  <RootParagraphStyleGroup Self="myprefixu64">
-    <ParagraphStyle Self="myprefixParagraphStyle/$ID/[No paragraph style]" Name="$ID/[No paragraph style]" Imported="false" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" FillColor="myprefixColor/Black" FontStyle="Regular" PointSize="12" HorizontalScale="100" KerningMethod="$ID/Metrics" Ligatures="true" PageNumberType="AutoPageNumber" StrokeWeight="1" Tracking="0" Composer="HL Composer" DropCapCharacters="0" DropCapLines="0" BaselineShift="0" Capitalization="Normal" StrokeColor="myprefixSwatch/None" HyphenateLadderLimit="3" VerticalScale="100" LeftIndent="0" RightIndent="0" FirstLineIndent="0" AutoLeading="120" AppliedLanguage="$ID/English: UK" Hyphenation="true" HyphenateAfterFirst="2" HyphenateBeforeLast="2" HyphenateCapitalizedWords="true" HyphenateWordsLongerThan="5" NoBreak="false" HyphenationZone="36" SpaceBefore="0" SpaceAfter="0" Underline="false" OTFFigureStyle="Default" DesiredWordSpacing="100" MaximumWordSpacing="133" MinimumWordSpacing="80" DesiredLetterSpacing="0" MaximumLetterSpacing="0" MinimumLetterSpacing="0" DesiredGlyphScaling="100" MaximumGlyphScaling="100" MinimumGlyphScaling="100" StartParagraph="Anywhere" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" Position="Normal" StrikeThru="false" CharacterAlignment="AlignEmCenter" KeepLinesTogether="false" StrokeTint="-1" FillTint="-1" OverprintStroke="false" OverprintFill="false" GradientStrokeAngle="0" GradientFillAngle="0" GradientStrokeLength="-1" GradientFillLength="-1" GradientStrokeStart="0 0" GradientFillStart="0 0" Skew="0" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleAboveOverprint="false" RuleBelowOverprint="false" RuleAbove="false" RuleBelow="false" LastLineIndent="0" HyphenateLastWord="true" ParagraphBreakType="Anywhere" SingleWordJustification="FullyJustified" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelowGapTint="-1" RuleBelowGapOverprint="false" Justification="LeftAlign" DropcapDetail="1" PositionalForm="None" OTFMark="true" HyphenWeight="5" OTFLocale="true" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFSlashedZero="false" OTFStylisticSets="0" OTFHistorical="false" OTFContextualAlternate="true" UnderlineGapOverprint="false" UnderlineGapTint="-1" UnderlineOffset="-9999" UnderlineOverprint="false" UnderlineTint="-1" UnderlineWeight="-9999" StrikeThroughGapOverprint="false" StrikeThroughGapTint="-1" StrikeThroughOffset="-9999" StrikeThroughOverprint="false" StrikeThroughTint="-1" StrikeThroughWeight="-9999" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" KeepWithPrevious="false" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" OTFSwash="false" Tsume="0" LeadingAki="-1" TrailingAki="-1" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" RubyOpenTypePro="true" RubyFontSize="-1" RubyAlignment="RubyJIS" RubyType="PerCharacterRuby" RubyParentSpacing="RubyParent121Aki" RubyXScale="100" RubyYScale="100" RubyXOffset="0" RubyYOffset="0" RubyPosition="AboveRight" RubyAutoAlign="true" RubyParentOverhangAmount="RubyOverhangOneRuby" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyTint="-1" RubyOverprintFill="Auto" RubyStrokeTint="-1" RubyOverprintStroke="Auto" RubyWeight="-1" KentenKind="None" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" KentenTint="-1" KentenOverprintFill="Auto" KentenStrokeTint="-1" KentenOverprintStroke="Auto" KentenWeight="-1" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" AutoTcy="0" AutoTcyIncludeRoman="false" Jidori="0" GridGyoudori="0" GridAlignFirstLineOnly="false" GridAlignment="None" CharacterRotation="0" RotateSingleByteCharacters="false" Rensuuji="true" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustTsume="true" ShataiAdjustRotation="false" Warichu="false" WarichuLines="2" WarichuSize="50" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsBeforeBreak="2" WarichuCharsAfterBreak="2" OTFHVKana="false" OTFProportionalMetrics="false" OTFRomanItalics="false" LeadingModel="LeadingModelAkiBelow" ScaleAffectsLineHeight="false" ParagraphGyoudori="false" CjkGridTracking="false" GlyphForm="None" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingStartAt="1" NumberingLevel="1" NumberingContinue="true" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign" NumberingExpression="^#.^t" BulletsTextAfter="^t" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" CharacterDirection="DefaultDirection" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" ParagraphKashidaWidth="2" XOffsetDiacritic="0" YOffsetDiacritic="0" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" KeyboardDirection="DefaultDirection">
+  <RootParagraphStyleGroup Self="u64">
+    <ParagraphStyle Self="ParagraphStyle/$ID/[No paragraph style]" Name="$ID/[No paragraph style]" Imported="false" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" FillColor="Color/Black" FontStyle="Regular" PointSize="12" HorizontalScale="100" KerningMethod="$ID/Metrics" Ligatures="true" PageNumberType="AutoPageNumber" StrokeWeight="1" Tracking="0" Composer="HL Composer" DropCapCharacters="0" DropCapLines="0" BaselineShift="0" Capitalization="Normal" StrokeColor="Swatch/None" HyphenateLadderLimit="3" VerticalScale="100" LeftIndent="0" RightIndent="0" FirstLineIndent="0" AutoLeading="120" AppliedLanguage="$ID/English: UK" Hyphenation="true" HyphenateAfterFirst="2" HyphenateBeforeLast="2" HyphenateCapitalizedWords="true" HyphenateWordsLongerThan="5" NoBreak="false" HyphenationZone="36" SpaceBefore="0" SpaceAfter="0" Underline="false" OTFFigureStyle="Default" DesiredWordSpacing="100" MaximumWordSpacing="133" MinimumWordSpacing="80" DesiredLetterSpacing="0" MaximumLetterSpacing="0" MinimumLetterSpacing="0" DesiredGlyphScaling="100" MaximumGlyphScaling="100" MinimumGlyphScaling="100" StartParagraph="Anywhere" KeepAllLinesTogether="false" KeepWithNext="0" KeepFirstLines="2" KeepLastLines="2" Position="Normal" StrikeThru="false" CharacterAlignment="AlignEmCenter" KeepLinesTogether="false" StrokeTint="-1" FillTint="-1" OverprintStroke="false" OverprintFill="false" GradientStrokeAngle="0" GradientFillAngle="0" GradientStrokeLength="-1" GradientFillLength="-1" GradientStrokeStart="0 0" GradientFillStart="0 0" Skew="0" RuleAboveLineWeight="1" RuleAboveTint="-1" RuleAboveOffset="0" RuleAboveLeftIndent="0" RuleAboveRightIndent="0" RuleAboveWidth="ColumnWidth" RuleBelowLineWeight="1" RuleBelowTint="-1" RuleBelowOffset="0" RuleBelowLeftIndent="0" RuleBelowRightIndent="0" RuleBelowWidth="ColumnWidth" RuleAboveOverprint="false" RuleBelowOverprint="false" RuleAbove="false" RuleBelow="false" LastLineIndent="0" HyphenateLastWord="true" ParagraphBreakType="Anywhere" SingleWordJustification="FullyJustified" OTFOrdinal="false" OTFFraction="false" OTFDiscretionaryLigature="false" OTFTitling="false" RuleAboveGapTint="-1" RuleAboveGapOverprint="false" RuleBelowGapTint="-1" RuleBelowGapOverprint="false" Justification="LeftAlign" DropcapDetail="1" PositionalForm="None" OTFMark="true" HyphenWeight="5" OTFLocale="true" HyphenateAcrossColumns="true" KeepRuleAboveInFrame="false" IgnoreEdgeAlignment="false" OTFSlashedZero="false" OTFStylisticSets="0" OTFHistorical="false" OTFContextualAlternate="true" UnderlineGapOverprint="false" UnderlineGapTint="-1" UnderlineOffset="-9999" UnderlineOverprint="false" UnderlineTint="-1" UnderlineWeight="-9999" StrikeThroughGapOverprint="false" StrikeThroughGapTint="-1" StrikeThroughOffset="-9999" StrikeThroughOverprint="false" StrikeThroughTint="-1" StrikeThroughWeight="-9999" MiterLimit="4" StrokeAlignment="OutsideAlignment" EndJoin="MiterEndJoin" SpanColumnType="SingleColumn" SplitColumnInsideGutter="6" SplitColumnOutsideGutter="0" KeepWithPrevious="false" SpanColumnMinSpaceBefore="0" SpanColumnMinSpaceAfter="0" OTFSwash="false" Tsume="0" LeadingAki="-1" TrailingAki="-1" KinsokuType="KinsokuPushInFirst" KinsokuHangType="None" BunriKinshi="true" RubyOpenTypePro="true" RubyFontSize="-1" RubyAlignment="RubyJIS" RubyType="PerCharacterRuby" RubyParentSpacing="RubyParent121Aki" RubyXScale="100" RubyYScale="100" RubyXOffset="0" RubyYOffset="0" RubyPosition="AboveRight" RubyAutoAlign="true" RubyParentOverhangAmount="RubyOverhangOneRuby" RubyOverhang="false" RubyAutoScaling="false" RubyParentScalingPercent="66" RubyTint="-1" RubyOverprintFill="Auto" RubyStrokeTint="-1" RubyOverprintStroke="Auto" RubyWeight="-1" KentenKind="None" KentenFontSize="-1" KentenXScale="100" KentenYScale="100" KentenPlacement="0" KentenAlignment="AlignKentenCenter" KentenPosition="AboveRight" KentenCustomCharacter="" KentenCharacterSet="CharacterInput" KentenTint="-1" KentenOverprintFill="Auto" KentenStrokeTint="-1" KentenOverprintStroke="Auto" KentenWeight="-1" Tatechuyoko="false" TatechuyokoXOffset="0" TatechuyokoYOffset="0" AutoTcy="0" AutoTcyIncludeRoman="false" Jidori="0" GridGyoudori="0" GridAlignFirstLineOnly="false" GridAlignment="None" CharacterRotation="0" RotateSingleByteCharacters="false" Rensuuji="true" ShataiMagnification="0" ShataiDegreeAngle="4500" ShataiAdjustTsume="true" ShataiAdjustRotation="false" Warichu="false" WarichuLines="2" WarichuSize="50" WarichuLineSpacing="0" WarichuAlignment="Auto" WarichuCharsBeforeBreak="2" WarichuCharsAfterBreak="2" OTFHVKana="false" OTFProportionalMetrics="false" OTFRomanItalics="false" LeadingModel="LeadingModelAkiBelow" ScaleAffectsLineHeight="false" ParagraphGyoudori="false" CjkGridTracking="false" GlyphForm="None" RubyAutoTcyDigits="0" RubyAutoTcyIncludeRoman="false" RubyAutoTcyAutoScale="true" TreatIdeographicSpaceAsSpace="false" AllowArbitraryHyphenation="false" BulletsAndNumberingListType="NoList" NumberingStartAt="1" NumberingLevel="1" NumberingContinue="true" NumberingApplyRestartPolicy="true" BulletsAlignment="LeftAlign" NumberingAlignment="LeftAlign" NumberingExpression="^#.^t" BulletsTextAfter="^t" DigitsType="DefaultDigits" Kashidas="DefaultKashidas" DiacriticPosition="OpentypePosition" CharacterDirection="DefaultDirection" ParagraphDirection="LeftToRightDirection" ParagraphJustification="DefaultJustification" ParagraphKashidaWidth="2" XOffsetDiacritic="0" YOffsetDiacritic="0" OTFOverlapSwash="false" OTFStylisticAlternate="false" OTFJustificationAlternate="false" OTFStretchedAlternate="false" KeyboardDirection="DefaultDirection">
       <Properties>
         <Leading type="enumeration">Auto</Leading>
         <TabList type="list"/>
         <AppliedFont type="string">Minion Pro</AppliedFont>
         <RuleAboveColor type="string">Text Color</RuleAboveColor>
         <RuleBelowColor type="string">Text Color</RuleBelowColor>
         <RuleAboveType type="object">StrokeStyle/$ID/Solid</RuleAboveType>
@@ -57,35 +57,35 @@
         <BulletsFontStyle type="enumeration">Nothing</BulletsFontStyle>
         <AppliedNumberingList type="object">NumberingList/$ID/[Default]</AppliedNumberingList>
         <NumberingRestartPolicies RestartPolicy="AnyPreviousLevel" LowerLevel="0" UpperLevel="0"/>
         <BulletsCharacterStyle type="object">CharacterStyle/$ID/[No character style]</BulletsCharacterStyle>
         <NumberingCharacterStyle type="object">CharacterStyle/$ID/[No character style]</NumberingCharacterStyle>
       </Properties>
     </ParagraphStyle>
-    <ParagraphStyle Self="myprefixParagraphStyle/$ID/NormalParagraphStyle" Name="$ID/NormalParagraphStyle" Imported="false" NextStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" KeyboardShortcut="0 0">
+    <ParagraphStyle Self="ParagraphStyle/$ID/NormalParagraphStyle" Name="$ID/NormalParagraphStyle" Imported="false" NextStyle="ParagraphStyle/$ID/NormalParagraphStyle" EmptyNestedStyles="true" EmptyLineStyles="true" EmptyGrepStyles="true" KeyboardShortcut="0 0">
       <Properties>
         <BasedOn type="string">$ID/[No paragraph style]</BasedOn>
         <PreviewColor type="enumeration">Nothing</PreviewColor>
       </Properties>
     </ParagraphStyle>
   </RootParagraphStyleGroup>
-  <TOCStyle Self="myprefixTOCStyle/$ID/DefaultTOCStyleName" TitleStyle="ParagraphStyle/$ID/[No paragraph style]" Title="Contents" Name="$ID/DefaultTOCStyleName" RunIn="false" IncludeHidden="false" IncludeBookDocuments="false" CreateBookmarks="true" SetStoryDirection="Horizontal" NumberedParagraphs="IncludeFullParagraph" MakeAnchor="false"/>
-  <RootCellStyleGroup Self="myprefixu6a">
-    <CellStyle Self="myprefixCellStyle/$ID/[None]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/[No paragraph style]" Name="$ID/[None]"/>
+  <TOCStyle Self="TOCStyle/$ID/DefaultTOCStyleName" TitleStyle="ParagraphStyle/$ID/[No paragraph style]" Title="Contents" Name="$ID/DefaultTOCStyleName" RunIn="false" IncludeHidden="false" IncludeBookDocuments="false" CreateBookmarks="true" SetStoryDirection="Horizontal" NumberedParagraphs="IncludeFullParagraph" MakeAnchor="false"/>
+  <RootCellStyleGroup Self="u6a">
+    <CellStyle Self="CellStyle/$ID/[None]" AppliedParagraphStyle="ParagraphStyle/$ID/[No paragraph style]" Name="$ID/[None]"/>
   </RootCellStyleGroup>
-  <RootTableStyleGroup Self="myprefixu6c">
-    <TableStyle Self="myprefixTableStyle/$ID/[No table style]" Name="$ID/[No table style]" StrokeOrder="BestJoins" TopBorderStrokeWeight="1" TopBorderStrokeType="StrokeStyle/$ID/Solid" TopBorderStrokeColor="Color/Black" TopBorderStrokeTint="100" TopBorderStrokeOverprint="false" TopBorderStrokeGapColor="Color/Paper" TopBorderStrokeGapTint="100" TopBorderStrokeGapOverprint="false" LeftBorderStrokeWeight="1" LeftBorderStrokeType="StrokeStyle/$ID/Solid" LeftBorderStrokeColor="Color/Black" LeftBorderStrokeTint="100" LeftBorderStrokeOverprint="false" LeftBorderStrokeGapColor="Color/Paper" LeftBorderStrokeGapTint="100" LeftBorderStrokeGapOverprint="false" BottomBorderStrokeWeight="1" BottomBorderStrokeType="StrokeStyle/$ID/Solid" BottomBorderStrokeColor="Color/Black" BottomBorderStrokeTint="100" BottomBorderStrokeOverprint="false" BottomBorderStrokeGapColor="Color/Paper" BottomBorderStrokeGapTint="100" BottomBorderStrokeGapOverprint="false" RightBorderStrokeWeight="1" RightBorderStrokeType="StrokeStyle/$ID/Solid" RightBorderStrokeColor="Color/Black" RightBorderStrokeTint="100" RightBorderStrokeOverprint="false" RightBorderStrokeGapColor="Color/Paper" RightBorderStrokeGapTint="100" RightBorderStrokeGapOverprint="false" SpaceBefore="4" SpaceAfter="-4" SkipFirstAlternatingStrokeRows="0" SkipLastAlternatingStrokeRows="0" StartRowStrokeCount="0" StartRowStrokeColor="Color/Black" StartRowStrokeWeight="1" StartRowStrokeType="StrokeStyle/$ID/Solid" StartRowStrokeTint="100" StartRowStrokeGapOverprint="false" StartRowStrokeGapColor="Color/Paper" StartRowStrokeGapTint="100" StartRowStrokeOverprint="false" EndRowStrokeCount="0" EndRowStrokeColor="Color/Black" EndRowStrokeWeight="0.25" EndRowStrokeType="StrokeStyle/$ID/Solid" EndRowStrokeTint="100" EndRowStrokeOverprint="false" EndRowStrokeGapColor="Color/Paper" EndRowStrokeGapTint="100" EndRowStrokeGapOverprint="false" SkipFirstAlternatingStrokeColumns="0" SkipLastAlternatingStrokeColumns="0" StartColumnStrokeCount="0" StartColumnStrokeColor="Color/Black" StartColumnStrokeWeight="1" StartColumnStrokeType="StrokeStyle/$ID/Solid" StartColumnStrokeTint="100" StartColumnStrokeOverprint="false" StartColumnStrokeGapColor="Color/Paper" StartColumnStrokeGapTint="100" StartColumnStrokeGapOverprint="false" EndColumnStrokeCount="0" EndColumnStrokeColor="Color/Black" EndColumnStrokeWeight="0.25" EndColumnLineStyle="StrokeStyle/$ID/Solid" EndColumnStrokeTint="100" EndColumnStrokeOverprint="false" EndColumnStrokeGapColor="Color/Paper" EndColumnStrokeGapTint="100" EndColumnStrokeGapOverprint="false" ColumnFillsPriority="false" SkipFirstAlternatingFillRows="0" SkipLastAlternatingFillRows="0" StartRowFillColor="Color/Black" StartRowFillCount="0" StartRowFillTint="20" StartRowFillOverprint="false" EndRowFillCount="0" EndRowFillColor="Swatch/None" EndRowFillTint="100" EndRowFillOverprint="false" SkipFirstAlternatingFillColumns="0" SkipLastAlternatingFillColumns="0" StartColumnFillCount="0" StartColumnFillColor="Color/Black" StartColumnFillTint="20" StartColumnFillOverprint="false" EndColumnFillCount="0" EndColumnFillColor="Swatch/None" EndColumnFillTint="100" EndColumnFillOverprint="false" HeaderRegionSameAsBodyRegion="true" FooterRegionSameAsBodyRegion="true" LeftColumnRegionSameAsBodyRegion="true" RightColumnRegionSameAsBodyRegion="true" HeaderRegionCellStyle="n" FooterRegionCellStyle="n" LeftColumnRegionCellStyle="n" RightColumnRegionCellStyle="n" BodyRegionCellStyle="CellStyle/$ID/[None]"/>
-    <TableStyle Self="myprefixTableStyle/$ID/[Basic Table]" Name="$ID/[Basic Table]" KeyboardShortcut="0 0">
+  <RootTableStyleGroup Self="u6c">
+    <TableStyle Self="TableStyle/$ID/[No table style]" Name="$ID/[No table style]" StrokeOrder="BestJoins" TopBorderStrokeWeight="1" TopBorderStrokeType="StrokeStyle/$ID/Solid" TopBorderStrokeColor="Color/Black" TopBorderStrokeTint="100" TopBorderStrokeOverprint="false" TopBorderStrokeGapColor="Color/Paper" TopBorderStrokeGapTint="100" TopBorderStrokeGapOverprint="false" LeftBorderStrokeWeight="1" LeftBorderStrokeType="StrokeStyle/$ID/Solid" LeftBorderStrokeColor="Color/Black" LeftBorderStrokeTint="100" LeftBorderStrokeOverprint="false" LeftBorderStrokeGapColor="Color/Paper" LeftBorderStrokeGapTint="100" LeftBorderStrokeGapOverprint="false" BottomBorderStrokeWeight="1" BottomBorderStrokeType="StrokeStyle/$ID/Solid" BottomBorderStrokeColor="Color/Black" BottomBorderStrokeTint="100" BottomBorderStrokeOverprint="false" BottomBorderStrokeGapColor="Color/Paper" BottomBorderStrokeGapTint="100" BottomBorderStrokeGapOverprint="false" RightBorderStrokeWeight="1" RightBorderStrokeType="StrokeStyle/$ID/Solid" RightBorderStrokeColor="Color/Black" RightBorderStrokeTint="100" RightBorderStrokeOverprint="false" RightBorderStrokeGapColor="Color/Paper" RightBorderStrokeGapTint="100" RightBorderStrokeGapOverprint="false" SpaceBefore="4" SpaceAfter="-4" SkipFirstAlternatingStrokeRows="0" SkipLastAlternatingStrokeRows="0" StartRowStrokeCount="0" StartRowStrokeColor="Color/Black" StartRowStrokeWeight="1" StartRowStrokeType="StrokeStyle/$ID/Solid" StartRowStrokeTint="100" StartRowStrokeGapOverprint="false" StartRowStrokeGapColor="Color/Paper" StartRowStrokeGapTint="100" StartRowStrokeOverprint="false" EndRowStrokeCount="0" EndRowStrokeColor="Color/Black" EndRowStrokeWeight="0.25" EndRowStrokeType="StrokeStyle/$ID/Solid" EndRowStrokeTint="100" EndRowStrokeOverprint="false" EndRowStrokeGapColor="Color/Paper" EndRowStrokeGapTint="100" EndRowStrokeGapOverprint="false" SkipFirstAlternatingStrokeColumns="0" SkipLastAlternatingStrokeColumns="0" StartColumnStrokeCount="0" StartColumnStrokeColor="Color/Black" StartColumnStrokeWeight="1" StartColumnStrokeType="StrokeStyle/$ID/Solid" StartColumnStrokeTint="100" StartColumnStrokeOverprint="false" StartColumnStrokeGapColor="Color/Paper" StartColumnStrokeGapTint="100" StartColumnStrokeGapOverprint="false" EndColumnStrokeCount="0" EndColumnStrokeColor="Color/Black" EndColumnStrokeWeight="0.25" EndColumnLineStyle="StrokeStyle/$ID/Solid" EndColumnStrokeTint="100" EndColumnStrokeOverprint="false" EndColumnStrokeGapColor="Color/Paper" EndColumnStrokeGapTint="100" EndColumnStrokeGapOverprint="false" ColumnFillsPriority="false" SkipFirstAlternatingFillRows="0" SkipLastAlternatingFillRows="0" StartRowFillColor="Color/Black" StartRowFillCount="0" StartRowFillTint="20" StartRowFillOverprint="false" EndRowFillCount="0" EndRowFillColor="Swatch/None" EndRowFillTint="100" EndRowFillOverprint="false" SkipFirstAlternatingFillColumns="0" SkipLastAlternatingFillColumns="0" StartColumnFillCount="0" StartColumnFillColor="Color/Black" StartColumnFillTint="20" StartColumnFillOverprint="false" EndColumnFillCount="0" EndColumnFillColor="Swatch/None" EndColumnFillTint="100" EndColumnFillOverprint="false" HeaderRegionSameAsBodyRegion="true" FooterRegionSameAsBodyRegion="true" LeftColumnRegionSameAsBodyRegion="true" RightColumnRegionSameAsBodyRegion="true" HeaderRegionCellStyle="n" FooterRegionCellStyle="n" LeftColumnRegionCellStyle="n" RightColumnRegionCellStyle="n" BodyRegionCellStyle="CellStyle/$ID/[None]"/>
+    <TableStyle Self="TableStyle/$ID/[Basic Table]" Name="$ID/[Basic Table]" KeyboardShortcut="0 0">
       <Properties>
         <BasedOn type="string">$ID/[No table style]</BasedOn>
       </Properties>
     </TableStyle>
   </RootTableStyleGroup>
-  <RootObjectStyleGroup Self="myprefixu75">
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[None]" Name="$ID/[None]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/[No paragraph style]" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" CornerOption="None">
+  <RootObjectStyleGroup Self="u75">
+    <ObjectStyle Self="ObjectStyle/$ID/[None]" Name="$ID/[None]" AppliedParagraphStyle="ParagraphStyle/$ID/[No paragraph style]" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" CornerOption="None">
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
       <TextFramePreference TextColumnCount="1" TextColumnGutter="12" TextColumnFixedWidth="144" UseFixedColumnWidth="false" FirstBaselineOffset="AscentOffset" MinimumFirstBaselineOffset="0" VerticalJustification="TopAlign" VerticalThreshold="0" IgnoreWrap="false" UseFlexibleColumnWidth="false" TextColumnMaxWidth="0" AutoSizingType="Off" AutoSizingReferencePoint="CenterPoint" UseMinimumHeightForAutoSizing="false" MinimumHeightForAutoSizing="0" UseMinimumWidthForAutoSizing="false" MinimumWidthForAutoSizing="0" UseNoLineBreaksForAutoSizing="false" VerticalBalanceColumns="false">
@@ -109,15 +109,15 @@
           <TextWrapOffset Top="0" Left="0" Bottom="0" Right="0"/>
         </Properties>
         <ContourOption ContourType="SameAsClipping" IncludeInsideEdges="false" ContourPathName="$ID/"/>
       </TextWrapPreference>
       <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
     </ObjectStyle>
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[Normal Graphics Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Graphics Frame]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/[No paragraph style]" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="false" EnableTextFrameBaselineOptions="false" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixColor/Black" StrokeTint="-1" OverprintStroke="false" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
+    <ObjectStyle Self="ObjectStyle/$ID/[Normal Graphics Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Graphics Frame]" AppliedParagraphStyle="ParagraphStyle/$ID/[No paragraph style]" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="false" EnableTextFrameBaselineOptions="false" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="1" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Color/Black" StrokeTint="-1" OverprintStroke="false" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
       <Properties>
         <BasedOn type="string">$ID/[None]</BasedOn>
       </Properties>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
@@ -148,15 +148,15 @@
       <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="Unknown" StoryOrientation="Unknown" StoryDirection="UnknownDirection"/>
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
       <ObjectStyleObjectEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleStrokeEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleFillEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleContentEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
     </ObjectStyle>
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[Normal Text Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Text Frame]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
+    <ObjectStyle Self="ObjectStyle/$ID/[Normal Text Frame]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Text Frame]" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="false" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
       <Properties>
         <BasedOn type="string">$ID/[None]</BasedOn>
       </Properties>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
@@ -187,15 +187,15 @@
       <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Unknown" StoryDirection="LeftToRightDirection"/>
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
       <ObjectStyleObjectEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleStrokeEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleFillEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleContentEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
     </ObjectStyle>
-    <ObjectStyle Self="myprefixObjectStyle/$ID/[Normal Grid]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Grid]" AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="true" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="myprefixSwatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="myprefixSwatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
+    <ObjectStyle Self="ObjectStyle/$ID/[Normal Grid]" EnableTextFrameAutoSizingOptions="false" EnableExportTagging="false" EnableObjectExportAltTextOptions="false" EnableObjectExportTaggedPdfOptions="false" EnableObjectExportEpubOptions="false" Name="$ID/[Normal Grid]" AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" ApplyNextParagraphStyle="false" EnableFill="true" EnableStroke="true" EnableParagraphStyle="false" EnableTextFrameGeneralOptions="true" EnableTextFrameBaselineOptions="true" EnableStoryOptions="true" EnableTextWrapAndOthers="false" EnableAnchoredObjectOptions="false" CornerRadius="12" FillColor="Swatch/None" FillTint="-1" StrokeWeight="0" MiterLimit="4" EndCap="ButtEndCap" EndJoin="MiterEndJoin" StrokeType="StrokeStyle/$ID/Solid" LeftLineEnd="None" RightLineEnd="None" StrokeColor="Swatch/None" StrokeTint="-1" GapColor="Swatch/None" GapTint="-1" StrokeAlignment="CenterAlignment" Nonprinting="false" GradientFillAngle="0" GradientStrokeAngle="0" AppliedNamedGrid="n" KeyboardShortcut="0 0" TopLeftCornerOption="None" TopRightCornerOption="None" BottomLeftCornerOption="None" BottomRightCornerOption="None" TopLeftCornerRadius="12" TopRightCornerRadius="12" BottomLeftCornerRadius="12" BottomRightCornerRadius="12" EnableFrameFittingOptions="false" CornerOption="None" EnableStrokeAndCornerOptions="true">
       <Properties>
         <BasedOn type="string">$ID/[None]</BasedOn>
       </Properties>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
@@ -227,10 +227,10 @@
       <FrameFittingOption AutoFit="false" LeftCrop="0" TopCrop="0" RightCrop="0" BottomCrop="0" FittingOnEmptyFrame="None" FittingAlignment="TopLeftAnchor"/>
       <ObjectStyleObjectEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleStrokeEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleFillEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
       <ObjectStyleContentEffectsCategorySettings EnableTransparency="true" EnableDropShadow="true" EnableFeather="true" EnableInnerShadow="true" EnableOuterGlow="true" EnableInnerGlow="true" EnableBevelEmboss="true" EnableSatin="true" EnableDirectionalFeather="true" EnableGradientFeather="true"/>
     </ObjectStyle>
   </RootObjectStyleGroup>
-  <TrapPreset Self="myprefixTrapPreset/$ID/k[No Trap Preset]" Name="$ID/k[No Trap Preset]" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
-  <TrapPreset Self="myprefixTrapPreset/$ID/kDefaultTrapStyleName" Name="$ID/kDefaultTrapStyleName" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
+  <TrapPreset Self="TrapPreset/$ID/k[No Trap Preset]" Name="$ID/k[No Trap Preset]" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
+  <TrapPreset Self="TrapPreset/$ID/kDefaultTrapStyleName" Name="$ID/kDefaultTrapStyleName" DefaultTrapWidth="0.25" BlackWidth="0.5" TrapJoin="MiterEndJoin" TrapEnd="MiterTrapEnds" ObjectsToImages="true" ImagesToImages="true" InternalImages="false" OneBitImages="true" ImagePlacement="CenterEdges" StepThreshold="10" BlackColorThreshold="100" BlackDensity="1.6" SlidingTrapThreshold="70" ColorReduction="100"/>
 </idPkg:Styles>
```

#### XML/BackingStory.xml

##### XML/BackingStory.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:BackingStory xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <XmlStory Self="myprefixu83" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
-    <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
-      <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]">
+  <XmlStory Self="u83" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
+    <ParagraphStyleRange AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle">
+      <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]">
         <Content>﻿﻿</Content>
-        <XMLElement Self="myprefixdi3" MarkupTag="XMLTag/Root">
-          <XMLElement Self="myprefixdi3i4" MarkupTag="XMLTag/module" XMLContent="myprefixu10d"/>
+        <XMLElement Self="di3" MarkupTag="XMLTag/Root">
+          <XMLElement Self="di3i4" MarkupTag="XMLTag/module" XMLContent="u10d"/>
         </XMLElement>
         <Content>﻿﻿﻿</Content>
       </CharacterStyleRange>
     </ParagraphStyleRange>
   </XmlStory>
 </idPkg:BackingStory>
```

#### XML/Mapping.xml

##### XML/Mapping.xml

```diff
@@ -1,6 +1,6 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Mapping xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <XMLImportMap Self="myprefixdid2" MarkupTag="XMLTag/bold" MappedStyle="myprefixCharacterStyle/bold"/>
-  <XMLImportMap Self="myprefixdi13f" MarkupTag="XMLTag/italique" MappedStyle="myprefixCharacterStyle/italique"/>
-  <XMLImportMap Self="myprefixdi141" MarkupTag="XMLTag/sup" MappedStyle="myprefixCharacterStyle/sup"/>
+  <XMLImportMap Self="did2" MarkupTag="XMLTag/bold" MappedStyle="CharacterStyle/bold"/>
+  <XMLImportMap Self="di13f" MarkupTag="XMLTag/italique" MappedStyle="CharacterStyle/italique"/>
+  <XMLImportMap Self="di141" MarkupTag="XMLTag/sup" MappedStyle="CharacterStyle/sup"/>
 </idPkg:Mapping>
```

#### XML/Tags.xml

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

```diff
@@ -1,11 +1,11 @@
-00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2731  <?xml version='1
-00000010: 2e30 2720 656e 636f 6469 6e67 3d27 5554  .0' encoding='UT
-00000020: 462d 3827 2073 7461 6e64 616c 6f6e 653d  F-8' standalone=
-00000030: 2779 6573 273f 3e0a 3c69 6450 6b67 3a54  'yes'?>.<idPkg:T
+00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
+00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
+00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
+00000030: 2279 6573 223f 3e0a 3c69 6450 6b67 3a54  "yes"?>.<idPkg:T
 00000040: 6167 7320 786d 6c6e 733a 6964 506b 673d  ags xmlns:idPkg=
 00000050: 2268 7474 703a 2f2f 6e73 2e61 646f 6265  "http://ns.adobe
 00000060: 2e63 6f6d 2f41 646f 6265 496e 4465 7369  .com/AdobeInDesi
 00000070: 676e 2f69 646d 6c2f 312e 302f 7061 636b  gn/idml/1.0/pack
 00000080: 6167 696e 6722 2044 4f4d 5665 7273 696f  aging" DOMVersio
 00000090: 6e3d 2231 302e 3022 3e0a 093c 584d 4c54  n="10.0">..<XMLT
 000000a0: 6167 2053 656c 663d 2258 4d4c 5461 672f  ag Self="XMLTag/
@@ -91,8 +91,8 @@
 000005a0: 4c54 6167 2f73 7570 2220 4e61 6d65 3d22  LTag/sup" Name="
 000005b0: 7375 7022 3e0a 0909 3c50 726f 7065 7274  sup">...<Propert
 000005c0: 6965 733e 0a09 0909 3c54 6167 436f 6c6f  ies>....<TagColo
 000005d0: 7220 7479 7065 3d22 656e 756d 6572 6174  r type="enumerat
 000005e0: 696f 6e22 3e52 6564 3c2f 5461 6743 6f6c  ion">Red</TagCol
 000005f0: 6f72 3e0a 0909 3c2f 5072 6f70 6572 7469  or>...</Properti
 00000600: 6573 3e0a 093c 2f58 4d4c 5461 673e 0a3c  es>..</XMLTag>.<
-00000610: 2f69 6450 6b67 3a54 6167 733e 0a         /idPkg:Tags>.
+00000610: 2f69 6450 6b67 3a54 6167 733e            /idPkg:Tags>
```

#### Comparing `Spreads/Spread_myprefixud8.xml` & `Spreads/Spread_ud8.xml`

 * *Files 12% similar despite different names*

##### Comparing `Spreads/Spread_myprefixud8.xml` & `Spreads/Spread_ud8.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Spread xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Spread Self="myprefixud8" FlattenerOverride="Default" AllowPageShuffle="true" ItemTransform="1 0 0 1 0 0" ShowMasterItems="true" PageCount="1" BindingLocation="0" PageTransitionType="None" PageTransitionDirection="NotApplicable" PageTransitionDuration="Medium">
+  <Spread Self="ud8" FlattenerOverride="Default" AllowPageShuffle="true" ItemTransform="1 0 0 1 0 0" ShowMasterItems="true" PageCount="1" BindingLocation="0" PageTransitionType="None" PageTransitionDirection="NotApplicable" PageTransitionDuration="Medium">
     <FlattenerPreference LineArtAndTextResolution="300" GradientAndMeshResolution="150" ClipComplexRegions="false" ConvertAllStrokesToOutlines="false" ConvertAllTextToOutlines="false">
       <Properties>
         <RasterVectorBalance type="double">50</RasterVectorBalance>
       </Properties>
     </FlattenerPreference>
-    <Page Self="myprefixudd" AppliedAlternateLayout="u9b" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="1" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="ua5" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
+    <Page Self="udd" AppliedAlternateLayout="u9b" LayoutRule="Off" SnapshotBlendingMode="IgnoreLayoutSnapshots" OptionalPage="false" GeometricBounds="0 0 759.6850393700788 566.9291338582677" ItemTransform="1 0 0 1 0 -379.8425196850394" Name="1" AppliedTrapPreset="TrapPreset/$ID/kDefaultTrapStyleName" OverrideList="" AppliedMaster="ua5" MasterPageTransform="1 0 0 1 0 0" TabOrder="" GridStartingPoint="TopOutside" UseMasterGrid="true">
       <Properties>
         <Descriptor type="list">
           <ListItem type="string"/>
           <ListItem type="enumeration">Arabic</ListItem>
           <ListItem type="boolean">true</ListItem>
           <ListItem type="boolean">false</ListItem>
           <ListItem type="long">1</ListItem>
@@ -21,15 +21,15 @@
       <MarginPreference ColumnCount="1" ColumnGutter="12" Top="36" Bottom="36" Left="36" Right="36" ColumnDirection="Horizontal" ColumnsPositions="0 494.92913385826773"/>
       <GridDataInformation FontStyle="Regular" PointSize="12" CharacterAki="0" LineAki="9" HorizontalScale="100" VerticalScale="100" LineAlignment="LeftOrTopLineJustify" GridAlignment="AlignEmCenter" CharacterAlignment="AlignEmCenter">
         <Properties>
           <AppliedFont type="string">Minion Pro</AppliedFont>
         </Properties>
       </GridDataInformation>
     </Page>
-    <Rectangle Self="myprefixudf" ContentType="GraphicType" StoryTitle="$ID/" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 17.763779527559194 -391.27559055118115">
+    <Rectangle Self="udf" ContentType="GraphicType" StoryTitle="$ID/" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 17.763779527559194 -391.27559055118115">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="144.56692913385828 58.582677165354326" LeftDirection="144.56692913385828 58.582677165354326" RightDirection="144.56692913385828 58.582677165354326"/>
               <PathPointType Anchor="144.56692913385828 199.46456692913392" LeftDirection="144.56692913385828 199.46456692913392" RightDirection="144.56692913385828 199.46456692913392"/>
               <PathPointType Anchor="403.46456692913387 199.46456692913392" LeftDirection="403.46456692913387 199.46456692913392" RightDirection="403.46456692913387 199.46456692913392"/>
@@ -48,16 +48,63 @@
       <FrameFittingOption RightCrop="44.102362204724386" BottomCrop="219.1181102362204"/>
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
+      <Image Self="u14a" Space="$ID/#Links_RGB" ActualPpi="72 72" EffectivePpi="72 72" ImageRenderingIntent="UseColorSettings" OverriddenPageItemProps="" LocalDisplaySetting="Default" ImageTypeName="$ID/JPEG" AppliedObjectStyle="ObjectStyle/$ID/[None]" ItemTransform="1 0 0 1 144.56692913385825 58.58267716535431" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" Visible="true" Name="$ID/">
+        <Properties>
+          <Profile type="string">$ID/None</Profile>
+          <GraphicBounds Left="0" Top="0" Right="303" Bottom="360"/>
+        </Properties>
+        <TextWrapPreference Inverse="false" ApplyToMasterPageOnly="false" TextWrapSide="BothSides" TextWrapMode="None">
+          <Properties>
+            <TextWrapOffset Top="0" Left="0" Bottom="0" Right="0"/>
+          </Properties>
+          <ContourOption ContourType="SameAsClipping" IncludeInsideEdges="false" ContourPathName="$ID/"/>
+        </TextWrapPreference>
+        <MetadataPacketPreference>
+          <Properties>
+            <Contents>&lt;?xpacket begin=&quot;﻿&quot; id=&quot;W5M0MpCehiHzreSzNTczkc9d&quot;?&gt;
+&lt;x:xmpmeta xmlns:x=&quot;adobe:ns:meta/&quot; x:xmptk=&quot;Adobe XMP Core 5.6-c011 79.156289, 2014/03/31-23:39:12        &quot;&gt;
+   &lt;rdf:RDF xmlns:rdf=&quot;http://www.w3.org/1999/02/22-rdf-syntax-ns#&quot;&gt;
+      &lt;rdf:Description rdf:about=&quot;&quot;
+            xmlns:tiff=&quot;http://ns.adobe.com/tiff/1.0/&quot;
+            xmlns:exif=&quot;http://ns.adobe.com/exif/1.0/&quot;&gt;
+         &lt;tiff:XResolution&gt;72/1&lt;/tiff:XResolution&gt;
+         &lt;tiff:YResolution&gt;72/1&lt;/tiff:YResolution&gt;
+         &lt;tiff:ResolutionUnit&gt;2&lt;/tiff:ResolutionUnit&gt;
+         &lt;tiff:YCbCrPositioning&gt;1&lt;/tiff:YCbCrPositioning&gt;
+         &lt;exif:ColorSpace&gt;1&lt;/exif:ColorSpace&gt;
+         &lt;exif:PixelXDimension&gt;360&lt;/exif:PixelXDimension&gt;
+         &lt;exif:PixelYDimension&gt;303&lt;/exif:PixelYDimension&gt;
+         &lt;exif:SceneCaptureType&gt;0&lt;/exif:SceneCaptureType&gt;
+         &lt;exif:ExifVersion&gt;0221&lt;/exif:ExifVersion&gt;
+         &lt;exif:FlashpixVersion&gt;0100&lt;/exif:FlashpixVersion&gt;
+         &lt;exif:ComponentsConfiguration&gt;
+            &lt;rdf:Seq&gt;
+               &lt;rdf:li&gt;1&lt;/rdf:li&gt;
+               &lt;rdf:li&gt;2&lt;/rdf:li&gt;
+               &lt;rdf:li&gt;3&lt;/rdf:li&gt;
+               &lt;rdf:li&gt;0&lt;/rdf:li&gt;
+            &lt;/rdf:Seq&gt;
+         &lt;/exif:ComponentsConfiguration&gt;
+      &lt;/rdf:Description&gt;
+   &lt;/rdf:RDF&gt;
+&lt;/x:xmpmeta&gt;
+&lt;?xpacket end=&quot;r&quot;?&gt;</Contents>
+          </Properties>
+        </MetadataPacketPreference>
+        <Link Self="u14e" AssetURL="$ID/" AssetID="$ID/" LinkResourceURI="file:../../IDML/media/bouboune.jpg" LinkResourceFormat="$ID/JPEG" StoredState="Normal" LinkClassID="35906" LinkClientID="257" LinkResourceModified="false" LinkObjectModified="false" ShowInUI="true" CanEmbed="true" CanUnembed="true" CanPackage="true" ImportPolicy="NoAutoImport" ExportPolicy="NoAutoExport" LinkImportStamp="file 129767622980000000 27644" LinkImportModificationTime="2012-03-21T01:11:38" LinkImportTime="2014-09-24T14:59:30" LinkResourceSize="0~6bfc"/>
+        <ClippingPathSettings ClippingType="None" InvertPath="false" IncludeInsideEdges="false" RestrictToFrame="false" UseHighResolutionImage="true" Threshold="25" Tolerance="2" InsetFrame="0" AppliedPathName="$ID/" Index="-1"/>
+        <ImageIOPreference ApplyPhotoshopClippingPath="true" AllowAutoEmbedding="true" AlphaChannelName="$ID/"/>
+      </Image>
     </Rectangle>
-    <TextFrame Self="myprefixuf3" ParentStory="myprefixue1" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 237.82677165354335 -166.29921259842524">
+    <TextFrame Self="uf3" ParentStory="ue1" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 237.82677165354335 -166.29921259842524">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="-76.06299212598424 -19.842519685039377" LeftDirection="-76.06299212598424 -19.842519685039377" RightDirection="-76.06299212598424 -19.842519685039377"/>
               <PathPointType Anchor="-76.06299212598424 -0.9448818897638205" LeftDirection="-76.06299212598424 -0.9448818897638205" RightDirection="-76.06299212598424 -0.9448818897638205"/>
               <PathPointType Anchor="182.83464566929132 -0.9448818897638205" LeftDirection="182.83464566929132 -0.9448818897638205" RightDirection="182.83464566929132 -0.9448818897638205"/>
@@ -75,15 +122,15 @@
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
     </TextFrame>
-    <TextFrame Self="myprefixu109" ParentStory="myprefixuf7" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 298.77165354330714 -98.26771653543307">
+    <TextFrame Self="u109" ParentStory="uf7" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[Normal Text Frame]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 298.77165354330714 -98.26771653543307">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="-137.00787401574803 -64.25196850393701" LeftDirection="-137.00787401574803 -64.25196850393701" RightDirection="-137.00787401574803 -64.25196850393701"/>
               <PathPointType Anchor="-137.00787401574803 51.968503937007945" LeftDirection="-137.00787401574803 51.968503937007945" RightDirection="-137.00787401574803 51.968503937007945"/>
               <PathPointType Anchor="121.88976377952753 51.968503937007945" LeftDirection="121.88976377952753 51.968503937007945" RightDirection="121.88976377952753 51.968503937007945"/>
@@ -101,15 +148,15 @@
       <ObjectExportOption EpubType="$ID/" UseExistingImage="false" CustomHeightType="DefaultHeight" CustomHeight="$ID/" CustomWidthType="DefaultWidth" CustomWidth="$ID/" AltTextSourceType="SourceXMLStructure" ActualTextSourceType="SourceXMLStructure" CustomAltText="$ID/" CustomActualText="$ID/" ApplyTagType="TagFromStructure" CustomImageConversion="false" ImageConversionType="JPEG" ImageExportResolution="Ppi300" GIFOptionsPalette="AdaptivePalette" GIFOptionsInterlaced="true" JPEGOptionsQuality="High" JPEGOptionsFormat="BaselineEncoding" ImageAlignment="AlignLeft" ImageSpaceBefore="0" ImageSpaceAfter="0" UseImagePageBreak="false" ImagePageBreak="PageBreakBefore" CustomImageAlignment="false" SpaceUnit="CssPixel" CustomLayout="false" CustomLayoutType="AlignmentAndSpacing" UseOriginalImage="false">
         <Properties>
           <AltMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
           <ActualMetadataProperty NamespacePrefix="$ID/" PropertyPath="$ID/"/>
         </Properties>
       </ObjectExportOption>
     </TextFrame>
-    <TextFrame Self="myprefixu11f" ParentStory="myprefixu10d" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="myprefixua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="myprefixObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 16.062992125984294 -357.16535433070874">
+    <TextFrame Self="u11f" ParentStory="u10d" PreviousTextFrame="n" NextTextFrame="n" ContentType="TextType" ParentInterfaceChangeCount="" TargetInterfaceChangeCount="" LastUpdatedInterfaceChangeCount="" OverriddenPageItemProps="" HorizontalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" VerticalLayoutConstraints="FlexibleDimension FixedDimension FlexibleDimension" GradientFillStart="0 0" GradientFillLength="0" GradientFillAngle="0" GradientStrokeStart="0 0" GradientStrokeLength="0" GradientStrokeAngle="0" ItemLayer="ua4" Locked="false" LocalDisplaySetting="Default" GradientFillHiliteLength="0" GradientFillHiliteAngle="0" GradientStrokeHiliteLength="0" GradientStrokeHiliteAngle="0" AppliedObjectStyle="ObjectStyle/$ID/[None]" Visible="true" Name="$ID/" ItemTransform="1 0 0 1 16.062992125984294 -357.16535433070874">
       <Properties>
         <PathGeometry>
           <GeometryPathType PathOpen="false">
             <PathPointArray>
               <PathPointType Anchor="141.73228346456693 19.84251968503935" LeftDirection="141.73228346456693 19.84251968503935" RightDirection="141.73228346456693 19.84251968503935"/>
               <PathPointType Anchor="141.73228346456693 310.8661417322836" LeftDirection="141.73228346456693 310.8661417322836" RightDirection="141.73228346456693 310.8661417322836"/>
               <PathPointType Anchor="409.13385826771633 310.8661417322836" LeftDirection="409.13385826771633 310.8661417322836" RightDirection="409.13385826771633 310.8661417322836"/>
```

#### Comparing `Stories/Story_myprefixu10d.xml` & `Stories/Story_u10d.xml`

 * *Files 22% similar despite different names*

##### Comparing `Stories/Story_myprefixu10d.xml` & `Stories/Story_u10d.xml`

```diff
@@ -1,16 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Story Self="myprefixu10d" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
+  <Story Self="u10d" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
-    <XMLElement Self="myprefixdi3i4" MarkupTag="XMLTag/module" XMLContent="myprefixu10d">
-      <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
-        <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]">
-          <XMLElement Self="myprefixdi3i4i1" MarkupTag="XMLTag/main_picture"/>
-          <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1"/>
-          <XMLElement Self="myprefixdi3i4i3" MarkupTag="XMLTag/Story" XMLContent="myprefixuf7"/>
+    <XMLElement Self="di3i4" MarkupTag="XMLTag/module" XMLContent="u10d">
+      <ParagraphStyleRange AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle">
+        <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]">
+          <XMLElement Self="di3i4i1" MarkupTag="XMLTag/main_picture" XMLContent="u14a">
+            <XMLAttribute Self="di3i4i1XMLAttributenhref" Name="href" Value="file:../../IDML/media/bouboune.jpg"/>
+          </XMLElement>
+          <XMLElement Self="di3i4i2" MarkupTag="XMLTag/headline" XMLContent="ue1"/>
+          <XMLElement Self="di3i4i3" MarkupTag="XMLTag/Story" XMLContent="uf7"/>
         </CharacterStyleRange>
       </ParagraphStyleRange>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

#### Comparing `Stories/Story_myprefixue1.xml` & `Stories/Story_ue1.xml`

 * *Files 17% similar despite different names*

##### Comparing `Stories/Story_myprefixue1.xml` & `Stories/Story_ue1.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Story Self="myprefixue1" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
+  <Story Self="ue1" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
-    <XMLElement Self="myprefixdi3i4i2" MarkupTag="XMLTag/headline" XMLContent="myprefixue1">
-      <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle">
-        <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" FillColor="myprefixColor/uba" FontStyle="Bold">
+    <XMLElement Self="di3i4i2" MarkupTag="XMLTag/headline" XMLContent="ue1">
+      <ParagraphStyleRange AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle">
+        <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]" FillColor="Color/uba" FontStyle="Bold">
           <Content>The Life Aquatic with Steve Zissou</Content>
         </CharacterStyleRange>
       </ParagraphStyleRange>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

#### Comparing `Stories/Story_myprefixuf7.xml` & `Stories/Story_uf7.xml`

 * *Files 14% similar despite different names*

##### Comparing `Stories/Story_myprefixuf7.xml` & `Stories/Story_uf7.xml`

```diff
@@ -1,57 +1,57 @@
 <?xml version="1.0" encoding="utf-8"?>
 <idPkg:Story xmlns:idPkg="http://ns.adobe.com/AdobeInDesign/idml/1.0/packaging" DOMVersion="10.0">
-  <Story Self="myprefixuf7" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
+  <Story Self="uf7" AppliedTOCStyle="n" TrackChanges="false" StoryTitle="$ID/" AppliedNamedGrid="n">
     <StoryPreference OpticalMarginAlignment="false" OpticalMarginSize="12" FrameType="TextFrameType" StoryOrientation="Horizontal" StoryDirection="LeftToRightDirection"/>
     <InCopyExportOption IncludeGraphicProxies="true" IncludeAllResources="false"/>
-    <XMLElement Self="myprefixdi3i4i3" MarkupTag="XMLTag/Story" XMLContent="myprefixuf7">
-      <ParagraphStyleRange AppliedParagraphStyle="myprefixParagraphStyle/$ID/NormalParagraphStyle" Justification="LeftJustified">
-        <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10"/>
-        <XMLElement Self="myprefixdi3i4i3i1" MarkupTag="XMLTag/article">
-          <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10">
+    <XMLElement Self="di3i4i3" MarkupTag="XMLTag/Story" XMLContent="uf7">
+      <ParagraphStyleRange AppliedParagraphStyle="ParagraphStyle/$ID/NormalParagraphStyle" Justification="LeftJustified">
+        <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]" PointSize="10"/>
+        <XMLElement Self="di3i4i3i1" MarkupTag="XMLTag/article">
+          <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]" PointSize="10">
             <Content>While oceanographer and documentarian</Content>
           </CharacterStyleRange>
-          <XMLElement MarkupTag="XMLTag/bold" Self="myprefixdi3i4i3i1i1">
-            <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/bold" PointSize="10">
+          <XMLElement MarkupTag="XMLTag/bold" Self="di3i4i3i1i1">
+            <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/bold" PointSize="10">
               <Properties/>
               <Content>Steve Zissou (Bill Murray) is working on his latest documentary at sea, his best friend Esteban du Plantier (Seymour Cassel)</Content>
             </CharacterStyleRange>
           </XMLElement>
-          <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10">
+          <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]" PointSize="10">
             <Properties/>
             <Content>is eaten by a creature Zissou describes as a &quot;Jaguar shark.&quot; For his next project, Zissou is determined to document the shark's destruction.
             The crew aboard Zissou's research vessel</Content>
           </CharacterStyleRange>
-          <XMLElement MarkupTag="XMLTag/italique" Self="myprefixdi3i4i3i1i2">
-            <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/italique" PointSize="10">
+          <XMLElement MarkupTag="XMLTag/italique" Self="di3i4i3i1i2">
+            <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/italique" PointSize="10">
               <Properties/>
               <Content>Belafonte</Content>
             </CharacterStyleRange>
           </XMLElement>
-          <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10">
+          <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]" PointSize="10">
             <Properties/>
             <Content>includes</Content>
           </CharacterStyleRange>
-          <XMLElement MarkupTag="XMLTag/italique" Self="myprefixdi3i4i3i1i3">
-            <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/italique" PointSize="10">
+          <XMLElement MarkupTag="XMLTag/italique" Self="di3i4i3i1i3">
+            <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/italique" PointSize="10">
               <Properties/>
               <Content>Pelé dos Santos (Seu Jorge)</Content>
             </CharacterStyleRange>
           </XMLElement>
-          <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" PointSize="10">
+          <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]" PointSize="10">
             <Properties/>
             <Content>, a safety expert and Brazilian musician who sings David Bowie songs in Portuguese, and Klaus Daimler (Willem Dafoe), the German second-in-command who viewed Zissou and Esteban as father figures</Content>
           </CharacterStyleRange>
         </XMLElement>
-        <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]">
+        <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]">
           <Br/>
           <Br/>
         </CharacterStyleRange>
-        <XMLElement Self="myprefixdi3i4i3i2" MarkupTag="XMLTag/informations">
-          <CharacterStyleRange AppliedCharacterStyle="myprefixCharacterStyle/$ID/[No character style]" FontStyle="Italic" PointSize="10">
+        <XMLElement Self="di3i4i3i2" MarkupTag="XMLTag/informations">
+          <CharacterStyleRange AppliedCharacterStyle="CharacterStyle/$ID/[No character style]" FontStyle="Italic" PointSize="10">
             <Content>The Life Aquatic with Steve Zissou is an American comedy-drama film directed, written, and co-produced by Wes Anderson.</Content>
           </CharacterStyleRange>
         </XMLElement>
       </ParagraphStyleRange>
     </XMLElement>
   </Story>
 </idPkg:Story>
```

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-bloc-notes.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-bloc-notes.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-bloc-notes.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs-3pages.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-courrier-des-lecteurs.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-edito.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-edito.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-edito.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/magazineA-template.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/magazineA-template.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/Jacques-Yves_Cousteau.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/media/bouboune.jpg` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/bouboune.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/media/default.jpg` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/media/default2.jpg` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/media/default2.jpg`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/module1.pdf` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/module1.pdf`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/package-pirate.zip` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/package-pirate.zip`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/page-9modules.idml` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.idml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/IDML/page-9modules.indd` & `SimpleIDML-1.1.6a1/tests/regressiontests/IDML/page-9modules.indd`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/SOAP/indesign-service.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/SOAP/indesign-service.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent2.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-forcecontent3.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-ignorecontent.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-nested-tags.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-extra-nodes2.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete-informations.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-delete.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-false.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-with-setcontent-remove-br.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml-without-picture.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/XML/article-1photo_import-xml.xml` & `SimpleIDML-1.1.6a1/tests/regressiontests/XML/article-1photo_import-xml.xml`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/components.py` & `SimpleIDML-1.1.6a1/tests/regressiontests/components.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/extras.py` & `SimpleIDML-1.1.6a1/tests/regressiontests/extras.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/id_package.py` & `SimpleIDML-1.1.6a1/tests/regressiontests/id_package.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/idml.py` & `SimpleIDML-1.1.6a1/tests/regressiontests/idml.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/indesign.py` & `SimpleIDML-1.1.6a1/tests/regressiontests/indesign.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/regressiontests/utils.py` & `SimpleIDML-1.1.6a1/tests/regressiontests/utils.py`

 * *Files identical despite different names*

### Comparing `SimpleIDML-1.1.3/tests/runtests.py` & `SimpleIDML-1.1.6a1/tests/runtests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
 import sys
 import unittest
 
 REGRESSION_TEST_DIRNAME = 'regressiontests'
-REGRESSION_TEST_DIR = os.path.join(os.path.dirname(__file__), REGRESSION_TEST_DIRNAME)
 
 sys.path.insert(0, os.path.join('..', 'src'))
 
 
 def load_suite_tests(only=None):
     only_module, only_test_case = None, None
     if only:
         args = only.split(".")
         only_module = args[0]
         only_test_case = args[1:] and args[1] or None
         only_function = args[2:] and args[2] or None
     suites = []
-    for dirpath, dirnames, filenames in os.walk(REGRESSION_TEST_DIR):
+    for dirpath, dirnames, filenames in os.walk(REGRESSION_TEST_DIRNAME):
         for f in filenames:
             basename, ext = os.path.splitext(f)
             if (ext == '.py') and (not only_module or (only_module == basename)):
                 modname = "%s.%s" % ('.'.join(dirpath.split('/')), basename)
                 package = __import__(modname, globals(), locals(), [], 0)
                 mod = sys.modules[modname]
                 if hasattr(mod, 'suite'):
```

