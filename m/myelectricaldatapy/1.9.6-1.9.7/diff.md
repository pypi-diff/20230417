# Comparing `tmp/myelectricaldatapy-1.9.6.tar.gz` & `tmp/myelectricaldatapy-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-1.9.6.tar", last modified: Fri Apr 14 06:38:39 2023, max compression
+gzip compressed data, was "myelectricaldatapy-1.9.7.tar", last modified: Mon Apr 17 15:27:33 2023, max compression
```

## Comparing `myelectricaldatapy-1.9.6.tar` & `myelectricaldatapy-1.9.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/mypdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-14 06:38:37.000000 myelectricaldatapy-1.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.639300 myelectricaldatapy-1.9.7/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/myelectricaldatapy/mypdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 15:27:33.000000 myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-17 15:27:32.000000 myelectricaldatapy-1.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:33.643300 myelectricaldatapy-1.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-17 15:27:23.000000 myelectricaldatapy-1.9.7/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-1.9.6/LICENSE` & `myelectricaldatapy-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.6/PKG-INFO` & `myelectricaldatapy-1.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.6
+Version: 1.9.7
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.6/README.md` & `myelectricaldatapy-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.6/myelectricaldatapy/analytics.py` & `myelectricaldatapy-1.9.7/myelectricaldatapy/analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,16 @@
                             ] = (
                                 self.df.value * price
                             )
                         elif offset == "price":
                             self.df.loc[(self.df.notes == mode), "price"] = (
                                 self.df.value * price
                             )
+                        else:
+                            self.df.loc[(self.df.notes == mode), "price"] = None
 
             if summary:
                 for note in notes:
                     self.df.loc[(self.df.notes == note), "sum_price"] = self.df[
                         (self.df.notes == note)
                     ].price.cumsum() + cum_price.get(note, 0)
```

### Comparing `myelectricaldatapy-1.9.6/myelectricaldatapy/auth.py` & `myelectricaldatapy-1.9.7/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.6/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-1.9.7/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.6/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-1.9.7/myelectricaldatapy/mypdl.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,34 +90,42 @@
         token: str,
         session: Any | None = None,
         timeout: int = TIMEOUT,
     ) -> None:
         """Initialize."""
         self._api: Enedis = Enedis(token, session, timeout)
         self.pdl = pdl
-        self._tempo_subs: bool = False
-        self._off_subs: bool = False
+        self._connected: bool = False
         self._ecowatt_subs: bool = False
         self._maxpower_subs: bool = False
-        self.intervals: list[Tuple[str, str]] = []
+        self._off_subs: bool = False
+        self._params: dict[str, dict[str, Any]] = {}
+        self._tempo_subs: bool = False
         self.access: dict[str, Any] = {}
-        self.contract: dict[str, Any] = {}
         self.address: dict[str, Any] = {}
-        self.tempo: dict[str, Any] = {}
+        self.contract: dict[str, Any] = {}
         self.ecowatt: dict[str, Any] = {}
+        self.has_collected: bool = False
+        self.intervals: list[Tuple[str, str]] = []
+        self.last_access: dt = dt.now()
+        self.last_refresh: dt | None = None
         self.max_power: dict[str, Any] = {}
-        self._connected: bool = False
-        self._params: dict[str, dict[str, Any]] = {PRODUCTION: {}, CONSUMPTION: {}}
+        self.tempo: dict[str, Any] = {}
 
     @property
     def is_connected(self) -> bool:
         """Connect state."""
         return self.access.get("valid", False) is True
 
     @property
+    def is_quota_reached(self) -> bool:
+        """Check quota."""
+        return self.access.get("quota_reached", True) is True
+
+    @property
     def has_intervals(self) -> bool:
         """Intervals exist."""
         return len(self.intervals) > 0
 
     @property
     def ecowatt_day(self) -> dict[str, Any]:
         """ecowatt."""
@@ -141,19 +149,15 @@
         return self._params[CONSUMPTION].get(ATTR_PRICES)
 
     @property
     def stats(self) -> dict[str, Any]:
         """Statistics."""
         stats = {}
         for mode, params in self._params.items():
