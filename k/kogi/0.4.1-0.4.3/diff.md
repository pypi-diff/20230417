# Comparing `tmp/kogi-0.4.1.tar.gz` & `tmp/kogi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kogi-0.4.1.tar", last modified: Wed Apr  5 11:42:42 2023, max compression
+gzip compressed data, was "kogi-0.4.3.tar", last modified: Mon Apr 17 03:42:33 2023, max compression
```

## Comparing `kogi-0.4.1.tar` & `kogi-0.4.3.tar`

### file list

```diff
@@ -1,93 +1,88 @@
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.498681 kogi-0.4.1/
--rw-r--r--   0 kimio      (501) staff       (20)      602 2023-04-05 11:42:42.498300 kogi-0.4.1/PKG-INFO
--rw-r--r--   0 kimio      (501) staff       (20)       27 2022-11-30 04:22:26.000000 kogi-0.4.1/README.md
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.262732 kogi-0.4.1/kogi/
--rw-r--r--   0 kimio      (501) staff       (20)      235 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)       86 2023-04-04 08:44:10.000000 kogi-0.4.1/kogi/ai.py
--rw-r--r--   0 kimio      (501) staff       (20)       40 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/canvas.py
--rw-r--r--   0 kimio      (501) staff       (20)     9622 2023-04-05 11:31:45.000000 kogi-0.4.1/kogi/chat.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.281917 kogi-0.4.1/kogi/data/
--rw-r--r--   0 kimio      (501) staff       (20)      622 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/data/common_loader.py
--rw-r--r--   0 kimio      (501) staff       (20)      301 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/data/diagnosis_ja.py
--rw-r--r--   0 kimio      (501) staff       (20)    31773 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/data/diagnosis_ja.txt
--rw-r--r--   0 kimio      (501) staff       (20)    11255 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/data/error.txt
--rw-r--r--   0 kimio      (501) staff       (20)      670 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/data/error_desc.py
--rw-r--r--   0 kimio      (501) staff       (20)     3054 2023-03-29 11:55:33.000000 kogi-0.4.1/kogi/hook.py
--rw-r--r--   0 kimio      (501) staff       (20)      119 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/jwu2.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.284590 kogi-0.4.1/kogi/liberr/
--rw-r--r--   0 kimio      (501) staff       (20)      210 2022-12-05 03:53:11.000000 kogi-0.4.1/kogi/liberr/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)     5733 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/liberr/_extract_emsg.py
--rw-r--r--   0 kimio      (501) staff       (20)     7332 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/liberr/_traceback2.py
--rw-r--r--   0 kimio      (501) staff       (20)    28678 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/liberr/emsg_rules.tsv
--rw-r--r--   0 kimio      (501) staff       (20)     1490 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/liberr/extract_vars.py
--rw-r--r--   0 kimio      (501) staff       (20)     5170 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/liberr/rulebase.py
--rw-r--r--   0 kimio      (501) staff       (20)     5824 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/pan.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.286250 kogi-0.4.1/kogi/problem/
--rw-r--r--   0 kimio      (501) staff       (20)      847 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/problem/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)     1874 2022-12-05 03:53:11.000000 kogi-0.4.1/kogi/problem/atcoder.py
--rw-r--r--   0 kimio      (501) staff       (20)     2846 2023-03-29 11:46:56.000000 kogi-0.4.1/kogi/problem/drill.py
--rw-r--r--   0 kimio      (501) staff       (20)     2777 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/problem/judge.py
--rw-r--r--   0 kimio      (501) staff       (20)      346 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/problem/testdata.py
--rw-r--r--   0 kimio      (501) staff       (20)      681 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/problem/timeout.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.306496 kogi-0.4.1/kogi/service/
--rw-r--r--   0 kimio      (501) staff       (20)      792 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/service/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)     1535 2023-04-05 11:41:23.000000 kogi-0.4.1/kogi/service/chatgpt.py
--rw-r--r--   0 kimio      (501) staff       (20)     2892 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/service/flaskapi.py
--rw-r--r--   0 kimio      (501) staff       (20)     5901 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/service/flaskserv.py
--rw-r--r--   0 kimio      (501) staff       (20)      464 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/service/globals.py
--rw-r--r--   0 kimio      (501) staff       (20)     5027 2022-12-05 03:53:11.000000 kogi-0.4.1/kogi/service/huggingface.py
--rw-r--r--   0 kimio      (501) staff       (20)     2630 2023-03-29 12:02:47.000000 kogi-0.4.1/kogi/service/s3logging.py
--rw-r--r--   0 kimio      (501) staff       (20)      711 2022-12-05 03:53:11.000000 kogi-0.4.1/kogi/service/slack.py
--rw-r--r--   0 kimio      (501) staff       (20)     2027 2022-12-05 03:53:11.000000 kogi-0.4.1/kogi/service/textra.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.309213 kogi-0.4.1/kogi/task/
--rw-r--r--   0 kimio      (501) staff       (20)        0 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/task/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)       82 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/task/all.py
--rw-r--r--   0 kimio      (501) staff       (20)     2197 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/task/code.py
--rw-r--r--   0 kimio      (501) staff       (20)      264 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/task/common.py
--rw-r--r--   0 kimio      (501) staff       (20)     6997 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/task/diagnosis.py
--rw-r--r--   0 kimio      (501) staff       (20)      933 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/task/multi.py
--rw-r--r--   0 kimio      (501) staff       (20)     1936 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/task/runner.py
--rw-r--r--   0 kimio      (501) staff       (20)     5946 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/transform.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.497856 kogi-0.4.1/kogi/ui/
--rw-r--r--   0 kimio      (501) staff       (20)      373 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/ui/__init__.py
--rw-r--r--   0 kimio      (501) staff       (20)    12317 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/_canvas.py
--rw-r--r--   0 kimio      (501) staff       (20)      110 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/_google.py
--rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-03-29 09:18:21.000000 kogi-0.4.1/kogi/ui/chatgpt-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      931 2022-12-05 03:53:11.000000 kogi-0.4.1/kogi/ui/content.py
--rw-r--r--   0 kimio      (501) staff       (20)     3973 2023-04-04 08:33:13.000000 kogi-0.4.1/kogi/ui/dialog.css
--rw-r--r--   0 kimio      (501) staff       (20)     1697 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/dialog.html
--rw-r--r--   0 kimio      (501) staff       (20)      907 2023-04-04 08:21:08.000000 kogi-0.4.1/kogi/ui/dialog.js
--rw-r--r--   0 kimio      (501) staff       (20)     2062 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/ui/dialog_colab.py
--rw-r--r--   0 kimio      (501) staff       (20)     1371 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/dialog_ipywidgets.py
--rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-03-29 09:19:44.000000 kogi-0.4.1/kogi/ui/error-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)     7378 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/ui/girl-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    30227 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/girl_think-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)     5877 2023-04-04 10:09:33.000000 kogi-0.4.1/kogi/ui/keylogin.py
--rw-r--r--   0 kimio      (501) staff       (20)     6629 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/kogi-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-03-29 09:17:43.000000 kogi-0.4.1/kogi/ui/kogi_doya-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    64452 2023-03-29 09:09:25.000000 kogi-0.4.1/kogi/ui/kogi_doya.png
--rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-03-29 09:17:48.000000 kogi-0.4.1/kogi/ui/kogi_error-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    67998 2023-03-29 09:09:15.000000 kogi-0.4.1/kogi/ui/kogi_error.png
--rw-r--r--   0 kimio      (501) staff       (20)    48169 2023-03-29 09:17:52.000000 kogi-0.4.1/kogi/ui/kogi_gaan-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    74475 2023-03-29 09:09:27.000000 kogi-0.4.1/kogi/ui/kogi_gaan.png
--rw-r--r--   0 kimio      (501) staff       (20)     8228 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/ui/kogi_vow-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      233 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/main.css
--rw-r--r--   0 kimio      (501) staff       (20)     4812 2023-04-05 11:35:00.000000 kogi-0.4.1/kogi/ui/message.py
--rw-r--r--   0 kimio      (501) staff       (20)     6473 2022-12-05 10:08:08.000000 kogi-0.4.1/kogi/ui/openai-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)    14764 2022-12-05 09:58:58.000000 kogi-0.4.1/kogi/ui/openai.png
--rw-r--r--   0 kimio      (501) staff       (20)    44338 2022-12-05 10:03:15.000000 kogi-0.4.1/kogi/ui/pan.png
--rw-r--r--   0 kimio      (501) staff       (20)     7620 2023-04-04 08:22:10.000000 kogi-0.4.1/kogi/ui/render.py
--rw-r--r--   0 kimio      (501) staff       (20)     4397 2023-03-29 09:02:38.000000 kogi-0.4.1/kogi/ui/rmt.py
--rw-r--r--   0 kimio      (501) staff       (20)     5914 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/ui/robot-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      652 2022-11-30 04:22:26.000000 kogi-0.4.1/kogi/ui/slides.py
--rw-r--r--   0 kimio      (501) staff       (20)     4551 2022-12-22 10:09:16.000000 kogi-0.4.1/kogi/ui/ta-fs8.png
--rw-r--r--   0 kimio      (501) staff       (20)      683 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/ui/typewriter.py
--rw-r--r--   0 kimio      (501) staff       (20)     2073 2023-02-02 09:07:06.000000 kogi-0.4.1/kogi/ui/wait_and_ready.py
-drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-05 11:42:42.264716 kogi-0.4.1/kogi.egg-info/
--rw-r--r--   0 kimio      (501) staff       (20)      602 2023-04-05 11:42:42.000000 kogi-0.4.1/kogi.egg-info/PKG-INFO
--rw-r--r--   0 kimio      (501) staff       (20)     1783 2023-04-05 11:42:42.000000 kogi-0.4.1/kogi.egg-info/SOURCES.txt
--rw-r--r--   0 kimio      (501) staff       (20)        1 2023-04-05 11:42:42.000000 kogi-0.4.1/kogi.egg-info/dependency_links.txt
--rw-r--r--   0 kimio      (501) staff       (20)       42 2023-04-05 11:42:42.000000 kogi-0.4.1/kogi.egg-info/requires.txt
--rw-r--r--   0 kimio      (501) staff       (20)        5 2023-04-05 11:42:42.000000 kogi-0.4.1/kogi.egg-info/top_level.txt
--rw-r--r--   0 kimio      (501) staff       (20)       38 2023-04-05 11:42:42.498766 kogi-0.4.1/setup.cfg
--rw-r--r--   0 kimio      (501) staff       (20)     1168 2023-04-05 11:41:52.000000 kogi-0.4.1/setup.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.676872 kogi-0.4.3/
+-rw-r--r--   0 kimio      (501) staff       (20)      602 2023-04-17 03:42:33.676576 kogi-0.4.3/PKG-INFO
+-rw-r--r--   0 kimio      (501) staff       (20)       27 2023-04-17 03:41:54.000000 kogi-0.4.3/README.md
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.636895 kogi-0.4.3/kogi/
+-rw-r--r--   0 kimio      (501) staff       (20)      235 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)       86 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ai.py
+-rw-r--r--   0 kimio      (501) staff       (20)       40 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/canvas.py
+-rw-r--r--   0 kimio      (501) staff       (20)    10338 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/chat.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.640963 kogi-0.4.3/kogi/data/
+-rw-r--r--   0 kimio      (501) staff       (20)      622 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/common_loader.py
+-rw-r--r--   0 kimio      (501) staff       (20)      301 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/diagnosis_ja.py
+-rw-r--r--   0 kimio      (501) staff       (20)    31773 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/diagnosis_ja.txt
+-rw-r--r--   0 kimio      (501) staff       (20)    11255 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/error.txt
+-rw-r--r--   0 kimio      (501) staff       (20)      670 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/data/error_desc.py
+-rw-r--r--   0 kimio      (501) staff       (20)     3073 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/hook.py
+-rw-r--r--   0 kimio      (501) staff       (20)      119 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/jwu2.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.644195 kogi-0.4.3/kogi/liberr/
+-rw-r--r--   0 kimio      (501) staff       (20)      210 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5733 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/_extract_emsg.py
+-rw-r--r--   0 kimio      (501) staff       (20)     7332 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/_traceback2.py
+-rw-r--r--   0 kimio      (501) staff       (20)    28678 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/emsg_rules.tsv
+-rw-r--r--   0 kimio      (501) staff       (20)     1490 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/extract_vars.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5170 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/liberr/rulebase.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5824 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/pan.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.647331 kogi-0.4.3/kogi/problem/
+-rw-r--r--   0 kimio      (501) staff       (20)      847 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1874 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/atcoder.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2846 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/drill.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2777 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/judge.py
+-rw-r--r--   0 kimio      (501) staff       (20)      346 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/testdata.py
+-rw-r--r--   0 kimio      (501) staff       (20)      681 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/problem/timeout.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.651896 kogi-0.4.3/kogi/service/
+-rw-r--r--   0 kimio      (501) staff       (20)      792 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1535 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/chatgpt.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2892 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/flaskapi.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5901 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/flaskserv.py
+-rw-r--r--   0 kimio      (501) staff       (20)      464 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/globals.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5027 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/huggingface.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2630 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/s3logging.py
+-rw-r--r--   0 kimio      (501) staff       (20)      711 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/slack.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2027 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/service/textra.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.655371 kogi-0.4.3/kogi/task/
+-rw-r--r--   0 kimio      (501) staff       (20)        0 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)       82 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/all.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2197 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/code.py
+-rw-r--r--   0 kimio      (501) staff       (20)      264 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/common.py
+-rw-r--r--   0 kimio      (501) staff       (20)     6997 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/diagnosis.py
+-rw-r--r--   0 kimio      (501) staff       (20)      933 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/multi.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1936 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/task/runner.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5946 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/transform.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.675983 kogi-0.4.3/kogi/ui/
+-rw-r--r--   0 kimio      (501) staff       (20)      373 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/__init__.py
+-rw-r--r--   0 kimio      (501) staff       (20)    12317 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/_canvas.py
+-rw-r--r--   0 kimio      (501) staff       (20)      110 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/_google.py
+-rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/chatgpt-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      931 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/content.py
+-rw-r--r--   0 kimio      (501) staff       (20)     3973 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog.css
+-rw-r--r--   0 kimio      (501) staff       (20)     1697 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog.html
+-rw-r--r--   0 kimio      (501) staff       (20)      907 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog.js
+-rw-r--r--   0 kimio      (501) staff       (20)     2062 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog_colab.py
+-rw-r--r--   0 kimio      (501) staff       (20)     1371 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/dialog_ipywidgets.py
+-rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/error-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     7378 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/girl-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    30227 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/girl_think-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     5937 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/keylogin.py
+-rw-r--r--   0 kimio      (501) staff       (20)     6629 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    40724 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_doya-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    42938 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_error-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)    48169 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_gaan-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     8228 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/kogi_vow-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      233 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/main.css
+-rw-r--r--   0 kimio      (501) staff       (20)     4812 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/message.py
+-rw-r--r--   0 kimio      (501) staff       (20)     6473 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/openai-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)     8080 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/render.py
+-rw-r--r--   0 kimio      (501) staff       (20)     4397 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/rmt.py
+-rw-r--r--   0 kimio      (501) staff       (20)     5914 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/robot-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      652 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/slides.py
+-rw-r--r--   0 kimio      (501) staff       (20)     4551 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/ta-fs8.png
+-rw-r--r--   0 kimio      (501) staff       (20)      683 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/typewriter.py
+-rw-r--r--   0 kimio      (501) staff       (20)     2073 2023-04-17 03:41:54.000000 kogi-0.4.3/kogi/ui/wait_and_ready.py
+drwxr-xr-x   0 kimio      (501) staff       (20)        0 2023-04-17 03:42:33.638498 kogi-0.4.3/kogi.egg-info/
+-rw-r--r--   0 kimio      (501) staff       (20)      602 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/PKG-INFO
+-rw-r--r--   0 kimio      (501) staff       (20)     1681 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/SOURCES.txt
+-rw-r--r--   0 kimio      (501) staff       (20)        1 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/dependency_links.txt
+-rw-r--r--   0 kimio      (501) staff       (20)       51 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/requires.txt
+-rw-r--r--   0 kimio      (501) staff       (20)        5 2023-04-17 03:42:33.000000 kogi-0.4.3/kogi.egg-info/top_level.txt
+-rw-r--r--   0 kimio      (501) staff       (20)       38 2023-04-17 03:42:33.676962 kogi-0.4.3/setup.cfg
+-rw-r--r--   0 kimio      (501) staff       (20)     1168 2023-04-17 03:41:54.000000 kogi-0.4.3/setup.py
```

### Comparing `kogi-0.4.1/PKG-INFO` & `kogi-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kogi
-Version: 0.4.1
+Version: 0.4.3
 Summary: Kogi Programming Assistant AI
 Home-page: https://github.com/kkuramitsu/kogi
 Author: Kimio Kuramitsu
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kogi-0.4.1/kogi/chat.py` & `kogi-0.4.3/kogi/chat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .ui._google import google_colab
 from .ui.render import Doc
 from .liberr import kogi_exc
 from .ui.message import display_dialog, append_message
