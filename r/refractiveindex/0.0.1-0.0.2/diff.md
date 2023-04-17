# Comparing `tmp/refractiveindex-0.0.1.tar.gz` & `tmp/refractiveindex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractiveindex-0.0.1.tar", max compression
+gzip compressed data, was "refractiveindex-0.0.2.tar", max compression
```

## Comparing `refractiveindex-0.0.1.tar` & `refractiveindex-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-04-11 05:30:37.229988 refractiveindex-0.0.1/LICENSE
--rw-r--r--   0        0        0     1194 2023-04-11 06:06:56.640570 refractiveindex-0.0.1/README.md
--rw-r--r--   0        0        0      309 2023-04-11 05:33:46.410392 refractiveindex-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       52 2023-04-11 05:26:30.997463 refractiveindex-0.0.1/refractiveindex/__init__.py
--rw-r--r--   0        0        0    16043 2023-04-11 05:25:42.073358 refractiveindex-0.0.1/refractiveindex/refractiveindex.py
--rw-r--r--   0        0        0     1862 2023-04-11 07:09:44.726620 refractiveindex-0.0.1/setup.py
--rw-r--r--   0        0        0     1562 2023-04-11 07:09:44.726846 refractiveindex-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-11 05:30:37.229988 refractiveindex-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1483 2023-04-17 01:36:57.102410 refractiveindex-0.0.2/README.md
+-rw-r--r--   0        0        0      309 2023-04-17 04:37:56.299176 refractiveindex-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-04-11 05:26:30.997463 refractiveindex-0.0.2/refractiveindex/__init__.py
+-rw-r--r--   0        0        0    16043 2023-04-17 04:36:33.571001 refractiveindex-0.0.2/refractiveindex/refractiveindex.py
+-rw-r--r--   0        0        0     2157 2023-04-17 04:38:17.977999 refractiveindex-0.0.2/setup.py
+-rw-r--r--   0        0        0     1851 2023-04-17 04:38:17.978192 refractiveindex-0.0.2/PKG-INFO
```

### Comparing `refractiveindex-0.0.1/LICENSE` & `refractiveindex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `refractiveindex-0.0.1/README.md` & `refractiveindex-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Easy Python interface to RefractiveIndex database
 
-The original database is here
+The original database<br>
 https://github.com/polyanskiy/refractiveindex.info-database
 
 Database files parsing was made with a modified version of `refractiveIndex.py` from [PyTMM project](https://github.com/kitchenknif/PyTMM) by [Pavel Dmitriev](https://github.com/kitchenknif).
 
 ## Installation
 
 ```
@@ -27,19 +27,25 @@
 SiO.get_refractive_index(wavelength_nm)
 # (1.96553846)
 
 SiO.get_extinction_coefficient(wavelength_nm)
 # (0.001)
 ```
 
-Note: here the time dependence is assumed to be $\mathrm{e}^{-\mathrm{i} \omega t}$, so $\operatorname{Im}\varepsilon > 0$ is responsible for the losses.
+Notes: 
+- here the time dependence is assumed to be $\mathrm{e}^{-\mathrm{i} \omega t}$, so $\operatorname{Im}\varepsilon > 0$ is responsible for the losses.
+- if there is a space in the name, one should write underscore instead of it, i.e. not `page='Rodriguez-de Marcos'` but `page='Rodriguez-de_Marcos'`.
 
 
 ## How to get material page names
 
 You can find the proper “page” name by hovering your cursor on the link in the Data section
 
 ![How to get page name](./fig/link.png)
 
-Or you can look up folders in this repository
-
+Or you can look up folders in this repository<br>
 https://github.com/polyanskiy/refractiveindex.info-database
+
+## Simular projects for Julia
+
+Julia interface to refractiveindex.info database<br>
+https://github.com/stillyslalom/RefractiveIndex.jl
```

### Comparing `refractiveindex-0.0.1/refractiveindex/refractiveindex.py` & `refractiveindex-0.0.2/refractiveindex/refractiveindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,20 +395,20 @@
     
 
 class RefractiveIndexMaterial:
     def __init__(self, shelf, book, page):
         BD = RefractiveIndex()
         self.material = BD.getMaterial(shelf=shelf, book=book, page=page)
         
-    def get_refractive_index(self, wavelenght_nm):
-        return self.material.getRefractiveIndex(np.copy(wavelenght_nm))
+    def get_refractive_index(self, wavelength_nm):
+        return self.material.getRefractiveIndex(np.copy(wavelength_nm))
     
-    def get_extinction_coefficient(self, wavelenght_nm):
-        return self.material.getExtinctionCoefficient(np.copy(wavelenght_nm))
+    def get_extinction_coefficient(self, wavelength_nm):
+        return self.material.getExtinctionCoefficient(np.copy(wavelength_nm))
     
-    def get_epsilon(self, wavelenght_nm, exp_type='exp_minus_i_omega_t'):
-        n = self.get_refractive_index(wavelenght_nm)
-        k = self.get_extinction_coefficient(wavelenght_nm)
+    def get_epsilon(self, wavelength_nm, exp_type='exp_minus_i_omega_t'):
+        n = self.get_refractive_index(wavelength_nm)
+        k = self.get_extinction_coefficient(wavelength_nm)
         if exp_type=='exp_minus_i_omega_t':
             return (n + 1j*k)**2
         else:
             return (n - 1j*k)**2
