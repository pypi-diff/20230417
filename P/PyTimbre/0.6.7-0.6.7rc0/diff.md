# Comparing `tmp/PyTimbre-0.6.7.tar.gz` & `tmp/PyTimbre-0.6.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTimbre-0.6.7.tar", last modified: Sat Apr 15 00:04:57 2023, max compression
+gzip compressed data, was "PyTimbre-0.6.7rc0.tar", last modified: Mon Apr 17 13:07:56 2023, max compression
```

## Comparing `PyTimbre-0.6.7.tar` & `PyTimbre-0.6.7rc0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.865787 PyTimbre-0.6.7/
--rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.7/LICENSE.txt
--rw-rw-rw-   0        0        0    13118 2023-04-15 00:04:57.865787 PyTimbre-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     5289 2023-04-13 01:01:21.000000 PyTimbre-0.6.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 00:04:57.865787 PyTimbre-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-15 00:03:14.000000 PyTimbre-0.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.808221 PyTimbre-0.6.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.823559 PyTimbre-0.6.7/src/PyTimbre.egg-info/
--rw-rw-rw-   0        0        0    13118 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 00:04:57.000000 PyTimbre-0.6.7/src/PyTimbre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.836414 PyTimbre-0.6.7/src/pytimbre/
--rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.7/src/pytimbre/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.843499 PyTimbre-0.6.7/src/pytimbre/audio_files/
--rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/__init__.py
--rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/ansi_standard_formatted_files.py
--rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/calibrated_binary_files.py
--rw-rw-rw-   0        0        0    70669 2023-03-31 16:13:47.000000 PyTimbre-0.6.7/src/pytimbre/audio_files/wavefile.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:04:57.864799 PyTimbre-0.6.7/src/pytimbre/spectral/
--rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.7/src/pytimbre/spectral/__init__.py
--rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.7/src/pytimbre/spectral/acoustic_weights.py
--rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.7/src/pytimbre/spectral/fractional_octave_band.py
--rw-rw-rw-   0        0        0    16760 2023-04-14 02:05:08.000000 PyTimbre-0.6.7/src/pytimbre/spectral/fundamental_frequency.py
--rw-rw-rw-   0        0        0    57407 2023-04-14 23:59:24.000000 PyTimbre-0.6.7/src/pytimbre/spectral/spectra.py
--rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.7/src/pytimbre/spectral/spectrogram.py
--rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.7/src/pytimbre/spectral/swipe.py
--rw-rw-rw-   0        0        0    30655 2023-04-14 23:54:59.000000 PyTimbre-0.6.7/src/pytimbre/spectral/time_histories.py
--rw-rw-rw-   0        0        0    84616 2023-04-13 01:25:20.000000 PyTimbre-0.6.7/src/pytimbre/waveform.py
--rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.7/src/pytimbre/yin.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.583383 PyTimbre-0.6.7rc0/
+-rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.7rc0/LICENSE.txt
+-rw-rw-rw-   0        0        0    13121 2023-04-17 13:07:56.582714 PyTimbre-0.6.7rc0/PKG-INFO
+-rw-rw-rw-   0        0        0     5289 2023-04-13 01:01:21.000000 PyTimbre-0.6.7rc0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:07:56.583383 PyTimbre-0.6.7rc0/setup.cfg
+-rw-rw-rw-   0        0        0     1074 2023-04-17 13:06:01.000000 PyTimbre-0.6.7rc0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.493721 PyTimbre-0.6.7rc0/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.507006 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/
+-rw-rw-rw-   0        0        0    13121 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 13:07:56.000000 PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.521864 PyTimbre-0.6.7rc0/src/pytimbre/
+-rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.7rc0/src/pytimbre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.541779 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/
+-rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/__init__.py
+-rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/ansi_standard_formatted_files.py
+-rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/calibrated_binary_files.py
+-rw-rw-rw-   0        0        0    70669 2023-03-31 16:13:47.000000 PyTimbre-0.6.7rc0/src/pytimbre/audio_files/wavefile.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:07:56.581713 PyTimbre-0.6.7rc0/src/pytimbre/spectral/
+-rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/__init__.py
+-rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/acoustic_weights.py
+-rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/fractional_octave_band.py
+-rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/fundamental_frequency.py
+-rw-rw-rw-   0        0        0    58655 2023-04-16 12:48:15.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectra.py
+-rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectrogram.py
+-rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/swipe.py
+-rw-rw-rw-   0        0        0    30413 2023-04-16 01:00:36.000000 PyTimbre-0.6.7rc0/src/pytimbre/spectral/time_histories.py
+-rw-rw-rw-   0        0        0    84616 2023-04-13 01:25:20.000000 PyTimbre-0.6.7rc0/src/pytimbre/waveform.py
+-rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.7rc0/src/pytimbre/yin.py
```

### Comparing `PyTimbre-0.6.7/LICENSE.txt` & `PyTimbre-0.6.7rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/PKG-INFO` & `PyTimbre-0.6.7rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.7
+Version: 0.6.7rc0
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
```

### Comparing `PyTimbre-0.6.7/README.md` & `PyTimbre-0.6.7rc0/README.md`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/setup.py` & `PyTimbre-0.6.7rc0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         HISTORY = history_file.read()
 
         with open('LICENSE.txt') as license_file:
             LICENSE = license_file.read()
 
 setup(
     name='PyTimbre',
-    version='0.6.7',
+    version='0.6.7c0',
     description='Python conversion of Timbre Toolbox',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY + '\n\n' + LICENSE,
     license='MIT',
     packages=find_packages('src'),
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
```

