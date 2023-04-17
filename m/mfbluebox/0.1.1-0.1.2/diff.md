# Comparing `tmp/mfbluebox-0.1.1.tar.gz` & `tmp/mfbluebox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfbluebox-0.1.1.tar", last modified: Mon Apr 17 10:59:32 2023, max compression
+gzip compressed data, was "mfbluebox-0.1.2.tar", last modified: Mon Apr 17 11:09:41 2023, max compression
```

## Comparing `mfbluebox-0.1.1.tar` & `mfbluebox-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:59:32.125630 mfbluebox-0.1.1/
--rw-rw-rw-   0        0        0     1061 2023-03-07 12:05:58.000000 mfbluebox-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     5367 2023-04-17 10:59:32.124636 mfbluebox-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3572 2023-04-17 10:40:09.000000 mfbluebox-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:59:32.050226 mfbluebox-0.1.1/bluebox/
--rw-rw-rw-   0        0        0      469 2023-04-17 10:53:40.000000 mfbluebox-0.1.1/bluebox/__init__.py
--rw-rw-rw-   0        0        0       87 2023-04-17 10:53:16.000000 mfbluebox-0.1.1/bluebox/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:59:32.068695 mfbluebox-0.1.1/bluebox/backends/
--rw-rw-rw-   0        0        0      724 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/backends/__init__.py
--rw-rw-rw-   0        0        0     2054 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/backends/backend_dummy.py
--rw-rw-rw-   0        0        0     4642 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/backends/backend_pyaudio.py
--rw-rw-rw-   0        0        0     1270 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/backends/base.py
--rw-rw-rw-   0        0        0     5869 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/box.py
--rw-rw-rw-   0        0        0     5374 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/cli.py
--rw-rw-rw-   0        0        0     4406 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/freqs.py
--rw-rw-rw-   0        0        0     2439 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/bluebox/wave.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:59:32.100245 mfbluebox-0.1.1/mfbluebox.egg-info/
--rw-rw-rw-   0        0        0     5367 2023-04-17 10:59:31.000000 mfbluebox-0.1.1/mfbluebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-04-17 10:59:31.000000 mfbluebox-0.1.1/mfbluebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:59:31.000000 mfbluebox-0.1.1/mfbluebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:59:31.000000 mfbluebox-0.1.1/mfbluebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:59:31.000000 mfbluebox-0.1.1/mfbluebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1017 2023-04-17 10:58:46.000000 mfbluebox-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 10:59:32.126651 mfbluebox-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 10:59:32.119108 mfbluebox-0.1.1/tests/
--rw-rw-rw-   0        0        0     4830 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/tests/test_box.py
--rw-rw-rw-   0        0        0      461 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/tests/test_cli.py
--rw-rw-rw-   0        0        0     3234 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/tests/test_freqs.py
--rw-rw-rw-   0        0        0     1815 2023-03-07 12:05:59.000000 mfbluebox-0.1.1/tests/test_wave.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:41.402208 mfbluebox-0.1.2/
+-rw-rw-rw-   0        0        0     1061 2023-03-07 12:05:58.000000 mfbluebox-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     5410 2023-04-17 11:09:41.400208 mfbluebox-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3607 2023-04-17 11:04:04.000000 mfbluebox-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:41.325444 mfbluebox-0.1.2/bluebox/
+-rw-rw-rw-   0        0        0      469 2023-04-17 11:08:58.000000 mfbluebox-0.1.2/bluebox/__init__.py
+-rw-rw-rw-   0        0        0       87 2023-04-17 10:53:16.000000 mfbluebox-0.1.2/bluebox/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:41.346474 mfbluebox-0.1.2/bluebox/backends/
+-rw-rw-rw-   0        0        0      724 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/backends/__init__.py
+-rw-rw-rw-   0        0        0     2054 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/backends/backend_dummy.py
+-rw-rw-rw-   0        0        0     4642 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/backends/backend_pyaudio.py
+-rw-rw-rw-   0        0        0     1270 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/backends/base.py
+-rw-rw-rw-   0        0        0     5869 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/box.py
+-rw-rw-rw-   0        0        0     5374 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/cli.py
+-rw-rw-rw-   0        0        0     4406 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/freqs.py
+-rw-rw-rw-   0        0        0     2439 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/bluebox/wave.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:41.379568 mfbluebox-0.1.2/mfbluebox.egg-info/
+-rw-rw-rw-   0        0        0     5410 2023-04-17 11:09:41.000000 mfbluebox-0.1.2/mfbluebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-04-17 11:09:41.000000 mfbluebox-0.1.2/mfbluebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:09:41.000000 mfbluebox-0.1.2/mfbluebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 11:09:41.000000 mfbluebox-0.1.2/mfbluebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 11:09:41.000000 mfbluebox-0.1.2/mfbluebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1017 2023-04-17 11:09:04.000000 mfbluebox-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:09:41.402208 mfbluebox-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:41.395088 mfbluebox-0.1.2/tests/
+-rw-rw-rw-   0        0        0     4830 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/tests/test_box.py
+-rw-rw-rw-   0        0        0      461 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/tests/test_cli.py
+-rw-rw-rw-   0        0        0     3234 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/tests/test_freqs.py
+-rw-rw-rw-   0        0        0     1815 2023-03-07 12:05:59.000000 mfbluebox-0.1.2/tests/test_wave.py
```

### Comparing `mfbluebox-0.1.1/LICENSE.md` & `mfbluebox-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/PKG-INFO` & `mfbluebox-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfbluebox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python (Dual-Tone) Multi-Frequency (DTMF) tone generator.
 Author-email: zeyus <support@zeyus.com>
 License: MIT License
         
         Copyright (c) 2023 zeyus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -37,36 +37,44 @@
 ### Why?
 
 Well, initially this was a fun little python 3 project from 2015, but I thought it would be nice to make it modern and extensible, essentially showcasing it as a framework, but this doesn't have to be limited to DTMF / MF, in theory with ease you could turn this into something that reads in code sequences (`str`) and outputs waves. Also due to issue #3 https://github.com/zeyus/Python3BlueBox/issues/3 it was clear that there were some bugs, so what better way to deal with it than adding tests and a way to decouple things!
 
 
 ## Installation
 