```

### Comparing `refractiveindex-0.0.1/setup.py` & `refractiveindex-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pyyaml>=5.0,<6.0', 'scipy>=1.9.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'refractiveindex',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
-    'long_description': "# Easy Python interface to RefractiveIndex database\n\nThe original database is here\nhttps://github.com/polyanskiy/refractiveindex.info-database\n\nDatabase files parsing was made with a modified version of `refractiveIndex.py` from [PyTMM project](https://github.com/kitchenknif/PyTMM) by [Pavel Dmitriev](https://github.com/kitchenknif).\n\n## Installation\n\n```\npip install refractiveindex\n```\n\n## Usage\n\n\n```python\nfrom refractiveindex import RefractiveIndexMaterial\n\nSiO = RefractiveIndexMaterial(shelf='main', book='SiO', page='Hass')\n\nwavelength_nm = 600  # [nm]\n\nSiO.get_epsilon(wavelength_nm)\n# (3.8633404437869827+0.003931076923076923j)\n\nSiO.get_refractive_index(wavelength_nm)\n# (1.96553846)\n\nSiO.get_extinction_coefficient(wavelength_nm)\n# (0.001)\n```\n\nNote: here the time dependence is assumed to be $\\mathrm{e}^{-\\mathrm{i} \\omega t}$, so $\\operatorname{Im}\\varepsilon > 0$ is responsible for the losses.\n\n\n## How to get material page names\n\nYou can find the proper “page” name by hovering your cursor on the link in the Data section\n\n![How to get page name](./fig/link.png)\n\nOr you can look up folders in this repository\n\nhttps://github.com/polyanskiy/refractiveindex.info-database\n",
+    'long_description': "# Easy Python interface to RefractiveIndex database\n\nThe original database<br>\nhttps://github.com/polyanskiy/refractiveindex.info-database\n\nDatabase files parsing was made with a modified version of `refractiveIndex.py` from [PyTMM project](https://github.com/kitchenknif/PyTMM) by [Pavel Dmitriev](https://github.com/kitchenknif).\n\n## Installation\n\n```\npip install refractiveindex\n```\n\n## Usage\n\n\n```python\nfrom refractiveindex import RefractiveIndexMaterial\n\nSiO = RefractiveIndexMaterial(shelf='main', book='SiO', page='Hass')\n\nwavelength_nm = 600  # [nm]\n\nSiO.get_epsilon(wavelength_nm)\n# (3.8633404437869827+0.003931076923076923j)\n\nSiO.get_refractive_index(wavelength_nm)\n# (1.96553846)\n\nSiO.get_extinction_coefficient(wavelength_nm)\n# (0.001)\n```\n\nNotes: \n- here the time dependence is assumed to be $\\mathrm{e}^{-\\mathrm{i} \\omega t}$, so $\\operatorname{Im}\\varepsilon > 0$ is responsible for the losses.\n- if there is a space in the name, one should write underscore instead of it, i.e. not `page='Rodriguez-de Marcos'` but `page='Rodriguez-de_Marcos'`.\n\n\n## How to get material page names\n\nYou can find the proper “page” name by hovering your cursor on the link in the Data section\n\n![How to get page name](./fig/link.png)\n\nOr you can look up folders in this repository<br>\nhttps://github.com/polyanskiy/refractiveindex.info-database\n\n## Simular projects for Julia\n\nJulia interface to refractiveindex.info database<br>\nhttps://github.com/stillyslalom/RefractiveIndex.jl\n",
     'author': 'Ivan Toftul',
     'author_email': 'toftul.ivan@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `refractiveindex-0.0.1/PKG-INFO` & `refractiveindex-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: refractiveindex
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Ivan Toftul
 Author-email: toftul.ivan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: pyyaml (>=5.0,<6.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Easy Python interface to RefractiveIndex database
 
-The original database is here
+The original database<br>
 https://github.com/polyanskiy/refractiveindex.info-database
 
 Database files parsing was made with a modified version of `refractiveIndex.py` from [PyTMM project](https://github.com/kitchenknif/PyTMM) by [Pavel Dmitriev](https://github.com/kitchenknif).
 
 ## Installation
 
 ```
@@ -40,20 +40,26 @@
 SiO.get_refractive_index(wavelength_nm)
 # (1.96553846)
 
 SiO.get_extinction_coefficient(wavelength_nm)
 # (0.001)
 ```
 
-Note: here the time dependence is assumed to be $\mathrm{e}^{-\mathrm{i} \omega t}$, so $\operatorname{Im}\varepsilon > 0$ is responsible for the losses.
+Notes: 
+- here the time dependence is assumed to be $\mathrm{e}^{-\mathrm{i} \omega t}$, so $\operatorname{Im}\varepsilon > 0$ is responsible for the losses.
+- if there is a space in the name, one should write underscore instead of it, i.e. not `page='Rodriguez-de Marcos'` but `page='Rodriguez-de_Marcos'`.
 
 
 ## How to get material page names
 
 You can find the proper “page” name by hovering your cursor on the link in the Data section
 
 ![How to get page name](./fig/link.png)
 
-Or you can look up folders in this repository
-
+Or you can look up folders in this repository<br>
 https://github.com/polyanskiy/refractiveindex.info-database
 
+## Simular projects for Julia
+
+Julia interface to refractiveindex.info database<br>
+https://github.com/stillyslalom/RefractiveIndex.jl
+
```