-import traceback
 import re
 import sys
+import traceback
+import time
 from IPython import get_ipython
 
 from .service import (
     translate, model_prompt, kogi_get,
     record_log, debug_print
 )
 
@@ -16,77 +17,97 @@
 class ChatAI(object):
     slots: dict
     chats: dict
 
     def __init__(self, slots=None):
         self.slots = slots or {}
         self.chats = {}
+        self.face_icon = '@kogi_plus'
+        self.prev_time = time.time()
 
     def get(self, key, value):
         return self.slots.get(key, value)
 
     def update(self, context: dict):
         self.chats = {}
         if context:
             self.slots = dict(context)
         else:
             self.slots = {}
-        self.slots['assistant'] = None
+        self.slots['rec_id'] = None
 
-    def record(self, task, input_text, output_text):
-        rec_id = len(self.records)
-        self.records.append((task, input_text, output_text))
-        return rec_id
+    def difftime(self):
+        t = time.time()
+        diff = int(t - self.prev_time)
+        self.prev_time = t
+        return diff
+
+    # def record(self, task, input_text, output_text):
+    #     rec_id = len(self.records)
+    #     self.records.append((task, input_text, output_text))
+    #     return rec_id
 
+    def likeit(self, rec_id, score):
+        if rec_id in self.chats:
+            context, prompt, response, data = self.chats[rec_id]
+            record_log(type='likeit', rec_id=rec_id, score=score,
+                       context=context, prompt=prompt, response=response, data=data)
+        self.slots['rec_id'] = None
+
+    def face(self, text):
+        return f'{self.face_icon}:{text}'
 
     def prompt(self, prompt):
