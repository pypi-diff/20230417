# Comparing `tmp/iloscar-0.1a0.tar.gz` & `tmp/iloscar-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar-0.1a0.tar", last modified: Tue Apr 11 20:32:17 2023, max compression
+gzip compressed data, was "iloscar-0.2.0b0.tar", last modified: Mon Apr 17 20:18:50 2023, max compression
```

## Comparing `iloscar-0.1a0.tar` & `iloscar-0.2.0b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.592731 iloscar-0.1a0/
--rw-r--r--   0 shihan     (504) staff       (20)      728 2023-04-11 20:32:17.592362 iloscar-0.1a0/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-04 17:29:12.000000 iloscar-0.1a0/README.md
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.589587 iloscar-0.1a0/iloscar/
--rw-r--r--   0 shihan     (504) staff       (20)      341 2023-04-05 02:45:38.000000 iloscar-0.1a0/iloscar/__init__.py
--rw-rw-r--   0 shihan     (504) staff       (20)     2006 2023-04-11 20:27:13.000000 iloscar-0.1a0/iloscar/app.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.590968 iloscar-0.1a0/iloscar/dat_y0/
--rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.1a0/iloscar/dat_y0/petm_steady.dat
--rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.1a0/iloscar/dat_y0/preind_steady.dat
--rw-rw-r--   0 shihan     (504) staff       (20)   106011 2023-04-09 03:50:44.000000 iloscar-0.1a0/iloscar/iLOSCAR_backend.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.591893 iloscar-0.1a0/iloscar/pages/
--rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-11 20:28:53.000000 iloscar-0.1a0/iloscar/pages/Function.py
--rw-rw-r--   0 shihan     (504) staff       (20)    26082 2023-04-11 20:28:43.000000 iloscar-0.1a0/iloscar/pages/forward.py
--rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-11 20:29:07.000000 iloscar-0.1a0/iloscar/pages/home.py
--rw-rw-r--   0 shihan     (504) staff       (20)    45707 2023-04-11 20:29:17.000000 iloscar-0.1a0/iloscar/pages/inverse.py
--rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.1a0/iloscar/style.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-11 20:32:17.590374 iloscar-0.1a0/iloscar.egg-info/
--rw-r--r--   0 shihan     (504) staff       (20)      728 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/SOURCES.txt
--rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/dependency_links.txt
--rw-r--r--   0 shihan     (504) staff       (20)      117 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/requires.txt
--rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-11 20:32:17.000000 iloscar-0.1a0/iloscar.egg-info/top_level.txt
--rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-11 20:32:17.592818 iloscar-0.1a0/setup.cfg
--rw-r--r--   0 shihan     (504) staff       (20)     1432 2023-04-11 20:31:11.000000 iloscar-0.1a0/setup.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:18:50.400522 iloscar-0.2.0b0/
+-rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 20:18:50.400262 iloscar-0.2.0b0/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)    17746 2023-04-17 20:16:31.000000 iloscar-0.2.0b0/README.md
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:18:50.396919 iloscar-0.2.0b0/iloscar/
+-rw-r--r--   0 shihan     (504) staff       (20)      341 2023-04-05 02:45:38.000000 iloscar-0.2.0b0/iloscar/__init__.py
+-rw-rw-r--   0 shihan     (504) staff       (20)     1755 2023-04-17 20:14:42.000000 iloscar-0.2.0b0/iloscar/app.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:18:50.398541 iloscar-0.2.0b0/iloscar/dat_y0/
+-rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.2.0b0/iloscar/dat_y0/petm_steady.dat
+-rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.2.0b0/iloscar/dat_y0/preind_steady.dat
+-rw-rw-r--   0 shihan     (504) staff       (20)   106518 2023-04-17 20:14:07.000000 iloscar-0.2.0b0/iloscar/iLOSCAR_backend.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:18:50.399646 iloscar-0.2.0b0/iloscar/pages/
+-rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-17 20:15:49.000000 iloscar-0.2.0b0/iloscar/pages/Function.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    26239 2023-04-17 20:15:24.000000 iloscar-0.2.0b0/iloscar/pages/forward.py
+-rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-17 20:15:56.000000 iloscar-0.2.0b0/iloscar/pages/home.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    46213 2023-04-17 20:15:41.000000 iloscar-0.2.0b0/iloscar/pages/inverse.py
+-rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.2.0b0/iloscar/style.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 20:18:50.398037 iloscar-0.2.0b0/iloscar.egg-info/
+-rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 20:18:50.000000 iloscar-0.2.0b0/iloscar.egg-info/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-17 20:18:50.000000 iloscar-0.2.0b0/iloscar.egg-info/SOURCES.txt
+-rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-17 20:18:50.000000 iloscar-0.2.0b0/iloscar.egg-info/dependency_links.txt
+-rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-17 20:18:50.000000 iloscar-0.2.0b0/iloscar.egg-info/requires.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-17 20:18:50.000000 iloscar-0.2.0b0/iloscar.egg-info/top_level.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-17 20:18:50.400581 iloscar-0.2.0b0/setup.cfg
+-rw-r--r--   0 shihan     (504) staff       (20)     1451 2023-04-17 20:17:36.000000 iloscar-0.2.0b0/setup.py
```

### Comparing `iloscar-0.1a0/iloscar/app.py` & `iloscar-0.2.0b0/iloscar/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 import dash
 from dash import html, dcc, DiskcacheManager, CeleryManager
 from dash_extensions.enrich import Output, DashProxy, Input, MultiplexerTransform
 import dash_bootstrap_components as dbc
 from iloscar.style import *
 import diskcache
 
