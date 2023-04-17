# Comparing `tmp/speech2speech-0.1.0.tar.gz` & `tmp/speech2speech-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech2speech-0.1.0.tar", last modified: Sat Apr 15 20:17:32 2023, max compression
+gzip compressed data, was "speech2speech-0.2.0.tar", last modified: Mon Apr 17 13:10:52 2023, max compression
```

## Comparing `speech2speech-0.1.0.tar` & `speech2speech-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-15 20:17:32.374057 speech2speech-0.1.0/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     6155 2023-04-15 20:17:32.374057 speech2speech-0.1.0/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     5438 2023-04-13 12:53:43.000000 speech2speech-0.1.0/README.md
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      612 2023-04-15 20:17:24.000000 speech2speech-0.1.0/pyproject.toml
--rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-15 20:17:32.374057 speech2speech-0.1.0/setup.cfg
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     8181 2023-04-15 20:05:42.000000 speech2speech-0.1.0/setup.py
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-15 20:17:32.370057 speech2speech-0.1.0/speech2speech/
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-15 20:17:32.370057 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     6155 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/SOURCES.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/dependency_links.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/top_level.txt
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-17 13:10:52.385020 speech2speech-0.2.0/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     6413 2023-04-17 13:10:52.385020 speech2speech-0.2.0/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     5721 2023-04-17 12:46:20.000000 speech2speech-0.2.0/README.md
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      612 2023-04-17 12:58:06.000000 speech2speech-0.2.0/pyproject.toml
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-17 13:10:52.385020 speech2speech-0.2.0/setup.cfg
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     8063 2023-04-17 13:08:30.000000 speech2speech-0.2.0/setup.py
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-17 13:10:52.385020 speech2speech-0.2.0/speech2speech/
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-17 13:10:52.385020 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     6413 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-17 13:10:52.000000 speech2speech-0.2.0/speech2speech/speech2speech.egg-info/top_level.txt
```

### Comparing `speech2speech-0.1.0/PKG-INFO` & `speech2speech-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 Metadata-Version: 2.1
 Name: speech2speech
-Version: 0.1.0
+Version: 0.2.0
 Summary: Source lang speech to machine translation to target lang speech
 Home-page: https://github.com/rcdalj/speech2speech
 Author: rcdalj
 Author-email: rcdalj1 <rcdalj1@gmail.com>
 Project-URL: Homepage, https://github.com/rcdalj/speech2speech
 Project-URL: Bug Tracker, https://github.com/rcdalj/speech2speech/issues
-Keywords: speech_recognition,machine_translation,text_to_speech,setuptools,development,python-3,chat-gpt,whisper-ai,pyaudio,gtts
+Keywords: speech_recognition,machine_translation,text_to_speech,python-3,chat-gpt,whisper-ai,pyaudio,gtts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3, <4
 Description-Content-Type: text/markdown
 
 # Speech2Speech
 