+        if self.slots['rec_id'] is not None:
+            self.likeit(self.slots['rec_id'], 0)
+            self.face_icon = '@kogi_minus'
+        else:
+            self.face_icon = '@kogi_plus'
         # 将来は分類モデルに置き換える
         if 'どうしたら' in prompt or 'どしたら' in prompt:
-            if 'emsg' not in self.slots:
-                return '@kogi:何をしたいの？'
             return self.error_hint(prompt)
         if '直して' in prompt or 'たすけて' in prompt or '助けて' in prompt:
-            if 'emsg' not in self.slots:
-                return '@kogi:何を？？'
-            return self.fix_code(self.slots['code'])
+            return self.fix_code(prompt)
         if prompt.startswith('+') or prompt.startswith('＋'):
             prompt = prompt[1:]
             if 'again' in self.slots:
                 return self.dialog_again(prompt)
-        return self.dialog(prompt)
+        return self.dialog_request(prompt)
 
     def no_response(self):
-        return '@robot:ChatGPTが反応しないんだけど..'
+        return 'AIが反応しない..'
 
-    def dialog(self, input_text):
+    def dialog_request(self, input_text):
         prompt = input_text
         response, tokens = model_prompt(prompt)
         if response == '':
             return self.no_response()
-        rec_id = record_log(type='prompt_dialog',
-                            prompt=prompt, response=response, tokens=tokens)
-        self.chats[rec_id] = (prompt, response, ('dialog', input_text))
-        self.slots['again'] = ('', prompt, response)
-        return response, rec_id
+        rec_id = record_log(type='prompt', prompt_type='request', difftime=self.difftime(),
+                            context='', prompt=prompt, response=response, tokens=tokens)
+        self.chats[rec_id] = ('', prompt, response,
+                              ('dialog_request', input_text))
+        self.slots['rec_id'] = rec_id
+        return self.face(response), rec_id
 
     def dialog_again(self, input_text):
         if 'again' in self.slots:
             context, prompt, response = self.slots['again']
