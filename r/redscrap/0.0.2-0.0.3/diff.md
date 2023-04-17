# Comparing `tmp/redscrap-0.0.2-py3-none-any.whl.zip` & `tmp/redscrap-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,44 @@
-Zip file size: 41240 bytes, number of entries: 37
+Zip file size: 43563 bytes, number of entries: 42
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 21:27 __init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 23:07 common/__init__.py
--rw-r--r--  2.0 unx    10434 b- defN 23-Apr-15 16:45 common/common_constants.py
--rw-r--r--  2.0 unx      868 b- defN 23-Apr-07 15:00 common/exceptions.py
--rw-r--r--  2.0 unx     7957 b- defN 23-Apr-15 18:46 common/image_downloader.py
--rw-r--r--  2.0 unx    11726 b- defN 23-Apr-15 16:45 common/io_operations.py
--rw-r--r--  2.0 unx     2064 b- defN 23-Apr-15 16:10 common/request_manager.py
--rw-r--r--  2.0 unx     1640 b- defN 23-Apr-15 16:12 common/string_builder.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 15:16 common/constants/__init__.py
+-rw-r--r--  2.0 unx    14149 b- defN 23-Apr-17 14:38 common/constants/common_constants.py
+-rw-r--r--  2.0 unx    16883 b- defN 23-Apr-17 11:30 common/constants/logging_constants.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 15:18 common/exceptions/__init__.py
+-rw-r--r--  2.0 unx     1107 b- defN 23-Apr-16 09:33 common/exceptions/main_exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 14:24 common/io_operations/__init__.py
+-rw-r--r--  2.0 unx     8697 b- defN 23-Apr-17 15:16 common/io_operations/image_downloader.py
+-rw-r--r--  2.0 unx    12460 b- defN 23-Apr-17 15:16 common/io_operations/io_operations.py
+-rw-r--r--  2.0 unx     2064 b- defN 23-Apr-15 16:10 common/io_operations/request_manager.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 10:01 common/logging/__init__.py
--rw-r--r--  2.0 unx    16881 b- defN 23-Apr-15 16:49 common/logging/logging_constants.py
--rw-r--r--  2.0 unx     9753 b- defN 23-Apr-15 16:49 common/logging/logging_setup.py
--rw-r--r--  2.0 unx     5992 b- defN 23-Apr-15 18:45 common/logging/loguru_setup.py
+-rw-r--r--  2.0 unx     9755 b- defN 23-Apr-17 15:17 common/logging/logging_setup.py
+-rw-r--r--  2.0 unx     6015 b- defN 23-Apr-17 15:17 common/logging/loguru_setup.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 13:26 common/logging/utils/__init__.py
 -rw-r--r--  2.0 unx      992 b- defN 23-Apr-14 21:28 common/logging/utils/color_formatter.py
 -rw-r--r--  2.0 unx     1615 b- defN 23-Apr-15 16:07 common/logging/utils/log_rotator.py
 -rw-r--r--  2.0 unx     1182 b- defN 23-Apr-14 22:20 common/logging/utils/logging_wrappers.py
 -rw-r--r--  2.0 unx     2092 b- defN 23-Apr-15 18:33 common/logging/utils/loguru_wrappers.py
--rw-r--r--  2.0 unx     1286 b- defN 23-Apr-15 16:49 common/logging/utils/padding_formatter.py
+-rw-r--r--  2.0 unx     1288 b- defN 23-Apr-17 15:17 common/logging/utils/padding_formatter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-17 15:17 common/utils/__init__.py
+-rw-r--r--  2.0 unx     1640 b- defN 23-Apr-15 16:12 common/utils/string_builder.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 23:07 common/validations/__init__.py
--rw-r--r--  2.0 unx     6554 b- defN 23-Apr-15 18:44 common/validations/parameter_validations.py
--rw-r--r--  2.0 unx     9371 b- defN 23-Apr-15 19:02 common/validations/reddit_api_validations.py
--rw-r--r--  2.0 unx     3507 b- defN 23-Apr-15 16:45 common/validations/url_validations.py
+-rw-r--r--  2.0 unx     6703 b- defN 23-Apr-17 15:26 common/validations/parameter_validations.py
+-rw-r--r--  2.0 unx     6889 b- defN 23-Apr-17 15:28 common/validations/reddit_api_validations.py
+-rw-r--r--  2.0 unx     3517 b- defN 23-Apr-17 15:16 common/validations/url_validations.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 21:27 core/__init__.py
--rw-r--r--  2.0 unx     3408 b- defN 23-Apr-15 16:49 core/main.py
+-rw-r--r--  2.0 unx     4647 b- defN 23-Apr-17 15:17 core/main.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-08 10:02 core/api/__init__.py
--rw-r--r--  2.0 unx     6035 b- defN 23-Apr-15 19:01 core/api/reddit_api.py
+-rw-r--r--  2.0 unx     6018 b- defN 23-Apr-17 15:28 core/api/reddit_api.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 19:19 core/helper/__init__.py
--rw-r--r--  2.0 unx    10084 b- defN 23-Apr-15 18:59 core/helper/main_helper.py
+-rw-r--r--  2.0 unx    11320 b- defN 23-Apr-17 15:26 core/helper/main_helper.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 16:57 core/scraper/__init__.py
--rw-r--r--  2.0 unx     9471 b- defN 23-Apr-15 19:39 core/scraper/comment_scraper.py
--rw-r--r--  2.0 unx     8435 b- defN 23-Apr-15 19:17 core/scraper/scraper_helper.py
--rw-r--r--  2.0 unx    11386 b- defN 23-Apr-15 18:46 core/scraper/thread_scraper.py
--rw-r--r--  2.0 unx     1129 b- defN 23-Apr-15 21:35 redscrap-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 21:35 redscrap-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-Apr-15 21:35 redscrap-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-15 21:35 redscrap-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3107 b- defN 23-Apr-15 21:35 redscrap-0.0.2.dist-info/RECORD
-37 files, 147126 bytes uncompressed, 36242 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx     9431 b- defN 23-Apr-17 16:11 core/scraper/comment_scraper.py
+-rw-r--r--  2.0 unx    10874 b- defN 23-Apr-17 16:39 core/scraper/scraper_helper.py
+-rw-r--r--  2.0 unx     9415 b- defN 23-Apr-17 16:37 core/scraper/thread_scraper.py
+-rw-r--r--  2.0 unx     1089 b- defN 23-Apr-17 17:48 redscrap-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1151 b- defN 23-Apr-17 17:48 redscrap-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 17:48 redscrap-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-Apr-17 17:48 redscrap-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-17 17:48 redscrap-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3602 b- defN 23-Apr-17 17:48 redscrap-0.0.3.dist-info/RECORD
+42 files, 154752 bytes uncompressed, 37743 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,35 +1,41 @@
 Filename: __init__.py
 Comment: 
 
 Filename: common/__init__.py
 Comment: 
 
-Filename: common/common_constants.py
+Filename: common/constants/__init__.py
 Comment: 
 
-Filename: common/exceptions.py
+Filename: common/constants/common_constants.py
 Comment: 
 
-Filename: common/image_downloader.py
+Filename: common/constants/logging_constants.py
 Comment: 
 
-Filename: common/io_operations.py
+Filename: common/exceptions/__init__.py
 Comment: 
 
-Filename: common/request_manager.py
+Filename: common/exceptions/main_exceptions.py
 Comment: 
 
-Filename: common/string_builder.py
+Filename: common/io_operations/__init__.py
 Comment: 
 
-Filename: common/logging/__init__.py
+Filename: common/io_operations/image_downloader.py
+Comment: 
+
+Filename: common/io_operations/io_operations.py
 Comment: 
 
-Filename: common/logging/logging_constants.py
+Filename: common/io_operations/request_manager.py
+Comment: 
+
+Filename: common/logging/__init__.py
 Comment: 
 
 Filename: common/logging/logging_setup.py
 Comment: 
 
 Filename: common/logging/loguru_setup.py
 Comment: 
@@ -48,14 +54,20 @@
 
 Filename: common/logging/utils/loguru_wrappers.py
 Comment: 
 
 Filename: common/logging/utils/padding_formatter.py
 Comment: 
 
+Filename: common/utils/__init__.py
+Comment: 
+
+Filename: common/utils/string_builder.py
+Comment: 
+
 Filename: common/validations/__init__.py
 Comment: 
 
 Filename: common/validations/parameter_validations.py
 Comment: 
 
 Filename: common/validations/reddit_api_validations.py
@@ -90,23 +102,26 @@
 
 Filename: core/scraper/scraper_helper.py
 Comment: 
 
 Filename: core/scraper/thread_scraper.py
 Comment: 
 
-Filename: redscrap-0.0.2.dist-info/METADATA
+Filename: redscrap-0.0.3.dist-info/LICENSE
+Comment: 
+
+Filename: redscrap-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: redscrap-0.0.2.dist-info/WHEEL
+Filename: redscrap-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: redscrap-0.0.2.dist-info/entry_points.txt
+Filename: redscrap-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: redscrap-0.0.2.dist-info/top_level.txt
+Filename: redscrap-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: redscrap-0.0.2.dist-info/RECORD
+Filename: redscrap-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## common/logging/logging_setup.py

```diff
@@ -1,14 +1,14 @@
 import logging
 import sys
 from logging import handlers
 import colorama     # type: ignore
 from colorama import Fore, Back, Style
 
-from common.logging.logging_constants import LoggingConstants      # type: ignore
+from common.constants.logging_constants import LoggingConstants      # type: ignore
 
 logging_constants = LoggingConstants()
 
 
 class FilterByModule(logging.Filter):
     """
     custom filter class called FilterByModule that inherits from logging.Filter. The filter method of this class
```

## common/logging/loguru_setup.py

```diff
@@ -1,12 +1,12 @@
 import sys
 
-from common.logging.logging_constants import LoggingConstants      # type: ignore
-from common.logging.utils.log_rotator import LogRotator      # type: ignore
-from common.logging.utils.padding_formatter import PaddingFormatter      # type: ignore
+from common.constants.logging_constants import LoggingConstants  # type: ignore
+from common.logging.utils.log_rotator import LogRotator  # type: ignore
+from common.logging.utils.padding_formatter import PaddingFormatter  # type: ignore
 
 constants = LoggingConstants()
 
 
 class LoguruSetup:
     """
     A class to set up logging for scripts.
@@ -22,33 +22,33 @@
         """
         Initializes LoggingSetup class.
         """
         super().__init__()
 
     @staticmethod
     def script_logger_config_dict(
-        logger,
-        output_directory: str,
-        log_filename: str,
-        level: str = constants.default_log_file_level,
-        log_format: str = constants.default_log_format,
-        colorize: bool = constants.default_log_colorizing,
-        rotation: str = constants.default_log_rotation,
-        retention: str = constants.default_log_retention,
-        compression: str = constants.default_log_compression,
-        delay: bool = constants.default_log_delay,
-        mode: str = constants.default_log_mode,
-        buffering: int = constants.default_log_buffering,
-        encoding: str = constants.default_log_encoding,
-        serialize: bool = constants.default_log_serialize,
-        backtrace: bool = constants.default_log_backtrace,
-        diagnose: bool = constants.default_log_diagnose,
-        enqueue: bool = constants.default_log_enqueue,
-        catch: bool = constants.default_log_catch,
-        debug: bool = False,
+            logger,
+            output_directory: str,
+            log_filename: str,
+            level: str = constants.default_log_file_level,
+            log_format: str = constants.default_log_format,
+            colorize: bool = constants.default_log_colorizing,
+            rotation: float = constants.default_log_rotation,
+            retention: str = constants.default_log_retention,
+            compression: str = constants.default_log_compression,
+            delay: bool = constants.default_log_delay,
+            mode: str = constants.default_log_mode,
+            buffering: int = constants.default_log_buffering,
+            encoding: str = constants.default_log_encoding,
+            serialize: bool = constants.default_log_serialize,
+            backtrace: bool = constants.default_log_backtrace,
+            diagnose: bool = constants.default_log_diagnose,
+            enqueue: bool = constants.default_log_enqueue,
+            catch: bool = constants.default_log_catch,
+            debug: bool = False,
     ):
         """
         Creates configuration object for scripts to setup logging.
 
         Args:
             output_directory:
             logger (Any): the logging object.
@@ -113,16 +113,15 @@
             "catch": catch,
         }
 
         config = {
             "handlers": [
                 sys_stdout_handler,
                 log_file_handler,
-            ],
-            # "extra": {"user": "someone"}
+            ]
         }
 
         logger.level("TRACE", color="<dim>", icon=constants.rocket_symbol)
         logger.level("DEBUG", color="<dim><cyan>", icon=constants.bug_symbol)
         logger.level("INFO", color="", icon=constants.info_symbol)
         logger.level("SUCCESS", icon=constants.green_circle_symbol)
         logger.level("WARNING", color="<yellow>", icon=constants.lightning_bolt_symbol)
```

