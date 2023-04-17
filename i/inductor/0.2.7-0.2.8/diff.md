# Comparing `tmp/inductor-0.2.7.tar.gz` & `tmp/inductor-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/workspaces/inductor/dist/.tmp-86mv_xut/inductor-0.2.7.tar", last modified: Thu Mar 30 17:34:46 2023, max compression
+gzip compressed data, was "/workspaces/inductor/dist/.tmp-oe8ppd00/inductor-0.2.8.tar", last modified: Mon Apr 17 10:13:58 2023, max compression
```

## Comparing `inductor-0.2.7.tar` & `inductor-0.2.8.tar`

### file list

```diff
@@ -1,610 +1,610 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:46.000000 inductor-0.2.7/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3130 2023-01-26 14:41:07.000000 inductor-0.2.7/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2022-12-18 07:02:56.000000 inductor-0.2.7/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)      202 2023-03-30 17:34:46.000000 inductor-0.2.7/PKG-INFO
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32836 2023-03-08 16:33:31.000000 inductor-0.2.7/inductor/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6459 2023-03-08 16:33:31.000000 inductor-0.2.7/inductor/cli.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/compute/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      169 2022-12-18 07:02:56.000000 inductor-0.2.7/inductor/compute/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1675 2023-03-08 16:33:31.000000 inductor-0.2.7/inductor/compute/common.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1747 2022-12-18 07:02:56.000000 inductor-0.2.7/inductor/compute/local.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10427 2023-03-23 19:54:50.000000 inductor-0.2.7/inductor/conftest.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/data/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      101 2022-12-18 07:02:56.000000 inductor-0.2.7/inductor/data/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/data/table/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      113 2022-12-18 07:02:56.000000 inductor-0.2.7/inductor/data/table/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24069 2023-03-10 17:04:19.000000 inductor-0.2.7/inductor/data/table/dynamodb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    28123 2023-02-23 06:08:55.000000 inductor-0.2.7/inductor/data/table/mysql.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30169 2023-02-23 06:08:55.000000 inductor-0.2.7/inductor/data/table/postgresql.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17688 2023-02-23 06:08:55.000000 inductor-0.2.7/inductor/data/table/snowflake.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22985 2023-02-23 06:08:55.000000 inductor-0.2.7/inductor/data/table/sqlite.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13835 2023-02-23 06:08:55.000000 inductor-0.2.7/inductor/data/table/table.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    36574 2023-03-08 16:33:31.000000 inductor-0.2.7/inductor/data/table/table_catalog.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4829 2023-03-08 16:33:31.000000 inductor-0.2.7/inductor/data/table/table_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3648 2023-03-24 06:34:54.000000 inductor-0.2.7/inductor/environment.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/ml/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      109 2022-12-18 07:02:56.000000 inductor-0.2.7/inductor/ml/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22685 2023-03-02 05:05:13.000000 inductor-0.2.7/inductor/ml/model_store.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/ui/
--rw-r--r--   0 vscode    (1000) vscode    (1000)   108018 2023-03-20 16:48:22.000000 inductor-0.2.7/inductor/ui/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/ui/frontend/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/ui/frontend/build/
--rw-r--r--   0 vscode    (1000) vscode    (1000)   102942 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/asset-manifest.json
--rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-03-30 16:55:47.000000 inductor-0.2.7/inductor/ui/frontend/build/favicon.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)      751 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/index.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5347 2023-03-30 16:55:47.000000 inductor-0.2.7/inductor/ui/frontend/build/logo192.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9664 2023-03-30 16:55:47.000000 inductor-0.2.7/inductor/ui/frontend/build/logo512.png
--rw-r--r--   0 vscode    (1000) vscode    (1000)      489 2023-03-30 16:55:47.000000 inductor-0.2.7/inductor/ui/frontend/build/manifest.json
--rw-r--r--   0 vscode    (1000) vscode    (1000)       67 2023-03-30 16:55:47.000000 inductor-0.2.7/inductor/ui/frontend/build/robots.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor/ui/frontend/build/static/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:46.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4597 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10592 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)  1360865 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/main.742afa3c.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3257 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)  5214586 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/main.742afa3c.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8169 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9826 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2696 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1091 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1970 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1132 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1820 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1005 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1793 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2868 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3794 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1460 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3292 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8448 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9738 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5704 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1275 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2061 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2703 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1305 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2617 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8874 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15381 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      447 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11751 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1126 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1946 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1993 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3062 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7785 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25599 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9397 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10636 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2209 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5571 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10479 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1252 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6229 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12983 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2088 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2750 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1931 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4683 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1643 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1539 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3685 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1629 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2793 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6635 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      555 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1157 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1347 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2745 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2268 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2827 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3931 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2105 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4566 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1477 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2844 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6130 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13815 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2363 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3181 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      964 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1934 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3306 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4325 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10896 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11926 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5348 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6717 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1699 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4190 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3932 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3293 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5068 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4839 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10843 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5246 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11994 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22720 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9262 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32789 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3553 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1468 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3657 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3511 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7049 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      329 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1292 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2502 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2477 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5019 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1843 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4336 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1113 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2398 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3687 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4618 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1498 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4000 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2874 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2595 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10400 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2155 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1836 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5561 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1464 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3762 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      631 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1360 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      619 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1561 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1204 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2303 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1904 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2097 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5052 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1267 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3252 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5609 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17469 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2267 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2534 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9993 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1245 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3378 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10315 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    29173 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1642 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1052 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2350 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1158 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2337 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2638 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2356 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4306 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3261 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12510 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1272 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2740 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      479 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1180 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2266 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      779 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1689 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15972 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12391 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      490 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2604 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3309 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6138 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8413 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8989 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2156 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      677 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1487 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2777 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9777 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1917 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4290 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6162 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15753 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2314 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9503 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3232 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5553 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1810 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3897 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1645 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3459 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3864 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7426 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      722 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1322 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      438 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      971 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7370 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1022 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1750 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1185 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2354 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7506 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3988 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7058 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1577 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2582 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5362 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2050 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1965 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2784 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1989 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2378 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5271 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4876 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14014 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1130 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4441 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4717 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9050 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1817 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6690 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      853 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1457 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1715 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2984 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1434 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3531 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2717 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6836 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2878 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16647 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4057 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12093 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      708 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1624 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1222 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2972 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1023 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2428 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1030 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2247 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2688 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9233 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1297 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5913 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7403 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1229 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2426 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2190 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4788 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2666 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5293 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2970 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1295 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3325 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8946 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25523 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      931 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2525 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5616 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12658 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3526 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11416 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2910 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9236 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2219 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5171 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      804 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1584 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2768 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5680 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2736 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      851 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1662 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1385 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2413 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1202 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2159 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19283 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3033 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8872 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4273 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17044 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18305 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2341 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5232 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1860 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3680 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1134 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2044 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2304 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4030 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2053 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3050 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1568 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      534 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1078 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2049 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7158 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      954 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1736 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1259 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2425 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4993 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      984 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2577 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1393 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3093 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1523 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2748 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3968 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4996 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2905 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5972 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2926 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12128 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17309 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1908 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1975 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1107 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2686 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1691 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3919 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2168 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3951 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1620 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4108 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1061 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2603 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1513 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2837 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2488 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6656 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7750 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22085 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8201 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23130 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9480 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    28299 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6357 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8308 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2204 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3739 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2408 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4611 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      759 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      606 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1520 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4463 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      539 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1040 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1243 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3432 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4534 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3085 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8744 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2795 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6887 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3700 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6709 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2707 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4863 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5647 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9609 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2360 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4307 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1962 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4038 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1698 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4006 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1254 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2090 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2230 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7205 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1552 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4667 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10058 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1066 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2112 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1546 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4508 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      837 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1798 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4544 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5371 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3808 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8379 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1024 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2037 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1564 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4835 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3822 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8980 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2743 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6512 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7790 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17100 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3558 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3729 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8105 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4282 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8817 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1567 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4106 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7321 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16385 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1617 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3717 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      907 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1991 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3431 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13007 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1795 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4250 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1325 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2139 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      960 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2458 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3037 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11612 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4321 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1964 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2913 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    33625 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    34751 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3514 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4573 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2627 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1782 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3922 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3990 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7867 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3272 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7429 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1012 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3428 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7557 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25986 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      900 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2806 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4843 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8564 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2700 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7260 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2946 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3785 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14076 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1218 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2896 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1853 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4129 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4518 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14101 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2620 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10005 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1164 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2589 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2319 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9303 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1565 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3551 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1654 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4076 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2065 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3463 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2652 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3930 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1486 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3810 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2127 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4495 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4464 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3921 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5335 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1496 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3628 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2357 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3453 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1587 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2520 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14461 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14997 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3191 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1883 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1462 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2361 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2484 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5515 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1408 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3490 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2249 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1602 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4465 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2158 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5043 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1922 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1376 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2063 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4182 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10979 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2213 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5936 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1343 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-03-30 16:56:06.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6304 2023-03-30 16:56:07.000000 inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2927 2022-12-18 07:02:56.000000 inductor-0.2.7/inductor/util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      202 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    61729 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       46 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      363 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-03-30 17:34:44.000000 inductor-0.2.7/inductor.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      341 2023-03-08 16:33:31.000000 inductor-0.2.7/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      808 2023-03-30 17:34:46.000000 inductor-0.2.7/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:58.000000 inductor-0.2.8/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3130 2023-01-26 14:41:07.000000 inductor-0.2.8/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2022-12-18 07:02:56.000000 inductor-0.2.8/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      276 2023-04-17 10:13:58.000000 inductor-0.2.8/PKG-INFO
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32836 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6459 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/cli.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/compute/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      169 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/compute/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1675 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/compute/common.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1747 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/compute/local.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10427 2023-03-23 19:54:50.000000 inductor-0.2.8/inductor/conftest.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/data/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      101 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/data/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/data/table/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      113 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/data/table/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24069 2023-03-10 17:04:19.000000 inductor-0.2.8/inductor/data/table/dynamodb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    28123 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/mysql.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    30169 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/postgresql.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17688 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/snowflake.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22985 2023-02-23 06:08:55.000000 inductor-0.2.8/inductor/data/table/sqlite.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13842 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/data/table/table.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    36687 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/data/table/table_catalog.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4829 2023-03-08 16:33:31.000000 inductor-0.2.8/inductor/data/table/table_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3640 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/environment.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ml/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      109 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/ml/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22685 2023-03-02 05:05:13.000000 inductor-0.2.8/inductor/ml/model_store.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   108271 2023-04-14 16:23:19.000000 inductor-0.2.8/inductor/ui/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/frontend/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/frontend/build/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   102942 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/asset-manifest.json
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      153 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/favicon.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      751 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/index.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5347 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/logo192.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9664 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/logo512.png
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      489 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/manifest.json
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       67 2023-04-17 10:09:38.000000 inductor-0.2.8/inductor/ui/frontend/build/robots.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor/ui/frontend/build/static/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4597 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10592 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)  1360865 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3257 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)  5214586 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8169 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9826 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2696 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1091 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1970 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1132 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1820 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1005 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1793 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2868 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3794 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1460 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3292 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8448 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9738 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5704 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1275 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2061 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2703 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1305 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2617 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8874 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15381 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      447 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11751 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1126 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1946 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1993 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3062 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7785 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25599 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9397 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10636 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2209 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5571 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10479 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1252 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6229 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12983 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2088 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2750 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1931 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4683 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1643 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1539 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3685 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1629 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2793 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6635 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      555 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1157 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1347 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2745 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2268 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2827 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3931 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2105 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4566 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1477 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2844 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6130 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13815 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2363 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3181 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      964 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1934 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3306 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4325 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10896 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11926 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5348 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6717 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1699 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4190 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3932 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3293 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5068 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4839 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10843 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5246 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11994 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22720 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9262 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32789 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3553 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1468 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3657 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3511 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7049 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      329 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1292 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2502 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2477 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5019 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1843 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4336 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1113 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2398 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3687 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4618 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1498 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4000 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2874 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2595 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10400 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2155 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1836 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5561 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1464 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3762 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      631 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1360 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      619 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1561 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1204 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2303 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1904 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2097 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5052 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1267 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3252 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5609 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17469 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2267 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2534 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9993 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1245 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3378 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10315 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    29173 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1642 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1052 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2350 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1158 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2337 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2638 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2356 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4306 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3261 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12510 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1272 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2740 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      479 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1105 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1180 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2266 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      779 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1689 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15972 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12391 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      490 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2604 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3309 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6138 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8413 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8989 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2922 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2156 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      677 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1487 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2777 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9777 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1917 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4290 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6162 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15753 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2314 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9503 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3232 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5553 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1810 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3897 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1645 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3459 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3864 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7426 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      722 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1322 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      438 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      971 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      399 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7370 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1022 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1750 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1185 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1938 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2354 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7506 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3988 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7058 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1577 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2582 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      633 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5362 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      860 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2050 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1965 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2784 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1989 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2378 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5271 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4876 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14014 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1130 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4441 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4717 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9050 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1817 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6690 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      853 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1457 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1715 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2984 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1434 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3531 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2717 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6836 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2878 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16647 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4057 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12093 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      708 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1624 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1222 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2972 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1023 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2428 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1030 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2247 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2688 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9233 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1297 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5913 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7403 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1229 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2426 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2190 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4788 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2666 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5293 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2970 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1295 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3325 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8946 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25523 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      931 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2525 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5616 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12658 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3526 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11416 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2910 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9236 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2219 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5171 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      804 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1584 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2768 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5680 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2736 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      851 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1662 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1385 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2413 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1202 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2159 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19283 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3033 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8872 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1345 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4273 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17044 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18305 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2341 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5232 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1302 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1860 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3680 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8613 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1134 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2044 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2304 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4030 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2053 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3050 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      823 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1568 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      534 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1078 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2049 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7158 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      954 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1736 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1259 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2425 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4993 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      984 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2577 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1393 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3093 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1523 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2748 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3968 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4996 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2905 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5972 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1428 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2926 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12128 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17309 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1908 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1075 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1975 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1107 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2686 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1691 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3919 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2168 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3951 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1620 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4108 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1061 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2603 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1513 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2837 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2488 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6656 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7750 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22085 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8201 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    23130 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9480 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    28299 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6357 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8308 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2204 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3739 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2408 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4611 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      759 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1483 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      606 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1520 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4463 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      539 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1040 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1243 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3432 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4534 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3085 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8744 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2795 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6887 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3700 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6709 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2707 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4863 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5647 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9609 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2360 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4307 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1962 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4038 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1698 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4006 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1254 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2090 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2230 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7205 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1552 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4667 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10058 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1066 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2112 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1546 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4508 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      837 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1798 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4544 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5371 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3808 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8379 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1024 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2037 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      713 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1564 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4835 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3822 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8980 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2743 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6512 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7790 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17100 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3558 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3729 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8105 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4282 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8817 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1567 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4106 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7321 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16385 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1617 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3717 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      907 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1991 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3431 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13007 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1795 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4250 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1325 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2139 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      960 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2458 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3037 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11612 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2224 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4321 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1964 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2913 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    33625 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    34751 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3514 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4573 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1340 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2627 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1782 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3922 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3990 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7867 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3272 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7429 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1012 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3428 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7557 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25986 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      900 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2806 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4843 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8564 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2700 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7260 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1761 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2946 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3785 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14076 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1218 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2896 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1853 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4129 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4518 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14101 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2620 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10005 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1164 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2589 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2319 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9303 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1565 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3551 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1654 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4076 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2065 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3463 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2652 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3930 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1486 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3810 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2127 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4495 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2236 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4464 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3921 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5335 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1496 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3628 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2357 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3453 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1587 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2520 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14461 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14997 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2183 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3191 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1883 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1462 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2361 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2484 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5515 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1408 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3490 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2249 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1602 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4465 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2158 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5043 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1922 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1376 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2063 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4182 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10979 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2213 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5936 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1343 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2565 2023-04-17 10:09:57.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6304 2023-04-17 10:09:58.000000 inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2927 2022-12-18 07:02:56.000000 inductor-0.2.8/inductor/util.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      276 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    61729 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       46 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      454 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-17 10:13:55.000000 inductor-0.2.8/inductor.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      341 2023-03-08 16:33:31.000000 inductor-0.2.8/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      902 2023-04-17 10:13:58.000000 inductor-0.2.8/setup.cfg
```

### Comparing `inductor-0.2.7/LICENSE` & `inductor-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/__init__.py` & `inductor-0.2.8/inductor/__init__.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/cli.py` & `inductor-0.2.8/inductor/cli.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/compute/common.py` & `inductor-0.2.8/inductor/compute/common.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/compute/local.py` & `inductor-0.2.8/inductor/compute/local.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/conftest.py` & `inductor-0.2.8/inductor/conftest.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/data/table/dynamodb.py` & `inductor-0.2.8/inductor/data/table/dynamodb.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/data/table/mysql.py` & `inductor-0.2.8/inductor/data/table/mysql.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/data/table/postgresql.py` & `inductor-0.2.8/inductor/data/table/postgresql.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/data/table/snowflake.py` & `inductor-0.2.8/inductor/data/table/snowflake.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/data/table/sqlite.py` & `inductor-0.2.8/inductor/data/table/sqlite.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/data/table/table.py` & `inductor-0.2.8/inductor/data/table/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     def values(self) -> List[Any]:
         """Returns a list containing the single value stored in each row.
 
         Requires that this table contains exactly one column.
 
         Raises:
-            RuntimeError if this table does not contain exactly one column.
+            RuntimeError: if this table does not contain exactly one column.
         """
         values = []
         column_name = None
         for row in self:
             if len(row) != 1:
                 raise RuntimeError(
                     "This table does not contain exactly one column.")