-            data = (
-                params.get("dataset", {})
-                .get("meter_reading", {})
-                .get("interval_reading", {})
-            )
+            data = params.get("data", {})
             analytics = EnedisAnalytics(data)
             resultat = analytics.get_data_analytics(
                 convertKwh=True,
                 convertUTC=False,
                 intervals=params.get(ATTR_INTERVALS, []),
                 groupby=True,
                 summary=True,
@@ -162,68 +166,41 @@
                 cum_price=params.get(ATTR_CUM_PRICE, {}),
                 start_date=params.get(ATTR_START),
                 tempo=self.tempo,
             )
             stats.update({mode: resultat})
         return stats
 
-    async def async_update(self, modes: dict[str, Any] | None = None) -> None:
-        """Update data.
-
-        modes = {
-            "consumption":{
-                "service":["daily_consumption" | "consumption_load_curve"],
-                start: [date],
-                end: [date]
-            },
-            "production":{
-                "service":["daily_production" | "production_load_curve"],
-                start: [date],
-                end: [date]
-            }
-        }
-        """
-        start = dt.now() - timedelta(days=1095)
-        end = dt.now() + timedelta(days=1)
-        funcs: dict[str, Callable[..., Any]] = {
-            DAILY_PROD: self._api.async_get_daily_production,
-            DETAIL_PROD: self._api.async_get_details_production,
-            DAILY_CONSUM: self._api.async_get_daily_consumption,
-            DETAIL_CONSUM: self._api.async_get_details_consumption,
-        }
-
+    async def async_update(self, force_refresh: bool = False) -> None:
+        """Update data."""
         self.access = await self._api.async_valid_access(self.pdl)
-        self.contract = await self._api.async_get_contract(self.pdl)
-        self.address = await self._api.async_get_address(self.pdl)
-        if self._ecowatt_subs:
-            self.ecowatt = await self._api.async_get_ecowatt(start, end)
-        if self._maxpower_subs:
-            self.max_power = await self._api.async_get_max_power(self.pdl, start, end)
-        if modes:
-            try:
-                validate = MODES_SCH(modes)
-            except vol.Error as error:
-                _LOGGER.error("The format is incorrect. (%s)", error)
-            else:
-                for mode, params in validate.items():
-                    service = params.get(ATTR_SERVICE)
-                    days = 370 if service in [DAILY_PROD, DAILY_CONSUM] else 7
-                    func = funcs[params.get(ATTR_SERVICE)]
-                    dt_start = (
-                        params.get(ATTR_START)
-                        if params.get(ATTR_START)
-                        else dt.now() - timedelta(days=days)
-                    )
-                    dt_end = params.get(ATTR_END) if params.get(ATTR_END) else end
-                    dataset = await func(self.pdl, dt_start, dt_end)
-                    self._params[mode].update(
-                        {"dataset": dataset, ATTR_START: dt_start}
-                    )
-                    if service in [DAILY_CONSUM, DETAIL_CONSUM] and self._tempo_subs:
-                        self.tempo = await self._api.async_get_tempo(dt_start, dt_end)
+        if "last_call" in self.access:
+            d_last_call = dt.strptime(
+                self.access["last_call"], "%Y-%m-%dT%H:%M:%S.%f"
+            ).date()
+            start = dt.now() - timedelta(days=1095)
+            end = dt.now() + timedelta(days=1)
+            if not self.contract or d_last_call != dt.now().date():
+                self.contract = await self._api.async_get_contract(self.pdl)
+            if not self.address or d_last_call != dt.now().date():
+                self.address = await self._api.async_get_address(self.pdl)
+            if self._ecowatt_subs:
+                self.ecowatt = await self._api.async_get_ecowatt(start, end)
+            if self._maxpower_subs:
+                self.max_power = await self._api.async_get_max_power(
+                    self.pdl, start, end
+                )
+            if self._params and (
+                d_last_call != dt.now().date()
+                or self.has_collected is False
+                or force_refresh is True
+            ):
+                await self.async_update_collects()
+                self.last_refresh = dt.now()
+            self.last_access = dt.now()
 
     def tempo_subscription(self, activate: bool = False) -> None:
         """Enable or Disable Tempo Subscription."""
         self._off_subs = False
         self._tempo_subs = activate is True
 
     def offpeak_subscription(self, activate: bool = False) -> None:
@@ -235,25 +212,21 @@
         """Enable or Disable Ecowatt Subscription."""
         self._ecowatt_subs = activate is True
 
     def maxpower_subscription(self, activate: bool = False) -> None:
         """Enable or Disable Max power Subscription."""
         self._maxpower_subs = activate is True
 
-    def set_intervals(self, mode: str, intervals: list[Tuple[str, str]]) -> None:
+    def _set_intervals(self, mode: str, intervals: list[Tuple[str, str]]) -> None:
         """Set intervals."""
         if isinstance(intervals, list):
             self.intervals = intervals
             self._params[mode].update({ATTR_INTERVALS: intervals})
 
-    def set_prices(
-        self,
-        mode: str,
-        prices: dict[str, Any],
-    ) -> None:
+    def _set_prices(self, mode: str, prices: dict[str, Any]) -> None:
         """Set intervals.
 
         prices = {
             "standard":{"price":[float]},
             "offpeak":{"price":[float]}
         }
         or
@@ -272,20 +245,72 @@
             else:
                 self.tempo_subscription(True)
                 self._params[mode].update({ATTR_PRICES: validate})
         else:
             self.offpeak_subscription(True)
             self._params[mode].update({ATTR_PRICES: validate})
 
-    def set_cumsum(self, mode: str, form: str, cum_sum: dict[str, Any]) -> None:
+    def _set_cumsum(self, mode: str, form: str, cum_sum: dict[str, Any]) -> None:
         """Set cumulative summary.
 
         mode: "production" or "consumption"
         format: "value" or "price"
         cum_sum = {"standard":[float], "offpeak":[float]}
         """
         try:
             validate = CUM_SCH(cum_sum)
         except vol.Error as error:
             _LOGGER.error("Format is incorrect (%s)", error)
         else:
             self._params[mode].update({f"cum_{form}".lower(): validate})
+
+    def set_collects(
+        self,
+        service: str,
+        start: dt | None = None,
+        end: dt | None = None,
+        intervals: list[Tuple[str, str]] | None = None,
+        prices: dict[str, Any] | None = None,
+        cum_value: dict[str, Any] | None = None,
+        cum_price: dict[str, Any] | None = None,
+    ) -> None:
+        """Set datas collect."""
+        funcs: dict[str, Callable[..., Any]] = {
+            DAILY_PROD: self._api.async_get_daily_production,
+            DETAIL_PROD: self._api.async_get_details_production,
+            DAILY_CONSUM: self._api.async_get_daily_consumption,
+            DETAIL_CONSUM: self._api.async_get_details_consumption,
+        }
+        days = 1095 if service in [DAILY_PROD, DAILY_CONSUM] else 7
+        mode = CONSUMPTION if service in [DAILY_CONSUM, DETAIL_CONSUM] else PRODUCTION
+        func = funcs[service]
+        dt_start = start if start else dt.now() - timedelta(days=days)
+        dt_end = end if end else dt.now() + timedelta(days=1)
+        self._params[mode] = {"func": func, ATTR_START: dt_start, ATTR_END: dt_end}
+        if intervals:
+            self._set_intervals(mode, intervals)
+        if prices:
+            self._set_prices(mode, prices)
+        if cum_value:
+            self._set_cumsum(mode, "value", cum_value)
+        if cum_price:
+            self._set_cumsum(mode, "price", cum_price)
+
+    async def async_update_collects(self) -> None:
+        """Update data to collect."""
+        dataset = {}
+        checked = True
+        self.has_collected = False
+        for mode, _param in self._params.items():
+            start = _param[ATTR_START]
+            end = _param[ATTR_END]
+            if func := _param.get("func"):
+                dataset = await func(self.pdl, start, end)
+                data = dataset.get("meter_reading", {}).get("interval_reading", {})
+                if len(data) != 0:
+                    checked = checked and len(data) != 0
+                    self._params[mode].pop("func")
+                    self._params[mode].update({"data": data})
+                if mode == CONSUMPTION and self._tempo_subs:
+                    self.tempo = await self._api.async_get_tempo(start, end)
+
+        self.has_collected = checked
```

### Comparing `myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.6
+Version: 1.9.7
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-1.9.7/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 myelectricaldatapy/mypdl.py
 myelectricaldatapy.egg-info/PKG-INFO
 myelectricaldatapy.egg-info/SOURCES.txt
 myelectricaldatapy.egg-info/dependency_links.txt
 myelectricaldatapy.egg-info/requires.txt
 myelectricaldatapy.egg-info/top_level.txt
 tests/__init__.py
+tests/conftest.py
 tests/consts.py
 tests/test_analytics.py
 tests/test_load_data.py
```

### Comparing `myelectricaldatapy-1.9.6/pyproject.toml` & `myelectricaldatapy-1.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.6/setup.py` & `myelectricaldatapy-1.9.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="myelectricaldatapy",
-    version="1.9.6",
+    version="1.9.7",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Fetch Linky data from myelectricaldata.fr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "pandas==1.4.3", "voluptuous>=0.13.1"],
```

### Comparing `myelectricaldatapy-1.9.6/tests/consts.py` & `myelectricaldatapy-1.9.7/tests/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ACCESS = {
     "valid": True,
     "consent_expiration_date": "2026-01-14T15:32:38",
     "call_number": 7,
     "quota_reached": False,
     "quota_limit": 50,
-    "quota_reset_at": "2023-01-14T23:59:59.999999",
-    "last_call": "2023-01-07T13:58:24.532501",
+    "quota_reset_at": "2023-03-01T23:59:59.999999",
+    "last_call": "2023-03-01T13:58:24.532501",
     "ban": False,
 }
 
 INVALID_ACCESS = {
     "valid": False,
     "information": "Vous avez dépassé votre quota journalier (50)",
     "consent_expiration_date": "2026-01-14T15:32:38",
     "call_number": 65,
     "quota_reached": True,
     "quota_limit": 50,
-    "quota_reset_at": "2023-01-14T23:59:59.999999",
+    "quota_reset_at": "2023-01-07T23:59:59.999999",
     "last_call": "2023-01-07T13:58:24.532501",
     "ban": False,
 }
 TEMPO = {"2023-3-1": "blue", "2023-3-2": "red", "2023-3-3": "blue"}
 INVALID_ECOWATT = {
     "detail": "Pas de données disponible entre la date du 2023-01-22 00:00:00 et 2023-01-22 00:00:00"  # noqa
 }
```

### Comparing `myelectricaldatapy-1.9.6/tests/test_analytics.py` & `myelectricaldatapy-1.9.7/tests/test_analytics.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,258 +1,219 @@
 """Tests analytics."""
 from __future__ import annotations
 
 from datetime import datetime as dt
 from typing import Any
-from unittest.mock import patch
+from unittest.mock import Mock, patch
 
 import pytest
 from freezegun import freeze_time
 
 import myelectricaldatapy
 from myelectricaldatapy import EnedisByPDL
 
-from .consts import ACCESS
-from .consts import DATASET_30 as DS_30
-from .consts import DATASET_DAILY as DS_DAILY
-from .consts import DATASET_DAILY_COMPARE as DS_COMPARE
-from .consts import TEMPO
+from .consts import DATASET_DAILY_COMPARE
 
 PDL = "012345"
 TOKEN = "xxxxxxxxxxxxx"
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_compute() -> None:
+async def test_compute(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test standard."""
-    dataset = DS_30
-    modes = {"consumption": {"service": "consumption_load_curve"}}
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("consumption_load_curve")
+    await api.async_update()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert resultat[0]["value"] == 1.296
 
