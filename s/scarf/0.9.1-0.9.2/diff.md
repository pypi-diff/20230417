# Comparing `tmp/scarf-0.9.1.tar.gz` & `tmp/scarf-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarf-0.9.1.tar", last modified: Tue Jul 13 12:26:52 2021, max compression
+gzip compressed data, was "scarf-0.9.2.tar", last modified: Sun Jul 18 15:52:35 2021, max compression
```

## Comparing `scarf-0.9.1.tar` & `scarf-0.9.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-13 12:26:52.163096 scarf-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-07-13 12:26:42.000000 scarf-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-07-13 12:26:42.000000 scarf-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-07-13 12:26:52.163096 scarf-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      952 2021-07-13 12:26:42.000000 scarf-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-07-13 12:26:42.000000 scarf-0.9.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-13 12:26:52.163096 scarf-0.9.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)   159264 2021-07-13 12:26:42.000000 scarf-0.9.1/bin/sgtsne
--rw-r--r--   0 runner    (1001) docker     (121)      190 2021-07-13 12:26:42.000000 scarf-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-07-13 12:26:42.000000 scarf-0.9.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-13 12:26:52.163096 scarf-0.9.1/scarf/
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10697 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/ann.py
--rw-r--r--   0 runner    (1001) docker     (121)    24490 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/assay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/bio_data.py
--rw-r--r--   0 runner    (1001) docker     (121)   192587 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/datastore.py
--rw-r--r--   0 runner    (1001) docker     (121)    10058 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     6283 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/feat_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4701 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/knn_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5693 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/mapping_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/markers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6339 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/meld_assay.py
--rw-r--r--   0 runner    (1001) docker     (121)    14514 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    25874 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    37987 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/readers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/umap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    40668 2021-07-13 12:26:42.000000 scarf-0.9.1/scarf/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-13 12:26:52.163096 scarf-0.9.1/scarf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-07-13 12:26:52.000000 scarf-0.9.1/scarf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-07-13 12:26:52.000000 scarf-0.9.1/scarf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-07-13 12:26:52.000000 scarf-0.9.1/scarf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-07-13 12:26:52.000000 scarf-0.9.1/scarf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-07-13 12:26:52.000000 scarf-0.9.1/scarf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-13 12:26:52.163096 scarf-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2021-07-13 12:26:42.000000 scarf-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-18 15:52:35.687398 scarf-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-07-18 15:52:25.000000 scarf-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-07-18 15:52:25.000000 scarf-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1719 2021-07-18 15:52:35.683398 scarf-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-07-18 15:52:25.000000 scarf-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-07-18 15:52:25.000000 scarf-0.9.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-18 15:52:35.683398 scarf-0.9.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)   159264 2021-07-18 15:52:25.000000 scarf-0.9.2/bin/sgtsne
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2021-07-18 15:52:25.000000 scarf-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2021-07-18 15:52:25.000000 scarf-0.9.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-18 15:52:35.683398 scarf-0.9.2/scarf/
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10697 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/ann.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24490 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/assay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/bio_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)   193016 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10055 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6283 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2981 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/feat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4701 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/knn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5693 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/mapping_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/markers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6339 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/meld_assay.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14514 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25973 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/plots.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38050 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/readers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3583 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/umap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40556 2021-07-18 15:52:25.000000 scarf-0.9.2/scarf/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-18 15:52:35.683398 scarf-0.9.2/scarf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1719 2021-07-18 15:52:35.000000 scarf-0.9.2/scarf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2021-07-18 15:52:35.000000 scarf-0.9.2/scarf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-07-18 15:52:35.000000 scarf-0.9.2/scarf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2021-07-18 15:52:35.000000 scarf-0.9.2/scarf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-07-18 15:52:35.000000 scarf-0.9.2/scarf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-18 15:52:35.687398 scarf-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2166 2021-07-18 15:52:25.000000 scarf-0.9.2/setup.py
```

### Comparing `scarf-0.9.1/LICENSE` & `scarf-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/bin/sgtsne` & `scarf-0.9.2/bin/sgtsne`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/__init__.py` & `scarf-0.9.2/scarf/__init__.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/ann.py` & `scarf-0.9.2/scarf/ann.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/assay.py` & `scarf-0.9.2/scarf/assay.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/bio_data.py` & `scarf-0.9.2/scarf/bio_data.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/datastore.py` & `scarf-0.9.2/scarf/datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
             res += '\n' + dtabs + ''.join([f"'{x}', " if n % 5 != 0 else f"'{x}', \n{dtabs}" for n, x in
                                            enumerate(assay.feats.columns, start=1)])
             res = res.rstrip('\n\t')[:-2]
             if 'projections' in self.z[i]:
                 targets = []
                 layouts = []
                 for j in self.z[i]['projections']:
-                    if 'indices' in self.z[i]['projections'][j]:
+                    if type(self.z[i]['projections'][j]) == zarr.Group:
                         targets.append(j)
                     else:
                         layouts.append(j)
                 if len(targets) > 0:
                     res += f"\n{stabs}Projected samples:"
                     res += '\n' + dtabs + ''.join([f"'{x}', " if n % 5 != 0 else f"'{x}', \n{dtabs}" for n, x in
                                                    enumerate(targets, start=1)])
@@ -2128,15 +2128,16 @@
                             mask_color: str = 'k', point_size: float = 10, ax_label_size: float = 12,
                             frame_offset: float = 0.05, spine_width: float = 0.5, spine_color: str = 'k',
                             displayed_sides: tuple = ('bottom', 'left'),
                             legend_ondata: bool = False, legend_onside: bool = True, legend_size: float = 12,
                             legends_per_col: int = 20, cbar_shrink: float = 0.6, marker_scale: float = 70,
                             lspacing: float = 0.1, cspacing: float = 1, savename: str = None, save_dpi: int = 300,
                             ax=None, force_ints_as_cats: bool = True, n_columns: int = 1, w_pad: float = 1,
-                            h_pad: float = 1, scatter_kwargs: dict = None, shuffle_zorder: bool = True):
+                            h_pad: float = 1, scatter_kwargs: dict = None, shuffle_zorder: bool = True,
+                            show_fig: bool = True):
         """
         Plots the reference and target cells in their unified space.
 
         This function helps plotting the reference and target cells the coordinates for which were obtained from
         either `run_unified_tsne` or `run_unified_umap`. Since the coordinates are not saved in the cell metadata
         but rather in the projections slot of the Zarr hierarchy, this function is needed to correctly fetch the values
         for reference and target cells. Additionally this function provides a way to colour target cells by bringing in
@@ -2192,14 +2193,15 @@
                    If None is provided the padding will be automatically added to avoid overlap.
                    Ignored if only plotting one scatterplot.
             h_pad: When plotting in multiple plots in a grid this decides the height padding between the plots.
                    If None is provided the padding will be automatically added to avoid overlap.
                    Ignored if only plotting one scatterplot.
             scatter_kwargs: Keyword argument to be passed to matplotlib's scatter command
             shuffle_zorder: Whether to shuffle the plot order of data points in the figure. (Default value: True)
+            show_fig: Whether to render the figure and display it using plt.show() (Default value: True)
 
         Returns:
             None
         """
 
         from .plots import plot_scatter
 
@@ -2260,15 +2262,15 @@
         if shuffle_zorder:
             df = df.sample(frac=1)
         return plot_scatter([df], ax, width, height, mask_color, cmap, color_key,
                             mask_values, mask_name, mask_color, point_size,
                             ax_label_size, frame_offset, spine_width, spine_color, displayed_sides,
                             legend_ondata, legend_onside, legend_size, legends_per_col, cbar_shrink, marker_scale,
                             lspacing, cspacing, savename, save_dpi, force_ints_as_cats, n_columns, w_pad, h_pad,
-                            scatter_kwargs)
+                            show_fig, scatter_kwargs)
 
 
 # Note for the docstring: Attributes are copied from BaseDataStore docstring since the constructor is inherited.
 # Meaning, for any attribute change in BaseDataStore a manual update to docstring here is needed as well. - RO
 class DataStore(MappingDatastore):
     """
     This class extends MappingDatastore and consequently inherits methods of all the other DataStore classes.
@@ -2767,15 +2769,15 @@
         else:
             print(self.z[start].tree(expand=True, level=depth))
 
     def plot_cells_dists(self, from_assay: str = None, cols: List[str] = None, cell_key: str = None,
                          group_key: str = None, color: str = 'steelblue', cmap: str = 'tab20',
                          fig_size: tuple = None, label_size: float = 10.0, title_size: float = 10.0,
                          sup_title: str = None, sup_title_size: float = 12.0, scatter_size: float = 1.0,
-                         max_points: int = 10000, show_on_single_row: bool = True) -> None:
+                         max_points: int = 10000, show_on_single_row: bool = True, show_fig: bool = True) -> None:
         """
         Makes violin plots of the distribution of values present in cell metadata. This method is designed to
         distribution of nCounts, nFeatures, percentMito and percentRibo cell attrbutes.
 
         Args:
             from_assay: Name of assay to be used. If no value is provided then the default assay will be used.
             cols: Column names from cell metadata table to be used for plotting. Be default, nCounts, nFeatures,
@@ -2796,14 +2798,15 @@
             sup_title_size: The font size of title for complete figure panel (Default value: 12.0 )
             scatter_size: Size of each point in the violin plot (Default value: 1.0)
             max_points: Maximum number of points to display over violin plot. Random uniform sampling will be performed
                         to bring down the number of datapoints to this value. This does not effect the violin plot.
                         (Default value: 10000)
             show_on_single_row: Show all subplots in a single row. It might be useful to set this to False if you have
                                 too many groups within each subplot (Default value: True)
+            show_fig: Whether to render the figure and display it using plt.show() (Default value: True)
 
         Returns:
             None
 
         """
 
         from .plots import plot_qc
@@ -2839,32 +2842,33 @@
             df['groups'] = np.zeros(len(df))
         if cell_key is not None:
             idx = self.cells.active_index(cell_key)
             df = df.reindex(idx)
 
         plot_qc(df, color=color, cmap=cmap, fig_size=fig_size, label_size=label_size, title_size=title_size,
                 sup_title=sup_title, sup_title_size=sup_title_size, scatter_size=scatter_size,
-                max_points=max_points, show_on_single_row=show_on_single_row)
+                max_points=max_points, show_on_single_row=show_on_single_row, show_fig=show_fig)
         return None
 
     def plot_layout(self, *, from_assay: str = None, cell_key: str = None,
                     layout_key: str = None, color_by: str = None, subselection_key: str = None,
                     size_vals=None, clip_fraction: float = 0.01,
                     width: float = 6, height: float = 6, default_color: str = 'steelblue',
                     cmap=None, color_key: dict = None, mask_values: list = None,
                     mask_name: str = 'NA', mask_color: str = 'k', point_size: float = 10,
-                    do_shading: bool = False, shade_npixels: int = 1000, shade_sampling: float = 0.1,
-                    shade_min_alpha: int = 10, spread_pixels: int = 1, spread_threshold: float = 0.2,
+                    do_shading: bool = False, shade_npixels: int = 1000, shade_min_alpha: int = 10,
+                    spread_pixels: int = 1, spread_threshold: float = 0.2,
                     ax_label_size: float = 12, frame_offset: float = 0.05, spine_width: float = 0.5,
                     spine_color: str = 'k', displayed_sides: tuple = ('bottom', 'left'),
                     legend_ondata: bool = True, legend_onside: bool = True, legend_size: float = 12,
                     legends_per_col: int = 20,  cbar_shrink: float = 0.6, marker_scale: float = 70,
                     lspacing: float = 0.1, cspacing: float = 1, shuffle_df: bool = False, sort_values: bool = False,
                     savename: str = None, save_dpi: int = 300, ax=None, force_ints_as_cats: bool = True,
-                    n_columns: int = 4, w_pad: float = 1, h_pad: float = 1, scatter_kwargs: dict = None):
+                    n_columns: int = 4, w_pad: float = 1, h_pad: float = 1, show_fig: bool = True,
+                    scatter_kwargs: dict = None):
         """
         Create a scatter plot with a chosen layout. The methods fetches the coordinates based from
         the cell metadata columns with `layout_key` prefix. DataShader library is used to draw fast
         rasterized image is `do_shading` is True. This can be useful when large number of cells are
         present to quickly render the plot and avoid over-plotting.
         The description of shading parameters has mostly been copied from the Datashader API that can be found here:
         https://holoviews.org/_modules/holoviews/operation/datashader.html
@@ -2905,16 +2909,14 @@
             do_shading: Sets shading mode on/off. If shading mode is off (default) then matplotlib's scatter function is
                         is used otherwise a rasterized image is generated using datashader library. Turn this on if you
                         have more than 100K cells to improve render time and also to avoid issues with overplotting.
                         (Default value: False)
             shade_npixels: Number of pixels to rasterize (for both height and width). This controls the resolution of
                            the figure. Adjust this according to the size of the image you want to generate.
                            (Default value: 1000)
-            shade_sampling: Specifies the smallest allowed sampling interval along the x and y axis. Larger values will
-                            lead loss of resolution (Default value: 0.1)
             shade_min_alpha: The minimum alpha value to use for non-empty pixels when doing colormapping, in [0, 255].
                              Use a higher value to avoid undersaturation, i.e. poorly visible low-value datapoints, at
                              the expense of the overall dynamic range. (Default value: 10)
             spread_pixels: Maximum number of pixels to spread on all sides (Default value: 1)
             spread_threshold:  When spreading, determines how far to spread. Spreading starts at 1 pixel, and stops
                                when the fraction of adjacent non-empty pixels reaches this threshold. Higher values
                                give more spreading, up to the `spread_pixels` allowed. (Default value: 0.2)
@@ -2953,15 +2955,16 @@
                        grid. Defaults to 4 but if the total amount of plots are less than 4 it will default to that
                        number.
             w_pad: When plotting in multiple plots in a grid this decides the width padding between the plots. 
                    If None is provided the padding will be automatically added to avoid overlap.
                    Ignored if only plotting one scatterplot. 
             h_pad: When plotting in multiple plots in a grid this decides the height padding between the plots. 
                    If None is provided the padding will be automatically added to avoid overlap.
-                   Ignored if only plotting one scatterplot. 
+                   Ignored if only plotting one scatterplot.
+            show_fig: Whether to render the figure and display it using plt.show() (Default value: True)
             scatter_kwargs: Keyword argument to be passed to matplotlib's scatter command
 
         Returns:
             None
 
         """
 
@@ -3016,26 +3019,27 @@
                     df = df.sort_values(by=c)
                 dfs.append(df)
 
         if n_columns > len(dfs):
             n_columns = len(dfs)
 
         if do_shading:
-            return shade_scatter(dfs, ax, width, shade_npixels, shade_sampling, spread_pixels, spread_threshold,
+            return shade_scatter(dfs, ax, width, shade_npixels, spread_pixels, spread_threshold,
                                  shade_min_alpha, cmap, color_key, mask_values, mask_name, mask_color,
                                  ax_label_size, frame_offset, spine_width, spine_color, displayed_sides,
                                  legend_ondata, legend_onside, legend_size, legends_per_col, cbar_shrink, marker_scale,
-                                 lspacing, cspacing, savename, save_dpi, force_ints_as_cats, n_columns, w_pad, h_pad)
+                                 lspacing, cspacing, savename, save_dpi, force_ints_as_cats, n_columns, w_pad, h_pad,
+                                 show_fig)
         else:
             return plot_scatter(dfs, ax, width, height, default_color, cmap, color_key,
                                 mask_values, mask_name, mask_color, point_size,
                                 ax_label_size, frame_offset, spine_width, spine_color, displayed_sides,
                                 legend_ondata, legend_onside, legend_size, legends_per_col, cbar_shrink,  marker_scale,
                                 lspacing, cspacing, savename, save_dpi, force_ints_as_cats, n_columns, w_pad, h_pad,
-                                scatter_kwargs)
+                                show_fig, scatter_kwargs)
 
     def plot_cluster_tree(self, *, from_assay: str = None, cell_key: str = None, feat_key: str = None,
                           cluster_key: str = None, fill_by_value: str = None, force_ints_as_cats: bool = True,
                           width: float = 1, lvr_factor: float = 0.5, vert_gap: float = 0.2,
                           min_node_size: float = 10, node_size_multiplier: float = 1e4, node_power: float = 1.2,
                           root_size: float = 100, non_leaf_size: float = 10,
                           show_labels: bool = True, fontsize: float = 10,
@@ -3150,15 +3154,15 @@
                                root_color=root_color, non_leaf_color=non_leaf_color, cmap=cmap,
                                color_key=color_key, edgecolors=edgecolors,
                                edgewidth=edgewidth, alpha=alpha, figsize=figsize, ax=ax, show_fig=show_fig,
                                savename=savename, save_dpi=save_dpi)
 
     def plot_marker_heatmap(self, *, from_assay: str = None, group_key: str = None, cell_key: str = None,
                             topn: int = 5, log_transform: bool = True, vmin: float = -1, vmax: float = 2,
-                            savename: str = None, save_dpi: int = 300, **heatmap_kwargs):
+                            savename: str = None, save_dpi: int = 300, show_fig: bool = True, **heatmap_kwargs):
         """
         Displays a heatmap of top marker gene expression for the chosen groups (usually cell clusters).
 
         Z-scores are calculated for each marker gene before plotting them. The groups are subjected to hierarchical
         clustering to bring groups with similar expression pattern in proximity.
 
         Args:
@@ -3173,14 +3177,15 @@
             log_transform: Whether to log-transform the values before displaying them in the heatmap.
                            (Default value: True)
             vmin: z-scores lower than this value are ceiled to this value. (Default value: -1)
             vmax: z-scores higher than this value are floored to this value. (Default value: 2)
             savename: Path where the rendered figure is to be saved. The format of the saved image depends on the
                       the extension present in the parameter value. (Default value: None)
             save_dpi: DPI when saving figure. (Default value: 300)
+            show_fig: Whether to render the figure and display it using plt.show() (Default value: True)
             **heatmap_kwargs: Keyword arguments to be forwarded to seaborn.clustermap.
 
         Returns:
             None
         """
         from .plots import plot_heatmap
 
@@ -3215,8 +3220,8 @@
         df = df.T
         df.index = assay.feats.to_pandas_dataframe(['ids', 'names']).set_index(
             'ids').reindex(df.index)['names'].values
         # noinspection PyTypeChecker
         df[df < vmin] = vmin
         # noinspection PyTypeChecker
         df[df > vmax] = vmax
-        plot_heatmap(df, savename=savename, save_dpi=save_dpi, **heatmap_kwargs)
+        plot_heatmap(df, savename=savename, save_dpi=save_dpi, show_fig=show_fig, **heatmap_kwargs)
```