@@ -172,16 +172,16 @@
 
     def value(self) -> Any:
         """Returns the single value stored in this table.
 
         Requires that this table contains exactly one value.
 
         Raises:
-            RuntimeError if table does not contain exactly one row and one
-            column.
+            RuntimeError: if table does not contain exactly one row and one
+                column.
         """
         v = None
         valid_data = False
         for row in self:
             if not valid_data:
                 if len(row) == 1:
                     v = list(row.values())[0]
@@ -280,15 +280,15 @@
     def __getitem__(self, key: Any) -> Row:
         """Returns row having given primary key.
 
         Args:
             key: Primary key value.
 
         Raises:
-            KeyError if no row exists having given primary key.
+            KeyError: if no row exists having given primary key.
         """
         row = self.get(key)
         if row is not None:
             return row
         else:
             raise KeyError("No row exists for given key.")
```

### Comparing `inductor-0.2.7/inductor/data/table/table_catalog.py` & `inductor-0.2.8/inductor/data/table/table_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,17 +213,17 @@
 
         Args:
             name: Name for this table.
             faster_query_columns: Names of columns for which SQL SELECT queries
                 should be accelerated (generally via creation of indexes).
 
         Raises:
-            RuntimeError if a table having given name already exists but does
-            not have the characteristics specified by this method call's
-            arguments.
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
         """
         table_spec = locals().copy()
         del table_spec["self"]
         if not self._run_time:
             self._table_creation_instructions.append(
                 (self.create_table.__name__, table_spec))
         elif isinstance(self._env, (environment.Local, environment.Server)):
@@ -281,17 +281,17 @@
             range_queries_only: If sql_queryable is True, should the table
                 only natively support range queries?  Ignored if sql_queryable
                 is False.
             faster_query_columns: Names of columns for which SQL SELECT queries
                 should be accelerated (generally via creation of indexes).
 
         Raises:
-            RuntimeError if a table having given name already exists but does
-            not have the characteristics specified by this method call's
-            arguments.
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
         """
         table_spec = locals().copy()
         del table_spec["self"]
         if not self._run_time:
             self._table_creation_instructions.append(
                 (self.create_keyed_table.__name__, table_spec))
         elif isinstance(self._env, (environment.Local, environment.Server)):