-        response, tokens = model_prompt(prompt, context=context, post_prompt=input_text)
+        prompt = f'{prompt}\n{input_text}'
+        response, tokens = model_prompt(prompt, context=context)
         if response == '':
             return self.no_response()
-        prompt=f'{context}\n{prompt}\n{input_text}'
-        rec_id = record_log(type='prompt_again',prompt=prompt, response=response, tokens=tokens)
-        self.chats[rec_id] = (prompt, response, ('dialog_again', input_text))
-        #self.slots['again'] = ('', prompt, response)
-        return response, rec_id
-
+        rec_id = record_log(type='prompt', prompt_type='again', difftime=self.difftime(),
+                            context=context, prompt=prompt, response=response, tokens=tokens)
+        self.chats[rec_id] = (context, prompt, response,
+                              ('dialog_again', input_text))
+        self.slots['rec_id'] = rec_id
+        return self.face(response), rec_id
 
     def get_context(self, include_eline=False, include_code=False):
-        ss=[]
+        ss = []
         if 'emsg' in self.slots:
             emsg = self.slots['emsg']
             ss.append(f'エラーの発生: {emsg}')
         if include_eline and 'eline' in self.slots:
             eline = self.slots['eline']
             ss.append(f'エラーの発生した行: {eline}')
         if include_code and 'code' in self.slots:
@@ -101,57 +122,57 @@
             ss.append('```')
         return '\n'.join(ss)
 
     def error_hint(self, prompt):
         emsg = self.slots['emsg']
         eline = self.slots['eline']
         context = self.get_context(include_eline=True)
-        prompt = '原因と解決のヒントを簡単に説明してください。'
+        prompt = '原因と解決のヒントを簡潔に教えてください。'
         response, tokens = model_prompt(prompt, context=context)
         if response == '':
             return self.no_response()
-        rec_id = record_log(type='prompt_error_hint',
-                            prompt=prompt, response=response, tokens=tokens,
-                            emsg=emsg, eline=eline)
-        self.chats[rec_id] = (prompt, response, ('error_hint', emsg, eline))
-        self.slots['again'] = (context, prompt, response)
-        return response, rec_id
+        rec_id = record_log(type='prompt', prompt_type='error', difftime=self.difftime(),
+                            context=context, prompt=prompt, response=response, tokens=tokens)
+        record_log(type='error_hint',
+                   response=response, tokens=tokens, emsg=emsg, eline=eline)
+        self.chats[rec_id] = (context, prompt, response,
+                              ('error_hint', emsg, eline))
+        self.slots['rec_id'] = rec_id
+        return self.face(response), rec_id
 
-    def fix_code(self, code):
+    def fix_code(self, prompt):
         emsg = self.slots['emsg']
         code = self.slots['code']
         if len(code) > 512:
-            return '@kogi:直すべきコードがちょっと長すぎるね', 0
+            return '@kogi:コードがちょっと長すぎるね', 0
         context = self.get_context(include_code=True)
         prompt = f'上記のコードを修正してください。'
         response, tokens = model_prompt(prompt, context=context)
         if response == '':
             return self.no_response()
-        rec_id = record_log(type='prompt_fix_code',
-                            prompt=prompt, response=response, tokens=tokens,
-                            emsg=emsg, code=code)
-        self.chats[rec_id] = (prompt, response, ('fix_code', emsg, code))
-        self.slots['again'] = (context, prompt, response)
-        return response, rec_id
-
-    def likeit(self, rec_id, score):
-        if rec_id in self.chats:
-            prompt, response, data = self.chats[rec_id]
-            record_log(type='likeit', rec_id=rec_id, score=score,
-                       prompt=prompt, response=response, data=data)
+        rec_id = record_log(type='prompt', prompt_type='code', difftime=self.difftime(),
+                            context=context, prompt=prompt, response=response, tokens=tokens)
+        record_log(type='fix_code',
+                   response=response, tokens=tokens, emsg=emsg, code=code)
+        self.chats[rec_id] = (context, prompt, response,
+                              ('fix_code', emsg, code))
+        self.slots['rec_id'] = rec_id
+        return self.face(response), rec_id
 
 
 _DefaultChatbot = ChatAI()
 
 
 def set_chatbot(chatbot):
     global _DefaultChatbot
     _DefaultChatbot = chatbot
 
-LIKEIT=[0, 0]
+
+LIKEIT = [0, 0]
+
 
 def start_dialog(bot, start='', height=None, placeholder='質問はこちらに'):
     height = kogi_get('height', height)
     target = display_dialog(start, height, placeholder)
 
     def display_user(doc):
         nonlocal target
@@ -175,53 +196,56 @@
             try:
                 if isinstance(user_text, str):
                     user_text = user_text.strip()
                 debug_print(user_text)
                 display_user(user_text)
                 doc, rec_id = bot.prompt(user_text)
                 doc = Doc.md(doc)
-                doc.add_likeit(rec_id, like=f'👍{LIKEIT[1]}', dislike=f'👎{LIKEIT[0]}')
+                doc.add_likeit(
+                    rec_id, like=f'👍{LIKEIT[1]}', dislike=f'👎{LIKEIT[0]}')
                 display_bot(doc)
             except:
                 traceback.print_exc()
                 display_bot('@robot:バグで処理に失敗しました。ごめんなさい')
 
         def like(docid, score):
             global LIKEIT
             nonlocal bot
             try:
-                debug_print(docid, score)
-                bot.likeit(docid, score)
-                LIKEIT[score]+=1
+                # debug_print(docid, score)
+                bot.likeit(docid, score if score > 0 else -1)
+                LIKEIT[score] += 1
             except:
                 traceback.print_exc()
                 display_bot('@robot:バグで処理に失敗しました。ごめんなさい')
 
-        # def say(prompt, text):
-        #     nonlocal bot
-        #     try:
-        #         debug_print(text, prompt)
-        #         display_user(text)
-        #         doc = bot.exec(prompt)
-        #         display_bot(doc)
-        #     except:
-        #         traceback.print_exc()
-        #         display_bot('@robot:バグで処理に失敗しました。ごめんなさい')
-
         google_colab.register_callback('notebook.ask', ask)
         google_colab.register_callback('notebook.like', like)
         # if start != '':
         #     ask(start)
     return target
 
 
+def remove_comment(code):
+    ss = []
+    for line in code.splitlines():
+        if '#kogi' in line:
+            line, _, _ = line.rpartition('#kogi')
+        if len(line) > 0:
+            ss.append(line)
+    return '\n'.join(ss)
+
+
 def call_and_start_kogi(actions, code: str = None, context: dict = None):
     for user_text in actions:
         _DefaultChatbot.update(context)
-        doc, rec_id = _DefaultChatbot.dialog(user_text)
+        code = remove_comment(code)
+        if len(code) > 0:
+            user_text = f'コーディング中:\n```\n{code}\n```\n{user_text}\n'
+        doc, rec_id = _DefaultChatbot.prompt(user_text)
         doc = Doc.md(doc)
         doc.add_likeit(rec_id)
         start_dialog(_DefaultChatbot, doc)
         return
 
 
 def error_message(record):
@@ -236,36 +260,34 @@
     if '_stacks' in record:
         for stack in record['_stacks'][::-1]:  # 逆順に
             if '-packages' in stack['filename']:
                 continue
             doc.append(stack['_doc'])
     else:
         doc.append(record['_doc'])
-    # doc.add_button('@error_hint', 'どうしたらいいの？')
-    # doc.add_button('@fix_code', '直してみて')
-    # doc.add_button('@xcall', '先生を呼んで')
+    doc.set_mention('@kogi_minus')
     return doc
 
 
 # _HIRA_PAT = re.compile('[あ-を]')
 
 
-# def is_kogi_call(record):
+# def is_direct_kogi_call(record):
 #     if record.get('etype') == 'NameError':
 #         eparams = record['_eparams']
 #         return re.search(_HIRA_PAT, eparams[0])
 #     return False
 
 
 def catch_and_start_kogi(exc_info=None, code: str = None, context: dict = None, exception=None, enable_dialog=True):
     if exc_info is None:
         exc_info = sys.exc_info()
     record = kogi_exc(code=code, exc_info=exc_info,
                       caught_ex=exception, translate=translate)
-    # if is_kogi_call(record):
+    # if is_direct_kogi_call(record):
     #     msg = record['_eparams'][0][1:-1]
     #     debug_print(msg)
     #     call_and_start_kogi([msg], code)
     #     return
 
     record_log(type='error', **record)
     messages = error_message(record)
```

### Comparing `kogi-0.4.1/kogi/data/common_loader.py` & `kogi-0.4.3/kogi/data/common_loader.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/data/diagnosis_ja.txt` & `kogi-0.4.3/kogi/data/diagnosis_ja.txt`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/data/error.txt` & `kogi-0.4.3/kogi/data/error.txt`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/data/error_desc.py` & `kogi-0.4.3/kogi/data/error_desc.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/hook.py` & `kogi-0.4.3/kogi/hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                     result = _RUNNER[key](
                         ipy, raw_cell, actions[0], catch_and_start_kogi)
                     if not isinstance(result, ExecutionResult):
                         result = RUN_CELL(ipy, 'pass', **kwargs)
                     return result
         if result is None:
             result = RUN_CELL(ipy, raw_cell, kwargs)
-            if 'from google.colab.output import _js' not in raw_cell:
+            if 'from google.colab.output import _js' not in raw_cell and raw_cell != "":
                 record_log(type='run_cell', code=raw_cell)
         return result
 
 
 def change_run_cell(func):
     @wraps(func)
     def run_cell(*args, **kwargs):
