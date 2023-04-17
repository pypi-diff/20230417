# Comparing `tmp/seawolf-0.1.tar.gz` & `tmp/seawolf-0.1.1.tar.gz`

## Comparing `seawolf-0.1.tar` & `seawolf-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 seawolf-0.1/setup.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/__init__.py
--rw-r--r--   0        0        0    22312 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/_axes.py
--rw-r--r--   0        0        0    18493 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/_axesTools.py
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/_colors.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/_style.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/test.py
--rw-r--r--   0        0        0   823636 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/fonts/CAMBRIAI.TTF
--rw-r--r--   0        0        0   808520 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/fonts/CAMBRIAZ.TTF
--rw-r--r--   0        0        0   314820 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/fonts/Cambria.ttf
--rw-r--r--   0        0        0   795416 2020-02-02 00:00:00.000000 seawolf-0.1/seawolf/fonts/cambriab.ttf
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 seawolf-0.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 seawolf-0.1/LICENSE
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 seawolf-0.1/README.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 seawolf-0.1/pyproject.toml
--rw-r--r--   0        0        0    41273 2020-02-02 00:00:00.000000 seawolf-0.1/PKG-INFO
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 seawolf-0.1.1/setup.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 seawolf-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/__init__.py
+-rw-r--r--   0        0        0    23832 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/_axes.py
+-rw-r--r--   0        0        0    22831 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/_axesTools.py
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/_colors.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/_style.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/test.py
+-rw-r--r--   0        0        0   823636 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/fonts/CAMBRIAI.TTF
+-rw-r--r--   0        0        0   808520 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/fonts/CAMBRIAZ.TTF
+-rw-r--r--   0        0        0   314820 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/fonts/Cambria.ttf
+-rw-r--r--   0        0        0   795416 2020-02-02 00:00:00.000000 seawolf-0.1.1/seawolf/fonts/cambriab.ttf
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 seawolf-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 seawolf-0.1.1/LICENSE
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 seawolf-0.1.1/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 seawolf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    41275 2020-02-02 00:00:00.000000 seawolf-0.1.1/PKG-INFO
```

### Comparing `seawolf-0.1/setup.py` & `seawolf-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from setuptools import setup
 
 
 _version = '0.1'
 
 setup(name='seawolf',
       version=_version,
-      description='Tools for plots',
+      description='Tools for matplotlib plots',
       author='Bayron Torres Gordillo',
       author_email='torres.bayron@gmail.com',
+      long_description=readme.read(),
+      long_description_content_type='text/markdown',
       install_requires=['numpy','pandas','seaborn','matplotlib'],
       packages=['seawolf'],
       include_package_data=True,
       license = 'BSD',
       platforms = ["Windows", "Linux", "Solaris", "Mac OS-X", "Unix"],
       python_requires='>=3.5'
     )
```

### Comparing `seawolf-0.1/seawolf/_axes.py` & `seawolf-0.1.1/seawolf/_axes.py`

 * *Files 9% similar despite different names*

```diff
@@ -101,24 +101,33 @@
     axis: str = "x",
     visible: bool = True,
     labels: list = (),
     labelrotation: int = 0,
     loc=None,
     limit=_np.Infinity,
     bgcolors=list(),
-    **kwargs
+    **kwargs,
 ) -> _plt.Axes:
     ax = _axTools.gca(ax)
 
     if labels is None:
         labels = list()
 
-    d, kwargs = _axTools.get_init_kwargs(kwargs)
+    if loc == "None":
+        if axis == "x":
+            def_dic = {"va": "top", "ha": "center"}
+        elif axis == "y":
+            def_dic = {"va": "center", "ha": "right"}
+    else:
+        def_dic = {"va": "center_baseline", "ha": "center"}
 
-    locs = ["in", "out", "bottom", "top", "left", "right", None]
+    d, kwargs = _axTools.get_init_kwargs(kwargs, defaults=def_dic)
+    print(kwargs)
+
+    locs = ["in", "on", "bottom", "top", "left", "right", None]
     if not loc in locs:
         raise ValueError("The value in LOC is not recognized: {0}".format(locs))
 
     orient, _ = _axTools.orient(ax)
 
     fig = ax.get_figure()
     fig.canvas.draw()
