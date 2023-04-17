# Comparing `tmp/chatgpt4-cli-1.4.8.tar.gz` & `tmp/chatgpt4-cli-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.4.8.tar", last modified: Mon Apr 10 11:02:18 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.4.9.tar", last modified: Mon Apr 17 09:35:51 2023, max compression
```

## Comparing `chatgpt4-cli-1.4.8.tar` & `chatgpt4-cli-1.4.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27403 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 11:02:18.000000 chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:02:18.371566 chatgpt4-cli-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-10 11:01:56.000000 chatgpt4-cli-1.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:35:51.614052 chatgpt4-cli-1.4.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:35:51.610719 chatgpt4-cli-1.4.9/GPTCLI/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-04-16 20:57:25.000000 chatgpt4-cli-1.4.9/GPTCLI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/GPTCLI/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2023-04-09 14:37:59.000000 chatgpt4-cli-1.4.9/GPTCLI/addons.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/GPTCLI/emage.py
+-rwxr-xr-x   0 root         (0) root         (0)    27488 2023-04-10 22:33:29.000000 chatgpt4-cli-1.4.9/GPTCLI/gptcli.py
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-04-08 11:57:02.000000 chatgpt4-cli-1.4.9/GPTCLI/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5638 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/GPTCLI/image.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-06 14:49:38.000000 chatgpt4-cli-1.4.9/GPTCLI/test.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13107 2023-04-17 09:35:51.610719 chatgpt4-cli-1.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12063 2023-04-16 20:57:36.000000 chatgpt4-cli-1.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:35:51.610719 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13107 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 09:35:51.614052 chatgpt4-cli-1.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-04-17 09:20:13.000000 chatgpt4-cli-1.4.9/setup.py
```

### Comparing `chatgpt4-cli-1.4.8/GPTCLI/addons.py` & `chatgpt4-cli-1.4.9/GPTCLI/addons.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.8/GPTCLI/emage.py` & `chatgpt4-cli-1.4.9/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.8/GPTCLI/gptcli.py` & `chatgpt4-cli-1.4.9/GPTCLI/gptcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,15 @@
         self.feedback = None
         self.failed_to_record = False
 
     def save_record(self) -> None:
         """Write prompts and responses in a file"""
         info_to_write = f"\n\n{date_stamp(args.prompt_prefix)}{args.message}\n\n{date_stamp(args.response_prefix)}{self.feedback}"
         try:
-            with open(self.filepath, "a") as fp:
+            with open(self.filepath, "a",encoding="utf-8") as fp:
                 fp.write(info_to_write)
         except Exception as e:
             logging.error(f"Failed to keep record - {getExc(e)}")
             self.failed_to_record = True
 
     def main(self, response: str) -> None:
         """Main method"""
@@ -431,30 +431,30 @@
 
         try:
             logging.info("Updating acts and prompts")
 
             for key, value in self.links.items():
                 resp = get(value)
                 if resp.status_code == 200:
-                    with open(path.join(app_dir, key), "w") as fh:
+                    with open(path.join(app_dir, key), "w",encoding="utf-8") as fh:
                         fh.write(resp.text)
                 else:
                     logging.error(
                         f'Failed to get prompts from "{value}" - [{resp.status_code} : {resp.reason}]'
                     )
         except Exception as e:
             logging.error(getExc(e))
 
     def read_contents(
         self, filename: str = None, delimiter: str = ",", resp: dict = {}
     ):
         """Read prompts and return in dict {act:prompt}"""
         import csv
 
-        with open(filename or self.fnm) as fh:
+        with open(filename or self.fnm,encoding="utf-8") as fh:
             for row in csv.DictReader(fh, delimiter=delimiter):
                 resp[row["act"]] = row["prompt"]
         return resp
 
     def display_info(self, resp: dict) -> None:
         """Displays acts and roles"""
         x = 0
@@ -484,15 +484,15 @@
                 for key, value in resp.items():
                     print(
                         f"{config_h.color_dict[args.input_color]}>>[{x}] {key} : {config_h.color_dict[args.output_color]}{value}{Fore.RESET}",
                         end="\n\n",
                     )
                     x += 1
             else:
-                with open(args.dump, "w") as fh:
+                with open(args.dump, "w",encoding="utf-8") as fh:
                     from json import dumps
 
                     data = json.dumps(resp, indent=4)
                     fh.write(data)
                     print(data)
             exit(0)
 
@@ -749,15 +749,15 @@
 
 def get_api_key() -> str:
     """Gets API from Key_path or args.key"""
     if any([args.key, environ.get("OPENAI_API_KEY")]):
         return args.key or environ.get("OPENAI_API_KEY")
     if args.key_path:
         try:
-            with open(args.key_path) as fh:
+            with open(args.key_path,encoding="utf-8") as fh:
                 return fh.readlines()[0]
         except Exception as e:
             exit(logging.critical("While opening Key_Path " + getExc(e)))
 
 
 def intro_train(
     error_msg: str = "Initializing default configurations - Kindly Wait",
```

### Comparing `chatgpt4-cli-1.4.8/GPTCLI/helper.py` & `chatgpt4-cli-1.4.9/GPTCLI/helper.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.8/GPTCLI/image.py` & `chatgpt4-cli-1.4.9/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.8/LICENSE` & `chatgpt4-cli-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.8/PKG-INFO` & `chatgpt4-cli-1.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,11 @@
-Metadata-Version: 2.1
-Name: chatgpt4-cli
-Version: 1.4.8
-Summary: Terminal for ChatGPT
-Home-page: https://github.com/Simatwa/gpt-cli
-Author: Smartwa Caleb
-Author-email: smartwacaleb@gmail.com
-Maintainer: Smartwa Caleb
-License: MIT
-Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.8&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.9&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -192,24 +172,29 @@
  - e.g ```_rollback 2```
 
 10._reset : Reset current chat and start new
  - e.g ```_reset Chat as if you are a 10 year old child```
 
 11._help : Show this help info
 
-* Use double `./` *(fullstop and forward slash)* to interact with **system commands**
-  e.g './ifconfig'
+* Use double `./` *(fullstop and forward slash)* to interact with
+
+**system commands**
+
+  e.g ```./ifconfig```
+
 </details>
 
 <details>
+
 <summary>
 
-  For more info run `gpt-cli -h`.
+For more info run `gpt-cli -h`.
 
-  </summary>
+</summary>
 
 ```
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
@@ -288,27 +273,31 @@
   --zero-show           Specifies not to stdout prompt of the act parsed
   --markdown            Stdout responses in markdown-format - disables
                         streaming
   --update              Download latest prompts - [awesome-chatgpt-prompts]
 
 ```
 
-  </details>
+</details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
 > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
 
 
 ## Motive
 
 <details>
+
 <summary>
+
 Love for `Terminal` ❤️
+
 </summary>
+
 As a `terminal guy` I used to find it uncomfortable to keep shifting from one window to next in order to access ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/Simatwa/gpt-cli)
 </details>
 
 ## Contributions
 
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
```

#### html2text {}

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.8 Summary: Terminal for
-ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
-Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
-Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense) Classifier:
-Intended Audience :: Developers Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
 generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
 assets/Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https:
 //github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
@@ -68,17 +58,17 @@
 cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ
 [Smartwa@ChatGPT4]â(%H:%M:%S)``` 7._load : Load configurations from the json
 file - e.g ```load DAN.json``` 8._save : Save the current Chat Configurations -
 e.g ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) -
 e.g ```_rollback 2``` 10._reset : Reset current chat and start new - e.g
 ```_reset Chat as if you are a 10 year old child``` 11._help : Show this help
 info * Use double `./` *(fullstop and forward slash)* to interact with **system
-commands** e.g './ifconfig'    For more info run `gpt-cli -h`.  ``` usage: gpt-
-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-7000]] [-
-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
+commands** e.g ```./ifconfig```    For more info run `gpt-cli -h`.  ``` usage:
+gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-
+7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
 [-cf path] [--disable-stream] [--new-record] [--disable-recording] [--zero-
 show] [--markdown] [--update] [message ...] Interact with ChatGPT at the
 terminal positional arguments: message Message to be send. optional arguments:
```

### Comparing `chatgpt4-cli-1.4.8/README.md` & `chatgpt4-cli-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,38 @@
+Metadata-Version: 2.1
+Name: chatgpt4-cli
+Version: 1.4.9
+Summary: Terminal for ChatGPT
+Home-page: https://github.com/Simatwa/gpt-cli
+Author: Smartwa Caleb
+Author-email: smartwacaleb@gmail.com
+Maintainer: Smartwa Caleb
+License: MIT
+Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: Free For Home Use
+Classifier: Topic :: Home Automation
+Classifier: Intended Audience :: Customer Service
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.8&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.9&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -172,24 +199,29 @@
  - e.g ```_rollback 2```
 
 10._reset : Reset current chat and start new
  - e.g ```_reset Chat as if you are a 10 year old child```
 
 11._help : Show this help info
 
-* Use double `./` *(fullstop and forward slash)* to interact with **system commands**
-  e.g './ifconfig'
+* Use double `./` *(fullstop and forward slash)* to interact with
+
+**system commands**
+
+  e.g ```./ifconfig```
+
 </details>
 
 <details>
+
 <summary>
 
-  For more info run `gpt-cli -h`.
+For more info run `gpt-cli -h`.
 
-  </summary>
+</summary>
 
 ```
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
@@ -268,27 +300,31 @@
   --zero-show           Specifies not to stdout prompt of the act parsed
   --markdown            Stdout responses in markdown-format - disables
                         streaming
   --update              Download latest prompts - [awesome-chatgpt-prompts]
 
 ```
 
