# Comparing `tmp/ppmi_downloader-0.7.2.tar.gz` & `tmp/ppmi_downloader-0.7.3.tar.gz`

## Comparing `ppmi_downloader-0.7.2.tar` & `ppmi_downloader-0.7.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/MANIFEST.in
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/build-mapping.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/conftest.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/.github/workflows/main.yml
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/ppmi_downloader/__init__.py
--rw-r--r--   0        0        0    41898 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/ppmi_downloader/guessed_to_real.json
--rw-r--r--   0        0        0    26562 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/ppmi_downloader/ppmi_downloader.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/ppmi_downloader/ppmi_logger.py
--rw-r--r--   0        0        0    26087 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/ppmi_downloader/ppmi_navigator.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/ppmi_downloader/selenium_grid_utils.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/ppmi_downloader/tests/test_ppmi_downloader.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/LICENSE
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/README.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/MANIFEST.in
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/build-mapping.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/conftest.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/ppmi_downloader/__init__.py
+-rw-r--r--   0        0        0    41898 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/ppmi_downloader/guessed_to_real.json
+-rw-r--r--   0        0        0    27688 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/ppmi_downloader/ppmi_downloader.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/ppmi_downloader/ppmi_logger.py
+-rw-r--r--   0        0        0    27944 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/ppmi_downloader/ppmi_navigator.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/ppmi_downloader/selenium_grid_utils.py
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/ppmi_downloader/tests/test_ppmi_downloader.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/README.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 ppmi_downloader-0.7.3/PKG-INFO
```

### Comparing `ppmi_downloader-0.7.2/build-mapping.py` & `ppmi_downloader-0.7.3/build-mapping.py`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/requirements.txt` & `ppmi_downloader-0.7.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/.github/workflows/main.yml` & `ppmi_downloader-0.7.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/.github/workflows/python-app.yml` & `ppmi_downloader-0.7.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/.github/workflows/tests.yml` & `ppmi_downloader-0.7.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/ppmi_downloader/guessed_to_real.json` & `ppmi_downloader-0.7.3/ppmi_downloader/guessed_to_real.json`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/ppmi_downloader/ppmi_downloader.py` & `ppmi_downloader-0.7.3/ppmi_downloader/ppmi_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import getpass
 import glob
 import json
 import os
 import os.path as op
+from pathlib import Path
 import pkg_resources
 import signal
 import socket
 import string
 import tempfile
 import xml.etree.ElementTree as ET
 from configparser import ConfigParser
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Optional, List
+from typing import Optional, List, Sequence
 
 import tqdm
 from bs4 import BeautifulSoup
 from selenium import webdriver
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
+from packaging import version
 
 import ppmi_downloader.ppmi_logger as logger
 from ppmi_downloader.ppmi_navigator import (
     PPMINavigator,
     ppmi_home_webpage,
     ppmi_main_webpage,
 )
 
 
+class fileMatchingError(Exception):
+    pass
+
+
 def get_ip_hostname():
     return socket.gethostbyname(socket.gethostname()) + ":4444"
 
 
 @contextmanager
 def timeout_manager(timeout):
     # Register a function to raise a TimeoutError on the signal.
@@ -68,40 +74,46 @@
         If set, specifies the url of the selenium grid to connect on
 
     Returns
     -------
     WebDriver
     """
     # Create Chrome webdriver
+    manager = ChromeDriverManager()
     options = webdriver.ChromeOptions()
     prefs = {
         "download.default_directory": tempdir,
         "download.prompt_for_download": False,
     }
+
     options.add_experimental_option("prefs", prefs)
     if headless:
-        options.add_argument("--headless")
+        # https://www.selenium.dev/blog/2023/headless-is-going-away/
+        if version.parse(manager.driver.get_browser_version()) < version.parse('109'):
+            options.add_argument("--headless")
+        else:
+            options.add_argument("--headless=new")
+        options.add_argument("--window-size=1920,1080")
+
     if remote is None:
         driver = webdriver.Chrome(
-            ChromeDriverManager().install(), chrome_options=options
+            ChromeDriverManager().install(), options=options
         )
     else:
         if remote == "hostname":
             remote = get_ip_hostname()
 
         options.add_argument("--ignore-ssl-errors=yes")
         options.add_argument("--ignore-certificate-errors")
-        options.add_argument("--headless")
         driver = None
         with timeout_manager(30):
             driver = webdriver.Remote(remote, options=options)
         if driver is None:
             logger.error("Unable to reach Remote selenium webdriver")
 
-    driver.set_window_size(1200, 720)
     driver.maximize_window()
     return driver
 
 
 class PPMIDownloader:
     """
     A downloader of PPMI metadata. Requires a PPMI account.