+cache = diskcache.Cache('./cache')
 
-def iloscar_run():
-    cache = diskcache.Cache('./cache')
-
-
-
-    external_stylesheets = [dbc.themes.SPACELAB]
-    # [
-    #     {
-    #         "href": (
-    #             "https://fonts.googleapis.com/css2?"
-    #             "family=Lato:wght@400;700&display=swap"
-    #         ),
-    #         "rel": "stylesheet",
-    #     },]
-    # [dbc.themes.SPACELAB]
-    app = DashProxy(__name__, use_pages=True, external_stylesheets=external_stylesheets,
-        background_callback_manager = DiskcacheManager(cache),
-        transforms=[MultiplexerTransform()])
-    sidebar = dbc.Nav(
-                [
-                    dbc.NavLink(
-                        [
-                            html.Div(page["name"], className="ms-2"),
-                        ],
-                        href=page["path"],
-                        active="exact",
-                    )
-                    for page in dash.page_registry.values()
-                ],
-                vertical=True,
-                pills=True,
-                className="bg-light",
-                style = {'fontSize': 20}
-    )
-
-
-    app.layout = dbc.Container([
-        dbc.Row([
-            dbc.Col(html.Div("Welcom to iLOSCAR",
-                             style={'fontSize':50, 'textAlign':'center'}))
-        ]),
-
-        html.Hr(),
-
-        dbc.Row(
+external_stylesheets = [dbc.themes.SPACELAB]
+# [
+#     {
+#         "href": (
+#             "https://fonts.googleapis.com/css2?"
+#             "family=Lato:wght@400;700&display=swap"
+#         ),
+#         "rel": "stylesheet",
+#     },]
+# [dbc.themes.SPACELAB]
+app = DashProxy(__name__, use_pages=True, external_stylesheets=external_stylesheets,
+    background_callback_manager = DiskcacheManager(cache),
+    transforms=[MultiplexerTransform()])
+sidebar = dbc.Nav(
             [
-                dbc.Col(
-                    [
-                        sidebar
-                    ], xs=4, sm=4, md=2, lg=2, xl=2, xxl=2),
-
-                dbc.Col(
+                dbc.NavLink(
                     [
-                        dash.page_container
-                    ], xs=8, sm=8, md=10, lg=10, xl=10, xxl=10)
-            ]
-        )
-    ], fluid=True)
+                        html.Div(page["name"], className="ms-2"),
+                    ],
+                    href=page["path"],
+                    active="exact",
+                )
+                for page in dash.page_registry.values()
+            ],
+            vertical=True,
+            pills=True,
+            className="bg-light",
+            style = {'fontSize': 20}
+)
+
+
+app.layout = dbc.Container([
+    dbc.Row([
+        dbc.Col(html.Div("Welcom to iLOSCAR",
+                         style={'fontSize':50, 'textAlign':'center'}))
+    ]),
+
+    html.Hr(),
+
+    dbc.Row(
+        [
+            dbc.Col(
+                [
+                    sidebar
+                ], xs=4, sm=4, md=2, lg=2, xl=2, xxl=2),
 
+            dbc.Col(
+                [
+                    dash.page_container
+                ], xs=8, sm=8, md=10, lg=10, xl=10, xxl=10)
+        ]
+    )
+], fluid=True)
 
 
-    app.run(debug=False, port = '7777')
-    print('iLOSCAR is running on http://127.0.0.1:7777/')
+if __name__ == "__main__":
+    app.run(debug=True, port = '7777')
```

### Comparing `iloscar-0.1a0/iloscar/dat_y0/petm_steady.dat` & `iloscar-0.2.0b0/iloscar/dat_y0/petm_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.1a0/iloscar/dat_y0/preind_steady.dat` & `iloscar-0.2.0b0/iloscar/dat_y0/preind_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.1a0/iloscar/iLOSCAR_backend.py` & `iloscar-0.2.0b0/iloscar/iLOSCAR_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,29 +32,29 @@
 import pandas as pd
 import numpy as np
 from numba import jit
 import sys
 
 import dash
 from dash import html, dcc