## common/logging/utils/padding_formatter.py

```diff
@@ -1,10 +1,10 @@
 import loguru
 
-from common.logging.logging_constants import LoggingConstants      # type: ignore
+from common.constants.logging_constants import LoggingConstants      # type: ignore
 
 logging_constants = LoggingConstants()
 
 
 class PaddingFormatter:
     """
     A logging formatter that adjusts padding length based on previously encountered values.
```

## common/validations/parameter_validations.py

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional
 from loguru import logger        # type: ignore
 import re
 import requests      # type: ignore
 
-from common.exceptions import SubredditNotFoundException         # type: ignore
+from common.exceptions.main_exceptions import SubredditNotFoundException         # type: ignore
 from common.logging.logging_setup import LoggingSetup        # type: ignore
-from common.common_constants import CommonConstants      # type: ignore
+from common.constants.common_constants import CommonConstants      # type: ignore
 from common.logging.utils.loguru_wrappers import logger_wraps        # type: ignore
 from core.api.reddit_api import RedditApi        # type: ignore
 
 
 class ParameterValidations:
     """
         A class that provides method to validate the application parameters
@@ -54,18 +54,20 @@
         """
         logger.debug("[2] VALIDATING PARAMS SET")
 
         # Remove white spaces
         sanitized_string = input_str.replace(" ", "")
 
         # Replace consecutive commas or semicolons with a single comma
-        sanitized_string = re.sub(r"[,;]+", ",", sanitized_string)
+        sanitized_string = re.sub(self.main_constants.replace_consecutive_commas_or_semicolons_regex,
+                                  ",", sanitized_string)
 
         # Remove any remaining empty groups
-        sanitized_string = re.sub(r"(^,)|(,$)|(^;)|(;$)|,{2,}", "", sanitized_string)
+        sanitized_string = re.sub(self.main_constants.remove_empty_groups_from_comma_or_semicolon_separated_string
+                                  , "", sanitized_string)
 
         # Check if the string contains any special characters
         pattern = self.main_constants.validate_and_split_string_regex
         if bool(re.match(pattern, sanitized_string)) is False:
             raise ValueError(
                 "Input string contains special characters other than commas and semicolons."
             )
@@ -135,18 +137,16 @@
 
         Args:
             reddit_user (str): The name of the user to check.
 
         Returns:
             bool: True if the user exists, False otherwise.
         """
-        url: str = "https://www.reddit.com/user/{}/about.json".format(reddit_user)
-        headers: dict[str, str] = {
-            "User-Agent": "Mozilla/5.0:com.martimdlima.redscrappy:v0.0.1 (by /u/mdlima__)"
-        }
+        url: str = "{}/user/{}/about.json".format(self.main_constants.reddit_url, reddit_user)
+        headers: dict[str, str] = self.main_constants.reddit_headers
 
         response = requests.get(url, headers=headers)
 
         if response.status_code == 200:
             logger.debug("USER EXISTS", True)
             # User exists
             exists = True
```

## common/validations/reddit_api_validations.py

```diff
@@ -1,16 +1,17 @@
 from typing import Optional, List
 from loguru import logger       # type: ignore
 import requests     # type: ignore
 import json
 
-from common.exceptions import SubredditNotFoundException, UserNotFoundException     # type: ignore
+from common.exceptions.main_exceptions import SubredditNotFoundException, UserNotFoundException, \
+    TokenErrorException  # type: ignore
 from common.logging.logging_setup import LoggingSetup   # type: ignore
-from common.common_constants import CommonConstants     # type: ignore
-from common.exceptions import TokenErrorException   # type: ignore
+from common.constants.common_constants import CommonConstants     # type: ignore
+from common.io_operations.request_manager import RequestManager
 from core.api.reddit_api import RedditApi       # type: ignore
 
 
 class RedditApiValidations:
     """
     A class that provides a number of methods to expose the reddit API
 
@@ -29,195 +30,118 @@
             Checks if the given username exists on Reddit API.
     """
 
 
     def __init__(self):
         self.logging_setup = LoggingSetup()
         self.main_constants = CommonConstants()
+        self.request_manager = RequestManager()
         self.reddit_api = RedditApi(self.main_constants.client_id, self.main_constants.secret_token,
                                     self.main_constants.username, self.main_constants.password)
 
-    def validate_subreddits_list(self, subreddits: List[str]):
+    def validate_subreddits_list(self, subreddits: List[str], verbose: bool):
         """
         Validates a list of subreddits
 
         Args:
             subreddits (str): list of comma or semicolon separated values
+            verbose (bool): Controls the verbosity level
         """
         logger.debug("[4] VALIDATE SUBREDDITS STEP")
 
         for sub_red in subreddits:
-            if self.validate_subreddit(sub_red) is False:
+            if self.validate_subreddit(sub_red, verbose) is False:
                 message = "The provided subreddit {} was not found. Please provide a valid one".format(sub_red)
                 raise SubredditNotFoundException(message)
 
-    def validate_subreddit(self, subreddit: str):
-        """
-        Validates if a subreddit exists
-
-        Args:
-            subreddit (str): the subreddit to validate
-        """
-        url = "https://www.reddit.com/r/{}.json".format(subreddit)
-        response = requests.get(url, headers=self.main_constants.user_agent)
-        is_valid: bool = False
-
-        if response.status_code == 200:
-            try:
-                data = response.json()
-                if len(data["data"]["children"]) > 0:
-                    msg = "SUBREDDIT {}: {}".format(subreddit, self.main_constants.check_mark_symbol)
-                    logger.debug(msg)
-                    is_valid = True
-            except ValueError:
-                pass
-        else:
-            msg = "SUBREDDIT {}: {}".format(subreddit, self.main_constants.cross_symbol)
-            logger.debug(msg)
-            is_valid = False
-        return is_valid
+        logger.info(
+            "Validation step: {}".format(self.main_constants.check_mark_symbol)) if verbose else None
 
-    def check_if_subreddit_exists(self, token: str, subreddit: str) -> Optional[bool]:
+    def validate_subreddit(self, subreddit: str, verbose: bool) -> Optional[bool]:
         """
         Checks if the given subreddit exists on Reddit API.
 
         Args:
-            token (str): The OAuth token for Reddit API.
             subreddit (str): The name of the subreddit to check.
+            verbose: (bool): Controls the verbosity level
 
         Returns:
             bool: True if the subreddit exists, False otherwise.
 
         Notes:
             According to Reddit's API rules changed the client's User-Agent string to something unique and descriptive,
             including the target platform, a unique application identifier, a version string, and your username
             as contact information, in the following format
         """
 
         # add authorization to our headers dictionary
+        url = "{}/r/{}/about".format(self.main_constants.reddit_api_base_url, subreddit)
+        token = self.reddit_api.generate_reddit_api_token(verbose)
         headers = self.reddit_api.generate_headers(token)
-        url = "https://oauth.reddit.com/r/{}/about".format(subreddit)
-        res = requests.get(url, headers=headers)
-        exists = None
+        res = self.request_manager.request_page(url, headers)
+
+        is_valid: bool = False
         if res.status_code == 200:
             res_dict = json.loads(res.text)
             res_data = res_dict["data"]
 
             if res_data.get("url") is not None:
                 logger.debug(
                     "SUBREDDIT {}: {}".format(subreddit, self.main_constants.check_mark_symbol))
-                exists = True
+                logger.info(
+                    "Validating subreddit {}: {}".format(subreddit, self.main_constants.check_mark_symbol)) \
+                    if verbose else None
+                is_valid = True
             else:
                 logger.debug(
                     "SUBREDDIT {}: {}".format(subreddit, self.main_constants.cross_symbol))
-                exists = False
-        return exists
+                logger.info(
+                    "Validating {}: {}".format(subreddit, self.main_constants.cross_symbol)) if verbose else None
+                is_valid = False
+        return is_valid
 
     def validate_reddit_user(self, reddit_user: str, verbose: bool) -> Optional[bool]:
         """
         Checks if the given username exists on Reddit API.
 
         Args:
             reddit_user (str): The name of the user to check.
-            verbose (bool): If True, logs the result of the check to the console.
+            verbose (bool): Controls the verbosity level
 
         Returns:
             bool: True if the user exists, False otherwise.
 
         Notes:
             According to Reddit's API rules changed the client's User-Agent string to something unique and descriptive,
             including the target platform, a unique application identifier, a version string, and your username
             as contact information, in the following format
 
-            This validation can also be accomplished by targeting this endpoints:
+            this check can also be accomplished by targeting this endpoint:
                 url = "{constants.reddit_api_base_url}/api/v1/user/{username}/trophies"
-                url: str = "https://www.reddit.com/user/{reddit_user}/about.json"
         """
 
-        is_valid = False
-
+        url: str = "{}/api/username_available.json?user={}".format(
+            self.main_constants.reddit_api_base_url, reddit_user)
         token = self.reddit_api.generate_reddit_api_token(verbose)
+        headers = self.reddit_api.generate_headers(token)
+        res = self.request_manager.request_page(url, headers)
 
-        # add authorization to our headers dictionary
-        headers: dict[str, str] = self.reddit_api.generate_headers(token)
-
-        url: str = "{}/api/username_available?user={}".format(self.main_constants.reddit_api_base_url, reddit_user)
-
-        logger.debug("REQUESTING URL: {}".format(url))
-        res = requests.get(url, headers=headers)
+        exists: bool = False
 
         if res.status_code == 200:
             # If the enpoint returns False, it means the username isn't available and as such the user exists
-            logger.debug("USER {} EXISTS: {}".format(reddit_user, self.main_constants.check_mark_symbol))
-            is_valid = True
-
-        logger.debug("STATUS_CODE: {}, IS_VALID: {}".format(res.status_code, is_valid))
-
-        if res.status_code == 403:
-            raise UserNotFoundException("Reddit User not Found")
-
-        return is_valid
-
-    def validate_user(self, token: str, reddit_user: str) -> Optional[bool]:
-        """
-        Checks if the given username exists on Reddit API.
-
-        Args:
-            token (str): The OAuth token for Reddit API.
-            reddit_user (str): The name of the user to check.
-
-        Returns:
-            bool: True if the user exists, False otherwise.
-
-        Notes:
-            According to Reddit's API rules changed the client's User-Agent string to something unique and descriptive,
-            including the target platform, a unique application identifier, a version string, and your username
-            as contact information, in the following format
-
-            this check can also be accomplished by targeting this endpoint:
-                url = "{constants.reddit_api_base_url}/api/v1/user/{username}/trophies"
-        """
-
-        url: str = "{}/api/username_available?user={}".format(self.main_constants.reddit_api_base_url, reddit_user)
-
-        # add authorization to our headers dictionary
-        headers = self.reddit_api.generate_headers(token)
-
-        res = requests.get(url, headers=headers)
-        exists = None
-        if res.status_code == 200:
-            if res is False:
-                # If the enpoint returns False, it means the username isn't available and as such the user exists
-                msg = "USER {} EXISTS: {}".format(reddit_user, self.main_constants.check_mark_symbol)
-                logger.debug(msg)
+            if res.json() is False:
                 exists = True
+                debug_msg = "USER {} EXISTS: {}".format(reddit_user, self.main_constants.check_mark_symbol)
+                info_msg = "User: {}: {}".format(reddit_user,
+                                                 self.main_constants.check_mark_symbol)
+                logger.debug(debug_msg)
+                logger.info(info_msg) if verbose else None
             else:
-                msg = "USER {} DOESN'T EXISTS: {}".format(reddit_user, self.main_constants.cross_symbol)
-                logger.debug(msg)
-                exists = False
-        return exists
-
-    def validate_user_v2(self, reddit_user: str) -> Optional[bool]:
-        """
-        Checks if the given username exists on Reddit API.
-
-        Args:
-            reddit_user (str): The name of the user to check.
+                debug_msg = "USER {} DOESN'T EXISTS: {}".format(reddit_user, self.main_constants.cross_symbol)
+                info_msg = "User: {}: {}".format(reddit_user,
+                                                 self.main_constants.cross_symbol)
+                logger.debug(debug_msg)
+                logger.info(info_msg) if verbose else None
+                raise UserNotFoundException("Reddit user {} not Found".format(reddit_user))
 
