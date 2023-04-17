# Comparing `tmp/Askpyro-1.72.tar.gz` & `tmp/Askpyro-1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Askpyro-1.72.tar", last modified: Mon Apr 17 06:08:00 2023, max compression
+gzip compressed data, was "Askpyro-1.73.tar", last modified: Mon Apr 17 14:50:05 2023, max compression
```

## Comparing `Askpyro-1.72.tar` & `Askpyro-1.73.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.071849 Askpyro-1.72/Askpyro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 06:07:59.000000 Askpyro-1.72/Askpyro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2023-04-17 06:08:00.000000 Askpyro-1.72/Askpyro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 06:07:59.000000 Askpyro-1.72/Askpyro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 06:07:59.000000 Askpyro-1.72/Askpyro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 06:07:36.000000 Askpyro-1.72/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 06:08:00.075849 Askpyro-1.72/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1933 2023-04-17 06:07:36.000000 Askpyro-1.72/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/askpyro/
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5553 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/conversation.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/askpyro/helpers/
--rw-r--r--   0 root         (0) root         (0)      814 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-04-17 06:07:36.000000 Askpyro-1.72/askpyro/helpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 06:08:00.075849 Askpyro-1.72/examples/
--rw-r--r--   0 root         (0) root         (0)      161 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/buttons.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/callback.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/filters.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-04-17 06:07:36.000000 Askpyro-1.72/examples/start.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 06:08:00.075849 Askpyro-1.72/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2963 2023-04-17 06:07:36.000000 Askpyro-1.72/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:50:05.073070 Askpyro-1.73/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:50:05.069070 Askpyro-1.73/Askpyro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-04-17 14:50:05.000000 Askpyro-1.73/Askpyro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-04-17 14:50:05.000000 Askpyro-1.73/Askpyro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:50:05.000000 Askpyro-1.73/Askpyro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:50:05.000000 Askpyro-1.73/Askpyro.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-17 14:50:05.000000 Askpyro-1.73/Askpyro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 14:50:05.000000 Askpyro-1.73/Askpyro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 14:49:34.000000 Askpyro-1.73/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-04-17 14:50:05.073070 Askpyro-1.73/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-04-17 14:49:34.000000 Askpyro-1.73/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:50:05.069070 Askpyro-1.73/askpyro/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-17 14:49:34.000000 Askpyro-1.73/askpyro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5553 2023-04-17 14:49:34.000000 Askpyro-1.73/askpyro/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-04-17 14:49:34.000000 Askpyro-1.73/askpyro/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:50:05.073070 Askpyro-1.73/askpyro/helpers/
+-rw-r--r--   0 root         (0) root         (0)      893 2023-04-17 14:49:34.000000 Askpyro-1.73/askpyro/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-04-17 14:49:34.000000 Askpyro-1.73/askpyro/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-17 14:49:34.000000 Askpyro-1.73/askpyro/helpers/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:50:05.073070 Askpyro-1.73/examples/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-04-17 14:49:34.000000 Askpyro-1.73/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-17 14:49:34.000000 Askpyro-1.73/examples/buttons.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 14:49:34.000000 Askpyro-1.73/examples/callback.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 14:49:34.000000 Askpyro-1.73/examples/filters.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-17 14:49:34.000000 Askpyro-1.73/examples/start.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 14:50:05.073070 Askpyro-1.73/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-04-17 14:49:34.000000 Askpyro-1.73/setup.py
```

### Comparing `Askpyro-1.72/Askpyro.egg-info/PKG-INFO` & `Askpyro-1.73/Askpyro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.72
+Version: 1.73
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
@@ -44,28 +44,28 @@
 ```python
   from askpyro import Askclient
   from pyrogram import Client ,filters
   
   app = Client("my_account")
   read = Askclient(app)
 
-  @app.on_message(filters.command("starr"))
+  @app.on_message(filters.command("start"))
   async def start_pm(c: app, m: Message):
     answer = await read.ask(m, text)
     if answer.text:
      print(answer.text)
     await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
 
   app.run()
 ```
 
 
 ### ɪɴsᴛᴀʟʟɪɴɢ
 
-``` bash
+```python
 pip3 install askpyro
 ```
 
 <details>
 <summary><h3>
 - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ </b>
 </h3></summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.72 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.73 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
 telegram chat messenger mtproto api client library python Platform: UNKNOWN
@@ -22,18 +22,18 @@
 Libraries Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ## á´sá´-á´ÊÊá´ > sá´á´Êá´ á´sá´-
 á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
 ```python from askpyro import Askclient from pyrogram import Client ,filters
 app = Client("my_account") read = Askclient(app) @app.on_message
-(filters.command("starr")) async def start_pm(c: app, m: Message): answer =
+(filters.command("start")) async def start_pm(c: app, m: Message): answer =
 await read.ask(m, text) if answer.text: print(answer.text) await answer.reply