@@ -343,26 +343,27 @@
             sqlite_file_path: Path to file giving sqlite database containing
                 the existing table to be added.
             sqlite_table_name: Name of existing table in file given by
                 sqlite_file_path. If not provided, the value of the name
                 argument is used.
             primary_key_column: If non-None, then the table will be treated as
                 being keyed by the column having name given by this parameter.
-                If None:
+                If None, then
+
                 - If the existing table has exactly one primary key column, then
                   the table will be treated as being keyed on that column.
                 - Otherwise, if the existing table has no primary key column
                   and exactly one unique index column, then the table will be
                   treated as being keyed on that column.
                 - Otherwise, the table will not be treated as being keyed.
 
         Raises:
-            RuntimeError if a table having given name already exists but does
-            not have the characteristics specified by this method call's
-            arguments.
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
         """
         if sqlite_table_name is None:
             sqlite_table_name = name
         table_spec = locals().copy()
         del table_spec["self"]
         if not self._run_time:
             self._table_creation_instructions.append(
@@ -434,30 +435,31 @@
             mysql_user: MySQL database server username.
             mysql_database: Name of MySQL database containing existing table.
             mysql_table_name: Name of existing table in database given by
                 preceding arguments. If not provided, the value of the name
                 argument is used.
             primary_key_column: If non-None, then the table will be treated as
                 being keyed by the column having name given by this parameter.
-                If None:
+                If None, then
+                
                 - If the existing table has exactly one primary key column, then
                   the table will be treated as being keyed on that column.
                 - Otherwise, if the existing table has no primary key column
                   and exactly one unique index column, then the table will be
                   treated as being keyed on that column.
                 - Otherwise, the table will not be treated as being keyed.
             mysql_port: Optionally, the port on which to connect to the database
                 server.
             mysql_password: Optionally, password for user.  If not provided,
                 password must be provided by secrets file.
 
         Raises:
-            RuntimeError if a table having given name already exists but does
-            not have the characteristics specified by this method call's
-            arguments.
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
         """
         if mysql_table_name is None:
             mysql_table_name = name
 
         table_spec = locals().copy()
         del table_spec["self"]
         if not self._run_time:
