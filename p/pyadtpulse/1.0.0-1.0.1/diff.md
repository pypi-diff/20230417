# Comparing `tmp/pyadtpulse-1.0.0-py3-none-any.whl.zip` & `tmp/pyadtpulse-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20116 bytes, number of entries: 11
--rw-r--r--  2.0 unx    30683 b- defN 23-Mar-28 16:07 pyadtpulse/__init__.py
+Zip file size: 20264 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    30711 b- defN 23-Apr-15 18:21 pyadtpulse/__init__.py
 -rw-r--r--  2.0 unx     1609 b- defN 23-Mar-28 16:07 pyadtpulse/const.py
--rw-r--r--  2.0 unx    24101 b- defN 23-Mar-28 16:07 pyadtpulse/site.py
+-rw-r--r--  2.0 unx    24098 b- defN 23-Apr-15 18:21 pyadtpulse/site.py
 -rw-r--r--  2.0 unx     4803 b- defN 23-Mar-28 16:07 pyadtpulse/util.py
 -rw-r--r--  2.0 unx     5089 b- defN 23-Mar-28 16:07 pyadtpulse/zones.py
--rw-r--r--  2.0 unx      581 b- defN 23-Mar-28 16:08 pyadtpulse-1.0.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3446 b- defN 23-Mar-28 16:08 pyadtpulse-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 16:08 pyadtpulse-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-28 16:08 pyadtpulse-1.0.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Nov-23 16:58 pyadtpulse-1.0.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx      875 b- defN 23-Mar-28 16:08 pyadtpulse-1.0.0.dist-info/RECORD
-11 files, 71291 bytes uncompressed, 18642 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx      581 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3646 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 22-Nov-23 16:58 pyadtpulse-1.0.1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      875 b- defN 23-Apr-16 22:48 pyadtpulse-1.0.1.dist-info/RECORD
+11 files, 71516 bytes uncompressed, 18790 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pyadtpulse/util.py
 Comment: 
 
 Filename: pyadtpulse/zones.py
 Comment: 
 
-Filename: pyadtpulse-1.0.0.dist-info/LICENSE.md
+Filename: pyadtpulse-1.0.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyadtpulse-1.0.0.dist-info/METADATA
+Filename: pyadtpulse-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pyadtpulse-1.0.0.dist-info/WHEEL
+Filename: pyadtpulse-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyadtpulse-1.0.0.dist-info/top_level.txt
+Filename: pyadtpulse-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyadtpulse-1.0.0.dist-info/zip-safe
+Filename: pyadtpulse-1.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: pyadtpulse-1.0.0.dist-info/RECORD
+Filename: pyadtpulse-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyadtpulse/__init__.py

