# Comparing `tmp/steam_market_history-3.0.4.tar.gz` & `tmp/steam_market_history-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam_market_history-3.0.4.tar", max compression
+gzip compressed data, was "steam_market_history-3.0.5.tar", max compression
```

## Comparing `steam_market_history-3.0.4.tar` & `steam_market_history-3.0.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-04-15 00:07:27.850930 steam_market_history-3.0.4/LICENSE
--rw-r--r--   0        0        0     6156 2023-04-15 00:07:27.850930 steam_market_history-3.0.4/README.md
--rw-r--r--   0        0        0      732 2023-04-15 00:07:27.859930 steam_market_history-3.0.4/pyproject.toml
--rw-r--r--   0        0        0      144 2023-04-15 00:07:27.859930 steam_market_history-3.0.4/steam_market_history/__init__.py
--rw-r--r--   0        0        0     2159 2023-04-15 00:07:27.859930 steam_market_history-3.0.4/steam_market_history/main.py
--rw-r--r--   0        0        0        0 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/__init__.py
--rw-r--r--   0        0        0      603 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/auth.py
--rw-r--r--   0        0        0     1341 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/generator.py
--rw-r--r--   0        0        0     3381 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/modules/steam.py
--rw-r--r--   0        0        0     6167 2023-04-15 00:07:27.860930 steam_market_history-3.0.4/steam_market_history/templates/index.html
--rw-r--r--   0        0        0     7052 1970-01-01 00:00:00.000000 steam_market_history-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-17 18:30:10.067003 steam_market_history-3.0.5/LICENSE
+-rw-r--r--   0        0        0     6545 2023-04-17 18:30:10.067003 steam_market_history-3.0.5/README.md
+-rw-r--r--   0        0        0      706 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/__init__.py
+-rw-r--r--   0        0        0     2693 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/main.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/modules/__init__.py
+-rw-r--r--   0        0        0     1312 2023-04-17 18:30:10.076003 steam_market_history-3.0.5/steam_market_history/modules/exporter.py
+-rw-r--r--   0        0        0     3572 2023-04-17 18:30:10.077003 steam_market_history-3.0.5/steam_market_history/modules/steam.py
+-rw-r--r--   0        0        0     6175 2023-04-17 18:30:10.077003 steam_market_history-3.0.5/steam_market_history/templates/index.html
+-rw-r--r--   0        0        0     7441 1970-01-01 00:00:00.000000 steam_market_history-3.0.5/PKG-INFO
```

### Comparing `steam_market_history-3.0.4/LICENSE` & `steam_market_history-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.0.4/README.md` & `steam_market_history-3.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <div id="top"></div>
 
 <!-- PROJECT SHIELDS -->
 