@@ -126,180 +135,208 @@
     ax.tick_params(
         grid_color=d["grid_color"],
         color=d["color"],
         grid_alpha=d["grid_alpha"],
         labelsize=d["fontsize"],
         axis=axis,
         labelrotation=labelrotation,
-        **kwargs
+        **kwargs,
     )
 
     if axis == "x":
         labels_ax = ax.get_xticklabels()
     elif axis == "y":
         labels_ax = ax.get_yticklabels()
+    else:
+        raise ValueError("axis value {0} is not available".format(axis))
 
     if len(labels) == 0:
         labels = [l.get_text() for l in labels_ax]
     elif len(labels) < len(labels_ax):
         for i in range(0, len(labels_ax) - len(labels)):
             labels.append(None)
 
     if len(bgcolors) > 0:
         bbox = dict(boxstyle="square", alpha=0.3)
         for i, c in enumerate(bgcolors):
             labels_ax[i].set_bbox(bbox)
             labels_ax[i].set_backgroundcolor(c)
 
+    if isinstance(d["colors"], list):
+        colors = d["colors"]
+    else:
+        colors = _axTools.getColorList(len(labels), d["colors"])
+
+    va_text = d["va"]
+    ha_text = d["ha"]
+
     if axis == "both":
         if visible == False:
             ax.axes.xaxis.set_visible(False)
             ax.axes.yaxis.set_visible(False)
             return
     else:
         if axis == "x":
             if visible == False:
                 ax.axes.xaxis.set_visible(False)
                 return
             else:
                 ax.axes.xaxis.set_visible(True)
+                ax.set_xticklabels(
+                    labels,
+                    rotation=labelrotation,
+                    ha=ha_text,
+                    va=va_text,
+                    weight=d["fontweight"],
+                )
 
         if axis == "y":
             if visible == False:
                 ax.axes.yaxis.set_visible(False)
                 return
             else:
                 ax.axes.yaxis.set_visible(True)
-
+                ax.set_yticklabels(
+                    labels,
+                    rotation=labelrotation,
+                    ha=ha_text,
+                    va=va_text,
+                    weight=d["fontweight"],
+                )
     # NO DIRECTION
     if loc is None:
         if axis == "x":
-            va_text = kwargs.get("va", "top")
-            ha_text = kwargs.get("ha", "center")
             ax.set_xticks(ax.get_xticks())
-            ax.set_xticklabels(
-                labels,
-                rotation=labelrotation,
-                ha=ha_text,
-                va=va_text,
-                weight=d["fontweight"],
-            )
+            for color, tick in zip(colors, ax.xaxis.get_major_ticks()):
+                tick.label1.set_color(color)
+
         if axis == "y":
-            va_text = "center"
-            ha_text = "right"
             ax.set_yticks(ax.get_yticks())
-            ax.set_yticklabels(
-                labels,
-                rotation=labelrotation,
-                ha=ha_text,
-                va=va_text,
-                weight=d["fontweight"],
-            )
-    else:
-        if isinstance(d["colors"], list):
-            colors = d["colors"]
-        else:
-            colors = _axTools.getColorList(len(labels), d["color"])
+            for color, tick in zip(colors, ax.yaxis.get_major_ticks()):
+                tick.label1.set_color(color)
 
+    else:
         if len(colors) < len(labels):
             _aux_ = _axTools.getColorList((len(labels) - len(colors)), d["color"])
             colors.extend(_aux_)
-        ha_text = "center"
-        va_text = "center_baseline"
 
         def get_data():
             data = _axTools.values_bars(ax)
             mask = data["value"] >= limit
             data.loc[mask, "value"] = 0
             return data
 
         values_iterables = None
 
-        if orient == "v":
-            if axis == "y":
-                if loc == "right":
-                    ax.yaxis.set_ticks_position("right")
-                    ax.yaxis.set_label_position("right")
-                elif loc == "left":
-                    ax.yaxis.set_ticks_position("left")
-                    ax.yaxis.set_label_position("left")
-
-            elif axis == "x":
-                if loc in ["left", "right"]:
-                    pass
-                elif loc == "top":
-                    ax.xaxis.set_ticks_position("top")
-                    ax.xaxis.set_label_position("top")
-                else:
-                    data = get_data()
-                    if loc == "in":
-                        posY = data["value"] / 2
-                    elif loc == "out":
-                        posY = data["value"]
+        if loc in ["bottom", "in", "on"]:
+            data = get_data()
+            posY = data["value"]
+
+            if axis == "x":
+                posX = [x.get_position()[0] for x in labels_ax]
+            else:
+                posX = [x.get_position()[1] for x in labels_ax]
+
+            if loc == "bottom":
+                if len(labels) != len(posY):
+                    posY = [0] * data.shape[0]
+
+            else:
+                if loc in ["in", "on"]:
+                    if axis == "x":
+                        posX = data["x"]
                     else:
-                        posY = [0] * data.shape[0]
-                    posX = data["x"]
-                    ax.set_xticklabels([])
-                    values_iterables = zip(labels, posX, posY + d["ypad"], colors)
+                        posX = data["y"]
+
+                    if loc == "in":
+                        posY = [x / 2 for x in posY]
+
+                    if len(labels) != len(posY):
+                        factor = int(len(posY) / len(labels))
+                        labels = labels * factor
+                        colors = colors * factor
 
-        elif orient == "h":
             if axis == "x":
-                if loc == "top":
-                    ax.xaxis.set_ticks_position("top")
-                    ax.xaxis.set_label_position("top")
-                else:
-                    pass
+                ax.set_xticklabels([])
+                values_iterables = zip(labels, posX, posY, colors)
             elif axis == "y":
-                if loc in ["right", "top"]:
-                    ax.yaxis.set_ticks_position("right")
-                    ax.yaxis.set_label_position("right")
-                elif loc == "left":
-                    ax.yaxis.set_ticks_position("left")
-                    ax.yaxis.set_label_position("left")
-                else:
-                    data = get_data()
-                    if loc == "in":
-                        posY = data["value"] / 2
-                    elif loc == "out":
-                        posY = data["value"]
+                ax.set_yticklabels([])
+                values_iterables = zip(labels, posY, posX, colors)
+
+        else:
+            if orient == "v":
+                if axis == "y":
+                    if loc == "right":
+                        ax.yaxis.set_ticks_position("right")
+                        ax.yaxis.set_label_position("right")
+                    elif loc == "left":
+                        ax.yaxis.set_ticks_position("left")
+                        ax.yaxis.set_label_position("left")
+                    elif loc == "top":
+                        print(
+                            "Loc '{0}' is not available in axis {1}".format(loc, axis)
+                        )
+
+                elif axis == "x":
+                    if loc in ["left", "right"]:
+                        print(
+                            "Loc '{0}' is not available in axis {1}".format(loc, axis)
+                        )
+                    elif loc == "top":
+                        ax.xaxis.set_ticks_position("top")
+                        ax.xaxis.set_label_position("top")
+
+            elif orient == "h":
+                if axis == "x":
+                    if loc == "top":
+                        ax.xaxis.set_ticks_position("top")
+                        ax.xaxis.set_label_position("top")
                     else:
-                        posY = [0] * data.shape[0]
-                    posX = data["y"]
-                    ax.set_yticklabels([])
-                    values_iterables = zip(labels, posY, posX + d["xpad"], colors)
+                        print(
+                            "Loc '{0}' is not available in axis {1}".format(loc, axis)
+                        )
+                elif axis == "y":
+                    if loc in ["right", "top"]:
+                        ax.yaxis.set_ticks_position("right")
+                        ax.yaxis.set_label_position("right")
+                    elif loc == "left":
+                        ax.yaxis.set_ticks_position("left")
+                        ax.yaxis.set_label_position("left")
 
         if not values_iterables is None:
             effects = [
                 path_effects.Stroke(
                     linewidth=d["shadow"],
                     foreground=d["shadowcolor"],
                     alpha=0.8,
                 ),
                 path_effects.Normal(),
             ]
 
             for name, x_pos, y_pos, c in values_iterables:
                 if orient == "h":
-                    PADT = -d["xpad"] if x_pos < 0 else d["xpad"]
+                    PADT = -1 * d["xpad"] if x_pos < 0 else d["xpad"]
                     if x_pos >= 0:
                         ha_text = "left"
                     elif x_pos < 0:
                         ha_text = "right"
                     x_pos = x_pos + PADT
+                    y_pos = y_pos + d["ypad"]
                 else:
-                    PADT = -d["ypad"] if y_pos < 0 else d["ypad"]
+                    PADT = -1 * d["ypad"] if y_pos < 0 else d["ypad"]
                     if x_pos >= 0:
                         va_text = "bottom"
                     elif x_pos < 0:
                         va_text = "top"
                     y_pos = y_pos + PADT