```diff
@@ -1,14 +1,14 @@
 """Base Python Class for pyadtpulse."""
 
 import logging
 import asyncio
-from random import uniform
 import re
 import time
+from random import uniform
 from threading import RLock, Thread
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import uvloop
 from aiohttp import (
     ClientConnectionError,
     ClientResponse,
@@ -31,18 +31,18 @@
     ADT_SYSTEM_URI,
     ADT_TIMEOUT_INTERVAL,
     ADT_TIMEOUT_URI,
     API_PREFIX,
     DEFAULT_API_HOST,
 )
 from pyadtpulse.util import (
+    AuthenticationException,
     DebugRLock,
     handle_response,
     make_soup,
-    AuthenticationException,
 )
 
 # FIXME -- circular reference
 # from pyadtpulse.site import ADTPulseSite
 
 if TYPE_CHECKING:
     from pyadtpulse.site import ADTPulseSite
@@ -107,61 +107,71 @@
                             Should be set to False for asynchronous usage
                             and async_login() should be called instead
                             Setting websession will override this
                             and not login
                         Defaults to True
             poll_interval (float, optional): number of seconds between update checks
         """
+        self._api_version: str = ADT_DEFAULT_VERSION
+        self._gateway_online: bool = False
+
         self._session = websession
         if self._session is not None:
             self._session.headers.update(ADT_DEFAULT_HTTP_HEADERS)
+
         self._init_login_info(username, password, fingerprint)
         self._user_agent = user_agent
-        self._api_version: str = ADT_DEFAULT_VERSION
 
         self._sync_task: Optional[asyncio.Task] = None
+        self._sync_timestamp = 0.0
         self._timeout_task: Optional[asyncio.Task] = None
+
         # FIXME use thread event/condition, regular condition?
         # defer initialization to make sure we have an event loop
         self._authenticated: Optional[asyncio.locks.Event] = None
+        self._login_exception: Optional[BaseException] = None
+
         self._updates_exist: Optional[asyncio.locks.Event] = None
+
+        self._last_timeout_reset = time.time()
+
         self._loop: Optional[asyncio.AbstractEventLoop] = None
         self._session_thread: Optional[Thread] = None
         self._attribute_lock: Union[RLock, DebugRLock]
         if not debug_locks:
             self._attribute_lock = RLock()
         else:
             self._attribute_lock = DebugRLock("PyADTPulse._attribute_lock")
-        self._last_timeout_reset = time.time()
-        self._sync_timestamp = 0.0
-        self._gateway_online: bool = False
-        self._login_exception: Optional[BaseException] = None
-        # fixme circular import, should be an ADTPulseSite
+
+        # FIXME: circular import, should be an ADTPulseSite
         if TYPE_CHECKING:
             self._sites: List[ADTPulseSite]
         else:
             self._sites: List[Any] = []
 
         self._api_host = service_host
         self._poll_interval = poll_interval
 
         # authenticate the user
         if do_login and self._session is None:
             self.login()
 
     def _init_login_info(self, username: str, password: str, fingerprint: str) -> None:
         if username is None or username == "":
-            raise ValueError("Username is madatory")
+            raise ValueError("Username is mandatory")
+
         pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b"
         if not re.match(pattern, username):
             raise ValueError("Username must be an email address")
         self._username = username
+
         if password is None or password == "":
             raise ValueError("Password is mandatory")
         self._password = password
+
         if fingerprint is None or fingerprint == "":
             raise ValueError("Fingerprint is required")
         self._fingerprint = fingerprint
 
     def __repr__(self) -> str:
         """Object representation."""
         return "<{}: {}>".format(self.__class__.__name__, self._username)
@@ -250,25 +260,23 @@
 
         Args:
             status (bool): True if gateway is online
         """
         with self._attribute_lock:
             if status == self._gateway_online:
                 return
-            if status:
-                LOG.warning(
-                    "ADT Pulse gateway is online, "
-                    f"setting poll interval to {self._poll_interval}"
-                )
-            else:
-                LOG.warning(
-                    "ADT Pulse gateway is offline, "
-                    "setting poll interval to"
-                    f"{ADT_GATEWAY_OFFLINE_POLL_INTERVAL}"
-                )
+
+            status_text = "ONLINE"
+            if not status:
+                status_text = "OFFLINE"
+                self._poll_interval = ADT_GATEWAY_OFFLINE_POLL_INTERVAL
+
+            LOG.warning(
+                f"ADT Pulse gateway {status_text}, poll interval={self._poll_interval}"
+            )
             self._gateway_online = status
 
     async def _async_fetch_version(self) -> None:
         with self._attribute_lock:
             result = None
             if self._session:
                 try:
@@ -278,14 +286,15 @@
                 except (ClientResponseError, ClientConnectionError):
                     LOG.warning(
                         "Error occurred during API version fetch, defaulting to"
                         f"{ADT_DEFAULT_VERSION}"
                     )
                     self._api_version = ADT_DEFAULT_VERSION
                     return
+
             if result is None:
                 LOG.warning(
                     "Error occurred during API version fetch, defaulting to"
                     f"{ADT_DEFAULT_VERSION}"
                 )
                 self._api_version = ADT_DEFAULT_VERSION
                 return
@@ -311,18 +320,15 @@
                 await self._initialize_sites(soup)
             else:
                 # FIXME: this will have to be fixed once multiple ADT sites
                 # are supported, since the summary_html only represents the
                 # alarm status of the current site!!
                 if len(self._sites) > 1:
                     LOG.error(
-                        (
-                            "pyadtpulse DOES NOT support an ADT account ",
-                            "with multiple sites yet!!!",
-                        )
+                        "pyadtpulse lacks support for ADT accounts with multiple sites!!!"
                     )
 
             for site in self._sites:
                 site._update_alarm_from_soup(soup)
                 site._update_zone_from_soup(soup)
 
     async def _initialize_sites(self, soup: BeautifulSoup) -> None:
@@ -338,30 +344,32 @@
             if signout_link:
                 m = re.search("networkid=(.+)&", signout_link)
                 if m and m.group(1) and m.group(1):
                     from pyadtpulse.site import ADTPulseSite
 
                     site_id = m.group(1)
                     LOG.debug(f"Discovered site id {site_id}: {site_name}")
+
                     # FIXME ADTPulseSite circular reference
                     new_site = ADTPulseSite(self, site_id, site_name)
+
                     # fetch zones first, so that we can have the status
                     # updated with _update_alarm_status
                     await new_site._fetch_zones(None)
                     new_site._update_alarm_from_soup(soup)
                     new_site._update_zone_from_soup(soup)
                     with self._attribute_lock:
                         self._sites.append(new_site)
                     return
             else:
                 LOG.warning(
                     f"Couldn't find site id for '{site_name}' in '{signout_link}'"
                 )
         else:
-            LOG.error(("ADT Pulse accounts with MULTIPLE sites not supported!!!"))
+            LOG.error("ADT Pulse accounts with MULTIPLE sites not supported!!!")
 
     # ...and current network id from:
     # <a id="p_signout1" class="p_signoutlink"
     # href="/myhome/16.0.0-131/access/signout.jsp?networkid=150616za043597&partner=adt"
     # onclick="return flagSignOutInProcess();">
     #
     # ... or perhaps better, just extract all from /system/settings.jsp
@@ -393,28 +401,35 @@
                 LOG.debug("ADT Pulse timeout task cancelled")
                 self._close_response(response)
                 return
 
     def _pulse_session_thread(self) -> None:
         # lock is released in sync_loop()
         self._attribute_lock.acquire()
-        LOG.debug("creating Pulse background thread")
+
+        LOG.debug("Creating ADT Pulse background thread")
         asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
         self._loop = asyncio.new_event_loop()
         self._loop.run_until_complete(self._sync_loop())
+
         self._loop.close()
         self._loop = None
         self._session_thread = None
 
     async def _sync_loop(self) -> None:
         result = await self.async_login()
         self._attribute_lock.release()
         if result:
             if self._sync_task is not None and self._timeout_task is not None:
-                await asyncio.wait((self._sync_task, self._timeout_task))
+                try:
+                    await asyncio.wait((self._sync_task, self._timeout_task))
+                except Exception as e:
+                    LOG.exception(
+                        f"Received exception while waiting for ADT Pulse service"
+                    )
             else:
                 # we should never get here
                 raise RuntimeError("Background pyadtpulse tasks not created")
 
     def login(self) -> None:
         """Login to ADT Pulse and generate access token.
 
@@ -425,16 +440,18 @@
         # probably shouldn't be a daemon thread
         self._session_thread = thread = Thread(
             target=self._pulse_session_thread,
             name="PyADTPulse Session",
             daemon=True,
         )
         self._attribute_lock.release()
+
         self._session_thread.start()
         time.sleep(1)
+
         # thread will unlock after async_login, so attempt to obtain
         # lock to block current thread until then
         # if it's still alive, no exception
         self._attribute_lock.acquire()
         self._attribute_lock.release()
         if not thread.is_alive():
             raise AuthenticationException(self._username)
@@ -467,14 +484,15 @@
         if self._session is None:
             self._session = ClientSession()
         self._session.headers.update(ADT_DEFAULT_HTTP_HEADERS)
         if self._authenticated is None:
             self._authenticated = asyncio.locks.Event()
         else:
             self._authenticated.clear()
+
         LOG.debug(f"Authenticating to ADT Pulse cloud service as {self._username}")
         await self._async_fetch_version()
 
         response = await self._async_query(
             ADT_LOGIN_URI,
             method="POST",
             extra_params={
@@ -548,14 +566,15 @@
 
     def logout(self) -> None:
         """Log out of ADT Pulse."""
         with self._attribute_lock:
             if self._loop is None:
                 raise RuntimeError("Attempting to call sync logout without sync login")
             sync_thread = self._session_thread
+
         coro = self.async_logout()
         asyncio.run_coroutine_threadsafe(coro, self._loop)
         if sync_thread is not None:
             sync_thread.join()
 
     async def _sync_check_task(self) -> None:
         LOG.debug("creating Pulse sync check task")
@@ -570,21 +589,24 @@
                     pi = self.poll_interval
                 else:
                     LOG.warning(
                         "Pulse gateway detected offline, polling every "
                         f"{ADT_GATEWAY_OFFLINE_POLL_INTERVAL} seconds"
                     )
                     pi = ADT_GATEWAY_OFFLINE_POLL_INTERVAL
+
                 await asyncio.sleep(pi)
                 response = await self._async_query(
                     ADT_SYNC_CHECK_URI,
                     extra_params={"ts": int(self._sync_timestamp * 1000)},
                 )
+
                 if response is None:
                     continue
+
                 text = await response.text()
                 if not handle_response(
                     response, logging.ERROR, "Error querying ADT sync"
                 ):
                     self._close_response(response)
                     continue
 
@@ -606,17 +628,19 @@
                     )
                     self._close_response(response)
                     self._sync_timestamp = time.time()
                     self._updates_exist.set()
                     if await self.async_update() is False:
                         LOG.debug("Pulse data update from sync task failed")
                     continue
+
                 LOG.debug(f"Sync token {text} indicates no remote updates to process")
                 self._close_response(response)
                 self._sync_timestamp = time.time()
+
             except asyncio.CancelledError:
                 LOG.debug("ADT Pulse sync check task cancelled")
                 self._close_response(response)
                 return
 
     @property
     def updates_exist(self) -> bool:
@@ -624,27 +648,29 @@
 
         Returns:
             bool: True if updated data exists
         """
         with self._attribute_lock:
             if self._updates_exist is None:
                 return False
+
             if self._updates_exist.is_set():
                 self._updates_exist.clear()
                 return True
             return False
 
     async def wait_for_update(self) -> None:
         """Wait for update.
 
         Blocks current async task until Pulse system
         signals an update
         """
         if self._updates_exist is None:
             raise RuntimeError("Update event does not exist")
+
         await self._updates_exist.wait()
         self._updates_exist.clear()
 
     @property
     def is_connected(self) -> bool:
         """Check if connected to ADT Pulse.
 
@@ -719,28 +745,30 @@
                     async with self._session.post(
                         url, headers=extra_headers, data=extra_params, timeout=timeout
                     ) as response:
                         await response.text()
                 else:
                     LOG.error(f"Invalid request method {method}")
                     return None
+
                 if response.status in RECOVERABLE_ERRORS:
                     retry = retry + 1
                     LOG.warning(
                         f"pyadtpulse query returned recover error code "
                         f"{response.status}, retrying (count ={retry})"
                     )
                     if retry == max_retries:
                         LOG.warning(
                             "pyadtpulse exceeded max retries of "
                             f"{max_retries}, giving up"
                         )
                         response.raise_for_status()
                     await asyncio.sleep(2**retry + uniform(0.0, 1.0))
                     continue
+
                 response.raise_for_status()
                 # success, break loop
                 retry = 4
             except ClientResponseError as err:
                 code = err.code
                 LOG.exception(
                     f"Received HTTP error code {code} in request to ADT Pulse"
```