-    dataset = DS_DAILY
-    modes = {"consumption": {"service": "daily_consumption"}}
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api = EnedisByPDL(pdl=PDL, token=TOKEN)
+    api.set_collects("daily_consumption")
+    await api.async_update()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert resultat[0]["value"] == 42.045
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_without_offpeak() -> None:
+async def test_without_offpeak(
+    mock_enedis: Mock,
+) -> None:  # pylint: disable=unused-argument
     """Test without offpeak , with price."""
-    dataset = DS_30
+    await mock_enedis()
     prices: dict[str, Any] = {"standard": {"price": 0.17}}
-    modes = {"consumption": {"service": "consumption_load_curve"}}
     # Test standard price
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_prices("consumption", prices)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("consumption_load_curve", prices=prices)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert round(resultat[0]["price"], 2) == 0.22
 
-    dataset = DS_DAILY
-    modes = {"consumption": {"service": "daily_consumption"}}
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("daily_consumption", prices=prices)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert round(resultat[0]["price"], 2) == 7.15
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_with_offpeak() -> None:
+async def test_with_offpeak(
+    mock_enedis: Mock,  # pylint: disable=unused-argument
+) -> None:
     """Test without offpeak , with price."""
-    dataset = DS_30
     intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
     prices: dict[str, Any] = {"standard": {"price": 0.17}, "offpeak": {"price": 0.18}}