```

### Comparing `kogi-0.4.1/kogi/liberr/_extract_emsg.py` & `kogi-0.4.3/kogi/liberr/_extract_emsg.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/liberr/_traceback2.py` & `kogi-0.4.3/kogi/liberr/_traceback2.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/liberr/emsg_rules.tsv` & `kogi-0.4.3/kogi/liberr/emsg_rules.tsv`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/liberr/extract_vars.py` & `kogi-0.4.3/kogi/liberr/extract_vars.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/liberr/rulebase.py` & `kogi-0.4.3/kogi/liberr/rulebase.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/pan.py` & `kogi-0.4.3/kogi/pan.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/problem/__init__.py` & `kogi-0.4.3/kogi/problem/__init__.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/problem/atcoder.py` & `kogi-0.4.3/kogi/problem/atcoder.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/problem/drill.py` & `kogi-0.4.3/kogi/problem/drill.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/problem/judge.py` & `kogi-0.4.3/kogi/problem/judge.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/problem/timeout.py` & `kogi-0.4.3/kogi/problem/timeout.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/__init__.py` & `kogi-0.4.3/kogi/service/__init__.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/chatgpt.py` & `kogi-0.4.3/kogi/service/chatgpt.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/flaskapi.py` & `kogi-0.4.3/kogi/service/flaskapi.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/flaskserv.py` & `kogi-0.4.3/kogi/service/flaskserv.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/huggingface.py` & `kogi-0.4.3/kogi/service/huggingface.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/s3logging.py` & `kogi-0.4.3/kogi/service/s3logging.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/slack.py` & `kogi-0.4.3/kogi/service/slack.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/service/textra.py` & `kogi-0.4.3/kogi/service/textra.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/task/code.py` & `kogi-0.4.3/kogi/task/code.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/task/diagnosis.py` & `kogi-0.4.3/kogi/task/diagnosis.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/task/multi.py` & `kogi-0.4.3/kogi/task/multi.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/task/runner.py` & `kogi-0.4.3/kogi/task/runner.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/transform.py` & `kogi-0.4.3/kogi/transform.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/_canvas.py` & `kogi-0.4.3/kogi/ui/_canvas.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/chatgpt-fs8.png` & `kogi-0.4.3/kogi/ui/chatgpt-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/content.py` & `kogi-0.4.3/kogi/ui/content.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/dialog.css` & `kogi-0.4.3/kogi/ui/dialog.css`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/dialog.html` & `kogi-0.4.3/kogi/ui/dialog.html`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/dialog.js` & `kogi-0.4.3/kogi/ui/dialog.js`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/dialog_colab.py` & `kogi-0.4.3/kogi/ui/dialog_colab.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/dialog_ipywidgets.py` & `kogi-0.4.3/kogi/ui/dialog_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/error-fs8.png` & `kogi-0.4.3/kogi/ui/error-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/girl-fs8.png` & `kogi-0.4.3/kogi/ui/girl-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/girl_think-fs8.png` & `kogi-0.4.3/kogi/ui/girl_think-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/keylogin.py` & `kogi-0.4.3/kogi/ui/keylogin.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,40 +145,46 @@
     '最近、どんどん上達している感じだね！',
     'なんだか、プログラミングは十分、得意そうだね！',
     'お、上級者来たね！',
 ]
 
 ZHTBL = str.maketrans('０１２３４５６７８９', '0123456789')
 STUDENT_CODE = 'm8YpbzR6ovEjyzJ8oXnpT3BlbkFJYwKQCc1DmrTOj4Adj'
-K='k'
+K = 'k'
+
+PID = ('223', '222', '220', '221', '122', '123')
+
+
+def check_uname(s):
+    for p in PID:
+        if s.startswith(p):
+            return True
+    return False
 
 
 def ulogin(uname, code, ucode, ukeys):
     try:
         kogi_set(approved=True)
         uname = uname.translate(ZHTBL)
-        is_student = uname.startswith("223") or uname.startswith(
-            "222") or uname.startswith("220") or uname.startswith("221")
+        is_student = check_uname(uname)
         average_time, ulevel = check_level(ukeys)
         kogi_set(uname=uname, ulevel=ulevel, approved=True)
         record_log(type='key', uname=uname, code=code,
                    ucode=ucode, average_time=average_time,
                    ulevel=ulevel, ukeys=ukeys)
         if is_student:
-          msg = f'コギーくんを呼んだわ！ {ULEVEL[ulevel-1]}'
-          kogi_set(openai_key=f's{K}-{STUDENT_CODE}Ag8')
+            msg = f'コギーくんを呼んだわ！ {ULEVEL[ulevel-1]}'
+            kogi_set(openai_key=f's{K}-{STUDENT_CODE}Ag8')
         else:
-          msg = f'学籍番号が変ですね。AIを使いたいなら再実行してね。'
+            msg = f'学籍番号が変ね。AIを使いたいなら再起動してね。'
         return JSON({'text': msg})
     except:
         traceback.print_exc()
         return JSON({'text': 'よろしく！'})
 
 
 def login(login_func=ulogin):
     if google_colab:
         google_colab.register_callback('notebook.login', login_func)
     doc = Doc.HTML(LOGIN_HTML)
     doc.set_mention('@ta')
     kogi_print(doc, height=280)
-
-
```

### Comparing `kogi-0.4.1/kogi/ui/kogi-fs8.png` & `kogi-0.4.3/kogi/ui/kogi-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/kogi_doya-fs8.png` & `kogi-0.4.3/kogi/ui/kogi_doya-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/kogi_error-fs8.png` & `kogi-0.4.3/kogi/ui/kogi_error-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/kogi_gaan-fs8.png` & `kogi-0.4.3/kogi/ui/kogi_gaan-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/kogi_vow-fs8.png` & `kogi-0.4.3/kogi/ui/kogi_vow-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/message.py` & `kogi-0.4.3/kogi/ui/message.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/openai-fs8.png` & `kogi-0.4.3/kogi/ui/openai-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/render.py` & `kogi-0.4.3/kogi/ui/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,23 @@
 
 # mini md
 
 _CODE = re.compile(r'(`[^`]+`)')
 _BOLD = re.compile(r'(__[^_]+__)')
 
 
+def replace_pre(s):
+    while '```' in s:
+        s = s.replace('```', '<pre>', 1).replace('```', '</pre>', 1)
+    return s
+
+
 def encode_md(s):
     s = s.replace('<', '&lt;').replace('>', '&gt;').replace('\n', '<br>')
