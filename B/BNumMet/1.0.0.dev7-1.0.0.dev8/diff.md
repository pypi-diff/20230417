# Comparing `tmp/BNumMet-1.0.0.dev7.tar.gz` & `tmp/BNumMet-1.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BNumMet-1.0.0.dev7.tar", last modified: Mon Apr 10 12:35:26 2023, max compression
+gzip compressed data, was "BNumMet-1.0.0.dev8.tar", last modified: Mon Apr 17 15:37:09 2023, max compression
```

## Comparing `BNumMet-1.0.0.dev7.tar` & `BNumMet-1.0.0.dev8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.679077 BNumMet-1.0.0.dev7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.679077 BNumMet-1.0.0.dev7/src/BNumMet/
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/LinearSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/NonLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/InterpolationVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LUVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LeastSquaresVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/NonLinearVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/RandomVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/src/BNumMet/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 12:35:26.000000 BNumMet-1.0.0.dev7/src/BNumMet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:35:26.683077 BNumMet-1.0.0.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_General.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_Interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_LeastSquares.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_LinealSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_NonLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_Random.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-10 12:35:14.000000 BNumMet-1.0.0.dev7/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-04-17 15:36:47.000000 BNumMet-1.0.0.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 15:36:47.000000 BNumMet-1.0.0.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-04-17 15:36:47.000000 BNumMet-1.0.0.dev8/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.628353 BNumMet-1.0.0.dev8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.632353 BNumMet-1.0.0.dev8/src/BNumMet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/LinearSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/NonLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.632353 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/InterpolationVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LUVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LeastSquaresVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/NonLinearVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/RandomVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.632353 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_General.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_Interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_LeastSquares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_LinealSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_NonLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_Random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_module.py
```

### Comparing `BNumMet-1.0.0.dev7/LICENSE` & `BNumMet-1.0.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/PKG-INFO` & `BNumMet-1.0.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BNumMet
-Version: 1.0.0.dev7
+Version: 1.0.0.dev8
 Summary: Basic Numerical Methods for Python 3
 Home-page: https://github.com/fbpazos/Trabajo-Fin-Master/tree/main/Python_BNumMet
 Author: Fernando Bellido Pazos
 Author-email: fbellidopazos@gmail.com
 License: AGPL-3.0
 Platform: unix
 Platform: linux
```

### Comparing `BNumMet-1.0.0.dev7/Readme.md` & `BNumMet-1.0.0.dev8/Readme.md`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/setup.cfg` & `BNumMet-1.0.0.dev8/setup.cfg`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/Interpolation.py` & `BNumMet-1.0.0.dev8/src/BNumMet/Interpolation.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/LinearSystems.py` & `BNumMet-1.0.0.dev8/src/BNumMet/LinearSystems.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/NonLinear.py` & `BNumMet-1.0.0.dev8/src/BNumMet/NonLinear.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/Random.py` & `BNumMet-1.0.0.dev8/src/BNumMet/Random.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/InterpolationVisualizer.py` & `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/InterpolationVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LUVisualizer.py` & `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LUVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/LeastSquaresVisualizer.py` & `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LeastSquaresVisualizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,22 +69,29 @@
         )
         self.polynomial_degree.observe(
             self.degree_change_poly, names="value"
         )  # observe the change of the int text
         # 3. Int text for selecting the number of sines and cosines
         self.sine_cosine_degree = widgets.BoundedIntText(  # int text for selecting the number of sines and cosines
             value=1,  # default value
-            description="Sines & Cosines degree:",  # description
+            description="",  # description
             disabled=False,
             min=0,
+            layout=widgets.Layout(width="50%")
+            # Make smaller width
         )
+
         self.sine_cosine_degree.observe(
             self.degree_change_sine_cosine, names="value"
         )  # observe the change of the int text
 
+        self.sine_cosine_degree_box = widgets.HBox(
+            [widgets.Label("Basis\n Elements:"), self.sine_cosine_degree]
+        )
+
         # 4. Checkbox for Error Bound Visualization
         self.error_bound = widgets.Checkbox(  # checkbox for error bound visualization
             value=False,  # default value
             description="Error Bound",  # description
             disabled=False,  # disable the checkbox
         )
 