-![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-badge)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-the-badge)
-![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-the-badge)
-![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/steam-market-history?style=for-the-badge)
-![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-history?style=for-the-badge)
-![GitLab](https://img.shields.io/gitlab/license/sustineo/steam-market-history?style=for-the-badge)
+[![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-badge)](https://pypi.org/project/steam-market-history/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-the-badge)](https://pypi.org/project/steam-market-history/)
+[![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/pipelines)
+[![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/issues)
+[![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/merge_requests)
+[![GitLab](https://img.shields.io/gitlab/license/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/blob/main/LICENSE)
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://gitlab.com/sustineo/steam-market-history">
     <img src="https://gitlab.com/sustineo/steam-market-history/-/raw/main/docs/images/logo.svg" alt="Logo" width="120" height="120">
   </a>
@@ -94,59 +94,61 @@
 
 Manual:
 
 1. Clone the repo
    ```sh
    git clone https://gitlab.com/sustineo/steam-market-history.git
    ```
-2. Install poetry (if not already installled)
+2. Install poetry (if not already installed)
    ```sh
    pip install poetry
    ```
 3. Install dependencies and start virtual environment
    ```sh
    poetry install && poetry shell
    ```
-4. Start virtual environment
-   ```sh
-   poetry shell
-   ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- USAGE EXAMPLES -->
 
 ## Usage
 
-Currently the following commands are supported:
+Currently, the following commands are supported:
 
 ### `export`
 
 Export your steam market history to a CSV or HTML file
 
-> When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your own computer. This package does not save your credentials in any way.
+> When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your computer. This package does not save your credentials in any way.
 
 Options:
 
 - `--csv` - Export to csv file
 - `--html` - Export to html file
 - `--path` - Output directory for all file based operations (default: current working directory)
 - `--launch` / `--no-launch` - Automatically open file(s) after export (default: `--launch`)
 - `--cache` / `--no-cache` - Create a file cache for all market transactions (default: `--no-cache`)
 - `--interactive` / `--non-interactive` - Interactive or non-interactive steam authentication [default: `--interactive`]
 
-Example:
+Examples:
 
+Export your steam market history to a HTML file:
+```shell
+steam-market-history export --html
 ```
-steam-market-history export --csv --path /tmp/out
+
+Export your steam market history to a CSV file in a specific directory:
+```shell
+steam-market-history export --csv --path /tmp/steam-market-history
 ```
 
 ### `version`
 
-Display detailed information about this package
+Display detailed information about this package. This includes the version, the license and the authors.
 
 ```
 steam-market-history version
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
@@ -182,22 +184,14 @@
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-<!-- CONTACT -->
-
-## Contact
-
-sustineo\_ - [@sustineo\_](https://twitter.com/sustineo_) - dev@sustineo.de
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
 <!-- ACKNOWLEDGMENTS -->
 
 ## Acknowledgments
 
 - [Typer](https://typer.tiangolo.com/)
 - [Choose a license](https://choosealicense.com/)
```

#### html2text {}

```diff
@@ -1,16 +1,21 @@
- ![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-
-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-
-market-history?style=for-the-badge) ![Gitlab pipeline status](https://
-img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-
-the-badge) ![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/
-steam-market-history?style=for-the-badge) ![GitLab merge requests](https://
+ [![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-
+badge)](https://pypi.org/project/steam-market-history/) [![PyPI - Python
+Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-
+the-badge)](https://pypi.org/project/steam-market-history/) [![Gitlab pipeline
+status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-
+history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/
+-/pipelines) [![GitLab issues](https://img.shields.io/gitlab/issues/open/
+sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/
+sustineo/steam-market-history/-/issues) [![GitLab merge requests](https://
 img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-
-history?style=for-the-badge) ![GitLab](https://img.shields.io/gitlab/license/
-sustineo/steam-market-history?style=for-the-badge)
+history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/
+-/merge_requests) [![GitLab](https://img.shields.io/gitlab/license/sustineo/
+steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-
+market-history/-/blob/main/LICENSE)
                                     [Logo]
                         **** steam-market-history ****
   An easy-to-use CLI to export your steam market history to various formats
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
@@ -31,31 +36,34 @@
 filterable results ### Built With - [Python](https://www.python.org/) - [Typer]
 (https://typer.tiangolo.com/)
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites - Python >= 3.8 ### Installation Pip
 (recommended): ```python pip install steam-market-history ``` Manual: 1. Clone
 the repo ```sh git clone https://gitlab.com/sustineo/steam-market-history.git
-``` 2. Install poetry (if not already installled) ```sh pip install poetry ```
+``` 2. Install poetry (if not already installed) ```sh pip install poetry ```
 3. Install dependencies and start virtual environment ```sh poetry install &&
-poetry shell ``` 4. Start virtual environment ```sh poetry shell ```
+poetry shell ```
                                                                   (back_to_top)
- ## Usage Currently the following commands are supported: ### `export` Export
+ ## Usage Currently, the following commands are supported: ### `export` Export
 your steam market history to a CSV or HTML file > When running the tool you
 will be prompted to insert your steam credentials. All processing is done
-locally on your own computer. This package does not save your credentials in
-any way. Options: - `--csv` - Export to csv file - `--html` - Export to html
-file - `--path` - Output directory for all file based operations (default:
-current working directory) - `--launch` / `--no-launch` - Automatically open
-file(s) after export (default: `--launch`) - `--cache` / `--no-cache` - Create
-a file cache for all market transactions (default: `--no-cache`) - `--
-interactive` / `--non-interactive` - Interactive or non-interactive steam
-authentication [default: `--interactive`] Example: ``` steam-market-history
-export --csv --path /tmp/out ``` ### `version` Display detailed information
-about this package ``` steam-market-history version ```
+locally on your computer. This package does not save your credentials in any
+way. Options: - `--csv` - Export to csv file - `--html` - Export to html file -
+`--path` - Output directory for all file based operations (default: current
+working directory) - `--launch` / `--no-launch` - Automatically open file(s)
+after export (default: `--launch`) - `--cache` / `--no-cache` - Create a file
+cache for all market transactions (default: `--no-cache`) - `--interactive` /
+`--non-interactive` - Interactive or non-interactive steam authentication
+[default: `--interactive`] Examples: Export your steam market history to a HTML
+file: ```shell steam-market-history export --html ``` Export your steam market
+history to a CSV file in a specific directory: ```shell steam-market-history
+export --csv --path /tmp/steam-market-history ``` ### `version` Display
+detailed information about this package. This includes the version, the license
+and the authors. ``` steam-market-history version ```
                                                                   (back_to_top)
  ## Roadmap - [ ] Add options of verbosity - [ ] Export to JSON See the [open
 issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full
 list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
@@ -66,16 +74,13 @@
 -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See `LICENSE` for more
 information.
                                                                   (back_to_top)
- ## Contact sustineo\_ - [@sustineo\_](https://twitter.com/sustineo_) -
-dev@sustineo.de
-                                                                  (back_to_top)
  ## Acknowledgments - [Typer](https://typer.tiangolo.com/) - [Choose a license]
 (https://choosealicense.com/)
                                                                   (back_to_top)
 ## Disclaimer: The Steam Market History Exported is a community project and is
 not affiliated with Valve or Steam.
                                                                   (back_to_top)
```

### Comparing `steam_market_history-3.0.4/pyproject.toml` & `steam_market_history-3.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "steam-market-history"
-version = "3.0.4"
+version = "3.0.5"
 description = "An easy-to-use CLI to export your steam market history to various formats"
 authors = ["Fabian Eulitz <dev@sustineo.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/fabieu/steam-market-history"
 keywords = ["steam", "CLI"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-beautifulsoup4 = "^4.11.1"
-steam = "^1.2.1"
+beautifulsoup4 = "^4.12.2"
 Jinja2 = "^3.1.2"
-typer = "^0.4.1"
+typer = "^0.7.0"
+steam = "^1.4.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-autopep8 = "^1.6.0"
-vermin = "^1.3.3"
-python-dotenv = "^0.20.0"
+pytest = "^7.3.1"
+autopep8 = "^2.0.2"
+vermin = "^1.5.1"
 
 [tool.poetry.scripts]
 steam-market-history = "steam_market_history.main:app"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `steam_market_history-3.0.4/steam_market_history/modules/generator.py` & `steam_market_history-3.0.5/steam_market_history/modules/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,28 @@
 from datetime import datetime
 from pathlib import Path
 
 # PyPi modules
 from jinja2 import Template, select_autoescape
 import typer
 
-# Local modules
 
-
-def generate_csv(market_transactions: list, path: Path, launch: bool) -> None:
+def to_csv(market_transactions: list, path: Path, launch: bool) -> None:
     filename = "steam-market-history.csv"
 
     with open(filename, 'w', newline='', encoding="utf-8") as file:
         writer = csv.writer(file, delimiter=',')
         writer.writerow(market_transactions[0].keys())
         writer.writerows([x.values() for x in market_transactions])
 
     if launch:
         typer.launch(str(path / filename), locate=True)
 
 
-def generate_html(market_transactions: list, path: Path, launch: bool) -> None:
+def to_html(market_transactions: list, path: Path, launch: bool) -> None:
     filename = "steam-market-history.html"
 
     with open(Path(__file__).parent.parent / "templates/index.html", encoding="utf-8") as template_file:
         template = Template(template_file.read(), autoescape=select_autoescape())
 
     with open(filename, 'w', encoding="utf-8") as rendered_file:
         current_date = datetime.now().strftime("%d.%m.%Y %H:%M")
```

### Comparing `steam_market_history-3.0.4/steam_market_history/modules/steam.py` & `steam_market_history-3.0.5/steam_market_history/modules/steam.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # Build-in modules
 import json
-import re
 import os
+import re
 
 # PyPi modules
 from bs4 import BeautifulSoup
+import steam.webauth as wa
 import typer
 
-# Local modules
-from steam_market_history.modules import auth
-
 app = typer.Typer()
 
 
-def fetch_market_history(interactive: bool) -> list:
+def login_cli() -> wa.WebAuth:
+    """
+    Login to Steam via CLI and return the authenticated websession
+    """
+    username = typer.prompt("Enter Steam username")
+    return wa.WebAuth(username).cli_login()
+
+
+def login_non_interactive() -> wa.WebAuth:
     """
-    Fetching market history from Steam with the session created by auth_steam() and returns an array containing all market listings
+    Login to Steam with username password, email_code and twofactor_code and return the authenticated websession
     """
+    username = os.getenv("STEAM_USERNAME")
+    password = os.getenv("STEAM_PASSWORD")
+    email_code = os.getenv("STEAM_EMAIL_CODE")
+    twofactor_code = os.getenv("STEAM_TWOFACTOR_CODE")
+    return wa.WebAuth(username).login(password=password, email_code=email_code,
+                                      twofactor_code=twofactor_code)
+
 
-    if interactive:
-        steam_session = auth.steam_auth_cli()
-    elif not interactive:
-        username = os.getenv("STEAM_USERNAME")
-        password = os.getenv("STEAM_PASSWORD")
-        email_code = os.getenv("STEAM_EMAIL_CODE")
-        twofactor_code = os.getenv("STEAM_TWOFACTOR_CODE")
-        steam_session = auth.steam_auth(username=username, password=password,
-                                        email_code=email_code, twofactor_code=twofactor_code)
+def fetch_market_history(steam_session: wa.WebAuth) -> list:
+    """
+    Fetch market history from Steam returns an array containing all market listings
+    """
 
     # Initialize content objects for storing the market history from Steam
     content = ""
     market_transactions = []
 
     start = 0
     count = 500
@@ -46,42 +54,42 @@
 
         # Update conditions for while loop
         start = page_content["start"] + count
 
         if page_content.get("total_count"):
             total_count = page_content["total_count"]
 
-    # Pulling content out of theHTML Response with the BeautifulSoup library
-    DOMdocument = BeautifulSoup(content, 'html.parser')
-    market_listing_rows = DOMdocument.find_all("div", class_="market_listing_row")
+    # Process market history with the BeautifulSoup library
+    document = BeautifulSoup(content, 'html.parser')
+    market_listing_rows = document.find_all("div", class_="market_listing_row")
 
     for row in market_listing_rows:
         price_element = row.find("span", class_="market_listing_price")
         item_name_element = row.find("span", class_="market_listing_item_name")
         game_name_element = row.find("span", class_="market_listing_game_name")
-        gainorloss_element = row.find("div", class_="market_listing_gainorloss")
+        gain_or_loss_element = row.find("div", class_="market_listing_gainorloss")
         listed_date_element = row.find("div", class_="market_listing_listed_date")
         item_img_element = row.find("img", class_="market_listing_item_img")
 
         price = price_element.text.strip() if price_element else None
         item_name = item_name_element.text.strip() if item_name_element else None
         game_name = game_name_element.text.strip() if game_name_element else None
-        gainorloss = gainorloss_element.text.strip() if gainorloss_element else None
+        gain_or_loss = gain_or_loss_element.text.strip() if gain_or_loss_element else None
         listed_date = listed_date_element.text.strip() if listed_date_element else None
         image_url = item_img_element.get("src") if item_img_element else None
 
-        # Format data
-        if (re.search(r"^\d+,(\d|-){2}$", price)):
+        # Format price of market listing item
+        if re.search(r"^\d+,(\d|-){2}$", price):
             price = price.replace(",--", ".00").replace(",", ".")
 
         # Format original steam data (market_listing_row) and add it to an array
-        if gainorloss in ["+", "-"]:
+        if gain_or_loss in ["+", "-"]:
             market_transactions.append({
                 "game_name": game_name,
                 "item_name": item_name,
                 "listed_date": listed_date,
                 "price": price,
-                "gainorloss": gainorloss,
+                "gain_or_loss": gain_or_loss,
                 "image_url": image_url,
             })
 
     return market_transactions
```

### Comparing `steam_market_history-3.0.4/steam_market_history/templates/index.html` & `steam_market_history-3.0.5/steam_market_history/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -97,21 +97,21 @@
           <tbody>
             {% for item in transactions %}
             <tr>
               <td><img src="{{ item.image_url }}" /></td>
               <td>{{ item.item_name }}</td>
               <td>{{ item.game_name }}</td>
               <td>{{ item.listed_date }}</td>
-              {% if item.gainorloss == '+'%}
+              {% if item.gain_or_loss == '+'%}
               <td class="item-bought">purchased</td>
-              {% elif item.gainorloss == '-'%}
+              {% elif item.gain_or_loss == '-'%}
               <td class="item-sold">sold</td>
               {% endif %}
               <td>
-                {% if item.gainorloss == '+'%} -{{ item.price }} {% elif item.gainorloss == '-'%}
+                {% if item.gain_or_loss == '+'%} -{{ item.price }} {% elif item.gain_or_loss == '-'%}
                 +{{ item.price }} {% endif %}
               </td>
             </tr>
             {% endfor %}
           </tbody>
         </table>
       </div>
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
 Steam_Market_History_-_{{current_date}}
 
 ****** Steam Market History Export ******
 Search and filter data in your steam market history
 Total transactions: {{ summary.totalTransactions }}
                Item           Game           Date listed      Transaction Price
                                                                                 {% if
-                                                                                item.gainorloss
+                                                                                item.gain_or_loss
 [{             {              {              {                                  == '+'%} -{
 {              {              {              {                                  { item.price }}
 item.image_url item.item_name item.game_name item.listed_date purchased   sold  {% elif
-}}]            }}             }}             }}                                 item.gainorloss
+}}]            }}             }}             }}                                 item.gain_or_loss
                                                                                 == '-'%} +{
                                                                                 { item.price }}
                                                                                 {% endif %}
```

### Comparing `steam_market_history-3.0.4/PKG-INFO` & `steam_market_history-3.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: steam-market-history
-Version: 3.0.4
+Version: 3.0.5
 Summary: An easy-to-use CLI to export your steam market history to various formats
 Home-page: https://github.com/fabieu/steam-market-history
 License: MIT
 Keywords: steam,CLI
 Author: Fabian Eulitz
 Author-email: dev@sustineo.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: steam (>=1.2.1,<2.0.0)
-Requires-Dist: typer (>=0.4.1,<0.5.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: steam (>=1.4.4,<2.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/fabieu/steam-market-history
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 
 <!-- PROJECT SHIELDS -->
 
-![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-badge)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-the-badge)
-![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-the-badge)
-![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/steam-market-history?style=for-the-badge)
-![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-history?style=for-the-badge)
-![GitLab](https://img.shields.io/gitlab/license/sustineo/steam-market-history?style=for-the-badge)
+[![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-badge)](https://pypi.org/project/steam-market-history/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-the-badge)](https://pypi.org/project/steam-market-history/)
+[![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/pipelines)
+[![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/issues)
+[![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/merge_requests)
+[![GitLab](https://img.shields.io/gitlab/license/sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/-/blob/main/LICENSE)
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://gitlab.com/sustineo/steam-market-history">
     <img src="https://gitlab.com/sustineo/steam-market-history/-/raw/main/docs/images/logo.svg" alt="Logo" width="120" height="120">
   </a>
@@ -117,59 +117,61 @@
 
 Manual:
 
 1. Clone the repo
    ```sh
    git clone https://gitlab.com/sustineo/steam-market-history.git
    ```
-2. Install poetry (if not already installled)
+2. Install poetry (if not already installed)
    ```sh
    pip install poetry
    ```
 3. Install dependencies and start virtual environment
    ```sh
    poetry install && poetry shell
    ```
-4. Start virtual environment
-   ```sh
-   poetry shell
-   ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- USAGE EXAMPLES -->
 
 ## Usage
 
-Currently the following commands are supported:
+Currently, the following commands are supported:
 
 ### `export`
 
 Export your steam market history to a CSV or HTML file
 
-> When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your own computer. This package does not save your credentials in any way.
+> When running the tool you will be prompted to insert your steam credentials. All processing is done locally on your computer. This package does not save your credentials in any way.
 
 Options:
 
 - `--csv` - Export to csv file
 - `--html` - Export to html file
 - `--path` - Output directory for all file based operations (default: current working directory)
 - `--launch` / `--no-launch` - Automatically open file(s) after export (default: `--launch`)
 - `--cache` / `--no-cache` - Create a file cache for all market transactions (default: `--no-cache`)
 - `--interactive` / `--non-interactive` - Interactive or non-interactive steam authentication [default: `--interactive`]
 
-Example:
+Examples:
 
+Export your steam market history to a HTML file:
+```shell
+steam-market-history export --html
 ```
-steam-market-history export --csv --path /tmp/out
+
+Export your steam market history to a CSV file in a specific directory:
+```shell
+steam-market-history export --csv --path /tmp/steam-market-history
 ```
 
 ### `version`
 
-Display detailed information about this package
+Display detailed information about this package. This includes the version, the license and the authors.
 
 ```
 steam-market-history version
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
@@ -205,22 +207,14 @@
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-<!-- CONTACT -->
-
-## Contact
-
-sustineo\_ - [@sustineo\_](https://twitter.com/sustineo_) - dev@sustineo.de
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
 <!-- ACKNOWLEDGMENTS -->
 
 ## Acknowledgments
 
 - [Typer](https://typer.tiangolo.com/)
 - [Choose a license](https://choosealicense.com/)
```

#### html2text {}

```diff
@@ -1,28 +1,33 @@
-Metadata-Version: 2.1 Name: steam-market-history Version: 3.0.4 Summary: An
+Metadata-Version: 2.1 Name: steam-market-history Version: 3.0.5 Summary: An
 easy-to-use CLI to export your steam market history to various formats Home-
 page: https://github.com/fabieu/steam-market-history License: MIT Keywords:
 steam,CLI Author: Fabian Eulitz Author-email: dev@sustineo.de Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist:
-beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: steam (>=1.2.1,<2.0.0)
-Requires-Dist: typer (>=0.4.1,<0.5.0) Project-URL: Repository, https://
+beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: steam (>=1.4.4,<2.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0) Project-URL: Repository, https://
 github.com/fabieu/steam-market-history Description-Content-Type: text/markdown
- ![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-
-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/steam-
-market-history?style=for-the-badge) ![Gitlab pipeline status](https://
-img.shields.io/gitlab/pipeline-status/sustineo/steam-market-history?style=for-
-the-badge) ![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/
-steam-market-history?style=for-the-badge) ![GitLab merge requests](https://
+ [![PyPI](https://img.shields.io/pypi/v/steam-market-history?style=for-the-
+badge)](https://pypi.org/project/steam-market-history/) [![PyPI - Python
+Version](https://img.shields.io/pypi/pyversions/steam-market-history?style=for-
+the-badge)](https://pypi.org/project/steam-market-history/) [![Gitlab pipeline
+status](https://img.shields.io/gitlab/pipeline-status/sustineo/steam-market-
+history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/
+-/pipelines) [![GitLab issues](https://img.shields.io/gitlab/issues/open/
+sustineo/steam-market-history?style=for-the-badge)](https://gitlab.com/
+sustineo/steam-market-history/-/issues) [![GitLab merge requests](https://
 img.shields.io/gitlab/merge-requests/open-raw/sustineo/steam-market-
-history?style=for-the-badge) ![GitLab](https://img.shields.io/gitlab/license/
-sustineo/steam-market-history?style=for-the-badge)
+history?style=for-the-badge)](https://gitlab.com/sustineo/steam-market-history/
+-/merge_requests) [![GitLab](https://img.shields.io/gitlab/license/sustineo/
+steam-market-history?style=for-the-badge)](https://gitlab.com/sustineo/steam-
+market-history/-/blob/main/LICENSE)
                                     [Logo]
                         **** steam-market-history ****
   An easy-to-use CLI to export your steam market history to various formats
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
@@ -43,31 +48,34 @@
 filterable results ### Built With - [Python](https://www.python.org/) - [Typer]
 (https://typer.tiangolo.com/)
                                                                   (back_to_top)
  ## Getting Started To get a local copy up and running follow these simple
 example steps. ### Prerequisites - Python >= 3.8 ### Installation Pip
 (recommended): ```python pip install steam-market-history ``` Manual: 1. Clone
 the repo ```sh git clone https://gitlab.com/sustineo/steam-market-history.git
-``` 2. Install poetry (if not already installled) ```sh pip install poetry ```
+``` 2. Install poetry (if not already installed) ```sh pip install poetry ```
 3. Install dependencies and start virtual environment ```sh poetry install &&
-poetry shell ``` 4. Start virtual environment ```sh poetry shell ```
+poetry shell ```
                                                                   (back_to_top)
- ## Usage Currently the following commands are supported: ### `export` Export
+ ## Usage Currently, the following commands are supported: ### `export` Export
 your steam market history to a CSV or HTML file > When running the tool you
 will be prompted to insert your steam credentials. All processing is done
-locally on your own computer. This package does not save your credentials in
-any way. Options: - `--csv` - Export to csv file - `--html` - Export to html
-file - `--path` - Output directory for all file based operations (default:
-current working directory) - `--launch` / `--no-launch` - Automatically open
-file(s) after export (default: `--launch`) - `--cache` / `--no-cache` - Create
-a file cache for all market transactions (default: `--no-cache`) - `--
-interactive` / `--non-interactive` - Interactive or non-interactive steam
-authentication [default: `--interactive`] Example: ``` steam-market-history
-export --csv --path /tmp/out ``` ### `version` Display detailed information
-about this package ``` steam-market-history version ```
+locally on your computer. This package does not save your credentials in any
+way. Options: - `--csv` - Export to csv file - `--html` - Export to html file -
+`--path` - Output directory for all file based operations (default: current
+working directory) - `--launch` / `--no-launch` - Automatically open file(s)
+after export (default: `--launch`) - `--cache` / `--no-cache` - Create a file
+cache for all market transactions (default: `--no-cache`) - `--interactive` /
+`--non-interactive` - Interactive or non-interactive steam authentication
+[default: `--interactive`] Examples: Export your steam market history to a HTML
+file: ```shell steam-market-history export --html ``` Export your steam market
+history to a CSV file in a specific directory: ```shell steam-market-history
+export --csv --path /tmp/steam-market-history ``` ### `version` Display
+detailed information about this package. This includes the version, the license
+and the authors. ``` steam-market-history version ```
                                                                   (back_to_top)
  ## Roadmap - [ ] Add options of verbosity - [ ] Export to JSON See the [open
 issues](https://gitlab.com/sustineo/steam-market-history/-/issues) for a full
 list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
@@ -78,16 +86,13 @@
 -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See `LICENSE` for more
 information.
                                                                   (back_to_top)
- ## Contact sustineo\_ - [@sustineo\_](https://twitter.com/sustineo_) -
-dev@sustineo.de
-                                                                  (back_to_top)
  ## Acknowledgments - [Typer](https://typer.tiangolo.com/) - [Choose a license]
 (https://choosealicense.com/)
                                                                   (back_to_top)
 ## Disclaimer: The Steam Market History Exported is a community project and is
 not affiliated with Valve or Steam.
                                                                   (back_to_top)
```