@@ -551,17 +553,17 @@
             dynamodb_endpoint_url: Optional Endpoint URL to be used to
                 communicate with the DynamoDB service. Intended to be used
                 to connect with a local DynamoDB instance for development
                 and testing purposes. In general, should not be provided
                 if utilizing an actual AWS account.
 
         Raises:
-            RuntimeError if a table having given name already exists but does
-            not have the characteristics specified by this method call's
-            arguments.
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
         """
         if dynamodb_table_name is None:
             dynamodb_table_name = name
         table_spec = locals().copy()
         del table_spec["self"]
         if not self._run_time:
             self._table_creation_instructions.append(
@@ -625,30 +627,31 @@
             postgresql_database: Name of PostgreSQL database containing
                 existing table.
             postgresql_table_name: Name of existing table in database given by
                 preceding arguments. If not provided, the value of the name
                 argument is used.
             primary_key_column: If non-None, then the table will be treated as
                 being keyed by the column having name given by this parameter.
-                If None:
+                If None, then
+                
                 - If the existing table has exactly one primary key column,
                   then the table will be treated as being keyed on that column.
                 - Otherwise, if the existing table has no primary key column
                   and exactly one unique index column, then the table will be
                   treated as being keyed on that column.
                 - Otherwise, the table will not be treated as being keyed.
             postgresql_port: Optionally, the port on which to connect to the
                 database server.
             postgresql_password: Optionally, password for user.  If not
                 provided, password must be provided by secrets file.
 
         Raises:
-            RuntimeError if a table having given name already exists but does
-            not have the characteristics specified by this method call's
-            arguments.
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
         """
         if postgresql_table_name is None:
             postgresql_table_name = name
 
         table_spec = locals().copy()
         del table_spec["self"]
         if not self._run_time:
@@ -762,17 +765,17 @@
             snowflake_table_name: Name of existing table in database given by
                 preceding arguments. If not provided, the value of the name
                 argument is used.
             snowflake_password: Optionally, password for user.  If not
                 provided, password must be provided by secrets file.
 
         Raises:
-            RuntimeError if a table having given name already exists but does
-            not have the characteristics specified by this method call's
-            arguments.
+            RuntimeError: if a table having given name already exists but does
+                not have the characteristics specified by this method call's
+                arguments.
         """
         from inductor.data.table import snowflake  # pylint: disable=import-outside-toplevel
 
         if snowflake_table_name is None:
             snowflake_table_name = name
 
         table_spec = locals().copy()
```

### Comparing `inductor-0.2.7/inductor/data/table/table_util.py` & `inductor-0.2.8/inductor/data/table/table_util.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/environment.py` & `inductor-0.2.8/inductor/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,27 +47,26 @@
                 with the same database_url.
             database_url: URL identifying database to be used for storage of
                 app metadata and Inductor-created tables.  This database should
                 be persistent independently of (and accessible from) the compute
                 node or container used to run the app.  The URL should have
                 format
                     system://username:password@host:port/database
-                where system is either mysql or postgresql.  The database role
+                where ``system`` is either mysql or postgresql.  The database role
                 identified by username should have the ability to create and
                 write to (as well as read) tables in the specified database.
             object_store_url: URL identifying object storage location to be
                 used for storage of app metadata and data.  This storage
                 location should be persisent independently of (and accessible
                 from) the server (e.g., compute node or container) used to run
-                the app.  The URL should have the following format:
+                the app.  The URL should have the following format\:
+                
                 - If using a filesystem mounted into node/container (e.g., via
-                  Amazon Elastic File System):
-                    file://path/to/use/
-                - If using AWS S3:
-                    s3://bucket/prefix/
+                  Amazon Elastic File System): ``file://path/to/use/``
+                - If using AWS S3: ``s3://bucket/prefix/``, 
                   where prefix is optional.
             http_host: Host to which Inductor's web server should bind.
             http_port: Port to which Inductor's web server should bind.
         """
         self.app_name = app_name
         self.database_url = database_url
         self.object_store_url = object_store_url
```

### Comparing `inductor-0.2.7/inductor/ml/model_store.py` & `inductor-0.2.8/inductor/ml/model_store.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/__init__.py` & `inductor-0.2.8/inductor/ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -747,25 +747,28 @@
             "config": self._plotly_config(),
             "style": self._plotly_style()
         }))
 
     def plotly_figure(
         self, fig: plotly.graph_objects.Figure, *,
         config: Optional[Dict] = None):
+        # pylint: disable=line-too-long
         """Appends the given Plotly figure.
 
-        Arbitrary Plotly figures can, for example, be created using Plotly
-        Express or Plotly's graph objects API.
+        Arbitrary Plotly figures can, for example, be created using
+        `Plotly Express <https://plotly.com/python/plotly-express/>`_
+        or Plotly's graph objects API.
 
         Args:
             fig: The Plotly figure to be appended.
-            config: Optional [additional configuration options](https://plotly.com/python/configuration-options/) # pylint: disable=line-too-long
+            config: Optional `additional configuration options <https://plotly.com/python/configuration-options/>`_
                 for figure behavior, as would be passed to the config parameter
                 of plotly.graph_objects.Figure.show().
         """
+        # pylint: enable=line-too-long
         if not isinstance(fig, plotly.graph_objects.Figure):
             raise TypeError(f"Unsupported fig type: {type(fig)}")
 
         fig_copy = plotly.graph_objects.Figure(fig)
         margin = self._plotly_layout(fig.layout.title.text,
                                      fig.layout.xaxis.title.text,
                                      fig.layout.yaxis.title.text).get("margin")
@@ -792,32 +795,34 @@
 
     def image(
         self,
         img: Union[str, Image.Image, np.ndarray, bytes],
         *,
         max_width: Optional[Union[int, float]] = None,
         max_height: Optional[int] = None):
+        # pylint: disable=line-too-long
         """Appends an image.
 
         Args:
             img: The image to be displayed.  If `str`, must be a URL for an
                 image. If `np.ndarray`, then should be convertible to
-                PIL.Image.Image via its [fromarray()](https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.fromarray) # pylint: disable=line-too-long
+                PIL.Image.Image via its `fromarray() <https://pillow.readthedocs.io/en/stable/reference/Image.html#PIL.Image.fromarray>`_
                 method. If `bytes`, then should be the contents of an image
                 file (e.g., as would be produced by PIL.Image.Image.save()).
             max_width: Optional maximum width for image; the image will be
                 resized as necessary to respect this argument.  Must be
                 positive if provided. If > 1, then interpreted as the maximum
                 display width for the image in pixels. If <= 1, then
                 interpreted as the maximum display width for the image as a
                 fraction of its container's width.
             max_height: Optional maximum height for image, in pixels; the
                 image will be resized as necessary to respect this argument.
                 Must be positive if provided.
         """
+        # pylint: enable=line-too-long
 
         if (max_width is not None and max_width <= 0):
             raise ValueError("max_width must be positive.")
         if (max_height is not None and max_height <= 0):
             raise ValueError("max_height must be positive.")
 
         props = {}
@@ -910,26 +915,28 @@
         self._append(_Element("Notify", props, [content]))
 
     def code(
         self,
         content: str,
         *,
         lang: Optional[str] = None):
+        # pylint: disable=line-too-long
         """Displays given content as code.
 
         Args:
             content: The code to be displayed.  Whitespace is trimmed via
                 inspect.cleandoc(): "All leading whitespace is removed from the
                 first line. Any leading whitespace that can be uniformly removed
                 from the second line onwards is removed. Empty lines at the
                 beginning and end are subsequently removed. Also, all tabs are
                 expanded to spaces."
             lang: Optionally, the name of the programming language to be used
-                for syntax highlighting; see [list of available languages](https://github.com/react-syntax-highlighter/react-syntax-highlighter/blob/master/AVAILABLE_LANGUAGES_PRISM.MD). # pylint: disable=line-too-long
+                for syntax highlighting; see `list of available languages <https://github.com/react-syntax-highlighter/react-syntax-highlighter/blob/master/AVAILABLE_LANGUAGES_PRISM.MD>`_.
         """