-        Returns:
-            bool: True if the user exists, False otherwise.
-        """
-        url: str = "https://www.reddit.com/user/{}/about.json".format(reddit_user)
-        headers: dict[str, str] = {
-            "User-Agent": "Mozilla/5.0:com.martimdlima.redscrappy:v0.0.1 (by /u/mdlima__)"
-        }
-
-        response = requests.get(url, headers=headers)
-        if response.status_code == 200:
-            logger.debug("USER EXISTS", True)
-            # User exists
-            exists = True
-        else:
-            logger.debug("USER DOESN'T EXIST", True)
-            # User does not exist
-            exists = False
         return exists
```

## common/validations/url_validations.py

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional
 import re
 import validators  # type: ignore
 from loguru import logger  # type: ignore
 
 from common.logging.logging_setup import LoggingSetup  # type: ignore
-from common.common_constants import CommonConstants  # type: ignore
+from common.constants.common_constants import CommonConstants  # type: ignore
 
 logging_setup = LoggingSetup()
 constants = CommonConstants()
 
 
 class UrlValidations:
     """
```

## core/main.py

```diff
@@ -1,44 +1,78 @@
 from pathlib import Path
 from loguru import logger  # type: ignore
 import click
 
 # import logging
-from common.io_operations import IOOperations  # type: ignore
+from common.io_operations.io_operations import IOOperations  # type: ignore
 from common.logging.loguru_setup import LoguruSetup  # type: ignore
-from common.logging.logging_constants import LoggingConstants  # type: ignore
+from common.constants.logging_constants import LoggingConstants  # type: ignore
 from core.helper.main_helper import MainHelper
 
 logging_constants = LoggingConstants()
 io_operations = IOOperations()
 main_helper = MainHelper()
 
+main = click.Group(help="JSON tools")
 
-@click.command()
+
+@main.command("user", help="Scrape user threads")
+@click.argument('reddit_user', type=str, nargs=-1)
+@click.option("-n", "--number_results", type=int, help="Number of threads to scrape")
+@click.option("-s", "--sorting_filter", type=click.Choice(["top", "hot", "new"]), default="hot", help="Filter threads")
+@click.option("-o", "--output", type=str, help="The directory to output the downloads")
+@click.option("-v", "--verbose", is_flag=True, default=False, help="Enables verbose mode")
+def main_scrape_user(number_results, sorting_filter, reddit_user, output, verbose):
+    # Setups directories used in the application
+    with logger.catch(reraise=True):
+        logger.remove()
+        output_directory = io_operations.init_directories(output)
+
+    # Setups logging for the application
+    LoguruSetup.script_logger_config_dict(
+        logger,
+        output_directory,
+        Path(logging_constants.log_filename).name,
+        logging_constants.default_log_stfout_level,
+        logging_constants.default_log_format,
+        logging_constants.default_log_colorizing,
+        logging_constants.default_log_rotation,
+        logging_constants.default_log_retention,
+        logging_constants.default_log_compression,
+        logging_constants.default_log_delay,
+        logging_constants.default_log_mode,
+        logging_constants.default_log_buffering,
+        logging_constants.default_log_encoding,
+        logging_constants.default_log_serialize,
+        logging_constants.default_log_backtrace,
+        logging_constants.default_log_diagnose,
+        logging_constants.default_log_enqueue,
+        logging_constants.default_log_catch,
+        False,  # enables/disables debug mode logs
+    )
+
+    main_helper.scrape_user(
+        "".join(reddit_user) if len(reddit_user) > 0 else None,
+        sorting_filter, number_results, output_directory, verbose)
+
+
+@main.command("subreddits", help="Scrape subreddits threads")
+@click.argument('subreddits', type=str, nargs=-1)
 @click.option("-n", "--number_results", type=int, help="Number of threads to scrape")
-@click.option("-x", "--scrape", type=click.Choice(["user", "subreddits"]), default="hot",
-              help="Scrape user or subreddit")
 @click.option("-s", "--sorting_filter", type=click.Choice(["top", "hot", "new"]), default="hot", help="Filter threads")
-@click.option("-u", "--reddit_user", type=str, help="The reddit user to search")
-@click.option("-r", "--subreddits", type=str, help="The subreddit/s to search")
 @click.option("-d", "--details", is_flag=True, default=False,
               help="If enable outputs the detailed list of threads of each subreddit provided into an individual file")
 @click.option("-o", "--output", type=str, help="The directory to output the downloads")
 @click.option("-v", "--verbose", is_flag=True, default=False, help="Enables verbose mode")
-def main(number_results, scrape, sorting_filter, reddit_user, subreddits, details, output, verbose):
-    """
-    Script main entry point
-    """
-
+def main_scrape_subreddits(number_results, sorting_filter, subreddits, details, output, verbose):
     # Setups directories used in the application
     with logger.catch(reraise=True):
         logger.remove()
         output_directory = io_operations.init_directories(output)
 
-    logger.debug("[1] - STARTING reddit_scrapper")
 
     # Setups logging for the application
     LoguruSetup.script_logger_config_dict(
         logger,
         output_directory,
         Path(logging_constants.log_filename).name,
         logging_constants.default_log_stfout_level,
@@ -55,24 +89,14 @@
         logging_constants.default_log_backtrace,
         logging_constants.default_log_diagnose,
         logging_constants.default_log_enqueue,
         logging_constants.default_log_catch,
         False,  # enables/disables debug mode logs
     )
 
-    # Scrapes a user or subreddit
-    match scrape:
-        case "user":
-            if not reddit_user:
-                msg = "If you want to scrape a user profile you must provide a reddit user"
-                raise click.exceptions.UsageError(msg)
-            else:
-                main_helper.scrape_user(reddit_user, sorting_filter, number_results, output_directory, verbose)
-
-        case "subreddits":
-            main_helper.scrape_subreddit(subreddits, sorting_filter, number_results, details, output_directory,  verbose)
-
-    logger.debug("[10] - ENDING reddit_scrapper")
+    main_helper.scrape_subreddit(
+        ", ".join(subreddits) if len(subreddits) > 0 else None
+        , sorting_filter, number_results, details, output_directory, verbose)
 
 
 if __name__ == "__main__":
-    main()  # pylint: disable=no-value-for-parameter
+    exit(main())  # pylint: disable=no-value-for-parameter
```

## core/api/reddit_api.py

```diff
@@ -1,16 +1,16 @@
 import logging
 from typing import Optional, Dict, Union
 from loguru import logger       # type: ignore
 import requests     # type: ignore
 
-from common.exceptions import SubredditNotFoundException, UserNotFoundException     # type: ignore
+from common.exceptions.main_exceptions import SubredditNotFoundException, \
+    UserNotFoundException, TokenErrorException  # type: ignore
 from common.logging.logging_setup import LoggingSetup   # type: ignore
-from common.common_constants import CommonConstants     # type: ignore
-from common.exceptions import TokenErrorException   # type: ignore
+from common.constants.common_constants import CommonConstants     # type: ignore
 
 
 class RedditApi:
     """
         A class that provides functions to access Reddit API.
 
     Methods:
```

## core/helper/main_helper.py

```diff
@@ -1,18 +1,19 @@
 import glob
 from pathlib import Path
 from typing import Any, Optional, List, Iterable
 from loguru import logger  # type: ignore
 from bs4 import ResultSet
 
-from common.image_downloader import ImageDownloader  # type: ignore
-from common.io_operations import IOOperations  # type: ignore
+from common.exceptions.main_exceptions import MissingRequiredParameter
+from common.io_operations.image_downloader import ImageDownloader  # type: ignore
+from common.io_operations.io_operations import IOOperations  # type: ignore
 from common.logging.loguru_setup import LoguruSetup  # type: ignore
-from common.logging.logging_constants import LoggingConstants  # type: ignore
-from common.common_constants import CommonConstants  # type: ignore
+from common.constants.logging_constants import LoggingConstants  # type: ignore
+from common.constants.common_constants import CommonConstants  # type: ignore
 from common.validations.parameter_validations import ParameterValidations  # type: ignore
 from common.validations.reddit_api_validations import RedditApiValidations  # type: ignore
 from core.api.reddit_api import RedditApi  # type: ignore
 from core.scraper.thread_scraper import ThreadScraper  # type: ignore
 from core.scraper.scraper_helper import ScraperHelper   # type: ignore
 
 
@@ -61,14 +62,17 @@
 
         Args:
             output_directory (str): Directory to output thread detailed information
             user_or_subreddit (str): The name of the user or subreddit to export data for.
             export_mode (str): The export mode, which can be "single", "multiple", or "user".
             threads_list (List[dict]): A list of dictionaries containing thread information.
             verbose (Optional[bool]): Whether to print verbose output.
+
+        Returns:
+            None
         """
 
         detailed_report = ""
 
         match export_mode:
             case "single":
                 detailed_report = "{}/reports/subreddits/{}_{}_summary.{}".format(
@@ -94,28 +98,41 @@
             verbose (Optional[bool]): Whether to print verbose output.
             output_directory: (str): Directory to output the downloaded files and reports
             number_results (int): The number of results to scrape.
 
         Returns:
             None
         """
+        user_reddit_profile_to_scrape = self.main_constants.user_profile_to_scrape
+
+        if reddit_user is None and user_reddit_profile_to_scrape is not None:
+            reddit_user = user_reddit_profile_to_scrape
+        elif (reddit_user is not None and user_reddit_profile_to_scrape is not None or reddit_user is not None
+              and user_reddit_profile_to_scrape is None):
+            reddit_user = reddit_user
+        else:
+            msg = "Missing reddit username. If you want to scrape a user profile you must provide a reddit user"
+            raise MissingRequiredParameter(msg)
+
         # validate reddit user
         is_user_valid = self.reddit_api_validations.validate_reddit_user(reddit_user, verbose)
 
         if is_user_valid:
             # Scrape user submissions
-            user_threads = self.thread_scraper.scrape_threads(reddit_user, sort, "user", verbose, number_results)
+            user_threads = self.thread_scraper.scrape_threads(
+                reddit_user, sort, "user", verbose,
+                number_results if number_results is not None else self.main_constants.user_num_threads_to_scrape)
 
             # Downloads scraped img urls
             self.image_downloader.download_img_url_list(
                 reddit_user, user_threads, "user", output_directory, verbose)
 
             img_output_dir = Path("{}/downloads/user/{}".format(output_directory, reddit_user))
 
-            image_files = self.scraper_helper.generate_list_of_img_files_in_dir(img_output_dir)
+            image_files = self.scraper_helper.get_list_of_img_files_in_dir(img_output_dir)
 
             # If the image list size is bigger than 0, sort the downloaded images by mime type and resolution
             if len(image_files) > 0:
                 self.io_operations.sort_by_mime_type_and_resolution(
                     img_output_dir,
                     img_output_dir,
                     True,
@@ -137,37 +154,45 @@
                     be used.
             sorting_type (str): A string indicating how to sort the posts. Valid values: 'hot', 'new', 'top',
                 'controversial', 'rising'.
             number_results (int, optional): The maximum number of posts to scrape. If None, all posts will be scraped.
             details (bool): If True, exports detailed information about each post to a JSON file.
             output_directory: (str): Directory to output the downloaded files and reports
             verbose (bool): If True, displays logging information during the scraping process.
+
+        Returns:
+            None
         """
 
         user_subreddits_list = self.main_constants.user_subreddits_list
 
         if subreddits is None and user_subreddits_list is not None:
             subreddits = user_subreddits_list
         elif (subreddits is not None and user_subreddits_list is not None or subreddits is not None
               and user_subreddits_list is None):
             subreddits = subreddits
+        else:
+            msg = "Missing subreddits. If you want to scrape a subreddit or multiple subreddits, provide one or " \
+                  "multiple subreddits separated by a comma or semi-colo"
+            raise MissingRequiredParameter(msg)
 
         # Validate Args
         subreddits = self.parameter_validations.validate_subreddits_parameter(subreddits)
 
         # Validate Subreddit
-        self.reddit_api_validations.validate_subreddits_list(subreddits)
+        self.reddit_api_validations.validate_subreddits_list(subreddits, verbose)
 
         subreddits_detailed_information_dict: dict = {}
 
         # Scrape posts and comments
         for subreddit in subreddits:
             # Scrapes n number of threads for the given subreddits, according to provided parameter max_count
             subreddit_threads_list = self.thread_scraper.scrape_threads(
-                subreddit, sorting_type, "subreddit", verbose, number_results if number_results is not None else None)
+                subreddit, sorting_type, "subreddit", verbose,
+                number_results if number_results is not None else self.main_constants.user_num_threads_to_scrape)
 
             subreddits_detailed_information_dict = {**subreddits_detailed_information_dict,
                                                     **subreddit_threads_list}
 
             img_output_dir = Path("{}/downloads/subreddit/{}".format(output_directory, subreddit))
 
             # Downloads scraped img urls
