# Comparing `tmp/flarespy-0.6.0.tar.gz` & `tmp/flarespy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.6.0.tar", max compression
+gzip compressed data, was "flarespy-0.6.1.tar", max compression
```

## Comparing `flarespy-0.6.0.tar` & `flarespy-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.6.0/LICENSE
--rw-r--r--   0        0        0      428 2023-04-16 16:38:22.310415 flarespy-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.6.0/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.6.0/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.6.0/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    25397 2023-04-16 16:37:37.272788 flarespy-0.6.0/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.6.0/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-16 16:38:11.870628 flarespy-0.6.0/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.6.1/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-17 04:22:15.023599 flarespy-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.6.1/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.6.1/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.6.1/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    25601 2023-04-17 04:20:16.226837 flarespy-0.6.1/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.6.1/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-17 04:22:15.020867 flarespy-0.6.1/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.6.1/PKG-INFO
```

### Comparing `flarespy-0.6.0/LICENSE` & `flarespy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.0/src/flarespy/Flare_model.py` & `flarespy-0.6.1/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.0/src/flarespy/data/model.dat` & `flarespy-0.6.1/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.0/src/flarespy/flarefinder.py` & `flarespy-0.6.1/src/flarespy/flarefinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,28 +231,32 @@
             self.meta["otype"] = query_result["OTYPE"][0]
             if "CV*" in query_result["OTYPES"][0].split("|"):
                 self.meta["otype"] = "CataclyV*"
 
     def _calculate_stellar_luminosity(self):
         # Query parallax from Gaia DR3
         coord = SkyCoord(self.ra, self.dec, unit="deg", frame="icrs", equinox="J2000")
-        radius = u.Quantity(30, u.arcsec)
+        radius = u.Quantity(5, u.arcmin)
         try:
             self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS, dtype=object)
             gaia_dr3_data = Gaia.cone_search_async(coord, radius).get_results()
+            gaia_dr3_data = gaia_dr3_data[gaia_dr3_data["dist"] < 5 / 3600]
 
             self.stellar_parameters.gaia3_source_id = gaia_dr3_data["source_id"].data.data[0]
             self.stellar_parameters.parallax = np.round(gaia_dr3_data["parallax"].data.data[0], 4)
             self.stellar_parameters.phot_g_mean_mag = np.round(gaia_dr3_data["phot_g_mean_mag"].data.data[0], 4)
             self.stellar_parameters.phot_bp_mean_mag = np.round(gaia_dr3_data["phot_bp_mean_mag"].data.data[0], 4)
             self.stellar_parameters.phot_rp_mean_mag = np.round(gaia_dr3_data["phot_rp_mean_mag"].data.data[0], 4)
             self.stellar_parameters.obs_duration = np.round(
                 self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.standardized_flux.value))[0].size, 4
             )
 
+            if self.stellar_parameters.parallax < 0:
+                self.stellar_parameters.parallax = np.nan
+
         except IndexError:
             pass
 
         # Query TESS mag from TIC
         tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
         tic_data.add_index("ID")
         try:
@@ -262,15 +266,15 @@
             t_mag = np.nan
 
         if self.stellar_parameters is not None:
             self.stellar_parameters.tess_mag = t_mag
 
             # Calculate stellar luminosity
             plx = self.stellar_parameters["parallax"]
-            if hasattr(plx, "mask") or np.isnan(t_mag):
+            if hasattr(plx, "mask") or np.isnan(t_mag) or np.isnan(plx):
                 self.meta["lum"] = np.nan
             else:
                 plx /= 1000
                 dist = 1 / plx * u.pc
                 flux = 10 ** (-t_mag / 2.5) * TESS_FLUX0
                 lum = 4 * np.pi * dist.to(u.cm) ** 2 * flux
                 self.meta["lum"] = lum.value
```

### Comparing `flarespy-0.6.0/src/flarespy/utils.py` & `flarespy-0.6.1/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.0/PKG-INFO` & `flarespy-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