@@ -177,15 +184,15 @@
             to_draw.append(curve)  # add the exponential to the list of marks to draw
             self.exponential_remarks(c, err)  # add the remarks to the remarks widget
 
         elif (
             change["new"] == "Sines & Cosines"
         ):  # if the function type is "Sines & Cosines" then we need to
             to_grid.append(
-                self.sine_cosine_degree
+                self.sine_cosine_degree_box
             )  # add the sine and cosine degree dropdown to the grid
             self.sine_cosine_degree.max = (
                 (  # set the max degree to half the number of data points - 1
                     len(self.x_data_lsp) - 1
                 )
                 // 2
             )  # max degree is half the number of data points - 1
@@ -196,15 +203,19 @@
                 curve
             )  # add the sine and cosine to the list of marks to draw
             self.sine_cosine_remarks(c, err)  # add the remarks to the remarks widget
 
         with self.fig.hold_sync():  # update the figure
             self.fig.marks = to_draw  # update the marks
             self.grid[0:2, 2:] = widgets.VBox(
-                to_grid
+                to_grid,
+                layout=widgets.Layout(  # set the layout of the grid
+                    width="auto",
+                    height="auto",
+                ),
             )  # update the grid (the dropdowns and degree selectors)
 
     def exponential_lsp(self):
         """
         This function returns the exponential function that best fits the data Using LSP
 
         Returns
@@ -256,15 +267,15 @@
             $err$
 
         Parameters
         ----------
         c : np.array
             The coefficients of the exponential function in the form of c[0]*x^c[1]
         """
-        self.remarks.value = f"The exponential function that best fits the data is: <br>$y = {c[0]:.4f}e^{{{c[1]:.4f}x}}$ <br><br> The coefficients of the exponential function are: <br>$c_0 = {c[0]:.4f}$ <br>$c_1 = {c[1]:.4f}$ <br><br> The error is: ${err:.4f}$"
+        self.remarks.value = f"The exponential function that best fits the data is: <br>$y = {c[0]:.4f}e^{{{c[1]:.4f}x}}$ <br><br> The coefficients of the exponential function are: <br>$c_0 = {c[0]:.4f}$ <br>$c_1 = {c[1]:.4f}$ <br><br> The error is: ${err:.4f}$ $\left(\sqrt{{\sum_i (y_i - f(x_i))^2}}\\right)$"
 
     def polynomial_lsp(self, degree):
         """
         This function returns the polynomial function of the given degree that best fits the data Using LSP
 
         Parameters
         ----------
@@ -336,15 +347,15 @@
                 # If the coefficient is 1, add power
 
         remarks += "$ <br><br> The coefficients of the polynomial function are: <br> "  # Second line of the remarks
 
         for i in range(len(c)):  # Add the coefficients of the polynomial function
             remarks += f"$c_{i} = {c[i]:.2f}$<br> "  # Add the coefficient
 
-        remarks += f"<br> The error is {err:.4f}"  # Third line of the remarks
+        remarks += f"<br> The error is ${err:.4f}$ $\left(\sqrt{{\sum_i (y_i - f(x_i))^2}}\\right)$ <br><br>"  # Third line of the remarks
 
         self.remarks.value = remarks  # Update the remarks
 
     def sine_cosine_lsp(self, degree):
         """
         This function returns the sine and cosine function of the given degree that best fits the data Using LSP
 
@@ -389,15 +400,27 @@
         curve = bq.Lines(
             x=self.x,
             y=y,
             scales={"x": self.x_sc, "y": self.y_sc},
             colors=["red"],
         )  # Make the curve object
 