@@ -140,27 +152,30 @@
             If set, specifies the url of the selenium grid to connect on
 
         """
         self.remote = remote
         if self.remote is None:
             self.remote = os.getenv("PPMI_SINGULARITY_SELENIUM_REMOTE")
         self.__set_credentials(config_file)
-        self.tempdir = tempfile.TemporaryDirectory(dir=os.path.abspath(tempdir))
+        self.tempdir = tempfile.TemporaryDirectory(
+            dir=os.path.abspath(tempdir))
         self.driver = get_driver(
             headless=headless, tempdir=self.tempdir.name, remote=self.remote
         )
         self.html = PPMINavigator(self.driver)
 
+        logger.debug(self.driver.desired_capabilities)
         logger.debug(self.tempdir)
 
         # Load real metadata names
         self._get_real_name()
 
         # Ids of the download checkboxes in the PPMI metadata download page
-        self.file_ids_path = Path(__file__).parent.joinpath(self.file_ids_default_path)
+        self.file_ids_path = Path(__file__).parent.joinpath(
+            self.file_ids_default_path)
         if not self.file_ids_path.exists():
             self.crawl_study_data(cache_file=self.file_ids_path)
 
         with open(self.file_ids_path, "r", encoding="utf-8") as fin:
             self.file_ids = json.load(fin)
 
         logger.debug(self.config_file, config_file)
@@ -237,17 +252,18 @@
         """
         cache_file = pkg_resources.resource_filename(
             "ppmi_downloader", "guessed_to_real.json"
         )
 
         with open(cache_file, "r", encoding="utf-8") as fi:
             self.guessed_to_real = json.load(fi)
-            self.real_to_guessed = {v: k for k, v in self.guessed_to_real.items()}
+            self.real_to_guessed = {v: k for k,
+                                    v in self.guessed_to_real.items()}
 
-    def init_and_log(self, headless: bool = True) -> None:
+    def init_and_log(self) -> None:
         """
         Initialize a driver, a ppmi navigator
         and login to ppmi portal
         """
         self.html.login(self.email, self.password)
 
     def crawl_checkboxes_id(self, soup):