+                    x_pos = x_pos + d["xpad"]
 
                 t = ax.text(
-                    x_pos + d["xpad"],
-                    y_pos + d["ypad"],
+                    x_pos,
+                    y_pos,
                     name,
                     va=va_text,
                     rotation=labelrotation,
                     color=c,
                     fontsize=d["fontsize"],
                     ha=ha_text,
                     weight=d["fontweight"],
@@ -458,15 +495,15 @@
     loc=0,
     title_fontsize=None,
     title_loc: str = "left",
     label_fontsize=None,
     labels: list() = None,
     handles: list() = None,
     borderpad=0.82,
-    **kwargs
+    **kwargs,
 ) -> _plt.Axes.legend:
     legend = None
 
     if type(loc) is tuple:
         bbox_to_anchor = loc
         loc = 0
     else:
@@ -535,15 +572,15 @@
         prop=propF,
         labels=labels,
         loc=loc,
         title_fontsize=title_fontsize,
         borderpad=borderpad,
         ncol=ncols,
         bbox_to_anchor=bbox_to_anchor,
-        **kwargs
+        **kwargs,
     )
 
     if not title_loc in ["left", "right", "center"]:
         title_loc = "left"
     legend._legend_box.align = title_loc
     legend.get_title().set_position((0, 5))
 
@@ -567,29 +604,32 @@
         return data
 
 
 def show_values(
     ax=None,
     dec: int = 1,
     minvalue: int = -_np.Infinity,
+    maxvalue: int = _np.Infinity,
     loc: str = "top",
-    ha: str = "auto",
-    va: str = "auto",
     kind: str = "bar",
     normBy: str = "c",
     display: str = "v",
     prefix: str = "",
     postfix: str = "",
     stack=False,
-    **kwargs
+    **kwargs,
 ) -> _plt.Axes:
     ax = _axTools.gca(ax)
     orient = "v"
+
     d, kwargs = _axTools.get_init_kwargs(
-        kwargs, remove_kwargs=False, inplace_kwargs=True
+        kwargs,
+        remove_kwargs=False,
+        inplace_kwargs=True,
+        defaults={"va": "auto", "ha": "auto"},
     )
 
     if dec == None:
         dec = 2 if display != "v" else 1
 
     if kind not in ["bar", "line", "point"]:
         raise ValueError("kind is not in bar, line or point")
@@ -639,54 +679,55 @@
             data["y"] = [y + d["ypad"] if y >= 0 else y - d["ypad"] for y in data["y"]]
 
     # Print values on plot
     _axTools.plot_values(
         ax=ax,
         data=data,
         minvalue=minvalue,
+        maxvalue=maxvalue,
         dec=dec,
-        ha=ha,
-        va=va,
         display=display,
         prefix=prefix,
         postfix=postfix,
         orient=orient,
-        **kwargs
+        **kwargs,
     )
 
 
 def set_values(
     ax=None,
+    values=list(),
     dec: int = 1,
     minvalue: int = -_np.Infinity,
+    maxvalue: int = _np.Infinity,
     loc: str = "top",
-    values=list(),
-    ha: str = "auto",
-    va: str = "auto",
     kind: str = "bar",
-    xpad: float = 0,
-    ypad: float = 0,
     display: str = "v",
     stack=False,
-    **kwargs
+    **kwargs,
 ):
     orient = "v"
 
     ax = _axTools.gca(ax)
+    d, _ = _axTools.get_init_kwargs(
+        kwargs=kwargs, remove_kwargs=False, inplace_kwargs=True
+    )
 
     if values is not None or not isinstance(values, (list)):
         if kind == "bar":
             data = _axTools.values_bars(ax=ax, normBy="c", loc=loc, stack=stack)
             orient, _ = _axTools.orient(ax)
         elif kind == "line":
             data = _axTools.values_line(ax=ax, orient=orient)
         elif kind == "point":
             data = _axTools.values_points(ax=ax)
 
-            # Add spacing for the data
+        # Add spacing for the data
+        xpad = d["xpad"]
+        ypad = d["ypad"]
         if kind != "line":
             if xpad != 0:
                 data["x"] = [x + xpad if x >= 0 else x - xpad for x in data["x"]]
             if ypad != 0:
                 data["y"] = [y + ypad if y >= 0 else y - ypad for y in data["y"]]
 
         if data.shape[0] >= len(values):