```

## core/scraper/comment_scraper.py

```diff
@@ -3,16 +3,16 @@
 
 import bs4
 from bs4 import BeautifulSoup
 from loguru import logger  # type: ignore
 import validators  # type: ignore
 
 from common.logging.logging_setup import LoggingSetup  # type: ignore
-from common.common_constants import CommonConstants  # type: ignore
-from common.image_downloader import ImageDownloader  # type: ignore
+from common.constants.common_constants import CommonConstants  # type: ignore
+from common.io_operations.image_downloader import ImageDownloader  # type: ignore
 from common.logging.utils.loguru_wrappers import logger_wraps  # type: ignore
 from common.validations.url_validations import UrlValidations  # type: ignore
 from core.scraper.scraper_helper import ScraperHelper
 
 
 class CommentScraper:
     """
@@ -35,14 +35,15 @@
         super().__init__()
         self.logging_funcs = LoggingSetup()
         self.constants = CommonConstants()
         self.validations = UrlValidations()
         self.image_downloader = ImageDownloader()
         self.scraper_helper = ScraperHelper()
         self.processed_comments = []
+        self.img_urls = []
 
     # noinspection PyUnresolvedReferences
     @logger_wraps()
     def scrape_comments(self, soup: BeautifulSoup) -> Tuple[List[Dict[str, any]], List[str]]:
         """
         Scrape comments from the given comments' element.
 
@@ -67,55 +68,30 @@
                         - 'urls': A list of strings representing the URLs found in the given comment.
                         - 'replies': A list of nested dictionaries representing the children replies for the given
                             reply.
                     - A list of strings representing the URLs of any images found in the comments.
         """
 
         comments: List[Dict[str, any]] = []
-        img_urls: List[str] = []
+        self.img_urls: List[str] = []
         self.processed_comments: List[str] = []
 
         comment_area: bs4.element.Tag = soup.find("div", attrs={"class": "commentarea"})
-        comments_link_listing: bs4.element.Tag = comment_area.find("div", attrs={"class", "sitetable"})
+        comments_link_listing = comment_area.find("div", attrs={"class", "sitetable"})
 
         for comment_ele in comments_link_listing:
-            c_ele: bs4.element.PageElement = comment_ele
+            c_ele: bs4.element.Tag = comment_ele
             if "thing" in c_ele.attrs["class"]:
                 if c_ele.attrs["data-permalink"] not in self.processed_comments:
-                    comment = {"text": c_ele.find("div", class_="md").text.strip(),
-                               "author": self.scraper_helper.construct_author_dict(c_ele),
-                               "rating": self.scraper_helper.construct_rating_dict(c_ele),
-                               "datetime": self.scraper_helper.construct_time_dict(c_ele),
-                               "url": c_ele.attrs["data-permalink"]
-                               }
-
-                    comment_has_children, comment_num_children = self.scraper_helper.define_children_fields(c_ele)
-
-                    comment["hasChildren"] = comment_has_children
-                    comment["numChildren"] = comment_num_children
-
-                    urls = self.scraper_helper.construct_urls_list(c_ele)
-                    img_urls = img_urls + urls
-                    comment["urls"] = urls
-
-                    comment["replies"] = []
-                    child_div = c_ele.find("div", attrs={"class", "child"})
-                    reply_divs = child_div.find_all("div", attrs={"class", "comment"})
-
-                    self.processed_comments.append(c_ele.attrs["data-permalink"])
-
-                    if reply_divs:
-                        replies, img_urls = self.scrape_replies(reply_divs)
-                        processed_replies: List[Dict[str, Any]] = self.scraper_helper.remove_empty_lists(replies)
-                        comment["replies"] = processed_replies
+                    comment = self.process_comment(c_ele)
                     comments.append(comment)
 
         logger.debug("Processed Replies: {}".format(len(self.processed_comments)))
 
-        return comments, list(set(img_urls))
+        return comments, list(set(self.img_urls))
 
     # noinspection PyUnresolvedReferences
     @logger_wraps()
     def scrape_replies(self, reply_divs: List[Any]) -> Tuple[List[Dict[str, Any]], List[str]]:
         """
         Scrapes the replies from the given reply divs and returns a list of dictionaries representing each reply.
 
@@ -142,34 +118,58 @@
         """
 
         replies: List[Dict[str, typing.Any]] = []
         img_urls: List[str] = []
 
         for reply_div in reply_divs:
             if reply_div.attrs["data-permalink"] not in self.processed_comments:
-                reply = {"text": reply_div.find("div", class_="md").text.strip(),
-                         "author": self.scraper_helper.construct_author_dict(reply_div),
-                         "rating": self.scraper_helper.construct_rating_dict(reply_div),
-                         "datetime": self.scraper_helper.construct_time_dict(reply_div),
-                         "url": reply_div.attrs["data-permalink"]}
-
-                reply_has_children, reply_num_children = self.scraper_helper.define_children_fields(reply_div)
-                reply["hasChildren"] = reply_has_children
-                reply["numChildren"] = reply_num_children
-
-                urls = self.scraper_helper.construct_urls_list(reply_div)
-                reply["urls"] = urls
-                img_urls = img_urls + urls
-                reply["replies"] = []
-
-                self.processed_comments.append(reply_div.attrs["data-permalink"])
-
-                nested_reply_divs = reply_div.find_all('div', class_='comment')
-                if nested_reply_divs:
-                    processed_replies, img_urls = self.scrape_replies(nested_reply_divs)
-                    post_processed_replies: List[Dict[str, Any]] = \
-                        self.scraper_helper.remove_empty_lists(processed_replies)
-                    reply['replies'] = post_processed_replies
-
+                reply = self.process_reply(reply_div)
                 replies.append(reply)
 
         return replies, list(set(img_urls))
+
+    def process_comment(self, comment_element: bs4.element.Tag):
+        comment_has_children, comment_num_children = self.scraper_helper.define_children_fields(comment_element)
+        urls = self.scraper_helper.construct_urls_list(comment_element)
+        self.img_urls = self.img_urls + urls
+
+        comment = {"text": comment_element.find("div", class_="md").text.strip(),
+                   "author": self.scraper_helper.construct_author_dict(comment_element),
+                   "rating": self.scraper_helper.construct_rating_dict(comment_element),
+                   "datetime": self.scraper_helper.construct_time_dict(comment_element),
+                   "url": comment_element.attrs["data-permalink"], "hasChildren": comment_has_children,
+                   "numChildren": comment_num_children, "urls": urls, "replies": []}
+
+        child_div = comment_element.find("div", attrs={"class", "child"})
+        reply_divs = child_div.find_all("div", attrs={"class", "comment"})
+
+        self.processed_comments.append(comment_element.attrs["data-permalink"])
+
+        if reply_divs:
+            replies, img_urls = self.scrape_replies(reply_divs)
+            processed_replies: List[Dict[str, Any]] = self.scraper_helper.remove_empty_lists(replies)
+            comment["replies"] = processed_replies
+
+        return comment
+
+    def process_reply(self, reply_element: bs4.element.Tag):
+        reply_has_children, reply_num_children = self.scraper_helper.define_children_fields(reply_element)
+        urls = self.scraper_helper.construct_urls_list(reply_element)
+        self.img_urls = self.img_urls + urls
+
+        reply = {"text": reply_element.find("div", class_="md").text.strip(),
+                 "author": self.scraper_helper.construct_author_dict(reply_element),
+                 "rating": self.scraper_helper.construct_rating_dict(reply_element),
+                 "datetime": self.scraper_helper.construct_time_dict(reply_element),
+                 "url": reply_element.attrs["data-permalink"], "hasChildren": reply_has_children,
+                 "numChildren": reply_num_children, "urls": urls, "replies": []}
+
+        self.processed_comments.append(reply_element.attrs["data-permalink"])
+
+        nested_reply_divs = reply_element.find_all('div', class_='comment')
+        if nested_reply_divs:
+            processed_replies, img_urls = self.scrape_replies(nested_reply_divs)
+            post_processed_replies: List[Dict[str, Any]] = \
+                self.scraper_helper.remove_empty_lists(processed_replies)
+            reply['replies'] = post_processed_replies
+
+        return reply
```

## core/scraper/scraper_helper.py

```diff
@@ -1,15 +1,16 @@
 import glob
 import re
+from loguru import logger
 from pathlib import Path
 from typing import Dict, Tuple, List, Any
-import bs4
+from bs4 import BeautifulSoup, element
 import validators
 
-from common.common_constants import CommonConstants  # type: ignore
+from common.constants.common_constants import CommonConstants  # type: ignore
 from common.validations.url_validations import UrlValidations  # type: ignore
 
 
 class ScraperHelper:
     """
     This class provides helper methods for web scraping comments and threads from forums.
 
@@ -30,15 +31,15 @@
 
     def __init__(self) -> None:
         super().__init__()
         self.constants = CommonConstants()
         self.validations = UrlValidations()
 
     # noinspection PyUnresolvedReferences