-from style import *
 
 import timeit
 import plotly.graph_objects as go
 
 
 from scipy import interpolate
 from scipy.optimize import root_scalar, toms748
 
 
 from scipy.integrate import solve_ivp
 
 from os.path import join, exists
 from os import makedirs
 
+from iloscar.style import *
 
 
 
 
 
 def init_start(params):
     # input: front-end user input
@@ -70,19 +70,23 @@
     FTYS = params['FTYS']
     FSED = params['FSED']
     LOADFLAG = params['LOADFLAG']
     RUN_TYPE = params['RUN_TYPE']   # AUTOMATICALLY Determined BY THE WEBSITE
     tsnsflag = params['tsnsflag']
 
     if RUN_TYPE == 2:
-        global target_type, target_file, target_file2
+        global target_type, target_file, target_file2, toms_low, toms_high
         target_type = params['target']
         target_file = params['target_file']
         target_file2 = params['target_file2']
         LOADFLAG = 1
+        toms_low = params['toms_low']
+        toms_high = params['toms_high']
+
+
 
     try:
         svstart = params['svstart']
     except:
         svstart = 0
     # if LOADFLAG == 1:
     #     svstart = 0
@@ -267,14 +271,15 @@
     ])
 
 ])
     return info_start, 'Success'
 
 
 def model_run(set_progress):
+
     global RUN_TYPE
     if RUN_TYPE == 1:
         start_time = timeit.default_timer()
 
 
         hpls = np.ones(NB) * HGUESS
 
@@ -346,15 +351,15 @@
 
                 hpls = np.ones(NB) * HGUESS
 
                 # ems_new = fmin(cost_function, init_guess, args = (tracer_type, hpls, tems, ems), disp = True)
                 # ems_new = root_scalar(cost_function, x0 = init_guess, x1 = init_guess+0.01, method = 'secant',
                 #                       args = (tracer_type, hpls, tems, ems))
                 # ems_new = ems_new.root