### Comparing `scarf-0.9.1/scarf/dendrogram.py` & `scarf-0.9.2/scarf/dendrogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         while len(q) > 0:
             i = q.pop(0)
             if self.graph.nodes[i]['nleaves'] > min_leaves:
                 d.append(i)
                 q.extend(list(self.graph.successors(i)))
         return d[1:]
 
-    def _get_mean_dist(self, start_node: int) -> np.float:
+    def _get_mean_dist(self, start_node: int) -> float:
         """
         Get mean distances in downstream tree of a node
         """
         s_nodes = self._successors(start_node, -1)
         return np.array([self.graph.nodes[x]['dist'] for x in s_nodes]).mean()
 
     def _are_subtrees_mergeable(self, s1: int, s2: int) -> bool:
```

### Comparing `scarf-0.9.1/scarf/downloader.py` & `scarf-0.9.2/scarf/downloader.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/feat_utils.py` & `scarf-0.9.2/scarf/feat_utils.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/knn_utils.py` & `scarf-0.9.2/scarf/knn_utils.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/mapping_utils.py` & `scarf-0.9.2/scarf/mapping_utils.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/markers.py` & `scarf-0.9.2/scarf/markers.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/meld_assay.py` & `scarf-0.9.2/scarf/meld_assay.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/metadata.py` & `scarf-0.9.2/scarf/metadata.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/plots.py` & `scarf-0.9.2/scarf/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     plt.tight_layout()
     plt.show()
 
 
 def plot_qc(data: pd.DataFrame, color: str = 'steelblue', cmap: str = 'tab20',
             fig_size: tuple = None, label_size: float = 10.0, title_size: float = 10,
             sup_title: str = None, sup_title_size: float = 12, scatter_size: float = 1.0,
-            max_points: int = 10000, show_on_single_row: bool = True):
+            max_points: int = 10000, show_on_single_row: bool = True, show_fig: bool = True):
     # TODO: add docstring description. Is this for qc of a plot, or for plotting a qc plot?
     n_plots = data.shape[1] - 1
     n_groups = data['groups'].nunique()
     if n_groups > 5 and show_on_single_row is True:
         logger.info(f"Too many groups in the plot. If you think that plot is too wide then consider turning "
                     f"`show_on_single_row` parameter to False")
     if show_on_single_row is True:
@@ -139,21 +139,27 @@
                           s=scatter_size, color='k', alpha=0.4)
         else:
             sns.stripplot(x='g', y='v', data=vals, jitter=0.4, ax=ax, orient='v',
                           s=scatter_size, color='k', alpha=0.4)
         ax.set_ylabel(data.columns[i], fontsize=label_size)
         ax.set_xlabel('')
         if n_groups == 1:
+            ax.set_xticks([])
             ax.set_xticklabels([])
         if data['groups'].nunique() == 1:
             ax.set_title('Median: %.1f' % (int(np.median(vals['v']))), fontsize=title_size)
-        clean_axis(ax)
+        # clean_axis(ax)
+        ax.figure.patch.set_alpha(0)
+        ax.patch.set_alpha(0)
     fig.suptitle(sup_title, fontsize=sup_title_size)
     plt.tight_layout()
-    plt.show()
+    if show_fig:
+        plt.show()
+    else:
+        return fig
 
 
 def plot_mean_var(nzm: np.ndarray, fv: np.ndarray, n_cells: np.ndarray, hvg: np.ndarray,
                   ax_label_fs: float = 12, fig_size: Tuple[float, float] = (4.5, 4.0),
                   ss: Tuple[float, float] = (3, 30), cmaps: Tuple[str, str] = ('winter', 'magma_r')):
     """
     Shows a mean-variance plot.
@@ -186,30 +192,32 @@
     clean_axis(ax, ts=8)
     ax.legend(frameon=False, fontsize=9)
     plt.tight_layout()
     plt.show()
 
 
 def plot_heatmap(cdf, fontsize: float = 10, width_factor: float = 0.03, height_factor: float = 0.02,
-                 cmap=cm.matter_r, savename: str = None, save_dpi: int = 300, figsize=None):
+                 cmap=cm.matter_r, savename: str = None, save_dpi: int = 300, figsize=None, show_fig: bool = True):
     """
     Shows a heatmap plot.
     """
     if figsize is None:
         figsize = (cdf.shape[1] * fontsize * width_factor, fontsize * cdf.shape[0] * height_factor)
     cgx = sns.clustermap(cdf, yticklabels=cdf.index, xticklabels=cdf.columns, method='ward',
                          figsize=figsize, cmap=cmap, rasterized=True)
     cgx.ax_heatmap.set_yticklabels(cdf.index[cgx.dendrogram_row.reordered_ind], fontsize=fontsize)
     cgx.ax_heatmap.set_xticklabels(cdf.columns[cgx.dendrogram_col.reordered_ind], fontsize=fontsize)
     cgx.ax_heatmap.figure.patch.set_alpha(0)
     cgx.ax_heatmap.patch.set_alpha(0)
     if savename:
         plt.savefig(savename, dpi=save_dpi)
-    plt.show()
-    return None
+    if show_fig:
+        plt.show()
+    else:
+        return cgx
 
 
 def _scatter_fix_type(v: pd.Series, ints_as_cats: bool) -> pd.Series:
     vt = v.dtype
     if v.nunique() == 1:
         return pd.Series(np.ones(len(v)), index=v.index).astype(np.float_)
     if vt in [np.bool_]:
@@ -382,24 +390,47 @@
         diff -= 1
     if not constrained:
         plt.tight_layout(w_pad=w_pad, h_pad=h_pad)
 
     return fig, axes
 
 
+def _create_axes(dfs, in_ax, width, height, w_pad, h_pad, n_columns):
+    if len(dfs) > 1:
+        if in_ax is not None:
+            logger.warning(f"'in_ax' will not be used as multiple attributes will be plotted. Using internal grid"
+                           f"layout")
+        _, axs = _make_grid(width, height, w_pad, h_pad, len(dfs), n_columns)
+    else:
+        if in_ax is None:
+            _, axs = plt.subplots(1, 1, figsize=(width, height), squeeze=False)
+        else:
+            axs = in_ax
+    return axs
+
+
+def _iter_dataframes(dfs, mask_values, mask_name, force_ints_as_cats):
+    for n, df in enumerate(dfs):
+        vc = df.columns[2]
+        v = _scatter_fix_mask(df[vc].copy(), mask_values, mask_name)
+        df[vc] = _scatter_fix_type(v, force_ints_as_cats)
+        yield n, df
+
+
 def plot_scatter(dfs, in_ax=None, width: float = 6, height: float = 6,
                  default_color: str = 'steelblue', color_map=None, color_key: dict = None,
                  mask_values: list = None, mask_name: str = 'NA', mask_color: str = 'k',
                  point_size: float = 10, ax_label_size: float = 12, frame_offset: float = 0.05,
                  spine_width: float = 0.5, spine_color: str = 'k', displayed_sides: tuple = ('bottom', 'left'),
                  legend_ondata: bool = True, legend_onside: bool = True,
                  legend_size: float = 12, legends_per_col: int = 20, cbar_shrink: float = 0.6,
                  marker_scale: float = 70, lspacing: float = 0.1, cspacing: float = 1,
                  savename: str = None, dpi: int = 300, force_ints_as_cats: bool = True,
-                 n_columns: int = 4, w_pad: float = 1, h_pad: float = 1, scatter_kwargs: dict = None):
+                 n_columns: int = 4, w_pad: float = 1, h_pad: float = 1, show_fig: bool = True,
+                 scatter_kwargs: dict = None):
     """
     Shows scatter plots. If more then one dataframe is provided it will place the scatterplots in a grid. 
     """
     from matplotlib.colors import to_hex
 
     def _handle_scatter_kwargs(sk):
         if sk is None:
@@ -412,122 +443,97 @@
             del sk['s']
         if 'lw' not in sk:
             sk['lw'] = 0.1
         if 'edgecolors' not in sk:
             sk['edgecolors'] = 'k'
         return sk
 
-    if len(dfs) > 1:
-        if in_ax is not None:
-            logger.warning(f"'in_ax' will not be used as multiple attributes will be plotted. Using internal grid"
-                           f"layout")
-        fig, axs = _make_grid(width, height, w_pad, h_pad, len(dfs), n_columns)
-    else:
-        if in_ax is None:
-            _, axs = plt.subplots(1, 1, figsize=(width, height), squeeze=False)
-        else:
-            axs = in_ax
-
-    for i, df in enumerate(dfs):
-        # noinspection DuplicatedCode
-        dim1, dim2, vc = df.columns[:3]
-        v = _scatter_fix_mask(df[vc].copy(), mask_values, mask_name)
-        v = _scatter_fix_type(v, force_ints_as_cats)
-        df[vc] = v
+    axs = _create_axes(dfs, in_ax, width, height, w_pad, h_pad, n_columns)
+    for n, df in _iter_dataframes(dfs, mask_values, mask_name, force_ints_as_cats):
+        v = df[df.columns[2]]
         col_map, col_key = _scatter_make_colors(v, color_map, color_key,
                                                 mask_color, mask_name)
         if v.dtype.name == 'category':
             df['c'] = [col_key[x] for x in v]
         else:
             if v.nunique() == 1:
                 df['c'] = [default_color for _ in v]
             else:
                 v = v.copy().fillna(0)
                 mmv = (v - v.min()) / (v.max() - v.min())
                 df['c'] = [to_hex(col_map(x)) for x in mmv]
         if 's' not in df:
             df['s'] = [point_size for _ in df.index]
         scatter_kwargs = _handle_scatter_kwargs(sk=scatter_kwargs)
-        ax = axs[int(i / n_columns), i % n_columns]
-        ax.scatter(df[dim1].values, df[dim2].values, c=df['c'].values, s=df['s'].values,
+        ax = axs[int(n / n_columns), n % n_columns]
+        ax.scatter(df.values[:, 0], df.values[:, 1], c=df['c'].values, s=df['s'].values,
                    rasterized=True, **scatter_kwargs)
         _scatter_label_axis(df, ax, ax_label_size, frame_offset)
         _scatter_cleanup(ax, spine_width, spine_color, displayed_sides)
         _scatter_legends(df, ax, col_map, col_key, legend_ondata, legend_onside,
                          legend_size, legends_per_col, marker_scale, lspacing, cspacing, cbar_shrink)
 
-    if in_ax is None:
-        if savename:
-            plt.savefig(savename, dpi=dpi, bbox_inches='tight')
+    if savename:
+        plt.savefig(savename, dpi=dpi, bbox_inches='tight')
+    if show_fig:
         plt.show()
     else:
         return axs
 
 
-def shade_scatter(dfs, in_ax=None, figsize: float = 6, pixels: int = 1000, sampling: float = 0.1,
+def shade_scatter(dfs, in_ax=None, figsize: float = 6, pixels: int = 1000,
                   spread_px: int = 1, spread_threshold: float = 0.2, min_alpha: int = 10,
                   color_map=None, color_key: dict = None,
                   mask_values: list = None, mask_name: str = 'NA', mask_color: str = 'k',
                   ax_label_size: float = 12, frame_offset: float = 0.05,
                   spine_width: float = 0.5, spine_color: str = 'k', displayed_sides: tuple = ('bottom', 'left'),
                   legend_ondata: bool = True, legend_onside: bool = True,
                   legend_size: float = 12, legends_per_col: int = 20, cbar_shrink: float = 0.6,
                   marker_scale: float = 70, lspacing: float = 0.1, cspacing: float = 1,
                   savename: str = None, dpi: int = 300, force_ints_as_cats: bool = True,
-                  n_columns: int = 4, w_pad: float = None, h_pad: float = None):
+                  n_columns: int = 4, w_pad: float = None, h_pad: float = None, show_fig: bool = True):
     """
     Shows shaded scatter plots. If more then one dataframe is provided it will place the scatterplots in a grid. 
     """
     import datashader as dsh
-    from IPython.display import display
     from datashader.mpl_ext import dsshow
     import datashader.transfer_functions as tf
     from functools import partial
 
-    if len(dfs) > 1:
-        if in_ax is not None:
-            logger.warning(f"'in_ax' will not be used as multiple attributes will be plotted. Using internal grid"
-                           f"layout")
-        fig, axs = _make_grid(figsize, figsize, w_pad, h_pad, len(dfs), n_columns)
-    else:
-        if in_ax is None:
-            _, axs = plt.subplots(1, 1, figsize=(figsize, figsize), squeeze=False)
-        else:
-            axs = in_ax
-
-    for i, df in enumerate(dfs):
+    axs = _create_axes(dfs, in_ax, figsize, figsize, w_pad, h_pad, n_columns)
+    for n, df in _iter_dataframes(dfs, mask_values, mask_name, force_ints_as_cats):
         dim1, dim2, vc = df.columns[:3]
-        v = _scatter_fix_mask(df[vc].copy(), mask_values, mask_name)
-        v = _scatter_fix_type(v, force_ints_as_cats)
-        df[vc] = v
+        v = df[vc]
         col_map, col_key = _scatter_make_colors(v, color_map, color_key,
                                                 mask_color, mask_name)
         if v.dtype.name == 'category':
             agg = dsh.count_cat(vc)
         else:
             if v.nunique() == 1:
                 agg = dsh.count(vc)
             else:
                 agg = dsh.mean(vc)
 
-        ax = axs[int(i / n_columns), i % n_columns]
+        ax = axs[int(n / n_columns), n % n_columns]
         artist = dsshow(df, dsh.Point(dim1, dim2), aggregator=agg, norm='eq_hist',
                         color_key=col_key, cmap=col_map, alpha_range=(min_alpha, 255),
                         shade_hook=partial(tf.dynspread, threshold=spread_threshold, max_px=spread_px),
                         plot_height=pixels, plot_width=pixels, aspect='equal', width_scale=1, height_scale=1,
                         ax=ax)
 
         _scatter_label_axis(df, ax, ax_label_size, frame_offset)
         _scatter_cleanup(ax, spine_width, spine_color, displayed_sides)
         _scatter_legends(df, ax, col_map, col_key, legend_ondata, legend_onside,
                          legend_size, legends_per_col, marker_scale, lspacing, cspacing, cbar_shrink)
 
     if savename:
         plt.savefig(savename, dpi=dpi, bbox_inches='tight')
-    if in_ax is not None:
+    if show_fig:
+        plt.show()
+    else:
         return axs
 
 
 def _draw_pie(ax, dist, colors, xpos, ypos, size):
     # https://stackoverflow.com/questions/56337732/how-to-plot-scatter-pie-chart-using-matplotlib
     cumsum = np.cumsum(dist)
     cumsum = cumsum / cumsum[-1]
```

### Comparing `scarf-0.9.1/scarf/readers.py` & `scarf-0.9.2/scarf/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,22 +350,23 @@
 
     Subclass of CrReader.
 
     Attributes:
         loc: Path for the directory containing the cellranger output.
         matFn: The file name for the matrix file.
     """