@@ -695,20 +736,19 @@
             n_items = data.shape[0]
         data["value"] = values[:n_items]
 
         _axTools.plot_values(
             ax=ax,
             data=data,
             minvalue=minvalue,
+            maxvalue=maxvalue,
             dec=dec,
-            ha=ha,
-            va=va,
             display=display,
             orient=orient,
-            **kwargs
+            **kwargs,
         )
 
     else:
         raise ValueError("`Values` data type is invalid")
 
 
 def set_figsize(figsize):
```

### Comparing `seawolf-0.1/seawolf/_colors.py` & `seawolf-0.1.1/seawolf/_colors.py`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/seawolf/_style.py` & `seawolf-0.1.1/seawolf/_style.py`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/seawolf/test.py` & `seawolf-0.1.1/seawolf/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,38 +14,38 @@
 url = "https://raw.github.com/mattdelhey/kaggle-titanic/master/Data/train.csv"
 titanic = pd.read_csv(url)
 # print(titanic.columns)
 
 sw.style.set(figsize=(8, 6))
 
 ax = sns.countplot(data=titanic, y="pclass", hue='sex')
-start = time.time()
-sw.show_values(
-    ax=ax, dec=0, color="black", fontweight="bold", loc="top", minvalue=3
+sw.show_values( minvalue=100, maxvalue=200,
+    ax=ax, dec=0, color="black", fontweight="bold", loc="top"
 )
+# sw.set_values(dec=1, values=[1,2,3,4,5,6], color='red')
 sw.set_legend(
     title="Sexo",
     ncols=1,
     labels=["Hombre", "Mujer"],
     label_fontsize=8,
     title_fontsize=10,
     title_loc="center",
     borderpad=1.22,
 )
 sw.set_title(title="Tabla 3", fontweight="bold")
 sw.set_subtitle(title="Conteo de sobrevivientes")
 sw.set_tickslabel(
     axis="y",
     labelrotation=0,
-    loc="bottom",
-    xpad=10,
-    color="white",
-    # colors = ['#c1c1c1', 'white', 'white'],
+    loc='in',
+    xpad=0,
+    ypad=0,
+    color="blue",
+    # colors = ['white', 'red', 'white'],
     shadow=0.5,
-    shadowcolor="white",
-    labels=["Baja", "Media", "Alta", "Baja", "Media", "Alta"],
+    shadowcolor="black",
+    labels=["Baja", "Media", "Alta"],
 )
 sw.theme(op='spine', left=True, bottom=True, spine_butt='left')
 ax.xaxis.grid(True)
 ax.set_axisbelow(True)
-print(time.time() - start)
-plt.show()
+plt.show()
```

### Comparing `seawolf-0.1/seawolf/fonts/CAMBRIAI.TTF` & `seawolf-0.1.1/seawolf/fonts/CAMBRIAI.TTF`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/seawolf/fonts/CAMBRIAZ.TTF` & `seawolf-0.1.1/seawolf/fonts/CAMBRIAZ.TTF`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/seawolf/fonts/Cambria.ttf` & `seawolf-0.1.1/seawolf/fonts/Cambria.ttf`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/seawolf/fonts/cambriab.ttf` & `seawolf-0.1.1/seawolf/fonts/cambriab.ttf`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/.gitignore` & `seawolf-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/LICENSE` & `seawolf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seawolf-0.1/pyproject.toml` & `seawolf-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "seawolf"
-version = "0.1"
+version = "0.1.1"
 authors = [
     { name="Bayron Torres Gordillo", email="torres.bayron@gmail.com" },
 ]
 description = "It is a library for the ease of plotting styles generated with matplotlib. Allows you to save time when giving the final style to the plots"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `seawolf-0.1/PKG-INFO` & `seawolf-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seawolf
-Version: 0.1
+Version: 0.1.1
 Summary: It is a library for the ease of plotting styles generated with matplotlib. Allows you to save time when giving the final style to the plots
 Project-URL: Homepage, https://github.com/bayrtxxx84/seawolf
 Project-URL: Bug Tracker, https://github.com/bayrtxxx84/seawolf/issues
 Author-email: Bayron Torres Gordillo <torres.bayron@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