-The Speech2Speech Python package **models all phases of speech-to-speech translation**, which include
-- recording speech, 
-- converting speech to text, 
-- translating text to a target language, and 
-- converting the translated text back to speech. 
-
-Each phase of the workflow creates a file, whose name is defined in the config.ini file. Advanced users can start or interrupt the workflow wherever they want by specifying their own files and adapting the config.ini file to refer to them. The user can also launch a specific phase of the workflow by clicking on the corresponding button.
-
-Speech2Speech is designed to be accessible to a **broad audience**, including non-technical users. The package **does not require any specialized software training or user knowledge** and can be used straight out of the box. This makes it incredibly accessible to a wide range of users, including those with visual impairments who can input text by dictating it and have the package read documents aloud.
-
-The package uses PyAudio, Open AI Whisper, Chat-GPT, and Google gttx and can automatically detect the source language used in speech. Users can, therefore, access accurate translations for a **wide range of languages** without having to switch between different translation tools. Although the quality of translation may vary depending on the target language, it is pretty good for popular languages such as English, French, Portuguese, Spanish, German, Dutch and Italian.
+The Speech2Speech Python package is a Streamlit Web application that **models 
+all phases of speech-to-speech translation**, including:
+- recording speech in the source language, 
+- converting the source language speech to source language text, 
+- translating the source language text to target language text, and 
+- converting the translated text to speech in the target language. 
+
+Speech2Speech is currently **configured to translate to and from 13 different 
+languages**. Although the quality of  translation may vary depending on the 
+target language, it is pretty good for popular languages such as English, 
+French, Portuguese, Spanish, German, Dutch and Italian. Speech2Speech **can be 
+configured for many more than just these languages** (specified in the config.
+ini file), as long as they are supported by Whisper AI, Chat-GPT and gtts, 
+the packages on which it depends.
+
+The package **automatically detects the source language used in speech**. The 
+user therefore is not asked to specify it.
+
+Speech2Speech is designed to be accessible to a **broad audience**. One of 
+the key advantages of Speech2Speech is that it's incredibly easy to use. 
+There is **no need to train the software or the user before actually using 
+the product**. It works well straight out of the box with no further tuning 
+or configuration required. This makes it a highly accessible tool that anyone can use, regardless of their technical expertise or experience with speech recognition and machine translation technology.
+
+Each phase of the workflow creates a file, whose name is defined in the 
+config.ini file. Advanced users can **start and/or interrupt the workflow 
+wherever they need** by inserting their own files in the speech2speech/data 
+subdirectory and adapting the config.ini file to refer to them. 
 
 Prerequisites
 -----------------------------------------------------------------------------
 Before using Speech2Speech, you need to sign up for an OpenAI account, create an API key, and set up an environment variable. Here's how to do it:
 
 1. **Signup and Create an OpenAI Account**: Go to the OpenAI website and 
    click on the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
@@ -112,8 +129,9 @@
    Page" button to reset the page.
    
 As indicated above, you can also use just parts of this full workflow by specifying the name(s) of the file(s) you want to use in the config.ini file and by clicking the relevant button of the user interface.
 
 What to do if you encounter issues
 -------------------------------
 
-If Chat-GPT or speech2speech get stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
+If Chat-GPT or Speech2Speech get stuck or you encounter any issues, simply 
+refresh the browser page.
```

### Comparing `speech2speech-0.1.0/README.md` & `speech2speech-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 # Speech2Speech
 
-The Speech2Speech Python package **models all phases of speech-to-speech translation**, which include
-- recording speech, 
-- converting speech to text, 
-- translating text to a target language, and 
-- converting the translated text back to speech. 
-
-Each phase of the workflow creates a file, whose name is defined in the config.ini file. Advanced users can start or interrupt the workflow wherever they want by specifying their own files and adapting the config.ini file to refer to them. The user can also launch a specific phase of the workflow by clicking on the corresponding button.
-
-Speech2Speech is designed to be accessible to a **broad audience**, including non-technical users. The package **does not require any specialized software training or user knowledge** and can be used straight out of the box. This makes it incredibly accessible to a wide range of users, including those with visual impairments who can input text by dictating it and have the package read documents aloud.
-
-The package uses PyAudio, Open AI Whisper, Chat-GPT, and Google gttx and can automatically detect the source language used in speech. Users can, therefore, access accurate translations for a **wide range of languages** without having to switch between different translation tools. Although the quality of translation may vary depending on the target language, it is pretty good for popular languages such as English, French, Portuguese, Spanish, German, Dutch and Italian.
+The Speech2Speech Python package is a Streamlit Web application that **models 
+all phases of speech-to-speech translation**, including:
+- recording speech in the source language, 
+- converting the source language speech to source language text, 
+- translating the source language text to target language text, and 
+- converting the translated text to speech in the target language. 
+
+Speech2Speech is currently **configured to translate to and from 13 different 
+languages**. Although the quality of  translation may vary depending on the 
+target language, it is pretty good for popular languages such as English, 
+French, Portuguese, Spanish, German, Dutch and Italian. Speech2Speech **can be 
+configured for many more than just these languages** (specified in the config.
+ini file), as long as they are supported by Whisper AI, Chat-GPT and gtts, 
+the packages on which it depends.
+
+The package **automatically detects the source language used in speech**. The 
+user therefore is not asked to specify it.
+
+Speech2Speech is designed to be accessible to a **broad audience**. One of 
+the key advantages of Speech2Speech is that it's incredibly easy to use. 
+There is **no need to train the software or the user before actually using 
+the product**. It works well straight out of the box with no further tuning 
+or configuration required. This makes it a highly accessible tool that anyone can use, regardless of their technical expertise or experience with speech recognition and machine translation technology.
+
+Each phase of the workflow creates a file, whose name is defined in the 
+config.ini file. Advanced users can **start and/or interrupt the workflow 
+wherever they need** by inserting their own files in the speech2speech/data 
+subdirectory and adapting the config.ini file to refer to them. 
 
 Prerequisites
 -----------------------------------------------------------------------------
 Before using Speech2Speech, you need to sign up for an OpenAI account, create an API key, and set up an environment variable. Here's how to do it:
 
 1. **Signup and Create an OpenAI Account**: Go to the OpenAI website and 
    click on the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
