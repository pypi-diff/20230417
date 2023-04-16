# Comparing `tmp/amarps-0.16.0.tar.gz` & `tmp/amarps-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarps-0.16.0.tar", max compression
+gzip compressed data, was "amarps-0.17.0.tar", max compression
```

## Comparing `amarps-0.16.0.tar` & `amarps-0.17.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2975 2023-03-31 19:56:38.178977 amarps-0.16.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-03-31 19:56:38.178977 amarps-0.16.0/LICENSE
--rw-r--r--   0        0        0      981 2023-03-31 19:56:38.178977 amarps-0.16.0/README.md
--rw-r--r--   0        0        0     1085 2023-03-31 19:56:38.178977 amarps-0.16.0/pyproject.toml
--rw-r--r--   0        0        0       79 2023-03-31 19:56:38.178977 amarps-0.16.0/src/amarps/__init__.py
--rw-r--r--   0        0        0       32 2023-03-31 19:56:38.178977 amarps-0.16.0/src/amarps/__main__.py
--rw-r--r--   0        0        0     2845 2023-03-31 19:56:38.178977 amarps-0.16.0/src/amarps/main.py
--rw-r--r--   0        0        0     1314 2023-03-31 19:56:38.178977 amarps-0.16.0/src/amarps/profile_page_selectors.yml
--rw-r--r--   0        0        0     1044 2023-03-31 19:56:38.178977 amarps-0.16.0/src/amarps/review_page_selectors.yml
--rw-r--r--   0        0        0     9762 2023-03-31 19:56:38.178977 amarps-0.16.0/src/amarps/scraper.py
--rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 amarps-0.16.0/setup.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 amarps-0.16.0/PKG-INFO
+-rw-r--r--   0        0        0     3101 2023-04-16 23:33:21.557134 amarps-0.17.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-04-16 23:33:21.557134 amarps-0.17.0/LICENSE
+-rw-r--r--   0        0        0      981 2023-04-16 23:33:21.557134 amarps-0.17.0/README.md
+-rw-r--r--   0        0        0     1111 2023-04-16 23:33:21.557134 amarps-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/__main__.py
+-rw-r--r--   0        0        0     2845 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/main.py
+-rw-r--r--   0        0        0     1314 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/profile_page_selectors.yml
+-rw-r--r--   0        0        0     1044 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/review_page_selectors.yml
+-rw-r--r--   0        0        0    10151 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/scraper.py
+-rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 amarps-0.17.0/setup.py
+-rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 amarps-0.17.0/PKG-INFO
```

### Comparing `amarps-0.16.0/CHANGELOG.md` & `amarps-0.17.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+## v0.17.0 (2023-04-17)
+
+### Feat
+
+- Download profiless together with reviews
+- Make formatting optional for certain fields
+
 ## v0.16.0 (2023-03-31)
 
 ### Feat
 
 - Improve JSON field name
 - Add profile username
-- Store command parameter in JSON output
+- Store command parameters in JSON output
 - Make integer conversion more correct
 
 ### Fix
 
 - Output messages of all log levels
 - Apply robust integer conversion
```

### Comparing `amarps-0.16.0/LICENSE` & `amarps-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amarps-0.16.0/README.md` & `amarps-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `amarps-0.16.0/pyproject.toml` & `amarps-0.17.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 authors = ["Joris Clement <joclement@posteo.net>"]
 description = "Download amazon product reviews and the reviewers profile information"
 license = "MIT"
 name = "amarps"
 readme = "README.md"
 repository = "https://github.com/joclement/amarps"
-version = "0.16.0"
+version = "0.17.0"
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4"
+python = "^3.8"
 click= "^8"
 selectorlib = "~0.16"
 selenium = "^4"
 webdriver-manager = "^3"
 selenium-wire = "^5"
 requests = "^2"
 click-log = "^0.4.0"
@@ -22,28 +22,28 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
 pytest-httpserver = "^1"
 pytest-random-order = "^1"
 pytest-rerunfailures = "^11"
 pytest-xdist = "^3"
-flake8 = "^6"
+flake8 = {version = "^6", python = ">=3.8.1"}
 mypy = ">=0.931,<=1.1.1"
 flake8-import-order = "^0.18"
 
 [tool.poetry.scripts]
 amarps = "amarps.main:main"
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 85
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.16.0"
+version = "0.17.0"
 version_files = [
     "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `amarps-0.16.0/src/amarps/main.py` & `amarps-0.17.0/src/amarps/main.py`

 * *Files identical despite different names*

### Comparing `amarps-0.16.0/src/amarps/profile_page_selectors.yml` & `amarps-0.17.0/src/amarps/profile_page_selectors.yml`

 * *Files identical despite different names*

### Comparing `amarps-0.16.0/src/amarps/review_page_selectors.yml` & `amarps-0.17.0/src/amarps/review_page_selectors.yml`

 * *Files identical despite different names*

### Comparing `amarps-0.16.0/src/amarps/scraper.py` & `amarps-0.17.0/src/amarps/scraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib.resources
 import json
 import logging
 from math import isclose
 import sys
 from time import sleep
