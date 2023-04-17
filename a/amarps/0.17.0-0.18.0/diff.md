# Comparing `tmp/amarps-0.17.0.tar.gz` & `tmp/amarps-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarps-0.17.0.tar", max compression
+gzip compressed data, was "amarps-0.18.0.tar", max compression
```

## Comparing `amarps-0.17.0.tar` & `amarps-0.18.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3101 2023-04-16 23:33:21.557134 amarps-0.17.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-04-16 23:33:21.557134 amarps-0.17.0/LICENSE
--rw-r--r--   0        0        0      981 2023-04-16 23:33:21.557134 amarps-0.17.0/README.md
--rw-r--r--   0        0        0     1111 2023-04-16 23:33:21.557134 amarps-0.17.0/pyproject.toml
--rw-r--r--   0        0        0       79 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/__init__.py
--rw-r--r--   0        0        0       32 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/__main__.py
--rw-r--r--   0        0        0     2845 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/main.py
--rw-r--r--   0        0        0     1314 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/profile_page_selectors.yml
--rw-r--r--   0        0        0     1044 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/review_page_selectors.yml
--rw-r--r--   0        0        0    10151 2023-04-16 23:33:21.557134 amarps-0.17.0/src/amarps/scraper.py
--rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 amarps-0.17.0/setup.py
--rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 amarps-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0     3286 2023-04-17 21:27:27.368943 amarps-0.18.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-04-17 21:27:27.368943 amarps-0.18.0/LICENSE
+-rw-r--r--   0        0        0     1001 2023-04-17 21:27:27.368943 amarps-0.18.0/README.md
+-rw-r--r--   0        0        0     1111 2023-04-17 21:27:27.368943 amarps-0.18.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/__main__.py
+-rw-r--r--   0        0        0     3466 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/main.py
+-rw-r--r--   0        0        0     1314 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/profile_page_selectors.yml
+-rw-r--r--   0        0        0     1044 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/review_page_selectors.yml
+-rw-r--r--   0        0        0    10807 2023-04-17 21:27:27.368943 amarps-0.18.0/src/amarps/scraper.py
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 amarps-0.18.0/setup.py
+-rw-r--r--   0        0        0     1975 1970-01-01 00:00:00.000000 amarps-0.18.0/PKG-INFO
```

### Comparing `amarps-0.17.0/CHANGELOG.md` & `amarps-0.18.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,24 @@
+## v0.18.0 (2023-04-17)
+
+### Feat
+
+- Sleep shortly after scrolling
+- Increase scrolling and make it configurable
+- Add debug log initializing browser
+
+### Refactor
+
+- Reduce redundancy
+
 ## v0.17.0 (2023-04-17)
 
 ### Feat
 
-- Download profiless together with reviews
+- Download profiles together with reviews
 - Make formatting optional for certain fields
 
 ## v0.16.0 (2023-03-31)
 
 ### Feat
 
 - Improve JSON field name