@@ -96,8 +113,9 @@
    Page" button to reset the page.
    
 As indicated above, you can also use just parts of this full workflow by specifying the name(s) of the file(s) you want to use in the config.ini file and by clicking the relevant button of the user interface.
 
 What to do if you encounter issues
 -------------------------------
 
-If Chat-GPT or speech2speech get stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
+If Chat-GPT or Speech2Speech get stuck or you encounter any issues, simply 
+refresh the browser page.
```

### Comparing `speech2speech-0.1.0/pyproject.toml` & `speech2speech-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "speech2speech"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="rcdalj1", email="rcdalj1@gmail.com" },
 ]
 description = "Source lang speech to machine translation to target lang speech"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `speech2speech-0.1.0/setup.py` & `speech2speech-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     name="speech2speech",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.1.0",  # Required
+    version="0.2.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description="Speech2Speech is a Python package that performs vocal  "
-                "recognition of your speech, followed by translation to a "
-                "target language  of your choice, which is then read out loud "
-                "by a high-quality voice.",  # Optional
+    description="Speech2Speech is a Python package that performs speech  "
+                "recognition of your voice, followed by translation to a "
+                "target language  of your choice, which is then read out "
+                "aloud by a high-quality voice.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
@@ -79,37 +79,35 @@
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
-        "Intended Audience :: Developers",
+        "Intended Audience :: End Users/Desktop",
         "Topic :: Speech Recognition :: Machine Translation :: Text to Speech",
         # Pick your license as you wish
-        "License :: OSI Approved :: MIT License",
+        "License :: Free for non-commercial use",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3 :: Only",
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
     keywords="speech_recognition, machine_translation, text_to_speech, "
-             "setuptools, development, python-3, chat-gpt, whisper-ai, "
+             "python-3, chat-gpt, whisper-ai, "
              "pyaudio, gtts",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
     package_dir={"": "speech2speech"},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
@@ -120,15 +118,15 @@
     #   py_modules=["my_module"],
     #
     packages=find_packages(where="speech2speech"),  # Required
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires=">=3.7, <4",
+    python_requires=">=3, <4",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     # install_requires=[],  # Optional
```

### Comparing `speech2speech-0.1.0/speech2speech/speech2speech.egg-info/PKG-INFO` & `speech2speech-0.2.0/speech2speech/speech2speech.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 Metadata-Version: 2.1
 Name: speech2speech