### Comparing `PyTimbre-0.6.7/src/PyTimbre.egg-info/PKG-INFO` & `PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.7
+Version: 0.6.7rc0
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
```

### Comparing `PyTimbre-0.6.7/src/PyTimbre.egg-info/SOURCES.txt` & `PyTimbre-0.6.7rc0/src/PyTimbre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/audio_files/ansi_standard_formatted_files.py` & `PyTimbre-0.6.7rc0/src/pytimbre/audio_files/ansi_standard_formatted_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/audio_files/calibrated_binary_files.py` & `PyTimbre-0.6.7rc0/src/pytimbre/audio_files/calibrated_binary_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/audio_files/wavefile.py` & `PyTimbre-0.6.7rc0/src/pytimbre/audio_files/wavefile.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/spectral/acoustic_weights.py` & `PyTimbre-0.6.7rc0/src/pytimbre/spectral/acoustic_weights.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/spectral/fractional_octave_band.py` & `PyTimbre-0.6.7rc0/src/pytimbre/spectral/fractional_octave_band.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/spectral/fundamental_frequency.py` & `PyTimbre-0.6.7rc0/src/pytimbre/spectral/fundamental_frequency.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,19 @@
     """
     There are many ways to calculate the fundamental frequency of a waveform. However, many of the methods require
     information that can easily be combined with the functions and classes that exist within the PyTimbre modules.
     This class gathers the methods into one system and builds a collection of public and protected elements to access
     the fundamental frequency calculators.
     """
 