## pyadtpulse/site.py

```diff
@@ -1,8 +1,9 @@
 """Module representing an ADT Pulse Site."""
+
 import logging
 import re
 from asyncio import get_event_loop, run_coroutine_threadsafe
 from datetime import datetime, timedelta
 from threading import RLock
 from typing import List, Optional, Union
 
@@ -28,15 +29,15 @@
 ADT_ALARM_DISARMING = "disarming"
 ADT_ARM_DISARM_TIMEOUT = timedelta(seconds=20)
 
 
 LOG = logging.getLogger(__name__)
 
 
-class ADTPulseSite(object):
+class ADTPulseSite:
     """Represents an individual ADT Pulse site."""
 
     __slots__ = (
         "_adt_service",
         "_id",
         "_name",
         "_status",
@@ -225,14 +226,15 @@
         soup = await make_soup(
             response,
             logging.WARNING,
             f"Failed updating ADT Pulse alarm {self._name} to {mode}",
         )
         if soup is None:
             return False
+
         arm_result = soup.find("div", {"class": "p_armDisarmWrapper"})
         if arm_result is not None:
             error_block = arm_result.find("div")
             if error_block is not None:
                 error_text = arm_result.get_text().replace("Arm AnywayCancel\n\n", "")
                 LOG.warning(
                     f"Could not set alarm state to {mode} " f"because {error_text}"
@@ -348,14 +350,15 @@
         LOG.debug("Updating alarm status")
         value = summary_html_soup.find("span", {"class": "p_boldNormalTextLarge"})
         sat_location = "security_button_0"
         with self._site_lock:
             if value:
                 text = value.text
                 last_updated = datetime.now()
+
                 if re.match("Disarmed", text):
                     if (
                         self._status != ADT_ALARM_ARMING
                         or last_updated - self._last_arm_disarm > ADT_ARM_DISARM_TIMEOUT
                     ):
                         self._status = ADT_ALARM_OFF
                         self._last_updated = last_updated
@@ -376,14 +379,15 @@
                 else:
                     LOG.warning(f"Failed to get alarm status from '{text}'")
                     self._adt_service._set_gateway_status(False)
                     self._status = ADT_ALARM_UNKNOWN
                     self._last_updated = last_updated
                     return
                 LOG.debug(f"Alarm status = {self._status}")
+
             if self._sat == "":
                 sat_button = summary_html_soup.find(
                     "input", {"type": "button", "id": sat_location}
                 )
                 if sat_button and sat_button.has_attr("onclick"):
                     on_click = sat_button["onclick"]
                     match = re.search(r"sat=([a-z0-9\-]+)", on_click)
@@ -613,14 +617,15 @@
                     return None
                 if state != "Unknown":
                     gateway_online = True
                 self._zones.update_state(zone, state)
                 self._zones.update_last_activity_timestamp(zone, last_update)
 
                 LOG.debug(f"Set zone {zone} - to {state} with timestamp {last_update}")
+
             self._adt_service._set_gateway_status(gateway_online)
             self._last_updated = datetime.now()
             return self._zones
 
     async def _async_update_zones(self) -> Optional[List[ADTPulseFlattendZone]]:
         """Update zones asynchronously.
```