-Version: 0.1.0
+Version: 0.2.0
 Summary: Source lang speech to machine translation to target lang speech
 Home-page: https://github.com/rcdalj/speech2speech
 Author: rcdalj
 Author-email: rcdalj1 <rcdalj1@gmail.com>
 Project-URL: Homepage, https://github.com/rcdalj/speech2speech
 Project-URL: Bug Tracker, https://github.com/rcdalj/speech2speech/issues
-Keywords: speech_recognition,machine_translation,text_to_speech,setuptools,development,python-3,chat-gpt,whisper-ai,pyaudio,gtts
+Keywords: speech_recognition,machine_translation,text_to_speech,python-3,chat-gpt,whisper-ai,pyaudio,gtts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3, <4
 Description-Content-Type: text/markdown
 
 # Speech2Speech
 
-The Speech2Speech Python package **models all phases of speech-to-speech translation**, which include
-- recording speech, 
-- converting speech to text, 
-- translating text to a target language, and 
-- converting the translated text back to speech. 
-
-Each phase of the workflow creates a file, whose name is defined in the config.ini file. Advanced users can start or interrupt the workflow wherever they want by specifying their own files and adapting the config.ini file to refer to them. The user can also launch a specific phase of the workflow by clicking on the corresponding button.
-
-Speech2Speech is designed to be accessible to a **broad audience**, including non-technical users. The package **does not require any specialized software training or user knowledge** and can be used straight out of the box. This makes it incredibly accessible to a wide range of users, including those with visual impairments who can input text by dictating it and have the package read documents aloud.
-
-The package uses PyAudio, Open AI Whisper, Chat-GPT, and Google gttx and can automatically detect the source language used in speech. Users can, therefore, access accurate translations for a **wide range of languages** without having to switch between different translation tools. Although the quality of translation may vary depending on the target language, it is pretty good for popular languages such as English, French, Portuguese, Spanish, German, Dutch and Italian.
+The Speech2Speech Python package is a Streamlit Web application that **models 
+all phases of speech-to-speech translation**, including:
+- recording speech in the source language, 
+- converting the source language speech to source language text, 
+- translating the source language text to target language text, and 
+- converting the translated text to speech in the target language. 
+
+Speech2Speech is currently **configured to translate to and from 13 different 
+languages**. Although the quality of  translation may vary depending on the 
+target language, it is pretty good for popular languages such as English, 
+French, Portuguese, Spanish, German, Dutch and Italian. Speech2Speech **can be 
+configured for many more than just these languages** (specified in the config.
+ini file), as long as they are supported by Whisper AI, Chat-GPT and gtts, 
+the packages on which it depends.
+
+The package **automatically detects the source language used in speech**. The 
+user therefore is not asked to specify it.
+
+Speech2Speech is designed to be accessible to a **broad audience**. One of 
+the key advantages of Speech2Speech is that it's incredibly easy to use. 
+There is **no need to train the software or the user before actually using 
+the product**. It works well straight out of the box with no further tuning 
+or configuration required. This makes it a highly accessible tool that anyone can use, regardless of their technical expertise or experience with speech recognition and machine translation technology.
+
+Each phase of the workflow creates a file, whose name is defined in the 
+config.ini file. Advanced users can **start and/or interrupt the workflow 
+wherever they need** by inserting their own files in the speech2speech/data 
+subdirectory and adapting the config.ini file to refer to them. 
 
 Prerequisites
 -----------------------------------------------------------------------------
 Before using Speech2Speech, you need to sign up for an OpenAI account, create an API key, and set up an environment variable. Here's how to do it:
 
 1. **Signup and Create an OpenAI Account**: Go to the OpenAI website and 
    click on the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
@@ -112,8 +129,9 @@
    Page" button to reset the page.
    
 As indicated above, you can also use just parts of this full workflow by specifying the name(s) of the file(s) you want to use in the config.ini file and by clicking the relevant button of the user interface.
 
 What to do if you encounter issues
 -------------------------------
 
-If Chat-GPT or speech2speech get stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
+If Chat-GPT or Speech2Speech get stuck or you encounter any issues, simply 
+refresh the browser page.
```

