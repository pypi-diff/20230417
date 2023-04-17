# Comparing `tmp/iso3166-2-0.0.1.tar.gz` & `tmp/iso3166-2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-2-0.0.1.tar", last modified: Sat Jan 14 13:06:01 2023, max compression
+gzip compressed data, was "iso3166-2-1.0.0.tar", last modified: Mon Apr 17 08:56:26 2023, max compression
```

## Comparing `iso3166-2-0.0.1.tar` & `iso3166-2-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 adammckenna   (501) staff       (20)        0 2023-01-14 13:06:01.354011 iso3166-2-0.0.1/
--rw-r--r--   0 adammckenna   (501) staff       (20)     1059 2022-10-29 15:38:39.000000 iso3166-2-0.0.1/LICENSE
--rw-r--r--   0 adammckenna   (501) staff       (20)    10283 2023-01-14 13:06:01.354221 iso3166-2-0.0.1/PKG-INFO
--rw-r--r--   0 adammckenna   (501) staff       (20)     8615 2023-01-10 20:25:04.000000 iso3166-2-0.0.1/README.md
-drwxr-xr-x   0 adammckenna   (501) staff       (20)        0 2023-01-14 13:06:01.351708 iso3166-2-0.0.1/iso3166_2/
--rw-r--r--   0 adammckenna   (501) staff       (20)      132 2023-01-07 16:37:11.000000 iso3166-2-0.0.1/iso3166_2/__init__.py
--rw-r--r--   0 adammckenna   (501) staff       (20)     6229 2023-01-09 16:42:53.000000 iso3166-2-0.0.1/iso3166_2/iso3166_2.py
-drwxr-xr-x   0 adammckenna   (501) staff       (20)        0 2023-01-14 13:06:01.353262 iso3166-2-0.0.1/iso3166_2.egg-info/
--rw-r--r--   0 adammckenna   (501) staff       (20)    10283 2023-01-14 13:06:01.000000 iso3166-2-0.0.1/iso3166_2.egg-info/PKG-INFO
--rw-r--r--   0 adammckenna   (501) staff       (20)      318 2023-01-14 13:06:01.000000 iso3166-2-0.0.1/iso3166_2.egg-info/SOURCES.txt
--rw-r--r--   0 adammckenna   (501) staff       (20)        1 2023-01-14 13:06:01.000000 iso3166-2-0.0.1/iso3166_2.egg-info/dependency_links.txt
--rw-r--r--   0 adammckenna   (501) staff       (20)        1 2023-01-14 13:06:01.000000 iso3166-2-0.0.1/iso3166_2.egg-info/not-zip-safe
--rw-r--r--   0 adammckenna   (501) staff       (20)      105 2023-01-14 13:06:01.000000 iso3166-2-0.0.1/iso3166_2.egg-info/requires.txt
--rw-r--r--   0 adammckenna   (501) staff       (20)       16 2023-01-14 13:06:01.000000 iso3166-2-0.0.1/iso3166_2.egg-info/top_level.txt
--rw-r--r--   0 adammckenna   (501) staff       (20)     1754 2023-01-14 13:06:01.355082 iso3166-2-0.0.1/setup.cfg
--rw-r--r--   0 adammckenna   (501) staff       (20)     2845 2023-01-08 22:11:50.000000 iso3166-2-0.0.1/setup.py
-drwxr-xr-x   0 adammckenna   (501) staff       (20)        0 2023-01-14 13:06:01.353782 iso3166-2-0.0.1/tests/
--rw-r--r--   0 adammckenna   (501) staff       (20)        0 2022-11-13 20:13:04.000000 iso3166-2-0.0.1/tests/__init__.py
--rw-r--r--   0 adammckenna   (501) staff       (20)    10231 2023-01-09 20:09:57.000000 iso3166-2-0.0.1/tests/test_iso31662.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.056643 iso3166-2-1.0.0/iso3166_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.056643 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1089432 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/iso3166-2-min.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2787107 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166-2-data/iso3166-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/iso3166_2/iso3166_2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.056643 iso3166-2-1.0.0/iso3166_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 08:56:26.000000 iso3166-2-1.0.0/iso3166_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 08:56:25.000000 iso3166-2-1.0.0/iso3166_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:26.060643 iso3166-2-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-04-17 08:56:09.000000 iso3166-2-1.0.0/tests/test_iso3166_2.py
```

### Comparing `iso3166-2-0.0.1/LICENSE` & `iso3166-2-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-2-0.0.1/PKG-INFO` & `iso3166-2-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,46 @@
-Metadata-Version: 2.1
-Name: iso3166-2
-Version: 0.0.1
-Summary: A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
-Home-page: https://github.com/amckenna41/iso3166-2
-Author: AJ McKenna, https://github.com/amckenna41
-Author-email: amckenna41@qub.ac.uk
-Maintainer: AJ McKenna
-License: MIT
-Download-URL: https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,iso3166-2,iso3166-1,alpha2,iso3166-updates,rest countries
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: Free For Educational Use
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 # ISO3166-2
 