```

### Comparing `amarps-0.17.0/LICENSE` & `amarps-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amarps-0.17.0/README.md` & `amarps-0.18.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [![Tests](https://github.com/joclement/amarps/workflows/Tests/badge.svg)](https://github.com/joclement/amarps/actions?workflow=Tests)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/joclement/amarps/main.svg)](https://results.pre-commit.ci/latest/github/joclement/amarps/main)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python Versions](https://img.shields.io/pypi/pyversions/amarps)](https://img.shields.io/pypi/pyversions/amarps)
 
 # Amazon Review Profile Scraper
 
-A very basic tool to scrape the user reviews of a product on Amazon the profiles that created those reviews.
+## Description
 
-It is intended to be used for research to analyze the quality of a user review based on
-other information belonging to the user.
+A very basic tool to scrape the user reviews of a product on Amazon and the
+profiles that created those reviews.
+
+It is intended to be used for research to analyze the quality of a user review
+based on other information belonging to the user.
 
 ## Usage
 
 1. Install this tool `pip install amarps`.
 2. Run `python -m amarps --help` to check the usage
 3. Run e.g. `python -m amarps https://www.amazon.com/product-reviews/B07ZPL752N/`
```

### Comparing `amarps-0.17.0/pyproject.toml` & `amarps-0.18.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Joris Clement <joclement@posteo.net>"]
 description = "Download amazon product reviews and the reviewers profile information"
 license = "MIT"
 name = "amarps"
 readme = "README.md"
 repository = "https://github.com/joclement/amarps"
-version = "0.17.0"
+version = "0.18.0"
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click= "^8"
 selectorlib = "~0.16"
 selenium = "^4"
@@ -35,15 +35,15 @@
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 85
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.17.0"
+version = "0.18.0"
 version_files = [
     "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `amarps-0.17.0/src/amarps/main.py` & `amarps-0.18.0/src/amarps/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 import sys
 from typing import Any, Dict, Optional
 
 import click
 import click_log
 
 from . import __version__
-from .scraper import logger, Scraper
+from .scraper import (
+    BROWSER,
+    HAVE_BROWSER_HEADLESS,
+    logger,
+    Scraper,
+    SCROLL_DEPTH_PROFILE_PAGE,
+    SCROLL_DEPTH_REVIEWS_PAGE,
+)
 
 
 click_log.basic_config(logger)
 
 
 def _get_command_parameters() -> Dict[str, Any]:
     params = click.get_current_context().params
@@ -67,51 +74,73 @@
     type=click.File("w"),
 )
 @click.option(
     "--browser",
     "-b",
     help="Set which browser should be used",
     type=click.Choice(["chrome", "firefox"]),
-    default="chrome",
+    default=BROWSER,
     show_default=True,
 )
 @click.option(
     "--headless/--no-headless",
     "have_browser_headless",
     help="Run browser in background making it more easily detectable as a web scraper",
-    default=False,
+    default=HAVE_BROWSER_HEADLESS,
     show_default=True,
 )
 @click.option(
     "--sleep-time",
     help="Time to wait for user input when the 1st request fails",
     type=int,
     default=60,
     show_default=True,
 )
+@click.option(
+    "--scroll-depth-profile",
+    help="Scroll depth for the profile pages",
+    type=int,
+    default=SCROLL_DEPTH_PROFILE_PAGE,
+    show_default=True,
+)
+@click.option(
+    "--scroll-depth-reviews",
+    help="Scroll depth for the reviews pages",
+    type=int,
+    default=SCROLL_DEPTH_REVIEWS_PAGE,
+    show_default=True,
+)
 def main(
     link: str,
     profiles: bool,
     start_page: int,
     stop_page: Optional[int],
     output: click.File,
     profile_link: bool,
     html_page: click.File,
     browser: str,
     have_browser_headless: bool,
     sleep_time: int,
+    scroll_depth_profile: int,
+    scroll_depth_reviews: int,
 ) -> None:
     """Download amazon product reviews and reviewers profile information
 
     LINK is an URL to the reviews of an amazon product or to an amazon profile.
-    Link must be of the form 'https://www.amazon.com/product-reviews/B01AMT0EYU/' and
+    Link must be of the form 'https://www.amazon.com/product-reviews/ID123ABC/' and
     must end with a '/'."
     """
     data = {"python_command_parameters": _get_command_parameters()}
 
-    arr = Scraper(html_page, browser, have_browser_headless)
+    arr = Scraper(
+        html_page,
+        browser,
+        have_browser_headless,
+        scroll_depth_profile,
+        scroll_depth_reviews,
+    )
     if profile_link:
         data.update(arr.get_profile_data(link))
     else:
         data.update(arr.extract(link, profiles, start_page, stop_page, sleep_time))
 
     output.write(json.dumps(data))
```

### Comparing `amarps-0.17.0/src/amarps/profile_page_selectors.yml` & `amarps-0.18.0/src/amarps/profile_page_selectors.yml`

 * *Files identical despite different names*

### Comparing `amarps-0.17.0/src/amarps/review_page_selectors.yml` & `amarps-0.18.0/src/amarps/review_page_selectors.yml`

 * *Files identical despite different names*

### Comparing `amarps-0.17.0/src/amarps/scraper.py` & `amarps-0.18.0/src/amarps/scraper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import importlib.resources
 import json
 import logging
 from math import isclose
+import random
 import sys
 from time import sleep
 from typing import Any, Callable, Dict, Final, List, Optional, Union
 
 from click import File
 import dateparser
 import requests
 from selectorlib import Extractor
 from selectorlib.formatter import Formatter
 from seleniumwire import webdriver
 
 
+BROWSER: Final = "chrome"
+HAVE_BROWSER_HEADLESS: Final = False
+SCROLL_DEPTH_PROFILE_PAGE: Final = 2000
+SCROLL_DEPTH_REVIEWS_PAGE: Final = 2000
+
+
 logger = logging.getLogger(__name__)
 
 
 def _get_page_url(base_url: str, page: int) -> str:
     return base_url + f"ref=cm_cr_arp_d_paging_btm_next_{page}?pageNumber={page}"
 
 
@@ -143,14 +150,16 @@
     def __str__(self):
         return f"HTTP error: {self.status_code}"
 
 
 def _init_browser_driver(
     browser: str, have_browser_headless: bool
 ) -> Union[webdriver.Chrome, webdriver.Firefox]:
+    logger.debug(f"Init browser '{browser}'")
+
     if browser == "chrome":
         from selenium.webdriver.chrome.service import Service
         from seleniumwire.webdriver import Chrome as BrowserDriver
         from seleniumwire.webdriver import ChromeOptions as BrowserDriverOptions
         from webdriver_manager.chrome import ChromeDriverManager as BrowserDriverManager
     elif browser == "firefox":
         from selenium.webdriver.firefox.service import Service
@@ -160,14 +169,15 @@
     else:
         raise ValueError(f"Invalid browser: {browser}")
 
     options = BrowserDriverOptions()
     options.set_capability("loggingPrefs", {"performance": "ALL"})
     if have_browser_headless:
         options.add_argument("--headless")
+
     return BrowserDriver(
         options=options,
         service=Service(BrowserDriverManager().install()),
     )
 
 
 class ImageSrcToBool(Formatter):
@@ -178,19 +188,23 @@
         return not isclose(len(response.content), 7186, rel_tol=0.05)
 
 
 class Scraper:
     def __init__(
         self,
         html_page_writer: Optional[File] = None,
-        browser: str = "chrome",
-        have_browser_headless: bool = False,
+        browser: str = BROWSER,
+        have_browser_headless: bool = HAVE_BROWSER_HEADLESS,
+        scroll_depth_profile_page: int = SCROLL_DEPTH_PROFILE_PAGE,
+        scroll_depth_reviews_page: int = SCROLL_DEPTH_REVIEWS_PAGE,
     ):
         self._html_page_writer = html_page_writer
         self.have_browser_headless = have_browser_headless
+        self.scroll_depth_profile_page = scroll_depth_profile_page
+        self.scroll_depth_reviews_page = scroll_depth_reviews_page
         self._webdriver = _init_browser_driver(browser, self.have_browser_headless)
 
         self._review_extractor = Extractor.from_yaml_string(
             importlib.resources.read_text("amarps", "review_page_selectors.yml"),
             formatters=Formatter.get_all(),
         )
         self._profile_extractor = Extractor.from_yaml_string(
@@ -208,38 +222,44 @@
         try:
             status = self._webdriver.last_request.response.status_code
             if status >= 400:
                 raise HttpError(status)
         except AttributeError:
             logger.warning("Failed to get HTTP status code")
 
-    def _get_html_data(self, url: str, check_status: bool = True) -> str:
+    def _get_html_data(
+        self, url: str, scroll_depth: int, check_status: bool = True
+    ) -> str:
         logger.info(f"Download {url}")
 
         self._webdriver.get(url)
-        self._webdriver.execute_script("window.scrollTo(0,20)")
+        self._webdriver.execute_script(f"window.scrollTo(0,{scroll_depth})")
+
+        sleep(random.random())
 
         html_page = self._webdriver.page_source
         if self._html_page_writer is not None:
             self._html_page_writer.write(html_page)
 
         if check_status:
             self._raise_for_status()
 
         return html_page
 
     def _get_data(self, url: str) -> Dict[str, Any]:
-        return self._review_extractor.extract(self._get_html_data(url), base_url=url)
+        return self._review_extractor.extract(
+            self._get_html_data(url, self.scroll_depth_reviews_page), base_url=url
+        )
 
     def get_profile_data(self, url: str) -> Dict[str, Any]:
         profile_data = dict()
         try:
             logger.info(f"Download profile {url}")
             profile_data = self._profile_extractor.extract(
-                self._get_html_data(url), base_url=url
+                self._get_html_data(url, self.scroll_depth_profile_page), base_url=url
             )
             logger.info(json.dumps(profile_data, indent=4))
         except TypeError as e:
             logger.error(e)
             profile_data["profile_error"] = f"Error: {e}"
         except HttpError as e:
             logger.error(e)
```

### Comparing `amarps-0.17.0/setup.py` & `amarps-0.18.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'webdriver-manager>=3,<4']
 
 entry_points = \
 {'console_scripts': ['amarps = amarps.main:main']}
 
 setup_kwargs = {
     'name': 'amarps',
-    'version': '0.17.0',
+    'version': '0.18.0',
     'description': 'Download amazon product reviews and the reviewers profile information',
-    'long_description': '[![Tests](https://github.com/joclement/amarps/workflows/Tests/badge.svg)](https://github.com/joclement/amarps/actions?workflow=Tests)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/joclement/amarps/main.svg)](https://results.pre-commit.ci/latest/github/joclement/amarps/main)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Python Versions](https://img.shields.io/pypi/pyversions/amarps)](https://img.shields.io/pypi/pyversions/amarps)\n\n# Amazon Review Profile Scraper\n\nA very basic tool to scrape the user reviews of a product on Amazon the profiles that created those reviews.\n\nIt is intended to be used for research to analyze the quality of a user review based on\nother information belonging to the user.\n\n## Usage\n\n1. Install this tool `pip install amarps`.\n2. Run `python -m amarps --help` to check the usage\n3. Run e.g. `python -m amarps https://www.amazon.com/product-reviews/B07ZPL752N/`\n',
+    'long_description': '[![Tests](https://github.com/joclement/amarps/workflows/Tests/badge.svg)](https://github.com/joclement/amarps/actions?workflow=Tests)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/joclement/amarps/main.svg)](https://results.pre-commit.ci/latest/github/joclement/amarps/main)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Python Versions](https://img.shields.io/pypi/pyversions/amarps)](https://img.shields.io/pypi/pyversions/amarps)\n\n# Amazon Review Profile Scraper\n\n## Description\n\nA very basic tool to scrape the user reviews of a product on Amazon and the\nprofiles that created those reviews.\n\nIt is intended to be used for research to analyze the quality of a user review\nbased on other information belonging to the user.\n\n## Usage\n\n1. Install this tool `pip install amarps`.\n2. Run `python -m amarps --help` to check the usage\n3. Run e.g. `python -m amarps https://www.amazon.com/product-reviews/B07ZPL752N/`\n',
     'author': 'Joris Clement',
     'author_email': 'joclement@posteo.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/joclement/amarps',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `amarps-0.17.0/PKG-INFO` & `amarps-0.18.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarps
-Version: 0.17.0
+Version: 0.18.0
 Summary: Download amazon product reviews and the reviewers profile information
 Home-page: https://github.com/joclement/amarps
 License: MIT
 Author: Joris Clement
 Author-email: joclement@posteo.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,18 +27,21 @@
 [![Tests](https://github.com/joclement/amarps/workflows/Tests/badge.svg)](https://github.com/joclement/amarps/actions?workflow=Tests)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/joclement/amarps/main.svg)](https://results.pre-commit.ci/latest/github/joclement/amarps/main)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python Versions](https://img.shields.io/pypi/pyversions/amarps)](https://img.shields.io/pypi/pyversions/amarps)
 
 # Amazon Review Profile Scraper
 
-A very basic tool to scrape the user reviews of a product on Amazon the profiles that created those reviews.
+## Description
 
-It is intended to be used for research to analyze the quality of a user review based on
-other information belonging to the user.
+A very basic tool to scrape the user reviews of a product on Amazon and the
+profiles that created those reviews.
+
+It is intended to be used for research to analyze the quality of a user review
+based on other information belonging to the user.
 
 ## Usage
 
 1. Install this tool `pip install amarps`.
 2. Run `python -m amarps --help` to check the usage
 3. Run e.g. `python -m amarps https://www.amazon.com/product-reviews/B07ZPL752N/`
```

