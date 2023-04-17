# Comparing `tmp/lidia-0.8.0.tar.gz` & `tmp/lidia-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidia-0.8.0.tar", last modified: Tue Apr  4 15:52:06 2023, max compression
+gzip compressed data, was "lidia-0.8.1.tar", last modified: Mon Apr 17 19:46:17 2023, max compression
```

## Comparing `lidia-0.8.0.tar` & `lidia-0.8.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-04-04 15:52:06.850226 lidia-0.8.0/
--rw-rw-r--   0 marek     (1000) marek     (1000)     1077 2023-02-17 09:15:54.000000 lidia-0.8.0/LICENSE.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)      110 2023-03-21 14:18:14.000000 lidia-0.8.0/MANIFEST.in
--rw-rw-r--   0 marek     (1000) marek     (1000)     2434 2023-04-04 15:52:06.850226 lidia-0.8.0/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)     1981 2023-03-21 14:18:14.000000 lidia-0.8.0/README.md
--rw-rw-r--   0 marek     (1000) marek     (1000)       85 2023-01-31 11:07:27.000000 lidia-0.8.0/pyproject.toml
--rw-rw-r--   0 marek     (1000) marek     (1000)      819 2023-04-04 15:52:06.854226 lidia-0.8.0/setup.cfg
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-04-04 15:52:06.838226 lidia-0.8.0/src/
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-04-04 15:52:06.846226 lidia-0.8.0/src/lidia/
--rw-rw-r--   0 marek     (1000) marek     (1000)       22 2023-04-04 15:49:54.000000 lidia-0.8.0/src/lidia/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)       32 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/__main__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)    12275 2023-04-04 15:43:56.000000 lidia-0.8.0/src/lidia/aircraft.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     3473 2023-02-17 09:15:54.000000 lidia-0.8.0/src/lidia/approach.html
--rw-rw-r--   0 marek     (1000) marek     (1000)     5095 2023-02-17 09:15:54.000000 lidia-0.8.0/src/lidia/cas.html
--rw-rw-r--   0 marek     (1000) marek     (1000)     3711 2023-03-28 12:39:55.000000 lidia-0.8.0/src/lidia/config.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     1022 2023-04-04 15:46:49.000000 lidia-0.8.0/src/lidia/info.html
--rw-rw-r--   0 marek     (1000) marek     (1000)     5049 2023-03-21 14:18:14.000000 lidia-0.8.0/src/lidia/lidia.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2465 2023-04-04 15:45:22.000000 lidia-0.8.0/src/lidia/mytypes.py
--rw-rw-r--   0 marek     (1000) marek     (1000)    27190 2023-04-04 15:13:12.000000 lidia-0.8.0/src/lidia/pfd.html
--rw-rw-r--   0 marek     (1000) marek     (1000)    15445 2023-02-28 11:19:48.000000 lidia-0.8.0/src/lidia/rpctask.html
--rw-rw-r--   0 marek     (1000) marek     (1000)     2253 2023-02-28 09:21:34.000000 lidia-0.8.0/src/lidia/server.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-04-04 15:52:06.846226 lidia-0.8.0/src/lidia/sources/
--rw-rw-r--   0 marek     (1000) marek     (1000)        0 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/sources/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2178 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/sources/approach.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     1528 2023-02-17 09:15:54.000000 lidia-0.8.0/src/lidia/sources/confighelp.md
--rw-rw-r--   0 marek     (1000) marek     (1000)     2360 2023-02-28 10:38:57.000000 lidia-0.8.0/src/lidia/sources/confighelp.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     5003 2023-04-04 15:45:07.000000 lidia-0.8.0/src/lidia/sources/demo.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2864 2023-02-28 10:35:09.000000 lidia-0.8.0/src/lidia/sources/flightgear.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     6414 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/sources/mytypes.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     3537 2023-02-28 11:07:21.000000 lidia-0.8.0/src/lidia/sources/rpctask.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2049 2023-02-28 10:38:33.000000 lidia-0.8.0/src/lidia/sources/smol.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-04-04 15:52:06.850226 lidia-0.8.0/src/lidia/static/
--rw-rw-r--   0 marek     (1000) marek     (1000)     1720 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/LICENSE.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)    87008 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/RobotoMono-Bold.ttf
--rw-rw-r--   0 marek     (1000) marek     (1000)    87788 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/RobotoMono-ExtraLight.ttf
--rw-rw-r--   0 marek     (1000) marek     (1000)    87592 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/RobotoMono-Light.ttf
--rw-rw-r--   0 marek     (1000) marek     (1000)    86820 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/RobotoMono-Medium.ttf
--rw-rw-r--   0 marek     (1000) marek     (1000)    86908 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/RobotoMono-Regular.ttf
--rw-rw-r--   0 marek     (1000) marek     (1000)    87076 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/RobotoMono-SemiBold.ttf
--rw-rw-r--   0 marek     (1000) marek     (1000)    87872 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/RobotoMono-Thin.ttf
--rw-rw-r--   0 marek     (1000) marek     (1000)     6868 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/controls.js
--rw-rw-r--   0 marek     (1000) marek     (1000)   117245 2023-01-31 11:07:27.000000 lidia-0.8.0/src/lidia/static/socket.io.js
--rw-rw-r--   0 marek     (1000) marek     (1000)     1747 2023-02-28 09:26:40.000000 lidia-0.8.0/src/lidia/static/style.css
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-04-04 15:52:06.850226 lidia-0.8.0/src/lidia/utils/
--rw-rw-r--   0 marek     (1000) marek     (1000)     3561 2023-04-03 14:46:01.000000 lidia-0.8.0/src/lidia/utils/pack_lidia.m
--rw-rw-r--   0 marek     (1000) marek     (1000)    21744 2023-04-04 14:56:44.000000 lidia-0.8.0/src/lidia/utils/pack_maker.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-04-04 15:52:06.846226 lidia-0.8.0/src/lidia.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)     2434 2023-04-04 15:52:06.000000 lidia-0.8.0/src/lidia.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)     1224 2023-04-04 15:52:06.000000 lidia-0.8.0/src/lidia.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-04-04 15:52:06.000000 lidia-0.8.0/src/lidia.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       43 2023-04-04 15:52:06.000000 lidia-0.8.0/src/lidia.egg-info/entry_points.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       97 2023-04-04 15:52:06.000000 lidia-0.8.0/src/lidia.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        6 2023-04-04 15:52:06.000000 lidia-0.8.0/src/lidia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.486624 lidia-0.8.1/
+-rw-rw-rw-   0        0        0     1097 2023-02-17 08:50:04.000000 lidia-0.8.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      114 2023-03-01 12:02:42.000000 lidia-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2519 2023-04-17 19:46:17.487624 lidia-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2052 2023-03-01 12:02:42.000000 lidia-0.8.1/README.md
+-rw-rw-rw-   0        0        0       88 2022-12-15 16:52:24.000000 lidia-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0      858 2023-04-17 19:46:17.492624 lidia-0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 19:46:16.543715 lidia-0.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 19:46:16.955289 lidia-0.8.1/src/lidia/
+-rw-rw-rw-   0        0        0       23 2023-04-17 19:44:25.000000 lidia-0.8.1/src/lidia/__init__.py
+-rw-rw-rw-   0        0        0       35 2022-06-02 23:11:14.000000 lidia-0.8.1/src/lidia/__main__.py
+-rw-rw-rw-   0        0        0    12690 2023-04-17 19:44:25.000000 lidia-0.8.1/src/lidia/aircraft.py
+-rw-rw-rw-   0        0        0     3584 2023-02-17 08:50:04.000000 lidia-0.8.1/src/lidia/approach.html
+-rw-rw-rw-   0        0        0     5293 2023-02-17 08:50:04.000000 lidia-0.8.1/src/lidia/cas.html
+-rw-rw-rw-   0        0        0     3821 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/config.py
+-rw-rw-rw-   0        0        0     1061 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/info.html
+-rw-rw-rw-   0        0        0     5165 2023-03-01 12:02:42.000000 lidia-0.8.1/src/lidia/lidia.py
+-rw-rw-rw-   0        0        0     2540 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/mytypes.py
+-rw-rw-rw-   0        0        0    27835 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/pfd.html
+-rw-rw-rw-   0        0        0    15774 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/rpctask.html
+-rw-rw-rw-   0        0        0     2312 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/server.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.131388 lidia-0.8.1/src/lidia/sources/
+-rw-rw-rw-   0        0        0        0 2022-06-13 10:57:36.000000 lidia-0.8.1/src/lidia/sources/__init__.py
+-rw-rw-rw-   0        0        0     2236 2022-12-19 19:16:52.000000 lidia-0.8.1/src/lidia/sources/approach.py
+-rw-rw-rw-   0        0        0     1551 2023-02-17 08:50:04.000000 lidia-0.8.1/src/lidia/sources/confighelp.md
+-rw-rw-rw-   0        0        0     2416 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/confighelp.py
+-rw-rw-rw-   0        0        0     5204 2023-04-17 19:44:25.000000 lidia-0.8.1/src/lidia/sources/demo.py
+-rw-rw-rw-   0        0        0     2937 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/flightgear.py
+-rw-rw-rw-   0        0        0     6600 2022-12-19 19:16:52.000000 lidia-0.8.1/src/lidia/sources/mytypes.py
+-rw-rw-rw-   0        0        0     3623 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/rpctask.py
+-rw-rw-rw-   0        0        0     2112 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/smol.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.370196 lidia-0.8.1/src/lidia/static/
+-rw-rw-rw-   0        0        0     1761 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/LICENSE.txt
+-rw-rw-rw-   0        0        0    87008 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    87788 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    87592 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    86820 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    86908 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87076 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    87872 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0     7073 2022-12-09 17:51:17.000000 lidia-0.8.1/src/lidia/static/controls.js
+-rw-rw-rw-   0        0        0   121824 2022-06-02 22:10:07.000000 lidia-0.8.1/src/lidia/static/socket.io.js
+-rw-rw-rw-   0        0        0     1853 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/static/style.css
+drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.484624 lidia-0.8.1/src/lidia/utils/
+-rw-rw-rw-   0        0        0     3654 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/utils/pack_lidia.m
+-rw-rw-rw-   0        0        0    22361 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/utils/pack_maker.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.011333 lidia-0.8.1/src/lidia.egg-info/
+-rw-rw-rw-   0        0        0     2519 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1224 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/top_level.txt
```

### Comparing `lidia-0.8.0/LICENSE.txt` & `lidia-0.8.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Marek S. Łukasiewicz
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Marek S. Łukasiewicz
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `lidia-0.8.0/PKG-INFO` & `lidia-0.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-Metadata-Version: 2.1
-Name: lidia
-Version: 0.8.0
-Summary: serve an aircraft instruments panel as a web page
-Home-page: https://gitlab.com/Maarrk/lidia
-Author: Marek S. Lukasiewicz
-Author-email: marek@lukasiewicz.tech
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Lidia
-
-![lidia](https://img.shields.io/pypi/v/lidia)
-
-_Lightweight Instrument Display Interface for Aircraft_
-
-lidia is a Python package for serving an aircraft instruments panel as a web page.
-
-![screenshot of top part of primary flight display page](https://gitlab.com/Maarrk/lidia/-/raw/main/readme-pfd.png)
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [lidia](https://pypi.org/project/lidia/).
-
-```bash
-pip install lidia
-```
-
-## Usage
-
-```bash
-lidia demo
-
-# if your Scripts folder isn't in Path:
-python3 -m lidia demo
-
-# use other source
-lidia rpctask
-
-# show general help
-lidia --help
-
-# show help for a specific source
-lidia demo --help
-
-# pass the main server arguments before the source name
-lidia -P 5556 demo
-```
-
-Then open the served page in a browser, by default [localhost:5555](http://localhost:5555).
-The controls for showing and hiding elements of the GUI are shown when hovering the mouse in the bottom left region of the page.
-
-## Support
-
-Report problems in [GitLab Issues](https://gitlab.com/Maarrk/lidia/-/issues)
-
-## Roadmap
-
-- Additional PFD indicators: ILS, VOR on HSI
-- Ship approach screen with views from the side and behind
-- CAS (Crew Alerting System) screen
-- Simple second order aircraft models
-- USB HID joystick source
-
-## Contributing
-
-- Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
-- Python code should be formatted with autopep8
-- Other source files should be formatted with Prettier
-- Install packages for development with `pip install -r requirements.txt`
-- To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
-
-## Acknowledgements
-
-This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
-
-Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: lidia
+Version: 0.8.1
+Summary: serve an aircraft instruments panel as a web page
+Home-page: https://gitlab.com/Maarrk/lidia
+Author: Marek S. Lukasiewicz
+Author-email: marek@lukasiewicz.tech
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Lidia
+
+![lidia](https://img.shields.io/pypi/v/lidia)
+
+_Lightweight Instrument Display Interface for Aircraft_
+
+lidia is a Python package for serving an aircraft instruments panel as a web page.
+
+![screenshot of top part of primary flight display page](https://gitlab.com/Maarrk/lidia/-/raw/main/readme-pfd.png)
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [lidia](https://pypi.org/project/lidia/).
+
+```bash
+pip install lidia
+```
+
+## Usage
+
+```bash
+lidia demo
+
+# if your Scripts folder isn't in Path:
+python3 -m lidia demo
+
+# use other source
+lidia rpctask
+
+# show general help
+lidia --help
+
+# show help for a specific source
+lidia demo --help
+
+# pass the main server arguments before the source name
+lidia -P 5556 demo
+```
+
+Then open the served page in a browser, by default [localhost:5555](http://localhost:5555).
+The controls for showing and hiding elements of the GUI are shown when hovering the mouse in the bottom left region of the page.
+
+## Support
+
+Report problems in [GitLab Issues](https://gitlab.com/Maarrk/lidia/-/issues)
+
+## Roadmap
+
+- Additional PFD indicators: ILS, VOR on HSI
+- Ship approach screen with views from the side and behind
+- CAS (Crew Alerting System) screen
+- Simple second order aircraft models
+- USB HID joystick source
+
+## Contributing
+
+- Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
+- Python code should be formatted with autopep8
+- Other source files should be formatted with Prettier
+- Install packages for development with `pip install -r requirements.txt`
+- To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
+
+## Acknowledgements
+
+This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
+
+Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `lidia-0.8.0/README.md` & `lidia-0.8.1/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# Lidia
-
-![lidia](https://img.shields.io/pypi/v/lidia)
-
-_Lightweight Instrument Display Interface for Aircraft_
-
-lidia is a Python package for serving an aircraft instruments panel as a web page.
-
-![screenshot of top part of primary flight display page](https://gitlab.com/Maarrk/lidia/-/raw/main/readme-pfd.png)
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [lidia](https://pypi.org/project/lidia/).
-
-```bash
-pip install lidia
-```
-
-## Usage
-
-```bash
-lidia demo
-
-# if your Scripts folder isn't in Path:
-python3 -m lidia demo
-
-# use other source
-lidia rpctask
-
-# show general help
-lidia --help
-
-# show help for a specific source
-lidia demo --help
-
-# pass the main server arguments before the source name
-lidia -P 5556 demo
-```
-
-Then open the served page in a browser, by default [localhost:5555](http://localhost:5555).
-The controls for showing and hiding elements of the GUI are shown when hovering the mouse in the bottom left region of the page.
-
-## Support
-
-Report problems in [GitLab Issues](https://gitlab.com/Maarrk/lidia/-/issues)
-
-## Roadmap
-
-- Additional PFD indicators: ILS, VOR on HSI
-- Ship approach screen with views from the side and behind
-- CAS (Crew Alerting System) screen
-- Simple second order aircraft models
-- USB HID joystick source
-
-## Contributing
-
-- Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
-- Python code should be formatted with autopep8
-- Other source files should be formatted with Prettier
-- Install packages for development with `pip install -r requirements.txt`
-- To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
-
-## Acknowledgements
-
-This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
-
-Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+# Lidia
+
+![lidia](https://img.shields.io/pypi/v/lidia)
+
+_Lightweight Instrument Display Interface for Aircraft_
+
+lidia is a Python package for serving an aircraft instruments panel as a web page.
+
+![screenshot of top part of primary flight display page](https://gitlab.com/Maarrk/lidia/-/raw/main/readme-pfd.png)
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [lidia](https://pypi.org/project/lidia/).
+
+```bash
+pip install lidia
+```
+
+## Usage
+
+```bash
+lidia demo
+
+# if your Scripts folder isn't in Path:
+python3 -m lidia demo
+
+# use other source
+lidia rpctask
+
+# show general help
+lidia --help
+
+# show help for a specific source
+lidia demo --help
+
+# pass the main server arguments before the source name
+lidia -P 5556 demo
+```
+
+Then open the served page in a browser, by default [localhost:5555](http://localhost:5555).
+The controls for showing and hiding elements of the GUI are shown when hovering the mouse in the bottom left region of the page.
+
+## Support
+
+Report problems in [GitLab Issues](https://gitlab.com/Maarrk/lidia/-/issues)
+
+## Roadmap
+
+- Additional PFD indicators: ILS, VOR on HSI
+- Ship approach screen with views from the side and behind
+- CAS (Crew Alerting System) screen
+- Simple second order aircraft models
+- USB HID joystick source
+
+## Contributing
+
+- Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
+- Python code should be formatted with autopep8
+- Other source files should be formatted with Prettier
+- Install packages for development with `pip install -r requirements.txt`
+- To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
+
+## Acknowledgements
+
+This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
+
+Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `lidia-0.8.0/setup.cfg` & `lidia-0.8.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6c69 6469 610a 7665 7273 696f 6e20  = lidia.version 
-00000020: 3d20 6174 7472 3a20 6c69 6469 612e 5f5f  = attr: lidia.__
-00000030: 7665 7273 696f 6e5f 5f0a 6175 7468 6f72  version__.author
-00000040: 203d 204d 6172 656b 2053 2e20 4c75 6b61   = Marek S. Luka
-00000050: 7369 6577 6963 7a0a 6175 7468 6f72 5f65  siewicz.author_e
-00000060: 6d61 696c 203d 206d 6172 656b 406c 756b  mail = marek@luk
-00000070: 6173 6965 7769 637a 2e74 6563 680a 6465  asiewicz.tech.de
-00000080: 7363 7269 7074 696f 6e20 3d20 7365 7276  scription = serv
-00000090: 6520 616e 2061 6972 6372 6166 7420 696e  e an aircraft in
-000000a0: 7374 7275 6d65 6e74 7320 7061 6e65 6c20  struments panel 
-000000b0: 6173 2061 2077 6562 2070 6167 650a 6c6f  as a web page.lo
-000000c0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
-000000d0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
-000000e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000f0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000100: 2074 6578 742f 6d61 726b 646f 776e 0a75   text/markdown.u
-00000110: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000120: 6c61 622e 636f 6d2f 4d61 6172 726b 2f6c  lab.com/Maarrk/l
-00000130: 6964 6961 0a63 6c61 7373 6966 6965 7273  idia.classifiers
-00000140: 203d 200a 0950 726f 6772 616d 6d69 6e67   = ..Programming
-00000150: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000160: 686f 6e20 3a3a 2033 0a09 4c69 6365 6e73  hon :: 3..Licens
-00000170: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000180: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000190: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-000001a0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000001b0: 6465 6e74 0a0a 5b6f 7074 696f 6e73 5d0a  dent..[options].
-000001c0: 7061 636b 6167 655f 6469 7220 3d20 0a09  package_dir = ..
-000001d0: 3d20 7372 630a 7061 636b 6167 6573 203d  = src.packages =
-000001e0: 2066 696e 643a 0a70 7974 686f 6e5f 7265   find:.python_re
-000001f0: 7175 6972 6573 203d 203e 3d33 2e37 0a69  quires = >=3.7.i
-00000200: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000210: 3d20 0a09 6576 656e 746c 6574 207e 3d20  = ..eventlet ~= 
-00000220: 302e 3333 2e31 0a09 6d73 6770 6163 6b20  0.33.1..msgpack 
-00000230: 7e3d 2031 2e30 2e34 0a09 7079 6461 6e74  ~= 1.0.4..pydant
-00000240: 6963 207e 3d20 312e 3130 2e32 0a09 7079  ic ~= 1.10.2..py
-00000250: 7468 6f6e 2d73 6f63 6b65 7469 6f20 7e3d  thon-socketio ~=
-00000260: 2035 2e36 2e30 0a09 5079 5941 4d4c 207e   5.6.0..PyYAML ~
-00000270: 3d20 362e 300a 0974 6f6d 6c69 207e 3d20  = 6.0..tomli ~= 
-00000280: 322e 302e 310a 696e 636c 7564 655f 7061  2.0.1.include_pa
-00000290: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-000002a0: 650a 0a5b 6f70 7469 6f6e 732e 656e 7472  e..[options.entr
-000002b0: 795f 706f 696e 7473 5d0a 636f 6e73 6f6c  y_points].consol
-000002c0: 655f 7363 7269 7074 7320 3d20 0a09 6c69  e_scripts = ..li
-000002d0: 6469 6120 3d20 6c69 6469 612e 6c69 6469  dia = lidia.lidi
-000002e0: 613a 6d61 696e 0a0a 5b6f 7074 696f 6e73  a:main..[options
-000002f0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0a  .packages.find].
-00000300: 7768 6572 6520 3d20 7372 630a 0a5b 6567  where = src..[eg
-00000310: 675f 696e 666f 5d0a 7461 675f 6275 696c  g_info].tag_buil
-00000320: 6420 3d20 0a74 6167 5f64 6174 6520 3d20  d = .tag_date = 
-00000330: 300a 0a                                  0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206c 6964 6961 0d0a 7665 7273 696f   = lidia..versio
+00000020: 6e20 3d20 6174 7472 3a20 6c69 6469 612e  n = attr: lidia.
+00000030: 5f5f 7665 7273 696f 6e5f 5f0d 0a61 7574  __version__..aut
+00000040: 686f 7220 3d20 4d61 7265 6b20 532e 204c  hor = Marek S. L
+00000050: 756b 6173 6965 7769 637a 0d0a 6175 7468  ukasiewicz..auth
+00000060: 6f72 5f65 6d61 696c 203d 206d 6172 656b  or_email = marek
+00000070: 406c 756b 6173 6965 7769 637a 2e74 6563  @lukasiewicz.tec
+00000080: 680d 0a64 6573 6372 6970 7469 6f6e 203d  h..description =
+00000090: 2073 6572 7665 2061 6e20 6169 7263 7261   serve an aircra
+000000a0: 6674 2069 6e73 7472 756d 656e 7473 2070  ft instruments p
+000000b0: 616e 656c 2061 7320 6120 7765 6220 7061  anel as a web pa
+000000c0: 6765 0d0a 6c6f 6e67 5f64 6573 6372 6970  ge..long_descrip
+000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000e0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
+000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
+00000120: 7073 3a2f 2f67 6974 6c61 622e 636f 6d2f  ps://gitlab.com/
+00000130: 4d61 6172 726b 2f6c 6964 6961 0d0a 636c  Maarrk/lidia..cl
+00000140: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+00000150: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000160: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000170: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+00000180: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000190: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+000001a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+000001b0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+000001d0: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+000001e0: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
+000001f0: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+00000200: 7265 7175 6972 6573 203d 203e 3d33 2e37  requires = >=3.7
+00000210: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000220: 6573 203d 200d 0a09 6576 656e 746c 6574  es = ...eventlet
+00000230: 207e 3d20 302e 3333 2e31 0d0a 096d 7367   ~= 0.33.1...msg
+00000240: 7061 636b 207e 3d20 312e 302e 340d 0a09  pack ~= 1.0.4...
+00000250: 7079 6461 6e74 6963 207e 3d20 312e 3130  pydantic ~= 1.10
+00000260: 2e32 0d0a 0970 7974 686f 6e2d 736f 636b  .2...python-sock
+00000270: 6574 696f 207e 3d20 352e 362e 300d 0a09  etio ~= 5.6.0...
+00000280: 5079 5941 4d4c 207e 3d20 362e 300d 0a09  PyYAML ~= 6.0...
+00000290: 746f 6d6c 6920 7e3d 2032 2e30 2e31 0d0a  tomli ~= 2.0.1..
+000002a0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+000002b0: 6461 7461 203d 2054 7275 650d 0a0d 0a5b  data = True....[
+000002c0: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
+000002d0: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
+000002e0: 6372 6970 7473 203d 200d 0a09 6c69 6469  cripts = ...lidi
+000002f0: 6120 3d20 6c69 6469 612e 6c69 6469 613a  a = lidia.lidia:
+00000300: 6d61 696e 0d0a 0d0a 5b6f 7074 696f 6e73  main....[options
+00000310: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+00000320: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+00000330: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000340: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000350: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `lidia-0.8.0/src/lidia/aircraft.py` & `lidia-0.8.1/src/lidia/aircraft.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,357 +1,358 @@
-import json
-from math import cos, sin, sqrt
-from time import time
-from pydantic import BaseModel
-from typing import Any, Dict, List, Optional, Sequence
-
-from .config import Config as LidiaConfig
-from .mytypes import VectorModel, IntFlagModel
-
-
-class Attitude(VectorModel):
-    """Aircraft attitude applied in order: roll, pitch, yaw"""
-    roll: float = 0
-    """Rotation along longitudinal axis to the right, in radians"""
-    pitch: float = 0
-    """Rotation along lateral axis nose up, in radians"""
-    yaw: float = 0
-    """Rotation along vertical axis clockwise seen from above, in radians"""
-
-
-class XYZ(VectorModel):
-    """Vector in aircraft coordinate system"""
-    x: float = 0
-    """Longitudinal axis forward"""
-    y: float = 0
-    """Lateral axis to the right"""
-    z: float = 0
-    """Vertical axis downward"""
-
-
-class NED(VectorModel):
-    """Vector in local horizon coordinate system"""
-    north: float = 0
-    east: float = 0
-    down: float = 0
-
-
-class Controls(VectorModel):
-    stick_right: float = 0
-    """Control stick input to roll right, between -1 and 1"""
-    stick_pull: float = 0
-    """Control stick input to pitch up, between -1 and 1"""
-    throttle: float = 0
-    """Engine power input, between 0 and 1"""
-    pedals_right: float = 0
-    """Pedals input to yaw right, between -1 and 1"""
-    collective_up: float = 0
-    """Collective input to increase lift, between 0 and 1"""
-
-
-class Borders(BaseModel):
-    low = Controls.from_list([-1, -1, 0, -1, 0])
-    high = Controls.from_list([1, 1, 1, 1, 1])
-
-    def smol(self) -> Dict[str, Any]:
-        return {
-            'low': self.low.smol(),
-            'high': self.high.smol(),
-        }
-
-
-class Buttons(IntFlagModel):
-    cyc_ftr: bool = False
-    coll_ftr: bool = False
-
-
-class Instruments(BaseModel):
-    ias: float = 0
-    """Indicated airspeed"""
-    gs: Optional[float] = None
-    """Groundspeed"""
-    alt: float = 0
-    """Barometric altitude"""
-    qnh: Optional[float] = 1013
-    """Altimeter setting, None for STD"""
-    ralt: Optional[float] = None
-    """Radio altimeter"""
-
-
-class CASMessage(BaseModel):
-    msg_id: int
-    blinking: bool
-
-
-class CAS(BaseModel):
-    """Crew Alerting System state"""
-    msgs: List[CASMessage]
-
-
-class Transforms:
-    @staticmethod
-    def _matmul(matrix: Sequence[float], multiplicand: Sequence[float]) -> List[float]:
-        """Multiply 3x3 matrix by 3-element vector or 3x3 matrix"""
-        assert len(matrix) == 9
-        assert len(multiplicand) == 3 or len(multiplicand) == 9
-        if len(multiplicand) == 3:
-            m = matrix
-            x, y, z = multiplicand
-            return [
-                x * m[0] + y * m[1] + z * m[2],
-                x * m[3] + y * m[4] + z * m[5],
-                x * m[6] + y * m[7] + z * m[8],
-            ]
-        elif len(multiplicand) == 9:
-            m = matrix
-            n = multiplicand
-            # aut
-            return [
-                m[0] * n[0] + m[1] * n[3] + m[2] * n[6], m[0] * n[1] + m[1] * n[4] + m[2] * n[7], m[0] * n[2] + m[1] * n[5] + m[2] * n[8],  # noqa
-                m[3] * n[0] + m[4] * n[3] + m[5] * n[6], m[3] * n[1] + m[4] * n[4] + m[5] * n[7], m[3] * n[2] + m[4] * n[5] + m[5] * n[8],  # noqa
-                m[6] * n[0] + m[7] * n[3] + m[8] * n[6], m[6] * n[1] + m[7] * n[4] + m[8] * n[7], m[6] * n[2] + m[7] * n[5] + m[8] * n[8],  # noqa
-            ]
-        else:
-            raise RuntimeError('Unreachable, check assertions')
-
-    @staticmethod
-    def _transpose(matrix: Sequence[float]) -> List[float]:
-        """Transpose 3x3 matrix"""
-        assert len(matrix) == 9
-        m = matrix
-        return [
-            m[0], m[3], m[6],
-            m[1], m[4], m[7],
-            m[2], m[5], m[8],
-        ]
-
-    @staticmethod
-    def _rotmat(att: Attitude) -> List[float]:
-        """Create 3x3 rotation matrix transforming body-frame vectors to outside frame"""
-        s, c = sin(att.roll), cos(att.roll)
-        rot_roll = [
-            1, 0, 0,
-            0, c, -s,
-            0, s, c,
-        ]
-        s, c = sin(att.pitch), cos(att.pitch)
-        rot_pitch = [
-            c, 0, s,
-            0, 1, 0,
-            -s, 0, c
-        ]
-        s, c = sin(att.yaw), cos(att.yaw)
-        rot_yaw = [
-            c, -s, 0,
-            s, c, 0,
-            0, 0, 1
-        ]
-
-        return Transforms._matmul(rot_yaw, Transforms._matmul(rot_pitch, rot_roll))
-
-
-class AircraftData(BaseModel):
-    """Non-recursive state of displayed aircraft"""
-
-    ned: Optional[NED] = None
-    """Position in local horizon coordinate system, in meters"""
-    att: Optional[Attitude] = None
-    """Aircraft attitude, in radians"""
-    v_body: Optional[XYZ] = None
-    """Velocity in body frame, in meters per second"""
-    v_ned: Optional[NED] = None
-    """Velocity in local horizon coordinate system, in meters per second"""
-    a_body: Optional[XYZ] = None
-    """Accelerations measured (with gravity) in body frame, in meters per second squared"""
-    a_ned: Optional[NED] = None
-    """Acceleration measured in local horizon coordinate system, in meters per second squared"""
-    ctrl: Optional[Controls] = None
-    """Control inceptors position, normalized by max deflection"""
-    brdr: Optional[Borders] = None
-    """Task borders for inceptors"""
-    btn: Optional[Buttons] = None
-    """Pressed buttons"""
-    instr: Optional[Instruments] = None
-    """Instrument values"""
-    t_boot: Optional[int] = None
-    """Time from the start of simulation, in milliseconds"""
-
-    class Config:
-        json_encoders = {
-            VectorModel: VectorModel.smol,
-            Borders: Borders.smol,
-            IntFlagModel: IntFlagModel.smol,
-        }
-
-    def smol(self) -> Dict[str, Any]:
-        """Return self as dictionary with SMOL-defined keys"""
-        # HACK: JSON roundtrip is required, because there is no encoder configuration for .dict()
-        return json.loads(self.json(models_as_dict=False, exclude={f for f in self.__fields__ if (getattr(self, f) is None or f in ['trgt', 'trim'])}))
-
-    @classmethod
-    def from_smol(cls, smol: dict) -> 'AircraftData':
-        state = cls()
-        for name in ['ned', 'v_ned']:
-            if name in smol:
-                setattr(state, name, NED.from_list(smol[name]))
-        if 'att' in smol:
-            state.att = Attitude.from_list(smol['att'])
-        for name in ['v_body', 'a_body']:
-            if name in smol:
-                setattr(state, name, XYZ.from_list(smol[name]))
-        if 'ctrl' in smol:
-            state.ctrl = Controls.from_list(smol['ctrl'])
-        # TODO: Borders
-        if 'btn' in smol:
-            state.btn = Buttons.from_list(smol['btn'])
-        if 'instr' in smol:
-            state.instr = Instruments()
-            for name in ['ias', 'gs', 'alt', 'qnh', 'alt']:
-                if name in smol['instr']:
-                    setattr(state.instr, name, smol['instr'][name])
-        if 't_boot' in smol:
-            state.t_boot = smol['t_boot']
-
-        return state
-
-    def xyz2ned(self, vec: XYZ) -> NED:
-        """Transform from body frame vector to outside frame coordinates
-
-        Assumes no rotation if `self.att` is missing"""
-        if self.att is None:
-            return NED.from_list([vec.x, vec.y, vec.z])
-        else:
-            return NED.from_list(Transforms._matmul(Transforms._rotmat(self.att), [vec.x, vec.y, vec.z]))
-
-    def ned2xyz(self, vec: NED) -> XYZ:
-        """Transform from outside frame to body frame coordinates
-
-        Assumes no rotation if `self.att` is missing"""
-        if self.att is None:
-            return XYZ.from_list([vec.north, vec.east, vec.down])
-        else:
-            return XYZ.from_list(Transforms._matmul(Transforms._transpose(Transforms._rotmat(self.att)), [vec.north, vec.east, vec.down]))
-
-    def model_instruments(self, config: LidiaConfig):
-        """Generate values for instruments based on known parameters and configuration"""
-        self._model_ias(config)
-        self._model_gs(config)
-        self._model_alt(config)
-        self._model_ralt(config)
-
-        # rotate acceleration to XYZ for sideslip
-        if self.a_body is None and self.a_ned is not None:
-            self.a_body = self.ned2xyz(self.a_ned)
-
-    def _get_instr(self) -> Instruments:
-        if self.instr is None:
-            self.instr = Instruments()
-        return self.instr
-
-    def _model_ias(self, config: LidiaConfig) -> bool:
-        ias = None
-        if self.v_body is not None:
-            ias = self.v_body.x
-        elif self.v_ned is not None and self.att is not None:
-            v_body = self.ned2xyz(self.v_ned)
-            ias = v_body.x
-
-        if ias is not None:
-            self._get_instr().ias = ias * config.instruments.speed_multiplier
-            return True
-        return False
-
-    def _model_gs(self, config: LidiaConfig) -> bool:
-        gs = None
-        if self.v_ned is not None:
-            gs = sqrt(self.v_ned.north ** 2 + self.v_ned.east ** 2)
-        elif self.v_body is not None and self.att is not None:
-            v_ned = self.xyz2ned(self.v_body)
-            gs = sqrt(v_ned.north ** 2 + v_ned.east ** 2)
-
-        if gs is not None:
-            self._get_instr().gs = gs * config.instruments.speed_multiplier
-            return True
-        return False
-
-    def _model_alt(self, config: LidiaConfig) -> bool:
-        if self.ned is not None:
-            self._get_instr().alt = -self.ned.down * config.instruments.altitude_multiplier
-            return True
-        return False
-
-    def _model_ralt(self, config: LidiaConfig) -> bool:
-        if self.ned is not None:
-            if abs(self.ned.down) <= config.instruments.radio_altimeter_activation:
-                self._get_instr().ralt = -self.ned.down * config.instruments.altitude_multiplier
-                return True
-        return False
-
-    def set_time(self, config: LidiaConfig):
-        if config.start_time is not None:
-            self.t_boot = int((time() - config.start_time) * 1000)
-
-
-class AircraftState(AircraftData):
-    """Full aircraft state containing target and trim condition
-
-    Split from `AircraftData` to prevent recursive definition"""
-
-    trgt: Optional[AircraftData] = None
-    """Target values for pilot to track"""
-    trim: Optional[AircraftData] = None
-    """Trim values"""
-
-    def smol(self) -> Dict[str, Any]:
-        data = super().smol()
-        if self.trgt is not None:
-            data['trgt'] = self.trgt.smol()
-        if self.trim is not None:
-            data['trim'] = self.trim.smol()
-        return data
-
-    @classmethod
-    def from_smol(cls, smol: dict) -> 'AircraftState':
-        state = cls(**super().from_smol(smol).dict())
-        for name in ['trgt', 'trim']:
-            if name in smol:
-                # For backwards compatibility
-                if smol[name] is List:
-                    # TODO: Some warning when logging setup available
-                    smol[name] = {'ctrl': {name: smol[name]}}
-                setattr(state, name, AircraftData.from_smol(smol[name]))
-
-        return state
-
-
-if __name__ == '__main__':
-    # run this from src/ folder like this: python -m lidia.aircraft
-    import os
-
-    config = LidiaConfig()
-    state = AircraftState()
-    state.ned = NED.from_list([0.0, 0.0, 0.0])
-    state.att = Attitude.from_list([0.0, 0.0, 0.0])
-    state.v_body = XYZ.from_list([0.0, 0.0, 0.0])
-    state.v_ned = NED.from_list([0.0, 0.0, 0.0])
-    state.a_body = XYZ.from_list([0.0, 0.0, 0.0])
-    state.ctrl = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
-    state.trgt = AircraftData()
-    state.trgt.ctrl = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
-    state.t_boot = 0x10000000
-    state.model_instruments(config)
-    print(state.smol())
-    import msgpack
-    packer = msgpack.Packer(use_single_float=False)
-    data_double = packer.pack(state.smol())
-    packer = msgpack.Packer(use_single_float=True)
-    data_float = packer.pack(state.smol())
-    data = data_double[:0x21] + data_float[0x15:]
-    for i, b in enumerate(data):
-        print(f'0x{b:02X}, ', end='')
-    print()
-    os.makedirs('lidia/data', exist_ok=True)
-    with open('lidia/data/aircraft.bin', 'wb') as out:
-        out.write(data)
-    roundtrip = msgpack.unpackb(data)
-    print(roundtrip)
-    print(AircraftState.from_smol(roundtrip))
+import json
+from math import cos, sin, sqrt
+from time import time
+from pydantic import BaseModel
+from typing import Any, Dict, List, Optional, Sequence
+
+from .config import Config as LidiaConfig
+from .mytypes import VectorModel, IntFlagModel
+
+
+class Attitude(VectorModel):
+    """Aircraft attitude applied in order: roll, pitch, yaw"""
+    roll: float = 0
+    """Rotation along longitudinal axis to the right, in radians"""
+    pitch: float = 0
+    """Rotation along lateral axis nose up, in radians"""
+    yaw: float = 0
+    """Rotation along vertical axis clockwise seen from above, in radians"""
+
+
+class XYZ(VectorModel):
+    """Vector in aircraft coordinate system"""
+    x: float = 0
+    """Longitudinal axis forward"""
+    y: float = 0
+    """Lateral axis to the right"""
+    z: float = 0
+    """Vertical axis downward"""
+
+
+class NED(VectorModel):
+    """Vector in local horizon coordinate system"""
+    north: float = 0
+    east: float = 0
+    down: float = 0
+
+
+class Controls(VectorModel):
+    stick_right: float = 0
+    """Control stick input to roll right, between -1 and 1"""
+    stick_pull: float = 0
+    """Control stick input to pitch up, between -1 and 1"""
+    throttle: float = 0
+    """Engine power input, between 0 and 1"""
+    pedals_right: float = 0
+    """Pedals input to yaw right, between -1 and 1"""
+    collective_up: float = 0
+    """Collective input to increase lift, between 0 and 1"""
+
+
+class Borders(BaseModel):
+    low = Controls.from_list([-1, -1, 0, -1, 0])
+    high = Controls.from_list([1, 1, 1, 1, 1])
+
+    def smol(self) -> Dict[str, Any]:
+        return {
+            'low': self.low.smol(),
+            'high': self.high.smol(),
+        }
+
+
+class Buttons(IntFlagModel):
+    cyc_ftr: bool = False
+    coll_ftr: bool = False
+
+
+class Instruments(BaseModel):
+    ias: float = 0
+    """Indicated airspeed"""
+    gs: Optional[float] = None
+    """Groundspeed"""
+    alt: float = 0
+    """Barometric altitude"""
+    qnh: Optional[float] = 1013
+    """Altimeter setting, None for STD"""
+    ralt: Optional[float] = None
+    """Radio altimeter"""
+
+
+class CASMessage(BaseModel):
+    msg_id: int
+    blinking: bool
+
+
+class CAS(BaseModel):
+    """Crew Alerting System state"""
+    msgs: List[CASMessage]
+
+
+class Transforms:
+    @staticmethod
+    def _matmul(matrix: Sequence[float], multiplicand: Sequence[float]) -> List[float]:
+        """Multiply 3x3 matrix by 3-element vector or 3x3 matrix"""
+        assert len(matrix) == 9
+        assert len(multiplicand) == 3 or len(multiplicand) == 9
+        if len(multiplicand) == 3:
+            m = matrix
+            x, y, z = multiplicand
+            return [
+                x * m[0] + y * m[1] + z * m[2],
+                x * m[3] + y * m[4] + z * m[5],
+                x * m[6] + y * m[7] + z * m[8],
+            ]
+        elif len(multiplicand) == 9:
+            m = matrix
+            n = multiplicand
+            # aut
+            return [
+                m[0] * n[0] + m[1] * n[3] + m[2] * n[6], m[0] * n[1] + m[1] * n[4] + m[2] * n[7], m[0] * n[2] + m[1] * n[5] + m[2] * n[8],  # noqa
+                m[3] * n[0] + m[4] * n[3] + m[5] * n[6], m[3] * n[1] + m[4] * n[4] + m[5] * n[7], m[3] * n[2] + m[4] * n[5] + m[5] * n[8],  # noqa
+                m[6] * n[0] + m[7] * n[3] + m[8] * n[6], m[6] * n[1] + m[7] * n[4] + m[8] * n[7], m[6] * n[2] + m[7] * n[5] + m[8] * n[8],  # noqa
+            ]
+        else:
+            raise RuntimeError('Unreachable, check assertions')
+
+    @staticmethod
+    def _transpose(matrix: Sequence[float]) -> List[float]:
+        """Transpose 3x3 matrix"""
+        assert len(matrix) == 9
+        m = matrix
+        return [
+            m[0], m[3], m[6],
+            m[1], m[4], m[7],
+            m[2], m[5], m[8],
+        ]
+
+    @staticmethod
+    def _rotmat(att: Attitude) -> List[float]:
+        """Create 3x3 rotation matrix transforming body-frame vectors to outside frame"""
+        s, c = sin(att.roll), cos(att.roll)
+        rot_roll = [
+            1, 0, 0,
+            0, c, -s,
+            0, s, c,
+        ]
+        s, c = sin(att.pitch), cos(att.pitch)
+        rot_pitch = [
+            c, 0, s,
+            0, 1, 0,
+            -s, 0, c
+        ]
+        s, c = sin(att.yaw), cos(att.yaw)
+        rot_yaw = [
+            c, -s, 0,
+            s, c, 0,
+            0, 0, 1
+        ]
+
+        return Transforms._matmul(rot_yaw, Transforms._matmul(rot_pitch, rot_roll))
+
+
+class AircraftData(BaseModel):
+    """Non-recursive state of displayed aircraft"""
+
+    ned: Optional[NED] = None
+    """Position in local horizon coordinate system, in meters"""
+    att: Optional[Attitude] = None
+    """Aircraft attitude, in radians"""
+    v_body: Optional[XYZ] = None
+    """Velocity in body frame, in meters per second"""
+    v_ned: Optional[NED] = None
+    """Velocity in local horizon coordinate system, in meters per second"""
+    a_body: Optional[XYZ] = None
+    """Acceleration measured (with gravity) in body frame, in meters per second squared"""
+    a_ned: Optional[NED] = None
+    """Acceleration measured in local horizon coordinate system, in meters per second squared"""
+    ctrl: Optional[Controls] = None
+    """Control inceptors position, normalized by max deflection"""
+    brdr: Optional[Borders] = None
+    """Task borders for inceptors"""
+    btn: Optional[Buttons] = None
+    """Pressed buttons"""
+    instr: Optional[Instruments] = None
+    """Instrument values"""
+    t_boot: Optional[int] = None
+    """Time from the start of simulation, in milliseconds"""
+
+    class Config:
+        json_encoders = {
+            VectorModel: VectorModel.smol,
+            Borders: Borders.smol,
+            IntFlagModel: IntFlagModel.smol,
+        }
+
+    def smol(self) -> Dict[str, Any]:
+        """Return self as dictionary with SMOL-defined keys"""
+        # HACK: JSON roundtrip is required, because there is no encoder configuration for .dict()
+        return json.loads(self.json(models_as_dict=False, exclude={f for f in self.__fields__ if (getattr(self, f) is None or f in ['trgt', 'trim'])}))
+
+    @classmethod
+    def from_smol(cls, smol: dict) -> 'AircraftData':
+        state = cls()
+        for name in ['ned', 'v_ned', 'a_ned']:
+            if name in smol:
+                setattr(state, name, NED.from_list(smol[name]))
+        if 'att' in smol:
+            state.att = Attitude.from_list(smol['att'])
+        for name in ['v_body', 'a_body']:
+            if name in smol:
+                setattr(state, name, XYZ.from_list(smol[name]))
+        if 'ctrl' in smol:
+            state.ctrl = Controls.from_list(smol['ctrl'])
+        # TODO: Borders
+        if 'btn' in smol:
+            state.btn = Buttons.from_list(smol['btn'])
+        if 'instr' in smol:
+            state.instr = Instruments()
+            for name in ['ias', 'gs', 'alt', 'qnh', 'alt']:
+                if name in smol['instr']:
+                    setattr(state.instr, name, smol['instr'][name])
+        if 't_boot' in smol:
+            state.t_boot = smol['t_boot']
+
+        return state
+
+    def xyz2ned(self, vec: XYZ) -> NED:
+        """Transform from body frame vector to outside frame coordinates
+
+        Assumes no rotation if `self.att` is missing"""
+        if self.att is None:
+            return NED.from_list([vec.x, vec.y, vec.z])
+        else:
+            return NED.from_list(Transforms._matmul(Transforms._rotmat(self.att), [vec.x, vec.y, vec.z]))
+
+    def ned2xyz(self, vec: NED) -> XYZ:
+        """Transform from outside frame to body frame coordinates
+
+        Assumes no rotation if `self.att` is missing"""
+        if self.att is None:
+            return XYZ.from_list([vec.north, vec.east, vec.down])
+        else:
+            return XYZ.from_list(Transforms._matmul(Transforms._transpose(Transforms._rotmat(self.att)), [vec.north, vec.east, vec.down]))
+
+    def model_instruments(self, config: LidiaConfig):
+        """Generate values for instruments based on known parameters and configuration"""
+        self._model_ias(config)
+        self._model_gs(config)
+        self._model_alt(config)
+        self._model_ralt(config)
+
+        # rotate acceleration to XYZ for sideslip
+        if self.a_body is None and self.a_ned is not None:
+            self.a_body = self.ned2xyz(self.a_ned)
+
+    def _get_instr(self) -> Instruments:
+        if self.instr is None:
+            self.instr = Instruments()
+        return self.instr
+
+    def _model_ias(self, config: LidiaConfig) -> bool:
+        ias = None
+        if self.v_body is not None:
+            ias = self.v_body.x
+        elif self.v_ned is not None and self.att is not None:
+            v_body = self.ned2xyz(self.v_ned)
+            ias = v_body.x
+
+        if ias is not None:
+            self._get_instr().ias = ias * config.instruments.speed_multiplier
+            return True
+        return False
+
+    def _model_gs(self, config: LidiaConfig) -> bool:
+        gs = None
+        if self.v_ned is not None:
+            gs = sqrt(self.v_ned.north ** 2 + self.v_ned.east ** 2)
+        elif self.v_body is not None and self.att is not None:
+            v_ned = self.xyz2ned(self.v_body)
+            gs = sqrt(v_ned.north ** 2 + v_ned.east ** 2)
+
+        if gs is not None:
+            self._get_instr().gs = gs * config.instruments.speed_multiplier
+            return True
+        return False
+
+    def _model_alt(self, config: LidiaConfig) -> bool:
+        if self.ned is not None:
+            self._get_instr().alt = -self.ned.down * config.instruments.altitude_multiplier
+            return True
+        return False
+
+    def _model_ralt(self, config: LidiaConfig) -> bool:
+        if self.ned is not None:
+            if abs(self.ned.down) <= config.instruments.radio_altimeter_activation:
+                self._get_instr().ralt = -self.ned.down * config.instruments.altitude_multiplier
+                return True
+        return False
+
+    def set_time(self, config: LidiaConfig):
+        if config.start_time is not None:
+            self.t_boot = int((time() - config.start_time) * 1000)
+
+
+class AircraftState(AircraftData):
+    """Full aircraft state containing target and trim condition
+
+    Split from `AircraftData` to prevent recursive definition"""
+
+    trgt: Optional[AircraftData] = None
+    """Target values for pilot to track"""
+    trim: Optional[AircraftData] = None
+    """Trim values"""
+
+    def smol(self) -> Dict[str, Any]:
+        data = super().smol()
+        if self.trgt is not None:
+            data['trgt'] = self.trgt.smol()
+        if self.trim is not None:
+            data['trim'] = self.trim.smol()
+        return data
+
+    @classmethod
+    def from_smol(cls, smol: dict) -> 'AircraftState':
+        state = cls(**super().from_smol(smol).dict())
+        for name in ['trgt', 'trim']:
+            if name in smol:
+                # For backwards compatibility
+                if smol[name] is List:
+                    # TODO: Some warning when logging setup available
+                    smol[name] = {'ctrl': {name: smol[name]}}
+                setattr(state, name, AircraftData.from_smol(smol[name]))
+
+        return state
+
+
+if __name__ == '__main__':
+    # run this from src/ folder like this: python -m lidia.aircraft
+    import os
+
+    config = LidiaConfig()
+    state = AircraftState()
+    state.ned = NED.from_list([0.0, 0.0, 0.0])
+    state.att = Attitude.from_list([0.0, 0.0, 0.0])
+    state.v_body = XYZ.from_list([0.0, 0.0, 0.0])
+    state.v_ned = NED.from_list([0.0, 0.0, 0.0])
+    state.a_body = XYZ.from_list([0.0, 0.0, 0.0])
+    state.a_ned = NED.from_list([0.0, 0.0, 0.0])
+    state.ctrl = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
+    state.trgt = AircraftData()
+    state.trgt.ctrl = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
+    state.t_boot = 0x10000000
+    state.model_instruments(config)
+    print(state.smol())
+    import msgpack
+    packer = msgpack.Packer(use_single_float=False)
+    data_double = packer.pack(state.smol())
+    packer = msgpack.Packer(use_single_float=True)
+    data_float = packer.pack(state.smol())
+    data = data_double[:0x21] + data_float[0x15:]
+    for i, b in enumerate(data):
+        print(f'0x{b:02X}, ', end='')
+    print()
+    os.makedirs('lidia/data', exist_ok=True)
+    with open('lidia/data/aircraft.bin', 'wb') as out:
+        out.write(data)
+    roundtrip = msgpack.unpackb(data)
+    print(roundtrip)
+    print(AircraftState.from_smol(roundtrip))
```

### Comparing `lidia-0.8.0/src/lidia/approach.html` & `lidia-0.8.1/src/lidia/approach.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-<!DOCTYPE html>
-<html>
-
-<head>
-  <title>Lidia Ship Approach</title>
-  <link rel="stylesheet" href="static/style.css" />
-  <script src="static/socket.io.js"></script>
-</head>
-
-<body>
-  <svg id="mainSvg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2200 1200" preserveAspectRatio="xMidYMid meet">
-    <g id="minimalRegion" data-extents="300 1400 900 800"></g>
-    <g id="horizontalRegion" data-extents="-100 2200 1300 -200"></g>
-    <g id="squareRegion" data-extents="-600 2300 1800 -100"></g>
-    <g transform="translate(1100 600)" fill="none">
-      <g transform="scale(10)" stroke="white">
-        <g id="helideck" transform="translate(0 0)" stroke-width="0.5">
-          <path d="M-120 -30 l40 -20 h180 v100 h-180 l-40 -20 z M-120 -30 l220 55 M-120 30 l220 -55 M50 -50 v100" />
-          <circle cx="0" cy="0" r="20" />
-        </g>
-      </g>
-      <g id="aircraft" class="aircraft" stroke-width="10" stroke="var(--pfdGreen)">
-        <path d="M-200 0 h100 M200 0 h-100 M0 200 v-100 M-30 0 h60 M0 -30 v60 M0 -195 l-60 100 h120 z" />
-        <circle cx="0" cy="0" r="200" />
-      </g>
-    </g>
-  </svg>
-
-  <script src="static/controls.js"></script>
-  <script type="text/javascript">
-    let svgElem = document.getElementById("mainSvg");
-    addControls(svgElem);
-  </script>
-
-  <script type="text/javascript">
-    var socket = io();
-
-    socket.on("echo", (s) => {
-      console.log(s);
-    });
-  </script>
-
-  <script type="text/javascript">
-    var socket = io();
-    var config = {
-      approach: {
-        nominal_alt: 3,
-        camera_height: 10,
-      }
-    };
-
-    function degrees(radians) {
-      return radians * 180 / Math.PI;
-    }
-
-    function radians(degrees) {
-      return degrees * Math.PI / 180;
-    }
-
-    function errorFill(difference) {
-      var e = Math.abs(difference);
-      if (e <= 0.03) return "#0f0";
-      else if (e <= 0.05) return "#ff0";
-      else return "#f00";
-    }
-
-    function limitRange(elem, oneSided = false) {
-      const outsideLimit = 10;
-      let rangeMin = oneSided ? 0 : -500;
-      let rangeMax = oneSided ? 1000 : 500;
-      let x = elem.transform.baseVal.getItem(0).matrix.e;
-      let y = elem.transform.baseVal.getItem(0).matrix.f;
-
-      // Clamp translate
-      elem.transform.baseVal.getItem(0).matrix.e = Math.max(
-        rangeMin - outsideLimit,
-        Math.min(rangeMax + outsideLimit, x)
-      );
-      elem.transform.baseVal.getItem(0).matrix.f = Math.max(
-        rangeMin - outsideLimit,
-        Math.min(rangeMax + outsideLimit, y)
-      );
-
-      let inside = x >= rangeMin && x <= rangeMax && y >= rangeMin && y <= rangeMax;
-      elem.style.stroke = inside ? "inherit" : "#f00";
-    }
-
-    const helideck = document.getElementById("helideck");
-    const initialStroke = helideck.getAttribute('stroke-width');
-    function updateDeck(s) {
-      let alt = -s.ned[2]; // Altitude above deck in meters
-      let scale = (config.approach.nominal_alt + config.approach.camera_height) / (alt + config.approach.camera_height);
-      let yaw = 0;
-      if ("att" in s) {
-        yaw = degrees(s.att[2]);
-      }
-      helideck.setAttribute("transform", `rotate(${-yaw}) scale(${scale}) translate(${-s.ned[1]} ${s.ned[0]})`);
-      helideck.setAttribute("stroke-width", initialStroke / scale);
-    }
-
-    socket.on("smol", (s) => {
-      if ("ned" in s) updateDeck(s);
-    });
-    socket.on("config", (s) => {
-      config = s;
-    });
-    socket.emit("config_request", {});
-  </script>
-
-</body>
-
+<!DOCTYPE html>
+<html>
+
+<head>
+  <title>Lidia Ship Approach</title>
+  <link rel="stylesheet" href="static/style.css" />
+  <script src="static/socket.io.js"></script>
+</head>
+
+<body>
+  <svg id="mainSvg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2200 1200" preserveAspectRatio="xMidYMid meet">
+    <g id="minimalRegion" data-extents="300 1400 900 800"></g>
+    <g id="horizontalRegion" data-extents="-100 2200 1300 -200"></g>
+    <g id="squareRegion" data-extents="-600 2300 1800 -100"></g>
+    <g transform="translate(1100 600)" fill="none">
+      <g transform="scale(10)" stroke="white">
+        <g id="helideck" transform="translate(0 0)" stroke-width="0.5">
+          <path d="M-120 -30 l40 -20 h180 v100 h-180 l-40 -20 z M-120 -30 l220 55 M-120 30 l220 -55 M50 -50 v100" />
+          <circle cx="0" cy="0" r="20" />
+        </g>
+      </g>
+      <g id="aircraft" class="aircraft" stroke-width="10" stroke="var(--pfdGreen)">
+        <path d="M-200 0 h100 M200 0 h-100 M0 200 v-100 M-30 0 h60 M0 -30 v60 M0 -195 l-60 100 h120 z" />
+        <circle cx="0" cy="0" r="200" />
+      </g>
+    </g>
+  </svg>
+
+  <script src="static/controls.js"></script>
+  <script type="text/javascript">
+    let svgElem = document.getElementById("mainSvg");
+    addControls(svgElem);
+  </script>
+
+  <script type="text/javascript">
+    var socket = io();
+
+    socket.on("echo", (s) => {
+      console.log(s);
+    });
+  </script>
+
+  <script type="text/javascript">
+    var socket = io();
+    var config = {
+      approach: {
+        nominal_alt: 3,
+        camera_height: 10,
+      }
+    };
+
+    function degrees(radians) {
+      return radians * 180 / Math.PI;
+    }
+
+    function radians(degrees) {
+      return degrees * Math.PI / 180;
+    }
+
+    function errorFill(difference) {
+      var e = Math.abs(difference);
+      if (e <= 0.03) return "#0f0";
+      else if (e <= 0.05) return "#ff0";
+      else return "#f00";
+    }
+
+    function limitRange(elem, oneSided = false) {
+      const outsideLimit = 10;
+      let rangeMin = oneSided ? 0 : -500;
+      let rangeMax = oneSided ? 1000 : 500;
+      let x = elem.transform.baseVal.getItem(0).matrix.e;
+      let y = elem.transform.baseVal.getItem(0).matrix.f;
+
+      // Clamp translate
+      elem.transform.baseVal.getItem(0).matrix.e = Math.max(
+        rangeMin - outsideLimit,
+        Math.min(rangeMax + outsideLimit, x)
+      );
+      elem.transform.baseVal.getItem(0).matrix.f = Math.max(
+        rangeMin - outsideLimit,
+        Math.min(rangeMax + outsideLimit, y)
+      );
+
+      let inside = x >= rangeMin && x <= rangeMax && y >= rangeMin && y <= rangeMax;
+      elem.style.stroke = inside ? "inherit" : "#f00";
+    }
+
+    const helideck = document.getElementById("helideck");
+    const initialStroke = helideck.getAttribute('stroke-width');
+    function updateDeck(s) {
+      let alt = -s.ned[2]; // Altitude above deck in meters
+      let scale = (config.approach.nominal_alt + config.approach.camera_height) / (alt + config.approach.camera_height);
+      let yaw = 0;
+      if ("att" in s) {
+        yaw = degrees(s.att[2]);
+      }
+      helideck.setAttribute("transform", `rotate(${-yaw}) scale(${scale}) translate(${-s.ned[1]} ${s.ned[0]})`);
+      helideck.setAttribute("stroke-width", initialStroke / scale);
+    }
+
+    socket.on("smol", (s) => {
+      if ("ned" in s) updateDeck(s);
+    });
+    socket.on("config", (s) => {
+      config = s;
+    });
+    socket.emit("config_request", {});
+  </script>
+
+</body>
+
 </html>
```

### Comparing `lidia-0.8.0/src/lidia/cas.html` & `lidia-0.8.1/src/lidia/cas.html`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-<!DOCTYPE html>
-<html>
-
-<head>
-  <title>Lidia CAS</title>
-  <link rel="stylesheet" href="static/style.css" />
-  <script src="static/socket.io.js"></script>
-  <style>
-    h2 {
-      font-size: x-large;
-      text-transform: uppercase;
-      border-bottom: 0.2em solid;
-    }
-
-    ul {
-      list-style: none;
-    }
-
-    li {
-      font-size: larger;
-      text-transform: uppercase;
-      margin-bottom: 0.5em;
-    }
-
-    .container {
-      margin: 0em 2em;
-    }
-
-    .inactive {
-      opacity: 0.5;
-    }
-
-    .warning {
-      color: var(--pfdRed);
-    }
-
-    .warningHighlight {
-      color: white;
-      background-color: var(--pfdRed);
-    }
-
-    .caution {
-      color: var(--pfdAmber);
-    }
-
-    .cautionHighlight {
-      color: black;
-      background-color: var(--pfdAmber);
-    }
-
-    .advisory {
-      color: var(--pfdCyan);
-    }
-
-    .advisoryHighlight {
-      color: white;
-      background-color: var(--pfdCyan);
-    }
-
-    .status {
-      color: white;
-    }
-
-    .statusHighlight {
-      color: black;
-      background-color: white;
-    }
-
-    .button {
-      padding: 0.5em;
-      font-size: 2em;
-      font-weight: 700;
-    }
-  </style>
-</head>
-
-<body>
-  <div class="container">
-    <div class="warning">
-      <h2>Warning</h2>
-      <ul id="warningList"></ul>
-    </div>
-    <div class="caution">
-      <h2>Caution</h2>
-      <ul id="cautionList"></ul>
-    </div>
-    <div class="advisory">
-      <h2>Advisory</h2>
-      <ul id="advisoryList"></ul>
-    </div>
-    <div class="status">
-      <h2>Status</h2>
-      <ul id="statusList"></ul>
-    </div>
-    <!-- Sending from browser to source would complicate a lot, disabled for now -->
-    <!-- <button id="ackButton" class="button">ACK</button> -->
-  </div>
-
-  <script type="text/javascript">
-    var socket = io();
-
-    socket.on("echo", (s) => {
-      console.log(s);
-    });
-  </script>
-
-  <script type="text/javascript">
-    var socket = io();
-    var config = {
-      cas: {
-        // Default events for development, this is replaced with configured events list, even if it is empty
-        events: {
-          101: { category: 1, text: "Require immediate flight crew awareness and response" },
-          102: { category: 2, text: "Require immediate flight crew awareness and subsequent response" },
-          103: { category: 3, text: "Require flight crew awareness and a possible future response" },
-          104: { category: 4, text: "Other operational status" },
-        }
-      }
-    };
-
-    const listElems = {
-      1: document.getElementById("warningList"),
-      2: document.getElementById("cautionList"),
-      3: document.getElementById("advisoryList"),
-      4: document.getElementById("statusList"),
-    };
-    function updateEvents(cas) {
-      let items = { 1: [], 2: [], 3: [], 4: [] };
-      for (const msg of cas.msgs) {
-        let msg_id = msg[0];
-        let blinking = msg[1];
-
-        let event = config.cas.events[msg_id];
-        if (event === undefined) {
-          console.error(`CAS event with id '${msg_id}' not found in configuration`);
-          continue;
-        }
-
-        let elem = document.createElement("li");
-        elem.textContent = event.text;
-        elem.dataset.category = event.category;
-        if (blinking) elem.classList.add("blinking");
-        items[event.category].push(elem);
-      }
-
-      for (let i = 1; i <= 4; i++) {
-        listElems[i].replaceChildren(...items[i]);
-      }
-    }
-
-    // // Sending from browser to source would complicate a lot, disabled for now
-    // function clickAck(event) {
-    //   socket.emit("input", { "cas": "ack" });
-    // }
-    // document.getElementById("ackButton").addEventListener("click", clickAck);
-
-    const highlightClasses = {
-      1: "warningHighlight",
-      2: "cautionHighlight",
-      3: "advisoryHighlight",
-      4: "statusHighlight",
-    }
-    var blinkingHighlight = false;
-    function toggleBlink() {
-      blinkingHighlight = !blinkingHighlight;
-      let blinkingElems = document.getElementsByClassName('blinking');
-      for (const elem of blinkingElems) {
-        let highlightClass = highlightClasses[elem.dataset.category];
-
-        if (blinkingHighlight) {
-          elem.classList.add(highlightClass);
-        } else {
-          elem.classList.remove(highlightClass);
-        }
-      }
-    }
-    setInterval(toggleBlink, 500);
-
-    socket.on("smol", (s) => {
-      if ("cas" in s) updateEvents(s.cas);
-    });
-    socket.on("config", (s) => {
-      config = s;
-    });
-    socket.emit("config_request", {});
-
-    // Testing only
-    updateEvents({ msgs: [] });
-    setTimeout(() => updateEvents({ msgs: [[101, true], [102, true]] }), 2000);
-    setTimeout(() => updateEvents({ msgs: [[101, false], [102, true]] }), 5000);
-    setTimeout(() => updateEvents({ msgs: [[101, false], [102, false]] }), 10000);
-    setTimeout(() => updateEvents({ msgs: [[102, false], [103, true]] }), 12000);
-    setTimeout(() => updateEvents({ msgs: [[102, false], [103, false]] }), 17000);
-    setTimeout(() => updateEvents({ msgs: [[102, false], [103, false], [104, false]] }), 22000);
-  </script>
-
-</body>
-
+<!DOCTYPE html>
+<html>
+
+<head>
+  <title>Lidia CAS</title>
+  <link rel="stylesheet" href="static/style.css" />
+  <script src="static/socket.io.js"></script>
+  <style>
+    h2 {
+      font-size: x-large;
+      text-transform: uppercase;
+      border-bottom: 0.2em solid;
+    }
+
+    ul {
+      list-style: none;
+    }
+
+    li {
+      font-size: larger;
+      text-transform: uppercase;
+      margin-bottom: 0.5em;
+    }
+
+    .container {
+      margin: 0em 2em;
+    }
+
+    .inactive {
+      opacity: 0.5;
+    }
+
+    .warning {
+      color: var(--pfdRed);
+    }
+
+    .warningHighlight {
+      color: white;
+      background-color: var(--pfdRed);
+    }
+
+    .caution {
+      color: var(--pfdAmber);
+    }
+
+    .cautionHighlight {
+      color: black;
+      background-color: var(--pfdAmber);
+    }
+
+    .advisory {
+      color: var(--pfdCyan);
+    }
+
+    .advisoryHighlight {
+      color: white;
+      background-color: var(--pfdCyan);
+    }
+
+    .status {
+      color: white;
+    }
+
+    .statusHighlight {
+      color: black;
+      background-color: white;
+    }
+
+    .button {
+      padding: 0.5em;
+      font-size: 2em;
+      font-weight: 700;
+    }
+  </style>
+</head>
+
+<body>
+  <div class="container">
+    <div class="warning">
+      <h2>Warning</h2>
+      <ul id="warningList"></ul>
+    </div>
+    <div class="caution">
+      <h2>Caution</h2>
+      <ul id="cautionList"></ul>
+    </div>
+    <div class="advisory">
+      <h2>Advisory</h2>
+      <ul id="advisoryList"></ul>
+    </div>
+    <div class="status">
+      <h2>Status</h2>
+      <ul id="statusList"></ul>
+    </div>
+    <!-- Sending from browser to source would complicate a lot, disabled for now -->
+    <!-- <button id="ackButton" class="button">ACK</button> -->
+  </div>
+
+  <script type="text/javascript">
+    var socket = io();
+
+    socket.on("echo", (s) => {
+      console.log(s);
+    });
+  </script>
+
+  <script type="text/javascript">
+    var socket = io();
+    var config = {
+      cas: {
+        // Default events for development, this is replaced with configured events list, even if it is empty
+        events: {
+          101: { category: 1, text: "Require immediate flight crew awareness and response" },
+          102: { category: 2, text: "Require immediate flight crew awareness and subsequent response" },
+          103: { category: 3, text: "Require flight crew awareness and a possible future response" },
+          104: { category: 4, text: "Other operational status" },
+        }
+      }
+    };
+
+    const listElems = {
+      1: document.getElementById("warningList"),
+      2: document.getElementById("cautionList"),
+      3: document.getElementById("advisoryList"),
+      4: document.getElementById("statusList"),
+    };
+    function updateEvents(cas) {
+      let items = { 1: [], 2: [], 3: [], 4: [] };
+      for (const msg of cas.msgs) {
+        let msg_id = msg[0];
+        let blinking = msg[1];
+
+        let event = config.cas.events[msg_id];
+        if (event === undefined) {
+          console.error(`CAS event with id '${msg_id}' not found in configuration`);
+          continue;
+        }
+
+        let elem = document.createElement("li");
+        elem.textContent = event.text;
+        elem.dataset.category = event.category;
+        if (blinking) elem.classList.add("blinking");
+        items[event.category].push(elem);
+      }
+
+      for (let i = 1; i <= 4; i++) {
+        listElems[i].replaceChildren(...items[i]);
+      }
+    }
+
+    // // Sending from browser to source would complicate a lot, disabled for now
+    // function clickAck(event) {
+    //   socket.emit("input", { "cas": "ack" });
+    // }
+    // document.getElementById("ackButton").addEventListener("click", clickAck);
+
+    const highlightClasses = {
+      1: "warningHighlight",
+      2: "cautionHighlight",
+      3: "advisoryHighlight",
+      4: "statusHighlight",
+    }
+    var blinkingHighlight = false;
+    function toggleBlink() {
+      blinkingHighlight = !blinkingHighlight;
+      let blinkingElems = document.getElementsByClassName('blinking');
+      for (const elem of blinkingElems) {
+        let highlightClass = highlightClasses[elem.dataset.category];
+
+        if (blinkingHighlight) {
+          elem.classList.add(highlightClass);
+        } else {
+          elem.classList.remove(highlightClass);
+        }
+      }
+    }
+    setInterval(toggleBlink, 500);
+
+    socket.on("smol", (s) => {
+      if ("cas" in s) updateEvents(s.cas);
+    });
+    socket.on("config", (s) => {
+      config = s;
+    });
+    socket.emit("config_request", {});
+
+    // Testing only
+    updateEvents({ msgs: [] });
+    setTimeout(() => updateEvents({ msgs: [[101, true], [102, true]] }), 2000);
+    setTimeout(() => updateEvents({ msgs: [[101, false], [102, true]] }), 5000);
+    setTimeout(() => updateEvents({ msgs: [[101, false], [102, false]] }), 10000);
+    setTimeout(() => updateEvents({ msgs: [[102, false], [103, true]] }), 12000);
+    setTimeout(() => updateEvents({ msgs: [[102, false], [103, false]] }), 17000);
+    setTimeout(() => updateEvents({ msgs: [[102, false], [103, false], [104, false]] }), 22000);
+  </script>
+
+</body>
+
 </html>
```

### Comparing `lidia-0.8.0/src/lidia/config.py` & `lidia-0.8.1/src/lidia/config.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from enum import Enum
-import os
-from os import path
-from typing import Dict, Optional
-from pydantic import Field
-
-from .mytypes import NestingModel
-
-
-class RpctaskConfig(NestingModel):
-    """Configuration for `rpctask`"""
-    correct_tolerance: float = 0.03
-    """Acceptable margin for green color"""
-    warning_tolerance: float = 0.05
-    """Acceptable margin for yellow color"""
-
-
-class PfdConfig(NestingModel):
-    """configuration for `pfd`"""
-    ias_never_exceed: float = 167.0
-    """Never exceed speed (Vne) shown on IAS tape"""
-    show_adi_target: bool = True
-    """Display the attitude target after receiving trgt.att"""
-    adi_target_roll: bool = True
-    """Rotate attitude target indicator to show desired roll"""
-    adi_target_yaw: bool = False
-    """Move attitude target indicator to show desired yaw"""
-    show_flightpath: bool = True
-    """Show flightpath vector (FPV) indicator on ADI"""
-    show_retrograde: bool = False
-    """Show reverse flight path vector on ADI"""
-    move_roll_ticks: bool = False
-    """Move roll angle scale with horizon, keeping sideslip triangle in place"""
-    sideslip_max: float = 15.0
-    """Maximal displayed sideslip angle, in degrees"""
-
-
-class ApproachConfig(NestingModel):
-    """Ship approach configuration"""
-    nominal_alt: float = 3
-    """Altitude at which the scale is 1, in meters"""
-    camera_height: float = 10
-    """Position of camera above aircraft origin, in meters
-
-    Larger values of this make the scale change less drastically at low altitude"""
-
-
-class InstrumentsConfig(NestingModel):
-    """Configuration for instruments visualisation, units etc."""
-    speed_multiplier: float = 3600.0 / 1852.0
-    """Scaling factor to change state velocity in meters per second to displayed IAS and GS, default for knots"""
-    altitude_multiplier: float = 1 / 0.3048
-    """Scaling factor to change state altitude in meters to displayed altitude, default for feet"""
-    radio_altimeter_activation: float = 2500.0 * 0.3048
-    """Activation height of radio altimeter above which it is not modeled, default 2500ft"""
-
-
-class CASCategory(Enum):
-    """Category (severity, type) of a message shown in CAS"""
-    WARNING = 1
-    """Red, blinking until acknowledged"""
-    CAUTION = 2
-    """Amber, blinking until acknowledged"""
-    ADVISORY = 3
-    """Green, blinking for a fixed time"""
-    STATUS = 4
-    """White messages"""
-
-
-class CASEvent(NestingModel):
-    """Event that can be displayed in CAS"""
-    category: CASCategory
-    """Category to put the message into"""
-    text: str
-    """Text to be shown"""
-
-
-class CASConfig(NestingModel):
-    """Configuration for Crew Alerting System, including events"""
-    events: Dict[int, CASEvent] = {}
-    """Dictionary of events by their integer id"""
-
-
-class Config(NestingModel):
-    """Root of configuration structure
-
-    Every config field in this and children should be provided with defaults,
-    that can be overriden by config files"""
-
-    json_schema_url: Optional[str] = Field(alias='$schema', default=None)
-    """Allow the `$schema` property for specifying JSON Schema URL"""
-    rpctask = RpctaskConfig()
-    pfd = PfdConfig()
-    approach = ApproachConfig()
-    instruments = InstrumentsConfig()
-    cas = CASConfig()
-    start_time: Optional[float] = None
-    """Epoch time in seconds of starting the program (see `time.time()`)"""
-
-
-def schema_location():
-    root_path = path.abspath(path.dirname(__file__))
-    data_path = path.join(root_path, 'data')
-    os.makedirs(data_path, exist_ok=True)
-    return path.join(data_path, 'lidia-config.json')
-
-
-def write_schema():
-    with open(schema_location(), 'w') as out:
-        out.write(Config.schema_json(by_alias=True))
+from enum import Enum
+import os
+from os import path
+from typing import Dict, Optional
+from pydantic import Field
+
+from .mytypes import NestingModel
+
+
+class RpctaskConfig(NestingModel):
+    """Configuration for `rpctask`"""
+    correct_tolerance: float = 0.03
+    """Acceptable margin for green color"""
+    warning_tolerance: float = 0.05
+    """Acceptable margin for yellow color"""
+
+
+class PfdConfig(NestingModel):
+    """configuration for `pfd`"""
+    ias_never_exceed: float = 167.0
+    """Never exceed speed (Vne) shown on IAS tape"""
+    show_adi_target: bool = True
+    """Display the attitude target after receiving trgt.att"""
+    adi_target_roll: bool = True
+    """Rotate attitude target indicator to show desired roll"""
+    adi_target_yaw: bool = False
+    """Move attitude target indicator to show desired yaw"""
+    show_flightpath: bool = True
+    """Show flightpath vector (FPV) indicator on ADI"""
+    show_retrograde: bool = False
+    """Show reverse flight path vector on ADI"""
+    move_roll_ticks: bool = False
+    """Move roll angle scale with horizon, keeping sideslip triangle in place"""
+    sideslip_max: float = 15.0
+    """Maximal displayed sideslip angle, in degrees"""
+
+
+class ApproachConfig(NestingModel):
+    """Ship approach configuration"""
+    nominal_alt: float = 3
+    """Altitude at which the scale is 1, in meters"""
+    camera_height: float = 10
+    """Position of camera above aircraft origin, in meters
+
+    Larger values of this make the scale change less drastically at low altitude"""
+
+
+class InstrumentsConfig(NestingModel):
+    """Configuration for instruments visualisation, units etc."""
+    speed_multiplier: float = 3600.0 / 1852.0
+    """Scaling factor to change state velocity in meters per second to displayed IAS and GS, default for knots"""
+    altitude_multiplier: float = 1 / 0.3048
+    """Scaling factor to change state altitude in meters to displayed altitude, default for feet"""
+    radio_altimeter_activation: float = 2500.0 * 0.3048
+    """Activation height of radio altimeter above which it is not modeled, default 2500ft"""
+
+
+class CASCategory(Enum):
+    """Category (severity, type) of a message shown in CAS"""
+    WARNING = 1
+    """Red, blinking until acknowledged"""
+    CAUTION = 2
+    """Amber, blinking until acknowledged"""
+    ADVISORY = 3
+    """Green, blinking for a fixed time"""
+    STATUS = 4
+    """White messages"""
+
+
+class CASEvent(NestingModel):
+    """Event that can be displayed in CAS"""
+    category: CASCategory
+    """Category to put the message into"""
+    text: str
+    """Text to be shown"""
+
+
+class CASConfig(NestingModel):
+    """Configuration for Crew Alerting System, including events"""
+    events: Dict[int, CASEvent] = {}
+    """Dictionary of events by their integer id"""
+
+
+class Config(NestingModel):
+    """Root of configuration structure
+
+    Every config field in this and children should be provided with defaults,
+    that can be overriden by config files"""
+
+    json_schema_url: Optional[str] = Field(alias='$schema', default=None)
+    """Allow the `$schema` property for specifying JSON Schema URL"""
+    rpctask = RpctaskConfig()
+    pfd = PfdConfig()
+    approach = ApproachConfig()
+    instruments = InstrumentsConfig()
+    cas = CASConfig()
+    start_time: Optional[float] = None
+    """Epoch time in seconds of starting the program (see `time.time()`)"""
+
+
+def schema_location():
+    root_path = path.abspath(path.dirname(__file__))
+    data_path = path.join(root_path, 'data')
+    os.makedirs(data_path, exist_ok=True)
+    return path.join(data_path, 'lidia-config.json')
+
+
+def write_schema():
+    with open(schema_location(), 'w') as out:
+        out.write(Config.schema_json(by_alias=True))
```

### Comparing `lidia-0.8.0/src/lidia/lidia.py` & `lidia-0.8.1/src/lidia/lidia.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import argparse
-import json
-from multiprocessing import Process, Queue
-from time import time
-import tomli
-import re
-from typing import Dict
-import yaml
-
-from . import __version__
-from .server import run_server
-from .config import Config
-from .sources.mytypes import RunFn, SetupFn
-
-from .sources import demo, rpctask, approach, smol, flightgear, confighelp
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        prog='lidia',
-        description='serve an aircraft instruments panel as a web page',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        epilog='you can also see help for a specific source: "lidia <src> --help"')
-    parser.add_argument('-V', '--version', action='version', version=f'{parser.prog} {__version__}',
-                        help='display package version')
-    parser.add_argument('-v', '--verbose', action='count', dest='verbosity',
-                        help='increase amount of printed information, can be added multiple times', default=0)
-    parser.add_argument('-q', '--quiet', action='count',
-                        help='decrease amount of printed information', default=0)
-    parser.add_argument('-c', '--config', type=str,
-                        help='config files separated with comma, in order of applying')
-    parser.add_argument('-C', '--config-keys', type=str,
-                        help='properties as comma separated dotted keys')
-    parser.add_argument('-H', '--http-host', type=str,
-                        help='hosts to accept for web page', default='0.0.0.0')
-    parser.add_argument('-P', '--http-port', type=int,
-                        help='port to serve the web page on', default=5555)
-    parser.add_argument('-U', '--passthrough-host', type=str,
-                        help='address to forward state to', default='127.0.0.1')
-    parser.add_argument('-O', '--passthrough-port', type=int,
-                        help='port to forward the state to (e.g. 50010)')
-    subparsers = parser.add_subparsers(title='source', required=True, dest='source',
-                                       help='source name', description='select where to get aircraft state')
-
-    sources: Dict[str, RunFn] = {}
-    for source_module in [demo, rpctask, approach, smol, flightgear, confighelp]:
-        setup: SetupFn = source_module.setup
-        name, run_function = setup(subparsers)
-        sources[name] = run_function
-
-    args = parser.parse_args()
-
-    args.verbosity -= args.quiet
-    if args.verbosity >= 1:
-        # mimic '=' specifier from python 3.8 to maintain 3.7 compatibility
-        print(f'args={args}')
-
-    config = Config()
-    if args.config is not None:
-        for config_filename in args.config.split(','):
-            config_filename: str
-            update_dict = None
-            if config_filename.lower().endswith('.json'):
-                update_dict = json.load(open(config_filename))
-            elif config_filename.lower().endswith('.yaml') or config_filename.lower().endswith('.yml'):
-                update_dict = yaml.safe_load(open(config_filename))
-            elif config_filename.lower().endswith('.toml'):
-                update_dict = tomli.load(open(config_filename, 'rb'))
-            else:
-                parser.error(
-                    'Config files have to end with ".json", ".yaml", ".yml" or ".toml" to detect correct parser type')
-            if update_dict is not None:
-                config = config.updated(update_dict)
-    if args.config_keys is not None:
-        # FIXME: does not handle single quote escaping
-        separator = re.compile(
-            r"""(?!\B"[^"]*),(?![^"]*"\B)""")  # comma not between double quotes
-        toml_string = '\n'.join(re.split(separator, args.config_keys))
-        update_dict = tomli.loads(toml_string)
-        config = config.updated(update_dict)
-    if config.start_time is None:
-        config.start_time = time()
-    if args.verbosity >= 1:
-        print(f'config=Config({config})')
-
-    queue = Queue()
-    server_process = Process(target=run_server, args=(queue, args, config))
-    server_process.start()
-
-    if args.verbosity >= 0 and not args.source.endswith('help'):
-        print(f"""\
-Lidia GUIs driven by '{args.source}' source served on:
-    - RPC task: http://localhost:{args.http_port}/rpctask
-    - Primary Flight Display: http://localhost:{args.http_port}/pfd
-    - Ship Approach: http://localhost:{args.http_port}/approach
-
-(see this list and configuration at http://localhost:{args.http_port}/info)""")
-        if args.passthrough_port is not None:
-            print(
-                f'State in SMOL forwarded via UDP to {args.passthrough_host}:{args.passthrough_port}')
-
-    try:
-        (sources[args.source])(queue, args, config)
-
-    except KeyboardInterrupt:
-        if args.verbosity >= 0 and not args.source.endswith('help'):
-            print('Exiting main loop')
-    except Exception as e:  # needed to stop the server process
-        server_process.terminate()
-        raise e
-
-    server_process.terminate()
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import json
+from multiprocessing import Process, Queue
+from time import time
+import tomli
+import re
+from typing import Dict
+import yaml
+
+from . import __version__
+from .server import run_server
+from .config import Config
+from .sources.mytypes import RunFn, SetupFn
+
+from .sources import demo, rpctask, approach, smol, flightgear, confighelp
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        prog='lidia',
+        description='serve an aircraft instruments panel as a web page',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        epilog='you can also see help for a specific source: "lidia <src> --help"')
+    parser.add_argument('-V', '--version', action='version', version=f'{parser.prog} {__version__}',
+                        help='display package version')
+    parser.add_argument('-v', '--verbose', action='count', dest='verbosity',
+                        help='increase amount of printed information, can be added multiple times', default=0)
+    parser.add_argument('-q', '--quiet', action='count',
+                        help='decrease amount of printed information', default=0)
+    parser.add_argument('-c', '--config', type=str,
+                        help='config files separated with comma, in order of applying')
+    parser.add_argument('-C', '--config-keys', type=str,
+                        help='properties as comma separated dotted keys')
+    parser.add_argument('-H', '--http-host', type=str,
+                        help='hosts to accept for web page', default='0.0.0.0')
+    parser.add_argument('-P', '--http-port', type=int,
+                        help='port to serve the web page on', default=5555)
+    parser.add_argument('-U', '--passthrough-host', type=str,
+                        help='address to forward state to', default='127.0.0.1')
+    parser.add_argument('-O', '--passthrough-port', type=int,
+                        help='port to forward the state to (e.g. 50010)')
+    subparsers = parser.add_subparsers(title='source', required=True, dest='source',
+                                       help='source name', description='select where to get aircraft state')
+
+    sources: Dict[str, RunFn] = {}
+    for source_module in [demo, rpctask, approach, smol, flightgear, confighelp]:
+        setup: SetupFn = source_module.setup
+        name, run_function = setup(subparsers)
+        sources[name] = run_function
+
+    args = parser.parse_args()
+
+    args.verbosity -= args.quiet
+    if args.verbosity >= 1:
+        # mimic '=' specifier from python 3.8 to maintain 3.7 compatibility
+        print(f'args={args}')
+
+    config = Config()
+    if args.config is not None:
+        for config_filename in args.config.split(','):
+            config_filename: str
+            update_dict = None
+            if config_filename.lower().endswith('.json'):
+                update_dict = json.load(open(config_filename))
+            elif config_filename.lower().endswith('.yaml') or config_filename.lower().endswith('.yml'):
+                update_dict = yaml.safe_load(open(config_filename))
+            elif config_filename.lower().endswith('.toml'):
+                update_dict = tomli.load(open(config_filename, 'rb'))
+            else:
+                parser.error(
+                    'Config files have to end with ".json", ".yaml", ".yml" or ".toml" to detect correct parser type')
+            if update_dict is not None:
+                config = config.updated(update_dict)
+    if args.config_keys is not None:
+        # FIXME: does not handle single quote escaping
+        separator = re.compile(
+            r"""(?!\B"[^"]*),(?![^"]*"\B)""")  # comma not between double quotes
+        toml_string = '\n'.join(re.split(separator, args.config_keys))
+        update_dict = tomli.loads(toml_string)
+        config = config.updated(update_dict)
+    if config.start_time is None:
+        config.start_time = time()
+    if args.verbosity >= 1:
+        print(f'config=Config({config})')
+
+    queue = Queue()
+    server_process = Process(target=run_server, args=(queue, args, config))
+    server_process.start()
+
+    if args.verbosity >= 0 and not args.source.endswith('help'):
+        print(f"""\
+Lidia GUIs driven by '{args.source}' source served on:
+    - RPC task: http://localhost:{args.http_port}/rpctask
+    - Primary Flight Display: http://localhost:{args.http_port}/pfd
+    - Ship Approach: http://localhost:{args.http_port}/approach
+
+(see this list and configuration at http://localhost:{args.http_port}/info)""")
+        if args.passthrough_port is not None:
+            print(
+                f'State in SMOL forwarded via UDP to {args.passthrough_host}:{args.passthrough_port}')
+
+    try:
+        (sources[args.source])(queue, args, config)
+
+    except KeyboardInterrupt:
+        if args.verbosity >= 0 and not args.source.endswith('help'):
+            print('Exiting main loop')
+    except Exception as e:  # needed to stop the server process
+        server_process.terminate()
+        raise e
+
+    server_process.terminate()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `lidia-0.8.0/src/lidia/mytypes.py` & `lidia-0.8.1/src/lidia/mytypes.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from typing import List
-from pydantic import BaseModel, Extra
-from pydantic.utils import deep_update
-
-
-# HACK: These classes rely on iteration through dict of fields in the order they were defined
-#       So far observed to work in CPython, but isn't guaranteed by language implementations
-
-class VectorModel(BaseModel):
-    """Vector data to be serialized as array in SMOL"""
-
-    def smol(self) -> List[float]:
-        return [getattr(self, name) for name in self.__fields__]
-
-    @classmethod
-    def from_list(cls, values):
-        return cls(**dict(zip(cls.__fields__, values)))
-
-    def __add__(self, other):
-        assert type(self) == type(other)
-        copy = self.copy()
-        for f in self.__fields__:
-            setattr(copy, f, getattr(self, f) + getattr(other, f))
-        return copy
-
-    def __neg__(self):
-        copy = self.copy()
-        for f in self.__fields__:
-            setattr(copy, f, -getattr(self, f))
-        return copy
-
-    def __sub__(self, other):
-        return self + (-other)
-
-    def __mul__(self, other):
-        o = float(other)
-        copy = self.copy()
-        for f in self.__fields__:
-            setattr(copy, f, getattr(self, f) * o)
-        return copy
-
-    def __truediv__(self, other):
-        return self * (1 / other)
-
-
-class IntFlagModel(BaseModel):
-    """Data like `enum.IntFlag` to be serialized as int bits in SMOL"""
-
-    def smol(self) -> List[int]:
-        result = []
-        for i, name in enumerate(self.__fields__):
-            if i % 32 == 0:
-                result.append(0)
-            if getattr(self, name):
-                result[i // 32] |= 1 << (i % 32)
-        return result
-
-    @classmethod
-    def from_list(cls, values):
-        b_values = []
-        for i, intval in enumerate(values):
-            b_values.append(intval[i // 32] & (1 << (i % 32)))
-        return cls(**dict(zip(cls.__fields__, b_values)))
-
-
-class NestingModel(BaseModel, extra=Extra.forbid):
-    """Extension to `pydantic.BaseModel` allowing for updating with nested dictionary"""
-
-    def updated(self, update_dict: dict[str, object]):
-        """Construct new model, overriding values provided in nested dictionary
-
-        The data is validated, both for type and not having keys undefined in the model"""
-        # return value is not annotated because it problems with type analysis for children
-        new_dict = deep_update(self.dict(by_alias=True), update_dict)
-        return self.__class__(**new_dict)
+from typing import List
+from pydantic import BaseModel, Extra
+from pydantic.utils import deep_update
+
+
+# HACK: These classes rely on iteration through dict of fields in the order they were defined
+#       So far observed to work in CPython, but isn't guaranteed by language implementations
+
+class VectorModel(BaseModel):
+    """Vector data to be serialized as array in SMOL"""
+
+    def smol(self) -> List[float]:
+        return [getattr(self, name) for name in self.__fields__]
+
+    @classmethod
+    def from_list(cls, values):
+        return cls(**dict(zip(cls.__fields__, values)))
+
+    def __add__(self, other):
+        assert type(self) == type(other)
+        copy = self.copy()
+        for f in self.__fields__:
+            setattr(copy, f, getattr(self, f) + getattr(other, f))
+        return copy
+
+    def __neg__(self):
+        copy = self.copy()
+        for f in self.__fields__:
+            setattr(copy, f, -getattr(self, f))
+        return copy
+
+    def __sub__(self, other):
+        return self + (-other)
+
+    def __mul__(self, other):
+        o = float(other)
+        copy = self.copy()
+        for f in self.__fields__:
+            setattr(copy, f, getattr(self, f) * o)
+        return copy
+
+    def __truediv__(self, other):
+        return self * (1 / other)
+
+
+class IntFlagModel(BaseModel):
+    """Data like `enum.IntFlag` to be serialized as int bits in SMOL"""
+
+    def smol(self) -> List[int]:
+        result = []
+        for i, name in enumerate(self.__fields__):
+            if i % 32 == 0:
+                result.append(0)
+            if getattr(self, name):
+                result[i // 32] |= 1 << (i % 32)
+        return result
+
+    @classmethod
+    def from_list(cls, values):
+        b_values = []
+        for i, intval in enumerate(values):
+            b_values.append(intval[i // 32] & (1 << (i % 32)))
+        return cls(**dict(zip(cls.__fields__, b_values)))
+
+
+class NestingModel(BaseModel, extra=Extra.forbid):
+    """Extension to `pydantic.BaseModel` allowing for updating with nested dictionary"""
+
+    def updated(self, update_dict: dict[str, object]):
+        """Construct new model, overriding values provided in nested dictionary
+
+        The data is validated, both for type and not having keys undefined in the model"""
+        # return value is not annotated because it problems with type analysis for children
+        new_dict = deep_update(self.dict(by_alias=True), update_dict)
+        return self.__class__(**new_dict)
```

### Comparing `lidia-0.8.0/src/lidia/pfd.html` & `lidia-0.8.1/src/lidia/pfd.html`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,645 +1,645 @@
-<!DOCTYPE html>
-
-<html>
-
-<head>
-  <title>Lidia PFD</title>
-  <meta charset="UTF-8">
-  <style type="text/css">
-    .tapeBackground {
-      fill: gray;
-    }
-
-    .tapeContour {
-      fill: none;
-      stroke: white;
-      stroke-width: 5;
-    }
-  </style>
-  <link rel="stylesheet" href="static/style.css" />
-  <script src="static/socket.io.js"></script>
-</head>
-
-<body>
-  <svg id="mainSvg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2100 1200" preserveAspectRatio="xMidYMid meet">
-    <defs>
-      <path id="attTarget"
-        d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M -1.5,0 h-2 l-2,-0.9 h-4 M 1.5,0 h2 l2,-0.9 h4 M 0,1.5 v1 M 0,-1.5 v-2"
-        stroke-linecap="round" fill="none" />
-      <path id="flightpathVector" d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M -2,0 h-3.5 M 2,0 h3.5 M 0,-2 v-1.5"
-        stroke-linecap="square" fill="none" />
-      <g id="flightpathRetrograde" stroke-linecap="square" fill="none">
-        <path d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M 0,-2 v-2 M -1.73, 1 l -1.73, 1 M 1.73, 1 l 1.73, 1" />
-        <path d="M -2.82,-2.82 L 2.82,2.82 M -2.82,2.82 L 2.82,-2.82" transform="scale(0.5)" />
-      </g>
-    </defs>
-    <g id="autopilotRegion" data-extents="0 1325 30 775">
-      <path id="PIC" d="M1050 15 v5 h15 v 10 l15 -15 l-15 -15 v10 h-15 z" fill="var(--pfdGreen)" stroke="none" />
-    </g>
-
-    <g id="adiRegion" data-extents="35 1325 585 775">
-      <g transform="translate(1050 310)">
-        <rect id="adiBackground" x="-275" y="-275" height="550" width="550" rx="25" />
-        <circle id="adiInnerBackground" cx="0" cy="0" r="240" />
-        <clipPath id="adiClip">
-          <use href="#adiBackground" />
-        </clipPath>
-        <clipPath id="adiInnerClip">
-          <use href="#adiInnerBackground" />
-        </clipPath>
-
-        <g clip-path="url(#adiClip)">
-          <g transform="scale(8)">
-            <g id="adiHorizon">
-              <rect x="-150" y="-150" width="300" height="150" fill="var(--pfdSky)" stroke="none" />
-              <rect x="-150" y="0" width="300" height="150" fill="var(--pfdGround)" stroke="none" />
-              <path d="M-150 0 h300" stroke="white" stroke-width="1.25" />
-            </g>
-          </g>
-        </g>
-
-        <use href="#adiInnerBackground" fill="white" fill-opacity="0.1" />
-        <g id="adiRollTicks" fill="white" stroke="white" stroke-width="3">
-          <path d="m0 -240 l15 -20 h-30 z" stroke="none" />
-          <path d="m0 -240 v-20" transform="rotate(10)" />
-          <path d="m0 -240 v-20" transform="rotate(20)" />
-          <path d="m0 -240 v-20" transform="rotate(30)" />
-          <path d="m0 -240 v-20" transform="rotate(60)" />
-          <path d="m0 -240 v-20" transform="rotate(-10)" />
-          <path d="m0 -240 v-20" transform="rotate(-20)" />
-          <path d="m0 -240 v-20" transform="rotate(-30)" />
-          <path d="m0 -240 v-20" transform="rotate(-60)" />
-          <path d="m0 -240 l10 -15 h-20 z" stroke="none" transform="rotate(45)" />
-          <path d="m0 -240 l10 -15 h-20 z" stroke="none" transform="rotate(-45)" />
-        </g>
-
-        <g clip-path="url(#adiInnerClip">
-          <g transform="scale(8)">
-            <g id="adiInnerHorizon" fill="white" stroke="white" stroke-width="0.625" font-size="5"
-              dominant-baseline="central">
-              <path d="m-2.5 -7.5 h5" />
-              <path d="m-2.5 -2.5 h5" />
-              <path d="m-2.5 2.5 h5" />
-              <path d="m-2.5 7.5 h5" />
-              <!-- Other ticks generated with script -->
-            </g>
-            <g id="flightpathIndicator" display="none">
-              <!-- <use href="#flightpathVector" stroke="black" stroke-width="1.0" /> -->
-              <use href="#flightpathVector" stroke="var(--pfdGreen)" stroke-width="0.625" />
-            </g>
-            <g id="flightpathRetrogradeIndicator" display="none">
-              <!-- <use href="#flightpathRetrograde" stroke="black" stroke-width="1.0" /> -->
-              <use href="#flightpathRetrograde" stroke="var(--pfdGreen)" stroke-width="0.625" />
-            </g>
-            <g id="adiTargetIndicator" display="none">
-              <use href="#attTarget" stroke="black" stroke-width="1.0" />
-              <use href="#attTarget" stroke="var(--pfdMagenta)" stroke-width="0.625" />
-            </g>
-          </g>
-        </g>
-
-        <g fill="white" stroke="black" stroke-width="1.5">
-          <!-- <path d="M0 -5 l-100 30 h200 z" /> -->
-          <path d="m70 25 h15 v-20 h100 v-15 h-115 z" />
-          <path d="m-70 25 h-15 v-20 h-100 v-15 h115 z" />
-          <circle cx="0" cy="0" r="10" />
-          <g id="adiRoll">
-            <path d="m0 -240 l15 20 h-30 z" />
-            <g transform="translate(0 -240) scale(30)" stroke-width="0.05">
-              <path id="adiSlipskidIndicator" d="m0.55 0.7333 l0.15 0.2 h-1.4 l0.15 -0.2 z" />
-            </g>
-          </g>
-        </g>
-      </g>
-    </g>
-
-    <g id="vsiRegion" data-extents="35 1505 585 1345">
-      <g transform="translate(1050 310)">
-        <path d="M300 0 v-200 l50 -70 h100 v540 h-100 l-50 -70 z" fill="gray" stroke="white" stroke-width="5" />
-        <path d="M380 0 h70" stroke="white" stroke-width="8" />
-        <g id="vsiTicks" stroke="white" stroke-width="5">
-          <path d="M380 33.1 L405 35.3 M380 66.0 L405 70.3 M380 98.4 L405 104.8 M380 130.0
-          L405 138.5 M380 160.6 L405 171.2 M380 190.0 L405 202.5 M380 218.0 L405 232.3" />
-          <path d="M380 160.6 L415 175.4 M380 218.0 L415 238.0" />
-        </g>
-        <use xlink:href="#vsiTicks" transform="scale (1, -1)" />
-        <g id="vsiText" fill="white" font-size="40" dominant-baseline="central" transform="translate(420)">
-          <text y="-240">2</text>
-          <text y="-180">1</text>
-          <text y="180">1</text>
-          <text y="240">2</text>
-        </g>
-        <line id="vsiIndicator" x1="320" y1="0" x2="370" y2="0" stroke="var(--pfdGreen)" stroke-width="8" />
-      </g>
-    </g>
-
-    <g id="vsidialRegionIgnored" display="none" data-extents="25 2080 585 1520">
-      <g transform="translate(1800 310)">
-        <circle cx="0" cy="0" r="275" fill="black" stroke="white" stroke-width="5" />
-        <g id="vsidialDial" text-anchor="middle" dominant-baseline="central" fill="white" stroke="white" font-size="50"
-          stroke-width="8">
-          <text x="0" y="-60" stroke="none">VSI</text>
-          <g font-size="30" stroke="none">
-            <text x="0" y="50">x100</text>
-            <text x="0" y="80">FT/MIN</text>
-            <text x="-120" y="-30">UP</text>
-            <text x="-120" y="30">DN</text>
-          </g>
-
-          <!-- Ticks generated with script -->
-        </g>
-        <g id="vsidialIndicator" stroke-width="5" stroke="white">
-          <path d="M0 0 h-150 v25 l-50 -25 l50 -25 v25" fill="white" />
-          <circle cx="0" cy="0" r="15" fill="black" />
-        </g>
-      </g>
-    </g>
-
-    <g id="altRegion" data-extents="35 1725 635 1545">
-      <g transform="translate(1550 310)">
-        <rect id="altBackground" x="0" y="-270" width="170" height="540" />
-        <use href="#altBackground" class="tapeBackground" />
-        <use href="#altBackground" class="tapeContour" />
-
-        <clipPath id="altClip">
-          <use href="#altBackground" />
-        </clipPath>
-
-        <g clip-path="url(#altClip)">
-          <g transform="scale(0.5)">
-            <g id="altTape" transform="translate(0 0)" fill="white" font-size="80" text-anchor="end"
-              dominant-baseline="central" stroke="white">
-              <!-- Ticks generated with script -->
-            </g>
-          </g>
-        </g>
-
-        <g id="altReadout">
-          <path id="altReadoutBackground" d="m1 0 l30 30 h80 v25 h60 v-110 h-60 v25 h-80 z" />
-          <clipPath id="altReadoutClip">
-            <use href="#altReadoutBackground" />
-          </clipPath>
-          <g clip-path="url(#altReadoutClip)" text-anchor="end" dominant-baseline="central">
-            <text id="altReadoutValue" x="110" y="0" id="alt_ro" fill="var(--pfdGreen)" font-size="50">00</text>
-            <g transform="scale(1.75) translate(94.5 0)">
-              <g id="altReadoutTape" transform="translate(0 0)" fill="var(--pfdGreen)" font-size="24">
-                <text x="0" y="-140">40</text>
-                <text x="0" y="-120">20</text>
-                <text x="0" y="-100">00</text>
-                <text x="0" y="-80">80</text>
-                <text x="0" y="-60">60</text>
-                <text x="0" y="-40">40</text>
-                <text x="0" y="-20">20</text>
-                <text x="0" y="0">00</text>
-                <text x="0" y="20">20</text>
-                <text x="0" y="40">40</text>
-                <text x="0" y="60">60</text>
-                <text x="0" y="80">80</text>
-                <text x="0" y="100">00</text>
-                <text x="0" y="120">20</text>
-                <text x="0" y="140">40</text>
-              </g>
-            </g>
-          </g>
-          <use href="#altReadoutBackground" class="tapeContour" />
-          <g id="altReadoutNegative" display="none">
-            <rect id="altReadoutNegativeBackground" x="30" y="30" width="80" height="25" />
-            <text x="70" y="42.5" text-anchor="middle" dominant-baseline="central" font-size="24" font-weight="700"
-              fill="var(--pfdAmber)">NEG</text>
-            <use href="#altReadoutNegativeBackground" class="tapeContour" />
-          </g>
-        </g>
-        <g id="altQnh" dominant-baseline="central" font-size="40" text-anchor="middle">
-          <text id="altQnhValue" x="85" y="295" fill="var(--pfdCyan)">STD</text>
-          <rect x="0" y="270" width="170" height="50" class="tapeContour" />
-        </g>
-      </g>
-    </g>
-
-    <g id="iasRegion" data-extents="35 755 635 575">
-      <g transform="translate(750 310)">
-        <rect id="iasBackground" x="-170" y="-270" width="170" height="540" />
-        <use href="#iasBackground" class="tapeBackground" />
-        <clipPath id="iasClip">
-          <use href="#iasBackground" />
-        </clipPath>
-
-        <g clip-path="url(#iasClip)">
-          <g transform="scale(6)">
-            <g id="iasTape" transform="translate(0 0)" fill="white" font-size="6" text-anchor="end"
-              dominant-baseline="central" stroke="white" stroke-width="1">
-              <g id="iasVne" transform="translate(0 -167)">
-                <path d="m0 0 h-30 " stroke="var(--pfdRed)" stroke-width="2" />
-              </g>
-
-              <path d="m0 10 h-10" />
-              <path d="m0 20 h-10" />
-              <path d="m0 30 h-10" />
-              <path d="m0 40 h-10" />
-              <!-- Other ticks generated with script -->
-            </g>
-          </g>
-        </g>
-        <use href="#iasBackground" class="tapeContour" />
-        <g id="iasReadout">
-          <path id="iasReadoutBackground" d="m-5 0 l-30 -30 h-135 v60 h135 z" />
-          <clipPath id="iasReadoutClip">
-            <use href="#iasReadoutBackground" />
-          </clipPath>
-          <g clip-path="url(#iasReadoutClip)" text-anchor="end" dominant-baseline="central">
-            <text id="iasReadoutValue" x="-60" y="0" id="IAS_ro" fill="var(--pfdGreen)" font-size="50">00</text>
-            <g transform="scale(35)">
-              <g id="iasReadoutTape" transform="translate(0 0)" fill="var(--pfdGreen)" font-size="1.2">
-                <text x="-1" y="-10">0</text>
-                <text x="-1" y="-9">9</text>
-                <text x="-1" y="-8">8</text>
-                <text x="-1" y="-7">7</text>
-                <text x="-1" y="-6">6</text>
-                <text x="-1" y="-5">5</text>
-                <text x="-1" y="-4">4</text>
-                <text x="-1" y="-3">3</text>
-                <text x="-1" y="-2">2</text>
-                <text x="-1" y="-1">1</text>
-                <text x="-1" y="0">0</text>
-                <text x="-1" y="1">9</text>
-              </g>
-            </g>
-          </g>
-          <use href="#iasReadoutBackground" class="tapeContour" />
-        </g>
-        <g id="iasGroundspeed" dominant-baseline="central" font-size="40">
-          <text x="-160" y="295" fill="white">GS</text>
-          <text id="iasGroundspeedValue" x="-10" y="295" fill="var(--pfdAmber)" text-anchor="end">---</text>
-          <rect x="-170" y="270" width="170" height="50" class="tapeContour" />
-        </g>
-      </g>
-    </g>
-
-    <g id="rhtRegion" data-extents="660 1805 1220 1545">
-      <g transform="translate(1550 940)">
-        <rect id="rhtBackground" x="0" y="-275" height="550" width="250" />
-        <use href="#rhtBackground" class="tapeBackground" />
-        <use href="#rhtBackground" class="tapeContour" />
-        <clipPath id="rhtClip">
-          <use href="#rhtBackground" />
-        </clipPath>
-        <g clip-path="url(#rhtClip)">
-          <g transform="scale(1 1)">
-            <g id="rhtTape" transform="translate(0 0)" fill="white" stroke="white" stroke-width="5"
-              dominant-baseline="central" font-size="40">
-              <rect x="0" y="0" height="10" width="250" fill="white" stroke="none" />
-              <rect x="0" y="10" height="500" width="500" fill="var(--pfdGround)" stroke="none" />
-
-              <!-- Ticks generated with script -->
-            </g>
-          </g>
-        </g>
-        <path d="M250 0 v-25 h-150 l-50 25 l50 25 h150 z" stroke="white" stroke-width="5" />
-        <text id="rhtValue" x="245" y="0" fill="var(--pfdAmber)" font-size="48" text-anchor="end"
-          dominant-baseline="central">---</text>
-      </g>
-    </g>
-
-    <g id="hsiRegion" data-extents="595 1325 1180 775">
-      <g transform="translate(1050 900)">
-        <circle cx="0" cy="0" r="275" fill="black" stroke="none" />
-        <circle cx="0" cy="0" r="137.5" fill="none" stroke="white" stroke-dasharray="3" stroke-width="3" />
-        <path d="M0 -280 l20 -20 h-40 z" stroke="white" stroke-width="5" />
-        <g id="hsiWheel" text-anchor="middle" dominant-baseline="hanging" fill="white" font-size="40" font-weight="600">
-          <text x="0" y="-225">N</text>
-          <text x="0" y="-225" transform="rotate(30)">3</text>
-          <text x="0" y="-225" transform="rotate(60)">6</text>
-          <text x="0" y="-225" transform="rotate(90)">E</text>
-          <text x="0" y="-225" transform="rotate(120)">12</text>
-          <text x="0" y="-225" transform="rotate(150)">15</text>
-          <text x="0" y="-225" transform="rotate(180)">S</text>
-          <text x="0" y="-225" transform="rotate(210)">21</text>
-          <text x="0" y="-225" transform="rotate(240)">24</text>
-          <text x="0" y="-225" transform="rotate(270)">W</text>
-          <text x="0" y="-225" transform="rotate(300)">30</text>
-          <text x="0" y="-225" transform="rotate(330)">33</text>
-
-          <!-- Ticks generated with script -->
-        </g>
-        <g id="hsiHeli">
-          <ellipse cx="0" cy="0" rx="12" ry="30" fill="white" />
-          <path d="M0 0 v60 M-7 50 h15" stroke-width="5" stroke="white" />
-          <path d="M-32 -32 l64 64 M-32 32 l64 -64" stroke-width="8" stroke="white" />
-        </g>
-      </g>
-    </g>
-
-    <g id="infoRegionIgnored" display="none">
-      <g id="wind_indicator">
-        <circle cx="1350" cy="660" r="40" stroke="white" stroke-width="3" />
-        <path id="wind_arrow" d="m1350 695 v-70 l-15 20 h30 l -15 -20" fill="white" stroke="white" stroke-width="5" />
-        <text id="wind_speed" fill="white" font-size="40" transform="translate(1400 670)">0</text>
-      </g>
-
-      <g id="general_info" fill="white" font-size="30" font-weight="500">
-        <g id="OAT">
-          <text transform="translate(1400 750)">OAT</text>
-          <text id="OAT_ro" transform="translate(1470 750)">15</text>
-          <text transform="translate(1510 750)">°C</text>
-        </g>
-
-        <g id="HSI_ovly">
-          <text id="OAT_ro" transform="translate(1400 790)">No Ovly</text>
-        </g>
-      </g>
-    </g>
-  </svg>
-  <script src="static/controls.js"></script>
-  <script type="text/javascript">
-    let svgElem = document.getElementById("mainSvg");
-    addControls(svgElem);
-  </script>
-
-  <script type="text/javascript">
-    function degrees(radians) {
-      return radians * 180 / Math.PI;
-    }
-
-    function radians(degrees) {
-      return degrees * Math.PI / 180;
-    }
-
-    function feet(meters) {
-      return meters / 0.3048;
-    }
-  </script>
-
-  <script type="text/javascript">
-    let altTapeHTML = [];
-    for (let alt = 0; alt <= 20000; alt += 1000) {
-      altTapeHTML.push(`
-        <g transform="translate(0 ${-alt})">
-          <path
-            d="M0 0 h50 M0 -100 h50 M0 -200 h50 M0 -300 h50 M0 -400 h50 M0 100 h50 M0 200 h50 M0 300 h50 M0 400 h50 M0 500 h50"
-            stroke-width="10" />
-          <g stroke-width="5" fill="none">
-            <path d="m0 0 l150 -150 v-200 l-150 -150" />
-            <path d="m0 0 l150 150 v200 l-150 150 " />
-            <path d="m0 0 l150 -110 v-40" />
-            <path d="m0 0 l150 110 v40" />
-          </g>
-          <text x="310" y="0">${alt}</text>
-          <text x="310" y="500">${alt - 500}</text>
-        </g>
-      `);
-    }
-    let altTape = document.getElementById("altTape");
-    altTape.innerHTML = altTape.innerHTML + altTapeHTML.join("");
-
-    let vsidialHTML = [];
-    const textR = 165;
-    for (let vsi = -20; vsi <= 20; vsi += 1) {
-      let angle = vsi * 8;
-      if (vsi % 5 === 0) {
-        vsidialHTML.push(`
-          <path d="M-275 0 h75" transform="rotate(${angle})" />
-          <text x="${-textR * Math.cos(radians(angle))}" y="${-textR * Math.sin(radians(angle))}"
-            stroke="none">${Math.abs(vsi)}</text>
-        `);
-      } else if (Math.abs(vsi) < 10) {
-        vsidialHTML.push(`
-          <path d="M-275 0 h50" transform="rotate(${angle})" />
-        `);
-      }
-    }
-    let vsidial = document.getElementById("vsidialDial");
-    vsidial.innerHTML = vsidial.innerHTML + vsidialHTML.join("");
-
-    let iasTapeHTML = [];
-    for (let ias = 0; ias <= 400; ias += 10) {
-      iasTapeHTML.push(`
-        <path d="m0 ${-ias} h-10" />
-        <text x="-12" y="${-ias}" stroke="none">${ias}</text>`);
-    }
-    let iasTape = document.getElementById("iasTape");
-    iasTape.innerHTML = iasTape.innerHTML + iasTapeHTML.join("");
-
-    let pitchHTML = [];
-    for (let pitch = -50; pitch <= 50; pitch += 10) {
-      if (pitch == 0) continue;
-
-      pitchHTML.push(`
-        <text x="-13" y="${-pitch}" text-anchor="end" stroke="none">${Math.abs(pitch)}</text>
-        <text x="13" y="${-pitch}" text-anchor="start" stroke="none">${Math.abs(pitch)}</text>
-        <path d="m-12 ${-pitch} h24" />
-        <path d="m-6 ${-pitch + Math.sign(pitch) * 5} h12" />
-      `);
-    }
-    let adiInnerHorizon = document.getElementById("adiInnerHorizon");
-    adiInnerHorizon.innerHTML = adiInnerHorizon.innerHTML + pitchHTML.join("");
-
-    let rhtTapeHTML = [];
-    for (let rht = 100; rht <= 2500; rht += 100) {
-      rhtTapeHTML.push(`
-        <text x="80" y="${-rht}" stroke="none">${rht}</text>
-        <path d="m0 ${-rht} h75"/>
-        <path d="m0 ${-rht + 20} h50"/>
-        <path d="m0 ${-rht + 40} h50"/>
-        <path d="m0 ${-rht + 60} h50"/>
-        <path d="m0 ${-rht + 80} h50"/>
-      `);
-    }
-    let rhtTape = document.getElementById("rhtTape");
-    rhtTape.innerHTML = rhtTape.innerHTML + rhtTapeHTML.join("");
-
-    let hsiWheelHTML = [];
-    for (let hdg = 0; hdg < 360; hdg += 5) {
-      let idx = hdg / 5;
-      hsiWheelHTML.push(`
-        <path d="M0 -275 v${idx % 6 === 0 ? 50 : idx % 2 === 0 ? 35 : 20}"
-          transform="rotate(${hdg})" stroke="white" stroke-width="7" />
-      `);
-    }
-    let hsiWheel = document.getElementById("hsiWheel");
-    hsiWheel.innerHTML = hsiWheel.innerHTML + hsiWheelHTML.join("");
-  </script>
-
-  <script type="text/javascript">
-    var socket = io();
-    var config = {
-      ias_never_exceed: 167,
-      rotate_adi_target: true,
-      show_adi_target: true,
-      adi_target_roll: true,
-      adi_target_yaw: false,
-      show_flightpath: true,
-      show_retrograde: false,
-      move_roll_ticks: false,
-      sideslip_max: 15,
-    };
-
-    function updateOptional(value, element, decimal = 0, width = 1) {
-      if (value !== null && isFinite(value)) {
-        element.textContent = value.toFixed(decimal).padStart(width, "0");
-        element.setAttribute("fill", "white");
-      } else {
-        element.textContent = "---";
-        element.setAttribute("fill", "var(--pfdAmber)");
-      }
-    }
-
-    function updateIAS(ias) {
-      document.getElementById("iasTape").setAttribute("transform", `translate(0 ${ias})`);
-      document.getElementById("iasReadoutValue").textContent = String(Math.floor(ias / 10)).padStart(2, "0");
-      document.getElementById("iasReadoutTape").setAttribute("transform", `translate(0 ${ias % 10})`);
-    }
-
-    function updateGS(groundspeed) {
-      updateOptional(groundspeed, document.getElementById("iasGroundspeedValue"), 0, 3);
-    }
-
-    function updateADI(roll, pitch) {
-      let horizonTransform = `rotate(${-roll}) translate(0 ${pitch}) `
-      document.getElementById("adiHorizon").setAttribute("transform", horizonTransform);
-      document.getElementById("adiInnerHorizon").setAttribute("transform", horizonTransform);
-      document.getElementById("adiRollTicks").setAttribute("transform", `rotate(${config.move_roll_ticks ? -roll : 0})`);
-      document.getElementById("adiRoll").setAttribute("transform", `rotate(${config.move_roll_ticks ? 0 : -roll})`);
-    }
-
-    function updateFPV(vx, vy, vz) {
-      document.getElementById("flightpathIndicator").setAttribute("display", (vx > 0 && config.show_flightpath) ? "block" : "none");
-      document.getElementById("flightpathRetrogradeIndicator").setAttribute("display", (vx < 0 && config.show_retrograde) ? "block" : "none");
-
-      let alpha = degrees(Math.atan2(vz, vx));
-      let beta = degrees(Math.atan2(vy, vx));
-      if (vx > 0) {
-        flightpathIndicator.setAttribute("transform", `translate(${beta} ${alpha})`);
-      } else if (vx < 0) {
-        flightpathRetrograde.setAttribute("transform", `translate(${beta - 180} ${alpha - 180})`);
-      }
-    }
-
-    function updateSlip(ay, az) {
-      let slip = degrees(Math.atan2(ay, az));
-      let relative = Math.max(-1, Math.min(1, slip / config.sideslip_max));
-      document.getElementById("adiSlipskidIndicator").setAttribute("transform", `translate(${relative})`);
-    }
-
-    function updateALT(alt) {
-      document.getElementById("altTape").setAttribute("transform", `translate(0 ${alt})`)
-      let readoutValue = String(Math.floor(Math.abs(alt) / 100)).padStart(2, "0");
-      if (alt < 0) { // Add the minus sign manually for consistent digits
-        readoutValue = "-" + readoutValue;
-      }
-      document.getElementById("altReadoutValue").textContent = readoutValue;
-
-      let tapeY = Math.abs(alt) % 100 * Math.sign(alt);
-      if (Math.abs(alt) >= 100 && Math.abs(tapeY) <= 20) { // Only show the part 20-00-20 if close to 0 altitude
-        tapeY += 100 * Math.sign(alt);
-      }
-      document.getElementById("altReadoutTape").setAttribute("transform", `translate(0 ${tapeY})`);
-
-      document.getElementById("altReadoutNegative").setAttribute("display", alt < 0 ? "block" : "none");
-    }
-
-    const qnhValue = document.getElementById("altQnhValue");
-    function updateQNH(qnh) {
-      if (qnh === null) {
-        qnhValue.innerHTML = "STD";
-        qnhValue.setAttribute("fill", "var(--pfdCyan)");
-      } else {
-        qnhValue.innerHTML = String(qnh);
-        qnhValue.setAttribute("fill", "white");
-      }
-    }
-
-    const vsiIndicator = document.getElementById("vsiIndicator");
-    const vsiX1 = parseFloat(vsiIndicator.getAttribute("x1"));
-    const vsiX2 = parseFloat(vsiIndicator.getAttribute("x2"));
-    function updateVSI(verticalSpeed) {
-      let direction = Math.sign(verticalSpeed);
-      let value = Math.abs(verticalSpeed);
-      const maxAngleDeg = 37;
-      let angleDeg = (value <= 10) ? (value / 10 * 25) : // first 10 hft/min is 25 degrees
-        (value - 10 + 25); // above 10 it's 10 deg per 10 hft/min
-      angleDeg = Math.min(angleDeg, maxAngleDeg); // limit to maximum angle
-      let angle = radians(angleDeg) * direction;
-
-      // positive vertical speed is lower y in svg
-      vsiIndicator.setAttribute("y1", -Math.sin(angle) * vsiX1);
-      vsiIndicator.setAttribute("y2", -Math.sin(angle) * vsiX2);
-
-      let dialAngle = Math.max(-170, Math.min(170, verticalSpeed * 8));
-      document.getElementById("vsidialIndicator").setAttribute("transform", `rotate(${dialAngle})`);
-    }
-
-    function updateRHT(rht) {
-      updateOptional(rht, document.getElementById("rhtValue"));
-      if (rht !== null && isFinite(rht)) {
-        document.getElementById("rhtTape").setAttribute("transform", `translate(0 ${rht})`);
-      } else {
-        document.getElementById("rhtTape").setAttribute("transform", `translate(0 0)`);
-      }
-    }
-
-    function updateHSI(hdg) {
-      document.getElementById("hsiWheel").setAttribute("transform", `rotate(${hdg})`);
-    }
-
-    const adiTargetIndicator = document.getElementById("adiTargetIndicator");
-    function updateTarget(s) {
-      if ("att" in s.trgt && "att" in s) {
-        const roll = degrees(s.att[0]);
-        const pitch = degrees(s.att[1]);
-        const yaw = degrees(s.att[2]);
-        const targetRoll = degrees(s.trgt.att[0]);
-        const targetPitch = degrees(s.trgt.att[1]);
-        const targetYaw = degrees(s.trgt.att[2]);
-        adiTargetIndicator.setAttribute("display", config.show_adi_target ? "block" : "none");
-        let horizonTransform = `rotate(${-roll}) translate(0 ${pitch})`;
-        let targetTransform = horizonTransform + ` translate(0 ${-targetPitch})`;
-        if (config.adi_target_yaw) {
-          targetTransform = targetTransform + ` translate(${targetYaw - yaw})`;
-        }
-        if (config.adi_target_roll) {
-          targetTransform = targetTransform + ` rotate(${targetRoll})`
-        }
-        adiTargetIndicator.setAttribute("transform", targetTransform);
-      }
-    }
-
-    function updateLimits() {
-      document.getElementById("iasVne").setAttribute("transform", `translate(0 ${-config.ias_never_exceed})`);
-    }
-
-    socket.on("smol", (s) => {
-      if ("att" in s) {
-        updateADI(degrees(s.att[0]), degrees(s.att[1]));
-        updateHSI(degrees(s.att[2]));
-      }
-      if ("v_ned" in s) {
-        updateVSI(feet(s.v_ned[2]) * -0.6); // from m/s down to 100ft/min up
-      }
-      if ("v_body" in s) {
-        updateFPV(s.v_body[0], s.v_body[1], s.v_body[2]); // units irrelevant
-      }
-      if ("a_body" in s) {
-        updateSlip(s.a_body[1], s.a_body[2]); // units irrelevant
-      }
-      if ("instr" in s) {
-        if ("ias" in s.instr) updateIAS(s.instr.ias);
-        if ("gs" in s.instr) updateGS(s.instr.gs);
-        if ("alt" in s.instr) updateALT(s.instr.alt);
-        if ("qnh" in s.instr) updateQNH(s.instr.qnh);
-        if ("ralt" in s.instr) updateRHT(s.instr.ralt);
-      }
-      if ("trgt" in s) {
-        updateTarget(s);
-      }
-    });
-    socket.on("config", (s) => {
-      if ("pfd" in s) {
-        config = s.pfd;
-        updateLimits();
-      }
-    });
-    socket.emit("config_request", {});
-  </script>
-</body>
-
-</html>
+<!DOCTYPE html>
+
+<html>
+
+<head>
+  <title>Lidia PFD</title>
+  <meta charset="UTF-8">
+  <style type="text/css">
+    .tapeBackground {
+      fill: gray;
+    }
+
+    .tapeContour {
+      fill: none;
+      stroke: white;
+      stroke-width: 5;
+    }
+  </style>
+  <link rel="stylesheet" href="static/style.css" />
+  <script src="static/socket.io.js"></script>
+</head>
+
+<body>
+  <svg id="mainSvg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2100 1200" preserveAspectRatio="xMidYMid meet">
+    <defs>
+      <path id="attTarget"
+        d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M -1.5,0 h-2 l-2,-0.9 h-4 M 1.5,0 h2 l2,-0.9 h4 M 0,1.5 v1 M 0,-1.5 v-2"
+        stroke-linecap="round" fill="none" />
+      <path id="flightpathVector" d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M -2,0 h-3.5 M 2,0 h3.5 M 0,-2 v-1.5"
+        stroke-linecap="square" fill="none" />
+      <g id="flightpathRetrograde" stroke-linecap="square" fill="none">
+        <path d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M 0,-2 v-2 M -1.73, 1 l -1.73, 1 M 1.73, 1 l 1.73, 1" />
+        <path d="M -2.82,-2.82 L 2.82,2.82 M -2.82,2.82 L 2.82,-2.82" transform="scale(0.5)" />
+      </g>
+    </defs>
+    <g id="autopilotRegion" data-extents="0 1325 30 775">
+      <path id="PIC" d="M1050 15 v5 h15 v 10 l15 -15 l-15 -15 v10 h-15 z" fill="var(--pfdGreen)" stroke="none" />
+    </g>
+
+    <g id="adiRegion" data-extents="35 1325 585 775">
+      <g transform="translate(1050 310)">
+        <rect id="adiBackground" x="-275" y="-275" height="550" width="550" rx="25" />
+        <circle id="adiInnerBackground" cx="0" cy="0" r="240" />
+        <clipPath id="adiClip">
+          <use href="#adiBackground" />
+        </clipPath>
+        <clipPath id="adiInnerClip">
+          <use href="#adiInnerBackground" />
+        </clipPath>
+
+        <g clip-path="url(#adiClip)">
+          <g transform="scale(8)">
+            <g id="adiHorizon">
+              <rect x="-150" y="-150" width="300" height="150" fill="var(--pfdSky)" stroke="none" />
+              <rect x="-150" y="0" width="300" height="150" fill="var(--pfdGround)" stroke="none" />
+              <path d="M-150 0 h300" stroke="white" stroke-width="1.25" />
+            </g>
+          </g>
+        </g>
+
+        <use href="#adiInnerBackground" fill="white" fill-opacity="0.1" />
+        <g id="adiRollTicks" fill="white" stroke="white" stroke-width="3">
+          <path d="m0 -240 l15 -20 h-30 z" stroke="none" />
+          <path d="m0 -240 v-20" transform="rotate(10)" />
+          <path d="m0 -240 v-20" transform="rotate(20)" />
+          <path d="m0 -240 v-20" transform="rotate(30)" />
+          <path d="m0 -240 v-20" transform="rotate(60)" />
+          <path d="m0 -240 v-20" transform="rotate(-10)" />
+          <path d="m0 -240 v-20" transform="rotate(-20)" />
+          <path d="m0 -240 v-20" transform="rotate(-30)" />
+          <path d="m0 -240 v-20" transform="rotate(-60)" />
+          <path d="m0 -240 l10 -15 h-20 z" stroke="none" transform="rotate(45)" />
+          <path d="m0 -240 l10 -15 h-20 z" stroke="none" transform="rotate(-45)" />
+        </g>
+
+        <g clip-path="url(#adiInnerClip">
+          <g transform="scale(8)">
+            <g id="adiInnerHorizon" fill="white" stroke="white" stroke-width="0.625" font-size="5"
+              dominant-baseline="central">
+              <path d="m-2.5 -7.5 h5" />
+              <path d="m-2.5 -2.5 h5" />
+              <path d="m-2.5 2.5 h5" />
+              <path d="m-2.5 7.5 h5" />
+              <!-- Other ticks generated with script -->
+            </g>
+            <g id="flightpathIndicator" display="none">
+              <!-- <use href="#flightpathVector" stroke="black" stroke-width="1.0" /> -->
+              <use href="#flightpathVector" stroke="var(--pfdGreen)" stroke-width="0.625" />
+            </g>
+            <g id="flightpathRetrogradeIndicator" display="none">
+              <!-- <use href="#flightpathRetrograde" stroke="black" stroke-width="1.0" /> -->
+              <use href="#flightpathRetrograde" stroke="var(--pfdGreen)" stroke-width="0.625" />
+            </g>
+            <g id="adiTargetIndicator" display="none">
+              <use href="#attTarget" stroke="black" stroke-width="1.0" />
+              <use href="#attTarget" stroke="var(--pfdMagenta)" stroke-width="0.625" />
+            </g>
+          </g>
+        </g>
+
+        <g fill="white" stroke="black" stroke-width="1.5">
+          <!-- <path d="M0 -5 l-100 30 h200 z" /> -->
+          <path d="m70 25 h15 v-20 h100 v-15 h-115 z" />
+          <path d="m-70 25 h-15 v-20 h-100 v-15 h115 z" />
+          <circle cx="0" cy="0" r="10" />
+          <g id="adiRoll">
+            <path d="m0 -240 l15 20 h-30 z" />
+            <g transform="translate(0 -240) scale(30)" stroke-width="0.05">
+              <path id="adiSlipskidIndicator" d="m0.55 0.7333 l0.15 0.2 h-1.4 l0.15 -0.2 z" />
+            </g>
+          </g>
+        </g>
+      </g>
+    </g>
+
+    <g id="vsiRegion" data-extents="35 1505 585 1345">
+      <g transform="translate(1050 310)">
+        <path d="M300 0 v-200 l50 -70 h100 v540 h-100 l-50 -70 z" fill="gray" stroke="white" stroke-width="5" />
+        <path d="M380 0 h70" stroke="white" stroke-width="8" />
+        <g id="vsiTicks" stroke="white" stroke-width="5">
+          <path d="M380 33.1 L405 35.3 M380 66.0 L405 70.3 M380 98.4 L405 104.8 M380 130.0
+          L405 138.5 M380 160.6 L405 171.2 M380 190.0 L405 202.5 M380 218.0 L405 232.3" />
+          <path d="M380 160.6 L415 175.4 M380 218.0 L415 238.0" />
+        </g>
+        <use xlink:href="#vsiTicks" transform="scale (1, -1)" />
+        <g id="vsiText" fill="white" font-size="40" dominant-baseline="central" transform="translate(420)">
+          <text y="-240">2</text>
+          <text y="-180">1</text>
+          <text y="180">1</text>
+          <text y="240">2</text>
+        </g>
+        <line id="vsiIndicator" x1="320" y1="0" x2="370" y2="0" stroke="var(--pfdGreen)" stroke-width="8" />
+      </g>
+    </g>
+
+    <g id="vsidialRegionIgnored" display="none" data-extents="25 2080 585 1520">
+      <g transform="translate(1800 310)">
+        <circle cx="0" cy="0" r="275" fill="black" stroke="white" stroke-width="5" />
+        <g id="vsidialDial" text-anchor="middle" dominant-baseline="central" fill="white" stroke="white" font-size="50"
+          stroke-width="8">
+          <text x="0" y="-60" stroke="none">VSI</text>
+          <g font-size="30" stroke="none">
+            <text x="0" y="50">x100</text>
+            <text x="0" y="80">FT/MIN</text>
+            <text x="-120" y="-30">UP</text>
+            <text x="-120" y="30">DN</text>
+          </g>
+
+          <!-- Ticks generated with script -->
+        </g>
+        <g id="vsidialIndicator" stroke-width="5" stroke="white">
+          <path d="M0 0 h-150 v25 l-50 -25 l50 -25 v25" fill="white" />
+          <circle cx="0" cy="0" r="15" fill="black" />
+        </g>
+      </g>
+    </g>
+
+    <g id="altRegion" data-extents="35 1725 635 1545">
+      <g transform="translate(1550 310)">
+        <rect id="altBackground" x="0" y="-270" width="170" height="540" />
+        <use href="#altBackground" class="tapeBackground" />
+        <use href="#altBackground" class="tapeContour" />
+
+        <clipPath id="altClip">
+          <use href="#altBackground" />
+        </clipPath>
+
+        <g clip-path="url(#altClip)">
+          <g transform="scale(0.5)">
+            <g id="altTape" transform="translate(0 0)" fill="white" font-size="80" text-anchor="end"
+              dominant-baseline="central" stroke="white">
+              <!-- Ticks generated with script -->
+            </g>
+          </g>
+        </g>
+
+        <g id="altReadout">
+          <path id="altReadoutBackground" d="m1 0 l30 30 h80 v25 h60 v-110 h-60 v25 h-80 z" />
+          <clipPath id="altReadoutClip">
+            <use href="#altReadoutBackground" />
+          </clipPath>
+          <g clip-path="url(#altReadoutClip)" text-anchor="end" dominant-baseline="central">
+            <text id="altReadoutValue" x="110" y="0" id="alt_ro" fill="var(--pfdGreen)" font-size="50">00</text>
+            <g transform="scale(1.75) translate(94.5 0)">
+              <g id="altReadoutTape" transform="translate(0 0)" fill="var(--pfdGreen)" font-size="24">
+                <text x="0" y="-140">40</text>
+                <text x="0" y="-120">20</text>
+                <text x="0" y="-100">00</text>
+                <text x="0" y="-80">80</text>
+                <text x="0" y="-60">60</text>
+                <text x="0" y="-40">40</text>
+                <text x="0" y="-20">20</text>
+                <text x="0" y="0">00</text>
+                <text x="0" y="20">20</text>
+                <text x="0" y="40">40</text>
+                <text x="0" y="60">60</text>
+                <text x="0" y="80">80</text>
+                <text x="0" y="100">00</text>
+                <text x="0" y="120">20</text>
+                <text x="0" y="140">40</text>
+              </g>
+            </g>
+          </g>
+          <use href="#altReadoutBackground" class="tapeContour" />
+          <g id="altReadoutNegative" display="none">
+            <rect id="altReadoutNegativeBackground" x="30" y="30" width="80" height="25" />
+            <text x="70" y="42.5" text-anchor="middle" dominant-baseline="central" font-size="24" font-weight="700"
+              fill="var(--pfdAmber)">NEG</text>
+            <use href="#altReadoutNegativeBackground" class="tapeContour" />
+          </g>
+        </g>
+        <g id="altQnh" dominant-baseline="central" font-size="40" text-anchor="middle">
+          <text id="altQnhValue" x="85" y="295" fill="var(--pfdCyan)">STD</text>
+          <rect x="0" y="270" width="170" height="50" class="tapeContour" />
+        </g>
+      </g>
+    </g>
+
+    <g id="iasRegion" data-extents="35 755 635 575">
+      <g transform="translate(750 310)">
+        <rect id="iasBackground" x="-170" y="-270" width="170" height="540" />
+        <use href="#iasBackground" class="tapeBackground" />
+        <clipPath id="iasClip">
+          <use href="#iasBackground" />
+        </clipPath>
+
+        <g clip-path="url(#iasClip)">
+          <g transform="scale(6)">
+            <g id="iasTape" transform="translate(0 0)" fill="white" font-size="6" text-anchor="end"
+              dominant-baseline="central" stroke="white" stroke-width="1">
+              <g id="iasVne" transform="translate(0 -167)">
+                <path d="m0 0 h-30 " stroke="var(--pfdRed)" stroke-width="2" />
+              </g>
+
+              <path d="m0 10 h-10" />
+              <path d="m0 20 h-10" />
+              <path d="m0 30 h-10" />
+              <path d="m0 40 h-10" />
+              <!-- Other ticks generated with script -->
+            </g>
+          </g>
+        </g>
+        <use href="#iasBackground" class="tapeContour" />
+        <g id="iasReadout">
+          <path id="iasReadoutBackground" d="m-5 0 l-30 -30 h-135 v60 h135 z" />
+          <clipPath id="iasReadoutClip">
+            <use href="#iasReadoutBackground" />
+          </clipPath>
+          <g clip-path="url(#iasReadoutClip)" text-anchor="end" dominant-baseline="central">
+            <text id="iasReadoutValue" x="-60" y="0" id="IAS_ro" fill="var(--pfdGreen)" font-size="50">00</text>
+            <g transform="scale(35)">
+              <g id="iasReadoutTape" transform="translate(0 0)" fill="var(--pfdGreen)" font-size="1.2">
+                <text x="-1" y="-10">0</text>
+                <text x="-1" y="-9">9</text>
+                <text x="-1" y="-8">8</text>
+                <text x="-1" y="-7">7</text>
+                <text x="-1" y="-6">6</text>
+                <text x="-1" y="-5">5</text>
+                <text x="-1" y="-4">4</text>
+                <text x="-1" y="-3">3</text>
+                <text x="-1" y="-2">2</text>
+                <text x="-1" y="-1">1</text>
+                <text x="-1" y="0">0</text>
+                <text x="-1" y="1">9</text>
+              </g>
+            </g>
+          </g>
+          <use href="#iasReadoutBackground" class="tapeContour" />
+        </g>
+        <g id="iasGroundspeed" dominant-baseline="central" font-size="40">
+          <text x="-160" y="295" fill="white">GS</text>
+          <text id="iasGroundspeedValue" x="-10" y="295" fill="var(--pfdAmber)" text-anchor="end">---</text>
+          <rect x="-170" y="270" width="170" height="50" class="tapeContour" />
+        </g>
+      </g>
+    </g>
+
+    <g id="rhtRegion" data-extents="660 1805 1220 1545">
+      <g transform="translate(1550 940)">
+        <rect id="rhtBackground" x="0" y="-275" height="550" width="250" />
+        <use href="#rhtBackground" class="tapeBackground" />
+        <use href="#rhtBackground" class="tapeContour" />
+        <clipPath id="rhtClip">
+          <use href="#rhtBackground" />
+        </clipPath>
+        <g clip-path="url(#rhtClip)">
+          <g transform="scale(1 1)">
+            <g id="rhtTape" transform="translate(0 0)" fill="white" stroke="white" stroke-width="5"
+              dominant-baseline="central" font-size="40">
+              <rect x="0" y="0" height="10" width="250" fill="white" stroke="none" />
+              <rect x="0" y="10" height="500" width="500" fill="var(--pfdGround)" stroke="none" />
+
+              <!-- Ticks generated with script -->
+            </g>
+          </g>
+        </g>
+        <path d="M250 0 v-25 h-150 l-50 25 l50 25 h150 z" stroke="white" stroke-width="5" />
+        <text id="rhtValue" x="245" y="0" fill="var(--pfdAmber)" font-size="48" text-anchor="end"
+          dominant-baseline="central">---</text>
+      </g>
+    </g>
+
+    <g id="hsiRegion" data-extents="595 1325 1180 775">
+      <g transform="translate(1050 900)">
+        <circle cx="0" cy="0" r="275" fill="black" stroke="none" />
+        <circle cx="0" cy="0" r="137.5" fill="none" stroke="white" stroke-dasharray="3" stroke-width="3" />
+        <path d="M0 -280 l20 -20 h-40 z" stroke="white" stroke-width="5" />
+        <g id="hsiWheel" text-anchor="middle" dominant-baseline="hanging" fill="white" font-size="40" font-weight="600">
+          <text x="0" y="-225">N</text>
+          <text x="0" y="-225" transform="rotate(30)">3</text>
+          <text x="0" y="-225" transform="rotate(60)">6</text>
+          <text x="0" y="-225" transform="rotate(90)">E</text>
+          <text x="0" y="-225" transform="rotate(120)">12</text>
+          <text x="0" y="-225" transform="rotate(150)">15</text>
+          <text x="0" y="-225" transform="rotate(180)">S</text>
+          <text x="0" y="-225" transform="rotate(210)">21</text>
+          <text x="0" y="-225" transform="rotate(240)">24</text>
+          <text x="0" y="-225" transform="rotate(270)">W</text>
+          <text x="0" y="-225" transform="rotate(300)">30</text>
+          <text x="0" y="-225" transform="rotate(330)">33</text>
+
+          <!-- Ticks generated with script -->
+        </g>
+        <g id="hsiHeli">
+          <ellipse cx="0" cy="0" rx="12" ry="30" fill="white" />
+          <path d="M0 0 v60 M-7 50 h15" stroke-width="5" stroke="white" />
+          <path d="M-32 -32 l64 64 M-32 32 l64 -64" stroke-width="8" stroke="white" />
+        </g>
+      </g>
+    </g>
+
+    <g id="infoRegionIgnored" display="none">
+      <g id="wind_indicator">
+        <circle cx="1350" cy="660" r="40" stroke="white" stroke-width="3" />
+        <path id="wind_arrow" d="m1350 695 v-70 l-15 20 h30 l -15 -20" fill="white" stroke="white" stroke-width="5" />
+        <text id="wind_speed" fill="white" font-size="40" transform="translate(1400 670)">0</text>
+      </g>
+
+      <g id="general_info" fill="white" font-size="30" font-weight="500">
+        <g id="OAT">
+          <text transform="translate(1400 750)">OAT</text>
+          <text id="OAT_ro" transform="translate(1470 750)">15</text>
+          <text transform="translate(1510 750)">°C</text>
+        </g>
+
+        <g id="HSI_ovly">
+          <text id="OAT_ro" transform="translate(1400 790)">No Ovly</text>
+        </g>
+      </g>
+    </g>
+  </svg>
+  <script src="static/controls.js"></script>
+  <script type="text/javascript">
+    let svgElem = document.getElementById("mainSvg");
+    addControls(svgElem);
+  </script>
+
+  <script type="text/javascript">
+    function degrees(radians) {
+      return radians * 180 / Math.PI;
+    }
+
+    function radians(degrees) {
+      return degrees * Math.PI / 180;
+    }
+
+    function feet(meters) {
+      return meters / 0.3048;
+    }
+  </script>
+
+  <script type="text/javascript">
+    let altTapeHTML = [];
+    for (let alt = 0; alt <= 20000; alt += 1000) {
+      altTapeHTML.push(`
+        <g transform="translate(0 ${-alt})">
+          <path
+            d="M0 0 h50 M0 -100 h50 M0 -200 h50 M0 -300 h50 M0 -400 h50 M0 100 h50 M0 200 h50 M0 300 h50 M0 400 h50 M0 500 h50"
+            stroke-width="10" />
+          <g stroke-width="5" fill="none">
+            <path d="m0 0 l150 -150 v-200 l-150 -150" />
+            <path d="m0 0 l150 150 v200 l-150 150 " />
+            <path d="m0 0 l150 -110 v-40" />
+            <path d="m0 0 l150 110 v40" />
+          </g>
+          <text x="310" y="0">${alt}</text>
+          <text x="310" y="500">${alt - 500}</text>
+        </g>
+      `);
+    }
+    let altTape = document.getElementById("altTape");
+    altTape.innerHTML = altTape.innerHTML + altTapeHTML.join("");
+
+    let vsidialHTML = [];
+    const textR = 165;
+    for (let vsi = -20; vsi <= 20; vsi += 1) {
+      let angle = vsi * 8;
+      if (vsi % 5 === 0) {
+        vsidialHTML.push(`
+          <path d="M-275 0 h75" transform="rotate(${angle})" />
+          <text x="${-textR * Math.cos(radians(angle))}" y="${-textR * Math.sin(radians(angle))}"
+            stroke="none">${Math.abs(vsi)}</text>
+        `);
+      } else if (Math.abs(vsi) < 10) {
+        vsidialHTML.push(`
+          <path d="M-275 0 h50" transform="rotate(${angle})" />
+        `);
+      }
+    }
+    let vsidial = document.getElementById("vsidialDial");
+    vsidial.innerHTML = vsidial.innerHTML + vsidialHTML.join("");
+
+    let iasTapeHTML = [];
+    for (let ias = 0; ias <= 400; ias += 10) {
+      iasTapeHTML.push(`
+        <path d="m0 ${-ias} h-10" />
+        <text x="-12" y="${-ias}" stroke="none">${ias}</text>`);
+    }
+    let iasTape = document.getElementById("iasTape");
+    iasTape.innerHTML = iasTape.innerHTML + iasTapeHTML.join("");
+
+    let pitchHTML = [];
+    for (let pitch = -50; pitch <= 50; pitch += 10) {
+      if (pitch == 0) continue;
+
+      pitchHTML.push(`
+        <text x="-13" y="${-pitch}" text-anchor="end" stroke="none">${Math.abs(pitch)}</text>
+        <text x="13" y="${-pitch}" text-anchor="start" stroke="none">${Math.abs(pitch)}</text>
+        <path d="m-12 ${-pitch} h24" />
+        <path d="m-6 ${-pitch + Math.sign(pitch) * 5} h12" />
+      `);
+    }
+    let adiInnerHorizon = document.getElementById("adiInnerHorizon");
+    adiInnerHorizon.innerHTML = adiInnerHorizon.innerHTML + pitchHTML.join("");
+
+    let rhtTapeHTML = [];
+    for (let rht = 100; rht <= 2500; rht += 100) {
+      rhtTapeHTML.push(`
+        <text x="80" y="${-rht}" stroke="none">${rht}</text>
+        <path d="m0 ${-rht} h75"/>
+        <path d="m0 ${-rht + 20} h50"/>
+        <path d="m0 ${-rht + 40} h50"/>
+        <path d="m0 ${-rht + 60} h50"/>
+        <path d="m0 ${-rht + 80} h50"/>
+      `);
+    }
+    let rhtTape = document.getElementById("rhtTape");
+    rhtTape.innerHTML = rhtTape.innerHTML + rhtTapeHTML.join("");
+
+    let hsiWheelHTML = [];
+    for (let hdg = 0; hdg < 360; hdg += 5) {
+      let idx = hdg / 5;
+      hsiWheelHTML.push(`
+        <path d="M0 -275 v${idx % 6 === 0 ? 50 : idx % 2 === 0 ? 35 : 20}"
+          transform="rotate(${hdg})" stroke="white" stroke-width="7" />
+      `);
+    }
+    let hsiWheel = document.getElementById("hsiWheel");
+    hsiWheel.innerHTML = hsiWheel.innerHTML + hsiWheelHTML.join("");
+  </script>
+
+  <script type="text/javascript">
+    var socket = io();
+    var config = {
+      ias_never_exceed: 167,
+      rotate_adi_target: true,
+      show_adi_target: true,
+      adi_target_roll: true,
+      adi_target_yaw: false,
+      show_flightpath: true,
+      show_retrograde: false,
+      move_roll_ticks: false,
+      sideslip_max: 15,
+    };
+
+    function updateOptional(value, element, decimal = 0, width = 1) {
+      if (value !== null && isFinite(value)) {
+        element.textContent = value.toFixed(decimal).padStart(width, "0");
+        element.setAttribute("fill", "white");
+      } else {
+        element.textContent = "---";
+        element.setAttribute("fill", "var(--pfdAmber)");
+      }
+    }
+
+    function updateIAS(ias) {
+      document.getElementById("iasTape").setAttribute("transform", `translate(0 ${ias})`);
+      document.getElementById("iasReadoutValue").textContent = String(Math.floor(ias / 10)).padStart(2, "0");
+      document.getElementById("iasReadoutTape").setAttribute("transform", `translate(0 ${ias % 10})`);
+    }
+
+    function updateGS(groundspeed) {
+      updateOptional(groundspeed, document.getElementById("iasGroundspeedValue"), 0, 3);
+    }
+
+    function updateADI(roll, pitch) {
+      let horizonTransform = `rotate(${-roll}) translate(0 ${pitch}) `
+      document.getElementById("adiHorizon").setAttribute("transform", horizonTransform);
+      document.getElementById("adiInnerHorizon").setAttribute("transform", horizonTransform);
+      document.getElementById("adiRollTicks").setAttribute("transform", `rotate(${config.move_roll_ticks ? -roll : 0})`);
+      document.getElementById("adiRoll").setAttribute("transform", `rotate(${config.move_roll_ticks ? 0 : -roll})`);
+    }
+
+    function updateFPV(vx, vy, vz) {
+      document.getElementById("flightpathIndicator").setAttribute("display", (vx > 0 && config.show_flightpath) ? "block" : "none");
+      document.getElementById("flightpathRetrogradeIndicator").setAttribute("display", (vx < 0 && config.show_retrograde) ? "block" : "none");
+
+      let alpha = degrees(Math.atan2(vz, vx));
+      let beta = degrees(Math.atan2(vy, vx));
+      if (vx > 0) {
+        flightpathIndicator.setAttribute("transform", `translate(${beta} ${alpha})`);
+      } else if (vx < 0) {
+        flightpathRetrograde.setAttribute("transform", `translate(${beta - 180} ${alpha - 180})`);
+      }
+    }
+
+    function updateSlip(ay, az) {
+      let slip = degrees(Math.atan2(ay, az));
+      let relative = Math.max(-1, Math.min(1, slip / config.sideslip_max));
+      document.getElementById("adiSlipskidIndicator").setAttribute("transform", `translate(${relative})`);
+    }
+
+    function updateALT(alt) {
+      document.getElementById("altTape").setAttribute("transform", `translate(0 ${alt})`)
+      let readoutValue = String(Math.floor(Math.abs(alt) / 100)).padStart(2, "0");
+      if (alt < 0) { // Add the minus sign manually for consistent digits
+        readoutValue = "-" + readoutValue;
+      }
+      document.getElementById("altReadoutValue").textContent = readoutValue;
+
+      let tapeY = Math.abs(alt) % 100 * Math.sign(alt);
+      if (Math.abs(alt) >= 100 && Math.abs(tapeY) <= 20) { // Only show the part 20-00-20 if close to 0 altitude
+        tapeY += 100 * Math.sign(alt);
+      }
+      document.getElementById("altReadoutTape").setAttribute("transform", `translate(0 ${tapeY})`);
+
+      document.getElementById("altReadoutNegative").setAttribute("display", alt < 0 ? "block" : "none");
+    }
+
+    const qnhValue = document.getElementById("altQnhValue");
+    function updateQNH(qnh) {
+      if (qnh === null) {
+        qnhValue.innerHTML = "STD";
+        qnhValue.setAttribute("fill", "var(--pfdCyan)");
+      } else {
+        qnhValue.innerHTML = String(qnh);
+        qnhValue.setAttribute("fill", "white");
+      }
+    }
+
+    const vsiIndicator = document.getElementById("vsiIndicator");
+    const vsiX1 = parseFloat(vsiIndicator.getAttribute("x1"));
+    const vsiX2 = parseFloat(vsiIndicator.getAttribute("x2"));
+    function updateVSI(verticalSpeed) {
+      let direction = Math.sign(verticalSpeed);
+      let value = Math.abs(verticalSpeed);
+      const maxAngleDeg = 37;
+      let angleDeg = (value <= 10) ? (value / 10 * 25) : // first 10 hft/min is 25 degrees
+        (value - 10 + 25); // above 10 it's 10 deg per 10 hft/min
+      angleDeg = Math.min(angleDeg, maxAngleDeg); // limit to maximum angle
+      let angle = radians(angleDeg) * direction;
+
+      // positive vertical speed is lower y in svg
+      vsiIndicator.setAttribute("y1", -Math.sin(angle) * vsiX1);
+      vsiIndicator.setAttribute("y2", -Math.sin(angle) * vsiX2);
+
+      let dialAngle = Math.max(-170, Math.min(170, verticalSpeed * 8));
+      document.getElementById("vsidialIndicator").setAttribute("transform", `rotate(${dialAngle})`);
+    }
+
+    function updateRHT(rht) {
+      updateOptional(rht, document.getElementById("rhtValue"));
+      if (rht !== null && isFinite(rht)) {
+        document.getElementById("rhtTape").setAttribute("transform", `translate(0 ${rht})`);
+      } else {
+        document.getElementById("rhtTape").setAttribute("transform", `translate(0 0)`);
+      }
+    }
+
+    function updateHSI(hdg) {
+      document.getElementById("hsiWheel").setAttribute("transform", `rotate(${hdg})`);
+    }
+
+    const adiTargetIndicator = document.getElementById("adiTargetIndicator");
+    function updateTarget(s) {
+      if ("att" in s.trgt && "att" in s) {
+        const roll = degrees(s.att[0]);
+        const pitch = degrees(s.att[1]);
+        const yaw = degrees(s.att[2]);
+        const targetRoll = degrees(s.trgt.att[0]);
+        const targetPitch = degrees(s.trgt.att[1]);
+        const targetYaw = degrees(s.trgt.att[2]);
+        adiTargetIndicator.setAttribute("display", config.show_adi_target ? "block" : "none");
+        let horizonTransform = `rotate(${-roll}) translate(0 ${pitch})`;
+        let targetTransform = horizonTransform + ` translate(0 ${-targetPitch})`;
+        if (config.adi_target_yaw) {
+          targetTransform = targetTransform + ` translate(${targetYaw - yaw})`;
+        }
+        if (config.adi_target_roll) {
+          targetTransform = targetTransform + ` rotate(${targetRoll})`
+        }
+        adiTargetIndicator.setAttribute("transform", targetTransform);
+      }
+    }
+
+    function updateLimits() {
+      document.getElementById("iasVne").setAttribute("transform", `translate(0 ${-config.ias_never_exceed})`);
+    }
+
+    socket.on("smol", (s) => {
+      if ("att" in s) {
+        updateADI(degrees(s.att[0]), degrees(s.att[1]));
+        updateHSI(degrees(s.att[2]));
+      }
+      if ("v_ned" in s) {
+        updateVSI(feet(s.v_ned[2]) * -0.6); // from m/s down to 100ft/min up
+      }
+      if ("v_body" in s) {
+        updateFPV(s.v_body[0], s.v_body[1], s.v_body[2]); // units irrelevant
+      }
+      if ("a_body" in s) {
+        updateSlip(s.a_body[1], s.a_body[2]); // units irrelevant
+      }
+      if ("instr" in s) {
+        if ("ias" in s.instr) updateIAS(s.instr.ias);
+        if ("gs" in s.instr) updateGS(s.instr.gs);
+        if ("alt" in s.instr) updateALT(s.instr.alt);
+        if ("qnh" in s.instr) updateQNH(s.instr.qnh);
+        if ("ralt" in s.instr) updateRHT(s.instr.ralt);
+      }
+      if ("trgt" in s) {
+        updateTarget(s);
+      }
+    });
+    socket.on("config", (s) => {
+      if ("pfd" in s) {
+        config = s.pfd;
+        updateLimits();
+      }
+    });
+    socket.emit("config_request", {});
+  </script>
+</body>
+
+</html>
```

### Comparing `lidia-0.8.0/src/lidia/rpctask.html` & `lidia-0.8.1/src/lidia/rpctask.html`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,329 +1,329 @@
-<!DOCTYPE html>
-<html>
-
-<head>
-  <title>Lidia RPC task</title>
-  <link rel="stylesheet" href="static/style.css" />
-  <script src="static/socket.io.js"></script>
-</head>
-
-<body>
-  <svg id="mainSvg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2100 1200" preserveAspectRatio="xMidYMid meet">
-    <defs>
-      <path id="bottomTriangle" stroke-width="2" d="m0,0 l-34.64,60 h69.28 z" />
-      <path id="star" fill="#f74afd" stroke-width="2" d="M25,0 L9,9 L0,25 L-9,9 L-25,0 L-9,-9 L0,-25 L9,-9 z" />
-      <circle id="pointCircle" cx="0" cy="0" r="23" stroke-width="2" />
-      <path id="axisLimits" d="M-50 -30 v60 M-30 -30 v60 M30 -30 v60 M50 -30 v60" stroke-dasharray="3,3"
-        stroke-width="3" />
-      <path id="borderShort"
-        d="M0,-30 v60 h-5 l-17.32,-10 l17.32,-10 l-17.32,-10 l17.32,-10 l-17.32,-10 l17.32,-10 z" />
-      <!-- The larger width prevents wrapping -->
-      <pattern id="borderGreen" x="0" y="0" width="1.1" height=".06">
-        <use href="#borderShort" fill="#0f0" transform="translate(22.32 30)" />
-      </pattern>
-      <pattern id="borderRed" x="0" y="0" width="1.1" height=".06">
-        <use href="#borderShort" fill="#f00" transform="translate(22.32 30)" />
-      </pattern>
-      <rect id="borderLong" x="-22.32" y="-1000" width="22.32" height="1000" />
-    </defs>
-    <rect width="2150" height="1250" x="-25" y="-25" fill="#000" />
-    <!-- Region extents -->
-    <!-- <rect width="630" height="1200" x="0" y="0" fill="#700" />
-    <rect width="340" height="1200" x="630" y="0" fill="#070" />
-    <rect width="1130" height="1200" x="970" y="0" fill="#007" /> -->
-    <g id="textRegion" data-extents="0 630 1200 0">
-      <rect width="500" height="500" x="60" y="70" fill="none" stroke="#fff" stroke-width="5" rx="15" />
-      <rect width="150" height="30" x="125" y="55" fill="#000" />
-      <use id="cycFtr" href="#pointCircle" fill="#000" transform="translate(420 150)" />
-      <rect width="500" height="500" x="60" y="630" fill="none" stroke="#fff" stroke-width="5" rx="15" />
-      <rect width="225" height="30" x="125" y="615" fill="#000" />
-      <use id="collFtr" href="#pointCircle" fill="#000" transform="translate(420 710)" />
-      <text fill="#fff" font-size="50">
-        <tspan x="130" y="80" font-size="30">CYCLIC</tspan>
-        <tspan x="125" y="170">FTR</tspan>
-        <tspan x="125" y="245">LON POS</tspan>
-        <tspan id="cycLonPercent" x="400" y="245">0</tspan>
-        <tspan x="495" y="245">%</tspan>
-        <tspan x="125" y="320">LAT POS</tspan>
-        <tspan id="cycLatPercent" x="400" y="320">0</tspan>
-        <tspan x="495" y="320">%</tspan>
-        <tspan x="130" y="640" font-size="30">COLLECTIVE</tspan>
-        <tspan x="125" y="730">FTR</tspan>
-        <tspan x="125" y="805">POS</tspan>
-        <tspan id="collPercent" x="400" y="805">0</tspan>
-        <tspan x="495" y="805">%</tspan>
-      </text>
-    </g>
-    <g id="collectiveRegion" stroke="#fff" data-extents="0 970 1200 630">
-      <g id="collOrigin" transform="translate(805 1075) rotate(270)">
-        <rect id="collBackground" width="1000" height="60" x="0" y="-30" />
-        <use href="#collBackground" fill="#4d4d4d" stroke-width="5" />
-        <clipPath id="collClip">
-          <use href="#collBackground" />
-        </clipPath>
-
-        <use id="collBoundaryLow" href="#borderShort" fill="#0f0" stroke="none" display="none" />
-        <g id="collBoundaryHigh" fill="#0f0" stroke="none" display="none" transform="translate(1000)">
-          <use href="#borderShort" transform="scale(-1 1)" />
-        </g>
-        <g transform="translate(0 -30)">
-          <g id="collTrimIndicator">
-            <use href="#bottomTriangle" fill="#02f7fa" transform="scale(1 -1)" />
-            <path fill=" none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v60" />
-          </g>
-        </g>
-        <use href="#star" id="collTargetIndicator" />
-        <g clip-path="url(#collClip)">
-          <use id="collTargetLimits" href="#axisLimits" />
-        </g>
-        <g transform="translate(0 30)">
-          <use id="collInputIndicator" href="#bottomTriangle" fill="#f00" />
-        </g>
-      </g>
-    </g>
-    <g id="cyclicRegion" stroke="#fff" data-extents="0 2100 1200 970">
-      <g id="cycOrigin" transform="translate(1525 575)">
-        <rect id="cycBackground" width="1000" height="1000" x="-500" y="-500" />
-        <use href="#cycBackground" fill="#4d4d4d" stroke-width="5" />
-        <clipPath id="cycClip">
-          <use href="#cycBackground" />
-        </clipPath>
-
-        <g id="cycLatOrigin" transform="translate(0 500)">
-          <g id="cycLatTrimIndicator">
-            <path fill="none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v-1000" />
-            <use href="#bottomTriangle" fill="#02f7fa" />
-          </g>
-          <use id="cycBoundaryLeft" href="#borderLong" fill="url(#borderGreen)" stroke="none" display="none"
-            transform="translate(-500)" />
-          <g id="cycBoundaryRight" fill="url(#borderGreen)" stroke="none" display="none" transform="translate(500)">
-            <use href="#borderLong" transform="scale(-1 1)" />
-          </g>
-        </g>
-        <g id="cycLonOrigin" transform="translate(500 0) rotate(90) scale(1 -1)">
-          <g id="cycLonTrimIndicator">
-            <path fill=" none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v-1000" />
-            <use href="#bottomTriangle" fill="#02f7fa" />
-          </g>
-          <use id="cycBoundaryLow" href="#borderLong" fill="url(#borderGreen)" stroke="none" display="none"
-            transform="translate(-500)" />
-          <g id="cycBoundaryHigh" fill="url(#borderGreen)" stroke="none" display="none" transform="translate(500)">
-            <use href="#borderLong" transform="scale(-1 1)" />
-          </g>
-        </g>
-        <use href="#star" id="cycTargetIndicator" />
-        <g clip-path="url(#cycClip)">
-          <g id="cycTargetLimits" fill="none" stroke-dasharray="3,3" stroke-width="3">
-            <circle id="cycLimitCorrect" cx="0" cy="0" r="30" />
-            <circle id="cycLimitWarning" cx="0" cy="0" r="50" />
-          </g>
-        </g>
-        <use id="cycInputIndicator" href="#pointCircle" fill="#f00" />
-      </g>
-    </g>
-    <g id="rudderRegion" stroke="#fff" data-extents="1200 2100 1560 970">
-      <g id="ruddOrigin" transform="translate(1525 1295)">
-        <rect id="ruddBackground" width="1000" height="60" x="-500" y="-30" />
-        <use href="#ruddBackground" fill="#4d4d4d" stroke-width="5" />
-        <clipPath id="ruddClip">
-          <use href="#ruddBackground" />
-        </clipPath>
-
-        <use id="ruddBoundaryLeft" href="#borderShort" fill="#0f0" stroke="none" display="none" />
-        <g id="ruddBoundaryRight" fill="#0f0" stroke="none" display="none" transform="translate(1000)">
-          <use href="#borderShort" transform="scale(-1 1)" />
-        </g>
-        <g transform="translate(0 30)">
-          <g id="ruddTrimIndicator">
-            <use href="#bottomTriangle" fill="#02f7fa" />
-            <path fill=" none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v-60" />
-          </g>
-        </g>
-        <use href="#star" id="ruddTargetIndicator" />
-        <g clip-path="url(#ruddClip)">
-          <use href="#axisLimits" id="ruddTargetLimits" />
-        </g>
-        <g transform="translate(0 -30) scale(1 -1)">
-          <use id="ruddInputIndicator" href="#bottomTriangle" fill="#f00" />
-        </g>
-      </g>
-    </g>
-  </svg>
-  <script src="static/controls.js"></script>
-  <script type="text/javascript">
-    let svgElem = document.getElementById("mainSvg");
-    addControls(svgElem);
-  </script>
-  <script type="text/javascript">
-    var socket = io();
-
-    socket.on("echo", (s) => {
-      console.log(s);
-    });
-  </script>
-  <script type="text/javascript">
-    var socket = io();
-    var config = {
-      correct_tolerance: 0.03,
-      warning_tolerance: 0.05,
-    };
-
-    function errorFill(difference) {
-      var e = Math.abs(difference);
-      if (e <= config.correct_tolerance) return "#0f0";
-      else if (e <= config.warning_tolerance) return "#ff0";
-      else return "#f00";
-    }
-
-    function limitRange(elem, oneSided = false) {
-      const outsideLimit = 10;
-      let rangeMin = oneSided ? 0 : -500;
-      let rangeMax = oneSided ? 1000 : 500;
-      let x = elem.transform.baseVal.getItem(0).matrix.e;
-      let y = elem.transform.baseVal.getItem(0).matrix.f;
-
-      // Clamp translate
-      elem.transform.baseVal.getItem(0).matrix.e = Math.max(
-        rangeMin - outsideLimit,
-        Math.min(rangeMax + outsideLimit, x)
-      );
-      elem.transform.baseVal.getItem(0).matrix.f = Math.max(
-        rangeMin - outsideLimit,
-        Math.min(rangeMax + outsideLimit, y)
-      );
-
-      let inside = x >= rangeMin && x <= rangeMax && y >= rangeMin && y <= rangeMax;
-      elem.style.stroke = inside ? "inherit" : "#f00";
-    }
-
-    const collInput = document.getElementById("collInputIndicator");
-    const cycInput = document.getElementById("cycInputIndicator");
-    const ruddInput = document.getElementById("ruddInputIndicator");
-    const collPercent = document.getElementById("collPercent");
-    const cycLatPercent = document.getElementById("cycLatPercent");
-    const cycLonPercent = document.getElementById("cycLonPercent");
-    function updateControl(s) {
-      collInput.setAttribute("transform", `translate(${s.ctrl[4] * 1000})`);
-      limitRange(collInput, true);
-      cycInput.setAttribute("transform", `translate(${s.ctrl[0] * 500} ${s.ctrl[1] * 500})`);
-      limitRange(cycInput);
-      ruddInput.setAttribute("transform", `translate(${s.ctrl[3] * 500})`);
-      limitRange(ruddInput);
-
-      collPercent.textContent = Math.round(s.ctrl[4] * 100);
-      // Goes from 0% on the left and 100% on the right instead of -1 to +1
-      cycLatPercent.textContent = Math.round((s.ctrl[0] + 1) * 50);
-      // Same as roll, but reversed: 0% is pulling the stick to +1
-      cycLonPercent.textContent = Math.round((1 - s.ctrl[1]) * 50);
-    }
-
-    const collTarget = document.getElementById("collTargetIndicator");
-    const collTargetLimits = document.getElementById("collTargetLimits");
-    const cycTarget = document.getElementById("cycTargetIndicator");
-    const cycTargetLimits = document.getElementById("cycTargetLimits");
-    const ruddTarget = document.getElementById("ruddTargetIndicator");
-    const ruddTargetLimits = document.getElementById("ruddTargetLimits");
-    function updateTarget(s) {
-      collTarget.setAttribute("transform", `translate(${s.trgt.ctrl[4] * 1000})`);
-      limitRange(collTarget, true);
-      cycTarget.setAttribute("transform", `translate(${s.trgt.ctrl[0] * 500} ${s.trgt.ctrl[1] * 500})`);
-      limitRange(cycTarget);
-      ruddTarget.setAttribute("transform", `translate(${s.trgt.ctrl[3] * 500})`);
-      limitRange(ruddTarget);
-
-      collTargetLimits.setAttribute("transform", `translate(${s.trgt.ctrl[4] * 1000})`);
-      cycTargetLimits.setAttribute("transform", `translate(${s.trgt.ctrl[0] * 500} ${s.trgt.ctrl[1] * 500})`);
-      ruddTargetLimits.setAttribute("transform", `translate(${s.trgt.ctrl[3] * 500})`);
-
-      if ("ctrl" in s) {
-        collInput.style.fill = errorFill(s.ctrl[4] - s.trgt.ctrl[4]);
-        // The error is defined in terms of percent of range and these go -1 to +1, so divide by 2
-        cycInput.style.fill = errorFill(
-          Math.sqrt(Math.pow(s.ctrl[0] - s.trgt.ctrl[0], 2) + Math.pow(s.ctrl[1] - s.trgt.ctrl[1], 2)) / 2
-        );
-        ruddInput.style.fill = errorFill((s.ctrl[3] - s.trgt.ctrl[3]) / 2);
-      }
-    }
-
-    const collTrim = document.getElementById("collTrimIndicator");
-    const cycLatTrim = document.getElementById("cycLatTrimIndicator");
-    const cycLonTrim = document.getElementById("cycLonTrimIndicator");
-    const ruddTrim = document.getElementById("ruddTrimIndicator");
-    function updateTrim(s) {
-      collTrim.setAttribute("transform", `translate(${s.trim.ctrl[4] * 1000})`);
-      limitRange(collTrim, true);
-      cycLatTrim.setAttribute("transform", `translate(${s.trim.ctrl[0] * 500})`);
-      limitRange(cycLatTrim);
-      cycLonTrim.setAttribute("transform", `translate(${s.trim.ctrl[1] * 500})`);
-      limitRange(cycLonTrim);
-      ruddTrim.setAttribute("transform", `translate(${s.trim.ctrl[3] * 500})`);
-      limitRange(ruddTrim);
-    }
-
-    const collBoundaryLow = document.getElementById("collBoundaryLow");
-    const collBoundaryHigh = document.getElementById("collBoundaryHigh");
-    const cycBoundaryLow = document.getElementById("cycBoundaryLow");
-    const cycBoundaryHigh = document.getElementById("cycBoundaryHigh");
-    const cycBoundaryLeft = document.getElementById("cycBoundaryLeft");
-    const cycBoundaryRight = document.getElementById("cycBoundaryRight");
-    const ruddBoundaryLeft = document.getElementById("ruddBoundaryLeft");
-    const ruddBoundaryRight = document.getElementById("ruddBoundaryRight");
-    function updateBorderPair(input, lowBdr, highBdr, lowRef, highRef, oneSided = false, pattern = false) {
-      if (lowBdr === (oneSided ? 0.0 : -1.0) && highBdr === 1.0) {
-        lowRef.style.display = "none";
-        highRef.style.display = "none";
-        return;
-      } else {
-        lowRef.style.display = "block";
-        highRef.style.display = "block";
-      }
-
-      lowRef.setAttribute("transform", `translate(${lowBdr * (oneSided ? 1000 : 500)})`);
-      highRef.setAttribute("transform", `translate(${highBdr * (oneSided ? 1000 : 500)})`);
-
-      if (input < lowBdr) lowRef.style.fill = pattern ? "url(#borderRed)" : "#f00";
-      else lowRef.style.fill = pattern ? "url(#borderGreen)" : "#0f0";
-      if (input > highBdr) highRef.style.fill = pattern ? "url(#borderRed)" : "#f00";
-      else highRef.style.fill = pattern ? "url(#borderGreen)" : "#0f0";
-    }
-    function updateBorders(s) {
-      updateBorderPair(s.ctrl[4], s.brdr.low[4], s.brdr.high[4], collBoundaryLow, collBoundaryHigh, true);
-      updateBorderPair(s.ctrl[0], s.brdr.low[0], s.brdr.high[0], cycBoundaryLeft, cycBoundaryRight, false, true);
-      updateBorderPair(s.ctrl[1], s.brdr.low[1], s.brdr.high[1], cycBoundaryLow, cycBoundaryHigh, false, true);
-      updateBorderPair(s.ctrl[3], s.brdr.low[3], s.brdr.high[3], ruddBoundaryLeft, ruddBoundaryRight, false, false);
-    }
-
-    const collFtr = document.getElementById("collFtr");
-    const cycFtr = document.getElementById("cycFtr");
-    function updateButtons(s) {
-      cycFtr.style.fill = s.btn[0] & (1 << 0) ? "#ff0" : "#000";
-      collFtr.style.fill = s.btn[0] & (1 << 1) ? "#ff0" : "#000";
-    }
-
-    function updateLimits() {
-      let correct = config.correct_tolerance * 1000;
-      let warning = config.warning_tolerance * 1000;
-      document.getElementById("axisLimits").setAttribute("d",
-        `M-${warning} -30 v60 M-${correct} -30 v60 M${correct} -30 v60 M${warning} -30 v60`);
-      document.getElementById("cycLimitCorrect").setAttribute("r", correct);
-      document.getElementById("cycLimitWarning").setAttribute("r", warning);
-    }
-
-    socket.on("smol", (s) => {
-      if ("ctrl" in s) updateControl(s);
-      if ("trgt" in s) updateTarget(s);
-      if ("trim" in s) updateTrim(s);
-      if ("brdr" in s) updateBorders(s);
-      if ("btn" in s) updateButtons(s);
-    });
-    socket.on("config", (c) => {
-      if ("rpctask" in c) {
-        config = c.rpctask;
-        updateLimits();
-      }
-    });
-    socket.emit("config_request", {});
-  </script>
-</body>
-
-</html>
+<!DOCTYPE html>
+<html>
+
+<head>
+  <title>Lidia RPC task</title>
+  <link rel="stylesheet" href="static/style.css" />
+  <script src="static/socket.io.js"></script>
+</head>
+
+<body>
+  <svg id="mainSvg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 2100 1200" preserveAspectRatio="xMidYMid meet">
+    <defs>
+      <path id="bottomTriangle" stroke-width="2" d="m0,0 l-34.64,60 h69.28 z" />
+      <path id="star" fill="#f74afd" stroke-width="2" d="M25,0 L9,9 L0,25 L-9,9 L-25,0 L-9,-9 L0,-25 L9,-9 z" />
+      <circle id="pointCircle" cx="0" cy="0" r="23" stroke-width="2" />
+      <path id="axisLimits" d="M-50 -30 v60 M-30 -30 v60 M30 -30 v60 M50 -30 v60" stroke-dasharray="3,3"
+        stroke-width="3" />
+      <path id="borderShort"
+        d="M0,-30 v60 h-5 l-17.32,-10 l17.32,-10 l-17.32,-10 l17.32,-10 l-17.32,-10 l17.32,-10 z" />
+      <!-- The larger width prevents wrapping -->
+      <pattern id="borderGreen" x="0" y="0" width="1.1" height=".06">
+        <use href="#borderShort" fill="#0f0" transform="translate(22.32 30)" />
+      </pattern>
+      <pattern id="borderRed" x="0" y="0" width="1.1" height=".06">
+        <use href="#borderShort" fill="#f00" transform="translate(22.32 30)" />
+      </pattern>
+      <rect id="borderLong" x="-22.32" y="-1000" width="22.32" height="1000" />
+    </defs>
+    <rect width="2150" height="1250" x="-25" y="-25" fill="#000" />
+    <!-- Region extents -->
+    <!-- <rect width="630" height="1200" x="0" y="0" fill="#700" />
+    <rect width="340" height="1200" x="630" y="0" fill="#070" />
+    <rect width="1130" height="1200" x="970" y="0" fill="#007" /> -->
+    <g id="textRegion" data-extents="0 630 1200 0">
+      <rect width="500" height="500" x="60" y="70" fill="none" stroke="#fff" stroke-width="5" rx="15" />
+      <rect width="150" height="30" x="125" y="55" fill="#000" />
+      <use id="cycFtr" href="#pointCircle" fill="#000" transform="translate(420 150)" />
+      <rect width="500" height="500" x="60" y="630" fill="none" stroke="#fff" stroke-width="5" rx="15" />
+      <rect width="225" height="30" x="125" y="615" fill="#000" />
+      <use id="collFtr" href="#pointCircle" fill="#000" transform="translate(420 710)" />
+      <text fill="#fff" font-size="50">
+        <tspan x="130" y="80" font-size="30">CYCLIC</tspan>
+        <tspan x="125" y="170">FTR</tspan>
+        <tspan x="125" y="245">LON POS</tspan>
+        <tspan id="cycLonPercent" x="400" y="245">0</tspan>
+        <tspan x="495" y="245">%</tspan>
+        <tspan x="125" y="320">LAT POS</tspan>
+        <tspan id="cycLatPercent" x="400" y="320">0</tspan>
+        <tspan x="495" y="320">%</tspan>
+        <tspan x="130" y="640" font-size="30">COLLECTIVE</tspan>
+        <tspan x="125" y="730">FTR</tspan>
+        <tspan x="125" y="805">POS</tspan>
+        <tspan id="collPercent" x="400" y="805">0</tspan>
+        <tspan x="495" y="805">%</tspan>
+      </text>
+    </g>
+    <g id="collectiveRegion" stroke="#fff" data-extents="0 970 1200 630">
+      <g id="collOrigin" transform="translate(805 1075) rotate(270)">
+        <rect id="collBackground" width="1000" height="60" x="0" y="-30" />
+        <use href="#collBackground" fill="#4d4d4d" stroke-width="5" />
+        <clipPath id="collClip">
+          <use href="#collBackground" />
+        </clipPath>
+
+        <use id="collBoundaryLow" href="#borderShort" fill="#0f0" stroke="none" display="none" />
+        <g id="collBoundaryHigh" fill="#0f0" stroke="none" display="none" transform="translate(1000)">
+          <use href="#borderShort" transform="scale(-1 1)" />
+        </g>
+        <g transform="translate(0 -30)">
+          <g id="collTrimIndicator">
+            <use href="#bottomTriangle" fill="#02f7fa" transform="scale(1 -1)" />
+            <path fill=" none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v60" />
+          </g>
+        </g>
+        <use href="#star" id="collTargetIndicator" />
+        <g clip-path="url(#collClip)">
+          <use id="collTargetLimits" href="#axisLimits" />
+        </g>
+        <g transform="translate(0 30)">
+          <use id="collInputIndicator" href="#bottomTriangle" fill="#f00" />
+        </g>
+      </g>
+    </g>
+    <g id="cyclicRegion" stroke="#fff" data-extents="0 2100 1200 970">
+      <g id="cycOrigin" transform="translate(1525 575)">
+        <rect id="cycBackground" width="1000" height="1000" x="-500" y="-500" />
+        <use href="#cycBackground" fill="#4d4d4d" stroke-width="5" />
+        <clipPath id="cycClip">
+          <use href="#cycBackground" />
+        </clipPath>
+
+        <g id="cycLatOrigin" transform="translate(0 500)">
+          <g id="cycLatTrimIndicator">
+            <path fill="none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v-1000" />
+            <use href="#bottomTriangle" fill="#02f7fa" />
+          </g>
+          <use id="cycBoundaryLeft" href="#borderLong" fill="url(#borderGreen)" stroke="none" display="none"
+            transform="translate(-500)" />
+          <g id="cycBoundaryRight" fill="url(#borderGreen)" stroke="none" display="none" transform="translate(500)">
+            <use href="#borderLong" transform="scale(-1 1)" />
+          </g>
+        </g>
+        <g id="cycLonOrigin" transform="translate(500 0) rotate(90) scale(1 -1)">
+          <g id="cycLonTrimIndicator">
+            <path fill=" none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v-1000" />
+            <use href="#bottomTriangle" fill="#02f7fa" />
+          </g>
+          <use id="cycBoundaryLow" href="#borderLong" fill="url(#borderGreen)" stroke="none" display="none"
+            transform="translate(-500)" />
+          <g id="cycBoundaryHigh" fill="url(#borderGreen)" stroke="none" display="none" transform="translate(500)">
+            <use href="#borderLong" transform="scale(-1 1)" />
+          </g>
+        </g>
+        <use href="#star" id="cycTargetIndicator" />
+        <g clip-path="url(#cycClip)">
+          <g id="cycTargetLimits" fill="none" stroke-dasharray="3,3" stroke-width="3">
+            <circle id="cycLimitCorrect" cx="0" cy="0" r="30" />
+            <circle id="cycLimitWarning" cx="0" cy="0" r="50" />
+          </g>
+        </g>
+        <use id="cycInputIndicator" href="#pointCircle" fill="#f00" />
+      </g>
+    </g>
+    <g id="rudderRegion" stroke="#fff" data-extents="1200 2100 1560 970">
+      <g id="ruddOrigin" transform="translate(1525 1295)">
+        <rect id="ruddBackground" width="1000" height="60" x="-500" y="-30" />
+        <use href="#ruddBackground" fill="#4d4d4d" stroke-width="5" />
+        <clipPath id="ruddClip">
+          <use href="#ruddBackground" />
+        </clipPath>
+
+        <use id="ruddBoundaryLeft" href="#borderShort" fill="#0f0" stroke="none" display="none" />
+        <g id="ruddBoundaryRight" fill="#0f0" stroke="none" display="none" transform="translate(1000)">
+          <use href="#borderShort" transform="scale(-1 1)" />
+        </g>
+        <g transform="translate(0 30)">
+          <g id="ruddTrimIndicator">
+            <use href="#bottomTriangle" fill="#02f7fa" />
+            <path fill=" none" stroke-dasharray="12,12" stroke-width="4" d="M0,0 v-60" />
+          </g>
+        </g>
+        <use href="#star" id="ruddTargetIndicator" />
+        <g clip-path="url(#ruddClip)">
+          <use href="#axisLimits" id="ruddTargetLimits" />
+        </g>
+        <g transform="translate(0 -30) scale(1 -1)">
+          <use id="ruddInputIndicator" href="#bottomTriangle" fill="#f00" />
+        </g>
+      </g>
+    </g>
+  </svg>
+  <script src="static/controls.js"></script>
+  <script type="text/javascript">
+    let svgElem = document.getElementById("mainSvg");
+    addControls(svgElem);
+  </script>
+  <script type="text/javascript">
+    var socket = io();
+
+    socket.on("echo", (s) => {
+      console.log(s);
+    });
+  </script>
+  <script type="text/javascript">
+    var socket = io();
+    var config = {
+      correct_tolerance: 0.03,
+      warning_tolerance: 0.05,
+    };
+
+    function errorFill(difference) {
+      var e = Math.abs(difference);
+      if (e <= config.correct_tolerance) return "#0f0";
+      else if (e <= config.warning_tolerance) return "#ff0";
+      else return "#f00";
+    }
+
+    function limitRange(elem, oneSided = false) {
+      const outsideLimit = 10;
+      let rangeMin = oneSided ? 0 : -500;
+      let rangeMax = oneSided ? 1000 : 500;
+      let x = elem.transform.baseVal.getItem(0).matrix.e;
+      let y = elem.transform.baseVal.getItem(0).matrix.f;
+
+      // Clamp translate
+      elem.transform.baseVal.getItem(0).matrix.e = Math.max(
+        rangeMin - outsideLimit,
+        Math.min(rangeMax + outsideLimit, x)
+      );
+      elem.transform.baseVal.getItem(0).matrix.f = Math.max(
+        rangeMin - outsideLimit,
+        Math.min(rangeMax + outsideLimit, y)
+      );
+
+      let inside = x >= rangeMin && x <= rangeMax && y >= rangeMin && y <= rangeMax;
+      elem.style.stroke = inside ? "inherit" : "#f00";
+    }
+
+    const collInput = document.getElementById("collInputIndicator");
+    const cycInput = document.getElementById("cycInputIndicator");
+    const ruddInput = document.getElementById("ruddInputIndicator");
+    const collPercent = document.getElementById("collPercent");
+    const cycLatPercent = document.getElementById("cycLatPercent");
+    const cycLonPercent = document.getElementById("cycLonPercent");
+    function updateControl(s) {
+      collInput.setAttribute("transform", `translate(${s.ctrl[4] * 1000})`);
+      limitRange(collInput, true);
+      cycInput.setAttribute("transform", `translate(${s.ctrl[0] * 500} ${s.ctrl[1] * 500})`);
+      limitRange(cycInput);
+      ruddInput.setAttribute("transform", `translate(${s.ctrl[3] * 500})`);
+      limitRange(ruddInput);
+
+      collPercent.textContent = Math.round(s.ctrl[4] * 100);
+      // Goes from 0% on the left and 100% on the right instead of -1 to +1
+      cycLatPercent.textContent = Math.round((s.ctrl[0] + 1) * 50);
+      // Same as roll, but reversed: 0% is pulling the stick to +1
+      cycLonPercent.textContent = Math.round((1 - s.ctrl[1]) * 50);
+    }
+
+    const collTarget = document.getElementById("collTargetIndicator");
+    const collTargetLimits = document.getElementById("collTargetLimits");
+    const cycTarget = document.getElementById("cycTargetIndicator");
+    const cycTargetLimits = document.getElementById("cycTargetLimits");
+    const ruddTarget = document.getElementById("ruddTargetIndicator");
+    const ruddTargetLimits = document.getElementById("ruddTargetLimits");
+    function updateTarget(s) {
+      collTarget.setAttribute("transform", `translate(${s.trgt.ctrl[4] * 1000})`);
+      limitRange(collTarget, true);
+      cycTarget.setAttribute("transform", `translate(${s.trgt.ctrl[0] * 500} ${s.trgt.ctrl[1] * 500})`);
+      limitRange(cycTarget);
+      ruddTarget.setAttribute("transform", `translate(${s.trgt.ctrl[3] * 500})`);
+      limitRange(ruddTarget);
+
+      collTargetLimits.setAttribute("transform", `translate(${s.trgt.ctrl[4] * 1000})`);
+      cycTargetLimits.setAttribute("transform", `translate(${s.trgt.ctrl[0] * 500} ${s.trgt.ctrl[1] * 500})`);
+      ruddTargetLimits.setAttribute("transform", `translate(${s.trgt.ctrl[3] * 500})`);
+
+      if ("ctrl" in s) {
+        collInput.style.fill = errorFill(s.ctrl[4] - s.trgt.ctrl[4]);
+        // The error is defined in terms of percent of range and these go -1 to +1, so divide by 2
+        cycInput.style.fill = errorFill(
+          Math.sqrt(Math.pow(s.ctrl[0] - s.trgt.ctrl[0], 2) + Math.pow(s.ctrl[1] - s.trgt.ctrl[1], 2)) / 2
+        );
+        ruddInput.style.fill = errorFill((s.ctrl[3] - s.trgt.ctrl[3]) / 2);
+      }
+    }
+
+    const collTrim = document.getElementById("collTrimIndicator");
+    const cycLatTrim = document.getElementById("cycLatTrimIndicator");
+    const cycLonTrim = document.getElementById("cycLonTrimIndicator");
+    const ruddTrim = document.getElementById("ruddTrimIndicator");
+    function updateTrim(s) {
+      collTrim.setAttribute("transform", `translate(${s.trim.ctrl[4] * 1000})`);
+      limitRange(collTrim, true);
+      cycLatTrim.setAttribute("transform", `translate(${s.trim.ctrl[0] * 500})`);
+      limitRange(cycLatTrim);
+      cycLonTrim.setAttribute("transform", `translate(${s.trim.ctrl[1] * 500})`);
+      limitRange(cycLonTrim);
+      ruddTrim.setAttribute("transform", `translate(${s.trim.ctrl[3] * 500})`);
+      limitRange(ruddTrim);
+    }
+
+    const collBoundaryLow = document.getElementById("collBoundaryLow");
+    const collBoundaryHigh = document.getElementById("collBoundaryHigh");
+    const cycBoundaryLow = document.getElementById("cycBoundaryLow");
+    const cycBoundaryHigh = document.getElementById("cycBoundaryHigh");
+    const cycBoundaryLeft = document.getElementById("cycBoundaryLeft");
+    const cycBoundaryRight = document.getElementById("cycBoundaryRight");
+    const ruddBoundaryLeft = document.getElementById("ruddBoundaryLeft");
+    const ruddBoundaryRight = document.getElementById("ruddBoundaryRight");
+    function updateBorderPair(input, lowBdr, highBdr, lowRef, highRef, oneSided = false, pattern = false) {
+      if (lowBdr === (oneSided ? 0.0 : -1.0) && highBdr === 1.0) {
+        lowRef.style.display = "none";
+        highRef.style.display = "none";
+        return;
+      } else {
+        lowRef.style.display = "block";
+        highRef.style.display = "block";
+      }
+
+      lowRef.setAttribute("transform", `translate(${lowBdr * (oneSided ? 1000 : 500)})`);
+      highRef.setAttribute("transform", `translate(${highBdr * (oneSided ? 1000 : 500)})`);
+
+      if (input < lowBdr) lowRef.style.fill = pattern ? "url(#borderRed)" : "#f00";
+      else lowRef.style.fill = pattern ? "url(#borderGreen)" : "#0f0";
+      if (input > highBdr) highRef.style.fill = pattern ? "url(#borderRed)" : "#f00";
+      else highRef.style.fill = pattern ? "url(#borderGreen)" : "#0f0";
+    }
+    function updateBorders(s) {
+      updateBorderPair(s.ctrl[4], s.brdr.low[4], s.brdr.high[4], collBoundaryLow, collBoundaryHigh, true);
+      updateBorderPair(s.ctrl[0], s.brdr.low[0], s.brdr.high[0], cycBoundaryLeft, cycBoundaryRight, false, true);
+      updateBorderPair(s.ctrl[1], s.brdr.low[1], s.brdr.high[1], cycBoundaryLow, cycBoundaryHigh, false, true);
+      updateBorderPair(s.ctrl[3], s.brdr.low[3], s.brdr.high[3], ruddBoundaryLeft, ruddBoundaryRight, false, false);
+    }
+
+    const collFtr = document.getElementById("collFtr");
+    const cycFtr = document.getElementById("cycFtr");
+    function updateButtons(s) {
+      cycFtr.style.fill = s.btn[0] & (1 << 0) ? "#ff0" : "#000";
+      collFtr.style.fill = s.btn[0] & (1 << 1) ? "#ff0" : "#000";
+    }
+
+    function updateLimits() {
+      let correct = config.correct_tolerance * 1000;
+      let warning = config.warning_tolerance * 1000;
+      document.getElementById("axisLimits").setAttribute("d",
+        `M-${warning} -30 v60 M-${correct} -30 v60 M${correct} -30 v60 M${warning} -30 v60`);
+      document.getElementById("cycLimitCorrect").setAttribute("r", correct);
+      document.getElementById("cycLimitWarning").setAttribute("r", warning);
+    }
+
+    socket.on("smol", (s) => {
+      if ("ctrl" in s) updateControl(s);
+      if ("trgt" in s) updateTarget(s);
+      if ("trim" in s) updateTrim(s);
+      if ("brdr" in s) updateBorders(s);
+      if ("btn" in s) updateButtons(s);
+    });
+    socket.on("config", (c) => {
+      if ("rpctask" in c) {
+        config = c.rpctask;
+        updateLimits();
+      }
+    });
+    socket.emit("config_request", {});
+  </script>
+</body>
+
+</html>
```

### Comparing `lidia-0.8.0/src/lidia/server.py` & `lidia-0.8.1/src/lidia/server.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from argparse import Namespace
-import queue
-import eventlet
-from msgpack import packb
-from multiprocessing import Queue
-from os import path
-import socket
-import socketio
-
-
-from .config import Config
-
-
-def background_loop(q: Queue, sio: socketio.Server, args: Namespace):
-    udp_host, udp_port = args.passthrough_host, args.passthrough_port
-    udp_sock = None
-    if udp_host is not None and udp_port is not None:
-        udp_sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-
-    while True:
-        try:
-            while not q.empty():
-                event, data = q.get()
-                sio.emit(event, data)
-                if args.verbosity >= 2:
-                    print(f"socketio.emit('{event}', {data})")
-                if event == 'smol' and udp_sock is not None:
-                    sent_len = udp_sock.sendto(
-                        packb(data), (udp_host, udp_port))
-                    if args.verbosity >= 2:
-                        print(
-                            f"sent {sent_len} bytes to udp:{udp_host}:{udp_port}")
-        except queue.Empty:
-            pass
-        eventlet.sleep(0.02)
-
-
-def run_server(q: Queue, args: Namespace, config: Config):
-    # specifying just local path breaks when run as a module
-    root_path = path.abspath(path.dirname(__file__))
-    static_files = {
-        '/': {'content_type': 'text/html', 'filename': path.join(root_path, 'rpctask.html')},
-        '/info': {'content_type': 'text/html', 'filename': path.join(root_path, 'info.html')},
-        '/rpctask': {'content_type': 'text/html', 'filename': path.join(root_path, 'rpctask.html')},
-        '/pfd': {'content_type': 'text/html', 'filename': path.join(root_path, 'pfd.html')},
-        '/approach': {'content_type': 'text/html', 'filename': path.join(root_path, 'approach.html')},
-        '/static': path.join(root_path, 'static'),
-    }
-
-    sio = socketio.Server()
-
-    @sio.on('config_request')
-    def config_request(_sid, _environ):
-        q.put(('config', config.dict()))
-
-    app = socketio.WSGIApp(sio, static_files=static_files)
-    eventlet.spawn(background_loop, q, sio, args)
-    eventlet.wsgi.server(eventlet.listen((args.http_host, args.http_port)),
-                         app, log_output=args.verbosity >= 3)
+from argparse import Namespace
+import queue
+import eventlet
+from msgpack import packb
+from multiprocessing import Queue
+from os import path
+import socket
+import socketio
+
+
+from .config import Config
+
+
+def background_loop(q: Queue, sio: socketio.Server, args: Namespace):
+    udp_host, udp_port = args.passthrough_host, args.passthrough_port
+    udp_sock = None
+    if udp_host is not None and udp_port is not None:
+        udp_sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+
+    while True:
+        try:
+            while not q.empty():
+                event, data = q.get()
+                sio.emit(event, data)
+                if args.verbosity >= 2:
+                    print(f"socketio.emit('{event}', {data})")
+                if event == 'smol' and udp_sock is not None:
+                    sent_len = udp_sock.sendto(
+                        packb(data), (udp_host, udp_port))
+                    if args.verbosity >= 2:
+                        print(
+                            f"sent {sent_len} bytes to udp:{udp_host}:{udp_port}")
+        except queue.Empty:
+            pass
+        eventlet.sleep(0.02)
+
+
+def run_server(q: Queue, args: Namespace, config: Config):
+    # specifying just local path breaks when run as a module
+    root_path = path.abspath(path.dirname(__file__))
+    static_files = {
+        '/': {'content_type': 'text/html', 'filename': path.join(root_path, 'rpctask.html')},
+        '/info': {'content_type': 'text/html', 'filename': path.join(root_path, 'info.html')},
+        '/rpctask': {'content_type': 'text/html', 'filename': path.join(root_path, 'rpctask.html')},
+        '/pfd': {'content_type': 'text/html', 'filename': path.join(root_path, 'pfd.html')},
+        '/approach': {'content_type': 'text/html', 'filename': path.join(root_path, 'approach.html')},
+        '/static': path.join(root_path, 'static'),
+    }
+
+    sio = socketio.Server()
+
+    @sio.on('config_request')
+    def config_request(_sid, _environ):
+        q.put(('config', config.dict()))
+
+    app = socketio.WSGIApp(sio, static_files=static_files)
+    eventlet.spawn(background_loop, q, sio, args)
+    eventlet.wsgi.server(eventlet.listen((args.http_host, args.http_port)),
+                         app, log_output=args.verbosity >= 3)
```

### Comparing `lidia-0.8.0/src/lidia/sources/approach.py` & `lidia-0.8.1/src/lidia/sources/approach.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""listen to UDP packets from RPC simulator for approach task"""
-from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
-from multiprocessing import Queue
-import socket
-from struct import unpack_from
-from typing import Tuple
-
-from ..aircraft import *
-from ..config import Config
-from .mytypes import RunFn
-
-
-def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
-    NAME = 'approach'
-    parser: ArgumentParser = subparsers.add_parser(
-        NAME,
-        help=__doc__,
-        formatter_class=ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-i', '--ip',
-                        help='listen UDP adress', default='0.0.0.0')
-    parser.add_argument('-p', '--port', type=int,
-                        help='listen UDP port', default=5004)
-
-    return (NAME, run)
-
-
-def run(q: Queue, args: Namespace, config: Config):
-    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
-        # Timeout is required to handle leaving with Ctrl+C
-        sock.settimeout(1.0)
-        sock.bind((args.ip, args.port))
-        if args.verbosity >= 0:
-            print(f'Listening for UDP packets on {args.ip}:{args.port}')
-
-        while True:
-            try:
-                data, _ = sock.recvfrom(1024)
-                # Contents of UDP packet is 4 doubles:
-                # - Position of helicopter north of ship, in meters
-                # - Position of helicopter east of ship, in meters
-                # - Position of helicopter above  ship, in meters
-                # - Helicopter heading, in radians
-                #   - 0 pointing north, pi/2 (90⁰) pointing east
-                (north, east, altitude, yaw) = unpack_from('>' + 'd' * 4, data)
-
-                state = AircraftState()
-                state.ned = NED()
-                state.ned.north = north
-                state.ned.east = east
-                state.ned.down = -altitude
-                state.att = Attitude()
-                state.att.yaw = yaw
-                state.model_instruments(config)
-                state.set_time(config)
-
-                q.put(('smol', state.smol()))
-            except socket.timeout:
-                continue
+"""listen to UDP packets from RPC simulator for approach task"""
+from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
+from multiprocessing import Queue
+import socket
+from struct import unpack_from
+from typing import Tuple
+
+from ..aircraft import *
+from ..config import Config
+from .mytypes import RunFn
+
+
+def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
+    NAME = 'approach'
+    parser: ArgumentParser = subparsers.add_parser(
+        NAME,
+        help=__doc__,
+        formatter_class=ArgumentDefaultsHelpFormatter)
+    parser.add_argument('-i', '--ip',
+                        help='listen UDP adress', default='0.0.0.0')
+    parser.add_argument('-p', '--port', type=int,
+                        help='listen UDP port', default=5004)
+
+    return (NAME, run)
+
+
+def run(q: Queue, args: Namespace, config: Config):
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
+        # Timeout is required to handle leaving with Ctrl+C
+        sock.settimeout(1.0)
+        sock.bind((args.ip, args.port))
+        if args.verbosity >= 0:
+            print(f'Listening for UDP packets on {args.ip}:{args.port}')
+
+        while True:
+            try:
+                data, _ = sock.recvfrom(1024)
+                # Contents of UDP packet is 4 doubles:
+                # - Position of helicopter north of ship, in meters
+                # - Position of helicopter east of ship, in meters
+                # - Position of helicopter above  ship, in meters
+                # - Helicopter heading, in radians
+                #   - 0 pointing north, pi/2 (90⁰) pointing east
+                (north, east, altitude, yaw) = unpack_from('>' + 'd' * 4, data)
+
+                state = AircraftState()
+                state.ned = NED()
+                state.ned.north = north
+                state.ned.east = east
+                state.ned.down = -altitude
+                state.att = Attitude()
+                state.att.yaw = yaw
+                state.model_instruments(config)
+                state.set_time(config)
+
+                q.put(('smol', state.smol()))
+            except socket.timeout:
+                continue
```

### Comparing `lidia-0.8.0/src/lidia/sources/confighelp.md` & `lidia-0.8.1/src/lidia/sources/confighelp.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Lidia config help
-
-The structure of configuration object is defined as the `Config` class in config.py file.
-
-## Config files
-
-Every time a configuration file is passed, fields in config objects are copied and then overwritten by the config file. This means there is no need to provide every property, only the ones to be changed.
-
-In case more than one file is passed, the first will be applied on top of defaults, and then the latter will override any present values, either left as default, or from first the file.
-
-To prevent silently failing in case of a mistyped key, every property is validated, both for name and type. To help with writing configuration, template files can be generated for each supported format by using this source. The template includes address of the JSON Schema file that describes the structure, allowing a text editor to provide hints. You need to run the confighelp source at least once to generate the schema (the schema generation requires `pydantic` so it isn't part of package build).
-
-By default the schema URL contains full path to the installed data folder. When sharing the configuration files, you might want to set it to:
-
-- local path relative to config file, like "lidia-config.json" if they are in same directory. (note lack of `file:` prefix)
-
-## Config-keys argument
-
-After all config files are processed, values can be overriden using CLI arguments. To do that pass a set of properties like
-
-```
-group.innergroup.value="string value, in quotes",group.innergroup.value2=2.0
-```
+# Lidia config help
+
+The structure of configuration object is defined as the `Config` class in config.py file.
+
+## Config files
+
+Every time a configuration file is passed, fields in config objects are copied and then overwritten by the config file. This means there is no need to provide every property, only the ones to be changed.
+
+In case more than one file is passed, the first will be applied on top of defaults, and then the latter will override any present values, either left as default, or from first the file.
+
+To prevent silently failing in case of a mistyped key, every property is validated, both for name and type. To help with writing configuration, template files can be generated for each supported format by using this source. The template includes address of the JSON Schema file that describes the structure, allowing a text editor to provide hints. You need to run the confighelp source at least once to generate the schema (the schema generation requires `pydantic` so it isn't part of package build).
+
+By default the schema URL contains full path to the installed data folder. When sharing the configuration files, you might want to set it to:
+
+- local path relative to config file, like "lidia-config.json" if they are in same directory. (note lack of `file:` prefix)
+
+## Config-keys argument
+
+After all config files are processed, values can be overriden using CLI arguments. To do that pass a set of properties like
+
+```
+group.innergroup.value="string value, in quotes",group.innergroup.value2=2.0
+```
```

### Comparing `lidia-0.8.0/src/lidia/sources/demo.py` & `lidia-0.8.1/src/lidia/sources/demo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,133 @@
-"""looping simulation demonstrating GUI"""
-from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentError, ArgumentParser, Namespace
-from math import pi, sin
-from multiprocessing import Queue
-from time import sleep, time
-from typing import Tuple
-
-from ..aircraft import *
-from ..config import Config
-from .mytypes import RunFn
-
-
-def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
-    NAME = 'demo'
-    parser: ArgumentParser = subparsers.add_parser(
-        NAME,
-        help=__doc__,
-        formatter_class=ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-T', '--period', type=float,
-                        help='loop time in seconds', default=5.0)
-    parser.add_argument('-f', '--frequency', type=float,
-                        help='number of messages sent per second', default=30.0)
-    parser.add_argument('--no-trim', action='store_false', dest='trim',
-                        help='do not demonstrate trim function')
-    parser.add_argument('--no-borders', action='store_false', dest='borders',
-                        help='do not demonstrate borders function')
-    parser.add_argument('--outside-range', action='store_true',
-                        help='demonstrate values outside allowed range')
-    parser.add_argument('--alt-zero', type=float,
-                        help='altitude to hover around', default=65.0)
-    parser.add_argument('--alt-change', type=float,
-                        help='altitude change amplitude', default=10.0)
-
-    return (NAME, run)
-
-
-def run(q: Queue, args: Namespace, config: Config):
-    if args.period <= 0:
-        raise ArgumentError(args.frequency, 'period must be positive')
-    if args.frequency <= 0:
-        raise ArgumentError(args.frequency, 'frequency must be positive')
-
-    outside_offset = 0.6 if args.outside_range else 0.0
-
-    def val(phase):
-        """Generate a sinusoidal value with phase offset (from 0 to 1)"""
-        return 0.6 * sin((time() / args.period + phase) * 2 * pi) + outside_offset
-
-    def cycle_index(): return int(time() // args.period) % 3
-    def current_phase(): return (time() / args.period) % 1
-
-    last_trim = Controls()
-    last_v_ned = NED()
-    last_time = time()
-
-    while True:
-        state = AircraftState()
-        state.ned = NED()
-        state.ned.down = -args.alt_zero - args.alt_change * val(0.75)
-
-        state.att = Attitude()
-        state.att.pitch = 0.5 * val(0)
-        state.att.roll = 0.5 * val(0.25)
-        state.att.yaw = 0.5 * val(0.5)
-
-        state.v_body = XYZ()
-        state.v_body.x = 15 + 2.5 * val(0.5)
-        state.v_body.y = 1 * val(0.65)
-        state.v_body.z = 2 * val(0.25)
-
-        state.v_ned = state.xyz2ned(state.v_body)
-
-        dt = time() - last_time
-        state.a_ned = NED(down=9.81) + (state.v_ned - last_v_ned) / dt
-        # a_body is simulated by instruments model if it's unset
-        last_v_ned = state.v_ned
-        last_time = time()
-
-        state.ctrl = Controls()
-        state.ctrl.stick_pull = val(0.1)
-        state.ctrl.stick_right = val(0.35)
-        state.ctrl.pedals_right = val(0.6)
-        state.ctrl.collective_up = 0.3 + 0.5 * (val(0.2) + outside_offset)
-
-        state.trgt = AircraftData()
-        state.trgt.ctrl = Controls()
-        state.trgt.ctrl.stick_pull = val(0.55)
-        state.trgt.ctrl.stick_right = val(0.3)
-        state.trgt.ctrl.pedals_right = val(0.5)
-        state.trgt.ctrl.collective_up = 0.3 + 0.5 * (val(0.4) + outside_offset)
-        state.trgt.att = Attitude()
-        state.trgt.att.roll = 0.3 * val(0.35)
-        state.trgt.att.pitch = 0.3 * val(0.1)
-
-        state.btn = Buttons()
-        if cycle_index() == 1 and args.trim:
-            if current_phase() < 0.4:
-                state.btn.coll_ftr = True
-            if current_phase() > 0.6:
-                state.btn.cyc_ftr = True
-
-        if state.btn.coll_ftr:
-            last_trim.collective_up = state.ctrl.collective_up
-        if state.btn.cyc_ftr:
-            last_trim.stick_right = state.ctrl.stick_right
-            last_trim.stick_pull = state.ctrl.stick_pull
-        state.trim = AircraftData()
-        state.trim.ctrl = last_trim
-
-        state.brdr = Borders()
-        if cycle_index() == 2 and args.borders:
-            if current_phase() < 0.5:
-                state.brdr.low = Controls.from_list(
-                    [-0.8, -0.8, 0.1, -0.8, 0.1])
-                state.brdr.high = Controls.from_list(
-                    [0.8, 0.8, 0.9, 0.8, 0.9])
-            if current_phase() > 0.5:
-                state.brdr.low = Controls.from_list(
-                    [-0.5, -0.5, 0.25, -0.5, 0.25])
-                state.brdr.high = Controls.from_list(
-                    [0.5, 0.5, 0.75, 0.5, 0.75])
-
-        state.model_instruments(config)
-        if cycle_index() == 0:
-            state.instr.gs = None
-            state.instr.ralt = None
-        else:
-            state.instr.qnh = None
-        state.set_time(config)
-
-        q.put(('smol', state.smol()))
-        sleep(1 / args.frequency)
+"""looping simulation demonstrating GUI"""
+from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentError, ArgumentParser, Namespace
+from math import pi, sin
+from multiprocessing import Queue
+from time import sleep, time
+from typing import Tuple
+
+from ..aircraft import *
+from ..config import Config
+from .mytypes import RunFn
+
+
+def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
+    NAME = 'demo'
+    parser: ArgumentParser = subparsers.add_parser(
+        NAME,
+        help=__doc__,
+        formatter_class=ArgumentDefaultsHelpFormatter)
+    parser.add_argument('-T', '--period', type=float,
+                        help='loop time in seconds', default=5.0)
+    parser.add_argument('-f', '--frequency', type=float,
+                        help='number of messages sent per second', default=30.0)
+    parser.add_argument('--no-trim', action='store_false', dest='trim',
+                        help='do not demonstrate trim function')
+    parser.add_argument('--no-borders', action='store_false', dest='borders',
+                        help='do not demonstrate borders function')
+    parser.add_argument('--outside-range', action='store_true',
+                        help='demonstrate values outside allowed range')
+    parser.add_argument('--alt-zero', type=float,
+                        help='altitude to hover around', default=65.0)
+    parser.add_argument('--alt-change', type=float,
+                        help='altitude change amplitude', default=10.0)
+
+    return (NAME, run)
+
+
+def run(q: Queue, args: Namespace, config: Config):
+    if args.period <= 0:
+        raise ArgumentError(args.frequency, 'period must be positive')
+    if args.frequency <= 0:
+        raise ArgumentError(args.frequency, 'frequency must be positive')
+
+    outside_offset = 0.6 if args.outside_range else 0.0
+
+    def val(phase):
+        """Generate a sinusoidal value with phase offset (from 0 to 1)"""
+        return 0.6 * sin((time() / args.period + phase) * 2 * pi) + outside_offset
+
+    def cycle_index(): return int(time() // args.period) % 3
+    def current_phase(): return (time() / args.period) % 1
+
+    last_trim = Controls()
+    last_v_ned = NED()
+    # prevent zero division on first iteration
+    last_time = time() - 1 / args.frequency
+
+    while True:
+        state = AircraftState()
+        state.ned = NED()
+        state.ned.down = -args.alt_zero - args.alt_change * val(0.75)
+
+        state.att = Attitude()
+        state.att.pitch = 0.5 * val(0)
+        state.att.roll = 0.5 * val(0.25)
+        state.att.yaw = 0.5 * val(0.5)
+
+        state.v_body = XYZ()
+        state.v_body.x = 15 + 2.5 * val(0.5)
+        state.v_body.y = 1 * val(0.65)
+        state.v_body.z = 2 * val(0.25)
+
+        state.v_ned = state.xyz2ned(state.v_body)
+
+        dt = time() - last_time
+        state.a_ned = NED(down=9.81) + (state.v_ned - last_v_ned) / dt
+        # a_body is simulated by instruments model if it's unset
+        last_v_ned = state.v_ned
+        last_time = time()
+
+        state.ctrl = Controls()
+        state.ctrl.stick_pull = val(0.1)
+        state.ctrl.stick_right = val(0.35)
+        state.ctrl.pedals_right = val(0.6)
+        state.ctrl.collective_up = 0.3 + 0.5 * (val(0.2) + outside_offset)
+
+        state.trgt = AircraftData()
+        state.trgt.ctrl = Controls()
+        state.trgt.ctrl.stick_pull = val(0.55)
+        state.trgt.ctrl.stick_right = val(0.3)
+        state.trgt.ctrl.pedals_right = val(0.5)
+        state.trgt.ctrl.collective_up = 0.3 + 0.5 * (val(0.4) + outside_offset)
+        state.trgt.att = Attitude()
+        state.trgt.att.roll = 0.3 * val(0.35)
+        state.trgt.att.pitch = 0.3 * val(0.1)
+
+        state.btn = Buttons()
+        if cycle_index() == 1 and args.trim:
+            if current_phase() < 0.4:
+                state.btn.coll_ftr = True
+            if current_phase() > 0.6:
+                state.btn.cyc_ftr = True
+
+        if state.btn.coll_ftr:
+            last_trim.collective_up = state.ctrl.collective_up
+        if state.btn.cyc_ftr:
+            last_trim.stick_right = state.ctrl.stick_right
+            last_trim.stick_pull = state.ctrl.stick_pull
+        state.trim = AircraftData()
+        state.trim.ctrl = last_trim
+
+        state.brdr = Borders()
+        if cycle_index() == 2 and args.borders:
+            if current_phase() < 0.5:
+                state.brdr.low = Controls.from_list(
+                    [-0.8, -0.8, 0.1, -0.8, 0.1])
+                state.brdr.high = Controls.from_list(
+                    [0.8, 0.8, 0.9, 0.8, 0.9])
+            if current_phase() > 0.5:
+                state.brdr.low = Controls.from_list(
+                    [-0.5, -0.5, 0.25, -0.5, 0.25])
+                state.brdr.high = Controls.from_list(
+                    [0.5, 0.5, 0.75, 0.5, 0.75])
+
+        state.model_instruments(config)
+        if cycle_index() == 0:
+            state.instr.gs = None
+            state.instr.ralt = None
+        else:
+            state.instr.qnh = None
+        state.set_time(config)
+
+        q.put(('smol', state.smol()))
+        sleep(1 / args.frequency)
```

### Comparing `lidia-0.8.0/src/lidia/sources/flightgear.py` & `lidia-0.8.1/src/lidia/sources/flightgear.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""listen to UDP packets from FlightGear native socket protocol"""
-from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
-from multiprocessing import Queue
-import socket
-from typing import Tuple
-
-from ..aircraft import *
-from ..config import Config
-from .mytypes import RunFn, FGNetFDM
-
-
-def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
-    NAME = 'flightgear'
-    parser: ArgumentParser = subparsers.add_parser(
-        NAME,
-        help=__doc__,
-        formatter_class=ArgumentDefaultsHelpFormatter,
-        epilog="""To send packets at 30Hz from a local FlightGear instance,
-add this command line argument: --native-fdm=socket,out,30,127.0.0.1,5004,udp""")
-    parser.add_argument('-i', '--ip',
-                        help='listen UDP adress', default='0.0.0.0')
-    parser.add_argument('-p', '--port', type=int,
-                        help='listen UDP port', default=5004)
-
-    return (NAME, run)
-
-
-def run(q: Queue, args: Namespace, config: Config):
-    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
-        # Timeout is required to handle leaving with Ctrl+C
-        sock.settimeout(1.0)
-        sock.bind((args.ip, args.port))
-        if args.verbosity >= 0:
-            print(f'Listening for UDP packets on {args.ip}:{args.port}')
-
-        while True:
-            try:
-                data, _ = sock.recvfrom(1024)
-                fg = FGNetFDM.from_bytes(data)
-
-                FT = 0.3048
-                """conversion multiplier from feet to meters"""
-
-                state = AircraftState()
-                state.ned = NED()
-                # TODO: Add argument for reference location, calculate north and east from that
-                state.ned.down = -fg.altitude
-                state.att = Attitude()
-                state.att.roll = fg.phi
-                state.att.pitch = fg.theta
-                state.att.yaw = fg.psi
-                # Velocities in ft/s
-                state.v_body = XYZ()
-                state.v_body.x = fg.v_body_u * FT
-                state.v_body.y = fg.v_body_v * FT
-                state.v_body.z = fg.v_body_w * FT
-                state.v_ned = NED()
-                state.v_ned.north = fg.v_north * FT
-                state.v_ned.east = fg.v_east * FT
-                state.v_ned.down = fg.v_down * FT
-                state.ctrl = Controls()
-                state.ctrl.stick_pull = -fg.elevator
-                state.ctrl.stick_right = fg.right_aileron
-                state.ctrl.pedals_right = fg.rudder
-
-                state.model_instruments(config)
-                if state.instr.ralt is not None:
-                    state.instr.ralt = fg.agl * config.instruments.altitude_multiplier
-                state.set_time(config)
-
-                q.put(('smol', state.smol()))
-            except socket.timeout:
-                continue
+"""listen to UDP packets from FlightGear native socket protocol"""
+from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
+from multiprocessing import Queue
+import socket
+from typing import Tuple
+
+from ..aircraft import *
+from ..config import Config
+from .mytypes import RunFn, FGNetFDM
+
+
+def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
+    NAME = 'flightgear'
+    parser: ArgumentParser = subparsers.add_parser(
+        NAME,
+        help=__doc__,
+        formatter_class=ArgumentDefaultsHelpFormatter,
+        epilog="""To send packets at 30Hz from a local FlightGear instance,
+add this command line argument: --native-fdm=socket,out,30,127.0.0.1,5004,udp""")
+    parser.add_argument('-i', '--ip',
+                        help='listen UDP adress', default='0.0.0.0')
+    parser.add_argument('-p', '--port', type=int,
+                        help='listen UDP port', default=5004)
+
+    return (NAME, run)
+
+
+def run(q: Queue, args: Namespace, config: Config):
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
+        # Timeout is required to handle leaving with Ctrl+C
+        sock.settimeout(1.0)
+        sock.bind((args.ip, args.port))
+        if args.verbosity >= 0:
+            print(f'Listening for UDP packets on {args.ip}:{args.port}')
+
+        while True:
+            try:
+                data, _ = sock.recvfrom(1024)
+                fg = FGNetFDM.from_bytes(data)
+
+                FT = 0.3048
+                """conversion multiplier from feet to meters"""
+
+                state = AircraftState()
+                state.ned = NED()
+                # TODO: Add argument for reference location, calculate north and east from that
+                state.ned.down = -fg.altitude
+                state.att = Attitude()
+                state.att.roll = fg.phi
+                state.att.pitch = fg.theta
+                state.att.yaw = fg.psi
+                # Velocities in ft/s
+                state.v_body = XYZ()
+                state.v_body.x = fg.v_body_u * FT
+                state.v_body.y = fg.v_body_v * FT
+                state.v_body.z = fg.v_body_w * FT
+                state.v_ned = NED()
+                state.v_ned.north = fg.v_north * FT
+                state.v_ned.east = fg.v_east * FT
+                state.v_ned.down = fg.v_down * FT
+                state.ctrl = Controls()
+                state.ctrl.stick_pull = -fg.elevator
+                state.ctrl.stick_right = fg.right_aileron
+                state.ctrl.pedals_right = fg.rudder
+
+                state.model_instruments(config)
+                if state.instr.ralt is not None:
+                    state.instr.ralt = fg.agl * config.instruments.altitude_multiplier
+                state.set_time(config)
+
+                q.put(('smol', state.smol()))
+            except socket.timeout:
+                continue
```

### Comparing `lidia-0.8.0/src/lidia/sources/mytypes.py` & `lidia-0.8.1/src/lidia/sources/mytypes.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-from argparse import _SubParsersAction, Namespace
-from multiprocessing import Queue
-from pydantic import BaseModel
-from struct import unpack_from
-from typing import Callable, NoReturn, Tuple
-
-from ..config import Config
-
-RunFn = Callable[[Queue, Namespace, Config], NoReturn]
-SetupFn = Callable[[_SubParsersAction], Tuple[str, RunFn]]
-
-
-FG_NET_FDM_VERSION = 24
-
-
-class FGNetFDM(BaseModel):
-    """FlightGear network communication structure from src/Network/net_fdm.hxx"""
-    version: int = 0
-    """increment when data values change"""
-    padding: int = 0
-    """padding"""
-    longitude: float = 0
-    """geodetic (radians)"""
-    latitude: float = 0
-    """geodetic (radians)"""
-    altitude: float = 0
-    """above sea level (meters)"""
-    agl: float = 0
-    """above ground level (meters)"""
-    phi: float = 0
-    """roll (radians)"""
-    theta: float = 0
-    """pitch (radians)"""
-    psi: float = 0
-    """yaw or true heading (radians)"""
-    alpha: float = 0
-    """angle of attack (radians)"""
-    beta: float = 0
-    """side slip angle (radians)"""
-    phidot: float = 0
-    """roll rate (radians/sec)"""
-    thetadot: float = 0
-    """pitch rate (radians/sec)"""
-    psidot: float = 0
-    """yaw rate (radians/sec)"""
-    vcas: float = 0
-    """calibrated airspeed"""
-    climb_rate: float = 0
-    """feet per second"""
-    v_north: float = 0
-    """north velocity in local/body frame, fps"""
-    v_east: float = 0
-    """east velocity in local/body frame, fps"""
-    v_down: float = 0
-    """down/vertical velocity in local/body frame, fps"""
-    v_body_u: float = 0
-    """ECEF velocity in body frame"""
-    v_body_v: float = 0
-    """ECEF velocity in body frame"""
-    v_body_w: float = 0
-    """ECEF velocity in body frame"""
-    A_X_pilot: float = 0
-    """X accel in body frame ft/sec^2"""
-    A_Y_pilot: float = 0
-    """Y accel in body frame ft/sec^2"""
-    A_Z_pilot: float = 0
-    """Z accel in body frame ft/sec^2"""
-    stall_warning: float = 0
-    """0.0 - 1.0 indicating the amount of stall"""
-    slip_deg: float = 0
-    """slip ball deflection"""
-    num_engines: int = 0
-    """Number of valid engines"""
-    eng_state: Tuple[int, int, int, int] = (0, 0, 0, 0)
-    """Engine state (off, cranking, running)"""
-    rpm: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Engine RPM rev/min"""
-    fuel_flow: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Fuel flow gallons/hr"""
-    fuel_px: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Fuel pressure psi"""
-    egt: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Exhuast gas temp deg F"""
-    cht: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Cylinder head temp deg F"""
-    mp_osi: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Manifold pressure"""
-    tit: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Turbine Inlet Temperature"""
-    oil_temp: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Oil temp deg F"""
-    oil_px: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    """Oil pressure psi"""
-    num_tanks: int = 0
-    """Max number of fuel tanks"""
-    fuel_quantity: Tuple[float, float, float, float] = (0, 0, 0, 0)
-    num_wheels: int = 0
-    wow: Tuple[int, int, int] = (0, 0, 0)
-    gear_pos: Tuple[float, float, float] = (0, 0, 0)
-    gear_steer: Tuple[float, float, float] = (0, 0, 0)
-    gear_compression: Tuple[float, float, float] = (0, 0, 0)
-    cur_time: int = 0
-    """current unix time"""
-    warp: int = 0
-    """offset in seconds to unix time"""
-    visibility: float = 0
-    """visibility in meters (for env. effects)"""
-    elevator: float = 0
-    elevator_trim_tab: float = 0
-    left_flap: float = 0
-    right_flap: float = 0
-    left_aileron: float = 0
-    right_aileron: float = 0
-    rudder: float = 0
-    nose_wheel: float = 0
-    speedbrake: float = 0
-    spoilers: float = 0
-
-    @classmethod
-    def from_bytes(cls, data):
-        version = unpack_from("!I", data)[0]
-        if version != FG_NET_FDM_VERSION:
-            raise ValueError(
-                f"Expected protocol version {FG_NET_FDM_VERSION}, got {version}")
-        this = cls()
-        decoded = unpack_from(
-            "!IIdddffffffffffffffffffffffIIIIIffffffffffffffffffffffffffffffffffffIffffIIIIfffffffffIifffffffffff", data)
-        this.version = decoded[0]
-        this.padding = decoded[1]
-        this.longitude = decoded[2]
-        this.latitude = decoded[3]
-        this.altitude = decoded[4]
-        this.agl = decoded[5]
-        this.phi = decoded[6]
-        this.theta = decoded[7]
-        this.psi = decoded[8]
-        this.alpha = decoded[9]
-        this.beta = decoded[10]
-        this.phidot = decoded[11]
-        this.thetadot = decoded[12]
-        this.psidot = decoded[13]
-        this.vcas = decoded[14]
-        this.climb_rate = decoded[15]
-        this.v_north = decoded[16]
-        this.v_east = decoded[17]
-        this.v_down = decoded[18]
-        this.v_body_u = decoded[19]
-        this.v_body_v = decoded[20]
-        this.v_body_w = decoded[21]
-        this.A_X_pilot = decoded[22]
-        this.A_Y_pilot = decoded[23]
-        this.A_Z_pilot = decoded[24]
-        this.stall_warning = decoded[25]
-        this.slip_deg = decoded[26]
-        this.num_engines = decoded[27]
-        this.eng_state = decoded[28:32]
-        this.rpm = decoded[32:36]
-        this.fuel_flow = decoded[36:40]
-        this.fuel_px = decoded[40:44]
-        this.egt = decoded[44:48]
-        this.cht = decoded[48:52]
-        this.mp_osi = decoded[52:56]
-        this.tit = decoded[56:60]
-        this.oil_temp = decoded[60:64]
-        this.oil_px = decoded[64:68]
-        this.num_tanks = decoded[68]
-        this.fuel_quantity = decoded[69:73]
-        this.num_wheels = decoded[73]
-        this.wow = decoded[74:77]
-        this.gear_pos = decoded[77:80]
-        this.gear_steer = decoded[80:83]
-        this.gear_compression = decoded[83:86]
-        this.cur_time = decoded[86]
-        this.warp = decoded[87]
-        this.visibility = decoded[88]
-        this.elevator = decoded[89]
-        this.elevator_trim_tab = decoded[90]
-        this.left_flap = decoded[91]
-        this.right_flap = decoded[92]
-        this.left_aileron = decoded[93]
-        this.right_aileron = decoded[94]
-        this.rudder = decoded[95]
-        this.nose_wheel = decoded[96]
-        this.speedbrake = decoded[97]
-        this.spoilers = decoded[98]
-        return this
+from argparse import _SubParsersAction, Namespace
+from multiprocessing import Queue
+from pydantic import BaseModel
+from struct import unpack_from
+from typing import Callable, NoReturn, Tuple
+
+from ..config import Config
+
+RunFn = Callable[[Queue, Namespace, Config], NoReturn]
+SetupFn = Callable[[_SubParsersAction], Tuple[str, RunFn]]
+
+
+FG_NET_FDM_VERSION = 24
+
+
+class FGNetFDM(BaseModel):
+    """FlightGear network communication structure from src/Network/net_fdm.hxx"""
+    version: int = 0
+    """increment when data values change"""
+    padding: int = 0
+    """padding"""
+    longitude: float = 0
+    """geodetic (radians)"""
+    latitude: float = 0
+    """geodetic (radians)"""
+    altitude: float = 0
+    """above sea level (meters)"""
+    agl: float = 0
+    """above ground level (meters)"""
+    phi: float = 0
+    """roll (radians)"""
+    theta: float = 0
+    """pitch (radians)"""
+    psi: float = 0
+    """yaw or true heading (radians)"""
+    alpha: float = 0
+    """angle of attack (radians)"""
+    beta: float = 0
+    """side slip angle (radians)"""
+    phidot: float = 0
+    """roll rate (radians/sec)"""
+    thetadot: float = 0
+    """pitch rate (radians/sec)"""
+    psidot: float = 0
+    """yaw rate (radians/sec)"""
+    vcas: float = 0
+    """calibrated airspeed"""
+    climb_rate: float = 0
+    """feet per second"""
+    v_north: float = 0
+    """north velocity in local/body frame, fps"""
+    v_east: float = 0
+    """east velocity in local/body frame, fps"""
+    v_down: float = 0
+    """down/vertical velocity in local/body frame, fps"""
+    v_body_u: float = 0
+    """ECEF velocity in body frame"""
+    v_body_v: float = 0
+    """ECEF velocity in body frame"""
+    v_body_w: float = 0
+    """ECEF velocity in body frame"""
+    A_X_pilot: float = 0
+    """X accel in body frame ft/sec^2"""
+    A_Y_pilot: float = 0
+    """Y accel in body frame ft/sec^2"""
+    A_Z_pilot: float = 0
+    """Z accel in body frame ft/sec^2"""
+    stall_warning: float = 0
+    """0.0 - 1.0 indicating the amount of stall"""
+    slip_deg: float = 0
+    """slip ball deflection"""
+    num_engines: int = 0
+    """Number of valid engines"""
+    eng_state: Tuple[int, int, int, int] = (0, 0, 0, 0)
+    """Engine state (off, cranking, running)"""
+    rpm: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Engine RPM rev/min"""
+    fuel_flow: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Fuel flow gallons/hr"""
+    fuel_px: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Fuel pressure psi"""
+    egt: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Exhuast gas temp deg F"""
+    cht: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Cylinder head temp deg F"""
+    mp_osi: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Manifold pressure"""
+    tit: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Turbine Inlet Temperature"""
+    oil_temp: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Oil temp deg F"""
+    oil_px: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    """Oil pressure psi"""
+    num_tanks: int = 0
+    """Max number of fuel tanks"""
+    fuel_quantity: Tuple[float, float, float, float] = (0, 0, 0, 0)
+    num_wheels: int = 0
+    wow: Tuple[int, int, int] = (0, 0, 0)
+    gear_pos: Tuple[float, float, float] = (0, 0, 0)
+    gear_steer: Tuple[float, float, float] = (0, 0, 0)
+    gear_compression: Tuple[float, float, float] = (0, 0, 0)
+    cur_time: int = 0
+    """current unix time"""
+    warp: int = 0
+    """offset in seconds to unix time"""
+    visibility: float = 0
+    """visibility in meters (for env. effects)"""
+    elevator: float = 0
+    elevator_trim_tab: float = 0
+    left_flap: float = 0
+    right_flap: float = 0
+    left_aileron: float = 0
+    right_aileron: float = 0
+    rudder: float = 0
+    nose_wheel: float = 0
+    speedbrake: float = 0
+    spoilers: float = 0
+
+    @classmethod
+    def from_bytes(cls, data):
+        version = unpack_from("!I", data)[0]
+        if version != FG_NET_FDM_VERSION:
+            raise ValueError(
+                f"Expected protocol version {FG_NET_FDM_VERSION}, got {version}")
+        this = cls()
+        decoded = unpack_from(
+            "!IIdddffffffffffffffffffffffIIIIIffffffffffffffffffffffffffffffffffffIffffIIIIfffffffffIifffffffffff", data)
+        this.version = decoded[0]
+        this.padding = decoded[1]
+        this.longitude = decoded[2]
+        this.latitude = decoded[3]
+        this.altitude = decoded[4]
+        this.agl = decoded[5]
+        this.phi = decoded[6]
+        this.theta = decoded[7]
+        this.psi = decoded[8]
+        this.alpha = decoded[9]
+        this.beta = decoded[10]
+        this.phidot = decoded[11]
+        this.thetadot = decoded[12]
+        this.psidot = decoded[13]
+        this.vcas = decoded[14]
+        this.climb_rate = decoded[15]
+        this.v_north = decoded[16]
+        this.v_east = decoded[17]
+        this.v_down = decoded[18]
+        this.v_body_u = decoded[19]
+        this.v_body_v = decoded[20]
+        this.v_body_w = decoded[21]
+        this.A_X_pilot = decoded[22]
+        this.A_Y_pilot = decoded[23]
+        this.A_Z_pilot = decoded[24]
+        this.stall_warning = decoded[25]
+        this.slip_deg = decoded[26]
+        this.num_engines = decoded[27]
+        this.eng_state = decoded[28:32]
+        this.rpm = decoded[32:36]
+        this.fuel_flow = decoded[36:40]
+        this.fuel_px = decoded[40:44]
+        this.egt = decoded[44:48]
+        this.cht = decoded[48:52]
+        this.mp_osi = decoded[52:56]
+        this.tit = decoded[56:60]
+        this.oil_temp = decoded[60:64]
+        this.oil_px = decoded[64:68]
+        this.num_tanks = decoded[68]
+        this.fuel_quantity = decoded[69:73]
+        this.num_wheels = decoded[73]
+        this.wow = decoded[74:77]
+        this.gear_pos = decoded[77:80]
+        this.gear_steer = decoded[80:83]
+        this.gear_compression = decoded[83:86]
+        this.cur_time = decoded[86]
+        this.warp = decoded[87]
+        this.visibility = decoded[88]
+        this.elevator = decoded[89]
+        this.elevator_trim_tab = decoded[90]
+        this.left_flap = decoded[91]
+        this.right_flap = decoded[92]
+        this.left_aileron = decoded[93]
+        this.right_aileron = decoded[94]
+        this.rudder = decoded[95]
+        this.nose_wheel = decoded[96]
+        this.speedbrake = decoded[97]
+        this.spoilers = decoded[98]
+        return this
```

### Comparing `lidia-0.8.0/src/lidia/sources/rpctask.py` & `lidia-0.8.1/src/lidia/sources/rpctask.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""listen to UDP packets from Rotorcraft-Pilot Coupling Task simulator"""
-from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
-from multiprocessing import Queue
-import socket
-from struct import unpack_from
-from typing import Tuple
-
-from ..aircraft import *
-from ..config import Config
-from .mytypes import RunFn
-
-
-def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
-    NAME = 'rpctask'
-    parser: ArgumentParser = subparsers.add_parser(
-        NAME,
-        help=__doc__,
-        formatter_class=ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-i', '--ip',
-                        help='listen UDP adress', default='0.0.0.0')
-    parser.add_argument('-p', '--port', type=int,
-                        help='listen UDP port', default=5004)
-
-    return (NAME, run)
-
-
-def run(q: Queue, args: Namespace, _config: Config):
-
-    last_trim = Controls()
-
-    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
-        # Timeout is required to handle leaving with Ctrl+C
-        sock.settimeout(1.0)
-        sock.bind((args.ip, args.port))
-        if args.verbosity >= 0:
-            print(f'Listening for UDP packets on {args.ip}:{args.port}')
-
-        while True:
-            try:
-                data, _ = sock.recvfrom(1024)
-                # As named in the original FlightGear protocol file
-                # cyclic has coordinates 0,0 in bottom left and 1,1 in top right
-                (pitch_ctrl, roll_ctrl, pwr_ctrl,
-                 pitch_target, roll_target, pwr_target,
-                 cyc_ftr, coll_ftr) = unpack_from('>' + 'd' * 8, data)
-
-                state = AircraftState()
-                state.ctrl = Controls()
-                state.ctrl.stick_right = (roll_ctrl * 2.0) - 1.0
-                state.ctrl.stick_pull = (pitch_ctrl * -2.0) + 1.0
-                state.ctrl.collective_up = pwr_ctrl
-
-                state.trgt = AircraftData()
-                state.trgt.ctrl = Controls()
-                state.trgt.ctrl.stick_right = (roll_target * 2.0) - 1.0
-                state.trgt.ctrl.stick_pull = (pitch_target * -2.0) + 1.0
-                state.trgt.ctrl.collective_up = pwr_target
-
-                state.btn = Buttons()
-                if cyc_ftr > 0.5:
-                    state.btn.cyc_ftr = True
-                if coll_ftr > 0.5:
-                    state.btn.coll_ftr = True
-
-                if len(data) >= 8 * 14:
-                    (up_bdr_cyc, low_bdr_cyc, right_bdr_cyc, left_bdr_cyc,
-                     up_bdr_coll, low_bdr_coll) = unpack_from('>' + 'd' * 6, data, 8 * 8)
-                    state.brdr = Borders()
-                    state.brdr.high.stick_right = (right_bdr_cyc * 2.0) - 1.0
-                    state.brdr.low.stick_right = (left_bdr_cyc * 2.0) - 1.0
-                    state.brdr.high.stick_pull = (low_bdr_cyc * -2.0) + 1.0
-                    state.brdr.low.stick_pull = (up_bdr_cyc * -2.0) + 1.0
-                    state.brdr.high.collective_up = up_bdr_coll
-                    state.brdr.low.collective_up = low_bdr_coll
-
-                if state.btn.coll_ftr:
-                    last_trim.collective_up = state.ctrl.collective_up
-                if state.btn.cyc_ftr:
-                    last_trim.stick_right = state.ctrl.stick_right
-                    last_trim.stick_pull = state.ctrl.stick_pull
-                state.trim = AircraftData()
-                state.trim.ctrl = last_trim
-
-                q.put(('smol', state.smol()))
-            except socket.timeout:
-                continue
+"""listen to UDP packets from Rotorcraft-Pilot Coupling Task simulator"""
+from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
+from multiprocessing import Queue
+import socket
+from struct import unpack_from
+from typing import Tuple
+
+from ..aircraft import *
+from ..config import Config
+from .mytypes import RunFn
+
+
+def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
+    NAME = 'rpctask'
+    parser: ArgumentParser = subparsers.add_parser(
+        NAME,
+        help=__doc__,
+        formatter_class=ArgumentDefaultsHelpFormatter)
+    parser.add_argument('-i', '--ip',
+                        help='listen UDP adress', default='0.0.0.0')
+    parser.add_argument('-p', '--port', type=int,
+                        help='listen UDP port', default=5004)
+
+    return (NAME, run)
+
+
+def run(q: Queue, args: Namespace, _config: Config):
+
+    last_trim = Controls()
+
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
+        # Timeout is required to handle leaving with Ctrl+C
+        sock.settimeout(1.0)
+        sock.bind((args.ip, args.port))
+        if args.verbosity >= 0:
+            print(f'Listening for UDP packets on {args.ip}:{args.port}')
+
+        while True:
+            try:
+                data, _ = sock.recvfrom(1024)
+                # As named in the original FlightGear protocol file
+                # cyclic has coordinates 0,0 in bottom left and 1,1 in top right
+                (pitch_ctrl, roll_ctrl, pwr_ctrl,
+                 pitch_target, roll_target, pwr_target,
+                 cyc_ftr, coll_ftr) = unpack_from('>' + 'd' * 8, data)
+
+                state = AircraftState()
+                state.ctrl = Controls()
+                state.ctrl.stick_right = (roll_ctrl * 2.0) - 1.0
+                state.ctrl.stick_pull = (pitch_ctrl * -2.0) + 1.0
+                state.ctrl.collective_up = pwr_ctrl
+
+                state.trgt = AircraftData()
+                state.trgt.ctrl = Controls()
+                state.trgt.ctrl.stick_right = (roll_target * 2.0) - 1.0
+                state.trgt.ctrl.stick_pull = (pitch_target * -2.0) + 1.0
+                state.trgt.ctrl.collective_up = pwr_target
+
+                state.btn = Buttons()
+                if cyc_ftr > 0.5:
+                    state.btn.cyc_ftr = True
+                if coll_ftr > 0.5:
+                    state.btn.coll_ftr = True
+
+                if len(data) >= 8 * 14:
+                    (up_bdr_cyc, low_bdr_cyc, right_bdr_cyc, left_bdr_cyc,
+                     up_bdr_coll, low_bdr_coll) = unpack_from('>' + 'd' * 6, data, 8 * 8)
+                    state.brdr = Borders()
+                    state.brdr.high.stick_right = (right_bdr_cyc * 2.0) - 1.0
+                    state.brdr.low.stick_right = (left_bdr_cyc * 2.0) - 1.0
+                    state.brdr.high.stick_pull = (low_bdr_cyc * -2.0) + 1.0
+                    state.brdr.low.stick_pull = (up_bdr_cyc * -2.0) + 1.0
+                    state.brdr.high.collective_up = up_bdr_coll
+                    state.brdr.low.collective_up = low_bdr_coll
+
+                if state.btn.coll_ftr:
+                    last_trim.collective_up = state.ctrl.collective_up
+                if state.btn.cyc_ftr:
+                    last_trim.stick_right = state.ctrl.stick_right
+                    last_trim.stick_pull = state.ctrl.stick_pull
+                state.trim = AircraftData()
+                state.trim.ctrl = last_trim
+
+                q.put(('smol', state.smol()))
+            except socket.timeout:
+                continue
```

### Comparing `lidia-0.8.0/src/lidia/sources/smol.py` & `lidia-0.8.1/src/lidia/sources/smol.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-
-"""listen to UDP packets with SMOL encoded as MessagePack or JSON"""
-from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
-import json
-import msgpack
-from multiprocessing import Queue
-import socket
-from typing import Tuple
-
-from ..aircraft import *
-from ..config import Config
-from .mytypes import RunFn
-
-
-def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
-    NAME = 'smol'
-    parser: ArgumentParser = subparsers.add_parser(
-        NAME,
-        help=__doc__,
-        formatter_class=ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-i', '--ip',
-                        help='listen UDP adress', default='0.0.0.0')
-    parser.add_argument('-p', '--port', type=int,
-                        help='listen UDP port', default=5004)
-
-    return (NAME, run)
-
-
-def run(q: Queue, args: Namespace, config: Config):
-
-    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
-        # Timeout is required to handle leaving with Ctrl+C
-        sock.settimeout(1.0)
-        sock.bind((args.ip, args.port))
-        if args.verbosity >= 0:
-            print(f'Listening for UDP packets on {args.ip}:{args.port}')
-
-        while True:
-            try:
-                data, _ = sock.recvfrom(1024)
-
-                decoded = None
-                if data[0] == ord('{'):
-                    try:
-                        decoded = json.loads(data)
-                    except json.JSONDecodeError as e:
-                        print(e)
-                else:
-                    try:
-                        decoded = msgpack.unpackb(data)
-                    except Exception as e:
-                        print(e)
-
-                if decoded is not None:
-                    try:
-                        state = AircraftState.from_smol(decoded)
-                        state.model_instruments(config)
-                        q.put(('smol', state.smol()))
-                    except Exception as e:
-                        print(e)
-
-            except socket.timeout:
-                continue
+
+"""listen to UDP packets with SMOL encoded as MessagePack or JSON"""
+from argparse import _SubParsersAction, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
+import json
+import msgpack
+from multiprocessing import Queue
+import socket
+from typing import Tuple
+
+from ..aircraft import *
+from ..config import Config
+from .mytypes import RunFn
+
+
+def setup(subparsers: _SubParsersAction) -> Tuple[str, RunFn]:
+    NAME = 'smol'
+    parser: ArgumentParser = subparsers.add_parser(
+        NAME,
+        help=__doc__,
+        formatter_class=ArgumentDefaultsHelpFormatter)
+    parser.add_argument('-i', '--ip',
+                        help='listen UDP adress', default='0.0.0.0')
+    parser.add_argument('-p', '--port', type=int,
+                        help='listen UDP port', default=5004)
+
+    return (NAME, run)
+
+
+def run(q: Queue, args: Namespace, config: Config):
+
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
+        # Timeout is required to handle leaving with Ctrl+C
+        sock.settimeout(1.0)
+        sock.bind((args.ip, args.port))
+        if args.verbosity >= 0:
+            print(f'Listening for UDP packets on {args.ip}:{args.port}')
+
+        while True:
+            try:
+                data, _ = sock.recvfrom(1024)
+
+                decoded = None
+                if data[0] == ord('{'):
+                    try:
+                        decoded = json.loads(data)
+                    except json.JSONDecodeError as e:
+                        print(e)
+                else:
+                    try:
+                        decoded = msgpack.unpackb(data)
+                    except Exception as e:
+                        print(e)
+
+                if decoded is not None:
+                    try:
+                        state = AircraftState.from_smol(decoded)
+                        state.model_instruments(config)
+                        q.put(('smol', state.smol()))
+                    except Exception as e:
+                        print(e)
+
+            except socket.timeout:
+                continue
```

### Comparing `lidia-0.8.0/src/lidia/static/LICENSE.txt` & `lidia-0.8.1/src/lidia/static/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-Roboto Mono
-
-Copyright 2015 Google
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-
-=====================================================================
-
-Socket.IO
-
-MIT License
-
-Copyright (c) 2014-2022 Guillermo Rauch
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Roboto Mono
+
+Copyright 2015 Google
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+=====================================================================
+
+Socket.IO
+
+MIT License
+
+Copyright (c) 2014-2022 Guillermo Rauch
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `lidia-0.8.0/src/lidia/static/RobotoMono-Bold.ttf` & `lidia-0.8.1/src/lidia/static/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.0/src/lidia/static/RobotoMono-ExtraLight.ttf` & `lidia-0.8.1/src/lidia/static/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.0/src/lidia/static/RobotoMono-Light.ttf` & `lidia-0.8.1/src/lidia/static/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.0/src/lidia/static/RobotoMono-Medium.ttf` & `lidia-0.8.1/src/lidia/static/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.0/src/lidia/static/RobotoMono-Regular.ttf` & `lidia-0.8.1/src/lidia/static/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.0/src/lidia/static/RobotoMono-SemiBold.ttf` & `lidia-0.8.1/src/lidia/static/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.0/src/lidia/static/RobotoMono-Thin.ttf` & `lidia-0.8.1/src/lidia/static/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.0/src/lidia/static/controls.js` & `lidia-0.8.1/src/lidia/static/controls.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,205 +1,205 @@
-function regionBoxChange(event) {
-    let name = event.target.id.slice(4).toLowerCase(); // Strip the "show" prefix
-    document.controls.regions.find((r) => r.name === name).show =
-        event.target.checked;
-    applySettings();
-}
-
-function alignmentChange(event) {
-    let x = event.target.x.baseVal.value;
-    let y = event.target.y.baseVal.value;
-    document.controls.alignHorizontal = x === 0 ? -1 : x === 75 ? 1 : 0;
-    document.controls.alignVertical = y === 0 ? -1 : y === 75 ? 1 : 0;
-    applySettings();
-}
-
-function addControls(svgElem) {
-    document.controls = {
-        regions: [],
-        alignHorizontal: 0,
-        alignVertical: 0,
-        svgElem: svgElem,
-    };
-
-    for (const child of svgElem.children) {
-        if (child.id.endsWith("Region") && child.dataset.extents) {
-            let nums = child.dataset.extents.split(" ");
-            let region = {
-                name: child.id.slice(0, -6), // Remove "Region" suffix
-                top: parseFloat(nums[0]),
-                right: parseFloat(nums[1]),
-                bottom: parseFloat(nums[2]),
-                left: parseFloat(nums[3]),
-                show: true,
-            };
-            document.controls.regions.push(region);
-        }
-    }
-
-    let container = document.createElement("div");
-    container.classList.add("controls");
-    document.body.appendChild(container);
-
-    let checks = document.createElement("p");
-    container.appendChild(checks);
-    let checksPrompt = document.createElement("span");
-    checksPrompt.innerText = "Show regions:";
-    checks.appendChild(checksPrompt);
-
-    for (const region of document.controls.regions) {
-        let capitalised = region.name[0].toUpperCase() + region.name.slice(1);
-
-        let span = document.createElement("span");
-        checks.appendChild(span);
-
-        let checkbox = document.createElement("input");
-        checkbox.id = "show" + capitalised;
-        checkbox.type = "checkbox";
-        checkbox.checked = true;
-        checkbox.addEventListener("change", regionBoxChange);
-        span.appendChild(checkbox);
-
-        let label = document.createElement("label");
-        label.innerText = region.name;
-        label.setAttribute("for", "show" + capitalised);
-        span.appendChild(label);
-    }
-
-    let alignment = document.createElement("p");
-    container.appendChild(alignment);
-    alignment.innerHTML = `
-    <span>Screen alignment:</span>
-    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" width="4em" height="4em">
-      <g id="alignGroup" stroke="none" fill="currentColor">
-        <rect x="0" y="0" width="25" height="25" rx="5" />
-        <rect x="37.5" y="0" width="25" height="25" rx="5" />
-        <rect x="75" y="0" width="25" height="25" rx="5" />
-        <rect x="0" y="37.5" width="25" height="25" rx="5" />
-        <rect x="37.5" y="37.5" width="25" height="25" rx="5" />
-        <rect x="75" y="37.5" width="25" height="25" rx="5" />
-        <rect x="0" y="75" width="25" height="25" rx="5" />
-        <rect x="37.5" y="75" width="25" height="25" rx="5" />
-        <rect x="75" y="75" width="25" height="25" rx="5" />
-      </g>
-    </svg>`;
-
-    for (rect of document.getElementById("alignGroup").children) {
-        rect.addEventListener("click", alignmentChange);
-    }
-
-    window.addEventListener("load", () => parseLocation());
-}
-
-function applySettings() {
-    const controls = document.controls;
-    const regions = document.controls.regions;
-
-    for (const region of regions) {
-        document.getElementById(region.name + "Region").style.display = region.show ?
-            "block" :
-            "none";
-        let capitalised = region.name[0].toUpperCase() + region.name.slice(1);
-        document.getElementById("show" + capitalised).checked = region.show;
-    }
-
-    let top = Math.min(...regions.filter((r) => r.show).map((r) => r.top));
-    top = isFinite(top) ? top : 0;
-    let right = Math.max(...regions.filter((r) => r.show).map((r) => r.right));
-    right = isFinite(right) ? right : 0;
-    let bottom = Math.max(...regions.filter((r) => r.show).map((r) => r.bottom));
-    bottom = isFinite(bottom) ? bottom : 0;
-    let left = Math.min(...regions.filter((r) => r.show).map((r) => r.left));
-    left = isFinite(left) ? left : 0;
-    controls.svgElem.setAttribute(
-        "viewBox",
-        `${left} ${top} ${right - left} ${bottom - top}`
-    );
-
-    let alignment =
-        (controls.alignHorizontal === -1 ?
-            "xMin" :
-            controls.alignHorizontal === 1 ?
-            "xMax" :
-            "xMid") +
-        (controls.alignVertical === -1 ?
-            "YMin" :
-            controls.alignVertical === 1 ?
-            "YMax" :
-            "YMid");
-    controls.svgElem.setAttribute("preserveAspectRatio", alignment + " meet");
-
-    let selectedX =
-        document.controls.alignHorizontal === -1 ?
-        0 :
-        document.controls.alignHorizontal === 0 ?
-        37.5 :
-        75;
-    let selectedY =
-        document.controls.alignVertical === -1 ?
-        0 :
-        document.controls.alignVertical === 0 ?
-        37.5 :
-        75;
-
-    for (rect of document.getElementById("alignGroup").children) {
-        let x = rect.x.baseVal.value;
-        let y = rect.y.baseVal.value;
-        rect.style.fill = x === selectedX && y === selectedY ? "#0f0" : "inherit";
-    }
-
-    let hashParts = [];
-    if (!document.controls.regions.every((r) => r.show)) {
-        // When everything is shown, don't put that into location
-        let shown = [];
-        for (const region of document.controls.regions) {
-            if (region.show) shown.push(region.name);
-        }
-        if (shown.length === 0) shown.push("none");
-        hashParts.push(shown.join(","));
-    }
-    if (alignment !== "xMidYMid") hashParts.push(alignment);
-
-    if (hashParts.length === 0)
-        history.pushState("", document.title, window.location.pathname);
-    else document.location.hash = hashParts.join("|");
-}
-
-function parseLocation() {
-    let hash = document.location.hash.replace("#", "");
-
-    const alignRe = /^xM(\w\w)YM(\w\w)$/;
-    const regionRe = new RegExp(
-        "(" + document.controls.regions.map((r) => r.name).join("|") + "|none)",
-        "i"
-    );
-    for (part of hash.split("|")) {
-        if (alignRe.test(part)) {
-            let m = part.match(alignRe);
-            settings.alignHorizontal = m[1] === "in" ? -1 : m[1] === "ax" ? 1 : 0;
-            settings.alignVertical = m[2] === "in" ? -1 : m[2] === "ax" ? 1 : 0;
-        }
-        if (regionRe.test(part)) {
-            for (let i = 0; i < document.controls.regions.length; i++) {
-                const region = document.controls.regions[i];
-                if (part.includes(region.name))
-                    document.controls.regions[i].show = true;
-                else document.controls.regions[i].show = false;
-            }
-        }
-    }
-
-    applySettings();
-}
-
-function showRegions() {
-    for (const region of document.controls.regions) {
-        let rect = document.createElementNS("http://www.w3.org/2000/svg", "rect");
-        rect.setAttribute("x", region.left);
-        rect.setAttribute("y", region.top);
-        rect.setAttribute("width", region.right - region.left);
-        rect.setAttribute("height", region.bottom - region.top);
-        rect.setAttribute("fill", "#f0f");
-        rect.setAttribute("fill-opacity", 0.5);
-        document.controls.svgElem.appendChild(rect);
-    }
+function regionBoxChange(event) {
+    let name = event.target.id.slice(4).toLowerCase(); // Strip the "show" prefix
+    document.controls.regions.find((r) => r.name === name).show =
+        event.target.checked;
+    applySettings();
+}
+
+function alignmentChange(event) {
+    let x = event.target.x.baseVal.value;
+    let y = event.target.y.baseVal.value;
+    document.controls.alignHorizontal = x === 0 ? -1 : x === 75 ? 1 : 0;
+    document.controls.alignVertical = y === 0 ? -1 : y === 75 ? 1 : 0;
+    applySettings();
+}
+
+function addControls(svgElem) {
+    document.controls = {
+        regions: [],
+        alignHorizontal: 0,
+        alignVertical: 0,
+        svgElem: svgElem,
+    };
+
+    for (const child of svgElem.children) {
+        if (child.id.endsWith("Region") && child.dataset.extents) {
+            let nums = child.dataset.extents.split(" ");
+            let region = {
+                name: child.id.slice(0, -6), // Remove "Region" suffix
+                top: parseFloat(nums[0]),
+                right: parseFloat(nums[1]),
+                bottom: parseFloat(nums[2]),
+                left: parseFloat(nums[3]),
+                show: true,
+            };
+            document.controls.regions.push(region);
+        }
+    }
+
+    let container = document.createElement("div");
+    container.classList.add("controls");
+    document.body.appendChild(container);
+
+    let checks = document.createElement("p");
+    container.appendChild(checks);
+    let checksPrompt = document.createElement("span");
+    checksPrompt.innerText = "Show regions:";
+    checks.appendChild(checksPrompt);
+
+    for (const region of document.controls.regions) {
+        let capitalised = region.name[0].toUpperCase() + region.name.slice(1);
+
+        let span = document.createElement("span");
+        checks.appendChild(span);
+
+        let checkbox = document.createElement("input");
+        checkbox.id = "show" + capitalised;
+        checkbox.type = "checkbox";
+        checkbox.checked = true;
+        checkbox.addEventListener("change", regionBoxChange);
+        span.appendChild(checkbox);
+
+        let label = document.createElement("label");
+        label.innerText = region.name;
+        label.setAttribute("for", "show" + capitalised);
+        span.appendChild(label);
+    }
+
+    let alignment = document.createElement("p");
+    container.appendChild(alignment);
+    alignment.innerHTML = `
+    <span>Screen alignment:</span>
+    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" width="4em" height="4em">
+      <g id="alignGroup" stroke="none" fill="currentColor">
+        <rect x="0" y="0" width="25" height="25" rx="5" />
+        <rect x="37.5" y="0" width="25" height="25" rx="5" />
+        <rect x="75" y="0" width="25" height="25" rx="5" />
+        <rect x="0" y="37.5" width="25" height="25" rx="5" />
+        <rect x="37.5" y="37.5" width="25" height="25" rx="5" />
+        <rect x="75" y="37.5" width="25" height="25" rx="5" />
+        <rect x="0" y="75" width="25" height="25" rx="5" />
+        <rect x="37.5" y="75" width="25" height="25" rx="5" />
+        <rect x="75" y="75" width="25" height="25" rx="5" />
+      </g>
+    </svg>`;
+
+    for (rect of document.getElementById("alignGroup").children) {
+        rect.addEventListener("click", alignmentChange);
+    }
+
+    window.addEventListener("load", () => parseLocation());
+}
+
+function applySettings() {
+    const controls = document.controls;
+    const regions = document.controls.regions;
+
+    for (const region of regions) {
+        document.getElementById(region.name + "Region").style.display = region.show ?
+            "block" :
+            "none";
+        let capitalised = region.name[0].toUpperCase() + region.name.slice(1);
+        document.getElementById("show" + capitalised).checked = region.show;
+    }
+
+    let top = Math.min(...regions.filter((r) => r.show).map((r) => r.top));
+    top = isFinite(top) ? top : 0;
+    let right = Math.max(...regions.filter((r) => r.show).map((r) => r.right));
+    right = isFinite(right) ? right : 0;
+    let bottom = Math.max(...regions.filter((r) => r.show).map((r) => r.bottom));
+    bottom = isFinite(bottom) ? bottom : 0;
+    let left = Math.min(...regions.filter((r) => r.show).map((r) => r.left));
+    left = isFinite(left) ? left : 0;
+    controls.svgElem.setAttribute(
+        "viewBox",
+        `${left} ${top} ${right - left} ${bottom - top}`
+    );
+
+    let alignment =
+        (controls.alignHorizontal === -1 ?
+            "xMin" :
+            controls.alignHorizontal === 1 ?
+            "xMax" :
+            "xMid") +
+        (controls.alignVertical === -1 ?
+            "YMin" :
+            controls.alignVertical === 1 ?
+            "YMax" :
+            "YMid");
+    controls.svgElem.setAttribute("preserveAspectRatio", alignment + " meet");
+
+    let selectedX =
+        document.controls.alignHorizontal === -1 ?
+        0 :
+        document.controls.alignHorizontal === 0 ?
+        37.5 :
+        75;
+    let selectedY =
+        document.controls.alignVertical === -1 ?
+        0 :
+        document.controls.alignVertical === 0 ?
+        37.5 :
+        75;
+
+    for (rect of document.getElementById("alignGroup").children) {
+        let x = rect.x.baseVal.value;
+        let y = rect.y.baseVal.value;
+        rect.style.fill = x === selectedX && y === selectedY ? "#0f0" : "inherit";
+    }
+
+    let hashParts = [];
+    if (!document.controls.regions.every((r) => r.show)) {
+        // When everything is shown, don't put that into location
+        let shown = [];
+        for (const region of document.controls.regions) {
+            if (region.show) shown.push(region.name);
+        }
+        if (shown.length === 0) shown.push("none");
+        hashParts.push(shown.join(","));
+    }
+    if (alignment !== "xMidYMid") hashParts.push(alignment);
+
+    if (hashParts.length === 0)
+        history.pushState("", document.title, window.location.pathname);
+    else document.location.hash = hashParts.join("|");
+}
+
+function parseLocation() {
+    let hash = document.location.hash.replace("#", "");
+
+    const alignRe = /^xM(\w\w)YM(\w\w)$/;
+    const regionRe = new RegExp(
+        "(" + document.controls.regions.map((r) => r.name).join("|") + "|none)",
+        "i"
+    );
+    for (part of hash.split("|")) {
+        if (alignRe.test(part)) {
+            let m = part.match(alignRe);
+            settings.alignHorizontal = m[1] === "in" ? -1 : m[1] === "ax" ? 1 : 0;
+            settings.alignVertical = m[2] === "in" ? -1 : m[2] === "ax" ? 1 : 0;
+        }
+        if (regionRe.test(part)) {
+            for (let i = 0; i < document.controls.regions.length; i++) {
+                const region = document.controls.regions[i];
+                if (part.includes(region.name))
+                    document.controls.regions[i].show = true;
+                else document.controls.regions[i].show = false;
+            }
+        }
+    }
+
+    applySettings();
+}
+
+function showRegions() {
+    for (const region of document.controls.regions) {
+        let rect = document.createElementNS("http://www.w3.org/2000/svg", "rect");
+        rect.setAttribute("x", region.left);
+        rect.setAttribute("y", region.top);
+        rect.setAttribute("width", region.right - region.left);
+        rect.setAttribute("height", region.bottom - region.top);
+        rect.setAttribute("fill", "#f0f");
+        rect.setAttribute("fill-opacity", 0.5);
+        document.controls.svgElem.appendChild(rect);
+    }
 }
```

### Comparing `lidia-0.8.0/src/lidia/static/socket.io.js` & `lidia-0.8.1/src/lidia/static/socket.io.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,4442 +1,4442 @@
-/*!
- * Socket.IO v4.4.1
- * (c) 2014-2022 Guillermo Rauch
- * Released under the MIT License.
- */
-(function(global, factory) {
-    typeof exports === "object" && typeof module !== "undefined" ?
-        (module.exports = factory()) :
-        typeof define === "function" && define.amd ?
-        define(factory) :
-        ((global =
-                typeof globalThis !== "undefined" ? globalThis : global || self),
-            (global.io = factory()));
-})(this, function() {
-    "use strict";
-
-    function _typeof(obj) {
-        "@babel/helpers - typeof";
-
-        if (typeof Symbol === "function" && typeof Symbol.iterator === "symbol") {
-            _typeof = function(obj) {
-                return typeof obj;
-            };
-        } else {
-            _typeof = function(obj) {
-                return obj &&
-                    typeof Symbol === "function" &&
-                    obj.constructor === Symbol &&
-                    obj !== Symbol.prototype ?
-                    "symbol" :
-                    typeof obj;
-            };
-        }
-
-        return _typeof(obj);
-    }
-
-    function _classCallCheck(instance, Constructor) {
-        if (!(instance instanceof Constructor)) {
-            throw new TypeError("Cannot call a class as a function");
-        }
-    }
-
-    function _defineProperties(target, props) {
-        for (var i = 0; i < props.length; i++) {
-            var descriptor = props[i];
-            descriptor.enumerable = descriptor.enumerable || false;
-            descriptor.configurable = true;
-            if ("value" in descriptor) descriptor.writable = true;
-            Object.defineProperty(target, descriptor.key, descriptor);
-        }
-    }
-
-    function _createClass(Constructor, protoProps, staticProps) {
-        if (protoProps) _defineProperties(Constructor.prototype, protoProps);
-        if (staticProps) _defineProperties(Constructor, staticProps);
-        return Constructor;
-    }
-
-    function _extends() {
-        _extends =
-            Object.assign ||
-            function(target) {
-                for (var i = 1; i < arguments.length; i++) {
-                    var source = arguments[i];
-
-                    for (var key in source) {
-                        if (Object.prototype.hasOwnProperty.call(source, key)) {
-                            target[key] = source[key];
-                        }
-                    }
-                }
-
-                return target;
-            };
-
-        return _extends.apply(this, arguments);
-    }
-
-    function _inherits(subClass, superClass) {
-        if (typeof superClass !== "function" && superClass !== null) {
-            throw new TypeError("Super expression must either be null or a function");
-        }
-
-        subClass.prototype = Object.create(superClass && superClass.prototype, {
-            constructor: {
-                value: subClass,
-                writable: true,
-                configurable: true,
-            },
-        });
-        if (superClass) _setPrototypeOf(subClass, superClass);
-    }
-
-    function _getPrototypeOf(o) {
-        _getPrototypeOf = Object.setPrototypeOf ?
-            Object.getPrototypeOf :
-            function _getPrototypeOf(o) {
-                return o.__proto__ || Object.getPrototypeOf(o);
-            };
-        return _getPrototypeOf(o);
-    }
-
-    function _setPrototypeOf(o, p) {
-        _setPrototypeOf =
-            Object.setPrototypeOf ||
-            function _setPrototypeOf(o, p) {
-                o.__proto__ = p;
-                return o;
-            };
-
-        return _setPrototypeOf(o, p);
-    }
-
-    function _isNativeReflectConstruct() {
-        if (typeof Reflect === "undefined" || !Reflect.construct) return false;
-        if (Reflect.construct.sham) return false;
-        if (typeof Proxy === "function") return true;
-
-        try {
-            Boolean.prototype.valueOf.call(
-                Reflect.construct(Boolean, [], function() {})
-            );
-            return true;
-        } catch (e) {
-            return false;
-        }
-    }
-
-    function _assertThisInitialized(self) {
-        if (self === void 0) {
-            throw new ReferenceError(
-                "this hasn't been initialised - super() hasn't been called"
-            );
-        }
-
-        return self;
-    }
-
-    function _possibleConstructorReturn(self, call) {
-        if (call && (typeof call === "object" || typeof call === "function")) {
-            return call;
-        } else if (call !== void 0) {
-            throw new TypeError(
-                "Derived constructors may only return object or undefined"
-            );
-        }
-
-        return _assertThisInitialized(self);
-    }
-
-    function _createSuper(Derived) {
-        var hasNativeReflectConstruct = _isNativeReflectConstruct();
-
-        return function _createSuperInternal() {
-            var Super = _getPrototypeOf(Derived),
-                result;
-
-            if (hasNativeReflectConstruct) {
-                var NewTarget = _getPrototypeOf(this).constructor;
-
-                result = Reflect.construct(Super, arguments, NewTarget);
-            } else {
-                result = Super.apply(this, arguments);
-            }
-
-            return _possibleConstructorReturn(this, result);
-        };
-    }
-
-    function _superPropBase(object, property) {
-        while (!Object.prototype.hasOwnProperty.call(object, property)) {
-            object = _getPrototypeOf(object);
-            if (object === null) break;
-        }
-
-        return object;
-    }
-
-    function _get(target, property, receiver) {
-        if (typeof Reflect !== "undefined" && Reflect.get) {
-            _get = Reflect.get;
-        } else {
-            _get = function _get(target, property, receiver) {
-                var base = _superPropBase(target, property);
-
-                if (!base) return;
-                var desc = Object.getOwnPropertyDescriptor(base, property);
-
-                if (desc.get) {
-                    return desc.get.call(receiver);
-                }
-
-                return desc.value;
-            };
-        }
-
-        return _get(target, property, receiver || target);
-    }
-
-    function _unsupportedIterableToArray(o, minLen) {
-        if (!o) return;
-        if (typeof o === "string") return _arrayLikeToArray(o, minLen);
-        var n = Object.prototype.toString.call(o).slice(8, -1);
-        if (n === "Object" && o.constructor) n = o.constructor.name;
-        if (n === "Map" || n === "Set") return Array.from(o);
-        if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n))
-            return _arrayLikeToArray(o, minLen);
-    }
-
-    function _arrayLikeToArray(arr, len) {
-        if (len == null || len > arr.length) len = arr.length;
-
-        for (var i = 0, arr2 = new Array(len); i < len; i++) arr2[i] = arr[i];
-
-        return arr2;
-    }
-
-    function _createForOfIteratorHelper(o, allowArrayLike) {
-        var it =
-            (typeof Symbol !== "undefined" && o[Symbol.iterator]) || o["@@iterator"];
-
-        if (!it) {
-            if (
-                Array.isArray(o) ||
-                (it = _unsupportedIterableToArray(o)) ||
-                (allowArrayLike && o && typeof o.length === "number")
-            ) {
-                if (it) o = it;
-                var i = 0;
-
-                var F = function() {};
-
-                return {
-                    s: F,
-                    n: function() {
-                        if (i >= o.length)
-                            return {
-                                done: true,
-                            };
-                        return {
-                            done: false,
-                            value: o[i++],
-                        };
-                    },
-                    e: function(e) {
-                        throw e;
-                    },
-                    f: F,
-                };
-            }
-
-            throw new TypeError(
-                "Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method."
-            );
-        }
-
-        var normalCompletion = true,
-            didErr = false,
-            err;
-        return {
-            s: function() {
-                it = it.call(o);
-            },
-            n: function() {
-                var step = it.next();
-                normalCompletion = step.done;
-                return step;
-            },
-            e: function(e) {
-                didErr = true;
-                err = e;
-            },
-            f: function() {
-                try {
-                    if (!normalCompletion && it.return != null) it.return();
-                } finally {
-                    if (didErr) throw err;
-                }
-            },
-        };
-    }
-
-    /**
-     * Parses an URI
-     *
-     * @author Steven Levithan <stevenlevithan.com> (MIT license)
-     * @api private
-     */
-    var re =
-        /^(?:(?![^:@]+:[^:@\/]*@)(http|https|ws|wss):\/\/)?((?:(([^:@]*)(?::([^:@]*))?)?@)?((?:[a-f0-9]{0,4}:){2,7}[a-f0-9]{0,4}|[^:\/?#]*)(?::(\d*))?)(((\/(?:[^?#](?![^?#\/]*\.[^?#\/.]+(?:[?#]|$)))*\/?)?([^?#\/]*))(?:\?([^#]*))?(?:#(.*))?)/;
-    var parts = [
-        "source",
-        "protocol",
-        "authority",
-        "userInfo",
-        "user",
-        "password",
-        "host",
-        "port",
-        "relative",
-        "path",
-        "directory",
-        "file",
-        "query",
-        "anchor",
-    ];
-
-    var parseuri = function parseuri(str) {
-        var src = str,
-            b = str.indexOf("["),
-            e = str.indexOf("]");
-
-        if (b != -1 && e != -1) {
-            str =
-                str.substring(0, b) +
-                str.substring(b, e).replace(/:/g, ";") +
-                str.substring(e, str.length);
-        }
-
-        var m = re.exec(str || ""),
-            uri = {},
-            i = 14;
-
-        while (i--) {
-            uri[parts[i]] = m[i] || "";
-        }
-
-        if (b != -1 && e != -1) {
-            uri.source = src;
-            uri.host = uri.host.substring(1, uri.host.length - 1).replace(/;/g, ":");
-            uri.authority = uri.authority
-                .replace("[", "")
-                .replace("]", "")
-                .replace(/;/g, ":");
-            uri.ipv6uri = true;
-        }
-
-        uri.pathNames = pathNames(uri, uri["path"]);
-        uri.queryKey = queryKey(uri, uri["query"]);
-        return uri;
-    };
-
-    function pathNames(obj, path) {
-        var regx = /\/{2,9}/g,
-            names = path.replace(regx, "/").split("/");
-
-        if (path.substr(0, 1) == "/" || path.length === 0) {
-            names.splice(0, 1);
-        }
-
-        if (path.substr(path.length - 1, 1) == "/") {
-            names.splice(names.length - 1, 1);
-        }
-
-        return names;
-    }
-
-    function queryKey(uri, query) {
-        var data = {};
-        query.replace(/(?:^|&)([^&=]*)=?([^&]*)/g, function($0, $1, $2) {
-            if ($1) {
-                data[$1] = $2;
-            }
-        });
-        return data;
-    }
-
-    /**
-     * URL parser.
-     *
-     * @param uri - url
-     * @param path - the request path of the connection
-     * @param loc - An object meant to mimic window.location.
-     *        Defaults to window.location.
-     * @public
-     */
-
-    function url(uri) {
-        var path =
-            arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : "";
-        var loc = arguments.length > 2 ? arguments[2] : undefined;
-        var obj = uri; // default to window.location
-
-        loc = loc || (typeof location !== "undefined" && location);
-        if (null == uri) uri = loc.protocol + "//" + loc.host; // relative path support
-
-        if (typeof uri === "string") {
-            if ("/" === uri.charAt(0)) {
-                if ("/" === uri.charAt(1)) {
-                    uri = loc.protocol + uri;
-                } else {
-                    uri = loc.host + uri;
-                }
-            }
-
-            if (!/^(https?|wss?):\/\//.test(uri)) {
-                if ("undefined" !== typeof loc) {
-                    uri = loc.protocol + "//" + uri;
-                } else {
-                    uri = "https://" + uri;
-                }
-            } // parse
-
-            obj = parseuri(uri);
-        } // make sure we treat `localhost:80` and `localhost` equally
-
-        if (!obj.port) {
-            if (/^(http|ws)$/.test(obj.protocol)) {
-                obj.port = "80";
-            } else if (/^(http|ws)s$/.test(obj.protocol)) {
-                obj.port = "443";
-            }
-        }
-
-        obj.path = obj.path || "/";
-        var ipv6 = obj.host.indexOf(":") !== -1;
-        var host = ipv6 ? "[" + obj.host + "]" : obj.host; // define unique id
-
-        obj.id = obj.protocol + "://" + host + ":" + obj.port + path; // define href
-
-        obj.href =
-            obj.protocol +
-            "://" +
-            host +
-            (loc && loc.port === obj.port ? "" : ":" + obj.port);
-        return obj;
-    }
-
-    var hasCors = {
-        exports: {}
-    };
-
-    /**
-     * Module exports.
-     *
-     * Logic borrowed from Modernizr:
-     *
-     *   - https://github.com/Modernizr/Modernizr/blob/master/feature-detects/cors.js
-     */
-
-    try {
-        hasCors.exports =
-            typeof XMLHttpRequest !== "undefined" &&
-            "withCredentials" in new XMLHttpRequest();
-    } catch (err) {
-        // if XMLHttp support is disabled in IE then it will throw
-        // when trying to create
-        hasCors.exports = false;
-    }
-
-    var hasCORS = hasCors.exports;
-
-    var globalThis = (function() {
-        if (typeof self !== "undefined") {
-            return self;
-        } else if (typeof window !== "undefined") {
-            return window;
-        } else {
-            return Function("return this")();
-        }
-    })();
-
-    // browser shim for xmlhttprequest module
-    function XMLHttpRequest$1(opts) {
-        var xdomain = opts.xdomain; // XMLHttpRequest can be disabled on IE
-
-        try {
-            if ("undefined" !== typeof XMLHttpRequest && (!xdomain || hasCORS)) {
-                return new XMLHttpRequest();
-            }
-        } catch (e) {}
-
-        if (!xdomain) {
-            try {
-                return new globalThis[["Active"].concat("Object").join("X")](
-                    "Microsoft.XMLHTTP"
-                );
-            } catch (e) {}
-        }
-    }
-
-    function pick(obj) {
-        for (
-            var _len = arguments.length,
-                attr = new Array(_len > 1 ? _len - 1 : 0),
-                _key = 1; _key < _len; _key++
-        ) {
-            attr[_key - 1] = arguments[_key];
-        }
-
-        return attr.reduce(function(acc, k) {
-            if (obj.hasOwnProperty(k)) {
-                acc[k] = obj[k];
-            }
-
-            return acc;
-        }, {});
-    } // Keep a reference to the real timeout functions so they can be used when overridden
-
-    var NATIVE_SET_TIMEOUT = setTimeout;
-    var NATIVE_CLEAR_TIMEOUT = clearTimeout;
-
-    function installTimerFunctions(obj, opts) {
-        if (opts.useNativeTimers) {
-            obj.setTimeoutFn = NATIVE_SET_TIMEOUT.bind(globalThis);
-            obj.clearTimeoutFn = NATIVE_CLEAR_TIMEOUT.bind(globalThis);
-        } else {
-            obj.setTimeoutFn = setTimeout.bind(globalThis);
-            obj.clearTimeoutFn = clearTimeout.bind(globalThis);
-        }
-    }
-
-    /**
-     * Expose `Emitter`.
-     */
-
-    var Emitter_1 = Emitter;
-    /**
-     * Initialize a new `Emitter`.
-     *
-     * @api public
-     */
-
-    function Emitter(obj) {
-        if (obj) return mixin(obj);
-    }
-    /**
-     * Mixin the emitter properties.
-     *
-     * @param {Object} obj
-     * @return {Object}
-     * @api private
-     */
-
-    function mixin(obj) {
-        for (var key in Emitter.prototype) {
-            obj[key] = Emitter.prototype[key];
-        }
-
-        return obj;
-    }
-    /**
-     * Listen on the given `event` with `fn`.
-     *
-     * @param {String} event
-     * @param {Function} fn
-     * @return {Emitter}
-     * @api public
-     */
-
-    Emitter.prototype.on = Emitter.prototype.addEventListener = function(
-        event,
-        fn
-    ) {
-        this._callbacks = this._callbacks || {};
-        (this._callbacks["$" + event] = this._callbacks["$" + event] || []).push(
-            fn
-        );
-        return this;
-    };
-    /**
-     * Adds an `event` listener that will be invoked a single
-     * time then automatically removed.
-     *
-     * @param {String} event
-     * @param {Function} fn
-     * @return {Emitter}
-     * @api public
-     */
-
-    Emitter.prototype.once = function(event, fn) {
-        function on() {
-            this.off(event, on);
-            fn.apply(this, arguments);
-        }
-
-        on.fn = fn;
-        this.on(event, on);
-        return this;
-    };
-    /**
-     * Remove the given callback for `event` or all
-     * registered callbacks.
-     *
-     * @param {String} event
-     * @param {Function} fn
-     * @return {Emitter}
-     * @api public
-     */
-
-    Emitter.prototype.off =
-        Emitter.prototype.removeListener =
-        Emitter.prototype.removeAllListeners =
-        Emitter.prototype.removeEventListener =
-        function(event, fn) {
-            this._callbacks = this._callbacks || {}; // all
-
-            if (0 == arguments.length) {
-                this._callbacks = {};
-                return this;
-            } // specific event
-
-            var callbacks = this._callbacks["$" + event];
-            if (!callbacks) return this; // remove all handlers
-
-            if (1 == arguments.length) {
-                delete this._callbacks["$" + event];
-                return this;
-            } // remove specific handler
-
-            var cb;
-
-            for (var i = 0; i < callbacks.length; i++) {
-                cb = callbacks[i];
-
-                if (cb === fn || cb.fn === fn) {
-                    callbacks.splice(i, 1);
-                    break;
-                }
-            } // Remove event specific arrays for event types that no
-            // one is subscribed for to avoid memory leak.
-
-            if (callbacks.length === 0) {
-                delete this._callbacks["$" + event];
-            }
-
-            return this;
-        };
-    /**
-     * Emit `event` with the given args.
-     *
-     * @param {String} event
-     * @param {Mixed} ...
-     * @return {Emitter}
-     */
-
-    Emitter.prototype.emit = function(event) {
-        this._callbacks = this._callbacks || {};
-        var args = new Array(arguments.length - 1),
-            callbacks = this._callbacks["$" + event];
-
-        for (var i = 1; i < arguments.length; i++) {
-            args[i - 1] = arguments[i];
-        }
-
-        if (callbacks) {
-            callbacks = callbacks.slice(0);
-
-            for (var i = 0, len = callbacks.length; i < len; ++i) {
-                callbacks[i].apply(this, args);
-            }
-        }
-
-        return this;
-    }; // alias used for reserved events (protected method)
-
-    Emitter.prototype.emitReserved = Emitter.prototype.emit;
-    /**
-     * Return array of callbacks for `event`.
-     *
-     * @param {String} event
-     * @return {Array}
-     * @api public
-     */
-
-    Emitter.prototype.listeners = function(event) {
-        this._callbacks = this._callbacks || {};
-        return this._callbacks["$" + event] || [];
-    };
-    /**
-     * Check if this emitter has `event` handlers.
-     *
-     * @param {String} event
-     * @return {Boolean}
-     * @api public
-     */
-
-    Emitter.prototype.hasListeners = function(event) {
-        return !!this.listeners(event).length;
-    };
-
-    var PACKET_TYPES = Object.create(null); // no Map = no polyfill
-
-    PACKET_TYPES["open"] = "0";
-    PACKET_TYPES["close"] = "1";
-    PACKET_TYPES["ping"] = "2";
-    PACKET_TYPES["pong"] = "3";
-    PACKET_TYPES["message"] = "4";
-    PACKET_TYPES["upgrade"] = "5";
-    PACKET_TYPES["noop"] = "6";
-    var PACKET_TYPES_REVERSE = Object.create(null);
-    Object.keys(PACKET_TYPES).forEach(function(key) {
-        PACKET_TYPES_REVERSE[PACKET_TYPES[key]] = key;
-    });
-    var ERROR_PACKET = {
-        type: "error",
-        data: "parser error",
-    };
-
-    var withNativeBlob$1 =
-        typeof Blob === "function" ||
-        (typeof Blob !== "undefined" &&
-            Object.prototype.toString.call(Blob) === "[object BlobConstructor]");
-    var withNativeArrayBuffer$2 = typeof ArrayBuffer === "function"; // ArrayBuffer.isView method is not defined in IE10
-
-    var isView$1 = function isView(obj) {
-        return typeof ArrayBuffer.isView === "function" ?
-            ArrayBuffer.isView(obj) :
-            obj && obj.buffer instanceof ArrayBuffer;
-    };
-
-    var encodePacket = function encodePacket(_ref, supportsBinary, callback) {
-        var type = _ref.type,
-            data = _ref.data;
-
-        if (withNativeBlob$1 && data instanceof Blob) {
-            if (supportsBinary) {
-                return callback(data);
-            } else {
-                return encodeBlobAsBase64(data, callback);
-            }
-        } else if (
-            withNativeArrayBuffer$2 &&
-            (data instanceof ArrayBuffer || isView$1(data))
-        ) {
-            if (supportsBinary) {
-                return callback(data);
-            } else {
-                return encodeBlobAsBase64(new Blob([data]), callback);
-            }
-        } // plain string
-
-        return callback(PACKET_TYPES[type] + (data || ""));
-    };
-
-    var encodeBlobAsBase64 = function encodeBlobAsBase64(data, callback) {
-        var fileReader = new FileReader();
-
-        fileReader.onload = function() {
-            var content = fileReader.result.split(",")[1];
-            callback("b" + content);
-        };
-
-        return fileReader.readAsDataURL(data);
-    };
-
-    /*
-     * base64-arraybuffer 1.0.1 <https://github.com/niklasvh/base64-arraybuffer>
-     * Copyright (c) 2021 Niklas von Hertzen <https://hertzen.com>
-     * Released under MIT License
-     */
-    var chars =
-        "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"; // Use a lookup table to find the index.
-
-    var lookup$1 = typeof Uint8Array === "undefined" ? [] : new Uint8Array(256);
-
-    for (var i$1 = 0; i$1 < chars.length; i$1++) {
-        lookup$1[chars.charCodeAt(i$1)] = i$1;
-    }
-
-    var decode$1 = function decode(base64) {
-        var bufferLength = base64.length * 0.75,
-            len = base64.length,
-            i,
-            p = 0,
-            encoded1,
-            encoded2,
-            encoded3,
-            encoded4;
-
-        if (base64[base64.length - 1] === "=") {
-            bufferLength--;
-
-            if (base64[base64.length - 2] === "=") {
-                bufferLength--;
-            }
-        }
-
-        var arraybuffer = new ArrayBuffer(bufferLength),
-            bytes = new Uint8Array(arraybuffer);
-
-        for (i = 0; i < len; i += 4) {
-            encoded1 = lookup$1[base64.charCodeAt(i)];
-            encoded2 = lookup$1[base64.charCodeAt(i + 1)];
-            encoded3 = lookup$1[base64.charCodeAt(i + 2)];
-            encoded4 = lookup$1[base64.charCodeAt(i + 3)];
-            bytes[p++] = (encoded1 << 2) | (encoded2 >> 4);
-            bytes[p++] = ((encoded2 & 15) << 4) | (encoded3 >> 2);
-            bytes[p++] = ((encoded3 & 3) << 6) | (encoded4 & 63);
-        }
-
-        return arraybuffer;
-    };
-
-    var withNativeArrayBuffer$1 = typeof ArrayBuffer === "function";
-
-    var decodePacket = function decodePacket(encodedPacket, binaryType) {
-        if (typeof encodedPacket !== "string") {
-            return {
-                type: "message",
-                data: mapBinary(encodedPacket, binaryType),
-            };
-        }
-
-        var type = encodedPacket.charAt(0);
-
-        if (type === "b") {
-            return {
-                type: "message",
-                data: decodeBase64Packet(encodedPacket.substring(1), binaryType),
-            };
-        }
-
-        var packetType = PACKET_TYPES_REVERSE[type];
-
-        if (!packetType) {
-            return ERROR_PACKET;
-        }
-
-        return encodedPacket.length > 1 ?
-            {
-                type: PACKET_TYPES_REVERSE[type],
-                data: encodedPacket.substring(1),
-            } :
-            {
-                type: PACKET_TYPES_REVERSE[type],
-            };
-    };
-
-    var decodeBase64Packet = function decodeBase64Packet(data, binaryType) {
-        if (withNativeArrayBuffer$1) {
-            var decoded = decode$1(data);
-            return mapBinary(decoded, binaryType);
-        } else {
-            return {
-                base64: true,
-                data: data,
-            }; // fallback for old browsers
-        }
-    };
-
-    var mapBinary = function mapBinary(data, binaryType) {
-        switch (binaryType) {
-            case "blob":
-                return data instanceof ArrayBuffer ? new Blob([data]) : data;
-
-            case "arraybuffer":
-            default:
-                return data;
-                // assuming the data is already an ArrayBuffer
-        }
-    };
-
-    var SEPARATOR = String.fromCharCode(30); // see https://en.wikipedia.org/wiki/Delimiter#ASCII_delimited_text
-
-    var encodePayload = function encodePayload(packets, callback) {
-        // some packets may be added to the array while encoding, so the initial length must be saved
-        var length = packets.length;
-        var encodedPackets = new Array(length);
-        var count = 0;
-        packets.forEach(function(packet, i) {
-            // force base64 encoding for binary packets
-            encodePacket(packet, false, function(encodedPacket) {
-                encodedPackets[i] = encodedPacket;
-
-                if (++count === length) {
-                    callback(encodedPackets.join(SEPARATOR));
-                }
-            });
-        });
-    };
-
-    var decodePayload = function decodePayload(encodedPayload, binaryType) {
-        var encodedPackets = encodedPayload.split(SEPARATOR);
-        var packets = [];
-
-        for (var i = 0; i < encodedPackets.length; i++) {
-            var decodedPacket = decodePacket(encodedPackets[i], binaryType);
-            packets.push(decodedPacket);
-
-            if (decodedPacket.type === "error") {
-                break;
-            }
-        }
-
-        return packets;
-    };
-
-    var protocol$1 = 4;
-
-    var Transport = /*#__PURE__*/ (function(_Emitter) {
-        _inherits(Transport, _Emitter);
-
-        var _super = _createSuper(Transport);
-
-        /**
-         * Transport abstract constructor.
-         *
-         * @param {Object} options.
-         * @api private
-         */
-        function Transport(opts) {
-            var _this;
-
-            _classCallCheck(this, Transport);
-
-            _this = _super.call(this);
-            _this.writable = false;
-            installTimerFunctions(_assertThisInitialized(_this), opts);
-            _this.opts = opts;
-            _this.query = opts.query;
-            _this.readyState = "";
-            _this.socket = opts.socket;
-            return _this;
-        }
-        /**
-         * Emits an error.
-         *
-         * @param {String} str
-         * @return {Transport} for chaining
-         * @api protected
-         */
-
-        _createClass(Transport, [{
-            key: "onError",
-            value: function onError(msg, desc) {
-                var err = new Error(msg); // @ts-ignore
-
-                err.type = "TransportError"; // @ts-ignore
-
-                err.description = desc;
-
-                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
-                    this,
-                    "error",
-                    err
-                );
-
-                return this;
-            },
-            /**
-             * Opens the transport.
-             *
-             * @api public
-             */
-        }, {
-            key: "open",
-            value: function open() {
-                if ("closed" === this.readyState || "" === this.readyState) {
-                    this.readyState = "opening";
-                    this.doOpen();
-                }
-
-                return this;
-            },
-            /**
-             * Closes the transport.
-             *
-             * @api public
-             */
-        }, {
-            key: "close",
-            value: function close() {
-                if ("opening" === this.readyState || "open" === this.readyState) {
-                    this.doClose();
-                    this.onClose();
-                }
-
-                return this;
-            },
-            /**
-             * Sends multiple packets.
-             *
-             * @param {Array} packets
-             * @api public
-             */
-        }, {
-            key: "send",
-            value: function send(packets) {
-                if ("open" === this.readyState) {
-                    this.write(packets);
-                }
-            },
-            /**
-             * Called upon open
-             *
-             * @api protected
-             */
-        }, {
-            key: "onOpen",
-            value: function onOpen() {
-                this.readyState = "open";
-                this.writable = true;
-
-                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
-                    this,
-                    "open"
-                );
-            },
-            /**
-             * Called with data.
-             *
-             * @param {String} data
-             * @api protected
-             */
-        }, {
-            key: "onData",
-            value: function onData(data) {
-                var packet = decodePacket(data, this.socket.binaryType);
-                this.onPacket(packet);
-            },
-            /**
-             * Called with a decoded packet.
-             *
-             * @api protected
-             */
-        }, {
-            key: "onPacket",
-            value: function onPacket(packet) {
-                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
-                    this,
-                    "packet",
-                    packet
-                );
-            },
-            /**
-             * Called upon close.
-             *
-             * @api protected
-             */
-        }, {
-            key: "onClose",
-            value: function onClose() {
-                this.readyState = "closed";
-
-                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
-                    this,
-                    "close"
-                );
-            },
-        }, ]);
-
-        return Transport;
-    })(Emitter_1);
-
-    var alphabet =
-        "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz-_".split(
-            ""
-        ),
-        length = 64,
-        map = {},
-        seed = 0,
-        i = 0,
-        prev;
-    /**
-     * Return a string representing the specified number.
-     *
-     * @param {Number} num The number to convert.
-     * @returns {String} The string representation of the number.
-     * @api public
-     */
-
-    function encode(num) {
-        var encoded = "";
-
-        do {
-            encoded = alphabet[num % length] + encoded;
-            num = Math.floor(num / length);
-        } while (num > 0);
-
-        return encoded;
-    }
-    /**
-     * Return the integer value specified by the given string.
-     *
-     * @param {String} str The string to convert.
-     * @returns {Number} The integer value represented by the string.
-     * @api public
-     */
-
-    function decode(str) {
-        var decoded = 0;
-
-        for (i = 0; i < str.length; i++) {
-            decoded = decoded * length + map[str.charAt(i)];
-        }
-
-        return decoded;
-    }
-    /**
-     * Yeast: A tiny growing id generator.
-     *
-     * @returns {String} A unique id.
-     * @api public
-     */
-
-    function yeast() {
-        var now = encode(+new Date());
-        if (now !== prev) return (seed = 0), (prev = now);
-        return now + "." + encode(seed++);
-    } //
-    // Map each character to its index.
-    //
-
-    for (; i < length; i++) {
-        map[alphabet[i]] = i;
-    } //
-    // Expose the `yeast`, `encode` and `decode` functions.
-    //
-
-    yeast.encode = encode;
-    yeast.decode = decode;
-    var yeast_1 = yeast;
-
-    var parseqs = {};
-
-    /**
-     * Compiles a querystring
-     * Returns string representation of the object
-     *
-     * @param {Object}
-     * @api private
-     */
-
-    parseqs.encode = function(obj) {
-        var str = "";
-
-        for (var i in obj) {
-            if (obj.hasOwnProperty(i)) {
-                if (str.length) str += "&";
-                str += encodeURIComponent(i) + "=" + encodeURIComponent(obj[i]);
-            }
-        }
-
-        return str;
-    };
-    /**
-     * Parses a simple querystring into an object
-     *
-     * @param {String} qs
-     * @api private
-     */
-
-    parseqs.decode = function(qs) {
-        var qry = {};
-        var pairs = qs.split("&");
-
-        for (var i = 0, l = pairs.length; i < l; i++) {
-            var pair = pairs[i].split("=");
-            qry[decodeURIComponent(pair[0])] = decodeURIComponent(pair[1]);
-        }
-
-        return qry;
-    };
-
-    var Polling = /*#__PURE__*/ (function(_Transport) {
-        _inherits(Polling, _Transport);
-
-        var _super = _createSuper(Polling);
-
-        function Polling() {
-            var _this;
-
-            _classCallCheck(this, Polling);
-
-            _this = _super.apply(this, arguments);
-            _this.polling = false;
-            return _this;
-        }
-        /**
-         * Transport name.
-         */
-
-        _createClass(Polling, [{
-            key: "name",
-            get: function get() {
-                return "polling";
-            },
-            /**
-             * Opens the socket (triggers polling). We write a PING message to determine
-             * when the transport is open.
-             *
-             * @api private
-             */
-        }, {
-            key: "doOpen",
-            value: function doOpen() {
-                this.poll();
-            },
-            /**
-             * Pauses polling.
-             *
-             * @param {Function} callback upon buffers are flushed and transport is paused
-             * @api private
-             */
-        }, {
-            key: "pause",
-            value: function pause(onPause) {
-                var _this2 = this;
-
-                this.readyState = "pausing";
-
-                var pause = function pause() {
-                    _this2.readyState = "paused";
-                    onPause();
-                };
-
-                if (this.polling || !this.writable) {
-                    var total = 0;
-
-                    if (this.polling) {
-                        total++;
-                        this.once("pollComplete", function() {
-                            --total || pause();
-                        });
-                    }
-
-                    if (!this.writable) {
-                        total++;
-                        this.once("drain", function() {
-                            --total || pause();
-                        });
-                    }
-                } else {
-                    pause();
-                }
-            },
-            /**
-             * Starts polling cycle.
-             *
-             * @api public
-             */
-        }, {
-            key: "poll",
-            value: function poll() {
-                this.polling = true;
-                this.doPoll();
-                this.emit("poll");
-            },
-            /**
-             * Overloads onData to detect payloads.
-             *
-             * @api private
-             */
-        }, {
-            key: "onData",
-            value: function onData(data) {
-                var _this3 = this;
-
-                var callback = function callback(packet) {
-                    // if its the first message we consider the transport open
-                    if ("opening" === _this3.readyState && packet.type === "open") {
-                        _this3.onOpen();
-                    } // if its a close packet, we close the ongoing requests
-
-                    if ("close" === packet.type) {
-                        _this3.onClose();
-
-                        return false;
-                    } // otherwise bypass onData and handle the message
-
-                    _this3.onPacket(packet);
-                }; // decode payload
-
-                decodePayload(data, this.socket.binaryType).forEach(callback); // if an event did not trigger closing
-
-                if ("closed" !== this.readyState) {
-                    // if we got data we're not polling
-                    this.polling = false;
-                    this.emit("pollComplete");
-
-                    if ("open" === this.readyState) {
-                        this.poll();
-                    }
-                }
-            },
-            /**
-             * For polling, send a close packet.
-             *
-             * @api private
-             */
-        }, {
-            key: "doClose",
-            value: function doClose() {
-                var _this4 = this;
-
-                var close = function close() {
-                    _this4.write([{
-                        type: "close",
-                    }, ]);
-                };
-
-                if ("open" === this.readyState) {
-                    close();
-                } else {
-                    // in case we're trying to close while
-                    // handshaking is in progress (GH-164)
-                    this.once("open", close);
-                }
-            },
-            /**
-             * Writes a packets payload.
-             *
-             * @param {Array} data packets
-             * @param {Function} drain callback
-             * @api private
-             */
-        }, {
-            key: "write",
-            value: function write(packets) {
-                var _this5 = this;
-
-                this.writable = false;
-                encodePayload(packets, function(data) {
-                    _this5.doWrite(data, function() {
-                        _this5.writable = true;
-
-                        _this5.emit("drain");
-                    });
-                });
-            },
-            /**
-             * Generates uri for connection.
-             *
-             * @api private
-             */
-        }, {
-            key: "uri",
-            value: function uri() {
-                var query = this.query || {};
-                var schema = this.opts.secure ? "https" : "http";
-                var port = ""; // cache busting is forced
-
-                if (false !== this.opts.timestampRequests) {
-                    query[this.opts.timestampParam] = yeast_1();
-                }
-
-                if (!this.supportsBinary && !query.sid) {
-                    query.b64 = 1;
-                } // avoid port if default for schema
-
-                if (
-                    this.opts.port &&
-                    (("https" === schema && Number(this.opts.port) !== 443) ||
-                        ("http" === schema && Number(this.opts.port) !== 80))
-                ) {
-                    port = ":" + this.opts.port;
-                }
-
-                var encodedQuery = parseqs.encode(query);
-                var ipv6 = this.opts.hostname.indexOf(":") !== -1;
-                return (
-                    schema +
-                    "://" +
-                    (ipv6 ? "[" + this.opts.hostname + "]" : this.opts.hostname) +
-                    port +
-                    this.opts.path +
-                    (encodedQuery.length ? "?" + encodedQuery : "")
-                );
-            },
-        }, ]);
-
-        return Polling;
-    })(Transport);
-
-    /**
-     * Empty function
-     */
-
-    function empty() {}
-
-    var hasXHR2 = (function() {
-        var xhr = new XMLHttpRequest$1({
-            xdomain: false,
-        });
-        return null != xhr.responseType;
-    })();
-
-    var XHR = /*#__PURE__*/ (function(_Polling) {
-        _inherits(XHR, _Polling);
-
-        var _super = _createSuper(XHR);
-
-        /**
-         * XHR Polling constructor.
-         *
-         * @param {Object} opts
-         * @api public
-         */
-        function XHR(opts) {
-            var _this;
-
-            _classCallCheck(this, XHR);
-
-            _this = _super.call(this, opts);
-
-            if (typeof location !== "undefined") {
-                var isSSL = "https:" === location.protocol;
-                var port = location.port; // some user agents have empty `location.port`
-
-                if (!port) {
-                    port = isSSL ? "443" : "80";
-                }
-
-                _this.xd =
-                    (typeof location !== "undefined" &&
-                        opts.hostname !== location.hostname) ||
-                    port !== opts.port;
-                _this.xs = opts.secure !== isSSL;
-            }
-            /**
-             * XHR supports binary
-             */
-
-            var forceBase64 = opts && opts.forceBase64;
-            _this.supportsBinary = hasXHR2 && !forceBase64;
-            return _this;
-        }
-        /**
-         * Creates a request.
-         *
-         * @param {String} method
-         * @api private
-         */
-
-        _createClass(XHR, [{
-            key: "request",
-            value: function request() {
-                var opts =
-                    arguments.length > 0 && arguments[0] !== undefined ?
-                    arguments[0] :
-                    {};
-
-                _extends(
-                    opts, {
-                        xd: this.xd,
-                        xs: this.xs,
-                    },
-                    this.opts
-                );
-
-                return new Request(this.uri(), opts);
-            },
-            /**
-             * Sends data.
-             *
-             * @param {String} data to send.
-             * @param {Function} called upon flush.
-             * @api private
-             */
-        }, {
-            key: "doWrite",
-            value: function doWrite(data, fn) {
-                var _this2 = this;
-
-                var req = this.request({
-                    method: "POST",
-                    data: data,
-                });
-                req.on("success", fn);
-                req.on("error", function(err) {
-                    _this2.onError("xhr post error", err);
-                });
-            },
-            /**
-             * Starts a poll cycle.
-             *
-             * @api private
-             */
-        }, {
-            key: "doPoll",
-            value: function doPoll() {
-                var _this3 = this;
-
-                var req = this.request();
-                req.on("data", this.onData.bind(this));
-                req.on("error", function(err) {
-                    _this3.onError("xhr poll error", err);
-                });
-                this.pollXhr = req;
-            },
-        }, ]);
-
-        return XHR;
-    })(Polling);
-    var Request = /*#__PURE__*/ (function(_Emitter) {
-        _inherits(Request, _Emitter);
-
-        var _super2 = _createSuper(Request);
-
-        /**
-         * Request constructor
-         *
-         * @param {Object} options
-         * @api public
-         */
-        function Request(uri, opts) {
-            var _this4;
-
-            _classCallCheck(this, Request);
-
-            _this4 = _super2.call(this);
-            installTimerFunctions(_assertThisInitialized(_this4), opts);
-            _this4.opts = opts;
-            _this4.method = opts.method || "GET";
-            _this4.uri = uri;
-            _this4.async = false !== opts.async;
-            _this4.data = undefined !== opts.data ? opts.data : null;
-
-            _this4.create();
-
-            return _this4;
-        }
-        /**
-         * Creates the XHR object and sends the request.
-         *
-         * @api private
-         */
-
-        _createClass(Request, [{
-            key: "create",
-            value: function create() {
-                var _this5 = this;
-
-                var opts = pick(
-                    this.opts,
-                    "agent",
-                    "pfx",
-                    "key",
-                    "passphrase",
-                    "cert",
-                    "ca",
-                    "ciphers",
-                    "rejectUnauthorized",
-                    "autoUnref"
-                );
-                opts.xdomain = !!this.opts.xd;
-                opts.xscheme = !!this.opts.xs;
-                var xhr = (this.xhr = new XMLHttpRequest$1(opts));
-
-                try {
-                    xhr.open(this.method, this.uri, this.async);
-
-                    try {
-                        if (this.opts.extraHeaders) {
-                            xhr.setDisableHeaderCheck && xhr.setDisableHeaderCheck(true);
-
-                            for (var i in this.opts.extraHeaders) {
-                                if (this.opts.extraHeaders.hasOwnProperty(i)) {
-                                    xhr.setRequestHeader(i, this.opts.extraHeaders[i]);
-                                }
-                            }
-                        }
-                    } catch (e) {}
-
-                    if ("POST" === this.method) {
-                        try {
-                            xhr.setRequestHeader(
-                                "Content-type",
-                                "text/plain;charset=UTF-8"
-                            );
-                        } catch (e) {}
-                    }
-
-                    try {
-                        xhr.setRequestHeader("Accept", "*/*");
-                    } catch (e) {} // ie6 check
-
-                    if ("withCredentials" in xhr) {
-                        xhr.withCredentials = this.opts.withCredentials;
-                    }
-
-                    if (this.opts.requestTimeout) {
-                        xhr.timeout = this.opts.requestTimeout;
-                    }
-
-                    xhr.onreadystatechange = function() {
-                        if (4 !== xhr.readyState) return;
-
-                        if (200 === xhr.status || 1223 === xhr.status) {
-                            _this5.onLoad();
-                        } else {
-                            // make sure the `error` event handler that's user-set
-                            // does not throw in the same tick and gets caught here
-                            _this5.setTimeoutFn(function() {
-                                _this5.onError(
-                                    typeof xhr.status === "number" ? xhr.status : 0
-                                );
-                            }, 0);
-                        }
-                    };
-
-                    xhr.send(this.data);
-                } catch (e) {
-                    // Need to defer since .create() is called directly from the constructor
-                    // and thus the 'error' event can only be only bound *after* this exception
-                    // occurs.  Therefore, also, we cannot throw here at all.
-                    this.setTimeoutFn(function() {
-                        _this5.onError(e);
-                    }, 0);
-                    return;
-                }
-
-                if (typeof document !== "undefined") {
-                    this.index = Request.requestsCount++;
-                    Request.requests[this.index] = this;
-                }
-            },
-            /**
-             * Called upon successful response.
-             *
-             * @api private
-             */
-        }, {
-            key: "onSuccess",
-            value: function onSuccess() {
-                this.emit("success");
-                this.cleanup();
-            },
-            /**
-             * Called if we have data.
-             *
-             * @api private
-             */
-        }, {
-            key: "onData",
-            value: function onData(data) {
-                this.emit("data", data);
-                this.onSuccess();
-            },
-            /**
-             * Called upon error.
-             *
-             * @api private
-             */
-        }, {
-            key: "onError",
-            value: function onError(err) {
-                this.emit("error", err);
-                this.cleanup(true);
-            },
-            /**
-             * Cleans up house.
-             *
-             * @api private
-             */
-        }, {
-            key: "cleanup",
-            value: function cleanup(fromError) {
-                if ("undefined" === typeof this.xhr || null === this.xhr) {
-                    return;
-                }
-
-                this.xhr.onreadystatechange = empty;
-
-                if (fromError) {
-                    try {
-                        this.xhr.abort();
-                    } catch (e) {}
-                }
-
-                if (typeof document !== "undefined") {
-                    delete Request.requests[this.index];
-                }
-
-                this.xhr = null;
-            },
-            /**
-             * Called upon load.
-             *
-             * @api private
-             */
-        }, {
-            key: "onLoad",
-            value: function onLoad() {
-                var data = this.xhr.responseText;
-
-                if (data !== null) {
-                    this.onData(data);
-                }
-            },
-            /**
-             * Aborts the request.
-             *
-             * @api public
-             */
-        }, {
-            key: "abort",
-            value: function abort() {
-                this.cleanup();
-            },
-        }, ]);
-
-        return Request;
-    })(Emitter_1);
-    Request.requestsCount = 0;
-    Request.requests = {};
-    /**
-     * Aborts pending requests when unloading the window. This is needed to prevent
-     * memory leaks (e.g. when using IE) and to ensure that no spurious error is
-     * emitted.
-     */
-
-    if (typeof document !== "undefined") {
-        // @ts-ignore
-        if (typeof attachEvent === "function") {
-            // @ts-ignore
-            attachEvent("onunload", unloadHandler);
-        } else if (typeof addEventListener === "function") {
-            var terminationEvent = "onpagehide" in globalThis ? "pagehide" : "unload";
-            addEventListener(terminationEvent, unloadHandler, false);
-        }
-    }
-
-    function unloadHandler() {
-        for (var i in Request.requests) {
-            if (Request.requests.hasOwnProperty(i)) {
-                Request.requests[i].abort();
-            }
-        }
-    }
-
-    var nextTick = (function() {
-        var isPromiseAvailable =
-            typeof Promise === "function" && typeof Promise.resolve === "function";
-
-        if (isPromiseAvailable) {
-            return function(cb) {
-                return Promise.resolve().then(cb);
-            };
-        } else {
-            return function(cb, setTimeoutFn) {
-                return setTimeoutFn(cb, 0);
-            };
-        }
-    })();
-    var WebSocket = globalThis.WebSocket || globalThis.MozWebSocket;
-    var usingBrowserWebSocket = true;
-    var defaultBinaryType = "arraybuffer";
-
-    var isReactNative =
-        typeof navigator !== "undefined" &&
-        typeof navigator.product === "string" &&
-        navigator.product.toLowerCase() === "reactnative";
-    var WS = /*#__PURE__*/ (function(_Transport) {
-        _inherits(WS, _Transport);
-
-        var _super = _createSuper(WS);
-
-        /**
-         * WebSocket transport constructor.
-         *
-         * @api {Object} connection options
-         * @api public
-         */
-        function WS(opts) {
-            var _this;
-
-            _classCallCheck(this, WS);
-
-            _this = _super.call(this, opts);
-            _this.supportsBinary = !opts.forceBase64;
-            return _this;
-        }
-        /**
-         * Transport name.
-         *
-         * @api public
-         */
-
-        _createClass(WS, [{
-            key: "name",
-            get: function get() {
-                return "websocket";
-            },
-            /**
-             * Opens socket.
-             *
-             * @api private
-             */
-        }, {
-            key: "doOpen",
-            value: function doOpen() {
-                if (!this.check()) {
-                    // let probe timeout
-                    return;
-                }
-
-                var uri = this.uri();
-                var protocols = this.opts.protocols; // React Native only supports the 'headers' option, and will print a warning if anything else is passed
-
-                var opts = isReactNative ?
-                    {} :
-                    pick(
-                        this.opts,
-                        "agent",
-                        "perMessageDeflate",
-                        "pfx",
-                        "key",
-                        "passphrase",
-                        "cert",
-                        "ca",
-                        "ciphers",
-                        "rejectUnauthorized",
-                        "localAddress",
-                        "protocolVersion",
-                        "origin",
-                        "maxPayload",
-                        "family",
-                        "checkServerIdentity"
-                    );
-
-                if (this.opts.extraHeaders) {
-                    opts.headers = this.opts.extraHeaders;
-                }
-
-                try {
-                    this.ws =
-                        usingBrowserWebSocket && !isReactNative ?
-                        protocols ?
-                        new WebSocket(uri, protocols) :
-                        new WebSocket(uri) :
-                        new WebSocket(uri, protocols, opts);
-                } catch (err) {
-                    return this.emit("error", err);
-                }
-
-                this.ws.binaryType = this.socket.binaryType || defaultBinaryType;
-                this.addEventListeners();
-            },
-            /**
-             * Adds event listeners to the socket
-             *
-             * @api private
-             */
-        }, {
-            key: "addEventListeners",
-            value: function addEventListeners() {
-                var _this2 = this;
-
-                this.ws.onopen = function() {
-                    if (_this2.opts.autoUnref) {
-                        _this2.ws._socket.unref();
-                    }
-
-                    _this2.onOpen();
-                };
-
-                this.ws.onclose = this.onClose.bind(this);
-
-                this.ws.onmessage = function(ev) {
-                    return _this2.onData(ev.data);
-                };
-
-                this.ws.onerror = function(e) {
-                    return _this2.onError("websocket error", e);
-                };
-            },
-            /**
-             * Writes data to socket.
-             *
-             * @param {Array} array of packets.
-             * @api private
-             */
-        }, {
-            key: "write",
-            value: function write(packets) {
-                var _this3 = this;
-
-                this.writable = false; // encodePacket efficient as it uses WS framing
-                // no need for encodePayload
-
-                var _loop = function _loop(i) {
-                    var packet = packets[i];
-                    var lastPacket = i === packets.length - 1;
-                    encodePacket(packet, _this3.supportsBinary, function(data) {
-                        // always create a new object (GH-437)
-                        var opts = {};
-                        // have a chance of informing us about it yet, in that case send will
-                        // throw an error
-
-                        try {
-                            if (usingBrowserWebSocket) {
-                                // TypeError is thrown when passing the second argument on Safari
-                                _this3.ws.send(data);
-                            }
-                        } catch (e) {}
-
-                        if (lastPacket) {
-                            // fake drain
-                            // defer to next tick to allow Socket to clear writeBuffer
-                            nextTick(function() {
-                                _this3.writable = true;
-
-                                _this3.emit("drain");
-                            }, _this3.setTimeoutFn);
-                        }
-                    });
-                };
-
-                for (var i = 0; i < packets.length; i++) {
-                    _loop(i);
-                }
-            },
-            /**
-             * Closes socket.
-             *
-             * @api private
-             */
-        }, {
-            key: "doClose",
-            value: function doClose() {
-                if (typeof this.ws !== "undefined") {
-                    this.ws.close();
-                    this.ws = null;
-                }
-            },
-            /**
-             * Generates uri for connection.
-             *
-             * @api private
-             */
-        }, {
-            key: "uri",
-            value: function uri() {
-                var query = this.query || {};
-                var schema = this.opts.secure ? "wss" : "ws";
-                var port = ""; // avoid port if default for schema
-
-                if (
-                    this.opts.port &&
-                    (("wss" === schema && Number(this.opts.port) !== 443) ||
-                        ("ws" === schema && Number(this.opts.port) !== 80))
-                ) {
-                    port = ":" + this.opts.port;
-                } // append timestamp to URI
-
-                if (this.opts.timestampRequests) {
-                    query[this.opts.timestampParam] = yeast_1();
-                } // communicate binary support capabilities
-
-                if (!this.supportsBinary) {
-                    query.b64 = 1;
-                }
-
-                var encodedQuery = parseqs.encode(query);
-                var ipv6 = this.opts.hostname.indexOf(":") !== -1;
-                return (
-                    schema +
-                    "://" +
-                    (ipv6 ? "[" + this.opts.hostname + "]" : this.opts.hostname) +
-                    port +
-                    this.opts.path +
-                    (encodedQuery.length ? "?" + encodedQuery : "")
-                );
-            },
-            /**
-             * Feature detection for WebSocket.
-             *
-             * @return {Boolean} whether this transport is available.
-             * @api public
-             */
-        }, {
-            key: "check",
-            value: function check() {
-                return (
-                    !!WebSocket &&
-                    !("__initialize" in WebSocket && this.name === WS.prototype.name)
-                );
-            },
-        }, ]);
-
-        return WS;
-    })(Transport);
-
-    var transports = {
-        websocket: WS,
-        polling: XHR,
-    };
-
-    var Socket$1 = /*#__PURE__*/ (function(_Emitter) {
-        _inherits(Socket, _Emitter);
-
-        var _super = _createSuper(Socket);
-
-        /**
-         * Socket constructor.
-         *
-         * @param {String|Object} uri or options
-         * @param {Object} opts - options
-         * @api public
-         */
-        function Socket(uri) {
-            var _this;
-
-            var opts =
-                arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};
-
-            _classCallCheck(this, Socket);
-
-            _this = _super.call(this);
-
-            if (uri && "object" === _typeof(uri)) {
-                opts = uri;
-                uri = null;
-            }
-
-            if (uri) {
-                uri = parseuri(uri);
-                opts.hostname = uri.host;
-                opts.secure = uri.protocol === "https" || uri.protocol === "wss";
-                opts.port = uri.port;
-                if (uri.query) opts.query = uri.query;
-            } else if (opts.host) {
-                opts.hostname = parseuri(opts.host).host;
-            }
-
-            installTimerFunctions(_assertThisInitialized(_this), opts);
-            _this.secure =
-                null != opts.secure ?
-                opts.secure :
-                typeof location !== "undefined" && "https:" === location.protocol;
-
-            if (opts.hostname && !opts.port) {
-                // if no port is specified manually, use the protocol default
-                opts.port = _this.secure ? "443" : "80";
-            }
-
-            _this.hostname =
-                opts.hostname ||
-                (typeof location !== "undefined" ? location.hostname : "localhost");
-            _this.port =
-                opts.port ||
-                (typeof location !== "undefined" && location.port ?
-                    location.port :
-                    _this.secure ?
-                    "443" :
-                    "80");
-            _this.transports = opts.transports || ["polling", "websocket"];
-            _this.readyState = "";
-            _this.writeBuffer = [];
-            _this.prevBufferLen = 0;
-            _this.opts = _extends({
-                    path: "/engine.io",
-                    agent: false,
-                    withCredentials: false,
-                    upgrade: true,
-                    timestampParam: "t",
-                    rememberUpgrade: false,
-                    rejectUnauthorized: true,
-                    perMessageDeflate: {
-                        threshold: 1024,
-                    },
-                    transportOptions: {},
-                    closeOnBeforeunload: true,
-                },
-                opts
-            );
-            _this.opts.path = _this.opts.path.replace(/\/$/, "") + "/";
-
-            if (typeof _this.opts.query === "string") {
-                _this.opts.query = parseqs.decode(_this.opts.query);
-            } // set on handshake
-
-            _this.id = null;
-            _this.upgrades = null;
-            _this.pingInterval = null;
-            _this.pingTimeout = null; // set on heartbeat
-
-            _this.pingTimeoutTimer = null;
-
-            if (typeof addEventListener === "function") {
-                if (_this.opts.closeOnBeforeunload) {
-                    // Firefox closes the connection when the "beforeunload" event is emitted but not Chrome. This event listener
-                    // ensures every browser behaves the same (no "disconnect" event at the Socket.IO level when the page is
-                    // closed/reloaded)
-                    addEventListener(
-                        "beforeunload",
-                        function() {
-                            if (_this.transport) {
-                                // silently close the transport
-                                _this.transport.removeAllListeners();
-
-                                _this.transport.close();
-                            }
-                        },
-                        false
-                    );
-                }
-
-                if (_this.hostname !== "localhost") {
-                    _this.offlineEventListener = function() {
-                        _this.onClose("transport close");
-                    };
-
-                    addEventListener("offline", _this.offlineEventListener, false);
-                }
-            }
-
-            _this.open();
-
-            return _this;
-        }
-        /**
-         * Creates transport of the given type.
-         *
-         * @param {String} transport name
-         * @return {Transport}
-         * @api private
-         */
-
-        _createClass(Socket, [{
-            key: "createTransport",
-            value: function createTransport(name) {
-                var query = clone(this.opts.query); // append engine.io protocol identifier
-
-                query.EIO = protocol$1; // transport name
-
-                query.transport = name; // session id if we already have one
-
-                if (this.id) query.sid = this.id;
-
-                var opts = _extends({}, this.opts.transportOptions[name], this.opts, {
-                    query: query,
-                    socket: this,
-                    hostname: this.hostname,
-                    secure: this.secure,
-                    port: this.port,
-                });
-
-                return new transports[name](opts);
-            },
-            /**
-             * Initializes transport to use and starts probe.
-             *
-             * @api private
-             */
-        }, {
-            key: "open",
-            value: function open() {
-                var _this2 = this;
-
-                var transport;
-
-                if (
-                    this.opts.rememberUpgrade &&
-                    Socket.priorWebsocketSuccess &&
-                    this.transports.indexOf("websocket") !== -1
-                ) {
-                    transport = "websocket";
-                } else if (0 === this.transports.length) {
-                    // Emit error on next tick so it can be listened to
-                    this.setTimeoutFn(function() {
-                        _this2.emitReserved("error", "No transports available");
-                    }, 0);
-                    return;
-                } else {
-                    transport = this.transports[0];
-                }
-
-                this.readyState = "opening"; // Retry with the next transport if the transport is disabled (jsonp: false)
-
-                try {
-                    transport = this.createTransport(transport);
-                } catch (e) {
-                    this.transports.shift();
-                    this.open();
-                    return;
-                }
-
-                transport.open();
-                this.setTransport(transport);
-            },
-            /**
-             * Sets the current transport. Disables the existing one (if any).
-             *
-             * @api private
-             */
-        }, {
-            key: "setTransport",
-            value: function setTransport(transport) {
-                var _this3 = this;
-
-                if (this.transport) {
-                    this.transport.removeAllListeners();
-                } // set up transport
-
-                this.transport = transport; // set up transport listeners
-
-                transport
-                    .on("drain", this.onDrain.bind(this))
-                    .on("packet", this.onPacket.bind(this))
-                    .on("error", this.onError.bind(this))
-                    .on("close", function() {
-                        _this3.onClose("transport close");
-                    });
-            },
-            /**
-             * Probes a transport.
-             *
-             * @param {String} transport name
-             * @api private
-             */
-        }, {
-            key: "probe",
-            value: function probe(name) {
-                var _this4 = this;
-
-                var transport = this.createTransport(name);
-                var failed = false;
-                Socket.priorWebsocketSuccess = false;
-
-                var onTransportOpen = function onTransportOpen() {
-                    if (failed) return;
-                    transport.send([{
-                        type: "ping",
-                        data: "probe",
-                    }, ]);
-                    transport.once("packet", function(msg) {
-                        if (failed) return;
-
-                        if ("pong" === msg.type && "probe" === msg.data) {
-                            _this4.upgrading = true;
-
-                            _this4.emitReserved("upgrading", transport);
-
-                            if (!transport) return;
-                            Socket.priorWebsocketSuccess = "websocket" === transport.name;
-
-                            _this4.transport.pause(function() {
-                                if (failed) return;
-                                if ("closed" === _this4.readyState) return;
-                                cleanup();
-
-                                _this4.setTransport(transport);
-
-                                transport.send([{
-                                    type: "upgrade",
-                                }, ]);
-
-                                _this4.emitReserved("upgrade", transport);
-
-                                transport = null;
-                                _this4.upgrading = false;
-
-                                _this4.flush();
-                            });
-                        } else {
-                            var err = new Error("probe error"); // @ts-ignore
-
-                            err.transport = transport.name;
-
-                            _this4.emitReserved("upgradeError", err);
-                        }
-                    });
-                };
-
-                function freezeTransport() {
-                    if (failed) return; // Any callback called by transport should be ignored since now
-
-                    failed = true;
-                    cleanup();
-                    transport.close();
-                    transport = null;
-                } // Handle any error that happens while probing
-
-                var onerror = function onerror(err) {
-                    var error = new Error("probe error: " + err); // @ts-ignore
-
-                    error.transport = transport.name;
-                    freezeTransport();
-
-                    _this4.emitReserved("upgradeError", error);
-                };
-
-                function onTransportClose() {
-                    onerror("transport closed");
-                } // When the socket is closed while we're probing
-
-                function onclose() {
-                    onerror("socket closed");
-                } // When the socket is upgraded while we're probing
-
-                function onupgrade(to) {
-                    if (transport && to.name !== transport.name) {
-                        freezeTransport();
-                    }
-                } // Remove all listeners on the transport and on self
-
-                var cleanup = function cleanup() {
-                    transport.removeListener("open", onTransportOpen);
-                    transport.removeListener("error", onerror);
-                    transport.removeListener("close", onTransportClose);
-
-                    _this4.off("close", onclose);
-
-                    _this4.off("upgrading", onupgrade);
-                };
-
-                transport.once("open", onTransportOpen);
-                transport.once("error", onerror);
-                transport.once("close", onTransportClose);
-                this.once("close", onclose);
-                this.once("upgrading", onupgrade);
-                transport.open();
-            },
-            /**
-             * Called when connection is deemed open.
-             *
-             * @api private
-             */
-        }, {
-            key: "onOpen",
-            value: function onOpen() {
-                this.readyState = "open";
-                Socket.priorWebsocketSuccess = "websocket" === this.transport.name;
-                this.emitReserved("open");
-                this.flush(); // we check for `readyState` in case an `open`
-                // listener already closed the socket
-
-                if (
-                    "open" === this.readyState &&
-                    this.opts.upgrade &&
-                    this.transport.pause
-                ) {
-                    var i = 0;
-                    var l = this.upgrades.length;
-
-                    for (; i < l; i++) {
-                        this.probe(this.upgrades[i]);
-                    }
-                }
-            },
-            /**
-             * Handles a packet.
-             *
-             * @api private
-             */
-        }, {
-            key: "onPacket",
-            value: function onPacket(packet) {
-                if (
-                    "opening" === this.readyState ||
-                    "open" === this.readyState ||
-                    "closing" === this.readyState
-                ) {
-                    this.emitReserved("packet", packet); // Socket is live - any packet counts
-
-                    this.emitReserved("heartbeat");
-
-                    switch (packet.type) {
-                        case "open":
-                            this.onHandshake(JSON.parse(packet.data));
-                            break;
-
-                        case "ping":
-                            this.resetPingTimeout();
-                            this.sendPacket("pong");
-                            this.emitReserved("ping");
-                            this.emitReserved("pong");
-                            break;
-
-                        case "error":
-                            var err = new Error("server error"); // @ts-ignore
-
-                            err.code = packet.data;
-                            this.onError(err);
-                            break;
-
-                        case "message":
-                            this.emitReserved("data", packet.data);
-                            this.emitReserved("message", packet.data);
-                            break;
-                    }
-                }
-            },
-            /**
-             * Called upon handshake completion.
-             *
-             * @param {Object} data - handshake obj
-             * @api private
-             */
-        }, {
-            key: "onHandshake",
-            value: function onHandshake(data) {
-                this.emitReserved("handshake", data);
-                this.id = data.sid;
-                this.transport.query.sid = data.sid;
-                this.upgrades = this.filterUpgrades(data.upgrades);
-                this.pingInterval = data.pingInterval;
-                this.pingTimeout = data.pingTimeout;
-                this.onOpen(); // In case open handler closes socket
-
-                if ("closed" === this.readyState) return;
-                this.resetPingTimeout();
-            },
-            /**
-             * Sets and resets ping timeout timer based on server pings.
-             *
-             * @api private
-             */
-        }, {
-            key: "resetPingTimeout",
-            value: function resetPingTimeout() {
-                var _this5 = this;
-
-                this.clearTimeoutFn(this.pingTimeoutTimer);
-                this.pingTimeoutTimer = this.setTimeoutFn(function() {
-                    _this5.onClose("ping timeout");
-                }, this.pingInterval + this.pingTimeout);
-
-                if (this.opts.autoUnref) {
-                    this.pingTimeoutTimer.unref();
-                }
-            },
-            /**
-             * Called on `drain` event
-             *
-             * @api private
-             */
-        }, {
-            key: "onDrain",
-            value: function onDrain() {
-                this.writeBuffer.splice(0, this.prevBufferLen); // setting prevBufferLen = 0 is very important
-                // for example, when upgrading, upgrade packet is sent over,
-                // and a nonzero prevBufferLen could cause problems on `drain`
-
-                this.prevBufferLen = 0;
-
-                if (0 === this.writeBuffer.length) {
-                    this.emitReserved("drain");
-                } else {
-                    this.flush();
-                }
-            },
-            /**
-             * Flush write buffers.
-             *
-             * @api private
-             */
-        }, {
-            key: "flush",
-            value: function flush() {
-                if (
-                    "closed" !== this.readyState &&
-                    this.transport.writable &&
-                    !this.upgrading &&
-                    this.writeBuffer.length
-                ) {
-                    this.transport.send(this.writeBuffer); // keep track of current length of writeBuffer
-                    // splice writeBuffer and callbackBuffer on `drain`
-
-                    this.prevBufferLen = this.writeBuffer.length;
-                    this.emitReserved("flush");
-                }
-            },
-            /**
-             * Sends a message.
-             *
-             * @param {String} message.
-             * @param {Function} callback function.
-             * @param {Object} options.
-             * @return {Socket} for chaining.
-             * @api public
-             */
-        }, {
-            key: "write",
-            value: function write(msg, options, fn) {
-                this.sendPacket("message", msg, options, fn);
-                return this;
-            },
-        }, {
-            key: "send",
-            value: function send(msg, options, fn) {
-                this.sendPacket("message", msg, options, fn);
-                return this;
-            },
-            /**
-             * Sends a packet.
-             *
-             * @param {String} packet type.
-             * @param {String} data.
-             * @param {Object} options.
-             * @param {Function} callback function.
-             * @api private
-             */
-        }, {
-            key: "sendPacket",
-            value: function sendPacket(type, data, options, fn) {
-                if ("function" === typeof data) {
-                    fn = data;
-                    data = undefined;
-                }
-
-                if ("function" === typeof options) {
-                    fn = options;
-                    options = null;
-                }
-
-                if ("closing" === this.readyState || "closed" === this.readyState) {
-                    return;
-                }
-
-                options = options || {};
-                options.compress = false !== options.compress;
-                var packet = {
-                    type: type,
-                    data: data,
-                    options: options,
-                };
-                this.emitReserved("packetCreate", packet);
-                this.writeBuffer.push(packet);
-                if (fn) this.once("flush", fn);
-                this.flush();
-            },
-            /**
-             * Closes the connection.
-             *
-             * @api public
-             */
-        }, {
-            key: "close",
-            value: function close() {
-                var _this6 = this;
-
-                var close = function close() {
-                    _this6.onClose("forced close");
-
-                    _this6.transport.close();
-                };
-
-                var cleanupAndClose = function cleanupAndClose() {
-                    _this6.off("upgrade", cleanupAndClose);
-
-                    _this6.off("upgradeError", cleanupAndClose);
-
-                    close();
-                };
-
-                var waitForUpgrade = function waitForUpgrade() {
-                    // wait for upgrade to finish since we can't send packets while pausing a transport
-                    _this6.once("upgrade", cleanupAndClose);
-
-                    _this6.once("upgradeError", cleanupAndClose);
-                };
-
-                if ("opening" === this.readyState || "open" === this.readyState) {
-                    this.readyState = "closing";
-
-                    if (this.writeBuffer.length) {
-                        this.once("drain", function() {
-                            if (_this6.upgrading) {
-                                waitForUpgrade();
-                            } else {
-                                close();
-                            }
-                        });
-                    } else if (this.upgrading) {
-                        waitForUpgrade();
-                    } else {
-                        close();
-                    }
-                }
-
-                return this;
-            },
-            /**
-             * Called upon transport error
-             *
-             * @api private
-             */
-        }, {
-            key: "onError",
-            value: function onError(err) {
-                Socket.priorWebsocketSuccess = false;
-                this.emitReserved("error", err);
-                this.onClose("transport error", err);
-            },
-            /**
-             * Called upon transport close.
-             *
-             * @api private
-             */
-        }, {
-            key: "onClose",
-            value: function onClose(reason, desc) {
-                if (
-                    "opening" === this.readyState ||
-                    "open" === this.readyState ||
-                    "closing" === this.readyState
-                ) {
-                    // clear timers
-                    this.clearTimeoutFn(this.pingTimeoutTimer); // stop event from firing again for transport
-
-                    this.transport.removeAllListeners("close"); // ensure transport won't stay open
-
-                    this.transport.close(); // ignore further transport communication
-
-                    this.transport.removeAllListeners();
-
-                    if (typeof removeEventListener === "function") {
-                        removeEventListener("offline", this.offlineEventListener, false);
-                    } // set ready state
-
-                    this.readyState = "closed"; // clear session id
-
-                    this.id = null; // emit close event
-
-                    this.emitReserved("close", reason, desc); // clean buffers after, so users can still
-                    // grab the buffers on `close` event
-
-                    this.writeBuffer = [];
-                    this.prevBufferLen = 0;
-                }
-            },
-            /**
-             * Filters upgrades, returning only those matching client transports.
-             *
-             * @param {Array} server upgrades
-             * @api private
-             *
-             */
-        }, {
-            key: "filterUpgrades",
-            value: function filterUpgrades(upgrades) {
-                var filteredUpgrades = [];
-                var i = 0;
-                var j = upgrades.length;
-
-                for (; i < j; i++) {
-                    if (~this.transports.indexOf(upgrades[i]))
-                        filteredUpgrades.push(upgrades[i]);
-                }
-
-                return filteredUpgrades;
-            },
-        }, ]);
-
-        return Socket;
-    })(Emitter_1);
-    Socket$1.protocol = protocol$1;
-
-    function clone(obj) {
-        var o = {};
-
-        for (var i in obj) {
-            if (obj.hasOwnProperty(i)) {
-                o[i] = obj[i];
-            }
-        }
-
-        return o;
-    }
-
-    var withNativeArrayBuffer = typeof ArrayBuffer === "function";
-
-    var isView = function isView(obj) {
-        return typeof ArrayBuffer.isView === "function" ?
-            ArrayBuffer.isView(obj) :
-            obj.buffer instanceof ArrayBuffer;
-    };
-
-    var toString = Object.prototype.toString;
-    var withNativeBlob =
-        typeof Blob === "function" ||
-        (typeof Blob !== "undefined" &&
-            toString.call(Blob) === "[object BlobConstructor]");
-    var withNativeFile =
-        typeof File === "function" ||
-        (typeof File !== "undefined" &&
-            toString.call(File) === "[object FileConstructor]");
-    /**
-     * Returns true if obj is a Buffer, an ArrayBuffer, a Blob or a File.
-     *
-     * @private
-     */
-
-    function isBinary(obj) {
-        return (
-            (withNativeArrayBuffer && (obj instanceof ArrayBuffer || isView(obj))) ||
-            (withNativeBlob && obj instanceof Blob) ||
-            (withNativeFile && obj instanceof File)
-        );
-    }
-
-    function hasBinary(obj, toJSON) {
-        if (!obj || _typeof(obj) !== "object") {
-            return false;
-        }
-
-        if (Array.isArray(obj)) {
-            for (var i = 0, l = obj.length; i < l; i++) {
-                if (hasBinary(obj[i])) {
-                    return true;
-                }
-            }
-
-            return false;
-        }
-
-        if (isBinary(obj)) {
-            return true;
-        }
-
-        if (
-            obj.toJSON &&
-            typeof obj.toJSON === "function" &&
-            arguments.length === 1
-        ) {
-            return hasBinary(obj.toJSON(), true);
-        }
-
-        for (var key in obj) {
-            if (
-                Object.prototype.hasOwnProperty.call(obj, key) &&
-                hasBinary(obj[key])
-            ) {
-                return true;
-            }
-        }
-
-        return false;
-    }
-
-    /**
-     * Replaces every Buffer | ArrayBuffer | Blob | File in packet with a numbered placeholder.
-     *
-     * @param {Object} packet - socket.io event packet
-     * @return {Object} with deconstructed packet and list of buffers
-     * @public
-     */
-
-    function deconstructPacket(packet) {
-        var buffers = [];
-        var packetData = packet.data;
-        var pack = packet;
-        pack.data = _deconstructPacket(packetData, buffers);
-        pack.attachments = buffers.length; // number of binary 'attachments'
-
-        return {
-            packet: pack,
-            buffers: buffers,
-        };
-    }
-
-    function _deconstructPacket(data, buffers) {
-        if (!data) return data;
-
-        if (isBinary(data)) {
-            var placeholder = {
-                _placeholder: true,
-                num: buffers.length,
-            };
-            buffers.push(data);
-            return placeholder;
-        } else if (Array.isArray(data)) {
-            var newData = new Array(data.length);
-
-            for (var i = 0; i < data.length; i++) {
-                newData[i] = _deconstructPacket(data[i], buffers);
-            }
-
-            return newData;
-        } else if (_typeof(data) === "object" && !(data instanceof Date)) {
-            var _newData = {};
-
-            for (var key in data) {
-                if (data.hasOwnProperty(key)) {
-                    _newData[key] = _deconstructPacket(data[key], buffers);
-                }
-            }
-
-            return _newData;
-        }
-
-        return data;
-    }
-    /**
-     * Reconstructs a binary packet from its placeholder packet and buffers
-     *
-     * @param {Object} packet - event packet with placeholders
-     * @param {Array} buffers - binary buffers to put in placeholder positions
-     * @return {Object} reconstructed packet
-     * @public
-     */
-
-    function reconstructPacket(packet, buffers) {
-        packet.data = _reconstructPacket(packet.data, buffers);
-        packet.attachments = undefined; // no longer useful
-
-        return packet;
-    }
-
-    function _reconstructPacket(data, buffers) {
-        if (!data) return data;
-
-        if (data && data._placeholder) {
-            return buffers[data.num]; // appropriate buffer (should be natural order anyway)
-        } else if (Array.isArray(data)) {
-            for (var i = 0; i < data.length; i++) {
-                data[i] = _reconstructPacket(data[i], buffers);
-            }
-        } else if (_typeof(data) === "object") {
-            for (var key in data) {
-                if (data.hasOwnProperty(key)) {
-                    data[key] = _reconstructPacket(data[key], buffers);
-                }
-            }
-        }
-
-        return data;
-    }
-
-    /**
-     * Protocol version.
-     *
-     * @public
-     */
-
-    var protocol = 5;
-    var PacketType;
-
-    (function(PacketType) {
-        PacketType[(PacketType["CONNECT"] = 0)] = "CONNECT";
-        PacketType[(PacketType["DISCONNECT"] = 1)] = "DISCONNECT";
-        PacketType[(PacketType["EVENT"] = 2)] = "EVENT";
-        PacketType[(PacketType["ACK"] = 3)] = "ACK";
-        PacketType[(PacketType["CONNECT_ERROR"] = 4)] = "CONNECT_ERROR";
-        PacketType[(PacketType["BINARY_EVENT"] = 5)] = "BINARY_EVENT";
-        PacketType[(PacketType["BINARY_ACK"] = 6)] = "BINARY_ACK";
-    })(PacketType || (PacketType = {}));
-    /**
-     * A socket.io Encoder instance
-     */
-
-    var Encoder = /*#__PURE__*/ (function() {
-        function Encoder() {
-            _classCallCheck(this, Encoder);
-        }
-
-        _createClass(Encoder, [{
-            key: "encode",
-            value:
-                /**
-                 * Encode a packet as a single string if non-binary, or as a
-                 * buffer sequence, depending on packet type.
-                 *
-                 * @param {Object} obj - packet object
-                 */
-                function encode(obj) {
-                    if (obj.type === PacketType.EVENT || obj.type === PacketType.ACK) {
-                        if (hasBinary(obj)) {
-                            obj.type =
-                                obj.type === PacketType.EVENT ?
-                                PacketType.BINARY_EVENT :
-                                PacketType.BINARY_ACK;
-                            return this.encodeAsBinary(obj);
-                        }
-                    }
-
-                    return [this.encodeAsString(obj)];
-                },
-            /**
-             * Encode packet as string.
-             */
-        }, {
-            key: "encodeAsString",
-            value: function encodeAsString(obj) {
-                // first is type
-                var str = "" + obj.type; // attachments if we have them
-
-                if (
-                    obj.type === PacketType.BINARY_EVENT ||
-                    obj.type === PacketType.BINARY_ACK
-                ) {
-                    str += obj.attachments + "-";
-                } // if we have a namespace other than `/`
-                // we append it followed by a comma `,`
-
-                if (obj.nsp && "/" !== obj.nsp) {
-                    str += obj.nsp + ",";
-                } // immediately followed by the id
-
-                if (null != obj.id) {
-                    str += obj.id;
-                } // json data
-
-                if (null != obj.data) {
-                    str += JSON.stringify(obj.data);
-                }
-
-                return str;
-            },
-            /**
-             * Encode packet as 'buffer sequence' by removing blobs, and
-             * deconstructing packet into object with placeholders and
-             * a list of buffers.
-             */
-        }, {
-            key: "encodeAsBinary",
-            value: function encodeAsBinary(obj) {
-                var deconstruction = deconstructPacket(obj);
-                var pack = this.encodeAsString(deconstruction.packet);
-                var buffers = deconstruction.buffers;
-                buffers.unshift(pack); // add packet info to beginning of data list
-
-                return buffers; // write all the buffers
-            },
-        }, ]);
-
-        return Encoder;
-    })();
-    /**
-     * A socket.io Decoder instance
-     *
-     * @return {Object} decoder
-     */
-
-    var Decoder = /*#__PURE__*/ (function(_Emitter) {
-        _inherits(Decoder, _Emitter);
-
-        var _super = _createSuper(Decoder);
-
-        function Decoder() {
-            _classCallCheck(this, Decoder);
-
-            return _super.call(this);
-        }
-        /**
-         * Decodes an encoded packet string into packet JSON.
-         *
-         * @param {String} obj - encoded packet
-         */
-
-        _createClass(
-            Decoder,
-            [{
-                key: "add",
-                value: function add(obj) {
-                    var packet;
-
-                    if (typeof obj === "string") {
-                        packet = this.decodeString(obj);
-
-                        if (
-                            packet.type === PacketType.BINARY_EVENT ||
-                            packet.type === PacketType.BINARY_ACK
-                        ) {
-                            // binary packet's json
-                            this.reconstructor = new BinaryReconstructor(packet); // no attachments, labeled binary but no binary data to follow
-
-                            if (packet.attachments === 0) {
-                                _get(
-                                    _getPrototypeOf(Decoder.prototype),
-                                    "emitReserved",
-                                    this
-                                ).call(this, "decoded", packet);
-                            }
-                        } else {
-                            // non-binary full packet
-                            _get(
-                                _getPrototypeOf(Decoder.prototype),
-                                "emitReserved",
-                                this
-                            ).call(this, "decoded", packet);
-                        }
-                    } else if (isBinary(obj) || obj.base64) {
-                        // raw binary data
-                        if (!this.reconstructor) {
-                            throw new Error(
-                                "got binary data when not reconstructing a packet"
-                            );
-                        } else {
-                            packet = this.reconstructor.takeBinaryData(obj);
-
-                            if (packet) {
-                                // received final buffer
-                                this.reconstructor = null;
-
-                                _get(
-                                    _getPrototypeOf(Decoder.prototype),
-                                    "emitReserved",
-                                    this
-                                ).call(this, "decoded", packet);
-                            }
-                        }
-                    } else {
-                        throw new Error("Unknown type: " + obj);
-                    }
-                },
-                /**
-                 * Decode a packet String (JSON data)
-                 *
-                 * @param {String} str
-                 * @return {Object} packet
-                 */
-            }, {
-                key: "decodeString",
-                value: function decodeString(str) {
-                    var i = 0; // look up type
-
-                    var p = {
-                        type: Number(str.charAt(0)),
-                    };
-
-                    if (PacketType[p.type] === undefined) {
-                        throw new Error("unknown packet type " + p.type);
-                    } // look up attachments if type binary
-
-                    if (
-                        p.type === PacketType.BINARY_EVENT ||
-                        p.type === PacketType.BINARY_ACK
-                    ) {
-                        var start = i + 1;
-
-                        while (str.charAt(++i) !== "-" && i != str.length) {}
-
-                        var buf = str.substring(start, i);
-
-                        if (buf != Number(buf) || str.charAt(i) !== "-") {
-                            throw new Error("Illegal attachments");
-                        }
-
-                        p.attachments = Number(buf);
-                    } // look up namespace (if any)
-
-                    if ("/" === str.charAt(i + 1)) {
-                        var _start = i + 1;
-
-                        while (++i) {
-                            var c = str.charAt(i);
-                            if ("," === c) break;
-                            if (i === str.length) break;
-                        }
-
-                        p.nsp = str.substring(_start, i);
-                    } else {
-                        p.nsp = "/";
-                    } // look up id
-
-                    var next = str.charAt(i + 1);
-
-                    if ("" !== next && Number(next) == next) {
-                        var _start2 = i + 1;
-
-                        while (++i) {
-                            var _c = str.charAt(i);
-
-                            if (null == _c || Number(_c) != _c) {
-                                --i;
-                                break;
-                            }
-
-                            if (i === str.length) break;
-                        }
-
-                        p.id = Number(str.substring(_start2, i + 1));
-                    } // look up json data
-
-                    if (str.charAt(++i)) {
-                        var payload = tryParse(str.substr(i));
-
-                        if (Decoder.isPayloadValid(p.type, payload)) {
-                            p.data = payload;
-                        } else {
-                            throw new Error("invalid payload");
-                        }
-                    }
-
-                    return p;
-                },
-            }, {
-                key: "destroy",
-                value:
-                    /**
-                     * Deallocates a parser's resources
-                     */
-                    function destroy() {
-                        if (this.reconstructor) {
-                            this.reconstructor.finishedReconstruction();
-                        }
-                    },
-            }, ],
-            [{
-                key: "isPayloadValid",
-                value: function isPayloadValid(type, payload) {
-                    switch (type) {
-                        case PacketType.CONNECT:
-                            return _typeof(payload) === "object";
-
-                        case PacketType.DISCONNECT:
-                            return payload === undefined;
-
-                        case PacketType.CONNECT_ERROR:
-                            return (
-                                typeof payload === "string" || _typeof(payload) === "object"
-                            );
-
-                        case PacketType.EVENT:
-                        case PacketType.BINARY_EVENT:
-                            return Array.isArray(payload) && payload.length > 0;
-
-                        case PacketType.ACK:
-                        case PacketType.BINARY_ACK:
-                            return Array.isArray(payload);
-                    }
-                },
-            }, ]
-        );
-
-        return Decoder;
-    })(Emitter_1);
-
-    function tryParse(str) {
-        try {
-            return JSON.parse(str);
-        } catch (e) {
-            return false;
-        }
-    }
-    /**
-     * A manager of a binary event's 'buffer sequence'. Should
-     * be constructed whenever a packet of type BINARY_EVENT is
-     * decoded.
-     *
-     * @param {Object} packet
-     * @return {BinaryReconstructor} initialized reconstructor
-     */
-
-    var BinaryReconstructor = /*#__PURE__*/ (function() {
-        function BinaryReconstructor(packet) {
-            _classCallCheck(this, BinaryReconstructor);
-
-            this.packet = packet;
-            this.buffers = [];
-            this.reconPack = packet;
-        }
-        /**
-         * Method to be called when binary data received from connection
-         * after a BINARY_EVENT packet.
-         *
-         * @param {Buffer | ArrayBuffer} binData - the raw binary data received
-         * @return {null | Object} returns null if more binary data is expected or
-         *   a reconstructed packet object if all buffers have been received.
-         */
-
-        _createClass(BinaryReconstructor, [{
-            key: "takeBinaryData",
-            value: function takeBinaryData(binData) {
-                this.buffers.push(binData);
-
-                if (this.buffers.length === this.reconPack.attachments) {
-                    // done with buffer list
-                    var packet = reconstructPacket(this.reconPack, this.buffers);
-                    this.finishedReconstruction();
-                    return packet;
-                }
-
-                return null;
-            },
-            /**
-             * Cleans up binary packet reconstruction variables.
-             */
-        }, {
-            key: "finishedReconstruction",
-            value: function finishedReconstruction() {
-                this.reconPack = null;
-                this.buffers = [];
-            },
-        }, ]);
-
-        return BinaryReconstructor;
-    })();
-
-    var parser = /*#__PURE__*/ Object.freeze({
-        __proto__: null,
-        protocol: protocol,
-        get PacketType() {
-            return PacketType;
-        },
-        Encoder: Encoder,
-        Decoder: Decoder,
-    });
-
-    function on(obj, ev, fn) {
-        obj.on(ev, fn);
-        return function subDestroy() {
-            obj.off(ev, fn);
-        };
-    }
-
-    /**
-     * Internal events.
-     * These events can't be emitted by the user.
-     */
-
-    var RESERVED_EVENTS = Object.freeze({
-        connect: 1,
-        connect_error: 1,
-        disconnect: 1,
-        disconnecting: 1,
-        // EventEmitter reserved events: https://nodejs.org/api/events.html#events_event_newlistener
-        newListener: 1,
-        removeListener: 1,
-    });
-    var Socket = /*#__PURE__*/ (function(_Emitter) {
-        _inherits(Socket, _Emitter);
-
-        var _super = _createSuper(Socket);
-
-        /**
-         * `Socket` constructor.
-         *
-         * @public
-         */
-        function Socket(io, nsp, opts) {
-            var _this;
-
-            _classCallCheck(this, Socket);
-
-            _this = _super.call(this);
-            _this.connected = false;
-            _this.disconnected = true;
-            _this.receiveBuffer = [];
-            _this.sendBuffer = [];
-            _this.ids = 0;
-            _this.acks = {};
-            _this.flags = {};
-            _this.io = io;
-            _this.nsp = nsp;
-
-            if (opts && opts.auth) {
-                _this.auth = opts.auth;
-            }
-
-            if (_this.io._autoConnect) _this.open();
-            return _this;
-        }
-        /**
-         * Subscribe to open, close and packet events
-         *
-         * @private
-         */
-
-        _createClass(Socket, [{
-            key: "subEvents",
-            value: function subEvents() {
-                if (this.subs) return;
-                var io = this.io;
-                this.subs = [
-                    on(io, "open", this.onopen.bind(this)),
-                    on(io, "packet", this.onpacket.bind(this)),
-                    on(io, "error", this.onerror.bind(this)),
-                    on(io, "close", this.onclose.bind(this)),
-                ];
-            },
-            /**
-             * Whether the Socket will try to reconnect when its Manager connects or reconnects
-             */
-        }, {
-            key: "active",
-            get: function get() {
-                return !!this.subs;
-            },
-            /**
-             * "Opens" the socket.
-             *
-             * @public
-             */
-        }, {
-            key: "connect",
-            value: function connect() {
-                if (this.connected) return this;
-                this.subEvents();
-                if (!this.io["_reconnecting"]) this.io.open(); // ensure open
-
-                if ("open" === this.io._readyState) this.onopen();
-                return this;
-            },
-            /**
-             * Alias for connect()
-             */
-        }, {
-            key: "open",
-            value: function open() {
-                return this.connect();
-            },
-            /**
-             * Sends a `message` event.
-             *
-             * @return self
-             * @public
-             */
-        }, {
-            key: "send",
-            value: function send() {
-                for (
-                    var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++
-                ) {
-                    args[_key] = arguments[_key];
-                }
-
-                args.unshift("message");
-                this.emit.apply(this, args);
-                return this;
-            },
-            /**
-             * Override `emit`.
-             * If the event is in `events`, it's emitted normally.
-             *
-             * @return self
-             * @public
-             */
-        }, {
-            key: "emit",
-            value: function emit(ev) {
-                if (RESERVED_EVENTS.hasOwnProperty(ev)) {
-                    throw new Error('"' + ev + '" is a reserved event name');
-                }
-
-                for (
-                    var _len2 = arguments.length,
-                        args = new Array(_len2 > 1 ? _len2 - 1 : 0),
-                        _key2 = 1; _key2 < _len2; _key2++
-                ) {
-                    args[_key2 - 1] = arguments[_key2];
-                }
-
-                args.unshift(ev);
-                var packet = {
-                    type: PacketType.EVENT,
-                    data: args,
-                };
-                packet.options = {};
-                packet.options.compress = this.flags.compress !== false; // event ack callback
-
-                if ("function" === typeof args[args.length - 1]) {
-                    var id = this.ids++;
-                    var ack = args.pop();
-
-                    this._registerAckCallback(id, ack);
-
-                    packet.id = id;
-                }
-
-                var isTransportWritable =
-                    this.io.engine &&
-                    this.io.engine.transport &&
-                    this.io.engine.transport.writable;
-                var discardPacket =
-                    this.flags["volatile"] && (!isTransportWritable || !this.connected);
-
-                if (discardPacket);
-                else if (this.connected) {
-                    this.packet(packet);
-                } else {
-                    this.sendBuffer.push(packet);
-                }
-
-                this.flags = {};
-                return this;
-            },
-            /**
-             * @private
-             */
-        }, {
-            key: "_registerAckCallback",
-            value: function _registerAckCallback(id, ack) {
-                var _this2 = this;
-
-                var timeout = this.flags.timeout;
-
-                if (timeout === undefined) {
-                    this.acks[id] = ack;
-                    return;
-                } // @ts-ignore
-
-                var timer = this.io.setTimeoutFn(function() {
-                    delete _this2.acks[id];
-
-                    for (var i = 0; i < _this2.sendBuffer.length; i++) {
-                        if (_this2.sendBuffer[i].id === id) {
-                            _this2.sendBuffer.splice(i, 1);
-                        }
-                    }
-
-                    ack.call(_this2, new Error("operation has timed out"));
-                }, timeout);
-
-                this.acks[id] = function() {
-                    // @ts-ignore
-                    _this2.io.clearTimeoutFn(timer);
-
-                    for (
-                        var _len3 = arguments.length, args = new Array(_len3), _key3 = 0; _key3 < _len3; _key3++
-                    ) {
-                        args[_key3] = arguments[_key3];
-                    }
-
-                    ack.apply(_this2, [null].concat(args));
-                };
-            },
-            /**
-             * Sends a packet.
-             *
-             * @param packet
-             * @private
-             */
-        }, {
-            key: "packet",
-            value: function packet(_packet) {
-                _packet.nsp = this.nsp;
-
-                this.io._packet(_packet);
-            },
-            /**
-             * Called upon engine `open`.
-             *
-             * @private
-             */
-        }, {
-            key: "onopen",
-            value: function onopen() {
-                var _this3 = this;
-
-                if (typeof this.auth == "function") {
-                    this.auth(function(data) {
-                        _this3.packet({
-                            type: PacketType.CONNECT,
-                            data: data,
-                        });
-                    });
-                } else {
-                    this.packet({
-                        type: PacketType.CONNECT,
-                        data: this.auth,
-                    });
-                }
-            },
-            /**
-             * Called upon engine or manager `error`.
-             *
-             * @param err
-             * @private
-             */
-        }, {
-            key: "onerror",
-            value: function onerror(err) {
-                if (!this.connected) {
-                    this.emitReserved("connect_error", err);
-                }
-            },
-            /**
-             * Called upon engine `close`.
-             *
-             * @param reason
-             * @private
-             */
-        }, {
-            key: "onclose",
-            value: function onclose(reason) {
-                this.connected = false;
-                this.disconnected = true;
-                delete this.id;
-                this.emitReserved("disconnect", reason);
-            },
-            /**
-             * Called with socket packet.
-             *
-             * @param packet
-             * @private
-             */
-        }, {
-            key: "onpacket",
-            value: function onpacket(packet) {
-                var sameNamespace = packet.nsp === this.nsp;
-                if (!sameNamespace) return;
-
-                switch (packet.type) {
-                    case PacketType.CONNECT:
-                        if (packet.data && packet.data.sid) {
-                            var id = packet.data.sid;
-                            this.onconnect(id);
-                        } else {
-                            this.emitReserved(
-                                "connect_error",
-                                new Error(
-                                    "It seems you are trying to reach a Socket.IO server in v2.x with a v3.x client, but they are not compatible (more information here: https://socket.io/docs/v3/migrating-from-2-x-to-3-0/)"
-                                )
-                            );
-                        }
-
-                        break;
-
-                    case PacketType.EVENT:
-                        this.onevent(packet);
-                        break;
-
-                    case PacketType.BINARY_EVENT:
-                        this.onevent(packet);
-                        break;
-
-                    case PacketType.ACK:
-                        this.onack(packet);
-                        break;
-
-                    case PacketType.BINARY_ACK:
-                        this.onack(packet);
-                        break;
-
-                    case PacketType.DISCONNECT:
-                        this.ondisconnect();
-                        break;
-
-                    case PacketType.CONNECT_ERROR:
-                        this.destroy();
-                        var err = new Error(packet.data.message); // @ts-ignore
-
-                        err.data = packet.data.data;
-                        this.emitReserved("connect_error", err);
-                        break;
-                }
-            },
-            /**
-             * Called upon a server event.
-             *
-             * @param packet
-             * @private
-             */
-        }, {
-            key: "onevent",
-            value: function onevent(packet) {
-                var args = packet.data || [];
-
-                if (null != packet.id) {
-                    args.push(this.ack(packet.id));
-                }
-
-                if (this.connected) {
-                    this.emitEvent(args);
-                } else {
-                    this.receiveBuffer.push(Object.freeze(args));
-                }
-            },
-        }, {
-            key: "emitEvent",
-            value: function emitEvent(args) {
-                if (this._anyListeners && this._anyListeners.length) {
-                    var listeners = this._anyListeners.slice();
-
-                    var _iterator = _createForOfIteratorHelper(listeners),
-                        _step;
-
-                    try {
-                        for (_iterator.s(); !(_step = _iterator.n()).done;) {
-                            var listener = _step.value;
-                            listener.apply(this, args);
-                        }
-                    } catch (err) {
-                        _iterator.e(err);
-                    } finally {
-                        _iterator.f();
-                    }
-                }
-
-                _get(_getPrototypeOf(Socket.prototype), "emit", this).apply(
-                    this,
-                    args
-                );
-            },
-            /**
-             * Produces an ack callback to emit with an event.
-             *
-             * @private
-             */
-        }, {
-            key: "ack",
-            value: function ack(id) {
-                var self = this;
-                var sent = false;
-                return function() {
-                    // prevent double callbacks
-                    if (sent) return;
-                    sent = true;
-
-                    for (
-                        var _len4 = arguments.length, args = new Array(_len4), _key4 = 0; _key4 < _len4; _key4++
-                    ) {
-                        args[_key4] = arguments[_key4];
-                    }
-
-                    self.packet({
-                        type: PacketType.ACK,
-                        id: id,
-                        data: args,
-                    });
-                };
-            },
-            /**
-             * Called upon a server acknowlegement.
-             *
-             * @param packet
-             * @private
-             */
-        }, {
-            key: "onack",
-            value: function onack(packet) {
-                var ack = this.acks[packet.id];
-
-                if ("function" === typeof ack) {
-                    ack.apply(this, packet.data);
-                    delete this.acks[packet.id];
-                }
-            },
-            /**
-             * Called upon server connect.
-             *
-             * @private
-             */
-        }, {
-            key: "onconnect",
-            value: function onconnect(id) {
-                this.id = id;
-                this.connected = true;
-                this.disconnected = false;
-                this.emitBuffered();
-                this.emitReserved("connect");
-            },
-            /**
-             * Emit buffered events (received and emitted).
-             *
-             * @private
-             */
-        }, {
-            key: "emitBuffered",
-            value: function emitBuffered() {
-                var _this4 = this;
-
-                this.receiveBuffer.forEach(function(args) {
-                    return _this4.emitEvent(args);
-                });
-                this.receiveBuffer = [];
-                this.sendBuffer.forEach(function(packet) {
-                    return _this4.packet(packet);
-                });
-                this.sendBuffer = [];
-            },
-            /**
-             * Called upon server disconnect.
-             *
-             * @private
-             */
-        }, {
-            key: "ondisconnect",
-            value: function ondisconnect() {
-                this.destroy();
-                this.onclose("io server disconnect");
-            },
-            /**
-             * Called upon forced client/server side disconnections,
-             * this method ensures the manager stops tracking us and
-             * that reconnections don't get triggered for this.
-             *
-             * @private
-             */
-        }, {
-            key: "destroy",
-            value: function destroy() {
-                if (this.subs) {
-                    // clean subscriptions to avoid reconnections
-                    this.subs.forEach(function(subDestroy) {
-                        return subDestroy();
-                    });
-                    this.subs = undefined;
-                }
-
-                this.io["_destroy"](this);
-            },
-            /**
-             * Disconnects the socket manually.
-             *
-             * @return self
-             * @public
-             */
-        }, {
-            key: "disconnect",
-            value: function disconnect() {
-                if (this.connected) {
-                    this.packet({
-                        type: PacketType.DISCONNECT,
-                    });
-                } // remove socket from pool
-
-                this.destroy();
-
-                if (this.connected) {
-                    // fire events
-                    this.onclose("io client disconnect");
-                }
-
-                return this;
-            },
-            /**
-             * Alias for disconnect()
-             *
-             * @return self
-             * @public
-             */
-        }, {
-            key: "close",
-            value: function close() {
-                return this.disconnect();
-            },
-            /**
-             * Sets the compress flag.
-             *
-             * @param compress - if `true`, compresses the sending data
-             * @return self
-             * @public
-             */
-        }, {
-            key: "compress",
-            value: function compress(_compress) {
-                this.flags.compress = _compress;
-                return this;
-            },
-            /**
-             * Sets a modifier for a subsequent event emission that the event message will be dropped when this socket is not
-             * ready to send messages.
-             *
-             * @returns self
-             * @public
-             */
-        }, {
-            key: "volatile",
-            get: function get() {
-                this.flags["volatile"] = true;
-                return this;
-            },
-            /**
-             * Sets a modifier for a subsequent event emission that the callback will be called with an error when the
-             * given number of milliseconds have elapsed without an acknowledgement from the server:
-             *
-             * ```
-             * socket.timeout(5000).emit("my-event", (err) => {
-             *   if (err) {
-             *     // the server did not acknowledge the event in the given delay
-             *   }
-             * });
-             * ```
-             *
-             * @returns self
-             * @public
-             */
-        }, {
-            key: "timeout",
-            value: function timeout(_timeout) {
-                this.flags.timeout = _timeout;
-                return this;
-            },
-            /**
-             * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the
-             * callback.
-             *
-             * @param listener
-             * @public
-             */
-        }, {
-            key: "onAny",
-            value: function onAny(listener) {
-                this._anyListeners = this._anyListeners || [];
-
-                this._anyListeners.push(listener);
-
-                return this;
-            },
-            /**
-             * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the
-             * callback. The listener is added to the beginning of the listeners array.
-             *
-             * @param listener
-             * @public
-             */
-        }, {
-            key: "prependAny",
-            value: function prependAny(listener) {
-                this._anyListeners = this._anyListeners || [];
-
-                this._anyListeners.unshift(listener);
-
-                return this;
-            },
-            /**
-             * Removes the listener that will be fired when any event is emitted.
-             *
-             * @param listener
-             * @public
-             */
-        }, {
-            key: "offAny",
-            value: function offAny(listener) {
-                if (!this._anyListeners) {
-                    return this;
-                }
-
-                if (listener) {
-                    var listeners = this._anyListeners;
-
-                    for (var i = 0; i < listeners.length; i++) {
-                        if (listener === listeners[i]) {
-                            listeners.splice(i, 1);
-                            return this;
-                        }
-                    }
-                } else {
-                    this._anyListeners = [];
-                }
-
-                return this;
-            },
-            /**
-             * Returns an array of listeners that are listening for any event that is specified. This array can be manipulated,
-             * e.g. to remove listeners.
-             *
-             * @public
-             */
-        }, {
-            key: "listenersAny",
-            value: function listenersAny() {
-                return this._anyListeners || [];
-            },
-        }, ]);
-
-        return Socket;
-    })(Emitter_1);
-
-    /**
-     * Expose `Backoff`.
-     */
-
-    var backo2 = Backoff;
-    /**
-     * Initialize backoff timer with `opts`.
-     *
-     * - `min` initial timeout in milliseconds [100]
-     * - `max` max timeout [10000]
-     * - `jitter` [0]
-     * - `factor` [2]
-     *
-     * @param {Object} opts
-     * @api public
-     */
-
-    function Backoff(opts) {
-        opts = opts || {};
-        this.ms = opts.min || 100;
-        this.max = opts.max || 10000;
-        this.factor = opts.factor || 2;
-        this.jitter = opts.jitter > 0 && opts.jitter <= 1 ? opts.jitter : 0;
-        this.attempts = 0;
-    }
-    /**
-     * Return the backoff duration.
-     *
-     * @return {Number}
-     * @api public
-     */
-
-    Backoff.prototype.duration = function() {
-        var ms = this.ms * Math.pow(this.factor, this.attempts++);
-
-        if (this.jitter) {
-            var rand = Math.random();
-            var deviation = Math.floor(rand * this.jitter * ms);
-            ms = (Math.floor(rand * 10) & 1) == 0 ? ms - deviation : ms + deviation;
-        }
-
-        return Math.min(ms, this.max) | 0;
-    };
-    /**
-     * Reset the number of attempts.
-     *
-     * @api public
-     */
-
-    Backoff.prototype.reset = function() {
-        this.attempts = 0;
-    };
-    /**
-     * Set the minimum duration
-     *
-     * @api public
-     */
-
-    Backoff.prototype.setMin = function(min) {
-        this.ms = min;
-    };
-    /**
-     * Set the maximum duration
-     *
-     * @api public
-     */
-
-    Backoff.prototype.setMax = function(max) {
-        this.max = max;
-    };
-    /**
-     * Set the jitter
-     *
-     * @api public
-     */
-
-    Backoff.prototype.setJitter = function(jitter) {
-        this.jitter = jitter;
-    };
-
-    var Manager = /*#__PURE__*/ (function(_Emitter) {
-        _inherits(Manager, _Emitter);
-
-        var _super = _createSuper(Manager);
-
-        function Manager(uri, opts) {
-            var _this;
-
-            _classCallCheck(this, Manager);
-
-            var _a;
-
-            _this = _super.call(this);
-            _this.nsps = {};
-            _this.subs = [];
-
-            if (uri && "object" === _typeof(uri)) {
-                opts = uri;
-                uri = undefined;
-            }
-
-            opts = opts || {};
-            opts.path = opts.path || "/socket.io";
-            _this.opts = opts;
-            installTimerFunctions(_assertThisInitialized(_this), opts);
-
-            _this.reconnection(opts.reconnection !== false);
-
-            _this.reconnectionAttempts(opts.reconnectionAttempts || Infinity);
-
-            _this.reconnectionDelay(opts.reconnectionDelay || 1000);
-
-            _this.reconnectionDelayMax(opts.reconnectionDelayMax || 5000);
-
-            _this.randomizationFactor(
-                (_a = opts.randomizationFactor) !== null && _a !== void 0 ? _a : 0.5
-            );
-
-            _this.backoff = new backo2({
-                min: _this.reconnectionDelay(),
-                max: _this.reconnectionDelayMax(),
-                jitter: _this.randomizationFactor(),
-            });
-
-            _this.timeout(null == opts.timeout ? 20000 : opts.timeout);
-
-            _this._readyState = "closed";
-            _this.uri = uri;
-
-            var _parser = opts.parser || parser;
-
-            _this.encoder = new _parser.Encoder();
-            _this.decoder = new _parser.Decoder();
-            _this._autoConnect = opts.autoConnect !== false;
-            if (_this._autoConnect) _this.open();
-            return _this;
-        }
-
-        _createClass(Manager, [{
-            key: "reconnection",
-            value: function reconnection(v) {
-                if (!arguments.length) return this._reconnection;
-                this._reconnection = !!v;
-                return this;
-            },
-        }, {
-            key: "reconnectionAttempts",
-            value: function reconnectionAttempts(v) {
-                if (v === undefined) return this._reconnectionAttempts;
-                this._reconnectionAttempts = v;
-                return this;
-            },
-        }, {
-            key: "reconnectionDelay",
-            value: function reconnectionDelay(v) {
-                var _a;
-
-                if (v === undefined) return this._reconnectionDelay;
-                this._reconnectionDelay = v;
-                (_a = this.backoff) === null || _a === void 0 ? void 0 : _a.setMin(v);
-                return this;
-            },
-        }, {
-            key: "randomizationFactor",
-            value: function randomizationFactor(v) {
-                var _a;
-
-                if (v === undefined) return this._randomizationFactor;
-                this._randomizationFactor = v;
-                (_a = this.backoff) === null || _a === void 0 ?
-                    void 0 :
-                    _a.setJitter(v);
-                return this;
-            },
-        }, {
-            key: "reconnectionDelayMax",
-            value: function reconnectionDelayMax(v) {
-                var _a;
-
-                if (v === undefined) return this._reconnectionDelayMax;
-                this._reconnectionDelayMax = v;
-                (_a = this.backoff) === null || _a === void 0 ? void 0 : _a.setMax(v);
-                return this;
-            },
-        }, {
-            key: "timeout",
-            value: function timeout(v) {
-                if (!arguments.length) return this._timeout;
-                this._timeout = v;
-                return this;
-            },
-            /**
-             * Starts trying to reconnect if reconnection is enabled and we have not
-             * started reconnecting yet
-             *
-             * @private
-             */
-        }, {
-            key: "maybeReconnectOnOpen",
-            value: function maybeReconnectOnOpen() {
-                // Only try to reconnect if it's the first time we're connecting
-                if (
-                    !this._reconnecting &&
-                    this._reconnection &&
-                    this.backoff.attempts === 0
-                ) {
-                    // keeps reconnection from firing twice for the same reconnection loop
-                    this.reconnect();
-                }
-            },
-            /**
-             * Sets the current transport `socket`.
-             *
-             * @param {Function} fn - optional, callback
-             * @return self
-             * @public
-             */
-        }, {
-            key: "open",
-            value: function open(fn) {
-                var _this2 = this;
-
-                if (~this._readyState.indexOf("open")) return this;
-                this.engine = new Socket$1(this.uri, this.opts);
-                var socket = this.engine;
-                var self = this;
-                this._readyState = "opening";
-                this.skipReconnect = false; // emit `open`
-
-                var openSubDestroy = on(socket, "open", function() {
-                    self.onopen();
-                    fn && fn();
-                }); // emit `error`
-
-                var errorSub = on(socket, "error", function(err) {
-                    self.cleanup();
-                    self._readyState = "closed";
-
-                    _this2.emitReserved("error", err);
-
-                    if (fn) {
-                        fn(err);
-                    } else {
-                        // Only do this if there is no fn to handle the error
-                        self.maybeReconnectOnOpen();
-                    }
-                });
-
-                if (false !== this._timeout) {
-                    var timeout = this._timeout;
-
-                    if (timeout === 0) {
-                        openSubDestroy(); // prevents a race condition with the 'open' event
-                    } // set timer
-
-                    var timer = this.setTimeoutFn(function() {
-                        openSubDestroy();
-                        socket.close(); // @ts-ignore
-
-                        socket.emit("error", new Error("timeout"));
-                    }, timeout);
-
-                    if (this.opts.autoUnref) {
-                        timer.unref();
-                    }
-
-                    this.subs.push(function subDestroy() {
-                        clearTimeout(timer);
-                    });
-                }
-
-                this.subs.push(openSubDestroy);
-                this.subs.push(errorSub);
-                return this;
-            },
-            /**
-             * Alias for open()
-             *
-             * @return self
-             * @public
-             */
-        }, {
-            key: "connect",
-            value: function connect(fn) {
-                return this.open(fn);
-            },
-            /**
-             * Called upon transport open.
-             *
-             * @private
-             */
-        }, {
-            key: "onopen",
-            value: function onopen() {
-                // clear old subs
-                this.cleanup(); // mark as open
-
-                this._readyState = "open";
-                this.emitReserved("open"); // add new subs
-
-                var socket = this.engine;
-                this.subs.push(
-                    on(socket, "ping", this.onping.bind(this)),
-                    on(socket, "data", this.ondata.bind(this)),
-                    on(socket, "error", this.onerror.bind(this)),
-                    on(socket, "close", this.onclose.bind(this)),
-                    on(this.decoder, "decoded", this.ondecoded.bind(this))
-                );
-            },
-            /**
-         * Called upon a ping.  var io;
-
-    if (newConnection) {
-      io = new Manager(source, opts);
-    } else {
-      if (!cache[id]) {
-        cache[id] = new Manager(source, opts);
-      }
-
-      io = cache[id];
-    }
-
-    if (parsed.query && !opts.query) {
-      opts.query = parsed.queryKey;
-    }
-
-    return io.socket(parsed.path, opts);
-  } // so that "lookup" can be used both as a function (e.g. `io(...)`) and as a
-  // namespace (e.g. `io.connect(...)`), for backward compatibility
-
-  _extends(lookup, {
-    Manager: Manager,
-    Socket: Socket,
-    io: lookup,
-    connect: lookup,
-  });
-
-  return lookup;
-});
-//# sourceMappingURL=socket.io.js.map
-
-         * @private
-         */
-        }, {
-            key: "onping",
-            value: function onping() {
-                this.emitReserved("ping");
-            },
-            /**
-             * Called with data.
-             *
-             * @private
-             */
-        }, {
-            key: "ondata",
-            value: function ondata(data) {
-                this.decoder.add(data);
-            },
-            /**
-             * Called when parser fully decodes a packet.
-             *
-             * @private
-             */
-        }, {
-            key: "ondecoded",
-            value: function ondecoded(packet) {
-                this.emitReserved("packet", packet);
-            },
-            /**
-             * Called upon socket error.
-             *
-             * @private
-             */
-        }, {
-            key: "onerror",
-            value: function onerror(err) {
-                this.emitReserved("error", err);
-            },
-            /**
-             * Creates a new socket for the given `nsp`.
-             *
-             * @return {Socket}
-             * @public
-             */
-        }, {
-            key: "socket",
-            value: function socket(nsp, opts) {
-                var socket = this.nsps[nsp];
-
-                if (!socket) {
-                    socket = new Socket(this, nsp, opts);
-                    this.nsps[nsp] = socket;
-                }
-
-                return socket;
-            },
-            /**
-             * Called upon a socket close.
-             *
-             * @param socket
-             * @private
-             */
-        }, {
-            key: "_destroy",
-            value: function _destroy(socket) {
-                var nsps = Object.keys(this.nsps);
-
-                for (var _i = 0, _nsps = nsps; _i < _nsps.length; _i++) {
-                    var nsp = _nsps[_i];
-                    var _socket = this.nsps[nsp];
-
-                    if (_socket.active) {
-                        return;
-                    }
-                }
-
-                this._close();
-            },
-            /**
-             * Writes a packet.
-             *
-             * @param packet
-             * @private
-             */
-        }, {
-            key: "_packet",
-            value: function _packet(packet) {
-                var encodedPackets = this.encoder.encode(packet);
-
-                for (var i = 0; i < encodedPackets.length; i++) {
-                    this.engine.write(encodedPackets[i], packet.options);
-                }
-            },
-            /**
-             * Clean up transport subscriptions and packet buffer.
-             *
-             * @private
-             */
-        }, {
-            key: "cleanup",
-            value: function cleanup() {
-                this.subs.forEach(function(subDestroy) {
-                    return subDestroy();
-                });
-                this.subs.length = 0;
-                this.decoder.destroy();
-            },
-            /**
-             * Close the current socket.
-             *
-             * @private
-             */
-        }, {
-            key: "_close",
-            value: function _close() {
-                this.skipReconnect = true;
-                this._reconnecting = false;
-                this.onclose("forced close");
-                if (this.engine) this.engine.close();
-            },
-            /**
-             * Alias for close()
-             *
-             * @private
-             */
-        }, {
-            key: "disconnect",
-            value: function disconnect() {
-                return this._close();
-            },
-            /**
-             * Called upon engine close.
-             *
-             * @private
-             */
-        }, {
-            key: "onclose",
-            value: function onclose(reason) {
-                this.cleanup();
-                this.backoff.reset();
-                this._readyState = "closed";
-                this.emitReserved("close", reason);
-
-                if (this._reconnection && !this.skipReconnect) {
-                    this.reconnect();
-                }
-            },
-            /**
-             * Attempt a reconnection.
-             *
-             * @private
-             */
-        }, {
-            key: "reconnect",
-            value: function reconnect() {
-                var _this3 = this;
-
-                if (this._reconnecting || this.skipReconnect) return this;
-                var self = this;
-
-                if (this.backoff.attempts >= this._reconnectionAttempts) {
-                    this.backoff.reset();
-                    this.emitReserved("reconnect_failed");
-                    this._reconnecting = false;
-                } else {
-                    var delay = this.backoff.duration();
-                    this._reconnecting = true;
-                    var timer = this.setTimeoutFn(function() {
-                        if (self.skipReconnect) return;
-
-                        _this3.emitReserved("reconnect_attempt", self.backoff.attempts); // check again for the case socket closed in above events
-
-                        if (self.skipReconnect) return;
-                        self.open(function(err) {
-                            if (err) {
-                                self._reconnecting = false;
-                                self.reconnect();
-
-                                _this3.emitReserved("reconnect_error", err);
-                            } else {
-                                self.onreconnect();
-                            }
-                        });
-                    }, delay);
-
-                    if (this.opts.autoUnref) {
-                        timer.unref();
-                    }
-
-                    this.subs.push(function subDestroy() {
-                        clearTimeout(timer);
-                    });
-                }
-            },
-            /**
-             * Called upon successful reconnect.
-             *
-             * @private
-             */
-        }, {
-            key: "onreconnect",
-            value: function onreconnect() {
-                var attempt = this.backoff.attempts;
-                this._reconnecting = false;
-                this.backoff.reset();
-                this.emitReserved("reconnect", attempt);
-            },
-        }, ]);
-
-        return Manager;
-    })(Emitter_1);
-
-    /**
-     * Managers cache.
-     */
-
-    var cache = {};
-
-    function lookup(uri, opts) {
-        if (_typeof(uri) === "object") {
-            opts = uri;
-            uri = undefined;
-        }
-
-        opts = opts || {};
-        var parsed = url(uri, opts.path || "/socket.io");
-        var source = parsed.source;
-        var id = parsed.id;
-        var path = parsed.path;
-        var sameNamespace = cache[id] && path in cache[id]["nsps"];
-        var newConnection =
-            opts.forceNew ||
-            opts["force new connection"] ||
-            false === opts.multiplex ||
-            sameNamespace;
-        var io;
-
-        if (newConnection) {
-            io = new Manager(source, opts);
-        } else {
-            if (!cache[id]) {
-                cache[id] = new Manager(source, opts);
-            }
-
-            io = cache[id];
-        }
-
-        if (parsed.query && !opts.query) {
-            opts.query = parsed.queryKey;
-        }
-
-        return io.socket(parsed.path, opts);
-    } // so that "lookup" can be used both as a function (e.g. `io(...)`) and as a
-    // namespace (e.g. `io.connect(...)`), for backward compatibility
-
-    _extends(lookup, {
-        Manager: Manager,
-        Socket: Socket,
-        io: lookup,
-        connect: lookup,
-    });
-
-    return lookup;
-});
+/*!
+ * Socket.IO v4.4.1
+ * (c) 2014-2022 Guillermo Rauch
+ * Released under the MIT License.
+ */
+(function(global, factory) {
+    typeof exports === "object" && typeof module !== "undefined" ?
+        (module.exports = factory()) :
+        typeof define === "function" && define.amd ?
+        define(factory) :
+        ((global =
+                typeof globalThis !== "undefined" ? globalThis : global || self),
+            (global.io = factory()));
+})(this, function() {
+    "use strict";
+
+    function _typeof(obj) {
+        "@babel/helpers - typeof";
+
+        if (typeof Symbol === "function" && typeof Symbol.iterator === "symbol") {
+            _typeof = function(obj) {
+                return typeof obj;
+            };
+        } else {
+            _typeof = function(obj) {
+                return obj &&
+                    typeof Symbol === "function" &&
+                    obj.constructor === Symbol &&
+                    obj !== Symbol.prototype ?
+                    "symbol" :
+                    typeof obj;
+            };
+        }
+
+        return _typeof(obj);
+    }
+
+    function _classCallCheck(instance, Constructor) {
+        if (!(instance instanceof Constructor)) {
+            throw new TypeError("Cannot call a class as a function");
+        }
+    }
+
+    function _defineProperties(target, props) {
+        for (var i = 0; i < props.length; i++) {
+            var descriptor = props[i];
+            descriptor.enumerable = descriptor.enumerable || false;
+            descriptor.configurable = true;
+            if ("value" in descriptor) descriptor.writable = true;
+            Object.defineProperty(target, descriptor.key, descriptor);
+        }
+    }
+
+    function _createClass(Constructor, protoProps, staticProps) {
+        if (protoProps) _defineProperties(Constructor.prototype, protoProps);
+        if (staticProps) _defineProperties(Constructor, staticProps);
+        return Constructor;
+    }
+
+    function _extends() {
+        _extends =
+            Object.assign ||
+            function(target) {
+                for (var i = 1; i < arguments.length; i++) {
+                    var source = arguments[i];
+
+                    for (var key in source) {
+                        if (Object.prototype.hasOwnProperty.call(source, key)) {
+                            target[key] = source[key];
+                        }
+                    }
+                }
+
+                return target;
+            };
+
+        return _extends.apply(this, arguments);
+    }
+
+    function _inherits(subClass, superClass) {
+        if (typeof superClass !== "function" && superClass !== null) {
+            throw new TypeError("Super expression must either be null or a function");
+        }
+
+        subClass.prototype = Object.create(superClass && superClass.prototype, {
+            constructor: {
+                value: subClass,
+                writable: true,
+                configurable: true,
+            },
+        });
+        if (superClass) _setPrototypeOf(subClass, superClass);
+    }
+
+    function _getPrototypeOf(o) {
+        _getPrototypeOf = Object.setPrototypeOf ?
+            Object.getPrototypeOf :
+            function _getPrototypeOf(o) {
+                return o.__proto__ || Object.getPrototypeOf(o);
+            };
+        return _getPrototypeOf(o);
+    }
+
+    function _setPrototypeOf(o, p) {
+        _setPrototypeOf =
+            Object.setPrototypeOf ||
+            function _setPrototypeOf(o, p) {
+                o.__proto__ = p;
+                return o;
+            };
+
+        return _setPrototypeOf(o, p);
+    }
+
+    function _isNativeReflectConstruct() {
+        if (typeof Reflect === "undefined" || !Reflect.construct) return false;
+        if (Reflect.construct.sham) return false;
+        if (typeof Proxy === "function") return true;
+
+        try {
+            Boolean.prototype.valueOf.call(
+                Reflect.construct(Boolean, [], function() {})
+            );
+            return true;
+        } catch (e) {
+            return false;
+        }
+    }
+
+    function _assertThisInitialized(self) {
+        if (self === void 0) {
+            throw new ReferenceError(
+                "this hasn't been initialised - super() hasn't been called"
+            );
+        }
+
+        return self;
+    }
+
+    function _possibleConstructorReturn(self, call) {
+        if (call && (typeof call === "object" || typeof call === "function")) {
+            return call;
+        } else if (call !== void 0) {
+            throw new TypeError(
+                "Derived constructors may only return object or undefined"
+            );
+        }
+
+        return _assertThisInitialized(self);
+    }
+
+    function _createSuper(Derived) {
+        var hasNativeReflectConstruct = _isNativeReflectConstruct();
+
+        return function _createSuperInternal() {
+            var Super = _getPrototypeOf(Derived),
+                result;
+
+            if (hasNativeReflectConstruct) {
+                var NewTarget = _getPrototypeOf(this).constructor;
+
+                result = Reflect.construct(Super, arguments, NewTarget);
+            } else {
+                result = Super.apply(this, arguments);
+            }
+
+            return _possibleConstructorReturn(this, result);
+        };
+    }
+
+    function _superPropBase(object, property) {
+        while (!Object.prototype.hasOwnProperty.call(object, property)) {
+            object = _getPrototypeOf(object);
+            if (object === null) break;
+        }
+
+        return object;
+    }
+
+    function _get(target, property, receiver) {
+        if (typeof Reflect !== "undefined" && Reflect.get) {
+            _get = Reflect.get;
+        } else {
+            _get = function _get(target, property, receiver) {
+                var base = _superPropBase(target, property);
+
+                if (!base) return;
+                var desc = Object.getOwnPropertyDescriptor(base, property);
+
+                if (desc.get) {
+                    return desc.get.call(receiver);
+                }
+
+                return desc.value;
+            };
+        }
+
+        return _get(target, property, receiver || target);
+    }
+
+    function _unsupportedIterableToArray(o, minLen) {
+        if (!o) return;
+        if (typeof o === "string") return _arrayLikeToArray(o, minLen);
+        var n = Object.prototype.toString.call(o).slice(8, -1);
+        if (n === "Object" && o.constructor) n = o.constructor.name;
+        if (n === "Map" || n === "Set") return Array.from(o);
+        if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n))
+            return _arrayLikeToArray(o, minLen);
+    }
+
+    function _arrayLikeToArray(arr, len) {
+        if (len == null || len > arr.length) len = arr.length;
+
+        for (var i = 0, arr2 = new Array(len); i < len; i++) arr2[i] = arr[i];
+
+        return arr2;
+    }
+
+    function _createForOfIteratorHelper(o, allowArrayLike) {
+        var it =
+            (typeof Symbol !== "undefined" && o[Symbol.iterator]) || o["@@iterator"];
+
+        if (!it) {
+            if (
+                Array.isArray(o) ||
+                (it = _unsupportedIterableToArray(o)) ||
+                (allowArrayLike && o && typeof o.length === "number")
+            ) {
+                if (it) o = it;
+                var i = 0;
+
+                var F = function() {};
+
+                return {
+                    s: F,
+                    n: function() {
+                        if (i >= o.length)
+                            return {
+                                done: true,
+                            };
+                        return {
+                            done: false,
+                            value: o[i++],
+                        };
+                    },
+                    e: function(e) {
+                        throw e;
+                    },
+                    f: F,
+                };
+            }
+
+            throw new TypeError(
+                "Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method."
+            );
+        }
+
+        var normalCompletion = true,
+            didErr = false,
+            err;
+        return {
+            s: function() {
+                it = it.call(o);
+            },
+            n: function() {
+                var step = it.next();
+                normalCompletion = step.done;
+                return step;
+            },
+            e: function(e) {
+                didErr = true;
+                err = e;
+            },
+            f: function() {
+                try {
+                    if (!normalCompletion && it.return != null) it.return();
+                } finally {
+                    if (didErr) throw err;
+                }
+            },
+        };
+    }
+
+    /**
+     * Parses an URI
+     *
+     * @author Steven Levithan <stevenlevithan.com> (MIT license)
+     * @api private
+     */
+    var re =
+        /^(?:(?![^:@]+:[^:@\/]*@)(http|https|ws|wss):\/\/)?((?:(([^:@]*)(?::([^:@]*))?)?@)?((?:[a-f0-9]{0,4}:){2,7}[a-f0-9]{0,4}|[^:\/?#]*)(?::(\d*))?)(((\/(?:[^?#](?![^?#\/]*\.[^?#\/.]+(?:[?#]|$)))*\/?)?([^?#\/]*))(?:\?([^#]*))?(?:#(.*))?)/;
+    var parts = [
+        "source",
+        "protocol",
+        "authority",
+        "userInfo",
+        "user",
+        "password",
+        "host",
+        "port",
+        "relative",
+        "path",
+        "directory",
+        "file",
+        "query",
+        "anchor",
+    ];
+
+    var parseuri = function parseuri(str) {
+        var src = str,
+            b = str.indexOf("["),
+            e = str.indexOf("]");
+
+        if (b != -1 && e != -1) {
+            str =
+                str.substring(0, b) +
+                str.substring(b, e).replace(/:/g, ";") +
+                str.substring(e, str.length);
+        }
+
+        var m = re.exec(str || ""),
+            uri = {},
+            i = 14;
+
+        while (i--) {
+            uri[parts[i]] = m[i] || "";
+        }
+
+        if (b != -1 && e != -1) {
+            uri.source = src;
+            uri.host = uri.host.substring(1, uri.host.length - 1).replace(/;/g, ":");
+            uri.authority = uri.authority
+                .replace("[", "")
+                .replace("]", "")
+                .replace(/;/g, ":");
+            uri.ipv6uri = true;
+        }
+
+        uri.pathNames = pathNames(uri, uri["path"]);
+        uri.queryKey = queryKey(uri, uri["query"]);
+        return uri;
+    };
+
+    function pathNames(obj, path) {
+        var regx = /\/{2,9}/g,
+            names = path.replace(regx, "/").split("/");
+
+        if (path.substr(0, 1) == "/" || path.length === 0) {
+            names.splice(0, 1);
+        }
+
+        if (path.substr(path.length - 1, 1) == "/") {
+            names.splice(names.length - 1, 1);
+        }
+
+        return names;
+    }
+
+    function queryKey(uri, query) {
+        var data = {};
+        query.replace(/(?:^|&)([^&=]*)=?([^&]*)/g, function($0, $1, $2) {
+            if ($1) {
+                data[$1] = $2;
+            }
+        });
+        return data;
+    }
+
+    /**
+     * URL parser.
+     *
+     * @param uri - url
+     * @param path - the request path of the connection
+     * @param loc - An object meant to mimic window.location.
+     *        Defaults to window.location.
+     * @public
+     */
+
+    function url(uri) {
+        var path =
+            arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : "";
+        var loc = arguments.length > 2 ? arguments[2] : undefined;
+        var obj = uri; // default to window.location
+
+        loc = loc || (typeof location !== "undefined" && location);
+        if (null == uri) uri = loc.protocol + "//" + loc.host; // relative path support
+
+        if (typeof uri === "string") {
+            if ("/" === uri.charAt(0)) {
+                if ("/" === uri.charAt(1)) {
+                    uri = loc.protocol + uri;
+                } else {
+                    uri = loc.host + uri;
+                }
+            }
+
+            if (!/^(https?|wss?):\/\//.test(uri)) {
+                if ("undefined" !== typeof loc) {
+                    uri = loc.protocol + "//" + uri;
+                } else {
+                    uri = "https://" + uri;
+                }
+            } // parse
+
+            obj = parseuri(uri);
+        } // make sure we treat `localhost:80` and `localhost` equally
+
+        if (!obj.port) {
+            if (/^(http|ws)$/.test(obj.protocol)) {
+                obj.port = "80";
+            } else if (/^(http|ws)s$/.test(obj.protocol)) {
+                obj.port = "443";
+            }
+        }
+
+        obj.path = obj.path || "/";
+        var ipv6 = obj.host.indexOf(":") !== -1;
+        var host = ipv6 ? "[" + obj.host + "]" : obj.host; // define unique id
+
+        obj.id = obj.protocol + "://" + host + ":" + obj.port + path; // define href
+
+        obj.href =
+            obj.protocol +
+            "://" +
+            host +
+            (loc && loc.port === obj.port ? "" : ":" + obj.port);
+        return obj;
+    }
+
+    var hasCors = {
+        exports: {}
+    };
+
+    /**
+     * Module exports.
+     *
+     * Logic borrowed from Modernizr:
+     *
+     *   - https://github.com/Modernizr/Modernizr/blob/master/feature-detects/cors.js
+     */
+
+    try {
+        hasCors.exports =
+            typeof XMLHttpRequest !== "undefined" &&
+            "withCredentials" in new XMLHttpRequest();
+    } catch (err) {
+        // if XMLHttp support is disabled in IE then it will throw
+        // when trying to create
+        hasCors.exports = false;
+    }
+
+    var hasCORS = hasCors.exports;
+
+    var globalThis = (function() {
+        if (typeof self !== "undefined") {
+            return self;
+        } else if (typeof window !== "undefined") {
+            return window;
+        } else {
+            return Function("return this")();
+        }
+    })();
+
+    // browser shim for xmlhttprequest module
+    function XMLHttpRequest$1(opts) {
+        var xdomain = opts.xdomain; // XMLHttpRequest can be disabled on IE
+
+        try {
+            if ("undefined" !== typeof XMLHttpRequest && (!xdomain || hasCORS)) {
+                return new XMLHttpRequest();
+            }
+        } catch (e) {}
+
+        if (!xdomain) {
+            try {
+                return new globalThis[["Active"].concat("Object").join("X")](
+                    "Microsoft.XMLHTTP"
+                );
+            } catch (e) {}
+        }
+    }
+
+    function pick(obj) {
+        for (
+            var _len = arguments.length,
+                attr = new Array(_len > 1 ? _len - 1 : 0),
+                _key = 1; _key < _len; _key++
+        ) {
+            attr[_key - 1] = arguments[_key];
+        }
+
+        return attr.reduce(function(acc, k) {
+            if (obj.hasOwnProperty(k)) {
+                acc[k] = obj[k];
+            }
+
+            return acc;
+        }, {});
+    } // Keep a reference to the real timeout functions so they can be used when overridden
+
+    var NATIVE_SET_TIMEOUT = setTimeout;
+    var NATIVE_CLEAR_TIMEOUT = clearTimeout;
+
+    function installTimerFunctions(obj, opts) {
+        if (opts.useNativeTimers) {
+            obj.setTimeoutFn = NATIVE_SET_TIMEOUT.bind(globalThis);
+            obj.clearTimeoutFn = NATIVE_CLEAR_TIMEOUT.bind(globalThis);
+        } else {
+            obj.setTimeoutFn = setTimeout.bind(globalThis);
+            obj.clearTimeoutFn = clearTimeout.bind(globalThis);
+        }
+    }
+
+    /**
+     * Expose `Emitter`.
+     */
+
+    var Emitter_1 = Emitter;
+    /**
+     * Initialize a new `Emitter`.
+     *
+     * @api public
+     */
+
+    function Emitter(obj) {
+        if (obj) return mixin(obj);
+    }
+    /**
+     * Mixin the emitter properties.
+     *
+     * @param {Object} obj
+     * @return {Object}
+     * @api private
+     */
+
+    function mixin(obj) {
+        for (var key in Emitter.prototype) {
+            obj[key] = Emitter.prototype[key];
+        }
+
+        return obj;
+    }
+    /**
+     * Listen on the given `event` with `fn`.
+     *
+     * @param {String} event
+     * @param {Function} fn
+     * @return {Emitter}
+     * @api public
+     */
+
+    Emitter.prototype.on = Emitter.prototype.addEventListener = function(
+        event,
+        fn
+    ) {
+        this._callbacks = this._callbacks || {};
+        (this._callbacks["$" + event] = this._callbacks["$" + event] || []).push(
+            fn
+        );
+        return this;
+    };
+    /**
+     * Adds an `event` listener that will be invoked a single
+     * time then automatically removed.
+     *
+     * @param {String} event
+     * @param {Function} fn
+     * @return {Emitter}
+     * @api public
+     */
+
+    Emitter.prototype.once = function(event, fn) {
+        function on() {
+            this.off(event, on);
+            fn.apply(this, arguments);
+        }
+
+        on.fn = fn;
+        this.on(event, on);
+        return this;
+    };
+    /**
+     * Remove the given callback for `event` or all
+     * registered callbacks.
+     *
+     * @param {String} event
+     * @param {Function} fn
+     * @return {Emitter}
+     * @api public
+     */
+
+    Emitter.prototype.off =
+        Emitter.prototype.removeListener =
+        Emitter.prototype.removeAllListeners =
+        Emitter.prototype.removeEventListener =
+        function(event, fn) {
+            this._callbacks = this._callbacks || {}; // all
+
+            if (0 == arguments.length) {
+                this._callbacks = {};
+                return this;
+            } // specific event
+
+            var callbacks = this._callbacks["$" + event];
+            if (!callbacks) return this; // remove all handlers
+
+            if (1 == arguments.length) {
+                delete this._callbacks["$" + event];
+                return this;
+            } // remove specific handler
+
+            var cb;
+
+            for (var i = 0; i < callbacks.length; i++) {
+                cb = callbacks[i];
+
+                if (cb === fn || cb.fn === fn) {
+                    callbacks.splice(i, 1);
+                    break;
+                }
+            } // Remove event specific arrays for event types that no
+            // one is subscribed for to avoid memory leak.
+
+            if (callbacks.length === 0) {
+                delete this._callbacks["$" + event];
+            }
+
+            return this;
+        };
+    /**
+     * Emit `event` with the given args.
+     *
+     * @param {String} event
+     * @param {Mixed} ...
+     * @return {Emitter}
+     */
+
+    Emitter.prototype.emit = function(event) {
+        this._callbacks = this._callbacks || {};
+        var args = new Array(arguments.length - 1),
+            callbacks = this._callbacks["$" + event];
+
+        for (var i = 1; i < arguments.length; i++) {
+            args[i - 1] = arguments[i];
+        }
+
+        if (callbacks) {
+            callbacks = callbacks.slice(0);
+
+            for (var i = 0, len = callbacks.length; i < len; ++i) {
+                callbacks[i].apply(this, args);
+            }
+        }
+
+        return this;
+    }; // alias used for reserved events (protected method)
+
+    Emitter.prototype.emitReserved = Emitter.prototype.emit;
+    /**
+     * Return array of callbacks for `event`.
+     *
+     * @param {String} event
+     * @return {Array}
+     * @api public
+     */
+
+    Emitter.prototype.listeners = function(event) {
+        this._callbacks = this._callbacks || {};
+        return this._callbacks["$" + event] || [];
+    };
+    /**
+     * Check if this emitter has `event` handlers.
+     *
+     * @param {String} event
+     * @return {Boolean}
+     * @api public
+     */
+
+    Emitter.prototype.hasListeners = function(event) {
+        return !!this.listeners(event).length;
+    };
+
+    var PACKET_TYPES = Object.create(null); // no Map = no polyfill
+
+    PACKET_TYPES["open"] = "0";
+    PACKET_TYPES["close"] = "1";
+    PACKET_TYPES["ping"] = "2";
+    PACKET_TYPES["pong"] = "3";
+    PACKET_TYPES["message"] = "4";
+    PACKET_TYPES["upgrade"] = "5";
+    PACKET_TYPES["noop"] = "6";
+    var PACKET_TYPES_REVERSE = Object.create(null);
+    Object.keys(PACKET_TYPES).forEach(function(key) {
+        PACKET_TYPES_REVERSE[PACKET_TYPES[key]] = key;
+    });
+    var ERROR_PACKET = {
+        type: "error",
+        data: "parser error",
+    };
+
+    var withNativeBlob$1 =
+        typeof Blob === "function" ||
+        (typeof Blob !== "undefined" &&
+            Object.prototype.toString.call(Blob) === "[object BlobConstructor]");
+    var withNativeArrayBuffer$2 = typeof ArrayBuffer === "function"; // ArrayBuffer.isView method is not defined in IE10
+
+    var isView$1 = function isView(obj) {
+        return typeof ArrayBuffer.isView === "function" ?
+            ArrayBuffer.isView(obj) :
+            obj && obj.buffer instanceof ArrayBuffer;
+    };
+
+    var encodePacket = function encodePacket(_ref, supportsBinary, callback) {
+        var type = _ref.type,
+            data = _ref.data;
+
+        if (withNativeBlob$1 && data instanceof Blob) {
+            if (supportsBinary) {
+                return callback(data);
+            } else {
+                return encodeBlobAsBase64(data, callback);
+            }
+        } else if (
+            withNativeArrayBuffer$2 &&
+            (data instanceof ArrayBuffer || isView$1(data))
+        ) {
+            if (supportsBinary) {
+                return callback(data);
+            } else {
+                return encodeBlobAsBase64(new Blob([data]), callback);
+            }
+        } // plain string
+
+        return callback(PACKET_TYPES[type] + (data || ""));
+    };
+
+    var encodeBlobAsBase64 = function encodeBlobAsBase64(data, callback) {
+        var fileReader = new FileReader();
+
+        fileReader.onload = function() {
+            var content = fileReader.result.split(",")[1];
+            callback("b" + content);
+        };
+
+        return fileReader.readAsDataURL(data);
+    };
+
+    /*
+     * base64-arraybuffer 1.0.1 <https://github.com/niklasvh/base64-arraybuffer>
+     * Copyright (c) 2021 Niklas von Hertzen <https://hertzen.com>
+     * Released under MIT License
+     */
+    var chars =
+        "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"; // Use a lookup table to find the index.
+
+    var lookup$1 = typeof Uint8Array === "undefined" ? [] : new Uint8Array(256);
+
+    for (var i$1 = 0; i$1 < chars.length; i$1++) {
+        lookup$1[chars.charCodeAt(i$1)] = i$1;
+    }
+
+    var decode$1 = function decode(base64) {
+        var bufferLength = base64.length * 0.75,
+            len = base64.length,
+            i,
+            p = 0,
+            encoded1,
+            encoded2,
+            encoded3,
+            encoded4;
+
+        if (base64[base64.length - 1] === "=") {
+            bufferLength--;
+
+            if (base64[base64.length - 2] === "=") {
+                bufferLength--;
+            }
+        }
+
+        var arraybuffer = new ArrayBuffer(bufferLength),
+            bytes = new Uint8Array(arraybuffer);
+
+        for (i = 0; i < len; i += 4) {
+            encoded1 = lookup$1[base64.charCodeAt(i)];
+            encoded2 = lookup$1[base64.charCodeAt(i + 1)];
+            encoded3 = lookup$1[base64.charCodeAt(i + 2)];
+            encoded4 = lookup$1[base64.charCodeAt(i + 3)];
+            bytes[p++] = (encoded1 << 2) | (encoded2 >> 4);
+            bytes[p++] = ((encoded2 & 15) << 4) | (encoded3 >> 2);
+            bytes[p++] = ((encoded3 & 3) << 6) | (encoded4 & 63);
+        }
+
+        return arraybuffer;
+    };
+
+    var withNativeArrayBuffer$1 = typeof ArrayBuffer === "function";
+
+    var decodePacket = function decodePacket(encodedPacket, binaryType) {
+        if (typeof encodedPacket !== "string") {
+            return {
+                type: "message",
+                data: mapBinary(encodedPacket, binaryType),
+            };
+        }
+
+        var type = encodedPacket.charAt(0);
+
+        if (type === "b") {
+            return {
+                type: "message",
+                data: decodeBase64Packet(encodedPacket.substring(1), binaryType),
+            };
+        }
+
+        var packetType = PACKET_TYPES_REVERSE[type];
+
+        if (!packetType) {
+            return ERROR_PACKET;
+        }
+
+        return encodedPacket.length > 1 ?
+            {
+                type: PACKET_TYPES_REVERSE[type],
+                data: encodedPacket.substring(1),
+            } :
+            {
+                type: PACKET_TYPES_REVERSE[type],
+            };
+    };
+
+    var decodeBase64Packet = function decodeBase64Packet(data, binaryType) {
+        if (withNativeArrayBuffer$1) {
+            var decoded = decode$1(data);
+            return mapBinary(decoded, binaryType);
+        } else {
+            return {
+                base64: true,
+                data: data,
+            }; // fallback for old browsers
+        }
+    };
+
+    var mapBinary = function mapBinary(data, binaryType) {
+        switch (binaryType) {
+            case "blob":
+                return data instanceof ArrayBuffer ? new Blob([data]) : data;
+
+            case "arraybuffer":
+            default:
+                return data;
+                // assuming the data is already an ArrayBuffer
+        }
+    };
+
+    var SEPARATOR = String.fromCharCode(30); // see https://en.wikipedia.org/wiki/Delimiter#ASCII_delimited_text
+
+    var encodePayload = function encodePayload(packets, callback) {
+        // some packets may be added to the array while encoding, so the initial length must be saved
+        var length = packets.length;
+        var encodedPackets = new Array(length);
+        var count = 0;
+        packets.forEach(function(packet, i) {
+            // force base64 encoding for binary packets
+            encodePacket(packet, false, function(encodedPacket) {
+                encodedPackets[i] = encodedPacket;
+
+                if (++count === length) {
+                    callback(encodedPackets.join(SEPARATOR));
+                }
+            });
+        });
+    };
+
+    var decodePayload = function decodePayload(encodedPayload, binaryType) {
+        var encodedPackets = encodedPayload.split(SEPARATOR);
+        var packets = [];
+
+        for (var i = 0; i < encodedPackets.length; i++) {
+            var decodedPacket = decodePacket(encodedPackets[i], binaryType);
+            packets.push(decodedPacket);
+
+            if (decodedPacket.type === "error") {
+                break;
+            }
+        }
+
+        return packets;
+    };
+
+    var protocol$1 = 4;
+
+    var Transport = /*#__PURE__*/ (function(_Emitter) {
+        _inherits(Transport, _Emitter);
+
+        var _super = _createSuper(Transport);
+
+        /**
+         * Transport abstract constructor.
+         *
+         * @param {Object} options.
+         * @api private
+         */
+        function Transport(opts) {
+            var _this;
+
+            _classCallCheck(this, Transport);
+
+            _this = _super.call(this);
+            _this.writable = false;
+            installTimerFunctions(_assertThisInitialized(_this), opts);
+            _this.opts = opts;
+            _this.query = opts.query;
+            _this.readyState = "";
+            _this.socket = opts.socket;
+            return _this;
+        }
+        /**
+         * Emits an error.
+         *
+         * @param {String} str
+         * @return {Transport} for chaining
+         * @api protected
+         */
+
+        _createClass(Transport, [{
+            key: "onError",
+            value: function onError(msg, desc) {
+                var err = new Error(msg); // @ts-ignore
+
+                err.type = "TransportError"; // @ts-ignore
+
+                err.description = desc;
+
+                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
+                    this,
+                    "error",
+                    err
+                );
+
+                return this;
+            },
+            /**
+             * Opens the transport.
+             *
+             * @api public
+             */
+        }, {
+            key: "open",
+            value: function open() {
+                if ("closed" === this.readyState || "" === this.readyState) {
+                    this.readyState = "opening";
+                    this.doOpen();
+                }
+
+                return this;
+            },
+            /**
+             * Closes the transport.
+             *
+             * @api public
+             */
+        }, {
+            key: "close",
+            value: function close() {
+                if ("opening" === this.readyState || "open" === this.readyState) {
+                    this.doClose();
+                    this.onClose();
+                }
+
+                return this;
+            },
+            /**
+             * Sends multiple packets.
+             *
+             * @param {Array} packets
+             * @api public
+             */
+        }, {
+            key: "send",
+            value: function send(packets) {
+                if ("open" === this.readyState) {
+                    this.write(packets);
+                }
+            },
+            /**
+             * Called upon open
+             *
+             * @api protected
+             */
+        }, {
+            key: "onOpen",
+            value: function onOpen() {
+                this.readyState = "open";
+                this.writable = true;
+
+                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
+                    this,
+                    "open"
+                );
+            },
+            /**
+             * Called with data.
+             *
+             * @param {String} data
+             * @api protected
+             */
+        }, {
+            key: "onData",
+            value: function onData(data) {
+                var packet = decodePacket(data, this.socket.binaryType);
+                this.onPacket(packet);
+            },
+            /**
+             * Called with a decoded packet.
+             *
+             * @api protected
+             */
+        }, {
+            key: "onPacket",
+            value: function onPacket(packet) {
+                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
+                    this,
+                    "packet",
+                    packet
+                );
+            },
+            /**
+             * Called upon close.
+             *
+             * @api protected
+             */
+        }, {
+            key: "onClose",
+            value: function onClose() {
+                this.readyState = "closed";
+
+                _get(_getPrototypeOf(Transport.prototype), "emit", this).call(
+                    this,
+                    "close"
+                );
+            },
+        }, ]);
+
+        return Transport;
+    })(Emitter_1);
+
+    var alphabet =
+        "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz-_".split(
+            ""
+        ),
+        length = 64,
+        map = {},
+        seed = 0,
+        i = 0,
+        prev;
+    /**
+     * Return a string representing the specified number.
+     *
+     * @param {Number} num The number to convert.
+     * @returns {String} The string representation of the number.
+     * @api public
+     */
+
+    function encode(num) {
+        var encoded = "";
+
+        do {
+            encoded = alphabet[num % length] + encoded;
+            num = Math.floor(num / length);
+        } while (num > 0);
+
+        return encoded;
+    }
+    /**
+     * Return the integer value specified by the given string.
+     *
+     * @param {String} str The string to convert.
+     * @returns {Number} The integer value represented by the string.
+     * @api public
+     */
+
+    function decode(str) {
+        var decoded = 0;
+
+        for (i = 0; i < str.length; i++) {
+            decoded = decoded * length + map[str.charAt(i)];
+        }
+
+        return decoded;
+    }
+    /**
+     * Yeast: A tiny growing id generator.
+     *
+     * @returns {String} A unique id.
+     * @api public
+     */
+
+    function yeast() {
+        var now = encode(+new Date());
+        if (now !== prev) return (seed = 0), (prev = now);
+        return now + "." + encode(seed++);
+    } //
+    // Map each character to its index.
+    //
+
+    for (; i < length; i++) {
+        map[alphabet[i]] = i;
+    } //
+    // Expose the `yeast`, `encode` and `decode` functions.
+    //
+
+    yeast.encode = encode;
+    yeast.decode = decode;
+    var yeast_1 = yeast;
+
+    var parseqs = {};
+
+    /**
+     * Compiles a querystring
+     * Returns string representation of the object
+     *
+     * @param {Object}
+     * @api private
+     */
+
+    parseqs.encode = function(obj) {
+        var str = "";
+
+        for (var i in obj) {
+            if (obj.hasOwnProperty(i)) {
+                if (str.length) str += "&";
+                str += encodeURIComponent(i) + "=" + encodeURIComponent(obj[i]);
+            }
+        }
+
+        return str;
+    };
+    /**
+     * Parses a simple querystring into an object
+     *
+     * @param {String} qs
+     * @api private
+     */
+
+    parseqs.decode = function(qs) {
+        var qry = {};
+        var pairs = qs.split("&");
+
+        for (var i = 0, l = pairs.length; i < l; i++) {
+            var pair = pairs[i].split("=");
+            qry[decodeURIComponent(pair[0])] = decodeURIComponent(pair[1]);
+        }
+
+        return qry;
+    };
+
+    var Polling = /*#__PURE__*/ (function(_Transport) {
+        _inherits(Polling, _Transport);
+
+        var _super = _createSuper(Polling);
+
+        function Polling() {
+            var _this;
+
+            _classCallCheck(this, Polling);
+
+            _this = _super.apply(this, arguments);
+            _this.polling = false;
+            return _this;
+        }
+        /**
+         * Transport name.
+         */
+
+        _createClass(Polling, [{
+            key: "name",
+            get: function get() {
+                return "polling";
+            },
+            /**
+             * Opens the socket (triggers polling). We write a PING message to determine
+             * when the transport is open.
+             *
+             * @api private
+             */
+        }, {
+            key: "doOpen",
+            value: function doOpen() {
+                this.poll();
+            },
+            /**
+             * Pauses polling.
+             *
+             * @param {Function} callback upon buffers are flushed and transport is paused
+             * @api private
+             */
+        }, {
+            key: "pause",
+            value: function pause(onPause) {
+                var _this2 = this;
+
+                this.readyState = "pausing";
+
+                var pause = function pause() {
+                    _this2.readyState = "paused";
+                    onPause();
+                };
+
+                if (this.polling || !this.writable) {
+                    var total = 0;
+
+                    if (this.polling) {
+                        total++;
+                        this.once("pollComplete", function() {
+                            --total || pause();
+                        });
+                    }
+
+                    if (!this.writable) {
+                        total++;
+                        this.once("drain", function() {
+                            --total || pause();
+                        });
+                    }
+                } else {
+                    pause();
+                }
+            },
+            /**
+             * Starts polling cycle.
+             *
+             * @api public
+             */
+        }, {
+            key: "poll",
+            value: function poll() {
+                this.polling = true;
+                this.doPoll();
+                this.emit("poll");
+            },
+            /**
+             * Overloads onData to detect payloads.
+             *
+             * @api private
+             */
+        }, {
+            key: "onData",
+            value: function onData(data) {
+                var _this3 = this;
+
+                var callback = function callback(packet) {
+                    // if its the first message we consider the transport open
+                    if ("opening" === _this3.readyState && packet.type === "open") {
+                        _this3.onOpen();
+                    } // if its a close packet, we close the ongoing requests
+
+                    if ("close" === packet.type) {
+                        _this3.onClose();
+
+                        return false;
+                    } // otherwise bypass onData and handle the message
+
+                    _this3.onPacket(packet);
+                }; // decode payload
+
+                decodePayload(data, this.socket.binaryType).forEach(callback); // if an event did not trigger closing
+
+                if ("closed" !== this.readyState) {
+                    // if we got data we're not polling
+                    this.polling = false;
+                    this.emit("pollComplete");
+
+                    if ("open" === this.readyState) {
+                        this.poll();
+                    }
+                }
+            },
+            /**
+             * For polling, send a close packet.
+             *
+             * @api private
+             */
+        }, {
+            key: "doClose",
+            value: function doClose() {
+                var _this4 = this;
+
+                var close = function close() {
+                    _this4.write([{
+                        type: "close",
+                    }, ]);
+                };
+
+                if ("open" === this.readyState) {
+                    close();
+                } else {
+                    // in case we're trying to close while
+                    // handshaking is in progress (GH-164)
+                    this.once("open", close);
+                }
+            },
+            /**
+             * Writes a packets payload.
+             *
+             * @param {Array} data packets
+             * @param {Function} drain callback
+             * @api private
+             */
+        }, {
+            key: "write",
+            value: function write(packets) {
+                var _this5 = this;
+
+                this.writable = false;
+                encodePayload(packets, function(data) {
+                    _this5.doWrite(data, function() {
+                        _this5.writable = true;
+
+                        _this5.emit("drain");
+                    });
+                });
+            },
+            /**
+             * Generates uri for connection.
+             *
+             * @api private
+             */
+        }, {
+            key: "uri",
+            value: function uri() {
+                var query = this.query || {};
+                var schema = this.opts.secure ? "https" : "http";
+                var port = ""; // cache busting is forced
+
+                if (false !== this.opts.timestampRequests) {
+                    query[this.opts.timestampParam] = yeast_1();
+                }
+
+                if (!this.supportsBinary && !query.sid) {
+                    query.b64 = 1;
+                } // avoid port if default for schema
+
+                if (
+                    this.opts.port &&
+                    (("https" === schema && Number(this.opts.port) !== 443) ||
+                        ("http" === schema && Number(this.opts.port) !== 80))
+                ) {
+                    port = ":" + this.opts.port;
+                }
+
+                var encodedQuery = parseqs.encode(query);
+                var ipv6 = this.opts.hostname.indexOf(":") !== -1;
+                return (
+                    schema +
+                    "://" +
+                    (ipv6 ? "[" + this.opts.hostname + "]" : this.opts.hostname) +
+                    port +
+                    this.opts.path +
+                    (encodedQuery.length ? "?" + encodedQuery : "")
+                );
+            },
+        }, ]);
+
+        return Polling;
+    })(Transport);
+
+    /**
+     * Empty function
+     */
+
+    function empty() {}
+
+    var hasXHR2 = (function() {
+        var xhr = new XMLHttpRequest$1({
+            xdomain: false,
+        });
+        return null != xhr.responseType;
+    })();
+
+    var XHR = /*#__PURE__*/ (function(_Polling) {
+        _inherits(XHR, _Polling);
+
+        var _super = _createSuper(XHR);
+
+        /**
+         * XHR Polling constructor.
+         *
+         * @param {Object} opts
+         * @api public
+         */
+        function XHR(opts) {
+            var _this;
+
+            _classCallCheck(this, XHR);
+
+            _this = _super.call(this, opts);
+
+            if (typeof location !== "undefined") {
+                var isSSL = "https:" === location.protocol;
+                var port = location.port; // some user agents have empty `location.port`
+
+                if (!port) {
+                    port = isSSL ? "443" : "80";
+                }
+
+                _this.xd =
+                    (typeof location !== "undefined" &&
+                        opts.hostname !== location.hostname) ||
+                    port !== opts.port;
+                _this.xs = opts.secure !== isSSL;
+            }
+            /**
+             * XHR supports binary
+             */
+
+            var forceBase64 = opts && opts.forceBase64;
+            _this.supportsBinary = hasXHR2 && !forceBase64;
+            return _this;
+        }
+        /**
+         * Creates a request.
+         *
+         * @param {String} method
+         * @api private
+         */
+
+        _createClass(XHR, [{
+            key: "request",
+            value: function request() {
+                var opts =
+                    arguments.length > 0 && arguments[0] !== undefined ?
+                    arguments[0] :
+                    {};
+
+                _extends(
+                    opts, {
+                        xd: this.xd,
+                        xs: this.xs,
+                    },
+                    this.opts
+                );
+
+                return new Request(this.uri(), opts);
+            },
+            /**
+             * Sends data.
+             *
+             * @param {String} data to send.
+             * @param {Function} called upon flush.
+             * @api private
+             */
+        }, {
+            key: "doWrite",
+            value: function doWrite(data, fn) {
+                var _this2 = this;
+
+                var req = this.request({
+                    method: "POST",
+                    data: data,
+                });
+                req.on("success", fn);
+                req.on("error", function(err) {
+                    _this2.onError("xhr post error", err);
+                });
+            },
+            /**
+             * Starts a poll cycle.
+             *
+             * @api private
+             */
+        }, {
+            key: "doPoll",
+            value: function doPoll() {
+                var _this3 = this;
+
+                var req = this.request();
+                req.on("data", this.onData.bind(this));
+                req.on("error", function(err) {
+                    _this3.onError("xhr poll error", err);
+                });
+                this.pollXhr = req;
+            },
+        }, ]);
+
+        return XHR;
+    })(Polling);
+    var Request = /*#__PURE__*/ (function(_Emitter) {
+        _inherits(Request, _Emitter);
+
+        var _super2 = _createSuper(Request);
+
+        /**
+         * Request constructor
+         *
+         * @param {Object} options
+         * @api public
+         */
+        function Request(uri, opts) {
+            var _this4;
+
+            _classCallCheck(this, Request);
+
+            _this4 = _super2.call(this);
+            installTimerFunctions(_assertThisInitialized(_this4), opts);
+            _this4.opts = opts;
+            _this4.method = opts.method || "GET";
+            _this4.uri = uri;
+            _this4.async = false !== opts.async;
+            _this4.data = undefined !== opts.data ? opts.data : null;
+
+            _this4.create();
+
+            return _this4;
+        }
+        /**
+         * Creates the XHR object and sends the request.
+         *
+         * @api private
+         */
+
+        _createClass(Request, [{
+            key: "create",
+            value: function create() {
+                var _this5 = this;
+
+                var opts = pick(
+                    this.opts,
+                    "agent",
+                    "pfx",
+                    "key",
+                    "passphrase",
+                    "cert",
+                    "ca",
+                    "ciphers",
+                    "rejectUnauthorized",
+                    "autoUnref"
+                );
+                opts.xdomain = !!this.opts.xd;
+                opts.xscheme = !!this.opts.xs;
+                var xhr = (this.xhr = new XMLHttpRequest$1(opts));
+
+                try {
+                    xhr.open(this.method, this.uri, this.async);
+
+                    try {
+                        if (this.opts.extraHeaders) {
+                            xhr.setDisableHeaderCheck && xhr.setDisableHeaderCheck(true);
+
+                            for (var i in this.opts.extraHeaders) {
+                                if (this.opts.extraHeaders.hasOwnProperty(i)) {
+                                    xhr.setRequestHeader(i, this.opts.extraHeaders[i]);
+                                }
+                            }
+                        }
+                    } catch (e) {}
+
+                    if ("POST" === this.method) {
+                        try {
+                            xhr.setRequestHeader(
+                                "Content-type",
+                                "text/plain;charset=UTF-8"
+                            );
+                        } catch (e) {}
+                    }
+
+                    try {
+                        xhr.setRequestHeader("Accept", "*/*");
+                    } catch (e) {} // ie6 check
+
+                    if ("withCredentials" in xhr) {
+                        xhr.withCredentials = this.opts.withCredentials;
+                    }
+
+                    if (this.opts.requestTimeout) {
+                        xhr.timeout = this.opts.requestTimeout;
+                    }
+
+                    xhr.onreadystatechange = function() {
+                        if (4 !== xhr.readyState) return;
+
+                        if (200 === xhr.status || 1223 === xhr.status) {
+                            _this5.onLoad();
+                        } else {
+                            // make sure the `error` event handler that's user-set
+                            // does not throw in the same tick and gets caught here
+                            _this5.setTimeoutFn(function() {
+                                _this5.onError(
+                                    typeof xhr.status === "number" ? xhr.status : 0
+                                );
+                            }, 0);
+                        }
+                    };
+
+                    xhr.send(this.data);
+                } catch (e) {
+                    // Need to defer since .create() is called directly from the constructor
+                    // and thus the 'error' event can only be only bound *after* this exception
+                    // occurs.  Therefore, also, we cannot throw here at all.
+                    this.setTimeoutFn(function() {
+                        _this5.onError(e);
+                    }, 0);
+                    return;
+                }
+
+                if (typeof document !== "undefined") {
+                    this.index = Request.requestsCount++;
+                    Request.requests[this.index] = this;
+                }
+            },
+            /**
+             * Called upon successful response.
+             *
+             * @api private
+             */
+        }, {
+            key: "onSuccess",
+            value: function onSuccess() {
+                this.emit("success");
+                this.cleanup();
+            },
+            /**
+             * Called if we have data.
+             *
+             * @api private
+             */
+        }, {
+            key: "onData",
+            value: function onData(data) {
+                this.emit("data", data);
+                this.onSuccess();
+            },
+            /**
+             * Called upon error.
+             *
+             * @api private
+             */
+        }, {
+            key: "onError",
+            value: function onError(err) {
+                this.emit("error", err);
+                this.cleanup(true);
+            },
+            /**
+             * Cleans up house.
+             *
+             * @api private
+             */
+        }, {
+            key: "cleanup",
+            value: function cleanup(fromError) {
+                if ("undefined" === typeof this.xhr || null === this.xhr) {
+                    return;
+                }
+
+                this.xhr.onreadystatechange = empty;
+
+                if (fromError) {
+                    try {
+                        this.xhr.abort();
+                    } catch (e) {}
+                }
+
+                if (typeof document !== "undefined") {
+                    delete Request.requests[this.index];
+                }
+
+                this.xhr = null;
+            },
+            /**
+             * Called upon load.
+             *
+             * @api private
+             */
+        }, {
+            key: "onLoad",
+            value: function onLoad() {
+                var data = this.xhr.responseText;
+
+                if (data !== null) {
+                    this.onData(data);
+                }
+            },
+            /**
+             * Aborts the request.
+             *
+             * @api public
+             */
+        }, {
+            key: "abort",
+            value: function abort() {
+                this.cleanup();
+            },
+        }, ]);
+
+        return Request;
+    })(Emitter_1);
+    Request.requestsCount = 0;
+    Request.requests = {};
+    /**
+     * Aborts pending requests when unloading the window. This is needed to prevent
+     * memory leaks (e.g. when using IE) and to ensure that no spurious error is
+     * emitted.
+     */
+
+    if (typeof document !== "undefined") {
+        // @ts-ignore
+        if (typeof attachEvent === "function") {
+            // @ts-ignore
+            attachEvent("onunload", unloadHandler);
+        } else if (typeof addEventListener === "function") {
+            var terminationEvent = "onpagehide" in globalThis ? "pagehide" : "unload";
+            addEventListener(terminationEvent, unloadHandler, false);
+        }
+    }
+
+    function unloadHandler() {
+        for (var i in Request.requests) {
+            if (Request.requests.hasOwnProperty(i)) {
+                Request.requests[i].abort();
+            }
+        }
+    }
+
+    var nextTick = (function() {
+        var isPromiseAvailable =
+            typeof Promise === "function" && typeof Promise.resolve === "function";
+
+        if (isPromiseAvailable) {
+            return function(cb) {
+                return Promise.resolve().then(cb);
+            };
+        } else {
+            return function(cb, setTimeoutFn) {
+                return setTimeoutFn(cb, 0);
+            };
+        }
+    })();
+    var WebSocket = globalThis.WebSocket || globalThis.MozWebSocket;
+    var usingBrowserWebSocket = true;
+    var defaultBinaryType = "arraybuffer";
+
+    var isReactNative =
+        typeof navigator !== "undefined" &&
+        typeof navigator.product === "string" &&
+        navigator.product.toLowerCase() === "reactnative";
+    var WS = /*#__PURE__*/ (function(_Transport) {
+        _inherits(WS, _Transport);
+
+        var _super = _createSuper(WS);
+
+        /**
+         * WebSocket transport constructor.
+         *
+         * @api {Object} connection options
+         * @api public
+         */
+        function WS(opts) {
+            var _this;
+
+            _classCallCheck(this, WS);
+
+            _this = _super.call(this, opts);
+            _this.supportsBinary = !opts.forceBase64;
+            return _this;
+        }
+        /**
+         * Transport name.
+         *
+         * @api public
+         */
+
+        _createClass(WS, [{
+            key: "name",
+            get: function get() {
+                return "websocket";
+            },
+            /**
+             * Opens socket.
+             *
+             * @api private
+             */
+        }, {
+            key: "doOpen",
+            value: function doOpen() {
+                if (!this.check()) {
+                    // let probe timeout
+                    return;
+                }
+
+                var uri = this.uri();
+                var protocols = this.opts.protocols; // React Native only supports the 'headers' option, and will print a warning if anything else is passed
+
+                var opts = isReactNative ?
+                    {} :
+                    pick(
+                        this.opts,
+                        "agent",
+                        "perMessageDeflate",
+                        "pfx",
+                        "key",
+                        "passphrase",
+                        "cert",
+                        "ca",
+                        "ciphers",
+                        "rejectUnauthorized",
+                        "localAddress",
+                        "protocolVersion",
+                        "origin",
+                        "maxPayload",
+                        "family",
+                        "checkServerIdentity"
+                    );
+
+                if (this.opts.extraHeaders) {
+                    opts.headers = this.opts.extraHeaders;
+                }
+
+                try {
+                    this.ws =
+                        usingBrowserWebSocket && !isReactNative ?
+                        protocols ?
+                        new WebSocket(uri, protocols) :
+                        new WebSocket(uri) :
+                        new WebSocket(uri, protocols, opts);
+                } catch (err) {
+                    return this.emit("error", err);
+                }
+
+                this.ws.binaryType = this.socket.binaryType || defaultBinaryType;
+                this.addEventListeners();
+            },
+            /**
+             * Adds event listeners to the socket
+             *
+             * @api private
+             */
+        }, {
+            key: "addEventListeners",
+            value: function addEventListeners() {
+                var _this2 = this;
+
+                this.ws.onopen = function() {
+                    if (_this2.opts.autoUnref) {
+                        _this2.ws._socket.unref();
+                    }
+
+                    _this2.onOpen();
+                };
+
+                this.ws.onclose = this.onClose.bind(this);
+
+                this.ws.onmessage = function(ev) {
+                    return _this2.onData(ev.data);
+                };
+
+                this.ws.onerror = function(e) {
+                    return _this2.onError("websocket error", e);
+                };
+            },
+            /**
+             * Writes data to socket.
+             *
+             * @param {Array} array of packets.
+             * @api private
+             */
+        }, {
+            key: "write",
+            value: function write(packets) {
+                var _this3 = this;
+
+                this.writable = false; // encodePacket efficient as it uses WS framing
+                // no need for encodePayload
+
+                var _loop = function _loop(i) {
+                    var packet = packets[i];
+                    var lastPacket = i === packets.length - 1;
+                    encodePacket(packet, _this3.supportsBinary, function(data) {
+                        // always create a new object (GH-437)
+                        var opts = {};
+                        // have a chance of informing us about it yet, in that case send will
+                        // throw an error
+
+                        try {
+                            if (usingBrowserWebSocket) {
+                                // TypeError is thrown when passing the second argument on Safari
+                                _this3.ws.send(data);
+                            }
+                        } catch (e) {}
+
+                        if (lastPacket) {
+                            // fake drain
+                            // defer to next tick to allow Socket to clear writeBuffer
+                            nextTick(function() {
+                                _this3.writable = true;
+
+                                _this3.emit("drain");
+                            }, _this3.setTimeoutFn);
+                        }
+                    });
+                };
+
+                for (var i = 0; i < packets.length; i++) {
+                    _loop(i);
+                }
+            },
+            /**
+             * Closes socket.
+             *
+             * @api private
+             */
+        }, {
+            key: "doClose",
+            value: function doClose() {
+                if (typeof this.ws !== "undefined") {
+                    this.ws.close();
+                    this.ws = null;
+                }
+            },
+            /**
+             * Generates uri for connection.
+             *
+             * @api private
+             */
+        }, {
+            key: "uri",
+            value: function uri() {
+                var query = this.query || {};
+                var schema = this.opts.secure ? "wss" : "ws";
+                var port = ""; // avoid port if default for schema
+
+                if (
+                    this.opts.port &&
+                    (("wss" === schema && Number(this.opts.port) !== 443) ||
+                        ("ws" === schema && Number(this.opts.port) !== 80))
+                ) {
+                    port = ":" + this.opts.port;
+                } // append timestamp to URI
+
+                if (this.opts.timestampRequests) {
+                    query[this.opts.timestampParam] = yeast_1();
+                } // communicate binary support capabilities
+
+                if (!this.supportsBinary) {
+                    query.b64 = 1;
+                }
+
+                var encodedQuery = parseqs.encode(query);
+                var ipv6 = this.opts.hostname.indexOf(":") !== -1;
+                return (
+                    schema +
+                    "://" +
+                    (ipv6 ? "[" + this.opts.hostname + "]" : this.opts.hostname) +
+                    port +
+                    this.opts.path +
+                    (encodedQuery.length ? "?" + encodedQuery : "")
+                );
+            },
+            /**
+             * Feature detection for WebSocket.
+             *
+             * @return {Boolean} whether this transport is available.
+             * @api public
+             */
+        }, {
+            key: "check",
+            value: function check() {
+                return (
+                    !!WebSocket &&
+                    !("__initialize" in WebSocket && this.name === WS.prototype.name)
+                );
+            },
+        }, ]);
+
+        return WS;
+    })(Transport);
+
+    var transports = {
+        websocket: WS,
+        polling: XHR,
+    };
+
+    var Socket$1 = /*#__PURE__*/ (function(_Emitter) {
+        _inherits(Socket, _Emitter);
+
+        var _super = _createSuper(Socket);
+
+        /**
+         * Socket constructor.
+         *
+         * @param {String|Object} uri or options
+         * @param {Object} opts - options
+         * @api public
+         */
+        function Socket(uri) {
+            var _this;
+
+            var opts =
+                arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};
+
+            _classCallCheck(this, Socket);
+
+            _this = _super.call(this);
+
+            if (uri && "object" === _typeof(uri)) {
+                opts = uri;
+                uri = null;
+            }
+
+            if (uri) {
+                uri = parseuri(uri);
+                opts.hostname = uri.host;
+                opts.secure = uri.protocol === "https" || uri.protocol === "wss";
+                opts.port = uri.port;
+                if (uri.query) opts.query = uri.query;
+            } else if (opts.host) {
+                opts.hostname = parseuri(opts.host).host;
+            }
+
+            installTimerFunctions(_assertThisInitialized(_this), opts);
+            _this.secure =
+                null != opts.secure ?
+                opts.secure :
+                typeof location !== "undefined" && "https:" === location.protocol;
+
+            if (opts.hostname && !opts.port) {
+                // if no port is specified manually, use the protocol default
+                opts.port = _this.secure ? "443" : "80";
+            }
+
+            _this.hostname =
+                opts.hostname ||
+                (typeof location !== "undefined" ? location.hostname : "localhost");
+            _this.port =
+                opts.port ||
+                (typeof location !== "undefined" && location.port ?
+                    location.port :
+                    _this.secure ?
+                    "443" :
+                    "80");
+            _this.transports = opts.transports || ["polling", "websocket"];
+            _this.readyState = "";
+            _this.writeBuffer = [];
+            _this.prevBufferLen = 0;
+            _this.opts = _extends({
+                    path: "/engine.io",
+                    agent: false,
+                    withCredentials: false,
+                    upgrade: true,
+                    timestampParam: "t",
+                    rememberUpgrade: false,
+                    rejectUnauthorized: true,
+                    perMessageDeflate: {
+                        threshold: 1024,
+                    },
+                    transportOptions: {},
+                    closeOnBeforeunload: true,
+                },
+                opts
+            );
+            _this.opts.path = _this.opts.path.replace(/\/$/, "") + "/";
+
+            if (typeof _this.opts.query === "string") {
+                _this.opts.query = parseqs.decode(_this.opts.query);
+            } // set on handshake
+
+            _this.id = null;
+            _this.upgrades = null;
+            _this.pingInterval = null;
+            _this.pingTimeout = null; // set on heartbeat
+
+            _this.pingTimeoutTimer = null;
+
+            if (typeof addEventListener === "function") {
+                if (_this.opts.closeOnBeforeunload) {
+                    // Firefox closes the connection when the "beforeunload" event is emitted but not Chrome. This event listener
+                    // ensures every browser behaves the same (no "disconnect" event at the Socket.IO level when the page is
+                    // closed/reloaded)
+                    addEventListener(
+                        "beforeunload",
+                        function() {
+                            if (_this.transport) {
+                                // silently close the transport
+                                _this.transport.removeAllListeners();
+
+                                _this.transport.close();
+                            }
+                        },
+                        false
+                    );
+                }
+
+                if (_this.hostname !== "localhost") {
+                    _this.offlineEventListener = function() {
+                        _this.onClose("transport close");
+                    };
+
+                    addEventListener("offline", _this.offlineEventListener, false);
+                }
+            }
+
+            _this.open();
+
+            return _this;
+        }
+        /**
+         * Creates transport of the given type.
+         *
+         * @param {String} transport name
+         * @return {Transport}
+         * @api private
+         */
+
+        _createClass(Socket, [{
+            key: "createTransport",
+            value: function createTransport(name) {
+                var query = clone(this.opts.query); // append engine.io protocol identifier
+
+                query.EIO = protocol$1; // transport name
+
+                query.transport = name; // session id if we already have one
+
+                if (this.id) query.sid = this.id;
+
+                var opts = _extends({}, this.opts.transportOptions[name], this.opts, {
+                    query: query,
+                    socket: this,
+                    hostname: this.hostname,
+                    secure: this.secure,
+                    port: this.port,
+                });
+
+                return new transports[name](opts);
+            },
+            /**
+             * Initializes transport to use and starts probe.
+             *
+             * @api private
+             */
+        }, {
+            key: "open",
+            value: function open() {
+                var _this2 = this;
+
+                var transport;
+
+                if (
+                    this.opts.rememberUpgrade &&
+                    Socket.priorWebsocketSuccess &&
+                    this.transports.indexOf("websocket") !== -1
+                ) {
+                    transport = "websocket";
+                } else if (0 === this.transports.length) {
+                    // Emit error on next tick so it can be listened to
+                    this.setTimeoutFn(function() {
+                        _this2.emitReserved("error", "No transports available");
+                    }, 0);
+                    return;
+                } else {
+                    transport = this.transports[0];
+                }
+
+                this.readyState = "opening"; // Retry with the next transport if the transport is disabled (jsonp: false)
+
+                try {
+                    transport = this.createTransport(transport);
+                } catch (e) {
+                    this.transports.shift();
+                    this.open();
+                    return;
+                }
+
+                transport.open();
+                this.setTransport(transport);
+            },
+            /**
+             * Sets the current transport. Disables the existing one (if any).
+             *
+             * @api private
+             */
+        }, {
+            key: "setTransport",
+            value: function setTransport(transport) {
+                var _this3 = this;
+
+                if (this.transport) {
+                    this.transport.removeAllListeners();
+                } // set up transport
+
+                this.transport = transport; // set up transport listeners
+
+                transport
+                    .on("drain", this.onDrain.bind(this))
+                    .on("packet", this.onPacket.bind(this))
+                    .on("error", this.onError.bind(this))
+                    .on("close", function() {
+                        _this3.onClose("transport close");
+                    });
+            },
+            /**
+             * Probes a transport.
+             *
+             * @param {String} transport name
+             * @api private
+             */
+        }, {
+            key: "probe",
+            value: function probe(name) {
+                var _this4 = this;
+
+                var transport = this.createTransport(name);
+                var failed = false;
+                Socket.priorWebsocketSuccess = false;
+
+                var onTransportOpen = function onTransportOpen() {
+                    if (failed) return;
+                    transport.send([{
+                        type: "ping",
+                        data: "probe",
+                    }, ]);
+                    transport.once("packet", function(msg) {
+                        if (failed) return;
+
+                        if ("pong" === msg.type && "probe" === msg.data) {
+                            _this4.upgrading = true;
+
+                            _this4.emitReserved("upgrading", transport);
+
+                            if (!transport) return;
+                            Socket.priorWebsocketSuccess = "websocket" === transport.name;
+
+                            _this4.transport.pause(function() {
+                                if (failed) return;
+                                if ("closed" === _this4.readyState) return;
+                                cleanup();
+
+                                _this4.setTransport(transport);
+
+                                transport.send([{
+                                    type: "upgrade",
+                                }, ]);
+
+                                _this4.emitReserved("upgrade", transport);
+
+                                transport = null;
+                                _this4.upgrading = false;
+
+                                _this4.flush();
+                            });
+                        } else {
+                            var err = new Error("probe error"); // @ts-ignore
+
+                            err.transport = transport.name;
+
+                            _this4.emitReserved("upgradeError", err);
+                        }
+                    });
+                };
+
+                function freezeTransport() {
+                    if (failed) return; // Any callback called by transport should be ignored since now
+
+                    failed = true;
+                    cleanup();
+                    transport.close();
+                    transport = null;
+                } // Handle any error that happens while probing
+
+                var onerror = function onerror(err) {
+                    var error = new Error("probe error: " + err); // @ts-ignore
+
+                    error.transport = transport.name;
+                    freezeTransport();
+
+                    _this4.emitReserved("upgradeError", error);
+                };
+
+                function onTransportClose() {
+                    onerror("transport closed");
+                } // When the socket is closed while we're probing
+
+                function onclose() {
+                    onerror("socket closed");
+                } // When the socket is upgraded while we're probing
+
+                function onupgrade(to) {
+                    if (transport && to.name !== transport.name) {
+                        freezeTransport();
+                    }
+                } // Remove all listeners on the transport and on self
+
+                var cleanup = function cleanup() {
+                    transport.removeListener("open", onTransportOpen);
+                    transport.removeListener("error", onerror);
+                    transport.removeListener("close", onTransportClose);
+
+                    _this4.off("close", onclose);
+
+                    _this4.off("upgrading", onupgrade);
+                };
+
+                transport.once("open", onTransportOpen);
+                transport.once("error", onerror);
+                transport.once("close", onTransportClose);
+                this.once("close", onclose);
+                this.once("upgrading", onupgrade);
+                transport.open();
+            },
+            /**
+             * Called when connection is deemed open.
+             *
+             * @api private
+             */
+        }, {
+            key: "onOpen",
+            value: function onOpen() {
+                this.readyState = "open";
+                Socket.priorWebsocketSuccess = "websocket" === this.transport.name;
+                this.emitReserved("open");
+                this.flush(); // we check for `readyState` in case an `open`
+                // listener already closed the socket
+
+                if (
+                    "open" === this.readyState &&
+                    this.opts.upgrade &&
+                    this.transport.pause
+                ) {
+                    var i = 0;
+                    var l = this.upgrades.length;
+
+                    for (; i < l; i++) {
+                        this.probe(this.upgrades[i]);
+                    }
+                }
+            },
+            /**
+             * Handles a packet.
+             *
+             * @api private
+             */
+        }, {
+            key: "onPacket",
+            value: function onPacket(packet) {
+                if (
+                    "opening" === this.readyState ||
+                    "open" === this.readyState ||
+                    "closing" === this.readyState
+                ) {
+                    this.emitReserved("packet", packet); // Socket is live - any packet counts
+
+                    this.emitReserved("heartbeat");
+
+                    switch (packet.type) {
+                        case "open":
+                            this.onHandshake(JSON.parse(packet.data));
+                            break;
+
+                        case "ping":
+                            this.resetPingTimeout();
+                            this.sendPacket("pong");
+                            this.emitReserved("ping");
+                            this.emitReserved("pong");
+                            break;
+
+                        case "error":
+                            var err = new Error("server error"); // @ts-ignore
+
+                            err.code = packet.data;
+                            this.onError(err);
+                            break;
+
+                        case "message":
+                            this.emitReserved("data", packet.data);
+                            this.emitReserved("message", packet.data);
+                            break;
+                    }
+                }
+            },
+            /**
+             * Called upon handshake completion.
+             *
+             * @param {Object} data - handshake obj
+             * @api private
+             */
+        }, {
+            key: "onHandshake",
+            value: function onHandshake(data) {
+                this.emitReserved("handshake", data);
+                this.id = data.sid;
+                this.transport.query.sid = data.sid;
+                this.upgrades = this.filterUpgrades(data.upgrades);
+                this.pingInterval = data.pingInterval;
+                this.pingTimeout = data.pingTimeout;
+                this.onOpen(); // In case open handler closes socket
+
+                if ("closed" === this.readyState) return;
+                this.resetPingTimeout();
+            },
+            /**
+             * Sets and resets ping timeout timer based on server pings.
+             *
+             * @api private
+             */
+        }, {
+            key: "resetPingTimeout",
+            value: function resetPingTimeout() {
+                var _this5 = this;
+
+                this.clearTimeoutFn(this.pingTimeoutTimer);
+                this.pingTimeoutTimer = this.setTimeoutFn(function() {
+                    _this5.onClose("ping timeout");
+                }, this.pingInterval + this.pingTimeout);
+
+                if (this.opts.autoUnref) {
+                    this.pingTimeoutTimer.unref();
+                }
+            },
+            /**
+             * Called on `drain` event
+             *
+             * @api private
+             */
+        }, {
+            key: "onDrain",
+            value: function onDrain() {
+                this.writeBuffer.splice(0, this.prevBufferLen); // setting prevBufferLen = 0 is very important
+                // for example, when upgrading, upgrade packet is sent over,
+                // and a nonzero prevBufferLen could cause problems on `drain`
+
+                this.prevBufferLen = 0;
+
+                if (0 === this.writeBuffer.length) {
+                    this.emitReserved("drain");
+                } else {
+                    this.flush();
+                }
+            },
+            /**
+             * Flush write buffers.
+             *
+             * @api private
+             */
+        }, {
+            key: "flush",
+            value: function flush() {
+                if (
+                    "closed" !== this.readyState &&
+                    this.transport.writable &&
+                    !this.upgrading &&
+                    this.writeBuffer.length
+                ) {
+                    this.transport.send(this.writeBuffer); // keep track of current length of writeBuffer
+                    // splice writeBuffer and callbackBuffer on `drain`
+
+                    this.prevBufferLen = this.writeBuffer.length;
+                    this.emitReserved("flush");
+                }
+            },
+            /**
+             * Sends a message.
+             *
+             * @param {String} message.
+             * @param {Function} callback function.
+             * @param {Object} options.
+             * @return {Socket} for chaining.
+             * @api public
+             */
+        }, {
+            key: "write",
+            value: function write(msg, options, fn) {
+                this.sendPacket("message", msg, options, fn);
+                return this;
+            },
+        }, {
+            key: "send",
+            value: function send(msg, options, fn) {
+                this.sendPacket("message", msg, options, fn);
+                return this;
+            },
+            /**
+             * Sends a packet.
+             *
+             * @param {String} packet type.
+             * @param {String} data.
+             * @param {Object} options.
+             * @param {Function} callback function.
+             * @api private
+             */
+        }, {
+            key: "sendPacket",
+            value: function sendPacket(type, data, options, fn) {
+                if ("function" === typeof data) {
+                    fn = data;
+                    data = undefined;
+                }
+
+                if ("function" === typeof options) {
+                    fn = options;
+                    options = null;
+                }
+
+                if ("closing" === this.readyState || "closed" === this.readyState) {
+                    return;
+                }
+
+                options = options || {};
+                options.compress = false !== options.compress;
+                var packet = {
+                    type: type,
+                    data: data,
+                    options: options,
+                };
+                this.emitReserved("packetCreate", packet);
+                this.writeBuffer.push(packet);
+                if (fn) this.once("flush", fn);
+                this.flush();
+            },
+            /**
+             * Closes the connection.
+             *
+             * @api public
+             */
+        }, {
+            key: "close",
+            value: function close() {
+                var _this6 = this;
+
+                var close = function close() {
+                    _this6.onClose("forced close");
+
+                    _this6.transport.close();
+                };
+
+                var cleanupAndClose = function cleanupAndClose() {
+                    _this6.off("upgrade", cleanupAndClose);
+
+                    _this6.off("upgradeError", cleanupAndClose);
+
+                    close();
+                };
+
+                var waitForUpgrade = function waitForUpgrade() {
+                    // wait for upgrade to finish since we can't send packets while pausing a transport
+                    _this6.once("upgrade", cleanupAndClose);
+
+                    _this6.once("upgradeError", cleanupAndClose);
+                };
+
+                if ("opening" === this.readyState || "open" === this.readyState) {
+                    this.readyState = "closing";
+
+                    if (this.writeBuffer.length) {
+                        this.once("drain", function() {
+                            if (_this6.upgrading) {
+                                waitForUpgrade();
+                            } else {
+                                close();
+                            }
+                        });
+                    } else if (this.upgrading) {
+                        waitForUpgrade();
+                    } else {
+                        close();
+                    }
+                }
+
+                return this;
+            },
+            /**
+             * Called upon transport error
+             *
+             * @api private
+             */
+        }, {
+            key: "onError",
+            value: function onError(err) {
+                Socket.priorWebsocketSuccess = false;
+                this.emitReserved("error", err);
+                this.onClose("transport error", err);
+            },
+            /**
+             * Called upon transport close.
+             *
+             * @api private
+             */
+        }, {
+            key: "onClose",
+            value: function onClose(reason, desc) {
+                if (
+                    "opening" === this.readyState ||
+                    "open" === this.readyState ||
+                    "closing" === this.readyState
+                ) {
+                    // clear timers
+                    this.clearTimeoutFn(this.pingTimeoutTimer); // stop event from firing again for transport
+
+                    this.transport.removeAllListeners("close"); // ensure transport won't stay open
+
+                    this.transport.close(); // ignore further transport communication
+
+                    this.transport.removeAllListeners();
+
+                    if (typeof removeEventListener === "function") {
+                        removeEventListener("offline", this.offlineEventListener, false);
+                    } // set ready state
+
+                    this.readyState = "closed"; // clear session id
+
+                    this.id = null; // emit close event
+
+                    this.emitReserved("close", reason, desc); // clean buffers after, so users can still
+                    // grab the buffers on `close` event
+
+                    this.writeBuffer = [];
+                    this.prevBufferLen = 0;
+                }
+            },
+            /**
+             * Filters upgrades, returning only those matching client transports.
+             *
+             * @param {Array} server upgrades
+             * @api private
+             *
+             */
+        }, {
+            key: "filterUpgrades",
+            value: function filterUpgrades(upgrades) {
+                var filteredUpgrades = [];
+                var i = 0;
+                var j = upgrades.length;
+
+                for (; i < j; i++) {
+                    if (~this.transports.indexOf(upgrades[i]))
+                        filteredUpgrades.push(upgrades[i]);
+                }
+
+                return filteredUpgrades;
+            },
+        }, ]);
+
+        return Socket;
+    })(Emitter_1);
+    Socket$1.protocol = protocol$1;
+
+    function clone(obj) {
+        var o = {};
+
+        for (var i in obj) {
+            if (obj.hasOwnProperty(i)) {
+                o[i] = obj[i];
+            }
+        }
+
+        return o;
+    }
+
+    var withNativeArrayBuffer = typeof ArrayBuffer === "function";
+
+    var isView = function isView(obj) {
+        return typeof ArrayBuffer.isView === "function" ?
+            ArrayBuffer.isView(obj) :
+            obj.buffer instanceof ArrayBuffer;
+    };
+
+    var toString = Object.prototype.toString;
+    var withNativeBlob =
+        typeof Blob === "function" ||
+        (typeof Blob !== "undefined" &&
+            toString.call(Blob) === "[object BlobConstructor]");
+    var withNativeFile =
+        typeof File === "function" ||
+        (typeof File !== "undefined" &&
+            toString.call(File) === "[object FileConstructor]");
+    /**
+     * Returns true if obj is a Buffer, an ArrayBuffer, a Blob or a File.
+     *
+     * @private
+     */
+
+    function isBinary(obj) {
+        return (
+            (withNativeArrayBuffer && (obj instanceof ArrayBuffer || isView(obj))) ||
+            (withNativeBlob && obj instanceof Blob) ||
+            (withNativeFile && obj instanceof File)
+        );
+    }
+
+    function hasBinary(obj, toJSON) {
+        if (!obj || _typeof(obj) !== "object") {
+            return false;
+        }
+
+        if (Array.isArray(obj)) {
+            for (var i = 0, l = obj.length; i < l; i++) {
+                if (hasBinary(obj[i])) {
+                    return true;
+                }
+            }
+
+            return false;
+        }
+
+        if (isBinary(obj)) {
+            return true;
+        }
+
+        if (
+            obj.toJSON &&
+            typeof obj.toJSON === "function" &&
+            arguments.length === 1
+        ) {
+            return hasBinary(obj.toJSON(), true);
+        }
+
+        for (var key in obj) {
+            if (
+                Object.prototype.hasOwnProperty.call(obj, key) &&
+                hasBinary(obj[key])
+            ) {
+                return true;
+            }
+        }
+
+        return false;
+    }
+
+    /**
+     * Replaces every Buffer | ArrayBuffer | Blob | File in packet with a numbered placeholder.
+     *
+     * @param {Object} packet - socket.io event packet
+     * @return {Object} with deconstructed packet and list of buffers
+     * @public
+     */
+
+    function deconstructPacket(packet) {
+        var buffers = [];
+        var packetData = packet.data;
+        var pack = packet;
+        pack.data = _deconstructPacket(packetData, buffers);
+        pack.attachments = buffers.length; // number of binary 'attachments'
+
+        return {
+            packet: pack,
+            buffers: buffers,
+        };
+    }
+
+    function _deconstructPacket(data, buffers) {
+        if (!data) return data;
+
+        if (isBinary(data)) {
+            var placeholder = {
+                _placeholder: true,
+                num: buffers.length,
+            };
+            buffers.push(data);
+            return placeholder;
+        } else if (Array.isArray(data)) {
+            var newData = new Array(data.length);
+
+            for (var i = 0; i < data.length; i++) {
+                newData[i] = _deconstructPacket(data[i], buffers);
+            }
+
+            return newData;
+        } else if (_typeof(data) === "object" && !(data instanceof Date)) {
+            var _newData = {};
+
+            for (var key in data) {
+                if (data.hasOwnProperty(key)) {
+                    _newData[key] = _deconstructPacket(data[key], buffers);
+                }
+            }
+
+            return _newData;
+        }
+
+        return data;
+    }
+    /**
+     * Reconstructs a binary packet from its placeholder packet and buffers
+     *
+     * @param {Object} packet - event packet with placeholders
+     * @param {Array} buffers - binary buffers to put in placeholder positions
+     * @return {Object} reconstructed packet
+     * @public
+     */
+
+    function reconstructPacket(packet, buffers) {
+        packet.data = _reconstructPacket(packet.data, buffers);
+        packet.attachments = undefined; // no longer useful
+
+        return packet;
+    }
+
+    function _reconstructPacket(data, buffers) {
+        if (!data) return data;
+
+        if (data && data._placeholder) {
+            return buffers[data.num]; // appropriate buffer (should be natural order anyway)
+        } else if (Array.isArray(data)) {
+            for (var i = 0; i < data.length; i++) {
+                data[i] = _reconstructPacket(data[i], buffers);
+            }
+        } else if (_typeof(data) === "object") {
+            for (var key in data) {
+                if (data.hasOwnProperty(key)) {
+                    data[key] = _reconstructPacket(data[key], buffers);
+                }
+            }
+        }
+
+        return data;
+    }
+
+    /**
+     * Protocol version.
+     *
+     * @public
+     */
+
+    var protocol = 5;
+    var PacketType;
+
+    (function(PacketType) {
+        PacketType[(PacketType["CONNECT"] = 0)] = "CONNECT";
+        PacketType[(PacketType["DISCONNECT"] = 1)] = "DISCONNECT";
+        PacketType[(PacketType["EVENT"] = 2)] = "EVENT";
+        PacketType[(PacketType["ACK"] = 3)] = "ACK";
+        PacketType[(PacketType["CONNECT_ERROR"] = 4)] = "CONNECT_ERROR";
+        PacketType[(PacketType["BINARY_EVENT"] = 5)] = "BINARY_EVENT";
+        PacketType[(PacketType["BINARY_ACK"] = 6)] = "BINARY_ACK";
+    })(PacketType || (PacketType = {}));
+    /**
+     * A socket.io Encoder instance
+     */
+
+    var Encoder = /*#__PURE__*/ (function() {
+        function Encoder() {
+            _classCallCheck(this, Encoder);
+        }
+
+        _createClass(Encoder, [{
+            key: "encode",
+            value:
+                /**
+                 * Encode a packet as a single string if non-binary, or as a
+                 * buffer sequence, depending on packet type.
+                 *
+                 * @param {Object} obj - packet object
+                 */
+                function encode(obj) {
+                    if (obj.type === PacketType.EVENT || obj.type === PacketType.ACK) {
+                        if (hasBinary(obj)) {
+                            obj.type =
+                                obj.type === PacketType.EVENT ?
+                                PacketType.BINARY_EVENT :
+                                PacketType.BINARY_ACK;
+                            return this.encodeAsBinary(obj);
+                        }
+                    }
+
+                    return [this.encodeAsString(obj)];
+                },
+            /**
+             * Encode packet as string.
+             */
+        }, {
+            key: "encodeAsString",
+            value: function encodeAsString(obj) {
+                // first is type
+                var str = "" + obj.type; // attachments if we have them
+
+                if (
+                    obj.type === PacketType.BINARY_EVENT ||
+                    obj.type === PacketType.BINARY_ACK
+                ) {
+                    str += obj.attachments + "-";
+                } // if we have a namespace other than `/`
+                // we append it followed by a comma `,`
+
+                if (obj.nsp && "/" !== obj.nsp) {
+                    str += obj.nsp + ",";
+                } // immediately followed by the id
+
+                if (null != obj.id) {
+                    str += obj.id;
+                } // json data
+
+                if (null != obj.data) {
+                    str += JSON.stringify(obj.data);
+                }
+
+                return str;
+            },
+            /**
+             * Encode packet as 'buffer sequence' by removing blobs, and
+             * deconstructing packet into object with placeholders and
+             * a list of buffers.
+             */
+        }, {
+            key: "encodeAsBinary",
+            value: function encodeAsBinary(obj) {
+                var deconstruction = deconstructPacket(obj);
+                var pack = this.encodeAsString(deconstruction.packet);
+                var buffers = deconstruction.buffers;
+                buffers.unshift(pack); // add packet info to beginning of data list
+
+                return buffers; // write all the buffers
+            },
+        }, ]);
+
+        return Encoder;
+    })();
+    /**
+     * A socket.io Decoder instance
+     *
+     * @return {Object} decoder
+     */
+
+    var Decoder = /*#__PURE__*/ (function(_Emitter) {
+        _inherits(Decoder, _Emitter);
+
+        var _super = _createSuper(Decoder);
+
+        function Decoder() {
+            _classCallCheck(this, Decoder);
+
+            return _super.call(this);
+        }
+        /**
+         * Decodes an encoded packet string into packet JSON.
+         *
+         * @param {String} obj - encoded packet
+         */
+
+        _createClass(
+            Decoder,
+            [{
+                key: "add",
+                value: function add(obj) {
+                    var packet;
+
+                    if (typeof obj === "string") {
+                        packet = this.decodeString(obj);
+
+                        if (
+                            packet.type === PacketType.BINARY_EVENT ||
+                            packet.type === PacketType.BINARY_ACK
+                        ) {
+                            // binary packet's json
+                            this.reconstructor = new BinaryReconstructor(packet); // no attachments, labeled binary but no binary data to follow
+
+                            if (packet.attachments === 0) {
+                                _get(
+                                    _getPrototypeOf(Decoder.prototype),
+                                    "emitReserved",
+                                    this
+                                ).call(this, "decoded", packet);
+                            }
+                        } else {
+                            // non-binary full packet
+                            _get(
+                                _getPrototypeOf(Decoder.prototype),
+                                "emitReserved",
+                                this
+                            ).call(this, "decoded", packet);
+                        }
+                    } else if (isBinary(obj) || obj.base64) {
+                        // raw binary data
+                        if (!this.reconstructor) {
+                            throw new Error(
+                                "got binary data when not reconstructing a packet"
+                            );
+                        } else {
+                            packet = this.reconstructor.takeBinaryData(obj);
+
+                            if (packet) {
+                                // received final buffer
+                                this.reconstructor = null;
+
+                                _get(
+                                    _getPrototypeOf(Decoder.prototype),
+                                    "emitReserved",
+                                    this
+                                ).call(this, "decoded", packet);
+                            }
+                        }
+                    } else {
+                        throw new Error("Unknown type: " + obj);
+                    }
+                },
+                /**
+                 * Decode a packet String (JSON data)
+                 *
+                 * @param {String} str
+                 * @return {Object} packet
+                 */
+            }, {
+                key: "decodeString",
+                value: function decodeString(str) {
+                    var i = 0; // look up type
+
+                    var p = {
+                        type: Number(str.charAt(0)),
+                    };
+
+                    if (PacketType[p.type] === undefined) {
+                        throw new Error("unknown packet type " + p.type);
+                    } // look up attachments if type binary
+
+                    if (
+                        p.type === PacketType.BINARY_EVENT ||
+                        p.type === PacketType.BINARY_ACK
+                    ) {
+                        var start = i + 1;
+
+                        while (str.charAt(++i) !== "-" && i != str.length) {}
+
+                        var buf = str.substring(start, i);
+
+                        if (buf != Number(buf) || str.charAt(i) !== "-") {
+                            throw new Error("Illegal attachments");
+                        }
+
+                        p.attachments = Number(buf);
+                    } // look up namespace (if any)
+
+                    if ("/" === str.charAt(i + 1)) {
+                        var _start = i + 1;
+
+                        while (++i) {
+                            var c = str.charAt(i);
+                            if ("," === c) break;
+                            if (i === str.length) break;
+                        }
+
+                        p.nsp = str.substring(_start, i);
+                    } else {
+                        p.nsp = "/";
+                    } // look up id
+
+                    var next = str.charAt(i + 1);
+
+                    if ("" !== next && Number(next) == next) {
+                        var _start2 = i + 1;
+
+                        while (++i) {
+                            var _c = str.charAt(i);
+
+                            if (null == _c || Number(_c) != _c) {
+                                --i;
+                                break;
+                            }
+
+                            if (i === str.length) break;
+                        }
+
+                        p.id = Number(str.substring(_start2, i + 1));
+                    } // look up json data
+
+                    if (str.charAt(++i)) {
+                        var payload = tryParse(str.substr(i));
+
+                        if (Decoder.isPayloadValid(p.type, payload)) {
+                            p.data = payload;
+                        } else {
+                            throw new Error("invalid payload");
+                        }
+                    }
+
+                    return p;
+                },
+            }, {
+                key: "destroy",
+                value:
+                    /**
+                     * Deallocates a parser's resources
+                     */
+                    function destroy() {
+                        if (this.reconstructor) {
+                            this.reconstructor.finishedReconstruction();
+                        }
+                    },
+            }, ],
+            [{
+                key: "isPayloadValid",
+                value: function isPayloadValid(type, payload) {
+                    switch (type) {
+                        case PacketType.CONNECT:
+                            return _typeof(payload) === "object";
+
+                        case PacketType.DISCONNECT:
+                            return payload === undefined;
+
+                        case PacketType.CONNECT_ERROR:
+                            return (
+                                typeof payload === "string" || _typeof(payload) === "object"
+                            );
+
+                        case PacketType.EVENT:
+                        case PacketType.BINARY_EVENT:
+                            return Array.isArray(payload) && payload.length > 0;
+
+                        case PacketType.ACK:
+                        case PacketType.BINARY_ACK:
+                            return Array.isArray(payload);
+                    }
+                },
+            }, ]
+        );
+
+        return Decoder;
+    })(Emitter_1);
+
+    function tryParse(str) {
+        try {
+            return JSON.parse(str);
+        } catch (e) {
+            return false;
+        }
+    }
+    /**
+     * A manager of a binary event's 'buffer sequence'. Should
+     * be constructed whenever a packet of type BINARY_EVENT is
+     * decoded.
+     *
+     * @param {Object} packet
+     * @return {BinaryReconstructor} initialized reconstructor
+     */
+
+    var BinaryReconstructor = /*#__PURE__*/ (function() {
+        function BinaryReconstructor(packet) {
+            _classCallCheck(this, BinaryReconstructor);
+
+            this.packet = packet;
+            this.buffers = [];
+            this.reconPack = packet;
+        }
+        /**
+         * Method to be called when binary data received from connection
+         * after a BINARY_EVENT packet.
+         *
+         * @param {Buffer | ArrayBuffer} binData - the raw binary data received
+         * @return {null | Object} returns null if more binary data is expected or
+         *   a reconstructed packet object if all buffers have been received.
+         */
+
+        _createClass(BinaryReconstructor, [{
+            key: "takeBinaryData",
+            value: function takeBinaryData(binData) {
+                this.buffers.push(binData);
+
+                if (this.buffers.length === this.reconPack.attachments) {
+                    // done with buffer list
+                    var packet = reconstructPacket(this.reconPack, this.buffers);
+                    this.finishedReconstruction();
+                    return packet;
+                }
+
+                return null;
+            },
+            /**
+             * Cleans up binary packet reconstruction variables.
+             */
+        }, {
+            key: "finishedReconstruction",
+            value: function finishedReconstruction() {
+                this.reconPack = null;
+                this.buffers = [];
+            },
+        }, ]);
+
+        return BinaryReconstructor;
+    })();
+
+    var parser = /*#__PURE__*/ Object.freeze({
+        __proto__: null,
+        protocol: protocol,
+        get PacketType() {
+            return PacketType;
+        },
+        Encoder: Encoder,
+        Decoder: Decoder,
+    });
+
+    function on(obj, ev, fn) {
+        obj.on(ev, fn);
+        return function subDestroy() {
+            obj.off(ev, fn);
+        };
+    }
+
+    /**
+     * Internal events.
+     * These events can't be emitted by the user.
+     */
+
+    var RESERVED_EVENTS = Object.freeze({
+        connect: 1,
+        connect_error: 1,
+        disconnect: 1,
+        disconnecting: 1,
+        // EventEmitter reserved events: https://nodejs.org/api/events.html#events_event_newlistener
+        newListener: 1,
+        removeListener: 1,
+    });
+    var Socket = /*#__PURE__*/ (function(_Emitter) {
+        _inherits(Socket, _Emitter);
+
+        var _super = _createSuper(Socket);
+
+        /**
+         * `Socket` constructor.
+         *
+         * @public
+         */
+        function Socket(io, nsp, opts) {
+            var _this;
+
+            _classCallCheck(this, Socket);
+
+            _this = _super.call(this);
+            _this.connected = false;
+            _this.disconnected = true;
+            _this.receiveBuffer = [];
+            _this.sendBuffer = [];
+            _this.ids = 0;
+            _this.acks = {};
+            _this.flags = {};
+            _this.io = io;
+            _this.nsp = nsp;
+
+            if (opts && opts.auth) {
+                _this.auth = opts.auth;
+            }
+
+            if (_this.io._autoConnect) _this.open();
+            return _this;
+        }
+        /**
+         * Subscribe to open, close and packet events
+         *
+         * @private
+         */
+
+        _createClass(Socket, [{
+            key: "subEvents",
+            value: function subEvents() {
+                if (this.subs) return;
+                var io = this.io;
+                this.subs = [
+                    on(io, "open", this.onopen.bind(this)),
+                    on(io, "packet", this.onpacket.bind(this)),
+                    on(io, "error", this.onerror.bind(this)),
+                    on(io, "close", this.onclose.bind(this)),
+                ];
+            },
+            /**
+             * Whether the Socket will try to reconnect when its Manager connects or reconnects
+             */
+        }, {
+            key: "active",
+            get: function get() {
+                return !!this.subs;
+            },
+            /**
+             * "Opens" the socket.
+             *
+             * @public
+             */
+        }, {
+            key: "connect",
+            value: function connect() {
+                if (this.connected) return this;
+                this.subEvents();
+                if (!this.io["_reconnecting"]) this.io.open(); // ensure open
+
+                if ("open" === this.io._readyState) this.onopen();
+                return this;
+            },
+            /**
+             * Alias for connect()
+             */
+        }, {
+            key: "open",
+            value: function open() {
+                return this.connect();
+            },
+            /**
+             * Sends a `message` event.
+             *
+             * @return self
+             * @public
+             */
+        }, {
+            key: "send",
+            value: function send() {
+                for (
+                    var _len = arguments.length, args = new Array(_len), _key = 0; _key < _len; _key++
+                ) {
+                    args[_key] = arguments[_key];
+                }
+
+                args.unshift("message");
+                this.emit.apply(this, args);
+                return this;
+            },
+            /**
+             * Override `emit`.
+             * If the event is in `events`, it's emitted normally.
+             *
+             * @return self
+             * @public
+             */
+        }, {
+            key: "emit",
+            value: function emit(ev) {
+                if (RESERVED_EVENTS.hasOwnProperty(ev)) {
+                    throw new Error('"' + ev + '" is a reserved event name');
+                }
+
+                for (
+                    var _len2 = arguments.length,
+                        args = new Array(_len2 > 1 ? _len2 - 1 : 0),
+                        _key2 = 1; _key2 < _len2; _key2++
+                ) {
+                    args[_key2 - 1] = arguments[_key2];
+                }
+
+                args.unshift(ev);
+                var packet = {
+                    type: PacketType.EVENT,
+                    data: args,
+                };
+                packet.options = {};
+                packet.options.compress = this.flags.compress !== false; // event ack callback
+
+                if ("function" === typeof args[args.length - 1]) {
+                    var id = this.ids++;
+                    var ack = args.pop();
+
+                    this._registerAckCallback(id, ack);
+
+                    packet.id = id;
+                }
+
+                var isTransportWritable =
+                    this.io.engine &&
+                    this.io.engine.transport &&
+                    this.io.engine.transport.writable;
+                var discardPacket =
+                    this.flags["volatile"] && (!isTransportWritable || !this.connected);
+
+                if (discardPacket);
+                else if (this.connected) {
+                    this.packet(packet);
+                } else {
+                    this.sendBuffer.push(packet);
+                }
+
+                this.flags = {};
+                return this;
+            },
+            /**
+             * @private
+             */
+        }, {
+            key: "_registerAckCallback",
+            value: function _registerAckCallback(id, ack) {
+                var _this2 = this;
+
+                var timeout = this.flags.timeout;
+
+                if (timeout === undefined) {
+                    this.acks[id] = ack;
+                    return;
+                } // @ts-ignore
+
+                var timer = this.io.setTimeoutFn(function() {
+                    delete _this2.acks[id];
+
+                    for (var i = 0; i < _this2.sendBuffer.length; i++) {
+                        if (_this2.sendBuffer[i].id === id) {
+                            _this2.sendBuffer.splice(i, 1);
+                        }
+                    }
+
+                    ack.call(_this2, new Error("operation has timed out"));
+                }, timeout);
+
+                this.acks[id] = function() {
+                    // @ts-ignore
+                    _this2.io.clearTimeoutFn(timer);
+
+                    for (
+                        var _len3 = arguments.length, args = new Array(_len3), _key3 = 0; _key3 < _len3; _key3++
+                    ) {
+                        args[_key3] = arguments[_key3];
+                    }
+
+                    ack.apply(_this2, [null].concat(args));
+                };
+            },
+            /**
+             * Sends a packet.
+             *
+             * @param packet
+             * @private
+             */
+        }, {
+            key: "packet",
+            value: function packet(_packet) {
+                _packet.nsp = this.nsp;
+
+                this.io._packet(_packet);
+            },
+            /**
+             * Called upon engine `open`.
+             *
+             * @private
+             */
+        }, {
+            key: "onopen",
+            value: function onopen() {
+                var _this3 = this;
+
+                if (typeof this.auth == "function") {
+                    this.auth(function(data) {
+                        _this3.packet({
+                            type: PacketType.CONNECT,
+                            data: data,
+                        });
+                    });
+                } else {
+                    this.packet({
+                        type: PacketType.CONNECT,
+                        data: this.auth,
+                    });
+                }
+            },
+            /**
+             * Called upon engine or manager `error`.
+             *
+             * @param err
+             * @private
+             */
+        }, {
+            key: "onerror",
+            value: function onerror(err) {
+                if (!this.connected) {
+                    this.emitReserved("connect_error", err);
+                }
+            },
+            /**
+             * Called upon engine `close`.
+             *
+             * @param reason
+             * @private
+             */
+        }, {
+            key: "onclose",
+            value: function onclose(reason) {
+                this.connected = false;
+                this.disconnected = true;
+                delete this.id;
+                this.emitReserved("disconnect", reason);
+            },
+            /**
+             * Called with socket packet.
+             *
+             * @param packet
+             * @private
+             */
+        }, {
+            key: "onpacket",
+            value: function onpacket(packet) {
+                var sameNamespace = packet.nsp === this.nsp;
+                if (!sameNamespace) return;
+
+                switch (packet.type) {
+                    case PacketType.CONNECT:
+                        if (packet.data && packet.data.sid) {
+                            var id = packet.data.sid;
+                            this.onconnect(id);
+                        } else {
+                            this.emitReserved(
+                                "connect_error",
+                                new Error(
+                                    "It seems you are trying to reach a Socket.IO server in v2.x with a v3.x client, but they are not compatible (more information here: https://socket.io/docs/v3/migrating-from-2-x-to-3-0/)"
+                                )
+                            );
+                        }
+
+                        break;
+
+                    case PacketType.EVENT:
+                        this.onevent(packet);
+                        break;
+
+                    case PacketType.BINARY_EVENT:
+                        this.onevent(packet);
+                        break;
+
+                    case PacketType.ACK:
+                        this.onack(packet);
+                        break;
+
+                    case PacketType.BINARY_ACK:
+                        this.onack(packet);
+                        break;
+
+                    case PacketType.DISCONNECT:
+                        this.ondisconnect();
+                        break;
+
+                    case PacketType.CONNECT_ERROR:
+                        this.destroy();
+                        var err = new Error(packet.data.message); // @ts-ignore
+
+                        err.data = packet.data.data;
+                        this.emitReserved("connect_error", err);
+                        break;
+                }
+            },
+            /**
+             * Called upon a server event.
+             *
+             * @param packet
+             * @private
+             */
+        }, {
+            key: "onevent",
+            value: function onevent(packet) {
+                var args = packet.data || [];
+
+                if (null != packet.id) {
+                    args.push(this.ack(packet.id));
+                }
+
+                if (this.connected) {
+                    this.emitEvent(args);
+                } else {
+                    this.receiveBuffer.push(Object.freeze(args));
+                }
+            },
+        }, {
+            key: "emitEvent",
+            value: function emitEvent(args) {
+                if (this._anyListeners && this._anyListeners.length) {
+                    var listeners = this._anyListeners.slice();
+
+                    var _iterator = _createForOfIteratorHelper(listeners),
+                        _step;
+
+                    try {
+                        for (_iterator.s(); !(_step = _iterator.n()).done;) {
+                            var listener = _step.value;
+                            listener.apply(this, args);
+                        }
+                    } catch (err) {
+                        _iterator.e(err);
+                    } finally {
+                        _iterator.f();
+                    }
+                }
+
+                _get(_getPrototypeOf(Socket.prototype), "emit", this).apply(
+                    this,
+                    args
+                );
+            },
+            /**
+             * Produces an ack callback to emit with an event.
+             *
+             * @private
+             */
+        }, {
+            key: "ack",
+            value: function ack(id) {
+                var self = this;
+                var sent = false;
+                return function() {
+                    // prevent double callbacks
+                    if (sent) return;
+                    sent = true;
+
+                    for (
+                        var _len4 = arguments.length, args = new Array(_len4), _key4 = 0; _key4 < _len4; _key4++
+                    ) {
+                        args[_key4] = arguments[_key4];
+                    }
+
+                    self.packet({
+                        type: PacketType.ACK,
+                        id: id,
+                        data: args,
+                    });
+                };
+            },
+            /**
+             * Called upon a server acknowlegement.
+             *
+             * @param packet
+             * @private
+             */
+        }, {
+            key: "onack",
+            value: function onack(packet) {
+                var ack = this.acks[packet.id];
+
+                if ("function" === typeof ack) {
+                    ack.apply(this, packet.data);
+                    delete this.acks[packet.id];
+                }
+            },
+            /**
+             * Called upon server connect.
+             *
+             * @private
+             */
+        }, {
+            key: "onconnect",
+            value: function onconnect(id) {
+                this.id = id;
+                this.connected = true;
+                this.disconnected = false;
+                this.emitBuffered();
+                this.emitReserved("connect");
+            },
+            /**
+             * Emit buffered events (received and emitted).
+             *
+             * @private
+             */
+        }, {
+            key: "emitBuffered",
+            value: function emitBuffered() {
+                var _this4 = this;
+
+                this.receiveBuffer.forEach(function(args) {
+                    return _this4.emitEvent(args);
+                });
+                this.receiveBuffer = [];
+                this.sendBuffer.forEach(function(packet) {
+                    return _this4.packet(packet);
+                });
+                this.sendBuffer = [];
+            },
+            /**
+             * Called upon server disconnect.
+             *
+             * @private
+             */
+        }, {
+            key: "ondisconnect",
+            value: function ondisconnect() {
+                this.destroy();
+                this.onclose("io server disconnect");
+            },
+            /**
+             * Called upon forced client/server side disconnections,
+             * this method ensures the manager stops tracking us and
+             * that reconnections don't get triggered for this.
+             *
+             * @private
+             */
+        }, {
+            key: "destroy",
+            value: function destroy() {
+                if (this.subs) {
+                    // clean subscriptions to avoid reconnections
+                    this.subs.forEach(function(subDestroy) {
+                        return subDestroy();
+                    });
+                    this.subs = undefined;
+                }
+
+                this.io["_destroy"](this);
+            },
+            /**
+             * Disconnects the socket manually.
+             *
+             * @return self
+             * @public
+             */
+        }, {
+            key: "disconnect",
+            value: function disconnect() {
+                if (this.connected) {
+                    this.packet({
+                        type: PacketType.DISCONNECT,
+                    });
+                } // remove socket from pool
+
+                this.destroy();
+
+                if (this.connected) {
+                    // fire events
+                    this.onclose("io client disconnect");
+                }
+
+                return this;
+            },
+            /**
+             * Alias for disconnect()
+             *
+             * @return self
+             * @public
+             */
+        }, {
+            key: "close",
+            value: function close() {
+                return this.disconnect();
+            },
+            /**
+             * Sets the compress flag.
+             *
+             * @param compress - if `true`, compresses the sending data
+             * @return self
+             * @public
+             */
+        }, {
+            key: "compress",
+            value: function compress(_compress) {
+                this.flags.compress = _compress;
+                return this;
+            },
+            /**
+             * Sets a modifier for a subsequent event emission that the event message will be dropped when this socket is not
+             * ready to send messages.
+             *
+             * @returns self
+             * @public
+             */
+        }, {
+            key: "volatile",
+            get: function get() {
+                this.flags["volatile"] = true;
+                return this;
+            },
+            /**
+             * Sets a modifier for a subsequent event emission that the callback will be called with an error when the
+             * given number of milliseconds have elapsed without an acknowledgement from the server:
+             *
+             * ```
+             * socket.timeout(5000).emit("my-event", (err) => {
+             *   if (err) {
+             *     // the server did not acknowledge the event in the given delay
+             *   }
+             * });
+             * ```
+             *
+             * @returns self
+             * @public
+             */
+        }, {
+            key: "timeout",
+            value: function timeout(_timeout) {
+                this.flags.timeout = _timeout;
+                return this;
+            },
+            /**
+             * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the
+             * callback.
+             *
+             * @param listener
+             * @public
+             */
+        }, {
+            key: "onAny",
+            value: function onAny(listener) {
+                this._anyListeners = this._anyListeners || [];
+
+                this._anyListeners.push(listener);
+
+                return this;
+            },
+            /**
+             * Adds a listener that will be fired when any event is emitted. The event name is passed as the first argument to the
+             * callback. The listener is added to the beginning of the listeners array.
+             *
+             * @param listener
+             * @public
+             */
+        }, {
+            key: "prependAny",
+            value: function prependAny(listener) {
+                this._anyListeners = this._anyListeners || [];
+
+                this._anyListeners.unshift(listener);
+
+                return this;
+            },
+            /**
+             * Removes the listener that will be fired when any event is emitted.
+             *
+             * @param listener
+             * @public
+             */
+        }, {
+            key: "offAny",
+            value: function offAny(listener) {
+                if (!this._anyListeners) {
+                    return this;
+                }
+
+                if (listener) {
+                    var listeners = this._anyListeners;
+
+                    for (var i = 0; i < listeners.length; i++) {
+                        if (listener === listeners[i]) {
+                            listeners.splice(i, 1);
+                            return this;
+                        }
+                    }
+                } else {
+                    this._anyListeners = [];
+                }
+
+                return this;
+            },
+            /**
+             * Returns an array of listeners that are listening for any event that is specified. This array can be manipulated,
+             * e.g. to remove listeners.
+             *
+             * @public
+             */
+        }, {
+            key: "listenersAny",
+            value: function listenersAny() {
+                return this._anyListeners || [];
+            },
+        }, ]);
+
+        return Socket;
+    })(Emitter_1);
+
+    /**
+     * Expose `Backoff`.
+     */
+
+    var backo2 = Backoff;
+    /**
+     * Initialize backoff timer with `opts`.
+     *
+     * - `min` initial timeout in milliseconds [100]
+     * - `max` max timeout [10000]
+     * - `jitter` [0]
+     * - `factor` [2]
+     *
+     * @param {Object} opts
+     * @api public
+     */
+
+    function Backoff(opts) {
+        opts = opts || {};
+        this.ms = opts.min || 100;
+        this.max = opts.max || 10000;
+        this.factor = opts.factor || 2;
+        this.jitter = opts.jitter > 0 && opts.jitter <= 1 ? opts.jitter : 0;
+        this.attempts = 0;
+    }
+    /**
+     * Return the backoff duration.
+     *
+     * @return {Number}
+     * @api public
+     */
+
+    Backoff.prototype.duration = function() {
+        var ms = this.ms * Math.pow(this.factor, this.attempts++);
+
+        if (this.jitter) {
+            var rand = Math.random();
+            var deviation = Math.floor(rand * this.jitter * ms);
+            ms = (Math.floor(rand * 10) & 1) == 0 ? ms - deviation : ms + deviation;
+        }
+
+        return Math.min(ms, this.max) | 0;
+    };
+    /**
+     * Reset the number of attempts.
+     *
+     * @api public
+     */
+
+    Backoff.prototype.reset = function() {
+        this.attempts = 0;
+    };
+    /**
+     * Set the minimum duration
+     *
+     * @api public
+     */
+
+    Backoff.prototype.setMin = function(min) {
+        this.ms = min;
+    };
+    /**
+     * Set the maximum duration
+     *
+     * @api public
+     */
+
+    Backoff.prototype.setMax = function(max) {
+        this.max = max;
+    };
+    /**
+     * Set the jitter
+     *
+     * @api public
+     */
+
+    Backoff.prototype.setJitter = function(jitter) {
+        this.jitter = jitter;
+    };
+
+    var Manager = /*#__PURE__*/ (function(_Emitter) {
+        _inherits(Manager, _Emitter);
+
+        var _super = _createSuper(Manager);
+
+        function Manager(uri, opts) {
+            var _this;
+
+            _classCallCheck(this, Manager);
+
+            var _a;
+
+            _this = _super.call(this);
+            _this.nsps = {};
+            _this.subs = [];
+
+            if (uri && "object" === _typeof(uri)) {
+                opts = uri;
+                uri = undefined;
+            }
+
+            opts = opts || {};
+            opts.path = opts.path || "/socket.io";
+            _this.opts = opts;
+            installTimerFunctions(_assertThisInitialized(_this), opts);
+
+            _this.reconnection(opts.reconnection !== false);
+
+            _this.reconnectionAttempts(opts.reconnectionAttempts || Infinity);
+
+            _this.reconnectionDelay(opts.reconnectionDelay || 1000);
+
+            _this.reconnectionDelayMax(opts.reconnectionDelayMax || 5000);
+
+            _this.randomizationFactor(
+                (_a = opts.randomizationFactor) !== null && _a !== void 0 ? _a : 0.5
+            );
+
+            _this.backoff = new backo2({
+                min: _this.reconnectionDelay(),
+                max: _this.reconnectionDelayMax(),
+                jitter: _this.randomizationFactor(),
+            });
+
+            _this.timeout(null == opts.timeout ? 20000 : opts.timeout);
+
+            _this._readyState = "closed";
+            _this.uri = uri;
+
+            var _parser = opts.parser || parser;
+
+            _this.encoder = new _parser.Encoder();
+            _this.decoder = new _parser.Decoder();
+            _this._autoConnect = opts.autoConnect !== false;
+            if (_this._autoConnect) _this.open();
+            return _this;
+        }
+
+        _createClass(Manager, [{
+            key: "reconnection",
+            value: function reconnection(v) {
+                if (!arguments.length) return this._reconnection;
+                this._reconnection = !!v;
+                return this;
+            },
+        }, {
+            key: "reconnectionAttempts",
+            value: function reconnectionAttempts(v) {
+                if (v === undefined) return this._reconnectionAttempts;
+                this._reconnectionAttempts = v;
+                return this;
+            },
+        }, {
+            key: "reconnectionDelay",
+            value: function reconnectionDelay(v) {
+                var _a;
+
+                if (v === undefined) return this._reconnectionDelay;
+                this._reconnectionDelay = v;
+                (_a = this.backoff) === null || _a === void 0 ? void 0 : _a.setMin(v);
+                return this;
+            },
+        }, {
+            key: "randomizationFactor",
+            value: function randomizationFactor(v) {
+                var _a;
+
+                if (v === undefined) return this._randomizationFactor;
+                this._randomizationFactor = v;
+                (_a = this.backoff) === null || _a === void 0 ?
+                    void 0 :
+                    _a.setJitter(v);
+                return this;
+            },
+        }, {
+            key: "reconnectionDelayMax",
+            value: function reconnectionDelayMax(v) {
+                var _a;
+
+                if (v === undefined) return this._reconnectionDelayMax;
+                this._reconnectionDelayMax = v;
+                (_a = this.backoff) === null || _a === void 0 ? void 0 : _a.setMax(v);
+                return this;
+            },
+        }, {
+            key: "timeout",
+            value: function timeout(v) {
+                if (!arguments.length) return this._timeout;
+                this._timeout = v;
+                return this;
+            },
+            /**
+             * Starts trying to reconnect if reconnection is enabled and we have not
+             * started reconnecting yet
+             *
+             * @private
+             */
+        }, {
+            key: "maybeReconnectOnOpen",
+            value: function maybeReconnectOnOpen() {
+                // Only try to reconnect if it's the first time we're connecting
+                if (
+                    !this._reconnecting &&
+                    this._reconnection &&
+                    this.backoff.attempts === 0
+                ) {
+                    // keeps reconnection from firing twice for the same reconnection loop
+                    this.reconnect();
+                }
+            },
+            /**
+             * Sets the current transport `socket`.
+             *
+             * @param {Function} fn - optional, callback
+             * @return self
+             * @public
+             */
+        }, {
+            key: "open",
+            value: function open(fn) {
+                var _this2 = this;
+
+                if (~this._readyState.indexOf("open")) return this;
+                this.engine = new Socket$1(this.uri, this.opts);
+                var socket = this.engine;
+                var self = this;
+                this._readyState = "opening";
+                this.skipReconnect = false; // emit `open`
+
+                var openSubDestroy = on(socket, "open", function() {
+                    self.onopen();
+                    fn && fn();
+                }); // emit `error`
+
+                var errorSub = on(socket, "error", function(err) {
+                    self.cleanup();
+                    self._readyState = "closed";
+
+                    _this2.emitReserved("error", err);
+
+                    if (fn) {
+                        fn(err);
+                    } else {
+                        // Only do this if there is no fn to handle the error
+                        self.maybeReconnectOnOpen();
+                    }
+                });
+
+                if (false !== this._timeout) {
+                    var timeout = this._timeout;
+
+                    if (timeout === 0) {
+                        openSubDestroy(); // prevents a race condition with the 'open' event
+                    } // set timer
+
+                    var timer = this.setTimeoutFn(function() {
+                        openSubDestroy();
+                        socket.close(); // @ts-ignore
+
+                        socket.emit("error", new Error("timeout"));
+                    }, timeout);
+
+                    if (this.opts.autoUnref) {
+                        timer.unref();
+                    }
+
+                    this.subs.push(function subDestroy() {
+                        clearTimeout(timer);
+                    });
+                }
+
+                this.subs.push(openSubDestroy);
+                this.subs.push(errorSub);
+                return this;
+            },
+            /**
+             * Alias for open()
+             *
+             * @return self
+             * @public
+             */
+        }, {
+            key: "connect",
+            value: function connect(fn) {
+                return this.open(fn);
+            },
+            /**
+             * Called upon transport open.
+             *
+             * @private
+             */
+        }, {
+            key: "onopen",
+            value: function onopen() {
+                // clear old subs
+                this.cleanup(); // mark as open
+
+                this._readyState = "open";
+                this.emitReserved("open"); // add new subs
+
+                var socket = this.engine;
+                this.subs.push(
+                    on(socket, "ping", this.onping.bind(this)),
+                    on(socket, "data", this.ondata.bind(this)),
+                    on(socket, "error", this.onerror.bind(this)),
+                    on(socket, "close", this.onclose.bind(this)),
+                    on(this.decoder, "decoded", this.ondecoded.bind(this))
+                );
+            },
+            /**
+         * Called upon a ping.  var io;
+
+    if (newConnection) {
+      io = new Manager(source, opts);
+    } else {
+      if (!cache[id]) {
+        cache[id] = new Manager(source, opts);
+      }
+
+      io = cache[id];
+    }
+
+    if (parsed.query && !opts.query) {
+      opts.query = parsed.queryKey;
+    }
+
+    return io.socket(parsed.path, opts);
+  } // so that "lookup" can be used both as a function (e.g. `io(...)`) and as a
+  // namespace (e.g. `io.connect(...)`), for backward compatibility
+
+  _extends(lookup, {
+    Manager: Manager,
+    Socket: Socket,
+    io: lookup,
+    connect: lookup,
+  });
+
+  return lookup;
+});
+//# sourceMappingURL=socket.io.js.map
+
+         * @private
+         */
+        }, {
+            key: "onping",
+            value: function onping() {
+                this.emitReserved("ping");
+            },
+            /**
+             * Called with data.
+             *
+             * @private
+             */
+        }, {
+            key: "ondata",
+            value: function ondata(data) {
+                this.decoder.add(data);
+            },
+            /**
+             * Called when parser fully decodes a packet.
+             *
+             * @private
+             */
+        }, {
+            key: "ondecoded",
+            value: function ondecoded(packet) {
+                this.emitReserved("packet", packet);
+            },
+            /**
+             * Called upon socket error.
+             *
+             * @private
+             */
+        }, {
+            key: "onerror",
+            value: function onerror(err) {
+                this.emitReserved("error", err);
+            },
+            /**
+             * Creates a new socket for the given `nsp`.
+             *
+             * @return {Socket}
+             * @public
+             */
+        }, {
+            key: "socket",
+            value: function socket(nsp, opts) {
+                var socket = this.nsps[nsp];
+
+                if (!socket) {
+                    socket = new Socket(this, nsp, opts);
+                    this.nsps[nsp] = socket;
+                }
+
+                return socket;
+            },
+            /**
+             * Called upon a socket close.
+             *
+             * @param socket
+             * @private
+             */
+        }, {
+            key: "_destroy",
+            value: function _destroy(socket) {
+                var nsps = Object.keys(this.nsps);
+
+                for (var _i = 0, _nsps = nsps; _i < _nsps.length; _i++) {
+                    var nsp = _nsps[_i];
+                    var _socket = this.nsps[nsp];
+
+                    if (_socket.active) {
+                        return;
+                    }
+                }
+
+                this._close();
+            },
+            /**
+             * Writes a packet.
+             *
+             * @param packet
+             * @private
+             */
+        }, {
+            key: "_packet",
+            value: function _packet(packet) {
+                var encodedPackets = this.encoder.encode(packet);
+
+                for (var i = 0; i < encodedPackets.length; i++) {
+                    this.engine.write(encodedPackets[i], packet.options);
+                }
+            },
+            /**
+             * Clean up transport subscriptions and packet buffer.
+             *
+             * @private
+             */
+        }, {
+            key: "cleanup",
+            value: function cleanup() {
+                this.subs.forEach(function(subDestroy) {
+                    return subDestroy();
+                });
+                this.subs.length = 0;
+                this.decoder.destroy();
+            },
+            /**
+             * Close the current socket.
+             *
+             * @private
+             */
+        }, {
+            key: "_close",
+            value: function _close() {
+                this.skipReconnect = true;
+                this._reconnecting = false;
+                this.onclose("forced close");
+                if (this.engine) this.engine.close();
+            },
+            /**
+             * Alias for close()
+             *
+             * @private
+             */
+        }, {
+            key: "disconnect",
+            value: function disconnect() {
+                return this._close();
+            },
+            /**
+             * Called upon engine close.
+             *
+             * @private
+             */
+        }, {
+            key: "onclose",
+            value: function onclose(reason) {
+                this.cleanup();
+                this.backoff.reset();
+                this._readyState = "closed";
+                this.emitReserved("close", reason);
+
+                if (this._reconnection && !this.skipReconnect) {
+                    this.reconnect();
+                }
+            },
+            /**
+             * Attempt a reconnection.
+             *
+             * @private
+             */
+        }, {
+            key: "reconnect",
+            value: function reconnect() {
+                var _this3 = this;
+
+                if (this._reconnecting || this.skipReconnect) return this;
+                var self = this;
+
+                if (this.backoff.attempts >= this._reconnectionAttempts) {
+                    this.backoff.reset();
+                    this.emitReserved("reconnect_failed");
+                    this._reconnecting = false;
+                } else {
+                    var delay = this.backoff.duration();
+                    this._reconnecting = true;
+                    var timer = this.setTimeoutFn(function() {
+                        if (self.skipReconnect) return;
+
+                        _this3.emitReserved("reconnect_attempt", self.backoff.attempts); // check again for the case socket closed in above events
+
+                        if (self.skipReconnect) return;
+                        self.open(function(err) {
+                            if (err) {
+                                self._reconnecting = false;
+                                self.reconnect();
+
+                                _this3.emitReserved("reconnect_error", err);
+                            } else {
+                                self.onreconnect();
+                            }
+                        });
+                    }, delay);
+
+                    if (this.opts.autoUnref) {
+                        timer.unref();
+                    }
+
+                    this.subs.push(function subDestroy() {
+                        clearTimeout(timer);
+                    });
+                }
+            },
+            /**
+             * Called upon successful reconnect.
+             *
+             * @private
+             */
+        }, {
+            key: "onreconnect",
+            value: function onreconnect() {
+                var attempt = this.backoff.attempts;
+                this._reconnecting = false;
+                this.backoff.reset();
+                this.emitReserved("reconnect", attempt);
+            },
+        }, ]);
+
+        return Manager;
+    })(Emitter_1);
+
+    /**
+     * Managers cache.
+     */
+
+    var cache = {};
+
+    function lookup(uri, opts) {
+        if (_typeof(uri) === "object") {
+            opts = uri;
+            uri = undefined;
+        }
+
+        opts = opts || {};
+        var parsed = url(uri, opts.path || "/socket.io");
+        var source = parsed.source;
+        var id = parsed.id;
+        var path = parsed.path;
+        var sameNamespace = cache[id] && path in cache[id]["nsps"];
+        var newConnection =
+            opts.forceNew ||
+            opts["force new connection"] ||
+            false === opts.multiplex ||
+            sameNamespace;
+        var io;
+
+        if (newConnection) {
+            io = new Manager(source, opts);
+        } else {
+            if (!cache[id]) {
+                cache[id] = new Manager(source, opts);
+            }
+
+            io = cache[id];
+        }
+
+        if (parsed.query && !opts.query) {
+            opts.query = parsed.queryKey;
+        }
+
+        return io.socket(parsed.path, opts);
+    } // so that "lookup" can be used both as a function (e.g. `io(...)`) and as a
+    // namespace (e.g. `io.connect(...)`), for backward compatibility
+
+    _extends(lookup, {
+        Manager: Manager,
+        Socket: Socket,
+        io: lookup,
+        connect: lookup,
+    });
+
+    return lookup;
+});
 //# sourceMappingURL=socket.io.js.map
```

### Comparing `lidia-0.8.0/src/lidia/static/style.css` & `lidia-0.8.1/src/lidia/static/style.css`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-:root {
-  --pfdGreen: #07ed35;
-  --pfdAmber: #ffbf00;
-  --pfdRed: #ff0f0f;
-  --pfdGround: #965b27;
-  --pfdSky: #1e88f5;
-  --pfdMagenta: #ff00ff;
-  --pfdCyan: #00ffff;
-}
-
-@font-face {
-  font-family: "Roboto Mono";
-  src: url("RobotoMono-Thin.ttf") format("truetype");
-  font-weight: 100;
-}
-
-@font-face {
-  font-family: "Roboto Mono";
-  src: url("RobotoMono-ExtraLight.ttf") format("truetype");
-  font-weight: 200;
-}
-
-@font-face {
-  font-family: "Roboto Mono";
-  src: url("RobotoMono-Light.ttf") format("truetype");
-  font-weight: 300;
-}
-
-@font-face {
-  font-family: "Roboto Mono";
-  src: url("RobotoMono-Regular.ttf") format("truetype");
-  font-weight: 400;
-}
-
-@font-face {
-  font-family: "Roboto Mono";
-  src: url("RobotoMono-Medium.ttf") format("truetype");
-  font-weight: 500;
-}
-
-@font-face {
-  font-family: "Roboto Mono";
-  src: url("RobotoMono-SemiBold.ttf") format("truetype");
-  font-weight: 600;
-}
-
-@font-face {
-  font-family: "Roboto Mono";
-  src: url("RobotoMono-Bold.ttf") format("truetype");
-  font-weight: 700;
-}
-
-html,
-body {
-  margin: 0;
-  padding: 0;
-  /* overflow: hidden; */
-  height: 100%;
-  width: 100%;
-  background-color: #000;
-  font-family: "Roboto Mono", monospace;
-}
-
-svg#mainSvg {
-  position: absolute;
-  top: 0;
-  left: 0;
-  height: 100%;
-  width: 100%;
-}
-
-.controls {
-  position: absolute;
-  bottom: 0;
-  left: 0;
-  padding: 2em;
-  border: 3px solid #fff;
-  border-radius: 10px;
-  font-size: larger;
-  color: #fff;
-  background-color: #4d4d4d;
-
-  opacity: 0;
-}
-
-.controls:hover {
-  opacity: 1;
-}
-
-.controls > p {
-  display: flex;
-  align-items: center;
-  gap: 12px;
-}
-
-.content {
-  color: #fff;
-  margin: 2rem auto;
-  padding: 0 1rem;
-  max-width: 60rem;
-  font-size: 1.2rem;
-}
-
-.content a {
-  color: var(--pfdCyan);
-}
+:root {
+  --pfdGreen: #07ed35;
+  --pfdAmber: #ffbf00;
+  --pfdRed: #ff0f0f;
+  --pfdGround: #965b27;
+  --pfdSky: #1e88f5;
+  --pfdMagenta: #ff00ff;
+  --pfdCyan: #00ffff;
+}
+
+@font-face {
+  font-family: "Roboto Mono";
+  src: url("RobotoMono-Thin.ttf") format("truetype");
+  font-weight: 100;
+}
+
+@font-face {
+  font-family: "Roboto Mono";
+  src: url("RobotoMono-ExtraLight.ttf") format("truetype");
+  font-weight: 200;
+}
+
+@font-face {
+  font-family: "Roboto Mono";
+  src: url("RobotoMono-Light.ttf") format("truetype");
+  font-weight: 300;
+}
+
+@font-face {
+  font-family: "Roboto Mono";
+  src: url("RobotoMono-Regular.ttf") format("truetype");
+  font-weight: 400;
+}
+
+@font-face {
+  font-family: "Roboto Mono";
+  src: url("RobotoMono-Medium.ttf") format("truetype");
+  font-weight: 500;
+}
+
+@font-face {
+  font-family: "Roboto Mono";
+  src: url("RobotoMono-SemiBold.ttf") format("truetype");
+  font-weight: 600;
+}
+
+@font-face {
+  font-family: "Roboto Mono";
+  src: url("RobotoMono-Bold.ttf") format("truetype");
+  font-weight: 700;
+}
+
+html,
+body {
+  margin: 0;
+  padding: 0;
+  /* overflow: hidden; */
+  height: 100%;
+  width: 100%;
+  background-color: #000;
+  font-family: "Roboto Mono", monospace;
+}
+
+svg#mainSvg {
+  position: absolute;
+  top: 0;
+  left: 0;
+  height: 100%;
+  width: 100%;
+}
+
+.controls {
+  position: absolute;
+  bottom: 0;
+  left: 0;
+  padding: 2em;
+  border: 3px solid #fff;
+  border-radius: 10px;
+  font-size: larger;
+  color: #fff;
+  background-color: #4d4d4d;
+
+  opacity: 0;
+}
+
+.controls:hover {
+  opacity: 1;
+}
+
+.controls > p {
+  display: flex;
+  align-items: center;
+  gap: 12px;
+}
+
+.content {
+  color: #fff;
+  margin: 2rem auto;
+  padding: 0 1rem;
+  max-width: 60rem;
+  font-size: 1.2rem;
+}
+
+.content a {
+  color: var(--pfdCyan);
+}
```

### Comparing `lidia-0.8.0/src/lidia/utils/pack_lidia.m` & `lidia-0.8.1/src/lidia/utils/pack_lidia.m`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-function data = pack_lidia( ...
-    ned_north, ...
-    ned_east, ...
-    ned_down, ...
-    att_roll, ...
-    att_pitch, ...
-    att_yaw, ...
-    v_body_x, ...
-    v_body_y, ...
-    v_body_z, ...
-    v_ned_north, ...
-    v_ned_east, ...
-    v_ned_down, ...
-    ctrl_stick_right, ...
-    ctrl_stick_pull, ...
-    ctrl_throttle, ...
-    ctrl_pedals_right, ...
-    ctrl_collective_up, ...
-    t_boot, ...
-    trgt_ctrl_stick_right, ...
-    trgt_ctrl_stick_pull, ...
-    trgt_ctrl_throttle, ...
-    trgt_ctrl_pedals_right, ...
-    trgt_ctrl_collective_up) % 23 arguments
-%PACK_LIDIA Pack aircraft data into binary format
-%   The output is array of bytes in MsgPack format, as expected by
-%   'smol' source of lidia package
-%
-%   This is generated using pack_maker.py to create code suitable for
-%   use in Simulink - known size of I/O (see below), no map or struct usage
-%
-%   Arguments:
-%       ned: Position in local horizon coordinate system, in meters
-%       att: Aircraft attitude, in radians
-%       v_body: Velocity in body frame, in meters per second
-%       v_ned: Velocity in local horizon coordinate system, in meters per second
-%       ctrl: Control inceptors position, normalized by max deflection
-%       t_boot: Time from the start of simulation, in milliseconds
-%       trgt_ctrl: TARGET Control inceptors position, normalized by max deflection
-
-    data = uint8([...
-        0x87, ... % map length 7
-        0xa3, 'ned', ... % string length 3
-        0x93, ... % array length 3
-        0xcb, b(double(ned_north)), ... % double
-        0xcb, b(double(ned_east)), ... % double
-        0xcb, b(double(ned_down)), ... % double
-        0xa3, 'att', ... % string length 3
-        0x93, ... % array length 3
-        0xca, b(single(att_roll)), ... % float
-        0xca, b(single(att_pitch)), ... % float
-        0xca, b(single(att_yaw)), ... % float
-        0xa6, 'v_body', ... % string length 6
-        0x93, ... % array length 3
-        0xca, b(single(v_body_x)), ... % float
-        0xca, b(single(v_body_y)), ... % float
-        0xca, b(single(v_body_z)), ... % float
-        0xa5, 'v_ned', ... % string length 5
-        0x93, ... % array length 3
-        0xca, b(single(v_ned_north)), ... % float
-        0xca, b(single(v_ned_east)), ... % float
-        0xca, b(single(v_ned_down)), ... % float
-        0xa4, 'ctrl', ... % string length 4
-        0x95, ... % array length 5
-        0xca, b(single(ctrl_stick_right)), ... % float
-        0xca, b(single(ctrl_stick_pull)), ... % float
-        0xca, b(single(ctrl_throttle)), ... % float
-        0xca, b(single(ctrl_pedals_right)), ... % float
-        0xca, b(single(ctrl_collective_up)), ... % float
-        0xa6, 't_boot', ... % string length 6
-        0xce, b(uint32(t_boot)), ... % 32-bit unsigned integer
-        0xa4, 'trgt', ... % string length 4
-        0x81, ... % map length 1
-        0xa4, 'ctrl', ... % string length 4
-        0x95, ... % array length 5
-        0xca, b(single(trgt_ctrl_stick_right)), ... % float
-        0xca, b(single(trgt_ctrl_stick_pull)), ... % float
-        0xca, b(single(trgt_ctrl_throttle)), ... % float
-        0xca, b(single(trgt_ctrl_pedals_right)), ... % float
-        0xca, b(single(trgt_ctrl_collective_up)), ... % float
-    ]);
-% data length 178 bytes
-end
-
-% You might need to manually configure Simulink output:
-%   Size: 1 178
-%   Type: uint8
-% The warning message "Wrap on overflow detected" can be ignored
-
-function bytes = b(value)
-    % reverse byte order to convert from little endian to big endian
-    bytes = typecast(swapbytes(value), 'uint8');
-end
+function data = pack_lidia( ...
+    ned_north, ...
+    ned_east, ...
+    ned_down, ...
+    att_roll, ...
+    att_pitch, ...
+    att_yaw, ...
+    v_body_x, ...
+    v_body_y, ...
+    v_body_z, ...
+    v_ned_north, ...
+    v_ned_east, ...
+    v_ned_down, ...
+    ctrl_stick_right, ...
+    ctrl_stick_pull, ...
+    ctrl_throttle, ...
+    ctrl_pedals_right, ...
+    ctrl_collective_up, ...
+    t_boot, ...
+    trgt_ctrl_stick_right, ...
+    trgt_ctrl_stick_pull, ...
+    trgt_ctrl_throttle, ...
+    trgt_ctrl_pedals_right, ...
+    trgt_ctrl_collective_up) % 23 arguments
+%PACK_LIDIA Pack aircraft data into binary format
+%   The output is array of bytes in MsgPack format, as expected by
+%   'smol' source of lidia package
+%
+%   This is generated using pack_maker.py to create code suitable for
+%   use in Simulink - known size of I/O (see below), no map or struct usage
+%
+%   Arguments:
+%       ned: Position in local horizon coordinate system, in meters
+%       att: Aircraft attitude, in radians
+%       v_body: Velocity in body frame, in meters per second
+%       v_ned: Velocity in local horizon coordinate system, in meters per second
+%       ctrl: Control inceptors position, normalized by max deflection
+%       t_boot: Time from the start of simulation, in milliseconds
+%       trgt_ctrl: TARGET Control inceptors position, normalized by max deflection
+
+    data = uint8([...
+        0x87, ... % map length 7
+        0xa3, 'ned', ... % string length 3
+        0x93, ... % array length 3
+        0xcb, b(double(ned_north)), ... % double
+        0xcb, b(double(ned_east)), ... % double
+        0xcb, b(double(ned_down)), ... % double
+        0xa3, 'att', ... % string length 3
+        0x93, ... % array length 3
+        0xca, b(single(att_roll)), ... % float
+        0xca, b(single(att_pitch)), ... % float
+        0xca, b(single(att_yaw)), ... % float
+        0xa6, 'v_body', ... % string length 6
+        0x93, ... % array length 3
+        0xca, b(single(v_body_x)), ... % float
+        0xca, b(single(v_body_y)), ... % float
+        0xca, b(single(v_body_z)), ... % float
+        0xa5, 'v_ned', ... % string length 5
+        0x93, ... % array length 3
+        0xca, b(single(v_ned_north)), ... % float
+        0xca, b(single(v_ned_east)), ... % float
+        0xca, b(single(v_ned_down)), ... % float
+        0xa4, 'ctrl', ... % string length 4
+        0x95, ... % array length 5
+        0xca, b(single(ctrl_stick_right)), ... % float
+        0xca, b(single(ctrl_stick_pull)), ... % float
+        0xca, b(single(ctrl_throttle)), ... % float
+        0xca, b(single(ctrl_pedals_right)), ... % float
+        0xca, b(single(ctrl_collective_up)), ... % float
+        0xa6, 't_boot', ... % string length 6
+        0xce, b(uint32(t_boot)), ... % 32-bit unsigned integer
+        0xa4, 'trgt', ... % string length 4
+        0x81, ... % map length 1
+        0xa4, 'ctrl', ... % string length 4
+        0x95, ... % array length 5
+        0xca, b(single(trgt_ctrl_stick_right)), ... % float
+        0xca, b(single(trgt_ctrl_stick_pull)), ... % float
+        0xca, b(single(trgt_ctrl_throttle)), ... % float
+        0xca, b(single(trgt_ctrl_pedals_right)), ... % float
+        0xca, b(single(trgt_ctrl_collective_up)), ... % float
+    ]);
+% data length 178 bytes
+end
+
+% You might need to manually configure Simulink output:
+%   Size: 1 178
+%   Type: uint8
+% The warning message "Wrap on overflow detected" can be ignored
+
+function bytes = b(value)
+    % reverse byte order to convert from little endian to big endian
+    bytes = typecast(swapbytes(value), 'uint8');
+end
```

### Comparing `lidia-0.8.0/src/lidia/utils/pack_maker.py` & `lidia-0.8.1/src/lidia/utils/pack_maker.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,617 +1,617 @@
-import argparse
-from enum import auto, IntEnum
-import inspect
-from io import StringIO, TextIOBase
-import os
-import platform
-from pydantic import BaseModel
-import re
-import sys
-from typing import Any, Dict, List, Tuple, Type
-
-# setup cross-platform getch() and clear()
-if platform.system() == "Windows":
-    import msvcrt
-
-    def getch():
-        return msvcrt.getwch()
-
-    def clear():
-        os.system('cls')
-else:
-    import tty
-    import termios
-
-    def getch():
-        fd = sys.stdin.fileno()
-        old_settings = termios.tcgetattr(fd)
-        try:
-            tty.setraw(sys.stdin.fileno())
-            ch = sys.stdin.read(1)
-        finally:
-            termios.tcsetattr(fd, termios.TCSADRAIN, old_settings)
-        return ch
-
-    def clear():
-        os.system('clear')
-
-this_path = os.path.dirname(os.path.realpath(__file__))
-lidia_path = os.path.join(this_path, '..', '..')
-sys.path.append(lidia_path)
-from lidia.aircraft import AircraftData, VectorModel  # noqa prevent moving to top of file
-
-
-class FieldInfo(BaseModel):
-    """Details of a `AircraftData` field"""
-
-    name: str
-    """Field name"""
-    docstring: str
-    """Field docstring"""
-    field_type: Type
-    """Contained type"""
-
-    @staticmethod
-    def inspect_AircraftData() -> List['FieldInfo']:
-        infos = []
-        pattern = re.compile(
-            r'^[ \t]+([a-z_]+): Optional\[(?:[A-Za-z]+)\] = None\n[ \t]+"""([^"]+)"""$', flags=re.MULTILINE)
-        for name, doc in re.findall(pattern, inspect.getsource(AircraftData)):
-            field = AircraftData.__fields__[name]
-            infos.append(FieldInfo(
-                name=name,
-                docstring=doc,
-                field_type=field.annotation.__args__[
-                    0],  # annotation type Optional
-            ))
-
-        return infos
-
-
-class Generator(IntEnum):
-    MATLAB = auto()
-    MBDYN = auto()
-    MBDYN_TYPE = auto()
-
-
-class Model:
-    def __init__(self, output: str, verbose=False):
-        self.output = output
-        self.editing_output = False
-        self.previous_output = ''
-        self.verbose = verbose
-        self.last_key = 0
-
-        self.parts = ['main', 'trgt', 'trim']
-        self.selected_part = self.parts[0]
-
-        # only serialization of vectors is supported
-        self.toggles = [info for info in FieldInfo.inspect_AircraftData()
-                        if (issubclass(info.field_type, VectorModel) or info.field_type is int)]
-        self.enabled = {part: ([False] * len(self.toggles))
-                        for part in self.parts}
-
-        self.generators = [
-            (Generator.MATLAB, 'MATLAB', '.m'),
-            (Generator.MBDYN, 'MBDyn', '{.set, .drv, .elm}'),
-        ]
-        self.enabled_gens = [False] * len(self.generators)
-
-        self.extra_choices = 3
-        self.selected_choice = 0
-
-        self.status = ''
-
-    @property
-    def choices_num(self) -> int:
-        return len(self.toggles) + len(self.parts) + len(self.generators) + self.extra_choices
-
-    @property
-    def selected_part_index(self) -> int:
-        return next(i for i, p in enumerate(self.parts) if p == self.selected_part)
-
-    @property
-    def enabled_num(self) -> int:
-        return sum(len([en for en in self.enabled[p] if en]) for p in self.parts)
-
-
-class Command(IntEnum):
-    QUIT = auto()
-    MAKE = auto()
-
-
-class Message(IntEnum):
-    KEY = auto()
-    STATUS = auto()
-
-
-def view(model: Model) -> None:
-    clear()
-    if model.editing_output:
-        print('Edit output filename')
-        print('Confirm editing with Enter, cancel with Esc\n')
-    else:
-        print('Choose fields to be serialized in message')
-        print('Use arrows or j, k to move, select with Enter or Space\n')
-
-    for i, (info, enabled) in enumerate(zip(model.toggles, model.enabled[model.selected_part])):
-        print('{}({}) {:<16}{} ({})'.format(
-            '->' if i == model.selected_choice else '  ',
-            '*' if enabled else ' ',
-            info.name if model.selected_part == model.parts[0] else '{}.{}'.format(
-                model.selected_part, info.name),
-            info.docstring,
-            info.field_type.__name__))
-    print()
-    for i, part in enumerate(model.parts):
-        print('{}({}) {} edit {} message'.format(
-            '->' if i == model.selected_choice - len(model.toggles) else '  ',
-            '*' if part == model.selected_part else ' ',
-            '[Tab]' if i == (model.selected_part_index +
-                             1) % len(model.parts) else '     ',
-            part))
-    print()
-    for i, (_, name, extension) in enumerate(model.generators):
-        print('{}({}) {}: {}{}'.format(
-            '->' if i == model.selected_choice -
-            len(model.toggles) - len(model.parts) else '  ',
-            '*' if model.enabled_gens[i] else ' ',
-            name,
-            model.output,
-            extension))
-
-    print('\n{}[o]utput file: {}'.format(
-        '->' if model.selected_choice == model.choices_num - 3 else '  ',
-        model.output + ('█' if model.editing_output else '')))
-    gen_count = model.enabled_gens.count(True)
-    field_count = sum([model.enabled[p].count(True) for p in model.parts])
-    print('{}[g]enerate with {} generator{} for {} field{}'.format(
-        '->' if model.selected_choice == model.choices_num - 2 else '  ',
-        gen_count, '' if gen_count == 1 else 's',
-        field_count, '' if field_count == 1 else 's',
-    ))
-    print('{}[q]uit'.format(
-        '->' if model.selected_choice == model.choices_num - 1 else '  '))
-
-    print('\n{}'.format(model.status))
-    if model.verbose:
-        print('last key pressed {}'.format(model.last_key))
-
-
-def update(model: Model, message: Message, data: Any) -> Tuple[Model, List[Command]]:
-    commands = []
-    if message == Message.KEY:
-        key: int = data
-        model.last_key = key
-
-        if model.editing_output:
-            model = update_output(model, key)
-        else:
-            model, cs = update_menu(model, key)
-            commands.extend(cs)
-
-    elif message == Message.STATUS:
-        status: str = data
-        model.status = status
-
-    return model, commands
-
-
-def update_output(model: Model, key: int) -> Model:
-    if key >= 32 and key <= 126:  # printable ASCII characters
-        model.output += chr(key)
-    elif key in [8, 127]:  # Backspace (Win, Linux)
-        model.output = model.output[:-1]
-    elif key == 13:  # Enter
-        if model.output == '':
-            model.status = 'Empty output filename!'
-        else:
-            model.editing_output = False
-            model.status = ''
-    elif key == 27:  # Esc
-        model.output = model.previous_output
-        model.editing_output = False
-        model.status = 'Edit cancelled'
-    return model
-
-
-def update_menu(model: Model, key: int) -> Tuple[Model, List[Command]]:
-    commands = []
-    if key in [ord('o'), ord('O')]:
-        model.selected_choice = model.choices_num - 3
-        model.previous_output = model.output
-        model.editing_output = True
-    elif key in [ord('g'), ord('G')]:
-        model.selected_choice = model.choices_num - 2
-        commands.append(Command.MAKE)
-    elif key in [ord('q'), ord('Q'), 3]:  # Ctrl+C
-        commands.append(Command.QUIT)
-    elif key in [ord('j'), ord('J'), 66, 80]:  # Linux down, Win down
-        model.selected_choice = (
-            model.selected_choice + 1) % model.choices_num
-    elif key in [ord('k'), ord('K'), 65, 72]:  # Linux up, Win up
-        model.selected_choice = (
-            model.selected_choice - 1) % model.choices_num
-    elif key == 9:  # Tab
-        model.selected_part = model.parts[(
-            model.selected_part_index + 1) % len(model.parts)]
-
-    elif key in [13, 32]:  # Enter, Space
-        i = model.selected_choice
-        if 0 <= i < len(model.toggles):
-            model.enabled[model.selected_part][i] = not model.enabled[model.selected_part][i]
-        i -= len(model.toggles)
-
-        if 0 <= i < len(model.parts):
-            model.selected_part = model.parts[i]
-        i -= len(model.parts)
-
-        if 0 <= i < len(model.generators):
-            model.enabled_gens[i] = not model.enabled_gens[i]
-        i -= len(model.generators)
-
-        if model.selected_choice == model.choices_num - 3:
-            model.previous_output = model.output
-            model.editing_output = True
-        elif model.selected_choice == model.choices_num - 2:
-            commands.append(Command.MAKE)
-        elif model.selected_choice == model.choices_num - 1:
-            commands.append(Command.QUIT)
-
-    return model, commands
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description='generate MATLAB function to pack data for lidia',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-v', '--verbose', action='store_true', dest='verbose',
-                        help='increase amount of shown information')
-    parser.add_argument('-o', '--output', default='pack_lidia',
-                        help='output file path')
-    args = parser.parse_args()
-
-    model = Model(os.path.normpath(args.output), args.verbose)
-    messages = []
-    while True:
-        commands = []
-        for msg, data in messages:
-            mdl, c = update(model, msg, data)
-            model = mdl
-            commands.extend(c)
-            messages.clear()
-
-        for cmd in commands:
-            if cmd == Command.QUIT:
-                sys.exit(0)
-            if cmd == Command.MAKE:
-                selected = {p: [info.name for info, en in zip(
-                    model.toggles, model.enabled[p]) if en] for p in model.parts}
-                if len(os.path.dirname(model.output)) > 0:
-                    os.makedirs(os.path.dirname(model.output), exist_ok=True)
-                filename = os.path.basename(model.output)
-
-                status = []
-                infos = {
-                    info.name: info for info in FieldInfo.inspect_AircraftData()}
-                for enabled, (gen, name, extension) in zip(model.enabled_gens, model.generators):
-                    if not enabled:
-                        continue
-
-                    out_path = model.output + extension
-                    if gen == Generator.MATLAB:
-                        forbidden_characters = re.findall(
-                            r'[^A-Za-z0-9_]', model.output)
-                        if len(forbidden_characters) > 0:
-                            status.append(
-                                f'Error: characters {set(forbidden_characters)} not allowed in MATLAB function name')
-                        else:
-                            with open(out_path, 'w') as out:
-                                codegen_matlab(out, filename, infos,
-                                               selected['main'], selected['trgt'], selected['trim'])
-                            status.append(
-                                f'Saved {name} generator to {out_path}')
-                    elif gen == Generator.MBDYN:
-                        codegen_mbdyn(model.output, infos,
-                                      selected['main'], selected['trgt'], selected['trim'])
-                        status.append(f'Saved {name} generator to {out_path}')
-                if model.enabled_gens.count(True) == 0:
-                    status.append('No output format enabled')
-                messages.append((Message.STATUS, '\n'.join(status)))
-
-        view(model)
-        if len(messages) > 0:
-            continue
-
-        key = ord(getch())
-        messages.append((Message.KEY, key))
-
-
-MBD_PREFIX = 'LIDIA_'
-
-
-def codegen_mbdyn(output: str, infos: Dict[str, FieldInfo],
-                  main_fields: List[str], trgt_fields: List[str], trim_fields: List[str]) -> None:
-    filename = os.path.basename(output)
-    defines = ['output']
-    for group, prefix in [(main_fields, ''), (trgt_fields, 'trgt_'), (trim_fields, 'trim_')]:
-        for f in group:
-            if issubclass(infos[f].field_type, BaseModel):
-                defines.extend(
-                    f'{prefix}{f}_{a}' for a in infos[f].field_type.__fields__)
-            else:
-                defines.append(f'{prefix}{f}')
-    with open(output + '.set', 'w') as out_set:
-        out_set.write('''##### Generated with pack_maker.py
-# constants definition file
-# include it in your model like this:
-#
-# include: "./{}.set";
-
-### identifiers:
-'''.format(filename))
-
-        next_id = 55000
-        for d in defines:
-            out_set.write('set: const integer {}{} = {};\n'.format(
-                MBD_PREFIX,
-                d.upper(),
-                next_id))
-            next_id += 1
-        out_set.write('''
-# vim:ft=mbd
-''')
-
-    with open(output + '.drv', 'w') as out_drv:
-        out_drv.write('''##### Generated with pack_maker.py
-# drive definition file
-# include it in your model like this:
-#
-# include: "./{}.drv";
-#
-# modify the following drive callers to get relevant data from model
-# example of getting Z-axis position of NODE_CG:
-#
-# drive caller: LIDIA_NED_DOWN, node, NODE_CG, structural, string, "X[3]", direct;
-
-### drive templates:
-'''.format(filename))
-        for d in defines[1:]:  # skip stream id
-            out_drv.write('drive caller: {}{}, const, 0;\n'.format(
-                MBD_PREFIX,
-                d.upper()))
-        out_drv.write('''
-# vim:ft=mbd
-''')
-
-    with open(output + '.elm', 'w') as out_elm:
-        out_elm.write('''##### Generated with pack_maker.py
-# output stream definition
-# include it in your model **inside the elements block** like this:
-#
-# include: "./{}.elm";
-# 
-# you also need to increase the number of output elements in the control data block:
-# begin: control data;
-#     output elements: +1;
-# end: control data;
-
-### output stream definition
-stream output: {}{},
-\tstream name, "Lidia output in SMOL format",
-\tcreate, no,
-\tport, 5100,
-\thost, "127.0.0.1",
-\tsocket type, udp,
-'''.format(filename, MBD_PREFIX, defines[0].upper()))
-
-        values = StringIO()
-        pack_fieldlists(Generator.MBDYN, values, infos,
-                        main_fields, trgt_fields, trim_fields)
-
-        out_elm.write('\tvalues, {},\n'.format(values.getvalue().count('\n')))
-        out_elm.write(values.getvalue())
-        out_elm.write('''
-\tmodifier, copy cast,
-\t\tswap, f, d, i,
-''')  # TODO: verify swapped types
-        type_out = StringIO()
-        pack_fieldlists(Generator.MBDYN_TYPE, type_out, infos,
-                        main_fields, trgt_fields, trim_fields)
-        out_elm.write(type_out.getvalue()[:-2]) # strip ending ',\n'
-        out_elm.write('''
-\t;
-
-# vim:ft=mbd
-''')
-
-
-def codegen_matlab(out: TextIOBase, function_name: str, infos: Dict[str, FieldInfo],
-                   main_fields: List[str], trgt_fields: List[str], trim_fields: List[str]) -> None:
-    out.write('function data = {}( ...\n    '.format(function_name))
-    arglist = []
-    for f in main_fields:
-        if issubclass(infos[f].field_type, BaseModel):
-            arglist.extend('{}_{}'.format(f, a)
-                           for a in infos[f].field_type.__fields__)
-        else:
-            arglist.append(f)
-    for f in trgt_fields:
-        if issubclass(infos[f].field_type, BaseModel):
-            arglist.extend('trgt_{}_{}'.format(f, a)
-                           for a in infos[f].field_type.__fields__)
-        else:
-            arglist.append('trgt_{}'.format(f))
-    for f in trim_fields:
-        if issubclass(infos[f].field_type, BaseModel):
-            arglist.extend('trim_{}_{}'.format(f, a)
-                           for a in infos[f].field_type.__fields__)
-        else:
-            arglist.append('trim_{}'.format(f))
-
-    out.write(', ...\n    '.join(arglist))
-    out.write(''') % {} arguments
-%PACK_LIDIA Pack aircraft data into binary format
-%   The output is array of bytes in MsgPack format, as expected by
-%   'smol' source of lidia package
-%
-%   This is generated using pack_maker.py to create code suitable for
-%   use in Simulink - known size of I/O (see below), no map or struct usage
-%
-%   Arguments:
-'''.format(len(arglist)))
-    for fieldgroup, arg_prefix, doc_prefix in [(main_fields, '', ''), (trgt_fields, 'trgt_', 'TARGET '), (trim_fields, 'trim_', 'TRIM ')]:
-        for f in fieldgroup:
-            out.write('%       {}{}: {}{}\n'.format(
-                arg_prefix, f, doc_prefix, infos[f].docstring))
-    out.write('''
-    data = uint8([...
-''')
-    length = pack_fieldlists(Generator.MATLAB, out,
-                             infos, main_fields, trgt_fields, trim_fields)
-
-    out.write('''    ]);
-% data length {0} bytes
-end
-
-% You might need to manually configure Simulink output:
-%   Size: 1 {0}
-%   Type: uint8
-% The warning message "Wrap on overflow detected" can be ignored
-
-function bytes = b(value)
-    % reverse byte order to convert from little endian to big endian
-    bytes = typecast(swapbytes(value), 'uint8');
-end
-'''.format(length))
-
-
-def pack_fieldlists(gen: Generator, out: TextIOBase, infos: Dict[str, FieldInfo], main_fields, trgt_fields, trim_fields) -> int:
-    length = 0
-
-    field_count = len(main_fields) + \
-        (1 if len(trgt_fields) > 0 else 0) + \
-        (1 if len(trim_fields) > 0 else 0)
-    length += pack_map(gen, out, field_count)
-
-    for function_name in main_fields:
-        length += pack_field(gen, out, infos[function_name], '')
-
-    for fieldgroup, prefix in [(trgt_fields, 'trgt'), (trim_fields, 'trim')]:
-        if len(fieldgroup) > 0:
-            length += pack_str(gen, out, prefix)
-            length += pack_map(gen, out, len(fieldgroup))
-            for function_name in fieldgroup:
-                length += pack_field(gen, out, infos[function_name], prefix)
-    return length
-
-
-def pack_field(gen: Generator, out: TextIOBase, info: FieldInfo, prefix: str) -> int:
-    length = 0
-    length += pack_str(gen, out, info.name)
-    if issubclass(info.field_type, VectorModel):
-        length += pack_vector(gen, out, info.name, info.field_type, prefix)
-    elif info.field_type is int:
-        length += pack_int(gen, out, info.name if len(prefix) ==
-                           0 else '{}_{}'.format(prefix, info.name))
-    else:
-        raise NotImplementedError(
-            'No code generation for class:', info.field_type)
-    return length
-
-
-def pack_vector(gen: Generator, out: TextIOBase, name: str, cls: Type[VectorModel], prefix: str) -> int:
-    length = 0
-    length += pack_array(gen, out, len(cls.__fields__))
-    for inner in cls.__fields__:
-        length += pack_float(gen, out, '{}{}_{}'.format(
-            '' if len(prefix) == 0 else (prefix + '_'),
-            name, inner), double=(name == 'ned'))  # special case for positional accuracy
-    return length
-
-
-def pack_map(gen: Generator, out: TextIOBase, count: int) -> int:
-    if count > 15:
-        raise NotImplementedError('only fixmap handled for now')
-    if gen == Generator.MATLAB:
-        out.write(
-            '        0x8{:x}, ... % map length {}\n'.format(count, count))
-    elif gen == Generator.MBDYN:
-        val = 0x80 + count
-        out.write(
-            f'\tdrive, const, {val},\t# 0x{val:02X} map length {count}\n')
-    elif gen == Generator.MBDYN_TYPE:
-        out.write('\t\tuint8_t,\n')
-    return 1
-
-
-def pack_array(gen: Generator, out: TextIOBase, count: int) -> int:
-    if count > 15:
-        raise NotImplementedError('only fixarray handled for now')
-    if gen == Generator.MATLAB:
-        out.write(
-            '        0x9{:x}, ... % array length {}\n'.format(count, count))
-    elif gen == Generator.MBDYN:
-        val = 0x90 + count
-        out.write(
-            f'\tdrive, const, {val},\t# 0x{val:02X} array length {count}\n')
-    elif gen == Generator.MBDYN_TYPE:
-        out.write('\t\tuint8_t,\n')
-
-    return 1
-
-
-def pack_str(gen: Generator, out: TextIOBase, data: str) -> int:
-    if len(data) > 31:
-        raise NotImplementedError('only fixstr handled for now')
-    if gen == Generator.MATLAB:
-        out.write("        0x{:x}, '{}', ... % string length {}\n".format(
-            0b10100000 + len(data), data, len(data)))
-    elif gen == Generator.MBDYN:
-        val = 0b10100000 + len(data)
-        out.write(
-            f'\tdrive, const, {val},\t# 0x{val:02X} string length {len(data)}\n')
-        for c in data:
-            out.write(f"\tdrive, const, {ord(c)},\t# '{c}'\n")
-    elif gen == Generator.MBDYN_TYPE:
-        for _ in range(len(data) + 1):
-            out.write('\t\tuint8_t,\n')
-    return 1 + len(data)
-
-
-def pack_float(gen: Generator, out: TextIOBase, name: str, double=False) -> int:
-    if gen == Generator.MATLAB:
-        out.write('        0xc{}, b({}({})), ... % {}\n'.format(
-            'b' if double else 'a',
-            'double' if double else 'single',
-            name,
-            'double' if double else 'float',
-        ))
-    elif gen == Generator.MBDYN:
-        val = 0xCB if double else 0xCA
-        out.write('\tdrive, const, {},\t# 0x{:02X} {}\n'.format(
-            val, val, 'double' if double else 'float'
-        ))
-        out.write(f'\tdrive, reference, {MBD_PREFIX}{name.upper()},\n')
-    elif gen == Generator.MBDYN_TYPE:
-        out.write('\t\tuint8_t,\n')
-        out.write(f'\t\t{"double" if double else "float"},\n')
-    return 9 if double else 5
-
-
-def pack_int(gen: Generator, out: TextIOBase, name: str) -> int:
-    if gen == Generator.MATLAB:
-        out.write(
-            '        0xce, b(uint32({})), ... % 32-bit unsigned integer\n'.format(name))
-    elif gen == Generator.MBDYN:
-        val = 0xCE
-        out.write(f'\tdrive, const, {val},\t# 0x{val:02X} uint32_t\n')
-        out.write(f'\tdrive, reference, {MBD_PREFIX}{name.upper()},\n')
-    elif gen == Generator.MBDYN_TYPE:
-        out.write('\t\tuint8_t,\n')
-        out.write('\t\tuint32_t,\n')
-    return 5
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+from enum import auto, IntEnum
+import inspect
+from io import StringIO, TextIOBase
+import os
+import platform
+from pydantic import BaseModel
+import re
+import sys
+from typing import Any, Dict, List, Tuple, Type
+
+# setup cross-platform getch() and clear()
+if platform.system() == "Windows":
+    import msvcrt
+
+    def getch():
+        return msvcrt.getwch()
+
+    def clear():
+        os.system('cls')
+else:
+    import tty
+    import termios
+
+    def getch():
+        fd = sys.stdin.fileno()
+        old_settings = termios.tcgetattr(fd)
+        try:
+            tty.setraw(sys.stdin.fileno())
+            ch = sys.stdin.read(1)
+        finally:
+            termios.tcsetattr(fd, termios.TCSADRAIN, old_settings)
+        return ch
+
+    def clear():
+        os.system('clear')
+
+this_path = os.path.dirname(os.path.realpath(__file__))
+lidia_path = os.path.join(this_path, '..', '..')
+sys.path.append(lidia_path)
+from lidia.aircraft import AircraftData, VectorModel  # noqa prevent moving to top of file
+
+
+class FieldInfo(BaseModel):
+    """Details of a `AircraftData` field"""
+
+    name: str
+    """Field name"""
+    docstring: str
+    """Field docstring"""
+    field_type: Type
+    """Contained type"""
+
+    @staticmethod
+    def inspect_AircraftData() -> List['FieldInfo']:
+        infos = []
+        pattern = re.compile(
+            r'^[ \t]+([a-z_]+): Optional\[(?:[A-Za-z]+)\] = None\n[ \t]+"""([^"]+)"""$', flags=re.MULTILINE)
+        for name, doc in re.findall(pattern, inspect.getsource(AircraftData)):
+            field = AircraftData.__fields__[name]
+            infos.append(FieldInfo(
+                name=name,
+                docstring=doc,
+                field_type=field.annotation.__args__[
+                    0],  # annotation type Optional
+            ))
+
+        return infos
+
+
+class Generator(IntEnum):
+    MATLAB = auto()
+    MBDYN = auto()
+    MBDYN_TYPE = auto()
+
+
+class Model:
+    def __init__(self, output: str, verbose=False):
+        self.output = output
+        self.editing_output = False
+        self.previous_output = ''
+        self.verbose = verbose
+        self.last_key = 0
+
+        self.parts = ['main', 'trgt', 'trim']
+        self.selected_part = self.parts[0]
+
+        # only serialization of vectors is supported
+        self.toggles = [info for info in FieldInfo.inspect_AircraftData()
+                        if (issubclass(info.field_type, VectorModel) or info.field_type is int)]
+        self.enabled = {part: ([False] * len(self.toggles))
+                        for part in self.parts}
+
+        self.generators = [
+            (Generator.MATLAB, 'MATLAB', '.m'),
+            (Generator.MBDYN, 'MBDyn', '{.set, .drv, .elm}'),
+        ]
+        self.enabled_gens = [False] * len(self.generators)
+
+        self.extra_choices = 3
+        self.selected_choice = 0
+
+        self.status = ''
+
+    @property
+    def choices_num(self) -> int:
+        return len(self.toggles) + len(self.parts) + len(self.generators) + self.extra_choices
+
+    @property
+    def selected_part_index(self) -> int:
+        return next(i for i, p in enumerate(self.parts) if p == self.selected_part)
+
+    @property
+    def enabled_num(self) -> int:
+        return sum(len([en for en in self.enabled[p] if en]) for p in self.parts)
+
+
+class Command(IntEnum):
+    QUIT = auto()
+    MAKE = auto()
+
+
+class Message(IntEnum):
+    KEY = auto()
+    STATUS = auto()
+
+
+def view(model: Model) -> None:
+    clear()
+    if model.editing_output:
+        print('Edit output filename')
+        print('Confirm editing with Enter, cancel with Esc\n')
+    else:
+        print('Choose fields to be serialized in message')
+        print('Use arrows or j, k to move, select with Enter or Space\n')
+
+    for i, (info, enabled) in enumerate(zip(model.toggles, model.enabled[model.selected_part])):
+        print('{}({}) {:<16}{} ({})'.format(
+            '->' if i == model.selected_choice else '  ',
+            '*' if enabled else ' ',
+            info.name if model.selected_part == model.parts[0] else '{}.{}'.format(
+                model.selected_part, info.name),
+            info.docstring,
+            info.field_type.__name__))
+    print()
+    for i, part in enumerate(model.parts):
+        print('{}({}) {} edit {} message'.format(
+            '->' if i == model.selected_choice - len(model.toggles) else '  ',
+            '*' if part == model.selected_part else ' ',
+            '[Tab]' if i == (model.selected_part_index +
+                             1) % len(model.parts) else '     ',
+            part))
+    print()
+    for i, (_, name, extension) in enumerate(model.generators):
+        print('{}({}) {}: {}{}'.format(
+            '->' if i == model.selected_choice -
+            len(model.toggles) - len(model.parts) else '  ',
+            '*' if model.enabled_gens[i] else ' ',
+            name,
+            model.output,
+            extension))
+
+    print('\n{}[o]utput file: {}'.format(
+        '->' if model.selected_choice == model.choices_num - 3 else '  ',
+        model.output + ('█' if model.editing_output else '')))
+    gen_count = model.enabled_gens.count(True)
+    field_count = sum([model.enabled[p].count(True) for p in model.parts])
+    print('{}[g]enerate with {} generator{} for {} field{}'.format(
+        '->' if model.selected_choice == model.choices_num - 2 else '  ',
+        gen_count, '' if gen_count == 1 else 's',
+        field_count, '' if field_count == 1 else 's',
+    ))
+    print('{}[q]uit'.format(
+        '->' if model.selected_choice == model.choices_num - 1 else '  '))
+
+    print('\n{}'.format(model.status))
+    if model.verbose:
+        print('last key pressed {}'.format(model.last_key))
+
+
+def update(model: Model, message: Message, data: Any) -> Tuple[Model, List[Command]]:
+    commands = []
+    if message == Message.KEY:
+        key: int = data
+        model.last_key = key
+
+        if model.editing_output:
+            model = update_output(model, key)
+        else:
+            model, cs = update_menu(model, key)
+            commands.extend(cs)
+
+    elif message == Message.STATUS:
+        status: str = data
+        model.status = status
+
+    return model, commands
+
+
+def update_output(model: Model, key: int) -> Model:
+    if key >= 32 and key <= 126:  # printable ASCII characters
+        model.output += chr(key)
+    elif key in [8, 127]:  # Backspace (Win, Linux)
+        model.output = model.output[:-1]
+    elif key == 13:  # Enter
+        if model.output == '':
+            model.status = 'Empty output filename!'
+        else:
+            model.editing_output = False
+            model.status = ''
+    elif key == 27:  # Esc
+        model.output = model.previous_output
+        model.editing_output = False
+        model.status = 'Edit cancelled'
+    return model
+
+
+def update_menu(model: Model, key: int) -> Tuple[Model, List[Command]]:
+    commands = []
+    if key in [ord('o'), ord('O')]:
+        model.selected_choice = model.choices_num - 3
+        model.previous_output = model.output
+        model.editing_output = True
+    elif key in [ord('g'), ord('G')]:
+        model.selected_choice = model.choices_num - 2
+        commands.append(Command.MAKE)
+    elif key in [ord('q'), ord('Q'), 3]:  # Ctrl+C
+        commands.append(Command.QUIT)
+    elif key in [ord('j'), ord('J'), 66, 80]:  # Linux down, Win down
+        model.selected_choice = (
+            model.selected_choice + 1) % model.choices_num
+    elif key in [ord('k'), ord('K'), 65, 72]:  # Linux up, Win up
+        model.selected_choice = (
+            model.selected_choice - 1) % model.choices_num
+    elif key == 9:  # Tab
+        model.selected_part = model.parts[(
+            model.selected_part_index + 1) % len(model.parts)]
+
+    elif key in [13, 32]:  # Enter, Space
+        i = model.selected_choice
+        if 0 <= i < len(model.toggles):
+            model.enabled[model.selected_part][i] = not model.enabled[model.selected_part][i]
+        i -= len(model.toggles)
+
+        if 0 <= i < len(model.parts):
+            model.selected_part = model.parts[i]
+        i -= len(model.parts)
+
+        if 0 <= i < len(model.generators):
+            model.enabled_gens[i] = not model.enabled_gens[i]
+        i -= len(model.generators)
+
+        if model.selected_choice == model.choices_num - 3:
+            model.previous_output = model.output
+            model.editing_output = True
+        elif model.selected_choice == model.choices_num - 2:
+            commands.append(Command.MAKE)
+        elif model.selected_choice == model.choices_num - 1:
+            commands.append(Command.QUIT)
+
+    return model, commands
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description='generate MATLAB function to pack data for lidia',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('-v', '--verbose', action='store_true', dest='verbose',
+                        help='increase amount of shown information')
+    parser.add_argument('-o', '--output', default='pack_lidia',
+                        help='output file path')
+    args = parser.parse_args()
+
+    model = Model(os.path.normpath(args.output), args.verbose)
+    messages = []
+    while True:
+        commands = []
+        for msg, data in messages:
+            mdl, c = update(model, msg, data)
+            model = mdl
+            commands.extend(c)
+            messages.clear()
+
+        for cmd in commands:
+            if cmd == Command.QUIT:
+                sys.exit(0)
+            if cmd == Command.MAKE:
+                selected = {p: [info.name for info, en in zip(
+                    model.toggles, model.enabled[p]) if en] for p in model.parts}
+                if len(os.path.dirname(model.output)) > 0:
+                    os.makedirs(os.path.dirname(model.output), exist_ok=True)
+                filename = os.path.basename(model.output)
+
+                status = []
+                infos = {
+                    info.name: info for info in FieldInfo.inspect_AircraftData()}
+                for enabled, (gen, name, extension) in zip(model.enabled_gens, model.generators):
+                    if not enabled:
+                        continue
+
+                    out_path = model.output + extension
+                    if gen == Generator.MATLAB:
+                        forbidden_characters = re.findall(
+                            r'[^A-Za-z0-9_]', model.output)
+                        if len(forbidden_characters) > 0:
+                            status.append(
+                                f'Error: characters {set(forbidden_characters)} not allowed in MATLAB function name')
+                        else:
+                            with open(out_path, 'w') as out:
+                                codegen_matlab(out, filename, infos,
+                                               selected['main'], selected['trgt'], selected['trim'])
+                            status.append(
+                                f'Saved {name} generator to {out_path}')
+                    elif gen == Generator.MBDYN:
+                        codegen_mbdyn(model.output, infos,
+                                      selected['main'], selected['trgt'], selected['trim'])
+                        status.append(f'Saved {name} generator to {out_path}')
+                if model.enabled_gens.count(True) == 0:
+                    status.append('No output format enabled')
+                messages.append((Message.STATUS, '\n'.join(status)))
+
+        view(model)
+        if len(messages) > 0:
+            continue
+
+        key = ord(getch())
+        messages.append((Message.KEY, key))
+
+
+MBD_PREFIX = 'LIDIA_'
+
+
+def codegen_mbdyn(output: str, infos: Dict[str, FieldInfo],
+                  main_fields: List[str], trgt_fields: List[str], trim_fields: List[str]) -> None:
+    filename = os.path.basename(output)
+    defines = ['output']
+    for group, prefix in [(main_fields, ''), (trgt_fields, 'trgt_'), (trim_fields, 'trim_')]:
+        for f in group:
+            if issubclass(infos[f].field_type, BaseModel):
+                defines.extend(
+                    f'{prefix}{f}_{a}' for a in infos[f].field_type.__fields__)
+            else:
+                defines.append(f'{prefix}{f}')
+    with open(output + '.set', 'w') as out_set:
+        out_set.write('''##### Generated with pack_maker.py
+# constants definition file
+# include it in your model like this:
+#
+# include: "./{}.set";
+
+### identifiers:
+'''.format(filename))
+
+        next_id = 55000
+        for d in defines:
+            out_set.write('set: const integer {}{} = {};\n'.format(
+                MBD_PREFIX,
+                d.upper(),
+                next_id))
+            next_id += 1
+        out_set.write('''
+# vim:ft=mbd
+''')
+
+    with open(output + '.drv', 'w') as out_drv:
+        out_drv.write('''##### Generated with pack_maker.py
+# drive definition file
+# include it in your model like this:
+#
+# include: "./{}.drv";
+#
+# modify the following drive callers to get relevant data from model
+# example of getting Z-axis position of NODE_CG:
+#
+# drive caller: LIDIA_NED_DOWN, node, NODE_CG, structural, string, "X[3]", direct;
+
+### drive templates:
+'''.format(filename))
+        for d in defines[1:]:  # skip stream id
+            out_drv.write('drive caller: {}{}, const, 0;\n'.format(
+                MBD_PREFIX,
+                d.upper()))
+        out_drv.write('''
+# vim:ft=mbd
+''')
+
+    with open(output + '.elm', 'w') as out_elm:
+        out_elm.write('''##### Generated with pack_maker.py
+# output stream definition
+# include it in your model **inside the elements block** like this:
+#
+# include: "./{}.elm";
+# 
+# you also need to increase the number of output elements in the control data block:
+# begin: control data;
+#     output elements: +1;
+# end: control data;
+
+### output stream definition
+stream output: {}{},
+\tstream name, "Lidia output in SMOL format",
+\tcreate, no,
+\tport, 5100,
+\thost, "127.0.0.1",
+\tsocket type, udp,
+'''.format(filename, MBD_PREFIX, defines[0].upper()))
+
+        values = StringIO()
+        pack_fieldlists(Generator.MBDYN, values, infos,
+                        main_fields, trgt_fields, trim_fields)
+
+        out_elm.write('\tvalues, {},\n'.format(values.getvalue().count('\n')))
+        out_elm.write(values.getvalue())
+        out_elm.write('''
+\tmodifier, copy cast,
+\t\tswap, f, d, i,
+''')  # TODO: verify swapped types
+        type_out = StringIO()
+        pack_fieldlists(Generator.MBDYN_TYPE, type_out, infos,
+                        main_fields, trgt_fields, trim_fields)
+        out_elm.write(type_out.getvalue()[:-2]) # strip ending ',\n'
+        out_elm.write('''
+\t;
+
+# vim:ft=mbd
+''')
+
+
+def codegen_matlab(out: TextIOBase, function_name: str, infos: Dict[str, FieldInfo],
+                   main_fields: List[str], trgt_fields: List[str], trim_fields: List[str]) -> None:
+    out.write('function data = {}( ...\n    '.format(function_name))
+    arglist = []
+    for f in main_fields:
+        if issubclass(infos[f].field_type, BaseModel):
+            arglist.extend('{}_{}'.format(f, a)
+                           for a in infos[f].field_type.__fields__)
+        else:
+            arglist.append(f)
+    for f in trgt_fields:
+        if issubclass(infos[f].field_type, BaseModel):
+            arglist.extend('trgt_{}_{}'.format(f, a)
+                           for a in infos[f].field_type.__fields__)
+        else:
+            arglist.append('trgt_{}'.format(f))
+    for f in trim_fields:
+        if issubclass(infos[f].field_type, BaseModel):
+            arglist.extend('trim_{}_{}'.format(f, a)
+                           for a in infos[f].field_type.__fields__)
+        else:
+            arglist.append('trim_{}'.format(f))
+
+    out.write(', ...\n    '.join(arglist))
+    out.write(''') % {} arguments
+%PACK_LIDIA Pack aircraft data into binary format
+%   The output is array of bytes in MsgPack format, as expected by
+%   'smol' source of lidia package
+%
+%   This is generated using pack_maker.py to create code suitable for
+%   use in Simulink - known size of I/O (see below), no map or struct usage
+%
+%   Arguments:
+'''.format(len(arglist)))
+    for fieldgroup, arg_prefix, doc_prefix in [(main_fields, '', ''), (trgt_fields, 'trgt_', 'TARGET '), (trim_fields, 'trim_', 'TRIM ')]:
+        for f in fieldgroup:
+            out.write('%       {}{}: {}{}\n'.format(
+                arg_prefix, f, doc_prefix, infos[f].docstring))
+    out.write('''
+    data = uint8([...
+''')
+    length = pack_fieldlists(Generator.MATLAB, out,
+                             infos, main_fields, trgt_fields, trim_fields)
+
+    out.write('''    ]);
+% data length {0} bytes
+end
+
+% You might need to manually configure Simulink output:
+%   Size: 1 {0}
+%   Type: uint8
+% The warning message "Wrap on overflow detected" can be ignored
+
+function bytes = b(value)
+    % reverse byte order to convert from little endian to big endian
+    bytes = typecast(swapbytes(value), 'uint8');
+end
+'''.format(length))
+
+
+def pack_fieldlists(gen: Generator, out: TextIOBase, infos: Dict[str, FieldInfo], main_fields, trgt_fields, trim_fields) -> int:
+    length = 0
+
+    field_count = len(main_fields) + \
+        (1 if len(trgt_fields) > 0 else 0) + \
+        (1 if len(trim_fields) > 0 else 0)
+    length += pack_map(gen, out, field_count)
+
+    for function_name in main_fields:
+        length += pack_field(gen, out, infos[function_name], '')
+
+    for fieldgroup, prefix in [(trgt_fields, 'trgt'), (trim_fields, 'trim')]:
+        if len(fieldgroup) > 0:
+            length += pack_str(gen, out, prefix)
+            length += pack_map(gen, out, len(fieldgroup))
+            for function_name in fieldgroup:
+                length += pack_field(gen, out, infos[function_name], prefix)
+    return length
+
+
+def pack_field(gen: Generator, out: TextIOBase, info: FieldInfo, prefix: str) -> int:
+    length = 0
+    length += pack_str(gen, out, info.name)
+    if issubclass(info.field_type, VectorModel):
+        length += pack_vector(gen, out, info.name, info.field_type, prefix)
+    elif info.field_type is int:
+        length += pack_int(gen, out, info.name if len(prefix) ==
+                           0 else '{}_{}'.format(prefix, info.name))
+    else:
+        raise NotImplementedError(
+            'No code generation for class:', info.field_type)
+    return length
+
+
+def pack_vector(gen: Generator, out: TextIOBase, name: str, cls: Type[VectorModel], prefix: str) -> int:
+    length = 0
+    length += pack_array(gen, out, len(cls.__fields__))
+    for inner in cls.__fields__:
+        length += pack_float(gen, out, '{}{}_{}'.format(
+            '' if len(prefix) == 0 else (prefix + '_'),
+            name, inner), double=(name == 'ned'))  # special case for positional accuracy
+    return length
+
+
+def pack_map(gen: Generator, out: TextIOBase, count: int) -> int:
+    if count > 15:
+        raise NotImplementedError('only fixmap handled for now')
+    if gen == Generator.MATLAB:
+        out.write(
+            '        0x8{:x}, ... % map length {}\n'.format(count, count))
+    elif gen == Generator.MBDYN:
+        val = 0x80 + count
+        out.write(
+            f'\tdrive, const, {val},\t# 0x{val:02X} map length {count}\n')
+    elif gen == Generator.MBDYN_TYPE:
+        out.write('\t\tuint8_t,\n')
+    return 1
+
+
+def pack_array(gen: Generator, out: TextIOBase, count: int) -> int:
+    if count > 15:
+        raise NotImplementedError('only fixarray handled for now')
+    if gen == Generator.MATLAB:
+        out.write(
+            '        0x9{:x}, ... % array length {}\n'.format(count, count))
+    elif gen == Generator.MBDYN:
+        val = 0x90 + count
+        out.write(
+            f'\tdrive, const, {val},\t# 0x{val:02X} array length {count}\n')
+    elif gen == Generator.MBDYN_TYPE:
+        out.write('\t\tuint8_t,\n')
+
+    return 1
+
+
+def pack_str(gen: Generator, out: TextIOBase, data: str) -> int:
+    if len(data) > 31:
+        raise NotImplementedError('only fixstr handled for now')
+    if gen == Generator.MATLAB:
+        out.write("        0x{:x}, '{}', ... % string length {}\n".format(
+            0b10100000 + len(data), data, len(data)))
+    elif gen == Generator.MBDYN:
+        val = 0b10100000 + len(data)
+        out.write(
+            f'\tdrive, const, {val},\t# 0x{val:02X} string length {len(data)}\n')
+        for c in data:
+            out.write(f"\tdrive, const, {ord(c)},\t# '{c}'\n")
+    elif gen == Generator.MBDYN_TYPE:
+        for _ in range(len(data) + 1):
+            out.write('\t\tuint8_t,\n')
+    return 1 + len(data)
+
+
+def pack_float(gen: Generator, out: TextIOBase, name: str, double=False) -> int:
+    if gen == Generator.MATLAB:
+        out.write('        0xc{}, b({}({})), ... % {}\n'.format(
+            'b' if double else 'a',
+            'double' if double else 'single',
+            name,
+            'double' if double else 'float',
+        ))
+    elif gen == Generator.MBDYN:
+        val = 0xCB if double else 0xCA
+        out.write('\tdrive, const, {},\t# 0x{:02X} {}\n'.format(
+            val, val, 'double' if double else 'float'
+        ))
+        out.write(f'\tdrive, reference, {MBD_PREFIX}{name.upper()},\n')
+    elif gen == Generator.MBDYN_TYPE:
+        out.write('\t\tuint8_t,\n')
+        out.write(f'\t\t{"double" if double else "float"},\n')
+    return 9 if double else 5
+
+
+def pack_int(gen: Generator, out: TextIOBase, name: str) -> int:
+    if gen == Generator.MATLAB:
+        out.write(
+            '        0xce, b(uint32({})), ... % 32-bit unsigned integer\n'.format(name))
+    elif gen == Generator.MBDYN:
+        val = 0xCE
+        out.write(f'\tdrive, const, {val},\t# 0x{val:02X} uint32_t\n')
+        out.write(f'\tdrive, reference, {MBD_PREFIX}{name.upper()},\n')
+    elif gen == Generator.MBDYN_TYPE:
+        out.write('\t\tuint8_t,\n')
+        out.write('\t\tuint32_t,\n')
+    return 5
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `lidia-0.8.0/src/lidia.egg-info/PKG-INFO` & `lidia-0.8.1/src/lidia.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-Metadata-Version: 2.1
-Name: lidia
-Version: 0.8.0
-Summary: serve an aircraft instruments panel as a web page
-Home-page: https://gitlab.com/Maarrk/lidia
-Author: Marek S. Lukasiewicz
-Author-email: marek@lukasiewicz.tech
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Lidia
-
-![lidia](https://img.shields.io/pypi/v/lidia)
-
-_Lightweight Instrument Display Interface for Aircraft_
-
-lidia is a Python package for serving an aircraft instruments panel as a web page.
-
-![screenshot of top part of primary flight display page](https://gitlab.com/Maarrk/lidia/-/raw/main/readme-pfd.png)
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [lidia](https://pypi.org/project/lidia/).
-
-```bash
-pip install lidia
-```
-
-## Usage
-
-```bash
-lidia demo
-
-# if your Scripts folder isn't in Path:
-python3 -m lidia demo
-
-# use other source
-lidia rpctask
-
-# show general help
-lidia --help
-
-# show help for a specific source
-lidia demo --help
-
-# pass the main server arguments before the source name
-lidia -P 5556 demo
-```
-
-Then open the served page in a browser, by default [localhost:5555](http://localhost:5555).
-The controls for showing and hiding elements of the GUI are shown when hovering the mouse in the bottom left region of the page.
-
-## Support
-
-Report problems in [GitLab Issues](https://gitlab.com/Maarrk/lidia/-/issues)
-
-## Roadmap
-
-- Additional PFD indicators: ILS, VOR on HSI
-- Ship approach screen with views from the side and behind
-- CAS (Crew Alerting System) screen
-- Simple second order aircraft models
-- USB HID joystick source
-
-## Contributing
-
-- Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
-- Python code should be formatted with autopep8
-- Other source files should be formatted with Prettier
-- Install packages for development with `pip install -r requirements.txt`
-- To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
-
-## Acknowledgements
-
-This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
-
-Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: lidia
+Version: 0.8.1
+Summary: serve an aircraft instruments panel as a web page
+Home-page: https://gitlab.com/Maarrk/lidia
+Author: Marek S. Lukasiewicz
+Author-email: marek@lukasiewicz.tech
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Lidia
+
+![lidia](https://img.shields.io/pypi/v/lidia)
+
+_Lightweight Instrument Display Interface for Aircraft_
+
+lidia is a Python package for serving an aircraft instruments panel as a web page.
+
+![screenshot of top part of primary flight display page](https://gitlab.com/Maarrk/lidia/-/raw/main/readme-pfd.png)
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [lidia](https://pypi.org/project/lidia/).
+
+```bash
+pip install lidia
+```
+
+## Usage
+
+```bash
+lidia demo
+
+# if your Scripts folder isn't in Path:
+python3 -m lidia demo
+
+# use other source
+lidia rpctask
+
+# show general help
+lidia --help
+
+# show help for a specific source
+lidia demo --help
+
+# pass the main server arguments before the source name
+lidia -P 5556 demo
+```
+
+Then open the served page in a browser, by default [localhost:5555](http://localhost:5555).
+The controls for showing and hiding elements of the GUI are shown when hovering the mouse in the bottom left region of the page.
+
+## Support
+
+Report problems in [GitLab Issues](https://gitlab.com/Maarrk/lidia/-/issues)
+
+## Roadmap
+
+- Additional PFD indicators: ILS, VOR on HSI
+- Ship approach screen with views from the side and behind
+- CAS (Crew Alerting System) screen
+- Simple second order aircraft models
+- USB HID joystick source
+
+## Contributing
+
+- Contributions should be made to the [GitLab repository](https://gitlab.com/Maarrk/lidia)
+- Python code should be formatted with autopep8
+- Other source files should be formatted with Prettier
+- Install packages for development with `pip install -r requirements.txt`
+- To properly run as a module without building and installing, **cd into `src/`** and run `python3 -m lidia`
+
+## Acknowledgements
+
+This software was developed in [Department of Aerospace Science and Technology](https://www.aero.polimi.it/) of Politecnico di Milano.
+
+Instrument graphics designed by Davide Marchesoli and Qiuyang Xia.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `lidia-0.8.0/src/lidia.egg-info/SOURCES.txt` & `lidia-0.8.1/src/lidia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