@@ -258,27 +274,27 @@
         """
         label_to_checkboxes_id = {}
         for checkbox in soup.find_all(type="checkbox"):
             if (checkbox_id := checkbox.get("id")) is not None:
                 if (href := checkbox.findNext()) is not None:
                     name = href.text
                     if name == "" or name is None:
-                        logger.warning(f"Found checkbox with no name {checkbox}")
+                        logger.warning(
+                            f"Found checkbox with no name {checkbox}")
                     else:
                         label_to_checkboxes_id[name.strip()] = checkbox_id
         return label_to_checkboxes_id
 
     def crawl_study_data(
-        self, cache_file: str = "study_data_to_checkbox_id.json", headless: bool = True
-    ):
+            self, cache_file: str = "study_data_to_checkbox_id.json"):
         """
         Creates a mapping between Study data checkbox's name
         and their corresponding checkbox id
         """
-        self.init_and_log(headless=headless)
+        self.init_and_log()
         self.html.click_button_chain(["Download", "Study Data", "ALL"])
         soup = BeautifulSoup(self.driver.page_source, features="lxml")
         study_name_to_checkbox = self.crawl_checkboxes_id(soup)
 
         def clean_name(name):
             to_replace = {
                 ord(c): "_"
@@ -290,32 +306,28 @@
         for name, checkbox in study_name_to_checkbox.items():
             if checkbox.isdigit() and "Archived" not in name:
                 study_name_to_checkbox_clean[clean_name(name)] = checkbox
 
         with open(cache_file, "w", encoding="utf-8") as fo:
             json.dump(study_name_to_checkbox_clean, fo, indent=0)
 
-        # self.driver.close()
-
     def crawl_advanced_search(
-        self, cache_file: str = "search_to_checkbox_id.json", headless: bool = True
-    ):
+            self, cache_file: str = "search_to_checkbox_id.json"):
         """
         Creates a mapping between Advances Search checkboxe's name
         and their corresponding checkbox id
         """
-        self.init_and_log(headless=headless)
-        self.html.click_button_chain(["Search", "Advanced Image Search (beta)"])
+        self.init_and_log()
+        self.html.click_button_chain(
+            ["Search", "Advanced Image Search (beta)"])
         soup = BeautifulSoup(self.driver.page_source, features="lxml")
         criteria_name_to_checkbox_id = self.crawl_checkboxes_id(soup)
         with open(cache_file, "w", encoding="utf-8") as fo:
             json.dump(criteria_name_to_checkbox_id, fo, indent=0)
 
-        # self.driver.close()
-
     def download_imaging_data(
         self,
         subject_ids: List[int],
         timeout: float = 600,
         destination_dir: str = ".",
         type: str = "archived",
     ):
@@ -349,15 +361,16 @@
         self.driver.get(ppmi_main_webpage)
         self.html.login(self.email, self.password)
 
         # navigate to search page
         self.driver.get(ppmi_home_webpage)
         # click on 'Search'
         # Click on 'Advanced Image Search (beta)'
-        self.html.click_button_chain(["Search", "Advanced Image Search (beta)"])
+        self.html.click_button_chain(
+            ["Search", "Advanced Image Search (beta)"])
 
         # Enter id's and add to collection
         self.html.enter_data("subjectIdText", subjectIds, By.ID)
         self.html.click_button("advSearchQuery", By.ID)
         self.html.Search_AdvancedImageSearchbeta_SelectAll()
         self.html.click_button("advResultAddCollectId", By.ID)
         self.html.enter_data(
@@ -386,28 +399,26 @@
                 return False
             for f in downloaded_files:
                 if f.endswith(".crdownload"):
                     filename = os.path.join(self.tempdir.name, f)
                     size = os.stat(filename).st_size
                     logger.debug("Size", size)
                     return False
-            assert f.endswith((".csv", ".zip", ".dcm", ".xml")), f
+            # assert f.endswith((".csv", ".zip", ".dcm", ".xml")), f
             return True
 
         try:
-            WebDriverWait(self.driver, timeout).until(download_complete)
+            WebDriverWait(self.driver, timeout, poll_frequency=5).until(
+                download_complete)
         except TimeoutException:
             self.quit()
             logger.error("Timeout when downloading imaging data", subject_ids)
         # Move file to cwd or extract zip file
         downloaded_files = os.listdir(self.tempdir.name)
 
-        # we got imaging data and metadata
-        assert len(downloaded_files) == 3
-
         # unzip files
         self.html.unzip_imaging_data(
             downloaded_files, self.tempdir.name, destination_dir
         )
 
     def download_3D_T1_info(
         self, timeout: float = 120, destination_dir: str = "."
@@ -426,34 +437,40 @@
         # Login to PPMI
         self.driver.get(ppmi_main_webpage)
         # self.html = PPMINavigator(self.driver)
         self.html.login(self.email, self.password)
 
         # navigate to metadata page
         self.driver.get(ppmi_home_webpage)
-        self.html.click_button_chain(["Search", "Advanced Image Search (beta)"])
+        self.html.click_button_chain(
+            ["Search", "Advanced Image Search (beta)"])
 
         # Click 3D checkbox
-        self.html.click_button("imgProtocol_checkBox1.Acquisition_Type.3D", By.ID)
+        self.html.click_button(
+            "imgProtocol_checkBox1.Acquisition_Type.3D", By.ID)
         # Click checkbox to display visit name in results
         self.html.click_button("RESET_VISIT.0", By.ID)
         # Click checkbox to display weighting in results
         self.html.click_button("RESET_PROTOCOL_STRING.1_Weighting", By.ID)
         # Click checkbox to display manufacturer in results
         self.html.click_button("RESET_PROTOCOL_STRING.1_Manufacturer", By.ID)
+        # Click checkbox to display slice thickness in results
+        self.html.click_button(
+            "RESET_PROTOCOL_NUMERIC.imgProtocol_1_Slice_Thickness", By.ID)
         # Click checkbox to display manufacturer model in results
         self.html.click_button("RESET_PROTOCOL_STRING.1_Mfg_Model", By.ID)
         # Click checkbox to display study date in results
         self.html.click_button("RESET_STUDY.0", By.ID)
         # Click checkbox to display field strength in results
         self.html.click_button(
             "RESET_PROTOCOL_NUMERIC.imgProtocol_1_Field_Strength", By.ID
         )
         # Click checkbox to display acquisition plane in results
-        self.html.click_button("RESET_PROTOCOL_STRING.1_Acquisition_Plane", By.ID)
+        self.html.click_button(
+            "RESET_PROTOCOL_STRING.1_Acquisition_Plane", By.ID)
 
         # Click search button
         self.html.click_button("advSearchQuery", By.ID)
         # Click CSV Download button
         self.html.click_button('//*[@type="button" and @value="CSV Download"]')
 
         # Wait for download to complete
@@ -466,32 +483,34 @@
                 if f.endswith(".crdownload"):
                     filename = os.path.join(self.tempdir.name, f)
                     size = os.stat(filename).st_size
                     logger.debug("Size", size)
                     return False
                 if f.endswith(".csv"):
                     return True
-            assert f.endswith(".csv"), f"file ends with: {f}"
+            # assert f.endswith(".csv"), f"file ends with: {f}"
             return True
 
         try:
-            WebDriverWait(self.driver, timeout).until(download_complete)
+            WebDriverWait(self.driver, timeout, poll_frequency=5).until(
+                download_complete)
         except TimeoutException:
             self.quit()
             logger.error("Unable to download T1 3D information")
 
         # Move file to cwd or extract zip file
-        file_name = self.html.unzip_metadata(self.tempdir.name, destination_dir)
+        file_name = self.html.unzip_metadata(
+            self.tempdir.name, destination_dir)
 
         return file_name
 
     def download_metadata(
         self,
         file_ids: str | List[str],
-        timeout: float = 120,
+        timeout: float = 600,
         destination_dir: str = ".",
     ) -> None:
         """
         Download metadata files from PPMI. Requires Google Chrome.
 
         Parameters
         ----------