-    def construct_author_dict(self, div_ele: bs4.element.PageElement) -> Dict[str, str]:
+    def construct_author_dict(self, div_ele: element.PageElement) -> Dict[str, str]:
         """
         Constructs a dictionary with the author's username and profile URL.
 
         Args:
             div_ele: A BeautifulSoup object representing a div element that contains the author's information.
 
         Returns:
@@ -51,15 +52,15 @@
         profile = author_el["href"]
 
         author = {"username": author_username, "profile": profile}
 
         return author
 
     # noinspection PyUnresolvedReferences
-    def construct_rating_dict(self, div_ele: bs4.element.PageElement) -> Dict[str, str]:
+    def construct_rating_dict(self, div_ele: element.PageElement) -> Dict[str, str]:
         """
         Constructs a dictionary with the comment's rating scores.
 
         Args:
             div_ele: A BeautifulSoup object representing a div element that contains the comment's rating scores.
 
         Returns:
@@ -82,15 +83,15 @@
         if score_likes is not None:
             parent_comment_author_score_likes = score_likes.text
             rating["score_likes"] = parent_comment_author_score_likes
 
         return rating
 
     # noinspection PyUnresolvedReferences
-    def construct_thread_rating_dict(self, div_ele: bs4.element.PageElement) -> Dict[str, str]:
+    def construct_thread_rating_dict(self, div_ele: element.PageElement) -> Dict[str, str]:
         """
         Constructs a dictionary with the thread's rating scores.
 
         Args:
             div_ele: A BeautifulSoup object representing a div element that contains the thread's rating scores.
 
         Returns:
@@ -114,15 +115,15 @@
         if score_likes is not None:
             parent_comment_author_score_likes = score_likes.text
             rating["score_likes"] = parent_comment_author_score_likes
 
         return rating
 
     # noinspection PyUnresolvedReferences
-    def construct_time_dict(self, div_ele: bs4.element.PageElement) -> Dict[str, str]:
+    def construct_time_dict(self, div_ele: element.PageElement) -> Dict[str, str]:
         """
         Constructs a dictionary with the time information of the comment or thread.
 
         Args:
             div_ele: A BeautifulSoup object representing a div element that contains the time information.
 
         Returns:
@@ -137,15 +138,15 @@
             time["time"] = time_el.attrs["title"]
             time["datetime"] = time_el.attrs["datetime"]
             time["time_since_posting"] = time_el.text
 
         return time
 
     # noinspection PyUnresolvedReferences
-    def define_children_fields(self, div_ele: bs4.element.PageElement) -> Tuple[bool, int]:
+    def define_children_fields(self, div_ele: element.PageElement) -> Tuple[bool, int]:
         """
         Defines the number of children and whether a comment or thread has children.
 
         Args:
             div_ele: A BeautifulSoup object representing a div element that contains the information about children.
 
         Returns:
@@ -164,15 +165,15 @@
             num_children = int(num_children)
             has_children = True if num_children > 0 else False
 
         return has_children, num_children
 
     # noinspection PyUnresolvedReferences
 
-    def construct_urls_list(self, div_ele: bs4.element.PageElement) -> List[str]:
+    def construct_urls_list(self, div_ele: element.PageElement) -> List[str]:
         """
         Constructs a list of URLs from the div element that contains the URLs.
 
         Args:
             div_ele: A BeautifulSoup object representing a div element that contains URLs.
 
         Returns:
@@ -201,20 +202,62 @@
                 elem = self.remove_empty_lists(elem)
                 if elem:
                     result.append(elem)
             else:
                 result.append(elem)
         return result
 
-    def generate_list_of_img_files_in_dir(self, directory: Path) -> List[str]:
+    def get_list_of_img_files_in_dir(self, directory: Path) -> List[str]:
         """Generate a list of image files in a directory.
 
         Args:
             directory (pathlib.Path): The directory to search for image files.
 
         Returns:
             list: A list of image file paths.
         """
 
         image_files = glob.glob(str(directory) + "/*.jpg") + glob.glob(str(directory) + "/*.png") \
                       + glob.glob(str(directory) + "/*.gif")
         return image_files
+
+    def define_threads_based_on_search_parameter(self, scrape_mode, request, subreddit_or_user):
+        threads = None
+        soup: BeautifulSoup = BeautifulSoup(request.text, "html.parser")
+
+        match scrape_mode:
+            case "subreddit":
+                threads_list_element = soup.find(
+                    "div", attrs={"class": "sitetable linklisting"})
+                threads = threads_list_element.find_all(
+                    "div", attrs={"data-subreddit-prefixed": "r/{}".format(subreddit_or_user)})
+            case "user":
+                threads_list_element = soup.find("div", attrs={"class": "sitetable linklisting"})
+                threads = threads_list_element.find_all("div", attrs={"data-author": subreddit_or_user})
+
+        return threads
+
+    def process_thread_images(self, thread_img_ele, thread_images):
+        if thread_img_ele is not None:
+            thread_image_a_tags = thread_img_ele.find_all("a", attrs={"class", "may-blank"})
+            thread_iframe_tag = thread_img_ele.find("iframe", attrs={"class", "media-embed"})
+
+            if thread_image_a_tags is not None and len(thread_image_a_tags) >= 1:
+                for thread_image_a_tag in thread_image_a_tags:
+                    logger.debug(thread_image_a_tag.attrs["href"])
+                    if self.validations.validate_if_url_is_a_valid_img_link(thread_image_a_tag.attrs["href"],
+                                                                            self.constants.possible_urls):
+                        thread_images.append(thread_image_a_tag.attrs["href"])
+
+                    img_tag = thread_img_ele.find("img", attrs={"class", "preview"})
+
+                    if img_tag is not None:
+                        logger.debug(img_tag.attrs["src"])
+                        if self.validations.validate_if_url_is_a_valid_img_link(
+                                img_tag.attrs["src"], self.constants.possible_urls):
+                            thread_images.append(img_tag.attrs["src"])
+
+            if thread_iframe_tag is not None:
+                logger.debug(thread_iframe_tag.attrs["src"])
+                if self.validations.validate_image_url(self.constants.possible_urls,
+                                                       thread_iframe_tag.attrs["src"]):
+                    thread_images.append(thread_iframe_tag.attrs["src"])
```

## core/scraper/thread_scraper.py

```diff
@@ -1,23 +1,22 @@
 import logging
 import time
 from typing import Any, Optional, Dict, Union
 import requests  # type: ignore
 from loguru import logger  # type: ignore
 from bs4 import BeautifulSoup, ResultSet
 
-from common.exceptions import TokenErrorException  # type: ignore
+from common.exceptions.main_exceptions import TokenErrorException  # type: ignore
 from common.logging.logging_setup import LoggingSetup  # type: ignore
-from common.common_constants import CommonConstants  # type: ignore
-from common.logging.utils.loguru_wrappers import logger_wraps
-#from common.logging.utils.loguru_wrappers import logger_wraps  # type: ignore
+from common.constants.common_constants import CommonConstants  # type: ignore
+from common.logging.utils.loguru_wrappers import logger_wraps   # type: ignore
 from common.validations.url_validations import UrlValidations  # type: ignore
-from common.request_manager import RequestManager  # type: ignore
-from common.image_downloader import ImageDownloader  # type: ignore
-from common.io_operations import IOOperations  # type: ignore
+from common.io_operations.request_manager import RequestManager  # type: ignore
+from common.io_operations.image_downloader import ImageDownloader  # type: ignore
+from common.io_operations.io_operations import IOOperations  # type: ignore
 from core.scraper.comment_scraper import CommentScraper  # type: ignore
 from core.api.reddit_api import RedditApi  # type: ignore
 from core.scraper.scraper_helper import ScraperHelper  # type: ignore
 
 
 class ThreadScraper:
     """
@@ -44,26 +43,26 @@
         self.image_downloader = ImageDownloader()
         self.scraper_helper = ScraperHelper()
         self.reddit_api = RedditApi(self.constants.client_id, self.constants.secret_token, self.constants.username,
                                     self.constants.password)
 
     @logger_wraps()
     def scrape_threads(self, subreddit_or_user: str, sort: str, scrape_mode: str, verbose: bool,
-                       max_counter: Optional[int] = None
+                       max_counter: Optional[int]
                        ) -> Dict[
         str, Union[Dict[str, Union[Dict[str, Any], Dict[str, Any], ResultSet[Any], Dict[str, Any], Any]], Any]]:
         """
         Scrape threads from a subreddit or user and return the results.
 
         Args:
             subreddit_or_user (str): The name of the subreddit or user from which to scrape threads.
             sort (str): The method to sort the threads, such as "hot" or "top".
             scrape_mode (str): The mode in which to scrape threads, either "subreddit" or "user".
             verbose (bool): A flag indicating whether to log verbose output.
-            max_counter (Optional[int], optional): The maximum number of threads to scrape. Defaults to None.
+            max_counter (Optional[int], optional): The maximum number of threads to scrape.
 
         Returns:
             Dict[str, Union[ Dict[str, Union[Dict[str, Any], Dict[str, Any], ResultSet[Any], Dict[str, Any], Any]],
                 Any]]:
                 A dictionary of thread URLs and their corresponding information, such as their author, datetime,
                  rating, URLs, and comments.
         """
@@ -93,40 +92,29 @@
         full = False
         if req.status_code == 200:
             msg = "\nCollecting information for {}....".format(url)
             logger.info(msg) if verbose else None
 
             soup: BeautifulSoup = BeautifulSoup(req.text, "html.parser")
 
-            if scrape_mode == "subreddit":
-                soup: BeautifulSoup = BeautifulSoup(req.text, "html.parser")
-                threads_list_element = soup.find(
-                    "div", attrs={"class": "sitetable linklisting"})
-                threads = threads_list_element.find_all(
-                    "div", attrs={"data-subreddit-prefixed": "r/{}".format(subreddit_or_user)})
-            else:
-                threads_list_element = soup.find("div", attrs={"class": "sitetable linklisting"})
-                threads = threads_list_element.find_all("div", attrs={"data-author": subreddit_or_user})
+            threads = self.scraper_helper.define_threads_based_on_search_parameter(scrape_mode, req, subreddit_or_user)
 
-            max_count = (int(max_counter) if max_counter is not None else len(threads))
+            max_count = int(max_counter)
 
             while full is not True:
                 for thread in threads:
                     try:
                         msg = "\nCollecting information from thread {} of {}...".format(counter, max_count)
                         logger.info(msg) if verbose else None
 
                         thread_details_path = thread.attrs["data-permalink"]
                         thread_url = self.constants.old_reddit_url + thread_details_path
-
-                        thread_comments, img_urls = self.scrape_single_thread(
-                            thread_details_path, verbose
-                        )
-
+                        thread_comments, img_urls = self.scrape_single_thread(thread_details_path, verbose)
                         current_thread = "{}".format(thread_url)
+
                         thread_img_urls[current_thread] = {
                             "author": self.scraper_helper.construct_author_dict(thread),
                             "datetime": self.scraper_helper.construct_time_dict(thread),
                             "rating": self.scraper_helper.construct_thread_rating_dict(thread),
                             "thread_url": thread_url,
                             "urls": img_urls,
                             "comments": thread_comments
@@ -144,28 +132,32 @@
                     except AttributeError:
                         continue
                 if full:
                     break
 
                 try:
                     next_button = soup.find("span", class_="next-button")
-                    next_page_link = next_button.find("a").attrs["href"]  # type: ignore
+                    if next_button is not None:
+                        next_page_link = next_button.find("a").attrs["href"]  # type: ignore
+                    else:
+                        full = True
+                        break
 
                     req = requests.get(next_page_link, headers=self.constants.user_agent, timeout=10)
                     soup: BeautifulSoup = BeautifulSoup(req.text, "html.parser")
                 except TokenErrorException as exc:
                     self.logging_funcs.print_exception_log(str(exc), verbose)
                     break
 
             threads_urls[subreddit_or_user] = thread_img_urls
 
-            logger.debug("[5] FINISHED SCRAPING STEP", verbose)
+            logger.debug("[5] FINISHED SCRAPING STEP")
         else:
             message = "Error fetching results.. Try again!"
-            self.logging_funcs.print_exception_log(message, verbose)
+            logger.exception(message, verbose)
 
         return threads_urls
 
     def scrape_single_thread(self, link: str, verbose: bool):
         """
         Scrapes the given Reddit thread URL and returns a tuple containing a list of image URLs and a dictionary of
          comments.