-    def __init__(self, f0: float = 10, f1: float = 10000, frequency_window_size: int = 2048, temporal_window: int =
-    256):
+    def __init__(self,
+                 f0: float = 10,
+                 f1: float = 10000,
+                 frequency_window_size: int = 2048,
+                 temporal_window: int = 256):
         """
         This build the class and initializes the element that are required for the calculation of the fundamental
         frequency.
 
         :param f0: float
             the starting frequency for the analysis
         :param f1: float
@@ -56,14 +59,17 @@
         #   Find local maxima
         peak_frequency_indices = find_peaks(spectrum.pressures_pascals,
                                             threshold=np.median(spectrum.pressures_pascals),
                                             distance=2)[0]
 
         #   If function doesn't have many candidate just return frequency at max value
         if len(peak_frequency_indices) < 5:
+            if len(peak_frequency_indices) == 0:
+                return np.nan
+
             #   find the index of the maximum peak
             peak_index = np.argmax(spectrum.pressures_decibels[peak_frequency_indices])
             return spectrum.frequencies[peak_frequency_indices[peak_index]]
         else:
             #   If one of the frequencies is the fundamental, it will possess a nearly integer relationship with the
             #   remaining peak values.
             #   Cut down to potential frequencies to the frequencies with the top 5 amplitudes
@@ -91,15 +97,15 @@
 
             return potential_fundamental_frequencies[np.argmin(sim)]
 
     def _swipe_spectral_estimation(self, x: Spectrum, strength_threshold: float = 0):
 
         # Compute pitch candidates
         pc = x.frequencies
-        loudness = x.pressures_pascals**2
+        loudness = x.pressures_pascals ** 2
 
         # Normalize loudness
         normalization_loudness = np.full_like(loudness, np.sqrt(np.sum(loudness * loudness, axis=0)))
         with np.errstate(divide='ignore', invalid='ignore'):
             loudness = loudness / normalization_loudness
 
         # Create pitch salience matrix
@@ -270,15 +276,14 @@
         k = k / np.linalg.norm(k[k > 0])
         if np.isnan(k).any():
             k = np.nan_to_num(k, nan=0)
 
         # Compute pitch strength
         return np.dot(k, normalized_loudness)
 
-
     @staticmethod
     def cumulative_mean_normalized_difference_function(frame, lag_max):
         """
         Computes Cumulative Mean Normalized Difference Function (CMNDF).
 
         Parameters
         ----------
```

### Comparing `PyTimbre-0.6.7/src/pytimbre/spectral/spectra.py` & `PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import warnings
 import datetime
 import numpy as np
 import scipy.fft
 import scipy.signal
 from .fractional_octave_band import FractionalOctaveBandTools as fob_tools
 from ..waveform import Waveform
@@ -472,14 +473,18 @@
         This is the energy within the signal that is explained by the harmonic partial frequencies and amplitudes. It
         is the square of all the amplitudes determined for the harmonic frequencies.
         """
 
         if self.partial_frequencies_indices is None:
             if self.fundamental_frequency is None:
                 self._calculate_fundamental_frequency()
+
+                if self._noise_energy is np.nan:
+                    self._harmonic_energy = np.nan
+                    return
             self._calculate_partial_pressures()
 
         if self._harmonic_energy is not None:
             return self._harmonic_energy
 
         self._harmonic_energy = 0
 
@@ -493,14 +498,19 @@
         """
         This is the energy of the signal not represented by the harmonic frequencies. It is simply the difference
         between the total energy and the energy explained by the harmonics.
         """
         if self.partial_frequencies_indices is None:
             if self.fundamental_frequency is None:
                 self._calculate_fundamental_frequency()
+
+                if self._noise_energy is np.nan:
+                    self._noisiness = np.nan
+                    return
+
             self._calculate_partial_pressures()
 
         if self._noise_energy is not None:
             return self._noise_energy
 
         self._noise_energy = self.spectral_energy - self.harmonic_energy
 
@@ -511,14 +521,18 @@
         """
         This is the ratio of the noise energy to the total energy. The higher the noisiness, the more noise-like the
         signal must be.
         """
         if self.partial_frequencies_indices is None:
             if self.fundamental_frequency is None:
                 self._calculate_fundamental_frequency()
+
+                if self.fundamental_frequency is np.nan:
+                    self._noisiness = np.nan
+                    return
             self._calculate_partial_pressures()
 
         if self._noisiness is not None:
             return self._noisiness
 
         self._noisiness = self.noise_energy / self.spectral_energy
 
@@ -532,14 +546,18 @@
         visual color attributes. It is three different energy ratios based on the description of the fundamental
         frequency.
         """
         if self._tri_stimulus is None:
             if self.partial_frequencies_indices is None:
                 if self.fundamental_frequency is None:
                     self._calculate_fundamental_frequency()
+
+                    if self.fundamental_frequency is np.nan:
+                        self._tri_stimulus = [np.nan, np.nan, np.nan]
+                        return
                 self._calculate_partial_pressures()
 
             harmonic_pressure_sum = np.sum(self.pressures_pascals[self.partial_frequencies_indices])
             t01 = self.pressures_pascals[self.partial_frequencies_indices[0]] / harmonic_pressure_sum
 
             t02 = np.sum(self.pressures_pascals[self.partial_frequencies_indices[1:4]]) / harmonic_pressure_sum
             t03 = np.sum(self.pressures_pascals[self.partial_frequencies_indices[4:]]) / harmonic_pressure_sum