+### PyPI
+
+```
+pip install mfbluebox
+```
+
+### Development
+
 ```
 git clone https://github.com/zeyus/Python3BlueBox.git
 cd PythonBlueBox
-pip install -r requirements.txt
+pip install .
 ```
 
 ### Requirements
 
 - Python 3 (tested on 3.9 - 3.11)
 
 ## Usage
 
 ### CLI
 
 ```
-python ./bluebox.py -h
+python -m bluebox -h
 ```
 
 Output:
 
 ```
-usage: bluebox.py [-h] [-l LENGTH] [-p PAUSE] [-a AMPLITUDE] [-s SAMPLE_RATE] [-m MF] [-d] [-b BACKEND] [-r PAD_PAUSE_DURATION] [-f FILE] [-P PIPE] [-S] [-i] [-v] [sequence]
+usage: __main__.py [-h] [-l LENGTH] [-p PAUSE] [-a AMPLITUDE] [-s SAMPLE_RATE] [-m MF] [-d] [-b BACKEND] [-r PAD_PAUSE_DURATION] [-f FILE] [-P PIPE] [-S] [-i] [-v] [sequence]
 
 Generate tone sequences.
 
 positional arguments:
   sequence              The sequence of tones to generate.
 
 options:
@@ -91,19 +99,19 @@
   -i, --interactive     Enter interactive mode.
   -v, --version         show program's version number and exit
 ```
 
 **Examples**
 
 ```
-python ./bluebox.py -i
+python -m bluebox -i
 ```
 
 ```
-python ./bluebox.py 123456789
+python -m bluebox 123456789
 ```
 
 ### API
 
 You mainly need an `BaseMF` subclass instance and a `Sequencer` instance.
 
 ```python
```

### Comparing `mfbluebox-0.1.1/README.md` & `mfbluebox-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,36 +14,44 @@
 ### Why?
 
 Well, initially this was a fun little python 3 project from 2015, but I thought it would be nice to make it modern and extensible, essentially showcasing it as a framework, but this doesn't have to be limited to DTMF / MF, in theory with ease you could turn this into something that reads in code sequences (`str`) and outputs waves. Also due to issue #3 https://github.com/zeyus/Python3BlueBox/issues/3 it was clear that there were some bugs, so what better way to deal with it than adding tests and a way to decouple things!
 
 
 ## Installation
 
+### PyPI
+
+```
+pip install mfbluebox
+```
+
+### Development
+
 ```
 git clone https://github.com/zeyus/Python3BlueBox.git
 cd PythonBlueBox
-pip install -r requirements.txt
+pip install .
 ```
 
 ### Requirements
 
 - Python 3 (tested on 3.9 - 3.11)
 
 ## Usage
 
 ### CLI
 
 ```
-python ./bluebox.py -h
+python -m bluebox -h
 ```
 
 Output:
 
 ```
-usage: bluebox.py [-h] [-l LENGTH] [-p PAUSE] [-a AMPLITUDE] [-s SAMPLE_RATE] [-m MF] [-d] [-b BACKEND] [-r PAD_PAUSE_DURATION] [-f FILE] [-P PIPE] [-S] [-i] [-v] [sequence]
+usage: __main__.py [-h] [-l LENGTH] [-p PAUSE] [-a AMPLITUDE] [-s SAMPLE_RATE] [-m MF] [-d] [-b BACKEND] [-r PAD_PAUSE_DURATION] [-f FILE] [-P PIPE] [-S] [-i] [-v] [sequence]
 
 Generate tone sequences.
 
 positional arguments:
   sequence              The sequence of tones to generate.
 
 options:
@@ -68,19 +76,19 @@
   -i, --interactive     Enter interactive mode.
   -v, --version         show program's version number and exit
 ```
 
 **Examples**
 
 ```
-python ./bluebox.py -i
+python -m bluebox -i
 ```
 
 ```
-python ./bluebox.py 123456789
+python -m bluebox 123456789
 ```
 
 ### API
 
 You mainly need an `BaseMF` subclass instance and a `Sequencer` instance.
 
 ```python
```