@@ -502,15 +521,16 @@
         destination_dir : str
           directory where to store the downloaded files
         """
 
         if not isinstance(file_ids, list):
             file_ids = [file_ids]
 
-        supported_files = set(self.file_ids.keys()) | set(self.real_to_guessed.keys())
+        supported_files = set(self.file_ids.keys()) | set(
+            self.real_to_guessed.keys())
         for file_name in tqdm.tqdm(file_ids):
             if file_name not in supported_files:
                 raise Exception(
                     f"Unsupported file name: {file_name}."
                 )
 
         # Login to PPMI
@@ -527,34 +547,37 @@
             # Look for the guessed name
             # if not present, retrieve the guessed name from the real name
             checkbox_id = self.file_ids.get(file_name, None)
             if checkbox_id is None:
                 guess = self.real_to_guessed[file_name]
                 checkbox_id = self.file_ids.get(guess)
             for checkbox in self.driver.find_elements(By.ID, checkbox_id)[0:2]:
+                logger.debug('Click checkbox', checkbox_id, file_name)
                 checkbox.click()
+
         self.html.click_button("downloadBtn", By.ID)
 
         # Wait for download to complete
         def download_complete(driver):
             downloaded_files = os.listdir(self.tempdir.name)
             # assert len(downloaded_files) <= 1
             if len(downloaded_files) == 0:
                 return False
             for f in downloaded_files:
                 if f.endswith(".crdownload"):
                     filename = os.path.join(self.tempdir.name, f)
                     size = os.stat(filename).st_size
                     logger.debug("Size", size)
                     return False
-            assert f.endswith((".csv", ".zip")), f"file ends with: {f}"
+            # assert f.endswith((".csv", ".zip")), f"file ends with: {f}"
             return True
 
         try:
-            WebDriverWait(self.driver, timeout).until(download_complete)
+            WebDriverWait(self.driver, timeout, poll_frequency=5).until(
+                download_complete)
         except TimeoutException as e:
             self.quit()
             raise e
 
         # Move file to cwd or extract zip file
         self.html.unzip_metadata(self.tempdir.name, destination_dir)
 
@@ -567,18 +590,34 @@
 
     def __init__(self, download_dir="PPMI"):
         self.download_dir = download_dir
         # Mapping between Study Data Event IDs and imaging visit names
         self.visit_map = {
             "SC": "Screening",
             "BL": "Baseline",
+            "V01": "Month 3",
+            "V02": "Month 6",
+            "V03": "Month 9",
             "V04": "Month 12",
+            "V05": "Month 18",
             "V06": "Month 24",
+            "V07": "Month 30",
             "V08": "Month 36",
+            "V09": "Month 42",
             "V10": "Month 48",
+            "V11": "Month 54",
+            "V12": "Month 60",
+            "V13": "Month 72",
+            "V14": "Month 84",
+            "V15": "Month 96",
+            "V16": "Month 108",
+            "V17": "Month 120",
+            "V18": "Month 132",
+            "V19": "Month 144",
+            "V20": "Month 156",
             "ST": "Symptomatic Therapy",
             "U01": "Unscheduled Visit 01",
             "U02": "Unscheduled Visit 02",
             "PW": "Premature Withdrawal",
         }
 
     def __parse_xml_metadata(self, xml_file):
@@ -639,15 +678,16 @@
             )
             for child in subject:
                 if child.tag == "subjectIdentifier":
                     subject_id = child.text
                 if child.tag == "visit":
                     visit_id = parse_visit(child)
                 if child.tag == "study":
-                    study_id, series_id, image_id, description = parse_study(child)
+                    study_id, series_id, image_id, description = parse_study(
+                        child)
             assert None not in (
                 subject_id,
                 visit_id,
                 study_id,
                 series_id,
                 image_id,
                 description,
@@ -705,28 +745,25 @@
                 descr,
             ) = self.__parse_xml_metadata(xml_file)
             if (
                 (subject_id == s_id)
                 and (self.visit_map[event_id] == visit_id)
                 and (description == descr)
             ):
-                expression = op.join(
-                    self.download_dir,
-                    subject_id,
-                    clean_desc(description),
-                    "*",
-                    f"S{series_id}",
-                    f"PPMI_{subject_id}_MR_*_S{series_id}_I{image_id}.nii",
-                )
-                files = glob.glob(expression)
-                assert (
-                    len(files) == 1
-                ), f"Found {len(files)} files matching {expression} while exactly 1 was expected"
+                subject_dir = Path(self.download_dir, subject_id)
+                expression = f"**/PPMI_{subject_id}_MR_*_S{series_id}_I{image_id}.nii"
+                files = [
+                    filename
+                    for filename in subject_dir.glob(expression)
+                ]
+                if len(files) != 1:
+                    raise fileMatchingError(
+                        f"Found {len(files)} files matching {subject_dir / expression} while exactly 1 was expected\n"
+                    )
                 file_name = files[0]
-                assert op.exists(file_name), "This should never happen :)"
                 return file_name
             # else:
             #     print(f'File {xml_file} is for {(s_id, visit_id, study_id, series_id, image_id, descr)} while we are looking for {subject_id, self.visit_map[event_id], description}')
 
         return None
         # raise Exception(
         #     f"Did not find any nifti file for subject {subject_id}, event {event_id} and protocol description {description}"
```

### Comparing `ppmi_downloader-0.7.2/ppmi_downloader/ppmi_logger.py` & `ppmi_downloader-0.7.3/ppmi_downloader/ppmi_logger.py`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/ppmi_downloader/ppmi_navigator.py` & `ppmi_downloader-0.7.3/ppmi_downloader/ppmi_navigator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import os.path as op
 import shutil
 import time
 import urllib.parse
 import zipfile
 from typing import Dict, List, Callable, Any
@@ -52,21 +53,25 @@
         r'''Take screenshot of the driver current page
 
         Parameters
         ----------
         function : str
             Name of the function
         '''
-        self.driver.get_screenshot_as_file(
-            f'error-{function}-{time.time_ns()}.png')
+        time_ns = time.time_ns()
+        filename = f'error-{function}-{time_ns}'
+        with open(f'{filename}.json', 'w') as fo:
+            json.dump(self.driver.desired_capabilities, fo)
+        self.driver.get_screenshot_as_file(f'{filename}.png')
 
     def wait_for_element_to_be_visible(self, field: str,
                                        BY: By = By.XPATH,
                                        timeout: float = TIMEOUT,
-                                       debug_name: str = '') -> WebElement:
+                                       debug_name: str = '',
+                                       raise_exception: bool = False) -> WebElement:
         r'''Wait for element to be visible
 
         Parameters
         ----------
         field : str
             The field used to find the element
         BY : selenium.webdriver.common.by.By
@@ -79,19 +84,33 @@
         Returns
         -------
         WebElement
             Element found by WebDriverWait
             An Exception is raised by WebDriverWait if not
 
         '''
-        logger.debug('Wait for element to be visible', field, BY, debug_name)
-        predicate = EC.visibility_of_element_located((BY, field))
-        element = WebDriverWait(self.driver, timeout,
-                                poll_frequency=1).until(predicate)
-        return element
+        try:
+            logger.debug('Wait for element to be visible',
+                         field, BY, debug_name)
+            predicate = EC.visibility_of_element_located((BY, field))
+            element = WebDriverWait(self.driver, timeout,
+                                    poll_frequency=1).until(predicate)
+            return element
+        except TimeoutException as e:
+            if raise_exception:
+                raise e
+            self.take_screenshot('wait_for_element_visible')
+            self.driver.quit()
+            logger.error('wait for element to be visible times out')
+        except Exception as e:
+            if raise_exception:
+                raise e
+            self.take_screenshot('wait_for_element_visible')
+            self.driver.quit()
+            logger.error(f'Unknown exception {e}')
 
     def enter_data(self, field: str,
                    data: str,
                    BY: By = By.XPATH,
                    debug_name: str = '',
                    trials: int = TRIALS) -> None:
         r'''Enter data in the given field
@@ -310,32 +329,33 @@
         password : str
             Users's password
 
         '''
         self.validate_cookie_policy()
         self.driver.get(ppmi_login_webpage)
         try:
-            self.wait_for_element_to_be_visible(
-                'ida-user-username', BY=By.CLASS_NAME)
+            self.wait_for_element_to_be_visible('ida-menu-option.sub-menu.user',
+                                                BY=By.CLASS_NAME,
+                                                raise_exception=True)
             logger.debug('Already logged in')
             return
         except (NoSuchElementException, TimeoutException):
             pass
 
         self.wait_for_element_to_be_visible('userEmail', BY=By.NAME)
         self.enter_data("userEmail", email, BY=By.NAME, debug_name='Email')
         self.wait_for_element_to_be_visible('userPassword', BY=By.NAME)
         self.enter_data("userPassword", password,
                         BY=By.NAME, debug_name='Password')
         self.wait_for_element_to_be_visible('button', BY=By.TAG_NAME)
         self.click_button("button", By.TAG_NAME, debug_name='Login button')
 
         try:
-            self.driver.find_element(
-                By.CLASS_NAME, 'register-input-error-msg.invalid-login')
+            self.driver.find_element(By.CLASS_NAME,
+                                     'register-input-error-msg.invalid-login')
             logger.error('Login Failed')
         except NoSuchElementException:
             logger.info('Login Successful')
 
     def unzip_file(self, filename: str, tempdir: str, destination_dir: str) -> None:
         r'''Helper function to unzip a file
 
@@ -370,19 +390,28 @@
         ----------
         source_dir : str
             Name of the directory where metadata are located
         destination_dir : str
             Name of the directory where to copy files
 
         '''
-        # Move file to cwd or extract zip file
-        downloaded_files = os.listdir(source_dir)
-        # we got either a csv or a zip file
-        assert len(downloaded_files) == 1
-        file_name = downloaded_files[0]
+        i = 0
+        is_metadata_ext = False
+        # Do check since sometimes we still have the temporary name
+        # used during downloading
+        while not is_metadata_ext and i < 10:
+            # Move file to cwd or extract zip file
+            downloaded_files = os.listdir(source_dir)
+            # we got either a csv or a zip file
+            assert len(downloaded_files) == 1
+            file_name = downloaded_files[0]
+            is_metadata_ext = file_name.endswith((".zip", ".csv"))
+            time.sleep(.5)
+            i += 1
+
         assert file_name.endswith((".zip", ".csv"))
         self.unzip_file(file_name, source_dir, destination_dir)
         return file_name
 
     def unzip_imaging_data(self, downloaded_files: List[str], tempdir: str, destination_dir: str) -> None:
         r'''Helper function to unzip imaging data
 
@@ -532,14 +561,27 @@
             return self.is_element_active('ida-menu-option.sub-menu.download')
 
         while not postcondition():
             self.click_button('ida-menu-option.sub-menu.download',
                               BY=By.CLASS_NAME,
                               debug_name='Download Hamburger submenu')
 
+    def HamburgerMenu_Search(self) -> None:
+        r'''Action to click on "Download" in HamburgerMenu
+
+        Click on button until postcondition is not met
+        '''
+        def postcondition() -> bool:
+            return self.is_element_active('ida-menu-option.sub-menu.search')
+
+        while not postcondition():
+            self.click_button('ida-menu-option.sub-menu.search',
+                              BY=By.CLASS_NAME,
+                              debug_name='Search Hamburger submenu')
+
     def Download(self) -> None:
         r'''Action to click on "Download"
 
         Action detects if HamburgerMenu is enabled or not
         to click on the correct Download button
         Click on button until postcondition is not met
         '''
@@ -570,15 +612,15 @@
         r'''Action to click on "All" in "Study Data" in "Download"
 
         Precondition: StudyData action
         Click on button until postcondition is not met
         '''
         studydata_url = 'https://ida.loni.usc.edu/pages/access/studyData.jsp'
         while self.driver.current_url != studydata_url:
-            self.click_button("ygtvlabelel71", BY=By.ID, debug_name='ALL')
+            self.click_button("ygtvlabelel74", BY=By.ID, debug_name='ALL')
 
     def Download_ImageCollections(self) -> None:
         r'''Action to click on "Image Collections" in "Download"
 
         Precondition: Download action
         Click on button until postcondition is not met
         '''
@@ -609,14 +651,18 @@
                                       debug_name='Generic Data')
 
     def Search(self) -> None:
         r'''Action to click on "Search"
 
         Click on button until postcondition is not met
         '''
+        if self.has_HamburgerMenu():
+            self.HamburgerMenu()
+            self.HamburgerMenu_Search()
+
         def postcondition() -> bool:
             try:
                 name = 'ida-menu-option.sub-menu.search.active'
                 predicate = EC.presence_of_element_located(
                     (By.CLASS_NAME, name))
                 WebDriverWait(self.driver, 2,
                               poll_frequency=1).until(predicate)
```

### Comparing `ppmi_downloader-0.7.2/ppmi_downloader/selenium_grid_utils.py` & `ppmi_downloader-0.7.3/ppmi_downloader/selenium_grid_utils.py`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/LICENSE` & `ppmi_downloader-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/README.md` & `ppmi_downloader-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ppmi_downloader-0.7.2/pyproject.toml` & `ppmi_downloader-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pathspec"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ppmi_downloader"
-version = "0.7.2"
+version = "0.7.3"
 description = "A downloader of PPMI files."
 authors = [{ name = "Tristan Glatard", email = "tristan.glatard@concordia.ca" }]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ppmi_downloader-0.7.2/PKG-INFO` & `ppmi_downloader-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppmi_downloader
-Version: 0.7.2
+Version: 0.7.3
 Summary: A downloader of PPMI files.
 Project-URL: Bug Tracker, https://github.com/LivingPark-MRI/ppmi-scraper/issues
 Author-email: Tristan Glatard <tristan.glatard@concordia.ca>
 License: MIT License
         
         Copyright (c) 2022 Tristan Glatard, Mohanad Arafe
```