-        err = np.linalg.norm(self.y_data_lsp - A @ c)  # Calculate the error
+        err = np.linalg.norm(
+            self.y_data_lsp
+            - [
+                np.sum(
+                    [
+                        c[i] * np.sin(i * x) + c[i + 1] * np.cos(i * x)
+                        for i in range(1, degree + 1)
+                    ]
+                )
+                + c[0]
+                for x in self.x_data_lsp
+            ]
+        )  # Calculate the error
 
         return curve, c, err
 
     def sine_cosine_remarks(self, c, err):
         """
         This function returns the remarks for the sine and cosine function
 
@@ -432,15 +455,15 @@
             )
 
         remarks += "$ <br><br> The coefficients of the sine and cosine function are: <br> "  # Second part of the remarks (coefficients)
 
         for i in range(len(c)):  # Iterate through coefficients
             remarks += f"$c_{i} = {c[i]:.2f}$ <br>"  # coefficient
 
-        remarks += f"<br> The error is: {err:.4f}"  # Third part of the remarks (error)
+        remarks += f"<br> The error is: ${err:.4f}$ $\left(\sqrt{{\sum_i (y_i - f(x_i))^2}}\\right)$ <br><br>"  # Third part of the remarks (error)
 
         self.remarks.value = remarks  # Set the remarks
 
     def run(self):
         self.initialize_components()
 
         return self.grid
```

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/NonLinearVisualizer.py` & `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/NonLinearVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/Visualizers/RandomVisualizer.py` & `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/RandomVisualizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -143,21 +143,27 @@
             button_style="",  # 'success', 'info', 'warning', 'danger' or ''
             tooltip="Run",
             icon="check",  # (FontAwesome names without the `fa-` prefix)
         )
         # Observer: Button for running the algorithm
         self.run_button.on_click(self.play_montecarlo)
 
+        self.pi_value = widgets.FloatText( # Widget: Pi value
+            value=0,
+            description="$\pi$:",
+            disabled=True,
+        )
         # Widget: Grid
         # =================================================================================================
         self.grid = widgets.GridspecLayout(4, 4)
         self.grid[0:2, 0:2] = self.figure1
         self.grid[2:4, 0:4] = self.figure2
-        self.grid[0:1, 2:4] = self.iterations_widget
-        self.grid[1:2, 2:4] = self.run_button
+        self.grid[0:1, 2:4] = widgets.VBox([self.iterations_widget,self.run_button])
+        
+        self.grid[1:2, 2:4] = self.pi_value
 
     def number_of_iterations(self):
         """
         Updates the number of iterations. This is called when the user plays the animation. It configures the x axis of the second figure. and the number of iterations of the algorithm.
         """
         self.iterations = self.iterations_widget.value
         self.x_sc2.max = self.iterations
@@ -194,14 +200,16 @@
             with self.current_value_line.hold_sync():  # Animation for the current value
                 self.current_value_line.x = [x for x in self.current_value_line.x] + [
                     self.current_iteration
                 ]
                 self.current_value_line.y = [y for y in self.current_value_line.y] + [
                     self.current_value
                 ]
+                self.pi_value.value = self.current_value
+            sleep(0.0001)
 
         self.run_button.disabled = False
 
     def run(self):
         """
         Runs the visualizer.
         """
```

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet/module.py` & `BNumMet-1.0.0.dev8/src/BNumMet/module.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet.egg-info/PKG-INFO` & `BNumMet-1.0.0.dev8/src/BNumMet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BNumMet
-Version: 1.0.0.dev7
+Version: 1.0.0.dev8
 Summary: Basic Numerical Methods for Python 3
 Home-page: https://github.com/fbpazos/Trabajo-Fin-Master/tree/main/Python_BNumMet
 Author: Fernando Bellido Pazos
 Author-email: fbellidopazos@gmail.com
 License: AGPL-3.0
 Platform: unix
 Platform: linux
```

### Comparing `BNumMet-1.0.0.dev7/src/BNumMet.egg-info/SOURCES.txt` & `BNumMet-1.0.0.dev8/src/BNumMet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/tests/test_General.py` & `BNumMet-1.0.0.dev8/tests/test_General.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/tests/test_Interpolation.py` & `BNumMet-1.0.0.dev8/tests/test_Interpolation.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/tests/test_LeastSquares.py` & `BNumMet-1.0.0.dev8/tests/test_LeastSquares.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/tests/test_LinealSystems.py` & `BNumMet-1.0.0.dev8/tests/test_LinealSystems.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/tests/test_NonLinear.py` & `BNumMet-1.0.0.dev8/tests/test_NonLinear.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/tests/test_Random.py` & `BNumMet-1.0.0.dev8/tests/test_Random.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev7/tests/test_module.py` & `BNumMet-1.0.0.dev8/tests/test_module.py`

 * *Files identical despite different names*