+        # pylint: enable=line-too-long
         props = {}
         if lang is not None:
             props["language"] = lang
         self._append(_Element("Code", props, [inspect.cleandoc(content)]))
 
     def download(
         self,
@@ -985,20 +992,19 @@
                 (if selectable is True).  If True, then this method does not
                 itself append the data table to the page; rather, it returns an
                 object whose `display()` method can subsequently be called to
                 append the data table to the page, and whose `value` field
                 provides the currently selected row (if selectable is True).
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 If selectable is True and a row has been selected, returns
                 the contents of the currently selected row as a Dict mapping
                 column name to column value.  Otherwise, returns None.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this data table to the page, and whose `value` field
                 provides the currently selected row, if selectable is True and
                 a row has been selected (as would be returned if defer_display
                 were False).
         """
         props = {}
@@ -1086,19 +1092,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with this checkbox;
                 otherwise, returns the value set by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         if label is None and id is None:
             raise ValueError(
@@ -1145,19 +1150,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with this toggle;
                 otherwise, returns the value set by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         if label is None and id is None:
             raise ValueError(
@@ -1214,19 +1218,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with this date
                 picker; otherwise, returns the value set by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         if label is None and id is None:
             raise ValueError(
@@ -1315,19 +1318,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with this date
                 range picker; otherwise, returns the value set by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         if label is None and id is None:
             raise ValueError(
@@ -1423,20 +1425,19 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with the select;
                 otherwise, returns the value set by the user (a string if multi
                 is False, otherwise a list of strings).
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         id_prefix = ("multi" if multi else "") + "select:"
         if id is None:
@@ -1523,19 +1524,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with the select;
                 otherwise, returns the value set by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         return self._append_select(
             values=values,
@@ -1574,19 +1574,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with the
                 multiselect; otherwise, returns the value(s) set by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         return self._append_select(
             values=values,
@@ -1632,20 +1631,19 @@
                 If True, then this method does not itself append the radio
                 button group to the page; rather, it returns an object whose
                 `display()` method can subsequently be called to append the
                 radio button group to the page, and whose `value` field provides
                 the radio button group's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with the radio
                 button group; otherwise, returns the value of the currently
                 selected radio button.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this radio button group to the page, and whose `value`
                 field provides the current value of the radio button group (as
                 would be returned if defer_display were False).
         """
         id_prefix = "radio:"
         if id is None:
@@ -1719,19 +1717,18 @@
                 If True, then this method does not itself append the button to
                 the page; rather, it returns an object whose `display()` method
                 can subsequently be called to append the button to the page, and
                 whose `value` field is True if this button was just pressed (and
                 False otherwise).
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 True if the user's last action was pressing this button, and
                 False otherwise.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this button to the page, and whose `value` field is True
                 if and only if the user's last action was pressing this button
                 (as would be returned if defer_display were False).
         """
         id = "button:" + (id if id is not None else label)
         props = {"id": id, "label": label}
@@ -1788,19 +1785,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with this input;
                 otherwise, returns the value inputted by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         if placeholder is None and label is None and id is None:
             raise ValueError(
@@ -1883,19 +1879,18 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 default_value if the user has not interacted with this number
                 input field; otherwise, returns the value inputted by the user.
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         if (not allow_float and default_value is not None
                 and isinstance(default_value, float)):
@@ -1953,21 +1948,20 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
+            If defer_display is False (the default)
                 None if no file has been selected by the user; otherwise,
                 returns a tuple containing (the uploaded contents of the
                 selected file as bytes, the browser-local path of the
                 selected file).
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         id = "file_upload:" + (id if id is not None else initial_message)
         props = {"id": id, "initialMessage": initial_message}
@@ -2022,23 +2016,22 @@
                 element to the page and returns its current value.  If True,
                 then this method does not itself append the element to the page;
                 rather, it returns an object whose `display()` method can
                 subsequently be called to append the element to the page, and
                 whose `value` field provides the element's current value.
 
         Returns:
-            If defer_display is False (the default):
-                If the user has not yet interacted with this slider:
+            If defer_display is False (the default)
+                If the user has not yet interacted with this slider
                     default_value, if provided; otherwise, min_max[0] if range
                     is False, or min_max if range is True.
-                If the user has interacted with this slider:
+                If the user has interacted with this slider
                     The value(s) selected by the user (i.e., a single integer
                     if range is False, and a pair of integers otherwise).
-
-            If defer_display is True:
+            If defer_display is True
                 An object whose `display()` method can subsequently be called to
                 append this element to the page, and whose `value` field
                 provides the current element value (as would be returned if
                 defer_display were False).
         """
         if len(min_max) != 2:
             raise ValueError("min_max must be a tuple of length 2.")
@@ -2118,40 +2111,40 @@
         return ContainerStackContextManager(
             _Element("Horizontal", {"align": align}), self)
 
     def tabs(self) -> ContainerStackContextManager:
         """Returns a context manager for a tab bar.
 
         Only tabs can be directly added to a page within the returned context.
-        For example (where p is a Page object):
+        For example (where p is a Page object)::
 
-        with p.tabs():
-            with p.tab("First Tab's Label"):
-                p.print("Content in first tab")
-            with p.tab("Second Tab's Label"):
-                p.print("Content in second tab")
-        p.print("Content after tabs")
+            with p.tabs():
+                with p.tab("First Tab's Label"):
+                    p.print("Content in first tab")
+                with p.tab("Second Tab's Label"):
+                    p.print("Content in second tab")
+            p.print("Content after tabs")
         """
         return ContainerStackContextManager(_Element("Tabs", {}), self)
 
     def tab(self, label: str, *,
         hot_keys: Optional[str] = None) -> ContainerStackContextManager:
         """Returns a context manager for a tab within a tab bar.
 
         Elements added to a page within the returned context are appended within
         a tab having the given label.  In conjunction with the tabs() method,
         this method can be used to create tabbed layouts as follows (where p is
-        a Page object):
+        a Page object)::
 
-        with p.tabs():
-            with p.tab("First Tab's Label"):
-                p.print("Content in first tab")
-            with p.tab("Second Tab's Label"):
-                p.print("Content in second tab")
-        p.print("Content after tabs")
+            with p.tabs():
+                with p.tab("First Tab's Label"):
+                    p.print("Content in first tab")
+                with p.tab("Second Tab's Label"):
+                    p.print("Content in second tab")
+            p.print("Content after tabs")
 
         Args:
             label: The label for this tab (which will be displayed in the tab
                 bar).
             hot_keys: Optional keyboard shortcut that can be used to display
                 this tab (e.g., "1", "command+g").
         """
@@ -2161,46 +2154,46 @@
 
         return ContainerStackContextManager(_Element("Tab", props), self)
 
     def columns(self) -> ContainerStackContextManager:
         """Returns a context manager for a columnar layout.
 
         Only columns can be directly added to a page within the returned
-        context.  For example (where p is a Page object):
+        context.  For example (where p is a Page object)::
 
-        with p.columns():
-            with p.column():
-                p.heading("Column 1")
-            with p.column():
-                p.heading("Column 2")
-                p.print("Content in second column")
-        p.print("Content after columns")
+            with p.columns():
+                with p.column():
+                    p.heading("Column 1")
+                with p.column():
+                    p.heading("Column 2")
+                    p.print("Content in second column")
+            p.print("Content after columns")
         """
         return ContainerStackContextManager(_Element("Columns", {}), self)
 
     def column(
         self,
         width: Optional[float] = None,
         align: Literal["left", "center", "right"] = "left"
     ) -> ContainerStackContextManager:
         """Returns a context manager for a column within a columnar layout.
 
         Elements added to a page within the returned context are appended
         vertically, with widths constrained to be at most the width of this
         column.  In conjunction with the columns() method, this method can be
         used to create multi-column layouts as follows (where p is a Page
-        object):
+        object)::
 
-        with p.columns():
-            with p.column():
-                p.heading("Column 1")
-            with p.column():
-                p.heading("Column 2")
-                p.print("Content in second column")
-        p.print("Content after columns")
+            with p.columns():
+                with p.column():
+                    p.heading("Column 1")
+                with p.column():
+                    p.heading("Column 2")
+                    p.print("Content in second column")
+            p.print("Content after columns")
 
         Args:
             width: Optionally, the width of this column, as a fraction of its
                 container's width.  If not provided, then this column will
                 occupy all width not occupied by other columns having explicitly
                 specified widths in the same columnar layout.  If multiple
                 columns in the same columnar layout do not have widths
@@ -2227,22 +2220,21 @@
         hot_keys: Optional[str] = None) -> ModalContextManager:
         """Returns a context manager for a modal.
 
         If the modal is not already open and trigger_open is True, then the
         modal is displayed.  Elements added to a page within the returned
         context are appended within the body of the modal.  The returned
         context manager also provides a close() method that can be used to
-        close the modal if it is currently displayed.  For example:
-        ```
-        with p.modal(p.button("Start training"), "Train a new model") as m:
-            name = p.input("Name for training run")
-            if p.button("Start"):
-                ...
-                m.close()
-        ```
+        close the modal if it is currently displayed.  For example::
+
+            with p.modal(p.button("Start training"), "Train a new model") as m:
+                name = p.input("Name for training run")
+                if p.button("Start"):
+                    ...
+                    m.close()
 
         Args:
             trigger_open: If the modal is not already open and trigger_open is
                 True, then the modal is displayed.  Otherwise (i.e., if the
                 modal is already open or trigger_open is False), this argument
                 has no effect.
             title: Optionally, the title to be displayed at the top of this
@@ -2365,16 +2357,15 @@
         If redirect() is called on a Page, then that Page's contents (if any)
         are ignored.  Can only be called once on a given Page instance.
 
         Args:
             url: URL to which to redirect the user's browser.
 
         Raises:
-            RuntimeError if redirect() has been called previously on this
-            Page.
+            RuntimeError: if redirect() has been called previously on this Page.
         """
         if self._redirect_url:
             raise RuntimeError(
                 "Attempted to call redirect() more than once on this Page.")
         self._redirect_url = url
 
     def navbar(
```

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/asset-manifest.json` & `inductor-0.2.8/inductor/ui/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/index.html` & `inductor-0.2.8/inductor/ui/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/logo192.png` & `inductor-0.2.8/inductor/ui/frontend/build/logo192.png`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/logo512.png` & `inductor-0.2.8/inductor/ui/frontend/build/logo512.png`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/787.cda612ba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/main.742afa3c.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/main.742afa3c.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/main.742afa3c.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abap.7a511d2e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_abnf.108d25be.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_actionscript.a53a050b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ada.0383c815.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_agda.78e921d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_al.31231b15.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_antlr4.e1ea142a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apacheconf.417190b7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apex.b5b749c3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_apl.77bf5b55.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_applescript.3919c20a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aql.5f5df97e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arduino.a2f329d1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_arff.c5d78406.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asciidoc.aae7e963.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asm6502.b3059f16.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_asmatmel.0ae58eda.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_aspnet.5a40c106.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autohotkey.fa50b409.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_autoit.46f5be8a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avisynth.093a19ce.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_avroIdl.09d1fcb6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bash.41237550.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_basic.97ee507d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_batch.7570ea45.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bbcode.c4748df5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bicep.7ef7f87c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_birb.4b4d2455.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bison.f9faadb0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bnf.1774a615.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brainfuck.373a8f58.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_brightscript.f9d27e34.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bro.0b5748f8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_bsl.9f434fd4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_c.93bb3f93.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cfscript.ec2850eb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_chaiscript.361867e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cil.f41c92bf.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clike.dd4ec48a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_clojure.6df8ec16.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cmake.fbc6ece0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cobol.2e66c598.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coffeescript.49c28a3a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_concurnas.194876fc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_coq.dd0971ee.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cpp.cffd172b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_crystal.574ecad1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csharp.94256fc3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cshtml.c2a29247.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csp.5a7e0ad2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_css.ee01e983.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cssExtras.d49cc4d7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_csv.3eb58e61.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_cypher.518302f1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_d.d0f05b3a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dart.7b831273.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dataweave.43503a23.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dax.8d17a98f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dhall.47fac09d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_diff.18205aa7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_django.b380c3bb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dnsZoneFile.aa6df23f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_docker.c1c25415.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_dot.11fb239c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ebnf.ad6ebcef.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_editorconfig.a3639952.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_eiffel.aaed1908.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ejs.c3c95368.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elixir.c2bfa848.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_elm.c3f25f30.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erb.5dd6fb38.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_erlang.a2df3d3f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_etlua.991d706a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_excelFormula.25fd44af.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_factor.aa9407b5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_falselang.cfad9d55.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.6b0d30d8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_flow.e1a28ca7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fortran.bac30bf2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_fsharp.9d6ef384.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ftl.87e6b2fd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gap.b0bd9e57.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gcode.d23c9ac3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gdscript.4a319a71.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gedcom.b0ae60c5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gherkin.d041bc66.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_git.8814e653.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_glsl.3af3261b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gml.4d6a2f7a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_gn.eab8f249.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_go.47664592.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_goModule.39cf5eaa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_graphql.24c759b4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_groovy.bde50d09.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haml.ec169a6d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_handlebars.fcf22d5d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haskell.4e1cd825.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_haxe.c617b99a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hcl.47809bc8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hlsl.b48b7ba6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hoon.f5ce3602.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hpkp.74d3b1ac.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_hsts.f4e5dec7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_http.487b6cd6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ichigojam.b4100cce.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icon.c958a9f4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_icuMessageFormat.34928c67.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_idris.e88f4d0c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_iecst.2a4fa8b4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ignore.36fffbaa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_inform7.fba15a77.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ini.99e17be9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_io.bffee041.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_j.7e55a801.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_java.9ce75912.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoc.19bdf5df.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javadoclike.76b47063.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javascript.87a2ca48.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_javastacktrace.4ad565b4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jexl.41b25908.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jolie.d58a6d3c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jq.ae37d0cb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsExtras.e44ab7d5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsTemplates.00dcc5fb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsdoc.8733130f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json.7f2fd656.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_json5.d75503f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsonp.f51579b2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsstacktrace.216e4db2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_jsx.75b842c1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_julia.cd84d33f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keepalived.727389c5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_keyman.3a493522.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kotlin.be4126b9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kumir.5f598c9c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_kusto.c02f03a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latex.462180d0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_latte.167edc98.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_less.b86f029c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lilypond.9646cee3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_liquid.278e7237.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lisp.e2a3fb75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_livescript.f3b5162d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_llvm.3d4c2701.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_log.06d95438.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lolcode.5072f711.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_lua.e637b841.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_magma.95ed9eca.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_makefile.7d65970f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markdown.107515ba.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markup.fdcdafb9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_markupTemplating.7d1805d3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_matlab.c872e62a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_maxscript.b528a49c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mel.fccdc7a2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mermaid.08793df8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mizar.267ee18a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_mongodb.6b430b5a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_monkey.45e2319c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_moonscript.8a9dbae2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n1ql.3dabf22b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_n4js.872bf57b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.a6dd0963.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_naniscript.65d0072e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nasm.9a27bea2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_neon.2ef4a41e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nevod.3a91e79e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nginx.ebcce88a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nim.56c75829.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nix.2888d23a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_nsis.a0da6b57.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_objectivec.d50633af.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ocaml.71ee5691.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_opencl.e45e70c4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_openqasm.285431bb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_oz.e7d7a884.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parigp.88b52198.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_parser.2e9fef31.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascal.184166b3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pascaligo.12e12063.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pcaxis.3c9d732d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_peoplecode.c39954f5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_perl.8220691f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_php.24fb5d96.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpExtras.9eb9a4ae.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_phpdoc.c5baec63.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_plsql.43544705.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powerquery.be03f945.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_powershell.2d956874.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_processing.dd66c2d0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_prolog.4cd4816b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_promql.68d76da2.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_properties.7d3c7fbe.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_protobuf.d6828b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_psl.2174621a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pug.22de817d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_puppet.67e8f3c4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_pure.0df154c6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purebasic.6f75a617.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_purescript.d3303a53.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_python.96043008.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_q.bdb3a524.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qml.dd3ccbe5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qore.ae46b63b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_qsharp.853f8ed7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_r.57423a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_racket.b89627d9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_reason.31b98ada.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_regex.6ac43a21.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rego.9a45d9fc.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_renpy.87c0a472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rest.b3744550.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rip.2b87342f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_roboconf.40dbf6f0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_robotframework.59010a31.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_ruby.6f692bdb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_rust.e51068d9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sas.c6b2c785.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sass.4cc09b8e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scala.08ab3704.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scheme.98d749c9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_scss.5da29955.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_shellSession.f359ec9d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smali.b747365e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smalltalk.bd4f0d49.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_smarty.0e2dccd8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sml.e758fe8d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solidity.1ea93159.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_solutionFile.ac9fb0be.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_soy.3fcd83d9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sparql.30cc7dce.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_splunkSpl.923a8ae1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sqf.5110d4e7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_sql.3767b035.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_squirrel.1072cc1f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stan.7a286129.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_stylus.a0246273.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_swift.529d54b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_systemd.5c8d4791.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Cs.a94b05a3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Templating.887bf1d0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_t4Vb.03cc01c7.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tap.61fe204e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tcl.608833a0.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_textile.2a9aad9d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_toml.b5681a2f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tremor.062f127b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tsx.7ad444fb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_tt2.af3c93e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_turtle.c8d9a059.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_twig.cc68d46c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typescript.8557b83e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_typoscript.97e47c29.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_unrealscript.e22a5c85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uorazor.fa15d1da.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_uri.006f9de8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_v.3010f896.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vala.3750323a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vbnet.464366a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_velocity.f2ad84f8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_verilog.a2f4765d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vhdl.9cb0cf03.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_vim.dc5fce5c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_visualBasic.d2e73e07.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_warpscript.09d8bed3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wasm.f7202a75.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_webIdl.d65252d3.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wiki.a6b95d65.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wolfram.a0eba5b8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_wren.a548417e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xeora.666d06ef.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xmlDoc.8ecc1358.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xojo.62407cc5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_xquery.01b466e6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yaml.8498f5a4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_yang.b4a63a3b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map` & `inductor-0.2.8/inductor/ui/frontend/build/static/js/react-syntax-highlighter_languages_refractor_zig.eea01d8e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor/util.py` & `inductor-0.2.8/inductor/util.py`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/inductor.egg-info/SOURCES.txt` & `inductor-0.2.8/inductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inductor-0.2.7/setup.cfg` & `inductor-0.2.8/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inductor
-version = 0.2.7
+version = 0.2.8
 url = https://inductor.ai
 license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
@@ -24,14 +24,20 @@
 	plotly>=5.11,<6
 	numpy>=1.21.6,<2
 	boto3>=1.24.76,<2
 	psycopg2>=2.9.5,<3
 python_requires = >=3.7
 
 [options.extras_require]
+mysql = 
+	PyMySQL>=1.0.2,<2
+postgres = 
+	psycopg2>=2.9.5,<3
+postgresql = 
+	psycopg2>=2.9.5,<3
 snowflake = 
 	snowflake-connector-python>=3.0.0,<4
 	pyarrow>=10.0.1,<10.1.0
 
 [options.packages.find]
 include = inductor**
```