## Comparing `pyadtpulse-1.0.0.dist-info/LICENSE.md` & `pyadtpulse-1.0.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyadtpulse-1.0.0.dist-info/METADATA` & `pyadtpulse-1.0.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyadtpulse
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python interface for ADT Pulse security systems
 Home-page: https://github.com/rsnodgrass/pyadtpulse
 Author: 
 Author-email: 
 License: Apache Software License
 Keywords: security system,adt,home automation,security alarm
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,19 @@
 arm/disarm support and none provided support for ADT Pulse when multiple sites existed
 under a single account. This attempts to provide APIs to both all the zones (motion 
 sensors, door sensors, etc) as well as arming and disarming individual sites.
 
 NOTE: Since this interacts with the unofficial ADT Pulse AJAX web service, the
 behavior is subject to change by ADT without notice.
 
+## Developer Note
+
+NOTE: This package use [pre-commit](https://pre-commit.com/) hooks for maintaining code quality.
+Please install pre-commit and enable it for your local git copy before committing.
+
 ## WARNING
 
 Do not reauthenticate to the ADT service frequently as ADT's service is not designed for high volume requests. E.g. every 5 minutes, not seconds. Keep your authenticated session to avoid logging in repeatedly.
 
 ## Installation
 
 ```
```

## Comparing `pyadtpulse-1.0.0.dist-info/RECORD` & `pyadtpulse-1.0.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyadtpulse/__init__.py,sha256=sHh5Ze-8PwVPu-qdMfjl5AHumrQvlsGCWHVMvIoKA2c,30683
+pyadtpulse/__init__.py,sha256=4v7UmlYB5D99BTWus3kjP9aYqqO70AM9zGXHFRUVYYU,30711
 pyadtpulse/const.py,sha256=q3xJ93olyh9pNKvywARCwsu9qnr-E8O3SkD8Z4BEGBw,1609
-pyadtpulse/site.py,sha256=6EzvAkp6VduCX6YKimFdL6WPkFwkuWwhp8h6F6hILAw,24101
+pyadtpulse/site.py,sha256=LJ6DIpZZTghO4cBbzNItpUipfY5tpjYWBO0IV_hVv8o,24098
 pyadtpulse/util.py,sha256=aTsrbEWoYkaAxnN0pU_ZoQ6eqyWTx-4_Ukihq8wwb88,4803
 pyadtpulse/zones.py,sha256=ZLdySMMGxMSvKGHqe9cDvFgchXlXnuCc-FFNRQSLqhE,5089
-pyadtpulse-1.0.0.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
-pyadtpulse-1.0.0.dist-info/METADATA,sha256=9FQXQ1pkantLv7gZY_fzzU4tX9P47LBfMUJsYqWEuZY,3446
-pyadtpulse-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyadtpulse-1.0.0.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
-pyadtpulse-1.0.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pyadtpulse-1.0.0.dist-info/RECORD,,
+pyadtpulse-1.0.1.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
+pyadtpulse-1.0.1.dist-info/METADATA,sha256=WoeWuL63GcJsL9FoPNgmmTM0RJvL6NzYLgGB5fBFmvU,3646
+pyadtpulse-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyadtpulse-1.0.1.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
+pyadtpulse-1.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyadtpulse-1.0.1.dist-info/RECORD,,
```