@@ -189,43 +181,19 @@
             # and scraping the details required
             soup: BeautifulSoup = BeautifulSoup(req.text, "html.parser")
 
             thread_images = []
 
             thread_img_ele = soup.find("div", attrs={"class", "expando"})
 
-            if thread_img_ele is not None:
-                thread_image_a_tags = thread_img_ele.find_all("a", attrs={"class", "may-blank"})
-                thread_iframe_tag = thread_img_ele.find("iframe", attrs={"class", "media-embed"})
-
-                if thread_image_a_tags is not None and len(thread_image_a_tags) >= 1:
-                    for thread_image_a_tag in thread_image_a_tags:
-                        logging.debug(thread_image_a_tag.attrs["href"])
-                        if self.validations.validate_if_url_is_a_valid_img_link(
-                                thread_image_a_tag.attrs["href"], self.constants.possible_urls):
-                            thread_images.append(thread_image_a_tag.attrs["href"])
-
-                        img_tag = thread_img_ele.find("img", attrs={"class", "preview"})
-
-                        if img_tag is not None:
-                            logging.debug(img_tag.attrs["src"])
-                            if self.validations.validate_if_url_is_a_valid_img_link(
-                                    img_tag.attrs["src"], self.constants.possible_urls):
-                                thread_images.append(img_tag.attrs["src"])
-
-                if thread_iframe_tag is not None:
-                    logging.debug(thread_iframe_tag.attrs["src"])
-                    if self.validations.validate_image_url(
-                            self.constants.possible_urls, thread_iframe_tag.attrs["src"]):
-                        thread_images.append(thread_iframe_tag.attrs["src"])
+            self.scraper_helper.process_thread_images(thread_img_ele, thread_images)
+            thread_comments, img_urls = self.comment_scrapper.scrape_comments(soup)
 
             thread_images = list(set(thread_images))
 
-            thread_comments, img_urls = self.comment_scrapper.scrape_comments(soup)
-
             # Remove all elements from thread_images that contain the value "crop=smart"
             thread_images = [x for x in thread_images if "crop=smart" not in x]
 
             logging.debug(thread_images)
             logging.debug(len(thread_images))
 
             img_urls = img_urls + thread_images
```

## Comparing `common/common_constants.py` & `common/constants/common_constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,95 @@
 import datetime
 from collections import defaultdict
 from pathlib import Path
 import os
 
 
 class CommonConstants:
-    """A class that contains constants used throughout the application.
+    """
+    A class that contains constants used throughout the application.
 
     Attributes:
         old_reddit_url (str): Old reddit base url.
         reddit_api_base_url (str): Reddit API base url.
         resolutions (defaultdict): Resolutions for the most popular resolutions.
         default_logger_format (str): Default logger format.
         default_logger_date_format (str): Default logger date format.
         attrs (dict): Default attributes for scraping reddit posts.
         possible_urls (list): Valid possible url prefixes that may appear during scraping.
         invalid_urls (list): Invalid possible url prefixes that may appear during scraping.
         match_url (str): Regex that match urls in the format https://subdomain.domain.
         domain_regex (str): Regex for validating domains.
+
+    Properties:
+        logs_default_output_directory (str): Logs default output directory.
+        user_reports_default_output_directory (str): User reports default output directory.
+        subreddits_reports_default_output_directory (str): Subreddits reports default output directory.
+        user_img_downloads_default_output_directory (str): User image downloads default output directory.
+        subreddits_img_downloads_default_output_directory (str): Subreddits default output directory.
+        client_id (str): User API key.
+        secret_token (str): User API secret.
+        username (str): User Reddit username.
+        password (str): User Reddit password.
+        user_subreddits_list (str): Subreddit user list. A string of comma-separated subreddits.
+        user_profile_to_scrape (str): Subreddit user list. A string of comma-separated subreddits.
+        user_subreddits_sort_method (str): Subreddit user list sort method. A string of comma-separated subreddits.
+        reddit_headers (dict): A dictionary containing the user agent header information.
+        check_mark_symbol (str): Check mark symbol.
+        cross_symbol (str): Cross symbol.
+        reddit_url (str): New Reddit base URL.
+        old_reddit_url (str): Old Reddit base URL.
+        reddit_api_base_url (str): Reddit API base URL.
+        output_path (Path): Output path for subreddits.
+        resolutions (defaultdict): a dictionary containing a tuple of integers representing a resolution as the key and the
+        corresponding resolution label as the value.
+        user_agent (str): User agent information for Reddit.
     """
 
     @property
+    def logs_default_output_directory(self):
+        """
+        Returns:
+            (str): Logs default output directory.
+        """
+        return "logs"
+
+    @property
+    def user_reports_default_output_directory(self):
+        """
+        Returns:
+            (str): User reports default output directory.
+        """
+        return "reports/users"
+
+    @property
+    def subreddits_reports_default_output_directory(self):
+        """
+        Returns:
+            (str): Subreddits reports default output directory.
+        """
+        return "reports/subreddits"
+
+    @property
+    def user_img_downloads_default_output_directory(self):
+        """
+        Returns:
+            (str): user image downloads default output directory.
+        """
+        return "downloads/user"
+
+    @property
+    def subreddits_img_downloads_default_output_directory(self):
+        """
+        Returns:
+            (str): subreddits default output directory.
+        """
+        return "downloads/subreddit"
+
+    @property
     def client_id(self):
         """
         Returns:
             (str): User API key.
         """
 
         return os.environ.get("REDDIT_API_KEY")
@@ -59,15 +124,28 @@
     @property
     def user_subreddits_list(self):
         """
         Returns:
             (str): Subreddit user list. A string of comma separated subreddits.
         """
 
-        return os.environ.get("SUBREDDIT_USER_LIST")
+        return os.environ.get("SUBREDDITS_TO_SCRAPE")
+
+    @property
+    def user_profile_to_scrape(self):
+        """
+        Returns:
+            (str): Subreddit user list. A string of comma separated subreddits.
+        """
+
+        return os.environ.get("REDDIT_USER_TO_SCRAPE")
+
+    @property
+    def user_num_threads_to_scrape(self):
+        return os.environ.get("NUM_THREADS_TO_SCRAPE")
 
     @property
     def user_subreddits_sort_method(self):
         """
         Returns:
             (str): Subreddit user list sort method. A string of comma separated subreddits.
         """
@@ -234,14 +312,34 @@
             (str): a string containing the regular expression.
         """
 
         reg = r"https?://(?:[-\w.]|(?:%[\da-fA-F]{2}))+/[-\w./?%&=]*"
         return reg
 
     @property
+    def replace_consecutive_commas_or_semicolons_regex(self):
+        """
+        Replace consecutive commas or semicolons with a single comma in a comma or semicolon separated string
+
+        Returns:
+            (str): a string containing the regular expression.
+        """
+        return r"[,;]+"
+
+    @property
+    def remove_empty_groups_from_comma_or_semicolon_separated_string(self):
+        """
+        Remove any remaining empty groups in a comma or semicolon separated string
+
+        Returns:
+            (str): a string containing the regular expression.
+        """
+        return r"(^,)|(,$)|(^;)|(;$)|,{2,}"
+
+    @property
     def domain_regex(self):
         """
         Returns the regular expression for validating domains.
 
         The first regular expression uses a positive lookahead to assert that the string contains between 1 and 254
         characters ((?=^.{1,254}$)). Then it uses a capturing group to match one or more repetitions of a subpattern
         that consists of one or more characters that are not a digit followed by an optional dot.
```

## Comparing `common/exceptions.py` & `common/exceptions/main_exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,7 +27,16 @@
     """
     Raises a custom exception with a message informing the user the file
     conversion process was unsuccessful.
     """
 
     def __init__(self, message: str):
         super().__init__(message)
+
+
+class MissingRequiredParameter(Exception):
+    """
+    Raises a custom exception with a message informing the user about missing required parameters
+    """
+
+    def __init__(self, message: str):
+        super().__init__(message)
```

## Comparing `common/image_downloader.py` & `common/io_operations/image_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import glob
+from contextlib import contextmanager
 from pathlib import Path
 from typing import List
 from urllib.parse import urlparse
 import requests  # type: ignore
 from loguru import logger  # type: ignore
 from tqdm import tqdm
 import httpx
 
 from common.logging.utils.loguru_wrappers import logger_wraps  # type: ignore
 from common.validations.url_validations import UrlValidations  # type: ignore
-from common.common_constants import CommonConstants  # type: ignore
-from common.io_operations import IOOperations  # type: ignore
+from common.constants.common_constants import CommonConstants  # type: ignore
+from common.io_operations.io_operations import IOOperations  # type: ignore
 
 
 class ImageDownloader:
     """
     The ImageDownloader class is used to download images from URLs.
 
     Methods:
@@ -67,95 +68,114 @@
 
         if log_mode == "subreddit":
             msg = "{} report: {} images scrapped for the subreddit {}".format(
                 subreddit_or_user, len(subreddit_thread_img_list), subreddit_or_user)
         else:
             msg = "{} report: {} images scrapped".format(
                 subreddit_or_user, len(subreddit_thread_img_list))
-        logger.debug(msg, verbose)
+        logger.debug(msg)
 
     def download_img_urls_sync(self, subreddits_img_list: List[str], output_directory: Path, verbose: bool) -> None:
         """
         Downloads the images from the URLs scrapped from the given subreddit.
 
         Args:
             subreddits_img_list (List[str]): list of subreddits images
             output_directory (Path): Directory to output the downloaded images
             verbose (bool): Whether to print verbose output.
         """
-        logger.debug("[6] STARTING IMAGE DOWNLOAD STEP", verbose)
+        logger.debug("[6] STARTING IMAGE DOWNLOAD STEP")
         logger.info("Downloading scraped images") if verbose else None
 
         if not output_directory.exists():
             output_directory.mkdir(parents=True)
 
         # Make a GET request to the specified URL using httpx.
-        transport = httpx.HTTPTransport(retries=0)
+        transport = httpx.HTTPTransport(retries=3)
         client = httpx.Client(transport=transport)
 
         failed_urls = subreddits_img_list
         downloaded_urls = []
 
         subreddits_img_list = list(set(subreddits_img_list))
 
         try:
-            # Wrapping the loop with tqdm and customize the appearance of the progress bar
-            for url in tqdm(
-                    subreddits_img_list,
-                    desc="Downloading images",
-                    ncols=100,
-                    colour="green",
-                    unit_scale=True,
-                    dynamic_ncols=True):
-                response = client.get(url)
-
-                if response.status_code == 200:
-                    # Raise an exception if the HTTP request fails.
-
-                    # set the output file path
-                    output_file = output_directory / Path(urlparse(url).path).name
-
-                    msg = "Response: {}".format(self.constants.check_mark_symbol)
-                    logger.debug(msg)
-
-                    failed_urls.remove(url)
-                    downloaded_urls.append(url)
-
-                    # If the response is ok and the output file doesn't exist, save it to it's destination
-                    if not output_file.exists():
-                        with open(output_file, "wb") as ifile:
-                            ifile.write(response.content)
-                            msg = "{} - Downloaded {} to target folder {}".format(
-                                self.constants.check_mark_symbol, url, output_file)
-                            logger.debug(msg)
-                    else:
-                        msg = "{} - Skipping: {} already exists in the target folder {}".format(
-                            self.constants.cross_symbol, url, output_directory)
-                        logger.debug(msg)
+            if verbose:
+                # Wrapping the loop with tqdm and customize the appearance of the progress bar
+                with tqdm(
+                        total=len(subreddits_img_list),
+                        desc="Downloading images",
+                        ncols=100,
+                        colour="green",
+                        unit_scale=True,
+                        dynamic_ncols=True) as pbar:
+                    for url in subreddits_img_list:
+                        response = client.get(url)
+
+                        if response.status_code == 200:
+                            self.download_img_url(url, response.content, output_directory, failed_urls, downloaded_urls)
+
+                        pbar.update(1)
+            else:
+                for url in subreddits_img_list:
+                    response = client.get(url)
+
+                    if response.status_code == 200:
+                        self.download_img_url(url, response.content, output_directory, failed_urls, downloaded_urls)
+
         finally:
             client.close()
 
