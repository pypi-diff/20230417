# Comparing `tmp/flarespy-0.6.2.tar.gz` & `tmp/flarespy-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.6.2.tar", max compression
+gzip compressed data, was "flarespy-0.6.3.tar", max compression
```

## Comparing `flarespy-0.6.2.tar` & `flarespy-0.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.6.2/LICENSE
--rw-r--r--   0        0        0      428 2023-04-17 05:48:36.621878 flarespy-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.6.2/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.6.2/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.6.2/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    26093 2023-04-17 05:47:33.319189 flarespy-0.6.2/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.6.2/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-17 05:48:36.617327 flarespy-0.6.2/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.6.3/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-17 07:44:11.814773 flarespy-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.6.3/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.6.3/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.6.3/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    26279 2023-04-17 07:55:38.454499 flarespy-0.6.3/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4572 2023-04-16 09:27:59.194030 flarespy-0.6.3/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-17 07:44:11.813057 flarespy-0.6.3/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.6.3/PKG-INFO
```

### Comparing `flarespy-0.6.2/LICENSE` & `flarespy-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.2/src/flarespy/Flare_model.py` & `flarespy-0.6.3/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.2/src/flarespy/data/model.dat` & `flarespy-0.6.3/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.2/src/flarespy/flarefinder.py` & `flarespy-0.6.3/src/flarespy/flarefinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,66 +232,28 @@
             self.meta["otype"] = "/"
         else:
             self.meta["otype"] = query_result["OTYPE"][0]
             if "CV*" in query_result["OTYPES"][0].split("|"):
                 self.meta["otype"] = "CataclyV*"
 
     def _calculate_stellar_luminosity(self):
-        # Query parallax from Gaia DR3
-        coord = SkyCoord(self.ra, self.dec, unit="deg", frame="icrs", equinox="J2000")
-        radius = u.Quantity(5, u.arcmin)
-
-        j = Gaia.cone_search_async(coord, radius)
-        r = j.get_results()
-
-        qr = QTable([r["ra"].filled(), r["dec"].filled(), r["pmra"].filled(0), r["pmdec"].filled(0)])
-        coords_gaia = SkyCoord(
-            qr["ra"], qr["dec"], pm_ra_cosdec=qr["pmra"], pm_dec=qr["pmdec"], frame="icrs", obstime=Time("J2016")
-        )
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", category=ErfaWarning)
-            coords_gaia_j2000 = coords_gaia.apply_space_motion(new_obstime=Time("J2000"))
-        dist = coord.separation(coords_gaia_j2000).arcsec
-
-        if (dist < 5).any():
-            target_index = np.argmin(dist)
-            self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS, dtype=object)
-            self.stellar_parameters.gaia3_source_id = r["source_id"].data.data[target_index]
-            self.stellar_parameters.parallax = np.round(r["parallax"].data.data[target_index], 4)
-            self.stellar_parameters.phot_g_mean_mag = np.round(r["phot_g_mean_mag"].data.data[target_index], 4)
-            self.stellar_parameters.phot_bp_mean_mag = np.round(r["phot_bp_mean_mag"].data.data[target_index], 4)
-            self.stellar_parameters.phot_rp_mean_mag = np.round(r["phot_rp_mean_mag"].data.data[target_index], 4)
-            self.stellar_parameters.obs_duration = np.round(
-                self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.standardized_flux.value))[0].size, 4
-            )
-
-            if self.stellar_parameters.parallax < 0:
-                self.stellar_parameters.parallax = np.nan
-
-        # Query TESS mag from TIC
-        tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
-        tic_data.add_index("ID")
-        try:
-            target_row = tic_data.loc[str(self.ticid)]
-            t_mag = target_row["Tmag"]
-        except KeyError:
-            t_mag = np.nan
-
         self.meta["lum"] = np.nan
-        if self.stellar_parameters is not None:
-            self.stellar_parameters.tess_mag = t_mag
+        if self.stellar_parameters is None:
+            self._query_stellar_parameters()
 
-            # Calculate stellar luminosity
-            plx = self.stellar_parameters["parallax"]
-            if ~np.isnan(t_mag) and ~np.isnan(plx):
-                plx /= 1000
-                dist = 1 / plx * u.pc
-                flux = 10 ** (-t_mag / 2.5) * TESS_FLUX0
-                lum = 4 * np.pi * dist.to(u.cm) ** 2 * flux
-                self.meta["lum"] = lum.value
+        # Calculate stellar luminosity
+        t_mag = self.stellar_parameters["tess_mag"]
+        plx = self.stellar_parameters["parallax"]
+
+        if ~np.isnan(t_mag) and ~np.isnan(plx):
+            plx /= 1000
+            dist = 1 / plx * u.pc
+            flux = 10 ** (-t_mag / 2.5) * TESS_FLUX0
+            lum = 4 * np.pi * dist.to(u.cm) ** 2 * flux
+            self.meta["lum"] = lum.value
 
     def _is_sso(self, i_peak: int, radius: float = 8):
         """Check if a candidate is caused by a Solar System Object (SSO) encounter."""
 
         mask = np.zeros_like(self.time, dtype=bool)
         mask[i_peak] = True
 