-  </details>
+</details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
 > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
 
 
 ## Motive
 
 <details>
+
 <summary>
+
 Love for `Terminal` ❤️
+
 </summary>
+
 As a `terminal guy` I used to find it uncomfortable to keep shifting from one window to next in order to access ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/Simatwa/gpt-cli)
 </details>
 
 ## Contributions
 
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
```

#### html2text {}

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.9 Summary: Terminal for
+ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
+Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
+Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
+Classifier: License :: OSI Approved :: MIT License Classifier: Development
+Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: License :: Free For Home Use
+Classifier: Topic :: Home Automation Classifier: Intended Audience :: Customer
+Service Classifier: Programming Language :: Python Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
 generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
 assets/Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https:
 //github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
@@ -58,17 +72,17 @@
 cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ
 [Smartwa@ChatGPT4]â(%H:%M:%S)``` 7._load : Load configurations from the json
 file - e.g ```load DAN.json``` 8._save : Save the current Chat Configurations -
 e.g ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) -
 e.g ```_rollback 2``` 10._reset : Reset current chat and start new - e.g
 ```_reset Chat as if you are a 10 year old child``` 11._help : Show this help
 info * Use double `./` *(fullstop and forward slash)* to interact with **system
-commands** e.g './ifconfig'    For more info run `gpt-cli -h`.  ``` usage: gpt-
-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-7000]] [-
-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
+commands** e.g ```./ifconfig```    For more info run `gpt-cli -h`.  ``` usage:
+gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-
+7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
 [-cf path] [--disable-stream] [--new-record] [--disable-recording] [--zero-
 show] [--markdown] [--update] [message ...] Interact with ChatGPT at the
 terminal positional arguments: message Message to be send. optional arguments:
```

### Comparing `chatgpt4-cli-1.4.8/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.4.8
+Version: 1.4.9
 Summary: Terminal for ChatGPT
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: Free For Home Use
+Classifier: Topic :: Home Automation
+Classifier: Intended Audience :: Customer Service
+Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.8&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.4.9&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -192,24 +199,29 @@
  - e.g ```_rollback 2```
 
 10._reset : Reset current chat and start new
  - e.g ```_reset Chat as if you are a 10 year old child```
 
 11._help : Show this help info
 
-* Use double `./` *(fullstop and forward slash)* to interact with **system commands**
-  e.g './ifconfig'
+* Use double `./` *(fullstop and forward slash)* to interact with
+
+**system commands**
+
+  e.g ```./ifconfig```
+
 </details>
 
 <details>
+
 <summary>
 
-  For more info run `gpt-cli -h`.
+For more info run `gpt-cli -h`.
 
-  </summary>
+</summary>
 
 ```
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
@@ -288,27 +300,31 @@
   --zero-show           Specifies not to stdout prompt of the act parsed
   --markdown            Stdout responses in markdown-format - disables
                         streaming
   --update              Download latest prompts - [awesome-chatgpt-prompts]
 
 ```
 
-  </details>
+</details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
 > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
 
 
 ## Motive
 
 <details>
+
 <summary>
+
 Love for `Terminal` ❤️
+
 </summary>
+
 As a `terminal guy` I used to find it uncomfortable to keep shifting from one window to next in order to access ChatGPT even after trying out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/Simatwa/gpt-cli)
 </details>
 
 ## Contributions
 
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
```

#### html2text {}

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.8 Summary: Terminal for
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.9 Summary: Terminal for
 ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense) Classifier:
-Intended Audience :: Developers Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Classifier: License :: OSI Approved :: MIT License Classifier: Development
+Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: License :: Free For Home Use
+Classifier: Topic :: Home Automation Classifier: Intended Audience :: Customer
+Service Classifier: Programming Language :: Python Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
 generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
@@ -68,17 +72,17 @@
 cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ
 [Smartwa@ChatGPT4]â(%H:%M:%S)``` 7._load : Load configurations from the json
 file - e.g ```load DAN.json``` 8._save : Save the current Chat Configurations -
 e.g ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) -
 e.g ```_rollback 2``` 10._reset : Reset current chat and start new - e.g
 ```_reset Chat as if you are a 10 year old child``` 11._help : Show this help
 info * Use double `./` *(fullstop and forward slash)* to interact with **system
-commands** e.g './ifconfig'    For more info run `gpt-cli -h`.  ``` usage: gpt-
-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-7000]] [-
-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
+commands** e.g ```./ifconfig```    For more info run `gpt-cli -h`.  ``` usage:
+gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-
+7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
 [-cf path] [--disable-stream] [--new-record] [--disable-recording] [--zero-
 show] [--markdown] [--update] [message ...] Interact with ChatGPT at the
 terminal positional arguments: message Message to be send. optional arguments:
```