@@ -554,14 +572,19 @@
         This measures the deviation of the amplitudes of the partials from the harmonics from the global or smoothed
         spectral envelope.
         """
         if self._harmonic_spectral_deviation is None:
             if self.partial_frequencies_indices is None:
                 if self.fundamental_frequency is None:
                     self._calculate_fundamental_frequency()
+
+                if self.fundamental_frequency is np.nan:
+                    self._harmonic_spectral_deviation = np.nan
+                    return
+
                 self._calculate_partial_pressures()
 
             self._harmonic_spectral_deviation = 0
             for h in range(1, len(self.partial_frequencies_indices) - 1):
                 self._harmonic_spectral_deviation += self.pressures_pascals[self.partial_frequencies_indices[h]] - (
                         self.pressures_pascals[self.partial_frequencies_indices[h - 1]] +
                         self.pressures_pascals[self.partial_frequencies_indices[h]] +
@@ -578,25 +601,30 @@
         In musical instruments, certain signals contain mostly even (trumpet) or odd (clarinet) harmonics. This ratio
         determines where the system is mostly odd or even.
         """
         if self._odd_even_ratio is None:
             if self.partial_frequencies_indices is None:
                 if self.fundamental_frequency is None:
                     self._calculate_fundamental_frequency()
+
+                if self.fundamental_frequency is np.nan:
+                    self._odd_even_ratio = np.nan
+                    return
+
                 self._calculate_partial_pressures()
 
             odd_energy = 0
             even_energy = 0
             for i in range(1, len(self.partial_frequencies_indices)):
                 if (i + 1) % 2 == 0:
                     even_energy += self.pressures_pascals[self.partial_frequencies_indices[i]] ** 2
                 else:
                     odd_energy += self.pressures_pascals[self.partial_frequencies_indices[i]] ** 2
 
-            self._odd_even_ratio = odd_energy / even_energy
+            self._odd_even_ratio = odd_energy / (even_energy + sys.float_info.epsilon)
 
         return self._odd_even_ratio
 
     @property
     def inharmonicity(self):
         """
         This is a measure of the deviation of the partial frequencies from the purely harmonic frequency.
@@ -605,21 +633,24 @@
             if self.partial_frequencies_indices is None:
                 if self.fundamental_frequency is None:
                     self._calculate_fundamental_frequency()
                 self._calculate_partial_pressures()
 
             f0 = self.fundamental_frequency
 
-            frequency_departure = 0
-            for i in range(1, len(self.partial_frequencies_indices)):
-                frequency_departure += (self.frequencies[self.partial_frequencies_indices[i]] - (i + 1) * f0) * \
-                                       self.pressures_pascals[self.partial_frequencies_indices[i]]
+            if f0 is np.nan:
+                self._inharmonicity = np.nan
+            else:
+                frequency_departure = 0
+                for i in range(1, len(self.partial_frequencies_indices)):
+                    frequency_departure += (self.frequencies[self.partial_frequencies_indices[i]] - (i + 1) * f0) * \
+                                           self.pressures_pascals[self.partial_frequencies_indices[i]]
 
-            self._inharmonicity = (2 / f0) * frequency_departure / np.sum(self.pressures_pascals[
-                                                                              self.partial_frequencies_indices] ** 2)
+                self._inharmonicity = (2 / f0) * frequency_departure / np.sum(self.pressures_pascals[
+                                                                                  self.partial_frequencies_indices] ** 2)
 
         return self._inharmonicity
 
     @property
     def fundamental_frequency(self):
         if self._fundamental_frequency is None:
             self._calculate_fundamental_frequency()
@@ -753,19 +784,26 @@
     def _calculate_fundamental_frequency(self):
         from .fundamental_frequency import FundamentalFrequencyCalculator
 
         calculator = FundamentalFrequencyCalculator(frequency_window_size=self._fft_size)
 
         f0 = list()
         f0.append(calculator.fundamental_swipe(self))
-        f0.append(calculator.fundamental_by_peaks(self))
-        if self._waveform is not None:
-            f0.append(calculator.fundamental_by_time(self.waveform))
+        # f0.append(calculator.fundamental_by_peaks(self))
+        # if self._waveform is not None:
+        #     f0.append(calculator.fundamental_by_time(self.waveform))
+
+        #   Convert the list to an array and remove any Nan values
+        f0 = np.asarray(f0)
+        f0 = f0[np.logical_not(np.isnan(f0))]
 
-        self._fundamental_frequency = np.median(np.asarray(f0))
+        if len(f0) < 1:
+            self._fundamental_frequency = np.nan
+        else:
+            self._fundamental_frequency = np.median(f0)
 
     def _calculate_partial_pressures(self):
         """
         We need to locate the partial pressure frequencies and amplitudes by calculating the index of each integer
         multiple of the fundamental frequency.
         """
```

### Comparing `PyTimbre-0.6.7/src/pytimbre/spectral/spectrogram.py` & `PyTimbre-0.6.7rc0/src/pytimbre/spectral/spectrogram.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/spectral/swipe.py` & `PyTimbre-0.6.7rc0/src/pytimbre/spectral/swipe.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/spectral/time_histories.py` & `PyTimbre-0.6.7rc0/src/pytimbre/spectral/time_histories.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,18 +162,19 @@
         """
 
         #   Create the DataFrame that will hold the data from the waveform and the spectrum objects
         names = ['time', 'lf', 'la', 'pnl']
         for f in self.frequencies:
             names.append('F{:06.0f}Hz'.format(f))
 