-from typing import Any, Dict, Final, List, Optional, Union
+from typing import Any, Callable, Dict, Final, List, Optional, Union
 
 from click import File
 import dateparser
 import requests
 from selectorlib import Extractor
 from selectorlib.formatter import Formatter
 from seleniumwire import webdriver
@@ -35,30 +35,49 @@
     parts = value.split(sep, maxsplit)
     if len(parts) < 2:
         raise ValueError(f"Input '{value}' not splittable with separator '{sep}'")
     logger.debug(parts)
     return parts
 
 
+def optional(formatFunction: Callable):
+    def formatWhenPossible(self: Formatter, value: str) -> Union[str, float, int]:
+        logger.debug(
+            f"Optionally format value '{value}' with function '{formatFunction}'"
+        )
+        try:
+            return formatFunction(self, value)
+        except Exception as e:
+            logger.error(
+                f"Keep original value, formatting '{value}' led to exception: {e}"
+            )
+            return value
+
+    return formatWhenPossible
+
+
 class ReviewDate(Formatter):
+    @optional
     def format(self, date: str) -> str:
         return _convert_date(" ".join(_split(date, " ", 10)[-3:]))
 
 
 class ProfileReviewDate(Formatter):
+    @optional
     def format(self, date: str) -> str:
         return _convert_date(_split(date, " · ")[-1])
 
 
 def _convert_rating(rating: str) -> float:
     logger.debug(rating)
     return float(_split(rating, " ")[0].replace(",", ".", 1))
 
 
 class AverageRating(Formatter):
+    @optional
     def format(self, rating: str) -> float:
         return _convert_rating(rating)
 
 
 class ReviewRating(Formatter):
     def format(self, rating: str) -> Optional[int]:
         try:
@@ -82,19 +101,21 @@
 
 def _convert_integer(number: str) -> int:
     logger.debug(number)
     return int(_remove_thousand_separator(number))
 
 
 class MyInteger(Formatter):
+    @optional
     def format(self, integer: str) -> int:
         return _convert_integer(integer)
 
 
 class NumRatings(Formatter):
+    @optional
     def format(self, num_ratings: str) -> int:
         return _convert_integer(_split(num_ratings, " global")[0])
 
 
 class FoundHelpful(Formatter):
     def format(self, found_helpful: Optional[str]) -> int:
         logger.debug(found_helpful)
@@ -206,48 +227,45 @@
 
         return html_page
 
     def _get_data(self, url: str) -> Dict[str, Any]:
         return self._review_extractor.extract(self._get_html_data(url), base_url=url)
 
     def get_profile_data(self, url: str) -> Dict[str, Any]:
+        profile_data = dict()
         try:
             logger.info(f"Download profile {url}")
             profile_data = self._profile_extractor.extract(
                 self._get_html_data(url), base_url=url
             )
             logger.info(json.dumps(profile_data, indent=4))
         except TypeError as e:
             logger.error(e)
             profile_data["profile_error"] = f"Error: {e}"
+        except HttpError as e:
+            logger.error(e)
+            profile_data = {"profile_error": str(e)}
+            if e.status_code not in self._IGNORE_PROFILE_HTTP_STATUS_CODES:
+                raise
+
+        if (
+            "profile_reviews" not in profile_data
+            and "profile_error" not in profile_data
+        ):
+            profile_data["profile_error"] = "No data could be extracted"
 
         return profile_data
 