-                ems_new, results = toms748(cost_function, -0.5, 5,
+                ems_new, results = toms748(cost_function, toms_low , toms_high,
                                         args = (tracer_type, hpls, tems, ems),
                                         xtol = 1e-4, rtol = 1e-8,
                                         full_output = True)
 
                 tracer_eval[i+1] = ems_new
 
                 # write out the ysol as the initial values for the next loop
@@ -437,15 +442,15 @@
                 hpls = np.ones(NB) * HGUESS
                 # ems_d13c_new = fmin(cost_function, init_guess, args = (tracer_type, hpls, tems, ems_d13c), disp = True)
 
                 # ems_d13c_new = root_scalar(cost_function, x0 = init_guess, x1 = init_guess+10, method = 'secant',
                 #              args = (tracer_type, hpls, tems, ems_d13c))
                 # ems_d13c_new = ems_d13c_new.root
 
-                ems_new, results = toms748(cost_function, -1, 10,
+                ems_new, results = toms748(cost_function, tom_low, toms_high,
                                         args = ('d13c_for_emi', hpls, tems, ems),
                                         xtol = 1e-4, rtol = 1e-8,
                                         full_output = True)
 
 
                 tracer_eval[i+1]= ems_new
 
@@ -549,15 +554,15 @@
 
                 # ems_new = fmin(cost_function, init_guess, args = (tracer_type, hpls,tems, ems), disp = True)
 
 
                 # ems_new = root_scalar(cost_function, x0 = init_guess, x1 = init_guess+diff_init_guess, method = 'secant', options ={'disp': True},
                 #                      args = (tracer_type, hpls, tems, ems))
 
-                ems_new, results = toms748(cost_function, -0.5, 5,
+                ems_new, results = toms748(cost_function, toms_low, toms_high,
                                         args = (tracer_type, hpls, tems, ems),
                                         xtol = 1e-4, rtol = 1e-8,
                                         full_output = True)
 
 
 
 
@@ -638,15 +643,15 @@
                 hpls = np.ones(NB) * HGUESS
 
                 # ems_new = fmin(cost_function, init_guess, args = ('pCO2', hpls, tems, ems), disp = True)
                 # ems_new = root_scalar(cost_function, x0 = init_guess, x1 = init_guess+0.01, method = 'secant',
                 #                       args = ('pCO2', hpls, tems, ems))
                 # ems_new = ems_new.root
 
-                ems_new, results = toms748(cost_function, -0.5, 5,
+                ems_new, results = toms748(cost_function, toms_low, toms_high,
                                         args = ('pCO2', hpls, tems, ems),
                                         xtol = 1e-4, rtol = 1e-8,
                                         full_output = True)
 
 
                 tracer_eval[i+1] = ems_new
 
@@ -728,14 +733,18 @@
                     hpls = np.ones(NB) * HGUESS
                     # ems_d13c_new = fmin(cost_function, init_guess, args = ('d13c', hpls, tems_d13c, ems_d13c), disp = True)
                     ems_d13c_new = root_scalar(cost_function, x0 = init_guess, x1 = init_guess+5, method = 'secant',
                                             xtol = 1e-4, rtol = 1e-8,
                                           args = ('d13c', hpls, tems_d13c, ems_d13c))
 
                     ems_d13c_new = ems_d13c_new.root
+                    if ems_d13c_new > 35:
+                        ems_d13c_new = 35
+                    elif ems_d13c_new < -80:
+                        ems_d13c_new = -80
 
 
                     d13c_eval[i]= ems_d13c_new
 
 
                 # write out hte ysol as the initial values for next loop
 
@@ -805,15 +814,15 @@
                 hpls = np.ones(NB) * HGUESS
 
                 # ems_new = fmin(cost_function, init_guess, args = ('GSpH', hpls, tems, ems), disp = True)
                 # ems_new = root_scalar(cost_function, x0 = init_guess, x1 = init_guess+0.01, method = 'secant',
                 #                       args = ('GSpH', hpls, tems, ems))
                 #
                 # ems_new = ems_new.root
-                ems_new, results = toms748(cost_function, -0.5, 5,
+                ems_new, results = toms748(cost_function, toms_low, toms_high,
                                         args = ('GSpH', hpls, tems, ems),
                                         xtol = 1e-4, rtol = 1e-8,
                                         full_output = True)
 
 
                 tracer_eval[i+1] = ems_new
 
@@ -899,31 +908,39 @@
                     # ems_d13c_new = fmin(cost_function, init_guess, args = ('d13c', hpls, tems_d13c, ems_d13c), disp = True)
                     ems_d13c_new = root_scalar(cost_function, x0 = init_guess, x1 = init_guess+5, method = 'secant',
                                           xtol = 1e-4, rtol = 1e-8,
                                           args = ('d13c', hpls, tems_d13c, ems_d13c))
 
 
                     ems_d13c_new = ems_d13c_new.root
+
+                    if ems_d13c_new > 35:
+                        ems_d13c_new = 35
+                    elif ems_d13c_new < -80:
+                        ems_d13c_new = -80
+
                     d13c_eval[i]= ems_d13c_new
 
 
 
 
 
+
+
                 # write out hte ysol as the initial values for next loop
 
                 ysol = solve_ivp(derivs, (tems_d13c[0], tems_d13c[1]), y0, args = [0, hpls], t_eval = [tems_d13c[1]], method = 'LSODA')
                 yfinal = ysol.y[:,-1]
                 yfinal[3*NB:4*NB] *= TSCAL
                 np.savetxt('inv_ystart.dat', yfinal)
 
             elapse = timeit.default_timer() - start_time
             print(f'{elapse: .2f}s used.')
 
-            
+
             RUN_TYPE = 3
             frccinp = interpolate.interp1d(t_target_d13c, (d13c_eval/1e3+1)*RST, bounds_error=False, fill_value=((d13c_eval[0]/1e3+1)*RST,0), kind = 'zero')
             # emi_d13c_scenario = np.vstack([t_target_d13c, d13c_eval]).T
             # np.savetxt('inverse_emission_d13c_results.dat', emi_d13c_scenario)
             t_end = np.minimum(t_target[-1], t_target_d13c[-1])
             t_start = np.minimum(t_target[0], t_target_d13c[0])
             tt = np.linspace(t_target_d13c[0], t_target_d13c[-1]-10, int((t_target[-1]-t_target[0])/100))
```

### Comparing `iloscar-0.1a0/iloscar/pages/Function.py` & `iloscar-0.2.0b0/iloscar/pages/Function.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1a0/iloscar/pages/forward.py` & `iloscar-0.2.0b0/iloscar/pages/forward.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     ('Comment', [ f'3: emission scenario with time-dependant d13c \n 2: emission scenario from the external files \n 1:carbon emission in uniform distribution \n 0: no carbon emission',
     'total amount of carbon input, \n only useful when Emission_Pattern == 1', 'd13c of input carbon, \n only useful when Emission_Pattern == 1', 'start year for the emission, \n only useful when Emission_Pattern == 1', 'duration for the emission, \n only useful when Emission_Pattern == 1',
 ]),
 
 ]))
 
 df_file = pd.DataFrame(OrderedDict([
-    ('File name', ['./preind_steady.dat', './1000_0500.dat', './preind_steady.dat']),
+    ('File name', ['./preind_steady.dat', './pulse_emi.dat', './preind_steady.dat']),
     ('Parameter', ['Initial steady state file name',
                    'Time-resolved carbon input ',
                    'File to save the final modeling results']),
     ('Comment', [ 'Required only when LOADFLAG == 1 in Step 1',
                   'Required only when Emission pattern == 2 or 3 in Step 3',
                   'Required only when Save ystart == 1'
 ]),
@@ -575,14 +575,15 @@
         prevent_initial_call = True
         )
 
 def initialize(data):
 
     if data:
         info_starting = init_start(data)
+
         return info_starting
 
     else:
         return [], 'Fail'
 
 # activate the progress bar
 @callback(Output('progress_bar', 'hidden'),
@@ -601,14 +602,15 @@
 
     else:
         return True, []
 
 # run the model
 @callback(output = [Output('info_integration', 'children'), Output('ysol', 'data'), Output('tsol', 'data')],
         inputs = [Input('progress_bar','hidden')],
+        state = State('parameters', 'data')
         background = True,
         progress = [Output('progress_bar', 'value'), Output('progress_bar', 'max')],
          running=[
         (Output("run", "disabled"), True, False),
         (Output('cancel_run', 'disabled'), False, True),
     ],
         cancel = [Input('cancel_run','n_clicks')],
@@ -617,15 +619,19 @@
         )
 def update_progress(set_progress,key):
 
 
     if key:
         return [], [], []
     else:
-        return model_run(set_progress)
+        try:
+            return model_run(set_progress)
+        except:
+            temp = init_start(data)
+            return model_run(set_progress)
 
 
 
 # # save the results
 # @callback(Output('info_wo_results','children'),
 #
 #             Input('run', 'n_clicks'), prevent_initial_call = True
```

### Comparing `iloscar-0.1a0/iloscar/pages/home.py` & `iloscar-0.2.0b0/iloscar/pages/home.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1a0/iloscar/pages/inverse.py` & `iloscar-0.2.0b0/iloscar/pages/inverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,28 +90,28 @@
         'thermalhaline transport', 'oceanic Ca concentration', 'oceanic Mg concentration', 'default OCN temperature change per double pCO2', 'silicate weathering exponent',
         'carbonate weathering exponent'
 
     ]),
 ]))
 
 df_carbon_emission_inv = pd.DataFrame(OrderedDict([
-    ('Value', [-55]),
-    ('Parameter', [ 'd13c emission']),
-    ('Unit', [ 'per mil']),
-    ('Comment', [  'd13c of input carbon, \n required for the single version'
+    ('Value', [-55, -0.5, 5]),
+    ('Parameter', [ 'd13c emission', 'Lower boundary in bracket for toms748 method. Absolute value equivalent to expected maximum organic burial rate',
+                        'Higher boundary in barcket for toms748 method. Value equivalent to maximum degassing rate']),
+    ('Unit', [ 'per mil', 'Gt/yr', 'Gt/yr']),
+    ('Comment', ['d13c of input carbon, \n required for the single version', 'Default settings can work for most applications. Adjust the value for extream case',
+    'Increase the absolute value can reduce the failure probability of experiment, but at the expense of running speed'
 ]),
 
 ]))
 
 df_file_inv = pd.DataFrame(OrderedDict([
-    ('File name', ['./preind_steady.dat', './test.dat']),
-    ('Parameter', ['Initial steady state file name',
-                   'Time-resolved carbon input ']),
-    ('Comment', [ 'Required only when LOADFLAG == 1 in Step 1',
-                  'Required only when Emission pattern == 2 or 3 in Step 3'
+    ('File name', ['./preind_steady.dat']),
+    ('Parameter', ['Initial steady state file name']),
+    ('Comment', [ 'Required in Inversion mode'
 ]),
 
 ]))
 
 inverse_mode = dash_table.DataTable(
     id='version_inv',
     data=df_mode_inv.to_dict('records'),
@@ -269,19 +269,19 @@
 
                     'fepl': 0.8, 'eph':1.8, 'rrain':6.1, "fsh":1,
                     'fsi0': 5e12, 'finc0': 12, 'd13cin': 1.5, 'd13cvc': -4.0,
                     'thc': 20, 'cac': 10.3e-3, 'mgc': 53e-3, 'sclim': 3, 'nsi':0.2,
                     'ncc': 0.4}
 param_model_inv = dcc.Store(id = 'param_model_inv_container', data = parameters_model_inv)
 
-parameters_carbon_inv = {'dccinp':-55}
+parameters_carbon_inv = {'dccinp':-55, 'toms_low': -0.5, 'toms_high': 5}
 param_carbon_inv = dcc.Store(id = 'param_carbon_inv_container', data = parameters_carbon_inv)
 
 
-parameters_file_inv = {'initfile': './preind_steady.dat', 'cinpfile': './1000_0500.dat'}
+parameters_file_inv = {'initfile': './preind_steady.dat', 'cinpfile': './pulse_emi.dat'}
 param_file_inv = dcc.Store(id = 'param_file_inv_container', data = parameters_file_inv)
 
 run_section_inv = html.Div(style = {'textAlign':'left', "margin-left": "10rem"}, children =
         [
         dbc.Label(style = {'fontSize': 24}, children = "Experiment name"),
         dbc.Input(placeholder = 'Input experiment name...', id = 'exp_name_inv', type = 'text'),
         dbc.FormText('The modeling results will be saved in a dictionary after experinent name', style = {'fontSize': 18})
@@ -706,29 +706,34 @@
         if key == 'Success':
             return False, 'Progressing...'
     else:
         return True, []
 # run the model
 @callback(output = [ Output('info_integration_inv', 'children'), Output('ysol_inv', 'data'), Output('tsol_inv', 'data')],
         inputs = Input('progress_bar_inv','hidden'),
+        state = State('paramters_inv', 'data')
         background = True,
         running=[
        (Output("run_inv", "disabled"), True, False),
        (Output('cancel_run_inv', 'disabled'), False, True),
    ],
         progress = [Output('progress_bar_inv', 'value'), Output('progress_bar_inv', 'max')],
         cancel = [Input('cancel_run_inv','n_clicks')],
         prevent_initial_call = True,
 
         )
-def update_progress(set_progress,key):
+def update_progress(set_progress,key, data):
     if key:
         return [], [], []
     else:
-        return model_run(set_progress)
+        try:
+            return model_run(set_progress)
+        except:
+            temp = init_start(data)
+            return model_run(set_progress)
 
 
 # save the results
 @callback(Output('info_wo_results_inv','children'),
             Input('ysol_inv', 'data'),
             Input('tsol_inv', 'data'), prevent_initial_call = True
             )
```

### Comparing `iloscar-0.1a0/iloscar/style.py` & `iloscar-0.2.0b0/iloscar/style.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.1a0/setup.py` & `iloscar-0.2.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1-alpha'
+VERSION = '0.2.0-beta'
 DESCRIPTION = 'iLOSCAR'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar",
     version=VERSION,
@@ -19,25 +19,25 @@
     license = 'MIT',
     author="Shihan Li",
     author_email="<shihan@tamu.edu>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=['iloscar', 'iloscar/pages'],
-    install_requires=['numpy', 'scipy', 'dash', 'plotly', 'pandas', 'numba', 'diskcache', 'statsmodels', 'dash_bootstrap_components','dash_extensions','dash[diskcache]'],
+    install_requires=['numpy', 'scipy', 'dash', 'plotly', 'pandas', 'numba', 'diskcache', 'statsmodels', 'dash_bootstrap_components','dash_extensions','dash[diskcache]', 'dill == 0.3.5.1'],
     keywords=['python', 'carbon cycle', 'model', 'paleoclimate', 'global warming', 'LOSCAR'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 
     include_package_data = True,
     package_data = {
     'iloscar': ['dat_y0/*.dat']
     },
-    python_requires='>=3.7, <3.11'
+    python_requires='>3.7, <3.11'
 
 )
```