-("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ ```
-bash pip3 install askpyro ```
+("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢
+```python pip3 install askpyro ```
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-90302f?logo=github]
 **** - á´xá´á´á´Êá´ ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-90302f?logo=github]
 **** - á´á´Êá´É¢Êá´á´ É¢Êá´á´á´ ****
 [https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-
 badge&logo=Telegram]
```

### Comparing `Askpyro-1.72/LICENSE` & `Askpyro-1.73/LICENSE`

 * *Files identical despite different names*

### Comparing `Askpyro-1.72/PKG-INFO` & `Askpyro-1.73/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.72
+Version: 1.73
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
@@ -44,28 +44,28 @@
 ```python
   from askpyro import Askclient
   from pyrogram import Client ,filters
   
   app = Client("my_account")
   read = Askclient(app)
 
-  @app.on_message(filters.command("starr"))
+  @app.on_message(filters.command("start"))
   async def start_pm(c: app, m: Message):
     answer = await read.ask(m, text)
     if answer.text:
      print(answer.text)
     await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
 
   app.run()
 ```
 
 
 ### ɪɴsᴛᴀʟʟɪɴɢ
 
-``` bash
+```python
 pip3 install askpyro
 ```
 
 <details>
 <summary><h3>
 - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ </b>
 </h3></summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.72 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.73 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
 URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
 telegram chat messenger mtproto api client library python Platform: UNKNOWN
@@ -22,18 +22,18 @@
 Libraries Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ## á´sá´-á´ÊÊá´ > sá´á´Êá´ á´sá´-
 á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
 ```python from askpyro import Askclient from pyrogram import Client ,filters
 app = Client("my_account") read = Askclient(app) @app.on_message
-(filters.command("starr")) async def start_pm(c: app, m: Message): answer =
+(filters.command("start")) async def start_pm(c: app, m: Message): answer =
 await read.ask(m, text) if answer.text: print(answer.text) await answer.reply
-("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ ```
-bash pip3 install askpyro ```
+("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢
+```python pip3 install askpyro ```
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-90302f?logo=github]
 **** - á´xá´á´á´Êá´ ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-90302f?logo=github]
 **** - á´á´Êá´É¢Êá´á´ É¢Êá´á´á´ ****
 [https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-
 badge&logo=Telegram]
```

### Comparing `Askpyro-1.72/README.md` & `Askpyro-1.73/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 ```python
   from askpyro import Askclient
   from pyrogram import Client ,filters
   
   app = Client("my_account")
   read = Askclient(app)
 
-  @app.on_message(filters.command("starr"))
+  @app.on_message(filters.command("start"))
   async def start_pm(c: app, m: Message):
     answer = await read.ask(m, text)
     if answer.text:
      print(answer.text)
     await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
 
   app.run()
 ```
 
 
 ### ɪɴsᴛᴀʟʟɪɴɢ
 
-``` bash
+```python
 pip3 install askpyro
 ```
 
 <details>
 <summary><h3>
 - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ </b>
 </h3></summary>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 ## á´sá´-á´ÊÊá´ > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê
 @á´á´á´[á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] ```python from askpyro import
 Askclient from pyrogram import Client ,filters app = Client("my_account") read
-= Askclient(app) @app.on_message(filters.command("starr")) async def start_pm
+= Askclient(app) @app.on_message(filters.command("start")) async def start_pm
 (c: app, m: Message): answer = await read.ask(m, text) if answer.text: print
 (answer.text) await answer.reply("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ```
-### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ ``` bash pip3 install askpyro ```
+### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ ```python pip3 install askpyro ```
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-90302f?logo=github]
 **** - á´xá´á´á´Êá´ ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-90302f?logo=github]
 **** - á´á´Êá´É¢Êá´á´ É¢Êá´á´á´ ****
 [https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-
 badge&logo=Telegram]
```

### Comparing `Askpyro-1.72/askpyro/conversation.py` & `Askpyro-1.73/askpyro/conversation.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.72/askpyro/errors.py` & `Askpyro-1.73/askpyro/errors.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.72/askpyro/helpers/__init__.py` & `Askpyro-1.73/askpyro/helpers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 GNU General Public License for more details.
 You should have received a copy of the GNU General Public License.
 
 along with Askpyro.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from .helpers import ikb, bki, ntb, btn, kb, kbtn, array_chunk, force_reply, ikb2
+from .parser import cleanhtml, escape_markdown, mention_html, mention_markdown
```

### Comparing `Askpyro-1.72/askpyro/helpers/helpers.py` & `Askpyro-1.73/askpyro/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.72/examples/buttons.py` & `Askpyro-1.73/examples/buttons.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.72/setup.py` & `Askpyro-1.73/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Askpyro.  If not, see <http://www.gnu.org/licenses/>.
 
 import re
 from sys import argv
 import setuptools
-from setuptools import setup, find_packages
 
 
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
-
+    
+def read(file: str) -> list:
+    with open(file, encoding="utf-8") as r:
+        return [i.strip() for i in r]
 
 
 setuptools.setup(
     name="Askpyro",
     packages=setuptools.find_packages(),
-    version="1.72",
+    version="1.73",
     description="Easy conversation handler for pyrogram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Askpyro/releases/latest",
     author="Abishnoi",
     author_email="abishnoi@askpyro.org",
@@ -67,8 +69,10 @@
     project_urls={
         "Tracker": "https://github.com/Abishnoi69/Askpyro/issues",
         "Community": "https://t.me/AbishnoiMF",
         "Source": "https://github.com/Abishnoi69/Askpyro",
         "Documentation": "https://github.com/Abishnoi69/askpyro/wiki",
     },
     python_requires="~=3.7",
+    zip_safe=False,
+    install_requires=read("requirements.txt")
 )
```