-    def _add_profiles(self, reviews: List[Dict[str, Any]]) -> None:
-        for review in reviews:
-            if review["profile_link"] is not None:
-                try:
-                    profile_data = self.get_profile_data(review["profile_link"])
-                    if profile_data["profile_reviews"] is None:
-                        profile_data["profile_error"] = "No data could be extracted"
-                except HttpError as e:
-                    logger.error(e)
-                    profile_data = {"profile_error": str(e)}
-                    if e.status_code not in self._IGNORE_PROFILE_HTTP_STATUS_CODES:
-                        raise
-                review.update(profile_data)
-            else:
-                logger.warning("No profile link was extracted")
-
     def _get_reviews(
         self,
         base_url: str,
         data: Dict[str, Any],
         start_page: int,
         stop_page: Optional[int],
+        download_profiles: bool,
     ) -> List[Dict[str, Any]]:
         reviews = []
         page = start_page
         if stop_page is None:
             stop_page = sys.maxsize
         current_url = _get_page_url(base_url, page)
         reviews_exist = True
@@ -255,14 +273,16 @@
 
         while reviews_exist and page <= stop_page:
             reviews_exist = False
             logger.info(json.dumps(reviews_data, indent=4))
 
             for r in reviews_data:
                 r["url"] = current_url
+                if download_profiles and r["profile_link"] is not None:
+                    r.update(self.get_profile_data(r["profile_link"]))
                 reviews.append(r)
 
             page += 1
             current_url = _get_page_url(base_url, page)
             next_page_data = self._get_data(current_url)
             if "reviews" in next_page_data and next_page_data["reviews"] is not None:
                 reviews_exist = True
@@ -288,13 +308,12 @@
                 logger.warning(
                     f"The query will be retried in {sleep_time} seconds, "
                     "please try to solve a CAPTCHA or login if possible"
                 )
                 sleep(sleep_time)
                 data = self._get_data(_get_page_url(base_url, start_page))
 
-        data["reviews"] = self._get_reviews(base_url, data, start_page, stop_page)
-
-        if download_profiles:
-            self._add_profiles(data["reviews"])
+        data["reviews"] = self._get_reviews(
+            base_url, data, start_page, stop_page, download_profiles
+        )
 
         return data
```

### Comparing `amarps-0.16.0/setup.py` & `amarps-0.17.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,25 @@
  'webdriver-manager>=3,<4']
 
 entry_points = \
 {'console_scripts': ['amarps = amarps.main:main']}
 
 setup_kwargs = {
     'name': 'amarps',
-    'version': '0.16.0',
+    'version': '0.17.0',
     'description': 'Download amazon product reviews and the reviewers profile information',
     'long_description': '[![Tests](https://github.com/joclement/amarps/workflows/Tests/badge.svg)](https://github.com/joclement/amarps/actions?workflow=Tests)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/joclement/amarps/main.svg)](https://results.pre-commit.ci/latest/github/joclement/amarps/main)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Python Versions](https://img.shields.io/pypi/pyversions/amarps)](https://img.shields.io/pypi/pyversions/amarps)\n\n# Amazon Review Profile Scraper\n\nA very basic tool to scrape the user reviews of a product on Amazon the profiles that created those reviews.\n\nIt is intended to be used for research to analyze the quality of a user review based on\nother information belonging to the user.\n\n## Usage\n\n1. Install this tool `pip install amarps`.\n2. Run `python -m amarps --help` to check the usage\n3. Run e.g. `python -m amarps https://www.amazon.com/product-reviews/B07ZPL752N/`\n',
     'author': 'Joris Clement',
     'author_email': 'joclement@posteo.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/joclement/amarps',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `amarps-0.16.0/PKG-INFO` & `amarps-0.17.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: amarps
-Version: 0.16.0
+Version: 0.17.0
 Summary: Download amazon product reviews and the reviewers profile information
 Home-page: https://github.com/joclement/amarps
 License: MIT
 Author: Joris Clement
 Author-email: joclement@posteo.net
-Requires-Python: >=3.8.1,<4
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: dateparser (>=1,<2)
 Requires-Dist: requests (>=2,<3)
```