+    s = replace_pre(s)
     for t in re.findall(_CODE, s):
         t2 = f'<code>{t[1:-1]}</code>'
         s = s.replace(t, t2)
     for t in re.findall(_BOLD, s):
         t2 = f'<b>{t[2:-2]}</b>'
         s = s.replace(t, t2)
     return s
@@ -23,14 +30,23 @@
         s = s.replace(t, t2)
     for t in re.findall(_BOLD, s):
         t2 = t[2:-2]
         s = s.replace(t, t2)
     return s
 
 
+# try:
+#     import markdown
+
+#     def encode_md(s):
+#         return markdown.markdown(s)
+# except ModuleNotFoundError:
+#     pass
+
+
 TERM = {
     'code': '\033[35m{}\033[0m',
     'glay': '\033[07m{}\033[0m',
     'red': '\033[31m{}\033[0m',
     'green': '\033[32m{}\033[0m',
     'yellow': '\033[33m{}\033[0m',
     'blue': '\033[34m{}\033[0m',
@@ -196,23 +212,26 @@
         button = f'''\
 <span id="b{frmid}">
 <button class="likeit" onclick="like({recid},1,'b{frmid}')">{like}</button>
 <button class="likeit" onclick="like({recid},0,'b{frmid}')">{{}}</button>
 </span>'''
         self.htmls.append(Doc(dislike, style=button))
 
-
     def add_button(self, cmd, message, frmid=None):
         frmid = frameid(frmid)
         cmd = f"'{cmd}'"
         button = f'<button id="b{frmid}" onclick="say({cmd},{frmid})">{{}}</button>'
         self.htmls.append(Doc(message, style=button))
 
-    def set_mention(self, mention):
-        self.mention = mention
+    def set_mention(self, mention: str):
+        if mention.startswith('@'):
+            mention, _, text = mention.partition(':')
+            self.mention = mention
+            return text
+        return mention
 
     def get_mention(self, default=None):
         if hasattr(self, 'mention'):
             return self.mention
         for d in self.htmls:
             if isinstance(d, Doc):
                 mention = d.get_mention()
@@ -230,14 +249,15 @@
                 if s != '':
                     script += s
         return script
 
     @classmethod
     def md(cls, s, style=None):
         doc = Doc(style=style)
+        s = doc.set_mention(s)
         doc.htmls.append(encode_md(s))
         doc.terms.append(encode_md_term(s))
         doc.texts.append(encode_md_text(s))
         return doc
 
     @classmethod
     def HTML(cls, html, text=None, css=None, script=None):
```

### Comparing `kogi-0.4.1/kogi/ui/rmt.py` & `kogi-0.4.3/kogi/ui/rmt.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/robot-fs8.png` & `kogi-0.4.3/kogi/ui/robot-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/slides.py` & `kogi-0.4.3/kogi/ui/slides.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/ta-fs8.png` & `kogi-0.4.3/kogi/ui/ta-fs8.png`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/typewriter.py` & `kogi-0.4.3/kogi/ui/typewriter.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi/ui/wait_and_ready.py` & `kogi-0.4.3/kogi/ui/wait_and_ready.py`

 * *Files identical despite different names*

### Comparing `kogi-0.4.1/kogi.egg-info/PKG-INFO` & `kogi-0.4.3/kogi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kogi
-Version: 0.4.1
+Version: 0.4.3
 Summary: Kogi Programming Assistant AI
 Home-page: https://github.com/kkuramitsu/kogi
 Author: Kimio Kuramitsu
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kogi-0.4.1/kogi.egg-info/SOURCES.txt` & `kogi-0.4.3/kogi.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -58,25 +58,20 @@
 kogi/ui/dialog_ipywidgets.py
 kogi/ui/error-fs8.png
 kogi/ui/girl-fs8.png
 kogi/ui/girl_think-fs8.png
 kogi/ui/keylogin.py
 kogi/ui/kogi-fs8.png
 kogi/ui/kogi_doya-fs8.png
-kogi/ui/kogi_doya.png
 kogi/ui/kogi_error-fs8.png
-kogi/ui/kogi_error.png
 kogi/ui/kogi_gaan-fs8.png
-kogi/ui/kogi_gaan.png
 kogi/ui/kogi_vow-fs8.png
 kogi/ui/main.css
 kogi/ui/message.py
 kogi/ui/openai-fs8.png
-kogi/ui/openai.png
-kogi/ui/pan.png
 kogi/ui/render.py
 kogi/ui/rmt.py
 kogi/ui/robot-fs8.png
 kogi/ui/slides.py
 kogi/ui/ta-fs8.png
 kogi/ui/typewriter.py
 kogi/ui/wait_and_ready.py
```

### Comparing `kogi-0.4.1/setup.py` & `kogi-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(name="kogi",
-      version="0.4.1",
+      version="0.4.3",
       license='MIT',
       author='Kimio Kuramitsu',
       description="Kogi Programming Assistant AI",
       url="https://github.com/kkuramitsu/kogi",
       packages=['kogi', 'kogi.liberr', 'kogi.task', 'kogi.data',
                 'kogi.service', 'kogi.problem', 'kogi.ui'],
       # package_dir={"": "src"},
```