-        for key in self.spectra[0].get_feature_names(include_sq_metrics=include_sq_metrics,
-                                                     include_harmonic_features=include_harmonic_features,
-                                                     include_spectral_features=include_spectral_features,
-                                                     include_temporal_features=include_temporal_features):
+        timbre_feature_names = self.spectra[0].get_feature_names(include_sq_metrics=include_sq_metrics,
+                                                                 include_harmonic_features=include_harmonic_features,
+                                                                 include_spectral_features=include_spectral_features,
+                                                                 include_temporal_features=include_temporal_features)
+        for key in timbre_feature_names:
             names.append(key)
 
         df = pd.DataFrame(columns=names, index=np.arange(len(self.times)))
 
         for i in range(df.shape[0]):
             s = self.spectra[i]
             if isinstance(s, Spectrum):
@@ -181,22 +182,20 @@
                                   s.perceived_noise_level]
 
                 for band_index in range(len(self.frequencies)):
                     df.iloc[i, 4 + band_index] = s.pressures_decibels[band_index]
 
                 n = 4 + len(self.frequencies)
 
-                for key in s.get_feature_names(include_sq_metrics=include_sq_metrics,
-                                               include_harmonic_features=include_harmonic_features,
-                                               include_spectral_features=include_spectral_features,
-                                               include_temporal_features=include_temporal_features):
-                    df.iloc[i, n] = s.get_average_features(include_sq_metrics=include_sq_metrics,
-                                                           include_harmonic_features=include_harmonic_features,
-                                                           include_spectral_features=include_spectral_features,
-                                                           include_temporal_features=include_temporal_features)[key]
+                features = s.get_average_features(include_sq_metrics=include_sq_metrics,
+                                                  include_harmonic_features=include_harmonic_features,
+                                                  include_spectral_features=include_spectral_features,
+                                                  include_temporal_features=include_temporal_features)
+                for key in timbre_feature_names:
+                    df.iloc[i, n] = features[key]
 
                     n += 1
 
         return df
 
     def save(self, filename: str):
         from ..audio_files.ansi_standard_formatted_files import StandardBinaryFile
```

### Comparing `PyTimbre-0.6.7/src/pytimbre/waveform.py` & `PyTimbre-0.6.7rc0/src/pytimbre/waveform.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.7/src/pytimbre/yin.py` & `PyTimbre-0.6.7rc0/src/pytimbre/yin.py`

 * *Files identical despite different names*

