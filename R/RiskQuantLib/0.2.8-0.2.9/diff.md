# Comparing `tmp/RiskQuantLib-0.2.8.tar.gz` & `tmp/RiskQuantLib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskQuantLib-0.2.8.tar", last modified: Sat Apr 15 13:32:11 2023, max compression
+gzip compressed data, was "RiskQuantLib-0.2.9.tar", last modified: Mon Apr 17 01:45:14 2023, max compression
```

## Comparing `RiskQuantLib-0.2.8.tar` & `RiskQuantLib-0.2.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:11.068575 RiskQuantLib-0.2.8/
--rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 RiskQuantLib-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 RiskQuantLib-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1120 2023-04-15 13:32:11.068575 RiskQuantLib-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 RiskQuantLib-0.2.8/README.md
--rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 RiskQuantLib-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 13:32:11.072619 RiskQuantLib-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1932 2023-04-15 11:55:34.000000 RiskQuantLib-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.341502 RiskQuantLib-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.426065 RiskQuantLib-0.2.8/src/RiskQuantLib/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.494060 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.499005 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/Instrument/
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/Instrument/__init__.py
--rw-rw-rw-   0        0        0      388 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.501999 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/InstrumentList/
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0      409 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Auto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.590515 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.601278 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.613513 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
--rw-rw-rw-   0        0        0     2677 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
--rw-rw-rw-   0        0        0      351 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
--rw-rw-rw-   0        0        0      355 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
--rw-rw-rw-   0        0        0      402 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
--rw-rw-rw-   0        0        0      369 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/sourceCodeDebugger.pyt
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.622684 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
--rw-rw-rw-   0        0        0     1474 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
--rw-rw-rw-   0        0        0     2151 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
--rw-rw-rw-   0        0        0     1515 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
--rw-rw-rw-   0        0        0     1101 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.631802 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/__pycache__/
--rw-rw-rw-   0        0        0      180 2022-12-14 06:06:02.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    14083 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/macro.pyt
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/__init__.py
--rw-rw-rw-   0        0        0    44560 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/builder.py
--rw-rw-rw-   0        0        0     9222 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/debugger.py
--rw-rw-rw-   0        0        0     1640 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/render.py
--rw-rw-rw-   0        0        0     8835 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/router.py
--rw-rw-rw-   0        0        0     4736 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Build/tree.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.652874 RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/__init__.py
--rw-rw-rw-   0        0        0      935 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.665731 RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/
--rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/instrumentList.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.679567 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.686339 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/__init__.py
--rw-rw-rw-   0        0        0     1207 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/copula.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.687747 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/__init__.py
--rw-rw-rw-   0        0        0     2181 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/kmv.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/__init__.py
--rw-rw-rw-   0        0        0      274 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Model/model.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.747683 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/iloc.py
--rw-rw-rw-   0        0        0     1107 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/loc.py
--rw-rw-rw-   0        0        0    60946 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/operation.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.753870 RiskQuantLib-0.2.8/src/RiskQuantLib/Property/
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Property/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Property/property.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:11.067055 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/
--rw-rw-rw-   0        0        0     4368 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/GUITool.py
--rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/__init__.py
--rw-rw-rw-   0        0        0     6514 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/codeBuilderTool.py
--rw-rw-rw-   0        0        0    10785 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/databaseTool.py
--rw-rw-rw-   0        0        0     1593 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/excelTool.py
--rw-rw-rw-   0        0        0    19343 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/fileTool.py
--rw-rw-rw-   0        0        0     4862 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/githubTool.py
--rw-rw-rw-   0        0        0     2817 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/mathTool.py
--rw-rw-rw-   0        0        0     1158 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/multiThreadTool.py
--rw-rw-rw-   0        0        0     4705 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/outlookTool.py
--rw-rw-rw-   0        0        0     4487 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/plotTool.py
--rw-rw-rw-   0        0        0     9707 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/pptTool.py
--rw-rw-rw-   0        0        0     9605 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/strTool.py
--rw-rw-rw-   0        0        0     6111 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/wordTool.py
--rw-rw-rw-   0        0        0    36938 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/__init__.py
--rw-rw-rw-   0        0        0      663 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.8/src/RiskQuantLib/module.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:10.492935 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2881 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      619 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-15 13:32:10.000000 RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:14.451061 RiskQuantLib-0.2.9/
+-rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 RiskQuantLib-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 RiskQuantLib-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1120 2023-04-17 01:45:14.454789 RiskQuantLib-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 RiskQuantLib-0.2.9/README.md
+-rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 RiskQuantLib-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 01:45:14.466165 RiskQuantLib-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1932 2023-04-17 01:42:50.000000 RiskQuantLib-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.462536 RiskQuantLib-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.534802 RiskQuantLib-0.2.9/src/RiskQuantLib/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.606372 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.630058 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/Instrument/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      388 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.647030 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Auto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.724671 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.740676 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.833325 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
+-rw-rw-rw-   0        0        0      351 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
+-rw-rw-rw-   0        0        0      355 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
+-rw-rw-rw-   0        0        0      402 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
+-rw-rw-rw-   0        0        0      369 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/sourceCodeDebugger.pyt
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.912093 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
+-rw-rw-rw-   0        0        0     1474 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
+-rw-rw-rw-   0        0        0     2151 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
+-rw-rw-rw-   0        0        0     1515 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
+-rw-rw-rw-   0        0        0     1101 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.920239 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/__pycache__/
+-rw-rw-rw-   0        0        0      180 2022-12-14 06:06:02.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14083 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/macro.pyt
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/__init__.py
+-rw-rw-rw-   0        0        0    44560 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/builder.py
+-rw-rw-rw-   0        0        0     9222 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/debugger.py
+-rw-rw-rw-   0        0        0     1640 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/render.py
+-rw-rw-rw-   0        0        0     8835 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/router.py
+-rw-rw-rw-   0        0        0     4736 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Build/tree.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.936303 RiskQuantLib-0.2.9/src/RiskQuantLib/Instrument/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      935 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.963757 RiskQuantLib-0.2.9/src/RiskQuantLib/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/InstrumentList/instrumentList.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.985692 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.996186 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/Copula/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/Copula/__init__.py
+-rw-rw-rw-   0        0        0     1207 2023-04-15 13:28:24.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/Copula/copula.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:14.019122 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/KMV/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/KMV/__init__.py
+-rw-rw-rw-   0        0        0     2181 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/KMV/kmv.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/__init__.py
+-rw-rw-rw-   0        0        0      274 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Model/model.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:14.074468 RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/iloc.py
+-rw-rw-rw-   0        0        0     1107 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/loc.py
+-rw-rw-rw-   0        0        0    60946 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/operation.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:14.091355 RiskQuantLib-0.2.9/src/RiskQuantLib/Property/
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Property/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Property/property.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:14.451061 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/
+-rw-rw-rw-   0        0        0     4368 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/GUITool.py
+-rw-rw-rw-   0        0        0        0 2022-11-15 07:39:49.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/__init__.py
+-rw-rw-rw-   0        0        0     6514 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/codeBuilderTool.py
+-rw-rw-rw-   0        0        0    10785 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/databaseTool.py
+-rw-rw-rw-   0        0        0     1593 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/excelTool.py
+-rw-rw-rw-   0        0        0    19343 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/fileTool.py
+-rw-rw-rw-   0        0        0     4862 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/githubTool.py
+-rw-rw-rw-   0        0        0     2817 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/mathTool.py
+-rw-rw-rw-   0        0        0     1158 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/multiThreadTool.py
+-rw-rw-rw-   0        0        0     4705 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/outlookTool.py
+-rw-rw-rw-   0        0        0     4487 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/plotTool.py
+-rw-rw-rw-   0        0        0     9707 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/pptTool.py
+-rw-rw-rw-   0        0        0     9605 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/strTool.py
+-rw-rw-rw-   0        0        0     6111 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/wordTool.py
+-rw-rw-rw-   0        0        0    36938 2023-04-15 13:28:25.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/__init__.py
+-rw-rw-rw-   0        0        0      665 2023-04-17 01:40:33.000000 RiskQuantLib-0.2.9/src/RiskQuantLib/module.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:45:13.603320 RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-04-17 01:45:13.000000 RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2881 2023-04-17 01:45:13.000000 RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:45:13.000000 RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      619 2023-04-17 01:45:13.000000 RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-04-17 01:45:13.000000 RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 01:45:13.000000 RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/top_level.txt
```

### Comparing `RiskQuantLib-0.2.8/LICENSE` & `RiskQuantLib-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/PKG-INFO` & `RiskQuantLib-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.2.8
+Version: 0.2.9
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.2.8/README.md` & `RiskQuantLib-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/setup.py` & `RiskQuantLib-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="RiskQuantLib",
-    version="0.2.8",
+    version="0.2.9",
     author="Syuya_Murakami",
     author_email="wxy135@mail.ustc.edu.cn",
     description="RiskQuantLib is a QuantLib derivative to evaluate risk.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://riskquantlib-doc.readthedocs.io/en/latest/index.html",
     project_urls={
```

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/Component/macro.pyt` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/Component/macro.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/builder.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/builder.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/debugger.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/debugger.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/render.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/render.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/router.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/router.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Build/tree.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Build/tree.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Instrument/instrument.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/InstrumentList/instrumentList.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/InstrumentList/instrumentList.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Model/Copula/copula.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Model/Copula/copula.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Model/KMV/kmv.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Model/KMV/kmv.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/iloc.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/iloc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/loc.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/loc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Operation/operation.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Operation/operation.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Property/property.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Property/property.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/GUITool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/GUITool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/codeBuilderTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/codeBuilderTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/databaseTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/databaseTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/excelTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/excelTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/fileTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/fileTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/githubTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/githubTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/mathTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/mathTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/multiThreadTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/multiThreadTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/outlookTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/outlookTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/plotTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/plotTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/pptTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/pptTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/strTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/strTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/Tool/wordTool.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/Tool/wordTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/__init__.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/__init__.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib/module.py` & `RiskQuantLib-0.2.9/src/RiskQuantLib/module.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 from RiskQuantLib.Build.render import *
 from RiskQuantLib.Build.tree import *
 
 # build module, contents below will be automatically built and replaced, self-defined functions shouldn't be written here
 #<module>
 #</module>
 #<moduleAutoImport>
-#</moduleAutoImport>
+#</moduleAutoImport>
```

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/PKG-INFO` & `RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.2.8
+Version: 0.2.9
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/SOURCES.txt` & `RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.2.8/src/RiskQuantLib.egg-info/entry_points.txt` & `RiskQuantLib-0.2.9/src/RiskQuantLib.egg-info/entry_points.txt`

 * *Files identical despite different names*