-[![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
-[![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-updates/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-updates/actions)
-[![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
-[![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-[![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-flag-icons)](https://github.com/amckenna41/iso3166-updates/issues)
-[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
-[![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates)
+[![iso3166_updates](https://img.shields.io/pypi/v/iso3166-2)](https://pypi.org/project/iso3166-2/)
+[![Build](https://img.shields.io/github/workflow/status/amckenna41/iso3166-2/Deploy%20to%20PyPI%20📦)](https://github.com/amckenna41/iso3166-2/actions)
+[![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-2/)
+[![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-2)](https://opensource.org/licenses/MIT)
+[![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2/issues)
+[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-2)](https://github.com/amckenna41/iso3166-2)
+[![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-2)](https://github.com/iso3166-2)
+[![codecov](https://codecov.io/gh/amckenna41/pySAR/branch/master/graph/badge.svg?token=4PQDVGKGYN)](https://codecov.io/gh/amckenna41/pySAR)
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=10px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="300" width="600"/>
-  <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/>
+  <!-- <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="300" width="400"/> -->
 </div>
 
 > Custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. Available via a Python software package; a demo is available [colab][here].
 
-
 Table of Contents
 -----------------
-
   * [Introduction](#introduction)
   * [Requirements](#requirements)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
-iso3166-2 is a Custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO3166-2 standard.
-
-The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces or states) of all countries coded in ISO 3166-1. The official name of the standard is Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code. It was first published in 1998 [[2]](#references).
-
+iso3166-2 is a custom-built Python wrapper for RestCountries (https://restcountries.com/) API which includes an abundance of information about all ISO3166 countries. But this package also includes information about all countrys' ISO3166-2 subdivision codes & names, which is absent from RestCountries. The International Organisation for Standards defines codes for the names of countries, dependent territories, special areas of geographical interest, and their principal subdivisions [[1]](#references). This repo focuses on the ISO3166-2 standard.
 
-* pycountry used for foundation and build on top of it.
+The ISO 3166-2 defines codes for identifying the principal subdivisions (e.g., provinces, states, municipality etc) of all countries coded in ISO 3166-1. The official name of the standard is "Codes for the representation of names of countries and their subdivisions – Part 2: Country subdivision code." It was first published in 1998 [[2]](#references). As of 29 November 2022 there are 5,043 codes defined in ISO 3166-2. For some countries, codes are defined for more than one level of subdivisions.
 
 Latest Updates
 --------------
-* Script that calls the getISO3166 every so often to check for latest updates to restcountries. 
-* Call check_for_updates GCP func.
+An important thing to note about the ISO3166-2 and its subdivision codes/names is that changes are made consistently to it, from a small subdivision name change to an addition/deletion of a subdivision. Therefore, it's important that this library and its jsons have the most up to date data. To achieve this, the [iso3166-updates][iso3166-updates] repo was created.
+
+The iso3166-updates repo is another software pacakge and accompanying API that pulls the latest updates and changes for any and all countries in the ISO3166. The API is called every few months to check for any updates, which will then be manually incorporated into this repo. Similarly, the getISO3166_2.py script is called regularly to check for any updates for all country data using the restcountries API. 
 
 Installaion
 -----------
 Install the latest version of iso3166-2 via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-2 --upgrade
@@ -93,42 +54,63 @@
 ```
 
 Requirements
 ------------
 * [python][python] >= 3.7
 * [requests][requests] >= 2.28.1
 * [iso3166][iso3166] >= 2.1.1
-* [pycountry][pycountry] >= 22.3.5
 
 Usage
 -----
+Download all ISO3166-2 subdivision data using getISO3166_2.py script, export to two JSONs:
+```bash
+python3 getISO3166_2.py --json_filename=iso3166_2.json --output_folder=iso3166_2
+```
 
-Create instance of Subdivisions class using a country's 2 letter alpha2 code:
+Import ISO3166_2 class and access the country and subdivision data:
 ```python
 import iso3166_2 as iso
 
+#access all country data
+canada_iso3166_2 = iso.country["CA"]
+denmark_iso3166_2 = iso.country["DK"]
+estonia_iso3166_2 = iso.country["EE"]
+fiji_iso3166_2 = iso.country["FJ"]
+
+#access all country subdivision data
 canada_iso3166_2 = iso.subdivisions["CA"]
 denmark_iso3166_2 = iso.subdivisions["DK"]
 estonia_iso3166_2 = iso.subdivisions["EE"]
 fiji_iso3166_2 = iso.subdivisions["FJ"]
 ```
 
-Get list of subdivisions:
+Get country data:
+```python
+import iso3166_2 as iso
+
+canada_iso3166_2.name #country name
+denmark_iso3166_2.currencies #country currencies
+estonia_iso3166_2.capital #country capital 
+fiji_iso3166_2.population #country population 
+```
+
+Get a specific subdivision's info:
 ```python
 import iso3166_2 as iso
 
-canada_iso3166_2["Subdivisions"]
-canada_iso3166_2.subdivisions
+canada_iso3166_2.subdivisions['CA-AB'] #Alberta subdivision
+denmark_iso3166_2.subdivisions['DK-81'] #Nordjylland subdivision
+estonia_iso3166_2.subdivisions['EE-899'] #Viljandi subdivision
+fiji_iso3166_2.subdivisions['FJ-03'] #Cakaudrove subdivision 
 ```
 
 Attributes
 ----------
 You can check the [ATTRIBUTES.md][attributes] file to get a description for each attribute/field in the json exports.
 
-
 Issues or Contributing
 ----------------------
 Any issues, errors or bugs can be raised via the [Issues](https://github.com/amckenna41/iso3166_updates/issues) tab in the repository. Due to the nature of the ISO consistently updating the ISO3166-2 codes/names every year the data in the JSON's may slightly lag behind these changes. My [iso3166-updates][iso3166-updates] repo was created to check for these updates periodically and implement them in the relevant repo's. 
 
 Contact
 -------
 If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
@@ -141,32 +123,22 @@
 
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
-<!-- To Do
------
-* Validate correct subdivision codes in json. Pycountry module doesnt have the latest codes, could use iso3166-updates repo.
-* iso3166-flag-icons repo, json just contains subdivisions with flags in the repo, not all countrys' subdivisions.
-* Create automated cron script that polls the iso3166-updates repo to check for any updates to codes.
-* Look at python-countries repo (https://github.com/leonkozlowski/python-countries).
-* pyPi software package for accessing all restcountries info + included subdivision info.
-* https://github.com/mledoze/countries -->
-
-
 [python]: https://www.python.org/downloads/release/python-360/
 [requests]: https://requests.readthedocs.io/
 [iso3166]: https://github.com/deactivated/python-iso3166
 [pycountry]: https://github.com/flyingcircusio/pycountry
 [PyPi]: https://pypi.org/project/pysar/
 [iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [colab]: https://github.com/amckenna41/iso3166-updates
-[attributes]: https://github.com/amckenna41/iso3166-updates
+[attributes]: https://github.com/amckenna41/iso3166-2/ATTRIBUTES.md 
 
 <!-- https://github.com/annexare/Countries -->
 
 <!-- 
 Look over below...
 iso3166-updates is a repo that consists of a series of scripts that check for any updates/changes to the ISO3166-1 and ISO3166-2 country codes and naming conventions, as per the ISO3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO3166 standard by the ISO defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which compromise the ISO3166-2 standard [[2]](#references). 
 
@@ -179,9 +151,7 @@
 
 **Intended Audience**
 This software and accompanying API is for anyone working with country data at the ISO3166 level. It's of high importance that the data that data you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (except 2001 and 2006). iso3166-updates not only 
  
 Also, it's aimed not just at developers of ISO3166 applications but for anyone working in that space, hence the creation of an easy to use API. 
 
 <em> The earliest date for any ISO3166 updates is 2000-06-21, and the most recent is 2022-11-29 </em> -->
-
-
```

### Comparing `iso3166-2-0.0.1/setup.cfg` & `iso3166-2-1.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-2
-version = 0.0.1
+version = 1.0.0
 description = A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard.
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/amckenna41/iso3166-2
 download_url = https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip
@@ -47,15 +47,14 @@
 python_requires = >=3.6
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requies = 
 	requests>=2.28.1
 	iso3166
-	pycountry
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 	pytest-flake8
 	pytest-timeout
```

### Comparing `iso3166-2-0.0.1/setup.py` & `iso3166-2-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
 
 #software metadata
 __name__ = 'iso3166-2'
-__version__ = "0.0.1"
+__version__ = "1.0.0"
 __description__ = "A Python package to access the most up-to-date and accurate info about countries and their associated subdivisons using the ISO3166-2 standard."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __maintainer__ = "AJ McKenna"
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-2'
 __download_url__ = "https://github.com/amckenna41/iso3166-2/archive/refs/heads/main.zip"
@@ -59,14 +59,13 @@
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
       install_requires=[
           'requests>=2.28.1',
-          'iso3166',
-          'pycountry'
+          'iso3166'
       ],
      test_suite=__test_suite__,
      packages=find_packages(),
      include_package_data=True,
      zip_safe=False)
```