-    modes = {"consumption": {"service": "consumption_load_curve"}}
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("consumption_load_curve", prices=prices, intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "offpeak"
     assert resultat[0]["value"] == 1.079
     assert resultat[0].get("sum_value") is not None
     assert resultat[0].get("sum_price") is not None
     print(resultat)
 
     # Without cums
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("consumption_load_curve", prices=prices, intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "offpeak"
     assert resultat[0]["value"] == 1.079
     assert round(resultat[2]["price"], 3) == 0.833
     assert resultat[0].get("sum_value") == 1.079
     print(resultat)
 
     # Whitout price
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("consumption_load_curve", intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
     assert resultat[27]["value"] == 1.296
     assert resultat[28]["value"] == 0.618
     print(resultat)
 
     # Daily
-    dataset = DS_DAILY
-    modes = {"consumption": {"service": "daily_consumption"}}
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_prices("consumption", prices)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("daily_consumption", prices=prices, intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["value"] == 42.045
     print(resultat)
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_daily_with_offpeak() -> None:
+async def test_daily_with_offpeak(
+    mock_enedis: Mock,  # pylint: disable=unused-argument
+) -> None:
     """Test daily with offpeak."""
     prices: dict[str, Any] = {"standard": {"price": 0.17}, "offpeak": {"price": 0.18}}
     intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
-    modes = {"consumption": {"service": "daily_consumption"}}
-    dataset = DS_DAILY
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects("daily_consumption", prices=prices, intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
     assert resultat[359]["value"] == 68.68
     print(resultat)
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_compare() -> None:
+async def test_compare(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test details compare."""
     prices: dict[str, Any] = {"standard": {"price": 0.17}, "offpeak": {"price": 0.18}}
     cumsum_value: dict[str, Any] = {
         "standard": {"sum_value": 0},
         "offpeak": {"sum_value": 0},
     }
     cumsum_price: dict[str, Any] = {
         "standard": {"sum_price": 0},
         "offpeak": {"sum_price": 0},
     }
     intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
-    dataset = DS_30
-    modes = {"consumption": {"service": "consumption_load_curve"}}
-
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    api.set_cumsum("consumption", "value", cumsum_value)
-    api.set_cumsum("consumption", "price", cumsum_price)
-
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat1 = api.stats["consumption"]
+    api.set_collects(
+        "consumption_load_curve",
+        prices=prices,
+        intervals=intervals,
+        cum_value=cumsum_value,
+        cum_price=cumsum_price,
+    )
+    await api.async_update()
+    resultat1 = api.stats["consumption"]
 
     print(resultat1)
     sum_value = 0
     for rslt in resultat1:
-        sum_value = sum_value + rslt["value"]
-
+        sum_value += rslt["value"]
     sum_value_1 = resultat1[26]["sum_value"] + resultat1[77]["sum_value"]
     assert round(sum_value, 3) == round(sum_value_1, 3)
-    dataset = DS_COMPARE
+
     with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
+        myelectricaldatapy.Enedis,
+        "async_get_daily_consumption",
+        return_value=DATASET_DAILY_COMPARE,
+    ):
+        api.set_collects(
+            "daily_consumption",
+            prices=prices,
+            intervals=intervals,
+            cum_value=cumsum_value,
+            cum_price=cumsum_price,
+        )
+        await api.async_update(force_refresh=True)
         resultat2 = api.stats["consumption"]
     assert round(sum_value, 3) == resultat2[2]["sum_value"]
     print(resultat2)
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_cumsums() -> None:
+async def test_cumsums(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test cummulative summary."""
     prices: dict[str, Any] = {"standard": {"price": 0.17}, "offpeak": {"price": 0.18}}
     cumsum_value: dict[str, Any] = {"standard": 100, "offpeak": 1000}
     cumsum_price: dict[str, Any] = {"standard": 50, "offpeak": 75}
     intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
-    dataset = DS_30
-    modes = {
-        "consumption": {
-            "service": "consumption_load_curve",
-            "start": dt.strptime("2023-03-01", "%Y-%m-%d"),
-            "end": dt.strptime("2023-03-08", "%Y-%m-%d"),
-        }
-    }
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    api.set_cumsum("consumption", "value", cumsum_value)
-    api.set_cumsum("consumption", "price", cumsum_price)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects(
+        "consumption_load_curve",
+        start=dt.strptime("2023-03-01", "%Y-%m-%d"),
+        end=dt.strptime("2023-03-08", "%Y-%m-%d"),
+        prices=prices,
+        intervals=intervals,
+        cum_value=cumsum_value,
+        cum_price=cumsum_price,
+    )
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
     # offpeak
     assert resultat[0]["sum_value"] == resultat[0]["value"] + 1000
     assert resultat[0]["sum_price"] == resultat[0]["price"] + 75
     # standard
     assert resultat[27]["sum_value"] == resultat[27]["value"] + 100
     assert resultat[27]["sum_price"] == resultat[27]["price"] + 50
 
 
 @freeze_time("2023-3-1")
 @pytest.mark.asyncio
-async def test_tempo() -> None:
+async def test_tempo(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test tempo pricings."""
     prices: dict[str, Any] = {
         "standard": {
             "blue": 0.2,
             "white": 0.3,
             "red": 3,
         },
@@ -261,108 +222,71 @@
             "white": 0.2,
             "red": 1.5,
         },
     }
     cumsum_value: dict[str, Any] = {"standard": 100, "offpeak": 1000}
     cumsum_price: dict[str, Any] = {"standard": 50, "offpeak": 75}
     intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
-    dataset = DS_30
-    modes = {"consumption": {"service": "consumption_load_curve"}}
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    api.set_cumsum("consumption", "value", cumsum_value)
-    api.set_cumsum("consumption", "price", cumsum_price)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ), patch.object(myelectricaldatapy.Enedis, "async_get_tempo", return_value=TEMPO):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
+    api.set_collects(
+        "consumption_load_curve",
+        prices=prices,
+        intervals=intervals,
+        cum_value=cumsum_value,
+        cum_price=cumsum_price,
+    )
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
 
     assert resultat[0]["tempo"] == "blue"
     assert resultat[0]["value"] == 1.079
     assert resultat[0]["sum_price"] == resultat[0]["price"] + 75
     assert resultat[0]["sum_value"] == resultat[0]["value"] + 1000
     assert api.tempo_day == "blue"
 
     # Check Daily -> compute not possible.
-    dataset = DS_DAILY
-    modes = {"production": {"service": "daily_production"}}
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ), patch.object(myelectricaldatapy.Enedis, "async_get_tempo", return_value=TEMPO):
-        await api.async_update(modes=modes)
-        resultat = api.stats["production"]
+    api.set_collects("daily_production", prices=prices, intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats.get("production")
     assert resultat[0].get("tempo") is None
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_standard_offpeak_cumsum() -> None:
+async def test_standard_offpeak_cumsum(
+    mock_enedis: Mock,  # pylint: disable=unused-argument
+) -> None:
     """Test with offpeak and cumsum."""
     prices: dict[str, Any] = {"standard": {"price": 0.5}, "offpeak": {"price": 1}}
     intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
-    dataset = DS_30
-    modes = {"consumption": {"service": "consumption_load_curve"}}
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
-
+    api.set_collects("consumption_load_curve", prices=prices, intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
     assert resultat[0]["value"] == 1.079
 
     # Test daily data , check ignore intervals.
-    dataset = DS_DAILY
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    api.set_intervals("consumption", intervals)
-    api.set_prices("consumption", prices)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
-
+    api.set_collects("daily_consumption", prices=prices, intervals=intervals)
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
     assert resultat[0]["price"] == resultat[0]["value"] * 0.5
 
 
 @pytest.mark.asyncio
-async def test_start_date() -> None:
+async def test_start_date(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test with start_date."""
-    dataset = DS_DAILY
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
-    modes = {
-        "consumption": {
-            "service": "consumption_load_curve",
-            "start": dt.strptime("2023-3-7", "%Y-%m-%d"),
-        }
-    }
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ), patch.object(
-        myelectricaldatapy.Enedis, "async_valid_access", return_value=ACCESS
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
-
-    print(resultat)
+    api.set_collects(
+        "consumption_load_curve", start=dt.strptime("2023-3-7", "%Y-%m-%d")
+    )
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
     assert len(resultat) == 0
 
-    dataset = DS_30
-    modes = {
-        "consumption": {
-            "service": "consumption_load_curve",
-            "start": dt.strptime("2023-3-7", "%Y-%m-%d"),
-        }
-    }
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ):
-        await api.async_update(modes=modes)
-        resultat = api.stats["consumption"]
-
-    print(resultat)
+    api.set_collects(
+        "consumption_load_curve", start=dt.strptime("2023-3-7", "%Y-%m-%d")
+    )
+    await api.async_update_collects()
+    resultat = api.stats["consumption"]
     assert len(resultat) == 0
```

### Comparing `myelectricaldatapy-1.9.6/tests/test_load_data.py` & `myelectricaldatapy-1.9.7/tests/test_load_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,132 +1,135 @@
 """Tests  Enedis api."""
 from __future__ import annotations
 
 from datetime import datetime as dt
-from unittest.mock import patch
+from unittest.mock import Mock, patch
 
 import pytest
 from freezegun import freeze_time
 
 import myelectricaldatapy
 from myelectricaldatapy import Enedis, EnedisByPDL
 
-from .consts import ACCESS
 from .consts import DATASET_30 as DS_30
-from .consts import ECOWATT, INVALID_ACCESS, INVALID_ECOWATT, TEMPO
+from .consts import INVALID_ACCESS, INVALID_ECOWATT
 
 PDL = "012345"
 TOKEN = "xxxxxxxxxxxxx"
 
 
 @freeze_time("2023-01-23")
 @pytest.mark.asyncio
-async def test_ecowatt() -> None:
+async def test_ecowatt(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test get ecowatt."""
     api = Enedis(token=TOKEN)
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=ECOWATT
-    ):
-        resultat = await api.async_get_ecowatt()
-        assert resultat["2023-01-22"]["value"] == 1
+    resultat = await api.async_get_ecowatt()
+    assert resultat["2023-01-22"]["value"] == 1
+
+    mypdl = EnedisByPDL(pdl=PDL, token=TOKEN)
+    mypdl.ecowatt_subscription(True)
+    await mypdl.async_update()
+    assert mypdl.ecowatt_day["message"] == "Pas d’alerte."
 
     with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=INVALID_ECOWATT
+        myelectricaldatapy.Enedis, "async_get_ecowatt", return_value=INVALID_ECOWATT
     ):
         resultat = await api.async_get_ecowatt()
         assert resultat.get("2023-01-22") is None
 
-    mypdl = EnedisByPDL(pdl=PDL, token=TOKEN)
-    dataset = DS_30
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ), patch.object(
-        myelectricaldatapy.Enedis, "async_get_ecowatt", return_value=ECOWATT
-    ):
-        mypdl.ecowatt_subscription(True)
-        await mypdl.async_update()
-
-    print(mypdl.ecowatt_day)
-    assert mypdl.ecowatt_day["message"] == "Pas d’alerte."
-
 
 @freeze_time("2023-3-3")
 @pytest.mark.asyncio
-async def test_tempoday() -> None:
+async def test_tempoday(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test get tempo day."""
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=TEMPO
-    ):
-        api = Enedis(token=TOKEN)
-        resultat = await api.async_get_tempo()
-        assert resultat["2023-3-1"] == "blue"
+    api = Enedis(token=TOKEN)
+    resultat = await api.async_get_tempo()
+    assert resultat["2023-3-1"] == "blue"
 
     mypdl = EnedisByPDL(pdl=PDL, token=TOKEN)
-    dataset = DS_30
-    modes = {"consumption": {"service": "consumption_load_curve"}}
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
-    ), patch.object(myelectricaldatapy.Enedis, "async_get_tempo", return_value=TEMPO):
-        mypdl.tempo_subscription(True)
-        await mypdl.async_update(modes=modes)
-        resultat = mypdl.stats["consumption"]
+    mypdl.set_collects("consumption_load_curve")
+    mypdl.tempo_subscription(True)
+    await mypdl.async_update()
+    resultat = mypdl.stats["consumption"]
     assert mypdl.tempo_day == "blue"
 
 
 @pytest.mark.asyncio
-async def test_valid_access() -> None:
+async def test_valid_access(
+    mock_enedis: Mock,  # pylint: disable=unused-argument
+) -> None:
     """Test access."""
-    with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=ACCESS
-    ):
-        api = Enedis(token=TOKEN)
-        resultat = await api.async_valid_access(PDL)
-        assert resultat["valid"] is True
+    api = Enedis(token=TOKEN)
+    resultat = await api.async_valid_access(PDL)
+    assert resultat["valid"] is True
 
-        resultat = await api.async_has_access(PDL)
-        assert resultat is True
+    resultat = await api.async_has_access(PDL)
+    assert resultat is True
 
     with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=INVALID_ACCESS
+        myelectricaldatapy.Enedis, "async_valid_access", return_value=INVALID_ACCESS
     ):
         api = Enedis(token=TOKEN)
         resultat = await api.async_valid_access(PDL)
         assert resultat["quota_reached"] is True
 
 
 @pytest.mark.asyncio
 async def test_fetch_data() -> None:
     """Test fetch data."""
-    dataset = DS_30
     with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
+        myelectricaldatapy.auth.EnedisAuth, "request", return_value=DS_30
     ):
         api = Enedis(token=TOKEN)
         resultat = await api.async_fetch_datas(
             service="comsumption_load_curve",
             pdl=PDL,
             start=dt.strptime("2022-12-30", "%Y-%m-%d"),
             end=dt.strptime("2022-12-31", "%Y-%m-%d"),
         )
         assert (
             resultat["meter_reading"]["interval_reading"]
-            == dataset["meter_reading"]["interval_reading"]  # noqa
+            == DS_30["meter_reading"]["interval_reading"]  # noqa
         )
 
 
 @pytest.mark.asyncio
 async def test_load() -> None:
     """Test load object."""
-    dataset = DS_30
     with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
+        myelectricaldatapy.auth.EnedisAuth, "request", return_value=DS_30
     ):
         api = Enedis(token=TOKEN)
         await api.async_get_max_power(PDL, dt.now(), dt.now())
         await api.async_get_contract(PDL)
         await api.async_get_address(PDL)
         await api.async_has_offpeak(PDL)
         await api.async_check_offpeak(PDL, dt.now())
         await api.async_get_identity(PDL)
         await api.async_get_daily_consumption(PDL, dt.now(), dt.now())
         await api.async_get_daily_production(PDL, dt.now(), dt.now())
         await api.async_get_details_production(PDL, dt.now(), dt.now())
+
+
+@pytest.mark.asyncio
+async def test_force_refresh(
+    mock_enedis: Mock,  # pylint: disable=unused-argument
+) -> None:
+    """Test refresh object."""
+
+    last_call = dt.now().strftime("%Y-%m-%dT%H:%M:%S.%f")
+    access = {
+        "valid": True,
+        "quota_reached": False,
+        "last_call": last_call,
+    }
+    with patch.object(
+        myelectricaldatapy.Enedis, "async_valid_access", return_value=access
+    ):
+        api = EnedisByPDL(pdl=PDL, token=TOKEN)
+        api.set_collects("consumption_load_curve")
+        await api.async_update()
+        save_refresh = api.last_refresh
+        await api.async_update()
+        assert api.last_refresh == save_refresh
+        await api.async_update(force_refresh=True)
+        assert api.last_refresh != save_refresh
```