@@ -341,14 +303,58 @@
         t_stop = self.time.value[i_stop]
 
         before = np.nonzero((time > t_start - window) & (time < t_start))[0]
         after = np.nonzero((time > t_stop) & (time < t_stop + window))[0]
 
         return False if (before.size and after.size) else True
 
+    def query_stellar_parameters(self):
+        self.stellar_parameters = pd.Series(
+            data=np.full_like(STELLAR_PARAMETER_COLUMNS, np.nan), index=STELLAR_PARAMETER_COLUMNS, dtype=object
+        )
+
+        # Query parallax from Gaia DR3
+        coord = SkyCoord(self.ra, self.dec, unit="deg", frame="icrs", equinox="J2000")
+        radius = u.Quantity(5, u.arcmin)
+
+        j = Gaia.cone_search_async(coord, radius)
+        r = j.get_results()
+
+        qr = QTable([r["ra"].filled(), r["dec"].filled(), r["pmra"].filled(0), r["pmdec"].filled(0)])
+        coords_gaia = SkyCoord(
+            qr["ra"], qr["dec"], pm_ra_cosdec=qr["pmra"], pm_dec=qr["pmdec"], frame="icrs", obstime=Time("J2016")
+        )
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=ErfaWarning)
+            coords_gaia_j2000 = coords_gaia.apply_space_motion(new_obstime=Time("J2000"))
+        dist = coord.separation(coords_gaia_j2000).arcsec
+
+        if (dist < 8).any():
+            target_index = np.argmin(dist)
+            self.stellar_parameters.gaia3_source_id = r["source_id"].data.data[target_index]
+            self.stellar_parameters.parallax = np.round(r["parallax"].data.data[target_index], 4)
+            self.stellar_parameters.phot_g_mean_mag = np.round(r["phot_g_mean_mag"].data.data[target_index], 4)
+            self.stellar_parameters.phot_bp_mean_mag = np.round(r["phot_bp_mean_mag"].data.data[target_index], 4)
+            self.stellar_parameters.phot_rp_mean_mag = np.round(r["phot_rp_mean_mag"].data.data[target_index], 4)
+            self.stellar_parameters.obs_duration = np.round(
+                self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
+            )
+
+            if self.stellar_parameters.parallax < 0:
+                self.stellar_parameters.parallax = np.nan
+
+        # Query TESS mag from TIC
+        tic_data = Catalogs.query_object(self.label, radius=0.02, catalog="TIC")
+        tic_data.add_index("ID")
+        try:
+            target_row = tic_data.loc[str(self.ticid)]
+            self.stellar_parameters.tess_mag = target_row["Tmag"]
+        except KeyError:
+            pass
+
     def detrend(self, window_length=0.3):
         """Detrend the lightcurve."""
 
         self._query_object_type_from_simbad()
 
         masked_lc = self._mask_eclipse()
         model_flux = self._generate_model()
@@ -409,15 +415,15 @@
         if self.candidates is not None:
             sso = np.zeros(len(self.candidates), dtype=bool)
             for row in self.candidates.itertuples():
                 sso[row.Index] = self._is_sso(row.i_peak)
 
             self.candidates.sso = sso
 
-    def calculate_parameters(self):
+    def calculate_candidate_parameters(self):
         """Calculate the parameters of the candidates."""
 
         if self.candidates is not None:
             proba_array = np.zeros(len(self.candidates))
             snr_array = np.zeros(len(self.candidates))
             for row in self.candidates.itertuples():
                 lc_candidate = self[row.i_start : row.i_stop + 1].remove_nans("standardized_flux")
@@ -456,18 +462,19 @@
                 if np.isnan(self.lum):
                     self.candidates.energy = np.full(len(self.candidates), np.nan)
                 else:
                     energy = ed * self.lum
                     self.candidates.energy = [np.format_float_scientific(x, precision=2) for x in energy]
 
     def find_flares(self):
+        self.query_stellar_parameters()
         self.detrend()
         self.find_candidates()
         self.detect_sso()
-        self.calculate_parameters()
+        self.calculate_candidate_parameters()
 
     def plot_candidates(self, figure_folder, threshold=0.5):
         """Plot the candidates."""
 
         if self.candidates is not None:
             t_extend = 30.2 * self.meta["TIMEDEL"]
             finite_mask = np.isfinite(self.standardized_flux)
```

### Comparing `flarespy-0.6.2/src/flarespy/utils.py` & `flarespy-0.6.3/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.6.2/PKG-INFO` & `flarespy-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.6.2
+Version: 0.6.3
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