-        self.generate_download_report(output_directory, subreddits_img_list, failed_urls)
+        self.generate_download_report(output_directory, subreddits_img_list, failed_urls, verbose)
 
-        logger.debug("[6] FINISHED IMAGE DOWNLOAD STEP", verbose)
+        logger.debug("[6] FINISHED IMAGE DOWNLOAD STEP")
+
+    @contextmanager
+    def download_img_url(self, url: str, payload, output_directory: Path, failed_urls, downloaded_urls) -> None:
+        # Raise an exception if the HTTP request fails.
+
+        # set the output file path
+        output_file = output_directory / Path(urlparse(url).path).name
+
+        msg = "Response: {}".format(self.constants.check_mark_symbol)
+        logger.debug(msg)
+
+        failed_urls.remove(url)
+        downloaded_urls.append(url)
+
+        # If the response is ok and the output file doesn't exist, save it to it's destination
+        if not output_file.exists():
+            with open(output_file, "wb") as ifile:
+                ifile.write(payload)
+                msg = "{} - Downloaded {} to target folder {}".format(
+                    self.constants.check_mark_symbol, url, output_file)
+                logger.debug(msg)
+        else:
+            msg = "{} - Skipping: {} already exists in the target folder {}".format(
+                self.constants.cross_symbol, url, output_directory)
+            logger.debug(msg)
 
     @logger_wraps()
-    def generate_download_report(self, output_dir: Path, subreddits_img_list: List[str], failed_urls: List[str]):
+    def generate_download_report(self, output_dir: Path, subreddits_img_list: List[str], failed_urls: List[str],
+                                 verbose: bool):
         """
         Generates report for the downloading process of the subreddits images
 
         Args:
             output_dir (Path): Output path
             subreddits_img_list (List[str]): List of images scraped from the subreddit
             failed_urls (List[str]): List of urls that failed the downloading process
+            verbose: (bool): controls the verbosity level
         """
         image_files = glob.glob(str(output_dir) + "/*.jpg") + glob.glob(str(output_dir) + "/*.png") + glob.glob(
             str(output_dir) + "/*.gif")
 
         total_url_list_length = len(subreddits_img_list)
         failed_urls_length = len(subreddits_img_list) - len(image_files) \
             if (len(subreddits_img_list) - len(image_files)) > 0 else 0
         downloaded_urls_length = (total_url_list_length - failed_urls_length)
 
-        logger.info("From {} urls scrapped, {} urls where downloaded successfully and {} urls failed download".format(
-            total_url_list_length, downloaded_urls_length, failed_urls_length))
-        logger.debug("Failed urls: {}".format(failed_urls))
+        info_msg = "From {} urls scrapped, {} urls where downloaded successfully and {} urls failed download".format(
+            total_url_list_length, downloaded_urls_length, failed_urls_length)
+        logger.info(info_msg) if verbose else None
+        debug_msg = "Failed urls: {}".format(failed_urls)
+        logger.debug(debug_msg)
```

## Comparing `common/io_operations.py` & `common/io_operations/io_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import glob
 import json
 import mimetypes
 import os
 import shutil
 import sys
+from contextlib import contextmanager
 from pathlib import Path
 from typing import Any
 from loguru import logger       # type: ignore
 from tqdm import tqdm
 from PIL import Image       # type: ignore
 
-from common.common_constants import CommonConstants     # type: ignore
+from common.constants.common_constants import CommonConstants     # type: ignore
 from common.logging.logging_setup import LoggingSetup       # type: ignore
 
 
 class IOOperations:
     """
     The IOOperations class provides methods for input-output operations, including writing detailed post information,
     validating directories, sorting files by MIME type and resolution, and deleting original files.
@@ -39,28 +40,27 @@
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.logging_funcs = LoggingSetup()
         self.constants = CommonConstants()
 
-    def validate_path(self, path):
+    def validate_path_is_dir_and_exists(self, path):
         if os.path.exists(path):
             if os.path.isfile(path):
                 logger.debug("Valid file path but not directory")
                 is_valid = False
             elif os.path.isdir(path):
                 logger.debug("Valid directory path")
                 is_valid = True
             else:
                 logger.debug("Valid path, but not a file or directory")
                 is_valid = False
         else:
-            logger.error("Error: Invalid Path:", path)
-            raise OSError("Error: Invalid Path:", path)
+            is_valid = False
 
         return is_valid
 
     def init_directory(self, path):
         """
         Checks if a directory exists at the given path and creates it if it does not exist.
 
@@ -72,20 +72,22 @@
             msg = "Directory created at {}".format(path)
             logger.debug(msg)
         else:
             msg = "Directory already exists at {}".format(path)
             logger.debug(msg)
 
     def init_directories(self, output):
-        output_directory = None
 
         if output is not None:
-            if self.validate_path(output):
+            validate_path_is_dir_and_exists = self.validate_path_is_dir_and_exists(output)
+            if validate_path_is_dir_and_exists:
                 logger.debug("Provided output parameter: {} is VALID".format(output))
                 output_directory = output
+            else:
+                output_directory = output
         else:
             # Check if the Documents folder exists in the user's home directory. If not attempt to create it
             if os.name == 'nt':  # for Windows systems
                 docs_folder = os.path.join(os.path.expanduser("~"), "Documents")
             else:  # for Linux and macOS systems
                 docs_folder = os.path.join(os.path.expanduser("~"), "Documents")
 
@@ -99,19 +101,23 @@
                     logger.debug("Documents folder created at:", output_directory)
                 except OSError as exc:
                     logger.error("Error creating Documents folder:", exc)
                     raise OSError("Error creating Documents folder:", exc)
 
             output_directory = os.path.join(docs_folder, "output")
 
-        user_reports = os.path.join(output_directory, "reports/users")
-        subreddit_reports = os.path.join(output_directory, "reports/subreddits")
-        subreddit_downloads_directory = os.path.join(output_directory, "downloads/subreddit")
-        user_downloads_directory = os.path.join(output_directory, "downloads/subreddit")
-        logs = os.path.join(output_directory, "logs")
+        user_reports = os.path.join(output_directory,
+                                    self.constants.user_reports_default_output_directory)
+        subreddit_reports = os.path.join(output_directory,
+                                         self.constants.subreddits_reports_default_output_directory)
+        subreddit_downloads_directory = os.path.join(output_directory,
+                                                     self.constants.subreddits_img_downloads_default_output_directory)
+        user_downloads_directory = os.path.join(output_directory,
+                                                self.constants.user_img_downloads_default_output_directory)
+        logs = os.path.join(output_directory, self.constants.logs_default_output_directory)
 
         self.init_directory(output_directory)
         self.init_directory(user_reports)
         self.init_directory(subreddit_reports)
         self.init_directory(subreddit_downloads_directory)
         self.init_directory(user_downloads_directory)
         self.init_directory(logs)
@@ -126,38 +132,41 @@
         """
         # Checking if input directory exists
         input_dir_path = Path(input_dir)
         if not input_dir_path.exists():
             logger.error("Input directory does not exist")
             sys.exit()
 
+    #  @contextmanager decorator allows the image file to be opened and closed automatically
+    @contextmanager
     def write_detailed_post_information(self, payload: Any, operation: str, filename: str, verbose: bool) -> None:
         """Write payload to a file in the specified format.
 
         Args:
             payload: The data to be written to the file.
             operation: The file operation mode ('w' for write, 'a' for append, etc.).
             filename: The path and filename of the file to write to.
             verbose: Boolean flag that controls the verbosity output
 
         Returns:
             None
         """
-        logger.debug("[9] STARTED WRITING SUBREDDIT REPORT INFORMATION STEP", verbose)
+        logger.debug("[9] STARTED WRITING SUBREDDIT REPORT INFORMATION STEP")
 
         extension = Path(filename).suffixes[-1]
 
         with open(filename, operation, encoding="utf-8") as file:
             if extension == ".txt":
                 file.write(payload)
             elif extension == ".json":
                 json_str = json.dumps(payload, indent=4)
                 file.write(json_str)
 
-        logger.debug("[9] FINISHED WRITING SUBREDDIT REPORT INFORMATION STEP", verbose)
+        logger.info("Report written to {}".format(filename)) if verbose else None
+        logger.debug("[9] FINISHED WRITING SUBREDDIT REPORT INFORMATION STEP")
 
     def create_output_folder_and_move_files(
             self, file_path: Path, output_dir: Path, matching_res: str, mimetype: str):
         """
         Creates the output folder and then moves the files to said folder
         Args:
             file_path (Path): Path to the file to be moved
@@ -178,78 +187,88 @@
         """Delete the original files from the input directory if `remove` is True.
 
         Args:
             input_dir (str): The path to the input directory.
             remove (bool): Whether to remove the original files.
             verbose (bool): Determines the level of verbosity
         """
-        logger.debug("[8] STARTED CLEANUP STEP", verbose)
+        logger.debug("[8] STARTED CLEANUP STEP")
         if remove:
             input_dir_path = input_dir
             for file in input_dir_path.iterdir():
                 if file.is_file():
                     file.unlink()
 
-        logger.debug("[8] FINISHED CLEANUP STEP", verbose)
+        logger.debug("[8] FINISHED CLEANUP STEP")
 
     def sort_by_mime_type_and_resolution(self, input_dir: Path, output_dir: Path, remove: bool, verbose):
         """Sort image files in the input directory by MIME type and resolution and save them to the
         output directory.
 
         Args:
             input_dir (Path): The path to the input directory.
             output_dir (Path): The path to the output directory.
             remove (bool): Whether to remove the original files.
             verbose (bool): Determines the level of verbosity
         """
-        logger.debug("[7] STARTED FILE SORTING STEP", verbose)
+        logger.debug("[7] STARTED FILE SORTING STEP")
 
         msg = "Sorting downloaded images"
         logger.info(msg) if verbose else None
 
         image_files = glob.glob(str(input_dir) + "/*.jpg") + glob.glob(str(input_dir) + "/*.png") + glob.glob(
             str(input_dir) + "/*.gif")
 
-        # Wrapping the loop with tqdm and customize the appearance of the progress bar
-        with tqdm(
-                total=len(image_files),
-                desc="Sorting images",
-                ncols=100,
-                colour="green",
-                unit_scale=True,
-                dynamic_ncols=True) as pbar:
+        if verbose:
+            # Wrapping the loop with tqdm and customize the appearance of the progress bar
+            with tqdm(
+                    total=len(image_files),
+                    desc="Sorting images",
+                    ncols=100,
+                    colour="green",
+                    unit_scale=True,
+                    dynamic_ncols=True) as pbar:
+
+                for file_path in Path(input_dir).glob("*.*"):
+                    self.sort_file(file_path, output_dir)
+                    pbar.update(1)
+
+        else:
             for file_path in Path(input_dir).glob("*.*"):
