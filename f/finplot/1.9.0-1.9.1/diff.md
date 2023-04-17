# Comparing `tmp/finplot-1.9.0.tar.gz` & `tmp/finplot-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\finplot-1.9.0.tar", last modified: Mon Nov 28 18:12:43 2022, max compression
+gzip compressed data, was "finplot-1.9.1.tar", last modified: Mon Apr 17 09:39:10 2023, max compression
```

## Comparing `finplot-1.9.0.tar` & `finplot-1.9.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 18:12:43.003087 finplot-1.9.0/
--rw-rw-rw-   0        0        0     3786 2022-11-28 18:12:43.002086 finplot-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2783 2021-05-22 08:27:11.000000 finplot-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 18:12:42.997119 finplot-1.9.0/finplot/
--rw-rw-rw-   0        0        0   110318 2022-11-28 03:09:04.000000 finplot-1.9.0/finplot/__init__.py
--rw-rw-rw-   0        0        0     1929 2022-09-01 21:08:58.000000 finplot-1.9.0/finplot/pdplot.py
-drwxrwxrwx   0        0        0        0 2022-11-28 18:12:43.001095 finplot-1.9.0/finplot.egg-info/
--rw-rw-rw-   0        0        0     3786 2022-11-28 18:12:41.000000 finplot-1.9.0/finplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2022-11-28 18:12:42.000000 finplot-1.9.0/finplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 18:12:41.000000 finplot-1.9.0/finplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2022-11-28 18:12:41.000000 finplot-1.9.0/finplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-28 18:12:41.000000 finplot-1.9.0/finplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-28 18:12:43.003087 finplot-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0      750 2022-11-28 18:11:32.000000 finplot-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:39:10.033070 finplot-1.9.1/
+-rw-rw-rw-   0        0        0     1092 2018-08-22 23:30:28.000000 finplot-1.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3195 2023-04-17 09:39:10.032101 finplot-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2783 2021-05-22 08:27:11.000000 finplot-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:39:10.028070 finplot-1.9.1/finplot/
+-rw-rw-rw-   0        0        0   115518 2023-04-03 18:21:46.000000 finplot-1.9.1/finplot/__init__.py
+-rw-rw-rw-   0        0        0     1992 2023-02-11 18:57:39.000000 finplot-1.9.1/finplot/live.py
+-rw-rw-rw-   0        0        0     1929 2022-09-01 21:08:58.000000 finplot-1.9.1/finplot/pdplot.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:39:10.031083 finplot-1.9.1/finplot.egg-info/
+-rw-rw-rw-   0        0        0     3195 2023-04-17 09:39:09.000000 finplot-1.9.1/finplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-17 09:39:09.000000 finplot-1.9.1/finplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:39:09.000000 finplot-1.9.1/finplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-04-17 09:39:09.000000 finplot-1.9.1/finplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 09:39:09.000000 finplot-1.9.1/finplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:39:10.033070 finplot-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      750 2023-04-17 09:37:32.000000 finplot-1.9.1/setup.py
```

### Comparing `finplot-1.9.0/PKG-INFO` & `finplot-1.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 Metadata-Version: 2.1
 Name: finplot
-Version: 1.9.0
+Version: 1.9.1
 Summary: Finance plotting
 Home-page: https://github.com/highfestiva/finplot
 Author: Jonas Byström
 Author-email: highfestiva@gmail.com
-License: UNKNOWN
-Description: # Finance Plot
-        
-        Finance Plotter, or finplot, is a performant library with a clean api to help you with your backtesting. It's
-        optionated with good defaults, so you can start doing your work without having to setup plots, colors, scales,
-        autoscaling, keybindings, handle panning+vertical zooming (which all non-finance libraries have problems with).
-        And best of all: it can show hundreds of thousands of datapoints without batting an eye.
-        
-        <img src="https://badge.fury.io/py/finplot.svg"/> <img src="https://pepy.tech/badge/finplot/month"/> <img src="https://img.shields.io/badge/License-MIT-yellow.svg"/>
-        
-        
-        ## Features
-        
-        * Great performance compared to mpl_finance, plotly and Bokeh
-        * Clean api
-        * Works with both stocks as well as cryptocurrencies on any time resolution
-        * Show as many charts as you want on the same time axis, zoom on all of them at once
-        * Auto-reload position where you were looking last run
-        * Overlays, fill between, value bands, symbols, labels, legend, volume profile, heatmaps, etc.
-        * Can show real-time updates, including orderbook. Save screenshot.
-        * Comes with a [dozen](https://github.com/highfestiva/finplot/blob/master/finplot/examples) great examples.
-        
-        ![feature1](https://raw.githubusercontent.com/highfestiva/finplot/master/feature1.png)
-        
-        ![feature2](https://raw.githubusercontent.com/highfestiva/finplot/master/feature2.jpg)
-        
-        ![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature3.jpg)
-        
-        ![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature-nuts.jpg)
-        
-        
-        ## What it is not
-        
-        finplot *is not a web app*. It does not help you create an homebrew exchange. It does not work with Jupyter Labs.
-        
-        It is only intended for you to do backtesting in. That is not to say that you can't create a ticker or a trade
-        widget yourself. The library is based on the eminent pyqtgraph, which is fast and flexible, so feel free to hack
-        away if that's what you want.
-        
-        
-        ## Easy installation
-        
-        ```bash
-        $ pip install finplot
-        ```
-        
-        
-        ## Example
-        
-        It's straight-forward to start using. This shows every daily candle of Apple since the 80'ies:
-        
-        ```python
-        import finplot as fplt
-        import yfinance
-        
-        df = yfinance.download('AAPL')
-        fplt.candlestick_ochl(df[['Open', 'Close', 'High', 'Low']])
-        fplt.show()
-        ```
-        
-        For more examples and a bunch of snippets, see the [examples](https://github.com/highfestiva/finplot/blob/master/finplot/examples/)
-        directory or the [wiki](https://github.com/highfestiva/finplot/wiki). There you'll find how to plot MACD, Parabolic SAR, RSI,
-        volume profile and much more.
-        
-        
-        ## Coffee
-        
-        For future support and features, consider a small donation.
-        
-        BTC: bc1qk8m8yh86l2pz4eypflchr0tkn5aeud6cmt426m
-        
-        ETH: 0x684d7d4C52ed428AE9a36B2407ba909D896cDB67
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Finance Plot
+
+Finance Plotter, or finplot, is a performant library with a clean api to help you with your backtesting. It's
+optionated with good defaults, so you can start doing your work without having to setup plots, colors, scales,
+autoscaling, keybindings, handle panning+vertical zooming (which all non-finance libraries have problems with).
+And best of all: it can show hundreds of thousands of datapoints without batting an eye.
+
+<img src="https://badge.fury.io/py/finplot.svg"/> <img src="https://pepy.tech/badge/finplot/month"/> <img src="https://img.shields.io/badge/License-MIT-yellow.svg"/>
+
+
+## Features
+
+* Great performance compared to mpl_finance, plotly and Bokeh
+* Clean api
+* Works with both stocks as well as cryptocurrencies on any time resolution
+* Show as many charts as you want on the same time axis, zoom on all of them at once
+* Auto-reload position where you were looking last run
+* Overlays, fill between, value bands, symbols, labels, legend, volume profile, heatmaps, etc.
+* Can show real-time updates, including orderbook. Save screenshot.
+* Comes with a [dozen](https://github.com/highfestiva/finplot/blob/master/finplot/examples) great examples.
+
+![feature1](https://raw.githubusercontent.com/highfestiva/finplot/master/feature1.png)
+
+![feature2](https://raw.githubusercontent.com/highfestiva/finplot/master/feature2.jpg)
+
+![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature3.jpg)
+
+![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature-nuts.jpg)
+
+
+## What it is not
+
+finplot *is not a web app*. It does not help you create an homebrew exchange. It does not work with Jupyter Labs.
+
+It is only intended for you to do backtesting in. That is not to say that you can't create a ticker or a trade
+widget yourself. The library is based on the eminent pyqtgraph, which is fast and flexible, so feel free to hack
+away if that's what you want.
+
+
+## Easy installation
+
+```bash
+$ pip install finplot
+```
+
+
+## Example
+
+It's straight-forward to start using. This shows every daily candle of Apple since the 80'ies:
+
+```python
+import finplot as fplt
+import yfinance
+
+df = yfinance.download('AAPL')
+fplt.candlestick_ochl(df[['Open', 'Close', 'High', 'Low']])
+fplt.show()
+```
+
+For more examples and a bunch of snippets, see the [examples](https://github.com/highfestiva/finplot/blob/master/finplot/examples/)
+directory or the [wiki](https://github.com/highfestiva/finplot/wiki). There you'll find how to plot MACD, Parabolic SAR, RSI,
+volume profile and much more.
+
+
+## Coffee
+
+For future support and features, consider a small donation.
+
+BTC: bc1qk8m8yh86l2pz4eypflchr0tkn5aeud6cmt426m
+
+ETH: 0x684d7d4C52ed428AE9a36B2407ba909D896cDB67
```

### Comparing `finplot-1.9.0/README.md` & `finplot-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `finplot-1.9.0/finplot/__init__.py` & `finplot-1.9.1/finplot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,6863 +33,7188 @@
 00000200: 726f 6d20 6461 7465 7574 696c 2e74 7a20  rom dateutil.tz 
 00000210: 696d 706f 7274 2074 7a6c 6f63 616c 0d0a  import tzlocal..
 00000220: 6672 6f6d 2064 6563 696d 616c 2069 6d70  from decimal imp
 00000230: 6f72 7420 4465 6369 6d61 6c0d 0a66 726f  ort Decimal..fro
 00000240: 6d20 6675 6e63 746f 6f6c 7320 696d 706f  m functools impo
 00000250: 7274 2070 6172 7469 616c 2c20 7061 7274  rt partial, part
 00000260: 6961 6c6d 6574 686f 640d 0a66 726f 6d20  ialmethod..from 
-00000270: 6d61 7468 2069 6d70 6f72 7420 6365 696c  math import ceil
-00000280: 2c20 666c 6f6f 722c 2066 6d6f 640d 0a69  , floor, fmod..i
-00000290: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-000002a0: 700d 0a69 6d70 6f72 7420 6f73 2e70 6174  p..import os.pat
-000002b0: 680d 0a69 6d70 6f72 7420 7061 6e64 6173  h..import pandas
-000002c0: 2061 7320 7064 0d0a 696d 706f 7274 2070   as pd..import p
-000002d0: 7971 7467 7261 7068 2061 7320 7067 0d0a  yqtgraph as pg..
-000002e0: 6672 6f6d 2070 7971 7467 7261 7068 2069  from pyqtgraph i
-000002f0: 6d70 6f72 7420 5174 436f 7265 2c20 5174  mport QtCore, Qt
-00000300: 4775 690d 0a0d 0a0d 0a0d 0a23 2061 7070  Gui........# app
-00000310: 726f 7072 6961 7465 2074 7970 6573 0d0a  ropriate types..
-00000320: 436f 6c6f 724d 6170 203d 2070 672e 436f  ColorMap = pg.Co
-00000330: 6c6f 724d 6170 0d0a 0d0a 2320 6d6f 6475  lorMap....# modu
-00000340: 6c65 2064 6566 696e 6974 696f 6e73 2c20  le definitions, 
-00000350: 6d6f 7374 6c79 2063 6f6c 6f72 730d 0a6c  mostly colors..l
-00000360: 6567 656e 645f 626f 7264 6572 5f63 6f6c  egend_border_col
-00000370: 6f72 203d 2027 2337 3737 270d 0a6c 6567  or = '#777'..leg
-00000380: 656e 645f 6669 6c6c 5f63 6f6c 6f72 2020  end_fill_color  
-00000390: 203d 2027 2336 3636 3827 0d0a 6c65 6765   = '#6668'..lege
-000003a0: 6e64 5f74 6578 745f 636f 6c6f 7220 2020  nd_text_color   
-000003b0: 3d20 2723 6464 6436 270d 0a73 6f66 745f  = '#ddd6'..soft_
-000003c0: 636f 6c6f 7273 203d 205b 2723 3166 3737  colors = ['#1f77
-000003d0: 6234 272c 2027 2366 6637 6630 6527 2c20  b4', '#ff7f0e', 
-000003e0: 2723 3263 6130 3263 272c 2027 2364 3632  '#2ca02c', '#d62
-000003f0: 3732 3827 2c20 2723 3934 3637 6264 272c  728', '#9467bd',
-00000400: 2027 2338 6335 3634 6227 2c20 2723 6533   '#8c564b', '#e3
-00000410: 3737 6332 272c 2027 2337 6637 6637 6627  77c2', '#7f7f7f'
-00000420: 2c20 2723 6263 6264 3232 272c 2027 2331  , '#bcbd22', '#1
-00000430: 3762 6563 6627 5d0d 0a68 6172 645f 636f  7becf']..hard_co
-00000440: 6c6f 7273 203d 205b 2723 3030 3030 3030  lors = ['#000000
-00000450: 272c 2027 2337 3732 3231 3127 2c20 2723  ', '#772211', '#
-00000460: 3030 3030 3636 272c 2027 2335 3535 3535  000066', '#55555
-00000470: 3527 2c20 2723 3030 3232 6363 272c 2027  5', '#0022cc', '
-00000480: 2366 6663 6330 3027 5d0d 0a63 6f6c 6d61  #ffcc00']..colma
-00000490: 705f 636c 6173 6820 3d20 436f 6c6f 724d  p_clash = ColorM
-000004a0: 6170 285b 302e 302c 2030 2e32 2c20 302e  ap([0.0, 0.2, 0.
-000004b0: 362c 2031 2e30 5d2c 205b 5b31 3237 2c20  6, 1.0], [[127, 
-000004c0: 3132 372c 2032 3535 2c20 3531 5d2c 205b  127, 255, 51], [
-000004d0: 302c 2030 2c20 3132 372c 2035 315d 2c20  0, 0, 127, 51], 
-000004e0: 5b32 3535 2c20 3531 2c20 3130 322c 2035  [255, 51, 102, 5
-000004f0: 315d 2c20 5b32 3535 2c20 3137 382c 2037  1], [255, 178, 7
-00000500: 362c 2035 315d 5d29 0d0a 666f 7265 6772  6, 51]])..foregr
-00000510: 6f75 6e64 203d 2027 2330 3030 270d 0a62  ound = '#000'..b
-00000520: 6163 6b67 726f 756e 6420 3d20 2723 6666  ackground = '#ff
-00000530: 6627 0d0a 6f64 645f 706c 6f74 5f62 6163  f'..odd_plot_bac
-00000540: 6b67 726f 756e 6420 3d20 2723 6561 6561  kground = '#eaea
-00000550: 6561 270d 0a63 616e 646c 655f 6275 6c6c  ea'..candle_bull
-00000560: 5f63 6f6c 6f72 203d 2027 2332 3661 3639  _color = '#26a69
-00000570: 6127 0d0a 6361 6e64 6c65 5f62 6561 725f  a'..candle_bear_
-00000580: 636f 6c6f 7220 3d20 2723 6566 3533 3530  color = '#ef5350
-00000590: 270d 0a63 616e 646c 655f 6275 6c6c 5f62  '..candle_bull_b
-000005a0: 6f64 795f 636f 6c6f 7220 3d20 6261 636b  ody_color = back
-000005b0: 6772 6f75 6e64 0d0a 6361 6e64 6c65 5f62  ground..candle_b
-000005c0: 6561 725f 626f 6479 5f63 6f6c 6f72 203d  ear_body_color =
-000005d0: 2063 616e 646c 655f 6265 6172 5f63 6f6c   candle_bear_col
-000005e0: 6f72 0d0a 6361 6e64 6c65 5f73 6861 646f  or..candle_shado
-000005f0: 775f 7769 6474 6820 3d20 310d 0a76 6f6c  w_width = 1..vol
-00000600: 756d 655f 6275 6c6c 5f63 6f6c 6f72 203d  ume_bull_color =
-00000610: 2027 2339 3264 3263 6327 0d0a 766f 6c75   '#92d2cc'..volu
-00000620: 6d65 5f62 6561 725f 636f 6c6f 7220 3d20  me_bear_color = 
-00000630: 2723 6637 6139 6137 270d 0a76 6f6c 756d  '#f7a9a7'..volum
-00000640: 655f 6275 6c6c 5f62 6f64 795f 636f 6c6f  e_bull_body_colo
-00000650: 7220 3d20 766f 6c75 6d65 5f62 756c 6c5f  r = volume_bull_
-00000660: 636f 6c6f 720d 0a76 6f6c 756d 655f 6e65  color..volume_ne
-00000670: 7574 7261 6c5f 636f 6c6f 7220 3d20 2723  utral_color = '#
-00000680: 6262 6227 0d0a 706f 635f 636f 6c6f 7220  bbb'..poc_color 
-00000690: 3d20 2723 3030 3627 0d0a 6261 6e64 5f63  = '#006'..band_c
-000006a0: 6f6c 6f72 203d 2027 2364 3264 6665 3627  olor = '#d2dfe6'
-000006b0: 0d0a 6372 6f73 735f 6861 6972 5f63 6f6c  ..cross_hair_col
-000006c0: 6f72 203d 2027 2330 3030 3727 0d0a 6472  or = '#0007'..dr
-000006d0: 6177 5f6c 696e 655f 636f 6c6f 7220 3d20  aw_line_color = 
-000006e0: 2723 3030 3027 0d0a 6472 6177 5f64 6f6e  '#000'..draw_don
-000006f0: 655f 636f 6c6f 7220 3d20 2723 3535 3527  e_color = '#555'
-00000700: 0d0a 7369 676e 6966 6963 616e 745f 6465  ..significant_de
-00000710: 6369 6d61 6c73 203d 2038 0d0a 7369 676e  cimals = 8..sign
-00000720: 6966 6963 616e 745f 6570 7320 3d20 3165  ificant_eps = 1e
-00000730: 2d38 0d0a 6d61 785f 7a6f 6f6d 5f70 6f69  -8..max_zoom_poi
-00000740: 6e74 7320 3d20 3230 2023 206e 756d 6265  nts = 20 # numbe
-00000750: 7220 6f66 2076 6973 6962 6c65 2063 616e  r of visible can
-00000760: 646c 6573 2077 6865 6e20 6d61 7869 6d75  dles when maximu
-00000770: 6d20 7a6f 6f6d 6564 2069 6e0d 0a74 6f70  m zoomed in..top
-00000780: 5f67 7261 7068 5f73 6361 6c65 203d 2032  _graph_scale = 2
-00000790: 0d0a 636c 616d 705f 6772 6964 203d 2054  ..clamp_grid = T
-000007a0: 7275 650d 0a72 6967 6874 5f6d 6172 6769  rue..right_margi
-000007b0: 6e5f 6361 6e64 6c65 7320 3d20 3520 2320  n_candles = 5 # 
-000007c0: 7768 6974 6573 7061 6365 2061 7420 7468  whitespace at th
-000007d0: 6520 7269 6768 742d 6861 6e64 2073 6964  e right-hand sid
-000007e0: 650d 0a73 6964 655f 6d61 7267 696e 203d  e..side_margin =
-000007f0: 2030 2e35 0d0a 6c6f 645f 6361 6e64 6c65   0.5..lod_candle
-00000800: 7320 3d20 3330 3030 0d0a 6c6f 645f 6c61  s = 3000..lod_la
-00000810: 6265 6c73 203d 2037 3030 0d0a 6361 6368  bels = 700..cach
-00000820: 655f 6361 6e64 6c65 5f66 6163 746f 7220  e_candle_factor 
-00000830: 3d20 3320 2320 6661 6374 6f72 2065 7874  = 3 # factor ext
-00000840: 7261 2063 616e 646c 6573 2072 656e 6465  ra candles rende
-00000850: 7265 6420 746f 2062 7566 6665 720d 0a79  red to buffer..y
-00000860: 5f70 6164 203d 2030 2e30 3320 2320 3325  _pad = 0.03 # 3%
-00000870: 2070 6164 6469 6e67 2061 7420 746f 7020   padding at top 
-00000880: 616e 6420 626f 7474 6f6d 206f 6620 6175  and bottom of au
-00000890: 746f 7a6f 6f6d 2070 6c6f 7473 0d0a 795f  tozoom plots..y_
-000008a0: 6c61 6265 6c5f 7769 6474 6820 3d20 3635  label_width = 65
-000008b0: 0d0a 6469 7370 6c61 795f 7469 6d65 7a6f  ..display_timezo
-000008c0: 6e65 203d 2074 7a6c 6f63 616c 2829 2023  ne = tzlocal() #
-000008d0: 2064 6566 6175 6c74 2074 6f20 6c6f 6361   default to loca
-000008e0: 6c0d 0a77 696e 782c 7769 6e79 2c77 696e  l..winx,winy,win
-000008f0: 772c 7769 6e68 203d 2033 3030 2c31 3530  w,winh = 300,150
-00000900: 2c38 3030 2c34 3030 0d0a 6c6f 675f 706c  ,800,400..log_pl
-00000910: 6f74 5f6f 6666 7365 7420 3d20 2d32 2e32  ot_offset = -2.2
-00000920: 3232 3232 3232 652d 3136 2023 2049 2063  222222e-16 # I c
-00000930: 6f75 6c64 2066 696c 6520 6120 6275 6720  ould file a bug 
-00000940: 7265 706f 7274 2c20 7072 6f62 6162 6c79  report, probably
-00000950: 2069 6e20 5079 5174 2c20 6275 7420 7468   in PyQt, but th
-00000960: 6973 2069 7320 6d6f 7265 2066 756e 0d0a  is is more fun..
-00000970: 2320 666f 726d 6174 3a20 6d6f 6465 2c20  # format: mode, 
-00000980: 6d69 6e2d 6475 7261 7469 6f6e 2c20 7064  min-duration, pd
-00000990: 2d66 7265 712d 666d 742c 2074 6963 6b2d  -freq-fmt, tick-
-000009a0: 7374 722d 6c65 6e0d 0a74 696d 655f 7370  str-len..time_sp
-000009b0: 6c69 7473 203d 205b 2827 7965 6172 7327  lits = [('years'
-000009c0: 2c20 322a 3336 352a 3234 2a36 302a 3630  , 2*365*24*60*60
-000009d0: 2c20 2027 5953 272c 2020 3429 2c20 2827  ,  'YS',  4), ('
-000009e0: 6d6f 6e74 6873 272c 2033 2a33 302a 3234  months', 3*30*24
-000009f0: 2a36 302a 3630 2c20 274d 5327 2c20 3130  *60*60, 'MS', 10
-00000a00: 292c 2028 2777 6565 6b73 272c 2020 2033  ), ('weeks',   3
-00000a10: 2a37 2a32 342a 3630 2a36 302c 2027 572d  *7*24*60*60, 'W-
-00000a20: 4d4f 4e27 2c20 3130 292c 0d0a 2020 2020  MON', 10),..    
-00000a30: 2020 2020 2020 2020 2020 2028 2764 6179             ('day
-00000a40: 7327 2c20 2020 2020 2033 2a32 342a 3630  s',      3*24*60
-00000a50: 2a36 302c 2020 2027 4427 2c20 3130 292c  *60,   'D', 10),
-00000a60: 2028 2768 6f75 7273 272c 2020 2020 2020   ('hours',      
-00000a70: 2020 392a 3630 2a36 302c 2027 3348 272c    9*60*60, '3H',
-00000a80: 2031 3629 2c20 2827 686f 7572 7327 2c20   16), ('hours', 
-00000a90: 2020 2020 2020 2033 2a36 302a 3630 2c20         3*60*60, 
-00000aa0: 2020 2020 2748 272c 2031 3629 2c0d 0a20      'H', 16),.. 
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00000ac0: 6d69 6e75 7465 7327 2c20 2020 2020 2020  minutes',       
-00000ad0: 2034 352a 3630 2c20 2731 3554 272c 2031   45*60, '15T', 1
-00000ae0: 3629 2c20 2827 6d69 6e75 7465 7327 2c20  6), ('minutes', 
-00000af0: 2020 2020 2020 2031 352a 3630 2c20 2735         15*60, '5
-00000b00: 5427 2c20 3136 292c 2028 276d 696e 7574  T', 16), ('minut
-00000b10: 6573 272c 2020 2020 2020 2020 2033 2a36  es',         3*6
-00000b20: 302c 2020 2020 2027 5427 2c20 3136 292c  0,     'T', 16),
-00000b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000b40: 2028 2773 6563 6f6e 6473 272c 2020 2020   ('seconds',    
-00000b50: 2020 2020 2020 2034 352c 2027 3135 5327         45, '15S'
-00000b60: 2c20 3139 292c 2028 2773 6563 6f6e 6473  , 19), ('seconds
-00000b70: 272c 2020 2020 2020 2020 2020 2031 352c  ',           15,
-00000b80: 2027 3553 272c 2031 3929 2c20 2827 7365   '5S', 19), ('se
-00000b90: 636f 6e64 7327 2c20 2020 2020 2020 2020  conds',         
-00000ba0: 2020 2033 2c20 2020 2020 2753 272c 2031     3,     'S', 1
-00000bb0: 3929 2c0d 0a20 2020 2020 2020 2020 2020  9),..           
-00000bc0: 2020 2020 2827 6d69 6c6c 6973 6563 6f6e      ('millisecon
-00000bd0: 6473 272c 2020 2020 2020 2030 2c20 2020  ds',       0,   
-00000be0: 274c 272c 2032 3329 5d0d 0a0d 0a61 7070  'L', 23)]....app
-00000bf0: 203d 204e 6f6e 650d 0a77 696e 646f 7773   = None..windows
-00000c00: 203d 205b 5d20 2320 6e6f 2067 630d 0a74   = [] # no gc..t
-00000c10: 696d 6572 7320 3d20 5b5d 2023 206e 6f20  imers = [] # no 
-00000c20: 6763 0d0a 736f 756e 6473 203d 207b 7d20  gc..sounds = {} 
-00000c30: 2320 6e6f 2067 630d 0a65 706f 6368 5f70  # no gc..epoch_p
-00000c40: 6572 696f 6420 3d20 3165 3330 0d0a 6c61  eriod = 1e30..la
-00000c50: 7374 5f61 7820 3d20 4e6f 6e65 2023 2061  st_ax = None # a
-00000c60: 6c77 6179 7320 6173 7375 6d65 2077 6520  lways assume we 
-00000c70: 7761 6e74 2074 6f20 706c 6f74 2069 6e20  want to plot in 
-00000c80: 7468 6520 6c61 7374 2061 7869 732c 2075  the last axis, u
-00000c90: 6e6c 6573 7320 6578 706c 6963 6974 6c79  nless explicitly
-00000ca0: 2073 7065 6369 6669 6564 0d0a 6f76 6572   specified..over
-00000cb0: 6c61 795f 6178 7320 3d20 5b5d 2023 2066  lay_axs = [] # f
-00000cc0: 6f72 206b 6565 7069 6e67 2074 7261 636b  or keeping track
-00000cd0: 206f 6620 6361 6e64 6c65 7374 6963 6b73   of candlesticks
-00000ce0: 2069 6e20 6f76 6572 6c61 7973 0d0a 7669   in overlays..vi
-00000cf0: 6577 7265 7374 6f72 6520 3d20 4661 6c73  ewrestore = Fals
-00000d00: 650d 0a6d 6173 7465 725f 6461 7461 203d  e..master_data =
-00000d10: 207b 7d0d 0a0d 0a0d 0a0d 0a6c 6572 7020   {}........lerp 
-00000d20: 3d20 6c61 6d62 6461 2074 2c61 2c62 3a20  = lambda t,a,b: 
-00000d30: 742a 622b 2831 2d74 292a 610d 0a0d 0a0d  t*b+(1-t)*a.....
-00000d40: 0a0d 0a63 6c61 7373 2045 706f 6368 4178  ...class EpochAx
-00000d50: 6973 4974 656d 2870 672e 4178 6973 4974  isItem(pg.AxisIt
-00000d60: 656d 293a 0d0a 2020 2020 6465 6620 5f5f  em):..    def __
-00000d70: 696e 6974 5f5f 2873 656c 662c 2076 622c  init__(self, vb,
-00000d80: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00000d90: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
-00000da0: 7228 292e 5f5f 696e 6974 5f5f 282a 6172  r().__init__(*ar
-00000db0: 6773 2c20 2a2a 6b77 6172 6773 290d 0a20  gs, **kwargs).. 
-00000dc0: 2020 2020 2020 2073 656c 662e 7662 203d         self.vb =
-00000dd0: 2076 620d 0a0d 0a20 2020 2064 6566 2074   vb....    def t
-00000de0: 6963 6b53 7472 696e 6773 2873 656c 662c  ickStrings(self,
-00000df0: 2076 616c 7565 732c 2073 6361 6c65 2c20   values, scale, 
-00000e00: 7370 6163 696e 6729 3a0d 0a20 2020 2020  spacing):..     
-00000e10: 2020 2069 6620 7365 6c66 2e6d 6f64 6520     if self.mode 
-00000e20: 3d3d 2027 6e75 6d27 3a0d 0a20 2020 2020  == 'num':..     
-00000e30: 2020 2020 2020 2072 6574 7572 6e20 5b27         return ['
-00000e40: 2567 2725 7620 666f 7220 7620 696e 2076  %g'%v for v in v
-00000e50: 616c 7565 735d 0d0a 2020 2020 2020 2020  alues]..        
-00000e60: 636f 6e76 203d 205f 7832 7965 6172 2069  conv = _x2year i
-00000e70: 6620 7365 6c66 2e6d 6f64 653d 3d27 7965  f self.mode=='ye
-00000e80: 6172 7327 2065 6c73 6520 5f78 326c 6f63  ars' else _x2loc
-00000e90: 616c 5f74 0d0a 2020 2020 2020 2020 7374  al_t..        st
-00000ea0: 7273 203d 205b 636f 6e76 2873 656c 662e  rs = [conv(self.
-00000eb0: 7662 2e64 6174 6173 7263 2c20 7661 6c75  vb.datasrc, valu
-00000ec0: 6529 5b30 5d20 666f 7220 7661 6c75 6520  e)[0] for value 
-00000ed0: 696e 2076 616c 7565 735d 0d0a 2020 2020  in values]..    
-00000ee0: 2020 2020 6966 2061 6c6c 2873 2e65 6e64      if all(s.end
-00000ef0: 7377 6974 6828 2720 3030 3a30 3027 2920  swith(' 00:00') 
-00000f00: 666f 7220 7320 696e 2073 7472 7320 6966  for s in strs if
-00000f10: 2073 293a 2023 2061 6c6c 2061 7420 6d69   s): # all at mi
-00000f20: 646e 6967 6874 202d 3e20 726f 756e 6420  dnight -> round 
-00000f30: 746f 2064 6179 730d 0a20 2020 2020 2020  to days..       
-00000f40: 2020 2020 2073 7472 7320 3d20 5b73 2e70       strs = [s.p
-00000f50: 6172 7469 7469 6f6e 2827 2027 295b 305d  artition(' ')[0]
-00000f60: 2066 6f72 2073 2069 6e20 7374 7273 5d0d   for s in strs].
-00000f70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000f80: 7374 7273 0d0a 0d0a 2020 2020 6465 6620  strs....    def 
-00000f90: 7469 636b 5661 6c75 6573 2873 656c 662c  tickValues(self,
-00000fa0: 206d 696e 5661 6c2c 206d 6178 5661 6c2c   minVal, maxVal,
-00000fb0: 2073 697a 6529 3a0d 0a20 2020 2020 2020   size):..       
-00000fc0: 2073 656c 662e 6d6f 6465 203d 2027 6e75   self.mode = 'nu
-00000fd0: 6d27 0d0a 2020 2020 2020 2020 6178 203d  m'..        ax =
-00000fe0: 2073 656c 662e 7662 2e70 6172 656e 7428   self.vb.parent(
-00000ff0: 290d 0a20 2020 2020 2020 2064 6174 6173  )..        datas
-00001000: 7263 203d 205f 6765 745f 6461 7461 7372  rc = _get_datasr
-00001010: 6328 6178 2c20 7265 7175 6972 653d 4661  c(ax, require=Fa
-00001020: 6c73 6529 0d0a 2020 2020 2020 2020 6966  lse)..        if
-00001030: 2064 6174 6173 7263 2069 7320 4e6f 6e65   datasrc is None
-00001040: 206f 7220 6e6f 7420 7365 6c66 2e76 622e   or not self.vb.
-00001050: 785f 696e 6465 7865 643a 0d0a 2020 2020  x_indexed:..    
-00001060: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00001070: 7570 6572 2829 2e74 6963 6b56 616c 7565  uper().tickValue
-00001080: 7328 6d69 6e56 616c 2c20 6d61 7856 616c  s(minVal, maxVal
-00001090: 2c20 7369 7a65 290d 0a20 2020 2020 2020  , size)..       
-000010a0: 2023 2063 616c 6375 6c61 7465 2069 6620   # calculate if 
-000010b0: 7765 2075 7365 2079 6561 7273 2c20 6461  we use years, da
-000010c0: 7973 2c20 6574 632e 0d0a 2020 2020 2020  ys, etc...      
-000010d0: 2020 7430 2c74 312c 5f2c 5f2c 5f20 3d20    t0,t1,_,_,_ = 
-000010e0: 6461 7461 7372 632e 6869 6c6f 286d 696e  datasrc.hilo(min
-000010f0: 5661 6c2c 206d 6178 5661 6c29 0d0a 2020  Val, maxVal)..  
-00001100: 2020 2020 2020 7430 2c74 3120 3d20 7064        t0,t1 = pd
-00001110: 2e74 6f5f 6461 7465 7469 6d65 2874 3029  .to_datetime(t0)
-00001120: 2c20 7064 2e74 6f5f 6461 7465 7469 6d65  , pd.to_datetime
-00001130: 2874 3129 0d0a 2020 2020 2020 2020 6474  (t1)..        dt
-00001140: 7320 3d20 2874 312d 7430 292e 746f 7461  s = (t1-t0).tota
-00001150: 6c5f 7365 636f 6e64 7328 290d 0a20 2020  l_seconds()..   
-00001160: 2020 2020 2067 6678 5f77 6964 7468 203d       gfx_width =
-00001170: 2069 6e74 2873 697a 6529 0d0a 2020 2020   int(size)..    
-00001180: 2020 2020 666f 7220 6d6f 6465 2c20 6474      for mode, dt
-00001190: 742c 2066 7265 712c 2074 6963 6b6c 656e  t, freq, ticklen
-000011a0: 2069 6e20 7469 6d65 5f73 706c 6974 733a   in time_splits:
-000011b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000011c0: 2064 7473 203e 2064 7474 3a0d 0a20 2020   dts > dtt:..   
-000011d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000011e0: 662e 6d6f 6465 203d 206d 6f64 650d 0a20  f.mode = mode.. 
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001200: 6573 6972 6564 5f74 6963 6b73 203d 2067  esired_ticks = g
-00001210: 6678 5f77 6964 7468 202f 2028 2874 6963  fx_width / ((tic
-00001220: 6b6c 656e 2b32 2920 2a20 3130 2920 2d20  klen+2) * 10) - 
-00001230: 3120 2320 616e 2061 7070 726f 7869 6d61  1 # an approxima
-00001240: 7469 6f6e 2069 7320 6669 6e65 0d0a 2020  tion is fine..  
-00001250: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001260: 2073 656c 662e 7662 2e64 6174 6173 7263   self.vb.datasrc
-00001270: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00001280: 206e 6f74 2073 656c 662e 7662 2e64 6174   not self.vb.dat
-00001290: 6173 7263 2e69 735f 736d 6f6f 7468 5f74  asrc.is_smooth_t
-000012a0: 696d 6528 293a 0d0a 2020 2020 2020 2020  ime():..        
-000012b0: 2020 2020 2020 2020 2020 2020 6465 7369              desi
-000012c0: 7265 645f 7469 636b 7320 2d3d 2031 2023  red_ticks -= 1 #
-000012d0: 206c 6561 7665 206d 6f72 6520 7370 6163   leave more spac
-000012e0: 6520 666f 7220 756e 6576 656e 6c79 2073  e for unevenly s
-000012f0: 7061 6365 6420 7469 636b 730d 0a20 2020  paced ticks..   
-00001300: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00001310: 6972 6564 5f74 6963 6b73 203d 206d 6178  ired_ticks = max
-00001320: 2864 6573 6972 6564 5f74 6963 6b73 2c20  (desired_ticks, 
-00001330: 3429 0d0a 2020 2020 2020 2020 2020 2020  4)..            
-00001340: 2020 2020 746f 5f6d 6964 6e69 6768 7420      to_midnight 
-00001350: 3d20 6672 6571 2069 6e20 2827 5953 272c  = freq in ('YS',
-00001360: 274d 5327 2c20 2757 2d4d 4f4e 272c 2027  'MS', 'W-MON', '
-00001370: 4427 290d 0a20 2020 2020 2020 2020 2020  D')..           
-00001380: 2020 2020 2074 7a20 3d20 6469 7370 6c61       tz = displa
-00001390: 795f 7469 6d65 7a6f 6e65 2069 6620 746f  y_timezone if to
-000013a0: 5f6d 6964 6e69 6768 7420 656c 7365 204e  _midnight else N
-000013b0: 6f6e 6520 2320 666f 7220 7368 6f72 7465  one # for shorte
-000013c0: 7220 7469 6d65 6672 616d 6573 2c20 7469  r timeframes, ti
-000013d0: 6d65 7a6f 6e65 2073 6565 6d73 2062 7567  mezone seems bug
-000013e0: 6779 0d0a 2020 2020 2020 2020 2020 2020  gy..            
-000013f0: 2020 2020 726e 6720 3d20 7064 2e64 6174      rng = pd.dat
-00001400: 655f 7261 6e67 6528 7430 2c20 7431 2c20  e_range(t0, t1, 
-00001410: 747a 3d74 7a2c 206e 6f72 6d61 6c69 7a65  tz=tz, normalize
-00001420: 3d74 6f5f 6d69 646e 6967 6874 2c20 6672  =to_midnight, fr
-00001430: 6571 3d66 7265 7129 0d0a 2020 2020 2020  eq=freq)..      
-00001440: 2020 2020 2020 2020 2020 7374 6570 7320            steps 
-00001450: 3d20 6c65 6e28 726e 6729 2069 6620 6c65  = len(rng) if le
-00001460: 6e28 726e 6729 2631 3d3d 3020 656c 7365  n(rng)&1==0 else
-00001470: 206c 656e 2872 6e67 292b 3120 2320 7265   len(rng)+1 # re
-00001480: 6475 6365 206a 6974 7465 7220 6265 7477  duce jitter betw
-00001490: 6565 6e20 652e 672e 2035 3c2d 2d3e 3130  een e.g. 5<-->10
-000014a0: 2074 6963 6b73 2066 6f72 2072 6573 6f6c   ticks for resol
-000014b0: 7574 696f 6e20 636c 6f73 6520 746f 206c  ution close to l
-000014c0: 696d 6974 0d0a 2020 2020 2020 2020 2020  imit..          
-000014d0: 2020 2020 2020 7374 6570 203d 2069 6e74        step = int
-000014e0: 2873 7465 7073 2f64 6573 6972 6564 5f74  (steps/desired_t
-000014f0: 6963 6b73 2920 6f72 2031 0d0a 2020 2020  icks) or 1..    
-00001500: 2020 2020 2020 2020 2020 2020 726e 6720              rng 
-00001510: 3d20 726e 675b 3a3a 7374 6570 5d0d 0a20  = rng[::step].. 
-00001520: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001530: 6620 6e6f 7420 746f 5f6d 6964 6e69 6768  f not to_midnigh
-00001540: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00001550: 2020 2020 2020 2020 7472 793a 2020 2020          try:    
-00001560: 726e 6720 3d20 726e 672e 726f 756e 6428  rng = rng.round(
-00001570: 6672 6571 3d66 7265 7129 0d0a 2020 2020  freq=freq)..    
-00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001590: 6578 6365 7074 3a20 7061 7373 0d0a 2020  except: pass..  
-000015a0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-000015b0: 203d 2073 656c 662e 7662 2e70 6172 656e   = self.vb.paren
-000015c0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-000015d0: 2020 2020 2072 6e67 203d 205f 7064 7469       rng = _pdti
-000015e0: 6d65 3269 6e64 6578 2861 783d 6178 2c20  me2index(ax=ax, 
-000015f0: 7473 3d70 642e 5365 7269 6573 2872 6e67  ts=pd.Series(rng
-00001600: 292c 2072 6571 7569 7265 5f74 696d 653d  ), require_time=
-00001610: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
-00001620: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-00001630: 205b 6365 696c 2869 2920 666f 7220 6920   [ceil(i) for i 
-00001640: 696e 2072 6e67 5d0d 0a20 2020 2020 2020  in rng]..       
-00001650: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001660: 5b28 302c 2069 6e64 6963 6573 295d 0d0a  [(0, indices)]..
-00001670: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00001680: 2830 2c5b 5d29 5d0d 0a0d 0a20 2020 2064  (0,[])]....    d
-00001690: 6566 2067 656e 6572 6174 6544 7261 7753  ef generateDrawS
-000016a0: 7065 6373 2873 656c 662c 2070 293a 0d0a  pecs(self, p):..
-000016b0: 2020 2020 2020 2020 7370 6563 7320 3d20          specs = 
-000016c0: 7375 7065 7228 292e 6765 6e65 7261 7465  super().generate
-000016d0: 4472 6177 5370 6563 7328 7029 0d0a 2020  DrawSpecs(p)..  
-000016e0: 2020 2020 2020 6966 2073 7065 6373 3a0d        if specs:.
-000016f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001700: 6e6f 7420 7365 6c66 2e73 7479 6c65 5b27  not self.style['
-00001710: 7368 6f77 5661 6c75 6573 275d 3a0d 0a20  showValues']:.. 
-00001720: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001730: 656e 2c70 302c 7031 203d 2073 7065 6373  en,p0,p1 = specs
-00001740: 5b30 5d20 2320 6178 6973 2073 7065 6373  [0] # axis specs
-00001750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001760: 2020 7370 6563 7320 3d20 5b28 5f6d 616b    specs = [(_mak
-00001770: 6570 656e 2827 2366 6666 3027 292c 7030  epen('#fff0'),p0
-00001780: 2c70 3129 5d20 2b20 6c69 7374 2873 7065  ,p1)] + list(spe
-00001790: 6373 5b31 3a5d 2920 2320 646f 6e27 7420  cs[1:]) # don't 
-000017a0: 6472 6177 2061 7869 7320 6966 2068 6964  draw axis if hid
-000017b0: 696e 6720 7661 6c75 6573 0d0a 2020 2020  ing values..    
-000017c0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000017d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000017e0: 2074 6872 6f77 206f 7574 2074 6963 6b73   throw out ticks
-000017f0: 2074 6861 7420 6172 6520 6f75 7420 6f66   that are out of
-00001800: 2062 6f75 6e64 730d 0a20 2020 2020 2020   bounds..       
-00001810: 2020 2020 2020 2020 2074 6578 745f 7370           text_sp
-00001820: 6563 7320 3d20 7370 6563 735b 325d 0d0a  ecs = specs[2]..
-00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001840: 6966 206c 656e 2874 6578 745f 7370 6563  if len(text_spec
-00001850: 7329 203e 3d20 343a 0d0a 2020 2020 2020  s) >= 4:..      
-00001860: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001870: 6374 2c66 6c61 6773 2c74 6578 7420 3d20  ct,flags,text = 
-00001880: 7465 7874 5f73 7065 6373 5b30 5d0d 0a20  text_specs[0].. 
+00000270: 6669 6e70 6c6f 742e 6c69 7665 2069 6d70  finplot.live imp
+00000280: 6f72 7420 4c69 7665 0d0a 6672 6f6d 206d  ort Live..from m
+00000290: 6174 6820 696d 706f 7274 2063 6569 6c2c  ath import ceil,
+000002a0: 2066 6c6f 6f72 2c20 666d 6f64 0d0a 696d   floor, fmod..im
+000002b0: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+000002c0: 0d0a 696d 706f 7274 206f 732e 7061 7468  ..import os.path
+000002d0: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
+000002e0: 6173 2070 640d 0a69 6d70 6f72 7420 7079  as pd..import py
+000002f0: 7174 6772 6170 6820 6173 2070 670d 0a66  qtgraph as pg..f
+00000300: 726f 6d20 7079 7174 6772 6170 6820 696d  rom pyqtgraph im
+00000310: 706f 7274 2051 7443 6f72 652c 2051 7447  port QtCore, QtG
+00000320: 7569 0d0a 0d0a 0d0a 0d0a 2320 6170 7072  ui........# appr
+00000330: 6f70 7269 6174 6520 7479 7065 730d 0a43  opriate types..C
+00000340: 6f6c 6f72 4d61 7020 3d20 7067 2e43 6f6c  olorMap = pg.Col
+00000350: 6f72 4d61 700d 0a0d 0a23 206d 6f64 756c  orMap....# modul
+00000360: 6520 6465 6669 6e69 7469 6f6e 732c 206d  e definitions, m
+00000370: 6f73 746c 7920 636f 6c6f 7273 0d0a 6c65  ostly colors..le
+00000380: 6765 6e64 5f62 6f72 6465 725f 636f 6c6f  gend_border_colo
+00000390: 7220 3d20 2723 3737 3727 0d0a 6c65 6765  r = '#777'..lege
+000003a0: 6e64 5f66 696c 6c5f 636f 6c6f 7220 2020  nd_fill_color   
+000003b0: 3d20 2723 3636 3638 270d 0a6c 6567 656e  = '#6668'..legen
+000003c0: 645f 7465 7874 5f63 6f6c 6f72 2020 203d  d_text_color   =
+000003d0: 2027 2364 6464 3627 0d0a 736f 6674 5f63   '#ddd6'..soft_c
+000003e0: 6f6c 6f72 7320 3d20 5b27 2331 6637 3762  olors = ['#1f77b
+000003f0: 3427 2c20 2723 6666 3766 3065 272c 2027  4', '#ff7f0e', '
+00000400: 2332 6361 3032 6327 2c20 2723 6436 3237  #2ca02c', '#d627
+00000410: 3238 272c 2027 2339 3436 3762 6427 2c20  28', '#9467bd', 
+00000420: 2723 3863 3536 3462 272c 2027 2365 3337  '#8c564b', '#e37
+00000430: 3763 3227 2c20 2723 3766 3766 3766 272c  7c2', '#7f7f7f',
+00000440: 2027 2362 6362 6432 3227 2c20 2723 3137   '#bcbd22', '#17
+00000450: 6265 6366 275d 0d0a 6861 7264 5f63 6f6c  becf']..hard_col
+00000460: 6f72 7320 3d20 5b27 2330 3030 3030 3027  ors = ['#000000'
+00000470: 2c20 2723 3737 3232 3131 272c 2027 2330  , '#772211', '#0
+00000480: 3030 3036 3627 2c20 2723 3535 3535 3535  00066', '#555555
+00000490: 272c 2027 2330 3032 3263 6327 2c20 2723  ', '#0022cc', '#
+000004a0: 6666 6363 3030 275d 0d0a 636f 6c6d 6170  ffcc00']..colmap
+000004b0: 5f63 6c61 7368 203d 2043 6f6c 6f72 4d61  _clash = ColorMa
+000004c0: 7028 5b30 2e30 2c20 302e 322c 2030 2e36  p([0.0, 0.2, 0.6
+000004d0: 2c20 312e 305d 2c20 5b5b 3132 372c 2031  , 1.0], [[127, 1
+000004e0: 3237 2c20 3235 352c 2035 315d 2c20 5b30  27, 255, 51], [0
+000004f0: 2c20 302c 2031 3237 2c20 3531 5d2c 205b  , 0, 127, 51], [
+00000500: 3235 352c 2035 312c 2031 3032 2c20 3531  255, 51, 102, 51
+00000510: 5d2c 205b 3235 352c 2031 3738 2c20 3736  ], [255, 178, 76
+00000520: 2c20 3531 5d5d 290d 0a66 6f72 6567 726f  , 51]])..foregro
+00000530: 756e 6420 3d20 2723 3030 3027 0d0a 6261  und = '#000'..ba
+00000540: 636b 6772 6f75 6e64 203d 2027 2366 6666  ckground = '#fff
+00000550: 270d 0a6f 6464 5f70 6c6f 745f 6261 636b  '..odd_plot_back
+00000560: 6772 6f75 6e64 203d 2027 2365 6165 6165  ground = '#eaeae
+00000570: 6127 0d0a 6361 6e64 6c65 5f62 756c 6c5f  a'..candle_bull_
+00000580: 636f 6c6f 7220 3d20 2723 3236 6136 3961  color = '#26a69a
+00000590: 270d 0a63 616e 646c 655f 6265 6172 5f63  '..candle_bear_c
+000005a0: 6f6c 6f72 203d 2027 2365 6635 3335 3027  olor = '#ef5350'
+000005b0: 0d0a 6361 6e64 6c65 5f62 756c 6c5f 626f  ..candle_bull_bo
+000005c0: 6479 5f63 6f6c 6f72 203d 2062 6163 6b67  dy_color = backg
+000005d0: 726f 756e 640d 0a63 616e 646c 655f 6265  round..candle_be
+000005e0: 6172 5f62 6f64 795f 636f 6c6f 7220 3d20  ar_body_color = 
+000005f0: 6361 6e64 6c65 5f62 6561 725f 636f 6c6f  candle_bear_colo
+00000600: 720d 0a63 616e 646c 655f 7368 6164 6f77  r..candle_shadow
+00000610: 5f77 6964 7468 203d 2031 0d0a 766f 6c75  _width = 1..volu
+00000620: 6d65 5f62 756c 6c5f 636f 6c6f 7220 3d20  me_bull_color = 
+00000630: 2723 3932 6432 6363 270d 0a76 6f6c 756d  '#92d2cc'..volum
+00000640: 655f 6265 6172 5f63 6f6c 6f72 203d 2027  e_bear_color = '
+00000650: 2366 3761 3961 3727 0d0a 766f 6c75 6d65  #f7a9a7'..volume
+00000660: 5f62 756c 6c5f 626f 6479 5f63 6f6c 6f72  _bull_body_color
+00000670: 203d 2076 6f6c 756d 655f 6275 6c6c 5f63   = volume_bull_c
+00000680: 6f6c 6f72 0d0a 766f 6c75 6d65 5f6e 6575  olor..volume_neu
+00000690: 7472 616c 5f63 6f6c 6f72 203d 2027 2362  tral_color = '#b
+000006a0: 6262 270d 0a70 6f63 5f63 6f6c 6f72 203d  bb'..poc_color =
+000006b0: 2027 2330 3036 270d 0a62 616e 645f 636f   '#006'..band_co
+000006c0: 6c6f 7220 3d20 2723 6432 6466 6536 270d  lor = '#d2dfe6'.
+000006d0: 0a63 726f 7373 5f68 6169 725f 636f 6c6f  .cross_hair_colo
+000006e0: 7220 3d20 2723 3030 3037 270d 0a64 7261  r = '#0007'..dra
+000006f0: 775f 6c69 6e65 5f63 6f6c 6f72 203d 2027  w_line_color = '
+00000700: 2330 3030 270d 0a64 7261 775f 646f 6e65  #000'..draw_done
+00000710: 5f63 6f6c 6f72 203d 2027 2335 3535 270d  _color = '#555'.
+00000720: 0a73 6967 6e69 6669 6361 6e74 5f64 6563  .significant_dec
+00000730: 696d 616c 7320 3d20 380d 0a73 6967 6e69  imals = 8..signi
+00000740: 6669 6361 6e74 5f65 7073 203d 2031 652d  ficant_eps = 1e-
+00000750: 380d 0a6d 6178 5f64 6563 696d 616c 7320  8..max_decimals 
+00000760: 3d20 3130 0d0a 6d61 785f 7a6f 6f6d 5f70  = 10..max_zoom_p
+00000770: 6f69 6e74 7320 3d20 3230 2023 206e 756d  oints = 20 # num
+00000780: 6265 7220 6f66 2076 6973 6962 6c65 2063  ber of visible c
+00000790: 616e 646c 6573 2077 6865 6e20 6d61 7869  andles when maxi
+000007a0: 6d75 6d20 7a6f 6f6d 6564 2069 6e0d 0a74  mum zoomed in..t
+000007b0: 6f70 5f67 7261 7068 5f73 6361 6c65 203d  op_graph_scale =
+000007c0: 2032 0d0a 636c 616d 705f 6772 6964 203d   2..clamp_grid =
+000007d0: 2054 7275 650d 0a72 6967 6874 5f6d 6172   True..right_mar
+000007e0: 6769 6e5f 6361 6e64 6c65 7320 3d20 3520  gin_candles = 5 
+000007f0: 2320 7768 6974 6573 7061 6365 2061 7420  # whitespace at 
+00000800: 7468 6520 7269 6768 742d 6861 6e64 2073  the right-hand s
+00000810: 6964 650d 0a73 6964 655f 6d61 7267 696e  ide..side_margin
+00000820: 203d 2030 2e35 0d0a 6c6f 645f 6361 6e64   = 0.5..lod_cand
+00000830: 6c65 7320 3d20 3330 3030 0d0a 6c6f 645f  les = 3000..lod_
+00000840: 6c61 6265 6c73 203d 2037 3030 0d0a 6361  labels = 700..ca
+00000850: 6368 655f 6361 6e64 6c65 5f66 6163 746f  che_candle_facto
+00000860: 7220 3d20 3320 2320 6661 6374 6f72 2065  r = 3 # factor e
+00000870: 7874 7261 2063 616e 646c 6573 2072 656e  xtra candles ren
+00000880: 6465 7265 6420 746f 2062 7566 6665 720d  dered to buffer.
+00000890: 0a79 5f70 6164 203d 2030 2e30 3320 2320  .y_pad = 0.03 # 
+000008a0: 3325 2070 6164 6469 6e67 2061 7420 746f  3% padding at to
+000008b0: 7020 616e 6420 626f 7474 6f6d 206f 6620  p and bottom of 
+000008c0: 6175 746f 7a6f 6f6d 2070 6c6f 7473 0d0a  autozoom plots..
+000008d0: 795f 6c61 6265 6c5f 7769 6474 6820 3d20  y_label_width = 
+000008e0: 3635 0d0a 6469 7370 6c61 795f 7469 6d65  65..display_time
+000008f0: 7a6f 6e65 203d 2074 7a6c 6f63 616c 2829  zone = tzlocal()
+00000900: 2023 2064 6566 6175 6c74 2074 6f20 6c6f   # default to lo
+00000910: 6361 6c0d 0a77 696e 782c 7769 6e79 2c77  cal..winx,winy,w
+00000920: 696e 772c 7769 6e68 203d 2033 3030 2c31  inw,winh = 300,1
+00000930: 3530 2c38 3030 2c34 3030 0d0a 6c6f 675f  50,800,400..log_
+00000940: 706c 6f74 5f6f 6666 7365 7420 3d20 2d32  plot_offset = -2
+00000950: 2e32 3232 3232 3232 652d 3136 2023 2049  .2222222e-16 # I
+00000960: 2063 6f75 6c64 2066 696c 6520 6120 6275   could file a bu
+00000970: 6720 7265 706f 7274 2c20 7072 6f62 6162  g report, probab
+00000980: 6c79 2069 6e20 5079 5174 2c20 6275 7420  ly in PyQt, but 
+00000990: 7468 6973 2069 7320 6d6f 7265 2066 756e  this is more fun
+000009a0: 0d0a 2320 666f 726d 6174 3a20 6d6f 6465  ..# format: mode
+000009b0: 2c20 6d69 6e2d 6475 7261 7469 6f6e 2c20  , min-duration, 
+000009c0: 7064 2d66 7265 712d 666d 742c 2074 6963  pd-freq-fmt, tic
+000009d0: 6b2d 7374 722d 6c65 6e0d 0a74 696d 655f  k-str-len..time_
+000009e0: 7370 6c69 7473 203d 205b 2827 7965 6172  splits = [('year
+000009f0: 7327 2c20 322a 3336 352a 3234 2a36 302a  s', 2*365*24*60*
+00000a00: 3630 2c20 2027 5953 272c 2020 3429 2c20  60,  'YS',  4), 
+00000a10: 2827 6d6f 6e74 6873 272c 2033 2a33 302a  ('months', 3*30*
+00000a20: 3234 2a36 302a 3630 2c20 274d 5327 2c20  24*60*60, 'MS', 
+00000a30: 3130 292c 2028 2777 6565 6b73 272c 2020  10), ('weeks',  
+00000a40: 2033 2a37 2a32 342a 3630 2a36 302c 2027   3*7*24*60*60, '
+00000a50: 572d 4d4f 4e27 2c20 3130 292c 0d0a 2020  W-MON', 10),..  
+00000a60: 2020 2020 2020 2020 2020 2020 2028 2764               ('d
+00000a70: 6179 7327 2c20 2020 2020 2033 2a32 342a  ays',      3*24*
+00000a80: 3630 2a36 302c 2020 2027 4427 2c20 3130  60*60,   'D', 10
+00000a90: 292c 2028 2768 6f75 7273 272c 2020 2020  ), ('hours',    
+00000aa0: 2020 2020 392a 3630 2a36 302c 2027 3348      9*60*60, '3H
+00000ab0: 272c 2031 3629 2c20 2827 686f 7572 7327  ', 16), ('hours'
+00000ac0: 2c20 2020 2020 2020 2033 2a36 302a 3630  ,        3*60*60
+00000ad0: 2c20 2020 2020 2748 272c 2031 3629 2c0d  ,     'H', 16),.
+00000ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000af0: 2827 6d69 6e75 7465 7327 2c20 2020 2020  ('minutes',     
+00000b00: 2020 2034 352a 3630 2c20 2731 3554 272c     45*60, '15T',
+00000b10: 2031 3629 2c20 2827 6d69 6e75 7465 7327   16), ('minutes'
+00000b20: 2c20 2020 2020 2020 2031 352a 3630 2c20  ,        15*60, 
+00000b30: 2735 5427 2c20 3136 292c 2028 276d 696e  '5T', 16), ('min
+00000b40: 7574 6573 272c 2020 2020 2020 2020 2033  utes',         3
+00000b50: 2a36 302c 2020 2020 2027 5427 2c20 3136  *60,     'T', 16
+00000b60: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00000b70: 2020 2028 2773 6563 6f6e 6473 272c 2020     ('seconds',  
+00000b80: 2020 2020 2020 2020 2034 352c 2027 3135           45, '15
+00000b90: 5327 2c20 3139 292c 2028 2773 6563 6f6e  S', 19), ('secon
+00000ba0: 6473 272c 2020 2020 2020 2020 2020 2031  ds',           1
+00000bb0: 352c 2027 3553 272c 2031 3929 2c20 2827  5, '5S', 19), ('
+00000bc0: 7365 636f 6e64 7327 2c20 2020 2020 2020  seconds',       
+00000bd0: 2020 2020 2033 2c20 2020 2020 2753 272c       3,     'S',
+00000be0: 2031 3929 2c0d 0a20 2020 2020 2020 2020   19),..         
+00000bf0: 2020 2020 2020 2827 6d69 6c6c 6973 6563        ('millisec
+00000c00: 6f6e 6473 272c 2020 2020 2020 2030 2c20  onds',       0, 
+00000c10: 2020 274c 272c 2032 3329 5d0d 0a0d 0a61    'L', 23)]....a
+00000c20: 7070 203d 204e 6f6e 650d 0a77 696e 646f  pp = None..windo
+00000c30: 7773 203d 205b 5d20 2320 6e6f 2067 630d  ws = [] # no gc.
+00000c40: 0a74 696d 6572 7320 3d20 5b5d 2023 206e  .timers = [] # n
+00000c50: 6f20 6763 0d0a 736f 756e 6473 203d 207b  o gc..sounds = {
+00000c60: 7d20 2320 6e6f 2067 630d 0a65 706f 6368  } # no gc..epoch
+00000c70: 5f70 6572 696f 6420 3d20 3165 3330 0d0a  _period = 1e30..
+00000c80: 6c61 7374 5f61 7820 3d20 4e6f 6e65 2023  last_ax = None #
+00000c90: 2061 6c77 6179 7320 6173 7375 6d65 2077   always assume w
+00000ca0: 6520 7761 6e74 2074 6f20 706c 6f74 2069  e want to plot i
+00000cb0: 6e20 7468 6520 6c61 7374 2061 7869 732c  n the last axis,
+00000cc0: 2075 6e6c 6573 7320 6578 706c 6963 6974   unless explicit
+00000cd0: 6c79 2073 7065 6369 6669 6564 0d0a 6f76  ly specified..ov
+00000ce0: 6572 6c61 795f 6178 7320 3d20 5b5d 2023  erlay_axs = [] #
+00000cf0: 2066 6f72 206b 6565 7069 6e67 2074 7261   for keeping tra
+00000d00: 636b 206f 6620 6361 6e64 6c65 7374 6963  ck of candlestic
+00000d10: 6b73 2069 6e20 6f76 6572 6c61 7973 0d0a  ks in overlays..
+00000d20: 7669 6577 7265 7374 6f72 6520 3d20 4661  viewrestore = Fa
+00000d30: 6c73 650d 0a6b 6579 5f65 7363 5f63 6c6f  lse..key_esc_clo
+00000d40: 7365 203d 2054 7275 6520 2320 4553 4320  se = True # ESC 
+00000d50: 6b65 7920 636c 6f73 6573 2077 696e 646f  key closes windo
+00000d60: 770d 0a6d 6173 7465 725f 6461 7461 203d  w..master_data =
+00000d70: 207b 7d0d 0a0d 0a0d 0a0d 0a6c 6572 7020   {}........lerp 
+00000d80: 3d20 6c61 6d62 6461 2074 2c61 2c62 3a20  = lambda t,a,b: 
+00000d90: 742a 622b 2831 2d74 292a 610d 0a0d 0a0d  t*b+(1-t)*a.....
+00000da0: 0a0d 0a63 6c61 7373 2045 706f 6368 4178  ...class EpochAx
+00000db0: 6973 4974 656d 2870 672e 4178 6973 4974  isItem(pg.AxisIt
+00000dc0: 656d 293a 0d0a 2020 2020 6465 6620 5f5f  em):..    def __
+00000dd0: 696e 6974 5f5f 2873 656c 662c 2076 622c  init__(self, vb,
+00000de0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00000df0: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
+00000e00: 7228 292e 5f5f 696e 6974 5f5f 282a 6172  r().__init__(*ar
+00000e10: 6773 2c20 2a2a 6b77 6172 6773 290d 0a20  gs, **kwargs).. 
+00000e20: 2020 2020 2020 2073 656c 662e 7662 203d         self.vb =
+00000e30: 2076 620d 0a0d 0a20 2020 2064 6566 2074   vb....    def t
+00000e40: 6963 6b53 7472 696e 6773 2873 656c 662c  ickStrings(self,
+00000e50: 2076 616c 7565 732c 2073 6361 6c65 2c20   values, scale, 
+00000e60: 7370 6163 696e 6729 3a0d 0a20 2020 2020  spacing):..     
+00000e70: 2020 2069 6620 7365 6c66 2e6d 6f64 6520     if self.mode 
+00000e80: 3d3d 2027 6e75 6d27 3a0d 0a20 2020 2020  == 'num':..     
+00000e90: 2020 2020 2020 2072 6574 7572 6e20 5b27         return ['
+00000ea0: 2567 2725 7620 666f 7220 7620 696e 2076  %g'%v for v in v
+00000eb0: 616c 7565 735d 0d0a 2020 2020 2020 2020  alues]..        
+00000ec0: 636f 6e76 203d 205f 7832 7965 6172 2069  conv = _x2year i
+00000ed0: 6620 7365 6c66 2e6d 6f64 653d 3d27 7965  f self.mode=='ye
+00000ee0: 6172 7327 2065 6c73 6520 5f78 326c 6f63  ars' else _x2loc
+00000ef0: 616c 5f74 0d0a 2020 2020 2020 2020 7374  al_t..        st
+00000f00: 7273 203d 205b 636f 6e76 2873 656c 662e  rs = [conv(self.
+00000f10: 7662 2e64 6174 6173 7263 2c20 7661 6c75  vb.datasrc, valu
+00000f20: 6529 5b30 5d20 666f 7220 7661 6c75 6520  e)[0] for value 
+00000f30: 696e 2076 616c 7565 735d 0d0a 2020 2020  in values]..    
+00000f40: 2020 2020 6966 2061 6c6c 2873 2e65 6e64      if all(s.end
+00000f50: 7377 6974 6828 2720 3030 3a30 3027 2920  swith(' 00:00') 
+00000f60: 666f 7220 7320 696e 2073 7472 7320 6966  for s in strs if
+00000f70: 2073 293a 2023 2061 6c6c 2061 7420 6d69   s): # all at mi
+00000f80: 646e 6967 6874 202d 3e20 726f 756e 6420  dnight -> round 
+00000f90: 746f 2064 6179 730d 0a20 2020 2020 2020  to days..       
+00000fa0: 2020 2020 2073 7472 7320 3d20 5b73 2e70       strs = [s.p
+00000fb0: 6172 7469 7469 6f6e 2827 2027 295b 305d  artition(' ')[0]
+00000fc0: 2066 6f72 2073 2069 6e20 7374 7273 5d0d   for s in strs].
+00000fd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000fe0: 7374 7273 0d0a 0d0a 2020 2020 6465 6620  strs....    def 
+00000ff0: 7469 636b 5661 6c75 6573 2873 656c 662c  tickValues(self,
+00001000: 206d 696e 5661 6c2c 206d 6178 5661 6c2c   minVal, maxVal,
+00001010: 2073 697a 6529 3a0d 0a20 2020 2020 2020   size):..       
+00001020: 2073 656c 662e 6d6f 6465 203d 2027 6e75   self.mode = 'nu
+00001030: 6d27 0d0a 2020 2020 2020 2020 6178 203d  m'..        ax =
+00001040: 2073 656c 662e 7662 2e70 6172 656e 7428   self.vb.parent(
+00001050: 290d 0a20 2020 2020 2020 2064 6174 6173  )..        datas
+00001060: 7263 203d 205f 6765 745f 6461 7461 7372  rc = _get_datasr
+00001070: 6328 6178 2c20 7265 7175 6972 653d 4661  c(ax, require=Fa
+00001080: 6c73 6529 0d0a 2020 2020 2020 2020 6966  lse)..        if
+00001090: 2064 6174 6173 7263 2069 7320 4e6f 6e65   datasrc is None
+000010a0: 206f 7220 6e6f 7420 7365 6c66 2e76 622e   or not self.vb.
+000010b0: 785f 696e 6465 7865 643a 0d0a 2020 2020  x_indexed:..    
+000010c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000010d0: 7570 6572 2829 2e74 6963 6b56 616c 7565  uper().tickValue
+000010e0: 7328 6d69 6e56 616c 2c20 6d61 7856 616c  s(minVal, maxVal
+000010f0: 2c20 7369 7a65 290d 0a20 2020 2020 2020  , size)..       
+00001100: 2023 2063 616c 6375 6c61 7465 2069 6620   # calculate if 
+00001110: 7765 2075 7365 2079 6561 7273 2c20 6461  we use years, da
+00001120: 7973 2c20 6574 632e 0d0a 2020 2020 2020  ys, etc...      
+00001130: 2020 7430 2c74 312c 5f2c 5f2c 5f20 3d20    t0,t1,_,_,_ = 
+00001140: 6461 7461 7372 632e 6869 6c6f 286d 696e  datasrc.hilo(min
+00001150: 5661 6c2c 206d 6178 5661 6c29 0d0a 2020  Val, maxVal)..  
+00001160: 2020 2020 2020 7430 2c74 3120 3d20 7064        t0,t1 = pd
+00001170: 2e74 6f5f 6461 7465 7469 6d65 2874 3029  .to_datetime(t0)
+00001180: 2c20 7064 2e74 6f5f 6461 7465 7469 6d65  , pd.to_datetime
+00001190: 2874 3129 0d0a 2020 2020 2020 2020 6474  (t1)..        dt
+000011a0: 7320 3d20 2874 312d 7430 292e 746f 7461  s = (t1-t0).tota
+000011b0: 6c5f 7365 636f 6e64 7328 290d 0a20 2020  l_seconds()..   
+000011c0: 2020 2020 2067 6678 5f77 6964 7468 203d       gfx_width =
+000011d0: 2069 6e74 2873 697a 6529 0d0a 2020 2020   int(size)..    
+000011e0: 2020 2020 666f 7220 6d6f 6465 2c20 6474      for mode, dt
+000011f0: 742c 2066 7265 712c 2074 6963 6b6c 656e  t, freq, ticklen
+00001200: 2069 6e20 7469 6d65 5f73 706c 6974 733a   in time_splits:
+00001210: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00001220: 2064 7473 203e 2064 7474 3a0d 0a20 2020   dts > dtt:..   
+00001230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001240: 662e 6d6f 6465 203d 206d 6f64 650d 0a20  f.mode = mode.. 
+00001250: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00001260: 6573 6972 6564 5f74 6963 6b73 203d 2067  esired_ticks = g
+00001270: 6678 5f77 6964 7468 202f 2028 2874 6963  fx_width / ((tic
+00001280: 6b6c 656e 2b32 2920 2a20 3130 2920 2d20  klen+2) * 10) - 
+00001290: 3120 2320 616e 2061 7070 726f 7869 6d61  1 # an approxima
+000012a0: 7469 6f6e 2069 7320 6669 6e65 0d0a 2020  tion is fine..  
+000012b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000012c0: 2073 656c 662e 7662 2e64 6174 6173 7263   self.vb.datasrc
+000012d0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+000012e0: 206e 6f74 2073 656c 662e 7662 2e64 6174   not self.vb.dat
+000012f0: 6173 7263 2e69 735f 736d 6f6f 7468 5f74  asrc.is_smooth_t
+00001300: 696d 6528 293a 0d0a 2020 2020 2020 2020  ime():..        
+00001310: 2020 2020 2020 2020 2020 2020 6465 7369              desi
+00001320: 7265 645f 7469 636b 7320 2d3d 2031 2023  red_ticks -= 1 #
+00001330: 206c 6561 7665 206d 6f72 6520 7370 6163   leave more spac
+00001340: 6520 666f 7220 756e 6576 656e 6c79 2073  e for unevenly s
+00001350: 7061 6365 6420 7469 636b 730d 0a20 2020  paced ticks..   
+00001360: 2020 2020 2020 2020 2020 2020 2064 6573               des
+00001370: 6972 6564 5f74 6963 6b73 203d 206d 6178  ired_ticks = max
+00001380: 2864 6573 6972 6564 5f74 6963 6b73 2c20  (desired_ticks, 
+00001390: 3429 0d0a 2020 2020 2020 2020 2020 2020  4)..            
+000013a0: 2020 2020 746f 5f6d 6964 6e69 6768 7420      to_midnight 
+000013b0: 3d20 6672 6571 2069 6e20 2827 5953 272c  = freq in ('YS',
+000013c0: 274d 5327 2c20 2757 2d4d 4f4e 272c 2027  'MS', 'W-MON', '
+000013d0: 4427 290d 0a20 2020 2020 2020 2020 2020  D')..           
+000013e0: 2020 2020 2074 7a20 3d20 6469 7370 6c61       tz = displa
+000013f0: 795f 7469 6d65 7a6f 6e65 2069 6620 746f  y_timezone if to
+00001400: 5f6d 6964 6e69 6768 7420 656c 7365 204e  _midnight else N
+00001410: 6f6e 6520 2320 666f 7220 7368 6f72 7465  one # for shorte
+00001420: 7220 7469 6d65 6672 616d 6573 2c20 7469  r timeframes, ti
+00001430: 6d65 7a6f 6e65 2073 6565 6d73 2062 7567  mezone seems bug
+00001440: 6779 0d0a 2020 2020 2020 2020 2020 2020  gy..            
+00001450: 2020 2020 726e 6720 3d20 7064 2e64 6174      rng = pd.dat
+00001460: 655f 7261 6e67 6528 7430 2c20 7431 2c20  e_range(t0, t1, 
+00001470: 747a 3d74 7a2c 206e 6f72 6d61 6c69 7a65  tz=tz, normalize
+00001480: 3d74 6f5f 6d69 646e 6967 6874 2c20 6672  =to_midnight, fr
+00001490: 6571 3d66 7265 7129 0d0a 2020 2020 2020  eq=freq)..      
+000014a0: 2020 2020 2020 2020 2020 7374 6570 7320            steps 
+000014b0: 3d20 6c65 6e28 726e 6729 2069 6620 6c65  = len(rng) if le
+000014c0: 6e28 726e 6729 2631 3d3d 3020 656c 7365  n(rng)&1==0 else
+000014d0: 206c 656e 2872 6e67 292b 3120 2320 7265   len(rng)+1 # re
+000014e0: 6475 6365 206a 6974 7465 7220 6265 7477  duce jitter betw
+000014f0: 6565 6e20 652e 672e 2035 3c2d 2d3e 3130  een e.g. 5<-->10
+00001500: 2074 6963 6b73 2066 6f72 2072 6573 6f6c   ticks for resol
+00001510: 7574 696f 6e20 636c 6f73 6520 746f 206c  ution close to l
+00001520: 696d 6974 0d0a 2020 2020 2020 2020 2020  imit..          
+00001530: 2020 2020 2020 7374 6570 203d 2069 6e74        step = int
+00001540: 2873 7465 7073 2f64 6573 6972 6564 5f74  (steps/desired_t
+00001550: 6963 6b73 2920 6f72 2031 0d0a 2020 2020  icks) or 1..    
+00001560: 2020 2020 2020 2020 2020 2020 726e 6720              rng 
+00001570: 3d20 726e 675b 3a3a 7374 6570 5d0d 0a20  = rng[::step].. 
+00001580: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001590: 6620 6e6f 7420 746f 5f6d 6964 6e69 6768  f not to_midnigh
+000015a0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+000015b0: 2020 2020 2020 2020 7472 793a 2020 2020          try:    
+000015c0: 726e 6720 3d20 726e 672e 726f 756e 6428  rng = rng.round(
+000015d0: 6672 6571 3d66 7265 7129 0d0a 2020 2020  freq=freq)..    
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 6578 6365 7074 3a20 7061 7373 0d0a 2020  except: pass..  
+00001600: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+00001610: 203d 2073 656c 662e 7662 2e70 6172 656e   = self.vb.paren
+00001620: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+00001630: 2020 2020 2072 6e67 203d 205f 7064 7469       rng = _pdti
+00001640: 6d65 3269 6e64 6578 2861 783d 6178 2c20  me2index(ax=ax, 
+00001650: 7473 3d70 642e 5365 7269 6573 2872 6e67  ts=pd.Series(rng
+00001660: 292c 2072 6571 7569 7265 5f74 696d 653d  ), require_time=
+00001670: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00001680: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+00001690: 205b 6365 696c 2869 2920 666f 7220 6920   [ceil(i) for i 
+000016a0: 696e 2072 6e67 5d0d 0a20 2020 2020 2020  in rng]..       
+000016b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000016c0: 5b28 302c 2069 6e64 6963 6573 295d 0d0a  [(0, indices)]..
+000016d0: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+000016e0: 2830 2c5b 5d29 5d0d 0a0d 0a20 2020 2064  (0,[])]....    d
+000016f0: 6566 2067 656e 6572 6174 6544 7261 7753  ef generateDrawS
+00001700: 7065 6373 2873 656c 662c 2070 293a 0d0a  pecs(self, p):..
+00001710: 2020 2020 2020 2020 7370 6563 7320 3d20          specs = 
+00001720: 7375 7065 7228 292e 6765 6e65 7261 7465  super().generate
+00001730: 4472 6177 5370 6563 7328 7029 0d0a 2020  DrawSpecs(p)..  
+00001740: 2020 2020 2020 6966 2073 7065 6373 3a0d        if specs:.
+00001750: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001760: 6e6f 7420 7365 6c66 2e73 7479 6c65 5b27  not self.style['
+00001770: 7368 6f77 5661 6c75 6573 275d 3a0d 0a20  showValues']:.. 
+00001780: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00001790: 656e 2c70 302c 7031 203d 2073 7065 6373  en,p0,p1 = specs
+000017a0: 5b30 5d20 2320 6178 6973 2073 7065 6373  [0] # axis specs
+000017b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017c0: 2020 7370 6563 7320 3d20 5b28 5f6d 616b    specs = [(_mak
+000017d0: 6570 656e 2827 2366 6666 3027 292c 7030  epen('#fff0'),p0
+000017e0: 2c70 3129 5d20 2b20 6c69 7374 2873 7065  ,p1)] + list(spe
+000017f0: 6373 5b31 3a5d 2920 2320 646f 6e27 7420  cs[1:]) # don't 
+00001800: 6472 6177 2061 7869 7320 6966 2068 6964  draw axis if hid
+00001810: 696e 6720 7661 6c75 6573 0d0a 2020 2020  ing values..    
+00001820: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00001830: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00001840: 2074 6872 6f77 206f 7574 2074 6963 6b73   throw out ticks
+00001850: 2074 6861 7420 6172 6520 6f75 7420 6f66   that are out of
+00001860: 2062 6f75 6e64 730d 0a20 2020 2020 2020   bounds..       
+00001870: 2020 2020 2020 2020 2074 6578 745f 7370           text_sp
+00001880: 6563 7320 3d20 7370 6563 735b 325d 0d0a  ecs = specs[2]..
 00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018a0: 2020 2069 6620 7265 6374 2e6c 6566 7428     if rect.left(
-000018b0: 2920 3c20 303a 0d0a 2020 2020 2020 2020  ) < 0:..        
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 6465 6c20 7465 7874 5f73 7065 6373 5b30  del text_specs[0
-000018e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000018f0: 2020 2020 2020 2072 6563 742c 666c 6167         rect,flag
-00001900: 732c 7465 7874 203d 2074 6578 745f 7370  s,text = text_sp
-00001910: 6563 735b 2d31 5d0d 0a20 2020 2020 2020  ecs[-1]..       
-00001920: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001930: 7265 6374 2e72 6967 6874 2829 203e 2073  rect.right() > s
-00001940: 656c 662e 6765 6f6d 6574 7279 2829 2e77  elf.geometry().w
-00001950: 6964 7468 2829 3a0d 0a20 2020 2020 2020  idth():..       
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2064 656c 2074 6578 745f 7370 6563 735b   del text_specs[
-00001980: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
-00001990: 2020 2020 2023 202e 2e2e 2061 6e64 2074       # ... and t
-000019a0: 686f 7365 2074 6861 7420 6f76 6572 6c61  hose that overla
-000019b0: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
-000019c0: 2020 2078 203d 2031 6536 0d0a 2020 2020     x = 1e6..    
-000019d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000019e0: 692c 2872 6563 742c 666c 6167 732c 7465  i,(rect,flags,te
-000019f0: 7874 2920 696e 2072 6576 6572 7365 6428  xt) in reversed(
-00001a00: 6c69 7374 2865 6e75 6d65 7261 7465 2874  list(enumerate(t
-00001a10: 6578 745f 7370 6563 7329 2929 3a0d 0a20  ext_specs))):.. 
-00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a30: 2020 2069 6620 7265 6374 2e72 6967 6874     if rect.right
-00001a40: 2829 203e 3d20 783a 0d0a 2020 2020 2020  () >= x:..      
-00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a60: 2020 6465 6c20 7465 7874 5f73 7065 6373    del text_specs
-00001a70: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00001a80: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 2020 2020 2020 7820 3d20 7265 6374          x = rect
-00001ab0: 2e6c 6566 7428 290d 0a20 2020 2020 2020  .left()..       
-00001ac0: 2072 6574 7572 6e20 7370 6563 730d 0a0d   return specs...
-00001ad0: 0a0d 0a0d 0a63 6c61 7373 2059 4178 6973  .....class YAxis
-00001ae0: 4974 656d 2870 672e 4178 6973 4974 656d  Item(pg.AxisItem
-00001af0: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-00001b00: 6974 5f5f 2873 656c 662c 2076 622c 202a  it__(self, vb, *
-00001b10: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-00001b20: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00001b30: 292e 5f5f 696e 6974 5f5f 282a 6172 6773  ).__init__(*args
-00001b40: 2c20 2a2a 6b77 6172 6773 290d 0a20 2020  , **kwargs)..   
-00001b50: 2020 2020 2073 656c 662e 7662 203d 2076       self.vb = v
-00001b60: 620d 0a20 2020 2020 2020 2073 656c 662e  b..        self.
-00001b70: 6869 6465 5f73 7472 696e 6773 203d 2046  hide_strings = F
-00001b80: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
-00001b90: 6c66 2e73 7479 6c65 5b27 6175 746f 4578  lf.style['autoEx
-00001ba0: 7061 6e64 5465 7874 5370 6163 6527 5d20  pandTextSpace'] 
-00001bb0: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-00001bc0: 2073 656c 662e 7374 796c 655b 2761 7574   self.style['aut
-00001bd0: 6f52 6564 7563 6554 6578 7453 7061 6365  oReduceTextSpace
-00001be0: 275d 203d 2046 616c 7365 0d0a 2020 2020  '] = False..    
-00001bf0: 2020 2020 7365 6c66 2e6e 6578 745f 666d      self.next_fm
-00001c00: 7420 3d20 2725 6727 0d0a 0d0a 2020 2020  t = '%g'....    
-00001c10: 6465 6620 7469 636b 5661 6c75 6573 2873  def tickValues(s
-00001c20: 656c 662c 206d 696e 5661 6c2c 206d 6178  elf, minVal, max
-00001c30: 5661 6c2c 2073 697a 6529 3a0d 0a20 2020  Val, size):..   
-00001c40: 2020 2020 2076 7320 3d20 7375 7065 7228       vs = super(
-00001c50: 292e 7469 636b 5661 6c75 6573 286d 696e  ).tickValues(min
-00001c60: 5661 6c2c 206d 6178 5661 6c2c 2073 697a  Val, maxVal, siz
-00001c70: 6529 0d0a 2020 2020 2020 2020 6966 206c  e)..        if l
-00001c80: 656e 2876 7329 203c 2033 3a0d 0a20 2020  en(vs) < 3:..   
-00001c90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001ca0: 7673 0d0a 2020 2020 2020 2020 7265 7475  vs..        retu
-00001cb0: 726e 2073 656c 662e 666d 745f 7661 6c75  rn self.fmt_valu
-00001cc0: 6573 2876 7329 0d0a 0d0a 2020 2020 6465  es(vs)....    de
-00001cd0: 6620 6c6f 6754 6963 6b56 616c 7565 7328  f logTickValues(
-00001ce0: 7365 6c66 2c20 6d69 6e56 616c 2c20 6d61  self, minVal, ma
-00001cf0: 7856 616c 2c20 7369 7a65 2c20 7374 6454  xVal, size, stdT
-00001d00: 6963 6b73 293a 0d0a 2020 2020 2020 2020  icks):..        
-00001d10: 7631 203d 2069 6e74 2866 6c6f 6f72 286d  v1 = int(floor(m
-00001d20: 696e 5661 6c29 290d 0a20 2020 2020 2020  inVal))..       
-00001d30: 2076 3220 3d20 696e 7428 6365 696c 286d   v2 = int(ceil(m
-00001d40: 6178 5661 6c29 290d 0a20 2020 2020 2020  axVal))..       
-00001d50: 206d 696e 6f72 203d 205b 5d0d 0a20 2020   minor = []..   
-00001d60: 2020 2020 2066 6f72 2076 2069 6e20 7261       for v in ra
-00001d70: 6e67 6528 7631 2c20 7632 293a 0d0a 2020  nge(v1, v2):..  
-00001d80: 2020 2020 2020 2020 2020 6d69 6e6f 722e            minor.
-00001d90: 6578 7465 6e64 285b 762b 6c20 666f 7220  extend([v+l for 
-00001da0: 6c20 696e 206e 702e 6c6f 6731 3028 6e70  l in np.log10(np
-00001db0: 2e6c 696e 7370 6163 6528 312c 2039 2e39  .linspace(1, 9.9
-00001dc0: 2c20 3930 2929 5d29 0d0a 2020 2020 2020  , 90))])..      
-00001dd0: 2020 6d69 6e6f 7220 3d20 5b78 2066 6f72    minor = [x for
-00001de0: 2078 2069 6e20 6d69 6e6f 7220 6966 2078   x in minor if x
-00001df0: 3e6d 696e 5661 6c20 616e 6420 783c 6d61  >minVal and x<ma
-00001e00: 7856 616c 5d0d 0a20 2020 2020 2020 2069  xVal]..        i
-00001e10: 6620 6e6f 7420 6d69 6e6f 723a 0d0a 2020  f not minor:..  
-00001e20: 2020 2020 2020 2020 2020 6d69 6e6f 722e            minor.
-00001e30: 6578 7465 6e64 286e 702e 6765 6f6d 7370  extend(np.geomsp
-00001e40: 6163 6528 6d69 6e56 616c 2c20 6d61 7856  ace(minVal, maxV
-00001e50: 616c 2c20 3729 5b31 3a2d 315d 290d 0a20  al, 7)[1:-1]).. 
-00001e60: 2020 2020 2020 2069 6620 6c65 6e28 6d69         if len(mi
-00001e70: 6e6f 7229 203e 2031 303a 0d0a 2020 2020  nor) > 10:..    
-00001e80: 2020 2020 2020 2020 6d69 6e6f 7220 3d20          minor = 
-00001e90: 6d69 6e6f 725b 3a3a 6c65 6e28 6d69 6e6f  minor[::len(mino
-00001ea0: 7229 2f2f 355d 0d0a 2020 2020 2020 2020  r)//5]..        
-00001eb0: 7673 203d 205b 284e 6f6e 652c 206d 696e  vs = [(None, min
-00001ec0: 6f72 295d 0d0a 2020 2020 2020 2020 7265  or)]..        re
-00001ed0: 7475 726e 2073 656c 662e 666d 745f 7661  turn self.fmt_va
-00001ee0: 6c75 6573 2876 7329 0d0a 0d0a 2020 2020  lues(vs)....    
-00001ef0: 6465 6620 7469 636b 5374 7269 6e67 7328  def tickStrings(
-00001f00: 7365 6c66 2c20 7661 6c75 6573 2c20 7363  self, values, sc
-00001f10: 616c 652c 2073 7061 6369 6e67 293a 0d0a  ale, spacing):..
-00001f20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001f30: 6869 6465 5f73 7472 696e 6773 3a0d 0a20  hide_strings:.. 
-00001f40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001f50: 6e20 5b5d 0d0a 2020 2020 2020 2020 7866  n []..        xf
-00001f60: 6f72 6d20 3d20 7365 6c66 2e76 622e 7973  orm = self.vb.ys
-00001f70: 6361 6c65 2e78 666f 726d 0d0a 2020 2020  cale.xform..    
-00001f80: 2020 2020 7265 7475 726e 205b 7365 6c66      return [self
-00001f90: 2e6e 6578 745f 666d 7425 7866 6f72 6d28  .next_fmt%xform(
-00001fa0: 7661 6c75 6529 2066 6f72 2076 616c 7565  value) for value
-00001fb0: 2069 6e20 7661 6c75 6573 5d0d 0a0d 0a20   in values].... 
-00001fc0: 2020 2064 6566 2066 6d74 5f76 616c 7565     def fmt_value
-00001fd0: 7328 7365 6c66 2c20 7673 293a 0d0a 2020  s(self, vs):..  
-00001fe0: 2020 2020 2020 7866 6f72 6d20 3d20 7365        xform = se
-00001ff0: 6c66 2e76 622e 7973 6361 6c65 2e78 666f  lf.vb.yscale.xfo
-00002000: 726d 0d0a 2020 2020 2020 2020 6773 203d  rm..        gs =
-00002010: 205b 2725 6727 2578 666f 726d 2876 2920   ['%g'%xform(v) 
-00002020: 666f 7220 7620 696e 2076 735b 2d31 5d5b  for v in vs[-1][
-00002030: 315d 5d0d 0a20 2020 2020 2020 2069 6620  1]]..        if 
-00002040: 6e6f 7420 6773 3a0d 0a20 2020 2020 2020  not gs:..       
-00002050: 2020 2020 2072 6574 7572 6e20 7673 0d0a       return vs..
-00002060: 2020 2020 2020 2020 6966 2061 6e79 285b          if any([
-00002070: 2765 2720 696e 2067 2066 6f72 2067 2069  'e' in g for g i
-00002080: 6e20 6773 5d29 3a0d 0a20 2020 2020 2020  n gs]):..       
-00002090: 2020 2020 206d 6178 6465 6320 3d20 6d61       maxdec = ma
-000020a0: 7828 5b6c 656e 2828 6729 2e70 6172 7469  x([len((g).parti
-000020b0: 7469 6f6e 2827 2e27 295b 325d 2e70 6172  tion('.')[2].par
-000020c0: 7469 7469 6f6e 2827 6527 295b 305d 2920  tition('e')[0]) 
-000020d0: 666f 7220 6720 696e 2067 7320 6966 2027  for g in gs if '
-000020e0: 6527 2069 6e20 675d 290d 0a20 2020 2020  e' in g])..     
-000020f0: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
-00002100: 5f66 6d74 203d 2027 2525 2e25 6965 2720  _fmt = '%%.%ie' 
-00002110: 2520 6d61 7864 6563 0d0a 2020 2020 2020  % maxdec..      
-00002120: 2020 656c 6966 2067 733a 0d0a 2020 2020    elif gs:..    
-00002130: 2020 2020 2020 2020 6d61 7864 6563 203d          maxdec =
-00002140: 206d 6178 285b 6c65 6e28 2867 292e 7061   max([len((g).pa
-00002150: 7274 6974 696f 6e28 272e 2729 5b32 5d29  rtition('.')[2])
-00002160: 2066 6f72 2067 2069 6e20 6773 5d29 0d0a   for g in gs])..
-00002170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002180: 2e6e 6578 745f 666d 7420 3d20 2725 252e  .next_fmt = '%%.
-00002190: 2569 6627 2025 206d 6178 6465 630d 0a20  %if' % maxdec.. 
-000021a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000021b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000021c0: 6578 745f 666d 7420 3d20 2725 6727 0d0a  ext_fmt = '%g'..
-000021d0: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-000021e0: 730d 0a0d 0a0d 0a0d 0a63 6c61 7373 2059  s........class Y
-000021f0: 5363 616c 653a 0d0a 2020 2020 6465 6620  Scale:..    def 
-00002200: 5f5f 696e 6974 5f5f 2873 656c 662c 2073  __init__(self, s
-00002210: 6361 6c65 7479 7065 2c20 7363 616c 6566  caletype, scalef
-00002220: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-00002230: 2e73 6361 6c65 7479 7065 203d 2073 6361  .scaletype = sca
-00002240: 6c65 7479 7065 0d0a 2020 2020 2020 2020  letype..        
-00002250: 7365 6c66 2e73 6574 5f73 6361 6c65 2873  self.set_scale(s
-00002260: 6361 6c65 6629 0d0a 0d0a 2020 2020 6465  calef)....    de
-00002270: 6620 7365 745f 7363 616c 6528 7365 6c66  f set_scale(self
-00002280: 2c20 7363 616c 6529 3a0d 0a20 2020 2020  , scale):..     
-00002290: 2020 2073 656c 662e 7363 616c 6566 203d     self.scalef =
-000022a0: 2073 6361 6c65 0d0a 0d0a 2020 2020 6465   scale....    de
-000022b0: 6620 7866 6f72 6d28 7365 6c66 2c20 7929  f xform(self, y)
-000022c0: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
-000022d0: 6c66 2e73 6361 6c65 7479 7065 203d 3d20  lf.scaletype == 
-000022e0: 276c 6f67 273a 0d0a 2020 2020 2020 2020  'log':..        
-000022f0: 2020 2020 7920 3d20 3130 2a2a 790d 0a20      y = 10**y.. 
-00002300: 2020 2020 2020 2079 203d 2079 202a 2073         y = y * s
-00002310: 656c 662e 7363 616c 6566 0d0a 2020 2020  elf.scalef..    
-00002320: 2020 2020 7265 7475 726e 2079 0d0a 0d0a      return y....
-00002330: 2020 2020 6465 6620 696e 7678 666f 726d      def invxform
-00002340: 2873 656c 662c 2079 2c20 7665 7269 6679  (self, y, verify
-00002350: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
-00002360: 2020 7920 2f3d 2073 656c 662e 7363 616c    y /= self.scal
-00002370: 6566 0d0a 2020 2020 2020 2020 6966 2073  ef..        if s
-00002380: 656c 662e 7363 616c 6574 7970 6520 3d3d  elf.scaletype ==
-00002390: 2027 6c6f 6727 3a0d 0a20 2020 2020 2020   'log':..       
-000023a0: 2020 2020 2069 6620 7665 7269 6679 2061       if verify a
-000023b0: 6e64 2079 203c 3d20 303a 0d0a 2020 2020  nd y <= 0:..    
-000023c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000023d0: 726e 202d 3165 3620 2f20 7365 6c66 2e73  rn -1e6 / self.s
-000023e0: 6361 6c65 660d 0a20 2020 2020 2020 2020  calef..         
-000023f0: 2020 2079 203d 206e 702e 6c6f 6731 3028     y = np.log10(
-00002400: 7929 0d0a 2020 2020 2020 2020 7265 7475  y)..        retu
-00002410: 726e 2079 0d0a 0d0a 0d0a 0d0a 636c 6173  rn y........clas
-00002420: 7320 5061 6e64 6173 4461 7461 536f 7572  s PandasDataSour
-00002430: 6365 3a0d 0a20 2020 2027 2727 4361 6e64  ce:..    '''Cand
-00002440: 6c65 2073 7469 636b 733a 2063 7265 6174  le sticks: creat
-00002450: 6520 7769 7468 2066 6976 6520 636f 6c75  e with five colu
-00002460: 6d6e 733a 2074 696d 652c 206f 7065 6e2c  mns: time, open,
-00002470: 2063 6c6f 7365 2c20 6869 2c20 6c6f 202d   close, hi, lo -
-00002480: 2069 6e20 7468 6174 206f 7264 6572 2e0d   in that order..
-00002490: 0a20 2020 2020 2020 566f 6c75 6d65 2062  .       Volume b
-000024a0: 6172 733a 2063 7265 6174 6520 7769 7468  ars: create with
-000024b0: 2074 6872 6565 2063 6f6c 756d 6e73 3a20   three columns: 
-000024c0: 7469 6d65 2c20 6f70 656e 2c20 636c 6f73  time, open, clos
-000024d0: 652c 2076 6f6c 756d 6520 2d20 696e 2074  e, volume - in t
-000024e0: 6861 7420 6f72 6465 722e 0d0a 2020 2020  hat order...    
-000024f0: 2020 2046 6f72 2061 6c6c 206f 7468 6572     For all other
-00002500: 2074 7970 6573 2c20 7469 6d65 206e 6565   types, time nee
-00002510: 6473 2074 6f20 6265 2066 6972 7374 2c20  ds to be first, 
-00002520: 7573 7561 6c6c 7920 666f 6c6c 6f77 6564  usually followed
-00002530: 2062 7920 6f6e 6520 6f72 206d 6f72 6520   by one or more 
-00002540: 592d 636f 6c75 6d6e 732e 2727 270d 0a20  Y-columns.'''.. 
-00002550: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00002560: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
-00002570: 2020 2020 6966 2074 7970 6528 6466 2e69      if type(df.i
-00002580: 6e64 6578 2920 3d3d 2070 642e 4461 7465  ndex) == pd.Date
-00002590: 7469 6d65 496e 6465 7820 6f72 2064 662e  timeIndex or df.
-000025a0: 696e 6465 785b 2d31 5d3e 3165 3720 6f72  index[-1]>1e7 or
-000025b0: 2027 2e52 616e 6765 496e 6465 7827 206e   '.RangeIndex' n
-000025c0: 6f74 2069 6e20 7374 7228 7479 7065 2864  ot in str(type(d
-000025d0: 662e 696e 6465 7829 293a 0d0a 2020 2020  f.index)):..    
-000025e0: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
-000025f0: 7265 7365 745f 696e 6465 7828 290d 0a20  reset_index().. 
-00002600: 2020 2020 2020 2073 656c 662e 6466 203d         self.df =
-00002610: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
-00002620: 2020 2020 2320 6d61 6e61 6765 2074 696d      # manage tim
-00002630: 6520 636f 6c75 6d6e 0d0a 2020 2020 2020  e column..      
-00002640: 2020 6966 205f 6861 735f 7469 6d65 636f    if _has_timeco
-00002650: 6c28 7365 6c66 2e64 6629 3a0d 0a20 2020  l(self.df):..   
-00002660: 2020 2020 2020 2020 2074 696d 6563 6f6c           timecol
-00002670: 203d 2073 656c 662e 6466 2e63 6f6c 756d   = self.df.colum
-00002680: 6e73 5b30 5d0d 0a20 2020 2020 2020 2020  ns[0]..         
-00002690: 2020 2064 7479 7065 203d 2073 7472 2864     dtype = str(d
-000026a0: 665b 7469 6d65 636f 6c5d 2e64 7479 7065  f[timecol].dtype
-000026b0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-000026c0: 736e 756d 203d 2028 2769 6e74 2720 696e  snum = ('int' in
-000026d0: 2064 7479 7065 206f 7220 2766 6c6f 6174   dtype or 'float
-000026e0: 2720 696e 2064 7479 7065 2920 616e 6420  ' in dtype) and 
-000026f0: 6466 5b74 696d 6563 6f6c 5d2e 696c 6f63  df[timecol].iloc
-00002700: 5b2d 315d 203c 2031 6537 0d0a 2020 2020  [-1] < 1e7..    
-00002710: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00002720: 736e 756d 3a0d 0a20 2020 2020 2020 2020  snum:..         
-00002730: 2020 2020 2020 2073 656c 662e 6466 5b74         self.df[t
-00002740: 696d 6563 6f6c 5d20 3d20 5f70 6474 696d  imecol] = _pdtim
-00002750: 6532 6570 6f63 6828 6466 5b74 696d 6563  e2epoch(df[timec
-00002760: 6f6c 5d29 0d0a 2020 2020 2020 2020 2020  ol])..          
-00002770: 2020 7365 6c66 2e73 7461 6e64 616c 6f6e    self.standalon
-00002780: 6520 3d20 5f69 735f 7374 616e 6461 6c6f  e = _is_standalo
-00002790: 6e65 2873 656c 662e 6466 5b74 696d 6563  ne(self.df[timec
-000027a0: 6f6c 5d29 0d0a 2020 2020 2020 2020 2020  ol])..          
-000027b0: 2020 7365 6c66 2e63 6f6c 5f64 6174 615f    self.col_data_
-000027c0: 6f66 6673 6574 203d 2031 2023 206e 6f2e  offset = 1 # no.
-000027d0: 206f 6620 7072 6563 6565 6469 6e67 2063   of preceeding c
-000027e0: 6f6c 756d 6e73 2066 6f72 206f 7468 6572  olumns for other
-000027f0: 2070 6c6f 7473 2061 6e64 2074 696d 6520   plots and time 
-00002800: 636f 6c75 6d6e 0d0a 2020 2020 2020 2020  column..        
-00002810: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00002820: 2020 2073 656c 662e 7374 616e 6461 6c6f     self.standalo
-00002830: 6e65 203d 2046 616c 7365 0d0a 2020 2020  ne = False..    
-00002840: 2020 2020 2020 2020 7365 6c66 2e63 6f6c          self.col
-00002850: 5f64 6174 615f 6f66 6673 6574 203d 2030  _data_offset = 0
-00002860: 2023 206e 6f2e 206f 6620 7072 6563 6565   # no. of precee
-00002870: 6469 6e67 2063 6f6c 756d 6e73 2066 6f72  ding columns for
-00002880: 206f 7468 6572 2070 6c6f 7473 2061 6e64   other plots and
-00002890: 2074 696d 6520 636f 6c75 6d6e 0d0a 2020   time column..  
-000028a0: 2020 2020 2020 2320 7365 7475 7020 6461        # setup da
-000028b0: 7461 2066 6f72 206a 6f69 6e69 6e67 2064  ta for joining d
-000028c0: 6174 6120 736f 7572 6365 7320 616e 6420  ata sources and 
-000028d0: 7a6f 6f6d 696e 670d 0a20 2020 2020 2020  zooming..       
-000028e0: 2073 656c 662e 7363 616c 655f 636f 6c73   self.scale_cols
-000028f0: 203d 205b 6920 666f 7220 6920 696e 2072   = [i for i in r
-00002900: 616e 6765 2873 656c 662e 636f 6c5f 6461  ange(self.col_da
-00002910: 7461 5f6f 6666 7365 742c 6c65 6e28 7365  ta_offset,len(se
-00002920: 6c66 2e64 662e 636f 6c75 6d6e 7329 2920  lf.df.columns)) 
-00002930: 6966 2073 656c 662e 6466 2e69 6c6f 635b  if self.df.iloc[
-00002940: 3a2c 695d 2e64 7479 7065 213d 6f62 6a65  :,i].dtype!=obje
-00002950: 6374 5d0d 0a20 2020 2020 2020 2073 656c  ct]..        sel
-00002960: 662e 6361 6368 655f 6869 6c6f 203d 204f  f.cache_hilo = O
-00002970: 7264 6572 6564 4469 6374 2829 0d0a 2020  rderedDict()..  
-00002980: 2020 2020 2020 7365 6c66 2e72 656e 616d        self.renam
-00002990: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-000029a0: 206e 6577 636f 6c73 203d 205b 5d0d 0a20   newcols = [].. 
-000029b0: 2020 2020 2020 2066 6f72 2063 6f6c 2069         for col i
-000029c0: 6e20 7365 6c66 2e64 662e 636f 6c75 6d6e  n self.df.column
-000029d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000029e0: 6f6c 6463 6f6c 203d 2063 6f6c 0d0a 2020  oldcol = col..  
-000029f0: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-00002a00: 636f 6c20 696e 206e 6577 636f 6c73 3a0d  col in newcols:.
-00002a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a20: 2063 6f6c 203d 2073 7472 2863 6f6c 292b   col = str(col)+
-00002a30: 272b 270d 0a20 2020 2020 2020 2020 2020  '+'..           
-00002a40: 206e 6577 636f 6c73 2e61 7070 656e 6428   newcols.append(
-00002a50: 636f 6c29 0d0a 2020 2020 2020 2020 2020  col)..          
-00002a60: 2020 6966 206f 6c64 636f 6c20 213d 2063    if oldcol != c
-00002a70: 6f6c 3a0d 0a20 2020 2020 2020 2020 2020  ol:..           
-00002a80: 2020 2020 2073 656c 662e 7265 6e61 6d65       self.rename
-00002a90: 735b 6f6c 6463 6f6c 5d20 3d20 636f 6c0d  s[oldcol] = col.
-00002aa0: 0a20 2020 2020 2020 2073 656c 662e 6466  .        self.df
-00002ab0: 2e63 6f6c 756d 6e73 203d 206e 6577 636f  .columns = newco
-00002ac0: 6c73 0d0a 2020 2020 2020 2020 7365 6c66  ls..        self
-00002ad0: 2e70 7265 5f75 7064 6174 6520 3d20 6c61  .pre_update = la
-00002ae0: 6d62 6461 2064 663a 2064 660d 0a20 2020  mbda df: df..   
-00002af0: 2020 2020 2073 656c 662e 706f 7374 5f75       self.post_u
-00002b00: 7064 6174 6520 3d20 6c61 6d62 6461 2064  pdate = lambda d
-00002b10: 663a 2064 660d 0a20 2020 2020 2020 2073  f: df..        s
-00002b20: 656c 662e 5f70 6572 696f 6420 3d20 4e6f  elf._period = No
-00002b30: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
-00002b40: 2e5f 736d 6f6f 7468 5f74 696d 6520 3d20  ._smooth_time = 
-00002b50: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
-00002b60: 6c66 2e69 735f 7370 6172 7365 203d 2073  lf.is_sparse = s
-00002b70: 656c 662e 6466 5b73 656c 662e 6466 2e63  elf.df[self.df.c
-00002b80: 6f6c 756d 6e73 5b73 656c 662e 636f 6c5f  olumns[self.col_
-00002b90: 6461 7461 5f6f 6666 7365 745d 5d2e 6973  data_offset]].is
-00002ba0: 6e75 6c6c 2829 2e73 756d 2829 2e6d 6178  null().sum().max
-00002bb0: 2829 203e 206c 656e 2873 656c 662e 6466  () > len(self.df
-00002bc0: 292f 2f32 0d0a 0d0a 2020 2020 4070 726f  )//2....    @pro
-00002bd0: 7065 7274 790d 0a20 2020 2064 6566 2070  perty..    def p
-00002be0: 6572 696f 645f 6e73 2873 656c 6629 3a0d  eriod_ns(self):.
-00002bf0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00002c00: 7365 6c66 2e64 6629 203c 3d20 313a 0d0a  self.df) <= 1:..
-00002c10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002c20: 726e 2031 0d0a 2020 2020 2020 2020 6966  rn 1..        if
-00002c30: 206e 6f74 2073 656c 662e 5f70 6572 696f   not self._perio
-00002c40: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-00002c50: 7469 6d65 636f 6c20 3d20 7365 6c66 2e64  timecol = self.d
-00002c60: 662e 636f 6c75 6d6e 735b 305d 0d0a 2020  f.columns[0]..  
-00002c70: 2020 2020 2020 2020 2020 7469 6d65 7320            times 
-00002c80: 3d20 7365 6c66 2e64 665b 7469 6d65 636f  = self.df[timeco
-00002c90: 6c5d 2e69 6c6f 635b 303a 3130 305d 0d0a  l].iloc[0:100]..
-00002ca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002cb0: 2e5f 7065 7269 6f64 203d 2069 6e74 2874  ._period = int(t
-00002cc0: 696d 6573 2e64 6966 6628 292e 6d65 6469  imes.diff().medi
-00002cd0: 616e 2829 2920 6966 206c 656e 2874 696d  an()) if len(tim
-00002ce0: 6573 293e 3120 656c 7365 2031 0d0a 2020  es)>1 else 1..  
-00002cf0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002d00: 662e 5f70 6572 696f 640d 0a0d 0a20 2020  f._period....   
-00002d10: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00002d20: 6465 6620 696e 6465 7828 7365 6c66 293a  def index(self):
-00002d30: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002d40: 2073 656c 662e 6466 2e69 6e64 6578 0d0a   self.df.index..
-00002d50: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00002d60: 0a20 2020 2064 6566 2078 2873 656c 6629  .    def x(self)
-00002d70: 3a0d 0a20 2020 2020 2020 2074 696d 6563  :..        timec
-00002d80: 6f6c 203d 2073 656c 662e 6466 2e63 6f6c  ol = self.df.col
-00002d90: 756d 6e73 5b30 5d0d 0a20 2020 2020 2020  umns[0]..       
-00002da0: 2072 6574 7572 6e20 7365 6c66 2e64 665b   return self.df[
-00002db0: 7469 6d65 636f 6c5d 0d0a 0d0a 2020 2020  timecol]....    
-00002dc0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
-00002dd0: 6566 2079 2873 656c 6629 3a0d 0a20 2020  ef y(self):..   
-00002de0: 2020 2020 2063 6f6c 203d 2073 656c 662e       col = self.
-00002df0: 6466 2e63 6f6c 756d 6e73 5b73 656c 662e  df.columns[self.
-00002e00: 636f 6c5f 6461 7461 5f6f 6666 7365 745d  col_data_offset]
-00002e10: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002e20: 2073 656c 662e 6466 5b63 6f6c 5d0d 0a0d   self.df[col]...
-00002e30: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00002e40: 2020 2020 6465 6620 7a28 7365 6c66 293a      def z(self):
-00002e50: 0d0a 2020 2020 2020 2020 636f 6c20 3d20  ..        col = 
-00002e60: 7365 6c66 2e64 662e 636f 6c75 6d6e 735b  self.df.columns[
-00002e70: 7365 6c66 2e63 6f6c 5f64 6174 615f 6f66  self.col_data_of
-00002e80: 6673 6574 2b31 5d0d 0a20 2020 2020 2020  fset+1]..       
-00002e90: 2072 6574 7572 6e20 7365 6c66 2e64 665b   return self.df[
-00002ea0: 636f 6c5d 0d0a 0d0a 2020 2020 4070 726f  col]....    @pro
-00002eb0: 7065 7274 790d 0a20 2020 2064 6566 2078  perty..    def x
-00002ec0: 6c65 6e28 7365 6c66 293a 0d0a 2020 2020  len(self):..    
-00002ed0: 2020 2020 7265 7475 726e 206c 656e 2873      return len(s
-00002ee0: 656c 662e 6466 290d 0a0d 0a20 2020 2064  elf.df)....    d
-00002ef0: 6566 2063 616c 635f 7369 676e 6966 6963  ef calc_signific
-00002f00: 616e 745f 6465 6369 6d61 6c73 2873 656c  ant_decimals(sel
-00002f10: 6629 3a0d 0a20 2020 2020 2020 2073 6572  f):..        ser
-00002f20: 203d 2073 656c 662e 7a20 6966 206c 656e   = self.z if len
-00002f30: 2873 656c 662e 7363 616c 655f 636f 6c73  (self.scale_cols
-00002f40: 293e 3120 656c 7365 2073 656c 662e 790d  )>1 else self.y.
-00002f50: 0a20 2020 2020 2020 2061 6273 6469 6666  .        absdiff
-00002f60: 203d 2073 6572 2e64 6966 6628 292e 6162   = ser.diff().ab
-00002f70: 7328 290d 0a20 2020 2020 2020 2061 6273  s()..        abs
-00002f80: 6469 6666 5b61 6273 6469 6666 3c31 652d  diff[absdiff<1e-
-00002f90: 3330 5d20 3d20 3165 3330 0d0a 2020 2020  30] = 1e30..    
-00002fa0: 2020 2020 6e75 6d20 3d20 736d 616c 6c65      num = smalle
-00002fb0: 7374 5f64 6966 6620 3d20 6162 7364 6966  st_diff = absdif
-00002fc0: 662e 6d69 6e28 290d 0a20 2020 2020 2020  f.min()..       
-00002fd0: 2066 6f72 205f 2069 6e20 7261 6e67 6528   for _ in range(
-00002fe0: 3229 3a0d 0a20 2020 2020 2020 2020 2020  2):..           
-00002ff0: 2073 203d 2027 2565 2720 2520 6e75 6d0d   s = '%e' % num.
-00003000: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-00003010: 652c 5f2c 6578 7020 3d20 732e 7061 7274  e,_,exp = s.part
-00003020: 6974 696f 6e28 2765 2729 0d0a 2020 2020  ition('e')..    
-00003030: 2020 2020 2020 2020 6261 7365 203d 2062          base = b
-00003040: 6173 652e 7273 7472 6970 2827 3027 290d  ase.rstrip('0').
-00003050: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-00003060: 203d 202d 696e 7428 6578 7029 0d0a 2020   = -int(exp)..  
-00003070: 2020 2020 2020 2020 2020 6d61 785f 6261            max_ba
-00003080: 7365 5f64 6563 696d 616c 7320 3d20 6d69  se_decimals = mi
-00003090: 6e28 352c 202d 6578 702b 3229 2069 6620  n(5, -exp+2) if 
-000030a0: 6578 7020 3c20 3020 656c 7365 2033 0d0a  exp < 0 else 3..
-000030b0: 2020 2020 2020 2020 2020 2020 6261 7365              base
-000030c0: 5f64 6563 696d 616c 7320 3d20 6d61 7828  _decimals = max(
-000030d0: 302c 206d 696e 286d 6178 5f62 6173 655f  0, min(max_base_
-000030e0: 6465 6369 6d61 6c73 2c20 6c65 6e28 6261  decimals, len(ba
-000030f0: 7365 292d 3229 290d 0a20 2020 2020 2020  se)-2))..       
-00003100: 2020 2020 2064 6563 696d 616c 7320 3d20       decimals = 
-00003110: 6578 7020 2b20 6261 7365 5f64 6563 696d  exp + base_decim
-00003120: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
-00003130: 2064 6563 696d 616c 7320 3d20 6d61 7828   decimals = max(
-00003140: 302c 206d 696e 2831 302c 2064 6563 696d  0, min(10, decim
-00003150: 616c 7329 290d 0a20 2020 2020 2020 2020  als))..         
-00003160: 2020 2069 6620 6465 6369 6d61 6c73 203c     if decimals <
-00003170: 3d20 333a 0d0a 2020 2020 2020 2020 2020  = 3:..          
-00003180: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
-00003190: 2020 2020 2020 2020 2023 2072 6574 7279           # retry
-000031a0: 2077 6974 6820 6675 6c6c 206e 756d 6265   with full numbe
-000031b0: 722c 2074 6f20 7365 6520 6966 2077 6520  r, to see if we 
-000031c0: 6361 6e20 6765 7420 7468 6520 6e75 6d62  can get the numb
-000031d0: 6572 206f 6620 6465 6369 6d61 6c73 2064  er of decimals d
-000031e0: 6f77 6e0d 0a20 2020 2020 2020 2020 2020  own..           
-000031f0: 206e 756d 203d 2073 6d61 6c6c 6573 745f   num = smallest_
-00003200: 6469 6666 202b 2061 6273 2873 6572 2e6d  diff + abs(ser.m
-00003210: 696e 2829 290d 0a20 2020 2020 2020 2073  in())..        s
-00003220: 6d61 6c6c 6573 745f 6469 6666 203d 206d  mallest_diff = m
-00003230: 6178 2831 302a 2a28 2d64 6563 696d 616c  ax(10**(-decimal
-00003240: 7329 2c20 736d 616c 6c65 7374 5f64 6966  s), smallest_dif
-00003250: 6629 0d0a 2020 2020 2020 2020 7265 7475  f)..        retu
-00003260: 726e 2064 6563 696d 616c 732c 2073 6d61  rn decimals, sma
-00003270: 6c6c 6573 745f 6469 6666 0d0a 0d0a 2020  llest_diff....  
-00003280: 2020 6465 6620 7570 6461 7465 5f69 6e69    def update_ini
-00003290: 745f 7828 7365 6c66 2c20 696e 6974 5f73  t_x(self, init_s
-000032a0: 7465 7073 293a 0d0a 2020 2020 2020 2020  teps):..        
-000032b0: 7365 6c66 2e69 6e69 745f 7830 2c20 7365  self.init_x0, se
-000032c0: 6c66 2e69 6e69 745f 7831 203d 205f 786d  lf.init_x1 = _xm
-000032d0: 696e 6d61 7828 7365 6c66 2c20 785f 696e  inmax(self, x_in
-000032e0: 6465 7865 643d 5472 7565 2c20 696e 6974  dexed=True, init
-000032f0: 5f73 7465 7073 3d69 6e69 745f 7374 6570  _steps=init_step
-00003300: 7329 0d0a 0d0a 2020 2020 6465 6620 636c  s)....    def cl
-00003310: 6f73 6573 745f 7469 6d65 2873 656c 662c  osest_time(self,
-00003320: 2078 293a 0d0a 2020 2020 2020 2020 7469   x):..        ti
-00003330: 6d65 636f 6c20 3d20 7365 6c66 2e64 662e  mecol = self.df.
-00003340: 636f 6c75 6d6e 735b 305d 0d0a 2020 2020  columns[0]..    
-00003350: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00003360: 6466 2e6c 6f63 5b69 6e74 2878 292c 2074  df.loc[int(x), t
-00003370: 696d 6563 6f6c 5d0d 0a0d 0a20 2020 2064  imecol]....    d
-00003380: 6566 2074 696d 6562 6173 6564 2873 656c  ef timebased(sel
-00003390: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-000033a0: 7572 6e20 7365 6c66 2e64 662e 696c 6f63  urn self.df.iloc
-000033b0: 5b2d 312c 305d 203e 2031 6537 0d0a 0d0a  [-1,0] > 1e7....
-000033c0: 2020 2020 6465 6620 6973 5f73 6d6f 6f74      def is_smoot
-000033d0: 685f 7469 6d65 2873 656c 6629 3a0d 0a20  h_time(self):.. 
-000033e0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-000033f0: 736d 6f6f 7468 5f74 696d 6520 6973 204e  smooth_time is N
-00003400: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00003410: 2020 2320 6c65 7373 2074 6861 6e20 3125    # less than 1%
-00003420: 2074 696d 6520 6465 6c74 6120 6973 2073   time delta is s
-00003430: 6d6f 6f74 680d 0a20 2020 2020 2020 2020  mooth..         
-00003440: 2020 2073 656c 662e 5f73 6d6f 6f74 685f     self._smooth_
-00003450: 7469 6d65 203d 2073 656c 662e 7469 6d65  time = self.time
-00003460: 6261 7365 6428 2920 616e 6420 286e 702e  based() and (np.
-00003470: 6162 7328 6e70 2e64 6966 6628 7365 6c66  abs(np.diff(self
-00003480: 2e78 2e76 616c 7565 735b 313a 3130 305d  .x.values[1:100]
-00003490: 295b 313a 5d2f 2f28 7365 6c66 2e70 6572  )[1:]//(self.per
-000034a0: 696f 645f 6e73 2f2f 3130 3030 292d 3130  iod_ns//1000)-10
-000034b0: 3030 2920 3c20 3130 292e 616c 6c28 290d  00) < 10).all().
-000034c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000034d0: 7365 6c66 2e5f 736d 6f6f 7468 5f74 696d  self._smooth_tim
-000034e0: 650d 0a0d 0a20 2020 2064 6566 2061 6464  e....    def add
-000034f0: 636f 6c73 2873 656c 662c 2064 6174 6173  cols(self, datas
-00003500: 7263 293a 0d0a 2020 2020 2020 2020 6e65  rc):..        ne
-00003510: 775f 7363 616c 655f 636f 6c73 203d 205b  w_scale_cols = [
-00003520: 632b 6c65 6e28 7365 6c66 2e64 662e 636f  c+len(self.df.co
-00003530: 6c75 6d6e 7329 2d64 6174 6173 7263 2e63  lumns)-datasrc.c
-00003540: 6f6c 5f64 6174 615f 6f66 6673 6574 2066  ol_data_offset f
-00003550: 6f72 2063 2069 6e20 6461 7461 7372 632e  or c in datasrc.
-00003560: 7363 616c 655f 636f 6c73 5d0d 0a20 2020  scale_cols]..   
-00003570: 2020 2020 2073 656c 662e 7363 616c 655f       self.scale_
-00003580: 636f 6c73 202b 3d20 6e65 775f 7363 616c  cols += new_scal
-00003590: 655f 636f 6c73 0d0a 2020 2020 2020 2020  e_cols..        
-000035a0: 6f72 6967 5f63 6f6c 5f64 6174 615f 636e  orig_col_data_cn
-000035b0: 7420 3d20 6c65 6e28 7365 6c66 2e64 662e  t = len(self.df.
-000035c0: 636f 6c75 6d6e 7329 0d0a 2020 2020 2020  columns)..      
-000035d0: 2020 6966 205f 6861 735f 7469 6d65 636f    if _has_timeco
-000035e0: 6c28 6461 7461 7372 632e 6466 293a 0d0a  l(datasrc.df):..
-000035f0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00003600: 636f 6c20 3d20 7365 6c66 2e64 662e 636f  col = self.df.co
-00003610: 6c75 6d6e 735b 305d 0d0a 2020 2020 2020  lumns[0]..      
-00003620: 2020 2020 2020 6466 203d 2073 656c 662e        df = self.
-00003630: 6466 2e73 6574 5f69 6e64 6578 2874 696d  df.set_index(tim
-00003640: 6563 6f6c 290d 0a20 2020 2020 2020 2020  ecol)..         
-00003650: 2020 2074 696d 6563 6f6c 203d 2074 696d     timecol = tim
-00003660: 6563 6f6c 2069 6620 7469 6d65 636f 6c20  ecol if timecol 
-00003670: 696e 2064 6174 6173 7263 2e64 662e 636f  in datasrc.df.co
-00003680: 6c75 6d6e 7320 656c 7365 2064 6174 6173  lumns else datas
-00003690: 7263 2e64 662e 636f 6c75 6d6e 735b 305d  rc.df.columns[0]
-000036a0: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
-000036b0: 7763 6f6c 7320 3d20 6461 7461 7372 632e  wcols = datasrc.
-000036c0: 6466 2e73 6574 5f69 6e64 6578 2874 696d  df.set_index(tim
-000036d0: 6563 6f6c 290d 0a20 2020 2020 2020 2065  ecol)..        e
-000036e0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000036f0: 2020 6466 203d 2073 656c 662e 6466 0d0a    df = self.df..
-00003700: 2020 2020 2020 2020 2020 2020 6e65 7763              newc
-00003710: 6f6c 7320 3d20 6461 7461 7372 632e 6466  ols = datasrc.df
-00003720: 0d0a 2020 2020 2020 2020 636f 6c73 203d  ..        cols =
-00003730: 206c 6973 7428 6e65 7763 6f6c 732e 636f   list(newcols.co
-00003740: 6c75 6d6e 7329 0d0a 2020 2020 2020 2020  lumns)..        
-00003750: 666f 7220 692c 636f 6c20 696e 2065 6e75  for i,col in enu
-00003760: 6d65 7261 7465 2863 6f6c 7329 3a0d 0a20  merate(cols):.. 
-00003770: 2020 2020 2020 2020 2020 206f 6c64 5f63             old_c
-00003780: 6f6c 203d 2063 6f6c 0d0a 2020 2020 2020  ol = col..      
-00003790: 2020 2020 2020 7768 696c 6520 636f 6c20        while col 
-000037a0: 696e 2073 656c 662e 6466 2e63 6f6c 756d  in self.df.colum
-000037b0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-000037c0: 2020 2020 2063 6f6c 735b 695d 203d 2063       cols[i] = c
-000037d0: 6f6c 203d 2073 7472 2863 6f6c 292b 272b  ol = str(col)+'+
-000037e0: 270d 0a20 2020 2020 2020 2020 2020 2069  '..            i
-000037f0: 6620 6f6c 645f 636f 6c20 213d 2063 6f6c  f old_col != col
-00003800: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003810: 2020 2064 6174 6173 7263 2e72 656e 616d     datasrc.renam
-00003820: 6573 5b6f 6c64 5f63 6f6c 5d20 3d20 636f  es[old_col] = co
-00003830: 6c0d 0a20 2020 2020 2020 206e 6577 636f  l..        newco
-00003840: 6c73 2e63 6f6c 756d 6e73 203d 2063 6f6c  ls.columns = col
-00003850: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00003860: 6466 203d 2064 662e 6a6f 696e 286e 6577  df = df.join(new
-00003870: 636f 6c73 2c20 686f 773d 276f 7574 6572  cols, how='outer
-00003880: 2729 0d0a 2020 2020 2020 2020 6966 205f  ')..        if _
-00003890: 6861 735f 7469 6d65 636f 6c28 6461 7461  has_timecol(data
-000038a0: 7372 632e 6466 293a 0d0a 2020 2020 2020  src.df):..      
-000038b0: 2020 2020 2020 7365 6c66 2e64 662e 7265        self.df.re
-000038c0: 7365 745f 696e 6465 7828 696e 706c 6163  set_index(inplac
-000038d0: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
-000038e0: 2064 6174 6173 7263 2e64 6620 3d20 7365   datasrc.df = se
-000038f0: 6c66 2e64 6620 2320 7468 6579 2061 7265  lf.df # they are
-00003900: 2074 6865 2073 616d 6520 6e6f 770d 0a20   the same now.. 
-00003910: 2020 2020 2020 2064 6174 6173 7263 2e69         datasrc.i
-00003920: 6e69 745f 7830 203d 2073 656c 662e 696e  nit_x0 = self.in
-00003930: 6974 5f78 300d 0a20 2020 2020 2020 2064  it_x0..        d
-00003940: 6174 6173 7263 2e69 6e69 745f 7831 203d  atasrc.init_x1 =
-00003950: 2073 656c 662e 696e 6974 5f78 310d 0a20   self.init_x1.. 
-00003960: 2020 2020 2020 2064 6174 6173 7263 2e63         datasrc.c
-00003970: 6f6c 5f64 6174 615f 6f66 6673 6574 203d  ol_data_offset =
-00003980: 206f 7269 675f 636f 6c5f 6461 7461 5f63   orig_col_data_c
-00003990: 6e74 0d0a 2020 2020 2020 2020 6461 7461  nt..        data
-000039a0: 7372 632e 7363 616c 655f 636f 6c73 203d  src.scale_cols =
-000039b0: 206e 6577 5f73 6361 6c65 5f63 6f6c 730d   new_scale_cols.
-000039c0: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-000039d0: 6368 655f 6869 6c6f 203d 204f 7264 6572  che_hilo = Order
-000039e0: 6564 4469 6374 2829 0d0a 2020 2020 2020  edDict()..      
-000039f0: 2020 7365 6c66 2e5f 7065 7269 6f64 203d    self._period =
-00003a00: 2073 656c 662e 5f73 6d6f 6f74 685f 7469   self._smooth_ti
-00003a10: 6d65 203d 204e 6f6e 650d 0a20 2020 2020  me = None..     
-00003a20: 2020 2064 6174 6173 7263 2e5f 7065 7269     datasrc._peri
-00003a30: 6f64 203d 2064 6174 6173 7263 2e5f 736d  od = datasrc._sm
-00003a40: 6f6f 7468 5f74 696d 6520 3d20 4e6f 6e65  ooth_time = None
-00003a50: 0d0a 2020 2020 2020 2020 6c64 6632 203d  ..        ldf2 =
-00003a60: 206c 656e 2873 656c 662e 6466 2920 2f20   len(self.df) / 
-00003a70: 320d 0a20 2020 2020 2020 2073 656c 662e  2..        self.
-00003a80: 6973 5f73 7061 7273 6520 3d20 7365 6c66  is_sparse = self
-00003a90: 2e69 735f 7370 6172 7365 206f 7220 7365  .is_sparse or se
-00003aa0: 6c66 2e64 665b 7365 6c66 2e64 662e 636f  lf.df[self.df.co
-00003ab0: 6c75 6d6e 735b 7365 6c66 2e63 6f6c 5f64  lumns[self.col_d
-00003ac0: 6174 615f 6f66 6673 6574 5d5d 2e69 736e  ata_offset]].isn
-00003ad0: 756c 6c28 292e 7375 6d28 292e 6d61 7828  ull().sum().max(
-00003ae0: 2920 3e20 6c64 6632 0d0a 2020 2020 2020  ) > ldf2..      
-00003af0: 2020 6461 7461 7372 632e 6973 5f73 7061    datasrc.is_spa
-00003b00: 7273 6520 3d20 6461 7461 7372 632e 6973  rse = datasrc.is
-00003b10: 5f73 7061 7273 6520 6f72 2064 6174 6173  _sparse or datas
-00003b20: 7263 2e64 665b 6461 7461 7372 632e 6466  rc.df[datasrc.df
-00003b30: 2e63 6f6c 756d 6e73 5b64 6174 6173 7263  .columns[datasrc
-00003b40: 2e63 6f6c 5f64 6174 615f 6f66 6673 6574  .col_data_offset
-00003b50: 5d5d 2e69 736e 756c 6c28 292e 7375 6d28  ]].isnull().sum(
-00003b60: 292e 6d61 7828 2920 3e20 6c64 6632 0d0a  ).max() > ldf2..
-00003b70: 0d0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
-00003b80: 2873 656c 662c 2064 6174 6173 7263 293a  (self, datasrc):
-00003b90: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
-00003ba0: 656c 662e 7072 655f 7570 6461 7465 2873  elf.pre_update(s
-00003bb0: 656c 662e 6466 290d 0a20 2020 2020 2020  elf.df)..       
-00003bc0: 206f 7269 675f 636f 6c73 203d 206c 6973   orig_cols = lis
-00003bd0: 7428 6466 2e63 6f6c 756d 6e73 290d 0a20  t(df.columns).. 
-00003be0: 2020 2020 2020 2074 696d 6563 6f6c 2c6f         timecol,o
-00003bf0: 7269 675f 636f 6c73 203d 206f 7269 675f  rig_cols = orig_
-00003c00: 636f 6c73 5b30 5d2c 6f72 6967 5f63 6f6c  cols[0],orig_col
-00003c10: 735b 313a 5d0d 0a20 2020 2020 2020 2064  s[1:]..        d
-00003c20: 6620 3d20 6466 2e73 6574 5f69 6e64 6578  f = df.set_index
-00003c30: 2874 696d 6563 6f6c 290d 0a20 2020 2020  (timecol)..     
-00003c40: 2020 2069 6e70 7574 5f64 6620 3d20 6461     input_df = da
-00003c50: 7461 7372 632e 6466 2e73 6574 5f69 6e64  tasrc.df.set_ind
-00003c60: 6578 2864 6174 6173 7263 2e64 662e 636f  ex(datasrc.df.co
-00003c70: 6c75 6d6e 735b 305d 290d 0a20 2020 2020  lumns[0])..     
-00003c80: 2020 2069 6e70 7574 5f64 662e 636f 6c75     input_df.colu
-00003c90: 6d6e 7320 3d20 5b73 656c 662e 7265 6e61  mns = [self.rena
-00003ca0: 6d65 732e 6765 7428 636f 6c2c 2063 6f6c  mes.get(col, col
-00003cb0: 2920 666f 7220 636f 6c20 696e 2069 6e70  ) for col in inp
-00003cc0: 7574 5f64 662e 636f 6c75 6d6e 735d 0d0a  ut_df.columns]..
-00003cd0: 2020 2020 2020 2020 2320 7061 6420 696e          # pad in
-00003ce0: 6465 7820 6966 2074 6865 2069 6e70 7574  dex if the input
-00003cf0: 2064 6174 6120 6973 2061 2073 7562 2d73   data is a sub-s
-00003d00: 6574 0d0a 2020 2020 2020 2020 6f75 7470  et..        outp
-00003d10: 7574 5f64 6620 3d20 7064 2e6d 6572 6765  ut_df = pd.merge
-00003d20: 2869 6e70 7574 5f64 662c 2064 665b 5b5d  (input_df, df[[]
-00003d30: 5d2c 2068 6f77 3d27 6f75 7465 7227 2c20  ], how='outer', 
-00003d40: 6c65 6674 5f69 6e64 6578 3d54 7275 652c  left_index=True,
-00003d50: 2072 6967 6874 5f69 6e64 6578 3d54 7275   right_index=Tru
-00003d60: 6529 0d0a 2020 2020 2020 2020 666f 7220  e)..        for 
-00003d70: 636f 6c20 696e 2064 662e 636f 6c75 6d6e  col in df.column
-00003d80: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00003d90: 6966 2063 6f6c 206e 6f74 2069 6e20 6f75  if col not in ou
-00003da0: 7470 7574 5f64 662e 636f 6c75 6d6e 733a  tput_df.columns:
-00003db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003dc0: 2020 6f75 7470 7574 5f64 665b 636f 6c5d    output_df[col]
-00003dd0: 203d 2064 665b 636f 6c5d 0d0a 2020 2020   = df[col]..    
-00003de0: 2020 2020 2320 6966 206e 6563 6365 7373      # if neccess
-00003df0: 6172 792c 2063 7574 206f 7574 2075 6e77  ary, cut out unw
-00003e00: 616e 7465 6420 6461 7461 0d0a 2020 2020  anted data..    
-00003e10: 2020 2020 6966 206c 656e 2869 6e70 7574      if len(input
-00003e20: 5f64 6629 203e 2030 2061 6e64 206c 656e  _df) > 0 and len
-00003e30: 2864 6629 203e 2030 3a0d 0a20 2020 2020  (df) > 0:..     
-00003e40: 2020 2020 2020 2073 7461 7274 5f69 6478         start_idx
-00003e50: 203d 2065 6e64 5f69 6478 203d 204e 6f6e   = end_idx = Non
-00003e60: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00003e70: 6620 696e 7075 745f 6466 2e69 6e64 6578  f input_df.index
-00003e80: 5b30 5d20 3e20 6466 2e69 6e64 6578 5b30  [0] > df.index[0
-00003e90: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
-00003ea0: 2020 2020 7374 6172 745f 6964 7820 3d20      start_idx = 
-00003eb0: 300d 0a20 2020 2020 2020 2020 2020 2069  0..            i
-00003ec0: 6620 696e 7075 745f 6466 2e69 6e64 6578  f input_df.index
-00003ed0: 5b2d 315d 203c 2064 662e 696e 6465 785b  [-1] < df.index[
-00003ee0: 2d31 5d3a 0d0a 2020 2020 2020 2020 2020  -1]:..          
-00003ef0: 2020 2020 2020 656e 645f 6964 7820 3d20        end_idx = 
-00003f00: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
-00003f10: 6966 2073 7461 7274 5f69 6478 2069 7320  if start_idx is 
-00003f20: 6e6f 7420 4e6f 6e65 206f 7220 656e 645f  not None or end_
-00003f30: 6964 7820 6973 206e 6f74 204e 6f6e 653a  idx is not None:
-00003f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003f50: 2020 6f75 7470 7574 5f64 6620 3d20 6f75    output_df = ou
-00003f60: 7470 7574 5f64 662e 6c6f 635b 696e 7075  tput_df.loc[inpu
-00003f70: 745f 6466 2e69 6e64 6578 5b73 7461 7274  t_df.index[start
-00003f80: 5f69 6478 3a65 6e64 5f69 6478 5d2c 203a  _idx:end_idx], :
-00003f90: 5d0d 0a20 2020 2020 2020 206f 7574 7075  ]..        outpu
-00003fa0: 745f 6466 203d 2073 656c 662e 706f 7374  t_df = self.post
-00003fb0: 5f75 7064 6174 6528 6f75 7470 7574 5f64  _update(output_d
-00003fc0: 6629 0d0a 2020 2020 2020 2020 6f75 7470  f)..        outp
-00003fd0: 7574 5f64 6620 3d20 6f75 7470 7574 5f64  ut_df = output_d
-00003fe0: 662e 7265 7365 745f 696e 6465 7828 290d  f.reset_index().
-00003ff0: 0a20 2020 2020 2020 2073 656c 662e 6466  .        self.df
-00004000: 203d 206f 7574 7075 745f 6466 5b5b 6f75   = output_df[[ou
-00004010: 7470 7574 5f64 662e 636f 6c75 6d6e 735b  tput_df.columns[
-00004020: 305d 5d2b 6f72 6967 5f63 6f6c 735d 2069  0]]+orig_cols] i
-00004030: 6620 6f72 6967 5f63 6f6c 7320 656c 7365  f orig_cols else
-00004040: 2069 6e70 7574 5f64 660d 0a20 2020 2020   input_df..     
-00004050: 2020 2073 656c 662e 696e 6974 5f78 3120     self.init_x1 
-00004060: 3d20 7365 6c66 2e78 6c65 6e20 2b20 7269  = self.xlen + ri
-00004070: 6768 745f 6d61 7267 696e 5f63 616e 646c  ght_margin_candl
-00004080: 6573 202d 2073 6964 655f 6d61 7267 696e  es - side_margin
-00004090: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-000040a0: 6163 6865 5f68 696c 6f20 3d20 4f72 6465  ache_hilo = Orde
-000040b0: 7265 6444 6963 7428 290d 0a20 2020 2020  redDict()..     
-000040c0: 2020 2073 656c 662e 5f70 6572 696f 6420     self._period 
-000040d0: 3d20 7365 6c66 2e5f 736d 6f6f 7468 5f74  = self._smooth_t
-000040e0: 696d 6520 3d20 4e6f 6e65 0d0a 0d0a 2020  ime = None....  
-000040f0: 2020 6465 6620 7365 745f 6466 2873 656c    def set_df(sel
-00004100: 662c 2064 6629 3a0d 0a20 2020 2020 2020  f, df):..       
-00004110: 2073 656c 662e 6466 203d 2064 660d 0a20   self.df = df.. 
-00004120: 2020 2020 2020 2073 656c 662e 6361 6368         self.cach
-00004130: 655f 6869 6c6f 203d 204f 7264 6572 6564  e_hilo = Ordered
-00004140: 4469 6374 2829 0d0a 2020 2020 2020 2020  Dict()..        
-00004150: 7365 6c66 2e5f 7065 7269 6f64 203d 2073  self._period = s
-00004160: 656c 662e 5f73 6d6f 6f74 685f 7469 6d65  elf._smooth_time
-00004170: 203d 204e 6f6e 650d 0a0d 0a20 2020 2064   = None....    d
-00004180: 6566 2068 696c 6f28 7365 6c66 2c20 7830  ef hilo(self, x0
-00004190: 2c20 7831 293a 0d0a 2020 2020 2020 2020  , x1):..        
-000041a0: 2727 2752 6574 7572 6e20 6669 7665 2076  '''Return five v
-000041b0: 616c 7565 7320 696e 2074 696d 6520 7261  alues in time ra
-000041c0: 6e67 653a 2074 302c 2074 312c 2068 6967  nge: t0, t1, hig
-000041d0: 6865 7374 2c20 6c6f 7765 7374 2c20 6e75  hest, lowest, nu
-000041e0: 6d62 6572 206f 6620 726f 7773 2e27 2727  mber of rows.'''
-000041f0: 0d0a 2020 2020 2020 2020 6966 2078 3020  ..        if x0 
-00004200: 3d3d 2078 313a 0d0a 2020 2020 2020 2020  == x1:..        
-00004210: 2020 2020 7830 203d 2078 3120 3d20 696e      x0 = x1 = in
-00004220: 7428 7831 290d 0a20 2020 2020 2020 2065  t(x1)..        e
-00004230: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00004240: 2020 7830 2c78 3120 3d20 696e 7428 7830    x0,x1 = int(x0
-00004250: 2b30 2e35 292c 696e 7428 7831 290d 0a20  +0.5),int(x1).. 
-00004260: 2020 2020 2020 2071 7565 7279 203d 2027         query = '
-00004270: 2569 2c25 6927 2025 2028 7830 2c78 3129  %i,%i' % (x0,x1)
-00004280: 0d0a 2020 2020 2020 2020 6966 2071 7565  ..        if que
-00004290: 7279 206e 6f74 2069 6e20 7365 6c66 2e63  ry not in self.c
-000042a0: 6163 6865 5f68 696c 6f3a 0d0a 2020 2020  ache_hilo:..    
-000042b0: 2020 2020 2020 2020 7620 3d20 7365 6c66          v = self
-000042c0: 2e63 6163 6865 5f68 696c 6f5b 7175 6572  .cache_hilo[quer
-000042d0: 795d 203d 2073 656c 662e 5f68 696c 6f28  y] = self._hilo(
-000042e0: 7830 2c20 7831 290d 0a20 2020 2020 2020  x0, x1)..       
-000042f0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00004300: 2020 2020 2320 7265 2d69 6e73 6572 7420      # re-insert 
-00004310: 746f 2072 6169 7365 2070 7269 6f0d 0a20  to raise prio.. 
-00004320: 2020 2020 2020 2020 2020 2076 203d 2073             v = s
-00004330: 656c 662e 6361 6368 655f 6869 6c6f 5b71  elf.cache_hilo[q
-00004340: 7565 7279 5d20 3d20 7365 6c66 2e63 6163  uery] = self.cac
-00004350: 6865 5f68 696c 6f2e 706f 7028 7175 6572  he_hilo.pop(quer
-00004360: 7929 0d0a 2020 2020 2020 2020 6966 206c  y)..        if l
-00004370: 656e 2873 656c 662e 6361 6368 655f 6869  en(self.cache_hi
-00004380: 6c6f 2920 3e20 3130 303a 2023 2064 726f  lo) > 100: # dro
-00004390: 7020 6966 2074 6f6f 206d 616e 790d 0a20  p if too many.. 
-000043a0: 2020 2020 2020 2020 2020 2064 656c 2073             del s
-000043b0: 656c 662e 6361 6368 655f 6869 6c6f 5b6e  elf.cache_hilo[n
-000043c0: 6578 7428 6974 6572 2873 656c 662e 6361  ext(iter(self.ca
-000043d0: 6368 655f 6869 6c6f 2929 5d0d 0a20 2020  che_hilo))]..   
-000043e0: 2020 2020 2072 6574 7572 6e20 760d 0a0d       return v...
-000043f0: 0a20 2020 2064 6566 205f 6869 6c6f 2873  .    def _hilo(s
-00004400: 656c 662c 2078 302c 2078 3129 3a0d 0a20  elf, x0, x1):.. 
-00004410: 2020 2020 2020 2064 6620 3d20 7365 6c66         df = self
-00004420: 2e64 662e 6c6f 635b 7830 3a78 312c 203a  .df.loc[x0:x1, :
-00004430: 5d0d 0a20 2020 2020 2020 2069 6620 6e6f  ]..        if no
-00004440: 7420 6c65 6e28 6466 293a 0d0a 2020 2020  t len(df):..    
-00004450: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
-00004460: 2c30 2c30 2c30 2c30 0d0a 2020 2020 2020  ,0,0,0,0..      
-00004470: 2020 7469 6d65 636f 6c20 3d20 6466 2e63    timecol = df.c
-00004480: 6f6c 756d 6e73 5b30 5d0d 0a20 2020 2020  olumns[0]..     
-00004490: 2020 2074 3020 3d20 6466 5b74 696d 6563     t0 = df[timec
-000044a0: 6f6c 5d2e 696c 6f63 5b30 5d0d 0a20 2020  ol].iloc[0]..   
-000044b0: 2020 2020 2074 3120 3d20 6466 5b74 696d       t1 = df[tim
-000044c0: 6563 6f6c 5d2e 696c 6f63 5b2d 315d 0d0a  ecol].iloc[-1]..
-000044d0: 2020 2020 2020 2020 7661 6c63 6f6c 7320          valcols 
-000044e0: 3d20 6466 2e63 6f6c 756d 6e73 5b73 656c  = df.columns[sel
-000044f0: 662e 7363 616c 655f 636f 6c73 5d0d 0a20  f.scale_cols].. 
-00004500: 2020 2020 2020 2068 6920 3d20 6466 5b76         hi = df[v
-00004510: 616c 636f 6c73 5d2e 6d61 7828 292e 6d61  alcols].max().ma
-00004520: 7828 290d 0a20 2020 2020 2020 206c 6f20  x()..        lo 
-00004530: 3d20 6466 5b76 616c 636f 6c73 5d2e 6d69  = df[valcols].mi
-00004540: 6e28 292e 6d69 6e28 290d 0a20 2020 2020  n().min()..     
-00004550: 2020 2072 6574 7572 6e20 7430 2c74 312c     return t0,t1,
-00004560: 6869 2c6c 6f2c 6c65 6e28 6466 290d 0a0d  hi,lo,len(df)...
-00004570: 0a20 2020 2064 6566 2072 6f77 7328 7365  .    def rows(se
-00004580: 6c66 2c20 636f 6c63 6e74 2c20 7830 2c20  lf, colcnt, x0, 
-00004590: 7831 2c20 7973 6361 6c65 2c20 6c6f 643d  x1, yscale, lod=
-000045a0: 5472 7565 293a 0d0a 2020 2020 2020 2020  True):..        
-000045b0: 6466 203d 2073 656c 662e 6466 2e6c 6f63  df = self.df.loc
-000045c0: 5b78 303a 7831 2c20 3a5d 0d0a 2020 2020  [x0:x1, :]..    
-000045d0: 2020 2020 6966 2073 656c 662e 6973 5f73      if self.is_s
-000045e0: 7061 7273 653a 0d0a 2020 2020 2020 2020  parse:..        
-000045f0: 2020 2020 6466 203d 2064 662e 6c6f 635b      df = df.loc[
-00004600: 6466 2e69 6c6f 635b 3a2c 7365 6c66 2e63  df.iloc[:,self.c
-00004610: 6f6c 5f64 6174 615f 6f66 6673 6574 5d2e  ol_data_offset].
-00004620: 6e6f 746e 6128 292c 203a 5d0d 0a20 2020  notna(), :]..   
-00004630: 2020 2020 206f 7269 676c 656e 203d 206c       origlen = l
-00004640: 656e 2864 6629 0d0a 2020 2020 2020 2020  en(df)..        
-00004650: 7265 7475 726e 2073 656c 662e 5f72 6f77  return self._row
-00004660: 7328 6466 2c20 636f 6c63 6e74 2c20 7973  s(df, colcnt, ys
-00004670: 6361 6c65 3d79 7363 616c 652c 206c 6f64  cale=yscale, lod
-00004680: 3d6c 6f64 292c 206f 7269 676c 656e 0d0a  =lod), origlen..
-00004690: 0d0a 2020 2020 6465 6620 5f72 6f77 7328  ..    def _rows(
-000046a0: 7365 6c66 2c20 6466 2c20 636f 6c63 6e74  self, df, colcnt
-000046b0: 2c20 7973 6361 6c65 2c20 6c6f 6429 3a0d  , yscale, lod):.
-000046c0: 0a20 2020 2020 2020 2069 6620 6c6f 6420  .        if lod 
-000046d0: 616e 6420 6c65 6e28 6466 2920 3e20 6c6f  and len(df) > lo
-000046e0: 645f 6361 6e64 6c65 733a 0d0a 2020 2020  d_candles:..    
-000046f0: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
-00004700: 696c 6f63 5b3a 3a6c 656e 2864 6629 2f2f  iloc[::len(df)//
-00004710: 6c6f 645f 6361 6e64 6c65 735d 0d0a 2020  lod_candles]..  
-00004720: 2020 2020 2020 636f 6c63 6e74 202d 3d20        colcnt -= 
-00004730: 3120 2320 7469 6d65 2069 7320 616c 7761  1 # time is alwa
-00004740: 7973 2069 6d70 6c69 6564 0d0a 2020 2020  ys implied..    
-00004750: 2020 2020 636f 6c69 6478 7320 3d20 5b30      colidxs = [0
-00004760: 5d20 2b20 6c69 7374 2872 616e 6765 2873  ] + list(range(s
-00004770: 656c 662e 636f 6c5f 6461 7461 5f6f 6666  elf.col_data_off
-00004780: 7365 742c 2073 656c 662e 636f 6c5f 6461  set, self.col_da
-00004790: 7461 5f6f 6666 7365 742b 636f 6c63 6e74  ta_offset+colcnt
-000047a0: 2929 0d0a 2020 2020 2020 2020 6466 7220  ))..        dfr 
-000047b0: 3d20 6466 2e69 6c6f 635b 3a2c 636f 6c69  = df.iloc[:,coli
-000047c0: 6478 735d 0d0a 2020 2020 2020 2020 6966  dxs]..        if
-000047d0: 2079 7363 616c 652e 7363 616c 6574 7970   yscale.scaletyp
-000047e0: 6520 3d3d 2027 6c6f 6727 206f 7220 7973  e == 'log' or ys
-000047f0: 6361 6c65 2e73 6361 6c65 6620 213d 2031  cale.scalef != 1
-00004800: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-00004810: 6672 203d 2064 6672 2e63 6f70 7928 290d  fr = dfr.copy().
-00004820: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00004830: 2069 2069 6e20 7261 6e67 6528 312c 2063   i in range(1, c
-00004840: 6f6c 636e 742b 3129 3a0d 0a20 2020 2020  olcnt+1):..     
-00004850: 2020 2020 2020 2020 2020 2063 6f6c 6e61             colna
-00004860: 6d65 203d 2064 6672 2e63 6f6c 756d 6e73  me = dfr.columns
-00004870: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00004880: 2020 2020 2069 6620 6466 725b 636f 6c6e       if dfr[coln
-00004890: 616d 655d 2e64 7479 7065 2021 3d20 6f62  ame].dtype != ob
-000048a0: 6a65 6374 3a0d 0a20 2020 2020 2020 2020  ject:..         
-000048b0: 2020 2020 2020 2020 2020 2064 6672 5b63             dfr[c
-000048c0: 6f6c 6e61 6d65 5d20 3d20 7973 6361 6c65  olname] = yscale
-000048d0: 2e69 6e76 7866 6f72 6d28 6466 722e 696c  .invxform(dfr.il
-000048e0: 6f63 5b3a 2c69 5d29 0d0a 2020 2020 2020  oc[:,i])..      
-000048f0: 2020 7265 7475 726e 2064 6672 0d0a 0d0a    return dfr....
-00004900: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
-00004910: 656c 662c 206f 7468 6572 293a 0d0a 2020  elf, other):..  
-00004920: 2020 2020 2020 7265 7475 726e 2069 6428        return id(
-00004930: 7365 6c66 2920 3d3d 2069 6428 6f74 6865  self) == id(othe
-00004940: 7229 206f 7220 6964 2873 656c 662e 6466  r) or id(self.df
-00004950: 2920 3d3d 2069 6428 6f74 6865 722e 6466  ) == id(other.df
-00004960: 290d 0a0d 0a20 2020 2064 6566 205f 5f68  )....    def __h
-00004970: 6173 685f 5f28 7365 6c66 293a 0d0a 2020  ash__(self):..  
-00004980: 2020 2020 2020 7265 7475 726e 2069 6428        return id(
-00004990: 7365 6c66 290d 0a0d 0a0d 0a63 6c61 7373  self)......class
-000049a0: 2046 696e 5769 6e64 6f77 2870 672e 4772   FinWindow(pg.Gr
-000049b0: 6170 6869 6373 4c61 796f 7574 5769 6467  aphicsLayoutWidg
-000049c0: 6574 293a 0d0a 2020 2020 6465 6620 5f5f  et):..    def __
-000049d0: 696e 6974 5f5f 2873 656c 662c 2074 6974  init__(self, tit
-000049e0: 6c65 2c20 2a2a 6b77 6172 6773 293a 0d0a  le, **kwargs):..
-000049f0: 2020 2020 2020 2020 676c 6f62 616c 2077          global w
-00004a00: 696e 782c 2077 696e 790d 0a20 2020 2020  inx, winy..     
-00004a10: 2020 2073 656c 662e 7469 746c 6520 3d20     self.title = 
-00004a20: 7469 746c 650d 0a20 2020 2020 2020 2070  title..        p
-00004a30: 672e 6d6b 5141 7070 2829 0d0a 2020 2020  g.mkQApp()..    
-00004a40: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00004a50: 6974 5f5f 282a 2a6b 7761 7267 7329 0d0a  it__(**kwargs)..
-00004a60: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00004a70: 5769 6e64 6f77 5469 746c 6528 7469 746c  WindowTitle(titl
-00004a80: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00004a90: 2e73 6574 4765 6f6d 6574 7279 2877 696e  .setGeometry(win
-00004aa0: 782c 2077 696e 792c 2077 696e 772c 2077  x, winy, winw, w
-00004ab0: 696e 6829 0d0a 2020 2020 2020 2020 7769  inh)..        wi
-00004ac0: 6e78 202b 3d20 3430 0d0a 2020 2020 2020  nx += 40..      
-00004ad0: 2020 7769 6e79 202b 3d20 3430 0d0a 2020    winy += 40..  
-00004ae0: 2020 2020 2020 7365 6c66 2e63 656e 7472        self.centr
-00004af0: 616c 5769 6467 6574 2e69 6e73 7461 6c6c  alWidget.install
-00004b00: 4576 656e 7446 696c 7465 7228 7365 6c66  EventFilter(self
-00004b10: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004b20: 6369 2e73 6574 436f 6e74 656e 7473 4d61  ci.setContentsMa
-00004b30: 7267 696e 7328 302c 2030 2c20 302c 2030  rgins(0, 0, 0, 0
-00004b40: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004b50: 6369 2e73 6574 5370 6163 696e 6728 2d31  ci.setSpacing(-1
-00004b60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00004b70: 636c 6f73 696e 6720 3d20 4661 6c73 650d  closing = False.
-00004b80: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00004b90: 0d0a 2020 2020 6465 6620 6178 7328 7365  ..    def axs(se
-00004ba0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00004bb0: 7475 726e 205b 6178 2066 6f72 2061 7820  turn [ax for ax 
-00004bc0: 696e 2073 656c 662e 6369 2e69 7465 6d73  in self.ci.items
-00004bd0: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
-00004be0: 782c 2070 672e 506c 6f74 4974 656d 295d  x, pg.PlotItem)]
-00004bf0: 0d0a 0d0a 2020 2020 6465 6620 6175 746f  ....    def auto
-00004c00: 5261 6e67 6545 6e61 626c 6564 2873 656c  RangeEnabled(sel
-00004c10: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00004c20: 7572 6e20 5b54 7275 652c 2054 7275 655d  urn [True, True]
-00004c30: 0d0a 0d0a 2020 2020 6465 6620 636c 6f73  ....    def clos
-00004c40: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
-00004c50: 2020 7365 6c66 2e63 6c6f 7369 6e67 203d    self.closing =
-00004c60: 2054 7275 650d 0a20 2020 2020 2020 205f   True..        _
-00004c70: 7361 7665 7769 6e64 6174 6128 7365 6c66  savewindata(self
-00004c80: 290d 0a20 2020 2020 2020 205f 636c 6561  )..        _clea
-00004c90: 725f 7469 6d65 7273 2829 0d0a 2020 2020  r_timers()..    
-00004ca0: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-00004cb0: 2829 2e63 6c6f 7365 2829 0d0a 0d0a 2020  ().close()....  
-00004cc0: 2020 6465 6620 6576 656e 7446 696c 7465    def eventFilte
-00004cd0: 7228 7365 6c66 2c20 6f62 6a2c 2065 7629  r(self, obj, ev)
-00004ce0: 3a0d 0a20 2020 2020 2020 2069 6620 6576  :..        if ev
-00004cf0: 2e74 7970 6528 293d 3d20 5174 436f 7265  .type()== QtCore
-00004d00: 2e51 4576 656e 742e 5479 7065 2e57 696e  .QEvent.Type.Win
-00004d10: 646f 7744 6561 6374 6976 6174 653a 0d0a  dowDeactivate:..
-00004d20: 2020 2020 2020 2020 2020 2020 5f73 6176              _sav
-00004d30: 6577 696e 6461 7461 2873 656c 6629 0d0a  ewindata(self)..
-00004d40: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00004d50: 616c 7365 0d0a 0d0a 2020 2020 6465 6620  alse....    def 
-00004d60: 6c65 6176 6545 7665 6e74 2873 656c 662c  leaveEvent(self,
-00004d70: 2065 7629 3a0d 0a20 2020 2020 2020 2069   ev):..        i
-00004d80: 6620 6e6f 7420 7365 6c66 2e63 6c6f 7369  f not self.closi
-00004d90: 6e67 3a0d 0a20 2020 2020 2020 2020 2020  ng:..           
-00004da0: 2073 7570 6572 2829 2e6c 6561 7665 4576   super().leaveEv
-00004db0: 656e 7428 6576 290d 0a0d 0a0d 0a63 6c61  ent(ev)......cla
-00004dc0: 7373 2046 696e 4372 6f73 7348 6169 723a  ss FinCrossHair:
-00004dd0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00004de0: 5f5f 2873 656c 662c 2061 782c 2063 6f6c  __(self, ax, col
-00004df0: 6f72 293a 0d0a 2020 2020 2020 2020 7365  or):..        se
-00004e00: 6c66 2e61 7820 3d20 6178 0d0a 2020 2020  lf.ax = ax..    
-00004e10: 2020 2020 7365 6c66 2e78 203d 2030 0d0a      self.x = 0..
-00004e20: 2020 2020 2020 2020 7365 6c66 2e79 203d          self.y =
-00004e30: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
-00004e40: 2e63 6c61 6d70 5f78 203d 2030 0d0a 2020  .clamp_x = 0..  
-00004e50: 2020 2020 2020 7365 6c66 2e63 6c61 6d70        self.clamp
-00004e60: 5f79 203d 2030 0d0a 2020 2020 2020 2020  _y = 0..        
-00004e70: 7365 6c66 2e69 6e66 6f73 203d 205b 5d0d  self.infos = [].
-00004e80: 0a20 2020 2020 2020 2070 656e 203d 2070  .        pen = p
-00004e90: 672e 6d6b 5065 6e28 636f 6c6f 723d 636f  g.mkPen(color=co
-00004ea0: 6c6f 722c 2073 7479 6c65 3d51 7443 6f72  lor, style=QtCor
-00004eb0: 652e 5174 2e50 656e 5374 796c 652e 4375  e.Qt.PenStyle.Cu
-00004ec0: 7374 6f6d 4461 7368 4c69 6e65 2c20 6461  stomDashLine, da
-00004ed0: 7368 3d5b 372c 2037 5d29 0d0a 2020 2020  sh=[7, 7])..    
-00004ee0: 2020 2020 7365 6c66 2e76 6c69 6e65 203d      self.vline =
-00004ef0: 2070 672e 496e 6669 6e69 7465 4c69 6e65   pg.InfiniteLine
-00004f00: 2861 6e67 6c65 3d39 302c 206d 6f76 6162  (angle=90, movab
-00004f10: 6c65 3d46 616c 7365 2c20 7065 6e3d 7065  le=False, pen=pe
-00004f20: 6e29 0d0a 2020 2020 2020 2020 7365 6c66  n)..        self
-00004f30: 2e68 6c69 6e65 203d 2070 672e 496e 6669  .hline = pg.Infi
-00004f40: 6e69 7465 4c69 6e65 2861 6e67 6c65 3d30  niteLine(angle=0
-00004f50: 2c20 6d6f 7661 626c 653d 4661 6c73 652c  , movable=False,
-00004f60: 2070 656e 3d70 656e 290d 0a20 2020 2020   pen=pen)..     
-00004f70: 2020 2073 656c 662e 7874 6578 7420 3d20     self.xtext = 
-00004f80: 7067 2e54 6578 7449 7465 6d28 636f 6c6f  pg.TextItem(colo
-00004f90: 723d 636f 6c6f 722c 2061 6e63 686f 723d  r=color, anchor=
-00004fa0: 2830 2c31 2929 0d0a 2020 2020 2020 2020  (0,1))..        
-00004fb0: 7365 6c66 2e79 7465 7874 203d 2070 672e  self.ytext = pg.
-00004fc0: 5465 7874 4974 656d 2863 6f6c 6f72 3d63  TextItem(color=c
-00004fd0: 6f6c 6f72 2c20 616e 6368 6f72 3d28 302c  olor, anchor=(0,
-00004fe0: 3029 290d 0a20 2020 2020 2020 2073 656c  0))..        sel
-00004ff0: 662e 766c 696e 652e 7365 745a 5661 6c75  f.vline.setZValu
-00005000: 6528 3530 290d 0a20 2020 2020 2020 2073  e(50)..        s
-00005010: 656c 662e 686c 696e 652e 7365 745a 5661  elf.hline.setZVa
-00005020: 6c75 6528 3530 290d 0a20 2020 2020 2020  lue(50)..       
-00005030: 2073 656c 662e 7874 6578 742e 7365 745a   self.xtext.setZ
-00005040: 5661 6c75 6528 3530 290d 0a20 2020 2020  Value(50)..     
-00005050: 2020 2073 656c 662e 7974 6578 742e 7365     self.ytext.se
-00005060: 745a 5661 6c75 6528 3530 290d 0a20 2020  tZValue(50)..   
-00005070: 2020 2020 2073 656c 662e 7368 6f77 2829       self.show()
-00005080: 0d0a 0d0a 2020 2020 6465 6620 7570 6461  ....    def upda
-00005090: 7465 2873 656c 662c 2070 6f69 6e74 3d4e  te(self, point=N
-000050a0: 6f6e 6529 3a0d 0a20 2020 2020 2020 2069  one):..        i
-000050b0: 6620 706f 696e 7420 6973 206e 6f74 204e  f point is not N
-000050c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000050d0: 2020 7365 6c66 2e78 2c73 656c 662e 7920    self.x,self.y 
-000050e0: 3d20 782c 7920 3d20 706f 696e 742e 7828  = x,y = point.x(
-000050f0: 292c 706f 696e 742e 7928 290d 0a20 2020  ),point.y()..   
-00005100: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00005110: 2020 2020 2020 2020 782c 7920 3d20 7365          x,y = se
-00005120: 6c66 2e78 2c73 656c 662e 790d 0a20 2020  lf.x,self.y..   
-00005130: 2020 2020 2078 2c79 203d 205f 636c 616d       x,y = _clam
-00005140: 705f 7879 2873 656c 662e 6178 2c20 782c  p_xy(self.ax, x,
-00005150: 7929 0d0a 2020 2020 2020 2020 6966 2078  y)..        if x
-00005160: 203d 3d20 7365 6c66 2e63 6c61 6d70 5f78   == self.clamp_x
-00005170: 2061 6e64 2079 203d 3d20 7365 6c66 2e63   and y == self.c
-00005180: 6c61 6d70 5f79 3a0d 0a20 2020 2020 2020  lamp_y:..       
-00005190: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-000051a0: 2020 2020 2073 656c 662e 636c 616d 705f       self.clamp_
-000051b0: 782c 7365 6c66 2e63 6c61 6d70 5f79 203d  x,self.clamp_y =
-000051c0: 2078 2c79 0d0a 2020 2020 2020 2020 7365   x,y..        se
-000051d0: 6c66 2e76 6c69 6e65 2e73 6574 506f 7328  lf.vline.setPos(
-000051e0: 7829 0d0a 2020 2020 2020 2020 7365 6c66  x)..        self
-000051f0: 2e68 6c69 6e65 2e73 6574 506f 7328 7929  .hline.setPos(y)
-00005200: 0d0a 2020 2020 2020 2020 7365 6c66 2e78  ..        self.x
-00005210: 7465 7874 2e73 6574 506f 7328 782c 2079  text.setPos(x, y
-00005220: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00005230: 7974 6578 742e 7365 7450 6f73 2878 2c20  ytext.setPos(x, 
-00005240: 7929 0d0a 2020 2020 2020 2020 726e 6720  y)..        rng 
-00005250: 3d20 7365 6c66 2e61 782e 7662 2e79 5f6d  = self.ax.vb.y_m
-00005260: 6178 202d 2073 656c 662e 6178 2e76 622e  ax - self.ax.vb.
-00005270: 795f 6d69 6e0d 0a20 2020 2020 2020 2072  y_min..        r
-00005280: 6e67 6d61 7820 3d20 6162 7328 7365 6c66  ngmax = abs(self
-00005290: 2e61 782e 7662 2e79 5f6d 696e 2920 2b20  .ax.vb.y_min) + 
-000052a0: 726e 6720 2320 616e 7920 6170 7072 6f78  rng # any approx
-000052b0: 696d 6174 696f 6e20 6973 2066 696e 650d  imation is fine.
-000052c0: 0a20 2020 2020 2020 2073 642c 7365 203d  .        sd,se =
-000052d0: 2028 7365 6c66 2e61 782e 7369 676e 6966   (self.ax.signif
-000052e0: 6963 616e 745f 6465 6369 6d61 6c73 2c73  icant_decimals,s
-000052f0: 656c 662e 6178 2e73 6967 6e69 6669 6361  elf.ax.significa
-00005300: 6e74 5f65 7073 2920 6966 2063 6c61 6d70  nt_eps) if clamp
-00005310: 5f67 7269 6420 656c 7365 2028 7369 676e  _grid else (sign
-00005320: 6966 6963 616e 745f 6465 6369 6d61 6c73  ificant_decimals
-00005330: 2c73 6967 6e69 6669 6361 6e74 5f65 7073  ,significant_eps
-00005340: 290d 0a20 2020 2020 2020 2074 696d 6562  )..        timeb
-00005350: 6173 6564 203d 2046 616c 7365 0d0a 2020  ased = False..  
-00005360: 2020 2020 2020 6966 2073 656c 662e 6178        if self.ax
-00005370: 2e76 622e 785f 696e 6465 7865 643a 0d0a  .vb.x_indexed:..
-00005380: 2020 2020 2020 2020 2020 2020 7874 6578              xtex
-00005390: 742c 7469 6d65 6261 7365 6420 3d20 5f78  t,timebased = _x
-000053a0: 326c 6f63 616c 5f74 2873 656c 662e 6178  2local_t(self.ax
-000053b0: 2e76 622e 6461 7461 7372 632c 2078 290d  .vb.datasrc, x).
-000053c0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-000053d0: 2020 2020 2020 2020 2020 2020 7874 6578              xtex
-000053e0: 7420 3d20 5f72 6f75 6e64 5f74 6f5f 7369  t = _round_to_si
-000053f0: 676e 6966 6963 616e 7428 726e 672c 2072  gnificant(rng, r
-00005400: 6e67 6d61 782c 2078 2c20 7364 2c20 7365  ngmax, x, sd, se
-00005410: 290d 0a20 2020 2020 2020 206c 696e 6561  )..        linea
-00005420: 725f 7920 3d20 790d 0a20 2020 2020 2020  r_y = y..       
-00005430: 2079 203d 2073 656c 662e 6178 2e76 622e   y = self.ax.vb.
-00005440: 7973 6361 6c65 2e78 666f 726d 2879 290d  yscale.xform(y).
-00005450: 0a20 2020 2020 2020 2079 7465 7874 203d  .        ytext =
-00005460: 205f 726f 756e 645f 746f 5f73 6967 6e69   _round_to_signi
-00005470: 6669 6361 6e74 2872 6e67 2c20 726e 676d  ficant(rng, rngm
-00005480: 6178 2c20 792c 2073 642c 2073 6529 0d0a  ax, y, sd, se)..
-00005490: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
-000054a0: 696d 6562 6173 6564 3a0d 0a20 2020 2020  imebased:..     
-000054b0: 2020 2020 2020 2069 6620 7874 6578 743a         if xtext:
-000054c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000054d0: 2020 7874 6578 7420 3d20 2778 2027 202b    xtext = 'x ' +
-000054e0: 2078 7465 7874 0d0a 2020 2020 2020 2020   xtext..        
-000054f0: 2020 2020 7974 6578 7420 3d20 2779 2027      ytext = 'y '
-00005500: 202b 2079 7465 7874 0d0a 2020 2020 2020   + ytext..      
-00005510: 2020 6661 725f 7269 6768 7420 3d20 7365    far_right = se
-00005520: 6c66 2e61 782e 7669 6577 5265 6374 2829  lf.ax.viewRect()
-00005530: 2e78 2829 202b 2073 656c 662e 6178 2e76  .x() + self.ax.v
-00005540: 6965 7752 6563 7428 292e 7769 6474 6828  iewRect().width(
-00005550: 292a 302e 390d 0a20 2020 2020 2020 2066  )*0.9..        f
-00005560: 6172 5f62 6f74 746f 6d20 3d20 7365 6c66  ar_bottom = self
-00005570: 2e61 782e 7669 6577 5265 6374 2829 2e79  .ax.viewRect().y
-00005580: 2829 202b 2073 656c 662e 6178 2e76 6965  () + self.ax.vie
-00005590: 7752 6563 7428 292e 6865 6967 6874 2829  wRect().height()
-000055a0: 2a30 2e31 0d0a 2020 2020 2020 2020 636c  *0.1..        cl
-000055b0: 6f73 6532 7269 6768 7420 3d20 7820 3e20  ose2right = x > 
-000055c0: 6661 725f 7269 6768 740d 0a20 2020 2020  far_right..     
-000055d0: 2020 2063 6c6f 7365 3262 6f74 746f 6d20     close2bottom 
-000055e0: 3d20 6c69 6e65 6172 5f79 203c 2066 6172  = linear_y < far
-000055f0: 5f62 6f74 746f 6d0d 0a20 2020 2020 2020  _bottom..       
-00005600: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00005610: 2020 2066 6f72 2069 6e66 6f20 696e 2073     for info in s
-00005620: 656c 662e 696e 666f 733a 0d0a 2020 2020  elf.infos:..    
-00005630: 2020 2020 2020 2020 2020 2020 7874 6578              xtex
-00005640: 742c 7974 6578 7420 3d20 696e 666f 2878  t,ytext = info(x
-00005650: 2c79 2c78 7465 7874 2c79 7465 7874 290d  ,y,xtext,ytext).
-00005660: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00005670: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-00005680: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00005690: 6e74 2827 4372 6f73 7368 6169 7220 6572  nt('Crosshair er
-000056a0: 726f 723a 272c 2074 7970 6528 6529 2c20  ror:', type(e), 
-000056b0: 6529 0d0a 2020 2020 2020 2020 7370 6163  e)..        spac
-000056c0: 6520 3d20 2720 2020 2020 2027 0d0a 2020  e = '      '..  
-000056d0: 2020 2020 2020 6966 2063 6c6f 7365 3272        if close2r
-000056e0: 6967 6874 3a0d 0a20 2020 2020 2020 2020  ight:..         
-000056f0: 2020 2078 7465 7874 203d 2078 7465 7874     xtext = xtext
-00005700: 202b 2073 7061 6365 0d0a 2020 2020 2020   + space..      
-00005710: 2020 2020 2020 7974 6578 7420 3d20 7974        ytext = yt
-00005720: 6578 7420 2b20 7370 6163 650d 0a20 2020  ext + space..   
-00005730: 2020 2020 2020 2020 2078 616e 6368 6f72           xanchor
-00005740: 203d 205b 312c 315d 0d0a 2020 2020 2020   = [1,1]..      
-00005750: 2020 2020 2020 7961 6e63 686f 7220 3d20        yanchor = 
-00005760: 5b31 2c30 5d0d 0a20 2020 2020 2020 2065  [1,0]..        e
-00005770: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00005780: 2020 7874 6578 7420 3d20 7370 6163 6520    xtext = space 
-00005790: 2b20 7874 6578 740d 0a20 2020 2020 2020  + xtext..       
-000057a0: 2020 2020 2079 7465 7874 203d 2073 7061       ytext = spa
-000057b0: 6365 202b 2079 7465 7874 0d0a 2020 2020  ce + ytext..    
-000057c0: 2020 2020 2020 2020 7861 6e63 686f 7220          xanchor 
-000057d0: 3d20 5b30 2c31 5d0d 0a20 2020 2020 2020  = [0,1]..       
-000057e0: 2020 2020 2079 616e 6368 6f72 203d 205b       yanchor = [
-000057f0: 302c 305d 0d0a 2020 2020 2020 2020 6966  0,0]..        if
-00005800: 2063 6c6f 7365 3262 6f74 746f 6d3a 0d0a   close2bottom:..
-00005810: 2020 2020 2020 2020 2020 2020 7974 6578              ytex
-00005820: 7420 3d20 7974 6578 7420 2b20 7370 6163  t = ytext + spac
-00005830: 650d 0a20 2020 2020 2020 2020 2020 2079  e..            y
-00005840: 616e 6368 6f72 203d 205b 312c 315d 0d0a  anchor = [1,1]..
-00005850: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00005860: 6c6f 7365 3272 6967 6874 3a0d 0a20 2020  lose2right:..   
-00005870: 2020 2020 2020 2020 2020 2020 2078 616e               xan
-00005880: 6368 6f72 203d 205b 312c 325d 0d0a 2020  chor = [1,2]..  
-00005890: 2020 2020 2020 7365 6c66 2e78 7465 7874        self.xtext
-000058a0: 2e73 6574 416e 6368 6f72 2878 616e 6368  .setAnchor(xanch
-000058b0: 6f72 290d 0a20 2020 2020 2020 2073 656c  or)..        sel
-000058c0: 662e 7974 6578 742e 7365 7441 6e63 686f  f.ytext.setAncho
-000058d0: 7228 7961 6e63 686f 7229 0d0a 2020 2020  r(yanchor)..    
-000058e0: 2020 2020 7365 6c66 2e78 7465 7874 2e73      self.xtext.s
-000058f0: 6574 5465 7874 2878 7465 7874 290d 0a20  etText(xtext).. 
-00005900: 2020 2020 2020 2073 656c 662e 7974 6578         self.ytex
-00005910: 742e 7365 7454 6578 7428 7974 6578 7429  t.setText(ytext)
-00005920: 0d0a 0d0a 2020 2020 6465 6620 7368 6f77  ....    def show
-00005930: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00005940: 2073 656c 662e 6178 2e61 6464 4974 656d   self.ax.addItem
-00005950: 2873 656c 662e 766c 696e 652c 2069 676e  (self.vline, ign
-00005960: 6f72 6542 6f75 6e64 733d 5472 7565 290d  oreBounds=True).
-00005970: 0a20 2020 2020 2020 2073 656c 662e 6178  .        self.ax
-00005980: 2e61 6464 4974 656d 2873 656c 662e 686c  .addItem(self.hl
-00005990: 696e 652c 2069 676e 6f72 6542 6f75 6e64  ine, ignoreBound
-000059a0: 733d 5472 7565 290d 0a20 2020 2020 2020  s=True)..       
-000059b0: 2073 656c 662e 6178 2e61 6464 4974 656d   self.ax.addItem
-000059c0: 2873 656c 662e 7874 6578 742c 2069 676e  (self.xtext, ign
-000059d0: 6f72 6542 6f75 6e64 733d 5472 7565 290d  oreBounds=True).
-000059e0: 0a20 2020 2020 2020 2073 656c 662e 6178  .        self.ax
-000059f0: 2e61 6464 4974 656d 2873 656c 662e 7974  .addItem(self.yt
-00005a00: 6578 742c 2069 676e 6f72 6542 6f75 6e64  ext, ignoreBound
-00005a10: 733d 5472 7565 290d 0a0d 0a20 2020 2064  s=True)....    d
-00005a20: 6566 2068 6964 6528 7365 6c66 293a 0d0a  ef hide(self):..
-00005a30: 2020 2020 2020 2020 7365 6c66 2e61 782e          self.ax.
-00005a40: 7265 6d6f 7665 4974 656d 2873 656c 662e  removeItem(self.
-00005a50: 7874 6578 7429 0d0a 2020 2020 2020 2020  xtext)..        
-00005a60: 7365 6c66 2e61 782e 7265 6d6f 7665 4974  self.ax.removeIt
-00005a70: 656d 2873 656c 662e 7974 6578 7429 0d0a  em(self.ytext)..
-00005a80: 2020 2020 2020 2020 7365 6c66 2e61 782e          self.ax.
-00005a90: 7265 6d6f 7665 4974 656d 2873 656c 662e  removeItem(self.
-00005aa0: 766c 696e 6529 0d0a 2020 2020 2020 2020  vline)..        
-00005ab0: 7365 6c66 2e61 782e 7265 6d6f 7665 4974  self.ax.removeIt
-00005ac0: 656d 2873 656c 662e 686c 696e 6529 0d0a  em(self.hline)..
-00005ad0: 0d0a 0d0a 0d0a 636c 6173 7320 4669 6e4c  ......class FinL
-00005ae0: 6567 656e 6449 7465 6d28 7067 2e4c 6567  egendItem(pg.Leg
-00005af0: 656e 6449 7465 6d29 3a0d 0a20 2020 2064  endItem):..    d
-00005b00: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00005b10: 2c20 626f 7264 6572 5f63 6f6c 6f72 2c20  , border_color, 
-00005b20: 6669 6c6c 5f63 6f6c 6f72 2c20 2a2a 6b77  fill_color, **kw
-00005b30: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00005b40: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00005b50: 282a 2a6b 7761 7267 7329 0d0a 2020 2020  (**kwargs)..    
-00005b60: 2020 2020 7365 6c66 2e6c 6179 6f75 742e      self.layout.
-00005b70: 7365 7456 6572 7469 6361 6c53 7061 6369  setVerticalSpaci
-00005b80: 6e67 2832 290d 0a20 2020 2020 2020 2073  ng(2)..        s
-00005b90: 656c 662e 6c61 796f 7574 2e73 6574 486f  elf.layout.setHo
-00005ba0: 7269 7a6f 6e74 616c 5370 6163 696e 6728  rizontalSpacing(
-00005bb0: 3230 290d 0a20 2020 2020 2020 2073 656c  20)..        sel
-00005bc0: 662e 6c61 796f 7574 2e73 6574 436f 6e74  f.layout.setCont
-00005bd0: 656e 7473 4d61 7267 696e 7328 322c 2032  entsMargins(2, 2
-00005be0: 2c20 3130 2c20 3229 0d0a 2020 2020 2020  , 10, 2)..      
-00005bf0: 2020 7365 6c66 2e62 6f72 6465 725f 636f    self.border_co
-00005c00: 6c6f 7220 3d20 626f 7264 6572 5f63 6f6c  lor = border_col
-00005c10: 6f72 0d0a 2020 2020 2020 2020 7365 6c66  or..        self
-00005c20: 2e66 696c 6c5f 636f 6c6f 7220 3d20 6669  .fill_color = fi
-00005c30: 6c6c 5f63 6f6c 6f72 0d0a 0d0a 2020 2020  ll_color....    
-00005c40: 6465 6620 7061 696e 7428 7365 6c66 2c20  def paint(self, 
-00005c50: 702c 202a 6172 6773 293a 0d0a 2020 2020  p, *args):..    
-00005c60: 2020 2020 702e 7365 7450 656e 2870 672e      p.setPen(pg.
-00005c70: 6d6b 5065 6e28 7365 6c66 2e62 6f72 6465  mkPen(self.borde
-00005c80: 725f 636f 6c6f 7229 290d 0a20 2020 2020  r_color))..     
-00005c90: 2020 2070 2e73 6574 4272 7573 6828 7067     p.setBrush(pg
-00005ca0: 2e6d 6b42 7275 7368 2873 656c 662e 6669  .mkBrush(self.fi
-00005cb0: 6c6c 5f63 6f6c 6f72 2929 0d0a 2020 2020  ll_color))..    
-00005cc0: 2020 2020 702e 6472 6177 5265 6374 2873      p.drawRect(s
-00005cd0: 656c 662e 626f 756e 6469 6e67 5265 6374  elf.boundingRect
-00005ce0: 2829 290d 0a0d 0a0d 0a0d 0a63 6c61 7373  ())........class
-00005cf0: 2046 696e 506f 6c79 4c69 6e65 2870 672e   FinPolyLine(pg.
-00005d00: 506f 6c79 4c69 6e65 524f 4929 3a0d 0a20  PolyLineROI):.. 
-00005d10: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00005d20: 7365 6c66 2c20 7662 2c20 2a61 7267 732c  self, vb, *args,
-00005d30: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00005d40: 2020 2020 2073 656c 662e 7662 203d 2076       self.vb = v
-00005d50: 6220 2320 696e 6974 2062 6566 6f72 6520  b # init before 
-00005d60: 7061 7265 6e74 2063 6f6e 7374 7275 6374  parent construct
-00005d70: 6f72 0d0a 2020 2020 2020 2020 7365 6c66  or..        self
-00005d80: 2e74 6578 7473 203d 205b 5d0d 0a20 2020  .texts = []..   
-00005d90: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00005da0: 6e69 745f 5f28 2a61 7267 732c 202a 2a6b  nit__(*args, **k
-00005db0: 7761 7267 7329 0d0a 0d0a 2020 2020 6465  wargs)....    de
-00005dc0: 6620 6164 6453 6567 6d65 6e74 2873 656c  f addSegment(sel
-00005dd0: 662c 2068 312c 2068 322c 2069 6e64 6578  f, h1, h2, index
-00005de0: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
-00005df0: 2073 7570 6572 2829 2e61 6464 5365 676d   super().addSegm
-00005e00: 656e 7428 6831 2c20 6832 2c20 696e 6465  ent(h1, h2, inde
-00005e10: 7829 0d0a 2020 2020 2020 2020 7465 7874  x)..        text
-00005e20: 203d 2070 672e 5465 7874 4974 656d 2863   = pg.TextItem(c
-00005e30: 6f6c 6f72 3d64 7261 775f 6c69 6e65 5f63  olor=draw_line_c
-00005e40: 6f6c 6f72 290d 0a20 2020 2020 2020 2074  olor)..        t
-00005e50: 6578 742e 7365 745a 5661 6c75 6528 3530  ext.setZValue(50
-00005e60: 290d 0a20 2020 2020 2020 2074 6578 742e  )..        text.
-00005e70: 7365 676d 656e 7420 3d20 7365 6c66 2e73  segment = self.s
-00005e80: 6567 6d65 6e74 735b 2d31 2069 6620 696e  egments[-1 if in
-00005e90: 6465 7820 6973 204e 6f6e 6520 656c 7365  dex is None else
-00005ea0: 2069 6e64 6578 5d0d 0a20 2020 2020 2020   index]..       
-00005eb0: 2069 6620 696e 6465 7820 6973 204e 6f6e   if index is Non
-00005ec0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00005ed0: 7365 6c66 2e74 6578 7473 2e61 7070 656e  self.texts.appen
-00005ee0: 6428 7465 7874 290d 0a20 2020 2020 2020  d(text)..       
-00005ef0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00005f00: 2020 2020 7365 6c66 2e74 6578 7473 2e69      self.texts.i
-00005f10: 6e73 6572 7428 696e 6465 782c 2074 6578  nsert(index, tex
-00005f20: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
-00005f30: 2e75 7064 6174 655f 7465 7874 2874 6578  .update_text(tex
-00005f40: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
-00005f50: 2e76 622e 6164 6449 7465 6d28 7465 7874  .vb.addItem(text
-00005f60: 2c20 6967 6e6f 7265 426f 756e 6473 3d54  , ignoreBounds=T
-00005f70: 7275 6529 0d0a 0d0a 2020 2020 6465 6620  rue)....    def 
-00005f80: 7265 6d6f 7665 5365 676d 656e 7428 7365  removeSegment(se
-00005f90: 6c66 2c20 7365 6729 3a0d 0a20 2020 2020  lf, seg):..     
-00005fa0: 2020 2073 7570 6572 2829 2e72 656d 6f76     super().remov
-00005fb0: 6553 6567 6d65 6e74 2873 6567 290d 0a20  eSegment(seg).. 
-00005fc0: 2020 2020 2020 2066 6f72 2074 6578 7420         for text 
-00005fd0: 696e 206c 6973 7428 7365 6c66 2e74 6578  in list(self.tex
-00005fe0: 7473 293a 0d0a 2020 2020 2020 2020 2020  ts):..          
-00005ff0: 2020 6966 2074 6578 742e 7365 676d 656e    if text.segmen
-00006000: 7420 3d3d 2073 6567 3a0d 0a20 2020 2020  t == seg:..     
-00006010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006020: 7662 2e72 656d 6f76 6549 7465 6d28 7465  vb.removeItem(te
-00006030: 7874 290d 0a20 2020 2020 2020 2020 2020  xt)..           
-00006040: 2020 2020 2073 656c 662e 7465 7874 732e       self.texts.
-00006050: 7265 6d6f 7665 2874 6578 7429 0d0a 0d0a  remove(text)....
-00006060: 2020 2020 6465 6620 7570 6461 7465 5f74      def update_t
-00006070: 6578 7428 7365 6c66 2c20 7465 7874 293a  ext(self, text):
-00006080: 0d0a 2020 2020 2020 2020 6830 203d 2074  ..        h0 = t
-00006090: 6578 742e 7365 676d 656e 742e 6861 6e64  ext.segment.hand
-000060a0: 6c65 735b 305d 5b27 6974 656d 275d 0d0a  les[0]['item']..
-000060b0: 2020 2020 2020 2020 6831 203d 2074 6578          h1 = tex
-000060c0: 742e 7365 676d 656e 742e 6861 6e64 6c65  t.segment.handle
-000060d0: 735b 315d 5b27 6974 656d 275d 0d0a 2020  s[1]['item']..  
-000060e0: 2020 2020 2020 6469 6666 203d 2068 312e        diff = h1.
-000060f0: 706f 7328 2920 2d20 6830 2e70 6f73 2829  pos() - h0.pos()
-00006100: 0d0a 2020 2020 2020 2020 6966 2064 6966  ..        if dif
-00006110: 662e 7928 2920 3c20 303a 0d0a 2020 2020  f.y() < 0:..    
-00006120: 2020 2020 2020 2020 7465 7874 2e73 6574          text.set
-00006130: 416e 6368 6f72 2828 302e 352c 3029 290d  Anchor((0.5,0)).
-00006140: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00006150: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00006160: 2e73 6574 416e 6368 6f72 2828 302e 352c  .setAnchor((0.5,
-00006170: 3129 290d 0a20 2020 2020 2020 2074 6578  1))..        tex
-00006180: 742e 7365 7450 6f73 2868 312e 706f 7328  t.setPos(h1.pos(
-00006190: 2929 0d0a 2020 2020 2020 2020 7465 7874  ))..        text
-000061a0: 2e73 6574 5465 7874 285f 6472 6177 5f6c  .setText(_draw_l
-000061b0: 696e 655f 7365 676d 656e 745f 7465 7874  ine_segment_text
-000061c0: 2873 656c 662c 2074 6578 742e 7365 676d  (self, text.segm
-000061d0: 656e 742c 2068 302e 706f 7328 292c 2068  ent, h0.pos(), h
-000061e0: 312e 706f 7328 2929 290d 0a0d 0a20 2020  1.pos()))....   
-000061f0: 2064 6566 2075 7064 6174 655f 7465 7874   def update_text
-00006200: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
-00006210: 2020 666f 7220 7465 7874 2069 6e20 7365    for text in se
-00006220: 6c66 2e74 6578 7473 3a0d 0a20 2020 2020  lf.texts:..     
-00006230: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-00006240: 7465 5f74 6578 7428 7465 7874 290d 0a0d  te_text(text)...
-00006250: 0a20 2020 2064 6566 206d 6f76 6550 6f69  .    def movePoi
-00006260: 6e74 2873 656c 662c 2068 616e 646c 652c  nt(self, handle,
-00006270: 2070 6f73 2c20 6d6f 6469 6669 6572 733d   pos, modifiers=
-00006280: 5174 436f 7265 2e51 742e 4b65 7962 6f61  QtCore.Qt.Keyboa
-00006290: 7264 4d6f 6469 6669 6572 2c20 6669 6e69  rdModifier, fini
-000062a0: 7368 3d54 7275 652c 2063 6f6f 7264 733d  sh=True, coords=
-000062b0: 2770 6172 656e 7427 293a 0d0a 2020 2020  'parent'):..    
-000062c0: 2020 2020 7375 7065 7228 292e 6d6f 7665      super().move
-000062d0: 506f 696e 7428 6861 6e64 6c65 2c20 706f  Point(handle, po
-000062e0: 732c 206d 6f64 6966 6965 7273 2c20 6669  s, modifiers, fi
-000062f0: 6e69 7368 2c20 636f 6f72 6473 290d 0a20  nish, coords).. 
-00006300: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-00006310: 7465 5f74 6578 7473 2829 0d0a 0d0a 2020  te_texts()....  
-00006320: 2020 6465 6620 7365 676d 656e 7443 6c69    def segmentCli
-00006330: 636b 6564 2873 656c 662c 2073 6567 6d65  cked(self, segme
-00006340: 6e74 2c20 6576 3d4e 6f6e 652c 2070 6f73  nt, ev=None, pos
-00006350: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
-00006360: 2070 6f73 203d 2073 6567 6d65 6e74 2e6d   pos = segment.m
-00006370: 6170 546f 5061 7265 6e74 2865 762e 706f  apToParent(ev.po
-00006380: 7328 2929 0d0a 2020 2020 2020 2020 706f  s())..        po
-00006390: 7320 3d20 5f63 6c61 6d70 5f70 6f69 6e74  s = _clamp_point
-000063a0: 2873 656c 662e 7662 2e70 6172 656e 7428  (self.vb.parent(
-000063b0: 292c 2070 6f73 290d 0a20 2020 2020 2020  ), pos)..       
-000063c0: 2073 7570 6572 2829 2e73 6567 6d65 6e74   super().segment
-000063d0: 436c 6963 6b65 6428 7365 676d 656e 742c  Clicked(segment,
-000063e0: 2070 6f73 3d70 6f73 290d 0a20 2020 2020   pos=pos)..     
-000063f0: 2020 2073 656c 662e 7570 6461 7465 5f74     self.update_t
-00006400: 6578 7473 2829 0d0a 0d0a 2020 2020 6465  exts()....    de
-00006410: 6620 6164 6448 616e 646c 6528 7365 6c66  f addHandle(self
-00006420: 2c20 696e 666f 2c20 696e 6465 783d 4e6f  , info, index=No
-00006430: 6e65 293a 0d0a 2020 2020 2020 2020 6861  ne):..        ha
-00006440: 6e64 6c65 203d 2073 7570 6572 2829 2e61  ndle = super().a
-00006450: 6464 4861 6e64 6c65 2869 6e66 6f2c 2069  ddHandle(info, i
-00006460: 6e64 6578 290d 0a20 2020 2020 2020 2068  ndex)..        h
-00006470: 616e 646c 652e 6d6f 7665 506f 696e 7420  andle.movePoint 
-00006480: 3d20 7061 7274 6961 6c28 5f72 6f69 6861  = partial(_roiha
-00006490: 6e64 6c65 5f6d 6f76 655f 736e 6170 2c20  ndle_move_snap, 
-000064a0: 7365 6c66 2e76 622c 2068 616e 646c 652e  self.vb, handle.
-000064b0: 6d6f 7665 506f 696e 7429 0d0a 2020 2020  movePoint)..    
-000064c0: 2020 2020 7265 7475 726e 2068 616e 646c      return handl
-000064d0: 650d 0a0d 0a0d 0a63 6c61 7373 2046 696e  e......class Fin
-000064e0: 4c69 6e65 2870 672e 4772 6170 6869 6373  Line(pg.Graphics
-000064f0: 4f62 6a65 6374 293a 0d0a 2020 2020 6465  Object):..    de
-00006500: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00006510: 2070 6f69 6e74 732c 2070 656e 293a 0d0a   points, pen):..
-00006520: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00006530: 5f5f 696e 6974 5f5f 2829 0d0a 2020 2020  __init__()..    
-00006540: 2020 2020 7365 6c66 2e70 6f69 6e74 7320      self.points 
-00006550: 3d20 706f 696e 7473 0d0a 2020 2020 2020  = points..      
-00006560: 2020 7365 6c66 2e70 656e 203d 2070 656e    self.pen = pen
-00006570: 0d0a 0d0a 2020 2020 6465 6620 7061 696e  ....    def pain
-00006580: 7428 7365 6c66 2c20 702c 202a 6172 6773  t(self, p, *args
-00006590: 293a 0d0a 2020 2020 2020 2020 702e 7365  ):..        p.se
-000065a0: 7450 656e 2873 656c 662e 7065 6e29 0d0a  tPen(self.pen)..
-000065b0: 2020 2020 2020 2020 702e 6472 6177 5061          p.drawPa
-000065c0: 7468 2873 656c 662e 7368 6170 6528 2929  th(self.shape())
-000065d0: 0d0a 0d0a 2020 2020 6465 6620 7368 6170  ....    def shap
-000065e0: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
-000065f0: 2020 7020 3d20 5174 4775 692e 5150 6169    p = QtGui.QPai
-00006600: 6e74 6572 5061 7468 2829 0d0a 2020 2020  nterPath()..    
-00006610: 2020 2020 702e 6d6f 7665 546f 282a 7365      p.moveTo(*se
-00006620: 6c66 2e70 6f69 6e74 735b 305d 290d 0a20  lf.points[0]).. 
-00006630: 2020 2020 2020 2070 2e6c 696e 6554 6f28         p.lineTo(
-00006640: 2a73 656c 662e 706f 696e 7473 5b31 5d29  *self.points[1])
-00006650: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00006660: 2070 0d0a 0d0a 2020 2020 6465 6620 626f   p....    def bo
-00006670: 756e 6469 6e67 5265 6374 2873 656c 6629  undingRect(self)
-00006680: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00006690: 6e20 7365 6c66 2e73 6861 7065 2829 2e62  n self.shape().b
-000066a0: 6f75 6e64 696e 6752 6563 7428 290d 0a0d  oundingRect()...
-000066b0: 0a0d 0a63 6c61 7373 2046 696e 456c 6c69  ...class FinElli
-000066c0: 7073 6528 7067 2e45 6c6c 6970 7365 524f  pse(pg.EllipseRO
-000066d0: 4929 3a0d 0a20 2020 2064 6566 2061 6464  I):..    def add
-000066e0: 526f 7461 7465 4861 6e64 6c65 2873 656c  RotateHandle(sel
-000066f0: 662c 202a 6172 6773 2c20 2a2a 6b77 6172  f, *args, **kwar
-00006700: 6773 293a 0d0a 2020 2020 2020 2020 7061  gs):..        pa
-00006710: 7373 0d0a 0d0a 0d0a 636c 6173 7320 4669  ss......class Fi
-00006720: 6e52 6563 7428 7067 2e52 6563 7452 4f49  nRect(pg.RectROI
-00006730: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-00006740: 6974 5f5f 2873 656c 662c 2061 782c 2062  it__(self, ax, b
-00006750: 7275 7368 2c20 2a61 7267 732c 202a 2a6b  rush, *args, **k
-00006760: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00006770: 2073 656c 662e 6178 203d 2061 780d 0a20   self.ax = ax.. 
-00006780: 2020 2020 2020 2073 656c 662e 6272 7573         self.brus
-00006790: 6820 3d20 6272 7573 680d 0a20 2020 2020  h = brush..     
-000067a0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-000067b0: 745f 5f28 2a61 7267 732c 202a 2a6b 7761  t__(*args, **kwa
-000067c0: 7267 7329 0d0a 0d0a 2020 2020 6465 6620  rgs)....    def 
-000067d0: 7061 696e 7428 7365 6c66 2c20 702c 202a  paint(self, p, *
-000067e0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-000067f0: 7220 3d20 5174 436f 7265 2e51 5265 6374  r = QtCore.QRect
-00006800: 4628 302c 2030 2c20 7365 6c66 2e73 7461  F(0, 0, self.sta
-00006810: 7465 5b27 7369 7a65 275d 5b30 5d2c 2073  te['size'][0], s
-00006820: 656c 662e 7374 6174 655b 2773 697a 6527  elf.state['size'
-00006830: 5d5b 315d 292e 6e6f 726d 616c 697a 6564  ][1]).normalized
-00006840: 2829 0d0a 2020 2020 2020 2020 702e 7365  ()..        p.se
-00006850: 7450 656e 2873 656c 662e 6375 7272 656e  tPen(self.curren
-00006860: 7450 656e 290d 0a20 2020 2020 2020 2070  tPen)..        p
-00006870: 2e73 6574 4272 7573 6828 7365 6c66 2e62  .setBrush(self.b
-00006880: 7275 7368 290d 0a20 2020 2020 2020 2070  rush)..        p
-00006890: 2e74 7261 6e73 6c61 7465 2872 2e6c 6566  .translate(r.lef
-000068a0: 7428 292c 2072 2e74 6f70 2829 290d 0a20  t(), r.top()).. 
-000068b0: 2020 2020 2020 2070 2e73 6361 6c65 2872         p.scale(r
-000068c0: 2e77 6964 7468 2829 2c20 722e 6865 6967  .width(), r.heig
-000068d0: 6874 2829 290d 0a20 2020 2020 2020 2070  ht())..        p
-000068e0: 2e64 7261 7752 6563 7428 302c 2030 2c20  .drawRect(0, 0, 
-000068f0: 312c 2031 290d 0a0d 0a20 2020 2064 6566  1, 1)....    def
-00006900: 2061 6464 5363 616c 6548 616e 646c 6528   addScaleHandle(
-00006910: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
-00006920: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00006930: 2069 6620 7365 6c66 2e72 6573 697a 6162   if self.resizab
-00006940: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
-00006950: 2073 7570 6572 2829 2e61 6464 5363 616c   super().addScal
-00006960: 6548 616e 646c 6528 2a61 7267 732c 202a  eHandle(*args, *
-00006970: 2a6b 7761 7267 7329 0d0a 0d0a 0d0a 636c  *kwargs)......cl
-00006980: 6173 7320 4669 6e56 6965 7742 6f78 2870  ass FinViewBox(p
-00006990: 672e 5669 6577 426f 7829 3a0d 0a20 2020  g.ViewBox):..   
-000069a0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-000069b0: 6c66 2c20 7769 6e2c 2069 6e69 745f 7374  lf, win, init_st
-000069c0: 6570 733d 3330 302c 2079 7363 616c 653d  eps=300, yscale=
-000069d0: 5953 6361 6c65 2827 6c69 6e65 6172 272c  YScale('linear',
-000069e0: 2031 292c 2076 5f7a 6f6f 6d5f 7363 616c   1), v_zoom_scal
-000069f0: 653d 312c 202a 6172 6773 2c20 2a2a 6b77  e=1, *args, **kw
-00006a00: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00006a10: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00006a20: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-00006a30: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006a40: 7769 6e20 3d20 7769 6e0d 0a20 2020 2020  win = win..     
-00006a50: 2020 2073 656c 662e 696e 6974 5f73 7465     self.init_ste
-00006a60: 7073 203d 2069 6e69 745f 7374 6570 730d  ps = init_steps.
-00006a70: 0a20 2020 2020 2020 2073 656c 662e 7973  .        self.ys
-00006a80: 6361 6c65 203d 2079 7363 616c 650d 0a20  cale = yscale.. 
-00006a90: 2020 2020 2020 2073 656c 662e 765f 7a6f         self.v_zo
-00006aa0: 6f6d 5f73 6361 6c65 203d 2076 5f7a 6f6f  om_scale = v_zoo
-00006ab0: 6d5f 7363 616c 650d 0a20 2020 2020 2020  m_scale..       
-00006ac0: 2073 656c 662e 6d61 7374 6572 5f76 6965   self.master_vie
-00006ad0: 7762 6f78 203d 204e 6f6e 650d 0a20 2020  wbox = None..   
-00006ae0: 2020 2020 2073 656c 662e 726f 6973 203d       self.rois =
-00006af0: 205b 5d0d 0a20 2020 2020 2020 2073 656c   []..        sel
-00006b00: 662e 7769 6e2e 5f69 734d 6f75 7365 4c65  f.win._isMouseLe
-00006b10: 6674 4472 6167 203d 2046 616c 7365 0d0a  ftDrag = False..
-00006b20: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00006b30: 6574 2829 0d0a 0d0a 2020 2020 6465 6620  et()....    def 
-00006b40: 7265 7365 7428 7365 6c66 293a 0d0a 2020  reset(self):..  
-00006b50: 2020 2020 2020 7365 6c66 2e76 5f7a 6f6f        self.v_zoo
-00006b60: 6d5f 6261 7365 6c69 6e65 203d 2030 2e35  m_baseline = 0.5
-00006b70: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
-00006b80: 5f61 7574 6f7a 6f6f 6d20 3d20 5472 7565  _autozoom = True
-00006b90: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-00006ba0: 6178 5f7a 6f6f 6d5f 706f 696e 7473 5f66  ax_zoom_points_f
-00006bb0: 203d 2031 0d0a 2020 2020 2020 2020 7365   = 1..        se
-00006bc0: 6c66 2e79 5f6d 6178 203d 2031 3030 300d  lf.y_max = 1000.
-00006bd0: 0a20 2020 2020 2020 2073 656c 662e 795f  .        self.y_
-00006be0: 6d69 6e20 3d20 300d 0a20 2020 2020 2020  min = 0..       
-00006bf0: 2073 656c 662e 795f 706f 7369 7469 7665   self.y_positive
-00006c00: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-00006c10: 2073 656c 662e 785f 696e 6465 7865 6420   self.x_indexed 
-00006c20: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
-00006c30: 7365 6c66 2e66 6f72 6365 5f72 616e 6765  self.force_range
-00006c40: 5f75 7064 6174 6520 3d20 300d 0a20 2020  _update = 0..   
-00006c50: 2020 2020 2077 6869 6c65 2073 656c 662e       while self.
-00006c60: 726f 6973 3a0d 0a20 2020 2020 2020 2020  rois:..         
-00006c70: 2020 2073 656c 662e 7265 6d6f 7665 5f6c     self.remove_l
-00006c80: 6173 745f 726f 6928 290d 0a20 2020 2020  ast_roi()..     
-00006c90: 2020 2073 656c 662e 6472 6177 5f6c 696e     self.draw_lin
-00006ca0: 6520 3d20 4e6f 6e65 0d0a 2020 2020 2020  e = None..      
-00006cb0: 2020 7365 6c66 2e64 7261 7769 6e67 203d    self.drawing =
-00006cc0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00006cd0: 7365 6c66 2e73 7461 6e64 616c 6f6e 6573  self.standalones
-00006ce0: 203d 2073 6574 2829 0d0a 2020 2020 2020   = set()..      
-00006cf0: 2020 7365 6c66 2e75 7064 6174 696e 675f    self.updating_
-00006d00: 6c69 6e6b 6564 203d 2046 616c 7365 0d0a  linked = False..
-00006d10: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00006d20: 5f64 6174 6173 7263 284e 6f6e 6529 0d0a  _datasrc(None)..
-00006d30: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00006d40: 4d6f 7573 6545 6e61 626c 6564 2878 3d54  MouseEnabled(x=T
-00006d50: 7275 652c 2079 3d46 616c 7365 290d 0a20  rue, y=False).. 
-00006d60: 2020 2020 2020 2073 656c 662e 7365 7452         self.setR
-00006d70: 616e 6765 2851 7443 6f72 652e 5152 6563  ange(QtCore.QRec
-00006d80: 7446 2870 672e 506f 696e 7428 302c 2030  tF(pg.Point(0, 0
-00006d90: 292c 2070 672e 506f 696e 7428 312c 2031  ), pg.Point(1, 1
-00006da0: 2929 290d 0a0d 0a20 2020 2064 6566 2073  )))....    def s
-00006db0: 6574 5f64 6174 6173 7263 2873 656c 662c  et_datasrc(self,
-00006dc0: 2064 6174 6173 7263 293a 0d0a 2020 2020   datasrc):..    
-00006dd0: 2020 2020 7365 6c66 2e64 6174 6173 7263      self.datasrc
-00006de0: 203d 2064 6174 6173 7263 0d0a 2020 2020   = datasrc..    
-00006df0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00006e00: 6461 7461 7372 633a 0d0a 2020 2020 2020  datasrc:..      
-00006e10: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00006e20: 2020 2020 2020 6461 7461 7372 632e 7570        datasrc.up
-00006e30: 6461 7465 5f69 6e69 745f 7828 7365 6c66  date_init_x(self
-00006e40: 2e69 6e69 745f 7374 6570 7329 0d0a 0d0a  .init_steps)....
-00006e50: 2020 2020 6465 6620 7072 655f 7072 6f63      def pre_proc
-00006e60: 6573 735f 6461 7461 2873 656c 6629 3a0d  ess_data(self):.
-00006e70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00006e80: 2e64 6174 6173 7263 2061 6e64 2073 656c  .datasrc and sel
-00006e90: 662e 6461 7461 7372 632e 7363 616c 655f  f.datasrc.scale_
-00006ea0: 636f 6c73 3a0d 0a20 2020 2020 2020 2020  cols:..         
-00006eb0: 2020 2064 6620 3d20 7365 6c66 2e64 6174     df = self.dat
-00006ec0: 6173 7263 2e64 662e 696c 6f63 5b3a 2c20  asrc.df.iloc[:, 
-00006ed0: 7365 6c66 2e64 6174 6173 7263 2e73 6361  self.datasrc.sca
-00006ee0: 6c65 5f63 6f6c 735d 0d0a 2020 2020 2020  le_cols]..      
-00006ef0: 2020 2020 2020 7365 6c66 2e79 5f6d 6178        self.y_max
-00006f00: 203d 2064 662e 6d61 7828 292e 6d61 7828   = df.max().max(
-00006f10: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00006f20: 656c 662e 795f 6d69 6e20 3d20 6466 2e6d  elf.y_min = df.m
-00006f30: 696e 2829 2e6d 696e 2829 0d0a 2020 2020  in().min()..    
-00006f40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00006f50: 795f 6d69 6e20 3c3d 2030 3a0d 0a20 2020  y_min <= 0:..   
-00006f60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006f70: 662e 795f 706f 7369 7469 7665 203d 2046  f.y_positive = F
-00006f80: 616c 7365 0d0a 0d0a 2020 2020 4070 726f  alse....    @pro
-00006f90: 7065 7274 790d 0a20 2020 2064 6566 2064  perty..    def d
-00006fa0: 6174 6173 7263 5f6f 725f 7374 616e 6461  atasrc_or_standa
-00006fb0: 6c6f 6e65 2873 656c 6629 3a0d 0a20 2020  lone(self):..   
-00006fc0: 2020 2020 2064 7320 3d20 7365 6c66 2e64       ds = self.d
-00006fd0: 6174 6173 7263 0d0a 2020 2020 2020 2020  atasrc..        
-00006fe0: 6966 206e 6f74 2064 7320 616e 6420 7365  if not ds and se
-00006ff0: 6c66 2e73 7461 6e64 616c 6f6e 6573 3a0d  lf.standalones:.
-00007000: 0a20 2020 2020 2020 2020 2020 2064 7320  .            ds 
-00007010: 3d20 6e65 7874 2869 7465 7228 7365 6c66  = next(iter(self
-00007020: 2e73 7461 6e64 616c 6f6e 6573 2929 0d0a  .standalones))..
-00007030: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00007040: 730d 0a0d 0a20 2020 2064 6566 2077 6865  s....    def whe
-00007050: 656c 4576 656e 7428 7365 6c66 2c20 6576  elEvent(self, ev
-00007060: 2c20 6178 6973 3d4e 6f6e 6529 3a0d 0a20  , axis=None):.. 
-00007070: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00007080: 6173 7465 725f 7669 6577 626f 783a 0d0a  aster_viewbox:..
-00007090: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000070a0: 726e 2073 656c 662e 6d61 7374 6572 5f76  rn self.master_v
-000070b0: 6965 7762 6f78 2e77 6865 656c 4576 656e  iewbox.wheelEven
-000070c0: 7428 6576 2c20 6178 6973 3d61 7869 7329  t(ev, axis=axis)
-000070d0: 0d0a 2020 2020 2020 2020 6966 2065 762e  ..        if ev.
-000070e0: 6d6f 6469 6669 6572 7328 2920 3d3d 2051  modifiers() == Q
-000070f0: 7443 6f72 652e 5174 2e4b 6579 626f 6172  tCore.Qt.Keyboar
-00007100: 644d 6f64 6966 6965 722e 436f 6e74 726f  dModifier.Contro
-00007110: 6c4d 6f64 6966 6965 723a 0d0a 2020 2020  lModifier:..    
-00007120: 2020 2020 2020 2020 7363 616c 655f 6661          scale_fa
-00007130: 6374 203d 2031 0d0a 2020 2020 2020 2020  ct = 1..        
-00007140: 2020 2020 7365 6c66 2e76 5f7a 6f6f 6d5f      self.v_zoom_
-00007150: 7363 616c 6520 2f3d 2031 2e30 3220 2a2a  scale /= 1.02 **
-00007160: 2028 6576 2e64 656c 7461 2829 202a 2073   (ev.delta() * s
-00007170: 656c 662e 7374 6174 655b 2777 6865 656c  elf.state['wheel
-00007180: 5363 616c 6546 6163 746f 7227 5d29 0d0a  ScaleFactor'])..
-00007190: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000071a0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-000071b0: 5f66 6163 7420 3d20 312e 3032 202a 2a20  _fact = 1.02 ** 
-000071c0: 2865 762e 6465 6c74 6128 2920 2a20 7365  (ev.delta() * se
-000071d0: 6c66 2e73 7461 7465 5b27 7768 6565 6c53  lf.state['wheelS
-000071e0: 6361 6c65 4661 6374 6f72 275d 290d 0a20  caleFactor']).. 
-000071f0: 2020 2020 2020 2076 7220 3d20 7365 6c66         vr = self
-00007200: 2e74 6172 6765 7452 6563 7428 290d 0a20  .targetRect().. 
-00007210: 2020 2020 2020 2063 656e 7465 7220 3d20         center = 
-00007220: 7365 6c66 2e6d 6170 546f 5669 6577 2865  self.mapToView(e
-00007230: 762e 7363 656e 6550 6f73 2829 290d 0a20  v.scenePos()).. 
-00007240: 2020 2020 2020 2070 6374 5f78 203d 2028         pct_x = (
-00007250: 6365 6e74 6572 2e78 2829 2d76 722e 6c65  center.x()-vr.le
-00007260: 6674 2829 2920 2f20 7672 2e77 6964 7468  ft()) / vr.width
-00007270: 2829 0d0a 2020 2020 2020 2020 6966 2070  ()..        if p
-00007280: 6374 5f78 203c 2030 2e30 353a 2023 207a  ct_x < 0.05: # z
-00007290: 6f6f 6d20 746f 2066 6172 206c 6566 7420  oom to far left 
-000072a0: 3d3e 2061 6c6c 2074 6865 2077 6179 206c  => all the way l
-000072b0: 6566 740d 0a20 2020 2020 2020 2020 2020  eft..           
-000072c0: 2063 656e 7465 7220 3d20 7067 2e50 6f69   center = pg.Poi
-000072d0: 6e74 2876 722e 6c65 6674 2829 2c20 6365  nt(vr.left(), ce
-000072e0: 6e74 6572 2e79 2829 290d 0a20 2020 2020  nter.y())..     
-000072f0: 2020 2065 6c69 6620 7063 745f 7820 3e20     elif pct_x > 
-00007300: 302e 3935 3a20 2320 7a6f 6f6d 2074 6f20  0.95: # zoom to 
-00007310: 6661 7220 7269 6768 7420 3d3e 2061 6c6c  far right => all
-00007320: 2074 6865 2077 6179 2072 6967 6874 0d0a   the way right..
-00007330: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
-00007340: 6572 203d 2070 672e 506f 696e 7428 7672  er = pg.Point(vr
-00007350: 2e72 6967 6874 2829 2c20 6365 6e74 6572  .right(), center
-00007360: 2e79 2829 290d 0a20 2020 2020 2020 2073  .y())..        s
-00007370: 656c 662e 7a6f 6f6d 5f72 6563 7428 7672  elf.zoom_rect(vr
-00007380: 2c20 7363 616c 655f 6661 6374 2c20 6365  , scale_fact, ce
-00007390: 6e74 6572 290d 0a20 2020 2020 2020 2023  nter)..        #
-000073a0: 2075 7064 6174 6520 6372 6f73 7368 6169   update crosshai
-000073b0: 720d 0a20 2020 2020 2020 205f 6d6f 7573  r..        _mous
-000073c0: 655f 6d6f 7665 6428 7365 6c66 2e77 696e  e_moved(self.win
-000073d0: 2c20 4e6f 6e65 290d 0a20 2020 2020 2020  , None)..       
-000073e0: 2065 762e 6163 6365 7074 2829 0d0a 0d0a   ev.accept()....
-000073f0: 2020 2020 6465 6620 6d6f 7573 6544 7261      def mouseDra
-00007400: 6745 7665 6e74 2873 656c 662c 2065 762c  gEvent(self, ev,
-00007410: 2061 7869 733d 4e6f 6e65 293a 0d0a 2020   axis=None):..  
-00007420: 2020 2020 2020 6178 6973 203d 2030 2023        axis = 0 #
-00007430: 2064 6f6e 2774 2063 6f6e 7374 7261 696e   don't constrain
-00007440: 2064 7261 6720 6469 7265 6374 696f 6e0d   drag direction.
-00007450: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007460: 2e6d 6173 7465 725f 7669 6577 626f 783a  .master_viewbox:
-00007470: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00007480: 7475 726e 2073 656c 662e 6d61 7374 6572  turn self.master
-00007490: 5f76 6965 7762 6f78 2e6d 6f75 7365 4472  _viewbox.mouseDr
-000074a0: 6167 4576 656e 7428 6576 2c20 6178 6973  agEvent(ev, axis
-000074b0: 3d61 7869 7329 0d0a 2020 2020 2020 2020  =axis)..        
-000074c0: 6966 206e 6f74 2073 656c 662e 6461 7461  if not self.data
-000074d0: 7372 633a 0d0a 2020 2020 2020 2020 2020  src:..          
-000074e0: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
-000074f0: 2020 6966 2065 762e 6275 7474 6f6e 2829    if ev.button()
-00007500: 203d 3d20 5174 436f 7265 2e51 742e 4d6f   == QtCore.Qt.Mo
-00007510: 7573 6542 7574 746f 6e2e 4c65 6674 4275  useButton.LeftBu
-00007520: 7474 6f6e 3a0d 0a20 2020 2020 2020 2020  tton:..         
-00007530: 2020 2073 656c 662e 6d6f 7573 654c 6566     self.mouseLef
-00007540: 7444 7261 6728 6576 2c20 6178 6973 290d  tDrag(ev, axis).
-00007550: 0a20 2020 2020 2020 2065 6c69 6620 6576  .        elif ev
-00007560: 2e62 7574 746f 6e28 2920 3d3d 2051 7443  .button() == QtC
-00007570: 6f72 652e 5174 2e4d 6f75 7365 4275 7474  ore.Qt.MouseButt
-00007580: 6f6e 2e4d 6964 646c 6542 7574 746f 6e3a  on.MiddleButton:
-00007590: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000075a0: 6c66 2e6d 6f75 7365 4d69 6464 6c65 4472  lf.mouseMiddleDr
-000075b0: 6167 2865 762c 2061 7869 7329 0d0a 2020  ag(ev, axis)..  
-000075c0: 2020 2020 2020 656c 6966 2065 762e 6275        elif ev.bu
-000075d0: 7474 6f6e 2829 203d 3d20 5174 436f 7265  tton() == QtCore
-000075e0: 2e51 742e 4d6f 7573 6542 7574 746f 6e2e  .Qt.MouseButton.
-000075f0: 5269 6768 7442 7574 746f 6e3a 0d0a 2020  RightButton:..  
-00007600: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00007610: 6f75 7365 5269 6768 7444 7261 6728 6576  ouseRightDrag(ev
-00007620: 2c20 6178 6973 290d 0a20 2020 2020 2020  , axis)..       
-00007630: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00007640: 2020 2020 7375 7065 7228 292e 6d6f 7573      super().mous
-00007650: 6544 7261 6745 7665 6e74 2865 762c 2061  eDragEvent(ev, a
-00007660: 7869 7329 0d0a 0d0a 2020 2020 6465 6620  xis)....    def 
-00007670: 6d6f 7573 654c 6566 7444 7261 6728 7365  mouseLeftDrag(se
-00007680: 6c66 2c20 6576 2c20 6178 6973 293a 0d0a  lf, ev, axis):..
-00007690: 2020 2020 2020 2020 2727 2743 7472 6c2b          '''Ctrl+
-000076a0: 4c42 7574 746f 6e20 6472 6177 206c 696e  LButton draw lin
-000076b0: 6573 2e27 2727 0d0a 2020 2020 2020 2020  es.'''..        
-000076c0: 6966 2065 762e 6d6f 6469 6669 6572 7328  if ev.modifiers(
-000076d0: 2920 213d 2051 7443 6f72 652e 5174 2e4b  ) != QtCore.Qt.K
-000076e0: 6579 626f 6172 644d 6f64 6966 6965 722e  eyboardModifier.
-000076f0: 436f 6e74 726f 6c4d 6f64 6966 6965 723a  ControlModifier:
-00007700: 0d0a 2020 2020 2020 2020 2020 2020 7375  ..            su
-00007710: 7065 7228 292e 6d6f 7573 6544 7261 6745  per().mouseDragE
-00007720: 7665 6e74 2865 762c 2061 7869 7329 0d0a  vent(ev, axis)..
-00007730: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-00007740: 762e 6973 4669 6e69 7368 2829 3a0d 0a20  v.isFinish():.. 
-00007750: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007760: 656c 662e 7769 6e2e 5f69 734d 6f75 7365  elf.win._isMouse
-00007770: 4c65 6674 4472 6167 203d 2046 616c 7365  LeftDrag = False
-00007780: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00007790: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000077a0: 2020 2020 2073 656c 662e 7769 6e2e 5f69       self.win._i
-000077b0: 734d 6f75 7365 4c65 6674 4472 6167 203d  sMouseLeftDrag =
-000077c0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-000077d0: 2020 2069 6620 6576 2e69 7346 696e 6973     if ev.isFinis
-000077e0: 6828 2920 6f72 2073 656c 662e 6472 6177  h() or self.draw
-000077f0: 696e 673a 0d0a 2020 2020 2020 2020 2020  ing:..          
-00007800: 2020 2020 2020 7365 6c66 2e72 6566 7265        self.refre
-00007810: 7368 5f61 6c6c 5f79 5f7a 6f6f 6d28 290d  sh_all_y_zoom().
-00007820: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007830: 6e6f 7420 7365 6c66 2e64 7261 7769 6e67  not self.drawing
-00007840: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00007850: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-00007860: 2020 2069 6620 7365 6c66 2e64 7261 775f     if self.draw_
-00007870: 6c69 6e65 2061 6e64 206e 6f74 2073 656c  line and not sel
-00007880: 662e 6472 6177 696e 673a 0d0a 2020 2020  f.drawing:..    
-00007890: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-000078a0: 5f64 7261 775f 6c69 6e65 5f63 6f6c 6f72  _draw_line_color
-000078b0: 2864 7261 775f 646f 6e65 5f63 6f6c 6f72  (draw_done_color
-000078c0: 290d 0a20 2020 2020 2020 2070 3120 3d20  )..        p1 = 
-000078d0: 7365 6c66 2e6d 6170 546f 5669 6577 2865  self.mapToView(e
-000078e0: 762e 706f 7328 2929 0d0a 2020 2020 2020  v.pos())..      
-000078f0: 2020 7031 203d 205f 636c 616d 705f 706f    p1 = _clamp_po
-00007900: 696e 7428 7365 6c66 2e70 6172 656e 7428  int(self.parent(
-00007910: 292c 2070 3129 0d0a 2020 2020 2020 2020  ), p1)..        
-00007920: 6966 206e 6f74 2073 656c 662e 6472 6177  if not self.draw
-00007930: 696e 673a 0d0a 2020 2020 2020 2020 2020  ing:..          
-00007940: 2020 2320 6164 6420 6e65 7720 6c69 6e65    # add new line
-00007950: 0d0a 2020 2020 2020 2020 2020 2020 7030  ..            p0
-00007960: 203d 2073 656c 662e 6d61 7054 6f56 6965   = self.mapToVie
-00007970: 7728 6576 2e6c 6173 7450 6f73 2829 290d  w(ev.lastPos()).
-00007980: 0a20 2020 2020 2020 2020 2020 2070 3020  .            p0 
-00007990: 3d20 5f63 6c61 6d70 5f70 6f69 6e74 2873  = _clamp_point(s
-000079a0: 656c 662e 7061 7265 6e74 2829 2c20 7030  elf.parent(), p0
-000079b0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-000079c0: 656c 662e 6472 6177 5f6c 696e 6520 3d20  elf.draw_line = 
-000079d0: 4669 6e50 6f6c 794c 696e 6528 7365 6c66  FinPolyLine(self
-000079e0: 2c20 5b70 302c 2070 315d 2c20 636c 6f73  , [p0, p1], clos
-000079f0: 6564 3d46 616c 7365 2c20 7065 6e3d 7067  ed=False, pen=pg
-00007a00: 2e6d 6b50 656e 2864 7261 775f 6c69 6e65  .mkPen(draw_line
-00007a10: 5f63 6f6c 6f72 292c 206d 6f76 6162 6c65  _color), movable
-00007a20: 3d46 616c 7365 290d 0a20 2020 2020 2020  =False)..       
-00007a30: 2020 2020 2073 656c 662e 6472 6177 5f6c       self.draw_l
-00007a40: 696e 652e 7365 745a 5661 6c75 6528 3430  ine.setZValue(40
-00007a50: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00007a60: 656c 662e 726f 6973 2e61 7070 656e 6428  elf.rois.append(
-00007a70: 7365 6c66 2e64 7261 775f 6c69 6e65 290d  self.draw_line).
-00007a80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007a90: 662e 6164 6449 7465 6d28 7365 6c66 2e64  f.addItem(self.d
-00007aa0: 7261 775f 6c69 6e65 290d 0a20 2020 2020  raw_line)..     
-00007ab0: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
-00007ac0: 696e 6720 3d20 5472 7565 0d0a 2020 2020  ing = True..    
-00007ad0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00007ae0: 2020 2020 2020 2023 2064 7261 7720 706c         # draw pl
-00007af0: 6163 6564 2070 6f69 6e74 2061 7420 656e  aced point at en
-00007b00: 6420 6f66 2070 6f6c 792d 6c69 6e65 0d0a  d of poly-line..
-00007b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007b20: 2e64 7261 775f 6c69 6e65 2e6d 6f76 6550  .draw_line.moveP
-00007b30: 6f69 6e74 282d 312c 2070 3129 0d0a 2020  oint(-1, p1)..  
-00007b40: 2020 2020 2020 6966 2065 762e 6973 4669        if ev.isFi
-00007b50: 6e69 7368 2829 3a0d 0a20 2020 2020 2020  nish():..       
-00007b60: 2020 2020 2073 656c 662e 6472 6177 696e       self.drawin
-00007b70: 6720 3d20 4661 6c73 650d 0a20 2020 2020  g = False..     
-00007b80: 2020 2065 762e 6163 6365 7074 2829 0d0a     ev.accept()..
-00007b90: 0d0a 2020 2020 6465 6620 6d6f 7573 654d  ..    def mouseM
-00007ba0: 6964 646c 6544 7261 6728 7365 6c66 2c20  iddleDrag(self, 
-00007bb0: 6576 2c20 6178 6973 293a 0d0a 2020 2020  ev, axis):..    
-00007bc0: 2020 2020 2727 2743 7472 6c2b 4d42 7574      '''Ctrl+MBut
-00007bd0: 746f 6e20 6472 6177 2065 6c6c 6970 7365  ton draw ellipse
-00007be0: 732e 2727 270d 0a20 2020 2020 2020 2069  s.'''..        i
-00007bf0: 6620 6576 2e6d 6f64 6966 6965 7273 2829  f ev.modifiers()
-00007c00: 2021 3d20 5174 436f 7265 2e51 742e 4b65   != QtCore.Qt.Ke
-00007c10: 7962 6f61 7264 4d6f 6469 6669 6572 2e43  yboardModifier.C
-00007c20: 6f6e 7472 6f6c 4d6f 6469 6669 6572 3a0d  ontrolModifier:.
-00007c30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00007c40: 7572 6e20 7375 7065 7228 292e 6d6f 7573  urn super().mous
-00007c50: 6544 7261 6745 7665 6e74 2865 762c 2061  eDragEvent(ev, a
-00007c60: 7869 7329 0d0a 2020 2020 2020 2020 7031  xis)..        p1
-00007c70: 203d 2073 656c 662e 6d61 7054 6f56 6965   = self.mapToVie
-00007c80: 7728 6576 2e70 6f73 2829 290d 0a20 2020  w(ev.pos())..   
-00007c90: 2020 2020 2070 3120 3d20 5f63 6c61 6d70       p1 = _clamp
-00007ca0: 5f70 6f69 6e74 2873 656c 662e 7061 7265  _point(self.pare
-00007cb0: 6e74 2829 2c20 7031 290d 0a20 2020 2020  nt(), p1)..     
-00007cc0: 2020 2064 6566 206e 6f6e 7a65 726f 7369     def nonzerosi
-00007cd0: 7a65 2861 2c20 6229 3a0d 0a20 2020 2020  ze(a, b):..     
-00007ce0: 2020 2020 2020 2063 203d 2062 2d61 0d0a         c = b-a..
-00007cf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00007d00: 726e 2070 672e 506f 696e 7428 6162 7328  rn pg.Point(abs(
-00007d10: 632e 7828 2929 206f 7220 312c 2061 6273  c.x()) or 1, abs
-00007d20: 2863 2e79 2829 2920 6f72 2031 652d 3329  (c.y()) or 1e-3)
-00007d30: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00007d40: 2073 656c 662e 6472 6177 696e 673a 0d0a   self.drawing:..
-00007d50: 2020 2020 2020 2020 2020 2020 2320 6164              # ad
-00007d60: 6420 6e65 7720 656c 6c69 7073 650d 0a20  d new ellipse.. 
-00007d70: 2020 2020 2020 2020 2020 2070 3020 3d20             p0 = 
-00007d80: 7365 6c66 2e6d 6170 546f 5669 6577 2865  self.mapToView(e
-00007d90: 762e 6c61 7374 506f 7328 2929 0d0a 2020  v.lastPos())..  
-00007da0: 2020 2020 2020 2020 2020 7030 203d 205f            p0 = _
-00007db0: 636c 616d 705f 706f 696e 7428 7365 6c66  clamp_point(self
-00007dc0: 2e70 6172 656e 7428 292c 2070 3029 0d0a  .parent(), p0)..
-00007dd0: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
-00007de0: 6e6f 6e7a 6572 6f73 697a 6528 7030 2c20  nonzerosize(p0, 
-00007df0: 7031 290d 0a20 2020 2020 2020 2020 2020  p1)..           
-00007e00: 2070 3020 3d20 5174 436f 7265 2e51 506f   p0 = QtCore.QPo
-00007e10: 696e 7446 2870 302e 7828 292d 732e 7828  intF(p0.x()-s.x(
-00007e20: 292f 322c 2070 302e 7928 292d 732e 7928  )/2, p0.y()-s.y(
-00007e30: 292f 3229 0d0a 2020 2020 2020 2020 2020  )/2)..          
-00007e40: 2020 7365 6c66 2e64 7261 775f 656c 6c69    self.draw_elli
-00007e50: 7073 6520 3d20 4669 6e45 6c6c 6970 7365  pse = FinEllipse
-00007e60: 2870 302c 2073 2c20 7065 6e3d 7067 2e6d  (p0, s, pen=pg.m
-00007e70: 6b50 656e 2864 7261 775f 6c69 6e65 5f63  kPen(draw_line_c
-00007e80: 6f6c 6f72 292c 206d 6f76 6162 6c65 3d54  olor), movable=T
-00007e90: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
-00007ea0: 2020 7365 6c66 2e64 7261 775f 656c 6c69    self.draw_elli
-00007eb0: 7073 652e 7365 745a 5661 6c75 6528 3830  pse.setZValue(80
-00007ec0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00007ed0: 656c 662e 726f 6973 2e61 7070 656e 6428  elf.rois.append(
-00007ee0: 7365 6c66 2e64 7261 775f 656c 6c69 7073  self.draw_ellips
-00007ef0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00007f00: 7365 6c66 2e61 6464 4974 656d 2873 656c  self.addItem(sel
-00007f10: 662e 6472 6177 5f65 6c6c 6970 7365 290d  f.draw_ellipse).
-00007f20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007f30: 662e 6472 6177 696e 6720 3d20 5472 7565  f.drawing = True
-00007f40: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00007f50: 0a20 2020 2020 2020 2020 2020 2063 203d  .            c =
-00007f60: 2073 656c 662e 6472 6177 5f65 6c6c 6970   self.draw_ellip
-00007f70: 7365 2e70 6f73 2829 202b 2073 656c 662e  se.pos() + self.
-00007f80: 6472 6177 5f65 6c6c 6970 7365 2e73 697a  draw_ellipse.siz
-00007f90: 6528 292a 302e 350d 0a20 2020 2020 2020  e()*0.5..       
-00007fa0: 2020 2020 2073 203d 206e 6f6e 7a65 726f       s = nonzero
-00007fb0: 7369 7a65 2863 2c20 7031 290d 0a20 2020  size(c, p1)..   
-00007fc0: 2020 2020 2020 2020 2073 656c 662e 6472           self.dr
-00007fd0: 6177 5f65 6c6c 6970 7365 2e73 6574 5369  aw_ellipse.setSi
-00007fe0: 7a65 2873 2a32 2c20 7570 6461 7465 3d46  ze(s*2, update=F
-00007ff0: 616c 7365 290d 0a20 2020 2020 2020 2020  alse)..         
-00008000: 2020 2073 656c 662e 6472 6177 5f65 6c6c     self.draw_ell
-00008010: 6970 7365 2e73 6574 506f 7328 632d 7329  ipse.setPos(c-s)
-00008020: 0d0a 2020 2020 2020 2020 6966 2065 762e  ..        if ev.
-00008030: 6973 4669 6e69 7368 2829 3a0d 0a20 2020  isFinish():..   
-00008040: 2020 2020 2020 2020 2073 656c 662e 6472           self.dr
-00008050: 6177 696e 6720 3d20 4661 6c73 650d 0a20  awing = False.. 
-00008060: 2020 2020 2020 2065 762e 6163 6365 7074         ev.accept
-00008070: 2829 0d0a 0d0a 2020 2020 6465 6620 6d6f  ()....    def mo
-00008080: 7573 6552 6967 6874 4472 6167 2873 656c  useRightDrag(sel
-00008090: 662c 2065 762c 2061 7869 7329 3a0d 0a20  f, ev, axis):.. 
-000080a0: 2020 2020 2020 2027 2727 5242 7574 746f         '''RButto
-000080b0: 6e20 6973 2062 6f78 207a 6f6f 6d2e 2041  n is box zoom. A
-000080c0: 7420 6c65 6173 7420 666f 7220 6e6f 772e  t least for now.
-000080d0: 2727 270d 0a20 2020 2020 2020 2065 762e  '''..        ev.
-000080e0: 6163 6365 7074 2829 0d0a 2020 2020 2020  accept()..      
-000080f0: 2020 6966 206e 6f74 2065 762e 6973 4669    if not ev.isFi
-00008100: 6e69 7368 2829 3a0d 0a20 2020 2020 2020  nish():..       
-00008110: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
-00008120: 5363 616c 6542 6f78 2865 762e 6275 7474  ScaleBox(ev.butt
-00008130: 6f6e 446f 776e 506f 7328 292c 2065 762e  onDownPos(), ev.
-00008140: 706f 7328 2929 0d0a 2020 2020 2020 2020  pos())..        
-00008150: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00008160: 2020 2073 656c 662e 7262 5363 616c 6542     self.rbScaleB
-00008170: 6f78 2e68 6964 6528 290d 0a20 2020 2020  ox.hide()..     
-00008180: 2020 2020 2020 2061 7820 3d20 5174 436f         ax = QtCo
-00008190: 7265 2e51 5265 6374 4628 7067 2e50 6f69  re.QRectF(pg.Poi
-000081a0: 6e74 2865 762e 6275 7474 6f6e 446f 776e  nt(ev.buttonDown
-000081b0: 506f 7328 6576 2e62 7574 746f 6e28 2929  Pos(ev.button())
-000081c0: 292c 2070 672e 506f 696e 7428 6576 2e70  ), pg.Point(ev.p
-000081d0: 6f73 2829 2929 0d0a 2020 2020 2020 2020  os()))..        
-000081e0: 2020 2020 6178 203d 2073 656c 662e 6368      ax = self.ch
-000081f0: 696c 6447 726f 7570 2e6d 6170 5265 6374  ildGroup.mapRect
-00008200: 4672 6f6d 5061 7265 6e74 2861 7829 0d0a  FromParent(ax)..
-00008210: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00008220: 782e 7769 6474 6828 2920 3c20 323a 2023  x.width() < 2: #
-00008230: 207a 6f6f 6d69 6e67 2074 6869 7320 6e61   zooming this na
-00008240: 7272 6f77 2069 7320 7072 6f62 6162 6c79  rrow is probably
-00008250: 2061 206d 6973 7461 6b65 0d0a 2020 2020   a mistake..    
-00008260: 2020 2020 2020 2020 2020 2020 6178 2e61              ax.a
-00008270: 646a 7573 7428 2d31 2c20 302c 202b 312c  djust(-1, 0, +1,
-00008280: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
-00008290: 2073 656c 662e 7368 6f77 4178 5265 6374   self.showAxRect
-000082a0: 2861 7829 0d0a 2020 2020 2020 2020 2020  (ax)..          
-000082b0: 2020 7365 6c66 2e61 7848 6973 746f 7279    self.axHistory
-000082c0: 506f 696e 7465 7220 2b3d 2031 0d0a 2020  Pointer += 1..  
-000082d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000082e0: 7848 6973 746f 7279 203d 2073 656c 662e  xHistory = self.
-000082f0: 6178 4869 7374 6f72 795b 3a73 656c 662e  axHistory[:self.
-00008300: 6178 4869 7374 6f72 7950 6f69 6e74 6572  axHistoryPointer
-00008310: 5d20 2b20 5b61 785d 0d0a 0d0a 2020 2020  ] + [ax]....    
-00008320: 6465 6620 6d6f 7573 6543 6c69 636b 4576  def mouseClickEv
-00008330: 656e 7428 7365 6c66 2c20 6576 293a 0d0a  ent(self, ev):..
-00008340: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008350: 6d61 7374 6572 5f76 6965 7762 6f78 3a0d  master_viewbox:.
-00008360: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00008370: 7572 6e20 7365 6c66 2e6d 6173 7465 725f  urn self.master_
-00008380: 7669 6577 626f 782e 6d6f 7573 6543 6c69  viewbox.mouseCli
-00008390: 636b 4576 656e 7428 6576 290d 0a20 2020  ckEvent(ev)..   
-000083a0: 2020 2020 2069 6620 5f6d 6f75 7365 5f63       if _mouse_c
-000083b0: 6c69 636b 6564 2873 656c 662c 2065 7629  licked(self, ev)
-000083c0: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
-000083d0: 762e 6163 6365 7074 2829 0d0a 2020 2020  v.accept()..    
-000083e0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-000083f0: 2020 2020 2020 2020 6966 2065 762e 6275          if ev.bu
-00008400: 7474 6f6e 2829 2021 3d20 5174 436f 7265  tton() != QtCore
-00008410: 2e51 742e 4d6f 7573 6542 7574 746f 6e2e  .Qt.MouseButton.
-00008420: 4c65 6674 4275 7474 6f6e 206f 7220 6576  LeftButton or ev
-00008430: 2e6d 6f64 6966 6965 7273 2829 2021 3d20  .modifiers() != 
-00008440: 5174 436f 7265 2e51 742e 4b65 7962 6f61  QtCore.Qt.Keyboa
-00008450: 7264 4d6f 6469 6669 6572 2e43 6f6e 7472  rdModifier.Contr
-00008460: 6f6c 4d6f 6469 6669 6572 206f 7220 6e6f  olModifier or no
-00008470: 7420 7365 6c66 2e64 7261 775f 6c69 6e65  t self.draw_line
-00008480: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00008490: 6574 7572 6e20 7375 7065 7228 292e 6d6f  eturn super().mo
-000084a0: 7573 6543 6c69 636b 4576 656e 7428 6576  useClickEvent(ev
-000084b0: 290d 0a20 2020 2020 2020 2023 2061 6464  )..        # add
-000084c0: 2061 6e6f 7468 6572 2073 6567 6d65 6e74   another segment
-000084d0: 2074 6f20 7468 6520 6375 7272 656e 746c   to the currentl
-000084e0: 7920 6472 6177 6e20 6c69 6e65 0d0a 2020  y drawn line..  
-000084f0: 2020 2020 2020 7020 3d20 7365 6c66 2e6d        p = self.m
-00008500: 6170 436c 6963 6b54 6f56 6965 7728 6576  apClickToView(ev
-00008510: 2e70 6f73 2829 290d 0a20 2020 2020 2020  .pos())..       
-00008520: 2070 203d 205f 636c 616d 705f 706f 696e   p = _clamp_poin
-00008530: 7428 7365 6c66 2e70 6172 656e 7428 292c  t(self.parent(),
-00008540: 2070 290d 0a20 2020 2020 2020 2073 656c   p)..        sel
-00008550: 662e 6170 7065 6e64 5f64 7261 775f 7365  f.append_draw_se
-00008560: 676d 656e 7428 7029 0d0a 2020 2020 2020  gment(p)..      
-00008570: 2020 7365 6c66 2e64 7261 7769 6e67 203d    self.drawing =
-00008580: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00008590: 6576 2e61 6363 6570 7428 290d 0a0d 0a20  ev.accept().... 
-000085a0: 2020 2064 6566 206d 6170 436c 6963 6b54     def mapClickT
-000085b0: 6f56 6965 7728 7365 6c66 2c20 706f 7329  oView(self, pos)
-000085c0: 3a0d 0a20 2020 2020 2020 2027 2727 6d61  :..        '''ma
-000085d0: 7054 6f56 6965 7728 2920 646f 6573 206e  pToView() does n
-000085e0: 6f74 2064 6f20 6772 6964 7320 7072 6f70  ot do grids prop
-000085f0: 6572 6c79 2069 6e20 656d 6265 6464 6564  erly in embedded
-00008600: 2077 6964 6765 7473 2e20 5374 7261 6e67   widgets. Strang
-00008610: 656c 792c 206f 6e6c 7920 6166 6665 6374  ely, only affect
-00008620: 2063 6c69 636b 732c 206e 6f74 2064 7261   clicks, not dra
-00008630: 6773 2e27 2727 0d0a 2020 2020 2020 2020  gs.'''..        
-00008640: 6966 2073 656c 662e 7769 6e2e 7061 7265  if self.win.pare
-00008650: 6e74 2829 2069 7320 6e6f 7420 4e6f 6e65  nt() is not None
-00008660: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
-00008670: 7820 3d20 7365 6c66 2e70 6172 656e 7428  x = self.parent(
-00008680: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00008690: 6620 6178 2e67 6574 4178 6973 2827 7269  f ax.getAxis('ri
-000086a0: 6768 7427 292e 6772 6964 3a0d 0a20 2020  ght').grid:..   
-000086b0: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-000086c0: 2e73 6574 5828 706f 732e 7828 2920 2b20  .setX(pos.x() + 
-000086d0: 7365 6c66 2e77 6964 7468 2829 290d 0a20  self.width()).. 
-000086e0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000086f0: 6178 2e67 6574 4178 6973 2827 626f 7474  ax.getAxis('bott
-00008700: 6f6d 2729 2e67 7269 643a 0d0a 2020 2020  om').grid:..    
-00008710: 2020 2020 2020 2020 2020 2020 706f 732e              pos.
-00008720: 7365 7459 2870 6f73 2e79 2829 202b 2073  setY(pos.y() + s
-00008730: 656c 662e 6865 6967 6874 2829 290d 0a20  elf.height()).. 
-00008740: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00008750: 7065 7228 292e 6d61 7054 6f56 6965 7728  per().mapToView(
-00008760: 706f 7329 0d0a 0d0a 2020 2020 6465 6620  pos)....    def 
-00008770: 6b65 7950 7265 7373 4576 656e 7428 7365  keyPressEvent(se
-00008780: 6c66 2c20 6576 293a 0d0a 2020 2020 2020  lf, ev):..      
-00008790: 2020 6966 2073 656c 662e 6d61 7374 6572    if self.master
-000087a0: 5f76 6965 7762 6f78 3a0d 0a20 2020 2020  _viewbox:..     
-000087b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000087c0: 6c66 2e6d 6173 7465 725f 7669 6577 626f  lf.master_viewbo
-000087d0: 782e 6b65 7950 7265 7373 4576 656e 7428  x.keyPressEvent(
-000087e0: 6576 290d 0a20 2020 2020 2020 2069 6620  ev)..        if 
-000087f0: 5f6b 6579 5f70 7265 7373 6564 2873 656c  _key_pressed(sel
-00008800: 662c 2065 7629 3a0d 0a20 2020 2020 2020  f, ev):..       
-00008810: 2020 2020 2065 762e 6163 6365 7074 2829       ev.accept()
-00008820: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00008830: 7475 726e 0d0a 2020 2020 2020 2020 7375  turn..        su
-00008840: 7065 7228 292e 6b65 7950 7265 7373 4576  per().keyPressEv
-00008850: 656e 7428 6576 290d 0a0d 0a20 2020 2064  ent(ev)....    d
-00008860: 6566 206c 696e 6b65 6456 6965 7743 6861  ef linkedViewCha
-00008870: 6e67 6564 2873 656c 662c 2076 6965 772c  nged(self, view,
-00008880: 2061 7869 7329 3a0d 0a20 2020 2020 2020   axis):..       
-00008890: 2069 6620 6e6f 7420 7365 6c66 2e64 6174   if not self.dat
-000088a0: 6173 7263 206f 7220 7365 6c66 2e75 7064  asrc or self.upd
-000088b0: 6174 696e 675f 6c69 6e6b 6564 3a0d 0a20  ating_linked:.. 
-000088c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000088d0: 6e0d 0a20 2020 2020 2020 2069 6620 7669  n..        if vi
-000088e0: 6577 2061 6e64 2073 656c 662e 6461 7461  ew and self.data
-000088f0: 7372 6320 616e 6420 7669 6577 2e64 6174  src and view.dat
-00008900: 6173 7263 3a0d 0a20 2020 2020 2020 2020  asrc:..         
-00008910: 2020 2073 656c 662e 7570 6461 7469 6e67     self.updating
-00008920: 5f6c 696e 6b65 6420 3d20 5472 7565 0d0a  _linked = True..
-00008930: 2020 2020 2020 2020 2020 2020 7472 203d              tr =
-00008940: 2073 656c 662e 7461 7267 6574 5265 6374   self.targetRect
-00008950: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00008960: 7672 203d 2076 6965 772e 7461 7267 6574  vr = view.target
-00008970: 5265 6374 2829 0d0a 2020 2020 2020 2020  Rect()..        
-00008980: 2020 2020 6973 5f64 6972 7479 203d 2076      is_dirty = v
-00008990: 6965 772e 666f 7263 655f 7261 6e67 655f  iew.force_range_
-000089a0: 7570 6461 7465 203e 2030 0d0a 2020 2020  update > 0..    
-000089b0: 2020 2020 2020 2020 6973 5f73 616d 655f          is_same_
-000089c0: 7363 616c 6520 3d20 7365 6c66 2e64 6174  scale = self.dat
-000089d0: 6173 7263 2e78 6c65 6e20 3d3d 2076 6965  asrc.xlen == vie
-000089e0: 772e 6461 7461 7372 632e 786c 656e 0d0a  w.datasrc.xlen..
-000089f0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00008a00: 735f 7361 6d65 5f73 6361 6c65 3a20 2320  s_same_scale: # 
-00008a10: 7374 6162 6c65 207a 6f6f 6d20 6261 7365  stable zoom base
-00008a20: 6420 6f6e 2069 6e64 6578 0d0a 2020 2020  d on index..    
-00008a30: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00008a40: 735f 6469 7274 7920 6f72 2061 6273 2876  s_dirty or abs(v
-00008a50: 722e 6c65 6674 2829 2d74 722e 6c65 6674  r.left()-tr.left
-00008a60: 2829 2920 3e3d 2031 206f 7220 6162 7328  ()) >= 1 or abs(
-00008a70: 7672 2e72 6967 6874 2829 2d74 722e 7269  vr.right()-tr.ri
-00008a80: 6768 7428 2929 203e 3d20 313a 0d0a 2020  ght()) >= 1:..  
-00008a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008aa0: 2020 6966 2069 735f 6469 7274 793a 0d0a    if is_dirty:..
-00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ac0: 2020 2020 2020 2020 7669 6577 2e66 6f72          view.for
-00008ad0: 6365 5f72 616e 6765 5f75 7064 6174 6520  ce_range_update 
-00008ae0: 2d3d 2031 0d0a 2020 2020 2020 2020 2020  -= 1..          
-00008af0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00008b00: 7064 6174 655f 795f 7a6f 6f6d 2876 722e  pdate_y_zoom(vr.
-00008b10: 6c65 6674 2829 2c20 7672 2e72 6967 6874  left(), vr.right
-00008b20: 2829 290d 0a20 2020 2020 2020 2020 2020  ())..           
-00008b30: 2065 6c73 653a 2023 2073 6c6f 7070 7920   else: # sloppy 
-00008b40: 6f6e 6520 6261 7365 6420 6f6e 2074 696d  one based on tim
-00008b50: 6520 7374 616d 7073 0d0a 2020 2020 2020  e stamps..      
-00008b60: 2020 2020 2020 2020 2020 7474 302c 7474            tt0,tt
-00008b70: 312c 5f2c 5f2c 5f20 3d20 7365 6c66 2e64  1,_,_,_ = self.d
-00008b80: 6174 6173 7263 2e68 696c 6f28 7472 2e6c  atasrc.hilo(tr.l
-00008b90: 6566 7428 292c 2074 722e 7269 6768 7428  eft(), tr.right(
-00008ba0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00008bb0: 2020 2020 7674 302c 7674 312c 5f2c 5f2c      vt0,vt1,_,_,
-00008bc0: 5f20 3d20 7669 6577 2e64 6174 6173 7263  _ = view.datasrc
-00008bd0: 2e68 696c 6f28 7672 2e6c 6566 7428 292c  .hilo(vr.left(),
-00008be0: 2076 722e 7269 6768 7428 2929 0d0a 2020   vr.right())..  
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 7065                pe
-00008c00: 7269 6f64 3220 3d20 7365 6c66 2e64 6174  riod2 = self.dat
-00008c10: 6173 7263 2e70 6572 696f 645f 6e73 202a  asrc.period_ns *
-00008c20: 2030 2e35 0d0a 2020 2020 2020 2020 2020   0.5..          
-00008c30: 2020 2020 2020 6966 2069 735f 6469 7274        if is_dirt
-00008c40: 7920 6f72 2061 6273 2876 7430 2d74 7430  y or abs(vt0-tt0
-00008c50: 2920 3e3d 2070 6572 696f 6432 206f 7220  ) >= period2 or 
-00008c60: 6162 7328 7674 312d 7474 3129 203e 3d20  abs(vt1-tt1) >= 
-00008c70: 7065 7269 6f64 323a 0d0a 2020 2020 2020  period2:..      
-00008c80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00008c90: 2069 735f 6469 7274 793a 0d0a 2020 2020   is_dirty:..    
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cb0: 2020 2020 7669 6577 2e66 6f72 6365 5f72      view.force_r
-00008cc0: 616e 6765 5f75 7064 6174 6520 2d3d 2031  ange_update -= 1
-00008cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008ce0: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
-00008cf0: 7265 6e74 2829 3a0d 0a20 2020 2020 2020  rent():..       
-00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d10: 2078 302c 7831 203d 205f 7064 7469 6d65   x0,x1 = _pdtime
-00008d20: 3269 6e64 6578 2873 656c 662e 7061 7265  2index(self.pare
-00008d30: 6e74 2829 2c20 7064 2e53 6572 6965 7328  nt(), pd.Series(
-00008d40: 5b76 7430 2c76 7431 5d29 2c20 616e 795f  [vt0,vt1]), any_
-00008d50: 656e 643d 5472 7565 290d 0a20 2020 2020  end=True)..     
-00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d70: 2020 2073 656c 662e 7570 6461 7465 5f79     self.update_y
-00008d80: 5f7a 6f6f 6d28 7830 2c20 7831 290d 0a20  _zoom(x0, x1).. 
-00008d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008da0: 7570 6461 7469 6e67 5f6c 696e 6b65 6420  updating_linked 
-00008db0: 3d20 4661 6c73 650d 0a0d 0a20 2020 2064  = False....    d
-00008dc0: 6566 207a 6f6f 6d5f 7265 6374 2873 656c  ef zoom_rect(sel
-00008dd0: 662c 2076 722c 2073 6361 6c65 5f66 6163  f, vr, scale_fac
-00008de0: 742c 2063 656e 7465 7229 3a0d 0a20 2020  t, center):..   
-00008df0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00008e00: 2e64 6174 6173 7263 3a0d 0a20 2020 2020  .datasrc:..     
-00008e10: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-00008e20: 2020 2020 2020 2078 3020 3d20 6365 6e74         x0 = cent
-00008e30: 6572 2e78 2829 202b 2028 7672 2e6c 6566  er.x() + (vr.lef
-00008e40: 7428 292d 6365 6e74 6572 2e78 2829 2920  t()-center.x()) 
-00008e50: 2a20 7363 616c 655f 6661 6374 0d0a 2020  * scale_fact..  
-00008e60: 2020 2020 2020 7831 203d 2063 656e 7465        x1 = cente
-00008e70: 722e 7828 2920 2b20 2876 722e 7269 6768  r.x() + (vr.righ
-00008e80: 7428 292d 6365 6e74 6572 2e78 2829 2920  t()-center.x()) 
-00008e90: 2a20 7363 616c 655f 6661 6374 0d0a 2020  * scale_fact..  
-00008ea0: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
-00008eb0: 655f 795f 7a6f 6f6d 2878 302c 2078 3129  e_y_zoom(x0, x1)
-00008ec0: 0d0a 0d0a 2020 2020 6465 6620 7061 6e5f  ....    def pan_
-00008ed0: 7828 7365 6c66 2c20 7374 6570 733d 4e6f  x(self, steps=No
-00008ee0: 6e65 2c20 7065 7263 656e 743d 4e6f 6e65  ne, percent=None
-00008ef0: 293a 0d0a 2020 2020 2020 2020 6966 2073  ):..        if s
-00008f00: 656c 662e 6461 7461 7372 6320 6973 204e  elf.datasrc is N
-00008f10: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00008f20: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
-00008f30: 2020 6966 2073 7465 7073 2069 7320 4e6f    if steps is No
-00008f40: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00008f50: 2073 7465 7073 203d 2069 6e74 2870 6572   steps = int(per
-00008f60: 6365 6e74 2f31 3030 2a73 656c 662e 7461  cent/100*self.ta
-00008f70: 7267 6574 5265 6374 2829 2e77 6964 7468  rgetRect().width
-00008f80: 2829 290d 0a20 2020 2020 2020 2074 7220  ())..        tr 
-00008f90: 3d20 7365 6c66 2e74 6172 6765 7452 6563  = self.targetRec
-00008fa0: 7428 290d 0a20 2020 2020 2020 2078 3120  t()..        x1 
-00008fb0: 3d20 7472 2e72 6967 6874 2829 202b 2073  = tr.right() + s
-00008fc0: 7465 7073 0d0a 2020 2020 2020 2020 7374  teps..        st
-00008fd0: 6172 7478 203d 202d 7369 6465 5f6d 6172  artx = -side_mar
-00008fe0: 6769 6e0d 0a20 2020 2020 2020 2065 6e64  gin..        end
-00008ff0: 7820 3d20 7365 6c66 2e64 6174 6173 7263  x = self.datasrc
-00009000: 2e78 6c65 6e20 2b20 7269 6768 745f 6d61  .xlen + right_ma
-00009010: 7267 696e 5f63 616e 646c 6573 202d 2073  rgin_candles - s
-00009020: 6964 655f 6d61 7267 696e 0d0a 2020 2020  ide_margin..    
-00009030: 2020 2020 6966 2078 3120 3e20 656e 6478      if x1 > endx
-00009040: 3a0d 0a20 2020 2020 2020 2020 2020 2078  :..            x
-00009050: 3120 3d20 656e 6478 0d0a 2020 2020 2020  1 = endx..      
-00009060: 2020 7830 203d 2078 3120 2d20 7472 2e77    x0 = x1 - tr.w
-00009070: 6964 7468 2829 0d0a 2020 2020 2020 2020  idth()..        
-00009080: 6966 2078 3020 3c20 7374 6172 7478 3a0d  if x0 < startx:.
-00009090: 0a20 2020 2020 2020 2020 2020 2078 3020  .            x0 
-000090a0: 3d20 7374 6172 7478 0d0a 2020 2020 2020  = startx..      
-000090b0: 2020 2020 2020 7831 203d 2078 3020 2b20        x1 = x0 + 
-000090c0: 7472 2e77 6964 7468 2829 0d0a 2020 2020  tr.width()..    
-000090d0: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
-000090e0: 795f 7a6f 6f6d 2878 302c 2078 3129 0d0a  y_zoom(x0, x1)..
-000090f0: 0d0a 2020 2020 6465 6620 7265 6672 6573  ..    def refres
-00009100: 685f 616c 6c5f 795f 7a6f 6f6d 2873 656c  h_all_y_zoom(sel
-00009110: 6629 3a0d 0a20 2020 2020 2020 2027 2727  f):..        '''
-00009120: 5468 6973 2075 7064 6174 6573 2059 207a  This updates Y z
-00009130: 6f6f 6d20 6f6e 2061 6c6c 2076 6965 7773  oom on all views
-00009140: 2c20 7375 6368 2061 7320 7768 656e 2061  , such as when a
-00009150: 206d 6f75 7365 2064 7261 6720 6973 2063   mouse drag is c
-00009160: 6f6d 706c 6574 6564 2e27 2727 0d0a 2020  ompleted.'''..  
-00009170: 2020 2020 2020 6d61 696e 5f76 6220 3d20        main_vb = 
-00009180: 7365 6c66 0d0a 2020 2020 2020 2020 6966  self..        if
-00009190: 2073 656c 662e 6c69 6e6b 6564 5669 6577   self.linkedView
-000091a0: 2830 293a 0d0a 2020 2020 2020 2020 2020  (0):..          
-000091b0: 2020 7365 6c66 2e66 6f72 6365 5f72 616e    self.force_ran
-000091c0: 6765 5f75 7064 6174 6520 3d20 3120 2320  ge_update = 1 # 
-000091d0: 6d61 696e 206e 6565 6420 746f 2075 7064  main need to upd
-000091e0: 6174 6520 6f6e 6c79 206f 6e63 6520 746f  ate only once to
-000091f0: 2075 730d 0a20 2020 2020 2020 2020 2020   us..           
-00009200: 206d 6169 6e5f 7662 203d 206c 6973 7428   main_vb = list(
-00009210: 7365 6c66 2e77 696e 2e61 7873 295b 305d  self.win.axs)[0]
-00009220: 2e76 620d 0a20 2020 2020 2020 206d 6169  .vb..        mai
-00009230: 6e5f 7662 2e66 6f72 6365 5f72 616e 6765  n_vb.force_range
-00009240: 5f75 7064 6174 6520 3d20 6c65 6e28 7365  _update = len(se
-00009250: 6c66 2e77 696e 2e61 7873 292d 3120 2320  lf.win.axs)-1 # 
-00009260: 7570 6461 7465 206d 6169 6e20 6173 206d  update main as m
-00009270: 616e 7920 7469 6d65 7320 6173 2074 6865  any times as the
-00009280: 7265 2061 7265 206f 7468 6572 2072 6f77  re are other row
-00009290: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-000092a0: 7570 6461 7465 5f79 5f7a 6f6f 6d28 290d  update_y_zoom().
-000092b0: 0a20 2020 2020 2020 2023 2072 6566 7265  .        # refre
-000092c0: 7368 2063 726f 7373 6861 6972 2077 6865  sh crosshair whe
-000092d0: 6e20 646f 6e65 0d0a 2020 2020 2020 2020  n done..        
-000092e0: 5f6d 6f75 7365 5f6d 6f76 6564 2873 656c  _mouse_moved(sel
-000092f0: 662e 7769 6e2c 204e 6f6e 6529 0d0a 0d0a  f.win, None)....
-00009300: 2020 2020 6465 6620 7570 6461 7465 5f79      def update_y
-00009310: 5f7a 6f6f 6d28 7365 6c66 2c20 7830 3d4e  _zoom(self, x0=N
-00009320: 6f6e 652c 2078 313d 4e6f 6e65 293a 0d0a  one, x1=None):..
-00009330: 2020 2020 2020 2020 6461 7461 7372 6320          datasrc 
-00009340: 3d20 7365 6c66 2e64 6174 6173 7263 5f6f  = self.datasrc_o
-00009350: 725f 7374 616e 6461 6c6f 6e65 0d0a 2020  r_standalone..  
-00009360: 2020 2020 2020 6966 2064 6174 6173 7263        if datasrc
-00009370: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00009380: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-00009390: 2020 2020 2020 2069 6620 7830 2069 7320         if x0 is 
-000093a0: 4e6f 6e65 206f 7220 7831 2069 7320 4e6f  None or x1 is No
-000093b0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000093c0: 2074 7220 3d20 7365 6c66 2e74 6172 6765   tr = self.targe
-000093d0: 7452 6563 7428 290d 0a20 2020 2020 2020  tRect()..       
-000093e0: 2020 2020 2078 3020 3d20 7472 2e6c 6566       x0 = tr.lef
-000093f0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-00009400: 2078 3120 3d20 7472 2e72 6967 6874 2829   x1 = tr.right()
-00009410: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00009420: 2078 312d 7830 203c 3d20 313a 0d0a 2020   x1-x0 <= 1:..  
-00009430: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00009440: 7475 726e 0d0a 2020 2020 2020 2020 2320  turn..        # 
-00009450: 6d61 6b65 2065 6467 6573 2072 6967 6964  make edges rigid
-00009460: 0d0a 2020 2020 2020 2020 786c 203d 206d  ..        xl = m
-00009470: 6178 285f 726f 756e 6428 7830 2d73 6964  ax(_round(x0-sid
-00009480: 655f 6d61 7267 696e 292b 7369 6465 5f6d  e_margin)+side_m
-00009490: 6172 6769 6e2c 202d 7369 6465 5f6d 6172  argin, -side_mar
-000094a0: 6769 6e29 0d0a 2020 2020 2020 2020 7872  gin)..        xr
-000094b0: 203d 206d 696e 285f 726f 756e 6428 7831   = min(_round(x1
-000094c0: 2d73 6964 655f 6d61 7267 696e 292b 7369  -side_margin)+si
-000094d0: 6465 5f6d 6172 6769 6e2c 2064 6174 6173  de_margin, datas
-000094e0: 7263 2e78 6c65 6e2b 7269 6768 745f 6d61  rc.xlen+right_ma
-000094f0: 7267 696e 5f63 616e 646c 6573 2d73 6964  rgin_candles-sid
-00009500: 655f 6d61 7267 696e 290d 0a20 2020 2020  e_margin)..     
-00009510: 2020 2064 786c 203d 2078 6c2d 7830 0d0a     dxl = xl-x0..
-00009520: 2020 2020 2020 2020 6478 7220 3d20 7872          dxr = xr
-00009530: 2d78 310d 0a20 2020 2020 2020 2069 6620  -x1..        if 
-00009540: 6478 6c20 3e20 303a 0d0a 2020 2020 2020  dxl > 0:..      
-00009550: 2020 2020 2020 7831 202b 3d20 6478 6c0d        x1 += dxl.
-00009560: 0a20 2020 2020 2020 2069 6620 6478 7220  .        if dxr 
-00009570: 3c20 303a 0d0a 2020 2020 2020 2020 2020  < 0:..          
-00009580: 2020 7830 202b 3d20 6478 720d 0a20 2020    x0 += dxr..   
-00009590: 2020 2020 2078 3020 3d20 6d61 7828 5f72       x0 = max(_r
-000095a0: 6f75 6e64 2878 302d 7369 6465 5f6d 6172  ound(x0-side_mar
-000095b0: 6769 6e29 2b73 6964 655f 6d61 7267 696e  gin)+side_margin
-000095c0: 2c20 2d73 6964 655f 6d61 7267 696e 290d  , -side_margin).
-000095d0: 0a20 2020 2020 2020 2078 3120 3d20 6d69  .        x1 = mi
-000095e0: 6e28 5f72 6f75 6e64 2878 312d 7369 6465  n(_round(x1-side
-000095f0: 5f6d 6172 6769 6e29 2b73 6964 655f 6d61  _margin)+side_ma
-00009600: 7267 696e 2c20 6461 7461 7372 632e 786c  rgin, datasrc.xl
-00009610: 656e 2b72 6967 6874 5f6d 6172 6769 6e5f  en+right_margin_
-00009620: 6361 6e64 6c65 732d 7369 6465 5f6d 6172  candles-side_mar
-00009630: 6769 6e29 0d0a 2020 2020 2020 2020 2320  gin)..        # 
-00009640: 6665 7463 6820 6869 2d6c 6f20 616e 6420  fetch hi-lo and 
-00009650: 7365 7420 7261 6e67 650d 0a20 2020 2020  set range..     
-00009660: 2020 205f 2c5f 2c68 692c 6c6f 2c63 6e74     _,_,hi,lo,cnt
-00009670: 203d 2064 6174 6173 7263 2e68 696c 6f28   = datasrc.hilo(
-00009680: 7830 2c20 7831 290d 0a20 2020 2020 2020  x0, x1)..       
-00009690: 2076 7220 3d20 7365 6c66 2e76 6965 7752   vr = self.viewR
-000096a0: 6563 7428 290d 0a20 2020 2020 2020 206d  ect()..        m
-000096b0: 696e 6c65 6e20 3d20 696e 7428 286d 6178  inlen = int((max
-000096c0: 5f7a 6f6f 6d5f 706f 696e 7473 2d30 2e35  _zoom_points-0.5
-000096d0: 2920 2a20 7365 6c66 2e6d 6178 5f7a 6f6f  ) * self.max_zoo
-000096e0: 6d5f 706f 696e 7473 5f66 202b 2030 2e35  m_points_f + 0.5
-000096f0: 3129 0d0a 2020 2020 2020 2020 6966 2028  1)..        if (
-00009700: 7831 2d78 3029 203c 2076 722e 7769 6474  x1-x0) < vr.widt
-00009710: 6828 2920 616e 6420 636e 7420 3c20 6d69  h() and cnt < mi
-00009720: 6e6c 656e 3a0d 0a20 2020 2020 2020 2020  nlen:..         
-00009730: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-00009740: 2020 2069 6620 6e6f 7420 7365 6c66 2e76     if not self.v
-00009750: 5f61 7574 6f7a 6f6f 6d3a 0d0a 2020 2020  _autozoom:..    
-00009760: 2020 2020 2020 2020 6869 203d 2076 722e          hi = vr.
-00009770: 626f 7474 6f6d 2829 0d0a 2020 2020 2020  bottom()..      
-00009780: 2020 2020 2020 6c6f 203d 2076 722e 746f        lo = vr.to
-00009790: 7028 290d 0a20 2020 2020 2020 2069 6620  p()..        if 
-000097a0: 7365 6c66 2e79 7363 616c 652e 7363 616c  self.yscale.scal
-000097b0: 6574 7970 6520 3d3d 2027 6c6f 6727 3a0d  etype == 'log':.
-000097c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000097d0: 6c6f 203c 2030 3a0d 0a20 2020 2020 2020  lo < 0:..       
-000097e0: 2020 2020 2020 2020 206c 6f20 3d20 302e           lo = 0.
-000097f0: 3035 202a 2073 656c 662e 7973 6361 6c65  05 * self.yscale
-00009800: 2e73 6361 6c65 6620 2320 7374 7261 6e67  .scalef # strang
-00009810: 6520 5154 206c 6f67 2073 6361 6c65 2072  e QT log scale r
-00009820: 656e 6465 7269 6e67 2c20 7768 6963 6820  endering, which 
-00009830: 4927 6d20 756e 6162 6c65 2074 6f20 636f  I'm unable to co
-00009840: 6d70 656e 7361 7465 2066 6f72 0d0a 2020  mpensate for..  
-00009850: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00009860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009870: 206c 6f20 3d20 6d61 7828 3165 2d31 3030   lo = max(1e-100
-00009880: 2c20 6c6f 290d 0a20 2020 2020 2020 2020  , lo)..         
-00009890: 2020 2072 6e67 203d 2028 6869 202f 206c     rng = (hi / l
-000098a0: 6f29 202a 2a20 2831 2f73 656c 662e 765f  o) ** (1/self.v_
-000098b0: 7a6f 6f6d 5f73 6361 6c65 290d 0a20 2020  zoom_scale)..   
-000098c0: 2020 2020 2020 2020 2072 6e67 203d 206d           rng = m
-000098d0: 696e 2872 6e67 2c20 3165 3530 2920 2320  in(rng, 1e50) # 
-000098e0: 6176 6f69 6420 666c 6f61 7420 6f76 6572  avoid float over
-000098f0: 666c 6f77 0d0a 2020 2020 2020 2020 2020  flow..          
-00009900: 2020 6261 7365 203d 2028 6869 2a6c 6f29    base = (hi*lo)
-00009910: 202a 2a20 7365 6c66 2e76 5f7a 6f6f 6d5f   ** self.v_zoom_
-00009920: 6261 7365 6c69 6e65 0d0a 2020 2020 2020  baseline..      
-00009930: 2020 2020 2020 7930 203d 2062 6173 6520        y0 = base 
-00009940: 2f20 726e 672a 2a73 656c 662e 765f 7a6f  / rng**self.v_zo
-00009950: 6f6d 5f62 6173 656c 696e 650d 0a20 2020  om_baseline..   
-00009960: 2020 2020 2020 2020 2079 3120 3d20 6261           y1 = ba
-00009970: 7365 202a 2072 6e67 2a2a 2831 2d73 656c  se * rng**(1-sel
-00009980: 662e 765f 7a6f 6f6d 5f62 6173 656c 696e  f.v_zoom_baselin
-00009990: 6529 0d0a 2020 2020 2020 2020 656c 7365  e)..        else
-000099a0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000099b0: 6e67 203d 2028 6869 2d6c 6f29 202f 2073  ng = (hi-lo) / s
-000099c0: 656c 662e 765f 7a6f 6f6d 5f73 6361 6c65  elf.v_zoom_scale
-000099d0: 0d0a 2020 2020 2020 2020 2020 2020 726e  ..            rn
-000099e0: 6720 3d20 6d61 7828 726e 672c 2032 652d  g = max(rng, 2e-
-000099f0: 3729 2023 2073 6f6d 6520 7665 7279 2077  7) # some very w
-00009a00: 6569 7264 2062 7567 2077 6865 7265 2068  eird bug where h
-00009a10: 6967 682f 6c6f 7720 6578 706f 6e65 6e74  igh/low exponent
-00009a20: 7320 7374 6f70 7320 7265 6e64 6572 696e  s stops renderin
-00009a30: 670d 0a20 2020 2020 2020 2020 2020 2062  g..            b
-00009a40: 6173 6520 3d20 2868 692b 6c6f 2920 2a20  ase = (hi+lo) * 
-00009a50: 7365 6c66 2e76 5f7a 6f6f 6d5f 6261 7365  self.v_zoom_base
-00009a60: 6c69 6e65 0d0a 2020 2020 2020 2020 2020  line..          
-00009a70: 2020 7930 203d 2062 6173 6520 2d20 726e    y0 = base - rn
-00009a80: 672a 7365 6c66 2e76 5f7a 6f6f 6d5f 6261  g*self.v_zoom_ba
-00009a90: 7365 6c69 6e65 0d0a 2020 2020 2020 2020  seline..        
-00009aa0: 2020 2020 7931 203d 2062 6173 6520 2b20      y1 = base + 
-00009ab0: 726e 672a 2831 2d73 656c 662e 765f 7a6f  rng*(1-self.v_zo
-00009ac0: 6f6d 5f62 6173 656c 696e 6529 0d0a 2020  om_baseline)..  
-00009ad0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00009ae0: 662e 785f 696e 6465 7865 643a 0d0a 2020  f.x_indexed:..  
-00009af0: 2020 2020 2020 2020 2020 7830 2c78 3120            x0,x1 
-00009b00: 3d20 5f78 6d69 6e6d 6178 2864 6174 6173  = _xminmax(datas
-00009b10: 7263 2c20 785f 696e 6465 7865 643d 4661  rc, x_indexed=Fa
-00009b20: 6c73 652c 2065 7874 7261 5f6d 6172 6769  lse, extra_margi
-00009b30: 6e3d 3029 0d0a 2020 2020 2020 2020 7265  n=0)..        re
-00009b40: 7475 726e 2073 656c 662e 7365 745f 7261  turn self.set_ra
-00009b50: 6e67 6528 7830 2c20 7930 2c20 7831 2c20  nge(x0, y0, x1, 
-00009b60: 7931 290d 0a0d 0a20 2020 2064 6566 2073  y1)....    def s
-00009b70: 6574 5f72 616e 6765 2873 656c 662c 2078  et_range(self, x
-00009b80: 302c 2079 302c 2078 312c 2079 3129 3a0d  0, y0, x1, y1):.
-00009b90: 0a20 2020 2020 2020 2069 6620 7830 2069  .        if x0 i
-00009ba0: 7320 4e6f 6e65 206f 7220 7831 2069 7320  s None or x1 is 
-00009bb0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00009bc0: 2020 2074 7220 3d20 7365 6c66 2e74 6172     tr = self.tar
-00009bd0: 6765 7452 6563 7428 290d 0a20 2020 2020  getRect()..     
-00009be0: 2020 2020 2020 2078 3020 3d20 7472 2e6c         x0 = tr.l
-00009bf0: 6566 7428 290d 0a20 2020 2020 2020 2020  eft()..         
-00009c00: 2020 2078 3120 3d20 7472 2e72 6967 6874     x1 = tr.right
-00009c10: 2829 0d0a 2020 2020 2020 2020 6966 206e  ()..        if n
-00009c20: 702e 6973 6e61 6e28 7930 2920 6f72 206e  p.isnan(y0) or n
-00009c30: 702e 6973 6e61 6e28 7931 293a 0d0a 2020  p.isnan(y1):..  
-00009c40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009c50: 0d0a 2020 2020 2020 2020 5f79 3020 3d20  ..        _y0 = 
-00009c60: 7365 6c66 2e79 7363 616c 652e 696e 7678  self.yscale.invx
-00009c70: 666f 726d 2879 302c 2076 6572 6966 793d  form(y0, verify=
-00009c80: 5472 7565 290d 0a20 2020 2020 2020 205f  True)..        _
-00009c90: 7931 203d 2073 656c 662e 7973 6361 6c65  y1 = self.yscale
-00009ca0: 2e69 6e76 7866 6f72 6d28 7931 2c20 7665  .invxform(y1, ve
-00009cb0: 7269 6679 3d54 7275 6529 0d0a 2020 2020  rify=True)..    
-00009cc0: 2020 2020 7365 6c66 2e73 6574 5261 6e67      self.setRang
-00009cd0: 6528 5174 436f 7265 2e51 5265 6374 4628  e(QtCore.QRectF(
-00009ce0: 7067 2e50 6f69 6e74 2878 302c 205f 7930  pg.Point(x0, _y0
-00009cf0: 292c 2070 672e 506f 696e 7428 7831 2c20  ), pg.Point(x1, 
-00009d00: 5f79 3129 292c 2070 6164 6469 6e67 3d30  _y1)), padding=0
-00009d10: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00009d20: 6e20 5472 7565 0d0a 0d0a 2020 2020 6465  n True....    de
-00009d30: 6620 7265 6d6f 7665 5f6c 6173 745f 726f  f remove_last_ro
-00009d40: 6928 7365 6c66 293a 0d0a 2020 2020 2020  i(self):..      
-00009d50: 2020 6966 2073 656c 662e 726f 6973 3a0d    if self.rois:.
-00009d60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00009d70: 6e6f 7420 6973 696e 7374 616e 6365 2873  not isinstance(s
-00009d80: 656c 662e 726f 6973 5b2d 315d 2c20 7067  elf.rois[-1], pg
-00009d90: 2e50 6f6c 794c 696e 6552 4f49 293a 0d0a  .PolyLineROI):..
-00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009db0: 7365 6c66 2e72 656d 6f76 6549 7465 6d28  self.removeItem(
-00009dc0: 7365 6c66 2e72 6f69 735b 2d31 5d29 0d0a  self.rois[-1])..
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 7365 6c66 2e72 6f69 7320 3d20 7365 6c66  self.rois = self
-00009df0: 2e72 6f69 735b 3a2d 315d 0d0a 2020 2020  .rois[:-1]..    
-00009e00: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00009e20: 203d 2073 656c 662e 726f 6973 5b2d 315d   = self.rois[-1]
-00009e30: 2e68 616e 646c 6573 5b2d 315d 5b27 6974  .handles[-1]['it
-00009e40: 656d 275d 0d0a 2020 2020 2020 2020 2020  em']..          
-00009e50: 2020 2020 2020 7365 6c66 2e72 6f69 735b        self.rois[
-00009e60: 2d31 5d2e 7265 6d6f 7665 4861 6e64 6c65  -1].removeHandle
-00009e70: 2868 290d 0a20 2020 2020 2020 2020 2020  (h)..           
-00009e80: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00009e90: 2e72 6f69 735b 2d31 5d2e 7365 676d 656e  .rois[-1].segmen
-00009ea0: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-00009eb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00009ec0: 6d6f 7665 4974 656d 2873 656c 662e 726f  moveItem(self.ro
-00009ed0: 6973 5b2d 315d 290d 0a20 2020 2020 2020  is[-1])..       
-00009ee0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00009ef0: 662e 726f 6973 203d 2073 656c 662e 726f  f.rois = self.ro
-00009f00: 6973 5b3a 2d31 5d0d 0a20 2020 2020 2020  is[:-1]..       
-00009f10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00009f20: 662e 6472 6177 5f6c 696e 6520 3d20 4e6f  f.draw_line = No
-00009f30: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00009f40: 6966 2073 656c 662e 726f 6973 3a0d 0a20  if self.rois:.. 
-00009f50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009f60: 6620 6973 696e 7374 616e 6365 2873 656c  f isinstance(sel
-00009f70: 662e 726f 6973 5b2d 315d 2c20 7067 2e50  f.rois[-1], pg.P
-00009f80: 6f6c 794c 696e 6552 4f49 293a 0d0a 2020  olyLineROI):..  
-00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fa0: 2020 7365 6c66 2e64 7261 775f 6c69 6e65    self.draw_line
-00009fb0: 203d 2073 656c 662e 726f 6973 5b2d 315d   = self.rois[-1]
-00009fc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009fd0: 2020 2020 2020 7365 6c66 2e73 6574 5f64        self.set_d
-00009fe0: 7261 775f 6c69 6e65 5f63 6f6c 6f72 2864  raw_line_color(d
-00009ff0: 7261 775f 6c69 6e65 5f63 6f6c 6f72 290d  raw_line_color).
-0000a000: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000a010: 7572 6e20 5472 7565 0d0a 0d0a 2020 2020  urn True....    
-0000a020: 6465 6620 6170 7065 6e64 5f64 7261 775f  def append_draw_
-0000a030: 7365 676d 656e 7428 7365 6c66 2c20 7029  segment(self, p)
-0000a040: 3a0d 0a20 2020 2020 2020 2068 3020 3d20  :..        h0 = 
-0000a050: 7365 6c66 2e64 7261 775f 6c69 6e65 2e68  self.draw_line.h
-0000a060: 616e 646c 6573 5b2d 315d 5b27 6974 656d  andles[-1]['item
-0000a070: 275d 0d0a 2020 2020 2020 2020 6831 203d  ']..        h1 =
-0000a080: 2073 656c 662e 6472 6177 5f6c 696e 652e   self.draw_line.
-0000a090: 6164 6446 7265 6548 616e 646c 6528 7029  addFreeHandle(p)
-0000a0a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
-0000a0b0: 7261 775f 6c69 6e65 2e61 6464 5365 676d  raw_line.addSegm
-0000a0c0: 656e 7428 6830 2c20 6831 290d 0a20 2020  ent(h0, h1)..   
-0000a0d0: 2020 2020 2073 656c 662e 6472 6177 696e       self.drawin
-0000a0e0: 6720 3d20 5472 7565 0d0a 0d0a 2020 2020  g = True....    
-0000a0f0: 6465 6620 7365 745f 6472 6177 5f6c 696e  def set_draw_lin
-0000a100: 655f 636f 6c6f 7228 7365 6c66 2c20 636f  e_color(self, co
-0000a110: 6c6f 7229 3a0d 0a20 2020 2020 2020 2069  lor):..        i
-0000a120: 6620 7365 6c66 2e64 7261 775f 6c69 6e65  f self.draw_line
-0000a130: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-0000a140: 656e 203d 2070 672e 6d6b 5065 6e28 636f  en = pg.mkPen(co
-0000a150: 6c6f 7229 0d0a 2020 2020 2020 2020 2020  lor)..          
-0000a160: 2020 666f 7220 7365 676d 656e 7420 696e    for segment in
-0000a170: 2073 656c 662e 6472 6177 5f6c 696e 652e   self.draw_line.
-0000a180: 7365 676d 656e 7473 3a0d 0a20 2020 2020  segments:..     
-0000a190: 2020 2020 2020 2020 2020 2073 6567 6d65             segme
-0000a1a0: 6e74 2e63 7572 7265 6e74 5065 6e20 3d20  nt.currentPen = 
-0000a1b0: 7365 676d 656e 742e 7065 6e20 3d20 7065  segment.pen = pe
-0000a1c0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-0000a1d0: 2020 2073 6567 6d65 6e74 2e75 7064 6174     segment.updat
-0000a1e0: 6528 290d 0a0d 0a20 2020 2064 6566 2073  e()....    def s
-0000a1f0: 7567 6765 7374 5061 6464 696e 6728 7365  uggestPadding(se
-0000a200: 6c66 2c20 6178 6973 293a 0d0a 2020 2020  lf, axis):..    
-0000a210: 2020 2020 7265 7475 726e 2030 0d0a 0d0a      return 0....
-0000a220: 0d0a 0d0a 636c 6173 7320 4669 6e50 6c6f  ....class FinPlo
-0000a230: 7449 7465 6d28 7067 2e47 7261 7068 6963  tItem(pg.Graphic
-0000a240: 734f 626a 6563 7429 3a0d 0a20 2020 2064  sObject):..    d
-0000a250: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000a260: 2c20 6178 2c20 6461 7461 7372 632c 206c  , ax, datasrc, l
-0000a270: 6f64 293a 0d0a 2020 2020 2020 2020 7375  od):..        su
-0000a280: 7065 7228 292e 5f5f 696e 6974 5f5f 2829  per().__init__()
-0000a290: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0000a2a0: 7820 3d20 6178 0d0a 2020 2020 2020 2020  x = ax..        
-0000a2b0: 7365 6c66 2e64 6174 6173 7263 203d 2064  self.datasrc = d
-0000a2c0: 6174 6173 7263 0d0a 2020 2020 2020 2020  atasrc..        
-0000a2d0: 7365 6c66 2e70 6963 7475 7265 203d 2051  self.picture = Q
-0000a2e0: 7447 7569 2e51 5069 6374 7572 6528 290d  tGui.QPicture().
-0000a2f0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
-0000a300: 696e 7465 7220 3d20 5174 4775 692e 5150  inter = QtGui.QP
-0000a310: 6169 6e74 6572 2829 0d0a 2020 2020 2020  ainter()..      
-0000a320: 2020 7365 6c66 2e64 6972 7479 203d 2054    self.dirty = T
-0000a330: 7275 650d 0a20 2020 2020 2020 2073 656c  rue..        sel
-0000a340: 662e 6c6f 6420 3d20 6c6f 640d 0a20 2020  f.lod = lod..   
-0000a350: 2020 2020 2073 656c 662e 6361 6368 6564       self.cached
-0000a360: 5265 6374 203d 204e 6f6e 650d 0a0d 0a20  Rect = None.... 
-0000a370: 2020 2064 6566 2072 6570 6169 6e74 2873     def repaint(s
-0000a380: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-0000a390: 656c 662e 6469 7274 7920 3d20 5472 7565  elf.dirty = True
-0000a3a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-0000a3b0: 6169 6e74 2873 656c 662e 7061 696e 7465  aint(self.painte
-0000a3c0: 7229 0d0a 0d0a 2020 2020 6465 6620 7061  r)....    def pa
-0000a3d0: 696e 7428 7365 6c66 2c20 702c 202a 6172  int(self, p, *ar
-0000a3e0: 6773 293a 0d0a 2020 2020 2020 2020 6966  gs):..        if
-0000a3f0: 2073 656c 662e 6461 7461 7372 632e 6973   self.datasrc.is
-0000a400: 5f73 7061 7273 653a 0d0a 2020 2020 2020  _sparse:..      
-0000a410: 2020 2020 2020 7365 6c66 2e64 6972 7479        self.dirty
-0000a420: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-0000a430: 2073 656c 662e 7570 6461 7465 5f64 6972   self.update_dir
-0000a440: 7479 5f70 6963 7475 7265 2873 656c 662e  ty_picture(self.
-0000a450: 7669 6577 5265 6374 2829 290d 0a20 2020  viewRect())..   
-0000a460: 2020 2020 2070 2e64 7261 7750 6963 7475       p.drawPictu
-0000a470: 7265 2830 2c20 302c 2073 656c 662e 7069  re(0, 0, self.pi
-0000a480: 6374 7572 6529 0d0a 0d0a 2020 2020 6465  cture)....    de
-0000a490: 6620 7570 6461 7465 5f64 6972 7479 5f70  f update_dirty_p
-0000a4a0: 6963 7475 7265 2873 656c 662c 2076 6973  icture(self, vis
-0000a4b0: 6962 6c65 5265 6374 293a 0d0a 2020 2020  ibleRect):..    
-0000a4c0: 2020 2020 6966 2073 656c 662e 6469 7274      if self.dirt
-0000a4d0: 7920 6f72 205c 0d0a 2020 2020 2020 2020  y or \..        
-0000a4e0: 2020 2020 2873 656c 662e 6c6f 6420 616e      (self.lod an
-0000a4f0: 6420 2320 7265 6765 6e65 7261 7465 2077  d # regenerate w
-0000a500: 6865 6e20 7a6f 6f6d 2063 6861 6e67 6573  hen zoom changes
-0000a510: 3f0d 0a20 2020 2020 2020 2020 2020 2020  ?..             
-0000a520: 2020 2028 7669 7369 626c 6552 6563 742e     (visibleRect.
-0000a530: 6c65 6674 2829 203c 2073 656c 662e 6361  left() < self.ca
-0000a540: 6368 6564 5265 6374 2e6c 6566 7428 2920  chedRect.left() 
-0000a550: 6f72 205c 0d0a 2020 2020 2020 2020 2020  or \..          
-0000a560: 2020 2020 2020 2076 6973 6962 6c65 5265         visibleRe
-0000a570: 6374 2e72 6967 6874 2829 203e 2073 656c  ct.right() > sel
-0000a580: 662e 6361 6368 6564 5265 6374 2e72 6967  f.cachedRect.rig
-0000a590: 6874 2829 206f 7220 5c0d 0a20 2020 2020  ht() or \..     
-0000a5a0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
-0000a5b0: 626c 6552 6563 742e 7769 6474 6828 2920  bleRect.width() 
-0000a5c0: 3c20 7365 6c66 2e63 6163 6865 6452 6563  < self.cachedRec
-0000a5d0: 742e 7769 6474 6828 2920 2f20 6361 6368  t.width() / cach
-0000a5e0: 655f 6361 6e64 6c65 5f66 6163 746f 7229  e_candle_factor)
-0000a5f0: 293a 2023 206f 7074 696d 697a 6520 7768  ): # optimize wh
-0000a600: 656e 207a 6f6f 6d69 6e67 2069 6e0d 0a20  en zooming in.. 
-0000a610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a620: 5f67 656e 6572 6174 655f 7069 6374 7572  _generate_pictur
-0000a630: 6528 7669 7369 626c 6552 6563 7429 0d0a  e(visibleRect)..
-0000a640: 0d0a 2020 2020 6465 6620 5f67 656e 6572  ..    def _gener
-0000a650: 6174 655f 7069 6374 7572 6528 7365 6c66  ate_picture(self
-0000a660: 2c20 626f 756e 6469 6e67 5265 6374 293a  , boundingRect):
-0000a670: 0d0a 2020 2020 2020 2020 7720 3d20 626f  ..        w = bo
-0000a680: 756e 6469 6e67 5265 6374 2e77 6964 7468  undingRect.width
-0000a690: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-0000a6a0: 2e63 6163 6865 6452 6563 7420 3d20 5174  .cachedRect = Qt
-0000a6b0: 436f 7265 2e51 5265 6374 4628 626f 756e  Core.QRectF(boun
-0000a6c0: 6469 6e67 5265 6374 2e6c 6566 7428 292d  dingRect.left()-
-0000a6d0: 2863 6163 6865 5f63 616e 646c 655f 6661  (cache_candle_fa
-0000a6e0: 6374 6f72 2d31 292a 302e 352a 772c 2030  ctor-1)*0.5*w, 0
-0000a6f0: 2c20 6361 6368 655f 6361 6e64 6c65 5f66  , cache_candle_f
-0000a700: 6163 746f 722a 772c 2030 290d 0a20 2020  actor*w, 0)..   
-0000a710: 2020 2020 2073 656c 662e 7061 696e 7465       self.painte
-0000a720: 722e 6265 6769 6e28 7365 6c66 2e70 6963  r.begin(self.pic
-0000a730: 7475 7265 290d 0a20 2020 2020 2020 2073  ture)..        s
-0000a740: 656c 662e 5f67 656e 6572 6174 655f 6475  elf._generate_du
-0000a750: 6d6d 795f 7069 6374 7572 6528 7365 6c66  mmy_picture(self
-0000a760: 2e76 6965 7752 6563 7428 2929 0d0a 2020  .viewRect())..  
-0000a770: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-0000a780: 6174 655f 7069 6374 7572 6528 7365 6c66  ate_picture(self
-0000a790: 2e63 6163 6865 6452 6563 7429 0d0a 2020  .cachedRect)..  
-0000a7a0: 2020 2020 2020 7365 6c66 2e70 6169 6e74        self.paint
-0000a7b0: 6572 2e65 6e64 2829 0d0a 2020 2020 2020  er.end()..      
-0000a7c0: 2020 7365 6c66 2e64 6972 7479 203d 2046    self.dirty = F
-0000a7d0: 616c 7365 0d0a 0d0a 2020 2020 6465 6620  alse....    def 
-0000a7e0: 5f67 656e 6572 6174 655f 6475 6d6d 795f  _generate_dummy_
-0000a7f0: 7069 6374 7572 6528 7365 6c66 2c20 626f  picture(self, bo
-0000a800: 756e 6469 6e67 5265 6374 293a 0d0a 2020  undingRect):..  
-0000a810: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
-0000a820: 7461 7372 632e 6973 5f73 7061 7273 653a  tasrc.is_sparse:
-0000a830: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000a840: 6a75 7374 2064 7261 7720 736f 6d65 7468  just draw someth
-0000a850: 696e 6720 746f 2065 6e73 7572 6520 5079  ing to ensure Py
-0000a860: 5174 2077 696c 6c20 7061 696e 7420 7573  Qt will paint us
-0000a870: 2061 6761 696e 0d0a 2020 2020 2020 2020   again..        
-0000a880: 2020 2020 7365 6c66 2e70 6169 6e74 6572      self.painter
-0000a890: 2e73 6574 5065 6e28 7067 2e6d 6b50 656e  .setPen(pg.mkPen
-0000a8a0: 2862 6163 6b67 726f 756e 6429 290d 0a20  (background)).. 
-0000a8b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a8c0: 7061 696e 7465 722e 7365 7442 7275 7368  painter.setBrush
-0000a8d0: 2870 672e 6d6b 4272 7573 6828 6261 636b  (pg.mkBrush(back
-0000a8e0: 6772 6f75 6e64 2929 0d0a 2020 2020 2020  ground))..      
-0000a8f0: 2020 2020 2020 6c2c 7220 3d20 626f 756e        l,r = boun
-0000a900: 6469 6e67 5265 6374 2e6c 6566 7428 292c  dingRect.left(),
-0000a910: 2062 6f75 6e64 696e 6752 6563 742e 7269   boundingRect.ri
-0000a920: 6768 7428 290d 0a20 2020 2020 2020 2020  ght()..         
-0000a930: 2020 2073 656c 662e 7061 696e 7465 722e     self.painter.
-0000a940: 6472 6177 5265 6374 2851 7443 6f72 652e  drawRect(QtCore.
-0000a950: 5152 6563 7446 286c 2c20 626f 756e 6469  QRectF(l, boundi
-0000a960: 6e67 5265 6374 2e74 6f70 2829 2c20 3165  ngRect.top(), 1e
-0000a970: 2d33 2c20 626f 756e 6469 6e67 5265 6374  -3, boundingRect
-0000a980: 2e68 6569 6768 7428 292a 3165 2d35 2929  .height()*1e-5))
-0000a990: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000a9a0: 6c66 2e70 6169 6e74 6572 2e64 7261 7752  lf.painter.drawR
-0000a9b0: 6563 7428 5174 436f 7265 2e51 5265 6374  ect(QtCore.QRect
-0000a9c0: 4628 722c 2062 6f75 6e64 696e 6752 6563  F(r, boundingRec
-0000a9d0: 742e 626f 7474 6f6d 2829 2c20 2d31 652d  t.bottom(), -1e-
-0000a9e0: 332c 202d 626f 756e 6469 6e67 5265 6374  3, -boundingRect
-0000a9f0: 2e68 6569 6768 7428 292a 3165 2d35 2929  .height()*1e-5))
-0000aa00: 0d0a 0d0a 2020 2020 6465 6620 626f 756e  ....    def boun
-0000aa10: 6469 6e67 5265 6374 2873 656c 6629 3a0d  dingRect(self):.
-0000aa20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000aa30: 5174 436f 7265 2e51 5265 6374 4628 7365  QtCore.QRectF(se
-0000aa40: 6c66 2e70 6963 7475 7265 2e62 6f75 6e64  lf.picture.bound
-0000aa50: 696e 6752 6563 7428 2929 0d0a 0d0a 0d0a  ingRect())......
-0000aa60: 0d0a 636c 6173 7320 4361 6e64 6c65 7374  ..class Candlest
-0000aa70: 6963 6b49 7465 6d28 4669 6e50 6c6f 7449  ickItem(FinPlotI
-0000aa80: 7465 6d29 3a0d 0a20 2020 2064 6566 205f  tem):..    def _
-0000aa90: 5f69 6e69 745f 5f28 7365 6c66 2c20 6178  _init__(self, ax
-0000aaa0: 2c20 6461 7461 7372 632c 2064 7261 775f  , datasrc, draw_
-0000aab0: 626f 6479 2c20 6472 6177 5f73 6861 646f  body, draw_shado
-0000aac0: 772c 2063 616e 646c 655f 7769 6474 682c  w, candle_width,
-0000aad0: 2063 6f6c 6f72 6675 6e63 293a 0d0a 2020   colorfunc):..  
-0000aae0: 2020 2020 2020 7365 6c66 2e63 6f6c 6f72        self.color
-0000aaf0: 7320 3d20 6469 6374 2862 756c 6c5f 7368  s = dict(bull_sh
-0000ab00: 6164 6f77 2020 2020 2020 3d20 6361 6e64  adow      = cand
-0000ab10: 6c65 5f62 756c 6c5f 636f 6c6f 722c 0d0a  le_bull_color,..
+000018a0: 6966 206c 656e 2874 6578 745f 7370 6563  if len(text_spec
+000018b0: 7329 203e 3d20 343a 0d0a 2020 2020 2020  s) >= 4:..      
+000018c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000018d0: 6374 2c66 6c61 6773 2c74 6578 7420 3d20  ct,flags,text = 
+000018e0: 7465 7874 5f73 7065 6373 5b30 5d0d 0a20  text_specs[0].. 
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001900: 2020 2069 6620 7265 6374 2e6c 6566 7428     if rect.left(
+00001910: 2920 3c20 303a 0d0a 2020 2020 2020 2020  ) < 0:..        
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 6465 6c20 7465 7874 5f73 7065 6373 5b30  del text_specs[0
+00001940: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00001950: 2020 2020 2020 2072 6563 742c 666c 6167         rect,flag
+00001960: 732c 7465 7874 203d 2074 6578 745f 7370  s,text = text_sp
+00001970: 6563 735b 2d31 5d0d 0a20 2020 2020 2020  ecs[-1]..       
+00001980: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001990: 7265 6374 2e72 6967 6874 2829 203e 2073  rect.right() > s
+000019a0: 656c 662e 6765 6f6d 6574 7279 2829 2e77  elf.geometry().w
+000019b0: 6964 7468 2829 3a0d 0a20 2020 2020 2020  idth():..       
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2064 656c 2074 6578 745f 7370 6563 735b   del text_specs[
+000019e0: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
+000019f0: 2020 2020 2023 202e 2e2e 2061 6e64 2074       # ... and t
+00001a00: 686f 7365 2074 6861 7420 6f76 6572 6c61  hose that overla
+00001a10: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
+00001a20: 2020 2078 203d 2031 6536 0d0a 2020 2020     x = 1e6..    
+00001a30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001a40: 692c 2872 6563 742c 666c 6167 732c 7465  i,(rect,flags,te
+00001a50: 7874 2920 696e 2072 6576 6572 7365 6428  xt) in reversed(
+00001a60: 6c69 7374 2865 6e75 6d65 7261 7465 2874  list(enumerate(t
+00001a70: 6578 745f 7370 6563 7329 2929 3a0d 0a20  ext_specs))):.. 
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2020 2069 6620 7265 6374 2e72 6967 6874     if rect.right
+00001aa0: 2829 203e 3d20 783a 0d0a 2020 2020 2020  () >= x:..      
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ac0: 2020 6465 6c20 7465 7874 5f73 7065 6373    del text_specs
+00001ad0: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
+00001ae0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b00: 2020 2020 2020 2020 7820 3d20 7265 6374          x = rect
+00001b10: 2e6c 6566 7428 290d 0a20 2020 2020 2020  .left()..       
+00001b20: 2072 6574 7572 6e20 7370 6563 730d 0a0d   return specs...
+00001b30: 0a0d 0a0d 0a63 6c61 7373 2059 4178 6973  .....class YAxis
+00001b40: 4974 656d 2870 672e 4178 6973 4974 656d  Item(pg.AxisItem
+00001b50: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
+00001b60: 6974 5f5f 2873 656c 662c 2076 622c 202a  it__(self, vb, *
+00001b70: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
+00001b80: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+00001b90: 292e 5f5f 696e 6974 5f5f 282a 6172 6773  ).__init__(*args
+00001ba0: 2c20 2a2a 6b77 6172 6773 290d 0a20 2020  , **kwargs)..   
+00001bb0: 2020 2020 2073 656c 662e 7662 203d 2076       self.vb = v
+00001bc0: 620d 0a20 2020 2020 2020 2073 656c 662e  b..        self.
+00001bd0: 6869 6465 5f73 7472 696e 6773 203d 2046  hide_strings = F
+00001be0: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
+00001bf0: 6c66 2e73 7479 6c65 5b27 6175 746f 4578  lf.style['autoEx
+00001c00: 7061 6e64 5465 7874 5370 6163 6527 5d20  pandTextSpace'] 
+00001c10: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
+00001c20: 2073 656c 662e 7374 796c 655b 2761 7574   self.style['aut
+00001c30: 6f52 6564 7563 6554 6578 7453 7061 6365  oReduceTextSpace
+00001c40: 275d 203d 2046 616c 7365 0d0a 2020 2020  '] = False..    
+00001c50: 2020 2020 7365 6c66 2e6e 6578 745f 666d      self.next_fm
+00001c60: 7420 3d20 2725 6727 0d0a 0d0a 2020 2020  t = '%g'....    
+00001c70: 6465 6620 7469 636b 5661 6c75 6573 2873  def tickValues(s
+00001c80: 656c 662c 206d 696e 5661 6c2c 206d 6178  elf, minVal, max
+00001c90: 5661 6c2c 2073 697a 6529 3a0d 0a20 2020  Val, size):..   
+00001ca0: 2020 2020 2076 7320 3d20 7375 7065 7228       vs = super(
+00001cb0: 292e 7469 636b 5661 6c75 6573 286d 696e  ).tickValues(min
+00001cc0: 5661 6c2c 206d 6178 5661 6c2c 2073 697a  Val, maxVal, siz
+00001cd0: 6529 0d0a 2020 2020 2020 2020 6966 206c  e)..        if l
+00001ce0: 656e 2876 7329 203c 2033 3a0d 0a20 2020  en(vs) < 3:..   
+00001cf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001d00: 7673 0d0a 2020 2020 2020 2020 7265 7475  vs..        retu
+00001d10: 726e 2073 656c 662e 666d 745f 7661 6c75  rn self.fmt_valu
+00001d20: 6573 2876 7329 0d0a 0d0a 2020 2020 6465  es(vs)....    de
+00001d30: 6620 6c6f 6754 6963 6b56 616c 7565 7328  f logTickValues(
+00001d40: 7365 6c66 2c20 6d69 6e56 616c 2c20 6d61  self, minVal, ma
+00001d50: 7856 616c 2c20 7369 7a65 2c20 7374 6454  xVal, size, stdT
+00001d60: 6963 6b73 293a 0d0a 2020 2020 2020 2020  icks):..        
+00001d70: 7631 203d 2069 6e74 2866 6c6f 6f72 286d  v1 = int(floor(m
+00001d80: 696e 5661 6c29 290d 0a20 2020 2020 2020  inVal))..       
+00001d90: 2076 3220 3d20 696e 7428 6365 696c 286d   v2 = int(ceil(m
+00001da0: 6178 5661 6c29 290d 0a20 2020 2020 2020  axVal))..       
+00001db0: 206d 696e 6f72 203d 205b 5d0d 0a20 2020   minor = []..   
+00001dc0: 2020 2020 2066 6f72 2076 2069 6e20 7261       for v in ra
+00001dd0: 6e67 6528 7631 2c20 7632 293a 0d0a 2020  nge(v1, v2):..  
+00001de0: 2020 2020 2020 2020 2020 6d69 6e6f 722e            minor.
+00001df0: 6578 7465 6e64 285b 762b 6c20 666f 7220  extend([v+l for 
+00001e00: 6c20 696e 206e 702e 6c6f 6731 3028 6e70  l in np.log10(np
+00001e10: 2e6c 696e 7370 6163 6528 312c 2039 2e39  .linspace(1, 9.9
+00001e20: 2c20 3930 2929 5d29 0d0a 2020 2020 2020  , 90))])..      
+00001e30: 2020 6d69 6e6f 7220 3d20 5b78 2066 6f72    minor = [x for
+00001e40: 2078 2069 6e20 6d69 6e6f 7220 6966 2078   x in minor if x
+00001e50: 3e6d 696e 5661 6c20 616e 6420 783c 6d61  >minVal and x<ma
+00001e60: 7856 616c 5d0d 0a20 2020 2020 2020 2069  xVal]..        i
+00001e70: 6620 6e6f 7420 6d69 6e6f 723a 0d0a 2020  f not minor:..  
+00001e80: 2020 2020 2020 2020 2020 6d69 6e6f 722e            minor.
+00001e90: 6578 7465 6e64 286e 702e 6765 6f6d 7370  extend(np.geomsp
+00001ea0: 6163 6528 6d69 6e56 616c 2c20 6d61 7856  ace(minVal, maxV
+00001eb0: 616c 2c20 3729 5b31 3a2d 315d 290d 0a20  al, 7)[1:-1]).. 
+00001ec0: 2020 2020 2020 2069 6620 6c65 6e28 6d69         if len(mi
+00001ed0: 6e6f 7229 203e 2031 303a 0d0a 2020 2020  nor) > 10:..    
+00001ee0: 2020 2020 2020 2020 6d69 6e6f 7220 3d20          minor = 
+00001ef0: 6d69 6e6f 725b 3a3a 6c65 6e28 6d69 6e6f  minor[::len(mino
+00001f00: 7229 2f2f 355d 0d0a 2020 2020 2020 2020  r)//5]..        
+00001f10: 7673 203d 205b 284e 6f6e 652c 206d 696e  vs = [(None, min
+00001f20: 6f72 295d 0d0a 2020 2020 2020 2020 7265  or)]..        re
+00001f30: 7475 726e 2073 656c 662e 666d 745f 7661  turn self.fmt_va
+00001f40: 6c75 6573 2876 7329 0d0a 0d0a 2020 2020  lues(vs)....    
+00001f50: 6465 6620 7469 636b 5374 7269 6e67 7328  def tickStrings(
+00001f60: 7365 6c66 2c20 7661 6c75 6573 2c20 7363  self, values, sc
+00001f70: 616c 652c 2073 7061 6369 6e67 293a 0d0a  ale, spacing):..
+00001f80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00001f90: 6869 6465 5f73 7472 696e 6773 3a0d 0a20  hide_strings:.. 
+00001fa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001fb0: 6e20 5b5d 0d0a 2020 2020 2020 2020 7866  n []..        xf
+00001fc0: 6f72 6d20 3d20 7365 6c66 2e76 622e 7973  orm = self.vb.ys
+00001fd0: 6361 6c65 2e78 666f 726d 0d0a 2020 2020  cale.xform..    
+00001fe0: 2020 2020 7265 7475 726e 205b 7365 6c66      return [self
+00001ff0: 2e6e 6578 745f 666d 7425 7866 6f72 6d28  .next_fmt%xform(
+00002000: 7661 6c75 6529 2066 6f72 2076 616c 7565  value) for value
+00002010: 2069 6e20 7661 6c75 6573 5d0d 0a0d 0a20   in values].... 
+00002020: 2020 2064 6566 2066 6d74 5f76 616c 7565     def fmt_value
+00002030: 7328 7365 6c66 2c20 7673 293a 0d0a 2020  s(self, vs):..  
+00002040: 2020 2020 2020 7866 6f72 6d20 3d20 7365        xform = se
+00002050: 6c66 2e76 622e 7973 6361 6c65 2e78 666f  lf.vb.yscale.xfo
+00002060: 726d 0d0a 2020 2020 2020 2020 6773 203d  rm..        gs =
+00002070: 205b 2725 6727 2578 666f 726d 2876 2920   ['%g'%xform(v) 
+00002080: 666f 7220 7620 696e 2076 735b 2d31 5d5b  for v in vs[-1][
+00002090: 315d 5d0d 0a20 2020 2020 2020 2069 6620  1]]..        if 
+000020a0: 6e6f 7420 6773 3a0d 0a20 2020 2020 2020  not gs:..       
+000020b0: 2020 2020 2072 6574 7572 6e20 7673 0d0a       return vs..
+000020c0: 2020 2020 2020 2020 6966 2061 6e79 285b          if any([
+000020d0: 2765 2720 696e 2067 2066 6f72 2067 2069  'e' in g for g i
+000020e0: 6e20 6773 5d29 3a0d 0a20 2020 2020 2020  n gs]):..       
+000020f0: 2020 2020 206d 6178 6465 6320 3d20 6d61       maxdec = ma
+00002100: 7828 5b6c 656e 2828 6729 2e70 6172 7469  x([len((g).parti
+00002110: 7469 6f6e 2827 2e27 295b 325d 2e70 6172  tion('.')[2].par
+00002120: 7469 7469 6f6e 2827 6527 295b 305d 2920  tition('e')[0]) 
+00002130: 666f 7220 6720 696e 2067 7320 6966 2027  for g in gs if '
+00002140: 6527 2069 6e20 675d 290d 0a20 2020 2020  e' in g])..     
+00002150: 2020 2020 2020 2073 656c 662e 6e65 7874         self.next
+00002160: 5f66 6d74 203d 2027 2525 2e25 6965 2720  _fmt = '%%.%ie' 
+00002170: 2520 6d61 7864 6563 0d0a 2020 2020 2020  % maxdec..      
+00002180: 2020 656c 6966 2067 733a 0d0a 2020 2020    elif gs:..    
+00002190: 2020 2020 2020 2020 6d61 7864 6563 203d          maxdec =
+000021a0: 206d 6178 285b 6c65 6e28 2867 292e 7061   max([len((g).pa
+000021b0: 7274 6974 696f 6e28 272e 2729 5b32 5d29  rtition('.')[2])
+000021c0: 2066 6f72 2067 2069 6e20 6773 5d29 0d0a   for g in gs])..
+000021d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000021e0: 2e6e 6578 745f 666d 7420 3d20 2725 252e  .next_fmt = '%%.
+000021f0: 2569 6627 2025 206d 6178 6465 630d 0a20  %if' % maxdec.. 
+00002200: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00002210: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00002220: 6578 745f 666d 7420 3d20 2725 6727 0d0a  ext_fmt = '%g'..
+00002230: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00002240: 730d 0a0d 0a0d 0a0d 0a63 6c61 7373 2059  s........class Y
+00002250: 5363 616c 653a 0d0a 2020 2020 6465 6620  Scale:..    def 
+00002260: 5f5f 696e 6974 5f5f 2873 656c 662c 2073  __init__(self, s
+00002270: 6361 6c65 7479 7065 2c20 7363 616c 6566  caletype, scalef
+00002280: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00002290: 2e73 6361 6c65 7479 7065 203d 2073 6361  .scaletype = sca
+000022a0: 6c65 7479 7065 0d0a 2020 2020 2020 2020  letype..        
+000022b0: 7365 6c66 2e73 6574 5f73 6361 6c65 2873  self.set_scale(s
+000022c0: 6361 6c65 6629 0d0a 0d0a 2020 2020 6465  calef)....    de
+000022d0: 6620 7365 745f 7363 616c 6528 7365 6c66  f set_scale(self
+000022e0: 2c20 7363 616c 6529 3a0d 0a20 2020 2020  , scale):..     
+000022f0: 2020 2073 656c 662e 7363 616c 6566 203d     self.scalef =
+00002300: 2073 6361 6c65 0d0a 0d0a 2020 2020 6465   scale....    de
+00002310: 6620 7866 6f72 6d28 7365 6c66 2c20 7929  f xform(self, y)
+00002320: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
+00002330: 6c66 2e73 6361 6c65 7479 7065 203d 3d20  lf.scaletype == 
+00002340: 276c 6f67 273a 0d0a 2020 2020 2020 2020  'log':..        
+00002350: 2020 2020 7920 3d20 3130 2a2a 790d 0a20      y = 10**y.. 
+00002360: 2020 2020 2020 2079 203d 2079 202a 2073         y = y * s
+00002370: 656c 662e 7363 616c 6566 0d0a 2020 2020  elf.scalef..    
+00002380: 2020 2020 7265 7475 726e 2079 0d0a 0d0a      return y....
+00002390: 2020 2020 6465 6620 696e 7678 666f 726d      def invxform
+000023a0: 2873 656c 662c 2079 2c20 7665 7269 6679  (self, y, verify
+000023b0: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
+000023c0: 2020 7920 2f3d 2073 656c 662e 7363 616c    y /= self.scal
+000023d0: 6566 0d0a 2020 2020 2020 2020 6966 2073  ef..        if s
+000023e0: 656c 662e 7363 616c 6574 7970 6520 3d3d  elf.scaletype ==
+000023f0: 2027 6c6f 6727 3a0d 0a20 2020 2020 2020   'log':..       
+00002400: 2020 2020 2069 6620 7665 7269 6679 2061       if verify a
+00002410: 6e64 2079 203c 3d20 303a 0d0a 2020 2020  nd y <= 0:..    
+00002420: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002430: 726e 202d 3165 3620 2f20 7365 6c66 2e73  rn -1e6 / self.s
+00002440: 6361 6c65 660d 0a20 2020 2020 2020 2020  calef..         
+00002450: 2020 2079 203d 206e 702e 6c6f 6731 3028     y = np.log10(
+00002460: 7929 0d0a 2020 2020 2020 2020 7265 7475  y)..        retu
+00002470: 726e 2079 0d0a 0d0a 0d0a 0d0a 636c 6173  rn y........clas
+00002480: 7320 5061 6e64 6173 4461 7461 536f 7572  s PandasDataSour
+00002490: 6365 3a0d 0a20 2020 2027 2727 4361 6e64  ce:..    '''Cand
+000024a0: 6c65 2073 7469 636b 733a 2063 7265 6174  le sticks: creat
+000024b0: 6520 7769 7468 2066 6976 6520 636f 6c75  e with five colu
+000024c0: 6d6e 733a 2074 696d 652c 206f 7065 6e2c  mns: time, open,
+000024d0: 2063 6c6f 7365 2c20 6869 2c20 6c6f 202d   close, hi, lo -
+000024e0: 2069 6e20 7468 6174 206f 7264 6572 2e0d   in that order..
+000024f0: 0a20 2020 2020 2020 566f 6c75 6d65 2062  .       Volume b
+00002500: 6172 733a 2063 7265 6174 6520 7769 7468  ars: create with
+00002510: 2074 6872 6565 2063 6f6c 756d 6e73 3a20   three columns: 
+00002520: 7469 6d65 2c20 6f70 656e 2c20 636c 6f73  time, open, clos
+00002530: 652c 2076 6f6c 756d 6520 2d20 696e 2074  e, volume - in t
+00002540: 6861 7420 6f72 6465 722e 0d0a 2020 2020  hat order...    
+00002550: 2020 2046 6f72 2061 6c6c 206f 7468 6572     For all other
+00002560: 2074 7970 6573 2c20 7469 6d65 206e 6565   types, time nee
+00002570: 6473 2074 6f20 6265 2066 6972 7374 2c20  ds to be first, 
+00002580: 7573 7561 6c6c 7920 666f 6c6c 6f77 6564  usually followed
+00002590: 2062 7920 6f6e 6520 6f72 206d 6f72 6520   by one or more 
+000025a0: 592d 636f 6c75 6d6e 732e 2727 270d 0a20  Y-columns.'''.. 
+000025b0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000025c0: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
+000025d0: 2020 2020 6966 2074 7970 6528 6466 2e69      if type(df.i
+000025e0: 6e64 6578 2920 3d3d 2070 642e 4461 7465  ndex) == pd.Date
+000025f0: 7469 6d65 496e 6465 7820 6f72 2064 662e  timeIndex or df.
+00002600: 696e 6465 785b 2d31 5d3e 3165 3820 6f72  index[-1]>1e8 or
+00002610: 2027 2e52 616e 6765 496e 6465 7827 206e   '.RangeIndex' n
+00002620: 6f74 2069 6e20 7374 7228 7479 7065 2864  ot in str(type(d
+00002630: 662e 696e 6465 7829 293a 0d0a 2020 2020  f.index)):..    
+00002640: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+00002650: 7265 7365 745f 696e 6465 7828 290d 0a20  reset_index().. 
+00002660: 2020 2020 2020 2073 656c 662e 6466 203d         self.df =
+00002670: 2064 662e 636f 7079 2829 0d0a 2020 2020   df.copy()..    
+00002680: 2020 2020 2320 6d61 6e61 6765 2074 696d      # manage tim
+00002690: 6520 636f 6c75 6d6e 0d0a 2020 2020 2020  e column..      
+000026a0: 2020 6966 205f 6861 735f 7469 6d65 636f    if _has_timeco
+000026b0: 6c28 7365 6c66 2e64 6629 3a0d 0a20 2020  l(self.df):..   
+000026c0: 2020 2020 2020 2020 2074 696d 6563 6f6c           timecol
+000026d0: 203d 2073 656c 662e 6466 2e63 6f6c 756d   = self.df.colum
+000026e0: 6e73 5b30 5d0d 0a20 2020 2020 2020 2020  ns[0]..         
+000026f0: 2020 2064 7479 7065 203d 2073 7472 2864     dtype = str(d
+00002700: 665b 7469 6d65 636f 6c5d 2e64 7479 7065  f[timecol].dtype
+00002710: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00002720: 736e 756d 203d 2028 2769 6e74 2720 696e  snum = ('int' in
+00002730: 2064 7479 7065 206f 7220 2766 6c6f 6174   dtype or 'float
+00002740: 2720 696e 2064 7479 7065 2920 616e 6420  ' in dtype) and 
+00002750: 6466 5b74 696d 6563 6f6c 5d2e 696c 6f63  df[timecol].iloc
+00002760: 5b2d 315d 203c 2031 6537 0d0a 2020 2020  [-1] < 1e7..    
+00002770: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00002780: 736e 756d 3a0d 0a20 2020 2020 2020 2020  snum:..         
+00002790: 2020 2020 2020 2073 656c 662e 6466 5b74         self.df[t
+000027a0: 696d 6563 6f6c 5d20 3d20 5f70 6474 696d  imecol] = _pdtim
+000027b0: 6532 6570 6f63 6828 6466 5b74 696d 6563  e2epoch(df[timec
+000027c0: 6f6c 5d29 0d0a 2020 2020 2020 2020 2020  ol])..          
+000027d0: 2020 7365 6c66 2e73 7461 6e64 616c 6f6e    self.standalon
+000027e0: 6520 3d20 5f69 735f 7374 616e 6461 6c6f  e = _is_standalo
+000027f0: 6e65 2873 656c 662e 6466 5b74 696d 6563  ne(self.df[timec
+00002800: 6f6c 5d29 0d0a 2020 2020 2020 2020 2020  ol])..          
+00002810: 2020 7365 6c66 2e63 6f6c 5f64 6174 615f    self.col_data_
+00002820: 6f66 6673 6574 203d 2031 2023 206e 6f2e  offset = 1 # no.
+00002830: 206f 6620 7072 6563 6565 6469 6e67 2063   of preceeding c
+00002840: 6f6c 756d 6e73 2066 6f72 206f 7468 6572  olumns for other
+00002850: 2070 6c6f 7473 2061 6e64 2074 696d 6520   plots and time 
+00002860: 636f 6c75 6d6e 0d0a 2020 2020 2020 2020  column..        
+00002870: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00002880: 2020 2073 656c 662e 7374 616e 6461 6c6f     self.standalo
+00002890: 6e65 203d 2046 616c 7365 0d0a 2020 2020  ne = False..    
+000028a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6c          self.col
+000028b0: 5f64 6174 615f 6f66 6673 6574 203d 2030  _data_offset = 0
+000028c0: 2023 206e 6f2e 206f 6620 7072 6563 6565   # no. of precee
+000028d0: 6469 6e67 2063 6f6c 756d 6e73 2066 6f72  ding columns for
+000028e0: 206f 7468 6572 2070 6c6f 7473 2061 6e64   other plots and
+000028f0: 2074 696d 6520 636f 6c75 6d6e 0d0a 2020   time column..  
+00002900: 2020 2020 2020 2320 7365 7475 7020 6461        # setup da
+00002910: 7461 2066 6f72 206a 6f69 6e69 6e67 2064  ta for joining d
+00002920: 6174 6120 736f 7572 6365 7320 616e 6420  ata sources and 
+00002930: 7a6f 6f6d 696e 670d 0a20 2020 2020 2020  zooming..       
+00002940: 2073 656c 662e 7363 616c 655f 636f 6c73   self.scale_cols
+00002950: 203d 205b 6920 666f 7220 6920 696e 2072   = [i for i in r
+00002960: 616e 6765 2873 656c 662e 636f 6c5f 6461  ange(self.col_da
+00002970: 7461 5f6f 6666 7365 742c 6c65 6e28 7365  ta_offset,len(se
+00002980: 6c66 2e64 662e 636f 6c75 6d6e 7329 2920  lf.df.columns)) 
+00002990: 6966 2073 656c 662e 6466 2e69 6c6f 635b  if self.df.iloc[
+000029a0: 3a2c 695d 2e64 7479 7065 213d 6f62 6a65  :,i].dtype!=obje
+000029b0: 6374 5d0d 0a20 2020 2020 2020 2073 656c  ct]..        sel
+000029c0: 662e 6361 6368 655f 6869 6c6f 203d 204f  f.cache_hilo = O
+000029d0: 7264 6572 6564 4469 6374 2829 0d0a 2020  rderedDict()..  
+000029e0: 2020 2020 2020 7365 6c66 2e72 656e 616d        self.renam
+000029f0: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
+00002a00: 206e 6577 636f 6c73 203d 205b 5d0d 0a20   newcols = [].. 
+00002a10: 2020 2020 2020 2066 6f72 2063 6f6c 2069         for col i
+00002a20: 6e20 7365 6c66 2e64 662e 636f 6c75 6d6e  n self.df.column
+00002a30: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00002a40: 6f6c 6463 6f6c 203d 2063 6f6c 0d0a 2020  oldcol = col..  
+00002a50: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+00002a60: 636f 6c20 696e 206e 6577 636f 6c73 3a0d  col in newcols:.
+00002a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a80: 2063 6f6c 203d 2073 7472 2863 6f6c 292b   col = str(col)+
+00002a90: 272b 270d 0a20 2020 2020 2020 2020 2020  '+'..           
+00002aa0: 206e 6577 636f 6c73 2e61 7070 656e 6428   newcols.append(
+00002ab0: 636f 6c29 0d0a 2020 2020 2020 2020 2020  col)..          
+00002ac0: 2020 6966 206f 6c64 636f 6c20 213d 2063    if oldcol != c
+00002ad0: 6f6c 3a0d 0a20 2020 2020 2020 2020 2020  ol:..           
+00002ae0: 2020 2020 2073 656c 662e 7265 6e61 6d65       self.rename
+00002af0: 735b 6f6c 6463 6f6c 5d20 3d20 636f 6c0d  s[oldcol] = col.
+00002b00: 0a20 2020 2020 2020 2073 656c 662e 6466  .        self.df
+00002b10: 2e63 6f6c 756d 6e73 203d 206e 6577 636f  .columns = newco
+00002b20: 6c73 0d0a 2020 2020 2020 2020 7365 6c66  ls..        self
+00002b30: 2e70 7265 5f75 7064 6174 6520 3d20 6c61  .pre_update = la
+00002b40: 6d62 6461 2064 663a 2064 660d 0a20 2020  mbda df: df..   
+00002b50: 2020 2020 2073 656c 662e 706f 7374 5f75       self.post_u
+00002b60: 7064 6174 6520 3d20 6c61 6d62 6461 2064  pdate = lambda d
+00002b70: 663a 2064 660d 0a20 2020 2020 2020 2073  f: df..        s
+00002b80: 656c 662e 5f70 6572 696f 6420 3d20 4e6f  elf._period = No
+00002b90: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
+00002ba0: 2e5f 736d 6f6f 7468 5f74 696d 6520 3d20  ._smooth_time = 
+00002bb0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+00002bc0: 6c66 2e69 735f 7370 6172 7365 203d 2073  lf.is_sparse = s
+00002bd0: 656c 662e 6466 5b73 656c 662e 6466 2e63  elf.df[self.df.c
+00002be0: 6f6c 756d 6e73 5b73 656c 662e 636f 6c5f  olumns[self.col_
+00002bf0: 6461 7461 5f6f 6666 7365 745d 5d2e 6973  data_offset]].is
+00002c00: 6e75 6c6c 2829 2e73 756d 2829 2e6d 6178  null().sum().max
+00002c10: 2829 203e 206c 656e 2873 656c 662e 6466  () > len(self.df
+00002c20: 292f 2f32 0d0a 0d0a 2020 2020 4070 726f  )//2....    @pro
+00002c30: 7065 7274 790d 0a20 2020 2064 6566 2070  perty..    def p
+00002c40: 6572 696f 645f 6e73 2873 656c 6629 3a0d  eriod_ns(self):.
+00002c50: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00002c60: 7365 6c66 2e64 6629 203c 3d20 313a 0d0a  self.df) <= 1:..
+00002c70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002c80: 726e 2031 0d0a 2020 2020 2020 2020 6966  rn 1..        if
+00002c90: 206e 6f74 2073 656c 662e 5f70 6572 696f   not self._perio
+00002ca0: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00002cb0: 7469 6d65 636f 6c20 3d20 7365 6c66 2e64  timecol = self.d
+00002cc0: 662e 636f 6c75 6d6e 735b 305d 0d0a 2020  f.columns[0]..  
+00002cd0: 2020 2020 2020 2020 2020 7469 6d65 7320            times 
+00002ce0: 3d20 7365 6c66 2e64 665b 7469 6d65 636f  = self.df[timeco
+00002cf0: 6c5d 2e69 6c6f 635b 303a 3130 305d 0d0a  l].iloc[0:100]..
+00002d00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002d10: 2e5f 7065 7269 6f64 203d 2069 6e74 2874  ._period = int(t
+00002d20: 696d 6573 2e64 6966 6628 292e 6d65 6469  imes.diff().medi
+00002d30: 616e 2829 2920 6966 206c 656e 2874 696d  an()) if len(tim
+00002d40: 6573 293e 3120 656c 7365 2031 0d0a 2020  es)>1 else 1..  
+00002d50: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002d60: 662e 5f70 6572 696f 640d 0a0d 0a20 2020  f._period....   
+00002d70: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00002d80: 6465 6620 696e 6465 7828 7365 6c66 293a  def index(self):
+00002d90: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002da0: 2073 656c 662e 6466 2e69 6e64 6578 0d0a   self.df.index..
+00002db0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00002dc0: 0a20 2020 2064 6566 2078 2873 656c 6629  .    def x(self)
+00002dd0: 3a0d 0a20 2020 2020 2020 2074 696d 6563  :..        timec
+00002de0: 6f6c 203d 2073 656c 662e 6466 2e63 6f6c  ol = self.df.col
+00002df0: 756d 6e73 5b30 5d0d 0a20 2020 2020 2020  umns[0]..       
+00002e00: 2072 6574 7572 6e20 7365 6c66 2e64 665b   return self.df[
+00002e10: 7469 6d65 636f 6c5d 0d0a 0d0a 2020 2020  timecol]....    
+00002e20: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00002e30: 6566 2079 2873 656c 6629 3a0d 0a20 2020  ef y(self):..   
+00002e40: 2020 2020 2063 6f6c 203d 2073 656c 662e       col = self.
+00002e50: 6466 2e63 6f6c 756d 6e73 5b73 656c 662e  df.columns[self.
+00002e60: 636f 6c5f 6461 7461 5f6f 6666 7365 745d  col_data_offset]
+00002e70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002e80: 2073 656c 662e 6466 5b63 6f6c 5d0d 0a0d   self.df[col]...
+00002e90: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00002ea0: 2020 2020 6465 6620 7a28 7365 6c66 293a      def z(self):
+00002eb0: 0d0a 2020 2020 2020 2020 636f 6c20 3d20  ..        col = 
+00002ec0: 7365 6c66 2e64 662e 636f 6c75 6d6e 735b  self.df.columns[
+00002ed0: 7365 6c66 2e63 6f6c 5f64 6174 615f 6f66  self.col_data_of
+00002ee0: 6673 6574 2b31 5d0d 0a20 2020 2020 2020  fset+1]..       
+00002ef0: 2072 6574 7572 6e20 7365 6c66 2e64 665b   return self.df[
+00002f00: 636f 6c5d 0d0a 0d0a 2020 2020 4070 726f  col]....    @pro
+00002f10: 7065 7274 790d 0a20 2020 2064 6566 2078  perty..    def x
+00002f20: 6c65 6e28 7365 6c66 293a 0d0a 2020 2020  len(self):..    
+00002f30: 2020 2020 7265 7475 726e 206c 656e 2873      return len(s
+00002f40: 656c 662e 6466 290d 0a0d 0a20 2020 2064  elf.df)....    d
+00002f50: 6566 2063 616c 635f 7369 676e 6966 6963  ef calc_signific
+00002f60: 616e 745f 6465 6369 6d61 6c73 2873 656c  ant_decimals(sel
+00002f70: 662c 2066 756c 6c29 3a0d 0a20 2020 2020  f, full):..     
+00002f80: 2020 2064 6566 2066 6c6f 6174 5f72 6f75     def float_rou
+00002f90: 6e64 2866 293a 0d0a 2020 2020 2020 2020  nd(f):..        
+00002fa0: 2020 2020 7265 7475 726e 2066 6c6f 6174      return float
+00002fb0: 2827 252e 3365 2725 6629 2023 2030 2e30  ('%.3e'%f) # 0.0
+00002fc0: 3039 3939 3734 3820 2d3e 2030 2e30 310d  0999748 -> 0.01.
+00002fd0: 0a20 2020 2020 2020 2064 6566 2072 656d  .        def rem
+00002fe0: 6169 6e64 6572 5f6f 6b28 612c 2062 293a  ainder_ok(a, b):
+00002ff0: 0d0a 2020 2020 2020 2020 2020 2020 6320  ..            c 
+00003000: 3d20 6120 2520 620d 0a20 2020 2020 2020  = a % b..       
+00003010: 2020 2020 2069 6620 6320 2f20 6220 3e20       if c / b > 
+00003020: 302e 3938 3a20 2320 7265 6d61 696e 6465  0.98: # remainde
+00003030: 7220 616c 6d6f 7374 2073 616d 6520 6173  r almost same as
+00003040: 2064 656e 6f6d 696e 6174 6f72 0d0a 2020   denominator..  
+00003050: 2020 2020 2020 2020 2020 2020 2020 6320                c 
+00003060: 3d20 6162 7328 632d 6229 0d0a 2020 2020  = abs(c-b)..    
+00003070: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00003080: 203c 2062 2a30 2e36 2023 2068 616c 6620   < b*0.6 # half 
+00003090: 6973 2066 696e 650d 0a20 2020 2020 2020  is fine..       
+000030a0: 2064 6566 2063 616c 635f 7364 2873 6572   def calc_sd(ser
+000030b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000030c0: 7365 7220 3d20 7365 722e 696c 6f63 5b3a  ser = ser.iloc[:
+000030d0: 3130 3030 5d0d 0a20 2020 2020 2020 2020  1000]..         
+000030e0: 2020 2061 6273 6469 6666 203d 2073 6572     absdiff = ser
+000030f0: 2e64 6966 6628 292e 6162 7328 290d 0a20  .diff().abs().. 
+00003100: 2020 2020 2020 2020 2020 2061 6273 6469             absdi
+00003110: 6666 5b61 6273 6469 6666 3c31 652d 3330  ff[absdiff<1e-30
+00003120: 5d20 3d20 3165 3330 0d0a 2020 2020 2020  ] = 1e30..      
+00003130: 2020 2020 2020 736d 616c 6c65 7374 5f64        smallest_d
+00003140: 6966 6620 3d20 6162 7364 6966 662e 6d69  iff = absdiff.mi
+00003150: 6e28 290d 0a20 2020 2020 2020 2020 2020  n()..           
+00003160: 2069 6620 736d 616c 6c65 7374 5f64 6966   if smallest_dif
+00003170: 6620 3e20 3165 3239 3a20 2320 6a75 7374  f > 1e29: # just
+00003180: 2030 733f 0d0a 2020 2020 2020 2020 2020   0s?..          
+00003190: 2020 2020 2020 7265 7475 726e 2030 0d0a        return 0..
+000031a0: 2020 2020 2020 2020 2020 2020 736d 616c              smal
+000031b0: 6c65 7374 5f64 6966 6620 3d20 666c 6f61  lest_diff = floa
+000031c0: 745f 726f 756e 6428 736d 616c 6c65 7374  t_round(smallest
+000031d0: 5f64 6966 6629 0d0a 2020 2020 2020 2020  _diff)..        
+000031e0: 2020 2020 6162 7373 6572 203d 2073 6572      absser = ser
+000031f0: 2e69 6c6f 635b 3a31 3030 5d2e 6162 7328  .iloc[:100].abs(
+00003200: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00003210: 6f72 205f 2069 6e20 7261 6e67 6528 3229  or _ in range(2)
+00003220: 3a20 2320 6368 6563 6b20 6966 2077 6520  : # check if we 
+00003230: 6861 7665 2061 2072 656d 6169 6e64 6572  have a remainder
+00003240: 2074 6861 7420 6973 2061 2062 6574 7465   that is a bette
+00003250: 7220 6570 7369 6c6f 6e0d 0a20 2020 2020  r epsilon..     
+00003260: 2020 2020 2020 2020 2020 2072 656d 6169             remai
+00003270: 6e64 6572 203d 205b 666d 6f64 2876 2c73  nder = [fmod(v,s
+00003280: 6d61 6c6c 6573 745f 6469 6666 2920 666f  mallest_diff) fo
+00003290: 7220 7620 696e 2061 6273 7365 725d 0d0a  r v in absser]..
+000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032b0: 7265 6d61 696e 6465 7220 3d20 5b76 2066  remainder = [v f
+000032c0: 6f72 2076 2069 6e20 7265 6d61 696e 6465  or v in remainde
+000032d0: 7220 6966 2076 3e73 6d61 6c6c 6573 745f  r if v>smallest_
+000032e0: 6469 6666 2f32 305d 0d0a 2020 2020 2020  diff/20]..      
+000032f0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00003300: 2072 656d 6169 6e64 6572 3a0d 0a20 2020   remainder:..   
+00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+00003330: 2020 2020 2020 2020 736d 616c 6c65 7374          smallest
+00003340: 5f64 6966 665f 7220 3d20 6d69 6e28 7265  _diff_r = min(re
+00003350: 6d61 696e 6465 7229 0d0a 2020 2020 2020  mainder)..      
+00003360: 2020 2020 2020 2020 2020 6966 2073 6d61            if sma
+00003370: 6c6c 6573 745f 6469 6666 2a30 2e30 3520  llest_diff*0.05 
+00003380: 3c20 736d 616c 6c65 7374 5f64 6966 665f  < smallest_diff_
+00003390: 7220 3c20 736d 616c 6c65 7374 5f64 6966  r < smallest_dif
+000033a0: 6620 2a20 302e 3720 616e 6420 7265 6d61  f * 0.7 and rema
+000033b0: 696e 6465 725f 6f6b 2873 6d61 6c6c 6573  inder_ok(smalles
+000033c0: 745f 6469 6666 2c20 736d 616c 6c65 7374  t_diff, smallest
+000033d0: 5f64 6966 665f 7229 3a0d 0a20 2020 2020  _diff_r):..     
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000033f0: 6d61 6c6c 6573 745f 6469 6666 203d 2073  mallest_diff = s
+00003400: 6d61 6c6c 6573 745f 6469 6666 5f72 0d0a  mallest_diff_r..
+00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003420: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00003430: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00003440: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00003450: 7475 726e 2073 6d61 6c6c 6573 745f 6469  turn smallest_di
+00003460: 6666 0d0a 2020 2020 2020 2020 6465 6620  ff..        def 
+00003470: 6361 6c63 5f64 6563 2873 6572 2c20 736d  calc_dec(ser, sm
+00003480: 616c 6c65 7374 5f64 6966 6629 3a0d 0a20  allest_diff):.. 
+00003490: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+000034a0: 7420 6675 6c6c 3a20 2320 6c69 6e65 2070  t full: # line p
+000034b0: 6c6f 7473 2075 7375 616c 6c79 2068 6176  lots usually hav
+000034c0: 6520 6578 7472 656d 6520 7265 736f 6c75  e extreme resolu
+000034d0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+000034e0: 2020 2020 2020 6162 736d 6178 203d 2073        absmax = s
+000034f0: 6572 2e69 6c6f 635b 3a33 3030 5d2e 6162  er.iloc[:300].ab
+00003500: 7328 292e 6d61 7828 290d 0a20 2020 2020  s().max()..     
+00003510: 2020 2020 2020 2020 2020 2073 203d 2027             s = '
+00003520: 252e 3365 2720 2520 6162 736d 6178 0d0a  %.3e' % absmax..
+00003530: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00003540: 3a20 2320 6361 6e64 6c65 730d 0a20 2020  : # candles..   
+00003550: 2020 2020 2020 2020 2020 2020 2073 203d               s =
+00003560: 2027 252e 3265 2720 2520 736d 616c 6c65   '%.2e' % smalle
+00003570: 7374 5f64 6966 660d 0a20 2020 2020 2020  st_diff..       
+00003580: 2020 2020 2062 6173 652c 5f2c 6578 7020       base,_,exp 
+00003590: 3d20 732e 7061 7274 6974 696f 6e28 2765  = s.partition('e
+000035a0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+000035b0: 6261 7365 203d 2062 6173 652e 7273 7472  base = base.rstr
+000035c0: 6970 2827 3027 290d 0a20 2020 2020 2020  ip('0')..       
+000035d0: 2020 2020 2065 7870 203d 202d 696e 7428       exp = -int(
+000035e0: 6578 7029 0d0a 2020 2020 2020 2020 2020  exp)..          
+000035f0: 2020 6d61 785f 6261 7365 5f64 6563 696d    max_base_decim
+00003600: 616c 7320 3d20 6d69 6e28 352c 202d 6578  als = min(5, -ex
+00003610: 702b 3229 2069 6620 6578 7020 3c20 3020  p+2) if exp < 0 
+00003620: 656c 7365 2033 0d0a 2020 2020 2020 2020  else 3..        
+00003630: 2020 2020 6261 7365 5f64 6563 696d 616c      base_decimal
+00003640: 7320 3d20 6d61 7828 302c 206d 696e 286d  s = max(0, min(m
+00003650: 6178 5f62 6173 655f 6465 6369 6d61 6c73  ax_base_decimals
+00003660: 2c20 6c65 6e28 6261 7365 292d 3229 290d  , len(base)-2)).
+00003670: 0a20 2020 2020 2020 2020 2020 2064 6563  .            dec
+00003680: 696d 616c 7320 3d20 6578 7020 2b20 6261  imals = exp + ba
+00003690: 7365 5f64 6563 696d 616c 730d 0a20 2020  se_decimals..   
+000036a0: 2020 2020 2020 2020 2064 6563 696d 616c           decimal
+000036b0: 7320 3d20 6d61 7828 302c 206d 696e 286d  s = max(0, min(m
+000036c0: 6178 5f64 6563 696d 616c 732c 2064 6563  ax_decimals, dec
+000036d0: 696d 616c 7329 290d 0a20 2020 2020 2020  imals))..       
+000036e0: 2020 2020 2069 6620 6e6f 7420 6675 6c6c       if not full
+000036f0: 3a20 2320 6170 706c 7920 6772 6964 2066  : # apply grid f
+00003700: 6f72 206c 696e 6520 706c 6f74 7320 6f6e  or line plots on
+00003710: 6c79 0d0a 2020 2020 2020 2020 2020 2020  ly..            
+00003720: 2020 2020 736d 616c 6c65 7374 5f64 6966      smallest_dif
+00003730: 6620 3d20 6d61 7828 3130 2a2a 282d 6465  f = max(10**(-de
+00003740: 6369 6d61 6c73 292c 2073 6d61 6c6c 6573  cimals), smalles
+00003750: 745f 6469 6666 290d 0a20 2020 2020 2020  t_diff)..       
+00003760: 2020 2020 2072 6574 7572 6e20 6465 6369       return deci
+00003770: 6d61 6c73 2c20 736d 616c 6c65 7374 5f64  mals, smallest_d
+00003780: 6966 660d 0a20 2020 2020 2020 2023 2066  iff..        # f
+00003790: 6972 7374 2063 616c 6375 6c61 7465 2045  irst calculate E
+000037a0: 5053 2066 6f72 2073 6572 6965 7320 3026  PS for series 0&
+000037b0: 312c 2074 6865 6e20 646f 2064 6563 696d  1, then do decim
+000037c0: 616c 730d 0a20 2020 2020 2020 2073 6473  als..        sds
+000037d0: 203d 205b 6361 6c63 5f73 6428 7365 6c66   = [calc_sd(self
+000037e0: 2e79 295d 2023 206d 6967 6874 2062 6520  .y)] # might be 
+000037f0: 616c 6c20 7a65 726f 7320 666f 7220 6261  all zeros for ba
+00003800: 7220 6368 6172 7473 0d0a 2020 2020 2020  r charts..      
+00003810: 2020 6966 206c 656e 2873 656c 662e 7363    if len(self.sc
+00003820: 616c 655f 636f 6c73 2920 3e20 313a 0d0a  ale_cols) > 1:..
+00003830: 2020 2020 2020 2020 2020 2020 7364 732e              sds.
+00003840: 6170 7065 6e64 2863 616c 635f 7364 2873  append(calc_sd(s
+00003850: 656c 662e 7a29 2920 2320 6966 2066 6972  elf.z)) # if fir
+00003860: 7374 2069 7320 6f70 656e 2c20 7468 6973  st is open, this
+00003870: 206d 6967 6874 2062 6520 636c 6f73 650d   might be close.
+00003880: 0a20 2020 2020 2020 2073 6473 203d 205b  .        sds = [
+00003890: 7364 2066 6f72 2073 6420 696e 2073 6473  sd for sd in sds
+000038a0: 2069 6620 7364 3e30 5d0d 0a20 2020 2020   if sd>0]..     
+000038b0: 2020 2062 6967 5f64 6966 6620 3d20 6d61     big_diff = ma
+000038c0: 7828 7364 7329 0d0a 2020 2020 2020 2020  x(sds)..        
+000038d0: 736d 616c 6c65 7374 5f64 6966 6620 3d20  smallest_diff = 
+000038e0: 6d69 6e28 5b73 6420 666f 7220 7364 2069  min([sd for sd i
+000038f0: 6e20 7364 7320 6966 2073 643e 6269 675f  n sds if sd>big_
+00003900: 6469 6666 2f31 3030 5d29 2023 2066 696c  diff/100]) # fil
+00003910: 7465 7220 6f75 7420 6578 7472 656d 656c  ter out extremel
+00003920: 7920 736d 616c 6c20 6570 7369 6c6f 6e73  y small epsilons
+00003930: 0d0a 2020 2020 2020 2020 7365 7220 3d20  ..        ser = 
+00003940: 7365 6c66 2e7a 2069 6620 6c65 6e28 7365  self.z if len(se
+00003950: 6c66 2e73 6361 6c65 5f63 6f6c 7329 203e  lf.scale_cols) >
+00003960: 2031 2065 6c73 6520 7365 6c66 2e79 0d0a   1 else self.y..
+00003970: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00003980: 616c 635f 6465 6328 7365 722c 2073 6d61  alc_dec(ser, sma
+00003990: 6c6c 6573 745f 6469 6666 290d 0a0d 0a20  llest_diff).... 
+000039a0: 2020 2064 6566 2075 7064 6174 655f 696e     def update_in
+000039b0: 6974 5f78 2873 656c 662c 2069 6e69 745f  it_x(self, init_
+000039c0: 7374 6570 7329 3a0d 0a20 2020 2020 2020  steps):..       
+000039d0: 2073 656c 662e 696e 6974 5f78 302c 2073   self.init_x0, s
+000039e0: 656c 662e 696e 6974 5f78 3120 3d20 5f78  elf.init_x1 = _x
+000039f0: 6d69 6e6d 6178 2873 656c 662c 2078 5f69  minmax(self, x_i
+00003a00: 6e64 6578 6564 3d54 7275 652c 2069 6e69  ndexed=True, ini
+00003a10: 745f 7374 6570 733d 696e 6974 5f73 7465  t_steps=init_ste
+00003a20: 7073 290d 0a0d 0a20 2020 2064 6566 2063  ps)....    def c
+00003a30: 6c6f 7365 7374 5f74 696d 6528 7365 6c66  losest_time(self
+00003a40: 2c20 7829 3a0d 0a20 2020 2020 2020 2074  , x):..        t
+00003a50: 696d 6563 6f6c 203d 2073 656c 662e 6466  imecol = self.df
+00003a60: 2e63 6f6c 756d 6e73 5b30 5d0d 0a20 2020  .columns[0]..   
+00003a70: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00003a80: 2e64 662e 6c6f 635b 696e 7428 7829 2c20  .df.loc[int(x), 
+00003a90: 7469 6d65 636f 6c5d 0d0a 0d0a 2020 2020  timecol]....    
+00003aa0: 6465 6620 7469 6d65 6261 7365 6428 7365  def timebased(se
+00003ab0: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+00003ac0: 7475 726e 2073 656c 662e 6466 2e69 6c6f  turn self.df.ilo
+00003ad0: 635b 2d31 2c30 5d20 3e20 3165 370d 0a0d  c[-1,0] > 1e7...
+00003ae0: 0a20 2020 2064 6566 2069 735f 736d 6f6f  .    def is_smoo
+00003af0: 7468 5f74 696d 6528 7365 6c66 293a 0d0a  th_time(self):..
+00003b00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003b10: 5f73 6d6f 6f74 685f 7469 6d65 2069 7320  _smooth_time is 
+00003b20: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00003b30: 2020 2023 206c 6573 7320 7468 616e 2031     # less than 1
+00003b40: 2520 7469 6d65 2064 656c 7461 2069 7320  % time delta is 
+00003b50: 736d 6f6f 7468 0d0a 2020 2020 2020 2020  smooth..        
+00003b60: 2020 2020 7365 6c66 2e5f 736d 6f6f 7468      self._smooth
+00003b70: 5f74 696d 6520 3d20 7365 6c66 2e74 696d  _time = self.tim
+00003b80: 6562 6173 6564 2829 2061 6e64 2028 6e70  ebased() and (np
+00003b90: 2e61 6273 286e 702e 6469 6666 2873 656c  .abs(np.diff(sel
+00003ba0: 662e 782e 7661 6c75 6573 5b31 3a31 3030  f.x.values[1:100
+00003bb0: 5d29 5b31 3a5d 2f2f 2873 656c 662e 7065  ])[1:]//(self.pe
+00003bc0: 7269 6f64 5f6e 732f 2f31 3030 3029 2d31  riod_ns//1000)-1
+00003bd0: 3030 3029 203c 2031 3029 2e61 6c6c 2829  000) < 10).all()
+00003be0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00003bf0: 2073 656c 662e 5f73 6d6f 6f74 685f 7469   self._smooth_ti
+00003c00: 6d65 0d0a 0d0a 2020 2020 6465 6620 6164  me....    def ad
+00003c10: 6463 6f6c 7328 7365 6c66 2c20 6461 7461  dcols(self, data
+00003c20: 7372 6329 3a0d 0a20 2020 2020 2020 206e  src):..        n
+00003c30: 6577 5f73 6361 6c65 5f63 6f6c 7320 3d20  ew_scale_cols = 
+00003c40: 5b63 2b6c 656e 2873 656c 662e 6466 2e63  [c+len(self.df.c
+00003c50: 6f6c 756d 6e73 292d 6461 7461 7372 632e  olumns)-datasrc.
+00003c60: 636f 6c5f 6461 7461 5f6f 6666 7365 7420  col_data_offset 
+00003c70: 666f 7220 6320 696e 2064 6174 6173 7263  for c in datasrc
+00003c80: 2e73 6361 6c65 5f63 6f6c 735d 0d0a 2020  .scale_cols]..  
+00003c90: 2020 2020 2020 7365 6c66 2e73 6361 6c65        self.scale
+00003ca0: 5f63 6f6c 7320 2b3d 206e 6577 5f73 6361  _cols += new_sca
+00003cb0: 6c65 5f63 6f6c 730d 0a20 2020 2020 2020  le_cols..       
+00003cc0: 206f 7269 675f 636f 6c5f 6461 7461 5f63   orig_col_data_c
+00003cd0: 6e74 203d 206c 656e 2873 656c 662e 6466  nt = len(self.df
+00003ce0: 2e63 6f6c 756d 6e73 290d 0a20 2020 2020  .columns)..     
+00003cf0: 2020 2069 6620 5f68 6173 5f74 696d 6563     if _has_timec
+00003d00: 6f6c 2864 6174 6173 7263 2e64 6629 3a0d  ol(datasrc.df):.
+00003d10: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00003d20: 6563 6f6c 203d 2073 656c 662e 6466 2e63  ecol = self.df.c
+00003d30: 6f6c 756d 6e73 5b30 5d0d 0a20 2020 2020  olumns[0]..     
+00003d40: 2020 2020 2020 2064 6620 3d20 7365 6c66         df = self
+00003d50: 2e64 662e 7365 745f 696e 6465 7828 7469  .df.set_index(ti
+00003d60: 6d65 636f 6c29 0d0a 2020 2020 2020 2020  mecol)..        
+00003d70: 2020 2020 7469 6d65 636f 6c20 3d20 7469      timecol = ti
+00003d80: 6d65 636f 6c20 6966 2074 696d 6563 6f6c  mecol if timecol
+00003d90: 2069 6e20 6461 7461 7372 632e 6466 2e63   in datasrc.df.c
+00003da0: 6f6c 756d 6e73 2065 6c73 6520 6461 7461  olumns else data
+00003db0: 7372 632e 6466 2e63 6f6c 756d 6e73 5b30  src.df.columns[0
+00003dc0: 5d0d 0a20 2020 2020 2020 2020 2020 206e  ]..            n
+00003dd0: 6577 636f 6c73 203d 2064 6174 6173 7263  ewcols = datasrc
+00003de0: 2e64 662e 7365 745f 696e 6465 7828 7469  .df.set_index(ti
+00003df0: 6d65 636f 6c29 0d0a 2020 2020 2020 2020  mecol)..        
+00003e00: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00003e10: 2020 2064 6620 3d20 7365 6c66 2e64 660d     df = self.df.
+00003e20: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+00003e30: 636f 6c73 203d 2064 6174 6173 7263 2e64  cols = datasrc.d
+00003e40: 660d 0a20 2020 2020 2020 2063 6f6c 7320  f..        cols 
+00003e50: 3d20 6c69 7374 286e 6577 636f 6c73 2e63  = list(newcols.c
+00003e60: 6f6c 756d 6e73 290d 0a20 2020 2020 2020  olumns)..       
+00003e70: 2066 6f72 2069 2c63 6f6c 2069 6e20 656e   for i,col in en
+00003e80: 756d 6572 6174 6528 636f 6c73 293a 0d0a  umerate(cols):..
+00003e90: 2020 2020 2020 2020 2020 2020 6f6c 645f              old_
+00003ea0: 636f 6c20 3d20 636f 6c0d 0a20 2020 2020  col = col..     
+00003eb0: 2020 2020 2020 2077 6869 6c65 2063 6f6c         while col
+00003ec0: 2069 6e20 7365 6c66 2e64 662e 636f 6c75   in self.df.colu
+00003ed0: 6d6e 733a 0d0a 2020 2020 2020 2020 2020  mns:..          
+00003ee0: 2020 2020 2020 636f 6c73 5b69 5d20 3d20        cols[i] = 
+00003ef0: 636f 6c20 3d20 7374 7228 636f 6c29 2b27  col = str(col)+'
+00003f00: 2b27 0d0a 2020 2020 2020 2020 2020 2020  +'..            
+00003f10: 6966 206f 6c64 5f63 6f6c 2021 3d20 636f  if old_col != co
+00003f20: 6c3a 0d0a 2020 2020 2020 2020 2020 2020  l:..            
+00003f30: 2020 2020 6461 7461 7372 632e 7265 6e61      datasrc.rena
+00003f40: 6d65 735b 6f6c 645f 636f 6c5d 203d 2063  mes[old_col] = c
+00003f50: 6f6c 0d0a 2020 2020 2020 2020 6e65 7763  ol..        newc
+00003f60: 6f6c 732e 636f 6c75 6d6e 7320 3d20 636f  ols.columns = co
+00003f70: 6c73 0d0a 2020 2020 2020 2020 7365 6c66  ls..        self
+00003f80: 2e64 6620 3d20 6466 2e6a 6f69 6e28 6e65  .df = df.join(ne
+00003f90: 7763 6f6c 732c 2068 6f77 3d27 6f75 7465  wcols, how='oute
+00003fa0: 7227 290d 0a20 2020 2020 2020 2069 6620  r')..        if 
+00003fb0: 5f68 6173 5f74 696d 6563 6f6c 2864 6174  _has_timecol(dat
+00003fc0: 6173 7263 2e64 6629 3a0d 0a20 2020 2020  asrc.df):..     
+00003fd0: 2020 2020 2020 2073 656c 662e 6466 2e72         self.df.r
+00003fe0: 6573 6574 5f69 6e64 6578 2869 6e70 6c61  eset_index(inpla
+00003ff0: 6365 3d54 7275 6529 0d0a 2020 2020 2020  ce=True)..      
+00004000: 2020 6461 7461 7372 632e 6466 203d 2073    datasrc.df = s
+00004010: 656c 662e 6466 2023 2074 6865 7920 6172  elf.df # they ar
+00004020: 6520 7468 6520 7361 6d65 206e 6f77 0d0a  e the same now..
+00004030: 2020 2020 2020 2020 6461 7461 7372 632e          datasrc.
+00004040: 696e 6974 5f78 3020 3d20 7365 6c66 2e69  init_x0 = self.i
+00004050: 6e69 745f 7830 0d0a 2020 2020 2020 2020  nit_x0..        
+00004060: 6461 7461 7372 632e 696e 6974 5f78 3120  datasrc.init_x1 
+00004070: 3d20 7365 6c66 2e69 6e69 745f 7831 0d0a  = self.init_x1..
+00004080: 2020 2020 2020 2020 6461 7461 7372 632e          datasrc.
+00004090: 636f 6c5f 6461 7461 5f6f 6666 7365 7420  col_data_offset 
+000040a0: 3d20 6f72 6967 5f63 6f6c 5f64 6174 615f  = orig_col_data_
+000040b0: 636e 740d 0a20 2020 2020 2020 2064 6174  cnt..        dat
+000040c0: 6173 7263 2e73 6361 6c65 5f63 6f6c 7320  asrc.scale_cols 
+000040d0: 3d20 6e65 775f 7363 616c 655f 636f 6c73  = new_scale_cols
+000040e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+000040f0: 6163 6865 5f68 696c 6f20 3d20 4f72 6465  ache_hilo = Orde
+00004100: 7265 6444 6963 7428 290d 0a20 2020 2020  redDict()..     
+00004110: 2020 2073 656c 662e 5f70 6572 696f 6420     self._period 
+00004120: 3d20 7365 6c66 2e5f 736d 6f6f 7468 5f74  = self._smooth_t
+00004130: 696d 6520 3d20 4e6f 6e65 0d0a 2020 2020  ime = None..    
+00004140: 2020 2020 6461 7461 7372 632e 5f70 6572      datasrc._per
+00004150: 696f 6420 3d20 6461 7461 7372 632e 5f73  iod = datasrc._s
+00004160: 6d6f 6f74 685f 7469 6d65 203d 204e 6f6e  mooth_time = Non
+00004170: 650d 0a20 2020 2020 2020 206c 6466 3220  e..        ldf2 
+00004180: 3d20 6c65 6e28 7365 6c66 2e64 6629 202f  = len(self.df) /
+00004190: 2f20 320d 0a20 2020 2020 2020 2073 656c  / 2..        sel
+000041a0: 662e 6973 5f73 7061 7273 6520 3d20 7365  f.is_sparse = se
+000041b0: 6c66 2e69 735f 7370 6172 7365 206f 7220  lf.is_sparse or 
+000041c0: 7365 6c66 2e64 665b 7365 6c66 2e64 662e  self.df[self.df.
+000041d0: 636f 6c75 6d6e 735b 7365 6c66 2e63 6f6c  columns[self.col
+000041e0: 5f64 6174 615f 6f66 6673 6574 5d5d 2e69  _data_offset]].i
+000041f0: 736e 756c 6c28 292e 7375 6d28 292e 6d61  snull().sum().ma
+00004200: 7828 2920 3e20 6c64 6632 0d0a 2020 2020  x() > ldf2..    
+00004210: 2020 2020 6461 7461 7372 632e 6973 5f73      datasrc.is_s
+00004220: 7061 7273 6520 3d20 6461 7461 7372 632e  parse = datasrc.
+00004230: 6973 5f73 7061 7273 6520 6f72 2064 6174  is_sparse or dat
+00004240: 6173 7263 2e64 665b 6461 7461 7372 632e  asrc.df[datasrc.
+00004250: 6466 2e63 6f6c 756d 6e73 5b64 6174 6173  df.columns[datas
+00004260: 7263 2e63 6f6c 5f64 6174 615f 6f66 6673  rc.col_data_offs
+00004270: 6574 5d5d 2e69 736e 756c 6c28 292e 7375  et]].isnull().su
+00004280: 6d28 292e 6d61 7828 2920 3e20 6c64 6632  m().max() > ldf2
+00004290: 0d0a 0d0a 2020 2020 6465 6620 7570 6461  ....    def upda
+000042a0: 7465 2873 656c 662c 2064 6174 6173 7263  te(self, datasrc
+000042b0: 293a 0d0a 2020 2020 2020 2020 6466 203d  ):..        df =
+000042c0: 2073 656c 662e 7072 655f 7570 6461 7465   self.pre_update
+000042d0: 2873 656c 662e 6466 290d 0a20 2020 2020  (self.df)..     
+000042e0: 2020 206f 7269 675f 636f 6c73 203d 206c     orig_cols = l
+000042f0: 6973 7428 6466 2e63 6f6c 756d 6e73 290d  ist(df.columns).
+00004300: 0a20 2020 2020 2020 2074 696d 6563 6f6c  .        timecol
+00004310: 2c6f 7269 675f 636f 6c73 203d 206f 7269  ,orig_cols = ori
+00004320: 675f 636f 6c73 5b30 5d2c 6f72 6967 5f63  g_cols[0],orig_c
+00004330: 6f6c 735b 313a 5d0d 0a20 2020 2020 2020  ols[1:]..       
+00004340: 2064 6620 3d20 6466 2e73 6574 5f69 6e64   df = df.set_ind
+00004350: 6578 2874 696d 6563 6f6c 290d 0a20 2020  ex(timecol)..   
+00004360: 2020 2020 2069 6e70 7574 5f64 6620 3d20       input_df = 
+00004370: 6461 7461 7372 632e 6466 2e73 6574 5f69  datasrc.df.set_i
+00004380: 6e64 6578 2864 6174 6173 7263 2e64 662e  ndex(datasrc.df.
+00004390: 636f 6c75 6d6e 735b 305d 290d 0a20 2020  columns[0])..   
+000043a0: 2020 2020 2069 6e70 7574 5f64 662e 636f       input_df.co
+000043b0: 6c75 6d6e 7320 3d20 5b73 656c 662e 7265  lumns = [self.re
+000043c0: 6e61 6d65 732e 6765 7428 636f 6c2c 2063  names.get(col, c
+000043d0: 6f6c 2920 666f 7220 636f 6c20 696e 2069  ol) for col in i
+000043e0: 6e70 7574 5f64 662e 636f 6c75 6d6e 735d  nput_df.columns]
+000043f0: 0d0a 2020 2020 2020 2020 2320 7061 6420  ..        # pad 
+00004400: 696e 6465 7820 6966 2074 6865 2069 6e70  index if the inp
+00004410: 7574 2064 6174 6120 6973 2061 2073 7562  ut data is a sub
+00004420: 2d73 6574 0d0a 2020 2020 2020 2020 6f75  -set..        ou
+00004430: 7470 7574 5f64 6620 3d20 7064 2e6d 6572  tput_df = pd.mer
+00004440: 6765 2869 6e70 7574 5f64 662c 2064 665b  ge(input_df, df[
+00004450: 5b5d 5d2c 2068 6f77 3d27 6f75 7465 7227  []], how='outer'
+00004460: 2c20 6c65 6674 5f69 6e64 6578 3d54 7275  , left_index=Tru
+00004470: 652c 2072 6967 6874 5f69 6e64 6578 3d54  e, right_index=T
+00004480: 7275 6529 0d0a 2020 2020 2020 2020 666f  rue)..        fo
+00004490: 7220 636f 6c20 696e 2064 662e 636f 6c75  r col in df.colu
+000044a0: 6d6e 733a 0d0a 2020 2020 2020 2020 2020  mns:..          
+000044b0: 2020 6966 2063 6f6c 206e 6f74 2069 6e20    if col not in 
+000044c0: 6f75 7470 7574 5f64 662e 636f 6c75 6d6e  output_df.column
+000044d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000044e0: 2020 2020 6f75 7470 7574 5f64 665b 636f      output_df[co
+000044f0: 6c5d 203d 2064 665b 636f 6c5d 0d0a 2020  l] = df[col]..  
+00004500: 2020 2020 2020 2320 6966 206e 6563 6365        # if necce
+00004510: 7373 6172 792c 2063 7574 206f 7574 2075  ssary, cut out u
+00004520: 6e77 616e 7465 6420 6461 7461 0d0a 2020  nwanted data..  
+00004530: 2020 2020 2020 6966 206c 656e 2869 6e70        if len(inp
+00004540: 7574 5f64 6629 203e 2030 2061 6e64 206c  ut_df) > 0 and l
+00004550: 656e 2864 6629 203e 2030 3a0d 0a20 2020  en(df) > 0:..   
+00004560: 2020 2020 2020 2020 2073 7461 7274 5f69           start_i
+00004570: 6478 203d 2065 6e64 5f69 6478 203d 204e  dx = end_idx = N
+00004580: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
+00004590: 2069 6620 696e 7075 745f 6466 2e69 6e64   if input_df.ind
+000045a0: 6578 5b30 5d20 3e20 6466 2e69 6e64 6578  ex[0] > df.index
+000045b0: 5b30 5d3a 0d0a 2020 2020 2020 2020 2020  [0]:..          
+000045c0: 2020 2020 2020 7374 6172 745f 6964 7820        start_idx 
+000045d0: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+000045e0: 2069 6620 696e 7075 745f 6466 2e69 6e64   if input_df.ind
+000045f0: 6578 5b2d 315d 203c 2064 662e 696e 6465  ex[-1] < df.inde
+00004600: 785b 2d31 5d3a 0d0a 2020 2020 2020 2020  x[-1]:..        
+00004610: 2020 2020 2020 2020 656e 645f 6964 7820          end_idx 
+00004620: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
+00004630: 2020 6966 2073 7461 7274 5f69 6478 2069    if start_idx i
+00004640: 7320 6e6f 7420 4e6f 6e65 206f 7220 656e  s not None or en
+00004650: 645f 6964 7820 6973 206e 6f74 204e 6f6e  d_idx is not Non
+00004660: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00004670: 2020 2020 6f75 7470 7574 5f64 6620 3d20      output_df = 
+00004680: 6f75 7470 7574 5f64 662e 6c6f 635b 696e  output_df.loc[in
+00004690: 7075 745f 6466 2e69 6e64 6578 5b73 7461  put_df.index[sta
+000046a0: 7274 5f69 6478 3a65 6e64 5f69 6478 5d2c  rt_idx:end_idx],
+000046b0: 203a 5d0d 0a20 2020 2020 2020 206f 7574   :]..        out
+000046c0: 7075 745f 6466 203d 2073 656c 662e 706f  put_df = self.po
+000046d0: 7374 5f75 7064 6174 6528 6f75 7470 7574  st_update(output
+000046e0: 5f64 6629 0d0a 2020 2020 2020 2020 6f75  _df)..        ou
+000046f0: 7470 7574 5f64 6620 3d20 6f75 7470 7574  tput_df = output
+00004700: 5f64 662e 7265 7365 745f 696e 6465 7828  _df.reset_index(
+00004710: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004720: 6466 203d 206f 7574 7075 745f 6466 5b5b  df = output_df[[
+00004730: 6f75 7470 7574 5f64 662e 636f 6c75 6d6e  output_df.column
+00004740: 735b 305d 5d2b 6f72 6967 5f63 6f6c 735d  s[0]]+orig_cols]
+00004750: 2069 6620 6f72 6967 5f63 6f6c 7320 656c   if orig_cols el
+00004760: 7365 206f 7574 7075 745f 6466 0d0a 2020  se output_df..  
+00004770: 2020 2020 2020 7365 6c66 2e69 6e69 745f        self.init_
+00004780: 7831 203d 2073 656c 662e 786c 656e 202b  x1 = self.xlen +
+00004790: 2072 6967 6874 5f6d 6172 6769 6e5f 6361   right_margin_ca
+000047a0: 6e64 6c65 7320 2d20 7369 6465 5f6d 6172  ndles - side_mar
+000047b0: 6769 6e0d 0a20 2020 2020 2020 2073 656c  gin..        sel
+000047c0: 662e 6361 6368 655f 6869 6c6f 203d 204f  f.cache_hilo = O
+000047d0: 7264 6572 6564 4469 6374 2829 0d0a 2020  rderedDict()..  
+000047e0: 2020 2020 2020 7365 6c66 2e5f 7065 7269        self._peri
+000047f0: 6f64 203d 2073 656c 662e 5f73 6d6f 6f74  od = self._smoot
+00004800: 685f 7469 6d65 203d 204e 6f6e 650d 0a0d  h_time = None...
+00004810: 0a20 2020 2064 6566 2073 6574 5f64 6628  .    def set_df(
+00004820: 7365 6c66 2c20 6466 293a 0d0a 2020 2020  self, df):..    
+00004830: 2020 2020 7365 6c66 2e64 6620 3d20 6466      self.df = df
+00004840: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00004850: 6163 6865 5f68 696c 6f20 3d20 4f72 6465  ache_hilo = Orde
+00004860: 7265 6444 6963 7428 290d 0a20 2020 2020  redDict()..     
+00004870: 2020 2073 656c 662e 5f70 6572 696f 6420     self._period 
+00004880: 3d20 7365 6c66 2e5f 736d 6f6f 7468 5f74  = self._smooth_t
+00004890: 696d 6520 3d20 4e6f 6e65 0d0a 0d0a 2020  ime = None....  
+000048a0: 2020 6465 6620 6869 6c6f 2873 656c 662c    def hilo(self,
+000048b0: 2078 302c 2078 3129 3a0d 0a20 2020 2020   x0, x1):..     
+000048c0: 2020 2027 2727 5265 7475 726e 2066 6976     '''Return fiv
+000048d0: 6520 7661 6c75 6573 2069 6e20 7469 6d65  e values in time
+000048e0: 2072 616e 6765 3a20 7430 2c20 7431 2c20   range: t0, t1, 
+000048f0: 6869 6768 6573 742c 206c 6f77 6573 742c  highest, lowest,
+00004900: 206e 756d 6265 7220 6f66 2072 6f77 732e   number of rows.
+00004910: 2727 270d 0a20 2020 2020 2020 2069 6620  '''..        if 
+00004920: 7830 203d 3d20 7831 3a0d 0a20 2020 2020  x0 == x1:..     
+00004930: 2020 2020 2020 2078 3020 3d20 7831 203d         x0 = x1 =
+00004940: 2069 6e74 2878 3129 0d0a 2020 2020 2020   int(x1)..      
+00004950: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00004960: 2020 2020 2078 302c 7831 203d 2069 6e74       x0,x1 = int
+00004970: 2878 302b 302e 3529 2c69 6e74 2878 3129  (x0+0.5),int(x1)
+00004980: 0d0a 2020 2020 2020 2020 7175 6572 7920  ..        query 
+00004990: 3d20 2725 692c 2569 2720 2520 2878 302c  = '%i,%i' % (x0,
+000049a0: 7831 290d 0a20 2020 2020 2020 2069 6620  x1)..        if 
+000049b0: 7175 6572 7920 6e6f 7420 696e 2073 656c  query not in sel
+000049c0: 662e 6361 6368 655f 6869 6c6f 3a0d 0a20  f.cache_hilo:.. 
+000049d0: 2020 2020 2020 2020 2020 2076 203d 2073             v = s
+000049e0: 656c 662e 6361 6368 655f 6869 6c6f 5b71  elf.cache_hilo[q
+000049f0: 7565 7279 5d20 3d20 7365 6c66 2e5f 6869  uery] = self._hi
+00004a00: 6c6f 2878 302c 2078 3129 0d0a 2020 2020  lo(x0, x1)..    
+00004a10: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00004a20: 2020 2020 2020 2023 2072 652d 696e 7365         # re-inse
+00004a30: 7274 2074 6f20 7261 6973 6520 7072 696f  rt to raise prio
+00004a40: 0d0a 2020 2020 2020 2020 2020 2020 7620  ..            v 
+00004a50: 3d20 7365 6c66 2e63 6163 6865 5f68 696c  = self.cache_hil
+00004a60: 6f5b 7175 6572 795d 203d 2073 656c 662e  o[query] = self.
+00004a70: 6361 6368 655f 6869 6c6f 2e70 6f70 2871  cache_hilo.pop(q
+00004a80: 7565 7279 290d 0a20 2020 2020 2020 2069  uery)..        i
+00004a90: 6620 6c65 6e28 7365 6c66 2e63 6163 6865  f len(self.cache
+00004aa0: 5f68 696c 6f29 203e 2031 3030 3a20 2320  _hilo) > 100: # 
+00004ab0: 6472 6f70 2069 6620 746f 6f20 6d61 6e79  drop if too many
+00004ac0: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+00004ad0: 6c20 7365 6c66 2e63 6163 6865 5f68 696c  l self.cache_hil
+00004ae0: 6f5b 6e65 7874 2869 7465 7228 7365 6c66  o[next(iter(self
+00004af0: 2e63 6163 6865 5f68 696c 6f29 295d 0d0a  .cache_hilo))]..
+00004b00: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00004b10: 0d0a 0d0a 2020 2020 6465 6620 5f68 696c  ....    def _hil
+00004b20: 6f28 7365 6c66 2c20 7830 2c20 7831 293a  o(self, x0, x1):
+00004b30: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
+00004b40: 656c 662e 6466 2e6c 6f63 5b78 303a 7831  elf.df.loc[x0:x1
+00004b50: 2c20 3a5d 0d0a 2020 2020 2020 2020 6966  , :]..        if
+00004b60: 206e 6f74 206c 656e 2864 6629 3a0d 0a20   not len(df):.. 
+00004b70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00004b80: 6e20 302c 302c 302c 302c 300d 0a20 2020  n 0,0,0,0,0..   
+00004b90: 2020 2020 2074 696d 6563 6f6c 203d 2064       timecol = d
+00004ba0: 662e 636f 6c75 6d6e 735b 305d 0d0a 2020  f.columns[0]..  
+00004bb0: 2020 2020 2020 7430 203d 2064 665b 7469        t0 = df[ti
+00004bc0: 6d65 636f 6c5d 2e69 6c6f 635b 305d 0d0a  mecol].iloc[0]..
+00004bd0: 2020 2020 2020 2020 7431 203d 2064 665b          t1 = df[
+00004be0: 7469 6d65 636f 6c5d 2e69 6c6f 635b 2d31  timecol].iloc[-1
+00004bf0: 5d0d 0a20 2020 2020 2020 2076 616c 636f  ]..        valco
+00004c00: 6c73 203d 2064 662e 636f 6c75 6d6e 735b  ls = df.columns[
+00004c10: 7365 6c66 2e73 6361 6c65 5f63 6f6c 735d  self.scale_cols]
+00004c20: 0d0a 2020 2020 2020 2020 6869 203d 2064  ..        hi = d
+00004c30: 665b 7661 6c63 6f6c 735d 2e6d 6178 2829  f[valcols].max()
+00004c40: 2e6d 6178 2829 0d0a 2020 2020 2020 2020  .max()..        
+00004c50: 6c6f 203d 2064 665b 7661 6c63 6f6c 735d  lo = df[valcols]
+00004c60: 2e6d 696e 2829 2e6d 696e 2829 0d0a 2020  .min().min()..  
+00004c70: 2020 2020 2020 7265 7475 726e 2074 302c        return t0,
+00004c80: 7431 2c68 692c 6c6f 2c6c 656e 2864 6629  t1,hi,lo,len(df)
+00004c90: 0d0a 0d0a 2020 2020 6465 6620 726f 7773  ....    def rows
+00004ca0: 2873 656c 662c 2063 6f6c 636e 742c 2078  (self, colcnt, x
+00004cb0: 302c 2078 312c 2079 7363 616c 652c 206c  0, x1, yscale, l
+00004cc0: 6f64 3d54 7275 652c 2072 6573 616d 703d  od=True, resamp=
+00004cd0: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+00004ce0: 6466 203d 2073 656c 662e 6466 2e6c 6f63  df = self.df.loc
+00004cf0: 5b78 303a 7831 2c20 3a5d 0d0a 2020 2020  [x0:x1, :]..    
+00004d00: 2020 2020 6966 2073 656c 662e 6973 5f73      if self.is_s
+00004d10: 7061 7273 653a 0d0a 2020 2020 2020 2020  parse:..        
+00004d20: 2020 2020 6466 203d 2064 662e 6c6f 635b      df = df.loc[
+00004d30: 6466 2e69 6c6f 635b 3a2c 7365 6c66 2e63  df.iloc[:,self.c
+00004d40: 6f6c 5f64 6174 615f 6f66 6673 6574 5d2e  ol_data_offset].
+00004d50: 6e6f 746e 6128 292c 203a 5d0d 0a20 2020  notna(), :]..   
+00004d60: 2020 2020 206f 7269 676c 656e 203d 206c       origlen = l
+00004d70: 656e 2864 6629 0d0a 2020 2020 2020 2020  en(df)..        
+00004d80: 7265 7475 726e 2073 656c 662e 5f72 6f77  return self._row
+00004d90: 7328 6466 2c20 636f 6c63 6e74 2c20 7973  s(df, colcnt, ys
+00004da0: 6361 6c65 3d79 7363 616c 652c 206c 6f64  cale=yscale, lod
+00004db0: 3d6c 6f64 2c20 7265 7361 6d70 3d72 6573  =lod, resamp=res
+00004dc0: 616d 7029 2c20 6f72 6967 6c65 6e0d 0a0d  amp), origlen...
+00004dd0: 0a20 2020 2064 6566 205f 726f 7773 2873  .    def _rows(s
+00004de0: 656c 662c 2064 662c 2063 6f6c 636e 742c  elf, df, colcnt,
+00004df0: 2079 7363 616c 652c 206c 6f64 2c20 7265   yscale, lod, re
+00004e00: 7361 6d70 293a 0d0a 2020 2020 2020 2020  samp):..        
+00004e10: 6966 206c 6f64 2061 6e64 206c 656e 2864  if lod and len(d
+00004e20: 6629 203e 206c 6f64 5f63 616e 646c 6573  f) > lod_candles
+00004e30: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00004e40: 6620 7265 7361 6d70 3a0d 0a20 2020 2020  f resamp:..     
+00004e50: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
+00004e60: 7365 6c66 2e5f 7265 7361 6d70 6c65 2864  self._resample(d
+00004e70: 662c 2063 6f6c 636e 742c 2072 6573 616d  f, colcnt, resam
+00004e80: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00004e90: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00004ea0: 2020 2020 2020 2064 6620 3d20 6466 2e69         df = df.i
+00004eb0: 6c6f 635b 3a3a 6c65 6e28 6466 292f 2f6c  loc[::len(df)//l
+00004ec0: 6f64 5f63 616e 646c 6573 5d0d 0a20 2020  od_candles]..   
+00004ed0: 2020 2020 2063 6f6c 636e 7420 2d3d 2031       colcnt -= 1
+00004ee0: 2023 2074 696d 6520 6973 2061 6c77 6179   # time is alway
+00004ef0: 7320 696d 706c 6965 640d 0a20 2020 2020  s implied..     
+00004f00: 2020 2063 6f6c 6964 7873 203d 205b 305d     colidxs = [0]
+00004f10: 202b 206c 6973 7428 7261 6e67 6528 7365   + list(range(se
+00004f20: 6c66 2e63 6f6c 5f64 6174 615f 6f66 6673  lf.col_data_offs
+00004f30: 6574 2c20 7365 6c66 2e63 6f6c 5f64 6174  et, self.col_dat
+00004f40: 615f 6f66 6673 6574 2b63 6f6c 636e 7429  a_offset+colcnt)
+00004f50: 290d 0a20 2020 2020 2020 2064 6672 203d  )..        dfr =
+00004f60: 2064 662e 696c 6f63 5b3a 2c63 6f6c 6964   df.iloc[:,colid
+00004f70: 7873 5d0d 0a20 2020 2020 2020 2069 6620  xs]..        if 
+00004f80: 7973 6361 6c65 2e73 6361 6c65 7479 7065  yscale.scaletype
+00004f90: 203d 3d20 276c 6f67 2720 6f72 2079 7363   == 'log' or ysc
+00004fa0: 616c 652e 7363 616c 6566 2021 3d20 313a  ale.scalef != 1:
+00004fb0: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00004fc0: 7220 3d20 6466 722e 636f 7079 2829 0d0a  r = dfr.copy()..
+00004fd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00004fe0: 6920 696e 2072 616e 6765 2831 2c20 636f  i in range(1, co
+00004ff0: 6c63 6e74 2b31 293a 0d0a 2020 2020 2020  lcnt+1):..      
+00005000: 2020 2020 2020 2020 2020 636f 6c6e 616d            colnam
+00005010: 6520 3d20 6466 722e 636f 6c75 6d6e 735b  e = dfr.columns[
+00005020: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00005030: 2020 2020 6966 2064 6672 5b63 6f6c 6e61      if dfr[colna
+00005040: 6d65 5d2e 6474 7970 6520 213d 206f 626a  me].dtype != obj
+00005050: 6563 743a 0d0a 2020 2020 2020 2020 2020  ect:..          
+00005060: 2020 2020 2020 2020 2020 6466 725b 636f            dfr[co
+00005070: 6c6e 616d 655d 203d 2079 7363 616c 652e  lname] = yscale.
+00005080: 696e 7678 666f 726d 2864 6672 2e69 6c6f  invxform(dfr.ilo
+00005090: 635b 3a2c 695d 290d 0a20 2020 2020 2020  c[:,i])..       
+000050a0: 2072 6574 7572 6e20 6466 720d 0a0d 0a20   return dfr.... 
+000050b0: 2020 2064 6566 205f 7265 7361 6d70 6c65     def _resample
+000050c0: 2873 656c 662c 2064 662c 2063 6f6c 636e  (self, df, colcn
+000050d0: 742c 2072 6573 616d 7029 3a0d 0a20 2020  t, resamp):..   
+000050e0: 2020 2020 2063 646f 203d 2073 656c 662e       cdo = self.
+000050f0: 636f 6c5f 6461 7461 5f6f 6666 7365 740d  col_data_offset.
+00005100: 0a20 2020 2020 2020 2073 616d 706c 655f  .        sample_
+00005110: 7261 7465 203d 206c 656e 2864 6629 202a  rate = len(df) *
+00005120: 2035 202f 2f20 6c6f 645f 6361 6e64 6c65   5 // lod_candle
+00005130: 730d 0a20 2020 2020 2020 206f 6666 7365  s..        offse
+00005140: 7420 3d20 6c65 6e28 6466 2920 2520 7361  t = len(df) % sa
+00005150: 6d70 6c65 5f72 6174 650d 0a20 2020 2020  mple_rate..     
+00005160: 2020 2064 6664 203d 2064 665b 5b64 662e     dfd = df[[df.
+00005170: 636f 6c75 6d6e 735b 305d 5d2b 5b64 662e  columns[0]]+[df.
+00005180: 636f 6c75 6d6e 735b 6364 6f5d 5d5d 2e69  columns[cdo]]].i
+00005190: 6c6f 635b 6f66 6673 6574 3a3a 7361 6d70  loc[offset::samp
+000051a0: 6c65 5f72 6174 655d 0d0a 2020 2020 2020  le_rate]..      
+000051b0: 2020 6320 3d20 6466 5b64 662e 636f 6c75    c = df[df.colu
+000051c0: 6d6e 735b 6364 6f2b 315d 5d2e 696c 6f63  mns[cdo+1]].iloc
+000051d0: 5b6f 6666 7365 742b 7361 6d70 6c65 5f72  [offset+sample_r
+000051e0: 6174 652d 313a 3a73 616d 706c 655f 7261  ate-1::sample_ra
+000051f0: 7465 5d0d 0a20 2020 2020 2020 2063 2e69  te]..        c.i
+00005200: 6e64 6578 202d 3d20 7361 6d70 6c65 5f72  ndex -= sample_r
+00005210: 6174 6520 2d20 310d 0a20 2020 2020 2020  ate - 1..       
+00005220: 2064 6664 5b64 662e 636f 6c75 6d6e 735b   dfd[df.columns[
+00005230: 6364 6f2b 315d 5d20 3d20 630d 0a20 2020  cdo+1]] = c..   
+00005240: 2020 2020 2069 6620 7265 7361 6d70 203d       if resamp =
+00005250: 3d20 2768 696c 6f27 3a0d 0a20 2020 2020  = 'hilo':..     
+00005260: 2020 2020 2020 2064 6664 5b64 662e 636f         dfd[df.co
+00005270: 6c75 6d6e 735b 6364 6f2b 325d 5d20 3d20  lumns[cdo+2]] = 
+00005280: 6466 5b64 662e 636f 6c75 6d6e 735b 6364  df[df.columns[cd
+00005290: 6f2b 325d 5d2e 726f 6c6c 696e 6728 7361  o+2]].rolling(sa
+000052a0: 6d70 6c65 5f72 6174 6529 2e6d 6178 2829  mple_rate).max()
+000052b0: 2e73 6869 6674 282d 7361 6d70 6c65 5f72  .shift(-sample_r
+000052c0: 6174 652b 3129 0d0a 2020 2020 2020 2020  ate+1)..        
+000052d0: 2020 2020 6466 645b 6466 2e63 6f6c 756d      dfd[df.colum
+000052e0: 6e73 5b63 646f 2b33 5d5d 203d 2064 665b  ns[cdo+3]] = df[
+000052f0: 6466 2e63 6f6c 756d 6e73 5b63 646f 2b33  df.columns[cdo+3
+00005300: 5d5d 2e72 6f6c 6c69 6e67 2873 616d 706c  ]].rolling(sampl
+00005310: 655f 7261 7465 292e 6d69 6e28 292e 7368  e_rate).min().sh
+00005320: 6966 7428 2d73 616d 706c 655f 7261 7465  ift(-sample_rate
+00005330: 2b31 290d 0a20 2020 2020 2020 2065 6c73  +1)..        els
+00005340: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00005350: 6466 645b 6466 2e63 6f6c 756d 6e73 5b63  dfd[df.columns[c
+00005360: 646f 2b32 5d5d 203d 2064 665b 6466 2e63  do+2]] = df[df.c
+00005370: 6f6c 756d 6e73 5b63 646f 2b32 5d5d 2e72  olumns[cdo+2]].r
+00005380: 6f6c 6c69 6e67 2873 616d 706c 655f 7261  olling(sample_ra
+00005390: 7465 292e 7375 6d28 292e 7368 6966 7428  te).sum().shift(
+000053a0: 2d73 616d 706c 655f 7261 7465 2b31 290d  -sample_rate+1).
+000053b0: 0a20 2020 2020 2020 2020 2020 2064 6664  .            dfd
+000053c0: 5b64 662e 636f 6c75 6d6e 735b 6364 6f2b  [df.columns[cdo+
+000053d0: 335d 5d20 3d20 6466 5b64 662e 636f 6c75  3]] = df[df.colu
+000053e0: 6d6e 735b 6364 6f2b 335d 5d2e 726f 6c6c  mns[cdo+3]].roll
+000053f0: 696e 6728 7361 6d70 6c65 5f72 6174 6529  ing(sample_rate)
+00005400: 2e73 756d 2829 2e73 6869 6674 282d 7361  .sum().shift(-sa
+00005410: 6d70 6c65 5f72 6174 652b 3129 0d0a 2020  mple_rate+1)..  
+00005420: 2020 2020 2020 2320 6170 7065 6e64 2074        # append t
+00005430: 7261 696c 696e 6720 636f 6c75 6d6e 730d  railing columns.
+00005440: 0a20 2020 2020 2020 2074 7261 696c 696e  .        trailin
+00005450: 675f 636f 6c69 6478 203d 2063 646f 202b  g_colidx = cdo +
+00005460: 2034 0d0a 2020 2020 2020 2020 666f 7220   4..        for 
+00005470: 6920 696e 2072 616e 6765 2874 7261 696c  i in range(trail
+00005480: 696e 675f 636f 6c69 6478 2c20 636f 6c63  ing_colidx, colc
+00005490: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
+000054a0: 2020 636f 6c20 3d20 6466 2e63 6f6c 756d    col = df.colum
+000054b0: 6e73 5b69 5d0d 0a20 2020 2020 2020 2020  ns[i]..         
+000054c0: 2020 2064 6664 5b63 6f6c 5d20 3d20 6466     dfd[col] = df
+000054d0: 5b63 6f6c 5d2e 696c 6f63 5b6f 6666 7365  [col].iloc[offse
+000054e0: 743a 3a73 616d 706c 655f 7261 7465 5d0d  t::sample_rate].
+000054f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005500: 6466 640d 0a0d 0a20 2020 2064 6566 205f  dfd....    def _
+00005510: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
+00005520: 7229 3a0d 0a20 2020 2020 2020 2072 6574  r):..        ret
+00005530: 7572 6e20 6964 2873 656c 6629 203d 3d20  urn id(self) == 
+00005540: 6964 286f 7468 6572 2920 6f72 2069 6428  id(other) or id(
+00005550: 7365 6c66 2e64 6629 203d 3d20 6964 286f  self.df) == id(o
+00005560: 7468 6572 2e64 6629 0d0a 0d0a 2020 2020  ther.df)....    
+00005570: 6465 6620 5f5f 6861 7368 5f5f 2873 656c  def __hash__(sel
+00005580: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+00005590: 7572 6e20 6964 2873 656c 6629 0d0a 0d0a  urn id(self)....
+000055a0: 0d0a 636c 6173 7320 4669 6e57 696e 646f  ..class FinWindo
+000055b0: 7728 7067 2e47 7261 7068 6963 734c 6179  w(pg.GraphicsLay
+000055c0: 6f75 7457 6964 6765 7429 3a0d 0a20 2020  outWidget):..   
+000055d0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000055e0: 6c66 2c20 7469 746c 652c 202a 2a6b 7761  lf, title, **kwa
+000055f0: 7267 7329 3a0d 0a20 2020 2020 2020 2067  rgs):..        g
+00005600: 6c6f 6261 6c20 7769 6e78 2c20 7769 6e79  lobal winx, winy
+00005610: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00005620: 6974 6c65 203d 2074 6974 6c65 0d0a 2020  itle = title..  
+00005630: 2020 2020 2020 7067 2e6d 6b51 4170 7028        pg.mkQApp(
+00005640: 290d 0a20 2020 2020 2020 2073 7570 6572  )..        super
+00005650: 2829 2e5f 5f69 6e69 745f 5f28 2a2a 6b77  ().__init__(**kw
+00005660: 6172 6773 290d 0a20 2020 2020 2020 2073  args)..        s
+00005670: 656c 662e 7365 7457 696e 646f 7754 6974  elf.setWindowTit
+00005680: 6c65 2874 6974 6c65 290d 0a20 2020 2020  le(title)..     
+00005690: 2020 2073 656c 662e 7365 7447 656f 6d65     self.setGeome
+000056a0: 7472 7928 7769 6e78 2c20 7769 6e79 2c20  try(winx, winy, 
+000056b0: 7769 6e77 2c20 7769 6e68 290d 0a20 2020  winw, winh)..   
+000056c0: 2020 2020 2077 696e 7820 2b3d 2034 300d       winx += 40.
+000056d0: 0a20 2020 2020 2020 2077 696e 7920 2b3d  .        winy +=
+000056e0: 2034 300d 0a20 2020 2020 2020 2073 656c   40..        sel
+000056f0: 662e 6365 6e74 7261 6c57 6964 6765 742e  f.centralWidget.
+00005700: 696e 7374 616c 6c45 7665 6e74 4669 6c74  installEventFilt
+00005710: 6572 2873 656c 6629 0d0a 2020 2020 2020  er(self)..      
+00005720: 2020 7365 6c66 2e63 692e 7365 7443 6f6e    self.ci.setCon
+00005730: 7465 6e74 734d 6172 6769 6e73 2830 2c20  tentsMargins(0, 
+00005740: 302c 2030 2c20 3029 0d0a 2020 2020 2020  0, 0, 0)..      
+00005750: 2020 7365 6c66 2e63 692e 7365 7453 7061    self.ci.setSpa
+00005760: 6369 6e67 282d 3129 0d0a 2020 2020 2020  cing(-1)..      
+00005770: 2020 7365 6c66 2e63 6c6f 7369 6e67 203d    self.closing =
+00005780: 2046 616c 7365 0d0a 0d0a 2020 2020 4070   False....    @p
+00005790: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+000057a0: 2061 7873 2873 656c 6629 3a0d 0a20 2020   axs(self):..   
+000057b0: 2020 2020 2072 6574 7572 6e20 5b61 7820       return [ax 
+000057c0: 666f 7220 6178 2069 6e20 7365 6c66 2e63  for ax in self.c
+000057d0: 692e 6974 656d 7320 6966 2069 7369 6e73  i.items if isins
+000057e0: 7461 6e63 6528 6178 2c20 7067 2e50 6c6f  tance(ax, pg.Plo
+000057f0: 7449 7465 6d29 5d0d 0a0d 0a20 2020 2064  tItem)]....    d
+00005800: 6566 2061 7574 6f52 616e 6765 456e 6162  ef autoRangeEnab
+00005810: 6c65 6428 7365 6c66 293a 0d0a 2020 2020  led(self):..    
+00005820: 2020 2020 7265 7475 726e 205b 5472 7565      return [True
+00005830: 2c20 5472 7565 5d0d 0a0d 0a20 2020 2064  , True]....    d
+00005840: 6566 2063 6c6f 7365 2873 656c 6629 3a0d  ef close(self):.
+00005850: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+00005860: 6f73 696e 6720 3d20 5472 7565 0d0a 2020  osing = True..  
+00005870: 2020 2020 2020 5f73 6176 6577 696e 6461        _savewinda
+00005880: 7461 2873 656c 6629 0d0a 2020 2020 2020  ta(self)..      
+00005890: 2020 5f63 6c65 6172 5f74 696d 6572 7328    _clear_timers(
+000058a0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000058b0: 6e20 7375 7065 7228 292e 636c 6f73 6528  n super().close(
+000058c0: 290d 0a0d 0a20 2020 2064 6566 2065 7665  )....    def eve
+000058d0: 6e74 4669 6c74 6572 2873 656c 662c 206f  ntFilter(self, o
+000058e0: 626a 2c20 6576 293a 0d0a 2020 2020 2020  bj, ev):..      
+000058f0: 2020 6966 2065 762e 7479 7065 2829 3d3d    if ev.type()==
+00005900: 2051 7443 6f72 652e 5145 7665 6e74 2e54   QtCore.QEvent.T
+00005910: 7970 652e 5769 6e64 6f77 4465 6163 7469  ype.WindowDeacti
+00005920: 7661 7465 3a0d 0a20 2020 2020 2020 2020  vate:..         
+00005930: 2020 205f 7361 7665 7769 6e64 6174 6128     _savewindata(
+00005940: 7365 6c66 290d 0a20 2020 2020 2020 2072  self)..        r
+00005950: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
+00005960: 2020 2064 6566 206c 6561 7665 4576 656e     def leaveEven
+00005970: 7428 7365 6c66 2c20 6576 293a 0d0a 2020  t(self, ev):..  
+00005980: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00005990: 662e 636c 6f73 696e 673a 0d0a 2020 2020  f.closing:..    
+000059a0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+000059b0: 6c65 6176 6545 7665 6e74 2865 7629 0d0a  leaveEvent(ev)..
+000059c0: 0d0a 0d0a 636c 6173 7320 4669 6e43 726f  ....class FinCro
+000059d0: 7373 4861 6972 3a0d 0a20 2020 2064 6566  ssHair:..    def
+000059e0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+000059f0: 6178 2c20 636f 6c6f 7229 3a0d 0a20 2020  ax, color):..   
+00005a00: 2020 2020 2073 656c 662e 6178 203d 2061       self.ax = a
+00005a10: 780d 0a20 2020 2020 2020 2073 656c 662e  x..        self.
+00005a20: 7820 3d20 300d 0a20 2020 2020 2020 2073  x = 0..        s
+00005a30: 656c 662e 7920 3d20 300d 0a20 2020 2020  elf.y = 0..     
+00005a40: 2020 2073 656c 662e 636c 616d 705f 7820     self.clamp_x 
+00005a50: 3d20 300d 0a20 2020 2020 2020 2073 656c  = 0..        sel
+00005a60: 662e 636c 616d 705f 7920 3d20 300d 0a20  f.clamp_y = 0.. 
+00005a70: 2020 2020 2020 2073 656c 662e 696e 666f         self.info
+00005a80: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00005a90: 7065 6e20 3d20 7067 2e6d 6b50 656e 2863  pen = pg.mkPen(c
+00005aa0: 6f6c 6f72 3d63 6f6c 6f72 2c20 7374 796c  olor=color, styl
+00005ab0: 653d 5174 436f 7265 2e51 742e 5065 6e53  e=QtCore.Qt.PenS
+00005ac0: 7479 6c65 2e43 7573 746f 6d44 6173 684c  tyle.CustomDashL
+00005ad0: 696e 652c 2064 6173 683d 5b37 2c20 375d  ine, dash=[7, 7]
+00005ae0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00005af0: 766c 696e 6520 3d20 7067 2e49 6e66 696e  vline = pg.Infin
+00005b00: 6974 654c 696e 6528 616e 676c 653d 3930  iteLine(angle=90
+00005b10: 2c20 6d6f 7661 626c 653d 4661 6c73 652c  , movable=False,
+00005b20: 2070 656e 3d70 656e 290d 0a20 2020 2020   pen=pen)..     
+00005b30: 2020 2073 656c 662e 686c 696e 6520 3d20     self.hline = 
+00005b40: 7067 2e49 6e66 696e 6974 654c 696e 6528  pg.InfiniteLine(
+00005b50: 616e 676c 653d 302c 206d 6f76 6162 6c65  angle=0, movable
+00005b60: 3d46 616c 7365 2c20 7065 6e3d 7065 6e29  =False, pen=pen)
+00005b70: 0d0a 2020 2020 2020 2020 7365 6c66 2e78  ..        self.x
+00005b80: 7465 7874 203d 2070 672e 5465 7874 4974  text = pg.TextIt
+00005b90: 656d 2863 6f6c 6f72 3d63 6f6c 6f72 2c20  em(color=color, 
+00005ba0: 616e 6368 6f72 3d28 302c 3129 290d 0a20  anchor=(0,1)).. 
+00005bb0: 2020 2020 2020 2073 656c 662e 7974 6578         self.ytex
+00005bc0: 7420 3d20 7067 2e54 6578 7449 7465 6d28  t = pg.TextItem(
+00005bd0: 636f 6c6f 723d 636f 6c6f 722c 2061 6e63  color=color, anc
+00005be0: 686f 723d 2830 2c30 2929 0d0a 2020 2020  hor=(0,0))..    
+00005bf0: 2020 2020 7365 6c66 2e76 6c69 6e65 2e73      self.vline.s
+00005c00: 6574 5a56 616c 7565 2835 3029 0d0a 2020  etZValue(50)..  
+00005c10: 2020 2020 2020 7365 6c66 2e68 6c69 6e65        self.hline
+00005c20: 2e73 6574 5a56 616c 7565 2835 3029 0d0a  .setZValue(50)..
+00005c30: 2020 2020 2020 2020 7365 6c66 2e78 7465          self.xte
+00005c40: 7874 2e73 6574 5a56 616c 7565 2835 3029  xt.setZValue(50)
+00005c50: 0d0a 2020 2020 2020 2020 7365 6c66 2e79  ..        self.y
+00005c60: 7465 7874 2e73 6574 5a56 616c 7565 2835  text.setZValue(5
+00005c70: 3029 0d0a 2020 2020 2020 2020 7365 6c66  0)..        self
+00005c80: 2e73 686f 7728 290d 0a0d 0a20 2020 2064  .show()....    d
+00005c90: 6566 2075 7064 6174 6528 7365 6c66 2c20  ef update(self, 
+00005ca0: 706f 696e 743d 4e6f 6e65 293a 0d0a 2020  point=None):..  
+00005cb0: 2020 2020 2020 6966 2070 6f69 6e74 2069        if point i
+00005cc0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00005cd0: 2020 2020 2020 2020 2073 656c 662e 782c           self.x,
+00005ce0: 7365 6c66 2e79 203d 2078 2c79 203d 2070  self.y = x,y = p
+00005cf0: 6f69 6e74 2e78 2829 2c70 6f69 6e74 2e79  oint.x(),point.y
+00005d00: 2829 0d0a 2020 2020 2020 2020 656c 7365  ()..        else
+00005d10: 3a0d 0a20 2020 2020 2020 2020 2020 2078  :..            x
+00005d20: 2c79 203d 2073 656c 662e 782c 7365 6c66  ,y = self.x,self
+00005d30: 2e79 0d0a 2020 2020 2020 2020 782c 7920  .y..        x,y 
+00005d40: 3d20 5f63 6c61 6d70 5f78 7928 7365 6c66  = _clamp_xy(self
+00005d50: 2e61 782c 2078 2c79 290d 0a20 2020 2020  .ax, x,y)..     
+00005d60: 2020 2069 6620 7820 3d3d 2073 656c 662e     if x == self.
+00005d70: 636c 616d 705f 7820 616e 6420 7920 3d3d  clamp_x and y ==
+00005d80: 2073 656c 662e 636c 616d 705f 793a 0d0a   self.clamp_y:..
+00005d90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005da0: 726e 0d0a 2020 2020 2020 2020 7365 6c66  rn..        self
+00005db0: 2e63 6c61 6d70 5f78 2c73 656c 662e 636c  .clamp_x,self.cl
+00005dc0: 616d 705f 7920 3d20 782c 790d 0a20 2020  amp_y = x,y..   
+00005dd0: 2020 2020 2073 656c 662e 766c 696e 652e       self.vline.
+00005de0: 7365 7450 6f73 2878 290d 0a20 2020 2020  setPos(x)..     
+00005df0: 2020 2073 656c 662e 686c 696e 652e 7365     self.hline.se
+00005e00: 7450 6f73 2879 290d 0a20 2020 2020 2020  tPos(y)..       
+00005e10: 2073 656c 662e 7874 6578 742e 7365 7450   self.xtext.setP
+00005e20: 6f73 2878 2c20 7929 0d0a 2020 2020 2020  os(x, y)..      
+00005e30: 2020 7365 6c66 2e79 7465 7874 2e73 6574    self.ytext.set
+00005e40: 506f 7328 782c 2079 290d 0a20 2020 2020  Pos(x, y)..     
+00005e50: 2020 2072 6e67 203d 2073 656c 662e 6178     rng = self.ax
+00005e60: 2e76 622e 795f 6d61 7820 2d20 7365 6c66  .vb.y_max - self
+00005e70: 2e61 782e 7662 2e79 5f6d 696e 0d0a 2020  .ax.vb.y_min..  
+00005e80: 2020 2020 2020 726e 676d 6178 203d 2061        rngmax = a
+00005e90: 6273 2873 656c 662e 6178 2e76 622e 795f  bs(self.ax.vb.y_
+00005ea0: 6d69 6e29 202b 2072 6e67 2023 2061 6e79  min) + rng # any
+00005eb0: 2061 7070 726f 7869 6d61 7469 6f6e 2069   approximation i
+00005ec0: 7320 6669 6e65 0d0a 2020 2020 2020 2020  s fine..        
+00005ed0: 7364 2c73 6520 3d20 2873 656c 662e 6178  sd,se = (self.ax
+00005ee0: 2e73 6967 6e69 6669 6361 6e74 5f64 6563  .significant_dec
+00005ef0: 696d 616c 732c 7365 6c66 2e61 782e 7369  imals,self.ax.si
+00005f00: 676e 6966 6963 616e 745f 6570 7329 2069  gnificant_eps) i
+00005f10: 6620 636c 616d 705f 6772 6964 2065 6c73  f clamp_grid els
+00005f20: 6520 2873 6967 6e69 6669 6361 6e74 5f64  e (significant_d
+00005f30: 6563 696d 616c 732c 7369 676e 6966 6963  ecimals,signific
+00005f40: 616e 745f 6570 7329 0d0a 2020 2020 2020  ant_eps)..      
+00005f50: 2020 7469 6d65 6261 7365 6420 3d20 4661    timebased = Fa
+00005f60: 6c73 650d 0a20 2020 2020 2020 2069 6620  lse..        if 
+00005f70: 7365 6c66 2e61 782e 7662 2e78 5f69 6e64  self.ax.vb.x_ind
+00005f80: 6578 6564 3a0d 0a20 2020 2020 2020 2020  exed:..         
+00005f90: 2020 2078 7465 7874 2c74 696d 6562 6173     xtext,timebas
+00005fa0: 6564 203d 205f 7832 6c6f 6361 6c5f 7428  ed = _x2local_t(
+00005fb0: 7365 6c66 2e61 782e 7662 2e64 6174 6173  self.ax.vb.datas
+00005fc0: 7263 2c20 7829 0d0a 2020 2020 2020 2020  rc, x)..        
+00005fd0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005fe0: 2020 2078 7465 7874 203d 205f 726f 756e     xtext = _roun
+00005ff0: 645f 746f 5f73 6967 6e69 6669 6361 6e74  d_to_significant
+00006000: 2872 6e67 2c20 726e 676d 6178 2c20 782c  (rng, rngmax, x,
+00006010: 2073 642c 2073 6529 0d0a 2020 2020 2020   sd, se)..      
+00006020: 2020 6c69 6e65 6172 5f79 203d 2079 0d0a    linear_y = y..
+00006030: 2020 2020 2020 2020 7920 3d20 7365 6c66          y = self
+00006040: 2e61 782e 7662 2e79 7363 616c 652e 7866  .ax.vb.yscale.xf
+00006050: 6f72 6d28 7929 0d0a 2020 2020 2020 2020  orm(y)..        
+00006060: 7974 6578 7420 3d20 5f72 6f75 6e64 5f74  ytext = _round_t
+00006070: 6f5f 7369 676e 6966 6963 616e 7428 726e  o_significant(rn
+00006080: 672c 2072 6e67 6d61 782c 2079 2c20 7364  g, rngmax, y, sd
+00006090: 2c20 7365 290d 0a20 2020 2020 2020 2069  , se)..        i
+000060a0: 6620 6e6f 7420 7469 6d65 6261 7365 643a  f not timebased:
+000060b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000060c0: 2078 7465 7874 3a0d 0a20 2020 2020 2020   xtext:..       
+000060d0: 2020 2020 2020 2020 2078 7465 7874 203d           xtext =
+000060e0: 2027 7820 2720 2b20 7874 6578 740d 0a20   'x ' + xtext.. 
+000060f0: 2020 2020 2020 2020 2020 2079 7465 7874             ytext
+00006100: 203d 2027 7920 2720 2b20 7974 6578 740d   = 'y ' + ytext.
+00006110: 0a20 2020 2020 2020 2066 6172 5f72 6967  .        far_rig
+00006120: 6874 203d 2073 656c 662e 6178 2e76 6965  ht = self.ax.vie
+00006130: 7752 6563 7428 292e 7828 2920 2b20 7365  wRect().x() + se
+00006140: 6c66 2e61 782e 7669 6577 5265 6374 2829  lf.ax.viewRect()
+00006150: 2e77 6964 7468 2829 2a30 2e39 0d0a 2020  .width()*0.9..  
+00006160: 2020 2020 2020 6661 725f 626f 7474 6f6d        far_bottom
+00006170: 203d 2073 656c 662e 6178 2e76 6965 7752   = self.ax.viewR
+00006180: 6563 7428 292e 7928 2920 2b20 7365 6c66  ect().y() + self
+00006190: 2e61 782e 7669 6577 5265 6374 2829 2e68  .ax.viewRect().h
+000061a0: 6569 6768 7428 292a 302e 310d 0a20 2020  eight()*0.1..   
+000061b0: 2020 2020 2063 6c6f 7365 3272 6967 6874       close2right
+000061c0: 203d 2078 203e 2066 6172 5f72 6967 6874   = x > far_right
+000061d0: 0d0a 2020 2020 2020 2020 636c 6f73 6532  ..        close2
+000061e0: 626f 7474 6f6d 203d 206c 696e 6561 725f  bottom = linear_
+000061f0: 7920 3c20 6661 725f 626f 7474 6f6d 0d0a  y < far_bottom..
+00006200: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00006210: 2020 2020 2020 2020 2020 666f 7220 696e            for in
+00006220: 666f 2069 6e20 7365 6c66 2e69 6e66 6f73  fo in self.infos
+00006230: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00006240: 2020 2078 7465 7874 2c79 7465 7874 203d     xtext,ytext =
+00006250: 2069 6e66 6f28 782c 792c 7874 6578 742c   info(x,y,xtext,
+00006260: 7974 6578 7429 0d0a 2020 2020 2020 2020  ytext)..        
+00006270: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00006280: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00006290: 2020 2020 7072 696e 7428 2743 726f 7373      print('Cross
+000062a0: 6861 6972 2065 7272 6f72 3a27 2c20 7479  hair error:', ty
+000062b0: 7065 2865 292c 2065 290d 0a20 2020 2020  pe(e), e)..     
+000062c0: 2020 2073 7061 6365 203d 2027 2020 2020     space = '    
+000062d0: 2020 270d 0a20 2020 2020 2020 2069 6620    '..        if 
+000062e0: 636c 6f73 6532 7269 6768 743a 0d0a 2020  close2right:..  
+000062f0: 2020 2020 2020 2020 2020 7874 6578 7420            xtext 
+00006300: 3d20 7874 6578 7420 2b20 7370 6163 650d  = xtext + space.
+00006310: 0a20 2020 2020 2020 2020 2020 2079 7465  .            yte
+00006320: 7874 203d 2079 7465 7874 202b 2073 7061  xt = ytext + spa
+00006330: 6365 0d0a 2020 2020 2020 2020 2020 2020  ce..            
+00006340: 7861 6e63 686f 7220 3d20 5b31 2c31 5d0d  xanchor = [1,1].
+00006350: 0a20 2020 2020 2020 2020 2020 2079 616e  .            yan
+00006360: 6368 6f72 203d 205b 312c 305d 0d0a 2020  chor = [1,0]..  
+00006370: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00006380: 2020 2020 2020 2020 2078 7465 7874 203d           xtext =
+00006390: 2073 7061 6365 202b 2078 7465 7874 0d0a   space + xtext..
+000063a0: 2020 2020 2020 2020 2020 2020 7974 6578              ytex
+000063b0: 7420 3d20 7370 6163 6520 2b20 7974 6578  t = space + ytex
+000063c0: 740d 0a20 2020 2020 2020 2020 2020 2078  t..            x
+000063d0: 616e 6368 6f72 203d 205b 302c 315d 0d0a  anchor = [0,1]..
+000063e0: 2020 2020 2020 2020 2020 2020 7961 6e63              yanc
+000063f0: 686f 7220 3d20 5b30 2c30 5d0d 0a20 2020  hor = [0,0]..   
+00006400: 2020 2020 2069 6620 636c 6f73 6532 626f       if close2bo
+00006410: 7474 6f6d 3a0d 0a20 2020 2020 2020 2020  ttom:..         
+00006420: 2020 2079 7465 7874 203d 2079 7465 7874     ytext = ytext
+00006430: 202b 2073 7061 6365 0d0a 2020 2020 2020   + space..      
+00006440: 2020 2020 2020 7961 6e63 686f 7220 3d20        yanchor = 
+00006450: 5b31 2c31 5d0d 0a20 2020 2020 2020 2020  [1,1]..         
+00006460: 2020 2069 6620 636c 6f73 6532 7269 6768     if close2righ
+00006470: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00006480: 2020 2020 7861 6e63 686f 7220 3d20 5b31      xanchor = [1
+00006490: 2c32 5d0d 0a20 2020 2020 2020 2073 656c  ,2]..        sel
+000064a0: 662e 7874 6578 742e 7365 7441 6e63 686f  f.xtext.setAncho
+000064b0: 7228 7861 6e63 686f 7229 0d0a 2020 2020  r(xanchor)..    
+000064c0: 2020 2020 7365 6c66 2e79 7465 7874 2e73      self.ytext.s
+000064d0: 6574 416e 6368 6f72 2879 616e 6368 6f72  etAnchor(yanchor
+000064e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000064f0: 7874 6578 742e 7365 7454 6578 7428 7874  xtext.setText(xt
+00006500: 6578 7429 0d0a 2020 2020 2020 2020 7365  ext)..        se
+00006510: 6c66 2e79 7465 7874 2e73 6574 5465 7874  lf.ytext.setText
+00006520: 2879 7465 7874 290d 0a0d 0a20 2020 2064  (ytext)....    d
+00006530: 6566 2073 686f 7728 7365 6c66 293a 0d0a  ef show(self):..
+00006540: 2020 2020 2020 2020 7365 6c66 2e61 782e          self.ax.
+00006550: 6164 6449 7465 6d28 7365 6c66 2e76 6c69  addItem(self.vli
+00006560: 6e65 2c20 6967 6e6f 7265 426f 756e 6473  ne, ignoreBounds
+00006570: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00006580: 7365 6c66 2e61 782e 6164 6449 7465 6d28  self.ax.addItem(
+00006590: 7365 6c66 2e68 6c69 6e65 2c20 6967 6e6f  self.hline, igno
+000065a0: 7265 426f 756e 6473 3d54 7275 6529 0d0a  reBounds=True)..
+000065b0: 2020 2020 2020 2020 7365 6c66 2e61 782e          self.ax.
+000065c0: 6164 6449 7465 6d28 7365 6c66 2e78 7465  addItem(self.xte
+000065d0: 7874 2c20 6967 6e6f 7265 426f 756e 6473  xt, ignoreBounds
+000065e0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+000065f0: 7365 6c66 2e61 782e 6164 6449 7465 6d28  self.ax.addItem(
+00006600: 7365 6c66 2e79 7465 7874 2c20 6967 6e6f  self.ytext, igno
+00006610: 7265 426f 756e 6473 3d54 7275 6529 0d0a  reBounds=True)..
+00006620: 0d0a 2020 2020 6465 6620 6869 6465 2873  ..    def hide(s
+00006630: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+00006640: 656c 662e 6178 2e72 656d 6f76 6549 7465  elf.ax.removeIte
+00006650: 6d28 7365 6c66 2e78 7465 7874 290d 0a20  m(self.xtext).. 
+00006660: 2020 2020 2020 2073 656c 662e 6178 2e72         self.ax.r
+00006670: 656d 6f76 6549 7465 6d28 7365 6c66 2e79  emoveItem(self.y
+00006680: 7465 7874 290d 0a20 2020 2020 2020 2073  text)..        s
+00006690: 656c 662e 6178 2e72 656d 6f76 6549 7465  elf.ax.removeIte
+000066a0: 6d28 7365 6c66 2e76 6c69 6e65 290d 0a20  m(self.vline).. 
+000066b0: 2020 2020 2020 2073 656c 662e 6178 2e72         self.ax.r
+000066c0: 656d 6f76 6549 7465 6d28 7365 6c66 2e68  emoveItem(self.h
+000066d0: 6c69 6e65 290d 0a0d 0a0d 0a0d 0a63 6c61  line)........cla
+000066e0: 7373 2046 696e 4c65 6765 6e64 4974 656d  ss FinLegendItem
+000066f0: 2870 672e 4c65 6765 6e64 4974 656d 293a  (pg.LegendItem):
+00006700: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00006710: 5f5f 2873 656c 662c 2062 6f72 6465 725f  __(self, border_
+00006720: 636f 6c6f 722c 2066 696c 6c5f 636f 6c6f  color, fill_colo
+00006730: 722c 202a 2a6b 7761 7267 7329 3a0d 0a20  r, **kwargs):.. 
+00006740: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00006750: 5f69 6e69 745f 5f28 2a2a 6b77 6172 6773  _init__(**kwargs
+00006760: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006770: 6c61 796f 7574 2e73 6574 5665 7274 6963  layout.setVertic
+00006780: 616c 5370 6163 696e 6728 3229 0d0a 2020  alSpacing(2)..  
+00006790: 2020 2020 2020 7365 6c66 2e6c 6179 6f75        self.layou
+000067a0: 742e 7365 7448 6f72 697a 6f6e 7461 6c53  t.setHorizontalS
+000067b0: 7061 6369 6e67 2832 3029 0d0a 2020 2020  pacing(20)..    
+000067c0: 2020 2020 7365 6c66 2e6c 6179 6f75 742e      self.layout.
+000067d0: 7365 7443 6f6e 7465 6e74 734d 6172 6769  setContentsMargi
+000067e0: 6e73 2832 2c20 322c 2031 302c 2032 290d  ns(2, 2, 10, 2).
+000067f0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+00006800: 7264 6572 5f63 6f6c 6f72 203d 2062 6f72  rder_color = bor
+00006810: 6465 725f 636f 6c6f 720d 0a20 2020 2020  der_color..     
+00006820: 2020 2073 656c 662e 6669 6c6c 5f63 6f6c     self.fill_col
+00006830: 6f72 203d 2066 696c 6c5f 636f 6c6f 720d  or = fill_color.
+00006840: 0a0d 0a20 2020 2064 6566 2070 6169 6e74  ...    def paint
+00006850: 2873 656c 662c 2070 2c20 2a61 7267 7329  (self, p, *args)
+00006860: 3a0d 0a20 2020 2020 2020 2070 2e73 6574  :..        p.set
+00006870: 5065 6e28 7067 2e6d 6b50 656e 2873 656c  Pen(pg.mkPen(sel
+00006880: 662e 626f 7264 6572 5f63 6f6c 6f72 2929  f.border_color))
+00006890: 0d0a 2020 2020 2020 2020 702e 7365 7442  ..        p.setB
+000068a0: 7275 7368 2870 672e 6d6b 4272 7573 6828  rush(pg.mkBrush(
+000068b0: 7365 6c66 2e66 696c 6c5f 636f 6c6f 7229  self.fill_color)
+000068c0: 290d 0a20 2020 2020 2020 2070 2e64 7261  )..        p.dra
+000068d0: 7752 6563 7428 7365 6c66 2e62 6f75 6e64  wRect(self.bound
+000068e0: 696e 6752 6563 7428 2929 0d0a 0d0a 0d0a  ingRect())......
+000068f0: 0d0a 636c 6173 7320 4669 6e50 6f6c 794c  ..class FinPolyL
+00006900: 696e 6528 7067 2e50 6f6c 794c 696e 6552  ine(pg.PolyLineR
+00006910: 4f49 293a 0d0a 2020 2020 6465 6620 5f5f  OI):..    def __
+00006920: 696e 6974 5f5f 2873 656c 662c 2076 622c  init__(self, vb,
+00006930: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00006940: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00006950: 2e76 6220 3d20 7662 2023 2069 6e69 7420  .vb = vb # init 
+00006960: 6265 666f 7265 2070 6172 656e 7420 636f  before parent co
+00006970: 6e73 7472 7563 746f 720d 0a20 2020 2020  nstructor..     
+00006980: 2020 2073 656c 662e 7465 7874 7320 3d20     self.texts = 
+00006990: 5b5d 0d0a 2020 2020 2020 2020 7375 7065  []..        supe
+000069a0: 7228 292e 5f5f 696e 6974 5f5f 282a 6172  r().__init__(*ar
+000069b0: 6773 2c20 2a2a 6b77 6172 6773 290d 0a0d  gs, **kwargs)...
+000069c0: 0a20 2020 2064 6566 2061 6464 5365 676d  .    def addSegm
+000069d0: 656e 7428 7365 6c66 2c20 6831 2c20 6832  ent(self, h1, h2
+000069e0: 2c20 696e 6465 783d 4e6f 6e65 293a 0d0a  , index=None):..
+000069f0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00006a00: 6164 6453 6567 6d65 6e74 2868 312c 2068  addSegment(h1, h
+00006a10: 322c 2069 6e64 6578 290d 0a20 2020 2020  2, index)..     
+00006a20: 2020 2074 6578 7420 3d20 7067 2e54 6578     text = pg.Tex
+00006a30: 7449 7465 6d28 636f 6c6f 723d 6472 6177  tItem(color=draw
+00006a40: 5f6c 696e 655f 636f 6c6f 7229 0d0a 2020  _line_color)..  
+00006a50: 2020 2020 2020 7465 7874 2e73 6574 5a56        text.setZV
+00006a60: 616c 7565 2835 3029 0d0a 2020 2020 2020  alue(50)..      
+00006a70: 2020 7465 7874 2e73 6567 6d65 6e74 203d    text.segment =
+00006a80: 2073 656c 662e 7365 676d 656e 7473 5b2d   self.segments[-
+00006a90: 3120 6966 2069 6e64 6578 2069 7320 4e6f  1 if index is No
+00006aa0: 6e65 2065 6c73 6520 696e 6465 785d 0d0a  ne else index]..
+00006ab0: 2020 2020 2020 2020 6966 2069 6e64 6578          if index
+00006ac0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00006ad0: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
+00006ae0: 732e 6170 7065 6e64 2874 6578 7429 0d0a  s.append(text)..
+00006af0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00006b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006b10: 7465 7874 732e 696e 7365 7274 2869 6e64  texts.insert(ind
+00006b20: 6578 2c20 7465 7874 290d 0a20 2020 2020  ex, text)..     
+00006b30: 2020 2073 656c 662e 7570 6461 7465 5f74     self.update_t
+00006b40: 6578 7428 7465 7874 290d 0a20 2020 2020  ext(text)..     
+00006b50: 2020 2073 656c 662e 7662 2e61 6464 4974     self.vb.addIt
+00006b60: 656d 2874 6578 742c 2069 676e 6f72 6542  em(text, ignoreB
+00006b70: 6f75 6e64 733d 5472 7565 290d 0a0d 0a20  ounds=True).... 
+00006b80: 2020 2064 6566 2072 656d 6f76 6553 6567     def removeSeg
+00006b90: 6d65 6e74 2873 656c 662c 2073 6567 293a  ment(self, seg):
+00006ba0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+00006bb0: 292e 7265 6d6f 7665 5365 676d 656e 7428  ).removeSegment(
+00006bc0: 7365 6729 0d0a 2020 2020 2020 2020 666f  seg)..        fo
+00006bd0: 7220 7465 7874 2069 6e20 6c69 7374 2873  r text in list(s
+00006be0: 656c 662e 7465 7874 7329 3a0d 0a20 2020  elf.texts):..   
+00006bf0: 2020 2020 2020 2020 2069 6620 7465 7874           if text
+00006c00: 2e73 6567 6d65 6e74 203d 3d20 7365 673a  .segment == seg:
+00006c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006c20: 2020 7365 6c66 2e76 622e 7265 6d6f 7665    self.vb.remove
+00006c30: 4974 656d 2874 6578 7429 0d0a 2020 2020  Item(text)..    
+00006c40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006c50: 2e74 6578 7473 2e72 656d 6f76 6528 7465  .texts.remove(te
+00006c60: 7874 290d 0a0d 0a20 2020 2064 6566 2075  xt)....    def u
+00006c70: 7064 6174 655f 7465 7874 2873 656c 662c  pdate_text(self,
+00006c80: 2074 6578 7429 3a0d 0a20 2020 2020 2020   text):..       
+00006c90: 2068 3020 3d20 7465 7874 2e73 6567 6d65   h0 = text.segme
+00006ca0: 6e74 2e68 616e 646c 6573 5b30 5d5b 2769  nt.handles[0]['i
+00006cb0: 7465 6d27 5d0d 0a20 2020 2020 2020 2068  tem']..        h
+00006cc0: 3120 3d20 7465 7874 2e73 6567 6d65 6e74  1 = text.segment
+00006cd0: 2e68 616e 646c 6573 5b31 5d5b 2769 7465  .handles[1]['ite
+00006ce0: 6d27 5d0d 0a20 2020 2020 2020 2064 6966  m']..        dif
+00006cf0: 6620 3d20 6831 2e70 6f73 2829 202d 2068  f = h1.pos() - h
+00006d00: 302e 706f 7328 290d 0a20 2020 2020 2020  0.pos()..       
+00006d10: 2069 6620 6469 6666 2e79 2829 203c 2030   if diff.y() < 0
+00006d20: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00006d30: 6578 742e 7365 7441 6e63 686f 7228 2830  ext.setAnchor((0
+00006d40: 2e35 2c30 2929 0d0a 2020 2020 2020 2020  .5,0))..        
+00006d50: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00006d60: 2020 2074 6578 742e 7365 7441 6e63 686f     text.setAncho
+00006d70: 7228 2830 2e35 2c31 2929 0d0a 2020 2020  r((0.5,1))..    
+00006d80: 2020 2020 7465 7874 2e73 6574 506f 7328      text.setPos(
+00006d90: 6831 2e70 6f73 2829 290d 0a20 2020 2020  h1.pos())..     
+00006da0: 2020 2074 6578 742e 7365 7454 6578 7428     text.setText(
+00006db0: 5f64 7261 775f 6c69 6e65 5f73 6567 6d65  _draw_line_segme
+00006dc0: 6e74 5f74 6578 7428 7365 6c66 2c20 7465  nt_text(self, te
+00006dd0: 7874 2e73 6567 6d65 6e74 2c20 6830 2e70  xt.segment, h0.p
+00006de0: 6f73 2829 2c20 6831 2e70 6f73 2829 2929  os(), h1.pos()))
+00006df0: 0d0a 0d0a 2020 2020 6465 6620 7570 6461  ....    def upda
+00006e00: 7465 5f74 6578 7473 2873 656c 6629 3a0d  te_texts(self):.
+00006e10: 0a20 2020 2020 2020 2066 6f72 2074 6578  .        for tex
+00006e20: 7420 696e 2073 656c 662e 7465 7874 733a  t in self.texts:
+00006e30: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00006e40: 6c66 2e75 7064 6174 655f 7465 7874 2874  lf.update_text(t
+00006e50: 6578 7429 0d0a 0d0a 2020 2020 6465 6620  ext)....    def 
+00006e60: 6d6f 7665 506f 696e 7428 7365 6c66 2c20  movePoint(self, 
+00006e70: 6861 6e64 6c65 2c20 706f 732c 206d 6f64  handle, pos, mod
+00006e80: 6966 6965 7273 3d51 7443 6f72 652e 5174  ifiers=QtCore.Qt
+00006e90: 2e4b 6579 626f 6172 644d 6f64 6966 6965  .KeyboardModifie
+00006ea0: 722c 2066 696e 6973 683d 5472 7565 2c20  r, finish=True, 
+00006eb0: 636f 6f72 6473 3d27 7061 7265 6e74 2729  coords='parent')
+00006ec0: 3a0d 0a20 2020 2020 2020 2073 7570 6572  :..        super
+00006ed0: 2829 2e6d 6f76 6550 6f69 6e74 2868 616e  ().movePoint(han
+00006ee0: 646c 652c 2070 6f73 2c20 6d6f 6469 6669  dle, pos, modifi
+00006ef0: 6572 732c 2066 696e 6973 682c 2063 6f6f  ers, finish, coo
+00006f00: 7264 7329 0d0a 2020 2020 2020 2020 7365  rds)..        se
+00006f10: 6c66 2e75 7064 6174 655f 7465 7874 7328  lf.update_texts(
+00006f20: 290d 0a0d 0a20 2020 2064 6566 2073 6567  )....    def seg
+00006f30: 6d65 6e74 436c 6963 6b65 6428 7365 6c66  mentClicked(self
+00006f40: 2c20 7365 676d 656e 742c 2065 763d 4e6f  , segment, ev=No
+00006f50: 6e65 2c20 706f 733d 4e6f 6e65 293a 0d0a  ne, pos=None):..
+00006f60: 2020 2020 2020 2020 706f 7320 3d20 7365          pos = se
+00006f70: 676d 656e 742e 6d61 7054 6f50 6172 656e  gment.mapToParen
+00006f80: 7428 6576 2e70 6f73 2829 290d 0a20 2020  t(ev.pos())..   
+00006f90: 2020 2020 2070 6f73 203d 205f 636c 616d       pos = _clam
+00006fa0: 705f 706f 696e 7428 7365 6c66 2e76 622e  p_point(self.vb.
+00006fb0: 7061 7265 6e74 2829 2c20 706f 7329 0d0a  parent(), pos)..
+00006fc0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00006fd0: 7365 676d 656e 7443 6c69 636b 6564 2873  segmentClicked(s
+00006fe0: 6567 6d65 6e74 2c20 706f 733d 706f 7329  egment, pos=pos)
+00006ff0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00007000: 7064 6174 655f 7465 7874 7328 290d 0a0d  pdate_texts()...
+00007010: 0a20 2020 2064 6566 2061 6464 4861 6e64  .    def addHand
+00007020: 6c65 2873 656c 662c 2069 6e66 6f2c 2069  le(self, info, i
+00007030: 6e64 6578 3d4e 6f6e 6529 3a0d 0a20 2020  ndex=None):..   
+00007040: 2020 2020 2068 616e 646c 6520 3d20 7375       handle = su
+00007050: 7065 7228 292e 6164 6448 616e 646c 6528  per().addHandle(
+00007060: 696e 666f 2c20 696e 6465 7829 0d0a 2020  info, index)..  
+00007070: 2020 2020 2020 6861 6e64 6c65 2e6d 6f76        handle.mov
+00007080: 6550 6f69 6e74 203d 2070 6172 7469 616c  ePoint = partial
+00007090: 285f 726f 6968 616e 646c 655f 6d6f 7665  (_roihandle_move
+000070a0: 5f73 6e61 702c 2073 656c 662e 7662 2c20  _snap, self.vb, 
+000070b0: 6861 6e64 6c65 2e6d 6f76 6550 6f69 6e74  handle.movePoint
+000070c0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000070d0: 6e20 6861 6e64 6c65 0d0a 0d0a 0d0a 636c  n handle......cl
+000070e0: 6173 7320 4669 6e4c 696e 6528 7067 2e47  ass FinLine(pg.G
+000070f0: 7261 7068 6963 734f 626a 6563 7429 3a0d  raphicsObject):.
+00007100: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00007110: 5f28 7365 6c66 2c20 706f 696e 7473 2c20  _(self, points, 
+00007120: 7065 6e29 3a0d 0a20 2020 2020 2020 2073  pen):..        s
+00007130: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00007140: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007150: 706f 696e 7473 203d 2070 6f69 6e74 730d  points = points.
+00007160: 0a20 2020 2020 2020 2073 656c 662e 7065  .        self.pe
+00007170: 6e20 3d20 7065 6e0d 0a0d 0a20 2020 2064  n = pen....    d
+00007180: 6566 2070 6169 6e74 2873 656c 662c 2070  ef paint(self, p
+00007190: 2c20 2a61 7267 7329 3a0d 0a20 2020 2020  , *args):..     
+000071a0: 2020 2070 2e73 6574 5065 6e28 7365 6c66     p.setPen(self
+000071b0: 2e70 656e 290d 0a20 2020 2020 2020 2070  .pen)..        p
+000071c0: 2e64 7261 7750 6174 6828 7365 6c66 2e73  .drawPath(self.s
+000071d0: 6861 7065 2829 290d 0a0d 0a20 2020 2064  hape())....    d
+000071e0: 6566 2073 6861 7065 2873 656c 6629 3a0d  ef shape(self):.
+000071f0: 0a20 2020 2020 2020 2070 203d 2051 7447  .        p = QtG
+00007200: 7569 2e51 5061 696e 7465 7250 6174 6828  ui.QPainterPath(
+00007210: 290d 0a20 2020 2020 2020 2070 2e6d 6f76  )..        p.mov
+00007220: 6554 6f28 2a73 656c 662e 706f 696e 7473  eTo(*self.points
+00007230: 5b30 5d29 0d0a 2020 2020 2020 2020 702e  [0])..        p.
+00007240: 6c69 6e65 546f 282a 7365 6c66 2e70 6f69  lineTo(*self.poi
+00007250: 6e74 735b 315d 290d 0a20 2020 2020 2020  nts[1])..       
+00007260: 2072 6574 7572 6e20 700d 0a0d 0a20 2020   return p....   
+00007270: 2064 6566 2062 6f75 6e64 696e 6752 6563   def boundingRec
+00007280: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
+00007290: 2020 7265 7475 726e 2073 656c 662e 7368    return self.sh
+000072a0: 6170 6528 292e 626f 756e 6469 6e67 5265  ape().boundingRe
+000072b0: 6374 2829 0d0a 0d0a 0d0a 636c 6173 7320  ct()......class 
+000072c0: 4669 6e45 6c6c 6970 7365 2870 672e 456c  FinEllipse(pg.El
+000072d0: 6c69 7073 6552 4f49 293a 0d0a 2020 2020  lipseROI):..    
+000072e0: 6465 6620 6164 6452 6f74 6174 6548 616e  def addRotateHan
+000072f0: 646c 6528 7365 6c66 2c20 2a61 7267 732c  dle(self, *args,
+00007300: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+00007310: 2020 2020 2070 6173 730d 0a0d 0a0d 0a63       pass......c
+00007320: 6c61 7373 2046 696e 5265 6374 2870 672e  lass FinRect(pg.
+00007330: 5265 6374 524f 4929 3a0d 0a20 2020 2064  RectROI):..    d
+00007340: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00007350: 2c20 6178 2c20 6272 7573 682c 202a 6172  , ax, brush, *ar
+00007360: 6773 2c20 2a2a 6b77 6172 6773 293a 0d0a  gs, **kwargs):..
+00007370: 2020 2020 2020 2020 7365 6c66 2e61 7820          self.ax 
+00007380: 3d20 6178 0d0a 2020 2020 2020 2020 7365  = ax..        se
+00007390: 6c66 2e62 7275 7368 203d 2062 7275 7368  lf.brush = brush
+000073a0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+000073b0: 292e 5f5f 696e 6974 5f5f 282a 6172 6773  ).__init__(*args
+000073c0: 2c20 2a2a 6b77 6172 6773 290d 0a0d 0a20  , **kwargs).... 
+000073d0: 2020 2064 6566 2070 6169 6e74 2873 656c     def paint(sel
+000073e0: 662c 2070 2c20 2a61 7267 7329 3a0d 0a20  f, p, *args):.. 
+000073f0: 2020 2020 2020 2072 203d 2051 7443 6f72         r = QtCor
+00007400: 652e 5152 6563 7446 2830 2c20 302c 2073  e.QRectF(0, 0, s
+00007410: 656c 662e 7374 6174 655b 2773 697a 6527  elf.state['size'
+00007420: 5d5b 305d 2c20 7365 6c66 2e73 7461 7465  ][0], self.state
+00007430: 5b27 7369 7a65 275d 5b31 5d29 2e6e 6f72  ['size'][1]).nor
+00007440: 6d61 6c69 7a65 6428 290d 0a20 2020 2020  malized()..     
+00007450: 2020 2070 2e73 6574 5065 6e28 7365 6c66     p.setPen(self
+00007460: 2e63 7572 7265 6e74 5065 6e29 0d0a 2020  .currentPen)..  
+00007470: 2020 2020 2020 702e 7365 7442 7275 7368        p.setBrush
+00007480: 2873 656c 662e 6272 7573 6829 0d0a 2020  (self.brush)..  
+00007490: 2020 2020 2020 702e 7472 616e 736c 6174        p.translat
+000074a0: 6528 722e 6c65 6674 2829 2c20 722e 746f  e(r.left(), r.to
+000074b0: 7028 2929 0d0a 2020 2020 2020 2020 702e  p())..        p.
+000074c0: 7363 616c 6528 722e 7769 6474 6828 292c  scale(r.width(),
+000074d0: 2072 2e68 6569 6768 7428 2929 0d0a 2020   r.height())..  
+000074e0: 2020 2020 2020 702e 6472 6177 5265 6374        p.drawRect
+000074f0: 2830 2c20 302c 2031 2c20 3129 0d0a 0d0a  (0, 0, 1, 1)....
+00007500: 2020 2020 6465 6620 6164 6453 6361 6c65      def addScale
+00007510: 4861 6e64 6c65 2873 656c 662c 202a 6172  Handle(self, *ar
+00007520: 6773 2c20 2a2a 6b77 6172 6773 293a 0d0a  gs, **kwargs):..
+00007530: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007540: 7265 7369 7a61 626c 653a 0d0a 2020 2020  resizable:..    
+00007550: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00007560: 6164 6453 6361 6c65 4861 6e64 6c65 282a  addScaleHandle(*
+00007570: 6172 6773 2c20 2a2a 6b77 6172 6773 290d  args, **kwargs).
+00007580: 0a0d 0a0d 0a63 6c61 7373 2046 696e 5669  .....class FinVi
+00007590: 6577 426f 7828 7067 2e56 6965 7742 6f78  ewBox(pg.ViewBox
+000075a0: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
+000075b0: 6974 5f5f 2873 656c 662c 2077 696e 2c20  it__(self, win, 
+000075c0: 696e 6974 5f73 7465 7073 3d33 3030 2c20  init_steps=300, 
+000075d0: 7973 6361 6c65 3d59 5363 616c 6528 276c  yscale=YScale('l
+000075e0: 696e 6561 7227 2c20 3129 2c20 765f 7a6f  inear', 1), v_zo
+000075f0: 6f6d 5f73 6361 6c65 3d31 2c20 2a61 7267  om_scale=1, *arg
+00007600: 732c 202a 2a6b 7761 7267 7329 3a0d 0a20  s, **kwargs):.. 
+00007610: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+00007620: 5f69 6e69 745f 5f28 2a61 7267 732c 202a  _init__(*args, *
+00007630: 2a6b 7761 7267 7329 0d0a 2020 2020 2020  *kwargs)..      
+00007640: 2020 7365 6c66 2e77 696e 203d 2077 696e    self.win = win
+00007650: 0d0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
+00007660: 6e69 745f 7374 6570 7320 3d20 696e 6974  nit_steps = init
+00007670: 5f73 7465 7073 0d0a 2020 2020 2020 2020  _steps..        
+00007680: 7365 6c66 2e79 7363 616c 6520 3d20 7973  self.yscale = ys
+00007690: 6361 6c65 0d0a 2020 2020 2020 2020 7365  cale..        se
+000076a0: 6c66 2e76 5f7a 6f6f 6d5f 7363 616c 6520  lf.v_zoom_scale 
+000076b0: 3d20 765f 7a6f 6f6d 5f73 6361 6c65 0d0a  = v_zoom_scale..
+000076c0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+000076d0: 7465 725f 7669 6577 626f 7820 3d20 4e6f  ter_viewbox = No
+000076e0: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
+000076f0: 2e72 6f69 7320 3d20 5b5d 0d0a 2020 2020  .rois = []..    
+00007700: 2020 2020 7365 6c66 2e77 696e 2e5f 6973      self.win._is
+00007710: 4d6f 7573 654c 6566 7444 7261 6720 3d20  MouseLeftDrag = 
+00007720: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
+00007730: 656c 662e 7265 7365 7428 290d 0a0d 0a20  elf.reset().... 
+00007740: 2020 2064 6566 2072 6573 6574 2873 656c     def reset(sel
+00007750: 6629 3a0d 0a20 2020 2020 2020 2073 656c  f):..        sel
+00007760: 662e 765f 7a6f 6f6d 5f62 6173 656c 696e  f.v_zoom_baselin
+00007770: 6520 3d20 302e 350d 0a20 2020 2020 2020  e = 0.5..       
+00007780: 2073 656c 662e 765f 6175 746f 7a6f 6f6d   self.v_autozoom
+00007790: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+000077a0: 2073 656c 662e 6d61 785f 7a6f 6f6d 5f70   self.max_zoom_p
+000077b0: 6f69 6e74 735f 6620 3d20 310d 0a20 2020  oints_f = 1..   
+000077c0: 2020 2020 2073 656c 662e 795f 6d61 7820       self.y_max 
+000077d0: 3d20 3130 3030 0d0a 2020 2020 2020 2020  = 1000..        
+000077e0: 7365 6c66 2e79 5f6d 696e 203d 2030 0d0a  self.y_min = 0..
+000077f0: 2020 2020 2020 2020 7365 6c66 2e79 5f70          self.y_p
+00007800: 6f73 6974 6976 6520 3d20 5472 7565 0d0a  ositive = True..
+00007810: 2020 2020 2020 2020 7365 6c66 2e78 5f69          self.x_i
+00007820: 6e64 6578 6564 203d 2054 7275 650d 0a20  ndexed = True.. 
+00007830: 2020 2020 2020 2073 656c 662e 666f 7263         self.forc
+00007840: 655f 7261 6e67 655f 7570 6461 7465 203d  e_range_update =
+00007850: 2030 0d0a 2020 2020 2020 2020 7768 696c   0..        whil
+00007860: 6520 7365 6c66 2e72 6f69 733a 0d0a 2020  e self.rois:..  
+00007870: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00007880: 656d 6f76 655f 6c61 7374 5f72 6f69 2829  emove_last_roi()
+00007890: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+000078a0: 7261 775f 6c69 6e65 203d 204e 6f6e 650d  raw_line = None.
+000078b0: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
+000078c0: 6177 696e 6720 3d20 4661 6c73 650d 0a20  awing = False.. 
+000078d0: 2020 2020 2020 2073 656c 662e 7374 616e         self.stan
+000078e0: 6461 6c6f 6e65 7320 3d20 7365 7428 290d  dalones = set().
+000078f0: 0a20 2020 2020 2020 2073 656c 662e 7570  .        self.up
+00007900: 6461 7469 6e67 5f6c 696e 6b65 6420 3d20  dating_linked = 
+00007910: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
+00007920: 656c 662e 7365 745f 6461 7461 7372 6328  elf.set_datasrc(
+00007930: 4e6f 6e65 290d 0a20 2020 2020 2020 2073  None)..        s
+00007940: 656c 662e 7365 744d 6f75 7365 456e 6162  elf.setMouseEnab
+00007950: 6c65 6428 783d 5472 7565 2c20 793d 4661  led(x=True, y=Fa
+00007960: 6c73 6529 0d0a 2020 2020 2020 2020 7365  lse)..        se
+00007970: 6c66 2e73 6574 5261 6e67 6528 5174 436f  lf.setRange(QtCo
+00007980: 7265 2e51 5265 6374 4628 7067 2e50 6f69  re.QRectF(pg.Poi
+00007990: 6e74 2830 2c20 3029 2c20 7067 2e50 6f69  nt(0, 0), pg.Poi
+000079a0: 6e74 2831 2c20 3129 2929 0d0a 0d0a 2020  nt(1, 1)))....  
+000079b0: 2020 6465 6620 7365 745f 6461 7461 7372    def set_datasr
+000079c0: 6328 7365 6c66 2c20 6461 7461 7372 6329  c(self, datasrc)
+000079d0: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+000079e0: 6461 7461 7372 6320 3d20 6461 7461 7372  datasrc = datasr
+000079f0: 630d 0a20 2020 2020 2020 2069 6620 6e6f  c..        if no
+00007a00: 7420 7365 6c66 2e64 6174 6173 7263 3a0d  t self.datasrc:.
+00007a10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007a20: 7572 6e0d 0a20 2020 2020 2020 2064 6174  urn..        dat
+00007a30: 6173 7263 2e75 7064 6174 655f 696e 6974  asrc.update_init
+00007a40: 5f78 2873 656c 662e 696e 6974 5f73 7465  _x(self.init_ste
+00007a50: 7073 290d 0a0d 0a20 2020 2064 6566 2070  ps)....    def p
+00007a60: 7265 5f70 726f 6365 7373 5f64 6174 6128  re_process_data(
+00007a70: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00007a80: 6966 2073 656c 662e 6461 7461 7372 6320  if self.datasrc 
+00007a90: 616e 6420 7365 6c66 2e64 6174 6173 7263  and self.datasrc
+00007aa0: 2e73 6361 6c65 5f63 6f6c 733a 0d0a 2020  .scale_cols:..  
+00007ab0: 2020 2020 2020 2020 2020 6466 203d 2073            df = s
+00007ac0: 656c 662e 6461 7461 7372 632e 6466 2e69  elf.datasrc.df.i
+00007ad0: 6c6f 635b 3a2c 2073 656c 662e 6461 7461  loc[:, self.data
+00007ae0: 7372 632e 7363 616c 655f 636f 6c73 5d0d  src.scale_cols].
+00007af0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007b00: 662e 795f 6d61 7820 3d20 6466 2e6d 6178  f.y_max = df.max
+00007b10: 2829 2e6d 6178 2829 0d0a 2020 2020 2020  ().max()..      
+00007b20: 2020 2020 2020 7365 6c66 2e79 5f6d 696e        self.y_min
+00007b30: 203d 2064 662e 6d69 6e28 292e 6d69 6e28   = df.min().min(
+00007b40: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00007b50: 6620 7365 6c66 2e79 5f6d 696e 203c 3d20  f self.y_min <= 
+00007b60: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00007b70: 2020 2020 7365 6c66 2e79 5f70 6f73 6974      self.y_posit
+00007b80: 6976 6520 3d20 4661 6c73 650d 0a0d 0a20  ive = False.... 
+00007b90: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+00007ba0: 2020 6465 6620 6461 7461 7372 635f 6f72    def datasrc_or
+00007bb0: 5f73 7461 6e64 616c 6f6e 6528 7365 6c66  _standalone(self
+00007bc0: 293a 0d0a 2020 2020 2020 2020 6473 203d  ):..        ds =
+00007bd0: 2073 656c 662e 6461 7461 7372 630d 0a20   self.datasrc.. 
+00007be0: 2020 2020 2020 2069 6620 6e6f 7420 6473         if not ds
+00007bf0: 2061 6e64 2073 656c 662e 7374 616e 6461   and self.standa
+00007c00: 6c6f 6e65 733a 0d0a 2020 2020 2020 2020  lones:..        
+00007c10: 2020 2020 6473 203d 206e 6578 7428 6974      ds = next(it
+00007c20: 6572 2873 656c 662e 7374 616e 6461 6c6f  er(self.standalo
+00007c30: 6e65 7329 290d 0a20 2020 2020 2020 2072  nes))..        r
+00007c40: 6574 7572 6e20 6473 0d0a 0d0a 2020 2020  eturn ds....    
+00007c50: 6465 6620 7768 6565 6c45 7665 6e74 2873  def wheelEvent(s
+00007c60: 656c 662c 2065 762c 2061 7869 733d 4e6f  elf, ev, axis=No
+00007c70: 6e65 293a 0d0a 2020 2020 2020 2020 6966  ne):..        if
+00007c80: 2073 656c 662e 6d61 7374 6572 5f76 6965   self.master_vie
+00007c90: 7762 6f78 3a0d 0a20 2020 2020 2020 2020  wbox:..         
+00007ca0: 2020 2072 6574 7572 6e20 7365 6c66 2e6d     return self.m
+00007cb0: 6173 7465 725f 7669 6577 626f 782e 7768  aster_viewbox.wh
+00007cc0: 6565 6c45 7665 6e74 2865 762c 2061 7869  eelEvent(ev, axi
+00007cd0: 733d 6178 6973 290d 0a20 2020 2020 2020  s=axis)..       
+00007ce0: 2069 6620 6576 2e6d 6f64 6966 6965 7273   if ev.modifiers
+00007cf0: 2829 203d 3d20 5174 436f 7265 2e51 742e  () == QtCore.Qt.
+00007d00: 4b65 7962 6f61 7264 4d6f 6469 6669 6572  KeyboardModifier
+00007d10: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
+00007d20: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00007d30: 6361 6c65 5f66 6163 7420 3d20 310d 0a20  cale_fact = 1.. 
+00007d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007d50: 765f 7a6f 6f6d 5f73 6361 6c65 202f 3d20  v_zoom_scale /= 
+00007d60: 312e 3032 202a 2a20 2865 762e 6465 6c74  1.02 ** (ev.delt
+00007d70: 6128 2920 2a20 7365 6c66 2e73 7461 7465  a() * self.state
+00007d80: 5b27 7768 6565 6c53 6361 6c65 4661 6374  ['wheelScaleFact
+00007d90: 6f72 275d 290d 0a20 2020 2020 2020 2065  or'])..        e
+00007da0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00007db0: 2020 7363 616c 655f 6661 6374 203d 2031    scale_fact = 1
+00007dc0: 2e30 3220 2a2a 2028 6576 2e64 656c 7461  .02 ** (ev.delta
+00007dd0: 2829 202a 2073 656c 662e 7374 6174 655b  () * self.state[
+00007de0: 2777 6865 656c 5363 616c 6546 6163 746f  'wheelScaleFacto
+00007df0: 7227 5d29 0d0a 2020 2020 2020 2020 7672  r'])..        vr
+00007e00: 203d 2073 656c 662e 7461 7267 6574 5265   = self.targetRe
+00007e10: 6374 2829 0d0a 2020 2020 2020 2020 6365  ct()..        ce
+00007e20: 6e74 6572 203d 2073 656c 662e 6d61 7054  nter = self.mapT
+00007e30: 6f56 6965 7728 6576 2e73 6365 6e65 506f  oView(ev.scenePo
+00007e40: 7328 2929 0d0a 2020 2020 2020 2020 7063  s())..        pc
+00007e50: 745f 7820 3d20 2863 656e 7465 722e 7828  t_x = (center.x(
+00007e60: 292d 7672 2e6c 6566 7428 2929 202f 2076  )-vr.left()) / v
+00007e70: 722e 7769 6474 6828 290d 0a20 2020 2020  r.width()..     
+00007e80: 2020 2069 6620 7063 745f 7820 3c20 302e     if pct_x < 0.
+00007e90: 3035 3a20 2320 7a6f 6f6d 2074 6f20 6661  05: # zoom to fa
+00007ea0: 7220 6c65 6674 203d 3e20 616c 6c20 7468  r left => all th
+00007eb0: 6520 7761 7920 6c65 6674 0d0a 2020 2020  e way left..    
+00007ec0: 2020 2020 2020 2020 6365 6e74 6572 203d          center =
+00007ed0: 2070 672e 506f 696e 7428 7672 2e6c 6566   pg.Point(vr.lef
+00007ee0: 7428 292c 2063 656e 7465 722e 7928 2929  t(), center.y())
+00007ef0: 0d0a 2020 2020 2020 2020 656c 6966 2070  ..        elif p
+00007f00: 6374 5f78 203e 2030 2e39 353a 2023 207a  ct_x > 0.95: # z
+00007f10: 6f6f 6d20 746f 2066 6172 2072 6967 6874  oom to far right
+00007f20: 203d 3e20 616c 6c20 7468 6520 7761 7920   => all the way 
+00007f30: 7269 6768 740d 0a20 2020 2020 2020 2020  right..         
+00007f40: 2020 2063 656e 7465 7220 3d20 7067 2e50     center = pg.P
+00007f50: 6f69 6e74 2876 722e 7269 6768 7428 292c  oint(vr.right(),
+00007f60: 2063 656e 7465 722e 7928 2929 0d0a 2020   center.y())..  
+00007f70: 2020 2020 2020 7365 6c66 2e7a 6f6f 6d5f        self.zoom_
+00007f80: 7265 6374 2876 722c 2073 6361 6c65 5f66  rect(vr, scale_f
+00007f90: 6163 742c 2063 656e 7465 7229 0d0a 2020  act, center)..  
+00007fa0: 2020 2020 2020 2320 7570 6461 7465 2063        # update c
+00007fb0: 726f 7373 6861 6972 0d0a 2020 2020 2020  rosshair..      
+00007fc0: 2020 5f6d 6f75 7365 5f6d 6f76 6564 2873    _mouse_moved(s
+00007fd0: 656c 662e 7769 6e2c 2073 656c 662c 204e  elf.win, self, N
+00007fe0: 6f6e 6529 0d0a 2020 2020 2020 2020 6576  one)..        ev
+00007ff0: 2e61 6363 6570 7428 290d 0a0d 0a20 2020  .accept()....   
+00008000: 2064 6566 206d 6f75 7365 4472 6167 4576   def mouseDragEv
+00008010: 656e 7428 7365 6c66 2c20 6576 2c20 6178  ent(self, ev, ax
+00008020: 6973 3d4e 6f6e 6529 3a0d 0a20 2020 2020  is=None):..     
+00008030: 2020 2061 7869 7320 3d20 3020 2320 646f     axis = 0 # do
+00008040: 6e27 7420 636f 6e73 7472 6169 6e20 6472  n't constrain dr
+00008050: 6167 2064 6972 6563 7469 6f6e 0d0a 2020  ag direction..  
+00008060: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
+00008070: 7374 6572 5f76 6965 7762 6f78 3a0d 0a20  ster_viewbox:.. 
+00008080: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00008090: 6e20 7365 6c66 2e6d 6173 7465 725f 7669  n self.master_vi
+000080a0: 6577 626f 782e 6d6f 7573 6544 7261 6745  ewbox.mouseDragE
+000080b0: 7665 6e74 2865 762c 2061 7869 733d 6178  vent(ev, axis=ax
+000080c0: 6973 290d 0a20 2020 2020 2020 2069 6620  is)..        if 
+000080d0: 6e6f 7420 7365 6c66 2e64 6174 6173 7263  not self.datasrc
+000080e0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000080f0: 6574 7572 6e0d 0a20 2020 2020 2020 2069  eturn..        i
+00008100: 6620 6576 2e62 7574 746f 6e28 2920 3d3d  f ev.button() ==
+00008110: 2051 7443 6f72 652e 5174 2e4d 6f75 7365   QtCore.Qt.Mouse
+00008120: 4275 7474 6f6e 2e4c 6566 7442 7574 746f  Button.LeftButto
+00008130: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
+00008140: 7365 6c66 2e6d 6f75 7365 4c65 6674 4472  self.mouseLeftDr
+00008150: 6167 2865 762c 2061 7869 7329 0d0a 2020  ag(ev, axis)..  
+00008160: 2020 2020 2020 656c 6966 2065 762e 6275        elif ev.bu
+00008170: 7474 6f6e 2829 203d 3d20 5174 436f 7265  tton() == QtCore
+00008180: 2e51 742e 4d6f 7573 6542 7574 746f 6e2e  .Qt.MouseButton.
+00008190: 4d69 6464 6c65 4275 7474 6f6e 3a0d 0a20  MiddleButton:.. 
+000081a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000081b0: 6d6f 7573 654d 6964 646c 6544 7261 6728  mouseMiddleDrag(
+000081c0: 6576 2c20 6178 6973 290d 0a20 2020 2020  ev, axis)..     
+000081d0: 2020 2065 6c69 6620 6576 2e62 7574 746f     elif ev.butto
+000081e0: 6e28 2920 3d3d 2051 7443 6f72 652e 5174  n() == QtCore.Qt
+000081f0: 2e4d 6f75 7365 4275 7474 6f6e 2e52 6967  .MouseButton.Rig
+00008200: 6874 4275 7474 6f6e 3a0d 0a20 2020 2020  htButton:..     
+00008210: 2020 2020 2020 2073 656c 662e 6d6f 7573         self.mous
+00008220: 6552 6967 6874 4472 6167 2865 762c 2061  eRightDrag(ev, a
+00008230: 7869 7329 0d0a 2020 2020 2020 2020 656c  xis)..        el
+00008240: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00008250: 2073 7570 6572 2829 2e6d 6f75 7365 4472   super().mouseDr
+00008260: 6167 4576 656e 7428 6576 2c20 6178 6973  agEvent(ev, axis
+00008270: 290d 0a0d 0a20 2020 2064 6566 206d 6f75  )....    def mou
+00008280: 7365 4c65 6674 4472 6167 2873 656c 662c  seLeftDrag(self,
+00008290: 2065 762c 2061 7869 7329 3a0d 0a20 2020   ev, axis):..   
+000082a0: 2020 2020 2027 2727 4374 726c 2b4c 4275       '''Ctrl+LBu
+000082b0: 7474 6f6e 2064 7261 7720 6c69 6e65 732e  tton draw lines.
+000082c0: 2727 270d 0a20 2020 2020 2020 2069 6620  '''..        if 
+000082d0: 6576 2e6d 6f64 6966 6965 7273 2829 2021  ev.modifiers() !
+000082e0: 3d20 5174 436f 7265 2e51 742e 4b65 7962  = QtCore.Qt.Keyb
+000082f0: 6f61 7264 4d6f 6469 6669 6572 2e43 6f6e  oardModifier.Con
+00008300: 7472 6f6c 4d6f 6469 6669 6572 3a0d 0a20  trolModifier:.. 
+00008310: 2020 2020 2020 2020 2020 2073 7570 6572             super
+00008320: 2829 2e6d 6f75 7365 4472 6167 4576 656e  ().mouseDragEven
+00008330: 7428 6576 2c20 6178 6973 290d 0a20 2020  t(ev, axis)..   
+00008340: 2020 2020 2020 2020 2069 6620 6576 2e69           if ev.i
+00008350: 7346 696e 6973 6828 293a 0d0a 2020 2020  sFinish():..    
+00008360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008370: 2e77 696e 2e5f 6973 4d6f 7573 654c 6566  .win._isMouseLef
+00008380: 7444 7261 6720 3d20 4661 6c73 650d 0a20  tDrag = False.. 
+00008390: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000083a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000083b0: 2020 7365 6c66 2e77 696e 2e5f 6973 4d6f    self.win._isMo
+000083c0: 7573 654c 6566 7444 7261 6720 3d20 5472  useLeftDrag = Tr
+000083d0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+000083e0: 6966 2065 762e 6973 4669 6e69 7368 2829  if ev.isFinish()
+000083f0: 206f 7220 7365 6c66 2e64 7261 7769 6e67   or self.drawing
+00008400: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00008410: 2020 2073 656c 662e 7265 6672 6573 685f     self.refresh_
+00008420: 616c 6c5f 795f 7a6f 6f6d 2829 0d0a 2020  all_y_zoom()..  
+00008430: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00008440: 2073 656c 662e 6472 6177 696e 673a 0d0a   self.drawing:..
+00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008460: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
+00008470: 6966 2073 656c 662e 6472 6177 5f6c 696e  if self.draw_lin
+00008480: 6520 616e 6420 6e6f 7420 7365 6c66 2e64  e and not self.d
+00008490: 7261 7769 6e67 3a0d 0a20 2020 2020 2020  rawing:..       
+000084a0: 2020 2020 2073 656c 662e 7365 745f 6472       self.set_dr
+000084b0: 6177 5f6c 696e 655f 636f 6c6f 7228 6472  aw_line_color(dr
+000084c0: 6177 5f64 6f6e 655f 636f 6c6f 7229 0d0a  aw_done_color)..
+000084d0: 2020 2020 2020 2020 7031 203d 2073 656c          p1 = sel
+000084e0: 662e 6d61 7054 6f56 6965 7728 6576 2e70  f.mapToView(ev.p
+000084f0: 6f73 2829 290d 0a20 2020 2020 2020 2070  os())..        p
+00008500: 3120 3d20 5f63 6c61 6d70 5f70 6f69 6e74  1 = _clamp_point
+00008510: 2873 656c 662e 7061 7265 6e74 2829 2c20  (self.parent(), 
+00008520: 7031 290d 0a20 2020 2020 2020 2069 6620  p1)..        if 
+00008530: 6e6f 7420 7365 6c66 2e64 7261 7769 6e67  not self.drawing
+00008540: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00008550: 2061 6464 206e 6577 206c 696e 650d 0a20   add new line.. 
+00008560: 2020 2020 2020 2020 2020 2070 3020 3d20             p0 = 
+00008570: 7365 6c66 2e6d 6170 546f 5669 6577 2865  self.mapToView(e
+00008580: 762e 6c61 7374 506f 7328 2929 0d0a 2020  v.lastPos())..  
+00008590: 2020 2020 2020 2020 2020 7030 203d 205f            p0 = _
+000085a0: 636c 616d 705f 706f 696e 7428 7365 6c66  clamp_point(self
+000085b0: 2e70 6172 656e 7428 292c 2070 3029 0d0a  .parent(), p0)..
+000085c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000085d0: 2e64 7261 775f 6c69 6e65 203d 2046 696e  .draw_line = Fin
+000085e0: 506f 6c79 4c69 6e65 2873 656c 662c 205b  PolyLine(self, [
+000085f0: 7030 2c20 7031 5d2c 2063 6c6f 7365 643d  p0, p1], closed=
+00008600: 4661 6c73 652c 2070 656e 3d70 672e 6d6b  False, pen=pg.mk
+00008610: 5065 6e28 6472 6177 5f6c 696e 655f 636f  Pen(draw_line_co
+00008620: 6c6f 7229 2c20 6d6f 7661 626c 653d 4661  lor), movable=Fa
+00008630: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
+00008640: 2020 7365 6c66 2e64 7261 775f 6c69 6e65    self.draw_line
+00008650: 2e73 6574 5a56 616c 7565 2834 3029 0d0a  .setZValue(40)..
+00008660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008670: 2e72 6f69 732e 6170 7065 6e64 2873 656c  .rois.append(sel
+00008680: 662e 6472 6177 5f6c 696e 6529 0d0a 2020  f.draw_line)..  
+00008690: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000086a0: 6464 4974 656d 2873 656c 662e 6472 6177  ddItem(self.draw
+000086b0: 5f6c 696e 6529 0d0a 2020 2020 2020 2020  _line)..        
+000086c0: 2020 2020 7365 6c66 2e64 7261 7769 6e67      self.drawing
+000086d0: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+000086e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000086f0: 2020 2020 2320 6472 6177 2070 6c61 6365      # draw place
+00008700: 6420 706f 696e 7420 6174 2065 6e64 206f  d point at end o
+00008710: 6620 706f 6c79 2d6c 696e 650d 0a20 2020  f poly-line..   
+00008720: 2020 2020 2020 2020 2073 656c 662e 6472           self.dr
+00008730: 6177 5f6c 696e 652e 6d6f 7665 506f 696e  aw_line.movePoin
+00008740: 7428 2d31 2c20 7031 290d 0a20 2020 2020  t(-1, p1)..     
+00008750: 2020 2069 6620 6576 2e69 7346 696e 6973     if ev.isFinis
+00008760: 6828 293a 0d0a 2020 2020 2020 2020 2020  h():..          
+00008770: 2020 7365 6c66 2e64 7261 7769 6e67 203d    self.drawing =
+00008780: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+00008790: 6576 2e61 6363 6570 7428 290d 0a0d 0a20  ev.accept().... 
+000087a0: 2020 2064 6566 206d 6f75 7365 4d69 6464     def mouseMidd
+000087b0: 6c65 4472 6167 2873 656c 662c 2065 762c  leDrag(self, ev,
+000087c0: 2061 7869 7329 3a0d 0a20 2020 2020 2020   axis):..       
+000087d0: 2027 2727 4374 726c 2b4d 4275 7474 6f6e   '''Ctrl+MButton
+000087e0: 2064 7261 7720 656c 6c69 7073 6573 2e27   draw ellipses.'
+000087f0: 2727 0d0a 2020 2020 2020 2020 6966 2065  ''..        if e
+00008800: 762e 6d6f 6469 6669 6572 7328 2920 213d  v.modifiers() !=
+00008810: 2051 7443 6f72 652e 5174 2e4b 6579 626f   QtCore.Qt.Keybo
+00008820: 6172 644d 6f64 6966 6965 722e 436f 6e74  ardModifier.Cont
+00008830: 726f 6c4d 6f64 6966 6965 723a 0d0a 2020  rolModifier:..  
+00008840: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008850: 2073 7570 6572 2829 2e6d 6f75 7365 4472   super().mouseDr
+00008860: 6167 4576 656e 7428 6576 2c20 6178 6973  agEvent(ev, axis
+00008870: 290d 0a20 2020 2020 2020 2070 3120 3d20  )..        p1 = 
+00008880: 7365 6c66 2e6d 6170 546f 5669 6577 2865  self.mapToView(e
+00008890: 762e 706f 7328 2929 0d0a 2020 2020 2020  v.pos())..      
+000088a0: 2020 7031 203d 205f 636c 616d 705f 706f    p1 = _clamp_po
+000088b0: 696e 7428 7365 6c66 2e70 6172 656e 7428  int(self.parent(
+000088c0: 292c 2070 3129 0d0a 2020 2020 2020 2020  ), p1)..        
+000088d0: 6465 6620 6e6f 6e7a 6572 6f73 697a 6528  def nonzerosize(
+000088e0: 612c 2062 293a 0d0a 2020 2020 2020 2020  a, b):..        
+000088f0: 2020 2020 6320 3d20 622d 610d 0a20 2020      c = b-a..   
+00008900: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008910: 7067 2e50 6f69 6e74 2861 6273 2863 2e78  pg.Point(abs(c.x
+00008920: 2829 2920 6f72 2031 2c20 6162 7328 632e  ()) or 1, abs(c.
+00008930: 7928 2929 206f 7220 3165 2d33 290d 0a20  y()) or 1e-3).. 
+00008940: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00008950: 6c66 2e64 7261 7769 6e67 3a0d 0a20 2020  lf.drawing:..   
+00008960: 2020 2020 2020 2020 2023 2061 6464 206e           # add n
+00008970: 6577 2065 6c6c 6970 7365 0d0a 2020 2020  ew ellipse..    
+00008980: 2020 2020 2020 2020 7030 203d 2073 656c          p0 = sel
+00008990: 662e 6d61 7054 6f56 6965 7728 6576 2e6c  f.mapToView(ev.l
+000089a0: 6173 7450 6f73 2829 290d 0a20 2020 2020  astPos())..     
+000089b0: 2020 2020 2020 2070 3020 3d20 5f63 6c61         p0 = _cla
+000089c0: 6d70 5f70 6f69 6e74 2873 656c 662e 7061  mp_point(self.pa
+000089d0: 7265 6e74 2829 2c20 7030 290d 0a20 2020  rent(), p0)..   
+000089e0: 2020 2020 2020 2020 2073 203d 206e 6f6e           s = non
+000089f0: 7a65 726f 7369 7a65 2870 302c 2070 3129  zerosize(p0, p1)
+00008a00: 0d0a 2020 2020 2020 2020 2020 2020 7030  ..            p0
+00008a10: 203d 2051 7443 6f72 652e 5150 6f69 6e74   = QtCore.QPoint
+00008a20: 4628 7030 2e78 2829 2d73 2e78 2829 2f32  F(p0.x()-s.x()/2
+00008a30: 2c20 7030 2e79 2829 2d73 2e79 2829 2f32  , p0.y()-s.y()/2
+00008a40: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00008a50: 656c 662e 6472 6177 5f65 6c6c 6970 7365  elf.draw_ellipse
+00008a60: 203d 2046 696e 456c 6c69 7073 6528 7030   = FinEllipse(p0
+00008a70: 2c20 732c 2070 656e 3d70 672e 6d6b 5065  , s, pen=pg.mkPe
+00008a80: 6e28 6472 6177 5f6c 696e 655f 636f 6c6f  n(draw_line_colo
+00008a90: 7229 2c20 6d6f 7661 626c 653d 5472 7565  r), movable=True
+00008aa0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00008ab0: 656c 662e 6472 6177 5f65 6c6c 6970 7365  elf.draw_ellipse
+00008ac0: 2e73 6574 5a56 616c 7565 2838 3029 0d0a  .setZValue(80)..
+00008ad0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008ae0: 2e72 6f69 732e 6170 7065 6e64 2873 656c  .rois.append(sel
+00008af0: 662e 6472 6177 5f65 6c6c 6970 7365 290d  f.draw_ellipse).
+00008b00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008b10: 662e 6164 6449 7465 6d28 7365 6c66 2e64  f.addItem(self.d
+00008b20: 7261 775f 656c 6c69 7073 6529 0d0a 2020  raw_ellipse)..  
+00008b30: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00008b40: 7261 7769 6e67 203d 2054 7275 650d 0a20  rawing = True.. 
+00008b50: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00008b60: 2020 2020 2020 2020 2020 6320 3d20 7365            c = se
+00008b70: 6c66 2e64 7261 775f 656c 6c69 7073 652e  lf.draw_ellipse.
+00008b80: 706f 7328 2920 2b20 7365 6c66 2e64 7261  pos() + self.dra
+00008b90: 775f 656c 6c69 7073 652e 7369 7a65 2829  w_ellipse.size()
+00008ba0: 2a30 2e35 0d0a 2020 2020 2020 2020 2020  *0.5..          
+00008bb0: 2020 7320 3d20 6e6f 6e7a 6572 6f73 697a    s = nonzerosiz
+00008bc0: 6528 632c 2070 3129 0d0a 2020 2020 2020  e(c, p1)..      
+00008bd0: 2020 2020 2020 7365 6c66 2e64 7261 775f        self.draw_
+00008be0: 656c 6c69 7073 652e 7365 7453 697a 6528  ellipse.setSize(
+00008bf0: 732a 322c 2075 7064 6174 653d 4661 6c73  s*2, update=Fals
+00008c00: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00008c10: 7365 6c66 2e64 7261 775f 656c 6c69 7073  self.draw_ellips
+00008c20: 652e 7365 7450 6f73 2863 2d73 290d 0a20  e.setPos(c-s).. 
+00008c30: 2020 2020 2020 2069 6620 6576 2e69 7346         if ev.isF
+00008c40: 696e 6973 6828 293a 0d0a 2020 2020 2020  inish():..      
+00008c50: 2020 2020 2020 7365 6c66 2e64 7261 7769        self.drawi
+00008c60: 6e67 203d 2046 616c 7365 0d0a 2020 2020  ng = False..    
+00008c70: 2020 2020 6576 2e61 6363 6570 7428 290d      ev.accept().
+00008c80: 0a0d 0a20 2020 2064 6566 206d 6f75 7365  ...    def mouse
+00008c90: 5269 6768 7444 7261 6728 7365 6c66 2c20  RightDrag(self, 
+00008ca0: 6576 2c20 6178 6973 293a 0d0a 2020 2020  ev, axis):..    
+00008cb0: 2020 2020 2727 2752 4275 7474 6f6e 2069      '''RButton i
+00008cc0: 7320 626f 7820 7a6f 6f6d 2e20 4174 206c  s box zoom. At l
+00008cd0: 6561 7374 2066 6f72 206e 6f77 2e27 2727  east for now.'''
+00008ce0: 0d0a 2020 2020 2020 2020 6576 2e61 6363  ..        ev.acc
+00008cf0: 6570 7428 290d 0a20 2020 2020 2020 2069  ept()..        i
+00008d00: 6620 6e6f 7420 6576 2e69 7346 696e 6973  f not ev.isFinis
+00008d10: 6828 293a 0d0a 2020 2020 2020 2020 2020  h():..          
+00008d20: 2020 7365 6c66 2e75 7064 6174 6553 6361    self.updateSca
+00008d30: 6c65 426f 7828 6576 2e62 7574 746f 6e44  leBox(ev.buttonD
+00008d40: 6f77 6e50 6f73 2829 2c20 6576 2e70 6f73  ownPos(), ev.pos
+00008d50: 2829 290d 0a20 2020 2020 2020 2065 6c73  ())..        els
+00008d60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00008d70: 7365 6c66 2e72 6253 6361 6c65 426f 782e  self.rbScaleBox.
+00008d80: 6869 6465 2829 0d0a 2020 2020 2020 2020  hide()..        
+00008d90: 2020 2020 6178 203d 2051 7443 6f72 652e      ax = QtCore.
+00008da0: 5152 6563 7446 2870 672e 506f 696e 7428  QRectF(pg.Point(
+00008db0: 6576 2e62 7574 746f 6e44 6f77 6e50 6f73  ev.buttonDownPos
+00008dc0: 2865 762e 6275 7474 6f6e 2829 2929 2c20  (ev.button())), 
+00008dd0: 7067 2e50 6f69 6e74 2865 762e 706f 7328  pg.Point(ev.pos(
+00008de0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+00008df0: 2061 7820 3d20 7365 6c66 2e63 6869 6c64   ax = self.child
+00008e00: 4772 6f75 702e 6d61 7052 6563 7446 726f  Group.mapRectFro
+00008e10: 6d50 6172 656e 7428 6178 290d 0a20 2020  mParent(ax)..   
+00008e20: 2020 2020 2020 2020 2069 6620 6178 2e77           if ax.w
+00008e30: 6964 7468 2829 203c 2032 3a20 2320 7a6f  idth() < 2: # zo
+00008e40: 6f6d 696e 6720 7468 6973 206e 6172 726f  oming this narro
+00008e50: 7720 6973 2070 726f 6261 626c 7920 6120  w is probably a 
+00008e60: 6d69 7374 616b 650d 0a20 2020 2020 2020  mistake..       
+00008e70: 2020 2020 2020 2020 2061 782e 6164 6a75           ax.adju
+00008e80: 7374 282d 312c 2030 2c20 2b31 2c20 3029  st(-1, 0, +1, 0)
+00008e90: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00008ea0: 6c66 2e73 686f 7741 7852 6563 7428 6178  lf.showAxRect(ax
+00008eb0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00008ec0: 656c 662e 6178 4869 7374 6f72 7950 6f69  elf.axHistoryPoi
+00008ed0: 6e74 6572 202b 3d20 310d 0a20 2020 2020  nter += 1..     
+00008ee0: 2020 2020 2020 2073 656c 662e 6178 4869         self.axHi
+00008ef0: 7374 6f72 7920 3d20 7365 6c66 2e61 7848  story = self.axH
+00008f00: 6973 746f 7279 5b3a 7365 6c66 2e61 7848  istory[:self.axH
+00008f10: 6973 746f 7279 506f 696e 7465 725d 202b  istoryPointer] +
+00008f20: 205b 6178 5d0d 0a0d 0a20 2020 2064 6566   [ax]....    def
+00008f30: 206d 6f75 7365 436c 6963 6b45 7665 6e74   mouseClickEvent
+00008f40: 2873 656c 662c 2065 7629 3a0d 0a20 2020  (self, ev):..   
+00008f50: 2020 2020 2069 6620 7365 6c66 2e6d 6173       if self.mas
+00008f60: 7465 725f 7669 6577 626f 783a 0d0a 2020  ter_viewbox:..  
+00008f70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008f80: 2073 656c 662e 6d61 7374 6572 5f76 6965   self.master_vie
+00008f90: 7762 6f78 2e6d 6f75 7365 436c 6963 6b45  wbox.mouseClickE
+00008fa0: 7665 6e74 2865 7629 0d0a 2020 2020 2020  vent(ev)..      
+00008fb0: 2020 6966 205f 6d6f 7573 655f 636c 6963    if _mouse_clic
+00008fc0: 6b65 6428 7365 6c66 2c20 6576 293a 0d0a  ked(self, ev):..
+00008fd0: 2020 2020 2020 2020 2020 2020 6576 2e61              ev.a
+00008fe0: 6363 6570 7428 290d 0a20 2020 2020 2020  ccept()..       
+00008ff0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00009000: 2020 2020 2069 6620 6576 2e62 7574 746f       if ev.butto
+00009010: 6e28 2920 213d 2051 7443 6f72 652e 5174  n() != QtCore.Qt
+00009020: 2e4d 6f75 7365 4275 7474 6f6e 2e4c 6566  .MouseButton.Lef
+00009030: 7442 7574 746f 6e20 6f72 2065 762e 6d6f  tButton or ev.mo
+00009040: 6469 6669 6572 7328 2920 213d 2051 7443  difiers() != QtC
+00009050: 6f72 652e 5174 2e4b 6579 626f 6172 644d  ore.Qt.KeyboardM
+00009060: 6f64 6966 6965 722e 436f 6e74 726f 6c4d  odifier.ControlM
+00009070: 6f64 6966 6965 7220 6f72 206e 6f74 2073  odifier or not s
+00009080: 656c 662e 6472 6177 5f6c 696e 653a 0d0a  elf.draw_line:..
+00009090: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000090a0: 726e 2073 7570 6572 2829 2e6d 6f75 7365  rn super().mouse
+000090b0: 436c 6963 6b45 7665 6e74 2865 7629 0d0a  ClickEvent(ev)..
+000090c0: 2020 2020 2020 2020 2320 6164 6420 616e          # add an
+000090d0: 6f74 6865 7220 7365 676d 656e 7420 746f  other segment to
+000090e0: 2074 6865 2063 7572 7265 6e74 6c79 2064   the currently d
+000090f0: 7261 776e 206c 696e 650d 0a20 2020 2020  rawn line..     
+00009100: 2020 2070 203d 2073 656c 662e 6d61 7043     p = self.mapC
+00009110: 6c69 636b 546f 5669 6577 2865 762e 706f  lickToView(ev.po
+00009120: 7328 2929 0d0a 2020 2020 2020 2020 7020  s())..        p 
+00009130: 3d20 5f63 6c61 6d70 5f70 6f69 6e74 2873  = _clamp_point(s
+00009140: 656c 662e 7061 7265 6e74 2829 2c20 7029  elf.parent(), p)
+00009150: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00009160: 7070 656e 645f 6472 6177 5f73 6567 6d65  ppend_draw_segme
+00009170: 6e74 2870 290d 0a20 2020 2020 2020 2073  nt(p)..        s
+00009180: 656c 662e 6472 6177 696e 6720 3d20 4661  elf.drawing = Fa
+00009190: 6c73 650d 0a20 2020 2020 2020 2065 762e  lse..        ev.
+000091a0: 6163 6365 7074 2829 0d0a 0d0a 2020 2020  accept()....    
+000091b0: 6465 6620 6d61 7043 6c69 636b 546f 5669  def mapClickToVi
+000091c0: 6577 2873 656c 662c 2070 6f73 293a 0d0a  ew(self, pos):..
+000091d0: 2020 2020 2020 2020 2727 276d 6170 546f          '''mapTo
+000091e0: 5669 6577 2829 2064 6f65 7320 6e6f 7420  View() does not 
+000091f0: 646f 2067 7269 6473 2070 726f 7065 726c  do grids properl
+00009200: 7920 696e 2065 6d62 6564 6465 6420 7769  y in embedded wi
+00009210: 6467 6574 732e 2053 7472 616e 6765 6c79  dgets. Strangely
+00009220: 2c20 6f6e 6c79 2061 6666 6563 7420 636c  , only affect cl
+00009230: 6963 6b73 2c20 6e6f 7420 6472 6167 732e  icks, not drags.
+00009240: 2727 270d 0a20 2020 2020 2020 2069 6620  '''..        if 
+00009250: 7365 6c66 2e77 696e 2e70 6172 656e 7428  self.win.parent(
+00009260: 2920 6973 206e 6f74 204e 6f6e 653a 0d0a  ) is not None:..
+00009270: 2020 2020 2020 2020 2020 2020 6178 203d              ax =
+00009280: 2073 656c 662e 7061 7265 6e74 2829 0d0a   self.parent()..
+00009290: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+000092a0: 782e 6765 7441 7869 7328 2772 6967 6874  x.getAxis('right
+000092b0: 2729 2e67 7269 643a 0d0a 2020 2020 2020  ').grid:..      
+000092c0: 2020 2020 2020 2020 2020 706f 732e 7365            pos.se
+000092d0: 7458 2870 6f73 2e78 2829 202b 2073 656c  tX(pos.x() + sel
+000092e0: 662e 7769 6474 6828 2929 0d0a 2020 2020  f.width())..    
+000092f0: 2020 2020 2020 2020 656c 6966 2061 782e          elif ax.
+00009300: 6765 7441 7869 7328 2762 6f74 746f 6d27  getAxis('bottom'
+00009310: 292e 6772 6964 3a0d 0a20 2020 2020 2020  ).grid:..       
+00009320: 2020 2020 2020 2020 2070 6f73 2e73 6574           pos.set
+00009330: 5928 706f 732e 7928 2920 2b20 7365 6c66  Y(pos.y() + self
+00009340: 2e68 6569 6768 7428 2929 0d0a 2020 2020  .height())..    
+00009350: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00009360: 2829 2e6d 6170 546f 5669 6577 2870 6f73  ().mapToView(pos
+00009370: 290d 0a0d 0a20 2020 2064 6566 206b 6579  )....    def key
+00009380: 5072 6573 7345 7665 6e74 2873 656c 662c  PressEvent(self,
+00009390: 2065 7629 3a0d 0a20 2020 2020 2020 2069   ev):..        i
+000093a0: 6620 7365 6c66 2e6d 6173 7465 725f 7669  f self.master_vi
+000093b0: 6577 626f 783a 0d0a 2020 2020 2020 2020  ewbox:..        
+000093c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000093d0: 6d61 7374 6572 5f76 6965 7762 6f78 2e6b  master_viewbox.k
+000093e0: 6579 5072 6573 7345 7665 6e74 2865 7629  eyPressEvent(ev)
+000093f0: 0d0a 2020 2020 2020 2020 6966 205f 6b65  ..        if _ke
+00009400: 795f 7072 6573 7365 6428 7365 6c66 2c20  y_pressed(self, 
+00009410: 6576 293a 0d0a 2020 2020 2020 2020 2020  ev):..          
+00009420: 2020 6576 2e61 6363 6570 7428 290d 0a20    ev.accept().. 
+00009430: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009440: 6e0d 0a20 2020 2020 2020 2073 7570 6572  n..        super
+00009450: 2829 2e6b 6579 5072 6573 7345 7665 6e74  ().keyPressEvent
+00009460: 2865 7629 0d0a 0d0a 2020 2020 6465 6620  (ev)....    def 
+00009470: 6c69 6e6b 6564 5669 6577 4368 616e 6765  linkedViewChange
+00009480: 6428 7365 6c66 2c20 7669 6577 2c20 6178  d(self, view, ax
+00009490: 6973 293a 0d0a 2020 2020 2020 2020 6966  is):..        if
+000094a0: 206e 6f74 2073 656c 662e 6461 7461 7372   not self.datasr
+000094b0: 6320 6f72 2073 656c 662e 7570 6461 7469  c or self.updati
+000094c0: 6e67 5f6c 696e 6b65 643a 0d0a 2020 2020  ng_linked:..    
+000094d0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+000094e0: 2020 2020 2020 2020 6966 2076 6965 7720          if view 
+000094f0: 616e 6420 7365 6c66 2e64 6174 6173 7263  and self.datasrc
+00009500: 2061 6e64 2076 6965 772e 6461 7461 7372   and view.datasr
+00009510: 633a 0d0a 2020 2020 2020 2020 2020 2020  c:..            
+00009520: 7365 6c66 2e75 7064 6174 696e 675f 6c69  self.updating_li
+00009530: 6e6b 6564 203d 2054 7275 650d 0a20 2020  nked = True..   
+00009540: 2020 2020 2020 2020 2074 7220 3d20 7365           tr = se
+00009550: 6c66 2e74 6172 6765 7452 6563 7428 290d  lf.targetRect().
+00009560: 0a20 2020 2020 2020 2020 2020 2076 7220  .            vr 
+00009570: 3d20 7669 6577 2e74 6172 6765 7452 6563  = view.targetRec
+00009580: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+00009590: 2069 735f 6469 7274 7920 3d20 7669 6577   is_dirty = view
+000095a0: 2e66 6f72 6365 5f72 616e 6765 5f75 7064  .force_range_upd
+000095b0: 6174 6520 3e20 300d 0a20 2020 2020 2020  ate > 0..       
+000095c0: 2020 2020 2069 735f 7361 6d65 5f73 6361       is_same_sca
+000095d0: 6c65 203d 2073 656c 662e 6461 7461 7372  le = self.datasr
+000095e0: 632e 786c 656e 203d 3d20 7669 6577 2e64  c.xlen == view.d
+000095f0: 6174 6173 7263 2e78 6c65 6e0d 0a20 2020  atasrc.xlen..   
+00009600: 2020 2020 2020 2020 2069 6620 6973 5f73           if is_s
+00009610: 616d 655f 7363 616c 653a 2023 2073 7461  ame_scale: # sta
+00009620: 626c 6520 7a6f 6f6d 2062 6173 6564 206f  ble zoom based o
+00009630: 6e20 696e 6465 780d 0a20 2020 2020 2020  n index..       
+00009640: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
+00009650: 6972 7479 206f 7220 6162 7328 7672 2e6c  irty or abs(vr.l
+00009660: 6566 7428 292d 7472 2e6c 6566 7428 2929  eft()-tr.left())
+00009670: 203e 3d20 3120 6f72 2061 6273 2876 722e   >= 1 or abs(vr.
+00009680: 7269 6768 7428 292d 7472 2e72 6967 6874  right()-tr.right
+00009690: 2829 2920 3e3d 2031 3a0d 0a20 2020 2020  ()) >= 1:..     
+000096a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000096b0: 6620 6973 5f64 6972 7479 3a0d 0a20 2020  f is_dirty:..   
+000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096d0: 2020 2020 2076 6965 772e 666f 7263 655f       view.force_
+000096e0: 7261 6e67 655f 7570 6461 7465 202d 3d20  range_update -= 
+000096f0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+00009700: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+00009710: 7465 5f79 5f7a 6f6f 6d28 7672 2e6c 6566  te_y_zoom(vr.lef
+00009720: 7428 292c 2076 722e 7269 6768 7428 2929  t(), vr.right())
+00009730: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00009740: 7365 3a20 2320 736c 6f70 7079 206f 6e65  se: # sloppy one
+00009750: 2062 6173 6564 206f 6e20 7469 6d65 2073   based on time s
+00009760: 7461 6d70 730d 0a20 2020 2020 2020 2020  tamps..         
+00009770: 2020 2020 2020 2074 7430 2c74 7431 2c5f         tt0,tt1,_
+00009780: 2c5f 2c5f 203d 2073 656c 662e 6461 7461  ,_,_ = self.data
+00009790: 7372 632e 6869 6c6f 2874 722e 6c65 6674  src.hilo(tr.left
+000097a0: 2829 2c20 7472 2e72 6967 6874 2829 290d  (), tr.right()).
+000097b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000097c0: 2076 7430 2c76 7431 2c5f 2c5f 2c5f 203d   vt0,vt1,_,_,_ =
+000097d0: 2076 6965 772e 6461 7461 7372 632e 6869   view.datasrc.hi
+000097e0: 6c6f 2876 722e 6c65 6674 2829 2c20 7672  lo(vr.left(), vr
+000097f0: 2e72 6967 6874 2829 290d 0a20 2020 2020  .right())..     
+00009800: 2020 2020 2020 2020 2020 2070 6572 696f             perio
+00009810: 6432 203d 2073 656c 662e 6461 7461 7372  d2 = self.datasr
+00009820: 632e 7065 7269 6f64 5f6e 7320 2a20 302e  c.period_ns * 0.
+00009830: 350d 0a20 2020 2020 2020 2020 2020 2020  5..             
+00009840: 2020 2069 6620 6973 5f64 6972 7479 206f     if is_dirty o
+00009850: 7220 6162 7328 7674 302d 7474 3029 203e  r abs(vt0-tt0) >
+00009860: 3d20 7065 7269 6f64 3220 6f72 2061 6273  = period2 or abs
+00009870: 2876 7431 2d74 7431 2920 3e3d 2070 6572  (vt1-tt1) >= per
+00009880: 696f 6432 3a0d 0a20 2020 2020 2020 2020  iod2:..         
+00009890: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000098a0: 5f64 6972 7479 3a0d 0a20 2020 2020 2020  _dirty:..       
+000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098c0: 2076 6965 772e 666f 7263 655f 7261 6e67   view.force_rang
+000098d0: 655f 7570 6461 7465 202d 3d20 310d 0a20  e_update -= 1.. 
+000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098f0: 2020 2069 6620 7365 6c66 2e70 6172 656e     if self.paren
+00009900: 7428 293a 0d0a 2020 2020 2020 2020 2020  t():..          
+00009910: 2020 2020 2020 2020 2020 2020 2020 7830                x0
+00009920: 2c78 3120 3d20 5f70 6474 696d 6532 696e  ,x1 = _pdtime2in
+00009930: 6465 7828 7365 6c66 2e70 6172 656e 7428  dex(self.parent(
+00009940: 292c 2070 642e 5365 7269 6573 285b 7674  ), pd.Series([vt
+00009950: 302c 7674 315d 292c 2061 6e79 5f65 6e64  0,vt1]), any_end
+00009960: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009980: 7365 6c66 2e75 7064 6174 655f 795f 7a6f  self.update_y_zo
+00009990: 6f6d 2878 302c 2078 3129 0d0a 2020 2020  om(x0, x1)..    
+000099a0: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
+000099b0: 6174 696e 675f 6c69 6e6b 6564 203d 2046  ating_linked = F
+000099c0: 616c 7365 0d0a 0d0a 2020 2020 6465 6620  alse....    def 
+000099d0: 7a6f 6f6d 5f72 6563 7428 7365 6c66 2c20  zoom_rect(self, 
+000099e0: 7672 2c20 7363 616c 655f 6661 6374 2c20  vr, scale_fact, 
+000099f0: 6365 6e74 6572 293a 0d0a 2020 2020 2020  center):..      
+00009a00: 2020 6966 206e 6f74 2073 656c 662e 6461    if not self.da
+00009a10: 7461 7372 633a 0d0a 2020 2020 2020 2020  tasrc:..        
+00009a20: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
+00009a30: 2020 2020 7830 203d 2063 656e 7465 722e      x0 = center.
+00009a40: 7828 2920 2b20 2876 722e 6c65 6674 2829  x() + (vr.left()
+00009a50: 2d63 656e 7465 722e 7828 2929 202a 2073  -center.x()) * s
+00009a60: 6361 6c65 5f66 6163 740d 0a20 2020 2020  cale_fact..     
+00009a70: 2020 2078 3120 3d20 6365 6e74 6572 2e78     x1 = center.x
+00009a80: 2829 202b 2028 7672 2e72 6967 6874 2829  () + (vr.right()
+00009a90: 2d63 656e 7465 722e 7828 2929 202a 2073  -center.x()) * s
+00009aa0: 6361 6c65 5f66 6163 740d 0a20 2020 2020  cale_fact..     
+00009ab0: 2020 2073 656c 662e 7570 6461 7465 5f79     self.update_y
+00009ac0: 5f7a 6f6f 6d28 7830 2c20 7831 290d 0a0d  _zoom(x0, x1)...
+00009ad0: 0a20 2020 2064 6566 2070 616e 5f78 2873  .    def pan_x(s
+00009ae0: 656c 662c 2073 7465 7073 3d4e 6f6e 652c  elf, steps=None,
+00009af0: 2070 6572 6365 6e74 3d4e 6f6e 6529 3a0d   percent=None):.
+00009b00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00009b10: 2e64 6174 6173 7263 2069 7320 4e6f 6e65  .datasrc is None
+00009b20: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00009b30: 6574 7572 6e0d 0a20 2020 2020 2020 2069  eturn..        i
+00009b40: 6620 7374 6570 7320 6973 204e 6f6e 653a  f steps is None:
+00009b50: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00009b60: 6570 7320 3d20 696e 7428 7065 7263 656e  eps = int(percen
+00009b70: 742f 3130 302a 7365 6c66 2e74 6172 6765  t/100*self.targe
+00009b80: 7452 6563 7428 292e 7769 6474 6828 2929  tRect().width())
+00009b90: 0d0a 2020 2020 2020 2020 7472 203d 2073  ..        tr = s
+00009ba0: 656c 662e 7461 7267 6574 5265 6374 2829  elf.targetRect()
+00009bb0: 0d0a 2020 2020 2020 2020 7831 203d 2074  ..        x1 = t
+00009bc0: 722e 7269 6768 7428 2920 2b20 7374 6570  r.right() + step
+00009bd0: 730d 0a20 2020 2020 2020 2073 7461 7274  s..        start
+00009be0: 7820 3d20 2d73 6964 655f 6d61 7267 696e  x = -side_margin
+00009bf0: 0d0a 2020 2020 2020 2020 656e 6478 203d  ..        endx =
+00009c00: 2073 656c 662e 6461 7461 7372 632e 786c   self.datasrc.xl
+00009c10: 656e 202b 2072 6967 6874 5f6d 6172 6769  en + right_margi
+00009c20: 6e5f 6361 6e64 6c65 7320 2d20 7369 6465  n_candles - side
+00009c30: 5f6d 6172 6769 6e0d 0a20 2020 2020 2020  _margin..       
+00009c40: 2069 6620 7831 203e 2065 6e64 783a 0d0a   if x1 > endx:..
+00009c50: 2020 2020 2020 2020 2020 2020 7831 203d              x1 =
+00009c60: 2065 6e64 780d 0a20 2020 2020 2020 2078   endx..        x
+00009c70: 3020 3d20 7831 202d 2074 722e 7769 6474  0 = x1 - tr.widt
+00009c80: 6828 290d 0a20 2020 2020 2020 2069 6620  h()..        if 
+00009c90: 7830 203c 2073 7461 7274 783a 0d0a 2020  x0 < startx:..  
+00009ca0: 2020 2020 2020 2020 2020 7830 203d 2073            x0 = s
+00009cb0: 7461 7274 780d 0a20 2020 2020 2020 2020  tartx..         
+00009cc0: 2020 2078 3120 3d20 7830 202b 2074 722e     x1 = x0 + tr.
+00009cd0: 7769 6474 6828 290d 0a20 2020 2020 2020  width()..       
+00009ce0: 2073 656c 662e 7570 6461 7465 5f79 5f7a   self.update_y_z
+00009cf0: 6f6f 6d28 7830 2c20 7831 290d 0a0d 0a20  oom(x0, x1).... 
+00009d00: 2020 2064 6566 2072 6566 7265 7368 5f61     def refresh_a
+00009d10: 6c6c 5f79 5f7a 6f6f 6d28 7365 6c66 293a  ll_y_zoom(self):
+00009d20: 0d0a 2020 2020 2020 2020 2727 2754 6869  ..        '''Thi
+00009d30: 7320 7570 6461 7465 7320 5920 7a6f 6f6d  s updates Y zoom
+00009d40: 206f 6e20 616c 6c20 7669 6577 732c 2073   on all views, s
+00009d50: 7563 6820 6173 2077 6865 6e20 6120 6d6f  uch as when a mo
+00009d60: 7573 6520 6472 6167 2069 7320 636f 6d70  use drag is comp
+00009d70: 6c65 7465 642e 2727 270d 0a20 2020 2020  leted.'''..     
+00009d80: 2020 206d 6169 6e5f 7662 203d 2073 656c     main_vb = sel
+00009d90: 660d 0a20 2020 2020 2020 2069 6620 7365  f..        if se
+00009da0: 6c66 2e6c 696e 6b65 6456 6965 7728 3029  lf.linkedView(0)
+00009db0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00009dc0: 656c 662e 666f 7263 655f 7261 6e67 655f  elf.force_range_
+00009dd0: 7570 6461 7465 203d 2031 2023 206d 6169  update = 1 # mai
+00009de0: 6e20 6e65 6564 2074 6f20 7570 6461 7465  n need to update
+00009df0: 206f 6e6c 7920 6f6e 6365 2074 6f20 7573   only once to us
+00009e00: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+00009e10: 696e 5f76 6220 3d20 6c69 7374 2873 656c  in_vb = list(sel
+00009e20: 662e 7769 6e2e 6178 7329 5b30 5d2e 7662  f.win.axs)[0].vb
+00009e30: 0d0a 2020 2020 2020 2020 6d61 696e 5f76  ..        main_v
+00009e40: 622e 666f 7263 655f 7261 6e67 655f 7570  b.force_range_up
+00009e50: 6461 7465 203d 206c 656e 2873 656c 662e  date = len(self.
+00009e60: 7769 6e2e 6178 7329 2d31 2023 2075 7064  win.axs)-1 # upd
+00009e70: 6174 6520 6d61 696e 2061 7320 6d61 6e79  ate main as many
+00009e80: 2074 696d 6573 2061 7320 7468 6572 6520   times as there 
+00009e90: 6172 6520 6f74 6865 7220 726f 7773 0d0a  are other rows..
+00009ea0: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
+00009eb0: 6174 655f 795f 7a6f 6f6d 2829 0d0a 2020  ate_y_zoom()..  
+00009ec0: 2020 2020 2020 2320 7265 6672 6573 6820        # refresh 
+00009ed0: 6372 6f73 7368 6169 7220 7768 656e 2064  crosshair when d
+00009ee0: 6f6e 650d 0a20 2020 2020 2020 205f 6d6f  one..        _mo
+00009ef0: 7573 655f 6d6f 7665 6428 7365 6c66 2e77  use_moved(self.w
+00009f00: 696e 2c20 7365 6c66 2c20 4e6f 6e65 290d  in, self, None).
+00009f10: 0a0d 0a20 2020 2064 6566 2075 7064 6174  ...    def updat
+00009f20: 655f 795f 7a6f 6f6d 2873 656c 662c 2078  e_y_zoom(self, x
+00009f30: 303d 4e6f 6e65 2c20 7831 3d4e 6f6e 6529  0=None, x1=None)
+00009f40: 3a0d 0a20 2020 2020 2020 2064 6174 6173  :..        datas
+00009f50: 7263 203d 2073 656c 662e 6461 7461 7372  rc = self.datasr
+00009f60: 635f 6f72 5f73 7461 6e64 616c 6f6e 650d  c_or_standalone.
+00009f70: 0a20 2020 2020 2020 2069 6620 6461 7461  .        if data
+00009f80: 7372 6320 6973 204e 6f6e 653a 0d0a 2020  src is None:..  
+00009f90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009fa0: 0d0a 2020 2020 2020 2020 6966 2078 3020  ..        if x0 
+00009fb0: 6973 204e 6f6e 6520 6f72 2078 3120 6973  is None or x1 is
+00009fc0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00009fd0: 2020 2020 7472 203d 2073 656c 662e 7461      tr = self.ta
+00009fe0: 7267 6574 5265 6374 2829 0d0a 2020 2020  rgetRect()..    
+00009ff0: 2020 2020 2020 2020 7830 203d 2074 722e          x0 = tr.
+0000a000: 6c65 6674 2829 0d0a 2020 2020 2020 2020  left()..        
+0000a010: 2020 2020 7831 203d 2074 722e 7269 6768      x1 = tr.righ
+0000a020: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+0000a030: 2069 6620 7831 2d78 3020 3c3d 2031 3a0d   if x1-x0 <= 1:.
+0000a040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a050: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
+0000a060: 2023 206d 616b 6520 6564 6765 7320 7269   # make edges ri
+0000a070: 6769 640d 0a20 2020 2020 2020 2078 6c20  gid..        xl 
+0000a080: 3d20 6d61 7828 5f72 6f75 6e64 2878 302d  = max(_round(x0-
+0000a090: 7369 6465 5f6d 6172 6769 6e29 2b73 6964  side_margin)+sid
+0000a0a0: 655f 6d61 7267 696e 2c20 2d73 6964 655f  e_margin, -side_
+0000a0b0: 6d61 7267 696e 290d 0a20 2020 2020 2020  margin)..       
+0000a0c0: 2078 7220 3d20 6d69 6e28 5f72 6f75 6e64   xr = min(_round
+0000a0d0: 2878 312d 7369 6465 5f6d 6172 6769 6e29  (x1-side_margin)
+0000a0e0: 2b73 6964 655f 6d61 7267 696e 2c20 6461  +side_margin, da
+0000a0f0: 7461 7372 632e 786c 656e 2b72 6967 6874  tasrc.xlen+right
+0000a100: 5f6d 6172 6769 6e5f 6361 6e64 6c65 732d  _margin_candles-
+0000a110: 7369 6465 5f6d 6172 6769 6e29 0d0a 2020  side_margin)..  
+0000a120: 2020 2020 2020 6478 6c20 3d20 786c 2d78        dxl = xl-x
+0000a130: 300d 0a20 2020 2020 2020 2064 7872 203d  0..        dxr =
+0000a140: 2078 722d 7831 0d0a 2020 2020 2020 2020   xr-x1..        
+0000a150: 6966 2064 786c 203e 2030 3a0d 0a20 2020  if dxl > 0:..   
+0000a160: 2020 2020 2020 2020 2078 3120 2b3d 2064           x1 += d
+0000a170: 786c 0d0a 2020 2020 2020 2020 6966 2064  xl..        if d
+0000a180: 7872 203c 2030 3a0d 0a20 2020 2020 2020  xr < 0:..       
+0000a190: 2020 2020 2078 3020 2b3d 2064 7872 0d0a       x0 += dxr..
+0000a1a0: 2020 2020 2020 2020 7830 203d 206d 6178          x0 = max
+0000a1b0: 285f 726f 756e 6428 7830 2d73 6964 655f  (_round(x0-side_
+0000a1c0: 6d61 7267 696e 292b 7369 6465 5f6d 6172  margin)+side_mar
+0000a1d0: 6769 6e2c 202d 7369 6465 5f6d 6172 6769  gin, -side_margi
+0000a1e0: 6e29 0d0a 2020 2020 2020 2020 7831 203d  n)..        x1 =
+0000a1f0: 206d 696e 285f 726f 756e 6428 7831 2d73   min(_round(x1-s
+0000a200: 6964 655f 6d61 7267 696e 292b 7369 6465  ide_margin)+side
+0000a210: 5f6d 6172 6769 6e2c 2064 6174 6173 7263  _margin, datasrc
+0000a220: 2e78 6c65 6e2b 7269 6768 745f 6d61 7267  .xlen+right_marg
+0000a230: 696e 5f63 616e 646c 6573 2d73 6964 655f  in_candles-side_
+0000a240: 6d61 7267 696e 290d 0a20 2020 2020 2020  margin)..       
+0000a250: 2023 2066 6574 6368 2068 692d 6c6f 2061   # fetch hi-lo a
+0000a260: 6e64 2073 6574 2072 616e 6765 0d0a 2020  nd set range..  
+0000a270: 2020 2020 2020 5f2c 5f2c 6869 2c6c 6f2c        _,_,hi,lo,
+0000a280: 636e 7420 3d20 6461 7461 7372 632e 6869  cnt = datasrc.hi
+0000a290: 6c6f 2878 302c 2078 3129 0d0a 2020 2020  lo(x0, x1)..    
+0000a2a0: 2020 2020 7672 203d 2073 656c 662e 7669      vr = self.vi
+0000a2b0: 6577 5265 6374 2829 0d0a 2020 2020 2020  ewRect()..      
+0000a2c0: 2020 6d69 6e6c 656e 203d 2069 6e74 2828    minlen = int((
+0000a2d0: 6d61 785f 7a6f 6f6d 5f70 6f69 6e74 732d  max_zoom_points-
+0000a2e0: 302e 3529 202a 2073 656c 662e 6d61 785f  0.5) * self.max_
+0000a2f0: 7a6f 6f6d 5f70 6f69 6e74 735f 6620 2b20  zoom_points_f + 
+0000a300: 302e 3531 290d 0a20 2020 2020 2020 2069  0.51)..        i
+0000a310: 6620 2878 312d 7830 2920 3c20 7672 2e77  f (x1-x0) < vr.w
+0000a320: 6964 7468 2829 2061 6e64 2063 6e74 203c  idth() and cnt <
+0000a330: 206d 696e 6c65 6e3a 0d0a 2020 2020 2020   minlen:..      
+0000a340: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+0000a350: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0000a360: 662e 765f 6175 746f 7a6f 6f6d 3a0d 0a20  f.v_autozoom:.. 
+0000a370: 2020 2020 2020 2020 2020 2068 6920 3d20             hi = 
+0000a380: 7672 2e62 6f74 746f 6d28 290d 0a20 2020  vr.bottom()..   
+0000a390: 2020 2020 2020 2020 206c 6f20 3d20 7672           lo = vr
+0000a3a0: 2e74 6f70 2829 0d0a 2020 2020 2020 2020  .top()..        
+0000a3b0: 6966 2073 656c 662e 7973 6361 6c65 2e73  if self.yscale.s
+0000a3c0: 6361 6c65 7479 7065 203d 3d20 276c 6f67  caletype == 'log
+0000a3d0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
+0000a3e0: 6966 206c 6f20 3c20 303a 0d0a 2020 2020  if lo < 0:..    
+0000a3f0: 2020 2020 2020 2020 2020 2020 6c6f 203d              lo =
+0000a400: 2030 2e30 3520 2a20 7365 6c66 2e79 7363   0.05 * self.ysc
+0000a410: 616c 652e 7363 616c 6566 2023 2073 7472  ale.scalef # str
+0000a420: 616e 6765 2051 5420 6c6f 6720 7363 616c  ange QT log scal
+0000a430: 6520 7265 6e64 6572 696e 672c 2077 6869  e rendering, whi
+0000a440: 6368 2049 276d 2075 6e61 626c 6520 746f  ch I'm unable to
+0000a450: 2063 6f6d 7065 6e73 6174 6520 666f 720d   compensate for.
+0000a460: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000a470: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000a480: 2020 2020 6c6f 203d 206d 6178 2831 652d      lo = max(1e-
+0000a490: 3130 302c 206c 6f29 0d0a 2020 2020 2020  100, lo)..      
+0000a4a0: 2020 2020 2020 726e 6720 3d20 2868 6920        rng = (hi 
+0000a4b0: 2f20 6c6f 2920 2a2a 2028 312f 7365 6c66  / lo) ** (1/self
+0000a4c0: 2e76 5f7a 6f6f 6d5f 7363 616c 6529 0d0a  .v_zoom_scale)..
+0000a4d0: 2020 2020 2020 2020 2020 2020 726e 6720              rng 
+0000a4e0: 3d20 6d69 6e28 726e 672c 2031 6535 3029  = min(rng, 1e50)
+0000a4f0: 2023 2061 766f 6964 2066 6c6f 6174 206f   # avoid float o
+0000a500: 7665 7266 6c6f 770d 0a20 2020 2020 2020  verflow..       
+0000a510: 2020 2020 2062 6173 6520 3d20 2868 692a       base = (hi*
+0000a520: 6c6f 2920 2a2a 2073 656c 662e 765f 7a6f  lo) ** self.v_zo
+0000a530: 6f6d 5f62 6173 656c 696e 650d 0a20 2020  om_baseline..   
+0000a540: 2020 2020 2020 2020 2079 3020 3d20 6261           y0 = ba
+0000a550: 7365 202f 2072 6e67 2a2a 7365 6c66 2e76  se / rng**self.v
+0000a560: 5f7a 6f6f 6d5f 6261 7365 6c69 6e65 0d0a  _zoom_baseline..
+0000a570: 2020 2020 2020 2020 2020 2020 7931 203d              y1 =
+0000a580: 2062 6173 6520 2a20 726e 672a 2a28 312d   base * rng**(1-
+0000a590: 7365 6c66 2e76 5f7a 6f6f 6d5f 6261 7365  self.v_zoom_base
+0000a5a0: 6c69 6e65 290d 0a20 2020 2020 2020 2065  line)..        e
+0000a5b0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0000a5c0: 2020 726e 6720 3d20 2868 692d 6c6f 2920    rng = (hi-lo) 
+0000a5d0: 2f20 7365 6c66 2e76 5f7a 6f6f 6d5f 7363  / self.v_zoom_sc
+0000a5e0: 616c 650d 0a20 2020 2020 2020 2020 2020  ale..           
+0000a5f0: 2072 6e67 203d 206d 6178 2872 6e67 2c20   rng = max(rng, 
+0000a600: 3265 2d37 2920 2320 736f 6d65 2076 6572  2e-7) # some ver
+0000a610: 7920 7765 6972 6420 6275 6720 7768 6572  y weird bug wher
+0000a620: 6520 6869 6768 2f6c 6f77 2065 7870 6f6e  e high/low expon
+0000a630: 656e 7473 2073 746f 7073 2072 656e 6465  ents stops rende
+0000a640: 7269 6e67 0d0a 2020 2020 2020 2020 2020  ring..          
+0000a650: 2020 6261 7365 203d 2028 6869 2b6c 6f29    base = (hi+lo)
+0000a660: 202a 2073 656c 662e 765f 7a6f 6f6d 5f62   * self.v_zoom_b
+0000a670: 6173 656c 696e 650d 0a20 2020 2020 2020  aseline..       
+0000a680: 2020 2020 2079 3020 3d20 6261 7365 202d       y0 = base -
+0000a690: 2072 6e67 2a73 656c 662e 765f 7a6f 6f6d   rng*self.v_zoom
+0000a6a0: 5f62 6173 656c 696e 650d 0a20 2020 2020  _baseline..     
+0000a6b0: 2020 2020 2020 2079 3120 3d20 6261 7365         y1 = base
+0000a6c0: 202b 2072 6e67 2a28 312d 7365 6c66 2e76   + rng*(1-self.v
+0000a6d0: 5f7a 6f6f 6d5f 6261 7365 6c69 6e65 290d  _zoom_baseline).
+0000a6e0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000a6f0: 7365 6c66 2e78 5f69 6e64 6578 6564 3a0d  self.x_indexed:.
+0000a700: 0a20 2020 2020 2020 2020 2020 2078 302c  .            x0,
+0000a710: 7831 203d 205f 786d 696e 6d61 7828 6461  x1 = _xminmax(da
+0000a720: 7461 7372 632c 2078 5f69 6e64 6578 6564  tasrc, x_indexed
+0000a730: 3d46 616c 7365 2c20 6578 7472 615f 6d61  =False, extra_ma
+0000a740: 7267 696e 3d30 290d 0a20 2020 2020 2020  rgin=0)..       
+0000a750: 2072 6574 7572 6e20 7365 6c66 2e73 6574   return self.set
+0000a760: 5f72 616e 6765 2878 302c 2079 302c 2078  _range(x0, y0, x
+0000a770: 312c 2079 3129 0d0a 0d0a 2020 2020 6465  1, y1)....    de
+0000a780: 6620 7365 745f 7261 6e67 6528 7365 6c66  f set_range(self
+0000a790: 2c20 7830 2c20 7930 2c20 7831 2c20 7931  , x0, y0, x1, y1
+0000a7a0: 293a 0d0a 2020 2020 2020 2020 6966 2078  ):..        if x
+0000a7b0: 3020 6973 204e 6f6e 6520 6f72 2078 3120  0 is None or x1 
+0000a7c0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+0000a7d0: 2020 2020 2020 7472 203d 2073 656c 662e        tr = self.
+0000a7e0: 7461 7267 6574 5265 6374 2829 0d0a 2020  targetRect()..  
+0000a7f0: 2020 2020 2020 2020 2020 7830 203d 2074            x0 = t
+0000a800: 722e 6c65 6674 2829 0d0a 2020 2020 2020  r.left()..      
+0000a810: 2020 2020 2020 7831 203d 2074 722e 7269        x1 = tr.ri
+0000a820: 6768 7428 290d 0a20 2020 2020 2020 2069  ght()..        i
+0000a830: 6620 6e70 2e69 736e 616e 2879 3029 206f  f np.isnan(y0) o
+0000a840: 7220 6e70 2e69 736e 616e 2879 3129 3a0d  r np.isnan(y1):.
+0000a850: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000a860: 7572 6e0d 0a20 2020 2020 2020 205f 7930  urn..        _y0
+0000a870: 203d 2073 656c 662e 7973 6361 6c65 2e69   = self.yscale.i
+0000a880: 6e76 7866 6f72 6d28 7930 2c20 7665 7269  nvxform(y0, veri
+0000a890: 6679 3d54 7275 6529 0d0a 2020 2020 2020  fy=True)..      
+0000a8a0: 2020 5f79 3120 3d20 7365 6c66 2e79 7363    _y1 = self.ysc
+0000a8b0: 616c 652e 696e 7678 666f 726d 2879 312c  ale.invxform(y1,
+0000a8c0: 2076 6572 6966 793d 5472 7565 290d 0a20   verify=True).. 
+0000a8d0: 2020 2020 2020 2073 656c 662e 7365 7452         self.setR
+0000a8e0: 616e 6765 2851 7443 6f72 652e 5152 6563  ange(QtCore.QRec
+0000a8f0: 7446 2870 672e 506f 696e 7428 7830 2c20  tF(pg.Point(x0, 
+0000a900: 5f79 3029 2c20 7067 2e50 6f69 6e74 2878  _y0), pg.Point(x
+0000a910: 312c 205f 7931 2929 2c20 7061 6464 696e  1, _y1)), paddin
+0000a920: 673d 3029 0d0a 2020 2020 2020 2020 7265  g=0)..        re
+0000a930: 7475 726e 2054 7275 650d 0a0d 0a20 2020  turn True....   
+0000a940: 2064 6566 2072 656d 6f76 655f 6c61 7374   def remove_last
+0000a950: 5f72 6f69 2873 656c 6629 3a0d 0a20 2020  _roi(self):..   
+0000a960: 2020 2020 2069 6620 7365 6c66 2e72 6f69       if self.roi
+0000a970: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0000a980: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000a990: 6528 7365 6c66 2e72 6f69 735b 2d31 5d2c  e(self.rois[-1],
+0000a9a0: 2070 672e 506f 6c79 4c69 6e65 524f 4929   pg.PolyLineROI)
+0000a9b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000a9c0: 2020 2073 656c 662e 7265 6d6f 7665 4974     self.removeIt
+0000a9d0: 656d 2873 656c 662e 726f 6973 5b2d 315d  em(self.rois[-1]
+0000a9e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a9f0: 2020 2073 656c 662e 726f 6973 203d 2073     self.rois = s
+0000aa00: 656c 662e 726f 6973 5b3a 2d31 5d0d 0a20  elf.rois[:-1].. 
+0000aa10: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000aa20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000aa30: 2020 6820 3d20 7365 6c66 2e72 6f69 735b    h = self.rois[
+0000aa40: 2d31 5d2e 6861 6e64 6c65 735b 2d31 5d5b  -1].handles[-1][
+0000aa50: 2769 7465 6d27 5d0d 0a20 2020 2020 2020  'item']..       
+0000aa60: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
+0000aa70: 6973 5b2d 315d 2e72 656d 6f76 6548 616e  is[-1].removeHan
+0000aa80: 646c 6528 6829 0d0a 2020 2020 2020 2020  dle(h)..        
+0000aa90: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0000aaa0: 656c 662e 726f 6973 5b2d 315d 2e73 6567  elf.rois[-1].seg
+0000aab0: 6d65 6e74 733a 0d0a 2020 2020 2020 2020  ments:..        
+0000aac0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000aad0: 2e72 656d 6f76 6549 7465 6d28 7365 6c66  .removeItem(self
+0000aae0: 2e72 6f69 735b 2d31 5d29 0d0a 2020 2020  .rois[-1])..    
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab00: 7365 6c66 2e72 6f69 7320 3d20 7365 6c66  self.rois = self
+0000ab10: 2e72 6f69 735b 3a2d 315d 0d0a 2020 2020  .rois[:-1]..    
 0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab30: 2020 2020 2020 2020 2020 2062 756c 6c5f             bull_
-0000ab40: 6672 616d 6520 2020 2020 2020 3d20 6361  frame       = ca
-0000ab50: 6e64 6c65 5f62 756c 6c5f 636f 6c6f 722c  ndle_bull_color,
+0000ab30: 7365 6c66 2e64 7261 775f 6c69 6e65 203d  self.draw_line =
+0000ab40: 204e 6f6e 650d 0a20 2020 2020 2020 2020   None..         
+0000ab50: 2020 2069 6620 7365 6c66 2e72 6f69 733a     if self.rois:
 0000ab60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ab70: 2020 2020 2020 2020 2020 2020 2062 756c               bul
-0000ab80: 6c5f 626f 6479 2020 2020 2020 2020 3d20  l_body        = 
-0000ab90: 6361 6e64 6c65 5f62 756c 6c5f 626f 6479  candle_bull_body
-0000aba0: 5f63 6f6c 6f72 2c0d 0a20 2020 2020 2020  _color,..       
-0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2020 2020 6265 6172 5f73 6861 646f 7720      bear_shadow 
-0000abd0: 2020 2020 203d 2063 616e 646c 655f 6265       = candle_be
-0000abe0: 6172 5f63 6f6c 6f72 2c0d 0a20 2020 2020  ar_color,..     
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 2020 2020 2020 6265 6172 5f66 7261 6d65        bear_frame
-0000ac10: 2020 2020 2020 203d 2063 616e 646c 655f         = candle_
-0000ac20: 6265 6172 5f63 6f6c 6f72 2c0d 0a20 2020  bear_color,..   
-0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac40: 2020 2020 2020 2020 6265 6172 5f62 6f64          bear_bod
-0000ac50: 7920 2020 2020 2020 203d 2063 616e 646c  y        = candl
-0000ac60: 655f 6265 6172 5f62 6f64 795f 636f 6c6f  e_bear_body_colo
-0000ac70: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-0000ac80: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000ac90: 6561 6b5f 6275 6c6c 5f73 6861 646f 7720  eak_bull_shadow 
-0000aca0: 3d20 6272 6967 6874 656e 2863 616e 646c  = brighten(candl
-0000acb0: 655f 6275 6c6c 5f63 6f6c 6f72 2c20 312e  e_bull_color, 1.
-0000acc0: 3229 2c0d 0a20 2020 2020 2020 2020 2020  2),..           
-0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ace0: 7765 616b 5f62 756c 6c5f 6672 616d 6520  weak_bull_frame 
-0000acf0: 203d 2062 7269 6768 7465 6e28 6361 6e64   = brighten(cand
-0000ad00: 6c65 5f62 756c 6c5f 636f 6c6f 722c 2031  le_bull_color, 1
-0000ad10: 2e32 292c 0d0a 2020 2020 2020 2020 2020  .2),..          
-0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad30: 2077 6561 6b5f 6275 6c6c 5f62 6f64 7920   weak_bull_body 
-0000ad40: 2020 3d20 6272 6967 6874 656e 2863 616e    = brighten(can
-0000ad50: 646c 655f 6275 6c6c 5f63 6f6c 6f72 2c20  dle_bull_color, 
-0000ad60: 312e 3229 2c0d 0a20 2020 2020 2020 2020  1.2),..         
-0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad80: 2020 7765 616b 5f62 6561 725f 7368 6164    weak_bear_shad
-0000ad90: 6f77 203d 2062 7269 6768 7465 6e28 6361  ow = brighten(ca
-0000ada0: 6e64 6c65 5f62 6561 725f 636f 6c6f 722c  ndle_bear_color,
-0000adb0: 2031 2e35 292c 0d0a 2020 2020 2020 2020   1.5),..        
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000add0: 2020 2077 6561 6b5f 6265 6172 5f66 7261     weak_bear_fra
-0000ade0: 6d65 2020 3d20 6272 6967 6874 656e 2863  me  = brighten(c
-0000adf0: 616e 646c 655f 6265 6172 5f63 6f6c 6f72  andle_bear_color
-0000ae00: 2c20 312e 3529 2c0d 0a20 2020 2020 2020  , 1.5),..       
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae20: 2020 2020 7765 616b 5f62 6561 725f 626f      weak_bear_bo
-0000ae30: 6479 2020 203d 2062 7269 6768 7465 6e28  dy   = brighten(
-0000ae40: 6361 6e64 6c65 5f62 6561 725f 636f 6c6f  candle_bear_colo
-0000ae50: 722c 2031 2e35 2929 0d0a 2020 2020 2020  r, 1.5))..      
-0000ae60: 2020 7365 6c66 2e64 7261 775f 626f 6479    self.draw_body
-0000ae70: 203d 2064 7261 775f 626f 6479 0d0a 2020   = draw_body..  
-0000ae80: 2020 2020 2020 7365 6c66 2e64 7261 775f        self.draw_
-0000ae90: 7368 6164 6f77 203d 2064 7261 775f 7368  shadow = draw_sh
-0000aea0: 6164 6f77 0d0a 2020 2020 2020 2020 7365  adow..        se
-0000aeb0: 6c66 2e63 616e 646c 655f 7769 6474 6820  lf.candle_width 
-0000aec0: 3d20 6361 6e64 6c65 5f77 6964 7468 0d0a  = candle_width..
-0000aed0: 2020 2020 2020 2020 7365 6c66 2e73 6861          self.sha
-0000aee0: 646f 775f 7769 6474 6820 3d20 6361 6e64  dow_width = cand
-0000aef0: 6c65 5f73 6861 646f 775f 7769 6474 680d  le_shadow_width.
-0000af00: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000af10: 6c6f 7266 756e 6320 3d20 636f 6c6f 7266  lorfunc = colorf
-0000af20: 756e 630d 0a20 2020 2020 2020 2073 656c  unc..        sel
-0000af30: 662e 785f 6f66 6673 6574 203d 2030 0d0a  f.x_offset = 0..
-0000af40: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-0000af50: 5f5f 696e 6974 5f5f 2861 782c 2064 6174  __init__(ax, dat
-0000af60: 6173 7263 2c20 6c6f 643d 5472 7565 290d  asrc, lod=True).
-0000af70: 0a0d 0a20 2020 2064 6566 2067 656e 6572  ...    def gener
-0000af80: 6174 655f 7069 6374 7572 6528 7365 6c66  ate_picture(self
-0000af90: 2c20 626f 756e 6469 6e67 5265 6374 293a  , boundingRect):
-0000afa0: 0d0a 2020 2020 2020 2020 7720 3d20 7365  ..        w = se
-0000afb0: 6c66 2e63 616e 646c 655f 7769 6474 680d  lf.candle_width.
-0000afc0: 0a20 2020 2020 2020 2077 3220 3d20 7720  .        w2 = w 
-0000afd0: 2a20 302e 350d 0a20 2020 2020 2020 206c  * 0.5..        l
-0000afe0: 6566 742c 7269 6768 7420 3d20 626f 756e  eft,right = boun
-0000aff0: 6469 6e67 5265 6374 2e6c 6566 7428 292c  dingRect.left(),
-0000b000: 2062 6f75 6e64 696e 6752 6563 742e 7269   boundingRect.ri
-0000b010: 6768 7428 290d 0a20 2020 2020 2020 2070  ght()..        p
-0000b020: 203d 2073 656c 662e 7061 696e 7465 720d   = self.painter.
-0000b030: 0a20 2020 2020 2020 2064 662c 6f72 6967  .        df,orig
-0000b040: 6c65 6e20 3d20 7365 6c66 2e64 6174 6173  len = self.datas
-0000b050: 7263 2e72 6f77 7328 352c 206c 6566 742c  rc.rows(5, left,
-0000b060: 2072 6967 6874 2c20 7973 6361 6c65 3d73   right, yscale=s
-0000b070: 656c 662e 6178 2e76 622e 7973 6361 6c65  elf.ax.vb.yscale
-0000b080: 290d 0a20 2020 2020 2020 2064 7261 7769  )..        drawi
-0000b090: 6e67 5f6d 616e 795f 7368 6164 6f77 7320  ng_many_shadows 
-0000b0a0: 3d20 7365 6c66 2e64 7261 775f 7368 6164  = self.draw_shad
-0000b0b0: 6f77 2061 6e64 206f 7269 676c 656e 203e  ow and origlen >
-0000b0c0: 206c 6f64 5f63 616e 646c 6573 2a32 2f2f   lod_candles*2//
-0000b0d0: 330d 0a20 2020 2020 2020 2066 6f72 2073  3..        for s
-0000b0e0: 6861 646f 772c 6672 616d 652c 626f 6479  hadow,frame,body
-0000b0f0: 2c64 665f 726f 7773 2069 6e20 7365 6c66  ,df_rows in self
-0000b100: 2e63 6f6c 6f72 6675 6e63 2873 656c 662c  .colorfunc(self,
-0000b110: 2073 656c 662e 6461 7461 7372 632c 2064   self.datasrc, d
-0000b120: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-0000b130: 2069 6478 7320 3d20 6466 5f72 6f77 732e   idxs = df_rows.
-0000b140: 696e 6465 780d 0a20 2020 2020 2020 2020  index..         
-0000b150: 2020 2072 6f77 7320 3d20 6466 5f72 6f77     rows = df_row
-0000b160: 732e 7661 6c75 6573 0d0a 2020 2020 2020  s.values..      
-0000b170: 2020 2020 2020 6966 2073 656c 662e 785f        if self.x_
-0000b180: 6f66 6673 6574 3a0d 0a20 2020 2020 2020  offset:..       
-0000b190: 2020 2020 2020 2020 2069 6478 7320 2b3d           idxs +=
-0000b1a0: 2073 656c 662e 785f 6f66 6673 6574 0d0a   self.x_offset..
-0000b1b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b1c0: 656c 662e 6472 6177 5f73 6861 646f 773a  elf.draw_shadow:
-0000b1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b1e0: 2020 702e 7365 7450 656e 2870 672e 6d6b    p.setPen(pg.mk
-0000b1f0: 5065 6e28 7368 6164 6f77 2c20 7769 6474  Pen(shadow, widt
-0000b200: 683d 7365 6c66 2e73 6861 646f 775f 7769  h=self.shadow_wi
-0000b210: 6474 6829 290d 0a20 2020 2020 2020 2020  dth))..         
-0000b220: 2020 2020 2020 2066 6f72 2078 2c28 742c         for x,(t,
-0000b230: 6f70 656e 2c63 6c6f 7365 2c68 6967 682c  open,close,high,
-0000b240: 6c6f 7729 2069 6e20 7a69 7028 6964 7873  low) in zip(idxs
-0000b250: 2c20 726f 7773 293a 0d0a 2020 2020 2020  , rows):..      
-0000b260: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000b270: 2068 6967 6820 3e20 6c6f 773a 0d0a 2020   high > low:..  
-0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 2020 2020 2020 702e 6472 6177 4c69 6e65        p.drawLine
-0000b2a0: 2851 7443 6f72 652e 5150 6f69 6e74 4628  (QtCore.QPointF(
-0000b2b0: 782c 206c 6f77 292c 2051 7443 6f72 652e  x, low), QtCore.
-0000b2c0: 5150 6f69 6e74 4628 782c 2068 6967 6829  QPointF(x, high)
-0000b2d0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0000b2e0: 6620 7365 6c66 2e64 7261 775f 626f 6479  f self.draw_body
-0000b2f0: 2061 6e64 206e 6f74 2064 7261 7769 6e67   and not drawing
-0000b300: 5f6d 616e 795f 7368 6164 6f77 733a 2023  _many_shadows: #
-0000b310: 2073 6574 746c 6520 7769 7468 206f 6e6c   settle with onl
-0000b320: 7920 6472 6177 696e 6720 7368 6164 6f77  y drawing shadow
-0000b330: 7320 6966 2074 6f6f 206d 7563 6820 6465  s if too much de
-0000b340: 7461 696c 0d0a 2020 2020 2020 2020 2020  tail..          
-0000b350: 2020 2020 2020 702e 7365 7450 656e 2870        p.setPen(p
-0000b360: 672e 6d6b 5065 6e28 6672 616d 6529 290d  g.mkPen(frame)).
-0000b370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b380: 2070 2e73 6574 4272 7573 6828 7067 2e6d   p.setBrush(pg.m
-0000b390: 6b42 7275 7368 2862 6f64 7929 290d 0a20  kBrush(body)).. 
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000b3b0: 6f72 2078 2c28 742c 6f70 656e 2c63 6c6f  or x,(t,open,clo
-0000b3c0: 7365 2c68 6967 682c 6c6f 7729 2069 6e20  se,high,low) in 
-0000b3d0: 7a69 7028 6964 7873 2c20 726f 7773 293a  zip(idxs, rows):
-0000b3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b3f0: 2020 2020 2020 702e 6472 6177 5265 6374        p.drawRect
-0000b400: 2851 7443 6f72 652e 5152 6563 7446 2878  (QtCore.QRectF(x
-0000b410: 2d77 322c 206f 7065 6e2c 2077 2c20 636c  -w2, open, w, cl
-0000b420: 6f73 652d 6f70 656e 2929 0d0a 0d0a 2020  ose-open))....  
-0000b430: 2020 6465 6620 726f 7763 6f6c 6f72 7328    def rowcolors(
-0000b440: 7365 6c66 2c20 7072 6566 6978 293a 0d0a  self, prefix):..
-0000b450: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-0000b460: 7365 6c66 2e63 6f6c 6f72 735b 7072 6566  self.colors[pref
-0000b470: 6978 2b27 5f73 6861 646f 7727 5d2c 2073  ix+'_shadow'], s
-0000b480: 656c 662e 636f 6c6f 7273 5b70 7265 6669  elf.colors[prefi
-0000b490: 782b 275f 6672 616d 6527 5d2c 2073 656c  x+'_frame'], sel
-0000b4a0: 662e 636f 6c6f 7273 5b70 7265 6669 782b  f.colors[prefix+
-0000b4b0: 275f 626f 6479 275d 5d0d 0a0d 0a0d 0a0d  '_body']].......
-0000b4c0: 0a63 6c61 7373 2048 6561 746d 6170 4974  .class HeatmapIt
-0000b4d0: 656d 2846 696e 506c 6f74 4974 656d 293a  em(FinPlotItem):
-0000b4e0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0000b4f0: 5f5f 2873 656c 662c 2061 782c 2064 6174  __(self, ax, dat
-0000b500: 6173 7263 2c20 7265 6374 5f73 697a 653d  asrc, rect_size=
-0000b510: 302e 392c 2066 696c 7465 725f 6c69 6d69  0.9, filter_limi
-0000b520: 743d 302c 2063 6f6c 6d61 703d 636f 6c6d  t=0, colmap=colm
-0000b530: 6170 5f63 6c61 7368 2c20 7768 6974 656f  ap_clash, whiteo
-0000b540: 7574 3d30 2e30 2c20 636f 6c63 7572 7665  ut=0.0, colcurve
-0000b550: 3d6c 616d 6264 6120 783a 706f 7728 782c  =lambda x:pow(x,
-0000b560: 3429 293a 0d0a 2020 2020 2020 2020 7365  4)):..        se
-0000b570: 6c66 2e72 6563 745f 7369 7a65 203d 2072  lf.rect_size = r
-0000b580: 6563 745f 7369 7a65 0d0a 2020 2020 2020  ect_size..      
-0000b590: 2020 7365 6c66 2e66 696c 7465 725f 6c69    self.filter_li
-0000b5a0: 6d69 7420 3d20 6669 6c74 6572 5f6c 696d  mit = filter_lim
-0000b5b0: 6974 0d0a 2020 2020 2020 2020 7365 6c66  it..        self
-0000b5c0: 2e63 6f6c 6d61 7020 3d20 636f 6c6d 6170  .colmap = colmap
-0000b5d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-0000b5e0: 6869 7465 6f75 7420 3d20 7768 6974 656f  hiteout = whiteo
-0000b5f0: 7574 0d0a 2020 2020 2020 2020 7365 6c66  ut..        self
-0000b600: 2e63 6f6c 6375 7276 6520 3d20 636f 6c63  .colcurve = colc
-0000b610: 7572 7665 0d0a 2020 2020 2020 2020 7365  urve..        se
-0000b620: 6c66 2e63 6f6c 5f64 6174 615f 656e 6420  lf.col_data_end 
-0000b630: 3d20 6c65 6e28 6461 7461 7372 632e 6466  = len(datasrc.df
-0000b640: 2e63 6f6c 756d 6e73 290d 0a20 2020 2020  .columns)..     
-0000b650: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0000b660: 745f 5f28 6178 2c20 6461 7461 7372 632c  t__(ax, datasrc,
-0000b670: 206c 6f64 3d46 616c 7365 290d 0a0d 0a20   lod=False).... 
-0000b680: 2020 2064 6566 2067 656e 6572 6174 655f     def generate_
-0000b690: 7069 6374 7572 6528 7365 6c66 2c20 626f  picture(self, bo
-0000b6a0: 756e 6469 6e67 5265 6374 293a 0d0a 2020  undingRect):..  
-0000b6b0: 2020 2020 2020 7072 6963 6573 203d 2073        prices = s
-0000b6c0: 656c 662e 6461 7461 7372 632e 6466 2e63  elf.datasrc.df.c
-0000b6d0: 6f6c 756d 6e73 5b73 656c 662e 6461 7461  olumns[self.data
-0000b6e0: 7372 632e 636f 6c5f 6461 7461 5f6f 6666  src.col_data_off
-0000b6f0: 7365 743a 7365 6c66 2e63 6f6c 5f64 6174  set:self.col_dat
-0000b700: 615f 656e 645d 0d0a 2020 2020 2020 2020  a_end]..        
-0000b710: 6830 203d 2028 7072 6963 6573 5b30 5d20  h0 = (prices[0] 
-0000b720: 2d20 7072 6963 6573 5b31 5d29 202a 2028  - prices[1]) * (
-0000b730: 312d 7365 6c66 2e72 6563 745f 7369 7a65  1-self.rect_size
-0000b740: 290d 0a20 2020 2020 2020 2068 3120 3d20  )..        h1 = 
-0000b750: 2870 7269 6365 735b 305d 202d 2070 7269  (prices[0] - pri
-0000b760: 6365 735b 315d 2920 2a20 2831 2d28 312d  ces[1]) * (1-(1-
-0000b770: 7365 6c66 2e72 6563 745f 7369 7a65 292a  self.rect_size)*
-0000b780: 3229 0d0a 2020 2020 2020 2020 7265 6374  2)..        rect
-0000b790: 5f73 697a 6532 203d 2030 2e35 202a 2073  _size2 = 0.5 * s
-0000b7a0: 656c 662e 7265 6374 5f73 697a 650d 0a20  elf.rect_size.. 
-0000b7b0: 2020 2020 2020 2064 6620 3d20 7365 6c66         df = self
-0000b7c0: 2e64 6174 6173 7263 2e64 662e 696c 6f63  .datasrc.df.iloc
-0000b7d0: 5b3a 2c20 7365 6c66 2e64 6174 6173 7263  [:, self.datasrc
-0000b7e0: 2e63 6f6c 5f64 6174 615f 6f66 6673 6574  .col_data_offset
-0000b7f0: 3a73 656c 662e 636f 6c5f 6461 7461 5f65  :self.col_data_e
-0000b800: 6e64 5d0d 0a20 2020 2020 2020 2076 616c  nd]..        val
-0000b810: 7565 7320 3d20 6466 2e76 616c 7565 730d  ues = df.values.
-0000b820: 0a20 2020 2020 2020 2023 206e 6f72 6d61  .        # norma
-0000b830: 6c69 7a65 0d0a 2020 2020 2020 2020 7661  lize..        va
-0000b840: 6c75 6573 202d 3d20 6e70 2e6e 616e 6d69  lues -= np.nanmi
-0000b850: 6e28 7661 6c75 6573 290d 0a20 2020 2020  n(values)..     
-0000b860: 2020 2076 616c 7565 7320 3d20 7661 6c75     values = valu
-0000b870: 6573 202f 2028 6e70 2e6e 616e 6d61 7828  es / (np.nanmax(
-0000b880: 7661 6c75 6573 2920 2f20 2831 2b73 656c  values) / (1+sel
-0000b890: 662e 7768 6974 656f 7574 2929 2023 206f  f.whiteout)) # o
-0000b8a0: 7665 7273 686f 6f74 2066 6f72 2063 6f6c  vershoot for col
-0000b8b0: 6f72 696e 670d 0a20 2020 2020 2020 206c  oring..        l
-0000b8c0: 696d 203d 2073 656c 662e 6669 6c74 6572  im = self.filter
-0000b8d0: 5f6c 696d 6974 202a 2028 312b 7365 6c66  _limit * (1+self
-0000b8e0: 2e77 6869 7465 6f75 7429 0d0a 2020 2020  .whiteout)..    
-0000b8f0: 2020 2020 7020 3d20 7365 6c66 2e70 6169      p = self.pai
-0000b900: 6e74 6572 0d0a 2020 2020 2020 2020 666f  nter..        fo
-0000b910: 7220 742c 726f 7720 696e 2065 6e75 6d65  r t,row in enume
-0000b920: 7261 7465 2876 616c 7565 7329 3a0d 0a20  rate(values):.. 
-0000b930: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-0000b940: 692c 7072 6963 6520 696e 2065 6e75 6d65  i,price in enume
-0000b950: 7261 7465 2870 7269 6365 7329 3a0d 0a20  rate(prices):.. 
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000b970: 203d 2072 6f77 5b63 695d 0d0a 2020 2020   = row[ci]..    
-0000b980: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-0000b990: 203e 3d20 6c69 6d3a 0d0a 2020 2020 2020   >= lim:..      
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 7620                v 
-0000b9b0: 3d20 3120 2d20 7365 6c66 2e63 6f6c 6375  = 1 - self.colcu
-0000b9c0: 7276 6528 3120 2d20 2876 2d6c 696d 292f  rve(1 - (v-lim)/
-0000b9d0: 2831 2d6c 696d 2929 0d0a 2020 2020 2020  (1-lim))..      
-0000b9e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000b9f0: 6c6f 7220 3d20 7365 6c66 2e63 6f6c 6d61  lor = self.colma
-0000ba00: 702e 6d61 7028 762c 206d 6f64 653d 2771  p.map(v, mode='q
-0000ba10: 636f 6c6f 7227 290d 0a20 2020 2020 2020  color')..       
-0000ba20: 2020 2020 2020 2020 2020 2020 2070 2e66               p.f
-0000ba30: 696c 6c52 6563 7428 5174 436f 7265 2e51  illRect(QtCore.Q
-0000ba40: 5265 6374 4628 742d 7265 6374 5f73 697a  RectF(t-rect_siz
-0000ba50: 6532 2c20 7365 6c66 2e61 782e 7662 2e79  e2, self.ax.vb.y
-0000ba60: 7363 616c 652e 696e 7678 666f 726d 2870  scale.invxform(p
-0000ba70: 7269 6365 2b68 3029 2c20 7365 6c66 2e72  rice+h0), self.r
-0000ba80: 6563 745f 7369 7a65 2c20 7365 6c66 2e61  ect_size, self.a
-0000ba90: 782e 7662 2e79 7363 616c 652e 696e 7678  x.vb.yscale.invx
-0000baa0: 666f 726d 2868 3129 292c 2063 6f6c 6f72  form(h1)), color
-0000bab0: 290d 0a0d 0a0d 0a0d 0a63 6c61 7373 2048  )........class H
-0000bac0: 6f72 697a 6f6e 7461 6c54 696d 6556 6f6c  orizontalTimeVol
-0000bad0: 756d 6549 7465 6d28 4361 6e64 6c65 7374  umeItem(Candlest
-0000bae0: 6963 6b49 7465 6d29 3a0d 0a20 2020 2064  ickItem):..    d
-0000baf0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000bb00: 2c20 6178 2c20 6461 7461 7372 632c 2063  , ax, datasrc, c
-0000bb10: 616e 646c 655f 7769 6474 683d 302e 382c  andle_width=0.8,
-0000bb20: 2064 7261 775f 7661 3d30 2e30 2c20 6472   draw_va=0.0, dr
-0000bb30: 6177 5f62 6f64 793d 302e 342c 2064 7261  aw_body=0.4, dra
-0000bb40: 775f 706f 633d 302e 302c 2063 6f6c 6f72  w_poc=0.0, color
-0000bb50: 6675 6e63 3d4e 6f6e 6529 3a0d 0a20 2020  func=None):..   
-0000bb60: 2020 2020 2027 2727 4120 6e65 6761 7469       '''A negati
-0000bb70: 7665 2064 7261 775f 626f 6479 2064 6f65  ve draw_body doe
-0000bb80: 7320 6e6f 7420 6d65 616e 2074 6861 7420  s not mean that 
-0000bb90: 7468 6520 6361 6e64 6c65 2069 7320 6472  the candle is dr
-0000bba0: 6177 6e20 696e 2074 6865 206f 7070 6f73  awn in the oppos
-0000bbb0: 6974 6520 6469 7265 6374 696f 6e20 2875  ite direction (u
-0000bbc0: 7365 206e 6567 6174 6976 6520 766f 6c75  se negative volu
-0000bbd0: 6d65 2066 6f72 2074 6861 7429 2c0d 0a20  me for that),.. 
-0000bbe0: 2020 2020 2020 2020 2020 6275 7420 696e            but in
-0000bbf0: 7374 6561 6420 7468 6174 2073 6372 6565  stead that scree
-0000bc00: 6e20 7363 616c 6520 7769 6c6c 2062 6520  n scale will be 
-0000bc10: 7573 6564 2069 6e73 7465 6164 206f 6620  used instead of 
-0000bc20: 696e 7465 7276 616c 2d72 656c 6174 6976  interval-relativ
-0000bc30: 6520 7363 616c 652e 2727 270d 0a20 2020  e scale.'''..   
-0000bc40: 2020 2020 2073 656c 662e 6472 6177 5f76       self.draw_v
-0000bc50: 6120 3d20 6472 6177 5f76 610d 0a20 2020  a = draw_va..   
-0000bc60: 2020 2020 2073 656c 662e 6472 6177 5f70       self.draw_p
-0000bc70: 6f63 203d 2064 7261 775f 706f 630d 0a20  oc = draw_poc.. 
-0000bc80: 2020 2020 2020 2023 2320 7365 6c66 2e63         ## self.c
-0000bc90: 6f6c 5f64 6174 615f 656e 6420 3d20 6c65  ol_data_end = le
-0000bca0: 6e28 6461 7461 7372 632e 6466 2e63 6f6c  n(datasrc.df.col
-0000bcb0: 756d 6e73 290d 0a20 2020 2020 2020 2063  umns)..        c
-0000bcc0: 6f6c 6f72 6675 6e63 203d 2063 6f6c 6f72  olorfunc = color
-0000bcd0: 6675 6e63 206f 7220 686f 7269 7a76 6f6c  func or horizvol
-0000bce0: 5f63 6f6c 6f72 6669 6c74 6572 2829 2023  _colorfilter() #
-0000bcf0: 2072 6573 6f6c 7665 2066 756e 6374 696f   resolve functio
-0000bd00: 6e20 6c6f 7765 7220 646f 776e 2069 6e20  n lower down in 
-0000bd10: 736f 7572 6365 2063 6f64 650d 0a20 2020  source code..   
-0000bd20: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-0000bd30: 6e69 745f 5f28 6178 2c20 6461 7461 7372  nit__(ax, datasr
-0000bd40: 632c 2064 7261 775f 7368 6164 6f77 3d46  c, draw_shadow=F
-0000bd50: 616c 7365 2c20 6361 6e64 6c65 5f77 6964  alse, candle_wid
-0000bd60: 7468 3d63 616e 646c 655f 7769 6474 682c  th=candle_width,
-0000bd70: 2064 7261 775f 626f 6479 3d64 7261 775f   draw_body=draw_
-0000bd80: 626f 6479 2c20 636f 6c6f 7266 756e 633d  body, colorfunc=
-0000bd90: 636f 6c6f 7266 756e 6329 0d0a 2020 2020  colorfunc)..    
-0000bda0: 2020 2020 7365 6c66 2e6c 6f64 203d 2046      self.lod = F
-0000bdb0: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
-0000bdc0: 6c66 2e63 6f6c 6f72 732e 7570 6461 7465  lf.colors.update
-0000bdd0: 2864 6963 7428 6e65 7574 7261 6c5f 7368  (dict(neutral_sh
-0000bde0: 6164 6f77 2020 3d20 766f 6c75 6d65 5f6e  adow  = volume_n
-0000bdf0: 6575 7472 616c 5f63 6f6c 6f72 2c0d 0a20  eutral_color,.. 
-0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be10: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000be20: 6575 7472 616c 5f66 7261 6d65 2020 203d  eutral_frame   =
-0000be30: 2076 6f6c 756d 655f 6e65 7574 7261 6c5f   volume_neutral_
-0000be40: 636f 6c6f 722c 0d0a 2020 2020 2020 2020  color,..        
-0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 2020 2020 2020 6e65 7574 7261 6c5f          neutral_
-0000be70: 626f 6479 2020 2020 3d20 766f 6c75 6d65  body    = volume
-0000be80: 5f6e 6575 7472 616c 5f63 6f6c 6f72 2c0d  _neutral_color,.
+0000ab70: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000ab80: 7365 6c66 2e72 6f69 735b 2d31 5d2c 2070  self.rois[-1], p
+0000ab90: 672e 506f 6c79 4c69 6e65 524f 4929 3a0d  g.PolyLineROI):.
+0000aba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000abb0: 2020 2020 2073 656c 662e 6472 6177 5f6c       self.draw_l
+0000abc0: 696e 6520 3d20 7365 6c66 2e72 6f69 735b  ine = self.rois[
+0000abd0: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
+0000abe0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000abf0: 745f 6472 6177 5f6c 696e 655f 636f 6c6f  t_draw_line_colo
+0000ac00: 7228 6472 6177 5f6c 696e 655f 636f 6c6f  r(draw_line_colo
+0000ac10: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+0000ac20: 7265 7475 726e 2054 7275 650d 0a0d 0a20  return True.... 
+0000ac30: 2020 2064 6566 2061 7070 656e 645f 6472     def append_dr
+0000ac40: 6177 5f73 6567 6d65 6e74 2873 656c 662c  aw_segment(self,
+0000ac50: 2070 293a 0d0a 2020 2020 2020 2020 6830   p):..        h0
+0000ac60: 203d 2073 656c 662e 6472 6177 5f6c 696e   = self.draw_lin
+0000ac70: 652e 6861 6e64 6c65 735b 2d31 5d5b 2769  e.handles[-1]['i
+0000ac80: 7465 6d27 5d0d 0a20 2020 2020 2020 2068  tem']..        h
+0000ac90: 3120 3d20 7365 6c66 2e64 7261 775f 6c69  1 = self.draw_li
+0000aca0: 6e65 2e61 6464 4672 6565 4861 6e64 6c65  ne.addFreeHandle
+0000acb0: 2870 290d 0a20 2020 2020 2020 2073 656c  (p)..        sel
+0000acc0: 662e 6472 6177 5f6c 696e 652e 6164 6453  f.draw_line.addS
+0000acd0: 6567 6d65 6e74 2868 302c 2068 3129 0d0a  egment(h0, h1)..
+0000ace0: 2020 2020 2020 2020 7365 6c66 2e64 7261          self.dra
+0000acf0: 7769 6e67 203d 2054 7275 650d 0a0d 0a20  wing = True.... 
+0000ad00: 2020 2064 6566 2073 6574 5f64 7261 775f     def set_draw_
+0000ad10: 6c69 6e65 5f63 6f6c 6f72 2873 656c 662c  line_color(self,
+0000ad20: 2063 6f6c 6f72 293a 0d0a 2020 2020 2020   color):..      
+0000ad30: 2020 6966 2073 656c 662e 6472 6177 5f6c    if self.draw_l
+0000ad40: 696e 653a 0d0a 2020 2020 2020 2020 2020  ine:..          
+0000ad50: 2020 7065 6e20 3d20 7067 2e6d 6b50 656e    pen = pg.mkPen
+0000ad60: 2863 6f6c 6f72 290d 0a20 2020 2020 2020  (color)..       
+0000ad70: 2020 2020 2066 6f72 2073 6567 6d65 6e74       for segment
+0000ad80: 2069 6e20 7365 6c66 2e64 7261 775f 6c69   in self.draw_li
+0000ad90: 6e65 2e73 6567 6d65 6e74 733a 0d0a 2020  ne.segments:..  
+0000ada0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000adb0: 676d 656e 742e 6375 7272 656e 7450 656e  gment.currentPen
+0000adc0: 203d 2073 6567 6d65 6e74 2e70 656e 203d   = segment.pen =
+0000add0: 2070 656e 0d0a 2020 2020 2020 2020 2020   pen..          
+0000ade0: 2020 2020 2020 7365 676d 656e 742e 7570        segment.up
+0000adf0: 6461 7465 2829 0d0a 0d0a 2020 2020 6465  date()....    de
+0000ae00: 6620 7375 6767 6573 7450 6164 6469 6e67  f suggestPadding
+0000ae10: 2873 656c 662c 2061 7869 7329 3a0d 0a20  (self, axis):.. 
+0000ae20: 2020 2020 2020 2072 6574 7572 6e20 300d         return 0.
+0000ae30: 0a0d 0a0d 0a0d 0a63 6c61 7373 2046 696e  .......class Fin
+0000ae40: 506c 6f74 4974 656d 2870 672e 4772 6170  PlotItem(pg.Grap
+0000ae50: 6869 6373 4f62 6a65 6374 293a 0d0a 2020  hicsObject):..  
+0000ae60: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000ae70: 656c 662c 2061 782c 2064 6174 6173 7263  elf, ax, datasrc
+0000ae80: 2c20 6c6f 6429 3a0d 0a20 2020 2020 2020  , lod):..       
+0000ae90: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+0000aea0: 5f28 290d 0a20 2020 2020 2020 2073 656c  _()..        sel
+0000aeb0: 662e 6178 203d 2061 780d 0a20 2020 2020  f.ax = ax..     
+0000aec0: 2020 2073 656c 662e 6461 7461 7372 6320     self.datasrc 
+0000aed0: 3d20 6461 7461 7372 630d 0a20 2020 2020  = datasrc..     
+0000aee0: 2020 2073 656c 662e 7069 6374 7572 6520     self.picture 
+0000aef0: 3d20 5174 4775 692e 5150 6963 7475 7265  = QtGui.QPicture
+0000af00: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0000af10: 2e70 6169 6e74 6572 203d 2051 7447 7569  .painter = QtGui
+0000af20: 2e51 5061 696e 7465 7228 290d 0a20 2020  .QPainter()..   
+0000af30: 2020 2020 2073 656c 662e 6469 7274 7920       self.dirty 
+0000af40: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+0000af50: 7365 6c66 2e6c 6f64 203d 206c 6f64 0d0a  self.lod = lod..
+0000af60: 2020 2020 2020 2020 7365 6c66 2e63 6163          self.cac
+0000af70: 6865 6452 6563 7420 3d20 4e6f 6e65 0d0a  hedRect = None..
+0000af80: 0d0a 2020 2020 6465 6620 7265 7061 696e  ..    def repain
+0000af90: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
+0000afa0: 2020 7365 6c66 2e64 6972 7479 203d 2054    self.dirty = T
+0000afb0: 7275 650d 0a20 2020 2020 2020 2073 656c  rue..        sel
+0000afc0: 662e 7061 696e 7428 7365 6c66 2e70 6169  f.paint(self.pai
+0000afd0: 6e74 6572 290d 0a0d 0a20 2020 2064 6566  nter)....    def
+0000afe0: 2070 6169 6e74 2873 656c 662c 2070 2c20   paint(self, p, 
+0000aff0: 2a61 7267 7329 3a0d 0a20 2020 2020 2020  *args):..       
+0000b000: 2069 6620 7365 6c66 2e64 6174 6173 7263   if self.datasrc
+0000b010: 2e69 735f 7370 6172 7365 3a0d 0a20 2020  .is_sparse:..   
+0000b020: 2020 2020 2020 2020 2073 656c 662e 6469           self.di
+0000b030: 7274 7920 3d20 5472 7565 0d0a 2020 2020  rty = True..    
+0000b040: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
+0000b050: 6469 7274 795f 7069 6374 7572 6528 7365  dirty_picture(se
+0000b060: 6c66 2e76 6965 7752 6563 7428 2929 0d0a  lf.viewRect())..
+0000b070: 2020 2020 2020 2020 702e 6472 6177 5069          p.drawPi
+0000b080: 6374 7572 6528 302c 2030 2c20 7365 6c66  cture(0, 0, self
+0000b090: 2e70 6963 7475 7265 290d 0a0d 0a20 2020  .picture)....   
+0000b0a0: 2064 6566 2075 7064 6174 655f 6469 7274   def update_dirt
+0000b0b0: 795f 7069 6374 7572 6528 7365 6c66 2c20  y_picture(self, 
+0000b0c0: 7669 7369 626c 6552 6563 7429 3a0d 0a20  visibleRect):.. 
+0000b0d0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0000b0e0: 6972 7479 206f 7220 5c0d 0a20 2020 2020  irty or \..     
+0000b0f0: 2020 2020 2020 2028 7365 6c66 2e6c 6f64         (self.lod
+0000b100: 2061 6e64 2023 2072 6567 656e 6572 6174   and # regenerat
+0000b110: 6520 7768 656e 207a 6f6f 6d20 6368 616e  e when zoom chan
+0000b120: 6765 733f 0d0a 2020 2020 2020 2020 2020  ges?..          
+0000b130: 2020 2020 2020 2876 6973 6962 6c65 5265        (visibleRe
+0000b140: 6374 2e6c 6566 7428 2920 3c20 7365 6c66  ct.left() < self
+0000b150: 2e63 6163 6865 6452 6563 742e 6c65 6674  .cachedRect.left
+0000b160: 2829 206f 7220 5c0d 0a20 2020 2020 2020  () or \..       
+0000b170: 2020 2020 2020 2020 2020 7669 7369 626c            visibl
+0000b180: 6552 6563 742e 7269 6768 7428 2920 3e20  eRect.right() > 
+0000b190: 7365 6c66 2e63 6163 6865 6452 6563 742e  self.cachedRect.
+0000b1a0: 7269 6768 7428 2920 6f72 205c 0d0a 2020  right() or \..  
+0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000b1c0: 6973 6962 6c65 5265 6374 2e77 6964 7468  isibleRect.width
+0000b1d0: 2829 203c 2073 656c 662e 6361 6368 6564  () < self.cached
+0000b1e0: 5265 6374 2e77 6964 7468 2829 202f 2063  Rect.width() / c
+0000b1f0: 6163 6865 5f63 616e 646c 655f 6661 6374  ache_candle_fact
+0000b200: 6f72 2929 3a20 2320 6f70 7469 6d69 7a65  or)): # optimize
+0000b210: 2077 6865 6e20 7a6f 6f6d 696e 6720 696e   when zooming in
+0000b220: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000b230: 6c66 2e5f 6765 6e65 7261 7465 5f70 6963  lf._generate_pic
+0000b240: 7475 7265 2876 6973 6962 6c65 5265 6374  ture(visibleRect
+0000b250: 290d 0a0d 0a20 2020 2064 6566 205f 6765  )....    def _ge
+0000b260: 6e65 7261 7465 5f70 6963 7475 7265 2873  nerate_picture(s
+0000b270: 656c 662c 2062 6f75 6e64 696e 6752 6563  elf, boundingRec
+0000b280: 7429 3a0d 0a20 2020 2020 2020 2077 203d  t):..        w =
+0000b290: 2062 6f75 6e64 696e 6752 6563 742e 7769   boundingRect.wi
+0000b2a0: 6474 6828 290d 0a20 2020 2020 2020 2073  dth()..        s
+0000b2b0: 656c 662e 6361 6368 6564 5265 6374 203d  elf.cachedRect =
+0000b2c0: 2051 7443 6f72 652e 5152 6563 7446 2862   QtCore.QRectF(b
+0000b2d0: 6f75 6e64 696e 6752 6563 742e 6c65 6674  oundingRect.left
+0000b2e0: 2829 2d28 6361 6368 655f 6361 6e64 6c65  ()-(cache_candle
+0000b2f0: 5f66 6163 746f 722d 3129 2a30 2e35 2a77  _factor-1)*0.5*w
+0000b300: 2c20 302c 2063 6163 6865 5f63 616e 646c  , 0, cache_candl
+0000b310: 655f 6661 6374 6f72 2a77 2c20 3029 0d0a  e_factor*w, 0)..
+0000b320: 2020 2020 2020 2020 7365 6c66 2e70 6169          self.pai
+0000b330: 6e74 6572 2e62 6567 696e 2873 656c 662e  nter.begin(self.
+0000b340: 7069 6374 7572 6529 0d0a 2020 2020 2020  picture)..      
+0000b350: 2020 7365 6c66 2e5f 6765 6e65 7261 7465    self._generate
+0000b360: 5f64 756d 6d79 5f70 6963 7475 7265 2873  _dummy_picture(s
+0000b370: 656c 662e 7669 6577 5265 6374 2829 290d  elf.viewRect()).
+0000b380: 0a20 2020 2020 2020 2073 656c 662e 6765  .        self.ge
+0000b390: 6e65 7261 7465 5f70 6963 7475 7265 2873  nerate_picture(s
+0000b3a0: 656c 662e 6361 6368 6564 5265 6374 290d  elf.cachedRect).
+0000b3b0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
+0000b3c0: 696e 7465 722e 656e 6428 290d 0a20 2020  inter.end()..   
+0000b3d0: 2020 2020 2073 656c 662e 6469 7274 7920       self.dirty 
+0000b3e0: 3d20 4661 6c73 650d 0a0d 0a20 2020 2064  = False....    d
+0000b3f0: 6566 205f 6765 6e65 7261 7465 5f64 756d  ef _generate_dum
+0000b400: 6d79 5f70 6963 7475 7265 2873 656c 662c  my_picture(self,
+0000b410: 2062 6f75 6e64 696e 6752 6563 7429 3a0d   boundingRect):.
+0000b420: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000b430: 2e64 6174 6173 7263 2e69 735f 7370 6172  .datasrc.is_spar
+0000b440: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000b450: 2023 206a 7573 7420 6472 6177 2073 6f6d   # just draw som
+0000b460: 6574 6869 6e67 2074 6f20 656e 7375 7265  ething to ensure
+0000b470: 2050 7951 7420 7769 6c6c 2070 6169 6e74   PyQt will paint
+0000b480: 2075 7320 6167 6169 6e0d 0a20 2020 2020   us again..     
+0000b490: 2020 2020 2020 2073 656c 662e 7061 696e         self.pain
+0000b4a0: 7465 722e 7365 7450 656e 2870 672e 6d6b  ter.setPen(pg.mk
+0000b4b0: 5065 6e28 6261 636b 6772 6f75 6e64 2929  Pen(background))
+0000b4c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000b4d0: 6c66 2e70 6169 6e74 6572 2e73 6574 4272  lf.painter.setBr
+0000b4e0: 7573 6828 7067 2e6d 6b42 7275 7368 2862  ush(pg.mkBrush(b
+0000b4f0: 6163 6b67 726f 756e 6429 290d 0a20 2020  ackground))..   
+0000b500: 2020 2020 2020 2020 206c 2c72 203d 2062           l,r = b
+0000b510: 6f75 6e64 696e 6752 6563 742e 6c65 6674  oundingRect.left
+0000b520: 2829 2c20 626f 756e 6469 6e67 5265 6374  (), boundingRect
+0000b530: 2e72 6967 6874 2829 0d0a 2020 2020 2020  .right()..      
+0000b540: 2020 2020 2020 7365 6c66 2e70 6169 6e74        self.paint
+0000b550: 6572 2e64 7261 7752 6563 7428 5174 436f  er.drawRect(QtCo
+0000b560: 7265 2e51 5265 6374 4628 6c2c 2062 6f75  re.QRectF(l, bou
+0000b570: 6e64 696e 6752 6563 742e 746f 7028 292c  ndingRect.top(),
+0000b580: 2031 652d 332c 2062 6f75 6e64 696e 6752   1e-3, boundingR
+0000b590: 6563 742e 6865 6967 6874 2829 2a31 652d  ect.height()*1e-
+0000b5a0: 3529 290d 0a20 2020 2020 2020 2020 2020  5))..           
+0000b5b0: 2073 656c 662e 7061 696e 7465 722e 6472   self.painter.dr
+0000b5c0: 6177 5265 6374 2851 7443 6f72 652e 5152  awRect(QtCore.QR
+0000b5d0: 6563 7446 2872 2c20 626f 756e 6469 6e67  ectF(r, bounding
+0000b5e0: 5265 6374 2e62 6f74 746f 6d28 292c 202d  Rect.bottom(), -
+0000b5f0: 3165 2d33 2c20 2d62 6f75 6e64 696e 6752  1e-3, -boundingR
+0000b600: 6563 742e 6865 6967 6874 2829 2a31 652d  ect.height()*1e-
+0000b610: 3529 290d 0a0d 0a20 2020 2064 6566 2062  5))....    def b
+0000b620: 6f75 6e64 696e 6752 6563 7428 7365 6c66  oundingRect(self
+0000b630: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+0000b640: 726e 2051 7443 6f72 652e 5152 6563 7446  rn QtCore.QRectF
+0000b650: 2873 656c 662e 7069 6374 7572 652e 626f  (self.picture.bo
+0000b660: 756e 6469 6e67 5265 6374 2829 290d 0a0d  undingRect())...
+0000b670: 0a0d 0a0d 0a63 6c61 7373 2043 616e 646c  .....class Candl
+0000b680: 6573 7469 636b 4974 656d 2846 696e 506c  estickItem(FinPl
+0000b690: 6f74 4974 656d 293a 0d0a 2020 2020 6465  otItem):..    de
+0000b6a0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0000b6b0: 2061 782c 2064 6174 6173 7263 2c20 6472   ax, datasrc, dr
+0000b6c0: 6177 5f62 6f64 792c 2064 7261 775f 7368  aw_body, draw_sh
+0000b6d0: 6164 6f77 2c20 6361 6e64 6c65 5f77 6964  adow, candle_wid
+0000b6e0: 7468 2c20 636f 6c6f 7266 756e 632c 2072  th, colorfunc, r
+0000b6f0: 6573 616d 703d 4e6f 6e65 293a 0d0a 2020  esamp=None):..  
+0000b700: 2020 2020 2020 7365 6c66 2e63 6f6c 6f72        self.color
+0000b710: 7320 3d20 6469 6374 2862 756c 6c5f 7368  s = dict(bull_sh
+0000b720: 6164 6f77 2020 2020 2020 3d20 6361 6e64  adow      = cand
+0000b730: 6c65 5f62 756c 6c5f 636f 6c6f 722c 0d0a  le_bull_color,..
+0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b750: 2020 2020 2020 2020 2020 2062 756c 6c5f             bull_
+0000b760: 6672 616d 6520 2020 2020 2020 3d20 6361  frame       = ca
+0000b770: 6e64 6c65 5f62 756c 6c5f 636f 6c6f 722c  ndle_bull_color,
+0000b780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b790: 2020 2020 2020 2020 2020 2020 2062 756c               bul
+0000b7a0: 6c5f 626f 6479 2020 2020 2020 2020 3d20  l_body        = 
+0000b7b0: 6361 6e64 6c65 5f62 756c 6c5f 626f 6479  candle_bull_body
+0000b7c0: 5f63 6f6c 6f72 2c0d 0a20 2020 2020 2020  _color,..       
+0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7e0: 2020 2020 6265 6172 5f73 6861 646f 7720      bear_shadow 
+0000b7f0: 2020 2020 203d 2063 616e 646c 655f 6265       = candle_be
+0000b800: 6172 5f63 6f6c 6f72 2c0d 0a20 2020 2020  ar_color,..     
+0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b820: 2020 2020 2020 6265 6172 5f66 7261 6d65        bear_frame
+0000b830: 2020 2020 2020 203d 2063 616e 646c 655f         = candle_
+0000b840: 6265 6172 5f63 6f6c 6f72 2c0d 0a20 2020  bear_color,..   
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2020 2020 2020 2020 6265 6172 5f62 6f64          bear_bod
+0000b870: 7920 2020 2020 2020 203d 2063 616e 646c  y        = candl
+0000b880: 655f 6265 6172 5f62 6f64 795f 636f 6c6f  e_bear_body_colo
+0000b890: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000b8b0: 6561 6b5f 6275 6c6c 5f73 6861 646f 7720  eak_bull_shadow 
+0000b8c0: 3d20 6272 6967 6874 656e 2863 616e 646c  = brighten(candl
+0000b8d0: 655f 6275 6c6c 5f63 6f6c 6f72 2c20 312e  e_bull_color, 1.
+0000b8e0: 3229 2c0d 0a20 2020 2020 2020 2020 2020  2),..           
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b900: 7765 616b 5f62 756c 6c5f 6672 616d 6520  weak_bull_frame 
+0000b910: 203d 2062 7269 6768 7465 6e28 6361 6e64   = brighten(cand
+0000b920: 6c65 5f62 756c 6c5f 636f 6c6f 722c 2031  le_bull_color, 1
+0000b930: 2e32 292c 0d0a 2020 2020 2020 2020 2020  .2),..          
+0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b950: 2077 6561 6b5f 6275 6c6c 5f62 6f64 7920   weak_bull_body 
+0000b960: 2020 3d20 6272 6967 6874 656e 2863 616e    = brighten(can
+0000b970: 646c 655f 6275 6c6c 5f63 6f6c 6f72 2c20  dle_bull_color, 
+0000b980: 312e 3229 2c0d 0a20 2020 2020 2020 2020  1.2),..         
+0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9a0: 2020 7765 616b 5f62 6561 725f 7368 6164    weak_bear_shad
+0000b9b0: 6f77 203d 2062 7269 6768 7465 6e28 6361  ow = brighten(ca
+0000b9c0: 6e64 6c65 5f62 6561 725f 636f 6c6f 722c  ndle_bear_color,
+0000b9d0: 2031 2e35 292c 0d0a 2020 2020 2020 2020   1.5),..        
+0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9f0: 2020 2077 6561 6b5f 6265 6172 5f66 7261     weak_bear_fra
+0000ba00: 6d65 2020 3d20 6272 6967 6874 656e 2863  me  = brighten(c
+0000ba10: 616e 646c 655f 6265 6172 5f63 6f6c 6f72  andle_bear_color
+0000ba20: 2c20 312e 3529 2c0d 0a20 2020 2020 2020  , 1.5),..       
+0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba40: 2020 2020 7765 616b 5f62 6561 725f 626f      weak_bear_bo
+0000ba50: 6479 2020 203d 2062 7269 6768 7465 6e28  dy   = brighten(
+0000ba60: 6361 6e64 6c65 5f62 6561 725f 636f 6c6f  candle_bear_colo
+0000ba70: 722c 2031 2e35 2929 0d0a 2020 2020 2020  r, 1.5))..      
+0000ba80: 2020 7365 6c66 2e64 7261 775f 626f 6479    self.draw_body
+0000ba90: 203d 2064 7261 775f 626f 6479 0d0a 2020   = draw_body..  
+0000baa0: 2020 2020 2020 7365 6c66 2e64 7261 775f        self.draw_
+0000bab0: 7368 6164 6f77 203d 2064 7261 775f 7368  shadow = draw_sh
+0000bac0: 6164 6f77 0d0a 2020 2020 2020 2020 7365  adow..        se
+0000bad0: 6c66 2e63 616e 646c 655f 7769 6474 6820  lf.candle_width 
+0000bae0: 3d20 6361 6e64 6c65 5f77 6964 7468 0d0a  = candle_width..
+0000baf0: 2020 2020 2020 2020 7365 6c66 2e73 6861          self.sha
+0000bb00: 646f 775f 7769 6474 6820 3d20 6361 6e64  dow_width = cand
+0000bb10: 6c65 5f73 6861 646f 775f 7769 6474 680d  le_shadow_width.
+0000bb20: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000bb30: 6c6f 7266 756e 6320 3d20 636f 6c6f 7266  lorfunc = colorf
+0000bb40: 756e 630d 0a20 2020 2020 2020 2073 656c  unc..        sel
+0000bb50: 662e 7265 7361 6d70 203d 2072 6573 616d  f.resamp = resam
+0000bb60: 700d 0a20 2020 2020 2020 2073 656c 662e  p..        self.
+0000bb70: 785f 6f66 6673 6574 203d 2030 0d0a 2020  x_offset = 0..  
+0000bb80: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+0000bb90: 696e 6974 5f5f 2861 782c 2064 6174 6173  init__(ax, datas
+0000bba0: 7263 2c20 6c6f 643d 5472 7565 290d 0a0d  rc, lod=True)...
+0000bbb0: 0a20 2020 2064 6566 2067 656e 6572 6174  .    def generat
+0000bbc0: 655f 7069 6374 7572 6528 7365 6c66 2c20  e_picture(self, 
+0000bbd0: 626f 756e 6469 6e67 5265 6374 293a 0d0a  boundingRect):..
+0000bbe0: 2020 2020 2020 2020 6c65 6674 2c72 6967          left,rig
+0000bbf0: 6874 203d 2062 6f75 6e64 696e 6752 6563  ht = boundingRec
+0000bc00: 742e 6c65 6674 2829 2c20 626f 756e 6469  t.left(), boundi
+0000bc10: 6e67 5265 6374 2e72 6967 6874 2829 0d0a  ngRect.right()..
+0000bc20: 2020 2020 2020 2020 7020 3d20 7365 6c66          p = self
+0000bc30: 2e70 6169 6e74 6572 0d0a 2020 2020 2020  .painter..      
+0000bc40: 2020 6466 2c6f 7269 676c 656e 203d 2073    df,origlen = s
+0000bc50: 656c 662e 6461 7461 7372 632e 726f 7773  elf.datasrc.rows
+0000bc60: 2835 2c20 6c65 6674 2c20 7269 6768 742c  (5, left, right,
+0000bc70: 2079 7363 616c 653d 7365 6c66 2e61 782e   yscale=self.ax.
+0000bc80: 7662 2e79 7363 616c 652c 2072 6573 616d  vb.yscale, resam
+0000bc90: 703d 7365 6c66 2e72 6573 616d 7029 0d0a  p=self.resamp)..
+0000bca0: 2020 2020 2020 2020 6620 3d20 6f72 6967          f = orig
+0000bcb0: 6c65 6e20 2f20 6c65 6e28 6466 2920 6966  len / len(df) if
+0000bcc0: 206c 656e 2864 6629 2065 6c73 6520 310d   len(df) else 1.
+0000bcd0: 0a20 2020 2020 2020 2077 203d 2073 656c  .        w = sel
+0000bce0: 662e 6361 6e64 6c65 5f77 6964 7468 202a  f.candle_width *
+0000bcf0: 2066 0d0a 2020 2020 2020 2020 7732 203d   f..        w2 =
+0000bd00: 2077 202a 2030 2e35 0d0a 2020 2020 2020   w * 0.5..      
+0000bd10: 2020 666f 7220 7368 6164 6f77 2c66 7261    for shadow,fra
+0000bd20: 6d65 2c62 6f64 792c 6466 5f72 6f77 7320  me,body,df_rows 
+0000bd30: 696e 2073 656c 662e 636f 6c6f 7266 756e  in self.colorfun
+0000bd40: 6328 7365 6c66 2c20 7365 6c66 2e64 6174  c(self, self.dat
+0000bd50: 6173 7263 2c20 6466 293a 0d0a 2020 2020  asrc, df):..    
+0000bd60: 2020 2020 2020 2020 6964 7873 203d 2064          idxs = d
+0000bd70: 665f 726f 7773 2e69 6e64 6578 0d0a 2020  f_rows.index..  
+0000bd80: 2020 2020 2020 2020 2020 726f 7773 203d            rows =
+0000bd90: 2064 665f 726f 7773 2e76 616c 7565 730d   df_rows.values.
+0000bda0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bdb0: 7365 6c66 2e78 5f6f 6666 7365 743a 0d0a  self.x_offset:..
+0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdd0: 6964 7873 202b 3d20 7365 6c66 2e78 5f6f  idxs += self.x_o
+0000bde0: 6666 7365 740d 0a20 2020 2020 2020 2020  ffset..         
+0000bdf0: 2020 2069 6620 7365 6c66 2e64 7261 775f     if self.draw_
+0000be00: 7368 6164 6f77 3a0d 0a20 2020 2020 2020  shadow:..       
+0000be10: 2020 2020 2020 2020 2070 2e73 6574 5065           p.setPe
+0000be20: 6e28 7067 2e6d 6b50 656e 2873 6861 646f  n(pg.mkPen(shado
+0000be30: 772c 2077 6964 7468 3d73 656c 662e 7368  w, width=self.sh
+0000be40: 6164 6f77 5f77 6964 7468 2929 0d0a 2020  adow_width))..  
+0000be50: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000be60: 7220 782c 2874 2c6f 7065 6e2c 636c 6f73  r x,(t,open,clos
+0000be70: 652c 6869 6768 2c6c 6f77 2920 696e 207a  e,high,low) in z
+0000be80: 6970 2869 6478 732c 2072 6f77 7329 3a0d  ip(idxs, rows):.
 0000be90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 2062 756c 6c5f 626f 6479 2020 2020 2020   bull_body      
-0000bec0: 203d 2063 616e 646c 655f 6275 6c6c 5f63   = candle_bull_c
-0000bed0: 6f6c 6f72 2929 0d0a 0d0a 2020 2020 6465  olor))....    de
-0000bee0: 6620 6765 6e65 7261 7465 5f70 6963 7475  f generate_pictu
-0000bef0: 7265 2873 656c 662c 2062 6f75 6e64 696e  re(self, boundin
-0000bf00: 6752 6563 7429 3a0d 0a20 2020 2020 2020  gRect):..       
-0000bf10: 2074 696d 6573 203d 2073 656c 662e 6461   times = self.da
-0000bf20: 7461 7372 632e 6466 2e69 6c6f 635b 3a2c  tasrc.df.iloc[:,
-0000bf30: 2030 5d0d 0a20 2020 2020 2020 2076 616c   0]..        val
-0000bf40: 7320 3d20 7365 6c66 2e64 6174 6173 7263  s = self.datasrc
-0000bf50: 2e64 662e 7661 6c75 6573 0d0a 2020 2020  .df.values..    
-0000bf60: 2020 2020 7072 6963 6573 203d 2076 616c      prices = val
-0000bf70: 735b 3a2c 2073 656c 662e 6461 7461 7372  s[:, self.datasr
-0000bf80: 632e 636f 6c5f 6461 7461 5f6f 6666 7365  c.col_data_offse
-0000bf90: 743a 3a32 5d0d 0a20 2020 2020 2020 2076  t::2]..        v
-0000bfa0: 6f6c 756d 6573 203d 2076 616c 735b 3a2c  olumes = vals[:,
-0000bfb0: 2073 656c 662e 6461 7461 7372 632e 636f   self.datasrc.co
-0000bfc0: 6c5f 6461 7461 5f6f 6666 7365 742b 313a  l_data_offset+1:
-0000bfd0: 3a32 5d2e 540d 0a20 2020 2020 2020 2023  :2].T..        #
-0000bfe0: 206e 6f72 6d61 6c69 7a65 0d0a 2020 2020   normalize..    
-0000bff0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-0000c000: 2020 2020 2020 6620 3d20 7365 6c66 2e64        f = self.d
-0000c010: 6174 6173 7263 2e70 6572 696f 645f 6e73  atasrc.period_ns
-0000c020: 202f 205f 6765 745f 6461 7461 7372 6328   / _get_datasrc(
-0000c030: 7365 6c66 2e61 7829 2e70 6572 696f 645f  self.ax).period_
-0000c040: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
-0000c050: 7469 6d65 7320 3d20 5f70 6474 696d 6532  times = _pdtime2
-0000c060: 696e 6465 7828 7365 6c66 2e61 782c 2074  index(self.ax, t
-0000c070: 696d 6573 2c20 7265 7175 6972 655f 7469  imes, require_ti
-0000c080: 6d65 3d54 7275 6529 0d0a 2020 2020 2020  me=True)..      
-0000c090: 2020 6578 6365 7074 2041 7373 6572 7469    except Asserti
-0000c0a0: 6f6e 4572 726f 723a 0d0a 2020 2020 2020  onError:..      
-0000c0b0: 2020 2020 2020 6620 3d20 310d 0a20 2020        f = 1..   
-0000c0c0: 2020 2020 2064 7261 775f 626f 6479 203d       draw_body =
-0000c0d0: 2073 656c 662e 6472 6177 5f62 6f64 790d   self.draw_body.
-0000c0e0: 0a20 2020 2020 2020 2069 6620 6472 6177  .        if draw
-0000c0f0: 5f62 6f64 7920 3c20 303a 0d0a 2020 2020  _body < 0:..    
-0000c100: 2020 2020 2020 2020 6620 2a3d 202d 6472          f *= -dr
-0000c110: 6177 5f62 6f64 7920 2a20 7365 6c66 2e61  aw_body * self.a
-0000c120: 782e 7662 2e74 6172 6765 7452 6563 7428  x.vb.targetRect(
-0000c130: 292e 7769 6474 6828 290d 0a20 2020 2020  ).width()..     
-0000c140: 2020 2020 2020 2064 7261 775f 626f 6479         draw_body
-0000c150: 203d 2031 0d0a 2020 2020 2020 2020 6269   = 1..        bi
-0000c160: 6e63 203d 206c 656e 2876 6f6c 756d 6573  nc = len(volumes
-0000c170: 290d 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-0000c180: 7420 6269 6e63 3a0d 0a20 2020 2020 2020  t binc:..       
-0000c190: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-0000c1a0: 2020 2020 2064 6976 766f 6c20 3d20 6e70       divvol = np
-0000c1b0: 2e6e 616e 6d61 7828 6e70 2e61 6273 2876  .nanmax(np.abs(v
-0000c1c0: 6f6c 756d 6573 292c 2061 7869 733d 3029  olumes), axis=0)
-0000c1d0: 0d0a 2020 2020 2020 2020 6469 7676 6f6c  ..        divvol
-0000c1e0: 5b64 6976 766f 6c3d 3d30 5d20 3d20 310d  [divvol==0] = 1.
-0000c1f0: 0a20 2020 2020 2020 2076 6f6c 756d 6573  .        volumes
-0000c200: 203d 2028 766f 6c75 6d65 7320 2a20 6620   = (volumes * f 
-0000c210: 2f20 6469 7676 6f6c 292e 540d 0a20 2020  / divvol).T..   
-0000c220: 2020 2020 2070 203d 2073 656c 662e 7061       p = self.pa
-0000c230: 696e 7465 720d 0a20 2020 2020 2020 2068  inter..        h
-0000c240: 203d 2031 652d 3130 0d0a 2020 2020 2020   = 1e-10..      
-0000c250: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0000c260: 286c 656e 2870 7269 6365 7329 293a 0d0a  (len(prices)):..
-0000c270: 2020 2020 2020 2020 2020 2020 7072 6372              prcr
-0000c280: 203d 2070 7269 6365 735b 695d 0d0a 2020   = prices[i]..  
-0000c290: 2020 2020 2020 2020 2020 7072 7620 3d20            prv = 
-0000c2a0: 7072 6372 5b7e 6e70 2e69 736e 616e 2870  prcr[~np.isnan(p
-0000c2b0: 7263 7229 5d0d 0a20 2020 2020 2020 2020  rcr)]..         
-0000c2c0: 2020 2069 6620 6c65 6e28 7072 7629 203e     if len(prv) >
-0000c2d0: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-0000c2e0: 2020 2020 2068 203d 206e 702e 6469 6666       h = np.diff
-0000c2f0: 2870 7276 292e 6d69 6e28 290d 0a20 2020  (prv).min()..   
-0000c300: 2020 2020 2020 2020 2074 203d 2074 696d           t = tim
-0000c310: 6573 5b69 5d0d 0a20 2020 2020 2020 2020  es[i]..         
-0000c320: 2020 2076 6f6c 7220 3d20 6e70 2e6e 616e     volr = np.nan
-0000c330: 5f74 6f5f 6e75 6d28 766f 6c75 6d65 735b  _to_num(volumes[
-0000c340: 695d 290d 0a0d 0a20 2020 2020 2020 2020  i])....         
-0000c350: 2020 2023 2063 616c 6320 706f 630d 0a20     # calc poc.. 
-0000c360: 2020 2020 2020 2020 2020 2070 6f63 6964             pocid
-0000c370: 7820 3d20 6e70 2e6e 616e 6172 676d 6178  x = np.nanargmax
-0000c380: 2876 6f6c 7229 0d0a 0d0a 2020 2020 2020  (volr)....      
-0000c390: 2020 2020 2020 2320 6472 6177 2076 616c        # draw val
-0000c3a0: 7565 2061 7265 610d 0a20 2020 2020 2020  ue area..       
-0000c3b0: 2020 2020 2069 6620 7365 6c66 2e64 7261       if self.dra
-0000c3c0: 775f 7661 3a0d 0a20 2020 2020 2020 2020  w_va:..         
-0000c3d0: 2020 2020 2020 2076 6f6c 7273 203d 2076         volrs = v
-0000c3e0: 6f6c 7220 2f20 6e70 2e6e 616e 7375 6d28  olr / np.nansum(
-0000c3f0: 766f 6c72 290d 0a20 2020 2020 2020 2020  volr)..         
-0000c400: 2020 2020 2020 2076 203d 2076 6f6c 7273         v = volrs
-0000c410: 5b70 6f63 6964 785d 0d0a 2020 2020 2020  [pocidx]..      
-0000c420: 2020 2020 2020 2020 2020 6120 3d20 6220            a = b 
-0000c430: 3d20 706f 6369 6478 0d0a 2020 2020 2020  = pocidx..      
-0000c440: 2020 2020 2020 2020 2020 7768 696c 6520            while 
-0000c450: 613e 3d30 206f 7220 623c 6269 6e63 3a0d  a>=0 or b<binc:.
-0000c460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c470: 2020 2020 2069 6620 7620 3e3d 2073 656c       if v >= sel
-0000c480: 662e 6472 6177 5f76 613a 0d0a 2020 2020  f.draw_va:..    
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000c4c0: 6120 3d20 6120 2d20 310d 0a20 2020 2020  a = a - 1..     
-0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000c4e0: 6220 3d20 6220 2b20 310d 0a20 2020 2020  b = b + 1..     
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000c500: 6120 3d20 766f 6c72 735b 6161 5d20 6966  a = volrs[aa] if
-0000c510: 2061 613e 3d30 2065 6c73 6520 300d 0a20   aa>=0 else 0.. 
-0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c530: 2020 2076 6220 3d20 766f 6c72 735b 6262     vb = volrs[bb
-0000c540: 5d20 6966 2062 623c 6269 6e63 2065 6c73  ] if bb<binc els
-0000c550: 6520 300d 0a20 2020 2020 2020 2020 2020  e 0..           
-0000c560: 2020 2020 2020 2020 2069 6620 7661 203e           if va >
-0000c570: 3d20 7662 3a20 2320 4e4f 5445 2062 6f74  = vb: # NOTE bot
-0000c580: 6820 3d3d 2069 7320 616c 736f 206f 6b0d  h == is also ok.
-0000c590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c5a0: 2020 2020 2020 2020 2061 203d 206d 6178           a = max
-0000c5b0: 2830 2c20 6161 290d 0a20 2020 2020 2020  (0, aa)..       
+0000bea0: 2020 2020 2069 6620 6869 6768 203e 206c       if high > l
+0000beb0: 6f77 3a0d 0a20 2020 2020 2020 2020 2020  ow:..           
+0000bec0: 2020 2020 2020 2020 2020 2020 2070 2e64               p.d
+0000bed0: 7261 774c 696e 6528 5174 436f 7265 2e51  rawLine(QtCore.Q
+0000bee0: 506f 696e 7446 2878 2c20 6c6f 7729 2c20  PointF(x, low), 
+0000bef0: 5174 436f 7265 2e51 506f 696e 7446 2878  QtCore.QPointF(x
+0000bf00: 2c20 6869 6768 2929 0d0a 2020 2020 2020  , high))..      
+0000bf10: 2020 2020 2020 6966 2073 656c 662e 6472        if self.dr
+0000bf20: 6177 5f62 6f64 793a 0d0a 2020 2020 2020  aw_body:..      
+0000bf30: 2020 2020 2020 2020 2020 702e 7365 7450            p.setP
+0000bf40: 656e 2870 672e 6d6b 5065 6e28 6672 616d  en(pg.mkPen(fram
+0000bf50: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+0000bf60: 2020 2020 2070 2e73 6574 4272 7573 6828       p.setBrush(
+0000bf70: 7067 2e6d 6b42 7275 7368 2862 6f64 7929  pg.mkBrush(body)
+0000bf80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000bf90: 2020 2066 6f72 2078 2c28 742c 6f70 656e     for x,(t,open
+0000bfa0: 2c63 6c6f 7365 2c68 6967 682c 6c6f 7729  ,close,high,low)
+0000bfb0: 2069 6e20 7a69 7028 6964 7873 2c20 726f   in zip(idxs, ro
+0000bfc0: 7773 293a 0d0a 2020 2020 2020 2020 2020  ws):..          
+0000bfd0: 2020 2020 2020 2020 2020 702e 6472 6177            p.draw
+0000bfe0: 5265 6374 2851 7443 6f72 652e 5152 6563  Rect(QtCore.QRec
+0000bff0: 7446 2878 2d77 322c 206f 7065 6e2c 2077  tF(x-w2, open, w
+0000c000: 2c20 636c 6f73 652d 6f70 656e 2929 0d0a  , close-open))..
+0000c010: 0d0a 2020 2020 6465 6620 726f 7763 6f6c  ..    def rowcol
+0000c020: 6f72 7328 7365 6c66 2c20 7072 6566 6978  ors(self, prefix
+0000c030: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+0000c040: 726e 205b 7365 6c66 2e63 6f6c 6f72 735b  rn [self.colors[
+0000c050: 7072 6566 6978 2b27 5f73 6861 646f 7727  prefix+'_shadow'
+0000c060: 5d2c 2073 656c 662e 636f 6c6f 7273 5b70  ], self.colors[p
+0000c070: 7265 6669 782b 275f 6672 616d 6527 5d2c  refix+'_frame'],
+0000c080: 2073 656c 662e 636f 6c6f 7273 5b70 7265   self.colors[pre
+0000c090: 6669 782b 275f 626f 6479 275d 5d0d 0a0d  fix+'_body']]...
+0000c0a0: 0a0d 0a0d 0a63 6c61 7373 2048 6561 746d  .....class Heatm
+0000c0b0: 6170 4974 656d 2846 696e 506c 6f74 4974  apItem(FinPlotIt
+0000c0c0: 656d 293a 0d0a 2020 2020 6465 6620 5f5f  em):..    def __
+0000c0d0: 696e 6974 5f5f 2873 656c 662c 2061 782c  init__(self, ax,
+0000c0e0: 2064 6174 6173 7263 2c20 7265 6374 5f73   datasrc, rect_s
+0000c0f0: 697a 653d 302e 392c 2066 696c 7465 725f  ize=0.9, filter_
+0000c100: 6c69 6d69 743d 302c 2063 6f6c 6d61 703d  limit=0, colmap=
+0000c110: 636f 6c6d 6170 5f63 6c61 7368 2c20 7768  colmap_clash, wh
+0000c120: 6974 656f 7574 3d30 2e30 2c20 636f 6c63  iteout=0.0, colc
+0000c130: 7572 7665 3d6c 616d 6264 6120 783a 706f  urve=lambda x:po
+0000c140: 7728 782c 3429 293a 0d0a 2020 2020 2020  w(x,4)):..      
+0000c150: 2020 7365 6c66 2e72 6563 745f 7369 7a65    self.rect_size
+0000c160: 203d 2072 6563 745f 7369 7a65 0d0a 2020   = rect_size..  
+0000c170: 2020 2020 2020 7365 6c66 2e66 696c 7465        self.filte
+0000c180: 725f 6c69 6d69 7420 3d20 6669 6c74 6572  r_limit = filter
+0000c190: 5f6c 696d 6974 0d0a 2020 2020 2020 2020  _limit..        
+0000c1a0: 7365 6c66 2e63 6f6c 6d61 7020 3d20 636f  self.colmap = co
+0000c1b0: 6c6d 6170 0d0a 2020 2020 2020 2020 7365  lmap..        se
+0000c1c0: 6c66 2e77 6869 7465 6f75 7420 3d20 7768  lf.whiteout = wh
+0000c1d0: 6974 656f 7574 0d0a 2020 2020 2020 2020  iteout..        
+0000c1e0: 7365 6c66 2e63 6f6c 6375 7276 6520 3d20  self.colcurve = 
+0000c1f0: 636f 6c63 7572 7665 0d0a 2020 2020 2020  colcurve..      
+0000c200: 2020 7365 6c66 2e63 6f6c 5f64 6174 615f    self.col_data_
+0000c210: 656e 6420 3d20 6c65 6e28 6461 7461 7372  end = len(datasr
+0000c220: 632e 6466 2e63 6f6c 756d 6e73 290d 0a20  c.df.columns).. 
+0000c230: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+0000c240: 5f69 6e69 745f 5f28 6178 2c20 6461 7461  _init__(ax, data
+0000c250: 7372 632c 206c 6f64 3d46 616c 7365 290d  src, lod=False).
+0000c260: 0a0d 0a20 2020 2064 6566 2067 656e 6572  ...    def gener
+0000c270: 6174 655f 7069 6374 7572 6528 7365 6c66  ate_picture(self
+0000c280: 2c20 626f 756e 6469 6e67 5265 6374 293a  , boundingRect):
+0000c290: 0d0a 2020 2020 2020 2020 7072 6963 6573  ..        prices
+0000c2a0: 203d 2073 656c 662e 6461 7461 7372 632e   = self.datasrc.
+0000c2b0: 6466 2e63 6f6c 756d 6e73 5b73 656c 662e  df.columns[self.
+0000c2c0: 6461 7461 7372 632e 636f 6c5f 6461 7461  datasrc.col_data
+0000c2d0: 5f6f 6666 7365 743a 7365 6c66 2e63 6f6c  _offset:self.col
+0000c2e0: 5f64 6174 615f 656e 645d 0d0a 2020 2020  _data_end]..    
+0000c2f0: 2020 2020 6830 203d 2028 7072 6963 6573      h0 = (prices
+0000c300: 5b30 5d20 2d20 7072 6963 6573 5b31 5d29  [0] - prices[1])
+0000c310: 202a 2028 312d 7365 6c66 2e72 6563 745f   * (1-self.rect_
+0000c320: 7369 7a65 290d 0a20 2020 2020 2020 2068  size)..        h
+0000c330: 3120 3d20 2870 7269 6365 735b 305d 202d  1 = (prices[0] -
+0000c340: 2070 7269 6365 735b 315d 2920 2a20 2831   prices[1]) * (1
+0000c350: 2d28 312d 7365 6c66 2e72 6563 745f 7369  -(1-self.rect_si
+0000c360: 7a65 292a 3229 0d0a 2020 2020 2020 2020  ze)*2)..        
+0000c370: 7265 6374 5f73 697a 6532 203d 2030 2e35  rect_size2 = 0.5
+0000c380: 202a 2073 656c 662e 7265 6374 5f73 697a   * self.rect_siz
+0000c390: 650d 0a20 2020 2020 2020 2064 6620 3d20  e..        df = 
+0000c3a0: 7365 6c66 2e64 6174 6173 7263 2e64 662e  self.datasrc.df.
+0000c3b0: 696c 6f63 5b3a 2c20 7365 6c66 2e64 6174  iloc[:, self.dat
+0000c3c0: 6173 7263 2e63 6f6c 5f64 6174 615f 6f66  asrc.col_data_of
+0000c3d0: 6673 6574 3a73 656c 662e 636f 6c5f 6461  fset:self.col_da
+0000c3e0: 7461 5f65 6e64 5d0d 0a20 2020 2020 2020  ta_end]..       
+0000c3f0: 2076 616c 7565 7320 3d20 6466 2e76 616c   values = df.val
+0000c400: 7565 730d 0a20 2020 2020 2020 2023 206e  ues..        # n
+0000c410: 6f72 6d61 6c69 7a65 0d0a 2020 2020 2020  ormalize..      
+0000c420: 2020 7661 6c75 6573 202d 3d20 6e70 2e6e    values -= np.n
+0000c430: 616e 6d69 6e28 7661 6c75 6573 290d 0a20  anmin(values).. 
+0000c440: 2020 2020 2020 2076 616c 7565 7320 3d20         values = 
+0000c450: 7661 6c75 6573 202f 2028 6e70 2e6e 616e  values / (np.nan
+0000c460: 6d61 7828 7661 6c75 6573 2920 2f20 2831  max(values) / (1
+0000c470: 2b73 656c 662e 7768 6974 656f 7574 2929  +self.whiteout))
+0000c480: 2023 206f 7665 7273 686f 6f74 2066 6f72   # overshoot for
+0000c490: 2063 6f6c 6f72 696e 670d 0a20 2020 2020   coloring..     
+0000c4a0: 2020 206c 696d 203d 2073 656c 662e 6669     lim = self.fi
+0000c4b0: 6c74 6572 5f6c 696d 6974 202a 2028 312b  lter_limit * (1+
+0000c4c0: 7365 6c66 2e77 6869 7465 6f75 7429 0d0a  self.whiteout)..
+0000c4d0: 2020 2020 2020 2020 7020 3d20 7365 6c66          p = self
+0000c4e0: 2e70 6169 6e74 6572 0d0a 2020 2020 2020  .painter..      
+0000c4f0: 2020 666f 7220 742c 726f 7720 696e 2065    for t,row in e
+0000c500: 6e75 6d65 7261 7465 2876 616c 7565 7329  numerate(values)
+0000c510: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+0000c520: 6f72 2063 692c 7072 6963 6520 696e 2065  or ci,price in e
+0000c530: 6e75 6d65 7261 7465 2870 7269 6365 7329  numerate(prices)
+0000c540: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000c550: 2020 2076 203d 2072 6f77 5b63 695d 0d0a     v = row[ci]..
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 6966 2076 203e 3d20 6c69 6d3a 0d0a 2020  if v >= lim:..  
+0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c590: 2020 7620 3d20 3120 2d20 7365 6c66 2e63    v = 1 - self.c
+0000c5a0: 6f6c 6375 7276 6528 3120 2d20 2876 2d6c  olcurve(1 - (v-l
+0000c5b0: 696d 292f 2831 2d6c 696d 2929 0d0a 2020  im)/(1-lim))..  
 0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2076 202b 3d20 7661 0d0a 2020 2020 2020   v += va..      
-0000c5e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c5f0: 2076 6120 3c3d 2076 623a 2023 204e 4f54   va <= vb: # NOT
-0000c600: 4520 626f 7468 203d 3d20 6973 2061 6c73  E both == is als
-0000c610: 6f20 6f6b 0d0a 2020 2020 2020 2020 2020  o ok..          
-0000c620: 2020 2020 2020 2020 2020 2020 2020 6220                b 
-0000c630: 3d20 6d69 6e28 6269 6e63 2d31 2c20 6262  = min(binc-1, bb
-0000c640: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000c650: 2020 2020 2020 2020 2020 2076 202b 3d20             v += 
-0000c660: 7662 0d0a 2020 2020 2020 2020 2020 2020  vb..            
-0000c670: 2020 2020 636f 6c6f 7220 3d20 7067 2e6d      color = pg.m
-0000c680: 6b43 6f6c 6f72 2862 616e 645f 636f 6c6f  kColor(band_colo
-0000c690: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
-0000c6a0: 2020 2020 702e 6669 6c6c 5265 6374 2851      p.fillRect(Q
-0000c6b0: 7443 6f72 652e 5152 6563 7446 2874 2c20  tCore.QRectF(t, 
-0000c6c0: 7072 6372 5b61 5d2c 2066 2c20 7072 6372  prcr[a], f, prcr
-0000c6d0: 5b62 5d2d 7072 6372 5b61 5d2b 6829 2c20  [b]-prcr[a]+h), 
-0000c6e0: 636f 6c6f 7229 0d0a 0d0a 2020 2020 2020  color)....      
-0000c6f0: 2020 2020 2020 2320 6472 6177 2068 6f72        # draw hor
-0000c700: 697a 6f6e 7461 6c20 6261 7273 0d0a 2020  izontal bars..  
-0000c710: 2020 2020 2020 2020 2020 6966 2064 7261            if dra
-0000c720: 775f 626f 6479 3a0d 0a20 2020 2020 2020  w_body:..       
-0000c730: 2020 2020 2020 2020 2068 3020 3d20 6820           h0 = h 
-0000c740: 2a20 2831 2d73 656c 662e 6361 6e64 6c65  * (1-self.candle
-0000c750: 5f77 6964 7468 292f 320d 0a20 2020 2020  _width)/2..     
-0000c760: 2020 2020 2020 2020 2020 2068 3120 3d20             h1 = 
-0000c770: 6820 2a20 7365 6c66 2e63 616e 646c 655f  h * self.candle_
-0000c780: 7769 6474 680d 0a20 2020 2020 2020 2020  width..         
-0000c790: 2020 2020 2020 2066 6f72 2073 6861 646f         for shado
-0000c7a0: 772c 6672 616d 652c 626f 6479 2c64 6174  w,frame,body,dat
-0000c7b0: 6120 696e 2073 656c 662e 636f 6c6f 7266  a in self.colorf
-0000c7c0: 756e 6328 7365 6c66 2c20 7365 6c66 2e64  unc(self, self.d
-0000c7d0: 6174 6173 7263 2c20 6e70 2e61 7272 6179  atasrc, np.array
-0000c7e0: 285b 7072 6372 2c20 766f 6c72 5d29 293a  ([prcr, volr])):
-0000c7f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c800: 2020 2020 2020 702e 7365 7450 656e 2870        p.setPen(p
-0000c810: 672e 6d6b 5065 6e28 6672 616d 6529 290d  g.mkPen(frame)).
-0000c820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c830: 2020 2020 2070 2e73 6574 4272 7573 6828       p.setBrush(
-0000c840: 7067 2e6d 6b42 7275 7368 2862 6f64 7929  pg.mkBrush(body)
-0000c850: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000c860: 2020 2020 2020 2070 7263 725f 2c76 6f6c         prcr_,vol
-0000c870: 725f 203d 2064 6174 610d 0a20 2020 2020  r_ = data..     
-0000c880: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c890: 6f72 2077 2c79 2069 6e20 7a69 7028 766f  or w,y in zip(vo
-0000c8a0: 6c72 5f2c 2070 7263 725f 293a 0d0a 2020  lr_, prcr_):..  
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8c0: 2020 2020 2020 6966 2061 6273 2877 2920        if abs(w) 
-0000c8d0: 3e20 3165 2d31 353a 0d0a 2020 2020 2020  > 1e-15:..      
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8f0: 2020 2020 2020 702e 6472 6177 5265 6374        p.drawRect
-0000c900: 2851 7443 6f72 652e 5152 6563 7446 2874  (QtCore.QRectF(t
-0000c910: 2c20 792b 6830 2c20 772a 6472 6177 5f62  , y+h0, w*draw_b
-0000c920: 6f64 792c 2068 3129 290d 0a0d 0a20 2020  ody, h1))....   
-0000c930: 2020 2020 2020 2020 2023 2064 7261 7720           # draw 
-0000c940: 706f 6320 6c69 6e65 0d0a 2020 2020 2020  poc line..      
-0000c950: 2020 2020 2020 6966 2073 656c 662e 6472        if self.dr
-0000c960: 6177 5f70 6f63 3a0d 0a20 2020 2020 2020  aw_poc:..       
-0000c970: 2020 2020 2020 2020 2079 203d 2070 7263           y = prc
-0000c980: 725b 706f 6369 6478 5d20 2b20 6820 2f20  r[pocidx] + h / 
-0000c990: 320d 0a20 2020 2020 2020 2020 2020 2020  2..             
-0000c9a0: 2020 2070 2e73 6574 5065 6e28 7067 2e6d     p.setPen(pg.m
-0000c9b0: 6b50 656e 2870 6f63 5f63 6f6c 6f72 2929  kPen(poc_color))
-0000c9c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c9d0: 2020 702e 6472 6177 4c69 6e65 2851 7443    p.drawLine(QtC
-0000c9e0: 6f72 652e 5150 6f69 6e74 4628 742c 2079  ore.QPointF(t, y
-0000c9f0: 292c 2051 7443 6f72 652e 5150 6f69 6e74  ), QtCore.QPoint
-0000ca00: 4628 742b 662a 7365 6c66 2e64 7261 775f  F(t+f*self.draw_
-0000ca10: 706f 632c 2079 2929 0d0a 0d0a 0d0a 0d0a  poc, y))........
-0000ca20: 636c 6173 7320 5363 6174 7465 724c 6162  class ScatterLab
-0000ca30: 656c 4974 656d 2846 696e 506c 6f74 4974  elItem(FinPlotIt
-0000ca40: 656d 293a 0d0a 2020 2020 6465 6620 5f5f  em):..    def __
-0000ca50: 696e 6974 5f5f 2873 656c 662c 2061 782c  init__(self, ax,
-0000ca60: 2064 6174 6173 7263 2c20 636f 6c6f 722c   datasrc, color,
-0000ca70: 2061 6e63 686f 7229 3a0d 0a20 2020 2020   anchor):..     
-0000ca80: 2020 2073 656c 662e 636f 6c6f 7220 3d20     self.color = 
-0000ca90: 636f 6c6f 720d 0a20 2020 2020 2020 2073  color..        s
-0000caa0: 656c 662e 7465 7874 5f69 7465 6d73 203d  elf.text_items =
-0000cab0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-0000cac0: 662e 616e 6368 6f72 203d 2061 6e63 686f  f.anchor = ancho
-0000cad0: 720d 0a20 2020 2020 2020 2073 656c 662e  r..        self.
-0000cae0: 7368 6f77 203d 2046 616c 7365 0d0a 2020  show = False..  
-0000caf0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-0000cb00: 696e 6974 5f5f 2861 782c 2064 6174 6173  init__(ax, datas
-0000cb10: 7263 2c20 6c6f 643d 5472 7565 290d 0a0d  rc, lod=True)...
-0000cb20: 0a20 2020 2064 6566 2067 656e 6572 6174  .    def generat
-0000cb30: 655f 7069 6374 7572 6528 7365 6c66 2c20  e_picture(self, 
-0000cb40: 626f 756e 6469 6e67 5f72 6563 7429 3a0d  bounding_rect):.
-0000cb50: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-0000cb60: 7365 6c66 2e67 6574 726f 7773 2862 6f75  self.getrows(bou
-0000cb70: 6e64 696e 675f 7265 6374 290d 0a20 2020  nding_rect)..   
-0000cb80: 2020 2020 2069 6620 6c65 6e28 726f 7773       if len(rows
-0000cb90: 2920 3e20 6c6f 645f 6c61 6265 6c73 3a20  ) > lod_labels: 
-0000cba0: 2320 646f 6e27 7420 6576 656e 2067 656e  # don't even gen
-0000cbb0: 6572 6174 6520 7768 656e 2074 6865 7265  erate when there
-0000cbc0: 2773 2074 6f6f 206d 616e 7920 6f66 2074  's too many of t
-0000cbd0: 6865 6d0d 0a20 2020 2020 2020 2020 2020  hem..           
-0000cbe0: 2073 656c 662e 636c 6561 725f 6974 656d   self.clear_item
-0000cbf0: 7328 6c69 7374 2873 656c 662e 7465 7874  s(list(self.text
-0000cc00: 5f69 7465 6d73 2e6b 6579 7328 2929 290d  _items.keys())).
-0000cc10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000cc20: 7572 6e0d 0a20 2020 2020 2020 2064 726f  urn..        dro
-0000cc30: 7073 203d 2073 6574 2873 656c 662e 7465  ps = set(self.te
-0000cc40: 7874 5f69 7465 6d73 2e6b 6579 7328 2929  xt_items.keys())
-0000cc50: 0d0a 2020 2020 2020 2020 6372 6561 7465  ..        create
-0000cc60: 6420 3d20 300d 0a20 2020 2020 2020 2066  d = 0..        f
-0000cc70: 6f72 2078 2c74 2c79 2c74 7874 2069 6e20  or x,t,y,txt in 
-0000cc80: 726f 7773 3a0d 0a20 2020 2020 2020 2020  rows:..         
-0000cc90: 2020 2074 7874 203d 2073 7472 2874 7874     txt = str(txt
-0000cca0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0000ccb0: 7368 746d 6c20 3d20 273c 2720 696e 2074  shtml = '<' in t
-0000ccc0: 7874 2061 6e64 2027 3e27 2069 6e20 7478  xt and '>' in tx
-0000ccd0: 740d 0a20 2020 2020 2020 2020 2020 206b  t..            k
-0000cce0: 6579 203d 2027 2573 3a25 2e38 6627 2025  ey = '%s:%.8f' %
-0000ccf0: 2028 742c 2079 290d 0a20 2020 2020 2020   (t, y)..       
-0000cd00: 2020 2020 2069 6620 6b65 7920 696e 2073       if key in s
-0000cd10: 656c 662e 7465 7874 5f69 7465 6d73 3a0d  elf.text_items:.
-0000cd20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd30: 2069 7465 6d20 3d20 7365 6c66 2e74 6578   item = self.tex
-0000cd40: 745f 6974 656d 735b 6b65 795d 0d0a 2020  t_items[key]..  
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2869                (i
-0000cd60: 7465 6d2e 7365 7448 746d 6c20 6966 2069  tem.setHtml if i
-0000cd70: 7368 746d 6c20 656c 7365 2069 7465 6d2e  shtml else item.
-0000cd80: 7365 7454 6578 7429 2874 7874 290d 0a20  setText)(txt).. 
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000cda0: 7465 6d2e 7365 7450 6f73 2878 2c20 7929  tem.setPos(x, y)
-0000cdb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cdc0: 2020 6472 6f70 732e 7265 6d6f 7665 286b    drops.remove(k
-0000cdd0: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
-0000cde0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0000cdf0: 2020 2020 2020 2020 6b77 7320 3d20 7b27          kws = {'
-0000ce00: 6874 6d6c 273a 7478 747d 2069 6620 6973  html':txt} if is
-0000ce10: 6874 6d6c 2065 6c73 6520 7b27 7465 7874  html else {'text
-0000ce20: 273a 7478 747d 0d0a 2020 2020 2020 2020  ':txt}..        
-0000ce30: 2020 2020 2020 2020 7365 6c66 2e74 6578          self.tex
-0000ce40: 745f 6974 656d 735b 6b65 795d 203d 2069  t_items[key] = i
-0000ce50: 7465 6d20 3d20 7067 2e54 6578 7449 7465  tem = pg.TextIte
-0000ce60: 6d28 636f 6c6f 723d 7365 6c66 2e63 6f6c  m(color=self.col
-0000ce70: 6f72 2c20 616e 6368 6f72 3d73 656c 662e  or, anchor=self.
-0000ce80: 616e 6368 6f72 2c20 2a2a 6b77 7329 0d0a  anchor, **kws)..
-0000ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cea0: 6974 656d 2e73 6574 506f 7328 782c 2079  item.setPos(x, y
-0000ceb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000cec0: 2020 2069 7465 6d2e 7365 7450 6172 656e     item.setParen
-0000ced0: 7449 7465 6d28 7365 6c66 290d 0a20 2020  tItem(self)..   
-0000cee0: 2020 2020 2020 2020 2020 2020 2063 7265               cre
-0000cef0: 6174 6564 202b 3d20 310d 0a20 2020 2020  ated += 1..     
-0000cf00: 2020 2069 6620 6372 6561 7465 6420 3e20     if created > 
-0000cf10: 3020 6f72 2073 656c 662e 6469 7274 793a  0 or self.dirty:
-0000cf20: 2023 206f 6e6c 7920 7265 6475 6365 2063   # only reduce c
-0000cf30: 6163 6865 2069 6620 7765 2776 6520 6164  ache if we've ad
-0000cf40: 6465 6420 736f 6d65 206e 6577 206f 7220  ded some new or 
-0000cf50: 7570 6461 7465 640d 0a20 2020 2020 2020  updated..       
-0000cf60: 2020 2020 2073 656c 662e 636c 6561 725f       self.clear_
-0000cf70: 6974 656d 7328 6472 6f70 7329 0d0a 0d0a  items(drops)....
-0000cf80: 2020 2020 6465 6620 636c 6561 725f 6974      def clear_it
-0000cf90: 656d 7328 7365 6c66 2c20 6472 6f70 5f6b  ems(self, drop_k
-0000cfa0: 6579 7329 3a0d 0a20 2020 2020 2020 2066  eys):..        f
-0000cfb0: 6f72 206b 6579 2069 6e20 6472 6f70 5f6b  or key in drop_k
-0000cfc0: 6579 733a 0d0a 2020 2020 2020 2020 2020  eys:..          
-0000cfd0: 2020 6974 656d 203d 2073 656c 662e 7465    item = self.te
-0000cfe0: 7874 5f69 7465 6d73 5b6b 6579 5d0d 0a20  xt_items[key].. 
-0000cff0: 2020 2020 2020 2020 2020 2069 7465 6d2e             item.
-0000d000: 7363 656e 6528 292e 7265 6d6f 7665 4974  scene().removeIt
-0000d010: 656d 2869 7465 6d29 0d0a 2020 2020 2020  em(item)..      
-0000d020: 2020 2020 2020 6465 6c20 7365 6c66 2e74        del self.t
-0000d030: 6578 745f 6974 656d 735b 6b65 795d 0d0a  ext_items[key]..
-0000d040: 0d0a 2020 2020 6465 6620 6765 7472 6f77  ..    def getrow
-0000d050: 7328 7365 6c66 2c20 626f 756e 6469 6e67  s(self, bounding
-0000d060: 5f72 6563 7429 3a0d 0a20 2020 2020 2020  _rect):..       
-0000d070: 206c 6566 742c 7269 6768 7420 3d20 626f   left,right = bo
-0000d080: 756e 6469 6e67 5f72 6563 742e 6c65 6674  unding_rect.left
-0000d090: 2829 2c20 626f 756e 6469 6e67 5f72 6563  (), bounding_rec
-0000d0a0: 742e 7269 6768 7428 290d 0a20 2020 2020  t.right()..     
-0000d0b0: 2020 2064 662c 5f20 3d20 7365 6c66 2e64     df,_ = self.d
-0000d0c0: 6174 6173 7263 2e72 6f77 7328 332c 206c  atasrc.rows(3, l
-0000d0d0: 6566 742c 2072 6967 6874 2c20 7973 6361  eft, right, ysca
-0000d0e0: 6c65 3d73 656c 662e 6178 2e76 622e 7973  le=self.ax.vb.ys
-0000d0f0: 6361 6c65 2c20 6c6f 643d 4661 6c73 6529  cale, lod=False)
-0000d100: 0d0a 2020 2020 2020 2020 726f 7773 203d  ..        rows =
-0000d110: 2064 662e 6472 6f70 6e61 2829 0d0a 2020   df.dropna()..  
-0000d120: 2020 2020 2020 6964 7873 203d 2072 6f77        idxs = row
-0000d130: 732e 696e 6465 780d 0a20 2020 2020 2020  s.index..       
-0000d140: 2072 6f77 7320 3d20 726f 7773 2e76 616c   rows = rows.val
-0000d150: 7565 730d 0a20 2020 2020 2020 2072 6f77  ues..        row
-0000d160: 7320 3d20 5b28 692c 742c 792c 7478 7429  s = [(i,t,y,txt)
-0000d170: 2066 6f72 2069 2c28 742c 792c 7478 7429   for i,(t,y,txt)
-0000d180: 2069 6e20 7a69 7028 6964 7873 2c20 726f   in zip(idxs, ro
-0000d190: 7773 2920 6966 2074 7874 5d0d 0a20 2020  ws) if txt]..   
-0000d1a0: 2020 2020 2072 6574 7572 6e20 726f 7773       return rows
-0000d1b0: 0d0a 0d0a 2020 2020 6465 6620 626f 756e  ....    def boun
-0000d1c0: 6469 6e67 5265 6374 2873 656c 6629 3a0d  dingRect(self):.
-0000d1d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000d1e0: 7365 6c66 2e76 6965 7752 6563 7428 290d  self.viewRect().
-0000d1f0: 0a0d 0a0d 0a64 6566 2063 7265 6174 655f  .....def create_
-0000d200: 706c 6f74 2874 6974 6c65 3d27 4669 6e61  plot(title='Fina
-0000d210: 6e63 6520 506c 6f74 272c 2072 6f77 733d  nce Plot', rows=
-0000d220: 312c 2069 6e69 745f 7a6f 6f6d 5f70 6572  1, init_zoom_per
-0000d230: 696f 6473 3d31 6531 302c 206d 6178 696d  iods=1e10, maxim
-0000d240: 697a 653d 5472 7565 2c20 7973 6361 6c65  ize=True, yscale
-0000d250: 3d27 6c69 6e65 6172 2729 3a0d 0a20 2020  ='linear'):..   
-0000d260: 2070 672e 7365 7443 6f6e 6669 674f 7074   pg.setConfigOpt
-0000d270: 696f 6e73 2866 6f72 6567 726f 756e 643d  ions(foreground=
-0000d280: 666f 7265 6772 6f75 6e64 2c20 6261 636b  foreground, back
-0000d290: 6772 6f75 6e64 3d62 6163 6b67 726f 756e  ground=backgroun
-0000d2a0: 6429 0d0a 2020 2020 7769 6e20 3d20 4669  d)..    win = Fi
-0000d2b0: 6e57 696e 646f 7728 7469 746c 6529 0d0a  nWindow(title)..
-0000d2c0: 2020 2020 2320 6e6f 726d 616c 6c79 2066      # normally f
-0000d2d0: 6972 7374 2067 7261 7068 2069 7320 6f66  irst graph is of
-0000d2e0: 2068 6967 6865 7220 7369 676e 6966 6963   higher signific
-0000d2f0: 616e 6365 2c20 736f 2065 6e6c 6172 6765  ance, so enlarge
-0000d300: 0d0a 2020 2020 7769 6e2e 6369 2e6c 6179  ..    win.ci.lay
-0000d310: 6f75 742e 7365 7452 6f77 5374 7265 7463  out.setRowStretc
-0000d320: 6846 6163 746f 7228 302c 2074 6f70 5f67  hFactor(0, top_g
-0000d330: 7261 7068 5f73 6361 6c65 290d 0a20 2020  raph_scale)..   
-0000d340: 2077 696e 2e73 686f 775f 6d61 7869 6d69   win.show_maximi
-0000d350: 7a65 6420 3d20 6d61 7869 6d69 7a65 0d0a  zed = maximize..
-0000d360: 2020 2020 6178 3020 3d20 6178 7320 3d20      ax0 = axs = 
-0000d370: 6372 6561 7465 5f70 6c6f 745f 7769 6467  create_plot_widg
-0000d380: 6574 286d 6173 7465 723d 7769 6e2c 2072  et(master=win, r
-0000d390: 6f77 733d 726f 7773 2c20 696e 6974 5f7a  ows=rows, init_z
-0000d3a0: 6f6f 6d5f 7065 7269 6f64 733d 696e 6974  oom_periods=init
-0000d3b0: 5f7a 6f6f 6d5f 7065 7269 6f64 732c 2079  _zoom_periods, y
-0000d3c0: 7363 616c 653d 7973 6361 6c65 290d 0a20  scale=yscale).. 
-0000d3d0: 2020 2061 7873 203d 2061 7873 2069 6620     axs = axs if 
-0000d3e0: 7479 7065 2861 7873 2920 696e 2028 7475  type(axs) in (tu
-0000d3f0: 706c 652c 6c69 7374 2920 656c 7365 205b  ple,list) else [
-0000d400: 6178 735d 0d0a 2020 2020 666f 7220 6178  axs]..    for ax
-0000d410: 2069 6e20 6178 733a 0d0a 2020 2020 2020   in axs:..      
-0000d420: 2020 7769 6e2e 6164 6449 7465 6d28 6178    win.addItem(ax
-0000d430: 2c20 636f 6c3d 3129 0d0a 2020 2020 2020  , col=1)..      
-0000d440: 2020 7769 6e2e 6e65 7874 526f 7728 290d    win.nextRow().
-0000d450: 0a20 2020 2072 6574 7572 6e20 6178 300d  .    return ax0.
-0000d460: 0a0d 0a0d 0a64 6566 2063 7265 6174 655f  .....def create_
-0000d470: 706c 6f74 5f77 6964 6765 7428 6d61 7374  plot_widget(mast
-0000d480: 6572 2c20 726f 7773 3d31 2c20 696e 6974  er, rows=1, init
-0000d490: 5f7a 6f6f 6d5f 7065 7269 6f64 733d 3165  _zoom_periods=1e
-0000d4a0: 3130 2c20 7973 6361 6c65 3d27 6c69 6e65  10, yscale='line
-0000d4b0: 6172 2729 3a0d 0a20 2020 2070 672e 7365  ar'):..    pg.se
-0000d4c0: 7443 6f6e 6669 674f 7074 696f 6e73 2866  tConfigOptions(f
-0000d4d0: 6f72 6567 726f 756e 643d 666f 7265 6772  oreground=foregr
-0000d4e0: 6f75 6e64 2c20 6261 636b 6772 6f75 6e64  ound, background
-0000d4f0: 3d62 6163 6b67 726f 756e 6429 0d0a 2020  =background)..  
-0000d500: 2020 676c 6f62 616c 206c 6173 745f 6178    global last_ax
-0000d510: 0d0a 2020 2020 6966 206d 6173 7465 7220  ..    if master 
-0000d520: 6e6f 7420 696e 2077 696e 646f 7773 3a0d  not in windows:.
-0000d530: 0a20 2020 2020 2020 2077 696e 646f 7773  .        windows
-0000d540: 2e61 7070 656e 6428 6d61 7374 6572 290d  .append(master).
-0000d550: 0a20 2020 2061 7873 203d 205b 5d0d 0a20  .    axs = [].. 
-0000d560: 2020 2070 7265 765f 6178 203d 204e 6f6e     prev_ax = Non
-0000d570: 650d 0a20 2020 2066 6f72 206e 2069 6e20  e..    for n in 
-0000d580: 7261 6e67 6528 726f 7773 293a 0d0a 2020  range(rows):..  
-0000d590: 2020 2020 2020 7973 6320 3d20 7973 6361        ysc = ysca
-0000d5a0: 6c65 5b6e 5d20 6966 2074 7970 6528 7973  le[n] if type(ys
-0000d5b0: 6361 6c65 2920 696e 2028 6c69 7374 2c74  cale) in (list,t
-0000d5c0: 7570 6c65 2920 656c 7365 2079 7363 616c  uple) else yscal
-0000d5d0: 650d 0a20 2020 2020 2020 2079 7363 203d  e..        ysc =
-0000d5e0: 2059 5363 616c 6528 7973 632c 2031 290d   YScale(ysc, 1).
-0000d5f0: 0a20 2020 2020 2020 2076 6965 7762 6f78  .        viewbox
-0000d600: 203d 2046 696e 5669 6577 426f 7828 6d61   = FinViewBox(ma
-0000d610: 7374 6572 2c20 696e 6974 5f73 7465 7073  ster, init_steps
-0000d620: 3d69 6e69 745f 7a6f 6f6d 5f70 6572 696f  =init_zoom_perio
-0000d630: 6473 2c20 7973 6361 6c65 3d79 7363 2c20  ds, yscale=ysc, 
-0000d640: 765f 7a6f 6f6d 5f73 6361 6c65 3d31 2d79  v_zoom_scale=1-y
-0000d650: 5f70 6164 2c20 656e 6162 6c65 4d65 6e75  _pad, enableMenu
-0000d660: 3d46 616c 7365 290d 0a20 2020 2020 2020  =False)..       
-0000d670: 2061 7820 3d20 7072 6576 5f61 7820 3d20   ax = prev_ax = 
-0000d680: 5f61 6464 5f74 696d 6573 7461 6d70 5f70  _add_timestamp_p
-0000d690: 6c6f 7428 6d61 7374 6572 3d6d 6173 7465  lot(master=maste
-0000d6a0: 722c 2070 7265 765f 6178 3d70 7265 765f  r, prev_ax=prev_
-0000d6b0: 6178 2c20 7669 6577 626f 783d 7669 6577  ax, viewbox=view
-0000d6c0: 626f 782c 2069 6e64 6578 3d6e 2c20 7973  box, index=n, ys
-0000d6d0: 6361 6c65 3d79 7363 290d 0a20 2020 2020  cale=ysc)..     
-0000d6e0: 2020 2069 6620 6178 733a 0d0a 2020 2020     if axs:..    
-0000d6f0: 2020 2020 2020 2020 6178 2e73 6574 584c          ax.setXL
-0000d700: 696e 6b28 6178 735b 305d 2e76 6229 0d0a  ink(axs[0].vb)..
-0000d710: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000d720: 2020 2020 2020 2020 2020 2076 6965 7762             viewb
-0000d730: 6f78 2e73 6574 466f 6375 7328 290d 0a20  ox.setFocus().. 
-0000d740: 2020 2020 2020 2061 7873 202b 3d20 5b61         axs += [a
-0000d750: 785d 0d0a 2020 2020 6966 2069 7369 6e73  x]..    if isins
-0000d760: 7461 6e63 6528 6d61 7374 6572 2c20 7067  tance(master, pg
-0000d770: 2e47 7261 7068 6963 734c 6179 6f75 7457  .GraphicsLayoutW
-0000d780: 6964 6765 7429 3a0d 0a20 2020 2020 2020  idget):..       
-0000d790: 2070 726f 7879 203d 2070 672e 5369 676e   proxy = pg.Sign
-0000d7a0: 616c 5072 6f78 7928 6d61 7374 6572 2e73  alProxy(master.s
-0000d7b0: 6365 6e65 2829 2e73 6967 4d6f 7573 654d  cene().sigMouseM
-0000d7c0: 6f76 6564 2c20 7261 7465 4c69 6d69 743d  oved, rateLimit=
-0000d7d0: 3134 342c 2073 6c6f 743d 7061 7274 6961  144, slot=partia
-0000d7e0: 6c28 5f6d 6f75 7365 5f6d 6f76 6564 2c20  l(_mouse_moved, 
-0000d7f0: 6d61 7374 6572 2929 0d0a 2020 2020 656c  master))..    el
-0000d800: 7365 3a0d 0a20 2020 2020 2020 2070 726f  se:..        pro
-0000d810: 7879 203d 205b 5d0d 0a20 2020 2020 2020  xy = []..       
-0000d820: 2066 6f72 2061 7820 696e 2061 7873 3a0d   for ax in axs:.
-0000d830: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0000d840: 7879 202b 3d20 5b70 672e 5369 676e 616c  xy += [pg.Signal
-0000d850: 5072 6f78 7928 6178 2e61 785f 7769 6467  Proxy(ax.ax_widg
-0000d860: 6574 2e73 6365 6e65 2829 2e73 6967 4d6f  et.scene().sigMo
-0000d870: 7573 654d 6f76 6564 2c20 7261 7465 4c69  useMoved, rateLi
-0000d880: 6d69 743d 3134 342c 2073 6c6f 743d 7061  mit=144, slot=pa
-0000d890: 7274 6961 6c28 5f6d 6f75 7365 5f6d 6f76  rtial(_mouse_mov
-0000d8a0: 6564 2c20 6d61 7374 6572 2929 5d0d 0a20  ed, master))].. 
-0000d8b0: 2020 206d 6173 7465 725f 6461 7461 5b6d     master_data[m
-0000d8c0: 6173 7465 725d 203d 2064 6963 7428 7072  aster] = dict(pr
-0000d8d0: 6f78 796d 6d3d 7072 6f78 792c 206c 6173  oxymm=proxy, las
-0000d8e0: 745f 6d6f 7573 655f 6576 733d 4e6f 6e65  t_mouse_evs=None
-0000d8f0: 2c20 6c61 7374 5f6d 6f75 7365 5f79 3d30  , last_mouse_y=0
-0000d900: 290d 0a20 2020 206c 6173 745f 6178 203d  )..    last_ax =
-0000d910: 2061 7873 5b30 5d0d 0a20 2020 2072 6574   axs[0]..    ret
-0000d920: 7572 6e20 6178 735b 305d 2069 6620 6c65  urn axs[0] if le
-0000d930: 6e28 6178 7329 203d 3d20 3120 656c 7365  n(axs) == 1 else
-0000d940: 2061 7873 0d0a 0d0a 0d0a 6465 6620 636c   axs......def cl
-0000d950: 6f73 6528 293a 0d0a 2020 2020 666f 7220  ose():..    for 
-0000d960: 7769 6e20 696e 2077 696e 646f 7773 3a0d  win in windows:.
-0000d970: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-0000d980: 2020 2020 2020 2020 2020 2077 696e 2e63             win.c
-0000d990: 6c6f 7365 2829 0d0a 2020 2020 2020 2020  lose()..        
-0000d9a0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0000d9b0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-0000d9c0: 2020 2020 7072 696e 7428 2757 696e 646f      print('Windo
-0000d9d0: 7720 636c 6f73 696e 6720 6572 726f 723a  w closing error:
-0000d9e0: 272c 2074 7970 6528 6529 2c20 6529 0d0a  ', type(e), e)..
-0000d9f0: 2020 2020 676c 6f62 616c 206c 6173 745f      global last_
-0000da00: 6178 0d0a 2020 2020 7769 6e64 6f77 732e  ax..    windows.
-0000da10: 636c 6561 7228 290d 0a20 2020 206f 7665  clear()..    ove
-0000da20: 726c 6179 5f61 7873 2e63 6c65 6172 2829  rlay_axs.clear()
-0000da30: 0d0a 2020 2020 5f63 6c65 6172 5f74 696d  ..    _clear_tim
-0000da40: 6572 7328 290d 0a20 2020 2073 6f75 6e64  ers()..    sound
-0000da50: 732e 636c 6561 7228 290d 0a20 2020 206d  s.clear()..    m
-0000da60: 6173 7465 725f 6461 7461 2e63 6c65 6172  aster_data.clear
-0000da70: 2829 0d0a 2020 2020 6c61 7374 5f61 7820  ()..    last_ax 
-0000da80: 3d20 4e6f 6e65 0d0a 0d0a 0d0a 6465 6620  = None......def 
-0000da90: 7072 6963 655f 636f 6c6f 7266 696c 7465  price_colorfilte
-0000daa0: 7228 6974 656d 2c20 6461 7461 7372 632c  r(item, datasrc,
-0000dab0: 2064 6629 3a0d 0a20 2020 206f 7065 6e63   df):..    openc
-0000dac0: 6f6c 203d 2064 662e 636f 6c75 6d6e 735b  ol = df.columns[
-0000dad0: 315d 0d0a 2020 2020 636c 6f73 6563 6f6c  1]..    closecol
-0000dae0: 203d 2064 662e 636f 6c75 6d6e 735b 325d   = df.columns[2]
-0000daf0: 0d0a 2020 2020 6973 5f75 7020 3d20 6466  ..    is_up = df
-0000db00: 5b6f 7065 6e63 6f6c 5d20 3c3d 2064 665b  [opencol] <= df[
-0000db10: 636c 6f73 6563 6f6c 5d20 2320 6f70 656e  closecol] # open
-0000db20: 206c 6f77 6572 2074 6861 6e20 636c 6f73   lower than clos
-0000db30: 6520 3d20 676f 6573 2075 700d 0a20 2020  e = goes up..   
-0000db40: 2079 6965 6c64 2069 7465 6d2e 726f 7763   yield item.rowc
-0000db50: 6f6c 6f72 7328 2762 756c 6c27 2920 2b20  olors('bull') + 
-0000db60: 5b64 662e 6c6f 635b 6973 5f75 702c 203a  [df.loc[is_up, :
-0000db70: 5d5d 0d0a 2020 2020 7969 656c 6420 6974  ]]..    yield it
-0000db80: 656d 2e72 6f77 636f 6c6f 7273 2827 6265  em.rowcolors('be
-0000db90: 6172 2729 202b 205b 6466 2e6c 6f63 5b7e  ar') + [df.loc[~
-0000dba0: 6973 5f75 702c 203a 5d5d 0d0a 0d0a 0d0a  is_up, :]]......
-0000dbb0: 6465 6620 766f 6c75 6d65 5f63 6f6c 6f72  def volume_color
-0000dbc0: 6669 6c74 6572 2869 7465 6d2c 2064 6174  filter(item, dat
-0000dbd0: 6173 7263 2c20 6466 293a 0d0a 2020 2020  asrc, df):..    
-0000dbe0: 6f70 656e 636f 6c20 3d20 6466 2e63 6f6c  opencol = df.col
-0000dbf0: 756d 6e73 5b33 5d0d 0a20 2020 2063 6c6f  umns[3]..    clo
-0000dc00: 7365 636f 6c20 3d20 6466 2e63 6f6c 756d  secol = df.colum
-0000dc10: 6e73 5b34 5d0d 0a20 2020 2069 735f 7570  ns[4]..    is_up
-0000dc20: 203d 2064 665b 6f70 656e 636f 6c5d 203c   = df[opencol] <
-0000dc30: 3d20 6466 5b63 6c6f 7365 636f 6c5d 2023  = df[closecol] #
-0000dc40: 206f 7065 6e20 6c6f 7765 7220 7468 616e   open lower than
-0000dc50: 2063 6c6f 7365 203d 2067 6f65 7320 7570   close = goes up
-0000dc60: 0d0a 2020 2020 7969 656c 6420 6974 656d  ..    yield item
-0000dc70: 2e72 6f77 636f 6c6f 7273 2827 6275 6c6c  .rowcolors('bull
-0000dc80: 2729 202b 205b 6466 2e6c 6f63 5b69 735f  ') + [df.loc[is_
-0000dc90: 7570 2c20 3a5d 5d0d 0a20 2020 2079 6965  up, :]]..    yie
-0000dca0: 6c64 2069 7465 6d2e 726f 7763 6f6c 6f72  ld item.rowcolor
-0000dcb0: 7328 2762 6561 7227 2920 2b20 5b64 662e  s('bear') + [df.
-0000dcc0: 6c6f 635b 7e69 735f 7570 2c20 3a5d 5d0d  loc[~is_up, :]].
-0000dcd0: 0a0d 0a0d 0a64 6566 2073 7472 656e 6774  .....def strengt
-0000dce0: 685f 636f 6c6f 7266 696c 7465 7228 6974  h_colorfilter(it
-0000dcf0: 656d 2c20 6461 7461 7372 632c 2064 6629  em, datasrc, df)
-0000dd00: 3a0d 0a20 2020 206f 7065 6e63 6f6c 203d  :..    opencol =
-0000dd10: 2064 662e 636f 6c75 6d6e 735b 315d 0d0a   df.columns[1]..
-0000dd20: 2020 2020 636c 6f73 6563 6f6c 203d 2064      closecol = d
-0000dd30: 662e 636f 6c75 6d6e 735b 325d 0d0a 2020  f.columns[2]..  
-0000dd40: 2020 7374 6172 7463 6f6c 203d 2064 662e    startcol = df.
-0000dd50: 636f 6c75 6d6e 735b 335d 0d0a 2020 2020  columns[3]..    
-0000dd60: 656e 6463 6f6c 203d 2064 662e 636f 6c75  endcol = df.colu
-0000dd70: 6d6e 735b 345d 0d0a 2020 2020 6973 5f75  mns[4]..    is_u
-0000dd80: 7020 3d20 6466 5b6f 7065 6e63 6f6c 5d20  p = df[opencol] 
-0000dd90: 3c3d 2064 665b 636c 6f73 6563 6f6c 5d20  <= df[closecol] 
-0000dda0: 2320 6f70 656e 206c 6f77 6572 2074 6861  # open lower tha
-0000ddb0: 6e20 636c 6f73 6520 3d20 676f 6573 2075  n close = goes u
-0000ddc0: 700d 0a20 2020 2069 735f 7374 726f 6e67  p..    is_strong
-0000ddd0: 203d 2064 665b 7374 6172 7463 6f6c 5d20   = df[startcol] 
-0000dde0: 3c3d 2064 665b 656e 6463 6f6c 5d0d 0a20  <= df[endcol].. 
-0000ddf0: 2020 2079 6965 6c64 2069 7465 6d2e 726f     yield item.ro
-0000de00: 7763 6f6c 6f72 7328 2762 756c 6c27 2920  wcolors('bull') 
-0000de10: 2b20 5b64 662e 6c6f 635b 6973 5f75 7026  + [df.loc[is_up&
-0000de20: 6973 5f73 7472 6f6e 672c 203a 5d5d 0d0a  is_strong, :]]..
-0000de30: 2020 2020 7969 656c 6420 6974 656d 2e72      yield item.r
-0000de40: 6f77 636f 6c6f 7273 2827 7765 616b 5f62  owcolors('weak_b
-0000de50: 756c 6c27 2920 2b20 5b64 662e 6c6f 635b  ull') + [df.loc[
-0000de60: 6973 5f75 7026 287e 6973 5f73 7472 6f6e  is_up&(~is_stron
-0000de70: 6729 2c20 3a5d 5d0d 0a20 2020 2079 6965  g), :]]..    yie
-0000de80: 6c64 2069 7465 6d2e 726f 7763 6f6c 6f72  ld item.rowcolor
-0000de90: 7328 2777 6561 6b5f 6265 6172 2729 202b  s('weak_bear') +
-0000dea0: 205b 6466 2e6c 6f63 5b28 7e69 735f 7570   [df.loc[(~is_up
-0000deb0: 2926 6973 5f73 7472 6f6e 672c 203a 5d5d  )&is_strong, :]]
-0000dec0: 0d0a 2020 2020 7969 656c 6420 6974 656d  ..    yield item
-0000ded0: 2e72 6f77 636f 6c6f 7273 2827 6265 6172  .rowcolors('bear
-0000dee0: 2729 202b 205b 6466 2e6c 6f63 5b28 7e69  ') + [df.loc[(~i
-0000def0: 735f 7570 2926 287e 6973 5f73 7472 6f6e  s_up)&(~is_stron
-0000df00: 6729 2c20 3a5d 5d0d 0a0d 0a0d 0a64 6566  g), :]]......def
-0000df10: 2076 6f6c 756d 655f 636f 6c6f 7266 696c   volume_colorfil
-0000df20: 7465 725f 7365 6374 696f 6e28 7365 6374  ter_section(sect
-0000df30: 696f 6e73 3d5b 5d29 3a0d 0a20 2020 2027  ions=[]):..    '
-0000df40: 2727 5468 6520 7365 6374 696f 6e73 2061  ''The sections a
-0000df50: 7267 756d 656e 7420 6973 2061 2028 7374  rgument is a (st
-0000df60: 6172 7469 6e67 5f69 6e64 6578 2c20 636f  arting_index, co
-0000df70: 6c6f 725f 6e61 6d65 2920 6172 7261 792e  lor_name) array.
-0000df80: 2727 270d 0a20 2020 2064 6566 205f 636f  '''..    def _co
-0000df90: 6c6f 7266 696c 7465 7228 7365 6374 696f  lorfilter(sectio
-0000dfa0: 6e73 2c20 6974 656d 2c20 6461 7461 7372  ns, item, datasr
-0000dfb0: 632c 2064 6629 3a0d 0a20 2020 2020 2020  c, df):..       
-0000dfc0: 2069 6620 6e6f 7420 7365 6374 696f 6e73   if not sections
-0000dfd0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0000dfe0: 6574 7572 6e20 766f 6c75 6d65 5f63 6f6c  eturn volume_col
-0000dff0: 6f72 6669 6c74 6572 2869 7465 6d2c 2064  orfilter(item, d
-0000e000: 6174 6173 7263 2c20 6466 290d 0a20 2020  atasrc, df)..   
-0000e010: 2020 2020 2066 6f72 2028 6930 2c63 6f6c       for (i0,col
-0000e020: 6e61 6d65 292c 2869 312c 5f29 2069 6e20  name),(i1,_) in 
-0000e030: 7a69 7028 7365 6374 696f 6e73 2c20 7365  zip(sections, se
-0000e040: 6374 696f 6e73 5b31 3a5d 2b5b 284e 6f6e  ctions[1:]+[(Non
-0000e050: 652c 276e 6575 7472 616c 2729 5d29 3a0d  e,'neutral')]):.
-0000e060: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
-0000e070: 7320 3d20 6466 2e69 6c6f 635b 6930 3a69  s = df.iloc[i0:i
-0000e080: 312c 203a 5d0d 0a20 2020 2020 2020 2020  1, :]..         
-0000e090: 2020 2079 6965 6c64 2069 7465 6d2e 726f     yield item.ro
-0000e0a0: 7763 6f6c 6f72 7328 636f 6c6e 616d 6529  wcolors(colname)
-0000e0b0: 202b 205b 726f 7773 5d0d 0a20 2020 2072   + [rows]..    r
-0000e0c0: 6574 7572 6e20 7061 7274 6961 6c28 5f63  eturn partial(_c
-0000e0d0: 6f6c 6f72 6669 6c74 6572 2c20 7365 6374  olorfilter, sect
-0000e0e0: 696f 6e73 290d 0a0d 0a0d 0a64 6566 2068  ions)......def h
-0000e0f0: 6f72 697a 766f 6c5f 636f 6c6f 7266 696c  orizvol_colorfil
-0000e100: 7465 7228 7365 6374 696f 6e73 3d5b 5d29  ter(sections=[])
-0000e110: 3a0d 0a20 2020 2027 2727 5468 6520 7365  :..    '''The se
-0000e120: 6374 696f 6e73 2061 7267 756d 656e 7420  ctions argument 
-0000e130: 6973 2061 2028 7374 6172 7469 6e67 5f69  is a (starting_i
-0000e140: 6e64 6578 2c20 636f 6c6f 725f 6e61 6d65  ndex, color_name
-0000e150: 2920 6172 7261 792e 2727 270d 0a20 2020  ) array.'''..   
-0000e160: 2064 6566 205f 636f 6c6f 7266 696c 7465   def _colorfilte
-0000e170: 7228 7365 6374 696f 6e73 2c20 6974 656d  r(sections, item
-0000e180: 2c20 6461 7461 7372 632c 2064 6174 6129  , datasrc, data)
-0000e190: 3a0d 0a20 2020 2020 2020 2069 6620 6e6f  :..        if no
-0000e1a0: 7420 7365 6374 696f 6e73 3a0d 0a20 2020  t sections:..   
-0000e1b0: 2020 2020 2020 2020 2079 6965 6c64 2069           yield i
-0000e1c0: 7465 6d2e 726f 7763 6f6c 6f72 7328 276e  tem.rowcolors('n
-0000e1d0: 6575 7472 616c 2729 202b 205b 6461 7461  eutral') + [data
-0000e1e0: 5d0d 0a20 2020 2020 2020 2066 6f72 2028  ]..        for (
-0000e1f0: 6930 2c63 6f6c 6e61 6d65 292c 2869 312c  i0,colname),(i1,
-0000e200: 5f29 2069 6e20 7a69 7028 7365 6374 696f  _) in zip(sectio
-0000e210: 6e73 2c20 7365 6374 696f 6e73 5b31 3a5d  ns, sections[1:]
-0000e220: 2b5b 284e 6f6e 652c 276e 6575 7472 616c  +[(None,'neutral
-0000e230: 2729 5d29 3a0d 0a20 2020 2020 2020 2020  ')]):..         
-0000e240: 2020 2072 6f77 7320 3d20 6461 7461 5b3a     rows = data[:
-0000e250: 2c20 6930 3a69 315d 0d0a 2020 2020 2020  , i0:i1]..      
-0000e260: 2020 2020 2020 7969 656c 6420 6974 656d        yield item
-0000e270: 2e72 6f77 636f 6c6f 7273 2863 6f6c 6e61  .rowcolors(colna
-0000e280: 6d65 2920 2b20 5b72 6f77 735d 0d0a 2020  me) + [rows]..  
-0000e290: 2020 7265 7475 726e 2070 6172 7469 616c    return partial
-0000e2a0: 285f 636f 6c6f 7266 696c 7465 722c 2073  (_colorfilter, s
-0000e2b0: 6563 7469 6f6e 7329 0d0a 0d0a 0d0a 6465  ections)......de
-0000e2c0: 6620 6361 6e64 6c65 7374 6963 6b5f 6f63  f candlestick_oc
-0000e2d0: 686c 2864 6174 6173 7263 2c20 6472 6177  hl(datasrc, draw
-0000e2e0: 5f62 6f64 793d 5472 7565 2c20 6472 6177  _body=True, draw
-0000e2f0: 5f73 6861 646f 773d 5472 7565 2c20 6361  _shadow=True, ca
-0000e300: 6e64 6c65 5f77 6964 7468 3d30 2e36 2c20  ndle_width=0.6, 
-0000e310: 6178 3d4e 6f6e 652c 2063 6f6c 6f72 6675  ax=None, colorfu
-0000e320: 6e63 3d70 7269 6365 5f63 6f6c 6f72 6669  nc=price_colorfi
-0000e330: 6c74 6572 293a 0d0a 2020 2020 6178 203d  lter):..    ax =
-0000e340: 205f 6372 6561 7465 5f70 6c6f 7428 6178   _create_plot(ax
-0000e350: 3d61 782c 206d 6178 696d 697a 653d 4661  =ax, maximize=Fa
-0000e360: 6c73 6529 0d0a 2020 2020 6461 7461 7372  lse)..    datasr
-0000e370: 6320 3d20 5f63 7265 6174 655f 6461 7461  c = _create_data
-0000e380: 7372 6328 6178 2c20 6461 7461 7372 6329  src(ax, datasrc)
-0000e390: 0d0a 2020 2020 6461 7461 7372 632e 7363  ..    datasrc.sc
-0000e3a0: 616c 655f 636f 6c73 203d 205b 332c 345d  ale_cols = [3,4]
-0000e3b0: 2023 206f 6e6c 7920 6869 2b6c 6f20 7363   # only hi+lo sc
-0000e3c0: 616c 6573 0d0a 2020 2020 5f73 6574 5f64  ales..    _set_d
-0000e3d0: 6174 6173 7263 2861 782c 2064 6174 6173  atasrc(ax, datas
-0000e3e0: 7263 290d 0a20 2020 2069 7465 6d20 3d20  rc)..    item = 
-0000e3f0: 4361 6e64 6c65 7374 6963 6b49 7465 6d28  CandlestickItem(
-0000e400: 6178 3d61 782c 2064 6174 6173 7263 3d64  ax=ax, datasrc=d
-0000e410: 6174 6173 7263 2c20 6472 6177 5f62 6f64  atasrc, draw_bod
-0000e420: 793d 6472 6177 5f62 6f64 792c 2064 7261  y=draw_body, dra
-0000e430: 775f 7368 6164 6f77 3d64 7261 775f 7368  w_shadow=draw_sh
-0000e440: 6164 6f77 2c20 6361 6e64 6c65 5f77 6964  adow, candle_wid
-0000e450: 7468 3d63 616e 646c 655f 7769 6474 682c  th=candle_width,
-0000e460: 2063 6f6c 6f72 6675 6e63 3d63 6f6c 6f72   colorfunc=color
-0000e470: 6675 6e63 290d 0a20 2020 205f 7570 6461  func)..    _upda
-0000e480: 7465 5f73 6967 6e69 6669 6361 6e74 7328  te_significants(
-0000e490: 6178 2c20 6461 7461 7372 632c 2066 6f72  ax, datasrc, for
-0000e4a0: 6365 3d54 7275 6529 0d0a 2020 2020 6974  ce=True)..    it
-0000e4b0: 656d 2e75 7064 6174 655f 6461 7461 203d  em.update_data =
-0000e4c0: 2070 6172 7469 616c 285f 7570 6461 7465   partial(_update
-0000e4d0: 5f64 6174 612c 204e 6f6e 652c 204e 6f6e  _data, None, Non
-0000e4e0: 652c 2069 7465 6d29 0d0a 2020 2020 6974  e, item)..    it
-0000e4f0: 656d 2e75 7064 6174 655f 6766 7820 3d20  em.update_gfx = 
-0000e500: 7061 7274 6961 6c28 5f75 7064 6174 655f  partial(_update_
-0000e510: 6766 782c 2069 7465 6d29 0d0a 2020 2020  gfx, item)..    
-0000e520: 6178 2e61 6464 4974 656d 2869 7465 6d29  ax.addItem(item)
-0000e530: 0d0a 2020 2020 7265 7475 726e 2069 7465  ..    return ite
-0000e540: 6d0d 0a0d 0a0d 0a64 6566 2072 656e 6b6f  m......def renko
-0000e550: 2878 2c20 793d 4e6f 6e65 2c20 6269 6e73  (x, y=None, bins
-0000e560: 3d4e 6f6e 652c 2073 7465 703d 4e6f 6e65  =None, step=None
-0000e570: 2c20 6178 3d4e 6f6e 652c 2063 6f6c 6f72  , ax=None, color
-0000e580: 6675 6e63 3d70 7269 6365 5f63 6f6c 6f72  func=price_color
-0000e590: 6669 6c74 6572 293a 0d0a 2020 2020 6178  filter):..    ax
-0000e5a0: 203d 205f 6372 6561 7465 5f70 6c6f 7428   = _create_plot(
-0000e5b0: 6178 3d61 782c 206d 6178 696d 697a 653d  ax=ax, maximize=
-0000e5c0: 4661 6c73 6529 0d0a 2020 2020 6461 7461  False)..    data
-0000e5d0: 7372 6320 3d20 5f63 7265 6174 655f 6461  src = _create_da
-0000e5e0: 7461 7372 6328 6178 2c20 782c 2079 290d  tasrc(ax, x, y).
-0000e5f0: 0a20 2020 206f 7269 6764 6620 3d20 6461  .    origdf = da
-0000e600: 7461 7372 632e 6466 0d0a 2020 2020 6164  tasrc.df..    ad
-0000e610: 6a20 3d20 5f61 646a 7573 745f 7265 6e6b  j = _adjust_renk
-0000e620: 6f5f 6c6f 675f 6461 7461 7372 6320 6966  o_log_datasrc if
-0000e630: 2061 782e 7662 2e79 7363 616c 652e 7363   ax.vb.yscale.sc
-0000e640: 616c 6574 7970 6520 3d3d 2027 6c6f 6727  aletype == 'log'
-0000e650: 2065 6c73 6520 5f61 646a 7573 745f 7265   else _adjust_re
-0000e660: 6e6b 6f5f 6461 7461 7372 630d 0a20 2020  nko_datasrc..   
-0000e670: 2073 7465 705f 6164 6a75 7374 5f72 656e   step_adjust_ren
-0000e680: 6b6f 5f64 6174 6173 7263 203d 2070 6172  ko_datasrc = par
-0000e690: 7469 616c 2861 646a 2c20 6269 6e73 2c20  tial(adj, bins, 
-0000e6a0: 7374 6570 290d 0a20 2020 2073 7465 705f  step)..    step_
-0000e6b0: 6164 6a75 7374 5f72 656e 6b6f 5f64 6174  adjust_renko_dat
-0000e6c0: 6173 7263 2864 6174 6173 7263 290d 0a20  asrc(datasrc).. 
-0000e6d0: 2020 2061 782e 6465 636f 7570 6c65 2829     ax.decouple()
-0000e6e0: 0d0a 2020 2020 6974 656d 203d 2063 616e  ..    item = can
-0000e6f0: 646c 6573 7469 636b 5f6f 6368 6c28 6461  dlestick_ochl(da
-0000e700: 7461 7372 632c 2064 7261 775f 7368 6164  tasrc, draw_shad
-0000e710: 6f77 3d46 616c 7365 2c20 6361 6e64 6c65  ow=False, candle
-0000e720: 5f77 6964 7468 3d31 2c20 6178 3d61 782c  _width=1, ax=ax,
-0000e730: 2063 6f6c 6f72 6675 6e63 3d63 6f6c 6f72   colorfunc=color
-0000e740: 6675 6e63 290d 0a20 2020 2069 7465 6d2e  func)..    item.
-0000e750: 636f 6c6f 7273 5b27 6275 6c6c 5f62 6f64  colors['bull_bod
-0000e760: 7927 5d20 3d20 6974 656d 2e63 6f6c 6f72  y'] = item.color
-0000e770: 735b 2762 756c 6c5f 6672 616d 6527 5d0d  s['bull_frame'].
-0000e780: 0a20 2020 2069 7465 6d2e 7570 6461 7465  .    item.update
-0000e790: 5f64 6174 6120 3d20 7061 7274 6961 6c28  _data = partial(
-0000e7a0: 5f75 7064 6174 655f 6461 7461 2c20 4e6f  _update_data, No
-0000e7b0: 6e65 2c20 7374 6570 5f61 646a 7573 745f  ne, step_adjust_
-0000e7c0: 7265 6e6b 6f5f 6461 7461 7372 632c 2069  renko_datasrc, i
-0000e7d0: 7465 6d29 0d0a 2020 2020 6974 656d 2e75  tem)..    item.u
-0000e7e0: 7064 6174 655f 6766 7820 3d20 7061 7274  pdate_gfx = part
-0000e7f0: 6961 6c28 5f75 7064 6174 655f 6766 782c  ial(_update_gfx,
-0000e800: 2069 7465 6d29 0d0a 2020 2020 676c 6f62   item)..    glob
-0000e810: 616c 2065 706f 6368 5f70 6572 696f 640d  al epoch_period.
-0000e820: 0a20 2020 2065 706f 6368 5f70 6572 696f  .    epoch_perio
-0000e830: 6420 3d20 286f 7269 6764 662e 696c 6f63  d = (origdf.iloc
-0000e840: 5b31 2c30 5d20 2d20 6f72 6967 6466 2e69  [1,0] - origdf.i
-0000e850: 6c6f 635b 302c 305d 2920 2f2f 2069 6e74  loc[0,0]) // int
-0000e860: 2831 6539 290d 0a20 2020 2072 6574 7572  (1e9)..    retur
-0000e870: 6e20 6974 656d 0d0a 0d0a 0d0a 6465 6620  n item......def 
-0000e880: 766f 6c75 6d65 5f6f 6376 2864 6174 6173  volume_ocv(datas
-0000e890: 7263 2c20 6361 6e64 6c65 5f77 6964 7468  rc, candle_width
-0000e8a0: 3d30 2e38 2c20 6178 3d4e 6f6e 652c 2063  =0.8, ax=None, c
-0000e8b0: 6f6c 6f72 6675 6e63 3d76 6f6c 756d 655f  olorfunc=volume_
-0000e8c0: 636f 6c6f 7266 696c 7465 7229 3a0d 0a20  colorfilter):.. 
-0000e8d0: 2020 2061 7820 3d20 5f63 7265 6174 655f     ax = _create_
-0000e8e0: 706c 6f74 2861 783d 6178 2c20 6d61 7869  plot(ax=ax, maxi
-0000e8f0: 6d69 7a65 3d46 616c 7365 290d 0a20 2020  mize=False)..   
-0000e900: 2064 6174 6173 7263 203d 205f 6372 6561   datasrc = _crea
-0000e910: 7465 5f64 6174 6173 7263 2861 782c 2064  te_datasrc(ax, d
-0000e920: 6174 6173 7263 290d 0a20 2020 205f 6164  atasrc)..    _ad
-0000e930: 6a75 7374 5f76 6f6c 756d 655f 6461 7461  just_volume_data
-0000e940: 7372 6328 6461 7461 7372 6329 0d0a 2020  src(datasrc)..  
-0000e950: 2020 5f73 6574 5f64 6174 6173 7263 2861    _set_datasrc(a
-0000e960: 782c 2064 6174 6173 7263 290d 0a20 2020  x, datasrc)..   
-0000e970: 2069 7465 6d20 3d20 4361 6e64 6c65 7374   item = Candlest
-0000e980: 6963 6b49 7465 6d28 6178 3d61 782c 2064  ickItem(ax=ax, d
-0000e990: 6174 6173 7263 3d64 6174 6173 7263 2c20  atasrc=datasrc, 
-0000e9a0: 6472 6177 5f62 6f64 793d 5472 7565 2c20  draw_body=True, 
-0000e9b0: 6472 6177 5f73 6861 646f 773d 4661 6c73  draw_shadow=Fals
-0000e9c0: 652c 2063 616e 646c 655f 7769 6474 683d  e, candle_width=
-0000e9d0: 6361 6e64 6c65 5f77 6964 7468 2c20 636f  candle_width, co
-0000e9e0: 6c6f 7266 756e 633d 636f 6c6f 7266 756e  lorfunc=colorfun
-0000e9f0: 6329 0d0a 2020 2020 5f75 7064 6174 655f  c)..    _update_
-0000ea00: 7369 676e 6966 6963 616e 7473 2861 782c  significants(ax,
-0000ea10: 2064 6174 6173 7263 2c20 666f 7263 653d   datasrc, force=
-0000ea20: 5472 7565 290d 0a20 2020 2069 7465 6d2e  True)..    item.
-0000ea30: 636f 6c6f 7273 5b27 6275 6c6c 5f62 6f64  colors['bull_bod
-0000ea40: 7927 5d20 3d20 6974 656d 2e63 6f6c 6f72  y'] = item.color
-0000ea50: 735b 2762 756c 6c5f 6672 616d 6527 5d0d  s['bull_frame'].
-0000ea60: 0a20 2020 2069 6620 636f 6c6f 7266 756e  .    if colorfun
-0000ea70: 6320 3d3d 2076 6f6c 756d 655f 636f 6c6f  c == volume_colo
-0000ea80: 7266 696c 7465 723a 2023 2061 7373 756d  rfilter: # assum
-0000ea90: 6520 6e6f 726d 616c 2076 6f6c 756d 6520  e normal volume 
-0000eaa0: 706c 6f74 0d0a 2020 2020 2020 2020 6974  plot..        it
-0000eab0: 656d 2e63 6f6c 6f72 735b 2762 756c 6c5f  em.colors['bull_
-0000eac0: 6672 616d 6527 5d20 3d20 766f 6c75 6d65  frame'] = volume
-0000ead0: 5f62 756c 6c5f 636f 6c6f 720d 0a20 2020  _bull_color..   
-0000eae0: 2020 2020 2069 7465 6d2e 636f 6c6f 7273       item.colors
-0000eaf0: 5b27 6275 6c6c 5f62 6f64 7927 5d20 203d  ['bull_body']  =
-0000eb00: 2076 6f6c 756d 655f 6275 6c6c 5f62 6f64   volume_bull_bod
-0000eb10: 795f 636f 6c6f 720d 0a20 2020 2020 2020  y_color..       
-0000eb20: 2069 7465 6d2e 636f 6c6f 7273 5b27 6265   item.colors['be
-0000eb30: 6172 5f66 7261 6d65 275d 203d 2076 6f6c  ar_frame'] = vol
-0000eb40: 756d 655f 6265 6172 5f63 6f6c 6f72 0d0a  ume_bear_color..
-0000eb50: 2020 2020 2020 2020 6974 656d 2e63 6f6c          item.col
-0000eb60: 6f72 735b 2762 6561 725f 626f 6479 275d  ors['bear_body']
-0000eb70: 2020 3d20 766f 6c75 6d65 5f62 6561 725f    = volume_bear_
-0000eb80: 636f 6c6f 720d 0a20 2020 2020 2020 2061  color..        a
-0000eb90: 782e 7662 2e76 5f7a 6f6f 6d5f 6261 7365  x.vb.v_zoom_base
-0000eba0: 6c69 6e65 203d 2030 0d0a 2020 2020 656c  line = 0..    el
-0000ebb0: 7365 3a0d 0a20 2020 2020 2020 2069 7465  se:..        ite
-0000ebc0: 6d2e 636f 6c6f 7273 5b27 7765 616b 5f62  m.colors['weak_b
-0000ebd0: 756c 6c5f 6672 616d 6527 5d20 3d20 6272  ull_frame'] = br
-0000ebe0: 6967 6874 656e 2876 6f6c 756d 655f 6275  ighten(volume_bu
-0000ebf0: 6c6c 5f63 6f6c 6f72 2c20 312e 3229 0d0a  ll_color, 1.2)..
-0000ec00: 2020 2020 2020 2020 6974 656d 2e63 6f6c          item.col
-0000ec10: 6f72 735b 2777 6561 6b5f 6275 6c6c 5f62  ors['weak_bull_b
-0000ec20: 6f64 7927 5d20 203d 2062 7269 6768 7465  ody']  = brighte
-0000ec30: 6e28 766f 6c75 6d65 5f62 756c 6c5f 636f  n(volume_bull_co
-0000ec40: 6c6f 722c 2031 2e32 290d 0a20 2020 2069  lor, 1.2)..    i
-0000ec50: 7465 6d2e 7570 6461 7465 5f64 6174 6120  tem.update_data 
-0000ec60: 3d20 7061 7274 6961 6c28 5f75 7064 6174  = partial(_updat
-0000ec70: 655f 6461 7461 2c20 4e6f 6e65 2c20 5f61  e_data, None, _a
-0000ec80: 646a 7573 745f 766f 6c75 6d65 5f64 6174  djust_volume_dat
-0000ec90: 6173 7263 2c20 6974 656d 290d 0a20 2020  asrc, item)..   
-0000eca0: 2069 7465 6d2e 7570 6461 7465 5f67 6678   item.update_gfx
-0000ecb0: 203d 2070 6172 7469 616c 285f 7570 6461   = partial(_upda
-0000ecc0: 7465 5f67 6678 2c20 6974 656d 290d 0a20  te_gfx, item).. 
-0000ecd0: 2020 2061 782e 6164 6449 7465 6d28 6974     ax.addItem(it
-0000ece0: 656d 290d 0a20 2020 2069 7465 6d2e 7365  em)..    item.se
-0000ecf0: 745a 5661 6c75 6528 2d32 3029 0d0a 2020  tZValue(-20)..  
-0000ed00: 2020 7265 7475 726e 2069 7465 6d0d 0a0d    return item...
-0000ed10: 0a0d 0a64 6566 2068 6f72 697a 5f74 696d  ...def horiz_tim
-0000ed20: 655f 766f 6c75 6d65 2864 6174 6173 7263  e_volume(datasrc
-0000ed30: 2c20 6178 3d4e 6f6e 652c 202a 2a6b 7761  , ax=None, **kwa
-0000ed40: 7267 7329 3a0d 0a20 2020 2027 2727 4472  rgs):..    '''Dr
-0000ed50: 6177 7320 6d75 6c74 6970 6c65 2066 6978  aws multiple fix
-0000ed60: 6564 2068 6f72 697a 6f6e 7461 6c20 766f  ed horizontal vo
-0000ed70: 6c75 6d65 732e 2054 6865 2069 6e70 7574  lumes. The input
-0000ed80: 2066 6f72 6d61 7420 6973 3a0d 0a20 2020   format is:..   
-0000ed90: 2020 2020 5b5b 7469 6d65 302c 205b 2870      [[time0, [(p
-0000eda0: 7269 6365 302c 766f 6c75 6d65 3029 2c28  rice0,volume0),(
-0000edb0: 7072 6963 6531 2c76 6f6c 756d 6531 292c  price1,volume1),
-0000edc0: 2e2e 2e5d 5d2c 202e 2e2e 5d0d 0a0d 0a20  ...]], ...].... 
-0000edd0: 2020 2020 2020 5468 6973 2063 6861 7274        This chart
-0000ede0: 206e 6565 6473 2074 6f20 6265 2070 6c6f   needs to be plo
-0000edf0: 7420 6c61 7374 2c20 736f 2069 7420 6b6e  t last, so it kn
-0000ee00: 6f77 7320 6966 2069 7420 636f 6e74 726f  ows if it contro
-0000ee10: 6c73 0d0a 2020 2020 2020 2077 6861 7420  ls..       what 
-0000ee20: 7469 6d65 2070 6572 696f 6473 2061 7265  time periods are
-0000ee30: 2073 686f 776e 2c20 6f72 2069 6620 6974   shown, or if it
-0000ee40: 7320 7573 696e 6720 7469 6d65 2061 6c72  s using time alr
-0000ee50: 6561 6479 2069 6e0d 0a20 2020 2020 2020  eady in..       
-0000ee60: 706c 6163 6520 6279 2061 6e6f 7468 6572  place by another
-0000ee70: 2070 6c6f 742e 2727 270d 0a20 2020 2023   plot.'''..    #
-0000ee80: 2075 7064 6174 6520 6861 6e64 6c69 6e67   update handling
-0000ee90: 2064 6566 6175 6c74 2069 6620 6e65 6365   default if nece
-0000eea0: 7373 6172 790d 0a20 2020 2067 6c6f 6261  ssary..    globa
-0000eeb0: 6c20 6d61 785f 7a6f 6f6d 5f70 6f69 6e74  l max_zoom_point
-0000eec0: 732c 2072 6967 6874 5f6d 6172 6769 6e5f  s, right_margin_
-0000eed0: 6361 6e64 6c65 730d 0a20 2020 2069 6620  candles..    if 
-0000eee0: 6d61 785f 7a6f 6f6d 5f70 6f69 6e74 7320  max_zoom_points 
-0000eef0: 3e20 3135 3a0d 0a20 2020 2020 2020 206d  > 15:..        m
-0000ef00: 6178 5f7a 6f6f 6d5f 706f 696e 7473 203d  ax_zoom_points =
-0000ef10: 2034 0d0a 2020 2020 6966 2072 6967 6874   4..    if right
-0000ef20: 5f6d 6172 6769 6e5f 6361 6e64 6c65 7320  _margin_candles 
-0000ef30: 3e20 333a 0d0a 2020 2020 2020 2020 7269  > 3:..        ri
-0000ef40: 6768 745f 6d61 7267 696e 5f63 616e 646c  ght_margin_candl
-0000ef50: 6573 203d 2031 0d0a 0d0a 2020 2020 6178  es = 1....    ax
-0000ef60: 203d 205f 6372 6561 7465 5f70 6c6f 7428   = _create_plot(
-0000ef70: 6178 3d61 782c 206d 6178 696d 697a 653d  ax=ax, maximize=
-0000ef80: 4661 6c73 6529 0d0a 2020 2020 6461 7461  False)..    data
-0000ef90: 7372 6320 3d20 5f70 7265 6164 6a75 7374  src = _preadjust
-0000efa0: 5f68 6f72 697a 5f64 6174 6173 7263 2864  _horiz_datasrc(d
-0000efb0: 6174 6173 7263 290d 0a20 2020 2064 6174  atasrc)..    dat
-0000efc0: 6173 7263 203d 205f 6372 6561 7465 5f64  asrc = _create_d
-0000efd0: 6174 6173 7263 2861 782c 2064 6174 6173  atasrc(ax, datas
-0000efe0: 7263 290d 0a20 2020 205f 6164 6a75 7374  rc)..    _adjust
-0000eff0: 5f68 6f72 697a 5f64 6174 6173 7263 2864  _horiz_datasrc(d
-0000f000: 6174 6173 7263 290d 0a20 2020 2069 6620  atasrc)..    if 
-0000f010: 6178 2e76 622e 6461 7461 7372 6320 6973  ax.vb.datasrc is
-0000f020: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000f030: 2020 2020 6461 7461 7372 632e 7374 616e      datasrc.stan
-0000f040: 6461 6c6f 6e65 203d 2054 7275 6520 2320  dalone = True # 
-0000f050: 6f6e 6c79 2066 6f72 6365 2073 7461 6e64  only force stand
-0000f060: 616c 6f6e 6520 6966 2074 6865 7265 2069  alone if there i
-0000f070: 7320 736f 6d65 7468 696e 6720 6f6e 206f  s something on o
-0000f080: 7572 2063 6861 7274 7320 616c 7265 6164  ur charts alread
-0000f090: 790d 0a20 2020 2064 6174 6173 7263 2e73  y..    datasrc.s
-0000f0a0: 6361 6c65 5f63 6f6c 7320 3d20 5b64 6174  cale_cols = [dat
-0000f0b0: 6173 7263 2e63 6f6c 5f64 6174 615f 6f66  asrc.col_data_of
-0000f0c0: 6673 6574 2c20 6c65 6e28 6461 7461 7372  fset, len(datasr
-0000f0d0: 632e 6466 2e63 6f6c 756d 6e73 292d 325d  c.df.columns)-2]
-0000f0e0: 2023 2066 6972 7374 2061 6e64 206c 6173   # first and las
-0000f0f0: 7420 7072 6963 6520 636f 6c75 6d6e 730d  t price columns.
-0000f100: 0a20 2020 2064 6174 6173 7263 2e70 7265  .    datasrc.pre
-0000f110: 5f75 7064 6174 6520 3d20 6c61 6d62 6461  _update = lambda
-0000f120: 2064 663a 2064 662e 6c6f 635b 3a2c 203a   df: df.loc[:, :
-0000f130: 6466 2e63 6f6c 756d 6e73 5b30 5d5d 2023  df.columns[0]] #
-0000f140: 2074 6872 6f77 2061 7761 7920 7072 6576   throw away prev
-0000f150: 696f 7573 2064 6174 610d 0a20 2020 2064  ious data..    d
-0000f160: 6174 6173 7263 2e70 6f73 745f 7570 6461  atasrc.post_upda
-0000f170: 7465 203d 206c 616d 6264 6120 6466 3a20  te = lambda df: 
-0000f180: 6466 2e64 726f 706e 6128 686f 773d 2761  df.dropna(how='a
-0000f190: 6c6c 2729 2023 206b 696c 6c20 616c 6c2d  ll') # kill all-
-0000f1a0: 4e61 4e73 0d0a 2020 2020 5f73 6574 5f64  NaNs..    _set_d
-0000f1b0: 6174 6173 7263 2861 782c 2064 6174 6173  atasrc(ax, datas
-0000f1c0: 7263 290d 0a20 2020 2069 7465 6d20 3d20  rc)..    item = 
-0000f1d0: 486f 7269 7a6f 6e74 616c 5469 6d65 566f  HorizontalTimeVo
-0000f1e0: 6c75 6d65 4974 656d 2861 783d 6178 2c20  lumeItem(ax=ax, 
-0000f1f0: 6461 7461 7372 633d 6461 7461 7372 632c  datasrc=datasrc,
-0000f200: 202a 2a6b 7761 7267 7329 0d0a 2020 2020   **kwargs)..    
-0000f210: 6974 656d 2e75 7064 6174 655f 6461 7461  item.update_data
-0000f220: 203d 2070 6172 7469 616c 285f 7570 6461   = partial(_upda
-0000f230: 7465 5f64 6174 612c 205f 7072 6561 646a  te_data, _preadj
-0000f240: 7573 745f 686f 7269 7a5f 6461 7461 7372  ust_horiz_datasr
-0000f250: 632c 205f 6164 6a75 7374 5f68 6f72 697a  c, _adjust_horiz
-0000f260: 5f64 6174 6173 7263 2c20 6974 656d 290d  _datasrc, item).
-0000f270: 0a20 2020 2069 7465 6d2e 7570 6461 7465  .    item.update
-0000f280: 5f67 6678 203d 2070 6172 7469 616c 285f  _gfx = partial(_
-0000f290: 7570 6461 7465 5f67 6678 2c20 6974 656d  update_gfx, item
-0000f2a0: 290d 0a20 2020 2069 7465 6d2e 7365 745a  )..    item.setZ
-0000f2b0: 5661 6c75 6528 2d31 3029 0d0a 2020 2020  Value(-10)..    
-0000f2c0: 6178 2e61 6464 4974 656d 2869 7465 6d29  ax.addItem(item)
-0000f2d0: 0d0a 2020 2020 7265 7475 726e 2069 7465  ..    return ite
-0000f2e0: 6d0d 0a0d 0a0d 0a64 6566 2068 6561 746d  m......def heatm
-0000f2f0: 6170 2864 6174 6173 7263 2c20 6178 3d4e  ap(datasrc, ax=N
-0000f300: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0d  one, **kwargs):.
-0000f310: 0a20 2020 2027 2727 4578 7065 6e73 6976  .    '''Expensiv
-0000f320: 6520 6675 6e63 7469 6f6e 2e20 4f6e 6c79  e function. Only
-0000f330: 2075 7365 206f 6e20 736d 616c 6c20 6461   use on small da
-0000f340: 7461 2073 6574 732e 2053 6565 2048 6561  ta sets. See Hea
-0000f350: 746d 6170 4974 656d 2066 6f72 206b 7761  tmapItem for kwa
-0000f360: 7267 732e 2049 6e70 7574 2064 6174 6173  rgs. Input datas
-0000f370: 7263 0d0a 2020 2020 2020 2068 6173 2078  rc..       has x
-0000f380: 2028 7469 6d65 2920 696e 2069 6e64 6578   (time) in index
-0000f390: 206f 7220 6669 7273 7420 636f 6c75 6d6e   or first column
-0000f3a0: 2c20 7920 2870 7269 6365 2920 6173 2063  , y (price) as c
-0000f3b0: 6f6c 756d 6e20 6e61 6d65 732c 2061 6e64  olumn names, and
-0000f3c0: 2069 6e74 656e 7369 7479 2028 636f 6c6f   intensity (colo
-0000f3d0: 7229 2061 730d 0a20 2020 2020 2020 6365  r) as..       ce
-0000f3e0: 6c6c 2076 616c 7565 732e 2727 270d 0a20  ll values.'''.. 
-0000f3f0: 2020 2061 7820 3d20 5f63 7265 6174 655f     ax = _create_
-0000f400: 706c 6f74 2861 783d 6178 2c20 6d61 7869  plot(ax=ax, maxi
-0000f410: 6d69 7a65 3d46 616c 7365 290d 0a20 2020  mize=False)..   
-0000f420: 2069 6620 6178 2e76 622e 765f 7a6f 6f6d   if ax.vb.v_zoom
-0000f430: 5f73 6361 6c65 203e 3d20 302e 393a 0d0a  _scale >= 0.9:..
-0000f440: 2020 2020 2020 2020 6178 2e76 622e 765f          ax.vb.v_
-0000f450: 7a6f 6f6d 5f73 6361 6c65 203d 2030 2e36  zoom_scale = 0.6
-0000f460: 0d0a 2020 2020 6461 7461 7372 6320 3d20  ..    datasrc = 
-0000f470: 5f63 7265 6174 655f 6461 7461 7372 6328  _create_datasrc(
-0000f480: 6178 2c20 6461 7461 7372 6329 0d0a 2020  ax, datasrc)..  
-0000f490: 2020 6461 7461 7372 632e 7363 616c 655f    datasrc.scale_
-0000f4a0: 636f 6c73 203d 205b 5d20 2320 646f 6573  cols = [] # does
-0000f4b0: 6e27 7420 7363 616c 650d 0a20 2020 205f  n't scale..    _
-0000f4c0: 7365 745f 6461 7461 7372 6328 6178 2c20  set_datasrc(ax, 
-0000f4d0: 6461 7461 7372 6329 0d0a 2020 2020 6974  datasrc)..    it
-0000f4e0: 656d 203d 2048 6561 746d 6170 4974 656d  em = HeatmapItem
-0000f4f0: 2861 783d 6178 2c20 6461 7461 7372 633d  (ax=ax, datasrc=
-0000f500: 6461 7461 7372 632c 202a 2a6b 7761 7267  datasrc, **kwarg
-0000f510: 7329 0d0a 2020 2020 6974 656d 2e75 7064  s)..    item.upd
-0000f520: 6174 655f 6461 7461 203d 2070 6172 7469  ate_data = parti
-0000f530: 616c 285f 7570 6461 7465 5f64 6174 612c  al(_update_data,
-0000f540: 204e 6f6e 652c 204e 6f6e 652c 2069 7465   None, None, ite
-0000f550: 6d29 0d0a 2020 2020 6974 656d 2e75 7064  m)..    item.upd
-0000f560: 6174 655f 6766 7820 3d20 7061 7274 6961  ate_gfx = partia
-0000f570: 6c28 5f75 7064 6174 655f 6766 782c 2069  l(_update_gfx, i
-0000f580: 7465 6d29 0d0a 2020 2020 6974 656d 2e73  tem)..    item.s
-0000f590: 6574 5a56 616c 7565 282d 3330 290d 0a20  etZValue(-30).. 
-0000f5a0: 2020 2061 782e 6164 6449 7465 6d28 6974     ax.addItem(it
-0000f5b0: 656d 290d 0a20 2020 2069 6620 6178 2e76  em)..    if ax.v
-0000f5c0: 622e 6461 7461 7372 6320 6973 206e 6f74  b.datasrc is not
-0000f5d0: 204e 6f6e 6520 616e 6420 6e6f 7420 6178   None and not ax
-0000f5e0: 2e76 622e 6461 7461 7372 632e 7469 6d65  .vb.datasrc.time
-0000f5f0: 6261 7365 6428 293a 2023 206d 616e 7561  based(): # manua
-0000f600: 6c20 7a6f 6f6d 2075 7064 6174 650d 0a20  l zoom update.. 
-0000f610: 2020 2020 2020 2061 782e 7365 7458 4c69         ax.setXLi
-0000f620: 6e6b 284e 6f6e 6529 0d0a 2020 2020 2020  nk(None)..      
-0000f630: 2020 6966 2061 782e 7072 6576 5f61 783a    if ax.prev_ax:
-0000f640: 0d0a 2020 2020 2020 2020 2020 2020 6178  ..            ax
-0000f650: 2e70 7265 765f 6178 2e73 6574 5f76 6973  .prev_ax.set_vis
-0000f660: 6962 6c65 2878 6178 6973 3d54 7275 6529  ible(xaxis=True)
-0000f670: 0d0a 2020 2020 2020 2020 6466 203d 2061  ..        df = a
-0000f680: 782e 7662 2e64 6174 6173 7263 2e64 660d  x.vb.datasrc.df.
-0000f690: 0a20 2020 2020 2020 2070 7269 6365 7320  .        prices 
-0000f6a0: 3d20 6466 2e63 6f6c 756d 6e73 5b61 782e  = df.columns[ax.
-0000f6b0: 7662 2e64 6174 6173 7263 2e63 6f6c 5f64  vb.datasrc.col_d
-0000f6c0: 6174 615f 6f66 6673 6574 3a69 7465 6d2e  ata_offset:item.
-0000f6d0: 636f 6c5f 6461 7461 5f65 6e64 5d0d 0a20  col_data_end].. 
-0000f6e0: 2020 2020 2020 2064 656c 7461 5f70 7269         delta_pri
-0000f6f0: 6365 203d 2061 6273 2870 7269 6365 735b  ce = abs(prices[
-0000f700: 305d 202d 2070 7269 6365 735b 315d 290d  0] - prices[1]).
-0000f710: 0a20 2020 2020 2020 2061 782e 7662 2e73  .        ax.vb.s
-0000f720: 6574 5f72 616e 6765 2830 2c20 6d69 6e28  et_range(0, min(
-0000f730: 6466 2e63 6f6c 756d 6e73 5b31 3a5d 292c  df.columns[1:]),
-0000f740: 206c 656e 2864 6629 2c20 6d61 7828 6466   len(df), max(df
-0000f750: 2e63 6f6c 756d 6e73 5b31 3a5d 292b 6465  .columns[1:])+de
-0000f760: 6c74 615f 7072 6963 6529 0d0a 2020 2020  lta_price)..    
-0000f770: 7265 7475 726e 2069 7465 6d0d 0a0d 0a0d  return item.....
-0000f780: 0a64 6566 2062 6172 2878 2c20 793d 4e6f  .def bar(x, y=No
-0000f790: 6e65 2c20 7769 6474 683d 302e 382c 2061  ne, width=0.8, a
-0000f7a0: 783d 4e6f 6e65 2c20 636f 6c6f 7266 756e  x=None, colorfun
-0000f7b0: 633d 7374 7265 6e67 7468 5f63 6f6c 6f72  c=strength_color
-0000f7c0: 6669 6c74 6572 2c20 2a2a 6b77 6172 6773  filter, **kwargs
-0000f7d0: 293a 0d0a 2020 2020 2727 2742 6172 2070  ):..    '''Bar p
-0000f7e0: 6c6f 7473 2061 7265 2064 6563 6f75 706c  lots are decoupl
-0000f7f0: 6564 2e20 5573 6520 766f 6c75 6d65 5f6f  ed. Use volume_o
-0000f800: 6376 2829 2069 6620 796f 7520 7761 6e74  cv() if you want
-0000f810: 2061 2062 6172 2070 6c6f 7420 7768 6963   a bar plot whic
-0000f820: 6820 7265 6c61 7465 7320 746f 206f 7468  h relates to oth
-0000f830: 6572 2074 696d 6520 706c 6f74 732e 2727  er time plots.''
-0000f840: 270d 0a20 2020 2067 6c6f 6261 6c20 7269  '..    global ri
-0000f850: 6768 745f 6d61 7267 696e 5f63 616e 646c  ght_margin_candl
-0000f860: 6573 2c20 6d61 785f 7a6f 6f6d 5f70 6f69  es, max_zoom_poi
-0000f870: 6e74 730d 0a20 2020 2072 6967 6874 5f6d  nts..    right_m
-0000f880: 6172 6769 6e5f 6361 6e64 6c65 7320 3d20  argin_candles = 
-0000f890: 300d 0a20 2020 206d 6178 5f7a 6f6f 6d5f  0..    max_zoom_
-0000f8a0: 706f 696e 7473 203d 206d 696e 286d 6178  points = min(max
-0000f8b0: 5f7a 6f6f 6d5f 706f 696e 7473 2c20 3829  _zoom_points, 8)
-0000f8c0: 0d0a 2020 2020 6178 203d 205f 6372 6561  ..    ax = _crea
-0000f8d0: 7465 5f70 6c6f 7428 6178 3d61 782c 206d  te_plot(ax=ax, m
-0000f8e0: 6178 696d 697a 653d 4661 6c73 6529 0d0a  aximize=False)..
-0000f8f0: 2020 2020 6178 2e64 6563 6f75 706c 6528      ax.decouple(
-0000f900: 290d 0a20 2020 2064 6174 6173 7263 203d  )..    datasrc =
-0000f910: 205f 6372 6561 7465 5f64 6174 6173 7263   _create_datasrc
-0000f920: 2861 782c 2078 2c20 7929 0d0a 2020 2020  (ax, x, y)..    
-0000f930: 5f61 646a 7573 745f 6261 725f 6461 7461  _adjust_bar_data
-0000f940: 7372 6328 6461 7461 7372 632c 206f 7264  src(datasrc, ord
-0000f950: 6572 5f63 6f6c 733d 4661 6c73 6529 2023  er_cols=False) #
-0000f960: 2064 6f6e 2774 2072 6561 7272 616e 6765   don't rearrange
-0000f970: 2063 6f6c 756d 6e73 2c20 646f 6e65 2066   columns, done f
-0000f980: 6f72 2075 7320 696e 2076 6f6c 756d 655f  or us in volume_
-0000f990: 6f63 7628 290d 0a20 2020 2069 7465 6d20  ocv()..    item 
-0000f9a0: 3d20 766f 6c75 6d65 5f6f 6376 2864 6174  = volume_ocv(dat
-0000f9b0: 6173 7263 2c20 6361 6e64 6c65 5f77 6964  asrc, candle_wid
-0000f9c0: 7468 3d77 6964 7468 2c20 6178 3d61 782c  th=width, ax=ax,
-0000f9d0: 2063 6f6c 6f72 6675 6e63 3d63 6f6c 6f72   colorfunc=color
-0000f9e0: 6675 6e63 290d 0a20 2020 2069 7465 6d2e  func)..    item.
-0000f9f0: 7570 6461 7465 5f64 6174 6120 3d20 7061  update_data = pa
-0000fa00: 7274 6961 6c28 5f75 7064 6174 655f 6461  rtial(_update_da
-0000fa10: 7461 2c20 4e6f 6e65 2c20 5f61 646a 7573  ta, None, _adjus
-0000fa20: 745f 6261 725f 6461 7461 7372 632c 2069  t_bar_datasrc, i
-0000fa30: 7465 6d29 0d0a 2020 2020 6974 656d 2e75  tem)..    item.u
-0000fa40: 7064 6174 655f 6766 7820 3d20 7061 7274  pdate_gfx = part
-0000fa50: 6961 6c28 5f75 7064 6174 655f 6766 782c  ial(_update_gfx,
-0000fa60: 2069 7465 6d29 0d0a 2020 2020 6178 2e76   item)..    ax.v
-0000fa70: 622e 7072 655f 7072 6f63 6573 735f 6461  b.pre_process_da
-0000fa80: 7461 2829 0d0a 2020 2020 6966 2061 782e  ta()..    if ax.
-0000fa90: 7662 2e79 5f6d 696e 203e 3d20 303a 0d0a  vb.y_min >= 0:..
-0000faa0: 2020 2020 2020 2020 6178 2e76 622e 765f          ax.vb.v_
-0000fab0: 7a6f 6f6d 5f62 6173 656c 696e 6520 3d20  zoom_baseline = 
-0000fac0: 300d 0a20 2020 2072 6574 7572 6e20 6974  0..    return it
-0000fad0: 656d 0d0a 0d0a 0d0a 6465 6620 6869 7374  em......def hist
-0000fae0: 2878 2c20 6269 6e73 2c20 6178 3d4e 6f6e  (x, bins, ax=Non
-0000faf0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-0000fb00: 2020 2068 6973 745f 6461 7461 203d 2070     hist_data = p
-0000fb10: 642e 6375 7428 782c 2062 696e 733d 6269  d.cut(x, bins=bi
-0000fb20: 6e73 292e 7661 6c75 655f 636f 756e 7473  ns).value_counts
-0000fb30: 2829 0d0a 2020 2020 6461 7461 203d 205b  ()..    data = [
-0000fb40: 2869 2e6d 6964 2c30 2c68 6973 745f 6461  (i.mid,0,hist_da
-0000fb50: 7461 2e6c 6f63 5b69 5d2c 6869 7374 5f64  ta.loc[i],hist_d
-0000fb60: 6174 612e 6c6f 635b 695d 2920 666f 7220  ata.loc[i]) for 
-0000fb70: 6920 696e 2073 6f72 7465 6428 6869 7374  i in sorted(hist
-0000fb80: 5f64 6174 612e 696e 6465 7829 5d0d 0a20  _data.index)].. 
-0000fb90: 2020 2064 6620 3d20 7064 2e44 6174 6146     df = pd.DataF
-0000fba0: 7261 6d65 2864 6174 612c 2063 6f6c 756d  rame(data, colum
-0000fbb0: 6e73 3d5b 2778 272c 275f 6f70 5f27 2c27  ns=['x','_op_','
-0000fbc0: 5f63 6c5f 272c 2762 696e 275d 290d 0a20  _cl_','bin']).. 
-0000fbd0: 2020 2064 662e 7365 745f 696e 6465 7828     df.set_index(
-0000fbe0: 2778 272c 2069 6e70 6c61 6365 3d54 7275  'x', inplace=Tru
-0000fbf0: 6529 0d0a 2020 2020 6974 656d 203d 2062  e)..    item = b
-0000fc00: 6172 2864 662c 2061 783d 6178 290d 0a20  ar(df, ax=ax).. 
-0000fc10: 2020 2064 656c 2069 7465 6d2e 7570 6461     del item.upda
-0000fc20: 7465 5f64 6174 610d 0a20 2020 2072 6574  te_data..    ret
-0000fc30: 7572 6e20 6974 656d 0d0a 0d0a 0d0a 6465  urn item......de
-0000fc40: 6620 706c 6f74 2878 2c20 793d 4e6f 6e65  f plot(x, y=None
-0000fc50: 2c20 636f 6c6f 723d 4e6f 6e65 2c20 7769  , color=None, wi
-0000fc60: 6474 683d 312c 2061 783d 4e6f 6e65 2c20  dth=1, ax=None, 
-0000fc70: 7374 796c 653d 4e6f 6e65 2c20 6c65 6765  style=None, lege
-0000fc80: 6e64 3d4e 6f6e 652c 207a 6f6f 6d73 6361  nd=None, zoomsca
-0000fc90: 6c65 3d54 7275 652c 202a 2a6b 7761 7267  le=True, **kwarg
-0000fca0: 7329 3a0d 0a20 2020 2061 7820 3d20 5f63  s):..    ax = _c
-0000fcb0: 7265 6174 655f 706c 6f74 2861 783d 6178  reate_plot(ax=ax
-0000fcc0: 2c20 6d61 7869 6d69 7a65 3d46 616c 7365  , maximize=False
-0000fcd0: 290d 0a20 2020 2075 7365 645f 636f 6c6f  )..    used_colo
-0000fce0: 7220 3d20 5f67 6574 5f63 6f6c 6f72 2861  r = _get_color(a
-0000fcf0: 782c 2073 7479 6c65 2c20 636f 6c6f 7229  x, style, color)
-0000fd00: 0d0a 2020 2020 6461 7461 7372 6320 3d20  ..    datasrc = 
-0000fd10: 5f63 7265 6174 655f 6461 7461 7372 6328  _create_datasrc(
-0000fd20: 6178 2c20 782c 2079 290d 0a20 2020 2069  ax, x, y)..    i
-0000fd30: 6620 6e6f 7420 7a6f 6f6d 7363 616c 653a  f not zoomscale:
-0000fd40: 0d0a 2020 2020 2020 2020 6461 7461 7372  ..        datasr
-0000fd50: 632e 7363 616c 655f 636f 6c73 203d 205b  c.scale_cols = [
-0000fd60: 5d0d 0a20 2020 205f 7365 745f 6461 7461  ]..    _set_data
-0000fd70: 7372 6328 6178 2c20 6461 7461 7372 6329  src(ax, datasrc)
-0000fd80: 0d0a 2020 2020 6966 206c 6567 656e 6420  ..    if legend 
-0000fd90: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000fda0: 2020 2020 2020 5f63 7265 6174 655f 6c65        _create_le
-0000fdb0: 6765 6e64 2861 7829 0d0a 2020 2020 7820  gend(ax)..    x 
-0000fdc0: 3d20 6461 7461 7372 632e 7820 6966 206e  = datasrc.x if n
-0000fdd0: 6f74 2061 782e 7662 2e78 5f69 6e64 6578  ot ax.vb.x_index
-0000fde0: 6564 2065 6c73 6520 6461 7461 7372 632e  ed else datasrc.
-0000fdf0: 696e 6465 780d 0a20 2020 2079 203d 2064  index..    y = d
-0000fe00: 6174 6173 7263 2e79 202f 2061 782e 7662  atasrc.y / ax.vb
-0000fe10: 2e79 7363 616c 652e 7363 616c 6566 0d0a  .yscale.scalef..
-0000fe20: 2020 2020 6966 2061 782e 7662 2e79 7363      if ax.vb.ysc
-0000fe30: 616c 652e 7363 616c 6574 7970 6520 3d3d  ale.scaletype ==
-0000fe40: 2027 6c6f 6727 3a0d 0a20 2020 2020 2020   'log':..       
-0000fe50: 2079 203d 2079 202b 206c 6f67 5f70 6c6f   y = y + log_plo
-0000fe60: 745f 6f66 6673 6574 0d0a 2020 2020 6966  t_offset..    if
-0000fe70: 2073 7479 6c65 2069 7320 4e6f 6e65 206f   style is None o
-0000fe80: 7220 616e 7928 6368 2069 6e20 7374 796c  r any(ch in styl
-0000fe90: 6520 666f 7220 6368 2069 6e20 272d 5f2e  e for ch in '-_.
-0000fea0: 2729 3a0d 0a20 2020 2020 2020 2063 6f6e  '):..        con
-0000feb0: 6e65 6374 5f64 6f74 7320 3d20 2766 696e  nect_dots = 'fin
-0000fec0: 6974 6527 2023 2073 616d 6520 6173 206d  ite' # same as m
-0000fed0: 6174 706c 6f74 6c69 623b 2075 7365 2064  atplotlib; use d
-0000fee0: 6174 6173 7263 2e73 7461 6e64 616c 6f6e  atasrc.standalon
-0000fef0: 653d 5472 7565 2069 6620 796f 7520 7761  e=True if you wa
-0000ff00: 6e74 2074 6f20 6b65 6570 2073 6570 6172  nt to keep separ
-0000ff10: 6174 6520 696e 7465 7276 616c 7320 6f6e  ate intervals on
-0000ff20: 2061 2070 6c6f 740d 0a20 2020 2020 2020   a plot..       
-0000ff30: 2069 7465 6d20 3d20 6178 2e70 6c6f 7428   item = ax.plot(
-0000ff40: 782c 2079 2c20 7065 6e3d 5f6d 616b 6570  x, y, pen=_makep
-0000ff50: 656e 2863 6f6c 6f72 3d75 7365 645f 636f  en(color=used_co
-0000ff60: 6c6f 722c 2073 7479 6c65 3d73 7479 6c65  lor, style=style
-0000ff70: 2c20 7769 6474 683d 7769 6474 6829 2c20  , width=width), 
-0000ff80: 6e61 6d65 3d6c 6567 656e 642c 2063 6f6e  name=legend, con
-0000ff90: 6e65 6374 3d63 6f6e 6e65 6374 5f64 6f74  nect=connect_dot
-0000ffa0: 7329 0d0a 2020 2020 2020 2020 6974 656d  s)..        item
-0000ffb0: 2e73 6574 446f 776e 7361 6d70 6c69 6e67  .setDownsampling
-0000ffc0: 2861 7574 6f3d 5472 7565 2c20 6d65 7468  (auto=True, meth
-0000ffd0: 6f64 3d27 7375 6273 616d 706c 6527 290d  od='subsample').
-0000ffe0: 0a20 2020 2020 2020 2069 7465 6d2e 7365  .        item.se
-0000fff0: 745a 5661 6c75 6528 3529 0d0a 2020 2020  tZValue(5)..    
-00010000: 656c 7365 3a0d 0a20 2020 2020 2020 2073  else:..        s
-00010010: 796d 626f 6c20 3d20 7b27 7627 3a27 7427  ymbol = {'v':'t'
-00010020: 2c20 275e 273a 2774 3127 2c20 273e 273a  , '^':'t1', '>':
-00010030: 2774 3227 2c20 273c 273a 2774 3327 7d2e  't2', '<':'t3'}.
-00010040: 6765 7428 7374 796c 652c 2073 7479 6c65  get(style, style
-00010050: 2920 2320 7472 616e 736c 6174 6520 736f  ) # translate so
-00010060: 6d65 2073 696d 696c 6172 2073 7479 6c65  me similar style
-00010070: 730d 0a20 2020 2020 2020 2079 6669 6c74  s..        yfilt
-00010080: 6572 203d 2079 2e6e 6f74 6e75 6c6c 2829  er = y.notnull()
-00010090: 0d0a 2020 2020 2020 2020 7365 7220 3d20  ..        ser = 
-000100a0: 792e 6c6f 635b 7966 696c 7465 725d 0d0a  y.loc[yfilter]..
-000100b0: 2020 2020 2020 2020 7820 3d20 782e 6c6f          x = x.lo
-000100c0: 635b 7966 696c 7465 725d 2e76 616c 7565  c[yfilter].value
-000100d0: 7320 6966 2068 6173 6174 7472 2878 2c20  s if hasattr(x, 
-000100e0: 276c 6f63 2729 2065 6c73 6520 785b 7966  'loc') else x[yf
-000100f0: 696c 7465 725d 0d0a 2020 2020 2020 2020  ilter]..        
-00010100: 6974 656d 203d 2061 782e 706c 6f74 2878  item = ax.plot(x
-00010110: 2c20 7365 722e 7661 6c75 6573 2c20 7065  , ser.values, pe
-00010120: 6e3d 4e6f 6e65 2c20 7379 6d62 6f6c 3d73  n=None, symbol=s
-00010130: 796d 626f 6c2c 2073 796d 626f 6c50 656e  ymbol, symbolPen
-00010140: 3d4e 6f6e 652c 2073 796d 626f 6c53 697a  =None, symbolSiz
-00010150: 653d 372a 7769 6474 682c 2073 796d 626f  e=7*width, symbo
-00010160: 6c42 7275 7368 3d70 672e 6d6b 4272 7573  lBrush=pg.mkBrus
-00010170: 6828 7573 6564 5f63 6f6c 6f72 292c 206e  h(used_color), n
-00010180: 616d 653d 6c65 6765 6e64 290d 0a20 2020  ame=legend)..   
-00010190: 2020 2020 2069 6620 7769 6474 6820 3c20       if width < 
-000101a0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-000101b0: 6974 656d 2e6f 7074 735b 2761 6e74 6961  item.opts['antia
-000101c0: 6c69 6173 275d 203d 2054 7275 650d 0a20  lias'] = True.. 
-000101d0: 2020 2020 2020 2069 7465 6d2e 7363 6174         item.scat
-000101e0: 7465 722e 5f64 6f70 6169 6e74 203d 2069  ter._dopaint = i
-000101f0: 7465 6d2e 7363 6174 7465 722e 7061 696e  tem.scatter.pain
-00010200: 740d 0a20 2020 2020 2020 2069 7465 6d2e  t..        item.
-00010210: 7363 6174 7465 722e 7061 696e 7420 3d20  scatter.paint = 
-00010220: 7061 7274 6961 6c28 5f70 6169 6e74 5f73  partial(_paint_s
-00010230: 6361 7474 6572 2c20 6974 656d 2e73 6361  catter, item.sca
-00010240: 7474 6572 290d 0a20 2020 2020 2020 2023  tter)..        #
-00010250: 206f 7074 696d 697a 6520 2877 6865 6e20   optimize (when 
-00010260: 6861 7669 6e67 206c 6172 6765 206e 756d  having large num
-00010270: 6265 7220 6f66 2070 6f69 6e74 7329 2062  ber of points) b
-00010280: 7920 6967 6e6f 7269 6e67 2073 6361 7474  y ignoring scatt
-00010290: 6572 2063 6c69 636b 2064 6574 6563 7469  er click detecti
-000102a0: 6f6e 0d0a 2020 2020 2020 2020 5f64 756d  on..        _dum
-000102b0: 6d79 5f6d 6f75 7365 5f63 6c69 636b 203d  my_mouse_click =
-000102c0: 206c 616d 6264 6120 6576 3a20 300d 0a20   lambda ev: 0.. 
-000102d0: 2020 2020 2020 2069 7465 6d2e 7363 6174         item.scat
-000102e0: 7465 722e 6d6f 7573 6543 6c69 636b 4576  ter.mouseClickEv
-000102f0: 656e 7420 3d20 5f64 756d 6d79 5f6d 6f75  ent = _dummy_mou
-00010300: 7365 5f63 6c69 636b 0d0a 2020 2020 2020  se_click..      
-00010310: 2020 6974 656d 2e73 6574 5a56 616c 7565    item.setZValue
-00010320: 2831 3029 0d0a 2020 2020 6974 656d 2e6f  (10)..    item.o
-00010330: 7074 735b 2768 616e 6465 645f 636f 6c6f  pts['handed_colo
-00010340: 7227 5d20 3d20 636f 6c6f 720d 0a20 2020  r'] = color..   
-00010350: 2069 7465 6d2e 6178 203d 2061 780d 0a20   item.ax = ax.. 
-00010360: 2020 2069 7465 6d2e 6461 7461 7372 6320     item.datasrc 
-00010370: 3d20 6461 7461 7372 630d 0a20 2020 205f  = datasrc..    _
-00010380: 7570 6461 7465 5f73 6967 6e69 6669 6361  update_significa
-00010390: 6e74 7328 6178 2c20 6461 7461 7372 632c  nts(ax, datasrc,
-000103a0: 2066 6f72 6365 3d46 616c 7365 290d 0a20   force=False).. 
-000103b0: 2020 2069 7465 6d2e 7570 6461 7465 5f64     item.update_d
-000103c0: 6174 6120 3d20 7061 7274 6961 6c28 5f75  ata = partial(_u
-000103d0: 7064 6174 655f 6461 7461 2c20 4e6f 6e65  pdate_data, None
-000103e0: 2c20 4e6f 6e65 2c20 6974 656d 290d 0a20  , None, item).. 
-000103f0: 2020 2069 7465 6d2e 7570 6461 7465 5f67     item.update_g
-00010400: 6678 203d 2070 6172 7469 616c 285f 7570  fx = partial(_up
-00010410: 6461 7465 5f67 6678 2c20 6974 656d 290d  date_gfx, item).
-00010420: 0a20 2020 2023 2061 6464 206c 6567 656e  .    # add legen
-00010430: 6420 746f 206d 6169 6e20 6178 2c20 6e6f  d to main ax, no
-00010440: 7420 746f 206f 7665 726c 6179 0d0a 2020  t to overlay..  
-00010450: 2020 6178 6d20 3d20 6178 2e76 622e 6d61    axm = ax.vb.ma
-00010460: 7374 6572 5f76 6965 7762 6f78 2e70 6172  ster_viewbox.par
-00010470: 656e 7428 2920 6966 2061 782e 7662 2e6d  ent() if ax.vb.m
-00010480: 6173 7465 725f 7669 6577 626f 7820 656c  aster_viewbox el
-00010490: 7365 2061 780d 0a20 2020 2069 6620 6178  se ax..    if ax
-000104a0: 6d2e 6c65 6765 6e64 2069 7320 6e6f 7420  m.legend is not 
-000104b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
-000104c0: 6620 6c65 6765 6e64 2061 6e64 2061 786d  f legend and axm
-000104d0: 2021 3d20 6178 3a0d 0a20 2020 2020 2020   != ax:..       
-000104e0: 2020 2020 2061 786d 2e6c 6567 656e 642e       axm.legend.
-000104f0: 6164 6449 7465 6d28 6974 656d 2c20 6e61  addItem(item, na
-00010500: 6d65 3d6c 6567 656e 6429 0d0a 2020 2020  me=legend)..    
-00010510: 2020 2020 666f 7220 5f2c 6c61 6265 6c20      for _,label 
-00010520: 696e 2061 786d 2e6c 6567 656e 642e 6974  in axm.legend.it
-00010530: 656d 733a 0d0a 2020 2020 2020 2020 2020  ems:..          
-00010540: 2020 6966 206c 6162 656c 2e74 6578 7420    if label.text 
-00010550: 3d3d 206c 6567 656e 643a 0d0a 2020 2020  == legend:..    
-00010560: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00010570: 6c2e 7365 7441 7474 7228 276a 7573 7469  l.setAttr('justi
-00010580: 6679 272c 2027 6c65 6674 2729 0d0a 2020  fy', 'left')..  
-00010590: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000105a0: 6265 6c2e 7365 7454 6578 7428 6c61 6265  bel.setText(labe
-000105b0: 6c2e 7465 7874 2c20 636f 6c6f 723d 6c65  l.text, color=le
-000105c0: 6765 6e64 5f74 6578 745f 636f 6c6f 7229  gend_text_color)
-000105d0: 0d0a 2020 2020 7265 7475 726e 2069 7465  ..    return ite
-000105e0: 6d0d 0a0d 0a0d 0a64 6566 206c 6162 656c  m......def label
-000105f0: 7328 782c 2079 3d4e 6f6e 652c 206c 6162  s(x, y=None, lab
-00010600: 656c 733d 4e6f 6e65 2c20 636f 6c6f 723d  els=None, color=
-00010610: 4e6f 6e65 2c20 6178 3d4e 6f6e 652c 2061  None, ax=None, a
-00010620: 6e63 686f 723d 2830 2e35 2c31 2929 3a0d  nchor=(0.5,1)):.
-00010630: 0a20 2020 2061 7820 3d20 5f63 7265 6174  .    ax = _creat
-00010640: 655f 706c 6f74 2861 783d 6178 2c20 6d61  e_plot(ax=ax, ma
-00010650: 7869 6d69 7a65 3d46 616c 7365 290d 0a20  ximize=False).. 
-00010660: 2020 2075 7365 645f 636f 6c6f 7220 3d20     used_color = 
-00010670: 5f67 6574 5f63 6f6c 6f72 2861 782c 2027  _get_color(ax, '
-00010680: 3f27 2c20 636f 6c6f 7229 0d0a 2020 2020  ?', color)..    
-00010690: 6461 7461 7372 6320 3d20 5f63 7265 6174  datasrc = _creat
-000106a0: 655f 6461 7461 7372 6328 6178 2c20 782c  e_datasrc(ax, x,
-000106b0: 2079 2c20 6c61 6265 6c73 290d 0a20 2020   y, labels)..   
-000106c0: 2064 6174 6173 7263 2e73 6361 6c65 5f63   datasrc.scale_c
-000106d0: 6f6c 7320 3d20 5b5d 2023 2064 6f6e 2774  ols = [] # don't
-000106e0: 2075 7365 2074 6869 7320 666f 7220 7363   use this for sc
-000106f0: 616c 696e 670d 0a20 2020 205f 7365 745f  aling..    _set_
-00010700: 6461 7461 7372 6328 6178 2c20 6461 7461  datasrc(ax, data
-00010710: 7372 6329 0d0a 2020 2020 6974 656d 203d  src)..    item =
-00010720: 2053 6361 7474 6572 4c61 6265 6c49 7465   ScatterLabelIte
-00010730: 6d28 6178 3d61 782c 2064 6174 6173 7263  m(ax=ax, datasrc
-00010740: 3d64 6174 6173 7263 2c20 636f 6c6f 723d  =datasrc, color=
-00010750: 7573 6564 5f63 6f6c 6f72 2c20 616e 6368  used_color, anch
-00010760: 6f72 3d61 6e63 686f 7229 0d0a 2020 2020  or=anchor)..    
-00010770: 5f75 7064 6174 655f 7369 676e 6966 6963  _update_signific
-00010780: 616e 7473 2861 782c 2064 6174 6173 7263  ants(ax, datasrc
-00010790: 2c20 666f 7263 653d 4661 6c73 6529 0d0a  , force=False)..
-000107a0: 2020 2020 6974 656d 2e75 7064 6174 655f      item.update_
-000107b0: 6461 7461 203d 2070 6172 7469 616c 285f  data = partial(_
-000107c0: 7570 6461 7465 5f64 6174 612c 204e 6f6e  update_data, Non
-000107d0: 652c 204e 6f6e 652c 2069 7465 6d29 0d0a  e, None, item)..
-000107e0: 2020 2020 6974 656d 2e75 7064 6174 655f      item.update_
-000107f0: 6766 7820 3d20 7061 7274 6961 6c28 5f75  gfx = partial(_u
-00010800: 7064 6174 655f 6766 782c 2069 7465 6d29  pdate_gfx, item)
-00010810: 0d0a 2020 2020 6178 2e61 6464 4974 656d  ..    ax.addItem
-00010820: 2869 7465 6d29 0d0a 2020 2020 6966 2061  (item)..    if a
-00010830: 782e 7662 2e76 5f7a 6f6f 6d5f 7363 616c  x.vb.v_zoom_scal
-00010840: 6520 3e20 302e 393a 2023 2061 646a 7573  e > 0.9: # adjus
-00010850: 7420 746f 206d 616b 6520 6869 2f6c 6f20  t to make hi/lo 
-00010860: 7465 7874 2066 6974 0d0a 2020 2020 2020  text fit..      
-00010870: 2020 6178 2e76 622e 765f 7a6f 6f6d 5f73    ax.vb.v_zoom_s
-00010880: 6361 6c65 203d 2030 2e39 0d0a 2020 2020  cale = 0.9..    
-00010890: 7265 7475 726e 2069 7465 6d0d 0a0d 0a0d  return item.....
-000108a0: 0a64 6566 2061 6464 5f6c 6567 656e 6428  .def add_legend(
-000108b0: 7465 7874 2c20 6178 3d4e 6f6e 6529 3a0d  text, ax=None):.
-000108c0: 0a20 2020 2061 7820 3d20 5f63 7265 6174  .    ax = _creat
-000108d0: 655f 706c 6f74 2861 783d 6178 2c20 6d61  e_plot(ax=ax, ma
-000108e0: 7869 6d69 7a65 3d46 616c 7365 290d 0a20  ximize=False).. 
-000108f0: 2020 205f 6372 6561 7465 5f6c 6567 656e     _create_legen
-00010900: 6428 6178 290d 0a20 2020 2072 6f77 203d  d(ax)..    row =
-00010910: 2061 782e 6c65 6765 6e64 2e6c 6179 6f75   ax.legend.layou
-00010920: 742e 726f 7743 6f75 6e74 2829 0d0a 2020  t.rowCount()..  
-00010930: 2020 6c61 6265 6c20 3d20 7067 2e4c 6162    label = pg.Lab
-00010940: 656c 4974 656d 2874 6578 742c 2063 6f6c  elItem(text, col
-00010950: 6f72 3d6c 6567 656e 645f 7465 7874 5f63  or=legend_text_c
-00010960: 6f6c 6f72 2c20 6a75 7374 6966 793d 276c  olor, justify='l
-00010970: 6566 7427 290d 0a20 2020 2061 782e 6c65  eft')..    ax.le
-00010980: 6765 6e64 2e6c 6179 6f75 742e 6164 6449  gend.layout.addI
-00010990: 7465 6d28 6c61 6265 6c2c 2072 6f77 2c20  tem(label, row, 
-000109a0: 302c 2031 2c20 3229 0d0a 2020 2020 7265  0, 1, 2)..    re
-000109b0: 7475 726e 206c 6162 656c 0d0a 0d0a 0d0a  turn label......
-000109c0: 6465 6620 6669 6c6c 5f62 6574 7765 656e  def fill_between
-000109d0: 2870 6c6f 7430 2c20 706c 6f74 312c 2063  (plot0, plot1, c
-000109e0: 6f6c 6f72 3d4e 6f6e 6529 3a0d 0a20 2020  olor=None):..   
-000109f0: 2075 7365 645f 636f 6c6f 7220 3d20 6272   used_color = br
-00010a00: 6967 6874 656e 285f 6765 745f 636f 6c6f  ighten(_get_colo
-00010a10: 7228 706c 6f74 302e 6178 2c20 4e6f 6e65  r(plot0.ax, None
-00010a20: 2c20 636f 6c6f 7229 2c20 312e 3329 0d0a  , color), 1.3)..
-00010a30: 2020 2020 6974 656d 203d 2070 672e 4669      item = pg.Fi
-00010a40: 6c6c 4265 7477 6565 6e49 7465 6d28 706c  llBetweenItem(pl
-00010a50: 6f74 302c 2070 6c6f 7431 2c20 6272 7573  ot0, plot1, brus
-00010a60: 683d 7067 2e6d 6b42 7275 7368 2875 7365  h=pg.mkBrush(use
-00010a70: 645f 636f 6c6f 7229 290d 0a20 2020 2069  d_color))..    i
-00010a80: 7465 6d2e 6178 203d 2070 6c6f 7430 2e61  tem.ax = plot0.a
-00010a90: 780d 0a20 2020 2069 7465 6d2e 7365 745a  x..    item.setZ
-00010aa0: 5661 6c75 6528 2d34 3029 0d0a 2020 2020  Value(-40)..    
-00010ab0: 6974 656d 2e61 782e 6164 6449 7465 6d28  item.ax.addItem(
-00010ac0: 6974 656d 290d 0a20 2020 2072 6574 7572  item)..    retur
-00010ad0: 6e20 6974 656d 0d0a 0d0a 0d0a 6465 6620  n item......def 
-00010ae0: 7365 745f 785f 706f 7328 786d 696e 2c20  set_x_pos(xmin, 
-00010af0: 786d 6178 2c20 6178 3d4e 6f6e 6529 3a0d  xmax, ax=None):.
-00010b00: 0a20 2020 2061 7820 3d20 5f63 7265 6174  .    ax = _creat
-00010b10: 655f 706c 6f74 2861 783d 6178 2c20 6d61  e_plot(ax=ax, ma
-00010b20: 7869 6d69 7a65 3d46 616c 7365 290d 0a20  ximize=False).. 
-00010b30: 2020 2078 6964 7830 2c78 6964 7831 203d     xidx0,xidx1 =
-00010b40: 205f 7064 7469 6d65 3269 6e64 6578 2861   _pdtime2index(a
-00010b50: 782c 2070 642e 5365 7269 6573 285b 786d  x, pd.Series([xm
-00010b60: 696e 2c20 786d 6178 5d29 290d 0a20 2020  in, xmax]))..   
-00010b70: 2061 782e 7662 2e75 7064 6174 655f 795f   ax.vb.update_y_
-00010b80: 7a6f 6f6d 2878 6964 7830 2c20 7869 6478  zoom(xidx0, xidx
-00010b90: 3129 0d0a 2020 2020 5f72 6570 6169 6e74  1)..    _repaint
-00010ba0: 5f63 616e 646c 6573 2829 0d0a 0d0a 0d0a  _candles()......
-00010bb0: 6465 6620 7365 745f 795f 7261 6e67 6528  def set_y_range(
-00010bc0: 796d 696e 2c20 796d 6178 2c20 6178 3d4e  ymin, ymax, ax=N
-00010bd0: 6f6e 6529 3a0d 0a20 2020 2061 7820 3d20  one):..    ax = 
-00010be0: 5f63 7265 6174 655f 706c 6f74 2861 783d  _create_plot(ax=
-00010bf0: 6178 2c20 6d61 7869 6d69 7a65 3d46 616c  ax, maximize=Fal
-00010c00: 7365 290d 0a20 2020 2061 782e 7365 744c  se)..    ax.setL
-00010c10: 696d 6974 7328 794d 696e 3d79 6d69 6e2c  imits(yMin=ymin,
-00010c20: 2079 4d61 783d 796d 6178 290d 0a20 2020   yMax=ymax)..   
-00010c30: 2061 782e 7662 2e76 5f61 7574 6f7a 6f6f   ax.vb.v_autozoo
-00010c40: 6d20 3d20 4661 6c73 650d 0a20 2020 2061  m = False..    a
-00010c50: 782e 7662 2e73 6574 5f72 616e 6765 284e  x.vb.set_range(N
-00010c60: 6f6e 652c 2079 6d69 6e2c 204e 6f6e 652c  one, ymin, None,
-00010c70: 2079 6d61 7829 0d0a 0d0a 0d0a 6465 6620   ymax)......def 
-00010c80: 7365 745f 795f 7363 616c 6528 7973 6361  set_y_scale(ysca
-00010c90: 6c65 3d27 6c69 6e65 6172 272c 2061 783d  le='linear', ax=
-00010ca0: 4e6f 6e65 293a 0d0a 2020 2020 6178 203d  None):..    ax =
-00010cb0: 205f 6372 6561 7465 5f70 6c6f 7428 6178   _create_plot(ax
-00010cc0: 3d61 782c 206d 6178 696d 697a 653d 4661  =ax, maximize=Fa
-00010cd0: 6c73 6529 0d0a 2020 2020 6178 2e73 6574  lse)..    ax.set
-00010ce0: 4c6f 674d 6f64 6528 793d 2879 7363 616c  LogMode(y=(yscal
-00010cf0: 653d 3d27 6c6f 6727 2929 0d0a 2020 2020  e=='log'))..    
-00010d00: 6178 2e76 622e 7973 6361 6c65 203d 2059  ax.vb.yscale = Y
-00010d10: 5363 616c 6528 7973 6361 6c65 2c20 6178  Scale(yscale, ax
-00010d20: 2e76 622e 7973 6361 6c65 2e73 6361 6c65  .vb.yscale.scale
-00010d30: 6629 0d0a 0d0a 0d0a 6465 6620 6164 645f  f)......def add_
-00010d40: 6261 6e64 2879 302c 2079 312c 2063 6f6c  band(y0, y1, col
-00010d50: 6f72 3d62 616e 645f 636f 6c6f 722c 2061  or=band_color, a
-00010d60: 783d 4e6f 6e65 293a 0d0a 2020 2020 6178  x=None):..    ax
-00010d70: 203d 205f 6372 6561 7465 5f70 6c6f 7428   = _create_plot(
-00010d80: 6178 3d61 782c 206d 6178 696d 697a 653d  ax=ax, maximize=
-00010d90: 4661 6c73 6529 0d0a 2020 2020 636f 6c6f  False)..    colo
-00010da0: 7220 3d20 5f67 6574 5f63 6f6c 6f72 2861  r = _get_color(a
-00010db0: 782c 204e 6f6e 652c 2063 6f6c 6f72 290d  x, None, color).
-00010dc0: 0a20 2020 2069 7820 3d20 6178 2e76 622e  .    ix = ax.vb.
-00010dd0: 7973 6361 6c65 2e69 6e76 7866 6f72 6d0d  yscale.invxform.
-00010de0: 0a20 2020 206c 7220 3d20 7067 2e4c 696e  .    lr = pg.Lin
-00010df0: 6561 7252 6567 696f 6e49 7465 6d28 5b69  earRegionItem([i
-00010e00: 7828 7930 292c 6978 2879 3129 5d2c 206f  x(y0),ix(y1)], o
-00010e10: 7269 656e 7461 7469 6f6e 3d70 672e 4c69  rientation=pg.Li
-00010e20: 6e65 6172 5265 6769 6f6e 4974 656d 2e48  nearRegionItem.H
-00010e30: 6f72 697a 6f6e 7461 6c2c 2062 7275 7368  orizontal, brush
-00010e40: 3d70 672e 6d6b 4272 7573 6828 636f 6c6f  =pg.mkBrush(colo
-00010e50: 7229 2c20 6d6f 7661 626c 653d 4661 6c73  r), movable=Fals
-00010e60: 6529 0d0a 2020 2020 6c72 2e6c 696e 6573  e)..    lr.lines
-00010e70: 5b30 5d2e 7365 7450 656e 2870 672e 6d6b  [0].setPen(pg.mk
-00010e80: 5065 6e28 4e6f 6e65 2929 0d0a 2020 2020  Pen(None))..    
-00010e90: 6c72 2e6c 696e 6573 5b31 5d2e 7365 7450  lr.lines[1].setP
-00010ea0: 656e 2870 672e 6d6b 5065 6e28 4e6f 6e65  en(pg.mkPen(None
-00010eb0: 2929 0d0a 2020 2020 6c72 2e73 6574 5a56  ))..    lr.setZV
-00010ec0: 616c 7565 282d 3530 290d 0a20 2020 206c  alue(-50)..    l
-00010ed0: 722e 6178 203d 2061 780d 0a20 2020 2061  r.ax = ax..    a
-00010ee0: 782e 6164 6449 7465 6d28 6c72 290d 0a20  x.addItem(lr).. 
-00010ef0: 2020 2072 6574 7572 6e20 6c72 0d0a 0d0a     return lr....
-00010f00: 0d0a 6465 6620 6164 645f 7265 6374 2870  ..def add_rect(p
-00010f10: 302c 2070 312c 2063 6f6c 6f72 3d62 616e  0, p1, color=ban
-00010f20: 645f 636f 6c6f 722c 2069 6e74 6572 6163  d_color, interac
-00010f30: 7469 7665 3d46 616c 7365 2c20 6178 3d4e  tive=False, ax=N
-00010f40: 6f6e 6529 3a0d 0a20 2020 2061 7820 3d20  one):..    ax = 
-00010f50: 5f63 7265 6174 655f 706c 6f74 2861 783d  _create_plot(ax=
-00010f60: 6178 2c20 6d61 7869 6d69 7a65 3d46 616c  ax, maximize=Fal
-00010f70: 7365 290d 0a20 2020 2078 5f70 7473 203d  se)..    x_pts =
-00010f80: 205f 7064 7469 6d65 3269 6e64 6578 2861   _pdtime2index(a
-00010f90: 782c 2070 642e 5365 7269 6573 285b 7030  x, pd.Series([p0
-00010fa0: 5b30 5d2c 2070 315b 305d 5d29 290d 0a20  [0], p1[0]])).. 
-00010fb0: 2020 2069 7820 3d20 6178 2e76 622e 7973     ix = ax.vb.ys
-00010fc0: 6361 6c65 2e69 6e76 7866 6f72 6d0d 0a20  cale.invxform.. 
-00010fd0: 2020 2079 302c 7931 203d 2073 6f72 7465     y0,y1 = sorte
-00010fe0: 6428 5b70 305b 315d 2c20 7031 5b31 5d5d  d([p0[1], p1[1]]
-00010ff0: 290d 0a20 2020 2070 6f73 2020 3d20 2878  )..    pos  = (x
-00011000: 5f70 7473 5b30 5d2c 2069 7828 7930 2929  _pts[0], ix(y0))
-00011010: 0d0a 2020 2020 7369 7a65 203d 2028 785f  ..    size = (x_
-00011020: 7074 735b 315d 2d70 6f73 5b30 5d2c 2069  pts[1]-pos[0], i
-00011030: 7828 7931 292d 6978 2879 3029 290d 0a20  x(y1)-ix(y0)).. 
-00011040: 2020 2072 6563 7420 3d20 4669 6e52 6563     rect = FinRec
-00011050: 7428 6178 3d61 782c 2062 7275 7368 3d70  t(ax=ax, brush=p
-00011060: 672e 6d6b 4272 7573 6828 636f 6c6f 7229  g.mkBrush(color)
-00011070: 2c20 706f 733d 706f 732c 2073 697a 653d  , pos=pos, size=
-00011080: 7369 7a65 2c20 6d6f 7661 626c 653d 696e  size, movable=in
-00011090: 7465 7261 6374 6976 652c 2072 6573 697a  teractive, resiz
-000110a0: 6162 6c65 3d69 6e74 6572 6163 7469 7665  able=interactive
-000110b0: 2c20 726f 7461 7461 626c 653d 4661 6c73  , rotatable=Fals
-000110c0: 6529 0d0a 2020 2020 7265 6374 2e73 6574  e)..    rect.set
-000110d0: 5a56 616c 7565 282d 3430 290d 0a20 2020  ZValue(-40)..   
-000110e0: 2069 6620 696e 7465 7261 6374 6976 653a   if interactive:
-000110f0: 0d0a 2020 2020 2020 2020 6178 2e76 622e  ..        ax.vb.
-00011100: 726f 6973 2e61 7070 656e 6428 7265 6374  rois.append(rect
-00011110: 290d 0a20 2020 2072 6563 742e 6178 203d  )..    rect.ax =
-00011120: 2061 780d 0a20 2020 2061 782e 6164 6449   ax..    ax.addI
-00011130: 7465 6d28 7265 6374 290d 0a20 2020 2072  tem(rect)..    r
-00011140: 6574 7572 6e20 7265 6374 0d0a 0d0a 0d0a  eturn rect......
-00011150: 6465 6620 6164 645f 6c69 6e65 2870 302c  def add_line(p0,
-00011160: 2070 312c 2063 6f6c 6f72 3d64 7261 775f   p1, color=draw_
-00011170: 6c69 6e65 5f63 6f6c 6f72 2c20 7769 6474  line_color, widt
-00011180: 683d 312c 2073 7479 6c65 3d4e 6f6e 652c  h=1, style=None,
-00011190: 2069 6e74 6572 6163 7469 7665 3d46 616c   interactive=Fal
-000111a0: 7365 2c20 6178 3d4e 6f6e 6529 3a0d 0a20  se, ax=None):.. 
-000111b0: 2020 2061 7820 3d20 5f63 7265 6174 655f     ax = _create_
-000111c0: 706c 6f74 2861 783d 6178 2c20 6d61 7869  plot(ax=ax, maxi
-000111d0: 6d69 7a65 3d46 616c 7365 290d 0a20 2020  mize=False)..   
-000111e0: 2075 7365 645f 636f 6c6f 7220 3d20 5f67   used_color = _g
-000111f0: 6574 5f63 6f6c 6f72 2861 782c 2073 7479  et_color(ax, sty
-00011200: 6c65 2c20 636f 6c6f 7229 0d0a 2020 2020  le, color)..    
-00011210: 7065 6e20 3d20 5f6d 616b 6570 656e 2863  pen = _makepen(c
-00011220: 6f6c 6f72 3d75 7365 645f 636f 6c6f 722c  olor=used_color,
-00011230: 2073 7479 6c65 3d73 7479 6c65 2c20 7769   style=style, wi
-00011240: 6474 683d 7769 6474 6829 0d0a 2020 2020  dth=width)..    
-00011250: 785f 7074 7320 3d20 5f70 6474 696d 6532  x_pts = _pdtime2
-00011260: 696e 6465 7828 6178 2c20 7064 2e53 6572  index(ax, pd.Ser
-00011270: 6965 7328 5b70 305b 305d 2c20 7031 5b30  ies([p0[0], p1[0
-00011280: 5d5d 2929 0d0a 2020 2020 6978 203d 2061  ]]))..    ix = a
-00011290: 782e 7662 2e79 7363 616c 652e 696e 7678  x.vb.yscale.invx
-000112a0: 666f 726d 0d0a 2020 2020 7074 7320 3d20  form..    pts = 
-000112b0: 5b28 785f 7074 735b 305d 2c20 6978 2870  [(x_pts[0], ix(p
-000112c0: 305b 315d 2929 2c20 2878 5f70 7473 5b31  0[1])), (x_pts[1
-000112d0: 5d2c 2069 7828 7031 5b31 5d29 295d 0d0a  ], ix(p1[1]))]..
-000112e0: 2020 2020 6966 2069 6e74 6572 6163 7469      if interacti
-000112f0: 7665 3a0d 0a20 2020 2020 2020 206c 696e  ve:..        lin
-00011300: 6520 3d20 4669 6e50 6f6c 794c 696e 6528  e = FinPolyLine(
-00011310: 6178 2e76 622c 2070 7473 2c20 636c 6f73  ax.vb, pts, clos
-00011320: 6564 3d46 616c 7365 2c20 7065 6e3d 7065  ed=False, pen=pe
-00011330: 6e2c 206d 6f76 6162 6c65 3d46 616c 7365  n, movable=False
-00011340: 290d 0a20 2020 2020 2020 2061 782e 7662  )..        ax.vb
-00011350: 2e72 6f69 732e 6170 7065 6e64 286c 696e  .rois.append(lin
-00011360: 6529 0d0a 2020 2020 656c 7365 3a0d 0a20  e)..    else:.. 
-00011370: 2020 2020 2020 206c 696e 6520 3d20 4669         line = Fi
-00011380: 6e4c 696e 6528 7074 732c 2070 656e 3d70  nLine(pts, pen=p
-00011390: 656e 290d 0a20 2020 206c 696e 652e 6178  en)..    line.ax
-000113a0: 203d 2061 780d 0a20 2020 2061 782e 7662   = ax..    ax.vb
-000113b0: 2e61 6464 4974 656d 286c 696e 6529 0d0a  .addItem(line)..
-000113c0: 2020 2020 7265 7475 726e 206c 696e 650d      return line.
-000113d0: 0a0d 0a0d 0a64 6566 2061 6464 5f74 6578  .....def add_tex
-000113e0: 7428 706f 732c 2073 2c20 636f 6c6f 723d  t(pos, s, color=
-000113f0: 6472 6177 5f6c 696e 655f 636f 6c6f 722c  draw_line_color,
-00011400: 2061 6e63 686f 723d 2830 2c30 292c 2061   anchor=(0,0), a
-00011410: 783d 4e6f 6e65 293a 0d0a 2020 2020 6178  x=None):..    ax
-00011420: 203d 205f 6372 6561 7465 5f70 6c6f 7428   = _create_plot(
-00011430: 6178 3d61 782c 206d 6178 696d 697a 653d  ax=ax, maximize=
-00011440: 4661 6c73 6529 0d0a 2020 2020 636f 6c6f  False)..    colo
-00011450: 7220 3d20 5f67 6574 5f63 6f6c 6f72 2861  r = _get_color(a
-00011460: 782c 204e 6f6e 652c 2063 6f6c 6f72 290d  x, None, color).
-00011470: 0a20 2020 2074 6578 7420 3d20 7067 2e54  .    text = pg.T
-00011480: 6578 7449 7465 6d28 732c 2063 6f6c 6f72  extItem(s, color
-00011490: 3d63 6f6c 6f72 2c20 616e 6368 6f72 3d61  =color, anchor=a
-000114a0: 6e63 686f 7229 0d0a 2020 2020 7820 3d20  nchor)..    x = 
-000114b0: 706f 735b 305d 0d0a 2020 2020 6966 2061  pos[0]..    if a
-000114c0: 782e 7662 2e64 6174 6173 7263 2069 7320  x.vb.datasrc is 
-000114d0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-000114e0: 2020 2078 203d 205f 7064 7469 6d65 3269     x = _pdtime2i
-000114f0: 6e64 6578 2861 782c 2070 642e 5365 7269  ndex(ax, pd.Seri
-00011500: 6573 285b 706f 735b 305d 5d29 295b 305d  es([pos[0]]))[0]
-00011510: 0d0a 2020 2020 7920 3d20 6178 2e76 622e  ..    y = ax.vb.
-00011520: 7973 6361 6c65 2e69 6e76 7866 6f72 6d28  yscale.invxform(
-00011530: 706f 735b 315d 290d 0a20 2020 2074 6578  pos[1])..    tex
-00011540: 742e 7365 7450 6f73 2878 2c20 7929 0d0a  t.setPos(x, y)..
-00011550: 2020 2020 7465 7874 2e73 6574 5a56 616c      text.setZVal
-00011560: 7565 2835 3029 0d0a 2020 2020 7465 7874  ue(50)..    text
-00011570: 2e61 7820 3d20 6178 0d0a 2020 2020 6178  .ax = ax..    ax
-00011580: 2e61 6464 4974 656d 2874 6578 742c 2069  .addItem(text, i
-00011590: 676e 6f72 6542 6f75 6e64 733d 5472 7565  gnoreBounds=True
-000115a0: 290d 0a20 2020 2072 6574 7572 6e20 7465  )..    return te
-000115b0: 7874 0d0a 0d0a 0d0a 6465 6620 7265 6d6f  xt......def remo
-000115c0: 7665 5f6c 696e 6528 6c69 6e65 293a 0d0a  ve_line(line):..
-000115d0: 2020 2020 7072 696e 7428 2772 656d 6f76      print('remov
-000115e0: 655f 6c69 6e65 2829 2069 7320 6465 7072  e_line() is depr
-000115f0: 6563 6174 6564 2c20 7573 6520 7265 6d6f  ecated, use remo
-00011600: 7665 5f70 7269 6d69 7469 7665 2829 2069  ve_primitive() i
-00011610: 6e73 7465 6164 2729 0d0a 2020 2020 7265  nstead')..    re
-00011620: 6d6f 7665 5f70 7269 6d69 7469 7665 286c  move_primitive(l
-00011630: 696e 6529 0d0a 0d0a 0d0a 6465 6620 7265  ine)......def re
-00011640: 6d6f 7665 5f74 6578 7428 7465 7874 293a  move_text(text):
-00011650: 0d0a 2020 2020 7072 696e 7428 2772 656d  ..    print('rem
-00011660: 6f76 655f 7465 7874 2829 2069 7320 6465  ove_text() is de
-00011670: 7072 6563 6174 6564 2c20 7573 6520 7265  precated, use re
-00011680: 6d6f 7665 5f70 7269 6d69 7469 7665 2829  move_primitive()
-00011690: 2069 6e73 7465 6164 2729 0d0a 2020 2020   instead')..    
-000116a0: 7265 6d6f 7665 5f70 7269 6d69 7469 7665  remove_primitive
-000116b0: 2874 6578 7429 0d0a 0d0a 0d0a 6465 6620  (text)......def 
-000116c0: 7265 6d6f 7665 5f70 7269 6d69 7469 7665  remove_primitive
-000116d0: 2870 7269 6d69 7469 7665 293a 0d0a 2020  (primitive):..  
-000116e0: 2020 6178 203d 2070 7269 6d69 7469 7665    ax = primitive
-000116f0: 2e61 780d 0a20 2020 2061 782e 7662 2e72  .ax..    ax.vb.r
-00011700: 656d 6f76 6549 7465 6d28 7072 696d 6974  emoveItem(primit
-00011710: 6976 6529 0d0a 2020 2020 6966 2070 7269  ive)..    if pri
-00011720: 6d69 7469 7665 2069 6e20 6178 2e76 622e  mitive in ax.vb.
-00011730: 726f 6973 3a0d 0a20 2020 2020 2020 2061  rois:..        a
-00011740: 782e 7662 2e72 6f69 732e 7265 6d6f 7665  x.vb.rois.remove
-00011750: 2870 7269 6d69 7469 7665 290d 0a20 2020  (primitive)..   
-00011760: 2069 6620 6861 7361 7474 7228 7072 696d   if hasattr(prim
-00011770: 6974 6976 652c 2027 7465 7874 7327 293a  itive, 'texts'):
-00011780: 0d0a 2020 2020 2020 2020 666f 7220 7478  ..        for tx
-00011790: 7420 696e 2070 7269 6d69 7469 7665 2e74  t in primitive.t
-000117a0: 6578 7473 3a0d 0a20 2020 2020 2020 2020  exts:..         
-000117b0: 2020 2061 782e 7662 2e72 656d 6f76 6549     ax.vb.removeI
-000117c0: 7465 6d28 7478 7429 0d0a 0d0a 0d0a 6465  tem(txt)......de
-000117d0: 6620 7365 745f 7469 6d65 5f69 6e73 7065  f set_time_inspe
-000117e0: 6374 6f72 2869 6e73 7065 6374 6f72 2c20  ctor(inspector, 
-000117f0: 6178 3d4e 6f6e 652c 2077 6865 6e3d 2763  ax=None, when='c
-00011800: 6c69 636b 2729 3a0d 0a20 2020 2027 2727  lick'):..    '''
-00011810: 4361 6c6c 6261 636b 2077 6865 6e20 636c  Callback when cl
-00011820: 6963 6b65 6420 6c69 6b65 2073 6f3a 2069  icked like so: i
-00011830: 6e73 7065 6374 6f72 2878 2c20 7929 2e27  nspector(x, y).'
-00011840: 2727 0d0a 2020 2020 6178 203d 2061 7820  ''..    ax = ax 
-00011850: 6966 2061 7820 656c 7365 206c 6173 745f  if ax else last_
-00011860: 6178 0d0a 2020 2020 6d61 7374 6572 203d  ax..    master =
-00011870: 2061 782e 6178 5f77 6964 6765 7420 6966   ax.ax_widget if
-00011880: 2068 6173 6174 7472 2861 782c 2027 6178   hasattr(ax, 'ax
-00011890: 5f77 6964 6765 7427 2920 656c 7365 2061  _widget') else a
-000118a0: 782e 7662 2e77 696e 0d0a 2020 2020 6966  x.vb.win..    if
-000118b0: 2077 6865 6e20 3d3d 2027 686f 7665 7227   when == 'hover'
-000118c0: 3a0d 0a20 2020 2020 2020 206d 6173 7465  :..        maste
-000118d0: 722e 7072 6f78 795f 686f 7665 7220 3d20  r.proxy_hover = 
-000118e0: 7067 2e53 6967 6e61 6c50 726f 7879 286d  pg.SignalProxy(m
-000118f0: 6173 7465 722e 7363 656e 6528 292e 7369  aster.scene().si
-00011900: 674d 6f75 7365 4d6f 7665 642c 2072 6174  gMouseMoved, rat
-00011910: 654c 696d 6974 3d31 352c 2073 6c6f 743d  eLimit=15, slot=
-00011920: 7061 7274 6961 6c28 5f69 6e73 7065 6374  partial(_inspect
-00011930: 5f70 6f73 2c20 6178 2c20 696e 7370 6563  _pos, ax, inspec
-00011940: 746f 7229 290d 0a20 2020 2065 6c69 6620  tor))..    elif 
-00011950: 7768 656e 2069 6e20 2827 6463 6c69 636b  when in ('dclick
-00011960: 272c 2027 646f 7562 6c65 2d63 6c69 636b  ', 'double-click
-00011970: 2729 3a0d 0a20 2020 2020 2020 206d 6173  '):..        mas
-00011980: 7465 722e 7072 6f78 795f 6463 6c69 636b  ter.proxy_dclick
-00011990: 203d 2070 672e 5369 676e 616c 5072 6f78   = pg.SignalProx
-000119a0: 7928 6d61 7374 6572 2e73 6365 6e65 2829  y(master.scene()
-000119b0: 2e73 6967 4d6f 7573 6543 6c69 636b 6564  .sigMouseClicked
-000119c0: 2c20 736c 6f74 3d70 6172 7469 616c 285f  , slot=partial(_
-000119d0: 696e 7370 6563 745f 636c 6963 6b65 642c  inspect_clicked,
-000119e0: 2061 782c 2069 6e73 7065 6374 6f72 2c20   ax, inspector, 
-000119f0: 5472 7565 2929 0d0a 2020 2020 656c 7365  True))..    else
-00011a00: 3a0d 0a20 2020 2020 2020 206d 6173 7465  :..        maste
-00011a10: 722e 7072 6f78 795f 636c 6963 6b20 3d20  r.proxy_click = 
-00011a20: 7067 2e53 6967 6e61 6c50 726f 7879 286d  pg.SignalProxy(m
-00011a30: 6173 7465 722e 7363 656e 6528 292e 7369  aster.scene().si
-00011a40: 674d 6f75 7365 436c 6963 6b65 642c 2073  gMouseClicked, s
-00011a50: 6c6f 743d 7061 7274 6961 6c28 5f69 6e73  lot=partial(_ins
-00011a60: 7065 6374 5f63 6c69 636b 6564 2c20 6178  pect_clicked, ax
-00011a70: 2c20 696e 7370 6563 746f 722c 2046 616c  , inspector, Fal
-00011a80: 7365 2929 0d0a 0d0a 0d0a 6465 6620 6164  se))......def ad
-00011a90: 645f 6372 6f73 7368 6169 725f 696e 666f  d_crosshair_info
-00011aa0: 2869 6e66 6f66 756e 632c 2061 783d 4e6f  (infofunc, ax=No
-00011ab0: 6e65 293a 0d0a 2020 2020 2727 2743 616c  ne):..    '''Cal
-00011ac0: 6c62 6163 6b20 7768 656e 2063 726f 7373  lback when cross
-00011ad0: 6861 6972 2075 7064 6174 6564 206c 696b  hair updated lik
-00011ae0: 6520 736f 3a20 696e 666f 2861 782c 782c  e so: info(ax,x,
-00011af0: 792c 7874 6578 742c 7974 6578 7429 3b20  y,xtext,ytext); 
-00011b00: 7468 6520 696e 666f 2829 0d0a 2020 2020  the info()..    
-00011b10: 2020 2063 616c 6c62 6163 6b20 6d75 7374     callback must
-00011b20: 2072 6574 7572 6e20 7477 6f20 7661 6c75   return two valu
-00011b30: 6573 3a20 7874 6578 7420 616e 6420 7974  es: xtext and yt
-00011b40: 6578 742e 2727 270d 0a20 2020 2061 7820  ext.'''..    ax 
-00011b50: 3d20 5f63 7265 6174 655f 706c 6f74 2861  = _create_plot(a
-00011b60: 783d 6178 2c20 6d61 7869 6d69 7a65 3d46  x=ax, maximize=F
-00011b70: 616c 7365 290d 0a20 2020 2061 782e 6372  alse)..    ax.cr
-00011b80: 6f73 7368 6169 722e 696e 666f 732e 6170  osshair.infos.ap
-00011b90: 7065 6e64 2869 6e66 6f66 756e 6329 0d0a  pend(infofunc)..
-00011ba0: 0d0a 0d0a 6465 6620 7469 6d65 725f 6361  ....def timer_ca
-00011bb0: 6c6c 6261 636b 2875 7064 6174 655f 6675  llback(update_fu
-00011bc0: 6e63 2c20 7365 636f 6e64 732c 2073 696e  nc, seconds, sin
-00011bd0: 676c 655f 7368 6f74 3d46 616c 7365 293a  gle_shot=False):
-00011be0: 0d0a 2020 2020 676c 6f62 616c 2074 696d  ..    global tim
-00011bf0: 6572 730d 0a20 2020 2074 696d 6572 203d  ers..    timer =
-00011c00: 2051 7443 6f72 652e 5154 696d 6572 2829   QtCore.QTimer()
-00011c10: 0d0a 2020 2020 7469 6d65 722e 7469 6d65  ..    timer.time
-00011c20: 6f75 742e 636f 6e6e 6563 7428 7570 6461  out.connect(upda
-00011c30: 7465 5f66 756e 6329 0d0a 2020 2020 6966  te_func)..    if
-00011c40: 2073 696e 676c 655f 7368 6f74 3a0d 0a20   single_shot:.. 
-00011c50: 2020 2020 2020 2074 696d 6572 2e73 6574         timer.set
-00011c60: 5369 6e67 6c65 5368 6f74 2854 7275 6529  SingleShot(True)
-00011c70: 0d0a 2020 2020 7469 6d65 722e 7374 6172  ..    timer.star
-00011c80: 7428 696e 7428 7365 636f 6e64 732a 3130  t(int(seconds*10
-00011c90: 3030 2929 0d0a 2020 2020 7469 6d65 7273  00))..    timers
-00011ca0: 2e61 7070 656e 6428 7469 6d65 7229 0d0a  .append(timer)..
-00011cb0: 2020 2020 7265 7475 726e 2074 696d 6572      return timer
-00011cc0: 0d0a 0d0a 0d0a 6465 6620 6175 746f 7669  ......def autovi
-00011cd0: 6577 7265 7374 6f72 6528 656e 6162 6c65  ewrestore(enable
-00011ce0: 3d54 7275 6529 3a0d 0a20 2020 2027 2727  =True):..    '''
-00011cf0: 5265 7374 6f72 2066 756e 6374 696f 6e61  Restor functiona
-00011d00: 6c69 7479 2073 6176 6573 2076 6965 7720  lity saves view 
-00011d10: 7a6f 6f6d 2063 6f6f 7264 696e 6174 6573  zoom coordinates
-00011d20: 2077 6865 6e20 636c 6f73 696e 6720 6120   when closing a 
-00011d30: 7769 6e64 6f77 2c20 616e 640d 0a20 2020  window, and..   
-00011d40: 2020 2020 6c6f 6164 2074 6865 6d20 7768      load them wh
-00011d50: 656e 2063 7265 6174 696e 6720 7468 6520  en creating the 
-00011d60: 706c 6f74 2028 7769 7468 2074 6865 2073  plot (with the s
-00011d70: 616d 6520 6e61 6d65 2920 6167 6169 6e2e  ame name) again.
-00011d80: 2727 270d 0a20 2020 2067 6c6f 6261 6c20  '''..    global 
-00011d90: 7669 6577 7265 7374 6f72 650d 0a20 2020  viewrestore..   
-00011da0: 2076 6965 7772 6573 746f 7265 203d 2065   viewrestore = e
-00011db0: 6e61 626c 650d 0a0d 0a0d 0a64 6566 2072  nable......def r
-00011dc0: 6566 7265 7368 2829 3a0d 0a20 2020 2066  efresh():..    f
-00011dd0: 6f72 2077 696e 2069 6e20 7769 6e64 6f77  or win in window
-00011de0: 733a 0d0a 2020 2020 2020 2020 7662 7320  s:..        vbs 
-00011df0: 3d20 5b61 782e 7662 2066 6f72 2061 7820  = [ax.vb for ax 
-00011e00: 696e 2077 696e 2e61 7873 5d20 2b20 5b61  in win.axs] + [a
-00011e10: 782e 7662 2066 6f72 2061 7820 696e 206f  x.vb for ax in o
-00011e20: 7665 726c 6179 5f61 7873 2069 6620 6178  verlay_axs if ax
-00011e30: 2e76 622e 7769 6e3d 3d77 696e 5d0d 0a20  .vb.win==win].. 
-00011e40: 2020 2020 2020 2066 6f72 2076 6220 696e         for vb in
-00011e50: 2076 6273 3a0d 0a20 2020 2020 2020 2020   vbs:..         
-00011e60: 2020 2076 622e 7072 655f 7072 6f63 6573     vb.pre_proces
-00011e70: 735f 6461 7461 2829 0d0a 2020 2020 2020  s_data()..      
-00011e80: 2020 6966 2076 6965 7772 6573 746f 7265    if viewrestore
-00011e90: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00011ea0: 6620 5f6c 6f61 6477 696e 6461 7461 2877  f _loadwindata(w
-00011eb0: 696e 293a 0d0a 2020 2020 2020 2020 2020  in):..          
-00011ec0: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00011ed0: 2020 2020 2020 2020 5f73 6574 5f6d 6178          _set_max
-00011ee0: 5f7a 6f6f 6d28 7662 7329 0d0a 2020 2020  _zoom(vbs)..    
-00011ef0: 2020 2020 666f 7220 7662 2069 6e20 7662      for vb in vb
-00011f00: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00011f10: 6461 7461 7372 6320 3d20 7662 2e64 6174  datasrc = vb.dat
-00011f20: 6173 7263 5f6f 725f 7374 616e 6461 6c6f  asrc_or_standalo
-00011f30: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00011f40: 6966 2064 6174 6173 7263 2061 6e64 2028  if datasrc and (
-00011f50: 7662 2e6c 696e 6b65 6456 6965 7728 3029  vb.linkedView(0)
-00011f60: 2069 7320 4e6f 6e65 206f 7220 7662 2e6c   is None or vb.l
-00011f70: 696e 6b65 6456 6965 7728 3029 2e64 6174  inkedView(0).dat
-00011f80: 6173 7263 2069 7320 4e6f 6e65 206f 7220  asrc is None or 
-00011f90: 7662 2e6d 6173 7465 725f 7669 6577 626f  vb.master_viewbo
-00011fa0: 7829 3a0d 0a20 2020 2020 2020 2020 2020  x):..           
-00011fb0: 2020 2020 2076 622e 7570 6461 7465 5f79       vb.update_y
-00011fc0: 5f7a 6f6f 6d28 6461 7461 7372 632e 696e  _zoom(datasrc.in
-00011fd0: 6974 5f78 302c 2064 6174 6173 7263 2e69  it_x0, datasrc.i
-00011fe0: 6e69 745f 7831 290d 0a20 2020 205f 7265  nit_x1)..    _re
-00011ff0: 7061 696e 745f 6361 6e64 6c65 7328 290d  paint_candles().
-00012000: 0a20 2020 2066 6f72 2077 696e 2069 6e20  .    for win in 
-00012010: 7769 6e64 6f77 733a 0d0a 2020 2020 2020  windows:..      
-00012020: 2020 5f6d 6f75 7365 5f6d 6f76 6564 2877    _mouse_moved(w
-00012030: 696e 2c20 4e6f 6e65 290d 0a0d 0a0d 0a64  in, None)......d
-00012040: 6566 2073 686f 7728 7174 5f65 7865 633d  ef show(qt_exec=
-00012050: 5472 7565 293a 0d0a 2020 2020 7265 6672  True):..    refr
-00012060: 6573 6828 290d 0a20 2020 2066 6f72 2077  esh()..    for w
-00012070: 696e 2069 6e20 7769 6e64 6f77 733a 0d0a  in in windows:..
-00012080: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00012090: 7461 6e63 6528 7769 6e2c 2046 696e 5769  tance(win, FinWi
-000120a0: 6e64 6f77 2920 6f72 2071 745f 6578 6563  ndow) or qt_exec
-000120b0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-000120c0: 6620 7769 6e2e 7368 6f77 5f6d 6178 696d  f win.show_maxim
-000120d0: 697a 6564 3a0d 0a20 2020 2020 2020 2020  ized:..         
-000120e0: 2020 2020 2020 2077 696e 2e73 686f 774d         win.showM
-000120f0: 6178 696d 697a 6564 2829 0d0a 2020 2020  aximized()..    
-00012100: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00012110: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00012120: 696e 2e73 686f 7728 290d 0a20 2020 2069  in.show()..    i
-00012130: 6620 7769 6e64 6f77 7320 616e 6420 7174  f windows and qt
-00012140: 5f65 7865 633a 0d0a 2020 2020 2020 2020  _exec:..        
-00012150: 676c 6f62 616c 206c 6173 745f 6178 2c20  global last_ax, 
-00012160: 6170 700d 0a20 2020 2020 2020 2061 7070  app..        app
-00012170: 203d 2051 7447 7569 2e51 4775 6941 7070   = QtGui.QGuiApp
-00012180: 6c69 6361 7469 6f6e 2e69 6e73 7461 6e63  lication.instanc
-00012190: 6528 290d 0a20 2020 2020 2020 2061 7070  e()..        app
-000121a0: 2e65 7865 6328 290d 0a20 2020 2020 2020  .exec()..       
-000121b0: 2077 696e 646f 7773 2e63 6c65 6172 2829   windows.clear()
-000121c0: 0d0a 2020 2020 2020 2020 6f76 6572 6c61  ..        overla
-000121d0: 795f 6178 732e 636c 6561 7228 290d 0a20  y_axs.clear().. 
-000121e0: 2020 2020 2020 205f 636c 6561 725f 7469         _clear_ti
-000121f0: 6d65 7273 2829 0d0a 2020 2020 2020 2020  mers()..        
-00012200: 736f 756e 6473 2e63 6c65 6172 2829 0d0a  sounds.clear()..
-00012210: 2020 2020 2020 2020 6d61 7374 6572 5f64          master_d
-00012220: 6174 612e 636c 6561 7228 290d 0a20 2020  ata.clear()..   
-00012230: 2020 2020 206c 6173 745f 6178 203d 204e       last_ax = N
-00012240: 6f6e 650d 0a0d 0a0d 0a64 6566 2070 6c61  one......def pla
-00012250: 795f 736f 756e 6428 6669 6c65 6e61 6d65  y_sound(filename
-00012260: 293a 0d0a 2020 2020 6966 2066 696c 656e  ):..    if filen
-00012270: 616d 6520 6e6f 7420 696e 2073 6f75 6e64  ame not in sound
-00012280: 733a 0d0a 2020 2020 2020 2020 6672 6f6d  s:..        from
-00012290: 2050 7951 7436 2e51 744d 756c 7469 6d65   PyQt6.QtMultime
-000122a0: 6469 6120 696d 706f 7274 2051 536f 756e  dia import QSoun
-000122b0: 6445 6666 6563 740d 0a20 2020 2020 2020  dEffect..       
-000122c0: 2073 203d 2073 6f75 6e64 735b 6669 6c65   s = sounds[file
-000122d0: 6e61 6d65 5d20 3d20 5153 6f75 6e64 4566  name] = QSoundEf
-000122e0: 6665 6374 2829 2023 2064 6973 616c 6c6f  fect() # disallo
-000122f0: 7720 6763 0d0a 2020 2020 2020 2020 732e  w gc..        s.
-00012300: 7365 7453 6f75 7263 6528 5174 436f 7265  setSource(QtCore
-00012310: 2e51 5572 6c2e 6672 6f6d 4c6f 6361 6c46  .QUrl.fromLocalF
-00012320: 696c 6528 6669 6c65 6e61 6d65 2929 0d0a  ile(filename))..
-00012330: 2020 2020 7320 3d20 736f 756e 6473 5b66      s = sounds[f
-00012340: 696c 656e 616d 655d 0d0a 2020 2020 732e  ilename]..    s.
-00012350: 706c 6179 2829 0d0a 0d0a 0d0a 6465 6620  play()......def 
-00012360: 7363 7265 656e 7368 6f74 2866 696c 652c  screenshot(file,
-00012370: 2066 6d74 3d27 706e 6727 293a 0d0a 2020   fmt='png'):..  
-00012380: 2020 6966 205f 696e 7465 726e 616c 5f77    if _internal_w
-00012390: 696e 646f 7773 5f6f 6e6c 7928 2920 616e  indows_only() an
-000123a0: 6420 6e6f 7420 6170 703a 0d0a 2020 2020  d not app:..    
-000123b0: 2020 2020 7072 696e 7428 2745 5252 4f52      print('ERROR
-000123c0: 3a20 7363 7265 656e 7368 6f74 206d 7573  : screenshot mus
-000123d0: 7420 6265 2063 616c 6c62 6163 6b65 6420  t be callbacked 
-000123e0: 6672 6f6d 2065 2e67 2e20 7469 6d65 725f  from e.g. timer_
-000123f0: 6361 6c6c 6261 636b 2829 2729 0d0a 2020  callback()')..  
-00012400: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00012410: 7365 0d0a 2020 2020 7472 793a 0d0a 2020  se..    try:..  
-00012420: 2020 2020 2020 6275 6666 6572 203d 2051        buffer = Q
-00012430: 7443 6f72 652e 5142 7566 6665 7228 290d  tCore.QBuffer().
-00012440: 0a20 2020 2020 2020 2061 7070 2e70 7269  .        app.pri
-00012450: 6d61 7279 5363 7265 656e 2829 2e67 7261  maryScreen().gra
-00012460: 6257 696e 646f 7728 7769 6e64 6f77 735b  bWindow(windows[
-00012470: 305d 2e77 696e 4964 2829 292e 7361 7665  0].winId()).save
-00012480: 2862 7566 6665 722c 2066 6d74 290d 0a20  (buffer, fmt).. 
-00012490: 2020 2020 2020 2066 696c 652e 7772 6974         file.writ
-000124a0: 6528 6275 6666 6572 2e64 6174 6128 2929  e(buffer.data())
-000124b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000124c0: 2054 7275 650d 0a20 2020 2065 7863 6570   True..    excep
-000124d0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-000124e0: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-000124f0: 2827 5363 7265 656e 7368 6f74 2065 7272  ('Screenshot err
-00012500: 6f72 3a27 2c20 7479 7065 2865 292c 2065  or:', type(e), e
-00012510: 290d 0a20 2020 2072 6574 7572 6e20 4661  )..    return Fa
-00012520: 6c73 650d 0a0d 0a0d 0a64 6566 2065 7870  lse......def exp
-00012530: 6572 696d 656e 7428 2a61 7267 732c 202a  eriment(*args, *
-00012540: 2a6b 7761 7267 7329 3a0d 0a20 2020 2069  *kwargs):..    i
-00012550: 6620 276f 7065 6e67 6c27 2069 6e20 6172  f 'opengl' in ar
-00012560: 6773 206f 7220 6b77 6172 6773 2e67 6574  gs or kwargs.get
-00012570: 2827 6f70 656e 676c 2729 3a0d 0a20 2020  ('opengl'):..   
-00012580: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00012590: 2020 2020 2020 2023 2070 6970 2069 6e73         # pip ins
-000125a0: 7461 6c6c 2050 794f 7065 6e47 4c20 5079  tall PyOpenGL Py
-000125b0: 4f70 656e 474c 2d61 6363 656c 6572 6174  OpenGL-accelerat
-000125c0: 6520 746f 2067 6574 2074 6869 7320 676f  e to get this go
-000125d0: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
-000125e0: 2069 6d70 6f72 7420 4f70 656e 474c 0d0a   import OpenGL..
-000125f0: 2020 2020 2020 2020 2020 2020 7067 2e73              pg.s
-00012600: 6574 436f 6e66 6967 4f70 7469 6f6e 7328  etConfigOptions(
-00012610: 7573 654f 7065 6e47 4c3d 5472 7565 2c20  useOpenGL=True, 
-00012620: 656e 6162 6c65 4578 7065 7269 6d65 6e74  enableExperiment
-00012630: 616c 3d54 7275 6529 0d0a 2020 2020 2020  al=True)..      
-00012640: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00012650: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-00012660: 2020 2020 2020 7072 696e 7428 2757 4152        print('WAR
-00012670: 4e49 4e47 3a20 4f70 656e 474c 2069 6e69  NING: OpenGL ini
-00012680: 7420 6572 726f 722e 272c 2074 7970 6528  t error.', type(
-00012690: 6529 2c20 6529 0d0a 0d0a 0d0a 2323 2323  e), e)......####
-000126a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000126b0: 2049 4e54 4552 4e41 4c53 2023 2323 2323   INTERNALS #####
-000126c0: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-000126d0: 0a0d 0a0d 0a64 6566 205f 6f70 656e 6669  .....def _openfi
-000126e0: 6c65 282a 6172 6773 293a 0d0a 2020 2020  le(*args):..    
-000126f0: 7265 7475 726e 206f 7065 6e28 2a61 7267  return open(*arg
-00012700: 7329 0d0a 0d0a 0d0a 6465 6620 5f6c 6f61  s)......def _loa
-00012710: 6477 696e 6461 7461 2877 696e 293a 0d0a  dwindata(win):..
-00012720: 2020 2020 7472 793a 206f 732e 6d6b 6469      try: os.mkdi
-00012730: 7228 6f73 2e70 6174 682e 6578 7061 6e64  r(os.path.expand
-00012740: 7573 6572 2827 7e2f 2e66 696e 706c 6f74  user('~/.finplot
-00012750: 2729 290d 0a20 2020 2065 7863 6570 743a  '))..    except:
-00012760: 2070 6173 730d 0a20 2020 2074 7279 3a0d   pass..    try:.
-00012770: 0a20 2020 2020 2020 2066 203d 206f 732e  .        f = os.
-00012780: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-00012790: 277e 2f2e 6669 6e70 6c6f 742f 272b 7769  '~/.finplot/'+wi
-000127a0: 6e2e 7469 746c 652e 7265 706c 6163 6528  n.title.replace(
-000127b0: 272f 272c 272d 2729 2b27 2e69 6e69 2729  '/','-')+'.ini')
-000127c0: 0d0a 2020 2020 2020 2020 7365 7474 696e  ..        settin
-000127d0: 6773 203d 205b 286b 2e73 7472 6970 2829  gs = [(k.strip()
-000127e0: 2c6c 6974 6572 616c 5f65 7661 6c28 762e  ,literal_eval(v.
-000127f0: 7374 7269 7028 2929 2920 666f 7220 6c69  strip())) for li
-00012800: 6e65 2069 6e20 5f6f 7065 6e66 696c 6528  ne in _openfile(
-00012810: 6629 2066 6f72 206b 2c64 2c76 2069 6e20  f) for k,d,v in 
-00012820: 5b6c 696e 652e 7061 7274 6974 696f 6e28  [line.partition(
-00012830: 273d 2729 5d20 6966 2076 5d0d 0a20 2020  '=')] if v]..   
-00012840: 2065 7863 6570 743a 0d0a 2020 2020 2020   except:..      
-00012850: 2020 7265 7475 726e 0d0a 2020 2020 6b76    return..    kv
-00012860: 7320 3d20 7b6b 3a76 2066 6f72 206b 2c76  s = {k:v for k,v
-00012870: 2069 6e20 7365 7474 696e 6773 7d0d 0a20   in settings}.. 
-00012880: 2020 2076 6273 203d 2073 6574 2861 782e     vbs = set(ax.
-00012890: 7662 2066 6f72 2061 7820 696e 2077 696e  vb for ax in win
-000128a0: 2e61 7873 290d 0a20 2020 207a 6f6f 6d5f  .axs)..    zoom_
-000128b0: 7365 7420 3d20 4661 6c73 650d 0a20 2020  set = False..   
-000128c0: 2066 6f72 2076 6220 696e 2076 6273 3a0d   for vb in vbs:.
-000128d0: 0a20 2020 2020 2020 2064 7320 3d20 7662  .        ds = vb
-000128e0: 2e64 6174 6173 7263 0d0a 2020 2020 2020  .datasrc..      
-000128f0: 2020 6966 2064 7320 616e 6420 2876 622e    if ds and (vb.
-00012900: 6c69 6e6b 6564 5669 6577 2830 2920 6973  linkedView(0) is
-00012910: 204e 6f6e 6520 6f72 2076 622e 6c69 6e6b   None or vb.link
-00012920: 6564 5669 6577 2830 292e 6461 7461 7372  edView(0).datasr
-00012930: 6320 6973 204e 6f6e 6520 6f72 2076 622e  c is None or vb.
-00012940: 6d61 7374 6572 5f76 6965 7762 6f78 293a  master_viewbox):
-00012950: 0d0a 2020 2020 2020 2020 2020 2020 7065  ..            pe
-00012960: 7269 6f64 5f6e 7320 3d20 6473 2e70 6572  riod_ns = ds.per
-00012970: 696f 645f 6e73 0d0a 2020 2020 2020 2020  iod_ns..        
-00012980: 2020 2020 6966 206b 7673 5b27 6d69 6e5f      if kvs['min_
-00012990: 7827 5d20 3e3d 2064 732e 782e 696c 6f63  x'] >= ds.x.iloc
-000129a0: 5b30 5d2d 7065 7269 6f64 5f6e 7320 616e  [0]-period_ns an
-000129b0: 6420 6b76 735b 276d 6178 5f78 275d 203c  d kvs['max_x'] <
-000129c0: 3d20 6473 2e78 2e69 6c6f 635b 2d31 5d2b  = ds.x.iloc[-1]+
-000129d0: 7065 7269 6f64 5f6e 733a 0d0a 2020 2020  period_ns:..    
-000129e0: 2020 2020 2020 2020 2020 2020 7830 2c78              x0,x
-000129f0: 3120 3d20 6473 2e78 2e6c 6f63 5b64 732e  1 = ds.x.loc[ds.
-00012a00: 783e 3d6b 7673 5b27 6d69 6e5f 7827 5d5d  x>=kvs['min_x']]
-00012a10: 2e69 6e64 6578 5b30 5d2c 2064 732e 782e  .index[0], ds.x.
-00012a20: 6c6f 635b 6473 2e78 3c3d 6b76 735b 276d  loc[ds.x<=kvs['m
-00012a30: 6178 5f78 275d 5d2e 696e 6465 785b 2d31  ax_x']].index[-1
-00012a40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012a50: 2020 2069 6620 7831 203d 3d20 6c65 6e28     if x1 == len(
-00012a60: 6473 2e78 292d 313a 0d0a 2020 2020 2020  ds.x)-1:..      
-00012a70: 2020 2020 2020 2020 2020 2020 2020 7831                x1
-00012a80: 202b 3d20 7269 6768 745f 6d61 7267 696e   += right_margin
-00012a90: 5f63 616e 646c 6573 0d0a 2020 2020 2020  _candles..      
-00012aa0: 2020 2020 2020 2020 2020 7831 202b 3d20            x1 += 
-00012ab0: 302e 350d 0a20 2020 2020 2020 2020 2020  0.5..           
-00012ac0: 2020 2020 207a 6f6f 6d5f 7365 7420 3d20       zoom_set = 
-00012ad0: 7662 2e75 7064 6174 655f 795f 7a6f 6f6d  vb.update_y_zoom
-00012ae0: 2878 302c 2078 3129 0d0a 2020 2020 7265  (x0, x1)..    re
-00012af0: 7475 726e 207a 6f6f 6d5f 7365 740d 0a0d  turn zoom_set...
-00012b00: 0a0d 0a64 6566 205f 7361 7665 7769 6e64  ...def _savewind
-00012b10: 6174 6128 7769 6e29 3a0d 0a20 2020 2069  ata(win):..    i
-00012b20: 6620 6e6f 7420 7669 6577 7265 7374 6f72  f not viewrestor
-00012b30: 653a 0d0a 2020 2020 2020 2020 7265 7475  e:..        retu
-00012b40: 726e 0d0a 2020 2020 7472 793a 0d0a 2020  rn..    try:..  
-00012b50: 2020 2020 2020 6d69 6e5f 7820 3d20 696e        min_x = in
-00012b60: 7428 3165 3130 3029 0d0a 2020 2020 2020  t(1e100)..      
-00012b70: 2020 6d61 785f 7820 3d20 696e 7428 2d31    max_x = int(-1
-00012b80: 6531 3030 290d 0a20 2020 2020 2020 2066  e100)..        f
-00012b90: 6f72 2061 7820 696e 2077 696e 2e61 7873  or ax in win.axs
-00012ba0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00012bb0: 6620 6178 2e76 622e 7461 7267 6574 5265  f ax.vb.targetRe
-00012bc0: 6374 2829 2e72 6967 6874 2829 203c 2034  ct().right() < 4
-00012bd0: 3a20 2320 6967 6e6f 7265 2065 6d70 7479  : # ignore empty
-00012be0: 2070 6c6f 7473 0d0a 2020 2020 2020 2020   plots..        
-00012bf0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00012c00: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00012c10: 2061 782e 7662 2e64 6174 6173 7263 2069   ax.vb.datasrc i
-00012c20: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00012c30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00012c40: 650d 0a20 2020 2020 2020 2020 2020 2074  e..            t
-00012c50: 302c 7431 2c5f 2c5f 2c5f 203d 2061 782e  0,t1,_,_,_ = ax.
-00012c60: 7662 2e64 6174 6173 7263 2e68 696c 6f28  vb.datasrc.hilo(
-00012c70: 6178 2e76 622e 7461 7267 6574 5265 6374  ax.vb.targetRect
-00012c80: 2829 2e6c 6566 7428 292c 2061 782e 7662  ().left(), ax.vb
-00012c90: 2e74 6172 6765 7452 6563 7428 292e 7269  .targetRect().ri
-00012ca0: 6768 7428 2929 0d0a 2020 2020 2020 2020  ght())..        
-00012cb0: 2020 2020 6d69 6e5f 7820 3d20 6e70 2e6e      min_x = np.n
-00012cc0: 616e 6d69 6e28 5b6d 696e 5f78 2c20 7430  anmin([min_x, t0
-00012cd0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00012ce0: 6d61 785f 7820 3d20 6e70 2e6e 616e 6d61  max_x = np.nanma
-00012cf0: 7828 5b6d 6178 5f78 2c20 7431 5d29 0d0a  x([max_x, t1])..
-00012d00: 2020 2020 2020 2020 6966 206e 702e 6d61          if np.ma
-00012d10: 7828 6e70 2e61 6273 285b 6d69 6e5f 782c  x(np.abs([min_x,
-00012d20: 206d 6178 5f78 5d29 2920 3c20 3165 3939   max_x])) < 1e99
-00012d30: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00012d40: 203d 2027 6d69 6e5f 7820 3d20 2573 5c6e   = 'min_x = %s\n
-00012d50: 6d61 785f 7820 3d20 2573 5c6e 2720 2520  max_x = %s\n' % 
-00012d60: 286d 696e 5f78 2c20 6d61 785f 7829 0d0a  (min_x, max_x)..
-00012d70: 2020 2020 2020 2020 2020 2020 6620 3d20              f = 
-00012d80: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
-00012d90: 6572 2827 7e2f 2e66 696e 706c 6f74 2f27  er('~/.finplot/'
-00012da0: 2b77 696e 2e74 6974 6c65 2e72 6570 6c61  +win.title.repla
-00012db0: 6365 2827 2f27 2c27 2d27 292b 272e 696e  ce('/','-')+'.in
-00012dc0: 6927 290d 0a20 2020 2020 2020 2020 2020  i')..           
-00012dd0: 2074 7279 3a20 6368 616e 6765 6420 3d20   try: changed = 
-00012de0: 5f6f 7065 6e66 696c 6528 6629 2e72 6561  _openfile(f).rea
-00012df0: 6428 2920 213d 2073 0d0a 2020 2020 2020  d() != s..      
-00012e00: 2020 2020 2020 6578 6365 7074 3a20 6368        except: ch
-00012e10: 616e 6765 6420 3d20 5472 7565 0d0a 2020  anged = True..  
-00012e20: 2020 2020 2020 2020 2020 6966 2063 6861            if cha
-00012e30: 6e67 6564 3a0d 0a20 2020 2020 2020 2020  nged:..         
-00012e40: 2020 2020 2020 205f 6f70 656e 6669 6c65         _openfile
-00012e50: 2866 2c20 2777 7427 292e 7772 6974 6528  (f, 'wt').write(
-00012e60: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00012e70: 2020 2020 2323 2070 7269 6e74 2827 2573      ## print('%s
-00012e80: 2073 6176 6564 2720 2520 7769 6e2e 7469   saved' % win.ti
-00012e90: 746c 6529 0d0a 2020 2020 6578 6365 7074  tle)..    except
-00012ea0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00012eb0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00012ec0: 2745 7272 6f72 2073 6176 696e 6720 706c  'Error saving pl
-00012ed0: 6f74 3a27 2c20 6529 0d0a 0d0a 0d0a 6465  ot:', e)......de
-00012ee0: 6620 5f69 6e74 6572 6e61 6c5f 7769 6e64  f _internal_wind
-00012ef0: 6f77 735f 6f6e 6c79 2829 3a0d 0a20 2020  ows_only():..   
-00012f00: 2020 7265 7475 726e 2061 6c6c 2869 7369    return all(isi
-00012f10: 6e73 7461 6e63 6528 7769 6e2c 4669 6e57  nstance(win,FinW
-00012f20: 696e 646f 7729 2066 6f72 2077 696e 2069  indow) for win i
-00012f30: 6e20 7769 6e64 6f77 7329 0d0a 0d0a 0d0a  n windows)......
-00012f40: 6465 6620 5f63 7265 6174 655f 706c 6f74  def _create_plot
-00012f50: 2861 783d 4e6f 6e65 2c20 2a2a 6b77 6172  (ax=None, **kwar
-00012f60: 6773 293a 0d0a 2020 2020 6966 2061 783a  gs):..    if ax:
-00012f70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00012f80: 2061 780d 0a20 2020 2069 6620 6c61 7374   ax..    if last
-00012f90: 5f61 783a 0d0a 2020 2020 2020 2020 7265  _ax:..        re
-00012fa0: 7475 726e 206c 6173 745f 6178 0d0a 2020  turn last_ax..  
-00012fb0: 2020 7265 7475 726e 2063 7265 6174 655f    return create_
-00012fc0: 706c 6f74 282a 2a6b 7761 7267 7329 0d0a  plot(**kwargs)..
-00012fd0: 0d0a 0d0a 6465 6620 5f63 7265 6174 655f  ....def _create_
-00012fe0: 6178 6973 2870 6f73 2c20 2a2a 6b77 6172  axis(pos, **kwar
-00012ff0: 6773 293a 0d0a 2020 2020 6966 2070 6f73  gs):..    if pos
-00013000: 203d 3d20 2778 273a 0d0a 2020 2020 2020   == 'x':..      
-00013010: 2020 7265 7475 726e 2045 706f 6368 4178    return EpochAx
-00013020: 6973 4974 656d 282a 2a6b 7761 7267 7329  isItem(**kwargs)
-00013030: 0d0a 2020 2020 656c 6966 2070 6f73 203d  ..    elif pos =
-00013040: 3d20 2779 273a 0d0a 2020 2020 2020 2020  = 'y':..        
-00013050: 7265 7475 726e 2059 4178 6973 4974 656d  return YAxisItem
-00013060: 282a 2a6b 7761 7267 7329 0d0a 0d0a 0d0a  (**kwargs)......
-00013070: 6465 6620 5f63 6c65 6172 5f74 696d 6572  def _clear_timer
-00013080: 7328 293a 0d0a 2020 2020 666f 7220 7469  s():..    for ti
-00013090: 6d65 7220 696e 2074 696d 6572 733a 0d0a  mer in timers:..
-000130a0: 2020 2020 2020 2020 7469 6d65 722e 7469          timer.ti
-000130b0: 6d65 6f75 742e 6469 7363 6f6e 6e65 6374  meout.disconnect
-000130c0: 2829 0d0a 2020 2020 7469 6d65 7273 2e63  ()..    timers.c
-000130d0: 6c65 6172 2829 0d0a 0d0a 0d0a 6465 6620  lear()......def 
-000130e0: 5f61 6464 5f74 696d 6573 7461 6d70 5f70  _add_timestamp_p
-000130f0: 6c6f 7428 6d61 7374 6572 2c20 7072 6576  lot(master, prev
-00013100: 5f61 782c 2076 6965 7762 6f78 2c20 696e  _ax, viewbox, in
-00013110: 6465 782c 2079 7363 616c 6529 3a0d 0a20  dex, yscale):.. 
-00013120: 2020 206e 6174 6976 655f 7769 6e20 3d20     native_win = 
-00013130: 6973 696e 7374 616e 6365 286d 6173 7465  isinstance(maste
-00013140: 722c 2070 672e 4772 6170 6869 6373 4c61  r, pg.GraphicsLa
-00013150: 796f 7574 5769 6467 6574 290d 0a20 2020  youtWidget)..   
-00013160: 2069 6620 6e61 7469 7665 5f77 696e 2061   if native_win a
-00013170: 6e64 2070 7265 765f 6178 2069 7320 6e6f  nd prev_ax is no
-00013180: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00013190: 2070 7265 765f 6178 2e73 6574 5f76 6973   prev_ax.set_vis
-000131a0: 6962 6c65 2878 6178 6973 3d46 616c 7365  ible(xaxis=False
-000131b0: 2920 2320 6869 6465 2074 6865 2077 686f  ) # hide the who
-000131c0: 6c65 2070 7265 7669 6f75 7320 6178 6973  le previous axis
-000131d0: 0d0a 2020 2020 6178 6573 203d 207b 2762  ..    axes = {'b
-000131e0: 6f74 746f 6d27 3a20 5f63 7265 6174 655f  ottom': _create_
-000131f0: 6178 6973 2870 6f73 3d27 7827 2c20 7662  axis(pos='x', vb
-00013200: 3d76 6965 7762 6f78 2c20 6f72 6965 6e74  =viewbox, orient
-00013210: 6174 696f 6e3d 2762 6f74 746f 6d27 292c  ation='bottom'),
-00013220: 0d0a 2020 2020 2020 2020 2020 2020 2772  ..            'r
-00013230: 6967 6874 273a 2020 5f63 7265 6174 655f  ight':  _create_
-00013240: 6178 6973 2870 6f73 3d27 7927 2c20 7662  axis(pos='y', vb
-00013250: 3d76 6965 7762 6f78 2c20 6f72 6965 6e74  =viewbox, orient
-00013260: 6174 696f 6e3d 2772 6967 6874 2729 7d0d  ation='right')}.
-00013270: 0a20 2020 2069 6620 6e61 7469 7665 5f77  .    if native_w
-00013280: 696e 3a0d 0a20 2020 2020 2020 2061 7820  in:..        ax 
-00013290: 3d20 7067 2e50 6c6f 7449 7465 6d28 7669  = pg.PlotItem(vi
-000132a0: 6577 426f 783d 7669 6577 626f 782c 2061  ewBox=viewbox, a
-000132b0: 7869 7349 7465 6d73 3d61 7865 732c 206e  xisItems=axes, n
-000132c0: 616d 653d 2770 6c6f 742d 2569 2725 696e  ame='plot-%i'%in
-000132d0: 6465 782c 2065 6e61 626c 654d 656e 753d  dex, enableMenu=
-000132e0: 4661 6c73 6529 0d0a 2020 2020 656c 7365  False)..    else
-000132f0: 3a0d 0a20 2020 2020 2020 2061 7877 203d  :..        axw =
-00013300: 2070 672e 506c 6f74 5769 6467 6574 2876   pg.PlotWidget(v
-00013310: 6965 7742 6f78 3d76 6965 7762 6f78 2c20  iewBox=viewbox, 
-00013320: 6178 6973 4974 656d 733d 6178 6573 2c20  axisItems=axes, 
-00013330: 6e61 6d65 3d27 706c 6f74 2d25 6927 2569  name='plot-%i'%i
-00013340: 6e64 6578 2c20 656e 6162 6c65 4d65 6e75  ndex, enableMenu
-00013350: 3d46 616c 7365 290d 0a20 2020 2020 2020  =False)..       
-00013360: 2061 7820 3d20 6178 772e 706c 6f74 4974   ax = axw.plotIt
-00013370: 656d 0d0a 2020 2020 2020 2020 6178 2e61  em..        ax.a
-00013380: 785f 7769 6467 6574 203d 2061 7877 0d0a  x_widget = axw..
-00013390: 2020 2020 6178 2e68 6964 6541 7869 7328      ax.hideAxis(
-000133a0: 276c 6566 7427 290d 0a20 2020 2069 6620  'left')..    if 
-000133b0: 795f 6c61 6265 6c5f 7769 6474 683a 0d0a  y_label_width:..
-000133c0: 2020 2020 2020 2020 6178 2e61 7865 735b          ax.axes[
-000133d0: 2772 6967 6874 275d 5b27 6974 656d 275d  'right']['item']
-000133e0: 2e73 6574 5769 6474 6828 795f 6c61 6265  .setWidth(y_labe
-000133f0: 6c5f 7769 6474 6829 2023 2074 6869 7320  l_width) # this 
-00013400: 6973 2074 6f20 7075 7420 616c 6c20 6772  is to put all gr
-00013410: 6170 6873 206f 6e20 6571 7561 6c20 666f  aphs on equal fo
-00013420: 6f74 696e 6720 7768 656e 2074 6578 7473  oting when texts
-00013430: 2076 6172 7920 6672 6f6d 2030 2e34 2074   vary from 0.4 t
-00013440: 6f20 3230 3030 3030 300d 0a20 2020 2061  o 2000000..    a
-00013450: 782e 6178 6573 5b27 7269 6768 7427 5d5b  x.axes['right'][
-00013460: 2769 7465 6d27 5d2e 7365 7453 7479 6c65  'item'].setStyle
-00013470: 2874 6963 6b4c 656e 6774 683d 2d35 2920  (tickLength=-5) 
-00013480: 2320 736f 6d65 2062 7567 2c20 746f 7461  # some bug, tota
-00013490: 6c6c 7920 756e 6578 706c 6963 6162 6c65  lly unexplicable
-000134a0: 2028 7768 7920 7365 7474 696e 6720 7468   (why setting th
-000134b0: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
-000134c0: 6167 6169 6e20 776f 756c 6420 6669 7820  again would fix 
-000134d0: 7265 7061 696e 7420 7769 6474 6820 6173  repaint width as
-000134e0: 2061 7869 7320 7363 616c 6520 646f 776e   axis scale down
-000134f0: 290d 0a20 2020 2061 782e 6178 6573 5b27  )..    ax.axes['
-00013500: 7269 6768 7427 5d5b 2769 7465 6d27 5d2e  right']['item'].
-00013510: 7365 745a 5661 6c75 6528 3330 2920 2320  setZValue(30) # 
-00013520: 7075 7420 6178 6973 2069 6e20 6672 6f6e  put axis in fron
-00013530: 7420 696e 7374 6561 6420 6f66 2062 6568  t instead of beh
-00013540: 696e 6420 6461 7461 0d0a 2020 2020 6178  ind data..    ax
-00013550: 2e61 7865 735b 2762 6f74 746f 6d27 5d5b  .axes['bottom'][
-00013560: 2769 7465 6d27 5d2e 7365 745a 5661 6c75  'item'].setZValu
-00013570: 6528 3330 290d 0a20 2020 2061 782e 7365  e(30)..    ax.se
-00013580: 744c 6f67 4d6f 6465 2879 3d28 7973 6361  tLogMode(y=(ysca
-00013590: 6c65 2e73 6361 6c65 7479 7065 3d3d 276c  le.scaletype=='l
-000135a0: 6f67 2729 290d 0a20 2020 2061 782e 7369  og'))..    ax.si
-000135b0: 676e 6966 6963 616e 745f 6465 6369 6d61  gnificant_decima
-000135c0: 6c73 203d 2073 6967 6e69 6669 6361 6e74  ls = significant
-000135d0: 5f64 6563 696d 616c 730d 0a20 2020 2061  _decimals..    a
-000135e0: 782e 7369 676e 6966 6963 616e 745f 6570  x.significant_ep
-000135f0: 7320 3d20 7369 676e 6966 6963 616e 745f  s = significant_
-00013600: 6570 730d 0a20 2020 2061 782e 6372 6f73  eps..    ax.cros
-00013610: 7368 6169 7220 3d20 4669 6e43 726f 7373  shair = FinCross
-00013620: 4861 6972 2861 782c 2063 6f6c 6f72 3d63  Hair(ax, color=c
-00013630: 726f 7373 5f68 6169 725f 636f 6c6f 7229  ross_hair_color)
-00013640: 0d0a 2020 2020 6178 2e68 6964 6542 7574  ..    ax.hideBut
-00013650: 746f 6e73 2829 0d0a 2020 2020 6178 2e6f  tons()..    ax.o
-00013660: 7665 726c 6179 203d 2070 6172 7469 616c  verlay = partial
-00013670: 285f 6178 5f6f 7665 726c 6179 2c20 6178  (_ax_overlay, ax
-00013680: 290d 0a20 2020 2061 782e 7365 745f 7669  )..    ax.set_vi
-00013690: 7369 626c 6520 3d20 7061 7274 6961 6c28  sible = partial(
-000136a0: 5f61 785f 7365 745f 7669 7369 626c 652c  _ax_set_visible,
-000136b0: 2061 7829 0d0a 2020 2020 6178 2e64 6563   ax)..    ax.dec
-000136c0: 6f75 706c 6520 3d20 7061 7274 6961 6c28  ouple = partial(
-000136d0: 5f61 785f 6465 636f 7570 6c65 2c20 6178  _ax_decouple, ax
-000136e0: 290d 0a20 2020 2061 782e 6469 7361 626c  )..    ax.disabl
-000136f0: 655f 785f 696e 6465 7820 3d20 7061 7274  e_x_index = part
-00013700: 6961 6c28 5f61 785f 6469 7361 626c 655f  ial(_ax_disable_
-00013710: 785f 696e 6465 782c 2061 7829 0d0a 2020  x_index, ax)..  
-00013720: 2020 6178 2e72 6573 6574 203d 2070 6172    ax.reset = par
-00013730: 7469 616c 285f 6178 5f72 6573 6574 2c20  tial(_ax_reset, 
-00013740: 6178 290d 0a20 2020 2061 782e 7072 6576  ax)..    ax.prev
-00013750: 5f61 7820 3d20 7072 6576 5f61 780d 0a20  _ax = prev_ax.. 
-00013760: 2020 2061 782e 7769 6e5f 696e 6465 7820     ax.win_index 
-00013770: 3d20 696e 6465 780d 0a20 2020 2069 6620  = index..    if 
-00013780: 696e 6465 7825 323a 0d0a 2020 2020 2020  index%2:..      
-00013790: 2020 7669 6577 626f 782e 7365 7442 6163    viewbox.setBac
-000137a0: 6b67 726f 756e 6443 6f6c 6f72 286f 6464  kgroundColor(odd
-000137b0: 5f70 6c6f 745f 6261 636b 6772 6f75 6e64  _plot_background
-000137c0: 290d 0a20 2020 2076 6965 7762 6f78 2e73  )..    viewbox.s
-000137d0: 6574 5061 7265 6e74 2861 7829 0d0a 2020  etParent(ax)..  
-000137e0: 2020 7265 7475 726e 2061 780d 0a0d 0a0d    return ax.....
-000137f0: 0a64 6566 205f 6178 5f6f 7665 726c 6179  .def _ax_overlay
-00013800: 2861 782c 2073 6361 6c65 3d30 2e32 352c  (ax, scale=0.25,
-00013810: 2079 6178 6973 3d46 616c 7365 293a 0d0a   yaxis=False):..
-00013820: 2020 2020 2727 2754 6865 2073 6361 6c65      '''The scale
-00013830: 2070 6172 616d 6574 6572 2064 6566 696e   parameter defin
-00013840: 6573 2068 6f77 2022 6869 6768 2075 7022  es how "high up"
-00013850: 206f 6e20 7468 6520 696e 6974 6961 6c20   on the initial 
-00013860: 706c 6f74 2074 6869 7320 6f76 6572 6c61  plot this overla
-00013870: 7920 7769 6c6c 2073 686f 772e 0d0a 2020  y will show...  
-00013880: 2020 2020 2054 6865 2079 6178 6973 2070       The yaxis p
-00013890: 6172 616d 6574 6572 2063 616e 2062 6520  arameter can be 
-000138a0: 6f6e 6520 6f66 205b 4661 6c73 652c 2027  one of [False, '
-000138b0: 6c69 6e65 6172 272c 2027 6c6f 6727 5d2e  linear', 'log'].
-000138c0: 2727 270d 0a20 2020 2079 7363 616c 6520  '''..    yscale 
-000138d0: 3d20 7961 7869 7320 6966 2079 6178 6973  = yaxis if yaxis
-000138e0: 2065 6c73 6520 276c 696e 6561 7227 0d0a   else 'linear'..
-000138f0: 2020 2020 7669 6577 626f 7820 3d20 4669      viewbox = Fi
-00013900: 6e56 6965 7742 6f78 2861 782e 7662 2e77  nViewBox(ax.vb.w
-00013910: 696e 2c20 696e 6974 5f73 7465 7073 3d61  in, init_steps=a
-00013920: 782e 7662 2e69 6e69 745f 7374 6570 732c  x.vb.init_steps,
-00013930: 2079 7363 616c 653d 5953 6361 6c65 2879   yscale=YScale(y
-00013940: 7363 616c 652c 2031 292c 2065 6e61 626c  scale, 1), enabl
-00013950: 654d 656e 753d 4661 6c73 6529 0d0a 2020  eMenu=False)..  
-00013960: 2020 7669 6577 626f 782e 6d61 7374 6572    viewbox.master
-00013970: 5f76 6965 7762 6f78 203d 2061 782e 7662  _viewbox = ax.vb
-00013980: 0d0a 2020 2020 7669 6577 626f 782e 7365  ..    viewbox.se
-00013990: 745a 5661 6c75 6528 2d35 290d 0a20 2020  tZValue(-5)..   
-000139a0: 2076 6965 7762 6f78 2e73 6574 4261 636b   viewbox.setBack
-000139b0: 6772 6f75 6e64 436f 6c6f 7228 6178 2e76  groundColor(ax.v
-000139c0: 622e 7374 6174 655b 2762 6163 6b67 726f  b.state['backgro
-000139d0: 756e 6427 5d29 0d0a 2020 2020 6178 2e76  und'])..    ax.v
-000139e0: 622e 7365 7442 6163 6b67 726f 756e 6443  b.setBackgroundC
-000139f0: 6f6c 6f72 284e 6f6e 6529 0d0a 2020 2020  olor(None)..    
-00013a00: 7669 6577 626f 782e 765f 7a6f 6f6d 5f73  viewbox.v_zoom_s
-00013a10: 6361 6c65 203d 2073 6361 6c65 0d0a 2020  cale = scale..  
-00013a20: 2020 6966 2068 6173 6174 7472 2861 782c    if hasattr(ax,
-00013a30: 2027 6178 5f77 6964 6765 7427 293a 0d0a   'ax_widget'):..
-00013a40: 2020 2020 2020 2020 6178 2e61 785f 7769          ax.ax_wi
-00013a50: 6467 6574 2e73 6365 6e65 2829 2e61 6464  dget.scene().add
-00013a60: 4974 656d 2876 6965 7762 6f78 290d 0a20  Item(viewbox).. 
-00013a70: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00013a80: 2020 6178 2e76 622e 7769 6e2e 6365 6e74    ax.vb.win.cent
-00013a90: 7261 6c57 6964 6765 742e 7363 656e 6528  ralWidget.scene(
-00013aa0: 292e 6164 6449 7465 6d28 7669 6577 626f  ).addItem(viewbo
-00013ab0: 7829 0d0a 2020 2020 7669 6577 626f 782e  x)..    viewbox.
-00013ac0: 7365 7458 4c69 6e6b 2861 782e 7662 290d  setXLink(ax.vb).
-00013ad0: 0a20 2020 2064 6566 2075 7064 6174 6556  .    def updateV
-00013ae0: 6965 7728 293a 0d0a 2020 2020 2020 2020  iew():..        
-00013af0: 7669 6577 626f 782e 7365 7447 656f 6d65  viewbox.setGeome
-00013b00: 7472 7928 6178 2e76 622e 7363 656e 6542  try(ax.vb.sceneB
-00013b10: 6f75 6e64 696e 6752 6563 7428 2929 0d0a  oundingRect())..
-00013b20: 2020 2020 6178 6f20 3d20 7067 2e50 6c6f      axo = pg.Plo
-00013b30: 7449 7465 6d28 656e 6162 6c65 4d65 6e75  tItem(enableMenu
-00013b40: 3d46 616c 7365 290d 0a20 2020 2061 786f  =False)..    axo
-00013b50: 2e73 6967 6e69 6669 6361 6e74 5f64 6563  .significant_dec
-00013b60: 696d 616c 7320 3d20 7369 676e 6966 6963  imals = signific
-00013b70: 616e 745f 6465 6369 6d61 6c73 0d0a 2020  ant_decimals..  
-00013b80: 2020 6178 6f2e 7369 676e 6966 6963 616e    axo.significan
-00013b90: 745f 6570 7320 3d20 7369 676e 6966 6963  t_eps = signific
-00013ba0: 616e 745f 6570 730d 0a20 2020 2061 786f  ant_eps..    axo
-00013bb0: 2e76 6220 3d20 7669 6577 626f 780d 0a20  .vb = viewbox.. 
-00013bc0: 2020 2061 786f 2e70 7265 765f 6178 203d     axo.prev_ax =
-00013bd0: 204e 6f6e 650d 0a20 2020 2061 786f 2e63   None..    axo.c
-00013be0: 726f 7373 6861 6972 203d 204e 6f6e 650d  rosshair = None.
-00013bf0: 0a20 2020 2061 786f 2e64 6563 6f75 706c  .    axo.decoupl
-00013c00: 6520 3d20 7061 7274 6961 6c28 5f61 785f  e = partial(_ax_
-00013c10: 6465 636f 7570 6c65 2c20 6178 6f29 0d0a  decouple, axo)..
-00013c20: 2020 2020 6178 6f2e 6469 7361 626c 655f      axo.disable_
-00013c30: 785f 696e 6465 7820 3d20 7061 7274 6961  x_index = partia
-00013c40: 6c28 5f61 785f 6469 7361 626c 655f 785f  l(_ax_disable_x_
-00013c50: 696e 6465 782c 2061 786f 290d 0a20 2020  index, axo)..   
-00013c60: 2061 786f 2e72 6573 6574 203d 2070 6172   axo.reset = par
-00013c70: 7469 616c 285f 6178 5f72 6573 6574 2c20  tial(_ax_reset, 
-00013c80: 6178 6f29 0d0a 2020 2020 6178 6f2e 6869  axo)..    axo.hi
-00013c90: 6465 4178 6973 2827 6c65 6674 2729 0d0a  deAxis('left')..
-00013ca0: 2020 2020 6178 6f2e 6869 6465 4178 6973      axo.hideAxis
-00013cb0: 2827 7269 6768 7427 290d 0a20 2020 2061  ('right')..    a
-00013cc0: 786f 2e68 6964 6541 7869 7328 2762 6f74  xo.hideAxis('bot
-00013cd0: 746f 6d27 290d 0a20 2020 2061 786f 2e68  tom')..    axo.h
-00013ce0: 6964 6542 7574 746f 6e73 2829 0d0a 2020  ideButtons()..  
-00013cf0: 2020 7669 6577 626f 782e 6164 6449 7465    viewbox.addIte
-00013d00: 6d28 6178 6f29 0d0a 2020 2020 6966 2079  m(axo)..    if y
-00013d10: 6178 6973 2061 6e64 2069 7369 6e73 7461  axis and isinsta
-00013d20: 6e63 6528 6178 6f2e 7662 2e77 696e 2c20  nce(axo.vb.win, 
-00013d30: 7067 2e47 7261 7068 6963 734c 6179 6f75  pg.GraphicsLayou
-00013d40: 7457 6964 6765 7429 3a0d 0a20 2020 2020  tWidget):..     
-00013d50: 2020 2061 7869 203d 205f 6372 6561 7465     axi = _create
-00013d60: 5f61 7869 7328 706f 733d 2779 272c 2076  _axis(pos='y', v
-00013d70: 623d 6178 6f2e 7662 2c20 6f72 6965 6e74  b=axo.vb, orient
-00013d80: 6174 696f 6e3d 276c 6566 7427 290d 0a20  ation='left').. 
-00013d90: 2020 2020 2020 2061 786f 2e73 6574 4178         axo.setAx
-00013da0: 6973 4974 656d 7328 7b27 6c65 6674 273a  isItems({'left':
-00013db0: 2061 7869 7d29 0d0a 2020 2020 2020 2020   axi})..        
-00013dc0: 6178 6f2e 7662 2e77 696e 2e61 6464 4974  axo.vb.win.addIt
-00013dd0: 656d 2861 7869 2c20 726f 773d 302c 2063  em(axi, row=0, c
-00013de0: 6f6c 3d30 290d 0a20 2020 2061 782e 7662  ol=0)..    ax.vb
-00013df0: 2e73 6967 5265 7369 7a65 642e 636f 6e6e  .sigResized.conn
-00013e00: 6563 7428 7570 6461 7465 5669 6577 290d  ect(updateView).
-00013e10: 0a20 2020 206f 7665 726c 6179 5f61 7873  .    overlay_axs
-00013e20: 2e61 7070 656e 6428 6178 6f29 0d0a 2020  .append(axo)..  
-00013e30: 2020 7570 6461 7465 5669 6577 2829 0d0a    updateView()..
-00013e40: 2020 2020 7265 7475 726e 2061 786f 0d0a      return axo..
-00013e50: 0d0a 0d0a 6465 6620 5f61 785f 7365 745f  ....def _ax_set_
-00013e60: 7669 7369 626c 6528 6178 2c20 6372 6f73  visible(ax, cros
-00013e70: 7368 6169 723d 4e6f 6e65 2c20 7861 7869  shair=None, xaxi
-00013e80: 733d 4e6f 6e65 2c20 7961 7869 733d 4e6f  s=None, yaxis=No
-00013e90: 6e65 2c20 7867 7269 643d 4e6f 6e65 2c20  ne, xgrid=None, 
-00013ea0: 7967 7269 643d 4e6f 6e65 293a 0d0a 2020  ygrid=None):..  
-00013eb0: 2020 6966 2063 726f 7373 6861 6972 203d    if crosshair =
-00013ec0: 3d20 4661 6c73 653a 0d0a 2020 2020 2020  = False:..      
-00013ed0: 2020 6178 2e63 726f 7373 6861 6972 2e68    ax.crosshair.h
-00013ee0: 6964 6528 290d 0a20 2020 2069 6620 7861  ide()..    if xa
-00013ef0: 7869 7320 6973 206e 6f74 204e 6f6e 653a  xis is not None:
-00013f00: 0d0a 2020 2020 2020 2020 6178 2e67 6574  ..        ax.get
-00013f10: 4178 6973 2827 626f 7474 6f6d 2729 2e73  Axis('bottom').s
-00013f20: 6574 5374 796c 6528 7368 6f77 5661 6c75  etStyle(showValu
-00013f30: 6573 3d78 6178 6973 290d 0a20 2020 2069  es=xaxis)..    i
-00013f40: 6620 7961 7869 7320 6973 206e 6f74 204e  f yaxis is not N
-00013f50: 6f6e 653a 0d0a 2020 2020 2020 2020 6178  one:..        ax
-00013f60: 2e67 6574 4178 6973 2827 7269 6768 7427  .getAxis('right'
-00013f70: 292e 7365 7453 7479 6c65 2873 686f 7756  ).setStyle(showV
-00013f80: 616c 7565 733d 7961 7869 7329 0d0a 2020  alues=yaxis)..  
-00013f90: 2020 6966 2078 6772 6964 2069 7320 6e6f    if xgrid is no
-00013fa0: 7420 4e6f 6e65 206f 7220 7967 7269 6420  t None or ygrid 
-00013fb0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00013fc0: 2020 2020 2020 6178 2e73 686f 7747 7269        ax.showGri
-00013fd0: 6428 783d 7867 7269 642c 2079 3d79 6772  d(x=xgrid, y=ygr
-00013fe0: 6964 290d 0a20 2020 2020 2020 2069 6620  id)..        if 
-00013ff0: 6178 2e67 6574 4178 6973 2827 7269 6768  ax.getAxis('righ
-00014000: 7427 293a 0d0a 2020 2020 2020 2020 2020  t'):..          
-00014010: 2020 6178 2e67 6574 4178 6973 2827 7269    ax.getAxis('ri
-00014020: 6768 7427 292e 7365 7445 6e61 626c 6564  ght').setEnabled
-00014030: 2846 616c 7365 290d 0a20 2020 2020 2020  (False)..       
-00014040: 2069 6620 6178 2e67 6574 4178 6973 2827   if ax.getAxis('
-00014050: 626f 7474 6f6d 2729 3a0d 0a20 2020 2020  bottom'):..     
-00014060: 2020 2020 2020 2061 782e 6765 7441 7869         ax.getAxi
-00014070: 7328 2762 6f74 746f 6d27 292e 7365 7445  s('bottom').setE
-00014080: 6e61 626c 6564 2846 616c 7365 290d 0a0d  nabled(False)...
-00014090: 0a0d 0a64 6566 205f 6178 5f64 6563 6f75  ...def _ax_decou
-000140a0: 706c 6528 6178 293a 0d0a 2020 2020 6178  ple(ax):..    ax
-000140b0: 2e73 6574 584c 696e 6b28 4e6f 6e65 290d  .setXLink(None).
-000140c0: 0a20 2020 2069 6620 6178 2e70 7265 765f  .    if ax.prev_
-000140d0: 6178 3a0d 0a20 2020 2020 2020 2061 782e  ax:..        ax.
-000140e0: 7072 6576 5f61 782e 7365 745f 7669 7369  prev_ax.set_visi
-000140f0: 626c 6528 7861 7869 733d 5472 7565 290d  ble(xaxis=True).
-00014100: 0a0d 0a0d 0a64 6566 205f 6178 5f64 6973  .....def _ax_dis
-00014110: 6162 6c65 5f78 5f69 6e64 6578 2861 782c  able_x_index(ax,
-00014120: 2064 6563 6f75 706c 653d 5472 7565 293a   decouple=True):
-00014130: 0d0a 2020 2020 6178 2e76 622e 785f 696e  ..    ax.vb.x_in
-00014140: 6465 7865 6420 3d20 4661 6c73 650d 0a20  dexed = False.. 
-00014150: 2020 2069 6620 6465 636f 7570 6c65 3a0d     if decouple:.
-00014160: 0a20 2020 2020 2020 205f 6178 5f64 6563  .        _ax_dec
-00014170: 6f75 706c 6528 6178 290d 0a0d 0a0d 0a64  ouple(ax)......d
-00014180: 6566 205f 6178 5f72 6573 6574 2861 7829  ef _ax_reset(ax)
-00014190: 3a0d 0a20 2020 2069 6620 6178 2e63 726f  :..    if ax.cro
-000141a0: 7373 6861 6972 2069 7320 6e6f 7420 4e6f  sshair is not No
-000141b0: 6e65 3a0d 0a20 2020 2020 2020 2061 782e  ne:..        ax.
-000141c0: 6372 6f73 7368 6169 722e 6869 6465 2829  crosshair.hide()
-000141d0: 0d0a 2020 2020 666f 7220 6974 656d 2069  ..    for item i
-000141e0: 6e20 6c69 7374 2861 782e 6974 656d 7329  n list(ax.items)
-000141f0: 3a0d 0a20 2020 2020 2020 2061 782e 7265  :..        ax.re
-00014200: 6d6f 7665 4974 656d 2869 7465 6d29 0d0a  moveItem(item)..
-00014210: 2020 2020 2020 2020 6966 2061 782e 7662          if ax.vb
-00014220: 2e6d 6173 7465 725f 7669 6577 626f 7820  .master_viewbox 
-00014230: 616e 6420 6861 7361 7474 7228 6974 656d  and hasattr(item
-00014240: 2c20 276e 616d 6527 2920 616e 6420 6974  , 'name') and it
-00014250: 656d 2e6e 616d 6528 293a 0d0a 2020 2020  em.name():..    
-00014260: 2020 2020 2020 2020 6c65 6765 6e64 203d          legend =
-00014270: 2061 782e 7662 2e6d 6173 7465 725f 7669   ax.vb.master_vi
-00014280: 6577 626f 782e 7061 7265 6e74 2829 2e6c  ewbox.parent().l
-00014290: 6567 656e 640d 0a20 2020 2020 2020 2020  egend..         
-000142a0: 2020 2069 6620 6c65 6765 6e64 3a0d 0a20     if legend:.. 
-000142b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000142c0: 6567 656e 642e 7265 6d6f 7665 4974 656d  egend.removeItem
-000142d0: 2869 7465 6d29 0d0a 2020 2020 6966 2061  (item)..    if a
-000142e0: 782e 6c65 6765 6e64 3a0d 0a20 2020 2020  x.legend:..     
-000142f0: 2020 2061 782e 6c65 6765 6e64 2e6f 7074     ax.legend.opt
-00014300: 735b 276f 6666 7365 7427 5d20 3d20 4e6f  s['offset'] = No
-00014310: 6e65 0d0a 2020 2020 2020 2020 6178 2e6c  ne..        ax.l
-00014320: 6567 656e 642e 7365 7450 6172 656e 7449  egend.setParentI
-00014330: 7465 6d28 4e6f 6e65 290d 0a20 2020 2020  tem(None)..     
-00014340: 2020 2061 782e 6c65 6765 6e64 203d 204e     ax.legend = N
-00014350: 6f6e 650d 0a20 2020 2061 782e 7662 2e72  one..    ax.vb.r
-00014360: 6573 6574 2829 0d0a 2020 2020 6178 2e76  eset()..    ax.v
-00014370: 622e 7365 745f 6461 7461 7372 6328 4e6f  b.set_datasrc(No
-00014380: 6e65 290d 0a20 2020 2069 6620 6178 2e63  ne)..    if ax.c
-00014390: 726f 7373 6861 6972 2069 7320 6e6f 7420  rosshair is not 
-000143a0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2061  None:..        a
-000143b0: 782e 6372 6f73 7368 6169 722e 7368 6f77  x.crosshair.show
-000143c0: 2829 0d0a 0d0a 0d0a 6465 6620 5f63 7265  ()......def _cre
-000143d0: 6174 655f 6c65 6765 6e64 2861 7829 3a0d  ate_legend(ax):.
-000143e0: 0a20 2020 2069 6620 6178 2e76 622e 6d61  .    if ax.vb.ma
-000143f0: 7374 6572 5f76 6965 7762 6f78 3a0d 0a20  ster_viewbox:.. 
-00014400: 2020 2020 2020 2061 7820 3d20 6178 2e76         ax = ax.v
-00014410: 622e 6d61 7374 6572 5f76 6965 7762 6f78  b.master_viewbox
-00014420: 2e70 6172 656e 7428 290d 0a20 2020 2069  .parent()..    i
-00014430: 6620 6178 2e6c 6567 656e 6420 6973 204e  f ax.legend is N
-00014440: 6f6e 653a 0d0a 2020 2020 2020 2020 6178  one:..        ax
-00014450: 2e6c 6567 656e 6420 3d20 4669 6e4c 6567  .legend = FinLeg
-00014460: 656e 6449 7465 6d28 626f 7264 6572 5f63  endItem(border_c
-00014470: 6f6c 6f72 3d6c 6567 656e 645f 626f 7264  olor=legend_bord
-00014480: 6572 5f63 6f6c 6f72 2c20 6669 6c6c 5f63  er_color, fill_c
-00014490: 6f6c 6f72 3d6c 6567 656e 645f 6669 6c6c  olor=legend_fill
-000144a0: 5f63 6f6c 6f72 2c20 7369 7a65 3d4e 6f6e  _color, size=Non
-000144b0: 652c 206f 6666 7365 743d 2833 2c32 2929  e, offset=(3,2))
-000144c0: 0d0a 2020 2020 2020 2020 6178 2e6c 6567  ..        ax.leg
-000144d0: 656e 642e 7365 7450 6172 656e 7449 7465  end.setParentIte
-000144e0: 6d28 6178 2e76 6229 0d0a 0d0a 0d0a 6465  m(ax.vb)......de
-000144f0: 6620 5f75 7064 6174 655f 7369 676e 6966  f _update_signif
-00014500: 6963 616e 7473 2861 782c 2064 6174 6173  icants(ax, datas
-00014510: 7263 2c20 666f 7263 6529 3a0d 0a20 2020  rc, force):..   
-00014520: 2023 2063 6865 636b 2069 6620 6e6f 2065   # check if no e
-00014530: 7073 696c 6f6e 2073 6574 2079 6574 0d0a  psilon set yet..
-00014540: 2020 2020 6465 6661 756c 745f 6465 6320      default_dec 
-00014550: 3d20 302e 3939 203c 2061 782e 7369 676e  = 0.99 < ax.sign
-00014560: 6966 6963 616e 745f 6465 6369 6d61 6c73  ificant_decimals
-00014570: 2f73 6967 6e69 6669 6361 6e74 5f64 6563  /significant_dec
-00014580: 696d 616c 7320 3c20 312e 3031 0d0a 2020  imals < 1.01..  
-00014590: 2020 6465 6661 756c 745f 6570 7320 3d20    default_eps = 
-000145a0: 302e 3939 203c 2061 782e 7369 676e 6966  0.99 < ax.signif
-000145b0: 6963 616e 745f 6570 732f 7369 676e 6966  icant_eps/signif
-000145c0: 6963 616e 745f 6570 7320 3c20 312e 3031  icant_eps < 1.01
-000145d0: 0d0a 2020 2020 6966 2066 6f72 6365 206f  ..    if force o
-000145e0: 7220 2864 6566 6175 6c74 5f64 6563 2061  r (default_dec a
-000145f0: 6e64 2064 6566 6175 6c74 5f65 7073 293a  nd default_eps):
-00014600: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00014610: 2020 2020 2020 2020 2020 2020 7364 2c73              sd,s
-00014620: 6520 3d20 6461 7461 7372 632e 6361 6c63  e = datasrc.calc
-00014630: 5f73 6967 6e69 6669 6361 6e74 5f64 6563  _significant_dec
-00014640: 696d 616c 7328 290d 0a20 2020 2020 2020  imals()..       
-00014650: 2020 2020 2069 6620 7364 206f 7220 7365       if sd or se
-00014660: 2021 3d20 7369 676e 6966 6963 616e 745f   != significant_
-00014670: 6570 733a 0d0a 2020 2020 2020 2020 2020  eps:..          
-00014680: 2020 2020 2020 6966 2066 6f72 6365 206f        if force o
-00014690: 7220 6465 6661 756c 745f 6465 6320 6f72  r default_dec or
-000146a0: 2073 6420 3e20 6178 2e73 6967 6e69 6669   sd > ax.signifi
-000146b0: 6361 6e74 5f64 6563 696d 616c 733a 0d0a  cant_decimals:..
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 2020 2020 6178 2e73 6967 6e69 6669 6361      ax.significa
-000146e0: 6e74 5f64 6563 696d 616c 7320 3d20 7364  nt_decimals = sd
-000146f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014700: 2020 6966 2066 6f72 6365 206f 7220 6465    if force or de
-00014710: 6661 756c 745f 6570 7320 6f72 2073 6520  fault_eps or se 
-00014720: 3c20 6178 2e73 6967 6e69 6669 6361 6e74  < ax.significant
-00014730: 5f65 7073 3a0d 0a20 2020 2020 2020 2020  _eps:..         
-00014740: 2020 2020 2020 2020 2020 2061 782e 7369             ax.si
-00014750: 676e 6966 6963 616e 745f 6570 7320 3d20  gnificant_eps = 
-00014760: 7365 0d0a 2020 2020 2020 2020 6578 6365  se..        exce
-00014770: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
-00014780: 2070 6173 7320 2320 6461 7461 7372 6320   pass # datasrc 
-00014790: 7072 6f62 6162 6c79 2066 756c 6c20 6176  probably full av
-000147a0: 204e 614e 730d 0a0d 0a0d 0a64 6566 205f   NaNs......def _
-000147b0: 6973 5f73 7461 6e64 616c 6f6e 6528 7469  is_standalone(ti
-000147c0: 6d65 7365 7229 3a0d 0a20 2020 2023 206d  meser):..    # m
-000147d0: 6f72 6520 7468 616e 204e 2070 6572 6365  ore than N perce
-000147e0: 6e74 2067 6170 7320 6f72 2074 696d 6520  nt gaps or time 
-000147f0: 7265 7665 7273 616c 7320 7072 6f62 6162  reversals probab
-00014800: 6c79 206d 6561 6e73 2074 6869 7320 6973  ly means this is
-00014810: 2061 2073 7461 6e64 616c 6f6e 6520 706c   a standalone pl
-00014820: 6f74 0d0a 2020 2020 7265 7475 726e 2074  ot..    return t
-00014830: 696d 6573 6572 2e69 736e 756c 6c28 292e  imeser.isnull().
-00014840: 7375 6d28 2920 2b20 2874 696d 6573 6572  sum() + (timeser
-00014850: 2e64 6966 6628 293c 3d30 292e 7375 6d28  .diff()<=0).sum(
-00014860: 2920 3e20 6c65 6e28 7469 6d65 7365 7229  ) > len(timeser)
-00014870: 2a30 2e31 0d0a 0d0a 0d0a 6465 6620 5f63  *0.1......def _c
-00014880: 7265 6174 655f 7365 7269 6573 2861 293a  reate_series(a):
-00014890: 0d0a 2020 2020 7265 7475 726e 2061 2069  ..    return a i
-000148a0: 6620 6973 696e 7374 616e 6365 2861 2c20  f isinstance(a, 
-000148b0: 7064 2e53 6572 6965 7329 2065 6c73 6520  pd.Series) else 
-000148c0: 7064 2e53 6572 6965 7328 6129 0d0a 0d0a  pd.Series(a)....
-000148d0: 0d0a 6465 6620 5f63 7265 6174 655f 6461  ..def _create_da
-000148e0: 7461 7372 6328 6178 2c20 2a61 7267 7329  tasrc(ax, *args)
-000148f0: 3a0d 0a20 2020 2064 6566 2064 6f5f 6372  :..    def do_cr
-00014900: 6561 7465 2861 7267 7329 3a0d 0a20 2020  eate(args):..   
-00014910: 2020 2020 2069 6620 6c65 6e28 6172 6773       if len(args
-00014920: 2920 3d3d 2031 2061 6e64 2074 7970 6528  ) == 1 and type(
-00014930: 6172 6773 5b30 5d29 203d 3d20 5061 6e64  args[0]) == Pand
-00014940: 6173 4461 7461 536f 7572 6365 3a0d 0a20  asDataSource:.. 
-00014950: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014960: 6e20 6172 6773 5b30 5d0d 0a20 2020 2020  n args[0]..     
-00014970: 2020 2069 6620 6c65 6e28 6172 6773 2920     if len(args) 
-00014980: 3d3d 2031 2061 6e64 2074 7970 6528 6172  == 1 and type(ar
-00014990: 6773 5b30 5d29 2069 6e20 286c 6973 742c  gs[0]) in (list,
-000149a0: 2074 7570 6c65 293a 0d0a 2020 2020 2020   tuple):..      
-000149b0: 2020 2020 2020 6172 6773 203d 205b 6e70        args = [np
-000149c0: 2e61 7272 6179 2861 7267 735b 305d 295d  .array(args[0])]
-000149d0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-000149e0: 2861 7267 7329 203d 3d20 3120 616e 6420  (args) == 1 and 
-000149f0: 7479 7065 2861 7267 735b 305d 2920 3d3d  type(args[0]) ==
-00014a00: 206e 702e 6e64 6172 7261 793a 0d0a 2020   np.ndarray:..  
-00014a10: 2020 2020 2020 2020 2020 6172 6773 203d            args =
-00014a20: 205b 7064 2e44 6174 6146 7261 6d65 2861   [pd.DataFrame(a
-00014a30: 7267 735b 305d 2e54 295d 0d0a 2020 2020  rgs[0].T)]..    
-00014a40: 2020 2020 6966 206c 656e 2861 7267 7329      if len(args)
-00014a50: 203d 3d20 3120 616e 6420 7479 7065 2861   == 1 and type(a
-00014a60: 7267 735b 305d 2920 3d3d 2070 642e 4461  rgs[0]) == pd.Da
-00014a70: 7461 4672 616d 653a 0d0a 2020 2020 2020  taFrame:..      
-00014a80: 2020 2020 2020 7265 7475 726e 2050 616e        return Pan
-00014a90: 6461 7344 6174 6153 6f75 7263 6528 6172  dasDataSource(ar
-00014aa0: 6773 5b30 5d29 0d0a 2020 2020 2020 2020  gs[0])..        
-00014ab0: 6172 6773 203d 205b 5f63 7265 6174 655f  args = [_create_
-00014ac0: 7365 7269 6573 2861 2920 666f 7220 6120  series(a) for a 
-00014ad0: 696e 2061 7267 735d 0d0a 2020 2020 2020  in args]..      
-00014ae0: 2020 7265 7475 726e 2050 616e 6461 7344    return PandasD
-00014af0: 6174 6153 6f75 7263 6528 7064 2e63 6f6e  ataSource(pd.con
-00014b00: 6361 7428 6172 6773 2c20 6178 6973 3d31  cat(args, axis=1
-00014b10: 2929 0d0a 2020 2020 6961 7267 7320 3d20  ))..    iargs = 
-00014b20: 5b61 2066 6f72 2061 2069 6e20 6172 6773  [a for a in args
-00014b30: 2069 6620 6120 6973 206e 6f74 204e 6f6e   if a is not Non
-00014b40: 655d 0d0a 2020 2020 6461 7461 7372 6320  e]..    datasrc 
-00014b50: 3d20 646f 5f63 7265 6174 6528 6961 7267  = do_create(iarg
-00014b60: 7329 0d0a 2020 2020 2320 6368 6563 6b20  s)..    # check 
-00014b70: 6966 2074 696d 6520 636f 6c75 6d6e 206d  if time column m
-00014b80: 6973 7369 6e67 0d0a 2020 2020 6966 206c  issing..    if l
-00014b90: 656e 2864 6174 6173 7263 2e64 662e 636f  en(datasrc.df.co
-00014ba0: 6c75 6d6e 7329 203d 3d20 313a 0d0a 2020  lumns) == 1:..  
-00014bb0: 2020 2020 2020 2320 6173 7375 6d65 2074        # assume t
-00014bc0: 696d 6520 6461 7461 2068 6173 2061 6c72  ime data has alr
-00014bd0: 6561 6479 2062 6565 6e20 6164 6465 6420  eady been added 
-00014be0: 6265 666f 7265 0d0a 2020 2020 2020 2020  before..        
-00014bf0: 666f 7220 6120 696e 2061 782e 7662 2e77  for a in ax.vb.w
-00014c00: 696e 2e61 7873 3a0d 0a20 2020 2020 2020  in.axs:..       
-00014c10: 2020 2020 2069 6620 612e 7662 2e64 6174       if a.vb.dat
-00014c20: 6173 7263 2061 6e64 206c 656e 2861 2e76  asrc and len(a.v
-00014c30: 622e 6461 7461 7372 632e 6466 2e63 6f6c  b.datasrc.df.col
-00014c40: 756d 6e73 2920 3e3d 2032 3a0d 0a20 2020  umns) >= 2:..   
-00014c50: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00014c60: 6173 7263 2e64 662e 636f 6c75 6d6e 7320  asrc.df.columns 
-00014c70: 3d20 612e 7662 2e64 6174 6173 7263 2e64  = a.vb.datasrc.d
-00014c80: 662e 636f 6c75 6d6e 735b 313a 6c65 6e28  f.columns[1:len(
-00014c90: 6461 7461 7372 632e 6466 2e63 6f6c 756d  datasrc.df.colum
-00014ca0: 6e73 292b 315d 0d0a 2020 2020 2020 2020  ns)+1]..        
-00014cb0: 2020 2020 2020 2020 636f 6c20 3d20 612e          col = a.
-00014cc0: 7662 2e64 6174 6173 7263 2e64 662e 636f  vb.datasrc.df.co
-00014cd0: 6c75 6d6e 735b 305d 0d0a 2020 2020 2020  lumns[0]..      
-00014ce0: 2020 2020 2020 2020 2020 6461 7461 7372            datasr
-00014cf0: 632e 6466 2e69 6e73 6572 7428 302c 2063  c.df.insert(0, c
-00014d00: 6f6c 2c20 612e 7662 2e64 6174 6173 7263  ol, a.vb.datasrc
-00014d10: 2e64 665b 636f 6c5d 290d 0a20 2020 2020  .df[col])..     
-00014d20: 2020 2020 2020 2020 2020 2064 6174 6173             datas
-00014d30: 7263 203d 2050 616e 6461 7344 6174 6153  rc = PandasDataS
-00014d40: 6f75 7263 6528 6461 7461 7372 632e 6466  ource(datasrc.df
-00014d50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014d60: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
-00014d70: 2020 6966 206c 656e 2864 6174 6173 7263    if len(datasrc
-00014d80: 2e64 662e 636f 6c75 6d6e 7329 203d 3d20  .df.columns) == 
-00014d90: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-00014da0: 6461 7461 7372 6320 3d20 5061 6e64 6173  datasrc = Pandas
-00014db0: 4461 7461 536f 7572 6365 2864 6174 6173  DataSource(datas
-00014dc0: 7263 2e64 662e 7265 7365 745f 696e 6465  rc.df.reset_inde
-00014dd0: 7828 2929 0d0a 2020 2020 656c 6966 206c  x())..    elif l
-00014de0: 656e 2869 6172 6773 2920 3e3d 2032 2061  en(iargs) >= 2 a
-00014df0: 6e64 206c 656e 2864 6174 6173 7263 2e64  nd len(datasrc.d
-00014e00: 662e 636f 6c75 6d6e 7329 203d 3d20 6c65  f.columns) == le
-00014e10: 6e28 6961 7267 7329 2b31 2061 6e64 206c  n(iargs)+1 and l
-00014e20: 656e 2869 6172 6773 2920 3d3d 206c 656e  en(iargs) == len
-00014e30: 2861 7267 7329 3a0d 0a20 2020 2020 2020  (args):..       
-00014e40: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00014e50: 2020 2069 6620 272e 496e 7427 2069 6e20     if '.Int' in 
-00014e60: 7374 7228 7479 7065 2869 6172 6773 5b30  str(type(iargs[0
-00014e70: 5d2e 696e 6465 7829 293a 0d0a 2020 2020  ].index)):..    
-00014e80: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00014e90: 7428 2757 4152 4e49 4e47 3a20 7065 7266  t('WARNING: perf
-00014ea0: 6f72 6d61 6e63 6520 7065 6e61 6c74 7920  ormance penalty 
-00014eb0: 616e 6420 6372 6173 6820 6d61 7920 6f63  and crash may oc
-00014ec0: 6375 7220 7768 656e 2075 7369 6e67 2069  cur when using i
-00014ed0: 6e74 3634 2069 6e73 7465 6164 206f 6620  nt64 instead of 
-00014ee0: 7261 6e67 6520 696e 6469 6365 732e 2729  range indices.')
-00014ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014f00: 2020 6966 2028 6961 7267 735b 305d 2e69    if (iargs[0].i
-00014f10: 6e64 6578 203d 3d20 7261 6e67 6528 6c65  ndex == range(le
-00014f20: 6e28 6961 7267 735b 305d 2929 292e 616c  n(iargs[0]))).al
-00014f30: 6c28 293a 0d0a 2020 2020 2020 2020 2020  l():..          
-00014f40: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00014f50: 2720 2d20 4669 7820 6279 202e 7265 7365  ' - Fix by .rese
-00014f60: 745f 696e 6465 7828 6472 6f70 3d54 7275  t_index(drop=Tru
-00014f70: 6529 2729 0d0a 2020 2020 2020 2020 2020  e)')..          
-00014f80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014f90: 205f 6372 6561 7465 5f64 6174 6173 7263   _create_datasrc
-00014fa0: 2861 782c 2064 6174 6173 7263 2e64 665b  (ax, datasrc.df[
-00014fb0: 6461 7461 7372 632e 6466 2e63 6f6c 756d  datasrc.df.colum
-00014fc0: 6e73 5b31 3a5d 5d29 0d0a 2020 2020 2020  ns[1:]])..      
-00014fd0: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-00014fe0: 2020 2020 2020 2070 7269 6e74 2827 5741         print('WA
-00014ff0: 524e 494e 473a 2069 6e70 7574 2064 6174  RNING: input dat
-00015000: 6120 736f 7572 6365 206d 6179 2063 6175  a source may cau
-00015010: 7365 2070 6572 666f 726d 616e 6365 2070  se performance p
-00015020: 656e 616c 7479 2061 6e64 2063 7261 7368  enalty and crash
-00015030: 2e27 290d 0a0d 0a20 2020 2069 6620 6461  .')....    if da
-00015040: 7461 7372 632e 7065 7269 6f64 5f6e 7320  tasrc.period_ns 
-00015050: 3c20 303a 0d0a 2020 2020 2020 2020 7072  < 0:..        pr
-00015060: 696e 7428 2757 4152 4e49 4e47 3a20 696e  int('WARNING: in
-00015070: 7075 7420 6461 7461 2073 6f75 7263 6520  put data source 
-00015080: 6861 7320 7469 6d65 2069 6e20 6465 7363  has time in desc
-00015090: 656e 6469 6e67 206f 7264 6572 2e20 5472  ending order. Tr
-000150a0: 7920 736f 7274 5f76 616c 7565 7328 2920  y sort_values() 
-000150b0: 6265 666f 7265 2063 616c 6c69 6e67 2e27  before calling.'
-000150c0: 290d 0a0d 0a20 2020 2023 2046 4958 3a20  )....    # FIX: 
-000150d0: 7374 7570 6964 2051 5420 6275 6720 6361  stupid QT bug ca
-000150e0: 7573 6573 2072 6563 7461 6e67 6c65 7320  uses rectangles 
-000150f0: 6c61 7267 6572 2074 6861 6e20 3247 2074  larger than 2G t
-00015100: 6f20 666c 6963 6b65 722c 2073 6f20 7363  o flicker, so sc
-00015110: 616c 6520 7265 6e64 6572 696e 6720 646f  ale rendering do
-00015120: 776e 2073 6f6d 650d 0a20 2020 2023 2046  wn some..    # F
-00015130: 4958 3a20 5079 5174 2035 2e31 352e 3220  IX: PyQt 5.15.2 
-00015140: 6c69 6e65 7320 3e31 6536 2061 7265 2062  lines >1e6 are b
-00015150: 6569 6e67 2063 6c69 7070 6564 2074 6f20  eing clipped to 
-00015160: 3165 3620 6475 7269 6e67 2074 6865 2066  1e6 during the f
-00015170: 6972 7374 2072 656e 6465 7220 7061 7373  irst render pass
-00015180: 2c20 736f 2073 6361 6c65 2064 6f77 6e20  , so scale down 
-00015190: 6966 203e 3165 360d 0a20 2020 2069 6620  if >1e6..    if 
-000151a0: 6461 7461 7372 632e 6466 2e69 6c6f 635b  datasrc.df.iloc[
-000151b0: 3a2c 2031 3a5d 2e6d 6178 286e 756d 6572  :, 1:].max(numer
-000151c0: 6963 5f6f 6e6c 793d 5472 7565 292e 6d61  ic_only=True).ma
-000151d0: 7828 2920 3e20 3165 363a 0d0a 2020 2020  x() > 1e6:..    
-000151e0: 2020 2020 6178 2e76 622e 7973 6361 6c65      ax.vb.yscale
-000151f0: 2e73 6574 5f73 6361 6c65 2869 6e74 2831  .set_scale(int(1
-00015200: 6536 2929 0d0a 2020 2020 7265 7475 726e  e6))..    return
-00015210: 2064 6174 6173 7263 0d0a 0d0a 0d0a 6465   datasrc......de
-00015220: 6620 5f73 6574 5f64 6174 6173 7263 2861  f _set_datasrc(a
-00015230: 782c 2064 6174 6173 7263 2c20 6164 6463  x, datasrc, addc
-00015240: 6f6c 733d 5472 7565 293a 0d0a 2020 2020  ols=True):..    
-00015250: 7669 6577 626f 7820 3d20 6178 2e76 620d  viewbox = ax.vb.
-00015260: 0a20 2020 2069 6620 6e6f 7420 6461 7461  .    if not data
-00015270: 7372 632e 7374 616e 6461 6c6f 6e65 3a0d  src.standalone:.
-00015280: 0a20 2020 2020 2020 2069 6620 7669 6577  .        if view
-00015290: 626f 782e 6461 7461 7372 6320 6973 204e  box.datasrc is N
-000152a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000152b0: 2020 7669 6577 626f 782e 7365 745f 6461    viewbox.set_da
-000152c0: 7461 7372 6328 6461 7461 7372 6329 2023  tasrc(datasrc) #
-000152d0: 2066 6f72 206d 7768 6565 6c20 7a6f 6f6d   for mwheel zoom
-000152e0: 2d73 6361 6c69 6e67 0d0a 2020 2020 2020  -scaling..      
-000152f0: 2020 2020 2020 5f73 6574 5f78 5f6c 696d        _set_x_lim
-00015300: 6974 7328 6178 2c20 6461 7461 7372 6329  its(ax, datasrc)
-00015310: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00015320: 0a20 2020 2020 2020 2020 2020 2074 3020  .            t0 
-00015330: 3d20 7669 6577 626f 782e 6461 7461 7372  = viewbox.datasr
-00015340: 632e 782e 6c6f 635b 305d 0d0a 2020 2020  c.x.loc[0]..    
-00015350: 2020 2020 2020 2020 6966 2061 6464 636f          if addco
-00015360: 6c73 3a0d 0a20 2020 2020 2020 2020 2020  ls:..           
-00015370: 2020 2020 2076 6965 7762 6f78 2e64 6174       viewbox.dat
-00015380: 6173 7263 2e61 6464 636f 6c73 2864 6174  asrc.addcols(dat
-00015390: 6173 7263 290d 0a20 2020 2020 2020 2020  asrc)..         
-000153a0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000153b0: 2020 2020 2020 2020 2020 7669 6577 626f            viewbo
-000153c0: 782e 6461 7461 7372 632e 6466 203d 2064  x.datasrc.df = d
-000153d0: 6174 6173 7263 2e64 660d 0a20 2020 2020  atasrc.df..     
-000153e0: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-000153f0: 6620 7765 206e 6565 6420 746f 2072 652d  f we need to re-
-00015400: 7265 6e64 6572 2070 7265 7669 6f75 7320  render previous 
-00015410: 706c 6f74 7320 6475 6520 746f 2063 6861  plots due to cha
-00015420: 6e67 6564 2069 6e64 6963 6573 0d0a 2020  nged indices..  
-00015430: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-00015440: 735f 7570 6461 7465 6420 3d20 7669 6577  s_updated = view
-00015450: 626f 782e 6461 7461 7372 632e 7469 6d65  box.datasrc.time
-00015460: 6261 7365 6428 2920 616e 6420 7430 2021  based() and t0 !
-00015470: 3d20 7669 6577 626f 782e 6461 7461 7372  = viewbox.datasr
-00015480: 632e 782e 6c6f 635b 305d 0d0a 2020 2020  c.x.loc[0]..    
-00015490: 2020 2020 2020 2020 666f 7220 6974 656d          for item
-000154a0: 2069 6e20 6178 2e69 7465 6d73 3a0d 0a20   in ax.items:.. 
-000154b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000154c0: 6620 6861 7361 7474 7228 6974 656d 2c20  f hasattr(item, 
-000154d0: 2764 6174 6173 7263 2729 2061 6e64 206e  'datasrc') and n
-000154e0: 6f74 2069 7465 6d2e 6461 7461 7372 632e  ot item.datasrc.
-000154f0: 7374 616e 6461 6c6f 6e65 3a0d 0a20 2020  standalone:..   
-00015500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015510: 2069 7465 6d2e 6461 7461 7372 632e 7365   item.datasrc.se
-00015520: 745f 6466 2876 6965 7762 6f78 2e64 6174  t_df(viewbox.dat
-00015530: 6173 7263 2e64 6629 2023 2065 7665 7279  asrc.df) # every
-00015540: 2070 6c6f 7420 6865 7265 206e 6f77 2068   plot here now h
-00015550: 6173 2074 6865 2073 616d 6520 7469 6d65  as the same time
-00015560: 2d66 7261 6d65 0d0a 2020 2020 2020 2020  -frame..        
-00015570: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00015580: 6e64 6963 6573 5f75 7064 6174 6564 3a0d  ndices_updated:.
-00015590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000155a0: 2020 2020 2020 2020 205f 7374 6172 745f           _start_
-000155b0: 7669 7375 616c 5f75 7064 6174 6528 6974  visual_update(it
-000155c0: 656d 290d 0a20 2020 2020 2020 2020 2020  em)..           
-000155d0: 2020 2020 2020 2020 2020 2020 205f 656e               _en
-000155e0: 645f 7669 7375 616c 5f75 7064 6174 6528  d_visual_update(
-000155f0: 6974 656d 290d 0a20 2020 2020 2020 2020  item)..         
-00015600: 2020 205f 7365 745f 785f 6c69 6d69 7473     _set_x_limits
-00015610: 2861 782c 2064 6174 6173 7263 290d 0a20  (ax, datasrc).. 
-00015620: 2020 2020 2020 2020 2020 2076 6965 7762             viewb
-00015630: 6f78 2e73 6574 5f64 6174 6173 7263 2876  ox.set_datasrc(v
-00015640: 6965 7762 6f78 2e64 6174 6173 7263 2920  iewbox.datasrc) 
-00015650: 2320 7570 6461 7465 207a 6f6f 6d0d 0a20  # update zoom.. 
-00015660: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00015670: 2020 7669 6577 626f 782e 7374 616e 6461    viewbox.standa
-00015680: 6c6f 6e65 732e 6164 6428 6461 7461 7372  lones.add(datasr
-00015690: 6329 0d0a 2020 2020 2020 2020 6461 7461  c)..        data
-000156a0: 7372 632e 7570 6461 7465 5f69 6e69 745f  src.update_init_
-000156b0: 7828 7669 6577 626f 782e 696e 6974 5f73  x(viewbox.init_s
-000156c0: 7465 7073 290d 0a20 2020 2020 2020 2069  teps)..        i
-000156d0: 6620 6461 7461 7372 632e 7469 6d65 6261  f datasrc.timeba
-000156e0: 7365 6428 2920 616e 6420 7669 6577 626f  sed() and viewbo
-000156f0: 782e 6461 7461 7372 6320 6973 206e 6f74  x.datasrc is not
-00015700: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00015710: 2020 2020 2323 2070 7269 6e74 2827 5741      ## print('WA
-00015720: 524e 494e 473a 2072 652d 696e 6465 7869  RNING: re-indexi
-00015730: 6e67 2073 7461 6e64 616c 6f6e 652c 2074  ng standalone, t
-00015740: 696d 652d 6261 7365 6420 706c 6f74 2729  ime-based plot')
-00015750: 0d0a 2020 2020 2020 2020 2020 2020 7664  ..            vd
-00015760: 6620 3d20 7669 6577 626f 782e 6461 7461  f = viewbox.data
-00015770: 7372 632e 6466 0d0a 2020 2020 2020 2020  src.df..        
-00015780: 2020 2020 6420 3d20 7b76 3a6b 2066 6f72      d = {v:k for
-00015790: 206b 2c76 2069 6e20 656e 756d 6572 6174   k,v in enumerat
-000157a0: 6528 7664 665b 7664 662e 636f 6c75 6d6e  e(vdf[vdf.column
-000157b0: 735b 305d 5d29 7d0d 0a20 2020 2020 2020  s[0]])}..       
-000157c0: 2020 2020 2064 6174 6173 7263 2e64 662e       datasrc.df.
-000157d0: 696e 6465 7820 3d20 5b64 5b69 5d20 666f  index = [d[i] fo
-000157e0: 7220 6920 696e 2064 6174 6173 7263 2e64  r i in datasrc.d
-000157f0: 665b 6461 7461 7372 632e 6466 2e63 6f6c  f[datasrc.df.col
-00015800: 756d 6e73 5b30 5d5d 5d0d 0a20 2020 2020  umns[0]]]..     
-00015810: 2020 2023 2320 6966 206e 6f74 2076 6965     ## if not vie
-00015820: 7762 6f78 2e78 5f69 6e64 6578 6564 3a0d  wbox.x_indexed:.
-00015830: 0a20 2020 2020 2020 2020 2020 2023 2320  .            ## 
-00015840: 5f73 6574 5f78 5f6c 696d 6974 7328 6178  _set_x_limits(ax
-00015850: 2c20 6461 7461 7372 6329 0d0a 2020 2020  , datasrc)..    
-00015860: 2320 7570 6461 7465 2070 6572 696f 6420  # update period 
-00015870: 6966 2074 6869 7320 6461 7461 7372 6320  if this datasrc 
-00015880: 6861 7320 6869 6768 6572 2074 696d 6520  has higher time 
-00015890: 7265 736f 6c75 7469 6f6e 0d0a 2020 2020  resolution..    
-000158a0: 676c 6f62 616c 2065 706f 6368 5f70 6572  global epoch_per
-000158b0: 696f 640d 0a20 2020 2069 6620 6461 7461  iod..    if data
-000158c0: 7372 632e 7469 6d65 6261 7365 6428 2920  src.timebased() 
-000158d0: 616e 6420 2865 706f 6368 5f70 6572 696f  and (epoch_perio
-000158e0: 6420 3e20 3165 3720 6f72 206e 6f74 2064  d > 1e7 or not d
-000158f0: 6174 6173 7263 2e73 7461 6e64 616c 6f6e  atasrc.standalon
-00015900: 6529 3a0d 0a20 2020 2020 2020 2065 705f  e):..        ep_
-00015910: 7365 6373 203d 2064 6174 6173 7263 2e70  secs = datasrc.p
-00015920: 6572 696f 645f 6e73 202f 2031 6539 0d0a  eriod_ns / 1e9..
-00015930: 2020 2020 2020 2020 6570 6f63 685f 7065          epoch_pe
-00015940: 7269 6f64 203d 2065 705f 7365 6373 2069  riod = ep_secs i
-00015950: 6620 6570 5f73 6563 7320 3c20 6570 6f63  f ep_secs < epoc
-00015960: 685f 7065 7269 6f64 2065 6c73 6520 6570  h_period else ep
-00015970: 6f63 685f 7065 7269 6f64 0d0a 0d0a 0d0a  och_period......
-00015980: 6465 6620 5f68 6173 5f74 696d 6563 6f6c  def _has_timecol
-00015990: 2864 6629 3a0d 0a20 2020 2072 6574 7572  (df):..    retur
-000159a0: 6e20 6c65 6e28 6466 2e63 6f6c 756d 6e73  n len(df.columns
-000159b0: 2920 3e3d 2032 0d0a 0d0a 0d0a 6465 6620  ) >= 2......def 
-000159c0: 5f73 6574 5f6d 6178 5f7a 6f6f 6d28 7662  _set_max_zoom(vb
-000159d0: 7329 3a0d 0a20 2020 2027 2727 5365 7420  s):..    '''Set 
-000159e0: 7468 6520 7265 6c61 7469 7665 2061 6c6c  the relative all
-000159f0: 6f77 6564 207a 6f6f 6d20 6c65 7665 6c20  owed zoom level 
-00015a00: 6265 7477 6565 6e20 6178 6573 2067 726f  between axes gro
-00015a10: 7570 732c 2077 6865 7265 2074 6865 206c  ups, where the l
-00015a20: 6f77 6573 742d 7265 736f 6c75 7469 6f6e  owest-resolution
-00015a30: 0d0a 2020 2020 2020 2070 6c6f 7420 696e  ..       plot in
-00015a40: 2065 6163 6820 6772 6f75 7020 7573 6573   each group uses
-00015a50: 206d 6178 5f7a 6f6f 6d5f 706f 696e 7473   max_zoom_points
-00015a60: 2c20 7768 696c 6520 7468 6520 6f74 6865  , while the othe
-00015a70: 7273 2067 6574 2061 2073 6361 6c65 203e  rs get a scale >
-00015a80: 3d31 206f 6620 7468 6569 720d 0a20 2020  =1 of their..   
-00015a90: 2020 2020 7265 7370 6563 7469 7665 2068      respective h
-00015aa0: 6967 6865 7374 207a 6f6f 6d20 6c65 7665  ighest zoom leve
-00015ab0: 6c2e 2727 270d 0a20 2020 2067 726f 7570  l.'''..    group
-00015ac0: 7320 3d20 6465 6661 756c 7464 6963 7428  s = defaultdict(
-00015ad0: 7365 7429 0d0a 2020 2020 666f 7220 7662  set)..    for vb
-00015ae0: 2069 6e20 7662 733a 0d0a 2020 2020 2020   in vbs:..      
-00015af0: 2020 6d61 7374 6572 5f76 6220 3d20 7662    master_vb = vb
-00015b00: 2e6c 696e 6b65 6456 6965 7728 3029 0d0a  .linkedView(0)..
-00015b10: 2020 2020 2020 2020 6966 2076 622e 6461          if vb.da
-00015b20: 7461 7372 6320 616e 6420 6d61 7374 6572  tasrc and master
-00015b30: 5f76 6220 616e 6420 6d61 7374 6572 5f76  _vb and master_v
-00015b40: 622e 6461 7461 7372 633a 0d0a 2020 2020  b.datasrc:..    
-00015b50: 2020 2020 2020 2020 6772 6f75 7073 5b6d          groups[m
-00015b60: 6173 7465 725f 7662 5d2e 6164 6428 7662  aster_vb].add(vb
-00015b70: 290d 0a20 2020 2020 2020 2020 2020 2067  )..            g
-00015b80: 726f 7570 735b 6d61 7374 6572 5f76 625d  roups[master_vb]
-00015b90: 2e61 6464 286d 6173 7465 725f 7662 290d  .add(master_vb).
-00015ba0: 0a20 2020 2066 6f72 2067 726f 7570 2069  .    for group i
-00015bb0: 6e20 6772 6f75 7073 2e76 616c 7565 7328  n groups.values(
-00015bc0: 293a 0d0a 2020 2020 2020 2020 6d69 6e6c  ):..        minl
-00015bd0: 656e 203d 206d 696e 286c 656e 2876 622e  en = min(len(vb.
-00015be0: 6461 7461 7372 632e 6466 2920 666f 7220  datasrc.df) for 
-00015bf0: 7662 2069 6e20 6772 6f75 7029 0d0a 2020  vb in group)..  
-00015c00: 2020 2020 2020 666f 7220 7662 2069 6e20        for vb in 
-00015c10: 6772 6f75 703a 0d0a 2020 2020 2020 2020  group:..        
-00015c20: 2020 2020 7662 2e6d 6178 5f7a 6f6f 6d5f      vb.max_zoom_
-00015c30: 706f 696e 7473 5f66 203d 206c 656e 2876  points_f = len(v
-00015c40: 622e 6461 7461 7372 632e 6466 2920 2f20  b.datasrc.df) / 
-00015c50: 6d69 6e6c 656e 0d0a 0d0a 0d0a 6465 6620  minlen......def 
-00015c60: 5f61 646a 7573 745f 7265 6e6b 6f5f 6461  _adjust_renko_da
-00015c70: 7461 7372 6328 6269 6e73 2c20 7374 6570  tasrc(bins, step
-00015c80: 2c20 6461 7461 7372 6329 3a0d 0a20 2020  , datasrc):..   
-00015c90: 2069 6620 6e6f 7420 6269 6e73 2061 6e64   if not bins and
-00015ca0: 206e 6f74 2073 7465 703a 0d0a 2020 2020   not step:..    
-00015cb0: 2020 2020 6269 6e73 203d 2035 300d 0a20      bins = 50.. 
-00015cc0: 2020 2069 6620 6e6f 7420 7374 6570 3a0d     if not step:.
-00015cd0: 0a20 2020 2020 2020 2073 7465 7020 3d20  .        step = 
-00015ce0: 2864 6174 6173 7263 2e79 2e6d 6178 2829  (datasrc.y.max()
-00015cf0: 2d64 6174 6173 7263 2e79 2e6d 696e 2829  -datasrc.y.min()
-00015d00: 2920 2f20 6269 6e73 0d0a 2020 2020 6272  ) / bins..    br
-00015d10: 6963 6b73 203d 2064 6174 6173 7263 2e79  icks = datasrc.y
-00015d20: 2e64 6966 6628 2920 2f20 7374 6570 0d0a  .diff() / step..
-00015d30: 2020 2020 6272 6963 6b73 203d 2028 6461      bricks = (da
-00015d40: 7461 7372 632e 795b 6272 6963 6b73 2e69  tasrc.y[bricks.i
-00015d50: 736e 756c 6c28 2920 7c20 2862 7269 636b  snull() | (brick
-00015d60: 732e 6162 7328 293e 3d30 2e35 295d 202f  s.abs()>=0.5)] /
-00015d70: 2073 7465 7029 2e72 6f75 6e64 2829 2e61   step).round().a
-00015d80: 7374 7970 6528 696e 7429 0d0a 2020 2020  stype(int)..    
-00015d90: 6578 7472 6173 203d 2064 6174 6173 7263  extras = datasrc
-00015da0: 2e64 662e 696c 6f63 5b3a 2c20 6461 7461  .df.iloc[:, data
-00015db0: 7372 632e 636f 6c5f 6461 7461 5f6f 6666  src.col_data_off
-00015dc0: 7365 742b 313a 5d0d 0a20 2020 2074 7320  set+1:]..    ts 
-00015dd0: 3d20 6461 7461 7372 632e 785b 6272 6963  = datasrc.x[bric
-00015de0: 6b73 2e69 6e64 6578 5d0d 0a20 2020 2075  ks.index]..    u
-00015df0: 7020 3d20 6272 6963 6b73 2e69 6c6f 635b  p = bricks.iloc[
-00015e00: 305d 202b 2031 0d0a 2020 2020 646e 203d  0] + 1..    dn =
-00015e10: 2075 7020 2d20 320d 0a20 2020 2064 6174   up - 2..    dat
-00015e20: 6120 3d20 5b5d 0d0a 2020 2020 666f 7220  a = []..    for 
-00015e30: 742c 692c 6272 6963 6b20 696e 207a 6970  t,i,brick in zip
-00015e40: 2874 732c 2062 7269 636b 732e 696e 6465  (ts, bricks.inde
-00015e50: 782c 2062 7269 636b 7329 3a0d 0a20 2020  x, bricks):..   
-00015e60: 2020 2020 2073 203d 2030 0d0a 2020 2020       s = 0..    
-00015e70: 2020 2020 6966 2062 7269 636b 203e 3d20      if brick >= 
-00015e80: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
-00015e90: 2078 302c 7831 2c73 203d 2075 702d 312c   x0,x1,s = up-1,
-00015ea0: 6272 6963 6b2c 2b31 0d0a 2020 2020 2020  brick,+1..      
-00015eb0: 2020 2020 2020 7570 203d 2062 7269 636b        up = brick
-00015ec0: 2b31 0d0a 2020 2020 2020 2020 2020 2020  +1..            
-00015ed0: 646e 203d 2062 7269 636b 2d32 0d0a 2020  dn = brick-2..  
-00015ee0: 2020 2020 2020 656c 6966 2062 7269 636b        elif brick
-00015ef0: 203c 3d20 646e 3a0d 0a20 2020 2020 2020   <= dn:..       
-00015f00: 2020 2020 2078 302c 7831 2c73 203d 2064       x0,x1,s = d
-00015f10: 6e2c 6272 6963 6b2d 312c 2d31 0d0a 2020  n,brick-1,-1..  
-00015f20: 2020 2020 2020 2020 2020 7570 203d 2062            up = b
-00015f30: 7269 636b 2b32 0d0a 2020 2020 2020 2020  rick+2..        
-00015f40: 2020 2020 646e 203d 2062 7269 636b 2d31      dn = brick-1
-00015f50: 0d0a 2020 2020 2020 2020 6966 2073 3a0d  ..        if s:.
-00015f60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00015f70: 2078 2069 6e20 7261 6e67 6528 7830 2c20   x in range(x0, 
-00015f80: 7831 2c20 7329 3a0d 0a20 2020 2020 2020  x1, s):..       
-00015f90: 2020 2020 2020 2020 2074 6420 3d20 6162           td = ab
-00015fa0: 7328 7831 2d78 292d 310d 0a20 2020 2020  s(x1-x)-1..     
-00015fb0: 2020 2020 2020 2020 2020 2064 7320 3d20             ds = 
-00015fc0: 3020 6966 2073 3e30 2065 6c73 6520 7374  0 if s>0 else st
-00015fd0: 6570 0d0a 2020 2020 2020 2020 2020 2020  ep..            
-00015fe0: 2020 2020 7920 3d20 782a 7374 6570 0d0a      y = x*step..
-00015ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016000: 7a20 3d20 6c69 7374 2865 7874 7261 732e  z = list(extras.
-00016010: 6c6f 635b 695d 290d 0a20 2020 2020 2020  loc[i])..       
-00016020: 2020 2020 2020 2020 2064 6174 612e 6170           data.ap
-00016030: 7065 6e64 285b 742d 7464 2c20 792b 6473  pend([t-td, y+ds
-00016040: 2c20 792b 7374 6570 2d64 732c 2079 2b73  , y+step-ds, y+s
-00016050: 7465 702c 2079 5d20 2b20 7a29 0d0a 2020  tep, y] + z)..  
-00016060: 2020 6461 7461 7372 632e 7365 745f 6466    datasrc.set_df
-00016070: 2870 642e 4461 7461 4672 616d 6528 6461  (pd.DataFrame(da
-00016080: 7461 2c20 636f 6c75 6d6e 733d 2774 696d  ta, columns='tim
-00016090: 6520 6f70 656e 2063 6c6f 7365 2068 6967  e open close hig
-000160a0: 6820 6c6f 7727 2e73 706c 6974 2829 2b6c  h low'.split()+l
-000160b0: 6973 7428 6578 7472 6173 2e63 6f6c 756d  ist(extras.colum
-000160c0: 6e73 2929 290d 0a0d 0a0d 0a64 6566 205f  ns)))......def _
-000160d0: 6164 6a75 7374 5f72 656e 6b6f 5f6c 6f67  adjust_renko_log
-000160e0: 5f64 6174 6173 7263 2862 696e 732c 2073  _datasrc(bins, s
-000160f0: 7465 702c 2064 6174 6173 7263 293a 0d0a  tep, datasrc):..
-00016100: 2020 2020 6461 7461 7372 632e 6466 2e6c      datasrc.df.l
-00016110: 6f63 5b3a 2c64 6174 6173 7263 2e64 662e  oc[:,datasrc.df.
-00016120: 636f 6c75 6d73 5b31 5d5d 203d 206e 702e  colums[1]] = np.
-00016130: 6c6f 6731 3028 6461 7461 7372 632e 6466  log10(datasrc.df
-00016140: 2e69 6c6f 635b 3a2c 315d 290d 0a20 2020  .iloc[:,1])..   
-00016150: 205f 6164 6a75 7374 5f72 656e 6b6f 5f64   _adjust_renko_d
-00016160: 6174 6173 7263 2862 696e 732c 2073 7465  atasrc(bins, ste
-00016170: 702c 2064 6174 6173 7263 290d 0a20 2020  p, datasrc)..   
-00016180: 2064 6174 6173 7263 2e64 662e 6c6f 635b   datasrc.df.loc[
-00016190: 3a2c 6461 7461 7372 632e 6466 2e63 6f6c  :,datasrc.df.col
-000161a0: 756d 735b 313a 355d 5d20 3d20 3130 2a2a  ums[1:5]] = 10**
-000161b0: 6461 7461 7372 632e 6466 2e69 6c6f 635b  datasrc.df.iloc[
-000161c0: 3a2c 313a 355d 0d0a 0d0a 0d0a 6465 6620  :,1:5]......def 
-000161d0: 5f61 646a 7573 745f 766f 6c75 6d65 5f64  _adjust_volume_d
-000161e0: 6174 6173 7263 2864 6174 6173 7263 293a  atasrc(datasrc):
-000161f0: 0d0a 2020 2020 6966 206c 656e 2864 6174  ..    if len(dat
-00016200: 6173 7263 2e64 662e 636f 6c75 6d6e 7329  asrc.df.columns)
-00016210: 203c 3d20 343a 0d0a 2020 2020 2020 2020   <= 4:..        
-00016220: 6461 7461 7372 632e 6466 2e69 6e73 6572  datasrc.df.inser
-00016230: 7428 332c 2027 5f7a 6572 6f5f 272c 205b  t(3, '_zero_', [
-00016240: 305d 2a6c 656e 2864 6174 6173 7263 2e64  0]*len(datasrc.d
-00016250: 6629 2920 2320 6261 7365 206f 6620 6361  f)) # base of ca
-00016260: 6e64 6c65 7320 6973 2061 6c77 6179 7320  ndles is always 
-00016270: 7a65 726f 0d0a 2020 2020 6461 7461 7372  zero..    datasr
-00016280: 632e 7365 745f 6466 2864 6174 6173 7263  c.set_df(datasrc
-00016290: 2e64 662e 696c 6f63 5b3a 2c5b 302c 332c  .df.iloc[:,[0,3,
-000162a0: 342c 312c 325d 5d29 2023 2072 652d 6172  4,1,2]]) # re-ar
-000162b0: 7261 6e67 6520 636f 6c75 6d6e 7320 666f  range columns fo
-000162c0: 7220 7265 6e64 6572 696e 670d 0a20 2020  r rendering..   
-000162d0: 2064 6174 6173 7263 2e73 6361 6c65 5f63   datasrc.scale_c
-000162e0: 6f6c 7320 3d20 5b31 2c20 325d 2023 2073  ols = [1, 2] # s
-000162f0: 6361 6c65 2062 7920 626f 7468 2062 6173  cale by both bas
-00016300: 656c 696e 6520 616e 6420 766f 6c75 6d65  eline and volume
-00016310: 0d0a 0d0a 0d0a 6465 6620 5f70 7265 6164  ......def _pread
-00016320: 6a75 7374 5f68 6f72 697a 5f64 6174 6173  just_horiz_datas
-00016330: 7263 2864 6174 6173 7263 293a 0d0a 2020  rc(datasrc):..  
-00016340: 2020 6172 7261 7969 6679 203d 206c 616d    arrayify = lam
-00016350: 6264 6120 643a 2064 2e76 616c 7565 7320  bda d: d.values 
-00016360: 6966 2074 7970 6528 6429 203d 3d20 7064  if type(d) == pd
-00016370: 2e44 6174 6146 7261 6d65 2065 6c73 6520  .DataFrame else 
-00016380: 640d 0a20 2020 2023 2063 7265 6174 6520  d..    # create 
-00016390: 6120 6461 7461 6672 616d 6520 6672 6f6d  a dataframe from
-000163a0: 2074 6865 2069 6e70 7574 2061 7272 6179   the input array
-000163b0: 0d0a 2020 2020 7469 6d65 7320 3d20 5b74  ..    times = [t
-000163c0: 2066 6f72 2074 2c72 6f77 2069 6e20 6461   for t,row in da
-000163d0: 7461 7372 635d 0d0a 2020 2020 6966 206c  tasrc]..    if l
-000163e0: 656e 2874 696d 6573 2920 3d3d 2031 3a20  en(times) == 1: 
-000163f0: 2320 6164 6420 616e 2065 6d70 7479 2074  # add an empty t
-00016400: 696d 6520 736c 6f74 0d0a 2020 2020 2020  ime slot..      
-00016410: 2020 7469 6d65 7320 3d20 5b74 696d 6573    times = [times
-00016420: 5b30 5d2c 2074 696d 6573 5b30 5d2b 315d  [0], times[0]+1]
-00016430: 0d0a 2020 2020 2020 2020 6461 7461 7372  ..        datasr
-00016440: 6320 3d20 6461 7461 7372 6320 2b20 5b5b  c = datasrc + [[
-00016450: 7469 6d65 735b 315d 2c20 5b28 702c 3029  times[1], [(p,0)
-00016460: 2066 6f72 2070 2c76 2069 6e20 6172 7261   for p,v in arra
-00016470: 7969 6679 2864 6174 6173 7263 5b30 5d5b  yify(datasrc[0][
-00016480: 315d 295d 5d5d 0d0a 2020 2020 6461 7461  1])]]]..    data
-00016490: 203d 205b 5b65 2066 6f72 2076 2069 6e20   = [[e for v in 
-000164a0: 6172 7261 7969 6679 2872 6f77 2920 666f  arrayify(row) fo
-000164b0: 7220 6520 696e 2076 5d20 666f 7220 742c  r e in v] for t,
-000164c0: 726f 7720 696e 2064 6174 6173 7263 5d0d  row in datasrc].
-000164d0: 0a20 2020 206d 6178 636f 6c73 203d 206d  .    maxcols = m
-000164e0: 6178 286c 656e 2872 6f77 2920 666f 7220  ax(len(row) for 
-000164f0: 726f 7720 696e 2064 6174 6129 0d0a 2020  row in data)..  
-00016500: 2020 7265 7475 726e 2070 642e 4461 7461    return pd.Data
-00016510: 4672 616d 6528 636f 6c75 6d6e 733d 7261  Frame(columns=ra
-00016520: 6e67 6528 6d61 7863 6f6c 7329 2c20 6461  nge(maxcols), da
-00016530: 7461 3d64 6174 612c 2069 6e64 6578 3d74  ta=data, index=t
-00016540: 696d 6573 290d 0a0d 0a0d 0a64 6566 205f  imes)......def _
-00016550: 6164 6a75 7374 5f68 6f72 697a 5f64 6174  adjust_horiz_dat
-00016560: 6173 7263 2864 6174 6173 7263 293a 0d0a  asrc(datasrc):..
-00016570: 2020 2020 2320 746f 2062 6520 6162 6c65      # to be able
-00016580: 2074 6f20 7363 616c 6520 7072 6f70 6572   to scale proper
-00016590: 6c79 2c20 6d6f 7665 2074 6865 206c 6173  ly, move the las
-000165a0: 7420 7477 6f20 7661 6c75 6573 2074 6f20  t two values to 
-000165b0: 7468 6520 6c61 7374 2074 776f 2063 6f6c  the last two col
-000165c0: 756d 6e73 0d0a 2020 2020 7661 6c75 6573  umns..    values
-000165d0: 203d 2064 6174 6173 7263 2e64 662e 696c   = datasrc.df.il
-000165e0: 6f63 5b3a 2c20 313a 5d2e 7661 6c75 6573  oc[:, 1:].values
-000165f0: 0d0a 2020 2020 666f 7220 692c 6e72 6f77  ..    for i,nrow
-00016600: 2069 6e20 656e 756d 6572 6174 6528 7661   in enumerate(va
-00016610: 6c75 6573 293a 0d0a 2020 2020 2020 2020  lues):..        
-00016620: 6f72 6f77 203d 206e 726f 775b 7e6e 702e  orow = nrow[~np.
-00016630: 6973 6e61 6e28 6e72 6f77 295d 0d0a 2020  isnan(nrow)]..  
-00016640: 2020 2020 2020 6966 206c 656e 286e 726f        if len(nro
-00016650: 7729 203d 3d20 6c65 6e28 6f72 6f77 2920  w) == len(orow) 
-00016660: 6f72 206c 656e 286f 726f 7729 203c 3d20  or len(orow) <= 
-00016670: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-00016680: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-00016690: 2020 6e72 6f77 5b2d 323a 5d20 3d20 6f72    nrow[-2:] = or
-000166a0: 6f77 5b2d 323a 5d0d 0a20 2020 2020 2020  ow[-2:]..       
-000166b0: 206e 726f 775b 6c65 6e28 6f72 6f77 292d   nrow[len(orow)-
-000166c0: 323a 6c65 6e28 6f72 6f77 295d 203d 206e  2:len(orow)] = n
-000166d0: 702e 6e61 6e0d 0a20 2020 2064 6174 6173  p.nan..    datas
-000166e0: 7263 2e64 665b 6461 7461 7372 632e 6466  rc.df[datasrc.df
-000166f0: 2e63 6f6c 756d 6e73 5b31 3a5d 5d20 3d20  .columns[1:]] = 
-00016700: 7661 6c75 6573 0d0a 0d0a 0d0a 6465 6620  values......def 
-00016710: 5f61 646a 7573 745f 6261 725f 6461 7461  _adjust_bar_data
-00016720: 7372 6328 6461 7461 7372 632c 206f 7264  src(datasrc, ord
-00016730: 6572 5f63 6f6c 733d 5472 7565 293a 0d0a  er_cols=True):..
-00016740: 2020 2020 6966 206c 656e 2864 6174 6173      if len(datas
-00016750: 7263 2e64 662e 636f 6c75 6d6e 7329 203c  rc.df.columns) <
-00016760: 3d20 323a 0d0a 2020 2020 2020 2020 6461  = 2:..        da
-00016770: 7461 7372 632e 6466 2e69 6e73 6572 7428  tasrc.df.insert(
-00016780: 312c 2027 5f62 6173 655f 272c 205b 305d  1, '_base_', [0]
-00016790: 2a6c 656e 2864 6174 6173 7263 2e64 6629  *len(datasrc.df)
-000167a0: 2920 2320 6261 7365 0d0a 2020 2020 6966  ) # base..    if
-000167b0: 206c 656e 2864 6174 6173 7263 2e64 662e   len(datasrc.df.
-000167c0: 636f 6c75 6d6e 7329 203c 3d20 343a 0d0a  columns) <= 4:..
-000167d0: 2020 2020 2020 2020 6461 7461 7372 632e          datasrc.
-000167e0: 6466 2e69 6e73 6572 7428 312c 2027 5f6f  df.insert(1, '_o
-000167f0: 7065 6e5f 272c 2020 5b30 5d2a 6c65 6e28  pen_',  [0]*len(
-00016800: 6461 7461 7372 632e 6466 2929 2023 2022  datasrc.df)) # "
-00016810: 6f70 656e 2220 666f 7220 636f 6c6f 720d  open" for color.
-00016820: 0a20 2020 2020 2020 2064 6174 6173 7263  .        datasrc
-00016830: 2e64 662e 696e 7365 7274 2832 2c20 275f  .df.insert(2, '_
-00016840: 636c 6f73 655f 272c 2064 6174 6173 7263  close_', datasrc
-00016850: 2e64 662e 696c 6f63 5b3a 2c20 335d 2920  .df.iloc[:, 3]) 
-00016860: 2320 2263 6c6f 7365 2220 2861 6374 7561  # "close" (actua
-00016870: 6c20 6261 7220 7661 6c75 6529 2066 6f72  l bar value) for
-00016880: 2063 6f6c 6f72 0d0a 2020 2020 6966 206f   color..    if o
-00016890: 7264 6572 5f63 6f6c 733a 0d0a 2020 2020  rder_cols:..    
-000168a0: 2020 2020 6461 7461 7372 632e 7365 745f      datasrc.set_
-000168b0: 6466 2864 6174 6173 7263 2e64 662e 696c  df(datasrc.df.il
-000168c0: 6f63 5b3a 2c5b 302c 332c 342c 312c 325d  oc[:,[0,3,4,1,2]
-000168d0: 5d29 2023 2072 652d 6172 7261 6e67 6520  ]) # re-arrange 
-000168e0: 636f 6c75 6d6e 7320 666f 7220 7265 6e64  columns for rend
-000168f0: 6572 696e 670d 0a20 2020 2064 6174 6173  ering..    datas
-00016900: 7263 2e73 6361 6c65 5f63 6f6c 7320 3d20  rc.scale_cols = 
-00016910: 5b31 2c20 325d 2023 2073 6361 6c65 2062  [1, 2] # scale b
-00016920: 7920 626f 7468 2062 6173 656c 696e 6520  y both baseline 
-00016930: 616e 6420 766f 6c75 6d65 0d0a 0d0a 0d0a  and volume......
-00016940: 6465 6620 5f75 7064 6174 655f 6461 7461  def _update_data
-00016950: 2870 7265 6164 6a75 7374 6675 6e63 2c20  (preadjustfunc, 
-00016960: 6164 6a75 7374 6675 6e63 2c20 6974 656d  adjustfunc, item
-00016970: 2c20 6473 2c20 6766 783d 5472 7565 293a  , ds, gfx=True):
-00016980: 0d0a 2020 2020 6966 2070 7265 6164 6a75  ..    if preadju
-00016990: 7374 6675 6e63 3a0d 0a20 2020 2020 2020  stfunc:..       
-000169a0: 2064 7320 3d20 7072 6561 646a 7573 7466   ds = preadjustf
-000169b0: 756e 6328 6473 290d 0a20 2020 2064 7320  unc(ds)..    ds 
-000169c0: 3d20 5f63 7265 6174 655f 6461 7461 7372  = _create_datasr
-000169d0: 6328 6974 656d 2e61 782c 2064 7329 0d0a  c(item.ax, ds)..
-000169e0: 2020 2020 6966 2061 646a 7573 7466 756e      if adjustfun
-000169f0: 633a 0d0a 2020 2020 2020 2020 6164 6a75  c:..        adju
-00016a00: 7374 6675 6e63 2864 7329 0d0a 2020 2020  stfunc(ds)..    
-00016a10: 6373 203d 206c 6973 7428 6974 656d 2e64  cs = list(item.d
-00016a20: 6174 6173 7263 2e64 662e 636f 6c75 6d6e  atasrc.df.column
-00016a30: 735b 3a31 5d29 202b 206c 6973 7428 6974  s[:1]) + list(it
-00016a40: 656d 2e64 6174 6173 7263 2e64 662e 636f  em.datasrc.df.co
-00016a50: 6c75 6d6e 735b 6974 656d 2e64 6174 6173  lumns[item.datas
-00016a60: 7263 2e63 6f6c 5f64 6174 615f 6f66 6673  rc.col_data_offs
-00016a70: 6574 3a5d 290d 0a20 2020 2069 6620 6c65  et:])..    if le
-00016a80: 6e28 6373 2920 3e3d 206c 656e 2864 732e  n(cs) >= len(ds.
-00016a90: 6466 2e63 6f6c 756d 6e73 293a 0d0a 2020  df.columns):..  
-00016aa0: 2020 2020 2020 6473 2e64 662e 636f 6c75        ds.df.colu
-00016ab0: 6d6e 7320 3d20 6373 5b3a 6c65 6e28 6473  mns = cs[:len(ds
-00016ac0: 2e64 662e 636f 6c75 6d6e 7329 5d0d 0a20  .df.columns)].. 
-00016ad0: 2020 2069 7465 6d2e 6461 7461 7372 632e     item.datasrc.
-00016ae0: 7570 6461 7465 2864 7329 0d0a 2020 2020  update(ds)..    
-00016af0: 5f73 6574 5f64 6174 6173 7263 2869 7465  _set_datasrc(ite
-00016b00: 6d2e 6178 2c20 6974 656d 2e64 6174 6173  m.ax, item.datas
-00016b10: 7263 2c20 6164 6463 6f6c 733d 4661 6c73  rc, addcols=Fals
-00016b20: 6529 0d0a 2020 2020 6966 2067 6678 3a0d  e)..    if gfx:.
-00016b30: 0a20 2020 2020 2020 2069 7465 6d2e 7570  .        item.up
-00016b40: 6461 7465 5f67 6678 2829 0d0a 0d0a 0d0a  date_gfx()......
-00016b50: 6465 6620 5f75 7064 6174 655f 6766 7828  def _update_gfx(
-00016b60: 6974 656d 293a 0d0a 2020 2020 5f73 7461  item):..    _sta
-00016b70: 7274 5f76 6973 7561 6c5f 7570 6461 7465  rt_visual_update
-00016b80: 2869 7465 6d29 0d0a 2020 2020 666f 7220  (item)..    for 
-00016b90: 6920 696e 2069 7465 6d2e 6178 2e69 7465  i in item.ax.ite
-00016ba0: 6d73 3a0d 0a20 2020 2020 2020 2069 6620  ms:..        if 
-00016bb0: 6920 3d3d 2069 7465 6d20 6f72 206e 6f74  i == item or not
-00016bc0: 2068 6173 6174 7472 2869 2c20 2764 6174   hasattr(i, 'dat
-00016bd0: 6173 7263 2729 3a0d 0a20 2020 2020 2020  asrc'):..       
-00016be0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00016bf0: 2020 2020 2020 206c 6320 3d20 6c65 6e28         lc = len(
-00016c00: 6974 656d 2e64 6174 6173 7263 2e64 6629  item.datasrc.df)
-00016c10: 0d0a 2020 2020 2020 2020 6c69 203d 206c  ..        li = l
-00016c20: 656e 2869 2e64 6174 6173 7263 2e64 6629  en(i.datasrc.df)
-00016c30: 0d0a 2020 2020 2020 2020 6966 206c 6320  ..        if lc 
-00016c40: 616e 6420 6c69 2061 6e64 206d 6178 286c  and li and max(l
-00016c50: 632c 6c69 292f 6d69 6e28 6c63 2c6c 6929  c,li)/min(lc,li)
-00016c60: 203e 2031 3030 3a20 2320 544f 444f 3a20   > 100: # TODO: 
-00016c70: 7368 6f75 6c64 2062 6520 7479 7065 6420  should be typed 
-00016c80: 696e 7374 6561 640d 0a20 2020 2020 2020  instead..       
-00016c90: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00016ca0: 2020 2020 2020 2063 6320 3d20 6974 656d         cc = item
-00016cb0: 2e64 6174 6173 7263 2e64 662e 636f 6c75  .datasrc.df.colu
-00016cc0: 6d6e 730d 0a20 2020 2020 2020 2063 6920  mns..        ci 
-00016cd0: 3d20 692e 6461 7461 7372 632e 6466 2e63  = i.datasrc.df.c
-00016ce0: 6f6c 756d 6e73 0d0a 2020 2020 2020 2020  olumns..        
-00016cf0: 6330 203d 205b 6320 666f 7220 6320 696e  c0 = [c for c in
-00016d00: 2063 6920 6966 2063 2069 6e20 6363 5d0d   ci if c in cc].
-00016d10: 0a20 2020 2020 2020 2063 3120 3d20 5b63  .        c1 = [c
-00016d20: 2066 6f72 2063 2069 6e20 6369 2069 6620   for c in ci if 
-00016d30: 6e6f 7420 6320 696e 2063 635d 0d0a 2020  not c in cc]..  
-00016d40: 2020 2020 2020 6466 5f63 6c69 7070 6564        df_clipped
-00016d50: 203d 2069 7465 6d2e 6461 7461 7372 632e   = item.datasrc.
-00016d60: 6466 5b63 305d 0d0a 2020 2020 2020 2020  df[c0]..        
-00016d70: 6966 2063 313a 0d0a 2020 2020 2020 2020  if c1:..        
-00016d80: 2020 2020 6466 5f63 6c69 7070 6564 203d      df_clipped =
-00016d90: 2064 665f 636c 6970 7065 642e 636f 7079   df_clipped.copy
-00016da0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00016db0: 666f 7220 6320 696e 2063 313a 0d0a 2020  for c in c1:..  
-00016dc0: 2020 2020 2020 2020 2020 2020 2020 6466                df
-00016dd0: 5f63 6c69 7070 6564 5b63 5d20 3d20 692e  _clipped[c] = i.
-00016de0: 6461 7461 7372 632e 6466 5b63 5d0d 0a20  datasrc.df[c].. 
-00016df0: 2020 2020 2020 2069 2e64 6174 6173 7263         i.datasrc
-00016e00: 2e73 6574 5f64 6628 6466 5f63 6c69 7070  .set_df(df_clipp
-00016e10: 6564 290d 0a20 2020 2020 2020 2062 7265  ed)..        bre
-00016e20: 616b 0d0a 2020 2020 7570 6461 7465 5f73  ak..    update_s
-00016e30: 6967 6469 6720 3d20 4661 6c73 650d 0a20  igdig = False.. 
-00016e40: 2020 2069 6620 6e6f 7420 6974 656d 2e64     if not item.d
-00016e50: 6174 6173 7263 2e73 7461 6e64 616c 6f6e  atasrc.standalon
-00016e60: 6520 616e 6420 6e6f 7420 6974 656d 2e61  e and not item.a
-00016e70: 782e 7662 2e77 696e 2e5f 6973 4d6f 7573  x.vb.win._isMous
-00016e80: 654c 6566 7444 7261 673a 0d0a 2020 2020  eLeftDrag:..    
-00016e90: 2020 2020 2320 6e65 7720 6c69 6d69 7473      # new limits
-00016ea0: 2077 6865 6e20 6578 7465 6e64 696e 672f   when extending/
-00016eb0: 7265 6475 6369 6e67 2061 6d6f 756e 7420  reducing amount 
-00016ec0: 6f66 2064 6174 610d 0a20 2020 2020 2020  of data..       
-00016ed0: 2078 5f6d 696e 2c78 3120 3d20 5f73 6574   x_min,x1 = _set
-00016ee0: 5f78 5f6c 696d 6974 7328 6974 656d 2e61  _x_limits(item.a
-00016ef0: 782c 2069 7465 6d2e 6461 7461 7372 6329  x, item.datasrc)
-00016f00: 0d0a 2020 2020 2020 2020 2320 7363 726f  ..        # scro
-00016f10: 6c6c 2061 6c6c 2070 6c6f 7473 2069 6620  ll all plots if 
-00016f20: 7765 2772 6520 6174 2074 6865 2066 6172  we're at the far
-00016f30: 2072 6967 6874 0d0a 2020 2020 2020 2020   right..        
-00016f40: 7472 203d 2069 7465 6d2e 6178 2e76 622e  tr = item.ax.vb.
-00016f50: 7461 7267 6574 5265 6374 2829 0d0a 2020  targetRect()..  
-00016f60: 2020 2020 2020 7830 203d 2078 3120 2d20        x0 = x1 - 
-00016f70: 7472 2e77 6964 7468 2829 0d0a 2020 2020  tr.width()..    
-00016f80: 2020 2020 6966 2078 3020 3c20 7269 6768      if x0 < righ
-00016f90: 745f 6d61 7267 696e 5f63 616e 646c 6573  t_margin_candles
-00016fa0: 202b 2073 6964 655f 6d61 7267 696e 3a0d   + side_margin:.
-00016fb0: 0a20 2020 2020 2020 2020 2020 2078 3020  .            x0 
-00016fc0: 3d20 2d73 6964 655f 6d61 7267 696e 0d0a  = -side_margin..
-00016fd0: 2020 2020 2020 2020 6966 2074 722e 7269          if tr.ri
-00016fe0: 6768 7428 2920 3c20 7831 202d 2035 202d  ght() < x1 - 5 -
-00016ff0: 2032 2a72 6967 6874 5f6d 6172 6769 6e5f   2*right_margin_
-00017000: 6361 6e64 6c65 733a 0d0a 2020 2020 2020  candles:..      
-00017010: 2020 2020 2020 7830 203d 2078 3120 3d20        x0 = x1 = 
-00017020: 4e6f 6e65 0d0a 2020 2020 2020 2020 7072  None..        pr
-00017030: 6576 5f74 6f70 203d 2069 7465 6d2e 6178  ev_top = item.ax
-00017040: 2e76 622e 7461 7267 6574 5265 6374 2829  .vb.targetRect()
-00017050: 2e74 6f70 2829 0d0a 2020 2020 2020 2020  .top()..        
-00017060: 6974 656d 2e61 782e 7662 2e75 7064 6174  item.ax.vb.updat
-00017070: 655f 795f 7a6f 6f6d 2878 302c 2078 3129  e_y_zoom(x0, x1)
-00017080: 0d0a 2020 2020 2020 2020 7468 6973 5f74  ..        this_t
-00017090: 6f70 203d 2069 7465 6d2e 6178 2e76 622e  op = item.ax.vb.
-000170a0: 7461 7267 6574 5265 6374 2829 2e74 6f70  targetRect().top
-000170b0: 2829 0d0a 2020 2020 2020 2020 6966 2074  ()..        if t
-000170c0: 6869 735f 746f 7020 616e 6420 6e6f 7420  his_top and not 
-000170d0: 2830 2e39 3920 3c20 6162 7328 7072 6576  (0.99 < abs(prev
-000170e0: 5f74 6f70 2f74 6869 735f 746f 7029 203c  _top/this_top) <
-000170f0: 2031 2e30 3129 3a0d 0a20 2020 2020 2020   1.01):..       
-00017100: 2020 2020 2075 7064 6174 655f 7369 6764       update_sigd
-00017110: 6967 203d 2054 7275 650d 0a20 2020 2020  ig = True..     
-00017120: 2020 2069 6620 6974 656d 2e61 782e 6178     if item.ax.ax
-00017130: 6573 5b27 626f 7474 6f6d 275d 5b27 6974  es['bottom']['it
-00017140: 656d 275d 2e69 7356 6973 6962 6c65 2829  em'].isVisible()
-00017150: 3a20 2320 7570 6461 7465 2061 7865 7320  : # update axes 
-00017160: 6966 2076 6973 6962 6c65 0d0a 2020 2020  if visible..    
-00017170: 2020 2020 2020 2020 6974 656d 2e61 782e          item.ax.
-00017180: 6178 6573 5b27 626f 7474 6f6d 275d 5b27  axes['bottom']['
-00017190: 6974 656d 275d 2e68 6964 6528 290d 0a20  item'].hide().. 
-000171a0: 2020 2020 2020 2020 2020 2069 7465 6d2e             item.
-000171b0: 6178 2e61 7865 735b 2762 6f74 746f 6d27  ax.axes['bottom'
-000171c0: 5d5b 2769 7465 6d27 5d2e 7368 6f77 2829  ]['item'].show()
-000171d0: 0d0a 2020 2020 5f65 6e64 5f76 6973 7561  ..    _end_visua
-000171e0: 6c5f 7570 6461 7465 2869 7465 6d29 0d0a  l_update(item)..
-000171f0: 2020 2020 6966 2075 7064 6174 655f 7369      if update_si
-00017200: 6764 6967 3a0d 0a20 2020 2020 2020 205f  gdig:..        _
-00017210: 7570 6461 7465 5f73 6967 6e69 6669 6361  update_significa
-00017220: 6e74 7328 6974 656d 2e61 782c 2069 7465  nts(item.ax, ite
-00017230: 6d2e 6178 2e76 622e 6461 7461 7372 632c  m.ax.vb.datasrc,
-00017240: 2066 6f72 6365 3d54 7275 6529 0d0a 0d0a   force=True)....
-00017250: 0d0a 6465 6620 5f73 7461 7274 5f76 6973  ..def _start_vis
-00017260: 7561 6c5f 7570 6461 7465 2869 7465 6d29  ual_update(item)
-00017270: 3a0d 0a20 2020 2069 6620 6973 696e 7374  :..    if isinst
-00017280: 616e 6365 2869 7465 6d2c 2046 696e 506c  ance(item, FinPl
-00017290: 6f74 4974 656d 293a 0d0a 2020 2020 2020  otItem):..      
-000172a0: 2020 6974 656d 2e61 782e 7265 6d6f 7665    item.ax.remove
-000172b0: 4974 656d 2869 7465 6d29 0d0a 2020 2020  Item(item)..    
-000172c0: 2020 2020 6974 656d 2e64 6972 7479 203d      item.dirty =
-000172d0: 2054 7275 650d 0a20 2020 2065 6c73 653a   True..    else:
-000172e0: 0d0a 2020 2020 2020 2020 7920 3d20 6974  ..        y = it
-000172f0: 656d 2e64 6174 6173 7263 2e79 202f 2069  em.datasrc.y / i
-00017300: 7465 6d2e 6178 2e76 622e 7973 6361 6c65  tem.ax.vb.yscale
-00017310: 2e73 6361 6c65 660d 0a20 2020 2020 2020  .scalef..       
-00017320: 2069 6620 6974 656d 2e61 782e 7662 2e79   if item.ax.vb.y
-00017330: 7363 616c 652e 7363 616c 6574 7970 6520  scale.scaletype 
-00017340: 3d3d 2027 6c6f 6727 3a0d 0a20 2020 2020  == 'log':..     
-00017350: 2020 2020 2020 2079 203d 2079 202b 206c         y = y + l
-00017360: 6f67 5f70 6c6f 745f 6f66 6673 6574 0d0a  og_plot_offset..
-00017370: 2020 2020 2020 2020 6974 656d 2e73 6574          item.set
-00017380: 4461 7461 2869 7465 6d2e 6461 7461 7372  Data(item.datasr
-00017390: 632e 696e 6465 782c 2079 290d 0a0d 0a0d  c.index, y).....
-000173a0: 0a64 6566 205f 656e 645f 7669 7375 616c  .def _end_visual
-000173b0: 5f75 7064 6174 6528 6974 656d 293a 0d0a  _update(item):..
-000173c0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000173d0: 6528 6974 656d 2c20 4669 6e50 6c6f 7449  e(item, FinPlotI
-000173e0: 7465 6d29 3a0d 0a20 2020 2020 2020 2069  tem):..        i
-000173f0: 7465 6d2e 6178 2e61 6464 4974 656d 2869  tem.ax.addItem(i
-00017400: 7465 6d29 0d0a 2020 2020 2020 2020 6974  tem)..        it
-00017410: 656d 2e72 6570 6169 6e74 2829 0d0a 0d0a  em.repaint()....
-00017420: 0d0a 6465 6620 5f73 6574 5f78 5f6c 696d  ..def _set_x_lim
-00017430: 6974 7328 6178 2c20 6461 7461 7372 6329  its(ax, datasrc)
-00017440: 3a0d 0a20 2020 2078 302c 7831 203d 205f  :..    x0,x1 = _
-00017450: 786d 696e 6d61 7828 6461 7461 7372 632c  xminmax(datasrc,
-00017460: 2078 5f69 6e64 6578 6564 3d61 782e 7662   x_indexed=ax.vb
-00017470: 2e78 5f69 6e64 6578 6564 290d 0a20 2020  .x_indexed)..   
-00017480: 2061 782e 7365 744c 696d 6974 7328 784d   ax.setLimits(xM
-00017490: 696e 3d78 302c 2078 4d61 783d 7831 290d  in=x0, xMax=x1).
-000174a0: 0a20 2020 2072 6574 7572 6e20 7830 2c78  .    return x0,x
-000174b0: 310d 0a0d 0a0d 0a64 6566 205f 786d 696e  1......def _xmin
-000174c0: 6d61 7828 6461 7461 7372 632c 2078 5f69  max(datasrc, x_i
-000174d0: 6e64 6578 6564 2c20 696e 6974 5f73 7465  ndexed, init_ste
-000174e0: 7073 3d4e 6f6e 652c 2065 7874 7261 5f6d  ps=None, extra_m
-000174f0: 6172 6769 6e3d 3029 3a0d 0a20 2020 2069  argin=0):..    i
-00017500: 6620 785f 696e 6465 7865 6420 616e 6420  f x_indexed and 
-00017510: 696e 6974 5f73 7465 7073 3a0d 0a20 2020  init_steps:..   
-00017520: 2020 2020 2023 2069 6e69 7469 616c 207a       # initial z
-00017530: 6f6f 6d0d 0a20 2020 2020 2020 2078 3020  oom..        x0 
-00017540: 3d20 6d61 7828 6461 7461 7372 632e 786c  = max(datasrc.xl
-00017550: 656e 2d69 6e69 745f 7374 6570 732c 2030  en-init_steps, 0
-00017560: 2920 2d20 7369 6465 5f6d 6172 6769 6e20  ) - side_margin 
-00017570: 2d20 6578 7472 615f 6d61 7267 696e 0d0a  - extra_margin..
-00017580: 2020 2020 2020 2020 7831 203d 2064 6174          x1 = dat
-00017590: 6173 7263 2e78 6c65 6e20 2b20 7269 6768  asrc.xlen + righ
-000175a0: 745f 6d61 7267 696e 5f63 616e 646c 6573  t_margin_candles
-000175b0: 202b 2073 6964 655f 6d61 7267 696e 202b   + side_margin +
-000175c0: 2065 7874 7261 5f6d 6172 6769 6e0d 0a20   extra_margin.. 
-000175d0: 2020 2065 6c69 6620 785f 696e 6465 7865     elif x_indexe
-000175e0: 643a 0d0a 2020 2020 2020 2020 2320 746f  d:..        # to
-000175f0: 7461 6c20 7820 7369 7a65 2066 6f72 2069  tal x size for i
-00017600: 6e64 6578 6564 2064 6174 610d 0a20 2020  ndexed data..   
-00017610: 2020 2020 2078 3020 3d20 2d73 6964 655f       x0 = -side_
-00017620: 6d61 7267 696e 202d 2065 7874 7261 5f6d  margin - extra_m
-00017630: 6172 6769 6e0d 0a20 2020 2020 2020 2078  argin..        x
-00017640: 3120 3d20 6461 7461 7372 632e 786c 656e  1 = datasrc.xlen
-00017650: 202b 2072 6967 6874 5f6d 6172 6769 6e5f   + right_margin_
-00017660: 6361 6e64 6c65 7320 2d20 3120 2b20 7369  candles - 1 + si
-00017670: 6465 5f6d 6172 6769 6e20 2b20 6578 7472  de_margin + extr
-00017680: 615f 6d61 7267 696e 2023 2061 6464 2061  a_margin # add a
-00017690: 6e6f 7468 6572 206d 6172 6769 6e20 746f  nother margin to
-000176a0: 2067 6574 2074 6865 2022 736e 6170 2062   get the "snap b
-000176b0: 6163 6b22 2073 656e 7361 7469 6f6e 0d0a  ack" sensation..
-000176c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000176d0: 2020 2023 2078 2073 697a 6520 666f 7220     # x size for 
-000176e0: 706c 6169 6e20 592d 6f76 6572 2d58 2064  plain Y-over-X d
-000176f0: 6174 6120 2869 2e65 2e20 6e6f 7420 696e  ata (i.e. not in
-00017700: 6465 7865 6429 0d0a 2020 2020 2020 2020  dexed)..        
-00017710: 7830 203d 2064 6174 6173 7263 2e78 2e6d  x0 = datasrc.x.m
-00017720: 696e 2829 0d0a 2020 2020 2020 2020 7831  in()..        x1
-00017730: 203d 2064 6174 6173 7263 2e78 2e6d 6178   = datasrc.x.max
-00017740: 2829 0d0a 2020 2020 2020 2020 2320 6578  ()..        # ex
-00017750: 7465 6e64 206d 6172 6769 6e20 6f6e 2064  tend margin on d
-00017760: 6563 6f75 706c 6564 2070 6c6f 7473 0d0a  ecoupled plots..
-00017770: 2020 2020 2020 2020 6420 3d20 2878 312d          d = (x1-
-00017780: 7830 2920 2a20 2830 2e32 2b65 7874 7261  x0) * (0.2+extra
-00017790: 5f6d 6172 6769 6e29 0d0a 2020 2020 2020  _margin)..      
-000177a0: 2020 7830 202d 3d20 640d 0a20 2020 2020    x0 -= d..     
-000177b0: 2020 2078 3120 2b3d 2064 0d0a 2020 2020     x1 += d..    
-000177c0: 7265 7475 726e 2078 302c 7831 0d0a 0d0a  return x0,x1....
-000177d0: 0d0a 6465 6620 5f72 6570 6169 6e74 5f63  ..def _repaint_c
-000177e0: 616e 646c 6573 2829 3a0d 0a20 2020 2027  andles():..    '
-000177f0: 2727 4361 6e64 6c65 7320 6172 6520 6f6e  ''Candles are on
-00017800: 6c79 2070 6172 7469 616c 6c79 2064 7261  ly partially dra
-00017810: 776e 2c20 616e 6420 7468 6572 6566 6f72  wn, and therefor
-00017820: 6520 6e65 6564 7320 6d61 6e75 616c 2064  e needs manual d
-00017830: 6972 7479 2072 656d 696e 6465 7220 7768  irty reminder wh
-00017840: 656e 6576 6572 2069 7420 676f 6573 206f  enever it goes o
-00017850: 6666 2d73 6372 6565 6e2e 2727 270d 0a20  ff-screen.'''.. 
-00017860: 2020 2061 7873 203d 205b 6178 2066 6f72     axs = [ax for
-00017870: 2077 696e 2069 6e20 7769 6e64 6f77 7320   win in windows 
-00017880: 666f 7220 6178 2069 6e20 7769 6e2e 6178  for ax in win.ax
-00017890: 735d 202b 206f 7665 726c 6179 5f61 7873  s] + overlay_axs
-000178a0: 0d0a 2020 2020 666f 7220 6178 2069 6e20  ..    for ax in 
-000178b0: 6178 733a 0d0a 2020 2020 2020 2020 666f  axs:..        fo
-000178c0: 7220 6974 656d 2069 6e20 6c69 7374 2861  r item in list(a
-000178d0: 782e 6974 656d 7329 3a0d 0a20 2020 2020  x.items):..     
-000178e0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000178f0: 616e 6365 2869 7465 6d2c 2046 696e 506c  ance(item, FinPl
-00017900: 6f74 4974 656d 293a 0d0a 2020 2020 2020  otItem):..      
-00017910: 2020 2020 2020 2020 2020 5f73 7461 7274            _start
-00017920: 5f76 6973 7561 6c5f 7570 6461 7465 2869  _visual_update(i
-00017930: 7465 6d29 0d0a 2020 2020 2020 2020 2020  tem)..          
-00017940: 2020 2020 2020 5f65 6e64 5f76 6973 7561        _end_visua
-00017950: 6c5f 7570 6461 7465 2869 7465 6d29 0d0a  l_update(item)..
-00017960: 0d0a 0d0a 6465 6620 5f70 6169 6e74 5f73  ....def _paint_s
-00017970: 6361 7474 6572 2869 7465 6d2c 2070 2c20  catter(item, p, 
-00017980: 2a61 7267 7329 3a0d 0a20 2020 2077 6974  *args):..    wit
-00017990: 6820 6e70 2e65 7272 7374 6174 6528 696e  h np.errstate(in
-000179a0: 7661 6c69 643d 2769 676e 6f72 6527 293a  valid='ignore'):
-000179b0: 2023 206d 616b 6520 7067 2773 206d 6173   # make pg's mas
-000179c0: 6b20 6372 6561 7469 6f6e 2063 616c 6c73  k creation calls
-000179d0: 2074 6f20 6e75 6d70 7920 7368 7574 2075   to numpy shut u
-000179e0: 700d 0a20 2020 2020 2020 2069 7465 6d2e  p..        item.
-000179f0: 5f64 6f70 6169 6e74 2870 2c20 2a61 7267  _dopaint(p, *arg
-00017a00: 7329 0d0a 0d0a 0d0a 6465 6620 5f6b 6579  s)......def _key
-00017a10: 5f70 7265 7373 6564 2876 622c 2065 7629  _pressed(vb, ev)
-00017a20: 3a0d 0a20 2020 2069 6620 6576 2e74 6578  :..    if ev.tex
-00017a30: 7428 2920 3d3d 2027 6727 3a20 2320 6772  t() == 'g': # gr
-00017a40: 6964 0d0a 2020 2020 2020 2020 676c 6f62  id..        glob
-00017a50: 616c 2063 6c61 6d70 5f67 7269 640d 0a20  al clamp_grid.. 
-00017a60: 2020 2020 2020 2063 6c61 6d70 5f67 7269         clamp_gri
-00017a70: 6420 3d20 6e6f 7420 636c 616d 705f 6772  d = not clamp_gr
-00017a80: 6964 0d0a 2020 2020 2020 2020 666f 7220  id..        for 
-00017a90: 7769 6e20 696e 2077 696e 646f 7773 3a0d  win in windows:.
-00017aa0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00017ab0: 2061 7820 696e 2077 696e 2e61 7873 3a0d   ax in win.axs:.
-00017ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ad0: 2061 782e 6372 6f73 7368 6169 722e 7570   ax.crosshair.up
-00017ae0: 6461 7465 2829 0d0a 2020 2020 656c 6966  date()..    elif
-00017af0: 2065 762e 7465 7874 2829 2069 6e20 2827   ev.text() in ('
-00017b00: 5c72 272c 2027 2027 293a 2023 2065 6e74  \r', ' '): # ent
-00017b10: 6572 2c20 7370 6163 650d 0a20 2020 2020  er, space..     
-00017b20: 2020 2076 622e 7365 745f 6472 6177 5f6c     vb.set_draw_l
-00017b30: 696e 655f 636f 6c6f 7228 6472 6177 5f64  ine_color(draw_d
-00017b40: 6f6e 655f 636f 6c6f 7229 0d0a 2020 2020  one_color)..    
-00017b50: 2020 2020 7662 2e64 7261 775f 6c69 6e65      vb.draw_line
-00017b60: 203d 204e 6f6e 650d 0a20 2020 2065 6c69   = None..    eli
-00017b70: 6620 6576 2e74 6578 7428 2920 696e 2028  f ev.text() in (
-00017b80: 275c 7837 6627 2c20 275c 6227 293a 2023  '\x7f', '\b'): #
-00017b90: 2064 656c 2c20 6261 636b 7370 6163 650d   del, backspace.
-00017ba0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00017bb0: 7662 2e72 656d 6f76 655f 6c61 7374 5f72  vb.remove_last_r
-00017bc0: 6f69 2829 3a0d 0a20 2020 2020 2020 2020  oi():..         
-00017bd0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00017be0: 0a20 2020 2065 6c69 6620 6576 2e6b 6579  .    elif ev.key
-00017bf0: 2829 203d 3d20 5174 436f 7265 2e51 742e  () == QtCore.Qt.
-00017c00: 4b65 792e 4b65 795f 4c65 6674 3a0d 0a20  Key.Key_Left:.. 
-00017c10: 2020 2020 2020 2076 622e 7061 6e5f 7828         vb.pan_x(
-00017c20: 7065 7263 656e 743d 2d31 3529 0d0a 2020  percent=-15)..  
-00017c30: 2020 656c 6966 2065 762e 6b65 7928 2920    elif ev.key() 
-00017c40: 3d3d 2051 7443 6f72 652e 5174 2e4b 6579  == QtCore.Qt.Key
-00017c50: 2e4b 6579 5f52 6967 6874 3a0d 0a20 2020  .Key_Right:..   
-00017c60: 2020 2020 2076 622e 7061 6e5f 7828 7065       vb.pan_x(pe
-00017c70: 7263 656e 743d 2b31 3529 0d0a 2020 2020  rcent=+15)..    
-00017c80: 656c 6966 2065 762e 6b65 7928 2920 3d3d  elif ev.key() ==
-00017c90: 2051 7443 6f72 652e 5174 2e4b 6579 2e4b   QtCore.Qt.Key.K
-00017ca0: 6579 5f48 6f6d 653a 0d0a 2020 2020 2020  ey_Home:..      
-00017cb0: 2020 7662 2e70 616e 5f78 2873 7465 7073    vb.pan_x(steps
-00017cc0: 3d2d 3165 3130 290d 0a20 2020 2020 2020  =-1e10)..       
-00017cd0: 205f 7265 7061 696e 745f 6361 6e64 6c65   _repaint_candle
-00017ce0: 7328 290d 0a20 2020 2065 6c69 6620 6576  s()..    elif ev
-00017cf0: 2e6b 6579 2829 203d 3d20 5174 436f 7265  .key() == QtCore
-00017d00: 2e51 742e 4b65 792e 4b65 795f 456e 643a  .Qt.Key.Key_End:
-00017d10: 0d0a 2020 2020 2020 2020 7662 2e70 616e  ..        vb.pan
-00017d20: 5f78 2873 7465 7073 3d2b 3165 3130 290d  _x(steps=+1e10).
-00017d30: 0a20 2020 2020 2020 205f 7265 7061 696e  .        _repain
-00017d40: 745f 6361 6e64 6c65 7328 290d 0a20 2020  t_candles()..   
-00017d50: 2065 6c69 6620 6576 2e6b 6579 2829 203d   elif ev.key() =
-00017d60: 3d20 5174 436f 7265 2e51 742e 4b65 792e  = QtCore.Qt.Key.
-00017d70: 4b65 795f 4573 6361 7065 3a0d 0a20 2020  Key_Escape:..   
-00017d80: 2020 2020 2076 622e 7769 6e2e 636c 6f73       vb.win.clos
-00017d90: 6528 290d 0a20 2020 2065 6c73 653a 0d0a  e()..    else:..
-00017da0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00017db0: 616c 7365 0d0a 2020 2020 7265 7475 726e  alse..    return
-00017dc0: 2054 7275 650d 0a0d 0a0d 0a64 6566 205f   True......def _
-00017dd0: 6d6f 7573 655f 636c 6963 6b65 6428 7662  mouse_clicked(vb
-00017de0: 2c20 6576 293a 0d0a 2020 2020 6966 2065  , ev):..    if e
-00017df0: 762e 6275 7474 6f6e 2829 203d 3d20 383a  v.button() == 8:
-00017e00: 2023 2062 6163 6b0d 0a20 2020 2020 2020   # back..       
-00017e10: 2076 622e 7061 6e5f 7828 7065 7263 656e   vb.pan_x(percen
-00017e20: 743d 2d33 3029 0d0a 2020 2020 656c 6966  t=-30)..    elif
-00017e30: 2065 762e 6275 7474 6f6e 2829 203d 3d20   ev.button() == 
-00017e40: 3136 3a20 2320 6677 640d 0a20 2020 2020  16: # fwd..     
-00017e50: 2020 2076 622e 7061 6e5f 7828 7065 7263     vb.pan_x(perc
-00017e60: 656e 743d 2b33 3029 0d0a 2020 2020 656c  ent=+30)..    el
-00017e70: 7365 3a0d 0a20 2020 2020 2020 2072 6574  se:..        ret
-00017e80: 7572 6e20 4661 6c73 650d 0a20 2020 2072  urn False..    r
-00017e90: 6574 7572 6e20 5472 7565 0d0a 0d0a 0d0a  eturn True......
-00017ea0: 6465 6620 5f6d 6f75 7365 5f6d 6f76 6564  def _mouse_moved
-00017eb0: 286d 6173 7465 722c 2065 7673 293a 0d0a  (master, evs):..
-00017ec0: 2020 2020 6966 2068 6173 6174 7472 286d      if hasattr(m
-00017ed0: 6173 7465 722c 2027 636c 6f73 696e 6727  aster, 'closing'
-00017ee0: 2920 616e 6420 6d61 7374 6572 2e63 6c6f  ) and master.clo
-00017ef0: 7369 6e67 3a0d 0a20 2020 2020 2020 2072  sing:..        r
-00017f00: 6574 7572 6e0d 0a20 2020 2069 6620 6e6f  eturn..    if no
-00017f10: 7420 6576 733a 0d0a 2020 2020 2020 2020  t evs:..        
-00017f20: 6576 7320 3d20 6d61 7374 6572 5f64 6174  evs = master_dat
-00017f30: 615b 6d61 7374 6572 5d5b 276c 6173 745f  a[master]['last_
-00017f40: 6d6f 7573 655f 6576 7327 5d0d 0a20 2020  mouse_evs']..   
-00017f50: 2020 2020 2069 6620 6e6f 7420 6576 733a       if not evs:
-00017f60: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00017f70: 7475 726e 0d0a 2020 2020 6d61 7374 6572  turn..    master
-00017f80: 5f64 6174 615b 6d61 7374 6572 5d5b 276c  _data[master]['l
-00017f90: 6173 745f 6d6f 7573 655f 6576 7327 5d20  ast_mouse_evs'] 
-00017fa0: 3d20 6576 730d 0a20 2020 2070 6f73 203d  = evs..    pos =
-00017fb0: 2065 7673 5b2d 315d 0d0a 2020 2020 2320   evs[-1]..    # 
-00017fc0: 616c 6c6f 7720 696e 7465 722d 7069 7865  allow inter-pixe
-00017fd0: 6c20 6d6f 7665 7320 6966 206d 6f76 696e  l moves if movin
-00017fe0: 6720 6d6f 7573 6520 736c 6f77 6c79 0d0a  g mouse slowly..
-00017ff0: 2020 2020 7920 3d20 706f 732e 7928 290d      y = pos.y().
-00018000: 0a20 2020 2064 7920 3d20 7920 2d20 6d61  .    dy = y - ma
-00018010: 7374 6572 5f64 6174 615b 6d61 7374 6572  ster_data[master
-00018020: 5d5b 276c 6173 745f 6d6f 7573 655f 7927  ]['last_mouse_y'
-00018030: 5d0d 0a20 2020 2069 6620 3020 3c20 6162  ]..    if 0 < ab
-00018040: 7328 6479 2920 3c3d 2031 3a0d 0a20 2020  s(dy) <= 1:..   
-00018050: 2020 2020 2070 6f73 2e73 6574 5928 706f       pos.setY(po
-00018060: 732e 7928 2920 2d20 6479 2f32 290d 0a20  s.y() - dy/2).. 
-00018070: 2020 206d 6173 7465 725f 6461 7461 5b6d     master_data[m
-00018080: 6173 7465 725d 5b27 6c61 7374 5f6d 6f75  aster]['last_mou
-00018090: 7365 5f79 275d 203d 2079 0d0a 2020 2020  se_y'] = y..    
-000180a0: 2320 6170 706c 7920 746f 2061 6c6c 2063  # apply to all c
-000180b0: 726f 7373 6861 6972 730d 0a20 2020 2066  rosshairs..    f
-000180c0: 6f72 2061 7820 696e 206d 6173 7465 722e  or ax in master.
-000180d0: 6178 733a 0d0a 2020 2020 2020 2020 6966  axs:..        if
-000180e0: 2061 782e 6973 5669 7369 626c 6528 2920   ax.isVisible() 
-000180f0: 616e 6420 6178 2e63 726f 7373 6861 6972  and ax.crosshair
-00018100: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00018110: 6f69 6e74 203d 2061 782e 7662 2e6d 6170  oint = ax.vb.map
-00018120: 5363 656e 6554 6f56 6965 7728 706f 7329  SceneToView(pos)
-00018130: 0d0a 2020 2020 2020 2020 2020 2020 6178  ..            ax
-00018140: 2e63 726f 7373 6861 6972 2e75 7064 6174  .crosshair.updat
-00018150: 6528 706f 696e 7429 0d0a 0d0a 0d0a 6465  e(point)......de
-00018160: 6620 5f77 6865 656c 5f65 7665 6e74 5f77  f _wheel_event_w
-00018170: 7261 7070 6572 2873 656c 662c 206f 7269  rapper(self, ori
-00018180: 675f 6675 6e63 2c20 6576 293a 0d0a 2020  g_func, ev):..  
-00018190: 2020 2320 7363 726f 6c6c 696e 6720 6f6e    # scrolling on
-000181a0: 2074 6865 2062 6f72 6465 7220 6973 2073   the border is s
-000181b0: 696d 706c 7920 616e 6e6f 7969 6e67 2c20  imply annoying, 
-000181c0: 706f 7020 696e 2061 2063 6f75 706c 6520  pop in a couple 
-000181d0: 6f66 2070 6978 656c 7320 746f 206d 616b  of pixels to mak
-000181e0: 6520 7375 7265 0d0a 2020 2020 6420 3d20  e sure..    d = 
-000181f0: 5174 436f 7265 2e51 506f 696e 7446 282d  QtCore.QPointF(-
-00018200: 322c 3029 0d0a 2020 2020 6576 203d 2051  2,0)..    ev = Q
-00018210: 7447 7569 2e51 5768 6565 6c45 7665 6e74  tGui.QWheelEvent
-00018220: 2865 762e 706f 7369 7469 6f6e 2829 2b64  (ev.position()+d
-00018230: 2c20 6576 2e67 6c6f 6261 6c50 6f73 6974  , ev.globalPosit
-00018240: 696f 6e28 292b 642c 2065 762e 7069 7865  ion()+d, ev.pixe
-00018250: 6c44 656c 7461 2829 2c20 6576 2e61 6e67  lDelta(), ev.ang
-00018260: 6c65 4465 6c74 6128 292c 2065 762e 6275  leDelta(), ev.bu
-00018270: 7474 6f6e 7328 292c 2065 762e 6d6f 6469  ttons(), ev.modi
-00018280: 6669 6572 7328 292c 2065 762e 7068 6173  fiers(), ev.phas
-00018290: 6528 292c 2046 616c 7365 290d 0a20 2020  e(), False)..   
-000182a0: 206f 7269 675f 6675 6e63 2873 656c 662c   orig_func(self,
-000182b0: 2065 7629 0d0a 0d0a 0d0a 6465 6620 5f69   ev)......def _i
-000182c0: 6e73 7065 6374 5f63 6c69 636b 6564 2861  nspect_clicked(a
-000182d0: 782c 2069 6e73 7065 6374 6f72 2c20 7768  x, inspector, wh
-000182e0: 656e 5f64 6f75 626c 655f 636c 6963 6b2c  en_double_click,
-000182f0: 2065 7673 293a 0d0a 2020 2020 6966 2065   evs):..    if e
-00018300: 7673 5b2d 315d 2e61 6363 6570 7465 6420  vs[-1].accepted 
-00018310: 6f72 2077 6865 6e5f 646f 7562 6c65 5f63  or when_double_c
-00018320: 6c69 636b 2021 3d20 6576 735b 2d31 5d2e  lick != evs[-1].
-00018330: 646f 7562 6c65 2829 3a0d 0a20 2020 2020  double():..     
-00018340: 2020 2072 6574 7572 6e0d 0a20 2020 2070     return..    p
-00018350: 6f73 203d 2065 7673 5b2d 315d 2e73 6365  os = evs[-1].sce
-00018360: 6e65 506f 7328 290d 0a20 2020 2072 6574  nePos()..    ret
-00018370: 7572 6e20 5f69 6e73 7065 6374 5f70 6f73  urn _inspect_pos
-00018380: 2861 782c 2069 6e73 7065 6374 6f72 2c20  (ax, inspector, 
-00018390: 2870 6f73 2c29 290d 0a0d 0a0d 0a64 6566  (pos,))......def
-000183a0: 205f 696e 7370 6563 745f 706f 7328 6178   _inspect_pos(ax
-000183b0: 2c20 696e 7370 6563 746f 722c 2070 6f73  , inspector, pos
-000183c0: 7329 3a0d 0a20 2020 2069 6620 6e6f 7420  s):..    if not 
-000183d0: 6178 2e76 622e 6461 7461 7372 633a 0d0a  ax.vb.datasrc:..
-000183e0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-000183f0: 2020 2020 706f 696e 7420 3d20 6178 2e76      point = ax.v
-00018400: 622e 6d61 7053 6365 6e65 546f 5669 6577  b.mapSceneToView
-00018410: 2870 6f73 735b 2d31 5d29 0d0a 2020 2020  (poss[-1])..    
-00018420: 7420 3d20 706f 696e 742e 7828 2920 2b20  t = point.x() + 
-00018430: 302e 350d 0a20 2020 2074 7279 3a0d 0a20  0.5..    try:.. 
-00018440: 2020 2020 2020 2074 203d 2061 782e 7662         t = ax.vb
-00018450: 2e64 6174 6173 7263 2e63 6c6f 7365 7374  .datasrc.closest
-00018460: 5f74 696d 6528 7429 0d0a 2020 2020 6578  _time(t)..    ex
-00018470: 6365 7074 204b 6579 4572 726f 723a 2023  cept KeyError: #
-00018480: 2077 6865 6e20 636c 6963 6b69 6e67 2062   when clicking b
-00018490: 6579 6f6e 6420 7269 6768 745f 6d61 7267  eyond right_marg
-000184a0: 696e 5f63 616e 646c 6573 0d0a 2020 2020  in_candles..    
-000184b0: 2020 2020 6966 2063 6c61 6d70 5f67 7269      if clamp_gri
-000184c0: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-000184d0: 7420 3d20 6178 2e76 622e 6461 7461 7372  t = ax.vb.datasr
-000184e0: 632e 782e 696c 6f63 5b2d 3120 6966 2074  c.x.iloc[-1 if t
-000184f0: 203e 2030 2065 6c73 6520 305d 0d0a 2020   > 0 else 0]..  
-00018500: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00018510: 696e 7370 6563 746f 7228 742c 2070 6f69  inspector(t, poi
-00018520: 6e74 2e79 2829 290d 0a20 2020 2065 7863  nt.y())..    exc
-00018530: 6570 7420 4f53 4572 726f 7220 6173 2065  ept OSError as e
-00018540: 3a0d 0a20 2020 2020 2020 2070 6173 730d  :..        pass.
-00018550: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
-00018560: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-00018570: 2020 2020 2070 7269 6e74 2827 496e 7370       print('Insp
-00018580: 6563 7469 6f6e 2065 7272 6f72 3a27 2c20  ection error:', 
-00018590: 7479 7065 2865 292c 2065 290d 0a0d 0a0d  type(e), e).....
-000185a0: 0a64 6566 2062 7269 6768 7465 6e28 636f  .def brighten(co
-000185b0: 6c6f 722c 2066 293a 0d0a 2020 2020 6966  lor, f):..    if
-000185c0: 206e 6f74 2063 6f6c 6f72 3a0d 0a20 2020   not color:..   
-000185d0: 2020 2020 2072 6574 7572 6e20 636f 6c6f       return colo
-000185e0: 720d 0a20 2020 2072 6574 7572 6e20 7067  r..    return pg
-000185f0: 2e6d 6b43 6f6c 6f72 2863 6f6c 6f72 292e  .mkColor(color).
-00018600: 6c69 6768 7465 7228 696e 7428 662a 3130  lighter(int(f*10
-00018610: 3029 290d 0a0d 0a0d 0a64 6566 205f 6765  0))......def _ge
-00018620: 745f 636f 6c6f 7228 6178 2c20 7374 796c  t_color(ax, styl
-00018630: 652c 2077 616e 7465 645f 636f 6c6f 7229  e, wanted_color)
-00018640: 3a0d 0a20 2020 2069 6620 7479 7065 2877  :..    if type(w
-00018650: 616e 7465 645f 636f 6c6f 7229 2069 6e20  anted_color) in 
-00018660: 2873 7472 2c20 5174 4775 692e 5143 6f6c  (str, QtGui.QCol
-00018670: 6f72 293a 0d0a 2020 2020 2020 2020 7265  or):..        re
-00018680: 7475 726e 2077 616e 7465 645f 636f 6c6f  turn wanted_colo
-00018690: 720d 0a20 2020 2069 6e64 6578 203d 2077  r..    index = w
-000186a0: 616e 7465 645f 636f 6c6f 7220 6966 2074  anted_color if t
-000186b0: 7970 6528 7761 6e74 6564 5f63 6f6c 6f72  ype(wanted_color
-000186c0: 2920 3d3d 2069 6e74 2065 6c73 6520 4e6f  ) == int else No
-000186d0: 6e65 0d0a 2020 2020 6973 5f6c 696e 6520  ne..    is_line 
-000186e0: 3d20 6c61 6d62 6461 2073 7479 6c65 3a20  = lambda style: 
-000186f0: 7374 796c 6520 6973 204e 6f6e 6520 6f72  style is None or
-00018700: 2061 6e79 2863 6820 696e 2073 7479 6c65   any(ch in style
-00018710: 2066 6f72 2063 6820 696e 2027 2d5f 2e27   for ch in '-_.'
-00018720: 290d 0a20 2020 2074 6869 735f 6c69 6e65  )..    this_line
-00018730: 203d 2069 735f 6c69 6e65 2873 7479 6c65   = is_line(style
-00018740: 290d 0a20 2020 2069 6620 7468 6973 5f6c  )..    if this_l
-00018750: 696e 653a 0d0a 2020 2020 2020 2020 636f  ine:..        co
-00018760: 6c6f 7273 203d 2073 6f66 745f 636f 6c6f  lors = soft_colo
-00018770: 7273 0d0a 2020 2020 656c 7365 3a0d 0a20  rs..    else:.. 
-00018780: 2020 2020 2020 2063 6f6c 6f72 7320 3d20         colors = 
-00018790: 6861 7264 5f63 6f6c 6f72 730d 0a20 2020  hard_colors..   
-000187a0: 2069 6620 696e 6465 7820 6973 204e 6f6e   if index is Non
-000187b0: 653a 0d0a 2020 2020 2020 2020 6176 6f69  e:..        avoi
-000187c0: 6420 3d20 7365 7428 692e 6f70 7473 5b27  d = set(i.opts['
-000187d0: 6861 6e64 6564 5f63 6f6c 6f72 275d 2066  handed_color'] f
-000187e0: 6f72 2069 2069 6e20 6178 2e69 7465 6d73  or i in ax.items
-000187f0: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
-00018800: 2c70 672e 506c 6f74 4461 7461 4974 656d  ,pg.PlotDataItem
-00018810: 2920 616e 6420 692e 6f70 7473 5b27 6861  ) and i.opts['ha
-00018820: 6e64 6564 5f63 6f6c 6f72 275d 2069 7320  nded_color'] is 
-00018830: 6e6f 7420 4e6f 6e65 2061 6e64 2074 6869  not None and thi
-00018840: 735f 6c69 6e65 3d3d 6973 5f6c 696e 6528  s_line==is_line(
-00018850: 692e 6f70 7473 5b27 7379 6d62 6f6c 275d  i.opts['symbol']
-00018860: 2929 0d0a 2020 2020 2020 2020 696e 6465  ))..        inde
-00018870: 7820 3d20 6c65 6e28 5b69 2066 6f72 2069  x = len([i for i
-00018880: 2069 6e20 6178 2e69 7465 6d73 2069 6620   in ax.items if 
-00018890: 6973 696e 7374 616e 6365 2869 2c70 672e  isinstance(i,pg.
-000188a0: 506c 6f74 4461 7461 4974 656d 2920 616e  PlotDataItem) an
-000188b0: 6420 692e 6f70 7473 5b27 6861 6e64 6564  d i.opts['handed
-000188c0: 5f63 6f6c 6f72 275d 2069 7320 4e6f 6e65  _color'] is None
-000188d0: 2061 6e64 2074 6869 735f 6c69 6e65 3d3d   and this_line==
-000188e0: 6973 5f6c 696e 6528 692e 6f70 7473 5b27  is_line(i.opts['
-000188f0: 7379 6d62 6f6c 275d 295d 290d 0a20 2020  symbol'])])..   
-00018900: 2020 2020 2077 6869 6c65 2069 6e64 6578       while index
-00018910: 2069 6e20 6176 6f69 643a 0d0a 2020 2020   in avoid:..    
-00018920: 2020 2020 2020 2020 696e 6465 7820 2b3d          index +=
-00018930: 2031 0d0a 2020 2020 7265 7475 726e 2063   1..    return c
-00018940: 6f6c 6f72 735b 696e 6465 7825 6c65 6e28  olors[index%len(
-00018950: 636f 6c6f 7273 295d 0d0a 0d0a 0d0a 6465  colors)]......de
-00018960: 6620 5f70 6474 696d 6532 6570 6f63 6828  f _pdtime2epoch(
-00018970: 7429 3a0d 0a20 2020 2069 6620 6973 696e  t):..    if isin
-00018980: 7374 616e 6365 2874 2c20 7064 2e53 6572  stance(t, pd.Ser
-00018990: 6965 7329 3a0d 0a20 2020 2020 2020 2069  ies):..        i
-000189a0: 6620 6973 696e 7374 616e 6365 2874 2e69  f isinstance(t.i
-000189b0: 6c6f 635b 305d 2c20 7064 2e54 696d 6573  loc[0], pd.Times
-000189c0: 7461 6d70 293a 0d0a 2020 2020 2020 2020  tamp):..        
-000189d0: 2020 2020 7265 7475 726e 2074 2e76 6965      return t.vie
-000189e0: 7728 2769 6e74 3634 2729 0d0a 2020 2020  w('int64')..    
-000189f0: 2020 2020 6820 3d20 6e70 2e6e 616e 6d61      h = np.nanma
-00018a00: 7828 742e 7661 6c75 6573 290d 0a20 2020  x(t.values)..   
-00018a10: 2020 2020 2069 6620 6820 3c20 3165 3130       if h < 1e10
-00018a20: 3a20 2320 6861 6e64 6c65 2073 2065 706f  : # handle s epo
-00018a30: 6368 730d 0a20 2020 2020 2020 2020 2020  chs..           
-00018a40: 2072 6574 7572 6e20 2874 2a31 6539 292e   return (t*1e9).
-00018a50: 6173 7479 7065 2827 696e 7436 3427 290d  astype('int64').
-00018a60: 0a20 2020 2020 2020 2069 6620 6820 3c20  .        if h < 
-00018a70: 3165 3133 3a20 2320 6861 6e64 6c65 206e  1e13: # handle n
-00018a80: 7320 6570 6f63 6873 0d0a 2020 2020 2020  s epochs..      
-00018a90: 2020 2020 2020 7265 7475 726e 2028 742a        return (t*
-00018aa0: 3165 3629 2e61 7374 7970 6528 2769 6e74  1e6).astype('int
-00018ab0: 3634 2729 0d0a 2020 2020 2020 2020 6966  64')..        if
-00018ac0: 2068 203c 2031 6531 363a 2023 2068 616e   h < 1e16: # han
-00018ad0: 646c 6520 7573 2065 706f 6368 730d 0a20  dle us epochs.. 
-00018ae0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00018af0: 6e20 2874 2a31 6533 292e 6173 7479 7065  n (t*1e3).astype
-00018b00: 2827 696e 7436 3427 290d 0a20 2020 2020  ('int64')..     
-00018b10: 2020 2072 6574 7572 6e20 742e 6173 7479     return t.asty
-00018b20: 7065 2827 696e 7436 3427 290d 0a20 2020  pe('int64')..   
-00018b30: 2072 6574 7572 6e20 740d 0a0d 0a0d 0a64   return t......d
-00018b40: 6566 205f 7064 7469 6d65 3269 6e64 6578  ef _pdtime2index
-00018b50: 2861 782c 2074 732c 2061 6e79 5f65 6e64  (ax, ts, any_end
-00018b60: 3d46 616c 7365 2c20 7265 7175 6972 655f  =False, require_
-00018b70: 7469 6d65 3d46 616c 7365 293a 0d0a 2020  time=False):..  
-00018b80: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00018b90: 7473 2e69 6c6f 635b 305d 2c20 7064 2e54  ts.iloc[0], pd.T
-00018ba0: 696d 6573 7461 6d70 293a 0d0a 2020 2020  imestamp):..    
-00018bb0: 2020 2020 7473 203d 2074 732e 7669 6577      ts = ts.view
-00018bc0: 2827 696e 7436 3427 290d 0a20 2020 2065  ('int64')..    e
-00018bd0: 6c73 653a 0d0a 2020 2020 2020 2020 6820  lse:..        h 
-00018be0: 3d20 6e70 2e6e 616e 6d61 7828 7473 2e76  = np.nanmax(ts.v
-00018bf0: 616c 7565 7329 0d0a 2020 2020 2020 2020  alues)..        
-00018c00: 6966 2068 203c 2031 6537 3a0d 0a20 2020  if h < 1e7:..   
-00018c10: 2020 2020 2020 2020 2069 6620 7265 7175           if requ
-00018c20: 6972 655f 7469 6d65 3a0d 0a20 2020 2020  ire_time:..     
-00018c30: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00018c40: 7420 4661 6c73 652c 2027 6e6f 7420 6120  t False, 'not a 
-00018c50: 7469 6d65 2073 6572 6965 7327 0d0a 2020  time series'..  
-00018c60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00018c70: 2074 730d 0a20 2020 2020 2020 2069 6620   ts..        if 
-00018c80: 6820 3c20 3165 3130 3a20 2320 6861 6e64  h < 1e10: # hand
-00018c90: 6c65 2073 2065 706f 6368 730d 0a20 2020  le s epochs..   
-00018ca0: 2020 2020 2020 2020 2074 7320 3d20 7473           ts = ts
-00018cb0: 2e61 7374 7970 6528 2766 6c6f 6174 3634  .astype('float64
-00018cc0: 2729 202a 2031 6539 0d0a 2020 2020 2020  ') * 1e9..      
-00018cd0: 2020 656c 6966 2068 203c 2031 6531 333a    elif h < 1e13:
-00018ce0: 2023 2068 616e 646c 6520 6d73 2065 706f   # handle ms epo
-00018cf0: 6368 730d 0a20 2020 2020 2020 2020 2020  chs..           
-00018d00: 2074 7320 3d20 7473 2e61 7374 7970 6528   ts = ts.astype(
-00018d10: 2766 6c6f 6174 3634 2729 202a 2031 6536  'float64') * 1e6
-00018d20: 0d0a 2020 2020 2020 2020 656c 6966 2068  ..        elif h
-00018d30: 203c 2031 6531 363a 2023 2068 616e 646c   < 1e16: # handl
-00018d40: 6520 7573 2065 706f 6368 730d 0a20 2020  e us epochs..   
-00018d50: 2020 2020 2020 2020 2074 7320 3d20 7473           ts = ts
-00018d60: 2e61 7374 7970 6528 2766 6c6f 6174 3634  .astype('float64
-00018d70: 2729 202a 2031 6533 0d0a 2020 2020 0d0a  ') * 1e3..    ..
-00018d80: 2020 2020 6461 7461 7372 6320 3d20 5f67      datasrc = _g
-00018d90: 6574 5f64 6174 6173 7263 2861 7829 0d0a  et_datasrc(ax)..
-00018da0: 2020 2020 7873 203d 2064 6174 6173 7263      xs = datasrc
-00018db0: 2e78 0d0a 0d0a 2020 2020 2320 7472 7920  .x....    # try 
-00018dc0: 6578 6163 7420 6d61 7463 6820 6265 666f  exact match befo
-00018dd0: 7265 2061 7070 726f 7869 6d61 7465 206d  re approximate m
-00018de0: 6174 6368 0d0a 2020 2020 6578 6163 7420  atch..    exact 
-00018df0: 3d20 6461 7461 7372 632e 696e 6465 785b  = datasrc.index[
-00018e00: 7873 2e69 7369 6e28 7473 295d 2e74 6f5f  xs.isin(ts)].to_
-00018e10: 6c69 7374 2829 0d0a 2020 2020 6966 206c  list()..    if l
-00018e20: 656e 2865 7861 6374 2920 3d3d 206c 656e  en(exact) == len
-00018e30: 2874 7329 3a0d 0a20 2020 2020 2020 2072  (ts):..        r
-00018e40: 6574 7572 6e20 6578 6163 740d 0a20 2020  eturn exact..   
-00018e50: 200d 0a20 2020 2072 203d 205b 5d0d 0a20   ..    r = [].. 
-00018e60: 2020 2066 6f72 2069 2c74 2069 6e20 656e     for i,t in en
-00018e70: 756d 6572 6174 6528 7473 293a 0d0a 2020  umerate(ts):..  
-00018e80: 2020 2020 2020 7873 7320 3d20 7873 2e6c        xss = xs.l
-00018e90: 6f63 5b78 733e 745d 0d0a 2020 2020 2020  oc[xs>t]..      
-00018ea0: 2020 6966 206c 656e 2878 7373 2920 3d3d    if len(xss) ==
-00018eb0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00018ec0: 2074 3020 3d20 7873 2e69 6c6f 635b 2d31   t0 = xs.iloc[-1
-00018ed0: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
-00018ee0: 6620 616e 795f 656e 6420 6f72 2074 3020  f any_end or t0 
-00018ef0: 3d3d 2074 3a0d 0a20 2020 2020 2020 2020  == t:..         
-00018f00: 2020 2020 2020 2072 2e61 7070 656e 6428         r.append(
-00018f10: 6c65 6e28 7873 292d 3129 0d0a 2020 2020  len(xs)-1)..    
-00018f20: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00018f30: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-00018f40: 2020 6966 2069 203e 2030 3a0d 0a20 2020    if i > 0:..   
-00018f50: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00018f60: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
-00018f70: 2020 2061 7373 6572 7420 7420 3c3d 2074     assert t <= t
-00018f80: 302c 2027 6d75 7374 2070 6c6f 7420 7468  0, 'must plot th
-00018f90: 6973 2070 7269 6d69 7469 7665 2069 6e20  is primitive in 
-00018fa0: 7072 696f 7220 7469 6d65 2d72 616e 6765  prior time-range
-00018fb0: 270d 0a20 2020 2020 2020 2069 3120 3d20  '..        i1 = 
-00018fc0: 7873 732e 696e 6465 785b 305d 0d0a 2020  xss.index[0]..  
-00018fd0: 2020 2020 2020 6930 203d 2069 312d 310d        i0 = i1-1.
-00018fe0: 0a20 2020 2020 2020 2069 6620 6930 203c  .        if i0 <
-00018ff0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00019000: 2069 302c 6931 203d 2030 2c31 0d0a 2020   i0,i1 = 0,1..  
-00019010: 2020 2020 2020 7430 2c74 3120 3d20 7873        t0,t1 = xs
-00019020: 2e6c 6f63 5b69 305d 2c20 7873 2e6c 6f63  .loc[i0], xs.loc
-00019030: 5b69 315d 0d0a 2020 2020 2020 2020 6474  [i1]..        dt
-00019040: 203d 2028 742d 7430 2920 2f20 2874 312d   = (t-t0) / (t1-
-00019050: 7430 290d 0a20 2020 2020 2020 2072 2e61  t0)..        r.a
-00019060: 7070 656e 6428 6c65 7270 2864 742c 2069  ppend(lerp(dt, i
-00019070: 302c 2069 3129 290d 0a20 2020 2072 6574  0, i1))..    ret
-00019080: 7572 6e20 720d 0a0d 0a0d 0a64 6566 205f  urn r......def _
-00019090: 6765 745f 6461 7461 7372 6328 6178 2c20  get_datasrc(ax, 
-000190a0: 7265 7175 6972 653d 5472 7565 293a 0d0a  require=True):..
-000190b0: 2020 2020 6966 2061 782e 7662 2e64 6174      if ax.vb.dat
-000190c0: 6173 7263 2069 7320 6e6f 7420 4e6f 6e65  asrc is not None
-000190d0: 206f 7220 6e6f 7420 6178 2e76 622e 785f   or not ax.vb.x_
-000190e0: 696e 6465 7865 643a 0d0a 2020 2020 2020  indexed:..      
-000190f0: 2020 7265 7475 726e 2061 782e 7662 2e64    return ax.vb.d
-00019100: 6174 6173 7263 0d0a 2020 2020 7662 7320  atasrc..    vbs 
-00019110: 3d20 5b61 782e 7662 2066 6f72 2077 696e  = [ax.vb for win
-00019120: 2069 6e20 7769 6e64 6f77 7320 666f 7220   in windows for 
-00019130: 6178 2069 6e20 7769 6e2e 6178 735d 0d0a  ax in win.axs]..
-00019140: 2020 2020 666f 7220 7662 2069 6e20 7662      for vb in vb
-00019150: 733a 0d0a 2020 2020 2020 2020 6966 2076  s:..        if v
-00019160: 622e 6461 7461 7372 633a 0d0a 2020 2020  b.datasrc:..    
-00019170: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-00019180: 622e 6461 7461 7372 630d 0a20 2020 2069  b.datasrc..    i
-00019190: 6620 7265 7175 6972 653a 0d0a 2020 2020  f require:..    
-000191a0: 2020 2020 6173 7365 7274 2061 782e 7662      assert ax.vb
-000191b0: 2e64 6174 6173 7263 2c20 276e 6f74 2070  .datasrc, 'not p
-000191c0: 6f73 7369 626c 6520 746f 2070 6c6f 7420  ossible to plot 
-000191d0: 7468 6973 2070 7269 6d69 7469 7665 2077  this primitive w
-000191e0: 6974 686f 7574 2061 2070 7269 6f72 2074  ithout a prior t
-000191f0: 696d 652d 7261 6e67 6520 746f 2063 6f6d  ime-range to com
-00019200: 7061 7265 2074 6f27 0d0a 0d0a 0d0a 6465  pare to'......de
-00019210: 6620 5f6d 696c 6c69 7365 636f 6e64 5f74  f _millisecond_t
-00019220: 7a5f 7772 6170 2873 293a 0d0a 2020 2020  z_wrap(s):..    
-00019230: 6966 206c 656e 2873 2920 3e20 3620 616e  if len(s) > 6 an
-00019240: 6420 735b 2d36 5d20 696e 2027 2b2d 2720  d s[-6] in '+-' 
-00019250: 616e 6420 735b 2d33 5d20 3d3d 2027 3a27  and s[-3] == ':'
-00019260: 3a20 2320 2b30 313a 3030 2066 6d74 2074  : # +01:00 fmt t
-00019270: 696d 657a 6f6e 6520 7072 6573 656e 743f  imezone present?
-00019280: 0d0a 2020 2020 2020 2020 7320 3d20 735b  ..        s = s[
-00019290: 3a2d 365d 0d0a 2020 2020 7265 7475 726e  :-6]..    return
-000192a0: 2028 732b 272e 3030 3030 3030 2729 2069   (s+'.000000') i
-000192b0: 6620 272e 2720 6e6f 7420 696e 2073 2065  f '.' not in s e
-000192c0: 6c73 6520 730d 0a0d 0a0d 0a64 6566 205f  lse s......def _
-000192d0: 7832 6c6f 6361 6c5f 7428 6461 7461 7372  x2local_t(datasr
-000192e0: 632c 2078 293a 0d0a 2020 2020 6966 2064  c, x):..    if d
-000192f0: 6973 706c 6179 5f74 696d 657a 6f6e 6520  isplay_timezone 
-00019300: 3d3d 204e 6f6e 653a 0d0a 2020 2020 2020  == None:..      
-00019310: 2020 7265 7475 726e 205f 7832 7574 6328    return _x2utc(
-00019320: 6461 7461 7372 632c 2078 290d 0a20 2020  datasrc, x)..   
-00019330: 2072 6574 7572 6e20 5f78 3274 2864 6174   return _x2t(dat
-00019340: 6173 7263 2c20 782c 206c 616d 6264 6120  asrc, x, lambda 
-00019350: 743a 205f 6d69 6c6c 6973 6563 6f6e 645f  t: _millisecond_
-00019360: 747a 5f77 7261 7028 6461 7465 7469 6d65  tz_wrap(datetime
-00019370: 2e66 726f 6d74 696d 6573 7461 6d70 2874  .fromtimestamp(t
-00019380: 2f31 6539 2c20 747a 3d64 6973 706c 6179  /1e9, tz=display
-00019390: 5f74 696d 657a 6f6e 6529 2e69 736f 666f  _timezone).isofo
-000193a0: 726d 6174 2873 6570 3d27 2027 2929 290d  rmat(sep=' '))).
-000193b0: 0a0d 0a0d 0a64 6566 205f 7832 7574 6328  .....def _x2utc(
-000193c0: 6461 7461 7372 632c 2078 293a 0d0a 2020  datasrc, x):..  
-000193d0: 2020 2320 7573 696e 6720 7064 2e74 6f5f    # using pd.to_
-000193e0: 6461 7465 7469 6d65 2061 6c6c 6f77 2066  datetime allow f
-000193f0: 6f72 2070 7265 2d31 3937 3020 6461 7465  or pre-1970 date
-00019400: 730d 0a20 2020 2072 6574 7572 6e20 5f78  s..    return _x
-00019410: 3274 2864 6174 6173 7263 2c20 782c 206c  2t(datasrc, x, l
-00019420: 616d 6264 6120 743a 2070 642e 746f 5f64  ambda t: pd.to_d
-00019430: 6174 6574 696d 6528 742c 2075 6e69 743d  atetime(t, unit=
-00019440: 276e 7327 292e 7374 7266 7469 6d65 2827  'ns').strftime('
-00019450: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-00019460: 532e 2566 2729 290d 0a0d 0a0d 0a64 6566  S.%f'))......def
-00019470: 205f 7832 7428 6461 7461 7372 632c 2078   _x2t(datasrc, x
-00019480: 2c20 7473 3273 7472 293a 0d0a 2020 2020  , ts2str):..    
-00019490: 6966 206e 6f74 2064 6174 6173 7263 3a0d  if not datasrc:.
-000194a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000194b0: 2727 2c46 616c 7365 0d0a 2020 2020 7472  '',False..    tr
-000194c0: 793a 0d0a 2020 2020 2020 2020 7820 2b3d  y:..        x +=
-000194d0: 2030 2e35 0d0a 2020 2020 2020 2020 742c   0.5..        t,
-000194e0: 5f2c 5f2c 5f2c 636e 7420 3d20 6461 7461  _,_,_,cnt = data
-000194f0: 7372 632e 6869 6c6f 2878 2c20 7829 0d0a  src.hilo(x, x)..
-00019500: 2020 2020 2020 2020 6966 2063 6e74 3a0d          if cnt:.
-00019510: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00019520: 6e6f 7420 6461 7461 7372 632e 7469 6d65  not datasrc.time
-00019530: 6261 7365 6428 293a 0d0a 2020 2020 2020  based():..      
-00019540: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00019550: 2027 2567 2720 2520 742c 2046 616c 7365   '%g' % t, False
-00019560: 0d0a 2020 2020 2020 2020 2020 2020 7320  ..            s 
-00019570: 3d20 7473 3273 7472 2874 290d 0a20 2020  = ts2str(t)..   
-00019580: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00019590: 2020 2020 2020 2069 6620 6570 6f63 685f         if epoch_
-000195a0: 7065 7269 6f64 203e 3d20 3233 2a36 302a  period >= 23*60*
-000195b0: 3630 3a20 2320 6461 796c 6967 6874 2073  60: # daylight s
-000195c0: 6176 696e 6773 2c20 6c65 6170 2073 6563  avings, leap sec
-000195d0: 6f6e 6473 2c20 6574 630d 0a20 2020 2020  onds, etc..     
-000195e0: 2020 2020 2020 2020 2020 2069 203d 2073             i = s
-000195f0: 2e69 6e64 6578 2827 2027 290d 0a20 2020  .index(' ')..   
-00019600: 2020 2020 2020 2020 2065 6c69 6620 6570           elif ep
-00019610: 6f63 685f 7065 7269 6f64 203e 3d20 3539  och_period >= 59
-00019620: 3a20 2320 636f 6e73 6964 6572 206c 6561  : # consider lea
-00019630: 7020 7365 636f 6e64 730d 0a20 2020 2020  p seconds..     
-00019640: 2020 2020 2020 2020 2020 2069 203d 2073             i = s
-00019650: 2e72 696e 6465 7828 273a 2729 0d0a 2020  .rindex(':')..  
-00019660: 2020 2020 2020 2020 2020 656c 6966 2065            elif e
-00019670: 706f 6368 5f70 6572 696f 6420 3e3d 2031  poch_period >= 1
-00019680: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019690: 2020 2069 203d 2073 2e69 6e64 6578 2827     i = s.index('
-000196a0: 2e27 2920 6966 2027 2e27 2069 6e20 7320  .') if '.' in s 
-000196b0: 656c 7365 206c 656e 2873 290d 0a20 2020  else len(s)..   
-000196c0: 2020 2020 2020 2020 2065 6c69 6620 6570           elif ep
-000196d0: 6f63 685f 7065 7269 6f64 203e 3d20 302e  och_period >= 0.
-000196e0: 3030 313a 0d0a 2020 2020 2020 2020 2020  001:..          
-000196f0: 2020 2020 2020 6920 3d20 2d33 0d0a 2020        i = -3..  
-00019700: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00019710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019720: 2069 203d 206c 656e 2873 290d 0a20 2020   i = len(s)..   
-00019730: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00019740: 735b 3a69 5d2c 5472 7565 0d0a 2020 2020  s[:i],True..    
-00019750: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00019760: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
-00019770: 696d 706f 7274 2074 7261 6365 6261 636b  import traceback
-00019780: 0d0a 2020 2020 2020 2020 7472 6163 6562  ..        traceb
-00019790: 6163 6b2e 7072 696e 745f 6578 6328 290d  ack.print_exc().
-000197a0: 0a20 2020 2072 6574 7572 6e20 2727 2c64  .    return '',d
-000197b0: 6174 6173 7263 2e74 696d 6562 6173 6564  atasrc.timebased
-000197c0: 2829 0d0a 0d0a 0d0a 6465 6620 5f78 3279  ()......def _x2y
-000197d0: 6561 7228 6461 7461 7372 632c 2078 293a  ear(datasrc, x):
-000197e0: 0d0a 2020 2020 742c 6861 7364 7320 3d20  ..    t,hasds = 
-000197f0: 5f78 326c 6f63 616c 5f74 2864 6174 6173  _x2local_t(datas
-00019800: 7263 2c20 7829 0d0a 2020 2020 7265 7475  rc, x)..    retu
-00019810: 726e 2074 5b3a 345d 2c68 6173 6473 0d0a  rn t[:4],hasds..
-00019820: 0d0a 0d0a 6465 6620 5f72 6f75 6e64 5f74  ....def _round_t
-00019830: 6f5f 7369 676e 6966 6963 616e 7428 726e  o_significant(rn
-00019840: 672c 2072 6e67 6d61 782c 2078 2c20 7369  g, rngmax, x, si
-00019850: 676e 6966 6963 616e 745f 6465 6369 6d61  gnificant_decima
-00019860: 6c73 2c20 7369 676e 6966 6963 616e 745f  ls, significant_
-00019870: 6570 7329 3a0d 0a20 2020 2069 735f 6869  eps):..    is_hi
-00019880: 6768 7265 7320 3d20 2872 6e67 2f73 6967  ghres = (rng/sig
-00019890: 6e69 6669 6361 6e74 5f65 7073 203e 2031  nificant_eps > 1
-000198a0: 6532 2061 6e64 2072 6e67 6d61 783c 3165  e2 and rngmax<1e
-000198b0: 2d32 2920 6f72 2061 6273 2872 6e67 6d61  -2) or abs(rngma
-000198c0: 7829 203e 2031 6537 206f 7220 726e 6720  x) > 1e7 or rng 
-000198d0: 3c20 3165 2d35 0d0a 2020 2020 7364 203d  < 1e-5..    sd =
-000198e0: 2073 6967 6e69 6669 6361 6e74 5f64 6563   significant_dec
-000198f0: 696d 616c 730d 0a20 2020 2069 6620 6973  imals..    if is
-00019900: 5f68 6967 6872 6573 2061 6e64 2061 6273  _highres and abs
-00019910: 2878 293e 303a 0d0a 2020 2020 2020 2020  (x)>0:..        
-00019920: 6578 7031 3020 3d20 666c 6f6f 7228 6e70  exp10 = floor(np
-00019930: 2e6c 6f67 3130 2861 6273 2878 2929 290d  .log10(abs(x))).
-00019940: 0a20 2020 2020 2020 2078 203d 2078 202f  .        x = x /
-00019950: 2028 3130 2a2a 6578 7031 3029 0d0a 2020   (10**exp10)..  
-00019960: 2020 2020 2020 726d 203d 2069 6e74 2861        rm = int(a
-00019970: 6273 286e 702e 6c6f 6731 3028 726e 676d  bs(np.log10(rngm
-00019980: 6178 2929 2920 6966 2072 6e67 6d61 783e  ax))) if rngmax>
-00019990: 3020 656c 7365 2030 0d0a 2020 2020 2020  0 else 0..      
-000199a0: 2020 7364 203d 206d 696e 2833 2c20 7364    sd = min(3, sd
-000199b0: 2b72 6d29 0d0a 2020 2020 2020 2020 666d  +rm)..        fm
-000199c0: 7420 3d20 2725 2525 692e 2569 6665 2525  t = '%%%i.%ife%%
-000199d0: 6927 2025 2028 7364 2c20 7364 290d 0a20  i' % (sd, sd).. 
-000199e0: 2020 2020 2020 2072 203d 2066 6d74 2025         r = fmt %
-000199f0: 2028 782c 2065 7870 3130 290d 0a20 2020   (x, exp10)..   
-00019a00: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00019a10: 6570 7320 3d20 666d 6f64 2878 2c20 7369  eps = fmod(x, si
-00019a20: 676e 6966 6963 616e 745f 6570 7329 0d0a  gnificant_eps)..
-00019a30: 2020 2020 2020 2020 6966 2061 6273 2865          if abs(e
-00019a40: 7073 2920 3e3d 2073 6967 6e69 6669 6361  ps) >= significa
-00019a50: 6e74 5f65 7073 2f32 3a0d 0a20 2020 2020  nt_eps/2:..     
-00019a60: 2020 2020 2020 2023 2072 6f75 6e64 2075         # round u
-00019a70: 700d 0a20 2020 2020 2020 2020 2020 2065  p..            e
-00019a80: 7073 202d 3d20 6e70 2e73 6967 6e28 6570  ps -= np.sign(ep
-00019a90: 7329 2a73 6967 6e69 6669 6361 6e74 5f65  s)*significant_e
-00019aa0: 7073 0d0a 2020 2020 2020 2020 7820 2d3d  ps..        x -=
-00019ab0: 2065 7073 0d0a 2020 2020 2020 2020 666d   eps..        fm
-00019ac0: 7420 3d20 2725 2525 692e 2569 6627 2025  t = '%%%i.%if' %
-00019ad0: 2028 7364 2c20 7364 290d 0a20 2020 2020   (sd, sd)..     
-00019ae0: 2020 2072 203d 2066 6d74 2025 2078 0d0a     r = fmt % x..
-00019af0: 2020 2020 7265 7475 726e 2072 0d0a 0d0a      return r....
-00019b00: 0d0a 6465 6620 5f72 6f69 6861 6e64 6c65  ..def _roihandle
-00019b10: 5f6d 6f76 655f 736e 6170 2876 622c 206f  _move_snap(vb, o
-00019b20: 7269 675f 6675 6e63 2c20 706f 732c 206d  rig_func, pos, m
-00019b30: 6f64 6966 6965 7273 3d51 7443 6f72 652e  odifiers=QtCore.
-00019b40: 5174 2e4b 6579 626f 6172 644d 6f64 6966  Qt.KeyboardModif
-00019b50: 6965 722c 2066 696e 6973 683d 5472 7565  ier, finish=True
-00019b60: 293a 0d0a 2020 2020 706f 7320 3d20 7662  ):..    pos = vb
-00019b70: 2e6d 6170 4465 7669 6365 546f 5669 6577  .mapDeviceToView
-00019b80: 2870 6f73 290d 0a20 2020 2070 6f73 203d  (pos)..    pos =
-00019b90: 205f 636c 616d 705f 706f 696e 7428 7662   _clamp_point(vb
-00019ba0: 2e70 6172 656e 7428 292c 2070 6f73 290d  .parent(), pos).
-00019bb0: 0a20 2020 2070 6f73 203d 2076 622e 6d61  .    pos = vb.ma
-00019bc0: 7056 6965 7754 6f44 6576 6963 6528 706f  pViewToDevice(po
-00019bd0: 7329 0d0a 2020 2020 6f72 6967 5f66 756e  s)..    orig_fun
-00019be0: 6328 706f 732c 206d 6f64 6966 6965 7273  c(pos, modifiers
-00019bf0: 3d6d 6f64 6966 6965 7273 2c20 6669 6e69  =modifiers, fini
-00019c00: 7368 3d66 696e 6973 6829 0d0a 0d0a 0d0a  sh=finish)......
-00019c10: 6465 6620 5f63 6c61 6d70 5f78 7928 6178  def _clamp_xy(ax
-00019c20: 2c20 782c 2079 293a 0d0a 2020 2020 7920  , x, y):..    y 
-00019c30: 3d20 6178 2e76 622e 7973 6361 6c65 2e78  = ax.vb.yscale.x
-00019c40: 666f 726d 2879 290d 0a20 2020 2069 6620  form(y)..    if 
-00019c50: 636c 616d 705f 6772 6964 2061 6e64 2061  clamp_grid and a
-00019c60: 782e 7662 2e78 5f69 6e64 6578 6564 3a0d  x.vb.x_indexed:.
-00019c70: 0a20 2020 2020 2020 2064 7320 3d20 6178  .        ds = ax
-00019c80: 2e76 622e 6461 7461 7372 630d 0a20 2020  .vb.datasrc..   
-00019c90: 2020 2020 2069 6620 7820 3c20 3020 6f72       if x < 0 or
-00019ca0: 2028 6473 2061 6e64 2078 203e 206c 656e   (ds and x > len
-00019cb0: 2864 732e 6466 292d 3129 3a0d 0a20 2020  (ds.df)-1):..   
-00019cc0: 2020 2020 2020 2020 2078 203d 2030 2069           x = 0 i
-00019cd0: 6620 7820 3c20 3020 656c 7365 206c 656e  f x < 0 else len
-00019ce0: 2864 732e 6466 292d 310d 0a20 2020 2020  (ds.df)-1..     
-00019cf0: 2020 2078 203d 205f 726f 756e 6428 7829     x = _round(x)
-00019d00: 0d0a 2020 2020 2020 2020 6570 7320 3d20  ..        eps = 
-00019d10: 6178 2e73 6967 6e69 6669 6361 6e74 5f65  ax.significant_e
-00019d20: 7073 0d0a 2020 2020 2020 2020 6966 2065  ps..        if e
-00019d30: 7073 203e 2031 652d 383a 0d0a 2020 2020  ps > 1e-8:..    
-00019d40: 2020 2020 2020 2020 6570 7332 203d 206e          eps2 = n
-00019d50: 702e 7369 676e 2879 2920 2a20 302e 3520  p.sign(y) * 0.5 
-00019d60: 2a20 6570 730d 0a20 2020 2020 2020 2020  * eps..         
-00019d70: 2020 2079 202d 3d20 666d 6f64 2879 2b65     y -= fmod(y+e
-00019d80: 7073 322c 2065 7073 2920 2d20 6570 7332  ps2, eps) - eps2
-00019d90: 0d0a 2020 2020 7920 3d20 6178 2e76 622e  ..    y = ax.vb.
-00019da0: 7973 6361 6c65 2e69 6e76 7866 6f72 6d28  yscale.invxform(
-00019db0: 792c 2076 6572 6966 793d 5472 7565 290d  y, verify=True).
-00019dc0: 0a20 2020 2072 6574 7572 6e20 782c 2079  .    return x, y
-00019dd0: 0d0a 0d0a 0d0a 6465 6620 5f63 6c61 6d70  ......def _clamp
-00019de0: 5f70 6f69 6e74 2861 782c 2070 293a 0d0a  _point(ax, p):..
-00019df0: 2020 2020 6966 2063 6c61 6d70 5f67 7269      if clamp_gri
-00019e00: 643a 0d0a 2020 2020 2020 2020 782c 7920  d:..        x,y 
-00019e10: 3d20 5f63 6c61 6d70 5f78 7928 6178 2c20  = _clamp_xy(ax, 
-00019e20: 702e 7828 292c 2070 2e79 2829 290d 0a20  p.x(), p.y()).. 
-00019e30: 2020 2020 2020 2072 6574 7572 6e20 7067         return pg
-00019e40: 2e50 6f69 6e74 2878 2c20 7929 0d0a 2020  .Point(x, y)..  
-00019e50: 2020 7265 7475 726e 2070 0d0a 0d0a 0d0a    return p......
-00019e60: 6465 6620 5f64 7261 775f 6c69 6e65 5f73  def _draw_line_s
-00019e70: 6567 6d65 6e74 5f74 6578 7428 706f 6c79  egment_text(poly
-00019e80: 6c69 6e65 2c20 7365 676d 656e 742c 2070  line, segment, p
-00019e90: 6f73 302c 2070 6f73 3129 3a0d 0a20 2020  os0, pos1):..   
-00019ea0: 2066 7365 6373 203d 204e 6f6e 650d 0a20   fsecs = None.. 
-00019eb0: 2020 2064 6174 6173 7263 203d 2070 6f6c     datasrc = pol
-00019ec0: 796c 696e 652e 7662 2e64 6174 6173 7263  yline.vb.datasrc
-00019ed0: 0d0a 2020 2020 6966 2064 6174 6173 7263  ..    if datasrc
-00019ee0: 2061 6e64 2063 6c61 6d70 5f67 7269 643a   and clamp_grid:
-00019ef0: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00019f00: 2020 2020 2020 2020 2020 2020 7830 2c78              x0,x
-00019f10: 3120 3d20 706f 7330 2e78 2829 2b30 2e35  1 = pos0.x()+0.5
-00019f20: 2c20 706f 7331 2e78 2829 2b30 2e35 0d0a  , pos1.x()+0.5..
-00019f30: 2020 2020 2020 2020 2020 2020 7430 2c5f              t0,_
-00019f40: 2c5f 2c5f 2c63 6e74 3020 3d20 6461 7461  ,_,_,cnt0 = data
-00019f50: 7372 632e 6869 6c6f 2878 302c 2078 3029  src.hilo(x0, x0)
-00019f60: 0d0a 2020 2020 2020 2020 2020 2020 7431  ..            t1
-00019f70: 2c5f 2c5f 2c5f 2c63 6e74 3120 3d20 6461  ,_,_,_,cnt1 = da
-00019f80: 7461 7372 632e 6869 6c6f 2878 312c 2078  tasrc.hilo(x1, x
-00019f90: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00019fa0: 6966 2063 6e74 3020 616e 6420 636e 7431  if cnt0 and cnt1
-00019fb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019fc0: 2020 2066 7365 6373 203d 2061 6273 2874     fsecs = abs(t
-00019fd0: 3120 2d20 7430 2920 2f20 3165 390d 0a20  1 - t0) / 1e9.. 
-00019fe0: 2020 2020 2020 2065 7863 6570 743a 0d0a         except:..
-00019ff0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0001a000: 0d0a 2020 2020 6469 6666 203d 2070 6f73  ..    diff = pos
-0001a010: 3120 2d20 706f 7330 0d0a 2020 2020 6966  1 - pos0..    if
-0001a020: 2066 7365 6373 2069 7320 4e6f 6e65 3a0d   fsecs is None:.
-0001a030: 0a20 2020 2020 2020 2066 7365 6373 203d  .        fsecs =
-0001a040: 2061 6273 2864 6966 662e 7828 292a 6570   abs(diff.x()*ep
-0001a050: 6f63 685f 7065 7269 6f64 290d 0a20 2020  och_period)..   
-0001a060: 2073 6563 7320 3d20 696e 7428 6673 6563   secs = int(fsec
-0001a070: 7329 0d0a 2020 2020 6d69 6e73 203d 2073  s)..    mins = s
-0001a080: 6563 732f 2f36 300d 0a20 2020 2068 6f75  ecs//60..    hou
-0001a090: 7273 203d 206d 696e 732f 2f36 300d 0a20  rs = mins//60.. 
-0001a0a0: 2020 206d 696e 7320 3d20 6d69 6e73 2536     mins = mins%6
-0001a0b0: 300d 0a20 2020 2073 6563 7320 3d20 7365  0..    secs = se
-0001a0c0: 6373 2536 300d 0a20 2020 2069 6620 686f  cs%60..    if ho
-0001a0d0: 7572 733d 3d30 2061 6e64 206d 696e 733d  urs==0 and mins=
-0001a0e0: 3d30 2061 6e64 2073 6563 7320 3c20 3630  =0 and secs < 60
-0001a0f0: 2061 6e64 2065 706f 6368 5f70 6572 696f   and epoch_perio
-0001a100: 6420 3c20 313a 0d0a 2020 2020 2020 2020  d < 1:..        
-0001a110: 6d73 6563 7320 3d20 696e 7428 2866 7365  msecs = int((fse
-0001a120: 6373 2d69 6e74 2866 7365 6373 2929 2a31  cs-int(fsecs))*1
-0001a130: 3030 3029 0d0a 2020 2020 2020 2020 7473  000)..        ts
-0001a140: 203d 2027 2530 2e32 693a 2530 2e32 692e   = '%0.2i:%0.2i.
-0001a150: 2530 2e33 6927 2025 2028 6d69 6e73 2c20  %0.3i' % (mins, 
-0001a160: 7365 6373 2c20 6d73 6563 7329 0d0a 2020  secs, msecs)..  
-0001a170: 2020 656c 6966 2068 6f75 7273 3d3d 3020    elif hours==0 
-0001a180: 616e 6420 6d69 6e73 203c 2036 3020 616e  and mins < 60 an
-0001a190: 6420 6570 6f63 685f 7065 7269 6f64 203c  d epoch_period <
-0001a1a0: 2036 303a 0d0a 2020 2020 2020 2020 7473   60:..        ts
-0001a1b0: 203d 2027 2530 2e32 693a 2530 2e32 693a   = '%0.2i:%0.2i:
-0001a1c0: 2530 2e32 6927 2025 2028 686f 7572 732c  %0.2i' % (hours,
-0001a1d0: 206d 696e 732c 2073 6563 7329 0d0a 2020   mins, secs)..  
-0001a1e0: 2020 656c 6966 2068 6f75 7273 203c 2032    elif hours < 2
-0001a1f0: 343a 0d0a 2020 2020 2020 2020 7473 203d  4:..        ts =
-0001a200: 2027 2530 2e32 693a 2530 2e32 6927 2025   '%0.2i:%0.2i' %
-0001a210: 2028 686f 7572 732c 206d 696e 7329 0d0a   (hours, mins)..
-0001a220: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001a230: 2020 2064 6179 7320 3d20 686f 7572 7320     days = hours 
-0001a240: 2f2f 2032 340d 0a20 2020 2020 2020 2068  // 24..        h
-0001a250: 6f75 7273 2025 3d20 3234 0d0a 2020 2020  ours %= 24..    
-0001a260: 2020 2020 7473 203d 2027 2569 6420 2530      ts = '%id %0
-0001a270: 2e32 693a 2530 2e32 6927 2025 2028 6461  .2i:%0.2i' % (da
-0001a280: 7973 2c20 686f 7572 732c 206d 696e 7329  ys, hours, mins)
-0001a290: 0d0a 2020 2020 2020 2020 6966 2074 732e  ..        if ts.
-0001a2a0: 656e 6473 7769 7468 2827 2030 303a 3030  endswith(' 00:00
-0001a2b0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0001a2c0: 2074 7320 3d20 7473 2e70 6172 7469 7469   ts = ts.partiti
-0001a2d0: 6f6e 2827 2027 295b 305d 0d0a 2020 2020  on(' ')[0]..    
-0001a2e0: 7973 6320 3d20 706f 6c79 6c69 6e65 2e76  ysc = polyline.v
-0001a2f0: 622e 7973 6361 6c65 0d0a 2020 2020 6966  b.yscale..    if
-0001a300: 2070 6f6c 796c 696e 652e 7662 2e79 5f70   polyline.vb.y_p
-0001a310: 6f73 6974 6976 653a 0d0a 2020 2020 2020  ositive:..      
-0001a320: 2020 7930 2c79 3120 3d20 7973 632e 7866    y0,y1 = ysc.xf
-0001a330: 6f72 6d28 706f 7330 2e79 2829 292c 2079  orm(pos0.y()), y
-0001a340: 7363 2e78 666f 726d 2870 6f73 312e 7928  sc.xform(pos1.y(
-0001a350: 2929 0d0a 2020 2020 2020 2020 6966 2079  ))..        if y
-0001a360: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-0001a370: 7661 6c75 6520 3d20 2725 2b2e 3266 2025  value = '%+.2f %
-0001a380: 2527 2025 2028 3130 3020 2a20 7931 202f  %' % (100 * y1 /
-0001a390: 2079 3020 2d20 3130 3029 0d0a 2020 2020   y0 - 100)..    
-0001a3a0: 2020 2020 656c 6966 206e 6f74 2079 313a      elif not y1:
-0001a3b0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-0001a3c0: 6c75 6520 3d20 2730 270d 0a20 2020 2020  lue = '0'..     
-0001a3d0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0001a3e0: 2020 2020 2020 7661 6c75 6520 3d20 272b        value = '+
-0001a3f0: e288 9e27 2069 6620 7931 3e30 2065 6c73  ...' if y1>0 els
-0001a400: 6520 272d e288 9e27 0d0a 2020 2020 656c  e '-...'..    el
-0001a410: 7365 3a0d 0a20 2020 2020 2020 2064 7920  se:..        dy 
-0001a420: 3d20 7973 632e 7866 6f72 6d28 6469 6666  = ysc.xform(diff
-0001a430: 2e79 2829 290d 0a20 2020 2020 2020 2069  .y())..        i
-0001a440: 6620 6479 2061 6e64 2028 6162 7328 6479  f dy and (abs(dy
-0001a450: 2920 3e3d 2031 6534 206f 7220 6162 7328  ) >= 1e4 or abs(
-0001a460: 6479 2920 3c3d 2031 652d 3229 3a0d 0a20  dy) <= 1e-2):.. 
-0001a470: 2020 2020 2020 2020 2020 2076 616c 7565             value
-0001a480: 203d 2027 252b 332e 3367 2720 2520 6479   = '%+3.3g' % dy
-0001a490: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001a4a0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0001a4b0: 7565 203d 2027 252b 322e 3266 2720 2520  ue = '%+2.2f' % 
-0001a4c0: 6479 0d0a 2020 2020 6578 7472 6120 3d20  dy..    extra = 
-0001a4d0: 5f64 7261 775f 6c69 6e65 5f65 7874 7261  _draw_line_extra
-0001a4e0: 5f74 6578 7428 706f 6c79 6c69 6e65 2c20  _text(polyline, 
-0001a4f0: 7365 676d 656e 742c 2070 6f73 302c 2070  segment, pos0, p
-0001a500: 6f73 3129 0d0a 2020 2020 7265 7475 726e  os1)..    return
-0001a510: 2027 2573 2025 7320 2825 7329 2720 2520   '%s %s (%s)' % 
-0001a520: 2876 616c 7565 2c20 6578 7472 612c 2074  (value, extra, t
-0001a530: 7329 0d0a 0d0a 0d0a 6465 6620 5f64 7261  s)......def _dra
-0001a540: 775f 6c69 6e65 5f65 7874 7261 5f74 6578  w_line_extra_tex
-0001a550: 7428 706f 6c79 6c69 6e65 2c20 7365 676d  t(polyline, segm
-0001a560: 656e 742c 2070 6f73 302c 2070 6f73 3129  ent, pos0, pos1)
-0001a570: 3a0d 0a20 2020 2027 2727 5368 6f77 7320  :..    '''Shows 
-0001a580: 7468 6520 7072 6f70 6f72 7469 6f6e 7320  the proportions 
-0001a590: 6f66 2074 6869 7320 6c69 6e65 2068 6569  of this line hei
-0001a5a0: 6768 7420 636f 6d70 6172 6564 2074 6f20  ght compared to 
-0001a5b0: 7468 6520 7072 6576 696f 7573 2073 6567  the previous seg
-0001a5c0: 6d65 6e74 2e27 2727 0d0a 2020 2020 7072  ment.'''..    pr
-0001a5d0: 6576 5f74 6578 7420 3d20 4e6f 6e65 0d0a  ev_text = None..
-0001a5e0: 2020 2020 666f 7220 7465 7874 2069 6e20      for text in 
-0001a5f0: 706f 6c79 6c69 6e65 2e74 6578 7473 3a0d  polyline.texts:.
-0001a600: 0a20 2020 2020 2020 2069 6620 7072 6576  .        if prev
-0001a610: 5f74 6578 7420 6973 206e 6f74 204e 6f6e  _text is not Non
-0001a620: 6520 616e 6420 7465 7874 2e73 6567 6d65  e and text.segme
-0001a630: 6e74 203d 3d20 7365 676d 656e 743a 0d0a  nt == segment:..
-0001a640: 2020 2020 2020 2020 2020 2020 6830 203d              h0 =
-0001a650: 2070 7265 765f 7465 7874 2e73 6567 6d65   prev_text.segme
-0001a660: 6e74 2e68 616e 646c 6573 5b30 5d5b 2769  nt.handles[0]['i
-0001a670: 7465 6d27 5d0d 0a20 2020 2020 2020 2020  tem']..         
-0001a680: 2020 2068 3120 3d20 7072 6576 5f74 6578     h1 = prev_tex
-0001a690: 742e 7365 676d 656e 742e 6861 6e64 6c65  t.segment.handle
-0001a6a0: 735b 315d 5b27 6974 656d 275d 0d0a 2020  s[1]['item']..  
-0001a6b0: 2020 2020 2020 2020 2020 7072 6576 5f63            prev_c
-0001a6c0: 6861 6e67 6520 3d20 6831 2e70 6f73 2829  hange = h1.pos()
-0001a6d0: 2e79 2829 202d 2068 302e 706f 7328 292e  .y() - h0.pos().
-0001a6e0: 7928 290d 0a20 2020 2020 2020 2020 2020  y()..           
-0001a6f0: 2074 6869 735f 6368 616e 6765 203d 2070   this_change = p
-0001a700: 6f73 312e 7928 2920 2d20 706f 7330 2e79  os1.y() - pos0.y
-0001a710: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0001a720: 6966 206e 6f74 2061 6273 2870 7265 765f  if not abs(prev_
-0001a730: 6368 616e 6765 2920 3e20 3165 2d31 343a  change) > 1e-14:
-0001a740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a750: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-0001a760: 2020 2020 2063 6861 6e67 655f 7061 7274       change_part
-0001a770: 203d 2061 6273 2874 6869 735f 6368 616e   = abs(this_chan
-0001a780: 6765 202f 2070 7265 765f 6368 616e 6765  ge / prev_change
-0001a790: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0001a7a0: 6574 7572 6e20 2720 3d20 313a 252e 3266  eturn ' = 1:%.2f
-0001a7b0: 2027 2025 2063 6861 6e67 655f 7061 7274   ' % change_part
-0001a7c0: 0d0a 2020 2020 2020 2020 7072 6576 5f74  ..        prev_t
-0001a7d0: 6578 7420 3d20 7465 7874 0d0a 2020 2020  ext = text..    
-0001a7e0: 7265 7475 726e 2027 270d 0a0d 0a0d 0a64  return ''......d
-0001a7f0: 6566 205f 6d61 6b65 7065 6e28 636f 6c6f  ef _makepen(colo
-0001a800: 722c 2073 7479 6c65 3d4e 6f6e 652c 2077  r, style=None, w
-0001a810: 6964 7468 3d31 293a 0d0a 2020 2020 6966  idth=1):..    if
-0001a820: 2073 7479 6c65 2069 7320 4e6f 6e65 206f   style is None o
-0001a830: 7220 7374 796c 6520 3d3d 2027 2d27 3a0d  r style == '-':.
-0001a840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a850: 7067 2e6d 6b50 656e 2863 6f6c 6f72 3d63  pg.mkPen(color=c
-0001a860: 6f6c 6f72 2c20 7769 6474 683d 7769 6474  olor, width=widt
-0001a870: 6829 0d0a 2020 2020 6461 7368 203d 205b  h)..    dash = [
-0001a880: 5d0d 0a20 2020 2066 6f72 2063 6820 696e  ]..    for ch in
-0001a890: 2073 7479 6c65 3a0d 0a20 2020 2020 2020   style:..       
-0001a8a0: 2069 6620 6368 203d 3d20 272d 273a 0d0a   if ch == '-':..
-0001a8b0: 2020 2020 2020 2020 2020 2020 6461 7368              dash
-0001a8c0: 202b 3d20 5b34 2c32 5d0d 0a20 2020 2020   += [4,2]..     
-0001a8d0: 2020 2065 6c69 6620 6368 203d 3d20 275f     elif ch == '_
-0001a8e0: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-0001a8f0: 6461 7368 202b 3d20 5b31 302c 325d 0d0a  dash += [10,2]..
-0001a900: 2020 2020 2020 2020 656c 6966 2063 6820          elif ch 
-0001a910: 3d3d 2027 2e27 3a0d 0a20 2020 2020 2020  == '.':..       
-0001a920: 2020 2020 2064 6173 6820 2b3d 205b 312c       dash += [1,
-0001a930: 325d 0d0a 2020 2020 2020 2020 656c 6966  2]..        elif
-0001a940: 2063 6820 3d3d 2027 2027 3a0d 0a20 2020   ch == ' ':..   
-0001a950: 2020 2020 2020 2020 2069 6620 6461 7368           if dash
-0001a960: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a970: 2020 2064 6173 685b 2d31 5d20 2b3d 2032     dash[-1] += 2
-0001a980: 0d0a 2020 2020 7265 7475 726e 2070 672e  ..    return pg.
-0001a990: 6d6b 5065 6e28 636f 6c6f 723d 636f 6c6f  mkPen(color=colo
-0001a9a0: 722c 2073 7479 6c65 3d51 7443 6f72 652e  r, style=QtCore.
-0001a9b0: 5174 2e50 656e 5374 796c 652e 4375 7374  Qt.PenStyle.Cust
-0001a9c0: 6f6d 4461 7368 4c69 6e65 2c20 6461 7368  omDashLine, dash
-0001a9d0: 3d64 6173 682c 2077 6964 7468 3d77 6964  =dash, width=wid
-0001a9e0: 7468 290d 0a0d 0a0d 0a64 6566 205f 726f  th)......def _ro
-0001a9f0: 756e 6428 7629 3a0d 0a20 2020 2072 6574  und(v):..    ret
-0001aa00: 7572 6e20 666c 6f6f 7228 762b 302e 3529  urn floor(v+0.5)
-0001aa10: 0d0a 0d0a 0d0a 7472 793a 0d0a 2020 2020  ......try:..    
-0001aa20: 7174 7665 7220 3d20 2725 642e 2564 2720  qtver = '%d.%d' 
-0001aa30: 2520 2851 7443 6f72 652e 5154 5f56 4552  % (QtCore.QT_VER
-0001aa40: 5349 4f4e 2f2f 3235 362f 2f32 3536 2c20  SION//256//256, 
-0001aa50: 5174 436f 7265 2e51 545f 5645 5253 494f  QtCore.QT_VERSIO
-0001aa60: 4e2f 2f32 3536 2532 3536 290d 0a20 2020  N//256%256)..   
-0001aa70: 2069 6620 7174 7665 7220 6e6f 7420 696e   if qtver not in
-0001aa80: 2028 2735 2e39 272c 2027 352e 3133 2729   ('5.9', '5.13')
-0001aa90: 2061 6e64 205b 696e 7428 6929 2066 6f72   and [int(i) for
-0001aaa0: 2069 2069 6e20 7067 2e5f 5f76 6572 7369   i in pg.__versi
-0001aab0: 6f6e 5f5f 2e73 706c 6974 2827 2e27 295d  on__.split('.')]
-0001aac0: 203c 3d20 5b30 2c31 312c 305d 3a0d 0a20   <= [0,11,0]:.. 
-0001aad0: 2020 2020 2020 2070 7269 6e74 2827 5741         print('WA
-0001aae0: 524e 494e 473a 2079 6f75 7220 7665 7273  RNING: your vers
-0001aaf0: 696f 6e20 6f66 2051 7420 6d61 7920 6e6f  ion of Qt may no
-0001ab00: 7420 706c 6f74 2063 7572 7665 7320 636f  t plot curves co
-0001ab10: 6e74 6169 6e69 6e67 204e 614e 7320 616e  ntaining NaNs an
-0001ab20: 6420 6973 206e 6f74 2072 6563 6f6d 6d65  d is not recomme
-0001ab30: 6e64 6564 2e27 290d 0a20 2020 2020 2020  nded.')..       
-0001ab40: 2070 7269 6e74 2827 5365 6520 6874 7470   print('See http
-0001ab50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-0001ab60: 7971 7467 7261 7068 2f70 7971 7467 7261  yqtgraph/pyqtgra
-0001ab70: 7068 2f69 7373 7565 732f 3130 3537 2729  ph/issues/1057')
-0001ab80: 0d0a 6578 6365 7074 3a0d 0a20 2020 2070  ..except:..    p
-0001ab90: 6173 730d 0a0d 0a69 6d70 6f72 7420 6c6f  ass....import lo
-0001aba0: 6361 6c65 0d0a 636f 6465 2c5f 203d 206c  cale..code,_ = l
-0001abb0: 6f63 616c 652e 6765 7464 6566 6175 6c74  ocale.getdefault
-0001abc0: 6c6f 6361 6c65 2829 0d0a 6966 2063 6f64  locale()..if cod
-0001abd0: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-0001abe0: 6420 5c0d 0a20 2020 2061 6e79 2873 616e  d \..    any(san
-0001abf0: 6374 696f 6e65 6420 696e 2063 6f64 652e  ctioned in code.
-0001ac00: 6c6f 7765 7228 2920 666f 7220 7361 6e63  lower() for sanc
-0001ac10: 7469 6f6e 6564 2069 6e20 275f 7275 205f  tioned in '_ru _
-0001ac20: 6279 2072 755f 2062 655f 272e 7370 6c69  by ru_ be_'.spli
-0001ac30: 7428 2929 206f 7220 5c0d 0a20 2020 2061  t()) or \..    a
-0001ac40: 6e79 2873 616e 6374 696f 6e65 6420 696e  ny(sanctioned in
-0001ac50: 2063 6f64 652e 6c6f 7765 7228 2920 666f   code.lower() fo
-0001ac60: 7220 7361 6e63 7469 6f6e 6564 2069 6e20  r sanctioned in 
-0001ac70: 2772 7520 6265 272e 7370 6c69 7428 2929  'ru be'.split())
-0001ac80: 3a0d 0a20 2020 2069 6d70 6f72 7420 6f73  :..    import os
-0001ac90: 0d0a 2020 2020 6f73 2e5f 6578 6974 2831  ..    os._exit(1
-0001aca0: 290d 0a20 2020 2061 7373 6572 7420 4661  )..    assert Fa
-0001acb0: 6c73 650d 0a0d 0a23 2064 6566 6175 6c74  lse....# default
-0001acc0: 2074 6f20 626c 6163 6b2d 6f6e 2d77 6869   to black-on-whi
-0001acd0: 7465 0d0a 7067 2e77 6964 6765 7473 2e47  te..pg.widgets.G
-0001ace0: 7261 7068 6963 7356 6965 772e 4772 6170  raphicsView.Grap
-0001acf0: 6869 6373 5669 6577 2e77 6865 656c 4576  hicsView.wheelEv
-0001ad00: 656e 7420 3d20 7061 7274 6961 6c6d 6574  ent = partialmet
-0001ad10: 686f 6428 5f77 6865 656c 5f65 7665 6e74  hod(_wheel_event
-0001ad20: 5f77 7261 7070 6572 2c20 7067 2e77 6964  _wrapper, pg.wid
-0001ad30: 6765 7473 2e47 7261 7068 6963 7356 6965  gets.GraphicsVie
-0001ad40: 772e 4772 6170 6869 6373 5669 6577 2e77  w.GraphicsView.w
-0001ad50: 6865 656c 4576 656e 7429 0d0a 2320 7573  heelEvent)..# us
-0001ad60: 6520 6669 6e70 6c6f 7420 696e 7374 6561  e finplot instea
-0001ad70: 6420 6f66 206d 6174 706c 6f74 6c69 620d  d of matplotlib.
-0001ad80: 0a70 642e 7365 745f 6f70 7469 6f6e 2827  .pd.set_option('
-0001ad90: 706c 6f74 7469 6e67 2e62 6163 6b65 6e64  plotting.backend
-0001ada0: 272c 2027 6669 6e70 6c6f 742e 7064 706c  ', 'finplot.pdpl
-0001adb0: 6f74 2729 0d0a 2320 7069 636b 2075 7020  ot')..# pick up 
-0001adc0: 7769 6e20 7265 736f 6c75 7469 6f6e 0d0a  win resolution..
-0001add0: 7472 793a 0d0a 2020 2020 696d 706f 7274  try:..    import
-0001ade0: 2063 7479 7065 730d 0a20 2020 2075 7365   ctypes..    use
-0001adf0: 7233 3220 3d20 6374 7970 6573 2e77 696e  r32 = ctypes.win
-0001ae00: 646c 6c2e 7573 6572 3332 0d0a 2020 2020  dll.user32..    
-0001ae10: 7573 6572 3332 2e53 6574 5072 6f63 6573  user32.SetProces
-0001ae20: 7344 5049 4177 6172 6528 290d 0a20 2020  sDPIAware()..   
-0001ae30: 206c 6f64 5f63 616e 646c 6573 203d 2069   lod_candles = i
-0001ae40: 6e74 2875 7365 7233 322e 4765 7453 7973  nt(user32.GetSys
-0001ae50: 7465 6d4d 6574 7269 6373 2830 2920 2a20  temMetrics(0) * 
-0001ae60: 312e 3629 0d0a 2020 2020 6361 6e64 6c65  1.6)..    candle
-0001ae70: 5f73 6861 646f 775f 7769 6474 6820 3d20  _shadow_width = 
-0001ae80: 696e 7428 7573 6572 3332 2e47 6574 5379  int(user32.GetSy
-0001ae90: 7374 656d 4d65 7472 6963 7328 3029 202f  stemMetrics(0) /
-0001aea0: 2f20 3231 3030 202b 2031 2920 2320 3235  / 2100 + 1) # 25
-0001aeb0: 3630 2061 6e64 2072 6573 6f6c 7574 696f  60 and resolutio
-0001aec0: 6e73 2061 626f 7665 202d 3e20 7769 6465  ns above -> wide
-0001aed0: 7220 7368 6164 6f77 730d 0a65 7863 6570  r shadows..excep
-0001aee0: 743a 0d0a 2020 2020 7061 7373 0d0a       t:..    pass..
+0000c5d0: 2020 636f 6c6f 7220 3d20 7365 6c66 2e63    color = self.c
+0000c5e0: 6f6c 6d61 702e 6d61 7028 762c 206d 6f64  olmap.map(v, mod
+0000c5f0: 653d 2771 636f 6c6f 7227 290d 0a20 2020  e='qcolor')..   
+0000c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c610: 2070 2e66 696c 6c52 6563 7428 5174 436f   p.fillRect(QtCo
+0000c620: 7265 2e51 5265 6374 4628 742d 7265 6374  re.QRectF(t-rect
+0000c630: 5f73 697a 6532 2c20 7365 6c66 2e61 782e  _size2, self.ax.
+0000c640: 7662 2e79 7363 616c 652e 696e 7678 666f  vb.yscale.invxfo
+0000c650: 726d 2870 7269 6365 2b68 3029 2c20 7365  rm(price+h0), se
+0000c660: 6c66 2e72 6563 745f 7369 7a65 2c20 7365  lf.rect_size, se
+0000c670: 6c66 2e61 782e 7662 2e79 7363 616c 652e  lf.ax.vb.yscale.
+0000c680: 696e 7678 666f 726d 2868 3129 292c 2063  invxform(h1)), c
+0000c690: 6f6c 6f72 290d 0a0d 0a0d 0a0d 0a63 6c61  olor)........cla
+0000c6a0: 7373 2048 6f72 697a 6f6e 7461 6c54 696d  ss HorizontalTim
+0000c6b0: 6556 6f6c 756d 6549 7465 6d28 4361 6e64  eVolumeItem(Cand
+0000c6c0: 6c65 7374 6963 6b49 7465 6d29 3a0d 0a20  lestickItem):.. 
+0000c6d0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000c6e0: 7365 6c66 2c20 6178 2c20 6461 7461 7372  self, ax, datasr
+0000c6f0: 632c 2063 616e 646c 655f 7769 6474 683d  c, candle_width=
+0000c700: 302e 382c 2064 7261 775f 7661 3d30 2e30  0.8, draw_va=0.0
+0000c710: 2c20 6472 6177 5f62 6f64 793d 302e 342c  , draw_body=0.4,
+0000c720: 2064 7261 775f 706f 633d 302e 302c 2063   draw_poc=0.0, c
+0000c730: 6f6c 6f72 6675 6e63 3d4e 6f6e 6529 3a0d  olorfunc=None):.
+0000c740: 0a20 2020 2020 2020 2027 2727 4120 6e65  .        '''A ne
+0000c750: 6761 7469 7665 2064 7261 775f 626f 6479  gative draw_body
+0000c760: 2064 6f65 7320 6e6f 7420 6d65 616e 2074   does not mean t
+0000c770: 6861 7420 7468 6520 6361 6e64 6c65 2069  hat the candle i
+0000c780: 7320 6472 6177 6e20 696e 2074 6865 206f  s drawn in the o
+0000c790: 7070 6f73 6974 6520 6469 7265 6374 696f  pposite directio
+0000c7a0: 6e20 2875 7365 206e 6567 6174 6976 6520  n (use negative 
+0000c7b0: 766f 6c75 6d65 2066 6f72 2074 6861 7429  volume for that)
+0000c7c0: 2c0d 0a20 2020 2020 2020 2020 2020 6275  ,..           bu
+0000c7d0: 7420 696e 7374 6561 6420 7468 6174 2073  t instead that s
+0000c7e0: 6372 6565 6e20 7363 616c 6520 7769 6c6c  creen scale will
+0000c7f0: 2062 6520 7573 6564 2069 6e73 7465 6164   be used instead
+0000c800: 206f 6620 696e 7465 7276 616c 2d72 656c   of interval-rel
+0000c810: 6174 6976 6520 7363 616c 652e 2727 270d  ative scale.'''.
+0000c820: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
+0000c830: 6177 5f76 6120 3d20 6472 6177 5f76 610d  aw_va = draw_va.
+0000c840: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
+0000c850: 6177 5f70 6f63 203d 2064 7261 775f 706f  aw_poc = draw_po
+0000c860: 630d 0a20 2020 2020 2020 2023 2320 7365  c..        ## se
+0000c870: 6c66 2e63 6f6c 5f64 6174 615f 656e 6420  lf.col_data_end 
+0000c880: 3d20 6c65 6e28 6461 7461 7372 632e 6466  = len(datasrc.df
+0000c890: 2e63 6f6c 756d 6e73 290d 0a20 2020 2020  .columns)..     
+0000c8a0: 2020 2063 6f6c 6f72 6675 6e63 203d 2063     colorfunc = c
+0000c8b0: 6f6c 6f72 6675 6e63 206f 7220 686f 7269  olorfunc or hori
+0000c8c0: 7a76 6f6c 5f63 6f6c 6f72 6669 6c74 6572  zvol_colorfilter
+0000c8d0: 2829 2023 2072 6573 6f6c 7665 2066 756e  () # resolve fun
+0000c8e0: 6374 696f 6e20 6c6f 7765 7220 646f 776e  ction lower down
+0000c8f0: 2069 6e20 736f 7572 6365 2063 6f64 650d   in source code.
+0000c900: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0000c910: 2e5f 5f69 6e69 745f 5f28 6178 2c20 6461  .__init__(ax, da
+0000c920: 7461 7372 632c 2064 7261 775f 7368 6164  tasrc, draw_shad
+0000c930: 6f77 3d46 616c 7365 2c20 6361 6e64 6c65  ow=False, candle
+0000c940: 5f77 6964 7468 3d63 616e 646c 655f 7769  _width=candle_wi
+0000c950: 6474 682c 2064 7261 775f 626f 6479 3d64  dth, draw_body=d
+0000c960: 7261 775f 626f 6479 2c20 636f 6c6f 7266  raw_body, colorf
+0000c970: 756e 633d 636f 6c6f 7266 756e 6329 0d0a  unc=colorfunc)..
+0000c980: 2020 2020 2020 2020 7365 6c66 2e6c 6f64          self.lod
+0000c990: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+0000c9a0: 2020 7365 6c66 2e63 6f6c 6f72 732e 7570    self.colors.up
+0000c9b0: 6461 7465 2864 6963 7428 6e65 7574 7261  date(dict(neutra
+0000c9c0: 6c5f 7368 6164 6f77 2020 3d20 766f 6c75  l_shadow  = volu
+0000c9d0: 6d65 5f6e 6575 7472 616c 5f63 6f6c 6f72  me_neutral_color
+0000c9e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca00: 2020 206e 6575 7472 616c 5f66 7261 6d65     neutral_frame
+0000ca10: 2020 203d 2076 6f6c 756d 655f 6e65 7574     = volume_neut
+0000ca20: 7261 6c5f 636f 6c6f 722c 0d0a 2020 2020  ral_color,..    
+0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca40: 2020 2020 2020 2020 2020 2020 6e65 7574              neut
+0000ca50: 7261 6c5f 626f 6479 2020 2020 3d20 766f  ral_body    = vo
+0000ca60: 6c75 6d65 5f6e 6575 7472 616c 5f63 6f6c  lume_neutral_col
+0000ca70: 6f72 2c0d 0a20 2020 2020 2020 2020 2020  or,..           
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 2020 2020 2062 756c 6c5f 626f 6479 2020       bull_body  
+0000caa0: 2020 2020 203d 2063 616e 646c 655f 6275       = candle_bu
+0000cab0: 6c6c 5f63 6f6c 6f72 2929 0d0a 0d0a 2020  ll_color))....  
+0000cac0: 2020 6465 6620 6765 6e65 7261 7465 5f70    def generate_p
+0000cad0: 6963 7475 7265 2873 656c 662c 2062 6f75  icture(self, bou
+0000cae0: 6e64 696e 6752 6563 7429 3a0d 0a20 2020  ndingRect):..   
+0000caf0: 2020 2020 2074 696d 6573 203d 2073 656c       times = sel
+0000cb00: 662e 6461 7461 7372 632e 6466 2e69 6c6f  f.datasrc.df.ilo
+0000cb10: 635b 3a2c 2030 5d0d 0a20 2020 2020 2020  c[:, 0]..       
+0000cb20: 2076 616c 7320 3d20 7365 6c66 2e64 6174   vals = self.dat
+0000cb30: 6173 7263 2e64 662e 7661 6c75 6573 0d0a  asrc.df.values..
+0000cb40: 2020 2020 2020 2020 7072 6963 6573 203d          prices =
+0000cb50: 2076 616c 735b 3a2c 2073 656c 662e 6461   vals[:, self.da
+0000cb60: 7461 7372 632e 636f 6c5f 6461 7461 5f6f  tasrc.col_data_o
+0000cb70: 6666 7365 743a 3a32 5d0d 0a20 2020 2020  ffset::2]..     
+0000cb80: 2020 2076 6f6c 756d 6573 203d 2076 616c     volumes = val
+0000cb90: 735b 3a2c 2073 656c 662e 6461 7461 7372  s[:, self.datasr
+0000cba0: 632e 636f 6c5f 6461 7461 5f6f 6666 7365  c.col_data_offse
+0000cbb0: 742b 313a 3a32 5d2e 540d 0a20 2020 2020  t+1::2].T..     
+0000cbc0: 2020 2023 206e 6f72 6d61 6c69 7a65 0d0a     # normalize..
+0000cbd0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+0000cbe0: 2020 2020 2020 2020 2020 6620 3d20 7365            f = se
+0000cbf0: 6c66 2e64 6174 6173 7263 2e70 6572 696f  lf.datasrc.perio
+0000cc00: 645f 6e73 202f 205f 6765 745f 6461 7461  d_ns / _get_data
+0000cc10: 7372 6328 7365 6c66 2e61 7829 2e70 6572  src(self.ax).per
+0000cc20: 696f 645f 6e73 0d0a 2020 2020 2020 2020  iod_ns..        
+0000cc30: 2020 2020 7469 6d65 7320 3d20 5f70 6474      times = _pdt
+0000cc40: 696d 6532 696e 6465 7828 7365 6c66 2e61  ime2index(self.a
+0000cc50: 782c 2074 696d 6573 2c20 7265 7175 6972  x, times, requir
+0000cc60: 655f 7469 6d65 3d54 7275 6529 0d0a 2020  e_time=True)..  
+0000cc70: 2020 2020 2020 6578 6365 7074 2041 7373        except Ass
+0000cc80: 6572 7469 6f6e 4572 726f 723a 0d0a 2020  ertionError:..  
+0000cc90: 2020 2020 2020 2020 2020 6620 3d20 310d            f = 1.
+0000cca0: 0a20 2020 2020 2020 2064 7261 775f 626f  .        draw_bo
+0000ccb0: 6479 203d 2073 656c 662e 6472 6177 5f62  dy = self.draw_b
+0000ccc0: 6f64 790d 0a20 2020 2020 2020 2069 6620  ody..        if 
+0000ccd0: 6472 6177 5f62 6f64 7920 3c20 303a 0d0a  draw_body < 0:..
+0000cce0: 2020 2020 2020 2020 2020 2020 6620 2a3d              f *=
+0000ccf0: 202d 6472 6177 5f62 6f64 7920 2a20 7365   -draw_body * se
+0000cd00: 6c66 2e61 782e 7662 2e74 6172 6765 7452  lf.ax.vb.targetR
+0000cd10: 6563 7428 292e 7769 6474 6828 290d 0a20  ect().width().. 
+0000cd20: 2020 2020 2020 2020 2020 2064 7261 775f             draw_
+0000cd30: 626f 6479 203d 2031 0d0a 2020 2020 2020  body = 1..      
+0000cd40: 2020 6269 6e63 203d 206c 656e 2876 6f6c    binc = len(vol
+0000cd50: 756d 6573 290d 0a20 2020 2020 2020 2069  umes)..        i
+0000cd60: 6620 6e6f 7420 6269 6e63 3a0d 0a20 2020  f not binc:..   
+0000cd70: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+0000cd80: 0a20 2020 2020 2020 2064 6976 766f 6c20  .        divvol 
+0000cd90: 3d20 6e70 2e6e 616e 6d61 7828 6e70 2e61  = np.nanmax(np.a
+0000cda0: 6273 2876 6f6c 756d 6573 292c 2061 7869  bs(volumes), axi
+0000cdb0: 733d 3029 0d0a 2020 2020 2020 2020 6469  s=0)..        di
+0000cdc0: 7676 6f6c 5b64 6976 766f 6c3d 3d30 5d20  vvol[divvol==0] 
+0000cdd0: 3d20 310d 0a20 2020 2020 2020 2076 6f6c  = 1..        vol
+0000cde0: 756d 6573 203d 2028 766f 6c75 6d65 7320  umes = (volumes 
+0000cdf0: 2a20 6620 2f20 6469 7676 6f6c 292e 540d  * f / divvol).T.
+0000ce00: 0a20 2020 2020 2020 2070 203d 2073 656c  .        p = sel
+0000ce10: 662e 7061 696e 7465 720d 0a20 2020 2020  f.painter..     
+0000ce20: 2020 2068 203d 2031 652d 3130 0d0a 2020     h = 1e-10..  
+0000ce30: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000ce40: 616e 6765 286c 656e 2870 7269 6365 7329  ange(len(prices)
+0000ce50: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000ce60: 7072 6372 203d 2070 7269 6365 735b 695d  prcr = prices[i]
+0000ce70: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000ce80: 7620 3d20 7072 6372 5b7e 6e70 2e69 736e  v = prcr[~np.isn
+0000ce90: 616e 2870 7263 7229 5d0d 0a20 2020 2020  an(prcr)]..     
+0000cea0: 2020 2020 2020 2069 6620 6c65 6e28 7072         if len(pr
+0000ceb0: 7629 203e 2031 3a0d 0a20 2020 2020 2020  v) > 1:..       
+0000cec0: 2020 2020 2020 2020 2068 203d 206e 702e           h = np.
+0000ced0: 6469 6666 2870 7276 292e 6d69 6e28 290d  diff(prv).min().
+0000cee0: 0a20 2020 2020 2020 2020 2020 2074 203d  .            t =
+0000cef0: 2074 696d 6573 5b69 5d0d 0a20 2020 2020   times[i]..     
+0000cf00: 2020 2020 2020 2076 6f6c 7220 3d20 6e70         volr = np
+0000cf10: 2e6e 616e 5f74 6f5f 6e75 6d28 766f 6c75  .nan_to_num(volu
+0000cf20: 6d65 735b 695d 290d 0a0d 0a20 2020 2020  mes[i])....     
+0000cf30: 2020 2020 2020 2023 2063 616c 6320 706f         # calc po
+0000cf40: 630d 0a20 2020 2020 2020 2020 2020 2070  c..            p
+0000cf50: 6f63 6964 7820 3d20 6e70 2e6e 616e 6172  ocidx = np.nanar
+0000cf60: 676d 6178 2876 6f6c 7229 0d0a 0d0a 2020  gmax(volr)....  
+0000cf70: 2020 2020 2020 2020 2020 2320 6472 6177            # draw
+0000cf80: 2076 616c 7565 2061 7265 610d 0a20 2020   value area..   
+0000cf90: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000cfa0: 2e64 7261 775f 7661 3a0d 0a20 2020 2020  .draw_va:..     
+0000cfb0: 2020 2020 2020 2020 2020 2076 6f6c 7273             volrs
+0000cfc0: 203d 2076 6f6c 7220 2f20 6e70 2e6e 616e   = volr / np.nan
+0000cfd0: 7375 6d28 766f 6c72 290d 0a20 2020 2020  sum(volr)..     
+0000cfe0: 2020 2020 2020 2020 2020 2076 203d 2076             v = v
+0000cff0: 6f6c 7273 5b70 6f63 6964 785d 0d0a 2020  olrs[pocidx]..  
+0000d000: 2020 2020 2020 2020 2020 2020 2020 6120                a 
+0000d010: 3d20 6220 3d20 706f 6369 6478 0d0a 2020  = b = pocidx..  
+0000d020: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+0000d030: 696c 6520 613e 3d30 206f 7220 623c 6269  ile a>=0 or b<bi
+0000d040: 6e63 3a0d 0a20 2020 2020 2020 2020 2020  nc:..           
+0000d050: 2020 2020 2020 2020 2069 6620 7620 3e3d           if v >=
+0000d060: 2073 656c 662e 6472 6177 5f76 613a 0d0a   self.draw_va:..
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0a0: 2020 2061 6120 3d20 6120 2d20 310d 0a20     aa = a - 1.. 
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2020 2062 6220 3d20 6220 2b20 310d 0a20     bb = b + 1.. 
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2076 6120 3d20 766f 6c72 735b 6161     va = volrs[aa
+0000d0f0: 5d20 6966 2061 613e 3d30 2065 6c73 6520  ] if aa>=0 else 
+0000d100: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+0000d110: 2020 2020 2020 2076 6220 3d20 766f 6c72         vb = volr
+0000d120: 735b 6262 5d20 6966 2062 623c 6269 6e63  s[bb] if bb<binc
+0000d130: 2065 6c73 6520 300d 0a20 2020 2020 2020   else 0..       
+0000d140: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d150: 7661 203e 3d20 7662 3a20 2320 4e4f 5445  va >= vb: # NOTE
+0000d160: 2062 6f74 6820 3d3d 2069 7320 616c 736f   both == is also
+0000d170: 206f 6b0d 0a20 2020 2020 2020 2020 2020   ok..           
+0000d180: 2020 2020 2020 2020 2020 2020 2061 203d               a =
+0000d190: 206d 6178 2830 2c20 6161 290d 0a20 2020   max(0, aa)..   
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2076 202b 3d20 7661 0d0a 2020       v += va..  
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 2020 6966 2076 6120 3c3d 2076 623a 2023    if va <= vb: #
+0000d1e0: 204e 4f54 4520 626f 7468 203d 3d20 6973   NOTE both == is
+0000d1f0: 2061 6c73 6f20 6f6b 0d0a 2020 2020 2020   also ok..      
+0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d210: 2020 6220 3d20 6d69 6e28 6269 6e63 2d31    b = min(binc-1
+0000d220: 2c20 6262 290d 0a20 2020 2020 2020 2020  , bb)..         
+0000d230: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000d240: 202b 3d20 7662 0d0a 2020 2020 2020 2020   += vb..        
+0000d250: 2020 2020 2020 2020 636f 6c6f 7220 3d20          color = 
+0000d260: 7067 2e6d 6b43 6f6c 6f72 2862 616e 645f  pg.mkColor(band_
+0000d270: 636f 6c6f 7229 0d0a 2020 2020 2020 2020  color)..        
+0000d280: 2020 2020 2020 2020 702e 6669 6c6c 5265          p.fillRe
+0000d290: 6374 2851 7443 6f72 652e 5152 6563 7446  ct(QtCore.QRectF
+0000d2a0: 2874 2c20 7072 6372 5b61 5d2c 2066 2c20  (t, prcr[a], f, 
+0000d2b0: 7072 6372 5b62 5d2d 7072 6372 5b61 5d2b  prcr[b]-prcr[a]+
+0000d2c0: 6829 2c20 636f 6c6f 7229 0d0a 0d0a 2020  h), color)....  
+0000d2d0: 2020 2020 2020 2020 2020 2320 6472 6177            # draw
+0000d2e0: 2068 6f72 697a 6f6e 7461 6c20 6261 7273   horizontal bars
+0000d2f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000d300: 2064 7261 775f 626f 6479 3a0d 0a20 2020   draw_body:..   
+0000d310: 2020 2020 2020 2020 2020 2020 2068 3020               h0 
+0000d320: 3d20 6820 2a20 2831 2d73 656c 662e 6361  = h * (1-self.ca
+0000d330: 6e64 6c65 5f77 6964 7468 292f 320d 0a20  ndle_width)/2.. 
+0000d340: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000d350: 3120 3d20 6820 2a20 7365 6c66 2e63 616e  1 = h * self.can
+0000d360: 646c 655f 7769 6474 680d 0a20 2020 2020  dle_width..     
+0000d370: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
+0000d380: 6861 646f 772c 6672 616d 652c 626f 6479  hadow,frame,body
+0000d390: 2c64 6174 6120 696e 2073 656c 662e 636f  ,data in self.co
+0000d3a0: 6c6f 7266 756e 6328 7365 6c66 2c20 7365  lorfunc(self, se
+0000d3b0: 6c66 2e64 6174 6173 7263 2c20 6e70 2e61  lf.datasrc, np.a
+0000d3c0: 7272 6179 285b 7072 6372 2c20 766f 6c72  rray([prcr, volr
+0000d3d0: 5d29 293a 0d0a 2020 2020 2020 2020 2020  ])):..          
+0000d3e0: 2020 2020 2020 2020 2020 702e 7365 7450            p.setP
+0000d3f0: 656e 2870 672e 6d6b 5065 6e28 6672 616d  en(pg.mkPen(fram
+0000d400: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+0000d410: 2020 2020 2020 2020 2070 2e73 6574 4272           p.setBr
+0000d420: 7573 6828 7067 2e6d 6b42 7275 7368 2862  ush(pg.mkBrush(b
+0000d430: 6f64 7929 290d 0a20 2020 2020 2020 2020  ody))..         
+0000d440: 2020 2020 2020 2020 2020 2070 7263 725f             prcr_
+0000d450: 2c76 6f6c 725f 203d 2064 6174 610d 0a20  ,volr_ = data.. 
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 2020 2066 6f72 2077 2c79 2069 6e20 7a69     for w,y in zi
+0000d480: 7028 766f 6c72 5f2c 2070 7263 725f 293a  p(volr_, prcr_):
+0000d490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d4a0: 2020 2020 2020 2020 2020 6966 2061 6273            if abs
+0000d4b0: 2877 2920 3e20 3165 2d31 353a 0d0a 2020  (w) > 1e-15:..  
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 2020 2020 2020 2020 2020 702e 6472 6177            p.draw
+0000d4e0: 5265 6374 2851 7443 6f72 652e 5152 6563  Rect(QtCore.QRec
+0000d4f0: 7446 2874 2c20 792b 6830 2c20 772a 6472  tF(t, y+h0, w*dr
+0000d500: 6177 5f62 6f64 792c 2068 3129 290d 0a0d  aw_body, h1))...
+0000d510: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
+0000d520: 7261 7720 706f 6320 6c69 6e65 0d0a 2020  raw poc line..  
+0000d530: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000d540: 662e 6472 6177 5f70 6f63 3a0d 0a20 2020  f.draw_poc:..   
+0000d550: 2020 2020 2020 2020 2020 2020 2079 203d               y =
+0000d560: 2070 7263 725b 706f 6369 6478 5d20 2b20   prcr[pocidx] + 
+0000d570: 6820 2f20 320d 0a20 2020 2020 2020 2020  h / 2..         
+0000d580: 2020 2020 2020 2070 2e73 6574 5065 6e28         p.setPen(
+0000d590: 7067 2e6d 6b50 656e 2870 6f63 5f63 6f6c  pg.mkPen(poc_col
+0000d5a0: 6f72 2929 0d0a 2020 2020 2020 2020 2020  or))..          
+0000d5b0: 2020 2020 2020 702e 6472 6177 4c69 6e65        p.drawLine
+0000d5c0: 2851 7443 6f72 652e 5150 6f69 6e74 4628  (QtCore.QPointF(
+0000d5d0: 742c 2079 292c 2051 7443 6f72 652e 5150  t, y), QtCore.QP
+0000d5e0: 6f69 6e74 4628 742b 662a 7365 6c66 2e64  ointF(t+f*self.d
+0000d5f0: 7261 775f 706f 632c 2079 2929 0d0a 0d0a  raw_poc, y))....
+0000d600: 0d0a 0d0a 636c 6173 7320 5363 6174 7465  ....class Scatte
+0000d610: 724c 6162 656c 4974 656d 2846 696e 506c  rLabelItem(FinPl
+0000d620: 6f74 4974 656d 293a 0d0a 2020 2020 6465  otItem):..    de
+0000d630: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0000d640: 2061 782c 2064 6174 6173 7263 2c20 636f   ax, datasrc, co
+0000d650: 6c6f 722c 2061 6e63 686f 7229 3a0d 0a20  lor, anchor):.. 
+0000d660: 2020 2020 2020 2073 656c 662e 636f 6c6f         self.colo
+0000d670: 7220 3d20 636f 6c6f 720d 0a20 2020 2020  r = color..     
+0000d680: 2020 2073 656c 662e 7465 7874 5f69 7465     self.text_ite
+0000d690: 6d73 203d 207b 7d0d 0a20 2020 2020 2020  ms = {}..       
+0000d6a0: 2073 656c 662e 616e 6368 6f72 203d 2061   self.anchor = a
+0000d6b0: 6e63 686f 720d 0a20 2020 2020 2020 2073  nchor..        s
+0000d6c0: 656c 662e 7368 6f77 203d 2046 616c 7365  elf.show = False
+0000d6d0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+0000d6e0: 292e 5f5f 696e 6974 5f5f 2861 782c 2064  ).__init__(ax, d
+0000d6f0: 6174 6173 7263 2c20 6c6f 643d 5472 7565  atasrc, lod=True
+0000d700: 290d 0a0d 0a20 2020 2064 6566 2067 656e  )....    def gen
+0000d710: 6572 6174 655f 7069 6374 7572 6528 7365  erate_picture(se
+0000d720: 6c66 2c20 626f 756e 6469 6e67 5f72 6563  lf, bounding_rec
+0000d730: 7429 3a0d 0a20 2020 2020 2020 2072 6f77  t):..        row
+0000d740: 7320 3d20 7365 6c66 2e67 6574 726f 7773  s = self.getrows
+0000d750: 2862 6f75 6e64 696e 675f 7265 6374 290d  (bounding_rect).
+0000d760: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0000d770: 726f 7773 2920 3e20 6c6f 645f 6c61 6265  rows) > lod_labe
+0000d780: 6c73 3a20 2320 646f 6e27 7420 6576 656e  ls: # don't even
+0000d790: 2067 656e 6572 6174 6520 7768 656e 2074   generate when t
+0000d7a0: 6865 7265 2773 2074 6f6f 206d 616e 7920  here's too many 
+0000d7b0: 6f66 2074 6865 6d0d 0a20 2020 2020 2020  of them..       
+0000d7c0: 2020 2020 2073 656c 662e 636c 6561 725f       self.clear_
+0000d7d0: 6974 656d 7328 6c69 7374 2873 656c 662e  items(list(self.
+0000d7e0: 7465 7874 5f69 7465 6d73 2e6b 6579 7328  text_items.keys(
+0000d7f0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000d800: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
+0000d810: 2064 726f 7073 203d 2073 6574 2873 656c   drops = set(sel
+0000d820: 662e 7465 7874 5f69 7465 6d73 2e6b 6579  f.text_items.key
+0000d830: 7328 2929 0d0a 2020 2020 2020 2020 6372  s())..        cr
+0000d840: 6561 7465 6420 3d20 300d 0a20 2020 2020  eated = 0..     
+0000d850: 2020 2066 6f72 2078 2c74 2c79 2c74 7874     for x,t,y,txt
+0000d860: 2069 6e20 726f 7773 3a0d 0a20 2020 2020   in rows:..     
+0000d870: 2020 2020 2020 2074 7874 203d 2073 7472         txt = str
+0000d880: 2874 7874 290d 0a20 2020 2020 2020 2020  (txt)..         
+0000d890: 2020 2069 7368 746d 6c20 3d20 273c 2720     ishtml = '<' 
+0000d8a0: 696e 2074 7874 2061 6e64 2027 3e27 2069  in txt and '>' i
+0000d8b0: 6e20 7478 740d 0a20 2020 2020 2020 2020  n txt..         
+0000d8c0: 2020 206b 6579 203d 2027 2573 3a25 2e38     key = '%s:%.8
+0000d8d0: 6627 2025 2028 742c 2079 290d 0a20 2020  f' % (t, y)..   
+0000d8e0: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
+0000d8f0: 696e 2073 656c 662e 7465 7874 5f69 7465  in self.text_ite
+0000d900: 6d73 3a0d 0a20 2020 2020 2020 2020 2020  ms:..           
+0000d910: 2020 2020 2069 7465 6d20 3d20 7365 6c66       item = self
+0000d920: 2e74 6578 745f 6974 656d 735b 6b65 795d  .text_items[key]
+0000d930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d940: 2020 2869 7465 6d2e 7365 7448 746d 6c20    (item.setHtml 
+0000d950: 6966 2069 7368 746d 6c20 656c 7365 2069  if ishtml else i
+0000d960: 7465 6d2e 7365 7454 6578 7429 2874 7874  tem.setText)(txt
+0000d970: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000d980: 2020 2069 7465 6d2e 7365 7450 6f73 2878     item.setPos(x
+0000d990: 2c20 7929 0d0a 2020 2020 2020 2020 2020  , y)..          
+0000d9a0: 2020 2020 2020 6472 6f70 732e 7265 6d6f        drops.remo
+0000d9b0: 7665 286b 6579 290d 0a20 2020 2020 2020  ve(key)..       
+0000d9c0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000d9d0: 2020 2020 2020 2020 2020 2020 6b77 7320              kws 
+0000d9e0: 3d20 7b27 6874 6d6c 273a 7478 747d 2069  = {'html':txt} i
+0000d9f0: 6620 6973 6874 6d6c 2065 6c73 6520 7b27  f ishtml else {'
+0000da00: 7465 7874 273a 7478 747d 0d0a 2020 2020  text':txt}..    
+0000da10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000da20: 2e74 6578 745f 6974 656d 735b 6b65 795d  .text_items[key]
+0000da30: 203d 2069 7465 6d20 3d20 7067 2e54 6578   = item = pg.Tex
+0000da40: 7449 7465 6d28 636f 6c6f 723d 7365 6c66  tItem(color=self
+0000da50: 2e63 6f6c 6f72 2c20 616e 6368 6f72 3d73  .color, anchor=s
+0000da60: 656c 662e 616e 6368 6f72 2c20 2a2a 6b77  elf.anchor, **kw
+0000da70: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+0000da80: 2020 2020 6974 656d 2e73 6574 506f 7328      item.setPos(
+0000da90: 782c 2079 290d 0a20 2020 2020 2020 2020  x, y)..         
+0000daa0: 2020 2020 2020 2069 7465 6d2e 7365 7450         item.setP
+0000dab0: 6172 656e 7449 7465 6d28 7365 6c66 290d  arentItem(self).
+0000dac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dad0: 2063 7265 6174 6564 202b 3d20 310d 0a20   created += 1.. 
+0000dae0: 2020 2020 2020 2069 6620 6372 6561 7465         if create
+0000daf0: 6420 3e20 3020 6f72 2073 656c 662e 6469  d > 0 or self.di
+0000db00: 7274 793a 2023 206f 6e6c 7920 7265 6475  rty: # only redu
+0000db10: 6365 2063 6163 6865 2069 6620 7765 2776  ce cache if we'v
+0000db20: 6520 6164 6465 6420 736f 6d65 206e 6577  e added some new
+0000db30: 206f 7220 7570 6461 7465 640d 0a20 2020   or updated..   
+0000db40: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+0000db50: 6561 725f 6974 656d 7328 6472 6f70 7329  ear_items(drops)
+0000db60: 0d0a 0d0a 2020 2020 6465 6620 636c 6561  ....    def clea
+0000db70: 725f 6974 656d 7328 7365 6c66 2c20 6472  r_items(self, dr
+0000db80: 6f70 5f6b 6579 7329 3a0d 0a20 2020 2020  op_keys):..     
+0000db90: 2020 2066 6f72 206b 6579 2069 6e20 6472     for key in dr
+0000dba0: 6f70 5f6b 6579 733a 0d0a 2020 2020 2020  op_keys:..      
+0000dbb0: 2020 2020 2020 6974 656d 203d 2073 656c        item = sel
+0000dbc0: 662e 7465 7874 5f69 7465 6d73 5b6b 6579  f.text_items[key
+0000dbd0: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
+0000dbe0: 7465 6d2e 7363 656e 6528 292e 7265 6d6f  tem.scene().remo
+0000dbf0: 7665 4974 656d 2869 7465 6d29 0d0a 2020  veItem(item)..  
+0000dc00: 2020 2020 2020 2020 2020 6465 6c20 7365            del se
+0000dc10: 6c66 2e74 6578 745f 6974 656d 735b 6b65  lf.text_items[ke
+0000dc20: 795d 0d0a 0d0a 2020 2020 6465 6620 6765  y]....    def ge
+0000dc30: 7472 6f77 7328 7365 6c66 2c20 626f 756e  trows(self, boun
+0000dc40: 6469 6e67 5f72 6563 7429 3a0d 0a20 2020  ding_rect):..   
+0000dc50: 2020 2020 206c 6566 742c 7269 6768 7420       left,right 
+0000dc60: 3d20 626f 756e 6469 6e67 5f72 6563 742e  = bounding_rect.
+0000dc70: 6c65 6674 2829 2c20 626f 756e 6469 6e67  left(), bounding
+0000dc80: 5f72 6563 742e 7269 6768 7428 290d 0a20  _rect.right().. 
+0000dc90: 2020 2020 2020 2064 662c 5f20 3d20 7365         df,_ = se
+0000dca0: 6c66 2e64 6174 6173 7263 2e72 6f77 7328  lf.datasrc.rows(
+0000dcb0: 332c 206c 6566 742c 2072 6967 6874 2c20  3, left, right, 
+0000dcc0: 7973 6361 6c65 3d73 656c 662e 6178 2e76  yscale=self.ax.v
+0000dcd0: 622e 7973 6361 6c65 2c20 6c6f 643d 4661  b.yscale, lod=Fa
+0000dce0: 6c73 6529 0d0a 2020 2020 2020 2020 726f  lse)..        ro
+0000dcf0: 7773 203d 2064 662e 6472 6f70 6e61 2829  ws = df.dropna()
+0000dd00: 0d0a 2020 2020 2020 2020 6964 7873 203d  ..        idxs =
+0000dd10: 2072 6f77 732e 696e 6465 780d 0a20 2020   rows.index..   
+0000dd20: 2020 2020 2072 6f77 7320 3d20 726f 7773       rows = rows
+0000dd30: 2e76 616c 7565 730d 0a20 2020 2020 2020  .values..       
+0000dd40: 2072 6f77 7320 3d20 5b28 692c 742c 792c   rows = [(i,t,y,
+0000dd50: 7478 7429 2066 6f72 2069 2c28 742c 792c  txt) for i,(t,y,
+0000dd60: 7478 7429 2069 6e20 7a69 7028 6964 7873  txt) in zip(idxs
+0000dd70: 2c20 726f 7773 2920 6966 2074 7874 5d0d  , rows) if txt].
+0000dd80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000dd90: 726f 7773 0d0a 0d0a 2020 2020 6465 6620  rows....    def 
+0000dda0: 626f 756e 6469 6e67 5265 6374 2873 656c  boundingRect(sel
+0000ddb0: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
+0000ddc0: 7572 6e20 7365 6c66 2e76 6965 7752 6563  urn self.viewRec
+0000ddd0: 7428 290d 0a0d 0a0d 0a64 6566 2063 7265  t()......def cre
+0000dde0: 6174 655f 706c 6f74 2874 6974 6c65 3d27  ate_plot(title='
+0000ddf0: 4669 6e61 6e63 6520 506c 6f74 272c 2072  Finance Plot', r
+0000de00: 6f77 733d 312c 2069 6e69 745f 7a6f 6f6d  ows=1, init_zoom
+0000de10: 5f70 6572 696f 6473 3d31 6531 302c 206d  _periods=1e10, m
+0000de20: 6178 696d 697a 653d 5472 7565 2c20 7973  aximize=True, ys
+0000de30: 6361 6c65 3d27 6c69 6e65 6172 2729 3a0d  cale='linear'):.
+0000de40: 0a20 2020 2070 672e 7365 7443 6f6e 6669  .    pg.setConfi
+0000de50: 674f 7074 696f 6e73 2866 6f72 6567 726f  gOptions(foregro
+0000de60: 756e 643d 666f 7265 6772 6f75 6e64 2c20  und=foreground, 
+0000de70: 6261 636b 6772 6f75 6e64 3d62 6163 6b67  background=backg
+0000de80: 726f 756e 6429 0d0a 2020 2020 7769 6e20  round)..    win 
+0000de90: 3d20 4669 6e57 696e 646f 7728 7469 746c  = FinWindow(titl
+0000dea0: 6529 0d0a 2020 2020 2320 6e6f 726d 616c  e)..    # normal
+0000deb0: 6c79 2066 6972 7374 2067 7261 7068 2069  ly first graph i
+0000dec0: 7320 6f66 2068 6967 6865 7220 7369 676e  s of higher sign
+0000ded0: 6966 6963 616e 6365 2c20 736f 2065 6e6c  ificance, so enl
+0000dee0: 6172 6765 0d0a 2020 2020 7769 6e2e 6369  arge..    win.ci
+0000def0: 2e6c 6179 6f75 742e 7365 7452 6f77 5374  .layout.setRowSt
+0000df00: 7265 7463 6846 6163 746f 7228 302c 2074  retchFactor(0, t
+0000df10: 6f70 5f67 7261 7068 5f73 6361 6c65 290d  op_graph_scale).
+0000df20: 0a20 2020 2077 696e 2e73 686f 775f 6d61  .    win.show_ma
+0000df30: 7869 6d69 7a65 6420 3d20 6d61 7869 6d69  ximized = maximi
+0000df40: 7a65 0d0a 2020 2020 6178 3020 3d20 6178  ze..    ax0 = ax
+0000df50: 7320 3d20 6372 6561 7465 5f70 6c6f 745f  s = create_plot_
+0000df60: 7769 6467 6574 286d 6173 7465 723d 7769  widget(master=wi
+0000df70: 6e2c 2072 6f77 733d 726f 7773 2c20 696e  n, rows=rows, in
+0000df80: 6974 5f7a 6f6f 6d5f 7065 7269 6f64 733d  it_zoom_periods=
+0000df90: 696e 6974 5f7a 6f6f 6d5f 7065 7269 6f64  init_zoom_period
+0000dfa0: 732c 2079 7363 616c 653d 7973 6361 6c65  s, yscale=yscale
+0000dfb0: 290d 0a20 2020 2061 7873 203d 2061 7873  )..    axs = axs
+0000dfc0: 2069 6620 7479 7065 2861 7873 2920 696e   if type(axs) in
+0000dfd0: 2028 7475 706c 652c 6c69 7374 2920 656c   (tuple,list) el
+0000dfe0: 7365 205b 6178 735d 0d0a 2020 2020 666f  se [axs]..    fo
+0000dff0: 7220 6178 2069 6e20 6178 733a 0d0a 2020  r ax in axs:..  
+0000e000: 2020 2020 2020 7769 6e2e 6164 6449 7465        win.addIte
+0000e010: 6d28 6178 2c20 636f 6c3d 3129 0d0a 2020  m(ax, col=1)..  
+0000e020: 2020 2020 2020 7769 6e2e 6e65 7874 526f        win.nextRo
+0000e030: 7728 290d 0a20 2020 2072 6574 7572 6e20  w()..    return 
+0000e040: 6178 300d 0a0d 0a0d 0a64 6566 2063 7265  ax0......def cre
+0000e050: 6174 655f 706c 6f74 5f77 6964 6765 7428  ate_plot_widget(
+0000e060: 6d61 7374 6572 2c20 726f 7773 3d31 2c20  master, rows=1, 
+0000e070: 696e 6974 5f7a 6f6f 6d5f 7065 7269 6f64  init_zoom_period
+0000e080: 733d 3165 3130 2c20 7973 6361 6c65 3d27  s=1e10, yscale='
+0000e090: 6c69 6e65 6172 2729 3a0d 0a20 2020 2070  linear'):..    p
+0000e0a0: 672e 7365 7443 6f6e 6669 674f 7074 696f  g.setConfigOptio
+0000e0b0: 6e73 2866 6f72 6567 726f 756e 643d 666f  ns(foreground=fo
+0000e0c0: 7265 6772 6f75 6e64 2c20 6261 636b 6772  reground, backgr
+0000e0d0: 6f75 6e64 3d62 6163 6b67 726f 756e 6429  ound=background)
+0000e0e0: 0d0a 2020 2020 676c 6f62 616c 206c 6173  ..    global las
+0000e0f0: 745f 6178 0d0a 2020 2020 6966 206d 6173  t_ax..    if mas
+0000e100: 7465 7220 6e6f 7420 696e 2077 696e 646f  ter not in windo
+0000e110: 7773 3a0d 0a20 2020 2020 2020 2077 696e  ws:..        win
+0000e120: 646f 7773 2e61 7070 656e 6428 6d61 7374  dows.append(mast
+0000e130: 6572 290d 0a20 2020 2061 7873 203d 205b  er)..    axs = [
+0000e140: 5d0d 0a20 2020 2070 7265 765f 6178 203d  ]..    prev_ax =
+0000e150: 204e 6f6e 650d 0a20 2020 2066 6f72 206e   None..    for n
+0000e160: 2069 6e20 7261 6e67 6528 726f 7773 293a   in range(rows):
+0000e170: 0d0a 2020 2020 2020 2020 7973 6320 3d20  ..        ysc = 
+0000e180: 7973 6361 6c65 5b6e 5d20 6966 2074 7970  yscale[n] if typ
+0000e190: 6528 7973 6361 6c65 2920 696e 2028 6c69  e(yscale) in (li
+0000e1a0: 7374 2c74 7570 6c65 2920 656c 7365 2079  st,tuple) else y
+0000e1b0: 7363 616c 650d 0a20 2020 2020 2020 2079  scale..        y
+0000e1c0: 7363 203d 2059 5363 616c 6528 7973 632c  sc = YScale(ysc,
+0000e1d0: 2031 290d 0a20 2020 2020 2020 2076 6965   1)..        vie
+0000e1e0: 7762 6f78 203d 2046 696e 5669 6577 426f  wbox = FinViewBo
+0000e1f0: 7828 6d61 7374 6572 2c20 696e 6974 5f73  x(master, init_s
+0000e200: 7465 7073 3d69 6e69 745f 7a6f 6f6d 5f70  teps=init_zoom_p
+0000e210: 6572 696f 6473 2c20 7973 6361 6c65 3d79  eriods, yscale=y
+0000e220: 7363 2c20 765f 7a6f 6f6d 5f73 6361 6c65  sc, v_zoom_scale
+0000e230: 3d31 2d79 5f70 6164 2c20 656e 6162 6c65  =1-y_pad, enable
+0000e240: 4d65 6e75 3d46 616c 7365 290d 0a20 2020  Menu=False)..   
+0000e250: 2020 2020 2061 7820 3d20 7072 6576 5f61       ax = prev_a
+0000e260: 7820 3d20 5f61 6464 5f74 696d 6573 7461  x = _add_timesta
+0000e270: 6d70 5f70 6c6f 7428 6d61 7374 6572 3d6d  mp_plot(master=m
+0000e280: 6173 7465 722c 2070 7265 765f 6178 3d70  aster, prev_ax=p
+0000e290: 7265 765f 6178 2c20 7669 6577 626f 783d  rev_ax, viewbox=
+0000e2a0: 7669 6577 626f 782c 2069 6e64 6578 3d6e  viewbox, index=n
+0000e2b0: 2c20 7973 6361 6c65 3d79 7363 290d 0a20  , yscale=ysc).. 
+0000e2c0: 2020 2020 2020 2069 6620 6178 733a 0d0a         if axs:..
+0000e2d0: 2020 2020 2020 2020 2020 2020 6178 2e73              ax.s
+0000e2e0: 6574 584c 696e 6b28 6178 735b 305d 2e76  etXLink(axs[0].v
+0000e2f0: 6229 0d0a 2020 2020 2020 2020 656c 7365  b)..        else
+0000e300: 3a0d 0a20 2020 2020 2020 2020 2020 2076  :..            v
+0000e310: 6965 7762 6f78 2e73 6574 466f 6375 7328  iewbox.setFocus(
+0000e320: 290d 0a20 2020 2020 2020 2061 7873 202b  )..        axs +
+0000e330: 3d20 5b61 785d 0d0a 2020 2020 6966 206d  = [ax]..    if m
+0000e340: 6173 7465 7220 6e6f 7420 696e 206d 6173  aster not in mas
+0000e350: 7465 725f 6461 7461 3a0d 0a20 2020 2020  ter_data:..     
+0000e360: 2020 206d 6173 7465 725f 6461 7461 5b6d     master_data[m
+0000e370: 6173 7465 725d 203d 207b 7d0d 0a20 2020  aster] = {}..   
+0000e380: 2069 6620 6973 696e 7374 616e 6365 286d   if isinstance(m
+0000e390: 6173 7465 722c 2070 672e 4772 6170 6869  aster, pg.Graphi
+0000e3a0: 6373 4c61 796f 7574 5769 6467 6574 293a  csLayoutWidget):
+0000e3b0: 0d0a 2020 2020 2020 2020 7072 6f78 7920  ..        proxy 
+0000e3c0: 3d20 7067 2e53 6967 6e61 6c50 726f 7879  = pg.SignalProxy
+0000e3d0: 286d 6173 7465 722e 7363 656e 6528 292e  (master.scene().
+0000e3e0: 7369 674d 6f75 7365 4d6f 7665 642c 2072  sigMouseMoved, r
+0000e3f0: 6174 654c 696d 6974 3d31 3434 2c20 736c  ateLimit=144, sl
+0000e400: 6f74 3d70 6172 7469 616c 285f 6d6f 7573  ot=partial(_mous
+0000e410: 655f 6d6f 7665 642c 206d 6173 7465 722c  e_moved, master,
+0000e420: 2061 7873 5b30 5d2e 7662 2929 0d0a 2020   axs[0].vb))..  
+0000e430: 2020 2020 2020 6d61 7374 6572 5f64 6174        master_dat
+0000e440: 615b 6d61 7374 6572 5d5b 6178 735b 305d  a[master][axs[0]
+0000e450: 2e76 625d 203d 2064 6963 7428 7072 6f78  .vb] = dict(prox
+0000e460: 796d 6d3d 7072 6f78 792c 206c 6173 745f  ymm=proxy, last_
+0000e470: 6d6f 7573 655f 6576 733d 4e6f 6e65 2c20  mouse_evs=None, 
+0000e480: 6c61 7374 5f6d 6f75 7365 5f79 3d30 290d  last_mouse_y=0).
+0000e490: 0a20 2020 2020 2020 2069 6620 2764 6566  .        if 'def
+0000e4a0: 6175 6c74 2720 6e6f 7420 696e 206d 6173  ault' not in mas
+0000e4b0: 7465 725f 6461 7461 5b6d 6173 7465 725d  ter_data[master]
+0000e4c0: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
+0000e4d0: 6173 7465 725f 6461 7461 5b6d 6173 7465  aster_data[maste
+0000e4e0: 725d 5b27 6465 6661 756c 7427 5d20 3d20  r]['default'] = 
+0000e4f0: 6d61 7374 6572 5f64 6174 615b 6d61 7374  master_data[mast
+0000e500: 6572 5d5b 6178 735b 305d 2e76 625d 0d0a  er][axs[0].vb]..
+0000e510: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000e520: 2020 2066 6f72 2061 7820 696e 2061 7873     for ax in axs
+0000e530: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+0000e540: 726f 7879 203d 2070 672e 5369 676e 616c  roxy = pg.Signal
+0000e550: 5072 6f78 7928 6178 2e61 785f 7769 6467  Proxy(ax.ax_widg
+0000e560: 6574 2e73 6365 6e65 2829 2e73 6967 4d6f  et.scene().sigMo
+0000e570: 7573 654d 6f76 6564 2c20 7261 7465 4c69  useMoved, rateLi
+0000e580: 6d69 743d 3134 342c 2073 6c6f 743d 7061  mit=144, slot=pa
+0000e590: 7274 6961 6c28 5f6d 6f75 7365 5f6d 6f76  rtial(_mouse_mov
+0000e5a0: 6564 2c20 6d61 7374 6572 2c20 6178 2e76  ed, master, ax.v
+0000e5b0: 6229 290d 0a20 2020 2020 2020 2020 2020  b))..           
+0000e5c0: 206d 6173 7465 725f 6461 7461 5b6d 6173   master_data[mas
+0000e5d0: 7465 725d 5b61 782e 7662 5d20 3d20 6469  ter][ax.vb] = di
+0000e5e0: 6374 2870 726f 7879 6d6d 3d70 726f 7879  ct(proxymm=proxy
+0000e5f0: 2c20 6c61 7374 5f6d 6f75 7365 5f65 7673  , last_mouse_evs
+0000e600: 3d4e 6f6e 652c 206c 6173 745f 6d6f 7573  =None, last_mous
+0000e610: 655f 793d 3029 0d0a 2020 2020 6c61 7374  e_y=0)..    last
+0000e620: 5f61 7820 3d20 6178 735b 305d 0d0a 2020  _ax = axs[0]..  
+0000e630: 2020 7265 7475 726e 2061 7873 5b30 5d20    return axs[0] 
+0000e640: 6966 206c 656e 2861 7873 2920 3d3d 2031  if len(axs) == 1
+0000e650: 2065 6c73 6520 6178 730d 0a0d 0a0d 0a64   else axs......d
+0000e660: 6566 2063 6c6f 7365 2829 3a0d 0a20 2020  ef close():..   
+0000e670: 2066 6f72 2077 696e 2069 6e20 7769 6e64   for win in wind
+0000e680: 6f77 733a 0d0a 2020 2020 2020 2020 7472  ows:..        tr
+0000e690: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000e6a0: 7769 6e2e 636c 6f73 6528 290d 0a20 2020  win.close()..   
+0000e6b0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0000e6c0: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+0000e6d0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0000e6e0: 5769 6e64 6f77 2063 6c6f 7369 6e67 2065  Window closing e
+0000e6f0: 7272 6f72 3a27 2c20 7479 7065 2865 292c  rror:', type(e),
+0000e700: 2065 290d 0a20 2020 2067 6c6f 6261 6c20   e)..    global 
+0000e710: 6c61 7374 5f61 780d 0a20 2020 2077 696e  last_ax..    win
+0000e720: 646f 7773 2e63 6c65 6172 2829 0d0a 2020  dows.clear()..  
+0000e730: 2020 6f76 6572 6c61 795f 6178 732e 636c    overlay_axs.cl
+0000e740: 6561 7228 290d 0a20 2020 205f 636c 6561  ear()..    _clea
+0000e750: 725f 7469 6d65 7273 2829 0d0a 2020 2020  r_timers()..    
+0000e760: 736f 756e 6473 2e63 6c65 6172 2829 0d0a  sounds.clear()..
+0000e770: 2020 2020 6d61 7374 6572 5f64 6174 612e      master_data.
+0000e780: 636c 6561 7228 290d 0a20 2020 206c 6173  clear()..    las
+0000e790: 745f 6178 203d 204e 6f6e 650d 0a0d 0a0d  t_ax = None.....
+0000e7a0: 0a64 6566 2070 7269 6365 5f63 6f6c 6f72  .def price_color
+0000e7b0: 6669 6c74 6572 2869 7465 6d2c 2064 6174  filter(item, dat
+0000e7c0: 6173 7263 2c20 6466 293a 0d0a 2020 2020  asrc, df):..    
+0000e7d0: 6f70 656e 636f 6c20 3d20 6466 2e63 6f6c  opencol = df.col
+0000e7e0: 756d 6e73 5b31 5d0d 0a20 2020 2063 6c6f  umns[1]..    clo
+0000e7f0: 7365 636f 6c20 3d20 6466 2e63 6f6c 756d  secol = df.colum
+0000e800: 6e73 5b32 5d0d 0a20 2020 2069 735f 7570  ns[2]..    is_up
+0000e810: 203d 2064 665b 6f70 656e 636f 6c5d 203c   = df[opencol] <
+0000e820: 3d20 6466 5b63 6c6f 7365 636f 6c5d 2023  = df[closecol] #
+0000e830: 206f 7065 6e20 6c6f 7765 7220 7468 616e   open lower than
+0000e840: 2063 6c6f 7365 203d 2067 6f65 7320 7570   close = goes up
+0000e850: 0d0a 2020 2020 7969 656c 6420 6974 656d  ..    yield item
+0000e860: 2e72 6f77 636f 6c6f 7273 2827 6275 6c6c  .rowcolors('bull
+0000e870: 2729 202b 205b 6466 2e6c 6f63 5b69 735f  ') + [df.loc[is_
+0000e880: 7570 2c20 3a5d 5d0d 0a20 2020 2079 6965  up, :]]..    yie
+0000e890: 6c64 2069 7465 6d2e 726f 7763 6f6c 6f72  ld item.rowcolor
+0000e8a0: 7328 2762 6561 7227 2920 2b20 5b64 662e  s('bear') + [df.
+0000e8b0: 6c6f 635b 7e69 735f 7570 2c20 3a5d 5d0d  loc[~is_up, :]].
+0000e8c0: 0a0d 0a0d 0a64 6566 2076 6f6c 756d 655f  .....def volume_
+0000e8d0: 636f 6c6f 7266 696c 7465 7228 6974 656d  colorfilter(item
+0000e8e0: 2c20 6461 7461 7372 632c 2064 6629 3a0d  , datasrc, df):.
+0000e8f0: 0a20 2020 206f 7065 6e63 6f6c 203d 2064  .    opencol = d
+0000e900: 662e 636f 6c75 6d6e 735b 335d 0d0a 2020  f.columns[3]..  
+0000e910: 2020 636c 6f73 6563 6f6c 203d 2064 662e    closecol = df.
+0000e920: 636f 6c75 6d6e 735b 345d 0d0a 2020 2020  columns[4]..    
+0000e930: 6973 5f75 7020 3d20 6466 5b6f 7065 6e63  is_up = df[openc
+0000e940: 6f6c 5d20 3c3d 2064 665b 636c 6f73 6563  ol] <= df[closec
+0000e950: 6f6c 5d20 2320 6f70 656e 206c 6f77 6572  ol] # open lower
+0000e960: 2074 6861 6e20 636c 6f73 6520 3d20 676f   than close = go
+0000e970: 6573 2075 700d 0a20 2020 2079 6965 6c64  es up..    yield
+0000e980: 2069 7465 6d2e 726f 7763 6f6c 6f72 7328   item.rowcolors(
+0000e990: 2762 756c 6c27 2920 2b20 5b64 662e 6c6f  'bull') + [df.lo
+0000e9a0: 635b 6973 5f75 702c 203a 5d5d 0d0a 2020  c[is_up, :]]..  
+0000e9b0: 2020 7969 656c 6420 6974 656d 2e72 6f77    yield item.row
+0000e9c0: 636f 6c6f 7273 2827 6265 6172 2729 202b  colors('bear') +
+0000e9d0: 205b 6466 2e6c 6f63 5b7e 6973 5f75 702c   [df.loc[~is_up,
+0000e9e0: 203a 5d5d 0d0a 0d0a 0d0a 6465 6620 7374   :]]......def st
+0000e9f0: 7265 6e67 7468 5f63 6f6c 6f72 6669 6c74  rength_colorfilt
+0000ea00: 6572 2869 7465 6d2c 2064 6174 6173 7263  er(item, datasrc
+0000ea10: 2c20 6466 293a 0d0a 2020 2020 6f70 656e  , df):..    open
+0000ea20: 636f 6c20 3d20 6466 2e63 6f6c 756d 6e73  col = df.columns
+0000ea30: 5b31 5d0d 0a20 2020 2063 6c6f 7365 636f  [1]..    closeco
+0000ea40: 6c20 3d20 6466 2e63 6f6c 756d 6e73 5b32  l = df.columns[2
+0000ea50: 5d0d 0a20 2020 2073 7461 7274 636f 6c20  ]..    startcol 
+0000ea60: 3d20 6466 2e63 6f6c 756d 6e73 5b33 5d0d  = df.columns[3].
+0000ea70: 0a20 2020 2065 6e64 636f 6c20 3d20 6466  .    endcol = df
+0000ea80: 2e63 6f6c 756d 6e73 5b34 5d0d 0a20 2020  .columns[4]..   
+0000ea90: 2069 735f 7570 203d 2064 665b 6f70 656e   is_up = df[open
+0000eaa0: 636f 6c5d 203c 3d20 6466 5b63 6c6f 7365  col] <= df[close
+0000eab0: 636f 6c5d 2023 206f 7065 6e20 6c6f 7765  col] # open lowe
+0000eac0: 7220 7468 616e 2063 6c6f 7365 203d 2067  r than close = g
+0000ead0: 6f65 7320 7570 0d0a 2020 2020 6973 5f73  oes up..    is_s
+0000eae0: 7472 6f6e 6720 3d20 6466 5b73 7461 7274  trong = df[start
+0000eaf0: 636f 6c5d 203c 3d20 6466 5b65 6e64 636f  col] <= df[endco
+0000eb00: 6c5d 0d0a 2020 2020 7969 656c 6420 6974  l]..    yield it
+0000eb10: 656d 2e72 6f77 636f 6c6f 7273 2827 6275  em.rowcolors('bu
+0000eb20: 6c6c 2729 202b 205b 6466 2e6c 6f63 5b69  ll') + [df.loc[i
+0000eb30: 735f 7570 2669 735f 7374 726f 6e67 2c20  s_up&is_strong, 
+0000eb40: 3a5d 5d0d 0a20 2020 2079 6965 6c64 2069  :]]..    yield i
+0000eb50: 7465 6d2e 726f 7763 6f6c 6f72 7328 2777  tem.rowcolors('w
+0000eb60: 6561 6b5f 6275 6c6c 2729 202b 205b 6466  eak_bull') + [df
+0000eb70: 2e6c 6f63 5b69 735f 7570 2628 7e69 735f  .loc[is_up&(~is_
+0000eb80: 7374 726f 6e67 292c 203a 5d5d 0d0a 2020  strong), :]]..  
+0000eb90: 2020 7969 656c 6420 6974 656d 2e72 6f77    yield item.row
+0000eba0: 636f 6c6f 7273 2827 7765 616b 5f62 6561  colors('weak_bea
+0000ebb0: 7227 2920 2b20 5b64 662e 6c6f 635b 287e  r') + [df.loc[(~
+0000ebc0: 6973 5f75 7029 2669 735f 7374 726f 6e67  is_up)&is_strong
+0000ebd0: 2c20 3a5d 5d0d 0a20 2020 2079 6965 6c64  , :]]..    yield
+0000ebe0: 2069 7465 6d2e 726f 7763 6f6c 6f72 7328   item.rowcolors(
+0000ebf0: 2762 6561 7227 2920 2b20 5b64 662e 6c6f  'bear') + [df.lo
+0000ec00: 635b 287e 6973 5f75 7029 2628 7e69 735f  c[(~is_up)&(~is_
+0000ec10: 7374 726f 6e67 292c 203a 5d5d 0d0a 0d0a  strong), :]]....
+0000ec20: 0d0a 6465 6620 766f 6c75 6d65 5f63 6f6c  ..def volume_col
+0000ec30: 6f72 6669 6c74 6572 5f73 6563 7469 6f6e  orfilter_section
+0000ec40: 2873 6563 7469 6f6e 733d 5b5d 293a 0d0a  (sections=[]):..
+0000ec50: 2020 2020 2727 2754 6865 2073 6563 7469      '''The secti
+0000ec60: 6f6e 7320 6172 6775 6d65 6e74 2069 7320  ons argument is 
+0000ec70: 6120 2873 7461 7274 696e 675f 696e 6465  a (starting_inde
+0000ec80: 782c 2063 6f6c 6f72 5f6e 616d 6529 2061  x, color_name) a
+0000ec90: 7272 6179 2e27 2727 0d0a 2020 2020 6465  rray.'''..    de
+0000eca0: 6620 5f63 6f6c 6f72 6669 6c74 6572 2873  f _colorfilter(s
+0000ecb0: 6563 7469 6f6e 732c 2069 7465 6d2c 2064  ections, item, d
+0000ecc0: 6174 6173 7263 2c20 6466 293a 0d0a 2020  atasrc, df):..  
+0000ecd0: 2020 2020 2020 6966 206e 6f74 2073 6563        if not sec
+0000ece0: 7469 6f6e 733a 0d0a 2020 2020 2020 2020  tions:..        
+0000ecf0: 2020 2020 7265 7475 726e 2076 6f6c 756d      return volum
+0000ed00: 655f 636f 6c6f 7266 696c 7465 7228 6974  e_colorfilter(it
+0000ed10: 656d 2c20 6461 7461 7372 632c 2064 6629  em, datasrc, df)
+0000ed20: 0d0a 2020 2020 2020 2020 666f 7220 2869  ..        for (i
+0000ed30: 302c 636f 6c6e 616d 6529 2c28 6931 2c5f  0,colname),(i1,_
+0000ed40: 2920 696e 207a 6970 2873 6563 7469 6f6e  ) in zip(section
+0000ed50: 732c 2073 6563 7469 6f6e 735b 313a 5d2b  s, sections[1:]+
+0000ed60: 5b28 4e6f 6e65 2c27 6e65 7574 7261 6c27  [(None,'neutral'
+0000ed70: 295d 293a 0d0a 2020 2020 2020 2020 2020  )]):..          
+0000ed80: 2020 726f 7773 203d 2064 662e 696c 6f63    rows = df.iloc
+0000ed90: 5b69 303a 6931 2c20 3a5d 0d0a 2020 2020  [i0:i1, :]..    
+0000eda0: 2020 2020 2020 2020 7969 656c 6420 6974          yield it
+0000edb0: 656d 2e72 6f77 636f 6c6f 7273 2863 6f6c  em.rowcolors(col
+0000edc0: 6e61 6d65 2920 2b20 5b72 6f77 735d 0d0a  name) + [rows]..
+0000edd0: 2020 2020 7265 7475 726e 2070 6172 7469      return parti
+0000ede0: 616c 285f 636f 6c6f 7266 696c 7465 722c  al(_colorfilter,
+0000edf0: 2073 6563 7469 6f6e 7329 0d0a 0d0a 0d0a   sections)......
+0000ee00: 6465 6620 686f 7269 7a76 6f6c 5f63 6f6c  def horizvol_col
+0000ee10: 6f72 6669 6c74 6572 2873 6563 7469 6f6e  orfilter(section
+0000ee20: 733d 5b5d 293a 0d0a 2020 2020 2727 2754  s=[]):..    '''T
+0000ee30: 6865 2073 6563 7469 6f6e 7320 6172 6775  he sections argu
+0000ee40: 6d65 6e74 2069 7320 6120 2873 7461 7274  ment is a (start
+0000ee50: 696e 675f 696e 6465 782c 2063 6f6c 6f72  ing_index, color
+0000ee60: 5f6e 616d 6529 2061 7272 6179 2e27 2727  _name) array.'''
+0000ee70: 0d0a 2020 2020 6465 6620 5f63 6f6c 6f72  ..    def _color
+0000ee80: 6669 6c74 6572 2873 6563 7469 6f6e 732c  filter(sections,
+0000ee90: 2069 7465 6d2c 2064 6174 6173 7263 2c20   item, datasrc, 
+0000eea0: 6461 7461 293a 0d0a 2020 2020 2020 2020  data):..        
+0000eeb0: 6966 206e 6f74 2073 6563 7469 6f6e 733a  if not sections:
+0000eec0: 0d0a 2020 2020 2020 2020 2020 2020 7969  ..            yi
+0000eed0: 656c 6420 6974 656d 2e72 6f77 636f 6c6f  eld item.rowcolo
+0000eee0: 7273 2827 6e65 7574 7261 6c27 2920 2b20  rs('neutral') + 
+0000eef0: 5b64 6174 615d 0d0a 2020 2020 2020 2020  [data]..        
+0000ef00: 666f 7220 2869 302c 636f 6c6e 616d 6529  for (i0,colname)
+0000ef10: 2c28 6931 2c5f 2920 696e 207a 6970 2873  ,(i1,_) in zip(s
+0000ef20: 6563 7469 6f6e 732c 2073 6563 7469 6f6e  ections, section
+0000ef30: 735b 313a 5d2b 5b28 4e6f 6e65 2c27 6e65  s[1:]+[(None,'ne
+0000ef40: 7574 7261 6c27 295d 293a 0d0a 2020 2020  utral')]):..    
+0000ef50: 2020 2020 2020 2020 726f 7773 203d 2064          rows = d
+0000ef60: 6174 615b 3a2c 2069 303a 6931 5d0d 0a20  ata[:, i0:i1].. 
+0000ef70: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+0000ef80: 2069 7465 6d2e 726f 7763 6f6c 6f72 7328   item.rowcolors(
+0000ef90: 636f 6c6e 616d 6529 202b 205b 726f 7773  colname) + [rows
+0000efa0: 5d0d 0a20 2020 2072 6574 7572 6e20 7061  ]..    return pa
+0000efb0: 7274 6961 6c28 5f63 6f6c 6f72 6669 6c74  rtial(_colorfilt
+0000efc0: 6572 2c20 7365 6374 696f 6e73 290d 0a0d  er, sections)...
+0000efd0: 0a0d 0a64 6566 2063 616e 646c 6573 7469  ...def candlesti
+0000efe0: 636b 5f6f 6368 6c28 6461 7461 7372 632c  ck_ochl(datasrc,
+0000eff0: 2064 7261 775f 626f 6479 3d54 7275 652c   draw_body=True,
+0000f000: 2064 7261 775f 7368 6164 6f77 3d54 7275   draw_shadow=Tru
+0000f010: 652c 2063 616e 646c 655f 7769 6474 683d  e, candle_width=
+0000f020: 302e 362c 2061 783d 4e6f 6e65 2c20 636f  0.6, ax=None, co
+0000f030: 6c6f 7266 756e 633d 7072 6963 655f 636f  lorfunc=price_co
+0000f040: 6c6f 7266 696c 7465 7229 3a0d 0a20 2020  lorfilter):..   
+0000f050: 2061 7820 3d20 5f63 7265 6174 655f 706c   ax = _create_pl
+0000f060: 6f74 2861 783d 6178 2c20 6d61 7869 6d69  ot(ax=ax, maximi
+0000f070: 7a65 3d46 616c 7365 290d 0a20 2020 2064  ze=False)..    d
+0000f080: 6174 6173 7263 203d 205f 6372 6561 7465  atasrc = _create
+0000f090: 5f64 6174 6173 7263 2861 782c 2064 6174  _datasrc(ax, dat
+0000f0a0: 6173 7263 2c20 6e63 6f6c 733d 3529 0d0a  asrc, ncols=5)..
+0000f0b0: 2020 2020 6461 7461 7372 632e 7363 616c      datasrc.scal
+0000f0c0: 655f 636f 6c73 203d 205b 332c 345d 2023  e_cols = [3,4] #
+0000f0d0: 206f 6e6c 7920 6869 2b6c 6f20 7363 616c   only hi+lo scal
+0000f0e0: 6573 0d0a 2020 2020 5f73 6574 5f64 6174  es..    _set_dat
+0000f0f0: 6173 7263 2861 782c 2064 6174 6173 7263  asrc(ax, datasrc
+0000f100: 290d 0a20 2020 2069 7465 6d20 3d20 4361  )..    item = Ca
+0000f110: 6e64 6c65 7374 6963 6b49 7465 6d28 6178  ndlestickItem(ax
+0000f120: 3d61 782c 2064 6174 6173 7263 3d64 6174  =ax, datasrc=dat
+0000f130: 6173 7263 2c20 6472 6177 5f62 6f64 793d  asrc, draw_body=
+0000f140: 6472 6177 5f62 6f64 792c 2064 7261 775f  draw_body, draw_
+0000f150: 7368 6164 6f77 3d64 7261 775f 7368 6164  shadow=draw_shad
+0000f160: 6f77 2c20 6361 6e64 6c65 5f77 6964 7468  ow, candle_width
+0000f170: 3d63 616e 646c 655f 7769 6474 682c 2063  =candle_width, c
+0000f180: 6f6c 6f72 6675 6e63 3d63 6f6c 6f72 6675  olorfunc=colorfu
+0000f190: 6e63 2c20 7265 7361 6d70 3d27 6869 6c6f  nc, resamp='hilo
+0000f1a0: 2729 0d0a 2020 2020 5f75 7064 6174 655f  ')..    _update_
+0000f1b0: 7369 676e 6966 6963 616e 7473 2861 782c  significants(ax,
+0000f1c0: 2064 6174 6173 7263 2c20 666f 7263 653d   datasrc, force=
+0000f1d0: 5472 7565 290d 0a20 2020 2069 7465 6d2e  True)..    item.
+0000f1e0: 7570 6461 7465 5f64 6174 6120 3d20 7061  update_data = pa
+0000f1f0: 7274 6961 6c28 5f75 7064 6174 655f 6461  rtial(_update_da
+0000f200: 7461 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ta, None, None, 
+0000f210: 6974 656d 290d 0a20 2020 2069 7465 6d2e  item)..    item.
+0000f220: 7570 6461 7465 5f67 6678 203d 2070 6172  update_gfx = par
+0000f230: 7469 616c 285f 7570 6461 7465 5f67 6678  tial(_update_gfx
+0000f240: 2c20 6974 656d 290d 0a20 2020 2061 782e  , item)..    ax.
+0000f250: 6164 6449 7465 6d28 6974 656d 290d 0a20  addItem(item).. 
+0000f260: 2020 2072 6574 7572 6e20 6974 656d 0d0a     return item..
+0000f270: 0d0a 0d0a 6465 6620 7265 6e6b 6f28 782c  ....def renko(x,
+0000f280: 2079 3d4e 6f6e 652c 2062 696e 733d 4e6f   y=None, bins=No
+0000f290: 6e65 2c20 7374 6570 3d4e 6f6e 652c 2061  ne, step=None, a
+0000f2a0: 783d 4e6f 6e65 2c20 636f 6c6f 7266 756e  x=None, colorfun
+0000f2b0: 633d 7072 6963 655f 636f 6c6f 7266 696c  c=price_colorfil
+0000f2c0: 7465 7229 3a0d 0a20 2020 2061 7820 3d20  ter):..    ax = 
+0000f2d0: 5f63 7265 6174 655f 706c 6f74 2861 783d  _create_plot(ax=
+0000f2e0: 6178 2c20 6d61 7869 6d69 7a65 3d46 616c  ax, maximize=Fal
+0000f2f0: 7365 290d 0a20 2020 2064 6174 6173 7263  se)..    datasrc
+0000f300: 203d 205f 6372 6561 7465 5f64 6174 6173   = _create_datas
+0000f310: 7263 2861 782c 2078 2c20 792c 206e 636f  rc(ax, x, y, nco
+0000f320: 6c73 3d33 290d 0a20 2020 206f 7269 6764  ls=3)..    origd
+0000f330: 6620 3d20 6461 7461 7372 632e 6466 0d0a  f = datasrc.df..
+0000f340: 2020 2020 6164 6a20 3d20 5f61 646a 7573      adj = _adjus
+0000f350: 745f 7265 6e6b 6f5f 6c6f 675f 6461 7461  t_renko_log_data
+0000f360: 7372 6320 6966 2061 782e 7662 2e79 7363  src if ax.vb.ysc
+0000f370: 616c 652e 7363 616c 6574 7970 6520 3d3d  ale.scaletype ==
+0000f380: 2027 6c6f 6727 2065 6c73 6520 5f61 646a   'log' else _adj
+0000f390: 7573 745f 7265 6e6b 6f5f 6461 7461 7372  ust_renko_datasr
+0000f3a0: 630d 0a20 2020 2073 7465 705f 6164 6a75  c..    step_adju
+0000f3b0: 7374 5f72 656e 6b6f 5f64 6174 6173 7263  st_renko_datasrc
+0000f3c0: 203d 2070 6172 7469 616c 2861 646a 2c20   = partial(adj, 
+0000f3d0: 6269 6e73 2c20 7374 6570 290d 0a20 2020  bins, step)..   
+0000f3e0: 2073 7465 705f 6164 6a75 7374 5f72 656e   step_adjust_ren
+0000f3f0: 6b6f 5f64 6174 6173 7263 2864 6174 6173  ko_datasrc(datas
+0000f400: 7263 290d 0a20 2020 2061 782e 6465 636f  rc)..    ax.deco
+0000f410: 7570 6c65 2829 0d0a 2020 2020 6974 656d  uple()..    item
+0000f420: 203d 2063 616e 646c 6573 7469 636b 5f6f   = candlestick_o
+0000f430: 6368 6c28 6461 7461 7372 632c 2064 7261  chl(datasrc, dra
+0000f440: 775f 7368 6164 6f77 3d46 616c 7365 2c20  w_shadow=False, 
+0000f450: 6361 6e64 6c65 5f77 6964 7468 3d31 2c20  candle_width=1, 
+0000f460: 6178 3d61 782c 2063 6f6c 6f72 6675 6e63  ax=ax, colorfunc
+0000f470: 3d63 6f6c 6f72 6675 6e63 290d 0a20 2020  =colorfunc)..   
+0000f480: 2069 7465 6d2e 636f 6c6f 7273 5b27 6275   item.colors['bu
+0000f490: 6c6c 5f62 6f64 7927 5d20 3d20 6974 656d  ll_body'] = item
+0000f4a0: 2e63 6f6c 6f72 735b 2762 756c 6c5f 6672  .colors['bull_fr
+0000f4b0: 616d 6527 5d0d 0a20 2020 2069 7465 6d2e  ame']..    item.
+0000f4c0: 7570 6461 7465 5f64 6174 6120 3d20 7061  update_data = pa
+0000f4d0: 7274 6961 6c28 5f75 7064 6174 655f 6461  rtial(_update_da
+0000f4e0: 7461 2c20 4e6f 6e65 2c20 7374 6570 5f61  ta, None, step_a
+0000f4f0: 646a 7573 745f 7265 6e6b 6f5f 6461 7461  djust_renko_data
+0000f500: 7372 632c 2069 7465 6d29 0d0a 2020 2020  src, item)..    
+0000f510: 6974 656d 2e75 7064 6174 655f 6766 7820  item.update_gfx 
+0000f520: 3d20 7061 7274 6961 6c28 5f75 7064 6174  = partial(_updat
+0000f530: 655f 6766 782c 2069 7465 6d29 0d0a 2020  e_gfx, item)..  
+0000f540: 2020 676c 6f62 616c 2065 706f 6368 5f70    global epoch_p
+0000f550: 6572 696f 640d 0a20 2020 2065 706f 6368  eriod..    epoch
+0000f560: 5f70 6572 696f 6420 3d20 286f 7269 6764  _period = (origd
+0000f570: 662e 696c 6f63 5b31 2c30 5d20 2d20 6f72  f.iloc[1,0] - or
+0000f580: 6967 6466 2e69 6c6f 635b 302c 305d 2920  igdf.iloc[0,0]) 
+0000f590: 2f2f 2069 6e74 2831 6539 290d 0a20 2020  // int(1e9)..   
+0000f5a0: 2072 6574 7572 6e20 6974 656d 0d0a 0d0a   return item....
+0000f5b0: 0d0a 6465 6620 766f 6c75 6d65 5f6f 6376  ..def volume_ocv
+0000f5c0: 2864 6174 6173 7263 2c20 6361 6e64 6c65  (datasrc, candle
+0000f5d0: 5f77 6964 7468 3d30 2e38 2c20 6178 3d4e  _width=0.8, ax=N
+0000f5e0: 6f6e 652c 2063 6f6c 6f72 6675 6e63 3d76  one, colorfunc=v
+0000f5f0: 6f6c 756d 655f 636f 6c6f 7266 696c 7465  olume_colorfilte
+0000f600: 7229 3a0d 0a20 2020 2061 7820 3d20 5f63  r):..    ax = _c
+0000f610: 7265 6174 655f 706c 6f74 2861 783d 6178  reate_plot(ax=ax
+0000f620: 2c20 6d61 7869 6d69 7a65 3d46 616c 7365  , maximize=False
+0000f630: 290d 0a20 2020 2064 6174 6173 7263 203d  )..    datasrc =
+0000f640: 205f 6372 6561 7465 5f64 6174 6173 7263   _create_datasrc
+0000f650: 2861 782c 2064 6174 6173 7263 2c20 6e63  (ax, datasrc, nc
+0000f660: 6f6c 733d 3429 0d0a 2020 2020 5f61 646a  ols=4)..    _adj
+0000f670: 7573 745f 766f 6c75 6d65 5f64 6174 6173  ust_volume_datas
+0000f680: 7263 2864 6174 6173 7263 290d 0a20 2020  rc(datasrc)..   
+0000f690: 205f 7365 745f 6461 7461 7372 6328 6178   _set_datasrc(ax
+0000f6a0: 2c20 6461 7461 7372 6329 0d0a 2020 2020  , datasrc)..    
+0000f6b0: 6974 656d 203d 2043 616e 646c 6573 7469  item = Candlesti
+0000f6c0: 636b 4974 656d 2861 783d 6178 2c20 6461  ckItem(ax=ax, da
+0000f6d0: 7461 7372 633d 6461 7461 7372 632c 2064  tasrc=datasrc, d
+0000f6e0: 7261 775f 626f 6479 3d54 7275 652c 2064  raw_body=True, d
+0000f6f0: 7261 775f 7368 6164 6f77 3d46 616c 7365  raw_shadow=False
+0000f700: 2c20 6361 6e64 6c65 5f77 6964 7468 3d63  , candle_width=c
+0000f710: 616e 646c 655f 7769 6474 682c 2063 6f6c  andle_width, col
+0000f720: 6f72 6675 6e63 3d63 6f6c 6f72 6675 6e63  orfunc=colorfunc
+0000f730: 2c20 7265 7361 6d70 3d27 7375 6d27 290d  , resamp='sum').
+0000f740: 0a20 2020 205f 7570 6461 7465 5f73 6967  .    _update_sig
+0000f750: 6e69 6669 6361 6e74 7328 6178 2c20 6461  nificants(ax, da
+0000f760: 7461 7372 632c 2066 6f72 6365 3d54 7275  tasrc, force=Tru
+0000f770: 6529 0d0a 2020 2020 6974 656d 2e63 6f6c  e)..    item.col
+0000f780: 6f72 735b 2762 756c 6c5f 626f 6479 275d  ors['bull_body']
+0000f790: 203d 2069 7465 6d2e 636f 6c6f 7273 5b27   = item.colors['
+0000f7a0: 6275 6c6c 5f66 7261 6d65 275d 0d0a 2020  bull_frame']..  
+0000f7b0: 2020 6966 2063 6f6c 6f72 6675 6e63 203d    if colorfunc =
+0000f7c0: 3d20 766f 6c75 6d65 5f63 6f6c 6f72 6669  = volume_colorfi
+0000f7d0: 6c74 6572 3a20 2320 6173 7375 6d65 206e  lter: # assume n
+0000f7e0: 6f72 6d61 6c20 766f 6c75 6d65 2070 6c6f  ormal volume plo
+0000f7f0: 740d 0a20 2020 2020 2020 2069 7465 6d2e  t..        item.
+0000f800: 636f 6c6f 7273 5b27 6275 6c6c 5f66 7261  colors['bull_fra
+0000f810: 6d65 275d 203d 2076 6f6c 756d 655f 6275  me'] = volume_bu
+0000f820: 6c6c 5f63 6f6c 6f72 0d0a 2020 2020 2020  ll_color..      
+0000f830: 2020 6974 656d 2e63 6f6c 6f72 735b 2762    item.colors['b
+0000f840: 756c 6c5f 626f 6479 275d 2020 3d20 766f  ull_body']  = vo
+0000f850: 6c75 6d65 5f62 756c 6c5f 626f 6479 5f63  lume_bull_body_c
+0000f860: 6f6c 6f72 0d0a 2020 2020 2020 2020 6974  olor..        it
+0000f870: 656d 2e63 6f6c 6f72 735b 2762 6561 725f  em.colors['bear_
+0000f880: 6672 616d 6527 5d20 3d20 766f 6c75 6d65  frame'] = volume
+0000f890: 5f62 6561 725f 636f 6c6f 720d 0a20 2020  _bear_color..   
+0000f8a0: 2020 2020 2069 7465 6d2e 636f 6c6f 7273       item.colors
+0000f8b0: 5b27 6265 6172 5f62 6f64 7927 5d20 203d  ['bear_body']  =
+0000f8c0: 2076 6f6c 756d 655f 6265 6172 5f63 6f6c   volume_bear_col
+0000f8d0: 6f72 0d0a 2020 2020 2020 2020 6178 2e76  or..        ax.v
+0000f8e0: 622e 765f 7a6f 6f6d 5f62 6173 656c 696e  b.v_zoom_baselin
+0000f8f0: 6520 3d20 300d 0a20 2020 2065 6c73 653a  e = 0..    else:
+0000f900: 0d0a 2020 2020 2020 2020 6974 656d 2e63  ..        item.c
+0000f910: 6f6c 6f72 735b 2777 6561 6b5f 6275 6c6c  olors['weak_bull
+0000f920: 5f66 7261 6d65 275d 203d 2062 7269 6768  _frame'] = brigh
+0000f930: 7465 6e28 766f 6c75 6d65 5f62 756c 6c5f  ten(volume_bull_
+0000f940: 636f 6c6f 722c 2031 2e32 290d 0a20 2020  color, 1.2)..   
+0000f950: 2020 2020 2069 7465 6d2e 636f 6c6f 7273       item.colors
+0000f960: 5b27 7765 616b 5f62 756c 6c5f 626f 6479  ['weak_bull_body
+0000f970: 275d 2020 3d20 6272 6967 6874 656e 2876  ']  = brighten(v
+0000f980: 6f6c 756d 655f 6275 6c6c 5f63 6f6c 6f72  olume_bull_color
+0000f990: 2c20 312e 3229 0d0a 2020 2020 6974 656d  , 1.2)..    item
+0000f9a0: 2e75 7064 6174 655f 6461 7461 203d 2070  .update_data = p
+0000f9b0: 6172 7469 616c 285f 7570 6461 7465 5f64  artial(_update_d
+0000f9c0: 6174 612c 204e 6f6e 652c 205f 6164 6a75  ata, None, _adju
+0000f9d0: 7374 5f76 6f6c 756d 655f 6461 7461 7372  st_volume_datasr
+0000f9e0: 632c 2069 7465 6d29 0d0a 2020 2020 6974  c, item)..    it
+0000f9f0: 656d 2e75 7064 6174 655f 6766 7820 3d20  em.update_gfx = 
+0000fa00: 7061 7274 6961 6c28 5f75 7064 6174 655f  partial(_update_
+0000fa10: 6766 782c 2069 7465 6d29 0d0a 2020 2020  gfx, item)..    
+0000fa20: 6178 2e61 6464 4974 656d 2869 7465 6d29  ax.addItem(item)
+0000fa30: 0d0a 2020 2020 6974 656d 2e73 6574 5a56  ..    item.setZV
+0000fa40: 616c 7565 282d 3230 290d 0a20 2020 2072  alue(-20)..    r
+0000fa50: 6574 7572 6e20 6974 656d 0d0a 0d0a 0d0a  eturn item......
+0000fa60: 6465 6620 686f 7269 7a5f 7469 6d65 5f76  def horiz_time_v
+0000fa70: 6f6c 756d 6528 6461 7461 7372 632c 2061  olume(datasrc, a
+0000fa80: 783d 4e6f 6e65 2c20 2a2a 6b77 6172 6773  x=None, **kwargs
+0000fa90: 293a 0d0a 2020 2020 2727 2744 7261 7773  ):..    '''Draws
+0000faa0: 206d 756c 7469 706c 6520 6669 7865 6420   multiple fixed 
+0000fab0: 686f 7269 7a6f 6e74 616c 2076 6f6c 756d  horizontal volum
+0000fac0: 6573 2e20 5468 6520 696e 7075 7420 666f  es. The input fo
+0000fad0: 726d 6174 2069 733a 0d0a 2020 2020 2020  rmat is:..      
+0000fae0: 205b 5b74 696d 6530 2c20 5b28 7072 6963   [[time0, [(pric
+0000faf0: 6530 2c76 6f6c 756d 6530 292c 2870 7269  e0,volume0),(pri
+0000fb00: 6365 312c 766f 6c75 6d65 3129 2c2e 2e2e  ce1,volume1),...
+0000fb10: 5d5d 2c20 2e2e 2e5d 0d0a 0d0a 2020 2020  ]], ...]....    
+0000fb20: 2020 2054 6869 7320 6368 6172 7420 6e65     This chart ne
+0000fb30: 6564 7320 746f 2062 6520 706c 6f74 206c  eds to be plot l
+0000fb40: 6173 742c 2073 6f20 6974 206b 6e6f 7773  ast, so it knows
+0000fb50: 2069 6620 6974 2063 6f6e 7472 6f6c 730d   if it controls.
+0000fb60: 0a20 2020 2020 2020 7768 6174 2074 696d  .       what tim
+0000fb70: 6520 7065 7269 6f64 7320 6172 6520 7368  e periods are sh
+0000fb80: 6f77 6e2c 206f 7220 6966 2069 7473 2075  own, or if its u
+0000fb90: 7369 6e67 2074 696d 6520 616c 7265 6164  sing time alread
+0000fba0: 7920 696e 0d0a 2020 2020 2020 2070 6c61  y in..       pla
+0000fbb0: 6365 2062 7920 616e 6f74 6865 7220 706c  ce by another pl
+0000fbc0: 6f74 2e27 2727 0d0a 2020 2020 2320 7570  ot.'''..    # up
+0000fbd0: 6461 7465 2068 616e 646c 696e 6720 6465  date handling de
+0000fbe0: 6661 756c 7420 6966 206e 6563 6573 7361  fault if necessa
+0000fbf0: 7279 0d0a 2020 2020 676c 6f62 616c 206d  ry..    global m
+0000fc00: 6178 5f7a 6f6f 6d5f 706f 696e 7473 2c20  ax_zoom_points, 
+0000fc10: 7269 6768 745f 6d61 7267 696e 5f63 616e  right_margin_can
+0000fc20: 646c 6573 0d0a 2020 2020 6966 206d 6178  dles..    if max
+0000fc30: 5f7a 6f6f 6d5f 706f 696e 7473 203e 2031  _zoom_points > 1
+0000fc40: 353a 0d0a 2020 2020 2020 2020 6d61 785f  5:..        max_
+0000fc50: 7a6f 6f6d 5f70 6f69 6e74 7320 3d20 340d  zoom_points = 4.
+0000fc60: 0a20 2020 2069 6620 7269 6768 745f 6d61  .    if right_ma
+0000fc70: 7267 696e 5f63 616e 646c 6573 203e 2033  rgin_candles > 3
+0000fc80: 3a0d 0a20 2020 2020 2020 2072 6967 6874  :..        right
+0000fc90: 5f6d 6172 6769 6e5f 6361 6e64 6c65 7320  _margin_candles 
+0000fca0: 3d20 310d 0a0d 0a20 2020 2061 7820 3d20  = 1....    ax = 
+0000fcb0: 5f63 7265 6174 655f 706c 6f74 2861 783d  _create_plot(ax=
+0000fcc0: 6178 2c20 6d61 7869 6d69 7a65 3d46 616c  ax, maximize=Fal
+0000fcd0: 7365 290d 0a20 2020 2064 6174 6173 7263  se)..    datasrc
+0000fce0: 203d 205f 7072 6561 646a 7573 745f 686f   = _preadjust_ho
+0000fcf0: 7269 7a5f 6461 7461 7372 6328 6461 7461  riz_datasrc(data
+0000fd00: 7372 6329 0d0a 2020 2020 6461 7461 7372  src)..    datasr
+0000fd10: 6320 3d20 5f63 7265 6174 655f 6461 7461  c = _create_data
+0000fd20: 7372 6328 6178 2c20 6461 7461 7372 6329  src(ax, datasrc)
+0000fd30: 0d0a 2020 2020 5f61 646a 7573 745f 686f  ..    _adjust_ho
+0000fd40: 7269 7a5f 6461 7461 7372 6328 6461 7461  riz_datasrc(data
+0000fd50: 7372 6329 0d0a 2020 2020 6966 2061 782e  src)..    if ax.
+0000fd60: 7662 2e64 6174 6173 7263 2069 7320 6e6f  vb.datasrc is no
+0000fd70: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000fd80: 2064 6174 6173 7263 2e73 7461 6e64 616c   datasrc.standal
+0000fd90: 6f6e 6520 3d20 5472 7565 2023 206f 6e6c  one = True # onl
+0000fda0: 7920 666f 7263 6520 7374 616e 6461 6c6f  y force standalo
+0000fdb0: 6e65 2069 6620 7468 6572 6520 6973 2073  ne if there is s
+0000fdc0: 6f6d 6574 6869 6e67 206f 6e20 6f75 7220  omething on our 
+0000fdd0: 6368 6172 7473 2061 6c72 6561 6479 0d0a  charts already..
+0000fde0: 2020 2020 6461 7461 7372 632e 7363 616c      datasrc.scal
+0000fdf0: 655f 636f 6c73 203d 205b 6461 7461 7372  e_cols = [datasr
+0000fe00: 632e 636f 6c5f 6461 7461 5f6f 6666 7365  c.col_data_offse
+0000fe10: 742c 206c 656e 2864 6174 6173 7263 2e64  t, len(datasrc.d
+0000fe20: 662e 636f 6c75 6d6e 7329 2d32 5d20 2320  f.columns)-2] # 
+0000fe30: 6669 7273 7420 616e 6420 6c61 7374 2070  first and last p
+0000fe40: 7269 6365 2063 6f6c 756d 6e73 0d0a 2020  rice columns..  
+0000fe50: 2020 6461 7461 7372 632e 7072 655f 7570    datasrc.pre_up
+0000fe60: 6461 7465 203d 206c 616d 6264 6120 6466  date = lambda df
+0000fe70: 3a20 6466 2e6c 6f63 5b3a 2c20 3a64 662e  : df.loc[:, :df.
+0000fe80: 636f 6c75 6d6e 735b 305d 5d20 2320 7468  columns[0]] # th
+0000fe90: 726f 7720 6177 6179 2070 7265 7669 6f75  row away previou
+0000fea0: 7320 6461 7461 0d0a 2020 2020 6461 7461  s data..    data
+0000feb0: 7372 632e 706f 7374 5f75 7064 6174 6520  src.post_update 
+0000fec0: 3d20 6c61 6d62 6461 2064 663a 2064 662e  = lambda df: df.
+0000fed0: 6472 6f70 6e61 2868 6f77 3d27 616c 6c27  dropna(how='all'
+0000fee0: 2920 2320 6b69 6c6c 2061 6c6c 2d4e 614e  ) # kill all-NaN
+0000fef0: 730d 0a20 2020 205f 7365 745f 6461 7461  s..    _set_data
+0000ff00: 7372 6328 6178 2c20 6461 7461 7372 6329  src(ax, datasrc)
+0000ff10: 0d0a 2020 2020 6974 656d 203d 2048 6f72  ..    item = Hor
+0000ff20: 697a 6f6e 7461 6c54 696d 6556 6f6c 756d  izontalTimeVolum
+0000ff30: 6549 7465 6d28 6178 3d61 782c 2064 6174  eItem(ax=ax, dat
+0000ff40: 6173 7263 3d64 6174 6173 7263 2c20 2a2a  asrc=datasrc, **
+0000ff50: 6b77 6172 6773 290d 0a20 2020 2069 7465  kwargs)..    ite
+0000ff60: 6d2e 7570 6461 7465 5f64 6174 6120 3d20  m.update_data = 
+0000ff70: 7061 7274 6961 6c28 5f75 7064 6174 655f  partial(_update_
+0000ff80: 6461 7461 2c20 5f70 7265 6164 6a75 7374  data, _preadjust
+0000ff90: 5f68 6f72 697a 5f64 6174 6173 7263 2c20  _horiz_datasrc, 
+0000ffa0: 5f61 646a 7573 745f 686f 7269 7a5f 6461  _adjust_horiz_da
+0000ffb0: 7461 7372 632c 2069 7465 6d29 0d0a 2020  tasrc, item)..  
+0000ffc0: 2020 6974 656d 2e75 7064 6174 655f 6766    item.update_gf
+0000ffd0: 7820 3d20 7061 7274 6961 6c28 5f75 7064  x = partial(_upd
+0000ffe0: 6174 655f 6766 782c 2069 7465 6d29 0d0a  ate_gfx, item)..
+0000fff0: 2020 2020 6974 656d 2e73 6574 5a56 616c      item.setZVal
+00010000: 7565 282d 3130 290d 0a20 2020 2061 782e  ue(-10)..    ax.
+00010010: 6164 6449 7465 6d28 6974 656d 290d 0a20  addItem(item).. 
+00010020: 2020 2072 6574 7572 6e20 6974 656d 0d0a     return item..
+00010030: 0d0a 0d0a 6465 6620 6865 6174 6d61 7028  ....def heatmap(
+00010040: 6461 7461 7372 632c 2061 783d 4e6f 6e65  datasrc, ax=None
+00010050: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+00010060: 2020 2727 2745 7870 656e 7369 7665 2066    '''Expensive f
+00010070: 756e 6374 696f 6e2e 204f 6e6c 7920 7573  unction. Only us
+00010080: 6520 6f6e 2073 6d61 6c6c 2064 6174 6120  e on small data 
+00010090: 7365 7473 2e20 5365 6520 4865 6174 6d61  sets. See Heatma
+000100a0: 7049 7465 6d20 666f 7220 6b77 6172 6773  pItem for kwargs
+000100b0: 2e20 496e 7075 7420 6461 7461 7372 630d  . Input datasrc.
+000100c0: 0a20 2020 2020 2020 6861 7320 7820 2874  .       has x (t
+000100d0: 696d 6529 2069 6e20 696e 6465 7820 6f72  ime) in index or
+000100e0: 2066 6972 7374 2063 6f6c 756d 6e2c 2079   first column, y
+000100f0: 2028 7072 6963 6529 2061 7320 636f 6c75   (price) as colu
+00010100: 6d6e 206e 616d 6573 2c20 616e 6420 696e  mn names, and in
+00010110: 7465 6e73 6974 7920 2863 6f6c 6f72 2920  tensity (color) 
+00010120: 6173 0d0a 2020 2020 2020 2063 656c 6c20  as..       cell 
+00010130: 7661 6c75 6573 2e27 2727 0d0a 2020 2020  values.'''..    
+00010140: 6178 203d 205f 6372 6561 7465 5f70 6c6f  ax = _create_plo
+00010150: 7428 6178 3d61 782c 206d 6178 696d 697a  t(ax=ax, maximiz
+00010160: 653d 4661 6c73 6529 0d0a 2020 2020 6966  e=False)..    if
+00010170: 2061 782e 7662 2e76 5f7a 6f6f 6d5f 7363   ax.vb.v_zoom_sc
+00010180: 616c 6520 3e3d 2030 2e39 3a0d 0a20 2020  ale >= 0.9:..   
+00010190: 2020 2020 2061 782e 7662 2e76 5f7a 6f6f       ax.vb.v_zoo
+000101a0: 6d5f 7363 616c 6520 3d20 302e 360d 0a20  m_scale = 0.6.. 
+000101b0: 2020 2064 6174 6173 7263 203d 205f 6372     datasrc = _cr
+000101c0: 6561 7465 5f64 6174 6173 7263 2861 782c  eate_datasrc(ax,
+000101d0: 2064 6174 6173 7263 290d 0a20 2020 2064   datasrc)..    d
+000101e0: 6174 6173 7263 2e73 6361 6c65 5f63 6f6c  atasrc.scale_col
+000101f0: 7320 3d20 5b5d 2023 2064 6f65 736e 2774  s = [] # doesn't
+00010200: 2073 6361 6c65 0d0a 2020 2020 5f73 6574   scale..    _set
+00010210: 5f64 6174 6173 7263 2861 782c 2064 6174  _datasrc(ax, dat
+00010220: 6173 7263 290d 0a20 2020 2069 7465 6d20  asrc)..    item 
+00010230: 3d20 4865 6174 6d61 7049 7465 6d28 6178  = HeatmapItem(ax
+00010240: 3d61 782c 2064 6174 6173 7263 3d64 6174  =ax, datasrc=dat
+00010250: 6173 7263 2c20 2a2a 6b77 6172 6773 290d  asrc, **kwargs).
+00010260: 0a20 2020 2069 7465 6d2e 7570 6461 7465  .    item.update
+00010270: 5f64 6174 6120 3d20 7061 7274 6961 6c28  _data = partial(
+00010280: 5f75 7064 6174 655f 6461 7461 2c20 4e6f  _update_data, No
+00010290: 6e65 2c20 4e6f 6e65 2c20 6974 656d 290d  ne, None, item).
+000102a0: 0a20 2020 2069 7465 6d2e 7570 6461 7465  .    item.update
+000102b0: 5f67 6678 203d 2070 6172 7469 616c 285f  _gfx = partial(_
+000102c0: 7570 6461 7465 5f67 6678 2c20 6974 656d  update_gfx, item
+000102d0: 290d 0a20 2020 2069 7465 6d2e 7365 745a  )..    item.setZ
+000102e0: 5661 6c75 6528 2d33 3029 0d0a 2020 2020  Value(-30)..    
+000102f0: 6178 2e61 6464 4974 656d 2869 7465 6d29  ax.addItem(item)
+00010300: 0d0a 2020 2020 6966 2061 782e 7662 2e64  ..    if ax.vb.d
+00010310: 6174 6173 7263 2069 7320 6e6f 7420 4e6f  atasrc is not No
+00010320: 6e65 2061 6e64 206e 6f74 2061 782e 7662  ne and not ax.vb
+00010330: 2e64 6174 6173 7263 2e74 696d 6562 6173  .datasrc.timebas
+00010340: 6564 2829 3a20 2320 6d61 6e75 616c 207a  ed(): # manual z
+00010350: 6f6f 6d20 7570 6461 7465 0d0a 2020 2020  oom update..    
+00010360: 2020 2020 6178 2e73 6574 584c 696e 6b28      ax.setXLink(
+00010370: 4e6f 6e65 290d 0a20 2020 2020 2020 2069  None)..        i
+00010380: 6620 6178 2e70 7265 765f 6178 3a0d 0a20  f ax.prev_ax:.. 
+00010390: 2020 2020 2020 2020 2020 2061 782e 7072             ax.pr
+000103a0: 6576 5f61 782e 7365 745f 7669 7369 626c  ev_ax.set_visibl
+000103b0: 6528 7861 7869 733d 5472 7565 290d 0a20  e(xaxis=True).. 
+000103c0: 2020 2020 2020 2064 6620 3d20 6178 2e76         df = ax.v
+000103d0: 622e 6461 7461 7372 632e 6466 0d0a 2020  b.datasrc.df..  
+000103e0: 2020 2020 2020 7072 6963 6573 203d 2064        prices = d
+000103f0: 662e 636f 6c75 6d6e 735b 6178 2e76 622e  f.columns[ax.vb.
+00010400: 6461 7461 7372 632e 636f 6c5f 6461 7461  datasrc.col_data
+00010410: 5f6f 6666 7365 743a 6974 656d 2e63 6f6c  _offset:item.col
+00010420: 5f64 6174 615f 656e 645d 0d0a 2020 2020  _data_end]..    
+00010430: 2020 2020 6465 6c74 615f 7072 6963 6520      delta_price 
+00010440: 3d20 6162 7328 7072 6963 6573 5b30 5d20  = abs(prices[0] 
+00010450: 2d20 7072 6963 6573 5b31 5d29 0d0a 2020  - prices[1])..  
+00010460: 2020 2020 2020 6178 2e76 622e 7365 745f        ax.vb.set_
+00010470: 7261 6e67 6528 302c 206d 696e 2864 662e  range(0, min(df.
+00010480: 636f 6c75 6d6e 735b 313a 5d29 2c20 6c65  columns[1:]), le
+00010490: 6e28 6466 292c 206d 6178 2864 662e 636f  n(df), max(df.co
+000104a0: 6c75 6d6e 735b 313a 5d29 2b64 656c 7461  lumns[1:])+delta
+000104b0: 5f70 7269 6365 290d 0a20 2020 2072 6574  _price)..    ret
+000104c0: 7572 6e20 6974 656d 0d0a 0d0a 0d0a 6465  urn item......de
+000104d0: 6620 6261 7228 782c 2079 3d4e 6f6e 652c  f bar(x, y=None,
+000104e0: 2077 6964 7468 3d30 2e38 2c20 6178 3d4e   width=0.8, ax=N
+000104f0: 6f6e 652c 2063 6f6c 6f72 6675 6e63 3d73  one, colorfunc=s
+00010500: 7472 656e 6774 685f 636f 6c6f 7266 696c  trength_colorfil
+00010510: 7465 722c 202a 2a6b 7761 7267 7329 3a0d  ter, **kwargs):.
+00010520: 0a20 2020 2027 2727 4261 7220 706c 6f74  .    '''Bar plot
+00010530: 7320 6172 6520 6465 636f 7570 6c65 642e  s are decoupled.
+00010540: 2055 7365 2076 6f6c 756d 655f 6f63 7628   Use volume_ocv(
+00010550: 2920 6966 2079 6f75 2077 616e 7420 6120  ) if you want a 
+00010560: 6261 7220 706c 6f74 2077 6869 6368 2072  bar plot which r
+00010570: 656c 6174 6573 2074 6f20 6f74 6865 7220  elates to other 
+00010580: 7469 6d65 2070 6c6f 7473 2e27 2727 0d0a  time plots.'''..
+00010590: 2020 2020 676c 6f62 616c 2072 6967 6874      global right
+000105a0: 5f6d 6172 6769 6e5f 6361 6e64 6c65 732c  _margin_candles,
+000105b0: 206d 6178 5f7a 6f6f 6d5f 706f 696e 7473   max_zoom_points
+000105c0: 0d0a 2020 2020 7269 6768 745f 6d61 7267  ..    right_marg
+000105d0: 696e 5f63 616e 646c 6573 203d 2030 0d0a  in_candles = 0..
+000105e0: 2020 2020 6d61 785f 7a6f 6f6d 5f70 6f69      max_zoom_poi
+000105f0: 6e74 7320 3d20 6d69 6e28 6d61 785f 7a6f  nts = min(max_zo
+00010600: 6f6d 5f70 6f69 6e74 732c 2038 290d 0a20  om_points, 8).. 
+00010610: 2020 2061 7820 3d20 5f63 7265 6174 655f     ax = _create_
+00010620: 706c 6f74 2861 783d 6178 2c20 6d61 7869  plot(ax=ax, maxi
+00010630: 6d69 7a65 3d46 616c 7365 290d 0a20 2020  mize=False)..   
+00010640: 2061 782e 6465 636f 7570 6c65 2829 0d0a   ax.decouple()..
+00010650: 2020 2020 6461 7461 7372 6320 3d20 5f63      datasrc = _c
+00010660: 7265 6174 655f 6461 7461 7372 6328 6178  reate_datasrc(ax
+00010670: 2c20 782c 2079 2c20 6e63 6f6c 733d 3129  , x, y, ncols=1)
+00010680: 0d0a 2020 2020 5f61 646a 7573 745f 6261  ..    _adjust_ba
+00010690: 725f 6461 7461 7372 6328 6461 7461 7372  r_datasrc(datasr
+000106a0: 632c 206f 7264 6572 5f63 6f6c 733d 4661  c, order_cols=Fa
+000106b0: 6c73 6529 2023 2064 6f6e 2774 2072 6561  lse) # don't rea
+000106c0: 7272 616e 6765 2063 6f6c 756d 6e73 2c20  rrange columns, 
+000106d0: 646f 6e65 2066 6f72 2075 7320 696e 2076  done for us in v
+000106e0: 6f6c 756d 655f 6f63 7628 290d 0a20 2020  olume_ocv()..   
+000106f0: 2069 7465 6d20 3d20 766f 6c75 6d65 5f6f   item = volume_o
+00010700: 6376 2864 6174 6173 7263 2c20 6361 6e64  cv(datasrc, cand
+00010710: 6c65 5f77 6964 7468 3d77 6964 7468 2c20  le_width=width, 
+00010720: 6178 3d61 782c 2063 6f6c 6f72 6675 6e63  ax=ax, colorfunc
+00010730: 3d63 6f6c 6f72 6675 6e63 290d 0a20 2020  =colorfunc)..   
+00010740: 2069 7465 6d2e 7570 6461 7465 5f64 6174   item.update_dat
+00010750: 6120 3d20 7061 7274 6961 6c28 5f75 7064  a = partial(_upd
+00010760: 6174 655f 6461 7461 2c20 4e6f 6e65 2c20  ate_data, None, 
+00010770: 5f61 646a 7573 745f 6261 725f 6461 7461  _adjust_bar_data
+00010780: 7372 632c 2069 7465 6d29 0d0a 2020 2020  src, item)..    
+00010790: 6974 656d 2e75 7064 6174 655f 6766 7820  item.update_gfx 
+000107a0: 3d20 7061 7274 6961 6c28 5f75 7064 6174  = partial(_updat
+000107b0: 655f 6766 782c 2069 7465 6d29 0d0a 2020  e_gfx, item)..  
+000107c0: 2020 6178 2e76 622e 7072 655f 7072 6f63    ax.vb.pre_proc
+000107d0: 6573 735f 6461 7461 2829 0d0a 2020 2020  ess_data()..    
+000107e0: 6966 2061 782e 7662 2e79 5f6d 696e 203e  if ax.vb.y_min >
+000107f0: 3d20 303a 0d0a 2020 2020 2020 2020 6178  = 0:..        ax
+00010800: 2e76 622e 765f 7a6f 6f6d 5f62 6173 656c  .vb.v_zoom_basel
+00010810: 696e 6520 3d20 300d 0a20 2020 2072 6574  ine = 0..    ret
+00010820: 7572 6e20 6974 656d 0d0a 0d0a 0d0a 6465  urn item......de
+00010830: 6620 6869 7374 2878 2c20 6269 6e73 2c20  f hist(x, bins, 
+00010840: 6178 3d4e 6f6e 652c 202a 2a6b 7761 7267  ax=None, **kwarg
+00010850: 7329 3a0d 0a20 2020 2068 6973 745f 6461  s):..    hist_da
+00010860: 7461 203d 2070 642e 6375 7428 782c 2062  ta = pd.cut(x, b
+00010870: 696e 733d 6269 6e73 292e 7661 6c75 655f  ins=bins).value_
+00010880: 636f 756e 7473 2829 0d0a 2020 2020 6461  counts()..    da
+00010890: 7461 203d 205b 2869 2e6d 6964 2c30 2c68  ta = [(i.mid,0,h
+000108a0: 6973 745f 6461 7461 2e6c 6f63 5b69 5d2c  ist_data.loc[i],
+000108b0: 6869 7374 5f64 6174 612e 6c6f 635b 695d  hist_data.loc[i]
+000108c0: 2920 666f 7220 6920 696e 2073 6f72 7465  ) for i in sorte
+000108d0: 6428 6869 7374 5f64 6174 612e 696e 6465  d(hist_data.inde
+000108e0: 7829 5d0d 0a20 2020 2064 6620 3d20 7064  x)]..    df = pd
+000108f0: 2e44 6174 6146 7261 6d65 2864 6174 612c  .DataFrame(data,
+00010900: 2063 6f6c 756d 6e73 3d5b 2778 272c 275f   columns=['x','_
+00010910: 6f70 5f27 2c27 5f63 6c5f 272c 2762 696e  op_','_cl_','bin
+00010920: 275d 290d 0a20 2020 2064 662e 7365 745f  '])..    df.set_
+00010930: 696e 6465 7828 2778 272c 2069 6e70 6c61  index('x', inpla
+00010940: 6365 3d54 7275 6529 0d0a 2020 2020 6974  ce=True)..    it
+00010950: 656d 203d 2062 6172 2864 662c 2061 783d  em = bar(df, ax=
+00010960: 6178 290d 0a20 2020 2064 656c 2069 7465  ax)..    del ite
+00010970: 6d2e 7570 6461 7465 5f64 6174 610d 0a20  m.update_data.. 
+00010980: 2020 2072 6574 7572 6e20 6974 656d 0d0a     return item..
+00010990: 0d0a 0d0a 6465 6620 706c 6f74 2878 2c20  ....def plot(x, 
+000109a0: 793d 4e6f 6e65 2c20 636f 6c6f 723d 4e6f  y=None, color=No
+000109b0: 6e65 2c20 7769 6474 683d 312c 2061 783d  ne, width=1, ax=
+000109c0: 4e6f 6e65 2c20 7374 796c 653d 4e6f 6e65  None, style=None
+000109d0: 2c20 6c65 6765 6e64 3d4e 6f6e 652c 207a  , legend=None, z
+000109e0: 6f6f 6d73 6361 6c65 3d54 7275 652c 202a  oomscale=True, *
+000109f0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2061  *kwargs):..    a
+00010a00: 7820 3d20 5f63 7265 6174 655f 706c 6f74  x = _create_plot
+00010a10: 2861 783d 6178 2c20 6d61 7869 6d69 7a65  (ax=ax, maximize
+00010a20: 3d46 616c 7365 290d 0a20 2020 2075 7365  =False)..    use
+00010a30: 645f 636f 6c6f 7220 3d20 5f67 6574 5f63  d_color = _get_c
+00010a40: 6f6c 6f72 2861 782c 2073 7479 6c65 2c20  olor(ax, style, 
+00010a50: 636f 6c6f 7229 0d0a 2020 2020 6461 7461  color)..    data
+00010a60: 7372 6320 3d20 5f63 7265 6174 655f 6461  src = _create_da
+00010a70: 7461 7372 6328 6178 2c20 782c 2079 2c20  tasrc(ax, x, y, 
+00010a80: 6e63 6f6c 733d 3129 0d0a 2020 2020 6966  ncols=1)..    if
+00010a90: 206e 6f74 207a 6f6f 6d73 6361 6c65 3a0d   not zoomscale:.
+00010aa0: 0a20 2020 2020 2020 2064 6174 6173 7263  .        datasrc
+00010ab0: 2e73 6361 6c65 5f63 6f6c 7320 3d20 5b5d  .scale_cols = []
+00010ac0: 0d0a 2020 2020 5f73 6574 5f64 6174 6173  ..    _set_datas
+00010ad0: 7263 2861 782c 2064 6174 6173 7263 290d  rc(ax, datasrc).
+00010ae0: 0a20 2020 2069 6620 6c65 6765 6e64 2069  .    if legend i
+00010af0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00010b00: 2020 2020 205f 6372 6561 7465 5f6c 6567       _create_leg
+00010b10: 656e 6428 6178 290d 0a20 2020 2078 203d  end(ax)..    x =
+00010b20: 2064 6174 6173 7263 2e78 2069 6620 6e6f   datasrc.x if no
+00010b30: 7420 6178 2e76 622e 785f 696e 6465 7865  t ax.vb.x_indexe
+00010b40: 6420 656c 7365 2064 6174 6173 7263 2e69  d else datasrc.i
+00010b50: 6e64 6578 0d0a 2020 2020 7920 3d20 6461  ndex..    y = da
+00010b60: 7461 7372 632e 7920 2f20 6178 2e76 622e  tasrc.y / ax.vb.
+00010b70: 7973 6361 6c65 2e73 6361 6c65 660d 0a20  yscale.scalef.. 
+00010b80: 2020 2069 6620 6178 2e76 622e 7973 6361     if ax.vb.ysca
+00010b90: 6c65 2e73 6361 6c65 7479 7065 203d 3d20  le.scaletype == 
+00010ba0: 276c 6f67 273a 0d0a 2020 2020 2020 2020  'log':..        
+00010bb0: 7920 3d20 7920 2b20 6c6f 675f 706c 6f74  y = y + log_plot
+00010bc0: 5f6f 6666 7365 740d 0a20 2020 2069 6620  _offset..    if 
+00010bd0: 7374 796c 6520 6973 204e 6f6e 6520 6f72  style is None or
+00010be0: 2061 6e79 2863 6820 696e 2073 7479 6c65   any(ch in style
+00010bf0: 2066 6f72 2063 6820 696e 2027 2d5f 2e27   for ch in '-_.'
+00010c00: 293a 0d0a 2020 2020 2020 2020 636f 6e6e  ):..        conn
+00010c10: 6563 745f 646f 7473 203d 2027 6669 6e69  ect_dots = 'fini
+00010c20: 7465 2720 2320 7361 6d65 2061 7320 6d61  te' # same as ma
+00010c30: 7470 6c6f 746c 6962 3b20 7573 6520 6461  tplotlib; use da
+00010c40: 7461 7372 632e 7374 616e 6461 6c6f 6e65  tasrc.standalone
+00010c50: 3d54 7275 6520 6966 2079 6f75 2077 616e  =True if you wan
+00010c60: 7420 746f 206b 6565 7020 7365 7061 7261  t to keep separa
+00010c70: 7465 2069 6e74 6572 7661 6c73 206f 6e20  te intervals on 
+00010c80: 6120 706c 6f74 0d0a 2020 2020 2020 2020  a plot..        
+00010c90: 6974 656d 203d 2061 782e 706c 6f74 2878  item = ax.plot(x
+00010ca0: 2c20 792c 2070 656e 3d5f 6d61 6b65 7065  , y, pen=_makepe
+00010cb0: 6e28 636f 6c6f 723d 7573 6564 5f63 6f6c  n(color=used_col
+00010cc0: 6f72 2c20 7374 796c 653d 7374 796c 652c  or, style=style,
+00010cd0: 2077 6964 7468 3d77 6964 7468 292c 206e   width=width), n
+00010ce0: 616d 653d 6c65 6765 6e64 2c20 636f 6e6e  ame=legend, conn
+00010cf0: 6563 743d 636f 6e6e 6563 745f 646f 7473  ect=connect_dots
+00010d00: 290d 0a20 2020 2020 2020 2069 7465 6d2e  )..        item.
+00010d10: 7365 7443 6c69 7054 6f56 6965 7728 5472  setClipToView(Tr
+00010d20: 7565 290d 0a20 2020 2020 2020 2069 7465  ue)..        ite
+00010d30: 6d2e 7365 7444 6f77 6e73 616d 706c 696e  m.setDownsamplin
+00010d40: 6728 6175 746f 3d54 7275 652c 206d 6574  g(auto=True, met
+00010d50: 686f 643d 2773 7562 7361 6d70 6c65 2729  hod='subsample')
+00010d60: 0d0a 2020 2020 2020 2020 6974 656d 2e73  ..        item.s
+00010d70: 6574 5a56 616c 7565 2835 290d 0a20 2020  etZValue(5)..   
+00010d80: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00010d90: 7379 6d62 6f6c 203d 207b 2776 273a 2774  symbol = {'v':'t
+00010da0: 272c 2027 5e27 3a27 7431 272c 2027 3e27  ', '^':'t1', '>'
+00010db0: 3a27 7432 272c 2027 3c27 3a27 7433 277d  :'t2', '<':'t3'}
+00010dc0: 2e67 6574 2873 7479 6c65 2c20 7374 796c  .get(style, styl
+00010dd0: 6529 2023 2074 7261 6e73 6c61 7465 2073  e) # translate s
+00010de0: 6f6d 6520 7369 6d69 6c61 7220 7374 796c  ome similar styl
+00010df0: 6573 0d0a 2020 2020 2020 2020 7966 696c  es..        yfil
+00010e00: 7465 7220 3d20 792e 6e6f 746e 756c 6c28  ter = y.notnull(
+00010e10: 290d 0a20 2020 2020 2020 2073 6572 203d  )..        ser =
+00010e20: 2079 2e6c 6f63 5b79 6669 6c74 6572 5d0d   y.loc[yfilter].
+00010e30: 0a20 2020 2020 2020 2078 203d 2078 2e6c  .        x = x.l
+00010e40: 6f63 5b79 6669 6c74 6572 5d2e 7661 6c75  oc[yfilter].valu
+00010e50: 6573 2069 6620 6861 7361 7474 7228 782c  es if hasattr(x,
+00010e60: 2027 6c6f 6327 2920 656c 7365 2078 5b79   'loc') else x[y
+00010e70: 6669 6c74 6572 5d0d 0a20 2020 2020 2020  filter]..       
+00010e80: 2069 7465 6d20 3d20 6178 2e70 6c6f 7428   item = ax.plot(
+00010e90: 782c 2073 6572 2e76 616c 7565 732c 2070  x, ser.values, p
+00010ea0: 656e 3d4e 6f6e 652c 2073 796d 626f 6c3d  en=None, symbol=
+00010eb0: 7379 6d62 6f6c 2c20 7379 6d62 6f6c 5065  symbol, symbolPe
+00010ec0: 6e3d 4e6f 6e65 2c20 7379 6d62 6f6c 5369  n=None, symbolSi
+00010ed0: 7a65 3d37 2a77 6964 7468 2c20 7379 6d62  ze=7*width, symb
+00010ee0: 6f6c 4272 7573 683d 7067 2e6d 6b42 7275  olBrush=pg.mkBru
+00010ef0: 7368 2875 7365 645f 636f 6c6f 7229 2c20  sh(used_color), 
+00010f00: 6e61 6d65 3d6c 6567 656e 6429 0d0a 2020  name=legend)..  
+00010f10: 2020 2020 2020 6966 2077 6964 7468 203c        if width <
+00010f20: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00010f30: 2069 7465 6d2e 6f70 7473 5b27 616e 7469   item.opts['anti
+00010f40: 616c 6961 7327 5d20 3d20 5472 7565 0d0a  alias'] = True..
+00010f50: 2020 2020 2020 2020 6974 656d 2e73 6361          item.sca
+00010f60: 7474 6572 2e5f 646f 7061 696e 7420 3d20  tter._dopaint = 
+00010f70: 6974 656d 2e73 6361 7474 6572 2e70 6169  item.scatter.pai
+00010f80: 6e74 0d0a 2020 2020 2020 2020 6974 656d  nt..        item
+00010f90: 2e73 6361 7474 6572 2e70 6169 6e74 203d  .scatter.paint =
+00010fa0: 2070 6172 7469 616c 285f 7061 696e 745f   partial(_paint_
+00010fb0: 7363 6174 7465 722c 2069 7465 6d2e 7363  scatter, item.sc
+00010fc0: 6174 7465 7229 0d0a 2020 2020 2020 2020  atter)..        
+00010fd0: 2320 6f70 7469 6d69 7a65 2028 7768 656e  # optimize (when
+00010fe0: 2068 6176 696e 6720 6c61 7267 6520 6e75   having large nu
+00010ff0: 6d62 6572 206f 6620 706f 696e 7473 2920  mber of points) 
+00011000: 6279 2069 676e 6f72 696e 6720 7363 6174  by ignoring scat
+00011010: 7465 7220 636c 6963 6b20 6465 7465 6374  ter click detect
+00011020: 696f 6e0d 0a20 2020 2020 2020 205f 6475  ion..        _du
+00011030: 6d6d 795f 6d6f 7573 655f 636c 6963 6b20  mmy_mouse_click 
+00011040: 3d20 6c61 6d62 6461 2065 763a 2030 0d0a  = lambda ev: 0..
+00011050: 2020 2020 2020 2020 6974 656d 2e73 6361          item.sca
+00011060: 7474 6572 2e6d 6f75 7365 436c 6963 6b45  tter.mouseClickE
+00011070: 7665 6e74 203d 205f 6475 6d6d 795f 6d6f  vent = _dummy_mo
+00011080: 7573 655f 636c 6963 6b0d 0a20 2020 2020  use_click..     
+00011090: 2020 2069 7465 6d2e 7365 745a 5661 6c75     item.setZValu
+000110a0: 6528 3130 290d 0a20 2020 2069 7465 6d2e  e(10)..    item.
+000110b0: 6f70 7473 5b27 6861 6e64 6564 5f63 6f6c  opts['handed_col
+000110c0: 6f72 275d 203d 2063 6f6c 6f72 0d0a 2020  or'] = color..  
+000110d0: 2020 6974 656d 2e61 7820 3d20 6178 0d0a    item.ax = ax..
+000110e0: 2020 2020 6974 656d 2e64 6174 6173 7263      item.datasrc
+000110f0: 203d 2064 6174 6173 7263 0d0a 2020 2020   = datasrc..    
+00011100: 5f75 7064 6174 655f 7369 676e 6966 6963  _update_signific
+00011110: 616e 7473 2861 782c 2064 6174 6173 7263  ants(ax, datasrc
+00011120: 2c20 666f 7263 653d 4661 6c73 6529 0d0a  , force=False)..
+00011130: 2020 2020 6974 656d 2e75 7064 6174 655f      item.update_
+00011140: 6461 7461 203d 2070 6172 7469 616c 285f  data = partial(_
+00011150: 7570 6461 7465 5f64 6174 612c 204e 6f6e  update_data, Non
+00011160: 652c 204e 6f6e 652c 2069 7465 6d29 0d0a  e, None, item)..
+00011170: 2020 2020 6974 656d 2e75 7064 6174 655f      item.update_
+00011180: 6766 7820 3d20 7061 7274 6961 6c28 5f75  gfx = partial(_u
+00011190: 7064 6174 655f 6766 782c 2069 7465 6d29  pdate_gfx, item)
+000111a0: 0d0a 2020 2020 2320 6164 6420 6c65 6765  ..    # add lege
+000111b0: 6e64 2074 6f20 6d61 696e 2061 782c 206e  nd to main ax, n
+000111c0: 6f74 2074 6f20 6f76 6572 6c61 790d 0a20  ot to overlay.. 
+000111d0: 2020 2061 786d 203d 2061 782e 7662 2e6d     axm = ax.vb.m
+000111e0: 6173 7465 725f 7669 6577 626f 782e 7061  aster_viewbox.pa
+000111f0: 7265 6e74 2829 2069 6620 6178 2e76 622e  rent() if ax.vb.
+00011200: 6d61 7374 6572 5f76 6965 7762 6f78 2065  master_viewbox e
+00011210: 6c73 6520 6178 0d0a 2020 2020 6966 2061  lse ax..    if a
+00011220: 786d 2e6c 6567 656e 6420 6973 206e 6f74  xm.legend is not
+00011230: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00011240: 6966 206c 6567 656e 6420 616e 6420 6178  if legend and ax
+00011250: 6d20 213d 2061 783a 0d0a 2020 2020 2020  m != ax:..      
+00011260: 2020 2020 2020 6178 6d2e 6c65 6765 6e64        axm.legend
+00011270: 2e61 6464 4974 656d 2869 7465 6d2c 206e  .addItem(item, n
+00011280: 616d 653d 6c65 6765 6e64 290d 0a20 2020  ame=legend)..   
+00011290: 2020 2020 2066 6f72 205f 2c6c 6162 656c       for _,label
+000112a0: 2069 6e20 6178 6d2e 6c65 6765 6e64 2e69   in axm.legend.i
+000112b0: 7465 6d73 3a0d 0a20 2020 2020 2020 2020  tems:..         
+000112c0: 2020 2069 6620 6c61 6265 6c2e 7465 7874     if label.text
+000112d0: 203d 3d20 6c65 6765 6e64 3a0d 0a20 2020   == legend:..   
+000112e0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+000112f0: 656c 2e73 6574 4174 7472 2827 6a75 7374  el.setAttr('just
+00011300: 6966 7927 2c20 276c 6566 7427 290d 0a20  ify', 'left').. 
+00011310: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011320: 6162 656c 2e73 6574 5465 7874 286c 6162  abel.setText(lab
+00011330: 656c 2e74 6578 742c 2063 6f6c 6f72 3d6c  el.text, color=l
+00011340: 6567 656e 645f 7465 7874 5f63 6f6c 6f72  egend_text_color
+00011350: 290d 0a20 2020 2072 6574 7572 6e20 6974  )..    return it
+00011360: 656d 0d0a 0d0a 0d0a 6465 6620 6c61 6265  em......def labe
+00011370: 6c73 2878 2c20 793d 4e6f 6e65 2c20 6c61  ls(x, y=None, la
+00011380: 6265 6c73 3d4e 6f6e 652c 2063 6f6c 6f72  bels=None, color
+00011390: 3d4e 6f6e 652c 2061 783d 4e6f 6e65 2c20  =None, ax=None, 
+000113a0: 616e 6368 6f72 3d28 302e 352c 3129 293a  anchor=(0.5,1)):
+000113b0: 0d0a 2020 2020 6178 203d 205f 6372 6561  ..    ax = _crea
+000113c0: 7465 5f70 6c6f 7428 6178 3d61 782c 206d  te_plot(ax=ax, m
+000113d0: 6178 696d 697a 653d 4661 6c73 6529 0d0a  aximize=False)..
+000113e0: 2020 2020 7573 6564 5f63 6f6c 6f72 203d      used_color =
+000113f0: 205f 6765 745f 636f 6c6f 7228 6178 2c20   _get_color(ax, 
+00011400: 273f 272c 2063 6f6c 6f72 290d 0a20 2020  '?', color)..   
+00011410: 2064 6174 6173 7263 203d 205f 6372 6561   datasrc = _crea
+00011420: 7465 5f64 6174 6173 7263 2861 782c 2078  te_datasrc(ax, x
+00011430: 2c20 792c 206c 6162 656c 732c 206e 636f  , y, labels, nco
+00011440: 6c73 3d33 290d 0a20 2020 2064 6174 6173  ls=3)..    datas
+00011450: 7263 2e73 6361 6c65 5f63 6f6c 7320 3d20  rc.scale_cols = 
+00011460: 5b5d 2023 2064 6f6e 2774 2075 7365 2074  [] # don't use t
+00011470: 6869 7320 666f 7220 7363 616c 696e 670d  his for scaling.
+00011480: 0a20 2020 205f 7365 745f 6461 7461 7372  .    _set_datasr
+00011490: 6328 6178 2c20 6461 7461 7372 6329 0d0a  c(ax, datasrc)..
+000114a0: 2020 2020 6974 656d 203d 2053 6361 7474      item = Scatt
+000114b0: 6572 4c61 6265 6c49 7465 6d28 6178 3d61  erLabelItem(ax=a
+000114c0: 782c 2064 6174 6173 7263 3d64 6174 6173  x, datasrc=datas
+000114d0: 7263 2c20 636f 6c6f 723d 7573 6564 5f63  rc, color=used_c
+000114e0: 6f6c 6f72 2c20 616e 6368 6f72 3d61 6e63  olor, anchor=anc
+000114f0: 686f 7229 0d0a 2020 2020 5f75 7064 6174  hor)..    _updat
+00011500: 655f 7369 676e 6966 6963 616e 7473 2861  e_significants(a
+00011510: 782c 2064 6174 6173 7263 2c20 666f 7263  x, datasrc, forc
+00011520: 653d 4661 6c73 6529 0d0a 2020 2020 6974  e=False)..    it
+00011530: 656d 2e75 7064 6174 655f 6461 7461 203d  em.update_data =
+00011540: 2070 6172 7469 616c 285f 7570 6461 7465   partial(_update
+00011550: 5f64 6174 612c 204e 6f6e 652c 204e 6f6e  _data, None, Non
+00011560: 652c 2069 7465 6d29 0d0a 2020 2020 6974  e, item)..    it
+00011570: 656d 2e75 7064 6174 655f 6766 7820 3d20  em.update_gfx = 
+00011580: 7061 7274 6961 6c28 5f75 7064 6174 655f  partial(_update_
+00011590: 6766 782c 2069 7465 6d29 0d0a 2020 2020  gfx, item)..    
+000115a0: 6178 2e61 6464 4974 656d 2869 7465 6d29  ax.addItem(item)
+000115b0: 0d0a 2020 2020 6966 2061 782e 7662 2e76  ..    if ax.vb.v
+000115c0: 5f7a 6f6f 6d5f 7363 616c 6520 3e20 302e  _zoom_scale > 0.
+000115d0: 393a 2023 2061 646a 7573 7420 746f 206d  9: # adjust to m
+000115e0: 616b 6520 6869 2f6c 6f20 7465 7874 2066  ake hi/lo text f
+000115f0: 6974 0d0a 2020 2020 2020 2020 6178 2e76  it..        ax.v
+00011600: 622e 765f 7a6f 6f6d 5f73 6361 6c65 203d  b.v_zoom_scale =
+00011610: 2030 2e39 0d0a 2020 2020 7265 7475 726e   0.9..    return
+00011620: 2069 7465 6d0d 0a0d 0a0d 0a64 6566 206c   item......def l
+00011630: 6976 6528 706c 6f74 733d 3129 3a0d 0a20  ive(plots=1):.. 
+00011640: 2020 2069 6620 706c 6f74 7320 3d3d 2031     if plots == 1
+00011650: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00011660: 6e20 4c69 7665 2829 0d0a 2020 2020 7265  n Live()..    re
+00011670: 7475 726e 205b 4c69 7665 2829 2066 6f72  turn [Live() for
+00011680: 205f 2069 6e20 7261 6e67 6528 706c 6f74   _ in range(plot
+00011690: 7329 5d0d 0a0d 0a0d 0a64 6566 2061 6464  s)]......def add
+000116a0: 5f6c 6567 656e 6428 7465 7874 2c20 6178  _legend(text, ax
+000116b0: 3d4e 6f6e 6529 3a0d 0a20 2020 2061 7820  =None):..    ax 
+000116c0: 3d20 5f63 7265 6174 655f 706c 6f74 2861  = _create_plot(a
+000116d0: 783d 6178 2c20 6d61 7869 6d69 7a65 3d46  x=ax, maximize=F
+000116e0: 616c 7365 290d 0a20 2020 205f 6372 6561  alse)..    _crea
+000116f0: 7465 5f6c 6567 656e 6428 6178 290d 0a20  te_legend(ax).. 
+00011700: 2020 2072 6f77 203d 2061 782e 6c65 6765     row = ax.lege
+00011710: 6e64 2e6c 6179 6f75 742e 726f 7743 6f75  nd.layout.rowCou
+00011720: 6e74 2829 0d0a 2020 2020 6c61 6265 6c20  nt()..    label 
+00011730: 3d20 7067 2e4c 6162 656c 4974 656d 2874  = pg.LabelItem(t
+00011740: 6578 742c 2063 6f6c 6f72 3d6c 6567 656e  ext, color=legen
+00011750: 645f 7465 7874 5f63 6f6c 6f72 2c20 6a75  d_text_color, ju
+00011760: 7374 6966 793d 276c 6566 7427 290d 0a20  stify='left').. 
+00011770: 2020 2061 782e 6c65 6765 6e64 2e6c 6179     ax.legend.lay
+00011780: 6f75 742e 6164 6449 7465 6d28 6c61 6265  out.addItem(labe
+00011790: 6c2c 2072 6f77 2c20 302c 2031 2c20 3229  l, row, 0, 1, 2)
+000117a0: 0d0a 2020 2020 7265 7475 726e 206c 6162  ..    return lab
+000117b0: 656c 0d0a 0d0a 0d0a 6465 6620 6669 6c6c  el......def fill
+000117c0: 5f62 6574 7765 656e 2870 6c6f 7430 2c20  _between(plot0, 
+000117d0: 706c 6f74 312c 2063 6f6c 6f72 3d4e 6f6e  plot1, color=Non
+000117e0: 6529 3a0d 0a20 2020 2075 7365 645f 636f  e):..    used_co
+000117f0: 6c6f 7220 3d20 6272 6967 6874 656e 285f  lor = brighten(_
+00011800: 6765 745f 636f 6c6f 7228 706c 6f74 302e  get_color(plot0.
+00011810: 6178 2c20 4e6f 6e65 2c20 636f 6c6f 7229  ax, None, color)
+00011820: 2c20 312e 3329 0d0a 2020 2020 6974 656d  , 1.3)..    item
+00011830: 203d 2070 672e 4669 6c6c 4265 7477 6565   = pg.FillBetwee
+00011840: 6e49 7465 6d28 706c 6f74 302c 2070 6c6f  nItem(plot0, plo
+00011850: 7431 2c20 6272 7573 683d 7067 2e6d 6b42  t1, brush=pg.mkB
+00011860: 7275 7368 2875 7365 645f 636f 6c6f 7229  rush(used_color)
+00011870: 290d 0a20 2020 2069 7465 6d2e 6178 203d  )..    item.ax =
+00011880: 2070 6c6f 7430 2e61 780d 0a20 2020 2069   plot0.ax..    i
+00011890: 7465 6d2e 7365 745a 5661 6c75 6528 2d34  tem.setZValue(-4
+000118a0: 3029 0d0a 2020 2020 6974 656d 2e61 782e  0)..    item.ax.
+000118b0: 6164 6449 7465 6d28 6974 656d 290d 0a20  addItem(item).. 
+000118c0: 2020 2072 6574 7572 6e20 6974 656d 0d0a     return item..
+000118d0: 0d0a 0d0a 6465 6620 7365 745f 785f 706f  ....def set_x_po
+000118e0: 7328 786d 696e 2c20 786d 6178 2c20 6178  s(xmin, xmax, ax
+000118f0: 3d4e 6f6e 6529 3a0d 0a20 2020 2061 7820  =None):..    ax 
+00011900: 3d20 5f63 7265 6174 655f 706c 6f74 2861  = _create_plot(a
+00011910: 783d 6178 2c20 6d61 7869 6d69 7a65 3d46  x=ax, maximize=F
+00011920: 616c 7365 290d 0a20 2020 2078 6964 7830  alse)..    xidx0
+00011930: 2c78 6964 7831 203d 205f 7064 7469 6d65  ,xidx1 = _pdtime
+00011940: 3269 6e64 6578 2861 782c 2070 642e 5365  2index(ax, pd.Se
+00011950: 7269 6573 285b 786d 696e 2c20 786d 6178  ries([xmin, xmax
+00011960: 5d29 290d 0a20 2020 2061 782e 7662 2e75  ]))..    ax.vb.u
+00011970: 7064 6174 655f 795f 7a6f 6f6d 2878 6964  pdate_y_zoom(xid
+00011980: 7830 2c20 7869 6478 3129 0d0a 2020 2020  x0, xidx1)..    
+00011990: 5f72 6570 6169 6e74 5f63 616e 646c 6573  _repaint_candles
+000119a0: 2829 0d0a 0d0a 0d0a 6465 6620 7365 745f  ()......def set_
+000119b0: 795f 7261 6e67 6528 796d 696e 2c20 796d  y_range(ymin, ym
+000119c0: 6178 2c20 6178 3d4e 6f6e 6529 3a0d 0a20  ax, ax=None):.. 
+000119d0: 2020 2061 7820 3d20 5f63 7265 6174 655f     ax = _create_
+000119e0: 706c 6f74 2861 783d 6178 2c20 6d61 7869  plot(ax=ax, maxi
+000119f0: 6d69 7a65 3d46 616c 7365 290d 0a20 2020  mize=False)..   
+00011a00: 2061 782e 7365 744c 696d 6974 7328 794d   ax.setLimits(yM
+00011a10: 696e 3d79 6d69 6e2c 2079 4d61 783d 796d  in=ymin, yMax=ym
+00011a20: 6178 290d 0a20 2020 2061 782e 7662 2e76  ax)..    ax.vb.v
+00011a30: 5f61 7574 6f7a 6f6f 6d20 3d20 4661 6c73  _autozoom = Fals
+00011a40: 650d 0a20 2020 2061 782e 7662 2e73 6574  e..    ax.vb.set
+00011a50: 5f72 616e 6765 284e 6f6e 652c 2079 6d69  _range(None, ymi
+00011a60: 6e2c 204e 6f6e 652c 2079 6d61 7829 0d0a  n, None, ymax)..
+00011a70: 0d0a 0d0a 6465 6620 7365 745f 795f 7363  ....def set_y_sc
+00011a80: 616c 6528 7973 6361 6c65 3d27 6c69 6e65  ale(yscale='line
+00011a90: 6172 272c 2061 783d 4e6f 6e65 293a 0d0a  ar', ax=None):..
+00011aa0: 2020 2020 6178 203d 205f 6372 6561 7465      ax = _create
+00011ab0: 5f70 6c6f 7428 6178 3d61 782c 206d 6178  _plot(ax=ax, max
+00011ac0: 696d 697a 653d 4661 6c73 6529 0d0a 2020  imize=False)..  
+00011ad0: 2020 6178 2e73 6574 4c6f 674d 6f64 6528    ax.setLogMode(
+00011ae0: 793d 2879 7363 616c 653d 3d27 6c6f 6727  y=(yscale=='log'
+00011af0: 2929 0d0a 2020 2020 6178 2e76 622e 7973  ))..    ax.vb.ys
+00011b00: 6361 6c65 203d 2059 5363 616c 6528 7973  cale = YScale(ys
+00011b10: 6361 6c65 2c20 6178 2e76 622e 7973 6361  cale, ax.vb.ysca
+00011b20: 6c65 2e73 6361 6c65 6629 0d0a 0d0a 0d0a  le.scalef)......
+00011b30: 6465 6620 6164 645f 6261 6e64 2879 302c  def add_band(y0,
+00011b40: 2079 312c 2063 6f6c 6f72 3d62 616e 645f   y1, color=band_
+00011b50: 636f 6c6f 722c 2061 783d 4e6f 6e65 293a  color, ax=None):
+00011b60: 0d0a 2020 2020 6178 203d 205f 6372 6561  ..    ax = _crea
+00011b70: 7465 5f70 6c6f 7428 6178 3d61 782c 206d  te_plot(ax=ax, m
+00011b80: 6178 696d 697a 653d 4661 6c73 6529 0d0a  aximize=False)..
+00011b90: 2020 2020 636f 6c6f 7220 3d20 5f67 6574      color = _get
+00011ba0: 5f63 6f6c 6f72 2861 782c 204e 6f6e 652c  _color(ax, None,
+00011bb0: 2063 6f6c 6f72 290d 0a20 2020 2069 7820   color)..    ix 
+00011bc0: 3d20 6178 2e76 622e 7973 6361 6c65 2e69  = ax.vb.yscale.i
+00011bd0: 6e76 7866 6f72 6d0d 0a20 2020 206c 7220  nvxform..    lr 
+00011be0: 3d20 7067 2e4c 696e 6561 7252 6567 696f  = pg.LinearRegio
+00011bf0: 6e49 7465 6d28 5b69 7828 7930 292c 6978  nItem([ix(y0),ix
+00011c00: 2879 3129 5d2c 206f 7269 656e 7461 7469  (y1)], orientati
+00011c10: 6f6e 3d70 672e 4c69 6e65 6172 5265 6769  on=pg.LinearRegi
+00011c20: 6f6e 4974 656d 2e48 6f72 697a 6f6e 7461  onItem.Horizonta
+00011c30: 6c2c 2062 7275 7368 3d70 672e 6d6b 4272  l, brush=pg.mkBr
+00011c40: 7573 6828 636f 6c6f 7229 2c20 6d6f 7661  ush(color), mova
+00011c50: 626c 653d 4661 6c73 6529 0d0a 2020 2020  ble=False)..    
+00011c60: 6c72 2e6c 696e 6573 5b30 5d2e 7365 7450  lr.lines[0].setP
+00011c70: 656e 2870 672e 6d6b 5065 6e28 4e6f 6e65  en(pg.mkPen(None
+00011c80: 2929 0d0a 2020 2020 6c72 2e6c 696e 6573  ))..    lr.lines
+00011c90: 5b31 5d2e 7365 7450 656e 2870 672e 6d6b  [1].setPen(pg.mk
+00011ca0: 5065 6e28 4e6f 6e65 2929 0d0a 2020 2020  Pen(None))..    
+00011cb0: 6c72 2e73 6574 5a56 616c 7565 282d 3530  lr.setZValue(-50
+00011cc0: 290d 0a20 2020 206c 722e 6178 203d 2061  )..    lr.ax = a
+00011cd0: 780d 0a20 2020 2061 782e 6164 6449 7465  x..    ax.addIte
+00011ce0: 6d28 6c72 290d 0a20 2020 2072 6574 7572  m(lr)..    retur
+00011cf0: 6e20 6c72 0d0a 0d0a 0d0a 6465 6620 6164  n lr......def ad
+00011d00: 645f 7265 6374 2870 302c 2070 312c 2063  d_rect(p0, p1, c
+00011d10: 6f6c 6f72 3d62 616e 645f 636f 6c6f 722c  olor=band_color,
+00011d20: 2069 6e74 6572 6163 7469 7665 3d46 616c   interactive=Fal
+00011d30: 7365 2c20 6178 3d4e 6f6e 6529 3a0d 0a20  se, ax=None):.. 
+00011d40: 2020 2061 7820 3d20 5f63 7265 6174 655f     ax = _create_
+00011d50: 706c 6f74 2861 783d 6178 2c20 6d61 7869  plot(ax=ax, maxi
+00011d60: 6d69 7a65 3d46 616c 7365 290d 0a20 2020  mize=False)..   
+00011d70: 2078 5f70 7473 203d 205f 7064 7469 6d65   x_pts = _pdtime
+00011d80: 3269 6e64 6578 2861 782c 2070 642e 5365  2index(ax, pd.Se
+00011d90: 7269 6573 285b 7030 5b30 5d2c 2070 315b  ries([p0[0], p1[
+00011da0: 305d 5d29 290d 0a20 2020 2069 7820 3d20  0]]))..    ix = 
+00011db0: 6178 2e76 622e 7973 6361 6c65 2e69 6e76  ax.vb.yscale.inv
+00011dc0: 7866 6f72 6d0d 0a20 2020 2079 302c 7931  xform..    y0,y1
+00011dd0: 203d 2073 6f72 7465 6428 5b70 305b 315d   = sorted([p0[1]
+00011de0: 2c20 7031 5b31 5d5d 290d 0a20 2020 2070  , p1[1]])..    p
+00011df0: 6f73 2020 3d20 2878 5f70 7473 5b30 5d2c  os  = (x_pts[0],
+00011e00: 2069 7828 7930 2929 0d0a 2020 2020 7369   ix(y0))..    si
+00011e10: 7a65 203d 2028 785f 7074 735b 315d 2d70  ze = (x_pts[1]-p
+00011e20: 6f73 5b30 5d2c 2069 7828 7931 292d 6978  os[0], ix(y1)-ix
+00011e30: 2879 3029 290d 0a20 2020 2072 6563 7420  (y0))..    rect 
+00011e40: 3d20 4669 6e52 6563 7428 6178 3d61 782c  = FinRect(ax=ax,
+00011e50: 2062 7275 7368 3d70 672e 6d6b 4272 7573   brush=pg.mkBrus
+00011e60: 6828 636f 6c6f 7229 2c20 706f 733d 706f  h(color), pos=po
+00011e70: 732c 2073 697a 653d 7369 7a65 2c20 6d6f  s, size=size, mo
+00011e80: 7661 626c 653d 696e 7465 7261 6374 6976  vable=interactiv
+00011e90: 652c 2072 6573 697a 6162 6c65 3d69 6e74  e, resizable=int
+00011ea0: 6572 6163 7469 7665 2c20 726f 7461 7461  eractive, rotata
+00011eb0: 626c 653d 4661 6c73 6529 0d0a 2020 2020  ble=False)..    
+00011ec0: 7265 6374 2e73 6574 5a56 616c 7565 282d  rect.setZValue(-
+00011ed0: 3430 290d 0a20 2020 2069 6620 696e 7465  40)..    if inte
+00011ee0: 7261 6374 6976 653a 0d0a 2020 2020 2020  ractive:..      
+00011ef0: 2020 6178 2e76 622e 726f 6973 2e61 7070    ax.vb.rois.app
+00011f00: 656e 6428 7265 6374 290d 0a20 2020 2072  end(rect)..    r
+00011f10: 6563 742e 6178 203d 2061 780d 0a20 2020  ect.ax = ax..   
+00011f20: 2061 782e 6164 6449 7465 6d28 7265 6374   ax.addItem(rect
+00011f30: 290d 0a20 2020 2072 6574 7572 6e20 7265  )..    return re
+00011f40: 6374 0d0a 0d0a 0d0a 6465 6620 6164 645f  ct......def add_
+00011f50: 6c69 6e65 2870 302c 2070 312c 2063 6f6c  line(p0, p1, col
+00011f60: 6f72 3d64 7261 775f 6c69 6e65 5f63 6f6c  or=draw_line_col
+00011f70: 6f72 2c20 7769 6474 683d 312c 2073 7479  or, width=1, sty
+00011f80: 6c65 3d4e 6f6e 652c 2069 6e74 6572 6163  le=None, interac
+00011f90: 7469 7665 3d46 616c 7365 2c20 6178 3d4e  tive=False, ax=N
+00011fa0: 6f6e 6529 3a0d 0a20 2020 2061 7820 3d20  one):..    ax = 
+00011fb0: 5f63 7265 6174 655f 706c 6f74 2861 783d  _create_plot(ax=
+00011fc0: 6178 2c20 6d61 7869 6d69 7a65 3d46 616c  ax, maximize=Fal
+00011fd0: 7365 290d 0a20 2020 2075 7365 645f 636f  se)..    used_co
+00011fe0: 6c6f 7220 3d20 5f67 6574 5f63 6f6c 6f72  lor = _get_color
+00011ff0: 2861 782c 2073 7479 6c65 2c20 636f 6c6f  (ax, style, colo
+00012000: 7229 0d0a 2020 2020 7065 6e20 3d20 5f6d  r)..    pen = _m
+00012010: 616b 6570 656e 2863 6f6c 6f72 3d75 7365  akepen(color=use
+00012020: 645f 636f 6c6f 722c 2073 7479 6c65 3d73  d_color, style=s
+00012030: 7479 6c65 2c20 7769 6474 683d 7769 6474  tyle, width=widt
+00012040: 6829 0d0a 2020 2020 785f 7074 7320 3d20  h)..    x_pts = 
+00012050: 5f70 6474 696d 6532 696e 6465 7828 6178  _pdtime2index(ax
+00012060: 2c20 7064 2e53 6572 6965 7328 5b70 305b  , pd.Series([p0[
+00012070: 305d 2c20 7031 5b30 5d5d 2929 0d0a 2020  0], p1[0]]))..  
+00012080: 2020 6978 203d 2061 782e 7662 2e79 7363    ix = ax.vb.ysc
+00012090: 616c 652e 696e 7678 666f 726d 0d0a 2020  ale.invxform..  
+000120a0: 2020 7074 7320 3d20 5b28 785f 7074 735b    pts = [(x_pts[
+000120b0: 305d 2c20 6978 2870 305b 315d 2929 2c20  0], ix(p0[1])), 
+000120c0: 2878 5f70 7473 5b31 5d2c 2069 7828 7031  (x_pts[1], ix(p1
+000120d0: 5b31 5d29 295d 0d0a 2020 2020 6966 2069  [1]))]..    if i
+000120e0: 6e74 6572 6163 7469 7665 3a0d 0a20 2020  nteractive:..   
+000120f0: 2020 2020 206c 696e 6520 3d20 4669 6e50       line = FinP
+00012100: 6f6c 794c 696e 6528 6178 2e76 622c 2070  olyLine(ax.vb, p
+00012110: 7473 2c20 636c 6f73 6564 3d46 616c 7365  ts, closed=False
+00012120: 2c20 7065 6e3d 7065 6e2c 206d 6f76 6162  , pen=pen, movab
+00012130: 6c65 3d46 616c 7365 290d 0a20 2020 2020  le=False)..     
+00012140: 2020 2061 782e 7662 2e72 6f69 732e 6170     ax.vb.rois.ap
+00012150: 7065 6e64 286c 696e 6529 0d0a 2020 2020  pend(line)..    
+00012160: 656c 7365 3a0d 0a20 2020 2020 2020 206c  else:..        l
+00012170: 696e 6520 3d20 4669 6e4c 696e 6528 7074  ine = FinLine(pt
+00012180: 732c 2070 656e 3d70 656e 290d 0a20 2020  s, pen=pen)..   
+00012190: 206c 696e 652e 6178 203d 2061 780d 0a20   line.ax = ax.. 
+000121a0: 2020 2061 782e 7662 2e61 6464 4974 656d     ax.vb.addItem
+000121b0: 286c 696e 6529 0d0a 2020 2020 7265 7475  (line)..    retu
+000121c0: 726e 206c 696e 650d 0a0d 0a0d 0a64 6566  rn line......def
+000121d0: 2061 6464 5f74 6578 7428 706f 732c 2073   add_text(pos, s
+000121e0: 2c20 636f 6c6f 723d 6472 6177 5f6c 696e  , color=draw_lin
+000121f0: 655f 636f 6c6f 722c 2061 6e63 686f 723d  e_color, anchor=
+00012200: 2830 2c30 292c 2061 783d 4e6f 6e65 293a  (0,0), ax=None):
+00012210: 0d0a 2020 2020 6178 203d 205f 6372 6561  ..    ax = _crea
+00012220: 7465 5f70 6c6f 7428 6178 3d61 782c 206d  te_plot(ax=ax, m
+00012230: 6178 696d 697a 653d 4661 6c73 6529 0d0a  aximize=False)..
+00012240: 2020 2020 636f 6c6f 7220 3d20 5f67 6574      color = _get
+00012250: 5f63 6f6c 6f72 2861 782c 204e 6f6e 652c  _color(ax, None,
+00012260: 2063 6f6c 6f72 290d 0a20 2020 2074 6578   color)..    tex
+00012270: 7420 3d20 7067 2e54 6578 7449 7465 6d28  t = pg.TextItem(
+00012280: 732c 2063 6f6c 6f72 3d63 6f6c 6f72 2c20  s, color=color, 
+00012290: 616e 6368 6f72 3d61 6e63 686f 7229 0d0a  anchor=anchor)..
+000122a0: 2020 2020 7820 3d20 706f 735b 305d 0d0a      x = pos[0]..
+000122b0: 2020 2020 6966 2061 782e 7662 2e64 6174      if ax.vb.dat
+000122c0: 6173 7263 2069 7320 6e6f 7420 4e6f 6e65  asrc is not None
+000122d0: 3a0d 0a20 2020 2020 2020 2078 203d 205f  :..        x = _
+000122e0: 7064 7469 6d65 3269 6e64 6578 2861 782c  pdtime2index(ax,
+000122f0: 2070 642e 5365 7269 6573 285b 706f 735b   pd.Series([pos[
+00012300: 305d 5d29 295b 305d 0d0a 2020 2020 7920  0]]))[0]..    y 
+00012310: 3d20 6178 2e76 622e 7973 6361 6c65 2e69  = ax.vb.yscale.i
+00012320: 6e76 7866 6f72 6d28 706f 735b 315d 290d  nvxform(pos[1]).
+00012330: 0a20 2020 2074 6578 742e 7365 7450 6f73  .    text.setPos
+00012340: 2878 2c20 7929 0d0a 2020 2020 7465 7874  (x, y)..    text
+00012350: 2e73 6574 5a56 616c 7565 2835 3029 0d0a  .setZValue(50)..
+00012360: 2020 2020 7465 7874 2e61 7820 3d20 6178      text.ax = ax
+00012370: 0d0a 2020 2020 6178 2e61 6464 4974 656d  ..    ax.addItem
+00012380: 2874 6578 742c 2069 676e 6f72 6542 6f75  (text, ignoreBou
+00012390: 6e64 733d 5472 7565 290d 0a20 2020 2072  nds=True)..    r
+000123a0: 6574 7572 6e20 7465 7874 0d0a 0d0a 0d0a  eturn text......
+000123b0: 6465 6620 7265 6d6f 7665 5f6c 696e 6528  def remove_line(
+000123c0: 6c69 6e65 293a 0d0a 2020 2020 7072 696e  line):..    prin
+000123d0: 7428 2772 656d 6f76 655f 6c69 6e65 2829  t('remove_line()
+000123e0: 2069 7320 6465 7072 6563 6174 6564 2c20   is deprecated, 
+000123f0: 7573 6520 7265 6d6f 7665 5f70 7269 6d69  use remove_primi
+00012400: 7469 7665 2829 2069 6e73 7465 6164 2729  tive() instead')
+00012410: 0d0a 2020 2020 7265 6d6f 7665 5f70 7269  ..    remove_pri
+00012420: 6d69 7469 7665 286c 696e 6529 0d0a 0d0a  mitive(line)....
+00012430: 0d0a 6465 6620 7265 6d6f 7665 5f74 6578  ..def remove_tex
+00012440: 7428 7465 7874 293a 0d0a 2020 2020 7072  t(text):..    pr
+00012450: 696e 7428 2772 656d 6f76 655f 7465 7874  int('remove_text
+00012460: 2829 2069 7320 6465 7072 6563 6174 6564  () is deprecated
+00012470: 2c20 7573 6520 7265 6d6f 7665 5f70 7269  , use remove_pri
+00012480: 6d69 7469 7665 2829 2069 6e73 7465 6164  mitive() instead
+00012490: 2729 0d0a 2020 2020 7265 6d6f 7665 5f70  ')..    remove_p
+000124a0: 7269 6d69 7469 7665 2874 6578 7429 0d0a  rimitive(text)..
+000124b0: 0d0a 0d0a 6465 6620 7265 6d6f 7665 5f70  ....def remove_p
+000124c0: 7269 6d69 7469 7665 2870 7269 6d69 7469  rimitive(primiti
+000124d0: 7665 293a 0d0a 2020 2020 6178 203d 2070  ve):..    ax = p
+000124e0: 7269 6d69 7469 7665 2e61 780d 0a20 2020  rimitive.ax..   
+000124f0: 2061 782e 7662 2e72 656d 6f76 6549 7465   ax.vb.removeIte
+00012500: 6d28 7072 696d 6974 6976 6529 0d0a 2020  m(primitive)..  
+00012510: 2020 6966 2070 7269 6d69 7469 7665 2069    if primitive i
+00012520: 6e20 6178 2e76 622e 726f 6973 3a0d 0a20  n ax.vb.rois:.. 
+00012530: 2020 2020 2020 2061 782e 7662 2e72 6f69         ax.vb.roi
+00012540: 732e 7265 6d6f 7665 2870 7269 6d69 7469  s.remove(primiti
+00012550: 7665 290d 0a20 2020 2069 6620 6861 7361  ve)..    if hasa
+00012560: 7474 7228 7072 696d 6974 6976 652c 2027  ttr(primitive, '
+00012570: 7465 7874 7327 293a 0d0a 2020 2020 2020  texts'):..      
+00012580: 2020 666f 7220 7478 7420 696e 2070 7269    for txt in pri
+00012590: 6d69 7469 7665 2e74 6578 7473 3a0d 0a20  mitive.texts:.. 
+000125a0: 2020 2020 2020 2020 2020 2061 782e 7662             ax.vb
+000125b0: 2e72 656d 6f76 6549 7465 6d28 7478 7429  .removeItem(txt)
+000125c0: 0d0a 0d0a 0d0a 6465 6620 7365 745f 7469  ......def set_ti
+000125d0: 6d65 5f69 6e73 7065 6374 6f72 2869 6e73  me_inspector(ins
+000125e0: 7065 6374 6f72 2c20 6178 3d4e 6f6e 652c  pector, ax=None,
+000125f0: 2077 6865 6e3d 2763 6c69 636b 2729 3a0d   when='click'):.
+00012600: 0a20 2020 2027 2727 4361 6c6c 6261 636b  .    '''Callback
+00012610: 2077 6865 6e20 636c 6963 6b65 6420 6c69   when clicked li
+00012620: 6b65 2073 6f3a 2069 6e73 7065 6374 6f72  ke so: inspector
+00012630: 2878 2c20 7929 2e27 2727 0d0a 2020 2020  (x, y).'''..    
+00012640: 6178 203d 2061 7820 6966 2061 7820 656c  ax = ax if ax el
+00012650: 7365 206c 6173 745f 6178 0d0a 2020 2020  se last_ax..    
+00012660: 6d61 7374 6572 203d 2061 782e 6178 5f77  master = ax.ax_w
+00012670: 6964 6765 7420 6966 2068 6173 6174 7472  idget if hasattr
+00012680: 2861 782c 2027 6178 5f77 6964 6765 7427  (ax, 'ax_widget'
+00012690: 2920 656c 7365 2061 782e 7662 2e77 696e  ) else ax.vb.win
+000126a0: 0d0a 2020 2020 6966 2077 6865 6e20 3d3d  ..    if when ==
+000126b0: 2027 686f 7665 7227 3a0d 0a20 2020 2020   'hover':..     
+000126c0: 2020 206d 6173 7465 722e 7072 6f78 795f     master.proxy_
+000126d0: 686f 7665 7220 3d20 7067 2e53 6967 6e61  hover = pg.Signa
+000126e0: 6c50 726f 7879 286d 6173 7465 722e 7363  lProxy(master.sc
+000126f0: 656e 6528 292e 7369 674d 6f75 7365 4d6f  ene().sigMouseMo
+00012700: 7665 642c 2072 6174 654c 696d 6974 3d31  ved, rateLimit=1
+00012710: 352c 2073 6c6f 743d 7061 7274 6961 6c28  5, slot=partial(
+00012720: 5f69 6e73 7065 6374 5f70 6f73 2c20 6178  _inspect_pos, ax
+00012730: 2c20 696e 7370 6563 746f 7229 290d 0a20  , inspector)).. 
+00012740: 2020 2065 6c69 6620 7768 656e 2069 6e20     elif when in 
+00012750: 2827 6463 6c69 636b 272c 2027 646f 7562  ('dclick', 'doub
+00012760: 6c65 2d63 6c69 636b 2729 3a0d 0a20 2020  le-click'):..   
+00012770: 2020 2020 206d 6173 7465 722e 7072 6f78       master.prox
+00012780: 795f 6463 6c69 636b 203d 2070 672e 5369  y_dclick = pg.Si
+00012790: 676e 616c 5072 6f78 7928 6d61 7374 6572  gnalProxy(master
+000127a0: 2e73 6365 6e65 2829 2e73 6967 4d6f 7573  .scene().sigMous
+000127b0: 6543 6c69 636b 6564 2c20 736c 6f74 3d70  eClicked, slot=p
+000127c0: 6172 7469 616c 285f 696e 7370 6563 745f  artial(_inspect_
+000127d0: 636c 6963 6b65 642c 2061 782c 2069 6e73  clicked, ax, ins
+000127e0: 7065 6374 6f72 2c20 5472 7565 2929 0d0a  pector, True))..
+000127f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00012800: 2020 206d 6173 7465 722e 7072 6f78 795f     master.proxy_
+00012810: 636c 6963 6b20 3d20 7067 2e53 6967 6e61  click = pg.Signa
+00012820: 6c50 726f 7879 286d 6173 7465 722e 7363  lProxy(master.sc
+00012830: 656e 6528 292e 7369 674d 6f75 7365 436c  ene().sigMouseCl
+00012840: 6963 6b65 642c 2073 6c6f 743d 7061 7274  icked, slot=part
+00012850: 6961 6c28 5f69 6e73 7065 6374 5f63 6c69  ial(_inspect_cli
+00012860: 636b 6564 2c20 6178 2c20 696e 7370 6563  cked, ax, inspec
+00012870: 746f 722c 2046 616c 7365 2929 0d0a 0d0a  tor, False))....
+00012880: 0d0a 6465 6620 6164 645f 6372 6f73 7368  ..def add_crossh
+00012890: 6169 725f 696e 666f 2869 6e66 6f66 756e  air_info(infofun
+000128a0: 632c 2061 783d 4e6f 6e65 293a 0d0a 2020  c, ax=None):..  
+000128b0: 2020 2727 2743 616c 6c62 6163 6b20 7768    '''Callback wh
+000128c0: 656e 2063 726f 7373 6861 6972 2075 7064  en crosshair upd
+000128d0: 6174 6564 206c 696b 6520 736f 3a20 696e  ated like so: in
+000128e0: 666f 2861 782c 782c 792c 7874 6578 742c  fo(ax,x,y,xtext,
+000128f0: 7974 6578 7429 3b20 7468 6520 696e 666f  ytext); the info
+00012900: 2829 0d0a 2020 2020 2020 2063 616c 6c62  ()..       callb
+00012910: 6163 6b20 6d75 7374 2072 6574 7572 6e20  ack must return 
+00012920: 7477 6f20 7661 6c75 6573 3a20 7874 6578  two values: xtex
+00012930: 7420 616e 6420 7974 6578 742e 2727 270d  t and ytext.'''.
+00012940: 0a20 2020 2061 7820 3d20 5f63 7265 6174  .    ax = _creat
+00012950: 655f 706c 6f74 2861 783d 6178 2c20 6d61  e_plot(ax=ax, ma
+00012960: 7869 6d69 7a65 3d46 616c 7365 290d 0a20  ximize=False).. 
+00012970: 2020 2061 782e 6372 6f73 7368 6169 722e     ax.crosshair.
+00012980: 696e 666f 732e 6170 7065 6e64 2869 6e66  infos.append(inf
+00012990: 6f66 756e 6329 0d0a 0d0a 0d0a 6465 6620  ofunc)......def 
+000129a0: 7469 6d65 725f 6361 6c6c 6261 636b 2875  timer_callback(u
+000129b0: 7064 6174 655f 6675 6e63 2c20 7365 636f  pdate_func, seco
+000129c0: 6e64 732c 2073 696e 676c 655f 7368 6f74  nds, single_shot
+000129d0: 3d46 616c 7365 293a 0d0a 2020 2020 676c  =False):..    gl
+000129e0: 6f62 616c 2074 696d 6572 730d 0a20 2020  obal timers..   
+000129f0: 2074 696d 6572 203d 2051 7443 6f72 652e   timer = QtCore.
+00012a00: 5154 696d 6572 2829 0d0a 2020 2020 7469  QTimer()..    ti
+00012a10: 6d65 722e 7469 6d65 6f75 742e 636f 6e6e  mer.timeout.conn
+00012a20: 6563 7428 7570 6461 7465 5f66 756e 6329  ect(update_func)
+00012a30: 0d0a 2020 2020 6966 2073 696e 676c 655f  ..    if single_
+00012a40: 7368 6f74 3a0d 0a20 2020 2020 2020 2074  shot:..        t
+00012a50: 696d 6572 2e73 6574 5369 6e67 6c65 5368  imer.setSingleSh
+00012a60: 6f74 2854 7275 6529 0d0a 2020 2020 7469  ot(True)..    ti
+00012a70: 6d65 722e 7374 6172 7428 696e 7428 7365  mer.start(int(se
+00012a80: 636f 6e64 732a 3130 3030 2929 0d0a 2020  conds*1000))..  
+00012a90: 2020 7469 6d65 7273 2e61 7070 656e 6428    timers.append(
+00012aa0: 7469 6d65 7229 0d0a 2020 2020 7265 7475  timer)..    retu
+00012ab0: 726e 2074 696d 6572 0d0a 0d0a 0d0a 6465  rn timer......de
+00012ac0: 6620 6175 746f 7669 6577 7265 7374 6f72  f autoviewrestor
+00012ad0: 6528 656e 6162 6c65 3d54 7275 6529 3a0d  e(enable=True):.
+00012ae0: 0a20 2020 2027 2727 5265 7374 6f72 2066  .    '''Restor f
+00012af0: 756e 6374 696f 6e61 6c69 7479 2073 6176  unctionality sav
+00012b00: 6573 2076 6965 7720 7a6f 6f6d 2063 6f6f  es view zoom coo
+00012b10: 7264 696e 6174 6573 2077 6865 6e20 636c  rdinates when cl
+00012b20: 6f73 696e 6720 6120 7769 6e64 6f77 2c20  osing a window, 
+00012b30: 616e 640d 0a20 2020 2020 2020 6c6f 6164  and..       load
+00012b40: 2074 6865 6d20 7768 656e 2063 7265 6174   them when creat
+00012b50: 696e 6720 7468 6520 706c 6f74 2028 7769  ing the plot (wi
+00012b60: 7468 2074 6865 2073 616d 6520 6e61 6d65  th the same name
+00012b70: 2920 6167 6169 6e2e 2727 270d 0a20 2020  ) again.'''..   
+00012b80: 2067 6c6f 6261 6c20 7669 6577 7265 7374   global viewrest
+00012b90: 6f72 650d 0a20 2020 2076 6965 7772 6573  ore..    viewres
+00012ba0: 746f 7265 203d 2065 6e61 626c 650d 0a0d  tore = enable...
+00012bb0: 0a0d 0a64 6566 2072 6566 7265 7368 2829  ...def refresh()
+00012bc0: 3a0d 0a20 2020 2066 6f72 2077 696e 2069  :..    for win i
+00012bd0: 6e20 7769 6e64 6f77 733a 0d0a 2020 2020  n windows:..    
+00012be0: 2020 2020 6178 7320 3d20 7769 6e2e 6178      axs = win.ax
+00012bf0: 7320 2b20 5b61 7820 666f 7220 6178 2069  s + [ax for ax i
+00012c00: 6e20 6f76 6572 6c61 795f 6178 7320 6966  n overlay_axs if
+00012c10: 2061 782e 7662 2e77 696e 3d3d 7769 6e5d   ax.vb.win==win]
+00012c20: 0d0a 2020 2020 2020 2020 666f 7220 6178  ..        for ax
+00012c30: 2069 6e20 6178 733a 0d0a 2020 2020 2020   in axs:..      
+00012c40: 2020 2020 2020 5f69 6d70 726f 7665 5f73        _improve_s
+00012c50: 6967 6e69 6669 6361 6e74 7328 6178 290d  ignificants(ax).
+00012c60: 0a20 2020 2020 2020 2076 6273 203d 205b  .        vbs = [
+00012c70: 6178 2e76 6220 666f 7220 6178 2069 6e20  ax.vb for ax in 
+00012c80: 6178 735d 0d0a 2020 2020 2020 2020 666f  axs]..        fo
+00012c90: 7220 7662 2069 6e20 7662 733a 0d0a 2020  r vb in vbs:..  
+00012ca0: 2020 2020 2020 2020 2020 7662 2e70 7265            vb.pre
+00012cb0: 5f70 726f 6365 7373 5f64 6174 6128 290d  _process_data().
+00012cc0: 0a20 2020 2020 2020 2069 6620 7669 6577  .        if view
+00012cd0: 7265 7374 6f72 653a 0d0a 2020 2020 2020  restore:..      
+00012ce0: 2020 2020 2020 6966 205f 6c6f 6164 7769        if _loadwi
+00012cf0: 6e64 6174 6128 7769 6e29 3a0d 0a20 2020  ndata(win):..   
+00012d00: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00012d10: 7469 6e75 650d 0a20 2020 2020 2020 205f  tinue..        _
+00012d20: 7365 745f 6d61 785f 7a6f 6f6d 2876 6273  set_max_zoom(vbs
+00012d30: 290d 0a20 2020 2020 2020 2066 6f72 2076  )..        for v
+00012d40: 6220 696e 2076 6273 3a0d 0a20 2020 2020  b in vbs:..     
+00012d50: 2020 2020 2020 2064 6174 6173 7263 203d         datasrc =
+00012d60: 2076 622e 6461 7461 7372 635f 6f72 5f73   vb.datasrc_or_s
+00012d70: 7461 6e64 616c 6f6e 650d 0a20 2020 2020  tandalone..     
+00012d80: 2020 2020 2020 2069 6620 6461 7461 7372         if datasr
+00012d90: 6320 616e 6420 2876 622e 6c69 6e6b 6564  c and (vb.linked
+00012da0: 5669 6577 2830 2920 6973 204e 6f6e 6520  View(0) is None 
+00012db0: 6f72 2076 622e 6c69 6e6b 6564 5669 6577  or vb.linkedView
+00012dc0: 2830 292e 6461 7461 7372 6320 6973 204e  (0).datasrc is N
+00012dd0: 6f6e 6520 6f72 2076 622e 6d61 7374 6572  one or vb.master
+00012de0: 5f76 6965 7762 6f78 293a 0d0a 2020 2020  _viewbox):..    
+00012df0: 2020 2020 2020 2020 2020 2020 7662 2e75              vb.u
+00012e00: 7064 6174 655f 795f 7a6f 6f6d 2864 6174  pdate_y_zoom(dat
+00012e10: 6173 7263 2e69 6e69 745f 7830 2c20 6461  asrc.init_x0, da
+00012e20: 7461 7372 632e 696e 6974 5f78 3129 0d0a  tasrc.init_x1)..
+00012e30: 2020 2020 5f72 6570 6169 6e74 5f63 616e      _repaint_can
+00012e40: 646c 6573 2829 0d0a 2020 2020 666f 7220  dles()..    for 
+00012e50: 6d64 2069 6e20 6d61 7374 6572 5f64 6174  md in master_dat
+00012e60: 612e 7661 6c75 6573 2829 3a0d 0a20 2020  a.values():..   
+00012e70: 2020 2020 2066 6f72 2076 6220 696e 206d       for vb in m
+00012e80: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00012e90: 6966 2074 7970 6528 7662 2920 213d 2073  if type(vb) != s
+00012ea0: 7472 3a20 2320 6967 6e6f 7265 2027 6465  tr: # ignore 'de
+00012eb0: 6661 756c 7427 0d0a 2020 2020 2020 2020  fault'..        
+00012ec0: 2020 2020 2020 2020 5f6d 6f75 7365 5f6d          _mouse_m
+00012ed0: 6f76 6564 2877 696e 2c20 7662 2c20 4e6f  oved(win, vb, No
+00012ee0: 6e65 290d 0a0d 0a0d 0a64 6566 2073 686f  ne)......def sho
+00012ef0: 7728 7174 5f65 7865 633d 5472 7565 293a  w(qt_exec=True):
+00012f00: 0d0a 2020 2020 7265 6672 6573 6828 290d  ..    refresh().
+00012f10: 0a20 2020 2066 6f72 2077 696e 2069 6e20  .    for win in 
+00012f20: 7769 6e64 6f77 733a 0d0a 2020 2020 2020  windows:..      
+00012f30: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00012f40: 7769 6e2c 2046 696e 5769 6e64 6f77 2920  win, FinWindow) 
+00012f50: 6f72 2071 745f 6578 6563 3a0d 0a20 2020  or qt_exec:..   
+00012f60: 2020 2020 2020 2020 2069 6620 7769 6e2e           if win.
+00012f70: 7368 6f77 5f6d 6178 696d 697a 6564 3a0d  show_maximized:.
+00012f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012f90: 2077 696e 2e73 686f 774d 6178 696d 697a   win.showMaximiz
+00012fa0: 6564 2829 0d0a 2020 2020 2020 2020 2020  ed()..          
+00012fb0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00012fc0: 2020 2020 2020 2020 2077 696e 2e73 686f           win.sho
+00012fd0: 7728 290d 0a20 2020 2069 6620 7769 6e64  w()..    if wind
+00012fe0: 6f77 7320 616e 6420 7174 5f65 7865 633a  ows and qt_exec:
+00012ff0: 0d0a 2020 2020 2020 2020 676c 6f62 616c  ..        global
+00013000: 206c 6173 745f 6178 2c20 6170 700d 0a20   last_ax, app.. 
+00013010: 2020 2020 2020 2061 7070 203d 2051 7447         app = QtG
+00013020: 7569 2e51 4775 6941 7070 6c69 6361 7469  ui.QGuiApplicati
+00013030: 6f6e 2e69 6e73 7461 6e63 6528 290d 0a20  on.instance().. 
+00013040: 2020 2020 2020 2061 7070 2e65 7865 6328         app.exec(
+00013050: 290d 0a20 2020 2020 2020 2077 696e 646f  )..        windo
+00013060: 7773 2e63 6c65 6172 2829 0d0a 2020 2020  ws.clear()..    
+00013070: 2020 2020 6f76 6572 6c61 795f 6178 732e      overlay_axs.
+00013080: 636c 6561 7228 290d 0a20 2020 2020 2020  clear()..       
+00013090: 205f 636c 6561 725f 7469 6d65 7273 2829   _clear_timers()
+000130a0: 0d0a 2020 2020 2020 2020 736f 756e 6473  ..        sounds
+000130b0: 2e63 6c65 6172 2829 0d0a 2020 2020 2020  .clear()..      
+000130c0: 2020 6d61 7374 6572 5f64 6174 612e 636c    master_data.cl
+000130d0: 6561 7228 290d 0a20 2020 2020 2020 206c  ear()..        l
+000130e0: 6173 745f 6178 203d 204e 6f6e 650d 0a0d  ast_ax = None...
+000130f0: 0a0d 0a64 6566 2070 6c61 795f 736f 756e  ...def play_soun
+00013100: 6428 6669 6c65 6e61 6d65 293a 0d0a 2020  d(filename):..  
+00013110: 2020 6966 2066 696c 656e 616d 6520 6e6f    if filename no
+00013120: 7420 696e 2073 6f75 6e64 733a 0d0a 2020  t in sounds:..  
+00013130: 2020 2020 2020 6672 6f6d 2050 7951 7436        from PyQt6
+00013140: 2e51 744d 756c 7469 6d65 6469 6120 696d  .QtMultimedia im
+00013150: 706f 7274 2051 536f 756e 6445 6666 6563  port QSoundEffec
+00013160: 740d 0a20 2020 2020 2020 2073 203d 2073  t..        s = s
+00013170: 6f75 6e64 735b 6669 6c65 6e61 6d65 5d20  ounds[filename] 
+00013180: 3d20 5153 6f75 6e64 4566 6665 6374 2829  = QSoundEffect()
+00013190: 2023 2064 6973 616c 6c6f 7720 6763 0d0a   # disallow gc..
+000131a0: 2020 2020 2020 2020 732e 7365 7453 6f75          s.setSou
+000131b0: 7263 6528 5174 436f 7265 2e51 5572 6c2e  rce(QtCore.QUrl.
+000131c0: 6672 6f6d 4c6f 6361 6c46 696c 6528 6669  fromLocalFile(fi
+000131d0: 6c65 6e61 6d65 2929 0d0a 2020 2020 7320  lename))..    s 
+000131e0: 3d20 736f 756e 6473 5b66 696c 656e 616d  = sounds[filenam
+000131f0: 655d 0d0a 2020 2020 732e 706c 6179 2829  e]..    s.play()
+00013200: 0d0a 0d0a 0d0a 6465 6620 7363 7265 656e  ......def screen
+00013210: 7368 6f74 2866 696c 652c 2066 6d74 3d27  shot(file, fmt='
+00013220: 706e 6727 293a 0d0a 2020 2020 6966 205f  png'):..    if _
+00013230: 696e 7465 726e 616c 5f77 696e 646f 7773  internal_windows
+00013240: 5f6f 6e6c 7928 2920 616e 6420 6e6f 7420  _only() and not 
+00013250: 6170 703a 0d0a 2020 2020 2020 2020 7072  app:..        pr
+00013260: 696e 7428 2745 5252 4f52 3a20 7363 7265  int('ERROR: scre
+00013270: 656e 7368 6f74 206d 7573 7420 6265 2063  enshot must be c
+00013280: 616c 6c62 6163 6b65 6420 6672 6f6d 2065  allbacked from e
+00013290: 2e67 2e20 7469 6d65 725f 6361 6c6c 6261  .g. timer_callba
+000132a0: 636b 2829 2729 0d0a 2020 2020 2020 2020  ck()')..        
+000132b0: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
+000132c0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000132d0: 6275 6666 6572 203d 2051 7443 6f72 652e  buffer = QtCore.
+000132e0: 5142 7566 6665 7228 290d 0a20 2020 2020  QBuffer()..     
+000132f0: 2020 2061 7070 2e70 7269 6d61 7279 5363     app.primarySc
+00013300: 7265 656e 2829 2e67 7261 6257 696e 646f  reen().grabWindo
+00013310: 7728 7769 6e64 6f77 735b 305d 2e77 696e  w(windows[0].win
+00013320: 4964 2829 292e 7361 7665 2862 7566 6665  Id()).save(buffe
+00013330: 722c 2066 6d74 290d 0a20 2020 2020 2020  r, fmt)..       
+00013340: 2066 696c 652e 7772 6974 6528 6275 6666   file.write(buff
+00013350: 6572 2e64 6174 6128 2929 0d0a 2020 2020  er.data())..    
+00013360: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+00013370: 0a20 2020 2065 7863 6570 7420 4578 6365  .    except Exce
+00013380: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
+00013390: 2020 2020 2070 7269 6e74 2827 5363 7265       print('Scre
+000133a0: 656e 7368 6f74 2065 7272 6f72 3a27 2c20  enshot error:', 
+000133b0: 7479 7065 2865 292c 2065 290d 0a20 2020  type(e), e)..   
+000133c0: 2072 6574 7572 6e20 4661 6c73 650d 0a0d   return False...
+000133d0: 0a0d 0a64 6566 2065 7870 6572 696d 656e  ...def experimen
+000133e0: 7428 2a61 7267 732c 202a 2a6b 7761 7267  t(*args, **kwarg
+000133f0: 7329 3a0d 0a20 2020 2069 6620 276f 7065  s):..    if 'ope
+00013400: 6e67 6c27 2069 6e20 6172 6773 206f 7220  ngl' in args or 
+00013410: 6b77 6172 6773 2e67 6574 2827 6f70 656e  kwargs.get('open
+00013420: 676c 2729 3a0d 0a20 2020 2020 2020 2074  gl'):..        t
+00013430: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00013440: 2023 2070 6970 2069 6e73 7461 6c6c 2050   # pip install P
+00013450: 794f 7065 6e47 4c20 5079 4f70 656e 474c  yOpenGL PyOpenGL
+00013460: 2d61 6363 656c 6572 6174 6520 746f 2067  -accelerate to g
+00013470: 6574 2074 6869 7320 676f 696e 670d 0a20  et this going.. 
+00013480: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
+00013490: 7420 4f70 656e 474c 0d0a 2020 2020 2020  t OpenGL..      
+000134a0: 2020 2020 2020 7067 2e73 6574 436f 6e66        pg.setConf
+000134b0: 6967 4f70 7469 6f6e 7328 7573 654f 7065  igOptions(useOpe
+000134c0: 6e47 4c3d 5472 7565 2c20 656e 6162 6c65  nGL=True, enable
+000134d0: 4578 7065 7269 6d65 6e74 616c 3d54 7275  Experimental=Tru
+000134e0: 6529 0d0a 2020 2020 2020 2020 6578 6365  e)..        exce
+000134f0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00013500: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00013510: 7072 696e 7428 2757 4152 4e49 4e47 3a20  print('WARNING: 
+00013520: 4f70 656e 474c 2069 6e69 7420 6572 726f  OpenGL init erro
+00013530: 722e 272c 2074 7970 6528 6529 2c20 6529  r.', type(e), e)
+00013540: 0d0a 0d0a 0d0a 2323 2323 2323 2323 2323  ......##########
+00013550: 2323 2323 2323 2323 2323 2049 4e54 4552  ########## INTER
+00013560: 4e41 4c53 2023 2323 2323 2323 2323 2323  NALS ###########
+00013570: 2323 2323 2323 2323 230d 0a0d 0a0d 0a64  #########......d
+00013580: 6566 205f 6f70 656e 6669 6c65 282a 6172  ef _openfile(*ar
+00013590: 6773 293a 0d0a 2020 2020 7265 7475 726e  gs):..    return
+000135a0: 206f 7065 6e28 2a61 7267 7329 0d0a 0d0a   open(*args)....
+000135b0: 0d0a 6465 6620 5f6c 6f61 6477 696e 6461  ..def _loadwinda
+000135c0: 7461 2877 696e 293a 0d0a 2020 2020 7472  ta(win):..    tr
+000135d0: 793a 206f 732e 6d6b 6469 7228 6f73 2e70  y: os.mkdir(os.p
+000135e0: 6174 682e 6578 7061 6e64 7573 6572 2827  ath.expanduser('
+000135f0: 7e2f 2e66 696e 706c 6f74 2729 290d 0a20  ~/.finplot')).. 
+00013600: 2020 2065 7863 6570 743a 2070 6173 730d     except: pass.
+00013610: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
+00013620: 2020 2066 203d 206f 732e 7061 7468 2e65     f = os.path.e
+00013630: 7870 616e 6475 7365 7228 277e 2f2e 6669  xpanduser('~/.fi
+00013640: 6e70 6c6f 742f 272b 7769 6e2e 7469 746c  nplot/'+win.titl
+00013650: 652e 7265 706c 6163 6528 272f 272c 272d  e.replace('/','-
+00013660: 2729 2b27 2e69 6e69 2729 0d0a 2020 2020  ')+'.ini')..    
+00013670: 2020 2020 7365 7474 696e 6773 203d 205b      settings = [
+00013680: 286b 2e73 7472 6970 2829 2c6c 6974 6572  (k.strip(),liter
+00013690: 616c 5f65 7661 6c28 762e 7374 7269 7028  al_eval(v.strip(
+000136a0: 2929 2920 666f 7220 6c69 6e65 2069 6e20  ))) for line in 
+000136b0: 5f6f 7065 6e66 696c 6528 6629 2066 6f72  _openfile(f) for
+000136c0: 206b 2c64 2c76 2069 6e20 5b6c 696e 652e   k,d,v in [line.
+000136d0: 7061 7274 6974 696f 6e28 273d 2729 5d20  partition('=')] 
+000136e0: 6966 2076 5d0d 0a20 2020 2020 2020 2069  if v]..        i
+000136f0: 6620 6e6f 7420 7365 7474 696e 6773 3a0d  f not settings:.
+00013700: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00013710: 7572 6e0d 0a20 2020 2065 7863 6570 743a  urn..    except:
+00013720: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00013730: 0d0a 2020 2020 6b76 7320 3d20 7b6b 3a76  ..    kvs = {k:v
+00013740: 2066 6f72 206b 2c76 2069 6e20 7365 7474   for k,v in sett
+00013750: 696e 6773 7d0d 0a20 2020 2076 6273 203d  ings}..    vbs =
+00013760: 2073 6574 2861 782e 7662 2066 6f72 2061   set(ax.vb for a
+00013770: 7820 696e 2077 696e 2e61 7873 290d 0a20  x in win.axs).. 
+00013780: 2020 207a 6f6f 6d5f 7365 7420 3d20 4661     zoom_set = Fa
+00013790: 6c73 650d 0a20 2020 2066 6f72 2076 6220  lse..    for vb 
+000137a0: 696e 2076 6273 3a0d 0a20 2020 2020 2020  in vbs:..       
+000137b0: 2064 7320 3d20 7662 2e64 6174 6173 7263   ds = vb.datasrc
+000137c0: 0d0a 2020 2020 2020 2020 6966 2064 7320  ..        if ds 
+000137d0: 616e 6420 2876 622e 6c69 6e6b 6564 5669  and (vb.linkedVi
+000137e0: 6577 2830 2920 6973 204e 6f6e 6520 6f72  ew(0) is None or
+000137f0: 2076 622e 6c69 6e6b 6564 5669 6577 2830   vb.linkedView(0
+00013800: 292e 6461 7461 7372 6320 6973 204e 6f6e  ).datasrc is Non
+00013810: 6520 6f72 2076 622e 6d61 7374 6572 5f76  e or vb.master_v
+00013820: 6965 7762 6f78 293a 0d0a 2020 2020 2020  iewbox):..      
+00013830: 2020 2020 2020 7065 7269 6f64 5f6e 7320        period_ns 
+00013840: 3d20 6473 2e70 6572 696f 645f 6e73 0d0a  = ds.period_ns..
+00013850: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00013860: 7673 5b27 6d69 6e5f 7827 5d20 3e3d 2064  vs['min_x'] >= d
+00013870: 732e 782e 696c 6f63 5b30 5d2d 7065 7269  s.x.iloc[0]-peri
+00013880: 6f64 5f6e 7320 616e 6420 6b76 735b 276d  od_ns and kvs['m
+00013890: 6178 5f78 275d 203c 3d20 6473 2e78 2e69  ax_x'] <= ds.x.i
+000138a0: 6c6f 635b 2d31 5d2b 7065 7269 6f64 5f6e  loc[-1]+period_n
+000138b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000138c0: 2020 2020 7830 2c78 3120 3d20 6473 2e78      x0,x1 = ds.x
+000138d0: 2e6c 6f63 5b64 732e 783e 3d6b 7673 5b27  .loc[ds.x>=kvs['
+000138e0: 6d69 6e5f 7827 5d5d 2e69 6e64 6578 5b30  min_x']].index[0
+000138f0: 5d2c 2064 732e 782e 6c6f 635b 6473 2e78  ], ds.x.loc[ds.x
+00013900: 3c3d 6b76 735b 276d 6178 5f78 275d 5d2e  <=kvs['max_x']].
+00013910: 696e 6465 785b 2d31 5d0d 0a20 2020 2020  index[-1]..     
+00013920: 2020 2020 2020 2020 2020 2069 6620 7831             if x1
+00013930: 203d 3d20 6c65 6e28 6473 2e78 292d 313a   == len(ds.x)-1:
+00013940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013950: 2020 2020 2020 7831 202b 3d20 7269 6768        x1 += righ
+00013960: 745f 6d61 7267 696e 5f63 616e 646c 6573  t_margin_candles
+00013970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013980: 2020 7831 202b 3d20 302e 350d 0a20 2020    x1 += 0.5..   
+00013990: 2020 2020 2020 2020 2020 2020 207a 6f6f               zoo
+000139a0: 6d5f 7365 7420 3d20 7662 2e75 7064 6174  m_set = vb.updat
+000139b0: 655f 795f 7a6f 6f6d 2878 302c 2078 3129  e_y_zoom(x0, x1)
+000139c0: 0d0a 2020 2020 7265 7475 726e 207a 6f6f  ..    return zoo
+000139d0: 6d5f 7365 740d 0a0d 0a0d 0a64 6566 205f  m_set......def _
+000139e0: 7361 7665 7769 6e64 6174 6128 7769 6e29  savewindata(win)
+000139f0: 3a0d 0a20 2020 2069 6620 6e6f 7420 7669  :..    if not vi
+00013a00: 6577 7265 7374 6f72 653a 0d0a 2020 2020  ewrestore:..    
+00013a10: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
+00013a20: 7472 793a 0d0a 2020 2020 2020 2020 6d69  try:..        mi
+00013a30: 6e5f 7820 3d20 696e 7428 3165 3130 3029  n_x = int(1e100)
+00013a40: 0d0a 2020 2020 2020 2020 6d61 785f 7820  ..        max_x 
+00013a50: 3d20 696e 7428 2d31 6531 3030 290d 0a20  = int(-1e100).. 
+00013a60: 2020 2020 2020 2066 6f72 2061 7820 696e         for ax in
+00013a70: 2077 696e 2e61 7873 3a0d 0a20 2020 2020   win.axs:..     
+00013a80: 2020 2020 2020 2069 6620 6178 2e76 622e         if ax.vb.
+00013a90: 7461 7267 6574 5265 6374 2829 2e72 6967  targetRect().rig
+00013aa0: 6874 2829 203c 2034 3a20 2320 6967 6e6f  ht() < 4: # igno
+00013ab0: 7265 2065 6d70 7479 2070 6c6f 7473 0d0a  re empty plots..
+00013ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ad0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00013ae0: 2020 2020 2020 6966 2061 782e 7662 2e64        if ax.vb.d
+00013af0: 6174 6173 7263 2069 7320 4e6f 6e65 3a0d  atasrc is None:.
+00013b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b10: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00013b20: 2020 2020 2020 2074 302c 7431 2c5f 2c5f         t0,t1,_,_
+00013b30: 2c5f 203d 2061 782e 7662 2e64 6174 6173  ,_ = ax.vb.datas
+00013b40: 7263 2e68 696c 6f28 6178 2e76 622e 7461  rc.hilo(ax.vb.ta
+00013b50: 7267 6574 5265 6374 2829 2e6c 6566 7428  rgetRect().left(
+00013b60: 292c 2061 782e 7662 2e74 6172 6765 7452  ), ax.vb.targetR
+00013b70: 6563 7428 292e 7269 6768 7428 2929 0d0a  ect().right())..
+00013b80: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
+00013b90: 7820 3d20 6e70 2e6e 616e 6d69 6e28 5b6d  x = np.nanmin([m
+00013ba0: 696e 5f78 2c20 7430 5d29 0d0a 2020 2020  in_x, t0])..    
+00013bb0: 2020 2020 2020 2020 6d61 785f 7820 3d20          max_x = 
+00013bc0: 6e70 2e6e 616e 6d61 7828 5b6d 6178 5f78  np.nanmax([max_x
+00013bd0: 2c20 7431 5d29 0d0a 2020 2020 2020 2020  , t1])..        
+00013be0: 6966 206e 702e 6d61 7828 6e70 2e61 6273  if np.max(np.abs
+00013bf0: 285b 6d69 6e5f 782c 206d 6178 5f78 5d29  ([min_x, max_x])
+00013c00: 2920 3c20 3165 3939 3a0d 0a20 2020 2020  ) < 1e99:..     
+00013c10: 2020 2020 2020 2073 203d 2027 6d69 6e5f         s = 'min_
+00013c20: 7820 3d20 2573 5c6e 6d61 785f 7820 3d20  x = %s\nmax_x = 
+00013c30: 2573 5c6e 2720 2520 286d 696e 5f78 2c20  %s\n' % (min_x, 
+00013c40: 6d61 785f 7829 0d0a 2020 2020 2020 2020  max_x)..        
+00013c50: 2020 2020 6620 3d20 6f73 2e70 6174 682e      f = os.path.
+00013c60: 6578 7061 6e64 7573 6572 2827 7e2f 2e66  expanduser('~/.f
+00013c70: 696e 706c 6f74 2f27 2b77 696e 2e74 6974  inplot/'+win.tit
+00013c80: 6c65 2e72 6570 6c61 6365 2827 2f27 2c27  le.replace('/','
+00013c90: 2d27 292b 272e 696e 6927 290d 0a20 2020  -')+'.ini')..   
+00013ca0: 2020 2020 2020 2020 2074 7279 3a20 6368           try: ch
+00013cb0: 616e 6765 6420 3d20 5f6f 7065 6e66 696c  anged = _openfil
+00013cc0: 6528 6629 2e72 6561 6428 2920 213d 2073  e(f).read() != s
+00013cd0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00013ce0: 6365 7074 3a20 6368 616e 6765 6420 3d20  cept: changed = 
+00013cf0: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+00013d00: 2020 6966 2063 6861 6e67 6564 3a0d 0a20    if changed:.. 
+00013d10: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00013d20: 6f70 656e 6669 6c65 2866 2c20 2777 7427  openfile(f, 'wt'
+00013d30: 292e 7772 6974 6528 7329 0d0a 2020 2020  ).write(s)..    
+00013d40: 2020 2020 2020 2020 2020 2020 2323 2070              ## p
+00013d50: 7269 6e74 2827 2573 2073 6176 6564 2720  rint('%s saved' 
+00013d60: 2520 7769 6e2e 7469 746c 6529 0d0a 2020  % win.title)..  
+00013d70: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00013d80: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+00013d90: 2020 7072 696e 7428 2745 7272 6f72 2073    print('Error s
+00013da0: 6176 696e 6720 706c 6f74 3a27 2c20 6529  aving plot:', e)
+00013db0: 0d0a 0d0a 0d0a 6465 6620 5f69 6e74 6572  ......def _inter
+00013dc0: 6e61 6c5f 7769 6e64 6f77 735f 6f6e 6c79  nal_windows_only
+00013dd0: 2829 3a0d 0a20 2020 2020 7265 7475 726e  ():..     return
+00013de0: 2061 6c6c 2869 7369 6e73 7461 6e63 6528   all(isinstance(
+00013df0: 7769 6e2c 4669 6e57 696e 646f 7729 2066  win,FinWindow) f
+00013e00: 6f72 2077 696e 2069 6e20 7769 6e64 6f77  or win in window
+00013e10: 7329 0d0a 0d0a 0d0a 6465 6620 5f63 7265  s)......def _cre
+00013e20: 6174 655f 706c 6f74 2861 783d 4e6f 6e65  ate_plot(ax=None
+00013e30: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+00013e40: 2020 6966 2061 783a 0d0a 2020 2020 2020    if ax:..      
+00013e50: 2020 7265 7475 726e 2061 780d 0a20 2020    return ax..   
+00013e60: 2069 6620 6c61 7374 5f61 783a 0d0a 2020   if last_ax:..  
+00013e70: 2020 2020 2020 7265 7475 726e 206c 6173        return las
+00013e80: 745f 6178 0d0a 2020 2020 7265 7475 726e  t_ax..    return
+00013e90: 2063 7265 6174 655f 706c 6f74 282a 2a6b   create_plot(**k
+00013ea0: 7761 7267 7329 0d0a 0d0a 0d0a 6465 6620  wargs)......def 
+00013eb0: 5f63 7265 6174 655f 6178 6973 2870 6f73  _create_axis(pos
+00013ec0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+00013ed0: 2020 6966 2070 6f73 203d 3d20 2778 273a    if pos == 'x':
+00013ee0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00013ef0: 2045 706f 6368 4178 6973 4974 656d 282a   EpochAxisItem(*
+00013f00: 2a6b 7761 7267 7329 0d0a 2020 2020 656c  *kwargs)..    el
+00013f10: 6966 2070 6f73 203d 3d20 2779 273a 0d0a  if pos == 'y':..
+00013f20: 2020 2020 2020 2020 7265 7475 726e 2059          return Y
+00013f30: 4178 6973 4974 656d 282a 2a6b 7761 7267  AxisItem(**kwarg
+00013f40: 7329 0d0a 0d0a 0d0a 6465 6620 5f63 6c65  s)......def _cle
+00013f50: 6172 5f74 696d 6572 7328 293a 0d0a 2020  ar_timers():..  
+00013f60: 2020 666f 7220 7469 6d65 7220 696e 2074    for timer in t
+00013f70: 696d 6572 733a 0d0a 2020 2020 2020 2020  imers:..        
+00013f80: 7469 6d65 722e 7469 6d65 6f75 742e 6469  timer.timeout.di
+00013f90: 7363 6f6e 6e65 6374 2829 0d0a 2020 2020  sconnect()..    
+00013fa0: 7469 6d65 7273 2e63 6c65 6172 2829 0d0a  timers.clear()..
+00013fb0: 0d0a 0d0a 6465 6620 5f61 6464 5f74 696d  ....def _add_tim
+00013fc0: 6573 7461 6d70 5f70 6c6f 7428 6d61 7374  estamp_plot(mast
+00013fd0: 6572 2c20 7072 6576 5f61 782c 2076 6965  er, prev_ax, vie
+00013fe0: 7762 6f78 2c20 696e 6465 782c 2079 7363  wbox, index, ysc
+00013ff0: 616c 6529 3a0d 0a20 2020 206e 6174 6976  ale):..    nativ
+00014000: 655f 7769 6e20 3d20 6973 696e 7374 616e  e_win = isinstan
+00014010: 6365 286d 6173 7465 722c 2070 672e 4772  ce(master, pg.Gr
+00014020: 6170 6869 6373 4c61 796f 7574 5769 6467  aphicsLayoutWidg
+00014030: 6574 290d 0a20 2020 2069 6620 6e61 7469  et)..    if nati
+00014040: 7665 5f77 696e 2061 6e64 2070 7265 765f  ve_win and prev_
+00014050: 6178 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ax is not None:.
+00014060: 0a20 2020 2020 2020 2070 7265 765f 6178  .        prev_ax
+00014070: 2e73 6574 5f76 6973 6962 6c65 2878 6178  .set_visible(xax
+00014080: 6973 3d46 616c 7365 2920 2320 6869 6465  is=False) # hide
+00014090: 2074 6865 2077 686f 6c65 2070 7265 7669   the whole previ
+000140a0: 6f75 7320 6178 6973 0d0a 2020 2020 6178  ous axis..    ax
+000140b0: 6573 203d 207b 2762 6f74 746f 6d27 3a20  es = {'bottom': 
+000140c0: 5f63 7265 6174 655f 6178 6973 2870 6f73  _create_axis(pos
+000140d0: 3d27 7827 2c20 7662 3d76 6965 7762 6f78  ='x', vb=viewbox
+000140e0: 2c20 6f72 6965 6e74 6174 696f 6e3d 2762  , orientation='b
+000140f0: 6f74 746f 6d27 292c 0d0a 2020 2020 2020  ottom'),..      
+00014100: 2020 2020 2020 2772 6967 6874 273a 2020        'right':  
+00014110: 5f63 7265 6174 655f 6178 6973 2870 6f73  _create_axis(pos
+00014120: 3d27 7927 2c20 7662 3d76 6965 7762 6f78  ='y', vb=viewbox
+00014130: 2c20 6f72 6965 6e74 6174 696f 6e3d 2772  , orientation='r
+00014140: 6967 6874 2729 7d0d 0a20 2020 2069 6620  ight')}..    if 
+00014150: 6e61 7469 7665 5f77 696e 3a0d 0a20 2020  native_win:..   
+00014160: 2020 2020 2061 7820 3d20 7067 2e50 6c6f       ax = pg.Plo
+00014170: 7449 7465 6d28 7669 6577 426f 783d 7669  tItem(viewBox=vi
+00014180: 6577 626f 782c 2061 7869 7349 7465 6d73  ewbox, axisItems
+00014190: 3d61 7865 732c 206e 616d 653d 2770 6c6f  =axes, name='plo
+000141a0: 742d 2569 2725 696e 6465 782c 2065 6e61  t-%i'%index, ena
+000141b0: 626c 654d 656e 753d 4661 6c73 6529 0d0a  bleMenu=False)..
+000141c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000141d0: 2020 2061 7877 203d 2070 672e 506c 6f74     axw = pg.Plot
+000141e0: 5769 6467 6574 2876 6965 7742 6f78 3d76  Widget(viewBox=v
+000141f0: 6965 7762 6f78 2c20 6178 6973 4974 656d  iewbox, axisItem
+00014200: 733d 6178 6573 2c20 6e61 6d65 3d27 706c  s=axes, name='pl
+00014210: 6f74 2d25 6927 2569 6e64 6578 2c20 656e  ot-%i'%index, en
+00014220: 6162 6c65 4d65 6e75 3d46 616c 7365 290d  ableMenu=False).
+00014230: 0a20 2020 2020 2020 2061 7820 3d20 6178  .        ax = ax
+00014240: 772e 706c 6f74 4974 656d 0d0a 2020 2020  w.plotItem..    
+00014250: 2020 2020 6178 2e61 785f 7769 6467 6574      ax.ax_widget
+00014260: 203d 2061 7877 0d0a 2020 2020 6178 2e68   = axw..    ax.h
+00014270: 6964 6541 7869 7328 276c 6566 7427 290d  ideAxis('left').
+00014280: 0a20 2020 2069 6620 795f 6c61 6265 6c5f  .    if y_label_
+00014290: 7769 6474 683a 0d0a 2020 2020 2020 2020  width:..        
+000142a0: 6178 2e61 7865 735b 2772 6967 6874 275d  ax.axes['right']
+000142b0: 5b27 6974 656d 275d 2e73 6574 5769 6474  ['item'].setWidt
+000142c0: 6828 795f 6c61 6265 6c5f 7769 6474 6829  h(y_label_width)
+000142d0: 2023 2074 6869 7320 6973 2074 6f20 7075   # this is to pu
+000142e0: 7420 616c 6c20 6772 6170 6873 206f 6e20  t all graphs on 
+000142f0: 6571 7561 6c20 666f 6f74 696e 6720 7768  equal footing wh
+00014300: 656e 2074 6578 7473 2076 6172 7920 6672  en texts vary fr
+00014310: 6f6d 2030 2e34 2074 6f20 3230 3030 3030  om 0.4 to 200000
+00014320: 300d 0a20 2020 2061 782e 6178 6573 5b27  0..    ax.axes['
+00014330: 7269 6768 7427 5d5b 2769 7465 6d27 5d2e  right']['item'].
+00014340: 7365 7453 7479 6c65 2874 6963 6b4c 656e  setStyle(tickLen
+00014350: 6774 683d 2d35 2920 2320 736f 6d65 2062  gth=-5) # some b
+00014360: 7567 2c20 746f 7461 6c6c 7920 756e 6578  ug, totally unex
+00014370: 706c 6963 6162 6c65 2028 7768 7920 7365  plicable (why se
+00014380: 7474 696e 6720 7468 6520 6465 6661 756c  tting the defaul
+00014390: 7420 7661 6c75 6520 6167 6169 6e20 776f  t value again wo
+000143a0: 756c 6420 6669 7820 7265 7061 696e 7420  uld fix repaint 
+000143b0: 7769 6474 6820 6173 2061 7869 7320 7363  width as axis sc
+000143c0: 616c 6520 646f 776e 290d 0a20 2020 2061  ale down)..    a
+000143d0: 782e 6178 6573 5b27 7269 6768 7427 5d5b  x.axes['right'][
+000143e0: 2769 7465 6d27 5d2e 7365 745a 5661 6c75  'item'].setZValu
+000143f0: 6528 3330 2920 2320 7075 7420 6178 6973  e(30) # put axis
+00014400: 2069 6e20 6672 6f6e 7420 696e 7374 6561   in front instea
+00014410: 6420 6f66 2062 6568 696e 6420 6461 7461  d of behind data
+00014420: 0d0a 2020 2020 6178 2e61 7865 735b 2762  ..    ax.axes['b
+00014430: 6f74 746f 6d27 5d5b 2769 7465 6d27 5d2e  ottom']['item'].
+00014440: 7365 745a 5661 6c75 6528 3330 290d 0a20  setZValue(30).. 
+00014450: 2020 2061 782e 7365 744c 6f67 4d6f 6465     ax.setLogMode
+00014460: 2879 3d28 7973 6361 6c65 2e73 6361 6c65  (y=(yscale.scale
+00014470: 7479 7065 3d3d 276c 6f67 2729 290d 0a20  type=='log')).. 
+00014480: 2020 2061 782e 7369 676e 6966 6963 616e     ax.significan
+00014490: 745f 666f 7263 6564 203d 2046 616c 7365  t_forced = False
+000144a0: 0d0a 2020 2020 6178 2e73 6967 6e69 6669  ..    ax.signifi
+000144b0: 6361 6e74 5f64 6563 696d 616c 7320 3d20  cant_decimals = 
+000144c0: 7369 676e 6966 6963 616e 745f 6465 6369  significant_deci
+000144d0: 6d61 6c73 0d0a 2020 2020 6178 2e73 6967  mals..    ax.sig
+000144e0: 6e69 6669 6361 6e74 5f65 7073 203d 2073  nificant_eps = s
+000144f0: 6967 6e69 6669 6361 6e74 5f65 7073 0d0a  ignificant_eps..
+00014500: 2020 2020 6178 2e63 726f 7373 6861 6972      ax.crosshair
+00014510: 203d 2046 696e 4372 6f73 7348 6169 7228   = FinCrossHair(
+00014520: 6178 2c20 636f 6c6f 723d 6372 6f73 735f  ax, color=cross_
+00014530: 6861 6972 5f63 6f6c 6f72 290d 0a20 2020  hair_color)..   
+00014540: 2061 782e 6869 6465 4275 7474 6f6e 7328   ax.hideButtons(
+00014550: 290d 0a20 2020 2061 782e 6f76 6572 6c61  )..    ax.overla
+00014560: 7920 3d20 7061 7274 6961 6c28 5f61 785f  y = partial(_ax_
+00014570: 6f76 6572 6c61 792c 2061 7829 0d0a 2020  overlay, ax)..  
+00014580: 2020 6178 2e73 6574 5f76 6973 6962 6c65    ax.set_visible
+00014590: 203d 2070 6172 7469 616c 285f 6178 5f73   = partial(_ax_s
+000145a0: 6574 5f76 6973 6962 6c65 2c20 6178 290d  et_visible, ax).
+000145b0: 0a20 2020 2061 782e 6465 636f 7570 6c65  .    ax.decouple
+000145c0: 203d 2070 6172 7469 616c 285f 6178 5f64   = partial(_ax_d
+000145d0: 6563 6f75 706c 652c 2061 7829 0d0a 2020  ecouple, ax)..  
+000145e0: 2020 6178 2e64 6973 6162 6c65 5f78 5f69    ax.disable_x_i
+000145f0: 6e64 6578 203d 2070 6172 7469 616c 285f  ndex = partial(_
+00014600: 6178 5f64 6973 6162 6c65 5f78 5f69 6e64  ax_disable_x_ind
+00014610: 6578 2c20 6178 290d 0a20 2020 2061 782e  ex, ax)..    ax.
+00014620: 7265 7365 7420 3d20 7061 7274 6961 6c28  reset = partial(
+00014630: 5f61 785f 7265 7365 742c 2061 7829 0d0a  _ax_reset, ax)..
+00014640: 2020 2020 6178 2e70 7265 765f 6178 203d      ax.prev_ax =
+00014650: 2070 7265 765f 6178 0d0a 2020 2020 6178   prev_ax..    ax
+00014660: 2e77 696e 5f69 6e64 6578 203d 2069 6e64  .win_index = ind
+00014670: 6578 0d0a 2020 2020 6966 2069 6e64 6578  ex..    if index
+00014680: 2532 3a0d 0a20 2020 2020 2020 2076 6965  %2:..        vie
+00014690: 7762 6f78 2e73 6574 4261 636b 6772 6f75  wbox.setBackgrou
+000146a0: 6e64 436f 6c6f 7228 6f64 645f 706c 6f74  ndColor(odd_plot
+000146b0: 5f62 6163 6b67 726f 756e 6429 0d0a 2020  _background)..  
+000146c0: 2020 7669 6577 626f 782e 7365 7450 6172    viewbox.setPar
+000146d0: 656e 7428 6178 290d 0a20 2020 2072 6574  ent(ax)..    ret
+000146e0: 7572 6e20 6178 0d0a 0d0a 0d0a 6465 6620  urn ax......def 
+000146f0: 5f61 785f 6f76 6572 6c61 7928 6178 2c20  _ax_overlay(ax, 
+00014700: 7363 616c 653d 302e 3235 2c20 7961 7869  scale=0.25, yaxi
+00014710: 733d 4661 6c73 6529 3a0d 0a20 2020 2027  s=False):..    '
+00014720: 2727 5468 6520 7363 616c 6520 7061 7261  ''The scale para
+00014730: 6d65 7465 7220 6465 6669 6e65 7320 686f  meter defines ho
+00014740: 7720 2268 6967 6820 7570 2220 6f6e 2074  w "high up" on t
+00014750: 6865 2069 6e69 7469 616c 2070 6c6f 7420  he initial plot 
+00014760: 7468 6973 206f 7665 726c 6179 2077 696c  this overlay wil
+00014770: 6c20 7368 6f77 2e0d 0a20 2020 2020 2020  l show...       
+00014780: 5468 6520 7961 7869 7320 7061 7261 6d65  The yaxis parame
+00014790: 7465 7220 6361 6e20 6265 206f 6e65 206f  ter can be one o
+000147a0: 6620 5b46 616c 7365 2c20 276c 696e 6561  f [False, 'linea
+000147b0: 7227 2c20 276c 6f67 275d 2e27 2727 0d0a  r', 'log'].'''..
+000147c0: 2020 2020 7973 6361 6c65 203d 2079 6178      yscale = yax
+000147d0: 6973 2069 6620 7961 7869 7320 656c 7365  is if yaxis else
+000147e0: 2027 6c69 6e65 6172 270d 0a20 2020 2076   'linear'..    v
+000147f0: 6965 7762 6f78 203d 2046 696e 5669 6577  iewbox = FinView
+00014800: 426f 7828 6178 2e76 622e 7769 6e2c 2069  Box(ax.vb.win, i
+00014810: 6e69 745f 7374 6570 733d 6178 2e76 622e  nit_steps=ax.vb.
+00014820: 696e 6974 5f73 7465 7073 2c20 7973 6361  init_steps, ysca
+00014830: 6c65 3d59 5363 616c 6528 7973 6361 6c65  le=YScale(yscale
+00014840: 2c20 3129 2c20 656e 6162 6c65 4d65 6e75  , 1), enableMenu
+00014850: 3d46 616c 7365 290d 0a20 2020 2076 6965  =False)..    vie
+00014860: 7762 6f78 2e6d 6173 7465 725f 7669 6577  wbox.master_view
+00014870: 626f 7820 3d20 6178 2e76 620d 0a20 2020  box = ax.vb..   
+00014880: 2076 6965 7762 6f78 2e73 6574 5a56 616c   viewbox.setZVal
+00014890: 7565 282d 3529 0d0a 2020 2020 7669 6577  ue(-5)..    view
+000148a0: 626f 782e 7365 7442 6163 6b67 726f 756e  box.setBackgroun
+000148b0: 6443 6f6c 6f72 2861 782e 7662 2e73 7461  dColor(ax.vb.sta
+000148c0: 7465 5b27 6261 636b 6772 6f75 6e64 275d  te['background']
+000148d0: 290d 0a20 2020 2061 782e 7662 2e73 6574  )..    ax.vb.set
+000148e0: 4261 636b 6772 6f75 6e64 436f 6c6f 7228  BackgroundColor(
+000148f0: 4e6f 6e65 290d 0a20 2020 2076 6965 7762  None)..    viewb
+00014900: 6f78 2e76 5f7a 6f6f 6d5f 7363 616c 6520  ox.v_zoom_scale 
+00014910: 3d20 7363 616c 650d 0a20 2020 2069 6620  = scale..    if 
+00014920: 6861 7361 7474 7228 6178 2c20 2761 785f  hasattr(ax, 'ax_
+00014930: 7769 6467 6574 2729 3a0d 0a20 2020 2020  widget'):..     
+00014940: 2020 2061 782e 6178 5f77 6964 6765 742e     ax.ax_widget.
+00014950: 7363 656e 6528 292e 6164 6449 7465 6d28  scene().addItem(
+00014960: 7669 6577 626f 7829 0d0a 2020 2020 656c  viewbox)..    el
+00014970: 7365 3a0d 0a20 2020 2020 2020 2061 782e  se:..        ax.
+00014980: 7662 2e77 696e 2e63 656e 7472 616c 5769  vb.win.centralWi
+00014990: 6467 6574 2e73 6365 6e65 2829 2e61 6464  dget.scene().add
+000149a0: 4974 656d 2876 6965 7762 6f78 290d 0a20  Item(viewbox).. 
+000149b0: 2020 2076 6965 7762 6f78 2e73 6574 584c     viewbox.setXL
+000149c0: 696e 6b28 6178 2e76 6229 0d0a 2020 2020  ink(ax.vb)..    
+000149d0: 6465 6620 7570 6461 7465 5669 6577 2829  def updateView()
+000149e0: 3a0d 0a20 2020 2020 2020 2076 6965 7762  :..        viewb
+000149f0: 6f78 2e73 6574 4765 6f6d 6574 7279 2861  ox.setGeometry(a
+00014a00: 782e 7662 2e73 6365 6e65 426f 756e 6469  x.vb.sceneBoundi
+00014a10: 6e67 5265 6374 2829 290d 0a20 2020 2061  ngRect())..    a
+00014a20: 786f 203d 2070 672e 506c 6f74 4974 656d  xo = pg.PlotItem
+00014a30: 2865 6e61 626c 654d 656e 753d 4661 6c73  (enableMenu=Fals
+00014a40: 6529 0d0a 2020 2020 6178 6f2e 7369 676e  e)..    axo.sign
+00014a50: 6966 6963 616e 745f 666f 7263 6564 203d  ificant_forced =
+00014a60: 2046 616c 7365 0d0a 2020 2020 6178 6f2e   False..    axo.
+00014a70: 7369 676e 6966 6963 616e 745f 6465 6369  significant_deci
+00014a80: 6d61 6c73 203d 2073 6967 6e69 6669 6361  mals = significa
+00014a90: 6e74 5f64 6563 696d 616c 730d 0a20 2020  nt_decimals..   
+00014aa0: 2061 786f 2e73 6967 6e69 6669 6361 6e74   axo.significant
+00014ab0: 5f65 7073 203d 2073 6967 6e69 6669 6361  _eps = significa
+00014ac0: 6e74 5f65 7073 0d0a 2020 2020 6178 6f2e  nt_eps..    axo.
+00014ad0: 7662 203d 2076 6965 7762 6f78 0d0a 2020  vb = viewbox..  
+00014ae0: 2020 6178 6f2e 7072 6576 5f61 7820 3d20    axo.prev_ax = 
+00014af0: 4e6f 6e65 0d0a 2020 2020 6178 6f2e 6372  None..    axo.cr
+00014b00: 6f73 7368 6169 7220 3d20 4e6f 6e65 0d0a  osshair = None..
+00014b10: 2020 2020 6178 6f2e 6465 636f 7570 6c65      axo.decouple
+00014b20: 203d 2070 6172 7469 616c 285f 6178 5f64   = partial(_ax_d
+00014b30: 6563 6f75 706c 652c 2061 786f 290d 0a20  ecouple, axo).. 
+00014b40: 2020 2061 786f 2e64 6973 6162 6c65 5f78     axo.disable_x
+00014b50: 5f69 6e64 6578 203d 2070 6172 7469 616c  _index = partial
+00014b60: 285f 6178 5f64 6973 6162 6c65 5f78 5f69  (_ax_disable_x_i
+00014b70: 6e64 6578 2c20 6178 6f29 0d0a 2020 2020  ndex, axo)..    
+00014b80: 6178 6f2e 7265 7365 7420 3d20 7061 7274  axo.reset = part
+00014b90: 6961 6c28 5f61 785f 7265 7365 742c 2061  ial(_ax_reset, a
+00014ba0: 786f 290d 0a20 2020 2061 786f 2e68 6964  xo)..    axo.hid
+00014bb0: 6541 7869 7328 276c 6566 7427 290d 0a20  eAxis('left').. 
+00014bc0: 2020 2061 786f 2e68 6964 6541 7869 7328     axo.hideAxis(
+00014bd0: 2772 6967 6874 2729 0d0a 2020 2020 6178  'right')..    ax
+00014be0: 6f2e 6869 6465 4178 6973 2827 626f 7474  o.hideAxis('bott
+00014bf0: 6f6d 2729 0d0a 2020 2020 6178 6f2e 6869  om')..    axo.hi
+00014c00: 6465 4275 7474 6f6e 7328 290d 0a20 2020  deButtons()..   
+00014c10: 2076 6965 7762 6f78 2e61 6464 4974 656d   viewbox.addItem
+00014c20: 2861 786f 290d 0a20 2020 2069 6620 7961  (axo)..    if ya
+00014c30: 7869 7320 616e 6420 6973 696e 7374 616e  xis and isinstan
+00014c40: 6365 2861 786f 2e76 622e 7769 6e2c 2070  ce(axo.vb.win, p
+00014c50: 672e 4772 6170 6869 6373 4c61 796f 7574  g.GraphicsLayout
+00014c60: 5769 6467 6574 293a 0d0a 2020 2020 2020  Widget):..      
+00014c70: 2020 6178 6920 3d20 5f63 7265 6174 655f    axi = _create_
+00014c80: 6178 6973 2870 6f73 3d27 7927 2c20 7662  axis(pos='y', vb
+00014c90: 3d61 786f 2e76 622c 206f 7269 656e 7461  =axo.vb, orienta
+00014ca0: 7469 6f6e 3d27 6c65 6674 2729 0d0a 2020  tion='left')..  
+00014cb0: 2020 2020 2020 6178 6f2e 7365 7441 7869        axo.setAxi
+00014cc0: 7349 7465 6d73 287b 276c 6566 7427 3a20  sItems({'left': 
+00014cd0: 6178 697d 290d 0a20 2020 2020 2020 2061  axi})..        a
+00014ce0: 786f 2e76 622e 7769 6e2e 6164 6449 7465  xo.vb.win.addIte
+00014cf0: 6d28 6178 692c 2072 6f77 3d30 2c20 636f  m(axi, row=0, co
+00014d00: 6c3d 3029 0d0a 2020 2020 6178 2e76 622e  l=0)..    ax.vb.
+00014d10: 7369 6752 6573 697a 6564 2e63 6f6e 6e65  sigResized.conne
+00014d20: 6374 2875 7064 6174 6556 6965 7729 0d0a  ct(updateView)..
+00014d30: 2020 2020 6f76 6572 6c61 795f 6178 732e      overlay_axs.
+00014d40: 6170 7065 6e64 2861 786f 290d 0a20 2020  append(axo)..   
+00014d50: 2075 7064 6174 6556 6965 7728 290d 0a20   updateView().. 
+00014d60: 2020 2072 6574 7572 6e20 6178 6f0d 0a0d     return axo...
+00014d70: 0a0d 0a64 6566 205f 6178 5f73 6574 5f76  ...def _ax_set_v
+00014d80: 6973 6962 6c65 2861 782c 2063 726f 7373  isible(ax, cross
+00014d90: 6861 6972 3d4e 6f6e 652c 2078 6178 6973  hair=None, xaxis
+00014da0: 3d4e 6f6e 652c 2079 6178 6973 3d4e 6f6e  =None, yaxis=Non
+00014db0: 652c 2078 6772 6964 3d4e 6f6e 652c 2079  e, xgrid=None, y
+00014dc0: 6772 6964 3d4e 6f6e 6529 3a0d 0a20 2020  grid=None):..   
+00014dd0: 2069 6620 6372 6f73 7368 6169 7220 3d3d   if crosshair ==
+00014de0: 2046 616c 7365 3a0d 0a20 2020 2020 2020   False:..       
+00014df0: 2061 782e 6372 6f73 7368 6169 722e 6869   ax.crosshair.hi
+00014e00: 6465 2829 0d0a 2020 2020 6966 2078 6178  de()..    if xax
+00014e10: 6973 2069 7320 6e6f 7420 4e6f 6e65 3a0d  is is not None:.
+00014e20: 0a20 2020 2020 2020 2061 782e 6765 7441  .        ax.getA
+00014e30: 7869 7328 2762 6f74 746f 6d27 292e 7365  xis('bottom').se
+00014e40: 7453 7479 6c65 2873 686f 7756 616c 7565  tStyle(showValue
+00014e50: 733d 7861 7869 7329 0d0a 2020 2020 6966  s=xaxis)..    if
+00014e60: 2079 6178 6973 2069 7320 6e6f 7420 4e6f   yaxis is not No
+00014e70: 6e65 3a0d 0a20 2020 2020 2020 2061 782e  ne:..        ax.
+00014e80: 6765 7441 7869 7328 2772 6967 6874 2729  getAxis('right')
+00014e90: 2e73 6574 5374 796c 6528 7368 6f77 5661  .setStyle(showVa
+00014ea0: 6c75 6573 3d79 6178 6973 290d 0a20 2020  lues=yaxis)..   
+00014eb0: 2069 6620 7867 7269 6420 6973 206e 6f74   if xgrid is not
+00014ec0: 204e 6f6e 6520 6f72 2079 6772 6964 2069   None or ygrid i
+00014ed0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00014ee0: 2020 2020 2061 782e 7368 6f77 4772 6964       ax.showGrid
+00014ef0: 2878 3d78 6772 6964 2c20 793d 7967 7269  (x=xgrid, y=ygri
+00014f00: 6429 0d0a 2020 2020 2020 2020 6966 2061  d)..        if a
+00014f10: 782e 6765 7441 7869 7328 2772 6967 6874  x.getAxis('right
+00014f20: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+00014f30: 2061 782e 6765 7441 7869 7328 2772 6967   ax.getAxis('rig
+00014f40: 6874 2729 2e73 6574 456e 6162 6c65 6428  ht').setEnabled(
+00014f50: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+00014f60: 6966 2061 782e 6765 7441 7869 7328 2762  if ax.getAxis('b
+00014f70: 6f74 746f 6d27 293a 0d0a 2020 2020 2020  ottom'):..      
+00014f80: 2020 2020 2020 6178 2e67 6574 4178 6973        ax.getAxis
+00014f90: 2827 626f 7474 6f6d 2729 2e73 6574 456e  ('bottom').setEn
+00014fa0: 6162 6c65 6428 4661 6c73 6529 0d0a 0d0a  abled(False)....
+00014fb0: 0d0a 6465 6620 5f61 785f 6465 636f 7570  ..def _ax_decoup
+00014fc0: 6c65 2861 7829 3a0d 0a20 2020 2061 782e  le(ax):..    ax.
+00014fd0: 7365 7458 4c69 6e6b 284e 6f6e 6529 0d0a  setXLink(None)..
+00014fe0: 2020 2020 6966 2061 782e 7072 6576 5f61      if ax.prev_a
+00014ff0: 783a 0d0a 2020 2020 2020 2020 6178 2e70  x:..        ax.p
+00015000: 7265 765f 6178 2e73 6574 5f76 6973 6962  rev_ax.set_visib
+00015010: 6c65 2878 6178 6973 3d54 7275 6529 0d0a  le(xaxis=True)..
+00015020: 0d0a 0d0a 6465 6620 5f61 785f 6469 7361  ....def _ax_disa
+00015030: 626c 655f 785f 696e 6465 7828 6178 2c20  ble_x_index(ax, 
+00015040: 6465 636f 7570 6c65 3d54 7275 6529 3a0d  decouple=True):.
+00015050: 0a20 2020 2061 782e 7662 2e78 5f69 6e64  .    ax.vb.x_ind
+00015060: 6578 6564 203d 2046 616c 7365 0d0a 2020  exed = False..  
+00015070: 2020 6966 2064 6563 6f75 706c 653a 0d0a    if decouple:..
+00015080: 2020 2020 2020 2020 5f61 785f 6465 636f          _ax_deco
+00015090: 7570 6c65 2861 7829 0d0a 0d0a 0d0a 6465  uple(ax)......de
+000150a0: 6620 5f61 785f 7265 7365 7428 6178 293a  f _ax_reset(ax):
+000150b0: 0d0a 2020 2020 6966 2061 782e 6372 6f73  ..    if ax.cros
+000150c0: 7368 6169 7220 6973 206e 6f74 204e 6f6e  shair is not Non
+000150d0: 653a 0d0a 2020 2020 2020 2020 6178 2e63  e:..        ax.c
+000150e0: 726f 7373 6861 6972 2e68 6964 6528 290d  rosshair.hide().
+000150f0: 0a20 2020 2066 6f72 2069 7465 6d20 696e  .    for item in
+00015100: 206c 6973 7428 6178 2e69 7465 6d73 293a   list(ax.items):
+00015110: 0d0a 2020 2020 2020 2020 6178 2e72 656d  ..        ax.rem
+00015120: 6f76 6549 7465 6d28 6974 656d 290d 0a20  oveItem(item).. 
+00015130: 2020 2020 2020 2069 6620 6178 2e76 622e         if ax.vb.
+00015140: 6d61 7374 6572 5f76 6965 7762 6f78 2061  master_viewbox a
+00015150: 6e64 2068 6173 6174 7472 2869 7465 6d2c  nd hasattr(item,
+00015160: 2027 6e61 6d65 2729 2061 6e64 2069 7465   'name') and ite
+00015170: 6d2e 6e61 6d65 2829 3a0d 0a20 2020 2020  m.name():..     
+00015180: 2020 2020 2020 206c 6567 656e 6420 3d20         legend = 
+00015190: 6178 2e76 622e 6d61 7374 6572 5f76 6965  ax.vb.master_vie
+000151a0: 7762 6f78 2e70 6172 656e 7428 292e 6c65  wbox.parent().le
+000151b0: 6765 6e64 0d0a 2020 2020 2020 2020 2020  gend..          
+000151c0: 2020 6966 206c 6567 656e 643a 0d0a 2020    if legend:..  
+000151d0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+000151e0: 6765 6e64 2e72 656d 6f76 6549 7465 6d28  gend.removeItem(
+000151f0: 6974 656d 290d 0a20 2020 2069 6620 6178  item)..    if ax
+00015200: 2e6c 6567 656e 643a 0d0a 2020 2020 2020  .legend:..      
+00015210: 2020 6178 2e6c 6567 656e 642e 6f70 7473    ax.legend.opts
+00015220: 5b27 6f66 6673 6574 275d 203d 204e 6f6e  ['offset'] = Non
+00015230: 650d 0a20 2020 2020 2020 2061 782e 6c65  e..        ax.le
+00015240: 6765 6e64 2e73 6574 5061 7265 6e74 4974  gend.setParentIt
+00015250: 656d 284e 6f6e 6529 0d0a 2020 2020 2020  em(None)..      
+00015260: 2020 6178 2e6c 6567 656e 6420 3d20 4e6f    ax.legend = No
+00015270: 6e65 0d0a 2020 2020 6178 2e76 622e 7265  ne..    ax.vb.re
+00015280: 7365 7428 290d 0a20 2020 2061 782e 7662  set()..    ax.vb
+00015290: 2e73 6574 5f64 6174 6173 7263 284e 6f6e  .set_datasrc(Non
+000152a0: 6529 0d0a 2020 2020 6966 2061 782e 6372  e)..    if ax.cr
+000152b0: 6f73 7368 6169 7220 6973 206e 6f74 204e  osshair is not N
+000152c0: 6f6e 653a 0d0a 2020 2020 2020 2020 6178  one:..        ax
+000152d0: 2e63 726f 7373 6861 6972 2e73 686f 7728  .crosshair.show(
+000152e0: 290d 0a20 2020 2061 782e 7369 676e 6966  )..    ax.signif
+000152f0: 6963 616e 745f 666f 7263 6564 203d 2046  icant_forced = F
+00015300: 616c 7365 0d0a 0d0a 0d0a 6465 6620 5f63  alse......def _c
+00015310: 7265 6174 655f 6c65 6765 6e64 2861 7829  reate_legend(ax)
+00015320: 3a0d 0a20 2020 2069 6620 6178 2e76 622e  :..    if ax.vb.
+00015330: 6d61 7374 6572 5f76 6965 7762 6f78 3a0d  master_viewbox:.
+00015340: 0a20 2020 2020 2020 2061 7820 3d20 6178  .        ax = ax
+00015350: 2e76 622e 6d61 7374 6572 5f76 6965 7762  .vb.master_viewb
+00015360: 6f78 2e70 6172 656e 7428 290d 0a20 2020  ox.parent()..   
+00015370: 2069 6620 6178 2e6c 6567 656e 6420 6973   if ax.legend is
+00015380: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00015390: 6178 2e6c 6567 656e 6420 3d20 4669 6e4c  ax.legend = FinL
+000153a0: 6567 656e 6449 7465 6d28 626f 7264 6572  egendItem(border
+000153b0: 5f63 6f6c 6f72 3d6c 6567 656e 645f 626f  _color=legend_bo
+000153c0: 7264 6572 5f63 6f6c 6f72 2c20 6669 6c6c  rder_color, fill
+000153d0: 5f63 6f6c 6f72 3d6c 6567 656e 645f 6669  _color=legend_fi
+000153e0: 6c6c 5f63 6f6c 6f72 2c20 7369 7a65 3d4e  ll_color, size=N
+000153f0: 6f6e 652c 206f 6666 7365 743d 2833 2c32  one, offset=(3,2
+00015400: 2929 0d0a 2020 2020 2020 2020 6178 2e6c  ))..        ax.l
+00015410: 6567 656e 642e 7365 7450 6172 656e 7449  egend.setParentI
+00015420: 7465 6d28 6178 2e76 6229 0d0a 0d0a 0d0a  tem(ax.vb)......
+00015430: 6465 6620 5f75 7064 6174 655f 7369 676e  def _update_sign
+00015440: 6966 6963 616e 7473 2861 782c 2064 6174  ificants(ax, dat
+00015450: 6173 7263 2c20 666f 7263 6529 3a0d 0a20  asrc, force):.. 
+00015460: 2020 2023 2063 6865 636b 2069 6620 6e6f     # check if no
+00015470: 2065 7073 696c 6f6e 2073 6574 2079 6574   epsilon set yet
+00015480: 0d0a 2020 2020 6465 6661 756c 745f 6465  ..    default_de
+00015490: 6320 3d20 302e 3939 203c 2061 782e 7369  c = 0.99 < ax.si
+000154a0: 676e 6966 6963 616e 745f 6465 6369 6d61  gnificant_decima
+000154b0: 6c73 2f73 6967 6e69 6669 6361 6e74 5f64  ls/significant_d
+000154c0: 6563 696d 616c 7320 3c20 312e 3031 0d0a  ecimals < 1.01..
+000154d0: 2020 2020 6465 6661 756c 745f 6570 7320      default_eps 
+000154e0: 3d20 302e 3939 203c 2061 782e 7369 676e  = 0.99 < ax.sign
+000154f0: 6966 6963 616e 745f 6570 732f 7369 676e  ificant_eps/sign
+00015500: 6966 6963 616e 745f 6570 7320 3c20 312e  ificant_eps < 1.
+00015510: 3031 0d0a 2020 2020 6966 2066 6f72 6365  01..    if force
+00015520: 206f 7220 2864 6566 6175 6c74 5f64 6563   or (default_dec
+00015530: 2061 6e64 2064 6566 6175 6c74 5f65 7073   and default_eps
+00015540: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
+00015550: 0d0a 2020 2020 2020 2020 2020 2020 7364  ..            sd
+00015560: 2c73 6520 3d20 6461 7461 7372 632e 6361  ,se = datasrc.ca
+00015570: 6c63 5f73 6967 6e69 6669 6361 6e74 5f64  lc_significant_d
+00015580: 6563 696d 616c 7328 6675 6c6c 3d66 6f72  ecimals(full=for
+00015590: 6365 290d 0a20 2020 2020 2020 2020 2020  ce)..           
+000155a0: 2069 6620 7364 206f 7220 7365 2021 3d20   if sd or se != 
+000155b0: 7369 676e 6966 6963 616e 745f 6570 733a  significant_eps:
+000155c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000155d0: 2020 6966 2028 666f 7263 6520 616e 6420    if (force and 
+000155e0: 6e6f 7420 6178 2e73 6967 6e69 6669 6361  not ax.significa
+000155f0: 6e74 5f66 6f72 6365 6429 206f 7220 6465  nt_forced) or de
+00015600: 6661 756c 745f 6465 6320 6f72 2073 6420  fault_dec or sd 
+00015610: 3e20 6178 2e73 6967 6e69 6669 6361 6e74  > ax.significant
+00015620: 5f64 6563 696d 616c 733a 0d0a 2020 2020  _decimals:..    
+00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015640: 6178 2e73 6967 6e69 6669 6361 6e74 5f64  ax.significant_d
+00015650: 6563 696d 616c 7320 3d20 7364 0d0a 2020  ecimals = sd..  
+00015660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015670: 2020 6178 2e73 6967 6e69 6669 6361 6e74    ax.significant
+00015680: 5f66 6f72 6365 6420 7c3d 2066 6f72 6365  _forced |= force
+00015690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000156a0: 2020 6966 2028 666f 7263 6520 616e 6420    if (force and 
+000156b0: 6e6f 7420 6178 2e73 6967 6e69 6669 6361  not ax.significa
+000156c0: 6e74 5f66 6f72 6365 6429 206f 7220 6465  nt_forced) or de
+000156d0: 6661 756c 745f 6570 7320 6f72 2073 6520  fault_eps or se 
+000156e0: 3c20 6178 2e73 6967 6e69 6669 6361 6e74  < ax.significant
+000156f0: 5f65 7073 3a0d 0a20 2020 2020 2020 2020  _eps:..         
+00015700: 2020 2020 2020 2020 2020 2061 782e 7369             ax.si
+00015710: 676e 6966 6963 616e 745f 6570 7320 3d20  gnificant_eps = 
+00015720: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
+00015730: 2020 2020 2020 2020 6178 2e73 6967 6e69          ax.signi
+00015740: 6669 6361 6e74 5f66 6f72 6365 6420 7c3d  ficant_forced |=
+00015750: 2066 6f72 6365 0d0a 2020 2020 2020 2020   force..        
+00015760: 6578 6365 7074 3a0d 0a20 2020 2020 2020  except:..       
+00015770: 2020 2020 2070 6173 7320 2320 6461 7461       pass # data
+00015780: 7372 6320 7072 6f62 6162 6c79 2066 756c  src probably ful
+00015790: 6c20 6176 204e 614e 730d 0a0d 0a0d 0a64  l av NaNs......d
+000157a0: 6566 205f 696d 7072 6f76 655f 7369 676e  ef _improve_sign
+000157b0: 6966 6963 616e 7473 2861 7829 3a0d 0a20  ificants(ax):.. 
+000157c0: 2020 2027 2727 466f 7263 6520 7570 6461     '''Force upda
+000157d0: 7465 206f 6620 7468 6520 4550 5320 6966  te of the EPS if
+000157e0: 2077 6520 626f 7468 2068 6176 6520 6e6f   we both have no
+000157f0: 2062 6172 732f 6361 6e64 6c65 7320 414e   bars/candles AN
+00015800: 4420 6120 6c6f 6720 7363 616c 652e 0d0a  D a log scale...
+00015810: 2020 2020 2020 2054 6869 7320 6973 2069         This is i
+00015820: 6e74 656e 6465 6420 746f 2066 6978 2074  ntended to fix t
+00015830: 6865 206c 6f77 6572 2070 6172 7420 6f66  he lower part of
+00015840: 2074 6865 2067 7269 6420 6f6e 206c 696e   the grid on lin
+00015850: 6520 706c 6f74 7320 6f6e 2061 206c 6f67  e plots on a log
+00015860: 2073 6361 6c65 2e27 2727 0d0a 2020 2020   scale.'''..    
+00015870: 6966 2061 782e 7662 2e79 7363 616c 652e  if ax.vb.yscale.
+00015880: 7363 616c 6574 7970 6520 3d3d 2027 6c6f  scaletype == 'lo
+00015890: 6727 3a0d 0a20 2020 2020 2020 2069 6620  g':..        if 
+000158a0: 6e6f 7420 616e 7928 6973 696e 7374 616e  not any(isinstan
+000158b0: 6365 2869 7465 6d2c 2043 616e 646c 6573  ce(item, Candles
+000158c0: 7469 636b 4974 656d 2920 666f 7220 6974  tickItem) for it
+000158d0: 656d 2069 6e20 6178 2e69 7465 6d73 293a  em in ax.items):
+000158e0: 0d0a 2020 2020 2020 2020 2020 2020 5f75  ..            _u
+000158f0: 7064 6174 655f 7369 676e 6966 6963 616e  pdate_significan
+00015900: 7473 2861 782c 2061 782e 7662 2e64 6174  ts(ax, ax.vb.dat
+00015910: 6173 7263 2c20 666f 7263 653d 5472 7565  asrc, force=True
+00015920: 290d 0a0d 0a0d 0a64 6566 205f 6973 5f73  )......def _is_s
+00015930: 7461 6e64 616c 6f6e 6528 7469 6d65 7365  tandalone(timese
+00015940: 7229 3a0d 0a20 2020 2023 206d 6f72 6520  r):..    # more 
+00015950: 7468 616e 204e 2070 6572 6365 6e74 2067  than N percent g
+00015960: 6170 7320 6f72 2074 696d 6520 7265 7665  aps or time reve
+00015970: 7273 616c 7320 7072 6f62 6162 6c79 206d  rsals probably m
+00015980: 6561 6e73 2074 6869 7320 6973 2061 2073  eans this is a s
+00015990: 7461 6e64 616c 6f6e 6520 706c 6f74 0d0a  tandalone plot..
+000159a0: 2020 2020 7265 7475 726e 2074 696d 6573      return times
+000159b0: 6572 2e69 736e 756c 6c28 292e 7375 6d28  er.isnull().sum(
+000159c0: 2920 2b20 2874 696d 6573 6572 2e64 6966  ) + (timeser.dif
+000159d0: 6628 293c 3d30 292e 7375 6d28 2920 3e20  f()<=0).sum() > 
+000159e0: 6c65 6e28 7469 6d65 7365 7229 2a30 2e31  len(timeser)*0.1
+000159f0: 0d0a 0d0a 0d0a 6465 6620 5f63 7265 6174  ......def _creat
+00015a00: 655f 7365 7269 6573 2861 293a 0d0a 2020  e_series(a):..  
+00015a10: 2020 7265 7475 726e 2061 2069 6620 6973    return a if is
+00015a20: 696e 7374 616e 6365 2861 2c20 7064 2e53  instance(a, pd.S
+00015a30: 6572 6965 7329 2065 6c73 6520 7064 2e53  eries) else pd.S
+00015a40: 6572 6965 7328 6129 0d0a 0d0a 0d0a 6465  eries(a)......de
+00015a50: 6620 5f63 7265 6174 655f 6461 7461 7372  f _create_datasr
+00015a60: 6328 6178 2c20 2a61 7267 732c 206e 636f  c(ax, *args, nco
+00015a70: 6c73 3d2d 3129 3a0d 0a20 2020 2064 6566  ls=-1):..    def
+00015a80: 2064 6f5f 6372 6561 7465 2861 7267 7329   do_create(args)
+00015a90: 3a0d 0a20 2020 2020 2020 2069 6620 6c65  :..        if le
+00015aa0: 6e28 6172 6773 2920 3d3d 2031 2061 6e64  n(args) == 1 and
+00015ab0: 2074 7970 6528 6172 6773 5b30 5d29 203d   type(args[0]) =
+00015ac0: 3d20 5061 6e64 6173 4461 7461 536f 7572  = PandasDataSour
+00015ad0: 6365 3a0d 0a20 2020 2020 2020 2020 2020  ce:..           
+00015ae0: 2072 6574 7572 6e20 6172 6773 5b30 5d0d   return args[0].
+00015af0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00015b00: 6172 6773 2920 3d3d 2031 2061 6e64 2074  args) == 1 and t
+00015b10: 7970 6528 6172 6773 5b30 5d29 2069 6e20  ype(args[0]) in 
+00015b20: 286c 6973 742c 2074 7570 6c65 293a 0d0a  (list, tuple):..
+00015b30: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00015b40: 203d 205b 6e70 2e61 7272 6179 2861 7267   = [np.array(arg
+00015b50: 735b 305d 295d 0d0a 2020 2020 2020 2020  s[0])]..        
+00015b60: 6966 206c 656e 2861 7267 7329 203d 3d20  if len(args) == 
+00015b70: 3120 616e 6420 7479 7065 2861 7267 735b  1 and type(args[
+00015b80: 305d 2920 3d3d 206e 702e 6e64 6172 7261  0]) == np.ndarra
+00015b90: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00015ba0: 6172 6773 203d 205b 7064 2e44 6174 6146  args = [pd.DataF
+00015bb0: 7261 6d65 2861 7267 735b 305d 2e54 295d  rame(args[0].T)]
+00015bc0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00015bd0: 2861 7267 7329 203d 3d20 3120 616e 6420  (args) == 1 and 
+00015be0: 7479 7065 2861 7267 735b 305d 2920 3d3d  type(args[0]) ==
+00015bf0: 2070 642e 4461 7461 4672 616d 653a 0d0a   pd.DataFrame:..
+00015c00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015c10: 726e 2050 616e 6461 7344 6174 6153 6f75  rn PandasDataSou
+00015c20: 7263 6528 6172 6773 5b30 5d29 0d0a 2020  rce(args[0])..  
+00015c30: 2020 2020 2020 6172 6773 203d 205b 5f63        args = [_c
+00015c40: 7265 6174 655f 7365 7269 6573 2861 2920  reate_series(a) 
+00015c50: 666f 7220 6120 696e 2061 7267 735d 0d0a  for a in args]..
+00015c60: 2020 2020 2020 2020 7265 7475 726e 2050          return P
+00015c70: 616e 6461 7344 6174 6153 6f75 7263 6528  andasDataSource(
+00015c80: 7064 2e63 6f6e 6361 7428 6172 6773 2c20  pd.concat(args, 
+00015c90: 6178 6973 3d31 2929 0d0a 2020 2020 6961  axis=1))..    ia
+00015ca0: 7267 7320 3d20 5b61 2066 6f72 2061 2069  rgs = [a for a i
+00015cb0: 6e20 6172 6773 2069 6620 6120 6973 206e  n args if a is n
+00015cc0: 6f74 204e 6f6e 655d 0d0a 2020 2020 6461  ot None]..    da
+00015cd0: 7461 7372 6320 3d20 646f 5f63 7265 6174  tasrc = do_creat
+00015ce0: 6528 6961 7267 7329 0d0a 2020 2020 2320  e(iargs)..    # 
+00015cf0: 6368 6563 6b20 6966 2074 696d 6520 636f  check if time co
+00015d00: 6c75 6d6e 206d 6973 7369 6e67 0d0a 2020  lumn missing..  
+00015d10: 2020 6966 206c 656e 2864 6174 6173 7263    if len(datasrc
+00015d20: 2e64 662e 636f 6c75 6d6e 7329 2069 6e20  .df.columns) in 
+00015d30: 2831 2c20 6e63 6f6c 732d 3129 3a0d 0a20  (1, ncols-1):.. 
+00015d40: 2020 2020 2020 2023 2061 7373 756d 6520         # assume 
+00015d50: 7469 6d65 2064 6174 6120 6861 7320 616c  time data has al
+00015d60: 7265 6164 7920 6265 656e 2061 6464 6564  ready been added
+00015d70: 2062 6566 6f72 650d 0a20 2020 2020 2020   before..       
+00015d80: 2066 6f72 2061 2069 6e20 6178 2e76 622e   for a in ax.vb.
+00015d90: 7769 6e2e 6178 733a 0d0a 2020 2020 2020  win.axs:..      
+00015da0: 2020 2020 2020 6966 2061 2e76 622e 6461        if a.vb.da
+00015db0: 7461 7372 6320 616e 6420 6c65 6e28 612e  tasrc and len(a.
+00015dc0: 7662 2e64 6174 6173 7263 2e64 662e 636f  vb.datasrc.df.co
+00015dd0: 6c75 6d6e 7329 203e 3d20 323a 0d0a 2020  lumns) >= 2:..  
+00015de0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00015df0: 7461 7372 632e 6466 2e63 6f6c 756d 6e73  tasrc.df.columns
+00015e00: 203d 2061 2e76 622e 6461 7461 7372 632e   = a.vb.datasrc.
+00015e10: 6466 2e63 6f6c 756d 6e73 5b31 3a6c 656e  df.columns[1:len
+00015e20: 2864 6174 6173 7263 2e64 662e 636f 6c75  (datasrc.df.colu
+00015e30: 6d6e 7329 2b31 5d0d 0a20 2020 2020 2020  mns)+1]..       
+00015e40: 2020 2020 2020 2020 2063 6f6c 203d 2061           col = a
+00015e50: 2e76 622e 6461 7461 7372 632e 6466 2e63  .vb.datasrc.df.c
+00015e60: 6f6c 756d 6e73 5b30 5d0d 0a20 2020 2020  olumns[0]..     
+00015e70: 2020 2020 2020 2020 2020 2064 6174 6173             datas
+00015e80: 7263 2e64 662e 696e 7365 7274 2830 2c20  rc.df.insert(0, 
+00015e90: 636f 6c2c 2061 2e76 622e 6461 7461 7372  col, a.vb.datasr
+00015ea0: 632e 6466 5b63 6f6c 5d29 0d0a 2020 2020  c.df[col])..    
+00015eb0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00015ec0: 7372 6320 3d20 5061 6e64 6173 4461 7461  src = PandasData
+00015ed0: 536f 7572 6365 2864 6174 6173 7263 2e64  Source(datasrc.d
+00015ee0: 6629 0d0a 2020 2020 2020 2020 2020 2020  f)..            
+00015ef0: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
+00015f00: 2020 2069 6620 6c65 6e28 6461 7461 7372     if len(datasr
+00015f10: 632e 6466 2e63 6f6c 756d 6e73 2920 696e  c.df.columns) in
+00015f20: 2028 312c 206e 636f 6c73 2d31 293a 0d0a   (1, ncols-1):..
+00015f30: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00015f40: 636f 6c73 203e 2031 3a0d 0a20 2020 2020  cols > 1:..     
+00015f50: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00015f60: 2866 2257 4152 4e49 4e47 3a20 7468 6973  (f"WARNING: this
+00015f70: 2074 7970 6520 6f66 2070 6c6f 7420 7761   type of plot wa
+00015f80: 6e74 7320 2569 2063 6f6c 756d 6e73 2f61  nts %i columns/a
+00015f90: 7267 732c 2062 7574 2079 6f75 2776 6520  rgs, but you've 
+00015fa0: 6f6e 6c79 2073 7570 706c 6965 6420 2569  only supplied %i
+00015fb0: 2220 2520 286e 636f 6c73 2c20 6c65 6e28  " % (ncols, len(
+00015fc0: 6461 7461 7372 632e 6466 2e63 6f6c 756d  datasrc.df.colum
+00015fd0: 6e73 2929 290d 0a20 2020 2020 2020 2020  ns)))..         
+00015fe0: 2020 2020 2020 2070 7269 6e74 2827 202d         print(' -
+00015ff0: 2041 7373 756d 696e 6720 7469 6d65 2063   Assuming time c
+00016000: 6f6c 756d 6e20 6973 206d 6973 7369 6e67  olumn is missing
+00016010: 2061 6e64 2075 7369 6e67 2069 6e64 6578   and using index
+00016020: 2069 6e73 7465 6164 2e27 290d 0a20 2020   instead.')..   
+00016030: 2020 2020 2020 2020 2064 6174 6173 7263           datasrc
+00016040: 203d 2050 616e 6461 7344 6174 6153 6f75   = PandasDataSou
+00016050: 7263 6528 6461 7461 7372 632e 6466 2e72  rce(datasrc.df.r
+00016060: 6573 6574 5f69 6e64 6578 2829 290d 0a20  eset_index()).. 
+00016070: 2020 2065 6c69 6620 6c65 6e28 6961 7267     elif len(iarg
+00016080: 7329 203e 3d20 3220 616e 6420 6c65 6e28  s) >= 2 and len(
+00016090: 6461 7461 7372 632e 6466 2e63 6f6c 756d  datasrc.df.colum
+000160a0: 6e73 2920 3d3d 206c 656e 2869 6172 6773  ns) == len(iargs
+000160b0: 292b 3120 616e 6420 6c65 6e28 6961 7267  )+1 and len(iarg
+000160c0: 7329 203d 3d20 6c65 6e28 6172 6773 293a  s) == len(args):
+000160d0: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+000160e0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+000160f0: 2e49 6e74 2720 696e 2073 7472 2874 7970  .Int' in str(typ
+00016100: 6528 6961 7267 735b 305d 2e69 6e64 6578  e(iargs[0].index
+00016110: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00016120: 2020 2020 2070 7269 6e74 2827 5741 524e       print('WARN
+00016130: 494e 473a 2070 6572 666f 726d 616e 6365  ING: performance
+00016140: 2070 656e 616c 7479 2061 6e64 2063 7261   penalty and cra
+00016150: 7368 206d 6179 206f 6363 7572 2077 6865  sh may occur whe
+00016160: 6e20 7573 696e 6720 696e 7436 3420 696e  n using int64 in
+00016170: 7374 6561 6420 6f66 2072 616e 6765 2069  stead of range i
+00016180: 6e64 6963 6573 2e27 290d 0a20 2020 2020  ndices.')..     
+00016190: 2020 2020 2020 2020 2020 2069 6620 2869             if (i
+000161a0: 6172 6773 5b30 5d2e 696e 6465 7820 3d3d  args[0].index ==
+000161b0: 2072 616e 6765 286c 656e 2869 6172 6773   range(len(iargs
+000161c0: 5b30 5d29 2929 2e61 6c6c 2829 3a0d 0a20  [0]))).all():.. 
+000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161e0: 2020 2070 7269 6e74 2827 202d 2046 6978     print(' - Fix
+000161f0: 2062 7920 2e72 6573 6574 5f69 6e64 6578   by .reset_index
+00016200: 2864 726f 703d 5472 7565 2927 290d 0a20  (drop=True)').. 
+00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016220: 2020 2072 6574 7572 6e20 5f63 7265 6174     return _creat
+00016230: 655f 6461 7461 7372 6328 6178 2c20 6461  e_datasrc(ax, da
+00016240: 7461 7372 632e 6466 5b64 6174 6173 7263  tasrc.df[datasrc
+00016250: 2e64 662e 636f 6c75 6d6e 735b 313a 5d5d  .df.columns[1:]]
+00016260: 2c20 6e63 6f6c 733d 6e63 6f6c 7329 0d0a  , ncols=ncols)..
+00016270: 2020 2020 2020 2020 6578 6365 7074 3a0d          except:.
+00016280: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00016290: 6e74 2827 5741 524e 494e 473a 2069 6e70  nt('WARNING: inp
+000162a0: 7574 2064 6174 6120 736f 7572 6365 206d  ut data source m
+000162b0: 6179 2063 6175 7365 2070 6572 666f 726d  ay cause perform
+000162c0: 616e 6365 2070 656e 616c 7479 2061 6e64  ance penalty and
+000162d0: 2063 7261 7368 2e27 290d 0a0d 0a20 2020   crash.')....   
+000162e0: 2061 7373 6572 7420 6c65 6e28 6461 7461   assert len(data
+000162f0: 7372 632e 6466 2e63 6f6c 756d 6e73 2920  src.df.columns) 
+00016300: 3e3d 206e 636f 6c73 2c20 2745 5252 4f52  >= ncols, 'ERROR
+00016310: 3a20 746f 6f20 6665 7720 636f 6c75 6d6e  : too few column
+00016320: 732f 6172 6773 2073 7570 706c 6965 6420  s/args supplied 
+00016330: 666f 7220 7468 6973 2070 6c6f 7427 0d0a  for this plot'..
+00016340: 0d0a 2020 2020 6966 2064 6174 6173 7263  ..    if datasrc
+00016350: 2e70 6572 696f 645f 6e73 203c 2030 3a0d  .period_ns < 0:.
+00016360: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+00016370: 5741 524e 494e 473a 2069 6e70 7574 2064  WARNING: input d
+00016380: 6174 6120 736f 7572 6365 2068 6173 2074  ata source has t
+00016390: 696d 6520 696e 2064 6573 6365 6e64 696e  ime in descendin
+000163a0: 6720 6f72 6465 722e 2054 7279 2073 6f72  g order. Try sor
+000163b0: 745f 7661 6c75 6573 2829 2062 6566 6f72  t_values() befor
+000163c0: 6520 6361 6c6c 696e 672e 2729 0d0a 0d0a  e calling.')....
+000163d0: 2020 2020 2320 4649 583a 2073 7475 7069      # FIX: stupi
+000163e0: 6420 5154 2062 7567 2063 6175 7365 7320  d QT bug causes 
+000163f0: 7265 6374 616e 676c 6573 206c 6172 6765  rectangles large
+00016400: 7220 7468 616e 2032 4720 746f 2066 6c69  r than 2G to fli
+00016410: 636b 6572 2c20 736f 2073 6361 6c65 2072  cker, so scale r
+00016420: 656e 6465 7269 6e67 2064 6f77 6e20 736f  endering down so
+00016430: 6d65 0d0a 2020 2020 2320 4649 583a 2050  me..    # FIX: P
+00016440: 7951 7420 352e 3135 2e32 206c 696e 6573  yQt 5.15.2 lines
+00016450: 203e 3165 3620 6172 6520 6265 696e 6720   >1e6 are being 
+00016460: 636c 6970 7065 6420 746f 2031 6536 2064  clipped to 1e6 d
+00016470: 7572 696e 6720 7468 6520 6669 7273 7420  uring the first 
+00016480: 7265 6e64 6572 2070 6173 732c 2073 6f20  render pass, so 
+00016490: 7363 616c 6520 646f 776e 2069 6620 3e31  scale down if >1
+000164a0: 6536 0d0a 2020 2020 6966 2064 6174 6173  e6..    if datas
+000164b0: 7263 2e64 662e 696c 6f63 5b3a 2c20 313a  rc.df.iloc[:, 1:
+000164c0: 5d2e 6d61 7828 6e75 6d65 7269 635f 6f6e  ].max(numeric_on
+000164d0: 6c79 3d54 7275 6529 2e6d 6178 2829 203e  ly=True).max() >
+000164e0: 2031 6536 3a0d 0a20 2020 2020 2020 2061   1e6:..        a
+000164f0: 782e 7662 2e79 7363 616c 652e 7365 745f  x.vb.yscale.set_
+00016500: 7363 616c 6528 696e 7428 3165 3629 290d  scale(int(1e6)).
+00016510: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
+00016520: 7372 630d 0a0d 0a0d 0a64 6566 205f 7365  src......def _se
+00016530: 745f 6461 7461 7372 6328 6178 2c20 6461  t_datasrc(ax, da
+00016540: 7461 7372 632c 2061 6464 636f 6c73 3d54  tasrc, addcols=T
+00016550: 7275 6529 3a0d 0a20 2020 2076 6965 7762  rue):..    viewb
+00016560: 6f78 203d 2061 782e 7662 0d0a 2020 2020  ox = ax.vb..    
+00016570: 6966 206e 6f74 2064 6174 6173 7263 2e73  if not datasrc.s
+00016580: 7461 6e64 616c 6f6e 653a 0d0a 2020 2020  tandalone:..    
+00016590: 2020 2020 6966 2076 6965 7762 6f78 2e64      if viewbox.d
+000165a0: 6174 6173 7263 2069 7320 4e6f 6e65 3a0d  atasrc is None:.
+000165b0: 0a20 2020 2020 2020 2020 2020 2076 6965  .            vie
+000165c0: 7762 6f78 2e73 6574 5f64 6174 6173 7263  wbox.set_datasrc
+000165d0: 2864 6174 6173 7263 2920 2320 666f 7220  (datasrc) # for 
+000165e0: 6d77 6865 656c 207a 6f6f 6d2d 7363 616c  mwheel zoom-scal
+000165f0: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
+00016600: 205f 7365 745f 785f 6c69 6d69 7473 2861   _set_x_limits(a
+00016610: 782c 2064 6174 6173 7263 290d 0a20 2020  x, datasrc)..   
+00016620: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00016630: 2020 2020 2020 2020 7430 203d 2076 6965          t0 = vie
+00016640: 7762 6f78 2e64 6174 6173 7263 2e78 2e6c  wbox.datasrc.x.l
+00016650: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
+00016660: 2020 2069 6620 6164 6463 6f6c 733a 0d0a     if addcols:..
+00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016680: 7669 6577 626f 782e 6461 7461 7372 632e  viewbox.datasrc.
+00016690: 6164 6463 6f6c 7328 6461 7461 7372 6329  addcols(datasrc)
+000166a0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000166b0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+000166c0: 2020 2020 2076 6965 7762 6f78 2e64 6174       viewbox.dat
+000166d0: 6173 7263 2e64 6620 3d20 6461 7461 7372  asrc.df = datasr
+000166e0: 632e 6466 0d0a 2020 2020 2020 2020 2020  c.df..          
+000166f0: 2020 2320 6368 6563 6b20 6966 2077 6520    # check if we 
+00016700: 6e65 6564 2074 6f20 7265 2d72 656e 6465  need to re-rende
+00016710: 7220 7072 6576 696f 7573 2070 6c6f 7473  r previous plots
+00016720: 2064 7565 2074 6f20 6368 616e 6765 6420   due to changed 
+00016730: 696e 6469 6365 730d 0a20 2020 2020 2020  indices..       
+00016740: 2020 2020 2069 6e64 6963 6573 5f75 7064       indices_upd
+00016750: 6174 6564 203d 2076 6965 7762 6f78 2e64  ated = viewbox.d
+00016760: 6174 6173 7263 2e74 696d 6562 6173 6564  atasrc.timebased
+00016770: 2829 2061 6e64 2074 3020 213d 2076 6965  () and t0 != vie
+00016780: 7762 6f78 2e64 6174 6173 7263 2e78 2e6c  wbox.datasrc.x.l
+00016790: 6f63 5b30 5d0d 0a20 2020 2020 2020 2020  oc[0]..         
+000167a0: 2020 2066 6f72 2069 7465 6d20 696e 2061     for item in a
+000167b0: 782e 6974 656d 733a 0d0a 2020 2020 2020  x.items:..      
+000167c0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
+000167d0: 6174 7472 2869 7465 6d2c 2027 6461 7461  attr(item, 'data
+000167e0: 7372 6327 2920 616e 6420 6e6f 7420 6974  src') and not it
+000167f0: 656d 2e64 6174 6173 7263 2e73 7461 6e64  em.datasrc.stand
+00016800: 616c 6f6e 653a 0d0a 2020 2020 2020 2020  alone:..        
+00016810: 2020 2020 2020 2020 2020 2020 6974 656d              item
+00016820: 2e64 6174 6173 7263 2e73 6574 5f64 6628  .datasrc.set_df(
+00016830: 7669 6577 626f 782e 6461 7461 7372 632e  viewbox.datasrc.
+00016840: 6466 2920 2320 6576 6572 7920 706c 6f74  df) # every plot
+00016850: 2068 6572 6520 6e6f 7720 6861 7320 7468   here now has th
+00016860: 6520 7361 6d65 2074 696d 652d 6672 616d  e same time-fram
+00016870: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00016880: 2020 2020 2020 2069 6620 696e 6469 6365         if indice
+00016890: 735f 7570 6461 7465 643a 0d0a 2020 2020  s_updated:..    
+000168a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168b0: 2020 2020 5f73 7461 7274 5f76 6973 7561      _start_visua
+000168c0: 6c5f 7570 6461 7465 2869 7465 6d29 0d0a  l_update(item)..
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168e0: 2020 2020 2020 2020 5f65 6e64 5f76 6973          _end_vis
+000168f0: 7561 6c5f 7570 6461 7465 2869 7465 6d29  ual_update(item)
+00016900: 0d0a 2020 2020 2020 2020 2020 2020 5f73  ..            _s
+00016910: 6574 5f78 5f6c 696d 6974 7328 6178 2c20  et_x_limits(ax, 
+00016920: 6461 7461 7372 6329 0d0a 2020 2020 2020  datasrc)..      
+00016930: 2020 2020 2020 7669 6577 626f 782e 7365        viewbox.se
+00016940: 745f 6461 7461 7372 6328 7669 6577 626f  t_datasrc(viewbo
+00016950: 782e 6461 7461 7372 6329 2023 2075 7064  x.datasrc) # upd
+00016960: 6174 6520 7a6f 6f6d 0d0a 2020 2020 656c  ate zoom..    el
+00016970: 7365 3a0d 0a20 2020 2020 2020 2076 6965  se:..        vie
+00016980: 7762 6f78 2e73 7461 6e64 616c 6f6e 6573  wbox.standalones
+00016990: 2e61 6464 2864 6174 6173 7263 290d 0a20  .add(datasrc).. 
+000169a0: 2020 2020 2020 2064 6174 6173 7263 2e75         datasrc.u
+000169b0: 7064 6174 655f 696e 6974 5f78 2876 6965  pdate_init_x(vie
+000169c0: 7762 6f78 2e69 6e69 745f 7374 6570 7329  wbox.init_steps)
+000169d0: 0d0a 2020 2020 2020 2020 6966 2064 6174  ..        if dat
+000169e0: 6173 7263 2e74 696d 6562 6173 6564 2829  asrc.timebased()
+000169f0: 2061 6e64 2076 6965 7762 6f78 2e64 6174   and viewbox.dat
+00016a00: 6173 7263 2069 7320 6e6f 7420 4e6f 6e65  asrc is not None
+00016a10: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00016a20: 2320 7072 696e 7428 2757 4152 4e49 4e47  # print('WARNING
+00016a30: 3a20 7265 2d69 6e64 6578 696e 6720 7374  : re-indexing st
+00016a40: 616e 6461 6c6f 6e65 2c20 7469 6d65 2d62  andalone, time-b
+00016a50: 6173 6564 2070 6c6f 7427 290d 0a20 2020  ased plot')..   
+00016a60: 2020 2020 2020 2020 2076 6466 203d 2076           vdf = v
+00016a70: 6965 7762 6f78 2e64 6174 6173 7263 2e64  iewbox.datasrc.d
+00016a80: 660d 0a20 2020 2020 2020 2020 2020 2064  f..            d
+00016a90: 203d 207b 763a 6b20 666f 7220 6b2c 7620   = {v:k for k,v 
+00016aa0: 696e 2065 6e75 6d65 7261 7465 2876 6466  in enumerate(vdf
+00016ab0: 5b76 6466 2e63 6f6c 756d 6e73 5b30 5d5d  [vdf.columns[0]]
+00016ac0: 297d 0d0a 2020 2020 2020 2020 2020 2020  )}..            
+00016ad0: 6461 7461 7372 632e 6466 2e69 6e64 6578  datasrc.df.index
+00016ae0: 203d 205b 645b 695d 2066 6f72 2069 2069   = [d[i] for i i
+00016af0: 6e20 6461 7461 7372 632e 6466 5b64 6174  n datasrc.df[dat
+00016b00: 6173 7263 2e64 662e 636f 6c75 6d6e 735b  asrc.df.columns[
+00016b10: 305d 5d5d 0d0a 2020 2020 2020 2020 2323  0]]]..        ##
+00016b20: 2069 6620 6e6f 7420 7669 6577 626f 782e   if not viewbox.
+00016b30: 785f 696e 6465 7865 643a 0d0a 2020 2020  x_indexed:..    
+00016b40: 2020 2020 2020 2020 2323 205f 7365 745f          ## _set_
+00016b50: 785f 6c69 6d69 7473 2861 782c 2064 6174  x_limits(ax, dat
+00016b60: 6173 7263 290d 0a20 2020 2023 2075 7064  asrc)..    # upd
+00016b70: 6174 6520 7065 7269 6f64 2069 6620 7468  ate period if th
+00016b80: 6973 2064 6174 6173 7263 2068 6173 2068  is datasrc has h
+00016b90: 6967 6865 7220 7469 6d65 2072 6573 6f6c  igher time resol
+00016ba0: 7574 696f 6e0d 0a20 2020 2067 6c6f 6261  ution..    globa
+00016bb0: 6c20 6570 6f63 685f 7065 7269 6f64 0d0a  l epoch_period..
+00016bc0: 2020 2020 6966 2064 6174 6173 7263 2e74      if datasrc.t
+00016bd0: 696d 6562 6173 6564 2829 2061 6e64 2028  imebased() and (
+00016be0: 6570 6f63 685f 7065 7269 6f64 203e 2031  epoch_period > 1
+00016bf0: 6537 206f 7220 6e6f 7420 6461 7461 7372  e7 or not datasr
+00016c00: 632e 7374 616e 6461 6c6f 6e65 293a 0d0a  c.standalone):..
+00016c10: 2020 2020 2020 2020 6570 5f73 6563 7320          ep_secs 
+00016c20: 3d20 6461 7461 7372 632e 7065 7269 6f64  = datasrc.period
+00016c30: 5f6e 7320 2f20 3165 390d 0a20 2020 2020  _ns / 1e9..     
+00016c40: 2020 2065 706f 6368 5f70 6572 696f 6420     epoch_period 
+00016c50: 3d20 6570 5f73 6563 7320 6966 2065 705f  = ep_secs if ep_
+00016c60: 7365 6373 203c 2065 706f 6368 5f70 6572  secs < epoch_per
+00016c70: 696f 6420 656c 7365 2065 706f 6368 5f70  iod else epoch_p
+00016c80: 6572 696f 640d 0a0d 0a0d 0a64 6566 205f  eriod......def _
+00016c90: 6861 735f 7469 6d65 636f 6c28 6466 293a  has_timecol(df):
+00016ca0: 0d0a 2020 2020 7265 7475 726e 206c 656e  ..    return len
+00016cb0: 2864 662e 636f 6c75 6d6e 7329 203e 3d20  (df.columns) >= 
+00016cc0: 320d 0a0d 0a0d 0a64 6566 205f 7365 745f  2......def _set_
+00016cd0: 6d61 785f 7a6f 6f6d 2876 6273 293a 0d0a  max_zoom(vbs):..
+00016ce0: 2020 2020 2727 2753 6574 2074 6865 2072      '''Set the r
+00016cf0: 656c 6174 6976 6520 616c 6c6f 7765 6420  elative allowed 
+00016d00: 7a6f 6f6d 206c 6576 656c 2062 6574 7765  zoom level betwe
+00016d10: 656e 2061 7865 7320 6772 6f75 7073 2c20  en axes groups, 
+00016d20: 7768 6572 6520 7468 6520 6c6f 7765 7374  where the lowest
+00016d30: 2d72 6573 6f6c 7574 696f 6e0d 0a20 2020  -resolution..   
+00016d40: 2020 2020 706c 6f74 2069 6e20 6561 6368      plot in each
+00016d50: 2067 726f 7570 2075 7365 7320 6d61 785f   group uses max_
+00016d60: 7a6f 6f6d 5f70 6f69 6e74 732c 2077 6869  zoom_points, whi
+00016d70: 6c65 2074 6865 206f 7468 6572 7320 6765  le the others ge
+00016d80: 7420 6120 7363 616c 6520 3e3d 3120 6f66  t a scale >=1 of
+00016d90: 2074 6865 6972 0d0a 2020 2020 2020 2072   their..       r
+00016da0: 6573 7065 6374 6976 6520 6869 6768 6573  espective highes
+00016db0: 7420 7a6f 6f6d 206c 6576 656c 2e27 2727  t zoom level.'''
+00016dc0: 0d0a 2020 2020 6772 6f75 7073 203d 2064  ..    groups = d
+00016dd0: 6566 6175 6c74 6469 6374 2873 6574 290d  efaultdict(set).
+00016de0: 0a20 2020 2066 6f72 2076 6220 696e 2076  .    for vb in v
+00016df0: 6273 3a0d 0a20 2020 2020 2020 206d 6173  bs:..        mas
+00016e00: 7465 725f 7662 203d 2076 622e 6c69 6e6b  ter_vb = vb.link
+00016e10: 6564 5669 6577 2830 290d 0a20 2020 2020  edView(0)..     
+00016e20: 2020 2069 6620 7662 2e64 6174 6173 7263     if vb.datasrc
+00016e30: 2061 6e64 206d 6173 7465 725f 7662 2061   and master_vb a
+00016e40: 6e64 206d 6173 7465 725f 7662 2e64 6174  nd master_vb.dat
+00016e50: 6173 7263 3a0d 0a20 2020 2020 2020 2020  asrc:..         
+00016e60: 2020 2067 726f 7570 735b 6d61 7374 6572     groups[master
+00016e70: 5f76 625d 2e61 6464 2876 6229 0d0a 2020  _vb].add(vb)..  
+00016e80: 2020 2020 2020 2020 2020 6772 6f75 7073            groups
+00016e90: 5b6d 6173 7465 725f 7662 5d2e 6164 6428  [master_vb].add(
+00016ea0: 6d61 7374 6572 5f76 6229 0d0a 2020 2020  master_vb)..    
+00016eb0: 666f 7220 6772 6f75 7020 696e 2067 726f  for group in gro
+00016ec0: 7570 732e 7661 6c75 6573 2829 3a0d 0a20  ups.values():.. 
+00016ed0: 2020 2020 2020 206d 696e 6c65 6e20 3d20         minlen = 
+00016ee0: 6d69 6e28 6c65 6e28 7662 2e64 6174 6173  min(len(vb.datas
+00016ef0: 7263 2e64 6629 2066 6f72 2076 6220 696e  rc.df) for vb in
+00016f00: 2067 726f 7570 290d 0a20 2020 2020 2020   group)..       
+00016f10: 2066 6f72 2076 6220 696e 2067 726f 7570   for vb in group
+00016f20: 3a0d 0a20 2020 2020 2020 2020 2020 2076  :..            v
+00016f30: 622e 6d61 785f 7a6f 6f6d 5f70 6f69 6e74  b.max_zoom_point
+00016f40: 735f 6620 3d20 6c65 6e28 7662 2e64 6174  s_f = len(vb.dat
+00016f50: 6173 7263 2e64 6629 202f 206d 696e 6c65  asrc.df) / minle
+00016f60: 6e0d 0a0d 0a0d 0a64 6566 205f 6164 6a75  n......def _adju
+00016f70: 7374 5f72 656e 6b6f 5f64 6174 6173 7263  st_renko_datasrc
+00016f80: 2862 696e 732c 2073 7465 702c 2064 6174  (bins, step, dat
+00016f90: 6173 7263 293a 0d0a 2020 2020 6966 206e  asrc):..    if n
+00016fa0: 6f74 2062 696e 7320 616e 6420 6e6f 7420  ot bins and not 
+00016fb0: 7374 6570 3a0d 0a20 2020 2020 2020 2062  step:..        b
+00016fc0: 696e 7320 3d20 3530 0d0a 2020 2020 6966  ins = 50..    if
+00016fd0: 206e 6f74 2073 7465 703a 0d0a 2020 2020   not step:..    
+00016fe0: 2020 2020 7374 6570 203d 2028 6461 7461      step = (data
+00016ff0: 7372 632e 792e 6d61 7828 292d 6461 7461  src.y.max()-data
+00017000: 7372 632e 792e 6d69 6e28 2929 202f 2062  src.y.min()) / b
+00017010: 696e 730d 0a20 2020 2062 7269 636b 7320  ins..    bricks 
+00017020: 3d20 6461 7461 7372 632e 792e 6469 6666  = datasrc.y.diff
+00017030: 2829 202f 2073 7465 700d 0a20 2020 2062  () / step..    b
+00017040: 7269 636b 7320 3d20 2864 6174 6173 7263  ricks = (datasrc
+00017050: 2e79 5b62 7269 636b 732e 6973 6e75 6c6c  .y[bricks.isnull
+00017060: 2829 207c 2028 6272 6963 6b73 2e61 6273  () | (bricks.abs
+00017070: 2829 3e3d 302e 3529 5d20 2f20 7374 6570  ()>=0.5)] / step
+00017080: 292e 726f 756e 6428 292e 6173 7479 7065  ).round().astype
+00017090: 2869 6e74 290d 0a20 2020 2065 7874 7261  (int)..    extra
+000170a0: 7320 3d20 6461 7461 7372 632e 6466 2e69  s = datasrc.df.i
+000170b0: 6c6f 635b 3a2c 2064 6174 6173 7263 2e63  loc[:, datasrc.c
+000170c0: 6f6c 5f64 6174 615f 6f66 6673 6574 2b31  ol_data_offset+1
+000170d0: 3a5d 0d0a 2020 2020 7473 203d 2064 6174  :]..    ts = dat
+000170e0: 6173 7263 2e78 5b62 7269 636b 732e 696e  asrc.x[bricks.in
+000170f0: 6465 785d 0d0a 2020 2020 7570 203d 2062  dex]..    up = b
+00017100: 7269 636b 732e 696c 6f63 5b30 5d20 2b20  ricks.iloc[0] + 
+00017110: 310d 0a20 2020 2064 6e20 3d20 7570 202d  1..    dn = up -
+00017120: 2032 0d0a 2020 2020 6461 7461 203d 205b   2..    data = [
+00017130: 5d0d 0a20 2020 2066 6f72 2074 2c69 2c62  ]..    for t,i,b
+00017140: 7269 636b 2069 6e20 7a69 7028 7473 2c20  rick in zip(ts, 
+00017150: 6272 6963 6b73 2e69 6e64 6578 2c20 6272  bricks.index, br
+00017160: 6963 6b73 293a 0d0a 2020 2020 2020 2020  icks):..        
+00017170: 7320 3d20 300d 0a20 2020 2020 2020 2069  s = 0..        i
+00017180: 6620 6272 6963 6b20 3e3d 2075 703a 0d0a  f brick >= up:..
+00017190: 2020 2020 2020 2020 2020 2020 7830 2c78              x0,x
+000171a0: 312c 7320 3d20 7570 2d31 2c62 7269 636b  1,s = up-1,brick
+000171b0: 2c2b 310d 0a20 2020 2020 2020 2020 2020  ,+1..           
+000171c0: 2075 7020 3d20 6272 6963 6b2b 310d 0a20   up = brick+1.. 
+000171d0: 2020 2020 2020 2020 2020 2064 6e20 3d20             dn = 
+000171e0: 6272 6963 6b2d 320d 0a20 2020 2020 2020  brick-2..       
+000171f0: 2065 6c69 6620 6272 6963 6b20 3c3d 2064   elif brick <= d
+00017200: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
+00017210: 7830 2c78 312c 7320 3d20 646e 2c62 7269  x0,x1,s = dn,bri
+00017220: 636b 2d31 2c2d 310d 0a20 2020 2020 2020  ck-1,-1..       
+00017230: 2020 2020 2075 7020 3d20 6272 6963 6b2b       up = brick+
+00017240: 320d 0a20 2020 2020 2020 2020 2020 2064  2..            d
+00017250: 6e20 3d20 6272 6963 6b2d 310d 0a20 2020  n = brick-1..   
+00017260: 2020 2020 2069 6620 733a 0d0a 2020 2020       if s:..    
+00017270: 2020 2020 2020 2020 666f 7220 7820 696e          for x in
+00017280: 2072 616e 6765 2878 302c 2078 312c 2073   range(x0, x1, s
+00017290: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000172a0: 2020 2020 7464 203d 2061 6273 2878 312d      td = abs(x1-
+000172b0: 7829 2d31 0d0a 2020 2020 2020 2020 2020  x)-1..          
+000172c0: 2020 2020 2020 6473 203d 2030 2069 6620        ds = 0 if 
+000172d0: 733e 3020 656c 7365 2073 7465 700d 0a20  s>0 else step.. 
+000172e0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+000172f0: 203d 2078 2a73 7465 700d 0a20 2020 2020   = x*step..     
+00017300: 2020 2020 2020 2020 2020 207a 203d 206c             z = l
+00017310: 6973 7428 6578 7472 6173 2e6c 6f63 5b69  ist(extras.loc[i
+00017320: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017330: 2020 2020 6461 7461 2e61 7070 656e 6428      data.append(
+00017340: 5b74 2d74 642c 2079 2b64 732c 2079 2b73  [t-td, y+ds, y+s
+00017350: 7465 702d 6473 2c20 792b 7374 6570 2c20  tep-ds, y+step, 
+00017360: 795d 202b 207a 290d 0a20 2020 2064 6174  y] + z)..    dat
+00017370: 6173 7263 2e73 6574 5f64 6628 7064 2e44  asrc.set_df(pd.D
+00017380: 6174 6146 7261 6d65 2864 6174 612c 2063  ataFrame(data, c
+00017390: 6f6c 756d 6e73 3d27 7469 6d65 206f 7065  olumns='time ope
+000173a0: 6e20 636c 6f73 6520 6869 6768 206c 6f77  n close high low
+000173b0: 272e 7370 6c69 7428 292b 6c69 7374 2865  '.split()+list(e
+000173c0: 7874 7261 732e 636f 6c75 6d6e 7329 2929  xtras.columns)))
+000173d0: 0d0a 0d0a 0d0a 6465 6620 5f61 646a 7573  ......def _adjus
+000173e0: 745f 7265 6e6b 6f5f 6c6f 675f 6461 7461  t_renko_log_data
+000173f0: 7372 6328 6269 6e73 2c20 7374 6570 2c20  src(bins, step, 
+00017400: 6461 7461 7372 6329 3a0d 0a20 2020 2064  datasrc):..    d
+00017410: 6174 6173 7263 2e64 662e 6c6f 635b 3a2c  atasrc.df.loc[:,
+00017420: 6461 7461 7372 632e 6466 2e63 6f6c 756d  datasrc.df.colum
+00017430: 735b 315d 5d20 3d20 6e70 2e6c 6f67 3130  s[1]] = np.log10
+00017440: 2864 6174 6173 7263 2e64 662e 696c 6f63  (datasrc.df.iloc
+00017450: 5b3a 2c31 5d29 0d0a 2020 2020 5f61 646a  [:,1])..    _adj
+00017460: 7573 745f 7265 6e6b 6f5f 6461 7461 7372  ust_renko_datasr
+00017470: 6328 6269 6e73 2c20 7374 6570 2c20 6461  c(bins, step, da
+00017480: 7461 7372 6329 0d0a 2020 2020 6461 7461  tasrc)..    data
+00017490: 7372 632e 6466 2e6c 6f63 5b3a 2c64 6174  src.df.loc[:,dat
+000174a0: 6173 7263 2e64 662e 636f 6c75 6d73 5b31  asrc.df.colums[1
+000174b0: 3a35 5d5d 203d 2031 302a 2a64 6174 6173  :5]] = 10**datas
+000174c0: 7263 2e64 662e 696c 6f63 5b3a 2c31 3a35  rc.df.iloc[:,1:5
+000174d0: 5d0d 0a0d 0a0d 0a64 6566 205f 6164 6a75  ]......def _adju
+000174e0: 7374 5f76 6f6c 756d 655f 6461 7461 7372  st_volume_datasr
+000174f0: 6328 6461 7461 7372 6329 3a0d 0a20 2020  c(datasrc):..   
+00017500: 2069 6620 6c65 6e28 6461 7461 7372 632e   if len(datasrc.
+00017510: 6466 2e63 6f6c 756d 6e73 2920 3c3d 2034  df.columns) <= 4
+00017520: 3a0d 0a20 2020 2020 2020 2064 6174 6173  :..        datas
+00017530: 7263 2e64 662e 696e 7365 7274 2833 2c20  rc.df.insert(3, 
+00017540: 275f 7a65 726f 5f27 2c20 5b30 5d2a 6c65  '_zero_', [0]*le
+00017550: 6e28 6461 7461 7372 632e 6466 2929 2023  n(datasrc.df)) #
+00017560: 2062 6173 6520 6f66 2063 616e 646c 6573   base of candles
+00017570: 2069 7320 616c 7761 7973 207a 6572 6f0d   is always zero.
+00017580: 0a20 2020 2064 6174 6173 7263 2e73 6574  .    datasrc.set
+00017590: 5f64 6628 6461 7461 7372 632e 6466 2e69  _df(datasrc.df.i
+000175a0: 6c6f 635b 3a2c 5b30 2c33 2c34 2c31 2c32  loc[:,[0,3,4,1,2
+000175b0: 5d5d 2920 2320 7265 2d61 7272 616e 6765  ]]) # re-arrange
+000175c0: 2063 6f6c 756d 6e73 2066 6f72 2072 656e   columns for ren
+000175d0: 6465 7269 6e67 0d0a 2020 2020 6461 7461  dering..    data
+000175e0: 7372 632e 7363 616c 655f 636f 6c73 203d  src.scale_cols =
+000175f0: 205b 312c 2032 5d20 2320 7363 616c 6520   [1, 2] # scale 
+00017600: 6279 2062 6f74 6820 6261 7365 6c69 6e65  by both baseline
+00017610: 2061 6e64 2076 6f6c 756d 650d 0a0d 0a0d   and volume.....
+00017620: 0a64 6566 205f 7072 6561 646a 7573 745f  .def _preadjust_
+00017630: 686f 7269 7a5f 6461 7461 7372 6328 6461  horiz_datasrc(da
+00017640: 7461 7372 6329 3a0d 0a20 2020 2061 7272  tasrc):..    arr
+00017650: 6179 6966 7920 3d20 6c61 6d62 6461 2064  ayify = lambda d
+00017660: 3a20 642e 7661 6c75 6573 2069 6620 7479  : d.values if ty
+00017670: 7065 2864 2920 3d3d 2070 642e 4461 7461  pe(d) == pd.Data
+00017680: 4672 616d 6520 656c 7365 2064 0d0a 2020  Frame else d..  
+00017690: 2020 2320 6372 6561 7465 2061 2064 6174    # create a dat
+000176a0: 6166 7261 6d65 2066 726f 6d20 7468 6520  aframe from the 
+000176b0: 696e 7075 7420 6172 7261 790d 0a20 2020  input array..   
+000176c0: 2074 696d 6573 203d 205b 7420 666f 7220   times = [t for 
+000176d0: 742c 726f 7720 696e 2064 6174 6173 7263  t,row in datasrc
+000176e0: 5d0d 0a20 2020 2069 6620 6c65 6e28 7469  ]..    if len(ti
+000176f0: 6d65 7329 203d 3d20 313a 2023 2061 6464  mes) == 1: # add
+00017700: 2061 6e20 656d 7074 7920 7469 6d65 2073   an empty time s
+00017710: 6c6f 740d 0a20 2020 2020 2020 2074 696d  lot..        tim
+00017720: 6573 203d 205b 7469 6d65 735b 305d 2c20  es = [times[0], 
+00017730: 7469 6d65 735b 305d 2b31 5d0d 0a20 2020  times[0]+1]..   
+00017740: 2020 2020 2064 6174 6173 7263 203d 2064       datasrc = d
+00017750: 6174 6173 7263 202b 205b 5b74 696d 6573  atasrc + [[times
+00017760: 5b31 5d2c 205b 2870 2c30 2920 666f 7220  [1], [(p,0) for 
+00017770: 702c 7620 696e 2061 7272 6179 6966 7928  p,v in arrayify(
+00017780: 6461 7461 7372 635b 305d 5b31 5d29 5d5d  datasrc[0][1])]]
+00017790: 5d0d 0a20 2020 2064 6174 6120 3d20 5b5b  ]..    data = [[
+000177a0: 6520 666f 7220 7620 696e 2061 7272 6179  e for v in array
+000177b0: 6966 7928 726f 7729 2066 6f72 2065 2069  ify(row) for e i
+000177c0: 6e20 765d 2066 6f72 2074 2c72 6f77 2069  n v] for t,row i
+000177d0: 6e20 6461 7461 7372 635d 0d0a 2020 2020  n datasrc]..    
+000177e0: 6d61 7863 6f6c 7320 3d20 6d61 7828 6c65  maxcols = max(le
+000177f0: 6e28 726f 7729 2066 6f72 2072 6f77 2069  n(row) for row i
+00017800: 6e20 6461 7461 290d 0a20 2020 2072 6574  n data)..    ret
+00017810: 7572 6e20 7064 2e44 6174 6146 7261 6d65  urn pd.DataFrame
+00017820: 2863 6f6c 756d 6e73 3d72 616e 6765 286d  (columns=range(m
+00017830: 6178 636f 6c73 292c 2064 6174 613d 6461  axcols), data=da
+00017840: 7461 2c20 696e 6465 783d 7469 6d65 7329  ta, index=times)
+00017850: 0d0a 0d0a 0d0a 6465 6620 5f61 646a 7573  ......def _adjus
+00017860: 745f 686f 7269 7a5f 6461 7461 7372 6328  t_horiz_datasrc(
+00017870: 6461 7461 7372 6329 3a0d 0a20 2020 2023  datasrc):..    #
+00017880: 2074 6f20 6265 2061 626c 6520 746f 2073   to be able to s
+00017890: 6361 6c65 2070 726f 7065 726c 792c 206d  cale properly, m
+000178a0: 6f76 6520 7468 6520 6c61 7374 2074 776f  ove the last two
+000178b0: 2076 616c 7565 7320 746f 2074 6865 206c   values to the l
+000178c0: 6173 7420 7477 6f20 636f 6c75 6d6e 730d  ast two columns.
+000178d0: 0a20 2020 2076 616c 7565 7320 3d20 6461  .    values = da
+000178e0: 7461 7372 632e 6466 2e69 6c6f 635b 3a2c  tasrc.df.iloc[:,
+000178f0: 2031 3a5d 2e76 616c 7565 730d 0a20 2020   1:].values..   
+00017900: 2066 6f72 2069 2c6e 726f 7720 696e 2065   for i,nrow in e
+00017910: 6e75 6d65 7261 7465 2876 616c 7565 7329  numerate(values)
+00017920: 3a0d 0a20 2020 2020 2020 206f 726f 7720  :..        orow 
+00017930: 3d20 6e72 6f77 5b7e 6e70 2e69 736e 616e  = nrow[~np.isnan
+00017940: 286e 726f 7729 5d0d 0a20 2020 2020 2020  (nrow)]..       
+00017950: 2069 6620 6c65 6e28 6e72 6f77 2920 3d3d   if len(nrow) ==
+00017960: 206c 656e 286f 726f 7729 206f 7220 6c65   len(orow) or le
+00017970: 6e28 6f72 6f77 2920 3c3d 2032 3a0d 0a20  n(orow) <= 2:.. 
+00017980: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00017990: 6e75 650d 0a20 2020 2020 2020 206e 726f  nue..        nro
+000179a0: 775b 2d32 3a5d 203d 206f 726f 775b 2d32  w[-2:] = orow[-2
+000179b0: 3a5d 0d0a 2020 2020 2020 2020 6e72 6f77  :]..        nrow
+000179c0: 5b6c 656e 286f 726f 7729 2d32 3a6c 656e  [len(orow)-2:len
+000179d0: 286f 726f 7729 5d20 3d20 6e70 2e6e 616e  (orow)] = np.nan
+000179e0: 0d0a 2020 2020 6461 7461 7372 632e 6466  ..    datasrc.df
+000179f0: 5b64 6174 6173 7263 2e64 662e 636f 6c75  [datasrc.df.colu
+00017a00: 6d6e 735b 313a 5d5d 203d 2076 616c 7565  mns[1:]] = value
+00017a10: 730d 0a0d 0a0d 0a64 6566 205f 6164 6a75  s......def _adju
+00017a20: 7374 5f62 6172 5f64 6174 6173 7263 2864  st_bar_datasrc(d
+00017a30: 6174 6173 7263 2c20 6f72 6465 725f 636f  atasrc, order_co
+00017a40: 6c73 3d54 7275 6529 3a0d 0a20 2020 2069  ls=True):..    i
+00017a50: 6620 6c65 6e28 6461 7461 7372 632e 6466  f len(datasrc.df
+00017a60: 2e63 6f6c 756d 6e73 2920 3c3d 2032 3a0d  .columns) <= 2:.
+00017a70: 0a20 2020 2020 2020 2064 6174 6173 7263  .        datasrc
+00017a80: 2e64 662e 696e 7365 7274 2831 2c20 275f  .df.insert(1, '_
+00017a90: 6261 7365 5f27 2c20 5b30 5d2a 6c65 6e28  base_', [0]*len(
+00017aa0: 6461 7461 7372 632e 6466 2929 2023 2062  datasrc.df)) # b
+00017ab0: 6173 650d 0a20 2020 2069 6620 6c65 6e28  ase..    if len(
+00017ac0: 6461 7461 7372 632e 6466 2e63 6f6c 756d  datasrc.df.colum
+00017ad0: 6e73 2920 3c3d 2034 3a0d 0a20 2020 2020  ns) <= 4:..     
+00017ae0: 2020 2064 6174 6173 7263 2e64 662e 696e     datasrc.df.in
+00017af0: 7365 7274 2831 2c20 275f 6f70 656e 5f27  sert(1, '_open_'
+00017b00: 2c20 205b 305d 2a6c 656e 2864 6174 6173  ,  [0]*len(datas
+00017b10: 7263 2e64 6629 2920 2320 226f 7065 6e22  rc.df)) # "open"
+00017b20: 2066 6f72 2063 6f6c 6f72 0d0a 2020 2020   for color..    
+00017b30: 2020 2020 6461 7461 7372 632e 6466 2e69      datasrc.df.i
+00017b40: 6e73 6572 7428 322c 2027 5f63 6c6f 7365  nsert(2, '_close
+00017b50: 5f27 2c20 6461 7461 7372 632e 6466 2e69  _', datasrc.df.i
+00017b60: 6c6f 635b 3a2c 2033 5d29 2023 2022 636c  loc[:, 3]) # "cl
+00017b70: 6f73 6522 2028 6163 7475 616c 2062 6172  ose" (actual bar
+00017b80: 2076 616c 7565 2920 666f 7220 636f 6c6f   value) for colo
+00017b90: 720d 0a20 2020 2069 6620 6f72 6465 725f  r..    if order_
+00017ba0: 636f 6c73 3a0d 0a20 2020 2020 2020 2064  cols:..        d
+00017bb0: 6174 6173 7263 2e73 6574 5f64 6628 6461  atasrc.set_df(da
+00017bc0: 7461 7372 632e 6466 2e69 6c6f 635b 3a2c  tasrc.df.iloc[:,
+00017bd0: 5b30 2c33 2c34 2c31 2c32 5d5d 2920 2320  [0,3,4,1,2]]) # 
+00017be0: 7265 2d61 7272 616e 6765 2063 6f6c 756d  re-arrange colum
+00017bf0: 6e73 2066 6f72 2072 656e 6465 7269 6e67  ns for rendering
+00017c00: 0d0a 2020 2020 6461 7461 7372 632e 7363  ..    datasrc.sc
+00017c10: 616c 655f 636f 6c73 203d 205b 312c 2032  ale_cols = [1, 2
+00017c20: 5d20 2320 7363 616c 6520 6279 2062 6f74  ] # scale by bot
+00017c30: 6820 6261 7365 6c69 6e65 2061 6e64 2076  h baseline and v
+00017c40: 6f6c 756d 650d 0a0d 0a0d 0a64 6566 205f  olume......def _
+00017c50: 7570 6461 7465 5f64 6174 6128 7072 6561  update_data(prea
+00017c60: 646a 7573 7466 756e 632c 2061 646a 7573  djustfunc, adjus
+00017c70: 7466 756e 632c 2069 7465 6d2c 2064 732c  tfunc, item, ds,
+00017c80: 2067 6678 3d54 7275 6529 3a0d 0a20 2020   gfx=True):..   
+00017c90: 2069 6620 7072 6561 646a 7573 7466 756e   if preadjustfun
+00017ca0: 633a 0d0a 2020 2020 2020 2020 6473 203d  c:..        ds =
+00017cb0: 2070 7265 6164 6a75 7374 6675 6e63 2864   preadjustfunc(d
+00017cc0: 7329 0d0a 2020 2020 6473 203d 205f 6372  s)..    ds = _cr
+00017cd0: 6561 7465 5f64 6174 6173 7263 2869 7465  eate_datasrc(ite
+00017ce0: 6d2e 6178 2c20 6473 290d 0a20 2020 2069  m.ax, ds)..    i
+00017cf0: 6620 6164 6a75 7374 6675 6e63 3a0d 0a20  f adjustfunc:.. 
+00017d00: 2020 2020 2020 2061 646a 7573 7466 756e         adjustfun
+00017d10: 6328 6473 290d 0a20 2020 2063 7320 3d20  c(ds)..    cs = 
+00017d20: 6c69 7374 2869 7465 6d2e 6461 7461 7372  list(item.datasr
+00017d30: 632e 6466 2e63 6f6c 756d 6e73 5b3a 315d  c.df.columns[:1]
+00017d40: 2920 2b20 6c69 7374 2869 7465 6d2e 6461  ) + list(item.da
+00017d50: 7461 7372 632e 6466 2e63 6f6c 756d 6e73  tasrc.df.columns
+00017d60: 5b69 7465 6d2e 6461 7461 7372 632e 636f  [item.datasrc.co
+00017d70: 6c5f 6461 7461 5f6f 6666 7365 743a 5d29  l_data_offset:])
+00017d80: 0d0a 2020 2020 6966 206c 656e 2863 7329  ..    if len(cs)
+00017d90: 203e 3d20 6c65 6e28 6473 2e64 662e 636f   >= len(ds.df.co
+00017da0: 6c75 6d6e 7329 3a0d 0a20 2020 2020 2020  lumns):..       
+00017db0: 2064 732e 6466 2e63 6f6c 756d 6e73 203d   ds.df.columns =
+00017dc0: 2063 735b 3a6c 656e 2864 732e 6466 2e63   cs[:len(ds.df.c
+00017dd0: 6f6c 756d 6e73 295d 0d0a 2020 2020 6974  olumns)]..    it
+00017de0: 656d 2e64 6174 6173 7263 2e75 7064 6174  em.datasrc.updat
+00017df0: 6528 6473 290d 0a20 2020 205f 7365 745f  e(ds)..    _set_
+00017e00: 6461 7461 7372 6328 6974 656d 2e61 782c  datasrc(item.ax,
+00017e10: 2069 7465 6d2e 6461 7461 7372 632c 2061   item.datasrc, a
+00017e20: 6464 636f 6c73 3d46 616c 7365 290d 0a20  ddcols=False).. 
+00017e30: 2020 2069 6620 6766 783a 0d0a 2020 2020     if gfx:..    
+00017e40: 2020 2020 6974 656d 2e75 7064 6174 655f      item.update_
+00017e50: 6766 7828 290d 0a0d 0a0d 0a64 6566 205f  gfx()......def _
+00017e60: 7570 6461 7465 5f67 6678 2869 7465 6d29  update_gfx(item)
+00017e70: 3a0d 0a20 2020 205f 7374 6172 745f 7669  :..    _start_vi
+00017e80: 7375 616c 5f75 7064 6174 6528 6974 656d  sual_update(item
+00017e90: 290d 0a20 2020 2066 6f72 2069 2069 6e20  )..    for i in 
+00017ea0: 6974 656d 2e61 782e 6974 656d 733a 0d0a  item.ax.items:..
+00017eb0: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
+00017ec0: 6974 656d 206f 7220 6e6f 7420 6861 7361  item or not hasa
+00017ed0: 7474 7228 692c 2027 6461 7461 7372 6327  ttr(i, 'datasrc'
+00017ee0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00017ef0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00017f00: 2020 6c63 203d 206c 656e 2869 7465 6d2e    lc = len(item.
+00017f10: 6461 7461 7372 632e 6466 290d 0a20 2020  datasrc.df)..   
+00017f20: 2020 2020 206c 6920 3d20 6c65 6e28 692e       li = len(i.
+00017f30: 6461 7461 7372 632e 6466 290d 0a20 2020  datasrc.df)..   
+00017f40: 2020 2020 2069 6620 6c63 2061 6e64 206c       if lc and l
+00017f50: 6920 616e 6420 6d61 7828 6c63 2c6c 6929  i and max(lc,li)
+00017f60: 2f6d 696e 286c 632c 6c69 2920 3e20 3130  /min(lc,li) > 10
+00017f70: 303a 2023 2054 4f44 4f3a 2073 686f 756c  0: # TODO: shoul
+00017f80: 6420 6265 2074 7970 6564 2069 6e73 7465  d be typed inste
+00017f90: 6164 0d0a 2020 2020 2020 2020 2020 2020  ad..            
+00017fa0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00017fb0: 2020 6363 203d 2069 7465 6d2e 6461 7461    cc = item.data
+00017fc0: 7372 632e 6466 2e63 6f6c 756d 6e73 0d0a  src.df.columns..
+00017fd0: 2020 2020 2020 2020 6369 203d 2069 2e64          ci = i.d
+00017fe0: 6174 6173 7263 2e64 662e 636f 6c75 6d6e  atasrc.df.column
+00017ff0: 730d 0a20 2020 2020 2020 2063 3020 3d20  s..        c0 = 
+00018000: 5b63 2066 6f72 2063 2069 6e20 6369 2069  [c for c in ci i
+00018010: 6620 6320 696e 2063 635d 0d0a 2020 2020  f c in cc]..    
+00018020: 2020 2020 6331 203d 205b 6320 666f 7220      c1 = [c for 
+00018030: 6320 696e 2063 6920 6966 206e 6f74 2063  c in ci if not c
+00018040: 2069 6e20 6363 5d0d 0a20 2020 2020 2020   in cc]..       
+00018050: 2064 665f 636c 6970 7065 6420 3d20 6974   df_clipped = it
+00018060: 656d 2e64 6174 6173 7263 2e64 665b 6330  em.datasrc.df[c0
+00018070: 5d0d 0a20 2020 2020 2020 2069 6620 6331  ]..        if c1
+00018080: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+00018090: 665f 636c 6970 7065 6420 3d20 6466 5f63  f_clipped = df_c
+000180a0: 6c69 7070 6564 2e63 6f70 7928 290d 0a20  lipped.copy().. 
+000180b0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+000180c0: 2069 6e20 6331 3a0d 0a20 2020 2020 2020   in c1:..       
+000180d0: 2020 2020 2020 2020 2064 665f 636c 6970           df_clip
+000180e0: 7065 645b 635d 203d 2069 2e64 6174 6173  ped[c] = i.datas
+000180f0: 7263 2e64 665b 635d 0d0a 2020 2020 2020  rc.df[c]..      
+00018100: 2020 692e 6461 7461 7372 632e 7365 745f    i.datasrc.set_
+00018110: 6466 2864 665f 636c 6970 7065 6429 0d0a  df(df_clipped)..
+00018120: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
+00018130: 2020 2075 7064 6174 655f 7369 6764 6967     update_sigdig
+00018140: 203d 2046 616c 7365 0d0a 2020 2020 6966   = False..    if
+00018150: 206e 6f74 2069 7465 6d2e 6461 7461 7372   not item.datasr
+00018160: 632e 7374 616e 6461 6c6f 6e65 2061 6e64  c.standalone and
+00018170: 206e 6f74 2069 7465 6d2e 6178 2e76 622e   not item.ax.vb.
+00018180: 7769 6e2e 5f69 734d 6f75 7365 4c65 6674  win._isMouseLeft
+00018190: 4472 6167 3a0d 0a20 2020 2020 2020 2023  Drag:..        #
+000181a0: 206e 6577 206c 696d 6974 7320 7768 656e   new limits when
+000181b0: 2065 7874 656e 6469 6e67 2f72 6564 7563   extending/reduc
+000181c0: 696e 6720 616d 6f75 6e74 206f 6620 6461  ing amount of da
+000181d0: 7461 0d0a 2020 2020 2020 2020 785f 6d69  ta..        x_mi
+000181e0: 6e2c 7831 203d 205f 7365 745f 785f 6c69  n,x1 = _set_x_li
+000181f0: 6d69 7473 2869 7465 6d2e 6178 2c20 6974  mits(item.ax, it
+00018200: 656d 2e64 6174 6173 7263 290d 0a20 2020  em.datasrc)..   
+00018210: 2020 2020 2023 2073 6372 6f6c 6c20 616c       # scroll al
+00018220: 6c20 706c 6f74 7320 6966 2077 6527 7265  l plots if we're
+00018230: 2061 7420 7468 6520 6661 7220 7269 6768   at the far righ
+00018240: 740d 0a20 2020 2020 2020 2074 7220 3d20  t..        tr = 
+00018250: 6974 656d 2e61 782e 7662 2e74 6172 6765  item.ax.vb.targe
+00018260: 7452 6563 7428 290d 0a20 2020 2020 2020  tRect()..       
+00018270: 2078 3020 3d20 7831 202d 2074 722e 7769   x0 = x1 - tr.wi
+00018280: 6474 6828 290d 0a20 2020 2020 2020 2069  dth()..        i
+00018290: 6620 7830 203c 2072 6967 6874 5f6d 6172  f x0 < right_mar
+000182a0: 6769 6e5f 6361 6e64 6c65 7320 2b20 7369  gin_candles + si
+000182b0: 6465 5f6d 6172 6769 6e3a 0d0a 2020 2020  de_margin:..    
+000182c0: 2020 2020 2020 2020 7830 203d 202d 7369          x0 = -si
+000182d0: 6465 5f6d 6172 6769 6e0d 0a20 2020 2020  de_margin..     
+000182e0: 2020 2069 6620 7472 2e72 6967 6874 2829     if tr.right()
+000182f0: 203c 2078 3120 2d20 3520 2d20 322a 7269   < x1 - 5 - 2*ri
+00018300: 6768 745f 6d61 7267 696e 5f63 616e 646c  ght_margin_candl
+00018310: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
+00018320: 2078 3020 3d20 7831 203d 204e 6f6e 650d   x0 = x1 = None.
+00018330: 0a20 2020 2020 2020 2070 7265 765f 746f  .        prev_to
+00018340: 7020 3d20 6974 656d 2e61 782e 7662 2e74  p = item.ax.vb.t
+00018350: 6172 6765 7452 6563 7428 292e 746f 7028  argetRect().top(
+00018360: 290d 0a20 2020 2020 2020 2069 7465 6d2e  )..        item.
+00018370: 6178 2e76 622e 7570 6461 7465 5f79 5f7a  ax.vb.update_y_z
+00018380: 6f6f 6d28 7830 2c20 7831 290d 0a20 2020  oom(x0, x1)..   
+00018390: 2020 2020 2074 6869 735f 746f 7020 3d20       this_top = 
+000183a0: 6974 656d 2e61 782e 7662 2e74 6172 6765  item.ax.vb.targe
+000183b0: 7452 6563 7428 292e 746f 7028 290d 0a20  tRect().top().. 
+000183c0: 2020 2020 2020 2069 6620 7468 6973 5f74         if this_t
+000183d0: 6f70 2061 6e64 206e 6f74 2028 302e 3939  op and not (0.99
+000183e0: 203c 2061 6273 2870 7265 765f 746f 702f   < abs(prev_top/
+000183f0: 7468 6973 5f74 6f70 2920 3c20 312e 3031  this_top) < 1.01
+00018400: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00018410: 7570 6461 7465 5f73 6967 6469 6720 3d20  update_sigdig = 
+00018420: 5472 7565 0d0a 2020 2020 2020 2020 6966  True..        if
+00018430: 2069 7465 6d2e 6178 2e61 7865 735b 2762   item.ax.axes['b
+00018440: 6f74 746f 6d27 5d5b 2769 7465 6d27 5d2e  ottom']['item'].
+00018450: 6973 5669 7369 626c 6528 293a 2023 2075  isVisible(): # u
+00018460: 7064 6174 6520 6178 6573 2069 6620 7669  pdate axes if vi
+00018470: 7369 626c 650d 0a20 2020 2020 2020 2020  sible..         
+00018480: 2020 2069 7465 6d2e 6178 2e61 7865 735b     item.ax.axes[
+00018490: 2762 6f74 746f 6d27 5d5b 2769 7465 6d27  'bottom']['item'
+000184a0: 5d2e 6869 6465 2829 0d0a 2020 2020 2020  ].hide()..      
+000184b0: 2020 2020 2020 6974 656d 2e61 782e 6178        item.ax.ax
+000184c0: 6573 5b27 626f 7474 6f6d 275d 5b27 6974  es['bottom']['it
+000184d0: 656d 275d 2e73 686f 7728 290d 0a20 2020  em'].show()..   
+000184e0: 205f 656e 645f 7669 7375 616c 5f75 7064   _end_visual_upd
+000184f0: 6174 6528 6974 656d 290d 0a20 2020 2069  ate(item)..    i
+00018500: 6620 7570 6461 7465 5f73 6967 6469 673a  f update_sigdig:
+00018510: 0d0a 2020 2020 2020 2020 5f75 7064 6174  ..        _updat
+00018520: 655f 7369 676e 6966 6963 616e 7473 2869  e_significants(i
+00018530: 7465 6d2e 6178 2c20 6974 656d 2e61 782e  tem.ax, item.ax.
+00018540: 7662 2e64 6174 6173 7263 2c20 666f 7263  vb.datasrc, forc
+00018550: 653d 5472 7565 290d 0a0d 0a0d 0a64 6566  e=True)......def
+00018560: 205f 7374 6172 745f 7669 7375 616c 5f75   _start_visual_u
+00018570: 7064 6174 6528 6974 656d 293a 0d0a 2020  pdate(item):..  
+00018580: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00018590: 6974 656d 2c20 4669 6e50 6c6f 7449 7465  item, FinPlotIte
+000185a0: 6d29 3a0d 0a20 2020 2020 2020 2069 7465  m):..        ite
+000185b0: 6d2e 6178 2e72 656d 6f76 6549 7465 6d28  m.ax.removeItem(
+000185c0: 6974 656d 290d 0a20 2020 2020 2020 2069  item)..        i
+000185d0: 7465 6d2e 6469 7274 7920 3d20 5472 7565  tem.dirty = True
+000185e0: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+000185f0: 2020 2020 2079 203d 2069 7465 6d2e 6461       y = item.da
+00018600: 7461 7372 632e 7920 2f20 6974 656d 2e61  tasrc.y / item.a
+00018610: 782e 7662 2e79 7363 616c 652e 7363 616c  x.vb.yscale.scal
+00018620: 6566 0d0a 2020 2020 2020 2020 6966 2069  ef..        if i
+00018630: 7465 6d2e 6178 2e76 622e 7973 6361 6c65  tem.ax.vb.yscale
+00018640: 2e73 6361 6c65 7479 7065 203d 3d20 276c  .scaletype == 'l
+00018650: 6f67 273a 0d0a 2020 2020 2020 2020 2020  og':..          
+00018660: 2020 7920 3d20 7920 2b20 6c6f 675f 706c    y = y + log_pl
+00018670: 6f74 5f6f 6666 7365 740d 0a20 2020 2020  ot_offset..     
+00018680: 2020 2069 7465 6d2e 7365 7444 6174 6128     item.setData(
+00018690: 6974 656d 2e64 6174 6173 7263 2e69 6e64  item.datasrc.ind
+000186a0: 6578 2c20 7929 0d0a 0d0a 0d0a 6465 6620  ex, y)......def 
+000186b0: 5f65 6e64 5f76 6973 7561 6c5f 7570 6461  _end_visual_upda
+000186c0: 7465 2869 7465 6d29 3a0d 0a20 2020 2069  te(item):..    i
+000186d0: 6620 6973 696e 7374 616e 6365 2869 7465  f isinstance(ite
+000186e0: 6d2c 2046 696e 506c 6f74 4974 656d 293a  m, FinPlotItem):
+000186f0: 0d0a 2020 2020 2020 2020 6974 656d 2e61  ..        item.a
+00018700: 782e 6164 6449 7465 6d28 6974 656d 290d  x.addItem(item).
+00018710: 0a20 2020 2020 2020 2069 7465 6d2e 7265  .        item.re
+00018720: 7061 696e 7428 290d 0a0d 0a0d 0a64 6566  paint()......def
+00018730: 205f 7365 745f 785f 6c69 6d69 7473 2861   _set_x_limits(a
+00018740: 782c 2064 6174 6173 7263 293a 0d0a 2020  x, datasrc):..  
+00018750: 2020 7830 2c78 3120 3d20 5f78 6d69 6e6d    x0,x1 = _xminm
+00018760: 6178 2864 6174 6173 7263 2c20 785f 696e  ax(datasrc, x_in
+00018770: 6465 7865 643d 6178 2e76 622e 785f 696e  dexed=ax.vb.x_in
+00018780: 6465 7865 6429 0d0a 2020 2020 6178 2e73  dexed)..    ax.s
+00018790: 6574 4c69 6d69 7473 2878 4d69 6e3d 7830  etLimits(xMin=x0
+000187a0: 2c20 784d 6178 3d78 3129 0d0a 2020 2020  , xMax=x1)..    
+000187b0: 7265 7475 726e 2078 302c 7831 0d0a 0d0a  return x0,x1....
+000187c0: 0d0a 6465 6620 5f78 6d69 6e6d 6178 2864  ..def _xminmax(d
+000187d0: 6174 6173 7263 2c20 785f 696e 6465 7865  atasrc, x_indexe
+000187e0: 642c 2069 6e69 745f 7374 6570 733d 4e6f  d, init_steps=No
+000187f0: 6e65 2c20 6578 7472 615f 6d61 7267 696e  ne, extra_margin
+00018800: 3d30 293a 0d0a 2020 2020 6966 2078 5f69  =0):..    if x_i
+00018810: 6e64 6578 6564 2061 6e64 2069 6e69 745f  ndexed and init_
+00018820: 7374 6570 733a 0d0a 2020 2020 2020 2020  steps:..        
+00018830: 2320 696e 6974 6961 6c20 7a6f 6f6d 0d0a  # initial zoom..
+00018840: 2020 2020 2020 2020 7830 203d 206d 6178          x0 = max
+00018850: 2864 6174 6173 7263 2e78 6c65 6e2d 696e  (datasrc.xlen-in
+00018860: 6974 5f73 7465 7073 2c20 3029 202d 2073  it_steps, 0) - s
+00018870: 6964 655f 6d61 7267 696e 202d 2065 7874  ide_margin - ext
+00018880: 7261 5f6d 6172 6769 6e0d 0a20 2020 2020  ra_margin..     
+00018890: 2020 2078 3120 3d20 6461 7461 7372 632e     x1 = datasrc.
+000188a0: 786c 656e 202b 2072 6967 6874 5f6d 6172  xlen + right_mar
+000188b0: 6769 6e5f 6361 6e64 6c65 7320 2b20 7369  gin_candles + si
+000188c0: 6465 5f6d 6172 6769 6e20 2b20 6578 7472  de_margin + extr
+000188d0: 615f 6d61 7267 696e 0d0a 2020 2020 656c  a_margin..    el
+000188e0: 6966 2078 5f69 6e64 6578 6564 3a0d 0a20  if x_indexed:.. 
+000188f0: 2020 2020 2020 2023 2074 6f74 616c 2078         # total x
+00018900: 2073 697a 6520 666f 7220 696e 6465 7865   size for indexe
+00018910: 6420 6461 7461 0d0a 2020 2020 2020 2020  d data..        
+00018920: 7830 203d 202d 7369 6465 5f6d 6172 6769  x0 = -side_margi
+00018930: 6e20 2d20 6578 7472 615f 6d61 7267 696e  n - extra_margin
+00018940: 0d0a 2020 2020 2020 2020 7831 203d 2064  ..        x1 = d
+00018950: 6174 6173 7263 2e78 6c65 6e20 2b20 7269  atasrc.xlen + ri
+00018960: 6768 745f 6d61 7267 696e 5f63 616e 646c  ght_margin_candl
+00018970: 6573 202d 2031 202b 2073 6964 655f 6d61  es - 1 + side_ma
+00018980: 7267 696e 202b 2065 7874 7261 5f6d 6172  rgin + extra_mar
+00018990: 6769 6e20 2320 6164 6420 616e 6f74 6865  gin # add anothe
+000189a0: 7220 6d61 7267 696e 2074 6f20 6765 7420  r margin to get 
+000189b0: 7468 6520 2273 6e61 7020 6261 636b 2220  the "snap back" 
+000189c0: 7365 6e73 6174 696f 6e0d 0a20 2020 2065  sensation..    e
+000189d0: 6c73 653a 0d0a 2020 2020 2020 2020 2320  lse:..        # 
+000189e0: 7820 7369 7a65 2066 6f72 2070 6c61 696e  x size for plain
+000189f0: 2059 2d6f 7665 722d 5820 6461 7461 2028   Y-over-X data (
+00018a00: 692e 652e 206e 6f74 2069 6e64 6578 6564  i.e. not indexed
+00018a10: 290d 0a20 2020 2020 2020 2078 3020 3d20  )..        x0 = 
+00018a20: 6461 7461 7372 632e 782e 6d69 6e28 290d  datasrc.x.min().
+00018a30: 0a20 2020 2020 2020 2078 3120 3d20 6461  .        x1 = da
+00018a40: 7461 7372 632e 782e 6d61 7828 290d 0a20  tasrc.x.max().. 
+00018a50: 2020 2020 2020 2023 2065 7874 656e 6420         # extend 
+00018a60: 6d61 7267 696e 206f 6e20 6465 636f 7570  margin on decoup
+00018a70: 6c65 6420 706c 6f74 730d 0a20 2020 2020  led plots..     
+00018a80: 2020 2064 203d 2028 7831 2d78 3029 202a     d = (x1-x0) *
+00018a90: 2028 302e 322b 6578 7472 615f 6d61 7267   (0.2+extra_marg
+00018aa0: 696e 290d 0a20 2020 2020 2020 2078 3020  in)..        x0 
+00018ab0: 2d3d 2064 0d0a 2020 2020 2020 2020 7831  -= d..        x1
+00018ac0: 202b 3d20 640d 0a20 2020 2072 6574 7572   += d..    retur
+00018ad0: 6e20 7830 2c78 310d 0a0d 0a0d 0a64 6566  n x0,x1......def
+00018ae0: 205f 7265 7061 696e 745f 6361 6e64 6c65   _repaint_candle
+00018af0: 7328 293a 0d0a 2020 2020 2727 2743 616e  s():..    '''Can
+00018b00: 646c 6573 2061 7265 206f 6e6c 7920 7061  dles are only pa
+00018b10: 7274 6961 6c6c 7920 6472 6177 6e2c 2061  rtially drawn, a
+00018b20: 6e64 2074 6865 7265 666f 7265 206e 6565  nd therefore nee
+00018b30: 6473 206d 616e 7561 6c20 6469 7274 7920  ds manual dirty 
+00018b40: 7265 6d69 6e64 6572 2077 6865 6e65 7665  reminder wheneve
+00018b50: 7220 6974 2067 6f65 7320 6f66 662d 7363  r it goes off-sc
+00018b60: 7265 656e 2e27 2727 0d0a 2020 2020 6178  reen.'''..    ax
+00018b70: 7320 3d20 5b61 7820 666f 7220 7769 6e20  s = [ax for win 
+00018b80: 696e 2077 696e 646f 7773 2066 6f72 2061  in windows for a
+00018b90: 7820 696e 2077 696e 2e61 7873 5d20 2b20  x in win.axs] + 
+00018ba0: 6f76 6572 6c61 795f 6178 730d 0a20 2020  overlay_axs..   
+00018bb0: 2066 6f72 2061 7820 696e 2061 7873 3a0d   for ax in axs:.
+00018bc0: 0a20 2020 2020 2020 2066 6f72 2069 7465  .        for ite
+00018bd0: 6d20 696e 206c 6973 7428 6178 2e69 7465  m in list(ax.ite
+00018be0: 6d73 293a 0d0a 2020 2020 2020 2020 2020  ms):..          
+00018bf0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00018c00: 6974 656d 2c20 4669 6e50 6c6f 7449 7465  item, FinPlotIte
+00018c10: 6d29 3a0d 0a20 2020 2020 2020 2020 2020  m):..           
+00018c20: 2020 2020 205f 7374 6172 745f 7669 7375       _start_visu
+00018c30: 616c 5f75 7064 6174 6528 6974 656d 290d  al_update(item).
+00018c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018c50: 205f 656e 645f 7669 7375 616c 5f75 7064   _end_visual_upd
+00018c60: 6174 6528 6974 656d 290d 0a0d 0a0d 0a64  ate(item)......d
+00018c70: 6566 205f 7061 696e 745f 7363 6174 7465  ef _paint_scatte
+00018c80: 7228 6974 656d 2c20 702c 202a 6172 6773  r(item, p, *args
+00018c90: 293a 0d0a 2020 2020 7769 7468 206e 702e  ):..    with np.
+00018ca0: 6572 7273 7461 7465 2869 6e76 616c 6964  errstate(invalid
+00018cb0: 3d27 6967 6e6f 7265 2729 3a20 2320 6d61  ='ignore'): # ma
+00018cc0: 6b65 2070 6727 7320 6d61 736b 2063 7265  ke pg's mask cre
+00018cd0: 6174 696f 6e20 6361 6c6c 7320 746f 206e  ation calls to n
+00018ce0: 756d 7079 2073 6875 7420 7570 0d0a 2020  umpy shut up..  
+00018cf0: 2020 2020 2020 6974 656d 2e5f 646f 7061        item._dopa
+00018d00: 696e 7428 702c 202a 6172 6773 290d 0a0d  int(p, *args)...
+00018d10: 0a0d 0a64 6566 205f 6b65 795f 7072 6573  ...def _key_pres
+00018d20: 7365 6428 7662 2c20 6576 293a 0d0a 2020  sed(vb, ev):..  
+00018d30: 2020 6966 2065 762e 7465 7874 2829 203d    if ev.text() =
+00018d40: 3d20 2767 273a 2023 2067 7269 640d 0a20  = 'g': # grid.. 
+00018d50: 2020 2020 2020 2067 6c6f 6261 6c20 636c         global cl
+00018d60: 616d 705f 6772 6964 0d0a 2020 2020 2020  amp_grid..      
+00018d70: 2020 636c 616d 705f 6772 6964 203d 206e    clamp_grid = n
+00018d80: 6f74 2063 6c61 6d70 5f67 7269 640d 0a20  ot clamp_grid.. 
+00018d90: 2020 2020 2020 2066 6f72 2077 696e 2069         for win i
+00018da0: 6e20 7769 6e64 6f77 733a 0d0a 2020 2020  n windows:..    
+00018db0: 2020 2020 2020 2020 666f 7220 6178 2069          for ax i
+00018dc0: 6e20 7769 6e2e 6178 733a 0d0a 2020 2020  n win.axs:..    
+00018dd0: 2020 2020 2020 2020 2020 2020 6178 2e63              ax.c
+00018de0: 726f 7373 6861 6972 2e75 7064 6174 6528  rosshair.update(
+00018df0: 290d 0a20 2020 2065 6c69 6620 6576 2e74  )..    elif ev.t
+00018e00: 6578 7428 2920 3d3d 2027 6927 3a20 2320  ext() == 'i': # 
+00018e10: 696e 7665 7274 0d0a 2020 2020 2020 2020  invert..        
+00018e20: 666f 7220 7769 6e20 696e 2077 696e 646f  for win in windo
+00018e30: 7773 3a0d 0a20 2020 2020 2020 2020 2020  ws:..           
+00018e40: 2066 6f72 2061 7820 696e 2077 696e 2e61   for ax in win.a
+00018e50: 7873 3a0d 0a20 2020 2020 2020 2020 2020  xs:..           
+00018e60: 2020 2020 2061 782e 7365 7454 7261 6e73       ax.setTrans
+00018e70: 666f 726d 2861 782e 7472 616e 7366 6f72  form(ax.transfor
+00018e80: 6d28 292e 7363 616c 6528 312c 2d31 292e  m().scale(1,-1).
+00018e90: 7472 616e 736c 6174 6528 302c 2d61 782e  translate(0,-ax.
+00018ea0: 6865 6967 6874 2829 2929 0d0a 2020 2020  height()))..    
+00018eb0: 656c 6966 2065 762e 7465 7874 2829 2069  elif ev.text() i
+00018ec0: 6e20 2827 5c72 272c 2027 2027 293a 2023  n ('\r', ' '): #
+00018ed0: 2065 6e74 6572 2c20 7370 6163 650d 0a20   enter, space.. 
+00018ee0: 2020 2020 2020 2076 622e 7365 745f 6472         vb.set_dr
+00018ef0: 6177 5f6c 696e 655f 636f 6c6f 7228 6472  aw_line_color(dr
+00018f00: 6177 5f64 6f6e 655f 636f 6c6f 7229 0d0a  aw_done_color)..
+00018f10: 2020 2020 2020 2020 7662 2e64 7261 775f          vb.draw_
+00018f20: 6c69 6e65 203d 204e 6f6e 650d 0a20 2020  line = None..   
+00018f30: 2065 6c69 6620 6576 2e74 6578 7428 2920   elif ev.text() 
+00018f40: 696e 2028 275c 7837 6627 2c20 275c 6227  in ('\x7f', '\b'
+00018f50: 293a 2023 2064 656c 2c20 6261 636b 7370  ): # del, backsp
+00018f60: 6163 650d 0a20 2020 2020 2020 2069 6620  ace..        if 
+00018f70: 6e6f 7420 7662 2e72 656d 6f76 655f 6c61  not vb.remove_la
+00018f80: 7374 5f72 6f69 2829 3a0d 0a20 2020 2020  st_roi():..     
+00018f90: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00018fa0: 6c73 650d 0a20 2020 2065 6c69 6620 6576  lse..    elif ev
+00018fb0: 2e6b 6579 2829 203d 3d20 5174 436f 7265  .key() == QtCore
+00018fc0: 2e51 742e 4b65 792e 4b65 795f 4c65 6674  .Qt.Key.Key_Left
+00018fd0: 3a0d 0a20 2020 2020 2020 2076 622e 7061  :..        vb.pa
+00018fe0: 6e5f 7828 7065 7263 656e 743d 2d31 3529  n_x(percent=-15)
+00018ff0: 0d0a 2020 2020 656c 6966 2065 762e 6b65  ..    elif ev.ke
+00019000: 7928 2920 3d3d 2051 7443 6f72 652e 5174  y() == QtCore.Qt
+00019010: 2e4b 6579 2e4b 6579 5f52 6967 6874 3a0d  .Key.Key_Right:.
+00019020: 0a20 2020 2020 2020 2076 622e 7061 6e5f  .        vb.pan_
+00019030: 7828 7065 7263 656e 743d 2b31 3529 0d0a  x(percent=+15)..
+00019040: 2020 2020 656c 6966 2065 762e 6b65 7928      elif ev.key(
+00019050: 2920 3d3d 2051 7443 6f72 652e 5174 2e4b  ) == QtCore.Qt.K
+00019060: 6579 2e4b 6579 5f48 6f6d 653a 0d0a 2020  ey.Key_Home:..  
+00019070: 2020 2020 2020 7662 2e70 616e 5f78 2873        vb.pan_x(s
+00019080: 7465 7073 3d2d 3165 3130 290d 0a20 2020  teps=-1e10)..   
+00019090: 2020 2020 205f 7265 7061 696e 745f 6361       _repaint_ca
+000190a0: 6e64 6c65 7328 290d 0a20 2020 2065 6c69  ndles()..    eli
+000190b0: 6620 6576 2e6b 6579 2829 203d 3d20 5174  f ev.key() == Qt
+000190c0: 436f 7265 2e51 742e 4b65 792e 4b65 795f  Core.Qt.Key.Key_
+000190d0: 456e 643a 0d0a 2020 2020 2020 2020 7662  End:..        vb
+000190e0: 2e70 616e 5f78 2873 7465 7073 3d2b 3165  .pan_x(steps=+1e
+000190f0: 3130 290d 0a20 2020 2020 2020 205f 7265  10)..        _re
+00019100: 7061 696e 745f 6361 6e64 6c65 7328 290d  paint_candles().
+00019110: 0a20 2020 2065 6c69 6620 6576 2e6b 6579  .    elif ev.key
+00019120: 2829 203d 3d20 5174 436f 7265 2e51 742e  () == QtCore.Qt.
+00019130: 4b65 792e 4b65 795f 4573 6361 7065 2061  Key.Key_Escape a
+00019140: 6e64 206b 6579 5f65 7363 5f63 6c6f 7365  nd key_esc_close
+00019150: 3a0d 0a20 2020 2020 2020 2076 622e 7769  :..        vb.wi
+00019160: 6e2e 636c 6f73 6528 290d 0a20 2020 2065  n.close()..    e
+00019170: 6c73 653a 0d0a 2020 2020 2020 2020 7265  lse:..        re
+00019180: 7475 726e 2046 616c 7365 0d0a 2020 2020  turn False..    
+00019190: 7265 7475 726e 2054 7275 650d 0a0d 0a0d  return True.....
+000191a0: 0a64 6566 205f 6d6f 7573 655f 636c 6963  .def _mouse_clic
+000191b0: 6b65 6428 7662 2c20 6576 293a 0d0a 2020  ked(vb, ev):..  
+000191c0: 2020 6966 2065 762e 6275 7474 6f6e 2829    if ev.button()
+000191d0: 203d 3d20 383a 2023 2062 6163 6b0d 0a20   == 8: # back.. 
+000191e0: 2020 2020 2020 2076 622e 7061 6e5f 7828         vb.pan_x(
+000191f0: 7065 7263 656e 743d 2d33 3029 0d0a 2020  percent=-30)..  
+00019200: 2020 656c 6966 2065 762e 6275 7474 6f6e    elif ev.button
+00019210: 2829 203d 3d20 3136 3a20 2320 6677 640d  () == 16: # fwd.
+00019220: 0a20 2020 2020 2020 2076 622e 7061 6e5f  .        vb.pan_
+00019230: 7828 7065 7263 656e 743d 2b33 3029 0d0a  x(percent=+30)..
+00019240: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00019250: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
+00019260: 0a20 2020 2072 6574 7572 6e20 5472 7565  .    return True
+00019270: 0d0a 0d0a 0d0a 6465 6620 5f6d 6f75 7365  ......def _mouse
+00019280: 5f6d 6f76 6564 286d 6173 7465 722c 2076  _moved(master, v
+00019290: 622c 2065 7673 293a 0d0a 2020 2020 6966  b, evs):..    if
+000192a0: 2068 6173 6174 7472 286d 6173 7465 722c   hasattr(master,
+000192b0: 2027 636c 6f73 696e 6727 2920 616e 6420   'closing') and 
+000192c0: 6d61 7374 6572 2e63 6c6f 7369 6e67 3a0d  master.closing:.
+000192d0: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
+000192e0: 0a20 2020 206d 6420 3d20 6d61 7374 6572  .    md = master
+000192f0: 5f64 6174 615b 6d61 7374 6572 5d2e 6765  _data[master].ge
+00019300: 7428 7662 2920 6f72 206d 6173 7465 725f  t(vb) or master_
+00019310: 6461 7461 5b6d 6173 7465 725d 5b27 6465  data[master]['de
+00019320: 6661 756c 7427 5d0d 0a20 2020 2069 6620  fault']..    if 
+00019330: 6e6f 7420 6576 733a 0d0a 2020 2020 2020  not evs:..      
+00019340: 2020 6576 7320 3d20 6d64 5b27 6c61 7374    evs = md['last
+00019350: 5f6d 6f75 7365 5f65 7673 275d 0d0a 2020  _mouse_evs']..  
+00019360: 2020 2020 2020 6966 206e 6f74 2065 7673        if not evs
+00019370: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00019380: 6574 7572 6e0d 0a20 2020 206d 645b 276c  eturn..    md['l
+00019390: 6173 745f 6d6f 7573 655f 6576 7327 5d20  ast_mouse_evs'] 
+000193a0: 3d20 6576 730d 0a20 2020 2070 6f73 203d  = evs..    pos =
+000193b0: 2065 7673 5b2d 315d 0d0a 2020 2020 2320   evs[-1]..    # 
+000193c0: 616c 6c6f 7720 696e 7465 722d 7069 7865  allow inter-pixe
+000193d0: 6c20 6d6f 7665 7320 6966 206d 6f76 696e  l moves if movin
+000193e0: 6720 6d6f 7573 6520 736c 6f77 6c79 0d0a  g mouse slowly..
+000193f0: 2020 2020 7920 3d20 706f 732e 7928 290d      y = pos.y().
+00019400: 0a20 2020 2064 7920 3d20 7920 2d20 6d64  .    dy = y - md
+00019410: 5b27 6c61 7374 5f6d 6f75 7365 5f79 275d  ['last_mouse_y']
+00019420: 0d0a 2020 2020 6966 2030 203c 2061 6273  ..    if 0 < abs
+00019430: 2864 7929 203c 3d20 313a 0d0a 2020 2020  (dy) <= 1:..    
+00019440: 2020 2020 706f 732e 7365 7459 2870 6f73      pos.setY(pos
+00019450: 2e79 2829 202d 2064 792f 3229 0d0a 2020  .y() - dy/2)..  
+00019460: 2020 6d64 5b27 6c61 7374 5f6d 6f75 7365    md['last_mouse
+00019470: 5f79 275d 203d 2079 0d0a 2020 2020 2320  _y'] = y..    # 
+00019480: 6170 706c 7920 746f 2061 6c6c 2063 726f  apply to all cro
+00019490: 7373 6861 6972 730d 0a20 2020 2066 6f72  sshairs..    for
+000194a0: 2061 7820 696e 206d 6173 7465 722e 6178   ax in master.ax
+000194b0: 733a 0d0a 2020 2020 2020 2020 6966 2061  s:..        if a
+000194c0: 782e 6973 5669 7369 626c 6528 2920 616e  x.isVisible() an
+000194d0: 6420 6178 2e63 726f 7373 6861 6972 3a0d  d ax.crosshair:.
+000194e0: 0a20 2020 2020 2020 2020 2020 2070 6f69  .            poi
+000194f0: 6e74 203d 2061 782e 7662 2e6d 6170 5363  nt = ax.vb.mapSc
+00019500: 656e 6554 6f56 6965 7728 706f 7329 0d0a  eneToView(pos)..
+00019510: 2020 2020 2020 2020 2020 2020 6178 2e63              ax.c
+00019520: 726f 7373 6861 6972 2e75 7064 6174 6528  rosshair.update(
+00019530: 706f 696e 7429 0d0a 0d0a 0d0a 6465 6620  point)......def 
+00019540: 5f77 6865 656c 5f65 7665 6e74 5f77 7261  _wheel_event_wra
+00019550: 7070 6572 2873 656c 662c 206f 7269 675f  pper(self, orig_
+00019560: 6675 6e63 2c20 6576 293a 0d0a 2020 2020  func, ev):..    
+00019570: 2320 7363 726f 6c6c 696e 6720 6f6e 2074  # scrolling on t
+00019580: 6865 2062 6f72 6465 7220 6973 2073 696d  he border is sim
+00019590: 706c 7920 616e 6e6f 7969 6e67 2c20 706f  ply annoying, po
+000195a0: 7020 696e 2061 2063 6f75 706c 6520 6f66  p in a couple of
+000195b0: 2070 6978 656c 7320 746f 206d 616b 6520   pixels to make 
+000195c0: 7375 7265 0d0a 2020 2020 6420 3d20 5174  sure..    d = Qt
+000195d0: 436f 7265 2e51 506f 696e 7446 282d 322c  Core.QPointF(-2,
+000195e0: 3029 0d0a 2020 2020 6576 203d 2051 7447  0)..    ev = QtG
+000195f0: 7569 2e51 5768 6565 6c45 7665 6e74 2865  ui.QWheelEvent(e
+00019600: 762e 706f 7369 7469 6f6e 2829 2b64 2c20  v.position()+d, 
+00019610: 6576 2e67 6c6f 6261 6c50 6f73 6974 696f  ev.globalPositio
+00019620: 6e28 292b 642c 2065 762e 7069 7865 6c44  n()+d, ev.pixelD
+00019630: 656c 7461 2829 2c20 6576 2e61 6e67 6c65  elta(), ev.angle
+00019640: 4465 6c74 6128 292c 2065 762e 6275 7474  Delta(), ev.butt
+00019650: 6f6e 7328 292c 2065 762e 6d6f 6469 6669  ons(), ev.modifi
+00019660: 6572 7328 292c 2065 762e 7068 6173 6528  ers(), ev.phase(
+00019670: 292c 2046 616c 7365 290d 0a20 2020 206f  ), False)..    o
+00019680: 7269 675f 6675 6e63 2873 656c 662c 2065  rig_func(self, e
+00019690: 7629 0d0a 0d0a 0d0a 6465 6620 5f69 6e73  v)......def _ins
+000196a0: 7065 6374 5f63 6c69 636b 6564 2861 782c  pect_clicked(ax,
+000196b0: 2069 6e73 7065 6374 6f72 2c20 7768 656e   inspector, when
+000196c0: 5f64 6f75 626c 655f 636c 6963 6b2c 2065  _double_click, e
+000196d0: 7673 293a 0d0a 2020 2020 6966 2065 7673  vs):..    if evs
+000196e0: 5b2d 315d 2e61 6363 6570 7465 6420 6f72  [-1].accepted or
+000196f0: 2077 6865 6e5f 646f 7562 6c65 5f63 6c69   when_double_cli
+00019700: 636b 2021 3d20 6576 735b 2d31 5d2e 646f  ck != evs[-1].do
+00019710: 7562 6c65 2829 3a0d 0a20 2020 2020 2020  uble():..       
+00019720: 2072 6574 7572 6e0d 0a20 2020 2070 6f73   return..    pos
+00019730: 203d 2065 7673 5b2d 315d 2e73 6365 6e65   = evs[-1].scene
+00019740: 506f 7328 290d 0a20 2020 2072 6574 7572  Pos()..    retur
+00019750: 6e20 5f69 6e73 7065 6374 5f70 6f73 2861  n _inspect_pos(a
+00019760: 782c 2069 6e73 7065 6374 6f72 2c20 2870  x, inspector, (p
+00019770: 6f73 2c29 290d 0a0d 0a0d 0a64 6566 205f  os,))......def _
+00019780: 696e 7370 6563 745f 706f 7328 6178 2c20  inspect_pos(ax, 
+00019790: 696e 7370 6563 746f 722c 2070 6f73 7329  inspector, poss)
+000197a0: 3a0d 0a20 2020 2069 6620 6e6f 7420 6178  :..    if not ax
+000197b0: 2e76 622e 6461 7461 7372 633a 0d0a 2020  .vb.datasrc:..  
+000197c0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+000197d0: 2020 706f 696e 7420 3d20 6178 2e76 622e    point = ax.vb.
+000197e0: 6d61 7053 6365 6e65 546f 5669 6577 2870  mapSceneToView(p
+000197f0: 6f73 735b 2d31 5d29 0d0a 2020 2020 7420  oss[-1])..    t 
+00019800: 3d20 706f 696e 742e 7828 2920 2b20 302e  = point.x() + 0.
+00019810: 350d 0a20 2020 2074 7279 3a0d 0a20 2020  5..    try:..   
+00019820: 2020 2020 2074 203d 2061 782e 7662 2e64       t = ax.vb.d
+00019830: 6174 6173 7263 2e63 6c6f 7365 7374 5f74  atasrc.closest_t
+00019840: 696d 6528 7429 0d0a 2020 2020 6578 6365  ime(t)..    exce
+00019850: 7074 204b 6579 4572 726f 723a 2023 2077  pt KeyError: # w
+00019860: 6865 6e20 636c 6963 6b69 6e67 2062 6579  hen clicking bey
+00019870: 6f6e 6420 7269 6768 745f 6d61 7267 696e  ond right_margin
+00019880: 5f63 616e 646c 6573 0d0a 2020 2020 2020  _candles..      
+00019890: 2020 6966 2063 6c61 6d70 5f67 7269 643a    if clamp_grid:
+000198a0: 0d0a 2020 2020 2020 2020 2020 2020 7420  ..            t 
+000198b0: 3d20 6178 2e76 622e 6461 7461 7372 632e  = ax.vb.datasrc.
+000198c0: 782e 696c 6f63 5b2d 3120 6966 2074 203e  x.iloc[-1 if t >
+000198d0: 2030 2065 6c73 6520 305d 0d0a 2020 2020   0 else 0]..    
+000198e0: 7472 793a 0d0a 2020 2020 2020 2020 696e  try:..        in
+000198f0: 7370 6563 746f 7228 742c 2070 6f69 6e74  spector(t, point
+00019900: 2e79 2829 290d 0a20 2020 2065 7863 6570  .y())..    excep
+00019910: 7420 4f53 4572 726f 7220 6173 2065 3a0d  t OSError as e:.
+00019920: 0a20 2020 2020 2020 2070 6173 730d 0a20  .        pass.. 
+00019930: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00019940: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+00019950: 2020 2070 7269 6e74 2827 496e 7370 6563     print('Inspec
+00019960: 7469 6f6e 2065 7272 6f72 3a27 2c20 7479  tion error:', ty
+00019970: 7065 2865 292c 2065 290d 0a0d 0a0d 0a64  pe(e), e)......d
+00019980: 6566 2062 7269 6768 7465 6e28 636f 6c6f  ef brighten(colo
+00019990: 722c 2066 293a 0d0a 2020 2020 6966 206e  r, f):..    if n
+000199a0: 6f74 2063 6f6c 6f72 3a0d 0a20 2020 2020  ot color:..     
+000199b0: 2020 2072 6574 7572 6e20 636f 6c6f 720d     return color.
+000199c0: 0a20 2020 2072 6574 7572 6e20 7067 2e6d  .    return pg.m
+000199d0: 6b43 6f6c 6f72 2863 6f6c 6f72 292e 6c69  kColor(color).li
+000199e0: 6768 7465 7228 696e 7428 662a 3130 3029  ghter(int(f*100)
+000199f0: 290d 0a0d 0a0d 0a64 6566 205f 6765 745f  )......def _get_
+00019a00: 636f 6c6f 7228 6178 2c20 7374 796c 652c  color(ax, style,
+00019a10: 2077 616e 7465 645f 636f 6c6f 7229 3a0d   wanted_color):.
+00019a20: 0a20 2020 2069 6620 7479 7065 2877 616e  .    if type(wan
+00019a30: 7465 645f 636f 6c6f 7229 2069 6e20 2873  ted_color) in (s
+00019a40: 7472 2c20 5174 4775 692e 5143 6f6c 6f72  tr, QtGui.QColor
+00019a50: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00019a60: 726e 2077 616e 7465 645f 636f 6c6f 720d  rn wanted_color.
+00019a70: 0a20 2020 2069 6e64 6578 203d 2077 616e  .    index = wan
+00019a80: 7465 645f 636f 6c6f 7220 6966 2074 7970  ted_color if typ
+00019a90: 6528 7761 6e74 6564 5f63 6f6c 6f72 2920  e(wanted_color) 
+00019aa0: 3d3d 2069 6e74 2065 6c73 6520 4e6f 6e65  == int else None
+00019ab0: 0d0a 2020 2020 6973 5f6c 696e 6520 3d20  ..    is_line = 
+00019ac0: 6c61 6d62 6461 2073 7479 6c65 3a20 7374  lambda style: st
+00019ad0: 796c 6520 6973 204e 6f6e 6520 6f72 2061  yle is None or a
+00019ae0: 6e79 2863 6820 696e 2073 7479 6c65 2066  ny(ch in style f
+00019af0: 6f72 2063 6820 696e 2027 2d5f 2e27 290d  or ch in '-_.').
+00019b00: 0a20 2020 2074 6869 735f 6c69 6e65 203d  .    this_line =
+00019b10: 2069 735f 6c69 6e65 2873 7479 6c65 290d   is_line(style).
+00019b20: 0a20 2020 2069 6620 7468 6973 5f6c 696e  .    if this_lin
+00019b30: 653a 0d0a 2020 2020 2020 2020 636f 6c6f  e:..        colo
+00019b40: 7273 203d 2073 6f66 745f 636f 6c6f 7273  rs = soft_colors
+00019b50: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+00019b60: 2020 2020 2063 6f6c 6f72 7320 3d20 6861       colors = ha
+00019b70: 7264 5f63 6f6c 6f72 730d 0a20 2020 2069  rd_colors..    i
+00019b80: 6620 696e 6465 7820 6973 204e 6f6e 653a  f index is None:
+00019b90: 0d0a 2020 2020 2020 2020 6176 6f69 6420  ..        avoid 
+00019ba0: 3d20 7365 7428 692e 6f70 7473 5b27 6861  = set(i.opts['ha
+00019bb0: 6e64 6564 5f63 6f6c 6f72 275d 2066 6f72  nded_color'] for
+00019bc0: 2069 2069 6e20 6178 2e69 7465 6d73 2069   i in ax.items i
+00019bd0: 6620 6973 696e 7374 616e 6365 2869 2c70  f isinstance(i,p
+00019be0: 672e 506c 6f74 4461 7461 4974 656d 2920  g.PlotDataItem) 
+00019bf0: 616e 6420 692e 6f70 7473 5b27 6861 6e64  and i.opts['hand
+00019c00: 6564 5f63 6f6c 6f72 275d 2069 7320 6e6f  ed_color'] is no
+00019c10: 7420 4e6f 6e65 2061 6e64 2074 6869 735f  t None and this_
+00019c20: 6c69 6e65 3d3d 6973 5f6c 696e 6528 692e  line==is_line(i.
+00019c30: 6f70 7473 5b27 7379 6d62 6f6c 275d 2929  opts['symbol']))
+00019c40: 0d0a 2020 2020 2020 2020 696e 6465 7820  ..        index 
+00019c50: 3d20 6c65 6e28 5b69 2066 6f72 2069 2069  = len([i for i i
+00019c60: 6e20 6178 2e69 7465 6d73 2069 6620 6973  n ax.items if is
+00019c70: 696e 7374 616e 6365 2869 2c70 672e 506c  instance(i,pg.Pl
+00019c80: 6f74 4461 7461 4974 656d 2920 616e 6420  otDataItem) and 
+00019c90: 692e 6f70 7473 5b27 6861 6e64 6564 5f63  i.opts['handed_c
+00019ca0: 6f6c 6f72 275d 2069 7320 4e6f 6e65 2061  olor'] is None a
+00019cb0: 6e64 2074 6869 735f 6c69 6e65 3d3d 6973  nd this_line==is
+00019cc0: 5f6c 696e 6528 692e 6f70 7473 5b27 7379  _line(i.opts['sy
+00019cd0: 6d62 6f6c 275d 295d 290d 0a20 2020 2020  mbol'])])..     
+00019ce0: 2020 2077 6869 6c65 2069 6e64 6578 2069     while index i
+00019cf0: 6e20 6176 6f69 643a 0d0a 2020 2020 2020  n avoid:..      
+00019d00: 2020 2020 2020 696e 6465 7820 2b3d 2031        index += 1
+00019d10: 0d0a 2020 2020 7265 7475 726e 2063 6f6c  ..    return col
+00019d20: 6f72 735b 696e 6465 7825 6c65 6e28 636f  ors[index%len(co
+00019d30: 6c6f 7273 295d 0d0a 0d0a 0d0a 6465 6620  lors)]......def 
+00019d40: 5f70 6474 696d 6532 6570 6f63 6828 7429  _pdtime2epoch(t)
+00019d50: 3a0d 0a20 2020 2069 6620 6973 696e 7374  :..    if isinst
+00019d60: 616e 6365 2874 2c20 7064 2e53 6572 6965  ance(t, pd.Serie
+00019d70: 7329 3a0d 0a20 2020 2020 2020 2069 6620  s):..        if 
+00019d80: 6973 696e 7374 616e 6365 2874 2e69 6c6f  isinstance(t.ilo
+00019d90: 635b 305d 2c20 7064 2e54 696d 6573 7461  c[0], pd.Timesta
+00019da0: 6d70 293a 0d0a 2020 2020 2020 2020 2020  mp):..          
+00019db0: 2020 7265 7475 726e 2074 2e76 6965 7728    return t.view(
+00019dc0: 2769 6e74 3634 2729 0d0a 2020 2020 2020  'int64')..      
+00019dd0: 2020 6820 3d20 6e70 2e6e 616e 6d61 7828    h = np.nanmax(
+00019de0: 742e 7661 6c75 6573 290d 0a20 2020 2020  t.values)..     
+00019df0: 2020 2069 6620 6820 3c20 3165 3130 3a20     if h < 1e10: 
+00019e00: 2320 6861 6e64 6c65 2073 2065 706f 6368  # handle s epoch
+00019e10: 730d 0a20 2020 2020 2020 2020 2020 2072  s..            r
+00019e20: 6574 7572 6e20 2874 2a31 6539 292e 6173  eturn (t*1e9).as
+00019e30: 7479 7065 2827 696e 7436 3427 290d 0a20  type('int64').. 
+00019e40: 2020 2020 2020 2069 6620 6820 3c20 3165         if h < 1e
+00019e50: 3133 3a20 2320 6861 6e64 6c65 206e 7320  13: # handle ns 
+00019e60: 6570 6f63 6873 0d0a 2020 2020 2020 2020  epochs..        
+00019e70: 2020 2020 7265 7475 726e 2028 742a 3165      return (t*1e
+00019e80: 3629 2e61 7374 7970 6528 2769 6e74 3634  6).astype('int64
+00019e90: 2729 0d0a 2020 2020 2020 2020 6966 2068  ')..        if h
+00019ea0: 203c 2031 6531 363a 2023 2068 616e 646c   < 1e16: # handl
+00019eb0: 6520 7573 2065 706f 6368 730d 0a20 2020  e us epochs..   
+00019ec0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00019ed0: 2874 2a31 6533 292e 6173 7479 7065 2827  (t*1e3).astype('
+00019ee0: 696e 7436 3427 290d 0a20 2020 2020 2020  int64')..       
+00019ef0: 2072 6574 7572 6e20 742e 6173 7479 7065   return t.astype
+00019f00: 2827 696e 7436 3427 290d 0a20 2020 2072  ('int64')..    r
+00019f10: 6574 7572 6e20 740d 0a0d 0a0d 0a64 6566  eturn t......def
+00019f20: 205f 7064 7469 6d65 3269 6e64 6578 2861   _pdtime2index(a
+00019f30: 782c 2074 732c 2061 6e79 5f65 6e64 3d46  x, ts, any_end=F
+00019f40: 616c 7365 2c20 7265 7175 6972 655f 7469  alse, require_ti
+00019f50: 6d65 3d46 616c 7365 293a 0d0a 2020 2020  me=False):..    
+00019f60: 6966 2069 7369 6e73 7461 6e63 6528 7473  if isinstance(ts
+00019f70: 2e69 6c6f 635b 305d 2c20 7064 2e54 696d  .iloc[0], pd.Tim
+00019f80: 6573 7461 6d70 293a 0d0a 2020 2020 2020  estamp):..      
+00019f90: 2020 7473 203d 2074 732e 7669 6577 2827    ts = ts.view('
+00019fa0: 696e 7436 3427 290d 0a20 2020 2065 6c73  int64')..    els
+00019fb0: 653a 0d0a 2020 2020 2020 2020 6820 3d20  e:..        h = 
+00019fc0: 6e70 2e6e 616e 6d61 7828 7473 2e76 616c  np.nanmax(ts.val
+00019fd0: 7565 7329 0d0a 2020 2020 2020 2020 6966  ues)..        if
+00019fe0: 2068 203c 2031 6537 3a0d 0a20 2020 2020   h < 1e7:..     
+00019ff0: 2020 2020 2020 2069 6620 7265 7175 6972         if requir
+0001a000: 655f 7469 6d65 3a0d 0a20 2020 2020 2020  e_time:..       
+0001a010: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0001a020: 4661 6c73 652c 2027 6e6f 7420 6120 7469  False, 'not a ti
+0001a030: 6d65 2073 6572 6965 7327 0d0a 2020 2020  me series'..    
+0001a040: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+0001a050: 730d 0a20 2020 2020 2020 2069 6620 6820  s..        if h 
+0001a060: 3c20 3165 3130 3a20 2320 6861 6e64 6c65  < 1e10: # handle
+0001a070: 2073 2065 706f 6368 730d 0a20 2020 2020   s epochs..     
+0001a080: 2020 2020 2020 2074 7320 3d20 7473 2e61         ts = ts.a
+0001a090: 7374 7970 6528 2766 6c6f 6174 3634 2729  stype('float64')
+0001a0a0: 202a 2031 6539 0d0a 2020 2020 2020 2020   * 1e9..        
+0001a0b0: 656c 6966 2068 203c 2031 6531 333a 2023  elif h < 1e13: #
+0001a0c0: 2068 616e 646c 6520 6d73 2065 706f 6368   handle ms epoch
+0001a0d0: 730d 0a20 2020 2020 2020 2020 2020 2074  s..            t
+0001a0e0: 7320 3d20 7473 2e61 7374 7970 6528 2766  s = ts.astype('f
+0001a0f0: 6c6f 6174 3634 2729 202a 2031 6536 0d0a  loat64') * 1e6..
+0001a100: 2020 2020 2020 2020 656c 6966 2068 203c          elif h <
+0001a110: 2031 6531 363a 2023 2068 616e 646c 6520   1e16: # handle 
+0001a120: 7573 2065 706f 6368 730d 0a20 2020 2020  us epochs..     
+0001a130: 2020 2020 2020 2074 7320 3d20 7473 2e61         ts = ts.a
+0001a140: 7374 7970 6528 2766 6c6f 6174 3634 2729  stype('float64')
+0001a150: 202a 2031 6533 0d0a 2020 2020 0d0a 2020   * 1e3..    ..  
+0001a160: 2020 6461 7461 7372 6320 3d20 5f67 6574    datasrc = _get
+0001a170: 5f64 6174 6173 7263 2861 7829 0d0a 2020  _datasrc(ax)..  
+0001a180: 2020 7873 203d 2064 6174 6173 7263 2e78    xs = datasrc.x
+0001a190: 0d0a 0d0a 2020 2020 2320 7472 7920 6578  ....    # try ex
+0001a1a0: 6163 7420 6d61 7463 6820 6265 666f 7265  act match before
+0001a1b0: 2061 7070 726f 7869 6d61 7465 206d 6174   approximate mat
+0001a1c0: 6368 0d0a 2020 2020 6578 6163 7420 3d20  ch..    exact = 
+0001a1d0: 6461 7461 7372 632e 696e 6465 785b 7873  datasrc.index[xs
+0001a1e0: 2e69 7369 6e28 7473 295d 2e74 6f5f 6c69  .isin(ts)].to_li
+0001a1f0: 7374 2829 0d0a 2020 2020 6966 206c 656e  st()..    if len
+0001a200: 2865 7861 6374 2920 3d3d 206c 656e 2874  (exact) == len(t
+0001a210: 7329 3a0d 0a20 2020 2020 2020 2072 6574  s):..        ret
+0001a220: 7572 6e20 6578 6163 740d 0a20 2020 200d  urn exact..    .
+0001a230: 0a20 2020 2072 203d 205b 5d0d 0a20 2020  .    r = []..   
+0001a240: 2066 6f72 2069 2c74 2069 6e20 656e 756d   for i,t in enum
+0001a250: 6572 6174 6528 7473 293a 0d0a 2020 2020  erate(ts):..    
+0001a260: 2020 2020 7873 7320 3d20 7873 2e6c 6f63      xss = xs.loc
+0001a270: 5b78 733e 745d 0d0a 2020 2020 2020 2020  [xs>t]..        
+0001a280: 6966 206c 656e 2878 7373 2920 3d3d 2030  if len(xss) == 0
+0001a290: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+0001a2a0: 3020 3d20 7873 2e69 6c6f 635b 2d31 5d0d  0 = xs.iloc[-1].
+0001a2b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a2c0: 616e 795f 656e 6420 6f72 2074 3020 3d3d  any_end or t0 ==
+0001a2d0: 2074 3a0d 0a20 2020 2020 2020 2020 2020   t:..           
+0001a2e0: 2020 2020 2072 2e61 7070 656e 6428 6c65       r.append(le
+0001a2f0: 6e28 7873 292d 3129 0d0a 2020 2020 2020  n(xs)-1)..      
+0001a300: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0001a310: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+0001a320: 6966 2069 203e 2030 3a0d 0a20 2020 2020  if i > 0:..     
+0001a330: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0001a340: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
+0001a350: 2061 7373 6572 7420 7420 3c3d 2074 302c   assert t <= t0,
+0001a360: 2027 6d75 7374 2070 6c6f 7420 7468 6973   'must plot this
+0001a370: 2070 7269 6d69 7469 7665 2069 6e20 7072   primitive in pr
+0001a380: 696f 7220 7469 6d65 2d72 616e 6765 270d  ior time-range'.
+0001a390: 0a20 2020 2020 2020 2069 3120 3d20 7873  .        i1 = xs
+0001a3a0: 732e 696e 6465 785b 305d 0d0a 2020 2020  s.index[0]..    
+0001a3b0: 2020 2020 6930 203d 2069 312d 310d 0a20      i0 = i1-1.. 
+0001a3c0: 2020 2020 2020 2069 6620 6930 203c 2030         if i0 < 0
+0001a3d0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0001a3e0: 302c 6931 203d 2030 2c31 0d0a 2020 2020  0,i1 = 0,1..    
+0001a3f0: 2020 2020 7430 2c74 3120 3d20 7873 2e6c      t0,t1 = xs.l
+0001a400: 6f63 5b69 305d 2c20 7873 2e6c 6f63 5b69  oc[i0], xs.loc[i
+0001a410: 315d 0d0a 2020 2020 2020 2020 6474 203d  1]..        dt =
+0001a420: 2028 742d 7430 2920 2f20 2874 312d 7430   (t-t0) / (t1-t0
+0001a430: 290d 0a20 2020 2020 2020 2072 2e61 7070  )..        r.app
+0001a440: 656e 6428 6c65 7270 2864 742c 2069 302c  end(lerp(dt, i0,
+0001a450: 2069 3129 290d 0a20 2020 2072 6574 7572   i1))..    retur
+0001a460: 6e20 720d 0a0d 0a0d 0a64 6566 205f 6765  n r......def _ge
+0001a470: 745f 6461 7461 7372 6328 6178 2c20 7265  t_datasrc(ax, re
+0001a480: 7175 6972 653d 5472 7565 293a 0d0a 2020  quire=True):..  
+0001a490: 2020 6966 2061 782e 7662 2e64 6174 6173    if ax.vb.datas
+0001a4a0: 7263 2069 7320 6e6f 7420 4e6f 6e65 206f  rc is not None o
+0001a4b0: 7220 6e6f 7420 6178 2e76 622e 785f 696e  r not ax.vb.x_in
+0001a4c0: 6465 7865 643a 0d0a 2020 2020 2020 2020  dexed:..        
+0001a4d0: 7265 7475 726e 2061 782e 7662 2e64 6174  return ax.vb.dat
+0001a4e0: 6173 7263 0d0a 2020 2020 7662 7320 3d20  asrc..    vbs = 
+0001a4f0: 5b61 782e 7662 2066 6f72 2077 696e 2069  [ax.vb for win i
+0001a500: 6e20 7769 6e64 6f77 7320 666f 7220 6178  n windows for ax
+0001a510: 2069 6e20 7769 6e2e 6178 735d 0d0a 2020   in win.axs]..  
+0001a520: 2020 666f 7220 7662 2069 6e20 7662 733a    for vb in vbs:
+0001a530: 0d0a 2020 2020 2020 2020 6966 2076 622e  ..        if vb.
+0001a540: 6461 7461 7372 633a 0d0a 2020 2020 2020  datasrc:..      
+0001a550: 2020 2020 2020 7265 7475 726e 2076 622e        return vb.
+0001a560: 6461 7461 7372 630d 0a20 2020 2069 6620  datasrc..    if 
+0001a570: 7265 7175 6972 653a 0d0a 2020 2020 2020  require:..      
+0001a580: 2020 6173 7365 7274 2061 782e 7662 2e64    assert ax.vb.d
+0001a590: 6174 6173 7263 2c20 276e 6f74 2070 6f73  atasrc, 'not pos
+0001a5a0: 7369 626c 6520 746f 2070 6c6f 7420 7468  sible to plot th
+0001a5b0: 6973 2070 7269 6d69 7469 7665 2077 6974  is primitive wit
+0001a5c0: 686f 7574 2061 2070 7269 6f72 2074 696d  hout a prior tim
+0001a5d0: 652d 7261 6e67 6520 746f 2063 6f6d 7061  e-range to compa
+0001a5e0: 7265 2074 6f27 0d0a 0d0a 0d0a 6465 6620  re to'......def 
+0001a5f0: 5f6d 696c 6c69 7365 636f 6e64 5f74 7a5f  _millisecond_tz_
+0001a600: 7772 6170 2873 293a 0d0a 2020 2020 6966  wrap(s):..    if
+0001a610: 206c 656e 2873 2920 3e20 3620 616e 6420   len(s) > 6 and 
+0001a620: 735b 2d36 5d20 696e 2027 2b2d 2720 616e  s[-6] in '+-' an
+0001a630: 6420 735b 2d33 5d20 3d3d 2027 3a27 3a20  d s[-3] == ':': 
+0001a640: 2320 2b30 313a 3030 2066 6d74 2074 696d  # +01:00 fmt tim
+0001a650: 657a 6f6e 6520 7072 6573 656e 743f 0d0a  ezone present?..
+0001a660: 2020 2020 2020 2020 7320 3d20 735b 3a2d          s = s[:-
+0001a670: 365d 0d0a 2020 2020 7265 7475 726e 2028  6]..    return (
+0001a680: 732b 272e 3030 3030 3030 2729 2069 6620  s+'.000000') if 
+0001a690: 272e 2720 6e6f 7420 696e 2073 2065 6c73  '.' not in s els
+0001a6a0: 6520 730d 0a0d 0a0d 0a64 6566 205f 7832  e s......def _x2
+0001a6b0: 6c6f 6361 6c5f 7428 6461 7461 7372 632c  local_t(datasrc,
+0001a6c0: 2078 293a 0d0a 2020 2020 6966 2064 6973   x):..    if dis
+0001a6d0: 706c 6179 5f74 696d 657a 6f6e 6520 3d3d  play_timezone ==
+0001a6e0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0001a6f0: 7265 7475 726e 205f 7832 7574 6328 6461  return _x2utc(da
+0001a700: 7461 7372 632c 2078 290d 0a20 2020 2072  tasrc, x)..    r
+0001a710: 6574 7572 6e20 5f78 3274 2864 6174 6173  eturn _x2t(datas
+0001a720: 7263 2c20 782c 206c 616d 6264 6120 743a  rc, x, lambda t:
+0001a730: 205f 6d69 6c6c 6973 6563 6f6e 645f 747a   _millisecond_tz
+0001a740: 5f77 7261 7028 6461 7465 7469 6d65 2e66  _wrap(datetime.f
+0001a750: 726f 6d74 696d 6573 7461 6d70 2874 2f31  romtimestamp(t/1
+0001a760: 6539 2c20 747a 3d64 6973 706c 6179 5f74  e9, tz=display_t
+0001a770: 696d 657a 6f6e 6529 2e69 736f 666f 726d  imezone).isoform
+0001a780: 6174 2873 6570 3d27 2027 2929 290d 0a0d  at(sep=' ')))...
+0001a790: 0a0d 0a64 6566 205f 7832 7574 6328 6461  ...def _x2utc(da
+0001a7a0: 7461 7372 632c 2078 293a 0d0a 2020 2020  tasrc, x):..    
+0001a7b0: 2320 7573 696e 6720 7064 2e74 6f5f 6461  # using pd.to_da
+0001a7c0: 7465 7469 6d65 2061 6c6c 6f77 2066 6f72  tetime allow for
+0001a7d0: 2070 7265 2d31 3937 3020 6461 7465 730d   pre-1970 dates.
+0001a7e0: 0a20 2020 2072 6574 7572 6e20 5f78 3274  .    return _x2t
+0001a7f0: 2864 6174 6173 7263 2c20 782c 206c 616d  (datasrc, x, lam
+0001a800: 6264 6120 743a 2070 642e 746f 5f64 6174  bda t: pd.to_dat
+0001a810: 6574 696d 6528 742c 2075 6e69 743d 276e  etime(t, unit='n
+0001a820: 7327 292e 7374 7266 7469 6d65 2827 2559  s').strftime('%Y
+0001a830: 2d25 6d2d 2564 2025 483a 254d 3a25 532e  -%m-%d %H:%M:%S.
+0001a840: 2566 2729 290d 0a0d 0a0d 0a64 6566 205f  %f'))......def _
+0001a850: 7832 7428 6461 7461 7372 632c 2078 2c20  x2t(datasrc, x, 
+0001a860: 7473 3273 7472 293a 0d0a 2020 2020 6966  ts2str):..    if
+0001a870: 206e 6f74 2064 6174 6173 7263 3a0d 0a20   not datasrc:.. 
+0001a880: 2020 2020 2020 2072 6574 7572 6e20 2727         return ''
+0001a890: 2c46 616c 7365 0d0a 2020 2020 7472 793a  ,False..    try:
+0001a8a0: 0d0a 2020 2020 2020 2020 7820 2b3d 2030  ..        x += 0
+0001a8b0: 2e35 0d0a 2020 2020 2020 2020 742c 5f2c  .5..        t,_,
+0001a8c0: 5f2c 5f2c 636e 7420 3d20 6461 7461 7372  _,_,cnt = datasr
+0001a8d0: 632e 6869 6c6f 2878 2c20 7829 0d0a 2020  c.hilo(x, x)..  
+0001a8e0: 2020 2020 2020 6966 2063 6e74 3a0d 0a20        if cnt:.. 
+0001a8f0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0001a900: 7420 6461 7461 7372 632e 7469 6d65 6261  t datasrc.timeba
+0001a910: 7365 6428 293a 0d0a 2020 2020 2020 2020  sed():..        
+0001a920: 2020 2020 2020 2020 7265 7475 726e 2027          return '
+0001a930: 2567 2720 2520 742c 2046 616c 7365 0d0a  %g' % t, False..
+0001a940: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
+0001a950: 7473 3273 7472 2874 290d 0a20 2020 2020  ts2str(t)..     
+0001a960: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001a970: 2020 2020 2069 6620 6570 6f63 685f 7065       if epoch_pe
+0001a980: 7269 6f64 203e 3d20 3233 2a36 302a 3630  riod >= 23*60*60
+0001a990: 3a20 2320 6461 796c 6967 6874 2073 6176  : # daylight sav
+0001a9a0: 696e 6773 2c20 6c65 6170 2073 6563 6f6e  ings, leap secon
+0001a9b0: 6473 2c20 6574 630d 0a20 2020 2020 2020  ds, etc..       
+0001a9c0: 2020 2020 2020 2020 2069 203d 2073 2e69           i = s.i
+0001a9d0: 6e64 6578 2827 2027 290d 0a20 2020 2020  ndex(' ')..     
+0001a9e0: 2020 2020 2020 2065 6c69 6620 6570 6f63         elif epoc
+0001a9f0: 685f 7065 7269 6f64 203e 3d20 3539 3a20  h_period >= 59: 
+0001aa00: 2320 636f 6e73 6964 6572 206c 6561 7020  # consider leap 
+0001aa10: 7365 636f 6e64 730d 0a20 2020 2020 2020  seconds..       
+0001aa20: 2020 2020 2020 2020 2069 203d 2073 2e72           i = s.r
+0001aa30: 696e 6465 7828 273a 2729 0d0a 2020 2020  index(':')..    
+0001aa40: 2020 2020 2020 2020 656c 6966 2065 706f          elif epo
+0001aa50: 6368 5f70 6572 696f 6420 3e3d 2031 3a0d  ch_period >= 1:.
+0001aa60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aa70: 2069 203d 2073 2e69 6e64 6578 2827 2e27   i = s.index('.'
+0001aa80: 2920 6966 2027 2e27 2069 6e20 7320 656c  ) if '.' in s el
+0001aa90: 7365 206c 656e 2873 290d 0a20 2020 2020  se len(s)..     
+0001aaa0: 2020 2020 2020 2065 6c69 6620 6570 6f63         elif epoc
+0001aab0: 685f 7065 7269 6f64 203e 3d20 302e 3030  h_period >= 0.00
+0001aac0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+0001aad0: 2020 2020 6920 3d20 2d33 0d0a 2020 2020      i = -3..    
+0001aae0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001aaf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001ab00: 203d 206c 656e 2873 290d 0a20 2020 2020   = len(s)..     
+0001ab10: 2020 2020 2020 2072 6574 7572 6e20 735b         return s[
+0001ab20: 3a69 5d2c 5472 7565 0d0a 2020 2020 6578  :i],True..    ex
+0001ab30: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0001ab40: 7320 653a 0d0a 2020 2020 2020 2020 696d  s e:..        im
+0001ab50: 706f 7274 2074 7261 6365 6261 636b 0d0a  port traceback..
+0001ab60: 2020 2020 2020 2020 7472 6163 6562 6163          tracebac
+0001ab70: 6b2e 7072 696e 745f 6578 6328 290d 0a20  k.print_exc().. 
+0001ab80: 2020 2072 6574 7572 6e20 2727 2c64 6174     return '',dat
+0001ab90: 6173 7263 2e74 696d 6562 6173 6564 2829  asrc.timebased()
+0001aba0: 0d0a 0d0a 0d0a 6465 6620 5f78 3279 6561  ......def _x2yea
+0001abb0: 7228 6461 7461 7372 632c 2078 293a 0d0a  r(datasrc, x):..
+0001abc0: 2020 2020 742c 6861 7364 7320 3d20 5f78      t,hasds = _x
+0001abd0: 326c 6f63 616c 5f74 2864 6174 6173 7263  2local_t(datasrc
+0001abe0: 2c20 7829 0d0a 2020 2020 7265 7475 726e  , x)..    return
+0001abf0: 2074 5b3a 345d 2c68 6173 6473 0d0a 0d0a   t[:4],hasds....
+0001ac00: 0d0a 6465 6620 5f72 6f75 6e64 5f74 6f5f  ..def _round_to_
+0001ac10: 7369 676e 6966 6963 616e 7428 726e 672c  significant(rng,
+0001ac20: 2072 6e67 6d61 782c 2078 2c20 7369 676e   rngmax, x, sign
+0001ac30: 6966 6963 616e 745f 6465 6369 6d61 6c73  ificant_decimals
+0001ac40: 2c20 7369 676e 6966 6963 616e 745f 6570  , significant_ep
+0001ac50: 7329 3a0d 0a20 2020 2069 735f 6869 6768  s):..    is_high
+0001ac60: 7265 7320 3d20 2872 6e67 2f73 6967 6e69  res = (rng/signi
+0001ac70: 6669 6361 6e74 5f65 7073 203e 2031 6532  ficant_eps > 1e2
+0001ac80: 2061 6e64 2072 6e67 6d61 783c 3165 2d32   and rngmax<1e-2
+0001ac90: 2920 6f72 2061 6273 2872 6e67 6d61 7829  ) or abs(rngmax)
+0001aca0: 203e 2031 6537 206f 7220 726e 6720 3c20   > 1e7 or rng < 
+0001acb0: 3165 2d35 0d0a 2020 2020 7364 203d 2073  1e-5..    sd = s
+0001acc0: 6967 6e69 6669 6361 6e74 5f64 6563 696d  ignificant_decim
+0001acd0: 616c 730d 0a20 2020 2069 6620 6973 5f68  als..    if is_h
+0001ace0: 6967 6872 6573 2061 6e64 2061 6273 2878  ighres and abs(x
+0001acf0: 293e 303a 0d0a 2020 2020 2020 2020 6578  )>0:..        ex
+0001ad00: 7031 3020 3d20 666c 6f6f 7228 6e70 2e6c  p10 = floor(np.l
+0001ad10: 6f67 3130 2861 6273 2878 2929 290d 0a20  og10(abs(x))).. 
+0001ad20: 2020 2020 2020 2078 203d 2078 202f 2028         x = x / (
+0001ad30: 3130 2a2a 6578 7031 3029 0d0a 2020 2020  10**exp10)..    
+0001ad40: 2020 2020 726d 203d 2069 6e74 2861 6273      rm = int(abs
+0001ad50: 286e 702e 6c6f 6731 3028 726e 676d 6178  (np.log10(rngmax
+0001ad60: 2929 2920 6966 2072 6e67 6d61 783e 3020  ))) if rngmax>0 
+0001ad70: 656c 7365 2030 0d0a 2020 2020 2020 2020  else 0..        
+0001ad80: 7364 203d 206d 696e 2833 2c20 7364 2b72  sd = min(3, sd+r
+0001ad90: 6d29 0d0a 2020 2020 2020 2020 666d 7420  m)..        fmt 
+0001ada0: 3d20 2725 2525 692e 2569 6665 2525 6927  = '%%%i.%ife%%i'
+0001adb0: 2025 2028 7364 2c20 7364 290d 0a20 2020   % (sd, sd)..   
+0001adc0: 2020 2020 2072 203d 2066 6d74 2025 2028       r = fmt % (
+0001add0: 782c 2065 7870 3130 290d 0a20 2020 2065  x, exp10)..    e
+0001ade0: 6c73 653a 0d0a 2020 2020 2020 2020 6570  lse:..        ep
+0001adf0: 7320 3d20 666d 6f64 2878 2c20 7369 676e  s = fmod(x, sign
+0001ae00: 6966 6963 616e 745f 6570 7329 0d0a 2020  ificant_eps)..  
+0001ae10: 2020 2020 2020 6966 2061 6273 2865 7073        if abs(eps
+0001ae20: 2920 3e3d 2073 6967 6e69 6669 6361 6e74  ) >= significant
+0001ae30: 5f65 7073 2f32 3a0d 0a20 2020 2020 2020  _eps/2:..       
+0001ae40: 2020 2020 2023 2072 6f75 6e64 2075 700d       # round up.
+0001ae50: 0a20 2020 2020 2020 2020 2020 2065 7073  .            eps
+0001ae60: 202d 3d20 6e70 2e73 6967 6e28 6570 7329   -= np.sign(eps)
+0001ae70: 2a73 6967 6e69 6669 6361 6e74 5f65 7073  *significant_eps
+0001ae80: 0d0a 2020 2020 2020 2020 7820 2d3d 2065  ..        x -= e
+0001ae90: 7073 0d0a 2020 2020 2020 2020 666d 7420  ps..        fmt 
+0001aea0: 3d20 2725 2525 692e 2569 6627 2025 2028  = '%%%i.%if' % (
+0001aeb0: 7364 2c20 7364 290d 0a20 2020 2020 2020  sd, sd)..       
+0001aec0: 2072 203d 2066 6d74 2025 2078 0d0a 2020   r = fmt % x..  
+0001aed0: 2020 7265 7475 726e 2072 0d0a 0d0a 0d0a    return r......
+0001aee0: 6465 6620 5f72 6f69 6861 6e64 6c65 5f6d  def _roihandle_m
+0001aef0: 6f76 655f 736e 6170 2876 622c 206f 7269  ove_snap(vb, ori
+0001af00: 675f 6675 6e63 2c20 706f 732c 206d 6f64  g_func, pos, mod
+0001af10: 6966 6965 7273 3d51 7443 6f72 652e 5174  ifiers=QtCore.Qt
+0001af20: 2e4b 6579 626f 6172 644d 6f64 6966 6965  .KeyboardModifie
+0001af30: 722c 2066 696e 6973 683d 5472 7565 293a  r, finish=True):
+0001af40: 0d0a 2020 2020 706f 7320 3d20 7662 2e6d  ..    pos = vb.m
+0001af50: 6170 4465 7669 6365 546f 5669 6577 2870  apDeviceToView(p
+0001af60: 6f73 290d 0a20 2020 2070 6f73 203d 205f  os)..    pos = _
+0001af70: 636c 616d 705f 706f 696e 7428 7662 2e70  clamp_point(vb.p
+0001af80: 6172 656e 7428 292c 2070 6f73 290d 0a20  arent(), pos).. 
+0001af90: 2020 2070 6f73 203d 2076 622e 6d61 7056     pos = vb.mapV
+0001afa0: 6965 7754 6f44 6576 6963 6528 706f 7329  iewToDevice(pos)
+0001afb0: 0d0a 2020 2020 6f72 6967 5f66 756e 6328  ..    orig_func(
+0001afc0: 706f 732c 206d 6f64 6966 6965 7273 3d6d  pos, modifiers=m
+0001afd0: 6f64 6966 6965 7273 2c20 6669 6e69 7368  odifiers, finish
+0001afe0: 3d66 696e 6973 6829 0d0a 0d0a 0d0a 6465  =finish)......de
+0001aff0: 6620 5f63 6c61 6d70 5f78 7928 6178 2c20  f _clamp_xy(ax, 
+0001b000: 782c 2079 293a 0d0a 2020 2020 7920 3d20  x, y):..    y = 
+0001b010: 6178 2e76 622e 7973 6361 6c65 2e78 666f  ax.vb.yscale.xfo
+0001b020: 726d 2879 290d 0a20 2020 2069 6620 636c  rm(y)..    if cl
+0001b030: 616d 705f 6772 6964 2061 6e64 2061 782e  amp_grid and ax.
+0001b040: 7662 2e78 5f69 6e64 6578 6564 3a0d 0a20  vb.x_indexed:.. 
+0001b050: 2020 2020 2020 2064 7320 3d20 6178 2e76         ds = ax.v
+0001b060: 622e 6461 7461 7372 630d 0a20 2020 2020  b.datasrc..     
+0001b070: 2020 2069 6620 7820 3c20 3020 6f72 2028     if x < 0 or (
+0001b080: 6473 2061 6e64 2078 203e 206c 656e 2864  ds and x > len(d
+0001b090: 732e 6466 292d 3129 3a0d 0a20 2020 2020  s.df)-1):..     
+0001b0a0: 2020 2020 2020 2078 203d 2030 2069 6620         x = 0 if 
+0001b0b0: 7820 3c20 3020 656c 7365 206c 656e 2864  x < 0 else len(d
+0001b0c0: 732e 6466 292d 310d 0a20 2020 2020 2020  s.df)-1..       
+0001b0d0: 2078 203d 205f 726f 756e 6428 7829 0d0a   x = _round(x)..
+0001b0e0: 2020 2020 2020 2020 6570 7320 3d20 6178          eps = ax
+0001b0f0: 2e73 6967 6e69 6669 6361 6e74 5f65 7073  .significant_eps
+0001b100: 0d0a 2020 2020 2020 2020 6966 2065 7073  ..        if eps
+0001b110: 203e 2031 652d 383a 0d0a 2020 2020 2020   > 1e-8:..      
+0001b120: 2020 2020 2020 6570 7332 203d 206e 702e        eps2 = np.
+0001b130: 7369 676e 2879 2920 2a20 302e 3520 2a20  sign(y) * 0.5 * 
+0001b140: 6570 730d 0a20 2020 2020 2020 2020 2020  eps..           
+0001b150: 2079 202d 3d20 666d 6f64 2879 2b65 7073   y -= fmod(y+eps
+0001b160: 322c 2065 7073 2920 2d20 6570 7332 0d0a  2, eps) - eps2..
+0001b170: 2020 2020 7920 3d20 6178 2e76 622e 7973      y = ax.vb.ys
+0001b180: 6361 6c65 2e69 6e76 7866 6f72 6d28 792c  cale.invxform(y,
+0001b190: 2076 6572 6966 793d 5472 7565 290d 0a20   verify=True).. 
+0001b1a0: 2020 2072 6574 7572 6e20 782c 2079 0d0a     return x, y..
+0001b1b0: 0d0a 0d0a 6465 6620 5f63 6c61 6d70 5f70  ....def _clamp_p
+0001b1c0: 6f69 6e74 2861 782c 2070 293a 0d0a 2020  oint(ax, p):..  
+0001b1d0: 2020 6966 2063 6c61 6d70 5f67 7269 643a    if clamp_grid:
+0001b1e0: 0d0a 2020 2020 2020 2020 782c 7920 3d20  ..        x,y = 
+0001b1f0: 5f63 6c61 6d70 5f78 7928 6178 2c20 702e  _clamp_xy(ax, p.
+0001b200: 7828 292c 2070 2e79 2829 290d 0a20 2020  x(), p.y())..   
+0001b210: 2020 2020 2072 6574 7572 6e20 7067 2e50       return pg.P
+0001b220: 6f69 6e74 2878 2c20 7929 0d0a 2020 2020  oint(x, y)..    
+0001b230: 7265 7475 726e 2070 0d0a 0d0a 0d0a 6465  return p......de
+0001b240: 6620 5f64 7261 775f 6c69 6e65 5f73 6567  f _draw_line_seg
+0001b250: 6d65 6e74 5f74 6578 7428 706f 6c79 6c69  ment_text(polyli
+0001b260: 6e65 2c20 7365 676d 656e 742c 2070 6f73  ne, segment, pos
+0001b270: 302c 2070 6f73 3129 3a0d 0a20 2020 2066  0, pos1):..    f
+0001b280: 7365 6373 203d 204e 6f6e 650d 0a20 2020  secs = None..   
+0001b290: 2064 6174 6173 7263 203d 2070 6f6c 796c   datasrc = polyl
+0001b2a0: 696e 652e 7662 2e64 6174 6173 7263 0d0a  ine.vb.datasrc..
+0001b2b0: 2020 2020 6966 2064 6174 6173 7263 2061      if datasrc a
+0001b2c0: 6e64 2063 6c61 6d70 5f67 7269 643a 0d0a  nd clamp_grid:..
+0001b2d0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+0001b2e0: 2020 2020 2020 2020 2020 7830 2c78 3120            x0,x1 
+0001b2f0: 3d20 706f 7330 2e78 2829 2b30 2e35 2c20  = pos0.x()+0.5, 
+0001b300: 706f 7331 2e78 2829 2b30 2e35 0d0a 2020  pos1.x()+0.5..  
+0001b310: 2020 2020 2020 2020 2020 7430 2c5f 2c5f            t0,_,_
+0001b320: 2c5f 2c63 6e74 3020 3d20 6461 7461 7372  ,_,cnt0 = datasr
+0001b330: 632e 6869 6c6f 2878 302c 2078 3029 0d0a  c.hilo(x0, x0)..
+0001b340: 2020 2020 2020 2020 2020 2020 7431 2c5f              t1,_
+0001b350: 2c5f 2c5f 2c63 6e74 3120 3d20 6461 7461  ,_,_,cnt1 = data
+0001b360: 7372 632e 6869 6c6f 2878 312c 2078 3129  src.hilo(x1, x1)
+0001b370: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001b380: 2063 6e74 3020 616e 6420 636e 7431 3a0d   cnt0 and cnt1:.
+0001b390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b3a0: 2066 7365 6373 203d 2061 6273 2874 3120   fsecs = abs(t1 
+0001b3b0: 2d20 7430 2920 2f20 3165 390d 0a20 2020  - t0) / 1e9..   
+0001b3c0: 2020 2020 2065 7863 6570 743a 0d0a 2020       except:..  
+0001b3d0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+0001b3e0: 2020 2020 6469 6666 203d 2070 6f73 3120      diff = pos1 
+0001b3f0: 2d20 706f 7330 0d0a 2020 2020 6966 2066  - pos0..    if f
+0001b400: 7365 6373 2069 7320 4e6f 6e65 3a0d 0a20  secs is None:.. 
+0001b410: 2020 2020 2020 2066 7365 6373 203d 2061         fsecs = a
+0001b420: 6273 2864 6966 662e 7828 292a 6570 6f63  bs(diff.x()*epoc
+0001b430: 685f 7065 7269 6f64 290d 0a20 2020 2073  h_period)..    s
+0001b440: 6563 7320 3d20 696e 7428 6673 6563 7329  ecs = int(fsecs)
+0001b450: 0d0a 2020 2020 6d69 6e73 203d 2073 6563  ..    mins = sec
+0001b460: 732f 2f36 300d 0a20 2020 2068 6f75 7273  s//60..    hours
+0001b470: 203d 206d 696e 732f 2f36 300d 0a20 2020   = mins//60..   
+0001b480: 206d 696e 7320 3d20 6d69 6e73 2536 300d   mins = mins%60.
+0001b490: 0a20 2020 2073 6563 7320 3d20 7365 6373  .    secs = secs
+0001b4a0: 2536 300d 0a20 2020 2069 6620 686f 7572  %60..    if hour
+0001b4b0: 733d 3d30 2061 6e64 206d 696e 733d 3d30  s==0 and mins==0
+0001b4c0: 2061 6e64 2073 6563 7320 3c20 3630 2061   and secs < 60 a
+0001b4d0: 6e64 2065 706f 6368 5f70 6572 696f 6420  nd epoch_period 
+0001b4e0: 3c20 313a 0d0a 2020 2020 2020 2020 6d73  < 1:..        ms
+0001b4f0: 6563 7320 3d20 696e 7428 2866 7365 6373  ecs = int((fsecs
+0001b500: 2d69 6e74 2866 7365 6373 2929 2a31 3030  -int(fsecs))*100
+0001b510: 3029 0d0a 2020 2020 2020 2020 7473 203d  0)..        ts =
+0001b520: 2027 2530 2e32 693a 2530 2e32 692e 2530   '%0.2i:%0.2i.%0
+0001b530: 2e33 6927 2025 2028 6d69 6e73 2c20 7365  .3i' % (mins, se
+0001b540: 6373 2c20 6d73 6563 7329 0d0a 2020 2020  cs, msecs)..    
+0001b550: 656c 6966 2068 6f75 7273 3d3d 3020 616e  elif hours==0 an
+0001b560: 6420 6d69 6e73 203c 2036 3020 616e 6420  d mins < 60 and 
+0001b570: 6570 6f63 685f 7065 7269 6f64 203c 2036  epoch_period < 6
+0001b580: 303a 0d0a 2020 2020 2020 2020 7473 203d  0:..        ts =
+0001b590: 2027 2530 2e32 693a 2530 2e32 693a 2530   '%0.2i:%0.2i:%0
+0001b5a0: 2e32 6927 2025 2028 686f 7572 732c 206d  .2i' % (hours, m
+0001b5b0: 696e 732c 2073 6563 7329 0d0a 2020 2020  ins, secs)..    
+0001b5c0: 656c 6966 2068 6f75 7273 203c 2032 343a  elif hours < 24:
+0001b5d0: 0d0a 2020 2020 2020 2020 7473 203d 2027  ..        ts = '
+0001b5e0: 2530 2e32 693a 2530 2e32 6927 2025 2028  %0.2i:%0.2i' % (
+0001b5f0: 686f 7572 732c 206d 696e 7329 0d0a 2020  hours, mins)..  
+0001b600: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001b610: 2064 6179 7320 3d20 686f 7572 7320 2f2f   days = hours //
+0001b620: 2032 340d 0a20 2020 2020 2020 2068 6f75   24..        hou
+0001b630: 7273 2025 3d20 3234 0d0a 2020 2020 2020  rs %= 24..      
+0001b640: 2020 7473 203d 2027 2569 6420 2530 2e32    ts = '%id %0.2
+0001b650: 693a 2530 2e32 6927 2025 2028 6461 7973  i:%0.2i' % (days
+0001b660: 2c20 686f 7572 732c 206d 696e 7329 0d0a  , hours, mins)..
+0001b670: 2020 2020 2020 2020 6966 2074 732e 656e          if ts.en
+0001b680: 6473 7769 7468 2827 2030 303a 3030 2729  dswith(' 00:00')
+0001b690: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+0001b6a0: 7320 3d20 7473 2e70 6172 7469 7469 6f6e  s = ts.partition
+0001b6b0: 2827 2027 295b 305d 0d0a 2020 2020 7973  (' ')[0]..    ys
+0001b6c0: 6320 3d20 706f 6c79 6c69 6e65 2e76 622e  c = polyline.vb.
+0001b6d0: 7973 6361 6c65 0d0a 2020 2020 6966 2070  yscale..    if p
+0001b6e0: 6f6c 796c 696e 652e 7662 2e79 5f70 6f73  olyline.vb.y_pos
+0001b6f0: 6974 6976 653a 0d0a 2020 2020 2020 2020  itive:..        
+0001b700: 7930 2c79 3120 3d20 7973 632e 7866 6f72  y0,y1 = ysc.xfor
+0001b710: 6d28 706f 7330 2e79 2829 292c 2079 7363  m(pos0.y()), ysc
+0001b720: 2e78 666f 726d 2870 6f73 312e 7928 2929  .xform(pos1.y())
+0001b730: 0d0a 2020 2020 2020 2020 6966 2079 303a  ..        if y0:
+0001b740: 0d0a 2020 2020 2020 2020 2020 2020 6761  ..            ga
+0001b750: 696e 203d 2079 3120 2f20 7930 202d 2031  in = y1 / y0 - 1
+0001b760: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001b770: 2067 6169 6e20 3e20 3130 3a0d 0a20 2020   gain > 10:..   
+0001b780: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0001b790: 7565 203d 2027 7825 6927 2025 2067 6169  ue = 'x%i' % gai
+0001b7a0: 6e0d 0a20 2020 2020 2020 2020 2020 2065  n..            e
+0001b7b0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0001b7c0: 2020 2020 2020 7661 6c75 6520 3d20 2725        value = '%
+0001b7d0: 2b2e 3266 2025 2527 2025 2028 3130 3020  +.2f %%' % (100 
+0001b7e0: 2a20 6761 696e 290d 0a20 2020 2020 2020  * gain)..       
+0001b7f0: 2065 6c69 6620 6e6f 7420 7931 3a0d 0a20   elif not y1:.. 
+0001b800: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0001b810: 203d 2027 3027 0d0a 2020 2020 2020 2020   = '0'..        
+0001b820: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001b830: 2020 2076 616c 7565 203d 2027 2be2 889e     value = '+...
+0001b840: 2720 6966 2079 313e 3020 656c 7365 2027  ' if y1>0 else '
+0001b850: 2de2 889e 270d 0a20 2020 2065 6c73 653a  -...'..    else:
+0001b860: 0d0a 2020 2020 2020 2020 6479 203d 2079  ..        dy = y
+0001b870: 7363 2e78 666f 726d 2864 6966 662e 7928  sc.xform(diff.y(
+0001b880: 2929 0d0a 2020 2020 2020 2020 6966 2064  ))..        if d
+0001b890: 7920 616e 6420 2861 6273 2864 7929 203e  y and (abs(dy) >
+0001b8a0: 3d20 3165 3420 6f72 2061 6273 2864 7929  = 1e4 or abs(dy)
+0001b8b0: 203c 3d20 3165 2d32 293a 0d0a 2020 2020   <= 1e-2):..    
+0001b8c0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+0001b8d0: 2725 2b33 2e33 6727 2025 2064 790d 0a20  '%+3.3g' % dy.. 
+0001b8e0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0001b8f0: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
+0001b900: 3d20 2725 2b32 2e32 6627 2025 2064 790d  = '%+2.2f' % dy.
+0001b910: 0a20 2020 2065 7874 7261 203d 205f 6472  .    extra = _dr
+0001b920: 6177 5f6c 696e 655f 6578 7472 615f 7465  aw_line_extra_te
+0001b930: 7874 2870 6f6c 796c 696e 652c 2073 6567  xt(polyline, seg
+0001b940: 6d65 6e74 2c20 706f 7330 2c20 706f 7331  ment, pos0, pos1
+0001b950: 290d 0a20 2020 2072 6574 7572 6e20 2725  )..    return '%
+0001b960: 7320 2573 2028 2573 2927 2025 2028 7661  s %s (%s)' % (va
+0001b970: 6c75 652c 2065 7874 7261 2c20 7473 290d  lue, extra, ts).
+0001b980: 0a0d 0a0d 0a64 6566 205f 6472 6177 5f6c  .....def _draw_l
+0001b990: 696e 655f 6578 7472 615f 7465 7874 2870  ine_extra_text(p
+0001b9a0: 6f6c 796c 696e 652c 2073 6567 6d65 6e74  olyline, segment
+0001b9b0: 2c20 706f 7330 2c20 706f 7331 293a 0d0a  , pos0, pos1):..
+0001b9c0: 2020 2020 2727 2753 686f 7773 2074 6865      '''Shows the
+0001b9d0: 2070 726f 706f 7274 696f 6e73 206f 6620   proportions of 
+0001b9e0: 7468 6973 206c 696e 6520 6865 6967 6874  this line height
+0001b9f0: 2063 6f6d 7061 7265 6420 746f 2074 6865   compared to the
+0001ba00: 2070 7265 7669 6f75 7320 7365 676d 656e   previous segmen
+0001ba10: 742e 2727 270d 0a20 2020 2070 7265 765f  t.'''..    prev_
+0001ba20: 7465 7874 203d 204e 6f6e 650d 0a20 2020  text = None..   
+0001ba30: 2066 6f72 2074 6578 7420 696e 2070 6f6c   for text in pol
+0001ba40: 796c 696e 652e 7465 7874 733a 0d0a 2020  yline.texts:..  
+0001ba50: 2020 2020 2020 6966 2070 7265 765f 7465        if prev_te
+0001ba60: 7874 2069 7320 6e6f 7420 4e6f 6e65 2061  xt is not None a
+0001ba70: 6e64 2074 6578 742e 7365 676d 656e 7420  nd text.segment 
+0001ba80: 3d3d 2073 6567 6d65 6e74 3a0d 0a20 2020  == segment:..   
+0001ba90: 2020 2020 2020 2020 2068 3020 3d20 7072           h0 = pr
+0001baa0: 6576 5f74 6578 742e 7365 676d 656e 742e  ev_text.segment.
+0001bab0: 6861 6e64 6c65 735b 305d 5b27 6974 656d  handles[0]['item
+0001bac0: 275d 0d0a 2020 2020 2020 2020 2020 2020  ']..            
+0001bad0: 6831 203d 2070 7265 765f 7465 7874 2e73  h1 = prev_text.s
+0001bae0: 6567 6d65 6e74 2e68 616e 646c 6573 5b31  egment.handles[1
+0001baf0: 5d5b 2769 7465 6d27 5d0d 0a20 2020 2020  ]['item']..     
+0001bb00: 2020 2020 2020 2070 7265 765f 6368 616e         prev_chan
+0001bb10: 6765 203d 2068 312e 706f 7328 292e 7928  ge = h1.pos().y(
+0001bb20: 2920 2d20 6830 2e70 6f73 2829 2e79 2829  ) - h0.pos().y()
+0001bb30: 0d0a 2020 2020 2020 2020 2020 2020 7468  ..            th
+0001bb40: 6973 5f63 6861 6e67 6520 3d20 706f 7331  is_change = pos1
+0001bb50: 2e79 2829 202d 2070 6f73 302e 7928 290d  .y() - pos0.y().
+0001bb60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001bb70: 6e6f 7420 6162 7328 7072 6576 5f63 6861  not abs(prev_cha
+0001bb80: 6e67 6529 203e 2031 652d 3134 3a0d 0a20  nge) > 1e-14:.. 
+0001bb90: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001bba0: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
+0001bbb0: 2020 6368 616e 6765 5f70 6172 7420 3d20    change_part = 
+0001bbc0: 6162 7328 7468 6973 5f63 6861 6e67 6520  abs(this_change 
+0001bbd0: 2f20 7072 6576 5f63 6861 6e67 6529 0d0a  / prev_change)..
+0001bbe0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001bbf0: 726e 2027 203d 2031 3a25 2e32 6620 2720  rn ' = 1:%.2f ' 
+0001bc00: 2520 6368 616e 6765 5f70 6172 740d 0a20  % change_part.. 
+0001bc10: 2020 2020 2020 2070 7265 765f 7465 7874         prev_text
+0001bc20: 203d 2074 6578 740d 0a20 2020 2072 6574   = text..    ret
+0001bc30: 7572 6e20 2727 0d0a 0d0a 0d0a 6465 6620  urn ''......def 
+0001bc40: 5f6d 616b 6570 656e 2863 6f6c 6f72 2c20  _makepen(color, 
+0001bc50: 7374 796c 653d 4e6f 6e65 2c20 7769 6474  style=None, widt
+0001bc60: 683d 3129 3a0d 0a20 2020 2069 6620 7374  h=1):..    if st
+0001bc70: 796c 6520 6973 204e 6f6e 6520 6f72 2073  yle is None or s
+0001bc80: 7479 6c65 203d 3d20 272d 273a 0d0a 2020  tyle == '-':..  
+0001bc90: 2020 2020 2020 7265 7475 726e 2070 672e        return pg.
+0001bca0: 6d6b 5065 6e28 636f 6c6f 723d 636f 6c6f  mkPen(color=colo
+0001bcb0: 722c 2077 6964 7468 3d77 6964 7468 290d  r, width=width).
+0001bcc0: 0a20 2020 2064 6173 6820 3d20 5b5d 0d0a  .    dash = []..
+0001bcd0: 2020 2020 666f 7220 6368 2069 6e20 7374      for ch in st
+0001bce0: 796c 653a 0d0a 2020 2020 2020 2020 6966  yle:..        if
+0001bcf0: 2063 6820 3d3d 2027 2d27 3a0d 0a20 2020   ch == '-':..   
+0001bd00: 2020 2020 2020 2020 2064 6173 6820 2b3d           dash +=
+0001bd10: 205b 342c 325d 0d0a 2020 2020 2020 2020   [4,2]..        
+0001bd20: 656c 6966 2063 6820 3d3d 2027 5f27 3a0d  elif ch == '_':.
+0001bd30: 0a20 2020 2020 2020 2020 2020 2064 6173  .            das
+0001bd40: 6820 2b3d 205b 3130 2c32 5d0d 0a20 2020  h += [10,2]..   
+0001bd50: 2020 2020 2065 6c69 6620 6368 203d 3d20       elif ch == 
+0001bd60: 272e 273a 0d0a 2020 2020 2020 2020 2020  '.':..          
+0001bd70: 2020 6461 7368 202b 3d20 5b31 2c32 5d0d    dash += [1,2].
+0001bd80: 0a20 2020 2020 2020 2065 6c69 6620 6368  .        elif ch
+0001bd90: 203d 3d20 2720 273a 0d0a 2020 2020 2020   == ' ':..      
+0001bda0: 2020 2020 2020 6966 2064 6173 683a 0d0a        if dash:..
+0001bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bdc0: 6461 7368 5b2d 315d 202b 3d20 320d 0a20  dash[-1] += 2.. 
+0001bdd0: 2020 2072 6574 7572 6e20 7067 2e6d 6b50     return pg.mkP
+0001bde0: 656e 2863 6f6c 6f72 3d63 6f6c 6f72 2c20  en(color=color, 
+0001bdf0: 7374 796c 653d 5174 436f 7265 2e51 742e  style=QtCore.Qt.
+0001be00: 5065 6e53 7479 6c65 2e43 7573 746f 6d44  PenStyle.CustomD
+0001be10: 6173 684c 696e 652c 2064 6173 683d 6461  ashLine, dash=da
+0001be20: 7368 2c20 7769 6474 683d 7769 6474 6829  sh, width=width)
+0001be30: 0d0a 0d0a 0d0a 6465 6620 5f72 6f75 6e64  ......def _round
+0001be40: 2876 293a 0d0a 2020 2020 7265 7475 726e  (v):..    return
+0001be50: 2066 6c6f 6f72 2876 2b30 2e35 290d 0a0d   floor(v+0.5)...
+0001be60: 0a0d 0a74 7279 3a0d 0a20 2020 2071 7476  ...try:..    qtv
+0001be70: 6572 203d 2027 2564 2e25 6427 2025 2028  er = '%d.%d' % (
+0001be80: 5174 436f 7265 2e51 545f 5645 5253 494f  QtCore.QT_VERSIO
+0001be90: 4e2f 2f32 3536 2f2f 3235 362c 2051 7443  N//256//256, QtC
+0001bea0: 6f72 652e 5154 5f56 4552 5349 4f4e 2f2f  ore.QT_VERSION//
+0001beb0: 3235 3625 3235 3629 0d0a 2020 2020 6966  256%256)..    if
+0001bec0: 2071 7476 6572 206e 6f74 2069 6e20 2827   qtver not in ('
+0001bed0: 352e 3927 2c20 2735 2e31 3327 2920 616e  5.9', '5.13') an
+0001bee0: 6420 5b69 6e74 2869 2920 666f 7220 6920  d [int(i) for i 
+0001bef0: 696e 2070 672e 5f5f 7665 7273 696f 6e5f  in pg.__version_
+0001bf00: 5f2e 7370 6c69 7428 272e 2729 5d20 3c3d  _.split('.')] <=
+0001bf10: 205b 302c 3131 2c30 5d3a 0d0a 2020 2020   [0,11,0]:..    
+0001bf20: 2020 2020 7072 696e 7428 2757 4152 4e49      print('WARNI
+0001bf30: 4e47 3a20 796f 7572 2076 6572 7369 6f6e  NG: your version
+0001bf40: 206f 6620 5174 206d 6179 206e 6f74 2070   of Qt may not p
+0001bf50: 6c6f 7420 6375 7276 6573 2063 6f6e 7461  lot curves conta
+0001bf60: 696e 696e 6720 4e61 4e73 2061 6e64 2069  ining NaNs and i
+0001bf70: 7320 6e6f 7420 7265 636f 6d6d 656e 6465  s not recommende
+0001bf80: 642e 2729 0d0a 2020 2020 2020 2020 7072  d.')..        pr
+0001bf90: 696e 7428 2753 6565 2068 7474 7073 3a2f  int('See https:/
+0001bfa0: 2f67 6974 6875 622e 636f 6d2f 7079 7174  /github.com/pyqt
+0001bfb0: 6772 6170 682f 7079 7174 6772 6170 682f  graph/pyqtgraph/
+0001bfc0: 6973 7375 6573 2f31 3035 3727 290d 0a65  issues/1057')..e
+0001bfd0: 7863 6570 743a 0d0a 2020 2020 7061 7373  xcept:..    pass
+0001bfe0: 0d0a 0d0a 696d 706f 7274 206c 6f63 616c  ....import local
+0001bff0: 650d 0a63 6f64 652c 5f20 3d20 6c6f 6361  e..code,_ = loca
+0001c000: 6c65 2e67 6574 6465 6661 756c 746c 6f63  le.getdefaultloc
+0001c010: 616c 6528 290d 0a69 6620 636f 6465 2069  ale()..if code i
+0001c020: 7320 6e6f 7420 4e6f 6e65 2061 6e64 205c  s not None and \
+0001c030: 0d0a 2020 2020 2861 6e79 2873 616e 6374  ..    (any(sanct
+0001c040: 696f 6e65 6420 696e 2063 6f64 652e 6c6f  ioned in code.lo
+0001c050: 7765 7228 2920 666f 7220 7361 6e63 7469  wer() for sancti
+0001c060: 6f6e 6564 2069 6e20 275f 7275 205f 6279  oned in '_ru _by
+0001c070: 2072 755f 2062 655f 272e 7370 6c69 7428   ru_ be_'.split(
+0001c080: 2929 206f 7220 5c0d 0a20 2020 2020 616e  )) or \..     an
+0001c090: 7928 7361 6e63 7469 6f6e 6564 2069 6e20  y(sanctioned in 
+0001c0a0: 636f 6465 2e6c 6f77 6572 2829 2066 6f72  code.lower() for
+0001c0b0: 2073 616e 6374 696f 6e65 6420 696e 2027   sanctioned in '
+0001c0c0: 7275 2062 6527 2e73 706c 6974 2829 2929  ru be'.split()))
+0001c0d0: 3a0d 0a20 2020 2069 6d70 6f72 7420 6f73  :..    import os
+0001c0e0: 0d0a 2020 2020 6f73 2e5f 6578 6974 2831  ..    os._exit(1
+0001c0f0: 290d 0a20 2020 2061 7373 6572 7420 4661  )..    assert Fa
+0001c100: 6c73 650d 0a0d 0a23 2064 6566 6175 6c74  lse....# default
+0001c110: 2074 6f20 626c 6163 6b2d 6f6e 2d77 6869   to black-on-whi
+0001c120: 7465 0d0a 7067 2e77 6964 6765 7473 2e47  te..pg.widgets.G
+0001c130: 7261 7068 6963 7356 6965 772e 4772 6170  raphicsView.Grap
+0001c140: 6869 6373 5669 6577 2e77 6865 656c 4576  hicsView.wheelEv
+0001c150: 656e 7420 3d20 7061 7274 6961 6c6d 6574  ent = partialmet
+0001c160: 686f 6428 5f77 6865 656c 5f65 7665 6e74  hod(_wheel_event
+0001c170: 5f77 7261 7070 6572 2c20 7067 2e77 6964  _wrapper, pg.wid
+0001c180: 6765 7473 2e47 7261 7068 6963 7356 6965  gets.GraphicsVie
+0001c190: 772e 4772 6170 6869 6373 5669 6577 2e77  w.GraphicsView.w
+0001c1a0: 6865 656c 4576 656e 7429 0d0a 2320 7573  heelEvent)..# us
+0001c1b0: 6520 6669 6e70 6c6f 7420 696e 7374 6561  e finplot instea
+0001c1c0: 6420 6f66 206d 6174 706c 6f74 6c69 620d  d of matplotlib.
+0001c1d0: 0a70 642e 7365 745f 6f70 7469 6f6e 2827  .pd.set_option('
+0001c1e0: 706c 6f74 7469 6e67 2e62 6163 6b65 6e64  plotting.backend
+0001c1f0: 272c 2027 6669 6e70 6c6f 742e 7064 706c  ', 'finplot.pdpl
+0001c200: 6f74 2729 0d0a 2320 7069 636b 2075 7020  ot')..# pick up 
+0001c210: 7769 6e20 7265 736f 6c75 7469 6f6e 0d0a  win resolution..
+0001c220: 7472 793a 0d0a 2020 2020 696d 706f 7274  try:..    import
+0001c230: 2063 7479 7065 730d 0a20 2020 2075 7365   ctypes..    use
+0001c240: 7233 3220 3d20 6374 7970 6573 2e77 696e  r32 = ctypes.win
+0001c250: 646c 6c2e 7573 6572 3332 0d0a 2020 2020  dll.user32..    
+0001c260: 7573 6572 3332 2e53 6574 5072 6f63 6573  user32.SetProces
+0001c270: 7344 5049 4177 6172 6528 290d 0a20 2020  sDPIAware()..   
+0001c280: 206c 6f64 5f63 616e 646c 6573 203d 2069   lod_candles = i
+0001c290: 6e74 2875 7365 7233 322e 4765 7453 7973  nt(user32.GetSys
+0001c2a0: 7465 6d4d 6574 7269 6373 2830 2920 2a20  temMetrics(0) * 
+0001c2b0: 312e 3629 0d0a 2020 2020 6361 6e64 6c65  1.6)..    candle
+0001c2c0: 5f73 6861 646f 775f 7769 6474 6820 3d20  _shadow_width = 
+0001c2d0: 696e 7428 7573 6572 3332 2e47 6574 5379  int(user32.GetSy
+0001c2e0: 7374 656d 4d65 7472 6963 7328 3029 202f  stemMetrics(0) /
+0001c2f0: 2f20 3231 3030 202b 2031 2920 2320 3235  / 2100 + 1) # 25
+0001c300: 3630 2061 6e64 2072 6573 6f6c 7574 696f  60 and resolutio
+0001c310: 6e73 2061 626f 7665 202d 3e20 7769 6465  ns above -> wide
+0001c320: 7220 7368 6164 6f77 730d 0a65 7863 6570  r shadows..excep
+0001c330: 743a 0d0a 2020 2020 7061 7373 0d0a       t:..    pass..
```

### Comparing `finplot-1.9.0/finplot/pdplot.py` & `finplot-1.9.1/finplot/pdplot.py`

 * *Files identical despite different names*

### Comparing `finplot-1.9.0/finplot.egg-info/PKG-INFO` & `finplot-1.9.1/finplot.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 Metadata-Version: 2.1
 Name: finplot
-Version: 1.9.0
+Version: 1.9.1
 Summary: Finance plotting
 Home-page: https://github.com/highfestiva/finplot
 Author: Jonas Byström
 Author-email: highfestiva@gmail.com
-License: UNKNOWN
-Description: # Finance Plot
-        
-        Finance Plotter, or finplot, is a performant library with a clean api to help you with your backtesting. It's
-        optionated with good defaults, so you can start doing your work without having to setup plots, colors, scales,
-        autoscaling, keybindings, handle panning+vertical zooming (which all non-finance libraries have problems with).
-        And best of all: it can show hundreds of thousands of datapoints without batting an eye.
-        
-        <img src="https://badge.fury.io/py/finplot.svg"/> <img src="https://pepy.tech/badge/finplot/month"/> <img src="https://img.shields.io/badge/License-MIT-yellow.svg"/>
-        
-        
-        ## Features
-        
-        * Great performance compared to mpl_finance, plotly and Bokeh
-        * Clean api
-        * Works with both stocks as well as cryptocurrencies on any time resolution
-        * Show as many charts as you want on the same time axis, zoom on all of them at once
-        * Auto-reload position where you were looking last run
-        * Overlays, fill between, value bands, symbols, labels, legend, volume profile, heatmaps, etc.
-        * Can show real-time updates, including orderbook. Save screenshot.
-        * Comes with a [dozen](https://github.com/highfestiva/finplot/blob/master/finplot/examples) great examples.
-        
-        ![feature1](https://raw.githubusercontent.com/highfestiva/finplot/master/feature1.png)
-        
-        ![feature2](https://raw.githubusercontent.com/highfestiva/finplot/master/feature2.jpg)
-        
-        ![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature3.jpg)
-        
-        ![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature-nuts.jpg)
-        
-        
-        ## What it is not
-        
-        finplot *is not a web app*. It does not help you create an homebrew exchange. It does not work with Jupyter Labs.
-        
-        It is only intended for you to do backtesting in. That is not to say that you can't create a ticker or a trade
-        widget yourself. The library is based on the eminent pyqtgraph, which is fast and flexible, so feel free to hack
-        away if that's what you want.
-        
-        
-        ## Easy installation
-        
-        ```bash
-        $ pip install finplot
-        ```
-        
-        
-        ## Example
-        
-        It's straight-forward to start using. This shows every daily candle of Apple since the 80'ies:
-        
-        ```python
-        import finplot as fplt
-        import yfinance
-        
-        df = yfinance.download('AAPL')
-        fplt.candlestick_ochl(df[['Open', 'Close', 'High', 'Low']])
-        fplt.show()
-        ```
-        
-        For more examples and a bunch of snippets, see the [examples](https://github.com/highfestiva/finplot/blob/master/finplot/examples/)
-        directory or the [wiki](https://github.com/highfestiva/finplot/wiki). There you'll find how to plot MACD, Parabolic SAR, RSI,
-        volume profile and much more.
-        
-        
-        ## Coffee
-        
-        For future support and features, consider a small donation.
-        
-        BTC: bc1qk8m8yh86l2pz4eypflchr0tkn5aeud6cmt426m
-        
-        ETH: 0x684d7d4C52ed428AE9a36B2407ba909D896cDB67
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Finance Plot
+
+Finance Plotter, or finplot, is a performant library with a clean api to help you with your backtesting. It's
+optionated with good defaults, so you can start doing your work without having to setup plots, colors, scales,
+autoscaling, keybindings, handle panning+vertical zooming (which all non-finance libraries have problems with).
+And best of all: it can show hundreds of thousands of datapoints without batting an eye.
+
+<img src="https://badge.fury.io/py/finplot.svg"/> <img src="https://pepy.tech/badge/finplot/month"/> <img src="https://img.shields.io/badge/License-MIT-yellow.svg"/>
+
+
+## Features
+
+* Great performance compared to mpl_finance, plotly and Bokeh
+* Clean api
+* Works with both stocks as well as cryptocurrencies on any time resolution
+* Show as many charts as you want on the same time axis, zoom on all of them at once
+* Auto-reload position where you were looking last run
+* Overlays, fill between, value bands, symbols, labels, legend, volume profile, heatmaps, etc.
+* Can show real-time updates, including orderbook. Save screenshot.
+* Comes with a [dozen](https://github.com/highfestiva/finplot/blob/master/finplot/examples) great examples.
+
+![feature1](https://raw.githubusercontent.com/highfestiva/finplot/master/feature1.png)
+
+![feature2](https://raw.githubusercontent.com/highfestiva/finplot/master/feature2.jpg)
+
+![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature3.jpg)
+
+![feature3](https://raw.githubusercontent.com/highfestiva/finplot/master/feature-nuts.jpg)
+
+
+## What it is not
+
+finplot *is not a web app*. It does not help you create an homebrew exchange. It does not work with Jupyter Labs.
+
+It is only intended for you to do backtesting in. That is not to say that you can't create a ticker or a trade
+widget yourself. The library is based on the eminent pyqtgraph, which is fast and flexible, so feel free to hack
+away if that's what you want.
+
+
+## Easy installation
+
+```bash
+$ pip install finplot
+```
+
+
+## Example
+
+It's straight-forward to start using. This shows every daily candle of Apple since the 80'ies:
+
+```python
+import finplot as fplt
+import yfinance
+
+df = yfinance.download('AAPL')
+fplt.candlestick_ochl(df[['Open', 'Close', 'High', 'Low']])
+fplt.show()
+```
+
+For more examples and a bunch of snippets, see the [examples](https://github.com/highfestiva/finplot/blob/master/finplot/examples/)
+directory or the [wiki](https://github.com/highfestiva/finplot/wiki). There you'll find how to plot MACD, Parabolic SAR, RSI,
+volume profile and much more.
+
+
+## Coffee
+
+For future support and features, consider a small donation.
+
+BTC: bc1qk8m8yh86l2pz4eypflchr0tkn5aeud6cmt426m
+
+ETH: 0x684d7d4C52ed428AE9a36B2407ba909D896cDB67
```

### Comparing `finplot-1.9.0/setup.py` & `finplot-1.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='finplot',
-    version='1.9.0',
+    version='1.9.1',
     author='Jonas Byström',
     author_email='highfestiva@gmail.com',
     description='Finance plotting',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/highfestiva/finplot',
     packages=['finplot'],
```