### Comparing `mfbluebox-0.1.1/bluebox/backends/__init__.py` & `mfbluebox-0.1.2/bluebox/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/bluebox/backends/backend_dummy.py` & `mfbluebox-0.1.2/bluebox/backends/backend_dummy.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/bluebox/backends/backend_pyaudio.py` & `mfbluebox-0.1.2/bluebox/backends/backend_pyaudio.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/bluebox/backends/base.py` & `mfbluebox-0.1.2/bluebox/backends/base.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/bluebox/box.py` & `mfbluebox-0.1.2/bluebox/box.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/bluebox/cli.py` & `mfbluebox-0.1.2/bluebox/cli.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/bluebox/freqs.py` & `mfbluebox-0.1.2/bluebox/freqs.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/bluebox/wave.py` & `mfbluebox-0.1.2/bluebox/wave.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/mfbluebox.egg-info/PKG-INFO` & `mfbluebox-0.1.2/mfbluebox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfbluebox
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python (Dual-Tone) Multi-Frequency (DTMF) tone generator.
 Author-email: zeyus <support@zeyus.com>
 License: MIT License
         
         Copyright (c) 2023 zeyus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -37,36 +37,44 @@
 ### Why?
 
 Well, initially this was a fun little python 3 project from 2015, but I thought it would be nice to make it modern and extensible, essentially showcasing it as a framework, but this doesn't have to be limited to DTMF / MF, in theory with ease you could turn this into something that reads in code sequences (`str`) and outputs waves. Also due to issue #3 https://github.com/zeyus/Python3BlueBox/issues/3 it was clear that there were some bugs, so what better way to deal with it than adding tests and a way to decouple things!
 
 
 ## Installation
 
+### PyPI
+
+```
+pip install mfbluebox
+```
+
+### Development
+
 ```
 git clone https://github.com/zeyus/Python3BlueBox.git
 cd PythonBlueBox
-pip install -r requirements.txt
+pip install .
 ```
 
 ### Requirements
 
 - Python 3 (tested on 3.9 - 3.11)
 
 ## Usage
 
 ### CLI
 
 ```
-python ./bluebox.py -h
+python -m bluebox -h
 ```
 
 Output:
 
 ```
-usage: bluebox.py [-h] [-l LENGTH] [-p PAUSE] [-a AMPLITUDE] [-s SAMPLE_RATE] [-m MF] [-d] [-b BACKEND] [-r PAD_PAUSE_DURATION] [-f FILE] [-P PIPE] [-S] [-i] [-v] [sequence]
+usage: __main__.py [-h] [-l LENGTH] [-p PAUSE] [-a AMPLITUDE] [-s SAMPLE_RATE] [-m MF] [-d] [-b BACKEND] [-r PAD_PAUSE_DURATION] [-f FILE] [-P PIPE] [-S] [-i] [-v] [sequence]
 
 Generate tone sequences.
 
 positional arguments:
   sequence              The sequence of tones to generate.
 
 options:
@@ -91,19 +99,19 @@
   -i, --interactive     Enter interactive mode.
   -v, --version         show program's version number and exit
 ```
 
 **Examples**
 
 ```
-python ./bluebox.py -i
+python -m bluebox -i
 ```
 
 ```
-python ./bluebox.py 123456789
+python -m bluebox 123456789
 ```
 
 ### API
 
 You mainly need an `BaseMF` subclass instance and a `Sequencer` instance.
 
 ```python
```

### Comparing `mfbluebox-0.1.1/pyproject.toml` & `mfbluebox-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mfbluebox"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="zeyus", email="support@zeyus.com" },
 ]
 description = "A python (Dual-Tone) Multi-Frequency (DTMF) tone generator."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mfbluebox-0.1.1/tests/test_box.py` & `mfbluebox-0.1.2/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/tests/test_freqs.py` & `mfbluebox-0.1.2/tests/test_freqs.py`

 * *Files identical despite different names*

### Comparing `mfbluebox-0.1.1/tests/test_wave.py` & `mfbluebox-0.1.2/tests/test_wave.py`

 * *Files identical despite different names*