-                try:
-                    with Image.open(file_path) as img:
-                        width, height = img.size
-                        mimetype, _ = mimetypes.guess_type(str(file_path))
-                        # checks if img path has a mimetype, and it starts with image/.*
-                        if mimetype and mimetype.startswith("image/"):
-                            # match the resolution to the resolutions in the resolutions dict
-                            matching_key = next((resolution for resolution in self.constants.resolutions.keys() if
-                                                 resolution[0] <= width <= resolution[2] and resolution[1] <= height <=
-                                                 resolution[3]), None)
-
-                            # If any of resolutions match, save the img to the corresponding folder, if it doesn't
-                            # save the image to an "other" folder
-                            if matching_key:
-                                matching_value = self.constants.resolutions[matching_key]
-
-                                msg = "The corresponding resolution designation for the matching resolution {} is {}."\
-                                    .format(matching_key, matching_value)
-                                logger.debug(msg)
-
-                                self.create_output_folder_and_move_files(
-                                    file_path, output_dir, matching_value, mimetype)
-                            else:
-                                logger.debug("The resolution is not in the dictionary.")
-
-                                self.create_output_folder_and_move_files(file_path, output_dir, "other", mimetype)
-
-                except IOError as exc:
-                    logger.error("Error occurred while processing %s: %s", file_path, exc)
-                pbar.update(1)
+                self.sort_file(file_path, output_dir)
 
-        logger.debug("[7] FINISHED FILE SORTING STEP", verbose)
+        logger.debug("[7] FINISHED FILE SORTING STEP")
 
         # if remove flag is passed delete the original files
         self.delete_original_files(input_dir, remove, verbose)
+
+    def sort_file(self, file_path: Path, output_dir: Path):
+        try:
+            with Image.open(file_path) as img:
+                width, height = img.size
+                mimetype, _ = mimetypes.guess_type(str(file_path))
+                # checks if img path has a mimetype, and it starts with image/.*
+                if mimetype and mimetype.startswith("image/"):
+                    # match the resolution to the resolutions in the resolutions dict
+                    matching_key = next(
+                        (resolution for resolution in self.constants.resolutions.keys()
+                         if resolution[0] <= width <= resolution[2] and
+                         resolution[1] <= height <= resolution[3]), None)
+
+                    # If any of resolutions match, save the img to the corresponding folder, if it doesn't
+                    # save the image to an "other" folder
+                    if matching_key:
+                        matching_value = self.constants.resolutions[matching_key]
+
+                        msg = "The corresponding resolution for the matching resolution {} is {}." \
+                            .format(matching_key, matching_value)
+                        logger.debug(msg)
+
+                        self.create_output_folder_and_move_files(
+                            file_path, output_dir, matching_value, mimetype)
+                    else:
+                        logger.debug("The resolution is not in the dictionary.")
+
+                        self.create_output_folder_and_move_files(file_path, output_dir, "other", mimetype)
+
+        except IOError as exc:
+            logger.error("Error occurred while processing %s: %s", file_path, exc)
```

## Comparing `common/request_manager.py` & `common/io_operations/request_manager.py`

 * *Files identical despite different names*

## Comparing `common/string_builder.py` & `common/utils/string_builder.py`

 * *Files identical despite different names*

## Comparing `common/logging/logging_constants.py` & `common/constants/logging_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
 
     @property
     def default_log_rotation(self):
         """
         A float representing the default maximum size of the log file before it is rotated.
 
         Returns:
-             (str): a float representing the default maximum size of the log file before it is rotated
+             (float): a float representing the default maximum size of the log file before it is rotated
         """
         return 5e8
 
     @property
     def default_log_retention(self):
         """
         A string representing the default retention period for log files.
```

## Comparing `redscrap-0.0.2.dist-info/METADATA` & `redscrap-0.0.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: redscrap
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Reddit scraper that can scrape a subreddit or a user for images and download them
 Home-page: https://github.com/martimdLima
 Author: Martim Lima
 Author-email: martim.d.lima@protonmail.com
 Keywords: development,setup,setuptools
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.0
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7, <4
+License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: beautifulsoup4
 Requires-Dist: loguru
 Requires-Dist: requests
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: validators
```

## Comparing `redscrap-0.0.2.dist-info/RECORD` & `redscrap-0.0.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 __init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-common/common_constants.py,sha256=j7Af7XlLwUcMU_W3iNogXMhJKnzTYqXLff_I2p_-Xbg,10434
-common/exceptions.py,sha256=X1DyuRxN1qIcFTlZjunkEu-IV4v8Rim_bOrm57NpTm4,868
-common/image_downloader.py,sha256=29dN5jBwHCQ9x0x7GNlgYtlUEfJTq3_iZusGNzCtT_A,7957
-common/io_operations.py,sha256=pwSaUEL01tJz-LZtn0vvzlyWz5MnOi4e-h6tY5T0nDw,11726
-common/request_manager.py,sha256=X6CzhIAVhBX18TNn18d3K4H82yEZkiSJMJE6XvsBO9o,2064
-common/string_builder.py,sha256=5xQeSv_secDR0Y7_EPhwRaTdcKkgJdXWejGVUwZFEPs,1640
+common/constants/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+common/constants/common_constants.py,sha256=myVfKDu3pqmIcLh6hpP8Fqrud1ZKsVEKlZKhmrEVtdE,14149
+common/constants/logging_constants.py,sha256=8rxVQv6mZ7DPzPr8Fhwn8r8Nph1B4sAPro3x-Diimj0,16883
+common/exceptions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+common/exceptions/main_exceptions.py,sha256=_G2i2FRMvvjbNB5IAe4BvING-Q_lSSKd_tIxAxKbbBw,1107
+common/io_operations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+common/io_operations/image_downloader.py,sha256=ti-MqELgWmJ0__PkLuzVD6h0SmekWwVxBhS5WtZr9Y0,8697
+common/io_operations/io_operations.py,sha256=_L2bwdxleBaAYOVVnNJzPV8IJ6oJWEcMm5NuV2UE_hs,12460
+common/io_operations/request_manager.py,sha256=X6CzhIAVhBX18TNn18d3K4H82yEZkiSJMJE6XvsBO9o,2064
 common/logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-common/logging/logging_constants.py,sha256=RELdXmERWNv3f334tZLDpXcN_z6SzL4bJ4yzVWty88Q,16881
-common/logging/logging_setup.py,sha256=K4o02qUx2CinREbLhVVYuZletHRfl3DXMCVa01ZY8ZA,9753
-common/logging/loguru_setup.py,sha256=GLruyC7D2OIg8T7r-VSEcL_JSHEIAplzefQOXY9lkFs,5992
+common/logging/logging_setup.py,sha256=2K7hmtu46eaDADtclS_Myp_K4PR07vQaCnku30y0UzY,9755
+common/logging/loguru_setup.py,sha256=2WVGLWZli5jiznXrkaMDxCdLko_lXGiPDUQ-Tzx3_Qs,6015
 common/logging/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 common/logging/utils/color_formatter.py,sha256=VhCwDpzIHsZsKfYd1IlBfx7N-reSe82Lm_ZRu1S1_BI,992
 common/logging/utils/log_rotator.py,sha256=NCq_LITtCvm306_vr7fKwL5UyDwIViYTp9NVGiviL0o,1615
 common/logging/utils/logging_wrappers.py,sha256=GbX_i5tvrNus2AUaI-zbORfzBamIXnR2RiDt3Ek2R3s,1182
 common/logging/utils/loguru_wrappers.py,sha256=lGHLMv12BasGc6viDg8LjTCk0KRZUtRHOeOLPx7558A,2092
-common/logging/utils/padding_formatter.py,sha256=8Snh4oi-2ZxR39_qQz6GnICg2xBolJl_KiqrYvfciKY,1286
+common/logging/utils/padding_formatter.py,sha256=rKkjBT-sxboLaURvZKvWKmE8hI1nWWt5xSEyl1jpKlc,1288
+common/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+common/utils/string_builder.py,sha256=5xQeSv_secDR0Y7_EPhwRaTdcKkgJdXWejGVUwZFEPs,1640
 common/validations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-common/validations/parameter_validations.py,sha256=bX6MU06eODLb1_iYBqrIBEiXetXQC1ep2vDF6hZAkyI,6554
-common/validations/reddit_api_validations.py,sha256=D_5W2QiDykp1y0l2cqvQI_cgihTO62wrq4r1MWeAlc0,9371
-common/validations/url_validations.py,sha256=vKxfXGqNK16hRbKhtAguUNPNyZ6Z5cpI2wIS57m-HpQ,3507
+common/validations/parameter_validations.py,sha256=NwRb38zvOxNj3d-XoR3Q77jtjqpaTVK7umn5miItsio,6703
+common/validations/reddit_api_validations.py,sha256=30SjcpYtKWEPMWc8_5qUQ2bMOMOw7svoZoAEGNTumM8,6889
+common/validations/url_validations.py,sha256=X0EcuNmFbh1pgauVa5_aHi280qa77mmxGIzdemHhfNM,3517
 core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-core/main.py,sha256=YeDeOmLPnNsaTkO__LAOgZchVu-VipOZCcqMYU5_mOM,3408
+core/main.py,sha256=dAa5KyC5WJb_-4ZCWMs8KMXvZYZH3E-95afhb6kqbzU,4647
 core/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-core/api/reddit_api.py,sha256=XsIfKw_qXC62zBWLHyDumtemxvH7qRpnK4_XqP-KJYs,6035
+core/api/reddit_api.py,sha256=CWZsIE56T4hnFD1U6CTZzkgOQQdXcIoAzjinOpeRePc,6018
 core/helper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-core/helper/main_helper.py,sha256=TnDgM7wP6NNFZE-tl8XLlw61bRc4azDhvS8fDJd8r6o,10084
+core/helper/main_helper.py,sha256=qQxatToJO8Zxy805Pk8g6b7dBhPT62UYxmjsIMc5rEU,11320
 core/scraper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-core/scraper/comment_scraper.py,sha256=ZZ7bjcJwc3o-B5OSbvg75BfiBu3R5VOQAXjBiHsSy_U,9471
-core/scraper/scraper_helper.py,sha256=shK-10-rWdg4uRrY4a_cEnlnDGrl66rURRoz12FIlRU,8435
-core/scraper/thread_scraper.py,sha256=pcEHF_DeIdI3gqPqqvN2xa3Dhw-ij71UaJ8p2tgNq24,11386
-redscrap-0.0.2.dist-info/METADATA,sha256=j-ANJL2ROjCGvTVR04II5Pa8uUHswy9dHzAoDlfMvLw,1129
-redscrap-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-redscrap-0.0.2.dist-info/entry_points.txt,sha256=tTH8sFcsimNSFmh7Yzw6B2XRu9QRdlwhNvnk_T2ELbM,44
-redscrap-0.0.2.dist-info/top_level.txt,sha256=DTy351DnTAnYmG3Y2LB89rn_9i2efCXvT-e7vBITiKo,21
-redscrap-0.0.2.dist-info/RECORD,,
+core/scraper/comment_scraper.py,sha256=wz_lm1KmcNgnLshTdB-1o-itjMJof4z-iGhbjD7VOwg,9431
+core/scraper/scraper_helper.py,sha256=BVpm0WOqTyL06nRMzn7f6YLUJWw6I4Figy8meWBlr_A,10874
+core/scraper/thread_scraper.py,sha256=IxDvnQjE8ofwvwaAHJiXCj0a4FqYyesI1yjElhaJ7lA,9415
+redscrap-0.0.3.dist-info/LICENSE,sha256=mYe2gnkfOYGs2FsK2prdfAcYAiURyyuHydEVbCYc534,1089
+redscrap-0.0.3.dist-info/METADATA,sha256=qnWLmq0M6fWoZgNEygAuQouDpdA0WDLTQRWhVyFBq6s,1151
+redscrap-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+redscrap-0.0.3.dist-info/entry_points.txt,sha256=tTH8sFcsimNSFmh7Yzw6B2XRu9QRdlwhNvnk_T2ELbM,44
+redscrap-0.0.3.dist-info/top_level.txt,sha256=DTy351DnTAnYmG3Y2LB89rn_9i2efCXvT-e7vBITiKo,21
+redscrap-0.0.3.dist-info/RECORD,,
```