-    def __init__(self, loc, file_type: str = None):
+    def __init__(self, loc, file_type: str = None, mtx_separator: str = ' '):
         """
         Args:
             loc (str): Path for the directory containing the cellranger output.
             file_type (str): Type of sequencing data ('rna' | 'atac')
         """
         self.loc: str = loc.rstrip('/') + '/'
         self.matFn = None
+        self.sep = mtx_separator
         super().__init__(self._handle_version(), file_type)
 
     def _handle_version(self):
         if os.path.isfile(self.loc + 'features.tsv.gz'):
             self.matFn = self.loc + 'matrix.mtx.gz'
             grps = {'feature_ids': ('features.tsv.gz', 0),
                     'feature_names': ('features.tsv.gz', 1),
@@ -432,15 +433,15 @@
             return v[idx.start: idx.end]
         else:
             raise ValueError("ERROR: assay feats is 3D. Something went really wrong. Create a github issue")
 
     # noinspection DuplicatedCode
     def consume(self, batch_size: int, lines_in_mem: int = int(1e5)) -> \
             Generator[List[np.ndarray], None, None]:
-        stream = pd.read_csv(self.matFn, skiprows=3, sep='\t',
+        stream = pd.read_csv(self.matFn, skiprows=3, sep=self.sep,
                              header=None, chunksize=lines_in_mem)
         start = 1
         dfs = []
         for df in stream:
             if df.iloc[-1, 1] - start >= batch_size:
                 idx = df[1] < batch_size + start
                 dfs.append(df[idx])
```

### Comparing `scarf-0.9.1/scarf/umap.py` & `scarf-0.9.2/scarf/umap.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/utils.py` & `scarf-0.9.2/scarf/utils.py`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/scarf/writers.py` & `scarf-0.9.2/scarf/writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 import pandas as pd
 from .utils import controlled_compute
 from .logging_utils import logger
 from scipy.sparse import csr_matrix
 
 __all__ = ['create_zarr_dataset', 'create_zarr_obj_array', 'create_zarr_count_assay',
            'subset_assay_zarr', 'dask_to_zarr', 'ZarrMerge', 'SubsetZarr',
-           'CrToZarr', 'H5adToZarr', 'MtxToZarr', 'NaboH5ToZarr', 'LoomToZarr', 'SparseToZarr']
+           'CrToZarr', 'H5adToZarr', 'MtxToZarr', 'NaboH5ToZarr', 'LoomToZarr', 'SparseToZarr',
+           'to_h5ad', 'to_mtx']
 
 
 def create_zarr_dataset(g: zarr.Group, name: str, chunks: tuple,
                         dtype: Any, shape: Tuple, overwrite: bool = True) -> zarr.hierarchy:
     """
     Creates and returns a Zarr array.
 
@@ -668,18 +669,15 @@
         import dask.array as daskarr
 
         return daskarr.from_zarr(self.iz[assay_name]['counts'], inline_array=True)
 
     def _prep_counts(self):
         n_cells = len(self.cellIdx)
         for assay_name in self.assays:
-            print (assay_name)
             raw_data = self._get_raw_data(assay_name)
-            print (self.iz[assay_name]['featureData']['ids'][:])
-            print (self.iz[assay_name]['featureData']['names'][:])
             create_zarr_count_assay(self.oz, assay_name, raw_data.chunksize, n_cells,
                                     self.iz[assay_name]['featureData']['ids'][:],
                                     self.iz[assay_name]['featureData']['names'][:], raw_data.dtype)
 
     def dump(self):
         for assay_name in self.assays:
             raw_data = self._get_raw_data(assay_name)
@@ -929,24 +927,24 @@
     n_feats_per_cell = assay.cells.fetch_all(f"{assay.name}_nFeatures").astype(int)
     tot_counts = int(n_feats_per_cell.sum())
     if compress:
         barcodes_fn = 'barcodes.tsv.gz'
         features_fn = 'features.tsv.gz'
         h = gzip.open(os.path.join(mtx_directory, 'matrix.mtx.gz'), 'wt')
     else:
-        barcodes_fn = 'barcodes.tsv.gz'
+        barcodes_fn = 'barcodes.tsv'
         features_fn = 'genes.tsv'
         h = open(os.path.join(mtx_directory, 'matrix.mtx'), 'w')
     h.write("%%MatrixMarket matrix coordinate integer general\n% Generated by Scarf\n")
     h.write(f"{assay.feats.N} {assay.cells.N} {tot_counts}\n")
     s = 0
     for i in tqdm(assay.rawData.blocks, total=assay.rawData.numblocks[0]):
         i = coo_matrix((i.compute()))
         df = pd.DataFrame({'col': i.col + 1, 'row': i.row + s + 1, 'd': i.data})
-        df.to_csv(h, sep=' ', header=False, index=False, mode='a')
+        df.to_csv(h, sep=' ', header=False, index=False, mode='a', line_terminator='\n')
         s += i.shape[0]
     h.close()
     assay.cells.to_pandas_dataframe(['ids']).to_csv(
         os.path.join(mtx_directory, barcodes_fn),
         sep='\t', header=False, index=False)
 
     assay.feats.to_pandas_dataframe(['ids', 'names']).to_csv(
```

### Comparing `scarf-0.9.1/scarf.egg-info/SOURCES.txt` & `scarf-0.9.2/scarf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scarf-0.9.1/setup.py` & `scarf-0.9.2/setup.py`

 * *Files identical despite different names*

