# Comparing `tmp/sozlukpy-0.0.6.tar.gz` & `tmp/sozlukpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sozlukpy-0.0.6.tar", last modified: Sat Dec  3 17:14:11 2022, max compression
+gzip compressed data, was "sozlukpy-0.0.7.tar", last modified: Mon Apr 17 19:39:33 2023, max compression
```

## Comparing `sozlukpy-0.0.6.tar` & `sozlukpy-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-12-03 17:14:11.696589 sozlukpy-0.0.6/
--rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 sozlukpy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2396 2022-12-03 17:14:11.695582 sozlukpy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1916 2022-12-03 17:13:50.000000 sozlukpy-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2022-12-03 17:14:11.697596 sozlukpy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      651 2022-12-03 17:08:19.000000 sozlukpy-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-03 17:14:11.683526 sozlukpy-0.0.6/sozlukpy/
--rw-rw-rw-   0        0        0     2309 2022-12-03 17:07:47.000000 sozlukpy-0.0.6/sozlukpy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-03 17:14:11.693464 sozlukpy-0.0.6/sozlukpy.egg-info/
--rw-rw-rw-   0        0        0     2396 2022-12-03 17:14:11.000000 sozlukpy-0.0.6/sozlukpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2022-12-03 17:14:11.000000 sozlukpy-0.0.6/sozlukpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-03 17:14:11.000000 sozlukpy-0.0.6/sozlukpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-12-03 17:14:11.000000 sozlukpy-0.0.6/sozlukpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 19:39:33.075987 sozlukpy-0.0.7/
+-rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 sozlukpy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2492 2023-04-17 19:39:33.074983 sozlukpy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1980 2023-04-17 19:35:54.000000 sozlukpy-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 19:39:33.075987 sozlukpy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-04-17 19:39:27.000000 sozlukpy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:39:33.063544 sozlukpy-0.0.7/sozlukpy/
+-rw-rw-rw-   0        0        0     2172 2023-04-17 19:30:08.000000 sozlukpy-0.0.7/sozlukpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:39:33.073977 sozlukpy-0.0.7/sozlukpy.egg-info/
+-rw-rw-rw-   0        0        0     2492 2023-04-17 19:39:32.000000 sozlukpy-0.0.7/sozlukpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-17 19:39:32.000000 sozlukpy-0.0.7/sozlukpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 19:39:32.000000 sozlukpy-0.0.7/sozlukpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 19:39:32.000000 sozlukpy-0.0.7/sozlukpy.egg-info/top_level.txt
```

### Comparing `sozlukpy-0.0.6/LICENSE` & `sozlukpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sozlukpy-0.0.6/PKG-INFO` & `sozlukpy-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sozlukpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A basic Turkish dictionary
-Home-page: 
+Home-page: https://gihtub.com/Meinos10/sozlukpy
 Author: Emre
 Author-email: E.tmen2023@gmail.com
 License: MIT
 Keywords: sozlukpy,sozlukpython,sozluk,sozluk-python,sozluk-py
 Requires: requests
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sozlukpy
+# [sozlukpy](https://pypi.org/project/sozlukpy/)
 
 A basic Turkish dictionary
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
@@ -37,49 +37,49 @@
 """
 Bir milletin, belli bir topluluÄŸun veya bir kuruluÅŸun simgesi olarak kullanÄ±lan, renk ve biÃ§imle Ã¶zelleÅŸtirilmiÅŸ, genellikle dikdÃ¶rtgen biÃ§iminde kumaÅŸ, sancak
 """
 
 # returns 'anlamlar'
 sozluk.anlamlar(kelime)
 """
-BAYRAK
-
-1 - Bir milletin, belli bir topluluÄŸun veya bir kuruluÅŸun simgesi olarak kullanÄ±lan, renk ve biÃ§imle Ã¶zelleÅŸtirilmiÅŸ, genellikle dikdÃ¶rtgen biÃ§iminde kumaÅŸ, sancak
-2 - Ã–ncÃ¼
-3 - Simge, sembol
-4 - Baklagilllerde diÄŸerlerinden daha Ã¼stte bulunan, daha bÃ¼yÃ¼k olan ve Ã§oÄŸunlukla baÅŸka bir renkte ve yuvarlakÃ§a olan taÃ§ yapraÄŸÄ±
-5 - Atletizmdeki bayrak yarÄ±ÅŸÄ±nda dÃ¶rt sporcunun elden ele geÃ§irdiÄŸi kÄ±sa, yuvarlak sopa
-6 - GerektiÄŸinde indirilip kaldÄ±rÄ±lan, aÃ§Ä±lÄ±p kapatÄ±lan kol
+{
+    '1': 'Bir milletin, belli bir topluluÄŸun veya bir kuruluÅŸun simgesi olarak kullanÄ±lan, renk ve biÃ§imle Ã¶zelleÅŸtirilmiÅŸ, genellikle dikdÃ¶rtgen biÃ§iminde kumaÅŸ, sancak', 
+    '2': 'Ã–ncÃ¼', 
+    '3': 'Simge, sembol', 
+    '4': 'Baklagilllerde diÄŸerlerinden daha Ã¼stte bulunan, daha bÃ¼yÃ¼k olan ve Ã§oÄŸunlukla baÅŸka bir renkte ve yuvarlakÃ§a olan taÃ§ yapraÄŸÄ±', 
+    '5': 'Atletizmdeki bayrak yarÄ±ÅŸÄ±nda dÃ¶rt sporcunun elden ele geÃ§irdiÄŸi kÄ±sa, yuvarlak sopa', 
+    '6': 'GerektiÄŸinde indirilip kaldÄ±rÄ±lan, aÃ§Ä±lÄ±p kapatÄ±lan kol'
+}
 """
 
 # returns 'ornekler'
 sozluk.ornekler(kelime)
 """
-BAYRAK
-
-- BayraklarÄ± bayrak yapan Ã¼stÃ¼ndeki kandÄ±r / Toprak eÄŸer uÄŸrunda Ã¶len varsa vatandÄ±r | Mithat Cemal Kuntay
-- Yeni bir sanat kuÅŸaÄŸÄ±nÄ±n bayraÄŸÄ±ydÄ± o. | Yusuf Ziya OrtaÃ§
-- KÄ±z, Sinekli Bakkal'Ä±n erkek dÃ¼nyasÄ±na meydan okuyan bir bayrak gibiydi. | Halide Edip AdÄ±var
-- Yoldan, bayraÄŸÄ± aÃ§Ä±k bir taksi Ã§evirdiler. | Mahmut Yesari
+{
+    '1': 'BayraklarÄ± bayrak yapan Ã¼stÃ¼ndeki kandÄ±r / Toprak eÄŸer uÄŸrunda Ã¶len varsa vatandÄ±r', 
+    '2': 'Yeni bir sanat kuÅŸaÄŸÄ±nÄ±n bayraÄŸÄ±ydÄ± o.', 
+    '3': "KÄ±z, Sinekli Bakkal'Ä±n erkek dÃ¼nyasÄ±na meydan okuyan bir bayrak gibiydi.", 
+    '4': 'Yoldan, bayraÄŸÄ± aÃ§Ä±k bir taksi Ã§evirdiler.'
+}
 """
 
 # returns 'atasozleri'
 sozluk.atasozleri(kelime)
 """
-BAYRAK
-
-1 - bayraÄŸÄ± yarÄ±ya indirmek
-2 - bayrak aÃ§mak
-3 - bayrak Ã§ekmek (veya asmak)
-4 - bayrak dikmek
-5 - bayrak gibi
-6 - bayraklarÄ± aÃ§mak
+{
+    '1': 'bayraÄŸÄ± yarÄ±ya indirmek', 
+    '2': 'bayrak aÃ§mak', 
+    '3': 'bayrak Ã§ekmek (veya asmak)', 
+    '4': 'bayrak dikmek', 
+    '5': 'bayrak gibi', 
+    '6': 'bayraklarÄ± aÃ§mak'
+}
 """
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
-[Telegram](https://t.me/ReWoxi) - [Github](https://github.com/Meinos10) - Discord: ```emree#0010```
+[Telegram](https://t.me/ReWoxi) - [Github](https://github.com/Meinos10)
```

### Comparing `sozlukpy-0.0.6/README.md` & `sozlukpy-0.0.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# sozlukpy
+# [sozlukpy](https://pypi.org/project/sozlukpy/)
 
 A basic Turkish dictionary
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
@@ -24,49 +24,49 @@
 """
 Bir milletin, belli bir topluluğun veya bir kuruluşun simgesi olarak kullanılan, renk ve biçimle özelleştirilmiş, genellikle dikdörtgen biçiminde kumaş, sancak
 """
 
 # returns 'anlamlar'
 sozluk.anlamlar(kelime)
 """
-BAYRAK
-
-1 - Bir milletin, belli bir topluluğun veya bir kuruluşun simgesi olarak kullanılan, renk ve biçimle özelleştirilmiş, genellikle dikdörtgen biçiminde kumaş, sancak
-2 - Öncü
-3 - Simge, sembol
-4 - Baklagilllerde diğerlerinden daha üstte bulunan, daha büyük olan ve çoğunlukla başka bir renkte ve yuvarlakça olan taç yaprağı
-5 - Atletizmdeki bayrak yarışında dört sporcunun elden ele geçirdiği kısa, yuvarlak sopa
-6 - Gerektiğinde indirilip kaldırılan, açılıp kapatılan kol
+{
+    '1': 'Bir milletin, belli bir topluluğun veya bir kuruluşun simgesi olarak kullanılan, renk ve biçimle özelleştirilmiş, genellikle dikdörtgen biçiminde kumaş, sancak', 
+    '2': 'Öncü', 
+    '3': 'Simge, sembol', 
+    '4': 'Baklagilllerde diğerlerinden daha üstte bulunan, daha büyük olan ve çoğunlukla başka bir renkte ve yuvarlakça olan taç yaprağı', 
+    '5': 'Atletizmdeki bayrak yarışında dört sporcunun elden ele geçirdiği kısa, yuvarlak sopa', 
+    '6': 'Gerektiğinde indirilip kaldırılan, açılıp kapatılan kol'
+}
 """
 
 # returns 'ornekler'
 sozluk.ornekler(kelime)
 """
-BAYRAK
-
-- Bayrakları bayrak yapan üstündeki kandır / Toprak eğer uğrunda ölen varsa vatandır | Mithat Cemal Kuntay
-- Yeni bir sanat kuşağının bayrağıydı o. | Yusuf Ziya Ortaç
-- Kız, Sinekli Bakkal'ın erkek dünyasına meydan okuyan bir bayrak gibiydi. | Halide Edip Adıvar
-- Yoldan, bayrağı açık bir taksi çevirdiler. | Mahmut Yesari
+{
+    '1': 'Bayrakları bayrak yapan üstündeki kandır / Toprak eğer uğrunda ölen varsa vatandır', 
+    '2': 'Yeni bir sanat kuşağının bayrağıydı o.', 
+    '3': "Kız, Sinekli Bakkal'ın erkek dünyasına meydan okuyan bir bayrak gibiydi.", 
+    '4': 'Yoldan, bayrağı açık bir taksi çevirdiler.'
+}
 """
 
 # returns 'atasozleri'
 sozluk.atasozleri(kelime)
 """
-BAYRAK
-
-1 - bayrağı yarıya indirmek
-2 - bayrak açmak
-3 - bayrak çekmek (veya asmak)
-4 - bayrak dikmek
-5 - bayrak gibi
-6 - bayrakları açmak
+{
+    '1': 'bayrağı yarıya indirmek', 
+    '2': 'bayrak açmak', 
+    '3': 'bayrak çekmek (veya asmak)', 
+    '4': 'bayrak dikmek', 
+    '5': 'bayrak gibi', 
+    '6': 'bayrakları açmak'
+}
 """
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
-[Telegram](https://t.me/ReWoxi) - [Github](https://github.com/Meinos10) - Discord: ```emree#0010```
+[Telegram](https://t.me/ReWoxi) - [Github](https://github.com/Meinos10)
```

### Comparing `sozlukpy-0.0.6/setup.py` & `sozlukpy-0.0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sozlukpy",
-    version="0.0.6",
+    version="0.0.7",
     description="A basic Turkish dictionary",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="",
+    url="https://gihtub.com/Meinos10/sozlukpy",
     author="Emre",
     author_email="E.tmen2023@gmail.com",
     license="MIT",
     #classifiers = [
     #"Programming Language :: Python :: 3",
     #"License :: OSI Approved :: MIT License",
     #"Operating System :: OS Independent",
```

### Comparing `sozlukpy-0.0.6/sozlukpy.egg-info/PKG-INFO` & `sozlukpy-0.0.7/sozlukpy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sozlukpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: A basic Turkish dictionary
-Home-page: 
+Home-page: https://gihtub.com/Meinos10/sozlukpy
 Author: Emre
 Author-email: E.tmen2023@gmail.com
 License: MIT
 Keywords: sozlukpy,sozlukpython,sozluk,sozluk-python,sozluk-py
 Requires: requests
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# sozlukpy
+# [sozlukpy](https://pypi.org/project/sozlukpy/)
 
 A basic Turkish dictionary
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
@@ -37,49 +37,49 @@
 """
 Bir milletin, belli bir topluluÄŸun veya bir kuruluÅŸun simgesi olarak kullanÄ±lan, renk ve biÃ§imle Ã¶zelleÅŸtirilmiÅŸ, genellikle dikdÃ¶rtgen biÃ§iminde kumaÅŸ, sancak
 """
 
 # returns 'anlamlar'
 sozluk.anlamlar(kelime)
 """
-BAYRAK
-
-1 - Bir milletin, belli bir topluluÄŸun veya bir kuruluÅŸun simgesi olarak kullanÄ±lan, renk ve biÃ§imle Ã¶zelleÅŸtirilmiÅŸ, genellikle dikdÃ¶rtgen biÃ§iminde kumaÅŸ, sancak
-2 - Ã–ncÃ¼
-3 - Simge, sembol
-4 - Baklagilllerde diÄŸerlerinden daha Ã¼stte bulunan, daha bÃ¼yÃ¼k olan ve Ã§oÄŸunlukla baÅŸka bir renkte ve yuvarlakÃ§a olan taÃ§ yapraÄŸÄ±
-5 - Atletizmdeki bayrak yarÄ±ÅŸÄ±nda dÃ¶rt sporcunun elden ele geÃ§irdiÄŸi kÄ±sa, yuvarlak sopa
-6 - GerektiÄŸinde indirilip kaldÄ±rÄ±lan, aÃ§Ä±lÄ±p kapatÄ±lan kol
+{
+    '1': 'Bir milletin, belli bir topluluÄŸun veya bir kuruluÅŸun simgesi olarak kullanÄ±lan, renk ve biÃ§imle Ã¶zelleÅŸtirilmiÅŸ, genellikle dikdÃ¶rtgen biÃ§iminde kumaÅŸ, sancak', 
+    '2': 'Ã–ncÃ¼', 
+    '3': 'Simge, sembol', 
+    '4': 'Baklagilllerde diÄŸerlerinden daha Ã¼stte bulunan, daha bÃ¼yÃ¼k olan ve Ã§oÄŸunlukla baÅŸka bir renkte ve yuvarlakÃ§a olan taÃ§ yapraÄŸÄ±', 
+    '5': 'Atletizmdeki bayrak yarÄ±ÅŸÄ±nda dÃ¶rt sporcunun elden ele geÃ§irdiÄŸi kÄ±sa, yuvarlak sopa', 
+    '6': 'GerektiÄŸinde indirilip kaldÄ±rÄ±lan, aÃ§Ä±lÄ±p kapatÄ±lan kol'
+}
 """
 
 # returns 'ornekler'
 sozluk.ornekler(kelime)
 """
-BAYRAK
-
-- BayraklarÄ± bayrak yapan Ã¼stÃ¼ndeki kandÄ±r / Toprak eÄŸer uÄŸrunda Ã¶len varsa vatandÄ±r | Mithat Cemal Kuntay
-- Yeni bir sanat kuÅŸaÄŸÄ±nÄ±n bayraÄŸÄ±ydÄ± o. | Yusuf Ziya OrtaÃ§
-- KÄ±z, Sinekli Bakkal'Ä±n erkek dÃ¼nyasÄ±na meydan okuyan bir bayrak gibiydi. | Halide Edip AdÄ±var
-- Yoldan, bayraÄŸÄ± aÃ§Ä±k bir taksi Ã§evirdiler. | Mahmut Yesari
+{
+    '1': 'BayraklarÄ± bayrak yapan Ã¼stÃ¼ndeki kandÄ±r / Toprak eÄŸer uÄŸrunda Ã¶len varsa vatandÄ±r', 
+    '2': 'Yeni bir sanat kuÅŸaÄŸÄ±nÄ±n bayraÄŸÄ±ydÄ± o.', 
+    '3': "KÄ±z, Sinekli Bakkal'Ä±n erkek dÃ¼nyasÄ±na meydan okuyan bir bayrak gibiydi.", 
+    '4': 'Yoldan, bayraÄŸÄ± aÃ§Ä±k bir taksi Ã§evirdiler.'
+}
 """
 
 # returns 'atasozleri'
 sozluk.atasozleri(kelime)
 """
-BAYRAK
-
-1 - bayraÄŸÄ± yarÄ±ya indirmek
-2 - bayrak aÃ§mak
-3 - bayrak Ã§ekmek (veya asmak)
-4 - bayrak dikmek
-5 - bayrak gibi
-6 - bayraklarÄ± aÃ§mak
+{
+    '1': 'bayraÄŸÄ± yarÄ±ya indirmek', 
+    '2': 'bayrak aÃ§mak', 
+    '3': 'bayrak Ã§ekmek (veya asmak)', 
+    '4': 'bayrak dikmek', 
+    '5': 'bayrak gibi', 
+    '6': 'bayraklarÄ± aÃ§mak'
+}
 """
 ```
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
-[Telegram](https://t.me/ReWoxi) - [Github](https://github.com/Meinos10) - Discord: ```emree#0010```
+[Telegram](https://t.me/ReWoxi) - [Github](https://github.com/Meinos10)
```

