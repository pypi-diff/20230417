# Comparing `tmp/py_spacy_redact_message-0.0.27.tar.gz` & `tmp/py_spacy_redact_message-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_spacy_redact_message-0.0.27.tar", last modified: Sun Apr 16 11:11:19 2023, max compression
+gzip compressed data, was "py_spacy_redact_message-0.0.28.tar", last modified: Mon Apr 17 09:57:26 2023, max compression
```

## Comparing `py_spacy_redact_message-0.0.27.tar` & `py_spacy_redact_message-0.0.28.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 11:11:19.019857 py_spacy_redact_message-0.0.27/
--rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.27/LICENSE
--rw-r--r--   0 alexilin   (501) staff       (20)      320 2023-04-16 11:11:19.019681 py_spacy_redact_message-0.0.27/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-16 11:04:17.000000 py_spacy_redact_message-0.0.27/README.md
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 11:11:19.017426 py_spacy_redact_message-0.0.27/py_spacy_redact_message/
--rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message/__init__.py
--rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message/main.py
-drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-16 11:11:19.019464 py_spacy_redact_message-0.0.27/py_spacy_redact_message.egg-info/
--rw-r--r--   0 alexilin   (501) staff       (20)      320 2023-04-16 11:11:19.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message.egg-info/PKG-INFO
--rw-r--r--   0 alexilin   (501) staff       (20)      393 2023-04-16 11:11:19.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message.egg-info/SOURCES.txt
--rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-16 11:11:19.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message.egg-info/dependency_links.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-16 11:11:19.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message.egg-info/entry_points.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-16 11:11:19.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message.egg-info/requires.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-16 11:11:19.000000 py_spacy_redact_message-0.0.27/py_spacy_redact_message.egg-info/top_level.txt
--rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:05:29.000000 py_spacy_redact_message-0.0.27/pyproject.toml
--rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-16 11:11:19.019900 py_spacy_redact_message-0.0.27/setup.cfg
--rw-r--r--   0 alexilin   (501) staff       (20)      772 2023-04-16 11:11:15.000000 py_spacy_redact_message-0.0.27/setup.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-17 09:57:26.786950 py_spacy_redact_message-0.0.28/
+-rw-r--r--   0 alexilin   (501) staff       (20)     1068 2023-04-15 10:09:58.000000 py_spacy_redact_message-0.0.28/LICENSE
+-rw-r--r--   0 alexilin   (501) staff       (20)      449 2023-04-17 09:57:26.786783 py_spacy_redact_message-0.0.28/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)       30 2023-04-16 11:04:17.000000 py_spacy_redact_message-0.0.28/README.md
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-17 09:57:26.785247 py_spacy_redact_message-0.0.28/py_spacy_redact_message/
+-rw-r--r--   0 alexilin   (501) staff       (20)        0 2023-04-15 10:52:13.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message/__init__.py
+-rw-r--r--   0 alexilin   (501) staff       (20)      780 2023-04-16 09:51:51.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message/main.py
+drwxr-xr-x   0 alexilin   (501) staff       (20)        0 2023-04-17 09:57:26.786560 py_spacy_redact_message-0.0.28/py_spacy_redact_message.egg-info/
+-rw-r--r--   0 alexilin   (501) staff       (20)      449 2023-04-17 09:57:26.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message.egg-info/PKG-INFO
+-rw-r--r--   0 alexilin   (501) staff       (20)      393 2023-04-17 09:57:26.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message.egg-info/SOURCES.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)        1 2023-04-17 09:57:26.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message.egg-info/dependency_links.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       77 2023-04-17 09:57:26.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message.egg-info/entry_points.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       12 2023-04-17 09:57:26.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message.egg-info/requires.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       24 2023-04-17 09:57:26.000000 py_spacy_redact_message-0.0.28/py_spacy_redact_message.egg-info/top_level.txt
+-rw-r--r--   0 alexilin   (501) staff       (20)       89 2023-04-16 10:05:29.000000 py_spacy_redact_message-0.0.28/pyproject.toml
+-rw-r--r--   0 alexilin   (501) staff       (20)       38 2023-04-17 09:57:26.786989 py_spacy_redact_message-0.0.28/setup.cfg
+-rw-r--r--   0 alexilin   (501) staff       (20)      885 2023-04-17 09:57:22.000000 py_spacy_redact_message-0.0.28/setup.py
```

### Comparing `py_spacy_redact_message-0.0.27/LICENSE` & `py_spacy_redact_message-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `py_spacy_redact_message-0.0.27/py_spacy_redact_message/main.py` & `py_spacy_redact_message-0.0.28/py_spacy_redact_message/main.py`

 * *Files identical despite different names*

