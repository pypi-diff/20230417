# Comparing `tmp/histomicsui-1.4.3.dev5.tar.gz` & `tmp/histomicsui-1.4.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicsui-1.4.3.dev5.tar", last modified: Fri Apr  7 20:32:29 2023, max compression
+gzip compressed data, was "histomicsui-1.4.3.dev8.tar", last modified: Tue Apr 11 17:13:22 2023, max compression
```

## Comparing `histomicsui-1.4.3.dev5.tar` & `histomicsui-1.4.3.dev8.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.576483 histomicsui-1.4.3.dev5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.548483 histomicsui-1.4.3.dev5/.circleci/
--rw-r--r--   0 root         (0) root         (0)     3793 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      303 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/.editorconfig
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/.git-blame-ignore-revs
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/.gitignore
--rw-r--r--   0 root         (0) root         (0)      690 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/.travis.yml
--rw-r--r--   0 root         (0) root         (0)    10173 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6974 2023-04-07 20:32:29.576483 histomicsui-1.4.3.dev5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6076 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/README.rst
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.548483 histomicsui-1.4.3.dev5/docs/
--rw-r--r--   0 root         (0) root         (0)     2399 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/docs/config_options.rst
--rw-r--r--   0 root         (0) root         (0)     5901 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/docs/controls.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.548483 histomicsui-1.4.3.dev5/docs/images/
--rwxr-xr-x   0 root         (0) root         (0)   133796 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/docs/images/difference.gif
--rwxr-xr-x   0 root         (0) root         (0)   133603 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/docs/images/intersect.gif
--rwxr-xr-x   0 root         (0) root         (0)   154141 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/docs/images/union.gif
--rwxr-xr-x   0 root         (0) root         (0)   168255 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/docs/images/xor.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.548483 histomicsui-1.4.3.dev5/histomicsui/
--rw-r--r--   0 root         (0) root         (0)    17578 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/constants.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.552483 histomicsui-1.4.3.dev5/histomicsui/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/aperio.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/case.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/cohort.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/image.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/meta.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/pathology.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/models/slide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.552483 histomicsui-1.4.3.dev5/histomicsui/rest/
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3728 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/rest/aperio.py
--rw-r--r--   0 root         (0) root         (0)     9313 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/rest/hui_resource.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/rest/image_browse_resource.py
--rw-r--r--   0 root         (0) root         (0)    15298 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/rest/system.py
--rw-r--r--   0 root         (0) root         (0)    28968 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/rest/tcga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.552483 histomicsui-1.4.3.dev5/histomicsui/web_client/
--rw-r--r--   0 root         (0) root         (0)     2450 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/app.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.552483 histomicsui-1.4.3.dev5/histomicsui/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/collections/StyleCollection.js
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/collections/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.556483 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/
--rw-r--r--   0 root         (0) root         (0)     1326 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/confirmDialog.js
--rw-r--r--   0 root         (0) root         (0)     3936 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/editElement.js
--rw-r--r--   0 root         (0) root         (0)     6663 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/editRegionOfInterest.js
--rw-r--r--   0 root         (0) root         (0)    11184 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/editStyleGroups.js
--rw-r--r--   0 root         (0) root         (0)      478 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/index.js
--rw-r--r--   0 root         (0) root         (0)     1153 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/metadataPlot.js
--rw-r--r--   0 root         (0) root         (0)     4936 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/openAnnotatedImage.js
--rw-r--r--   0 root         (0) root         (0)     2588 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/openImage.js
--rw-r--r--   0 root         (0) root         (0)    22740 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/saveAnnotation.js
--rw-r--r--   0 root         (0) root         (0)       78 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.556483 histomicsui-1.4.3.dev5/histomicsui/web_client/models/
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/models/StyleModel.js
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     5376 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.556483 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/
--rw-r--r--   0 root         (0) root         (0)    23413 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/AnnotationSelector.js
--rw-r--r--   0 root         (0) root         (0)    43398 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/DrawWidget.js
--rw-r--r--   0 root         (0) root         (0)    14204 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/MetadataPlot.js
--rw-r--r--   0 root         (0) root         (0)    22033 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/MetadataWidget.js
--rw-r--r--   0 root         (0) root         (0)     8115 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/OverviewWidget.js
--rw-r--r--   0 root         (0) root         (0)     1121 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/RegionSelector.js
--rw-r--r--   0 root         (0) root         (0)     9946 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/ZoomWidget.js
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/panels/index.js
--rw-r--r--   0 root         (0) root         (0)     1485 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/router.js
--rw-r--r--   0 root         (0) root         (0)      292 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.556483 histomicsui-1.4.3.dev5/histomicsui/web_client/static/
--rwxr-xr-x   0 root         (0) root         (0)     5072 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/static/favicon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.544483 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.556483 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/body/
--rw-r--r--   0 root         (0) root         (0)      504 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/body/configView.styl
--rw-r--r--   0 root         (0) root         (0)      883 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/body/frontPage.styl
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/body/image.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.556483 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/dialogs/
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
--rw-r--r--   0 root         (0) root         (0)      769 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.556483 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/layout/
--rw-r--r--   0 root         (0) root         (0)      976 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/layout/header.styl
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/layout/headerImage.styl
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/layout/layout.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.560483 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/
--rw-r--r--   0 root         (0) root         (0)     1666 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
--rw-r--r--   0 root         (0) root         (0)     2747 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/drawWidget.styl
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/regionSelector.styl
--rw-r--r--   0 root         (0) root         (0)      877 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.560483 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/popover/
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
--rw-r--r--   0 root         (0) root         (0)     1847 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.560483 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/views/
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/views/itemList.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.544483 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.560483 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/body/
--rw-r--r--   0 root         (0) root         (0)     5608 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/body/configView.pug
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/body/frontPage.pug
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/body/image.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.560483 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/
--rw-r--r--   0 root         (0) root         (0)      501 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/confirmDialog.pug
--rw-r--r--   0 root         (0) root         (0)     2079 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/editElement.pug
--rw-r--r--   0 root         (0) root         (0)     1730 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
--rw-r--r--   0 root         (0) root         (0)     3201 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
--rw-r--r--   0 root         (0) root         (0)     1541 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/openImage.pug
--rw-r--r--   0 root         (0) root         (0)     5392 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.560483 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/header.pug
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/headerAnalyses.pug
--rw-r--r--   0 root         (0) root         (0)     1467 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/headerImage.pug
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/headerUser.pug
--rw-r--r--   0 root         (0) root         (0)      157 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/layout.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.564483 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/
--rw-r--r--   0 root         (0) root         (0)     3961 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/annotationSelector.pug
--rw-r--r--   0 root         (0) root         (0)     5673 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/drawWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2166 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/drawWidgetElement.pug
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/metadataPlot.pug
--rw-r--r--   0 root         (0) root         (0)      815 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/metadataWidget.pug
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/overviewWidget.pug
--rw-r--r--   0 root         (0) root         (0)      398 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/panel.pug
--rw-r--r--   0 root         (0) root         (0)      345 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/regionSelector.pug
--rw-r--r--   0 root         (0) root         (0)     1281 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/zoomWidget.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.564483 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/popover/
--rw-r--r--   0 root         (0) root         (0)      576 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/popover/annotationContextMenu.pug
--rw-r--r--   0 root         (0) root         (0)     1404 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/popover/annotationPopover.pug
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.564483 histomicsui-1.4.3.dev5/histomicsui/web_client/views/
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/HierarchyWidget.js
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/View.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.564483 histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/
--rw-r--r--   0 root         (0) root         (0)     7205 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)      776 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/FrontPageView.js
--rw-r--r--   0 root         (0) root         (0)    68106 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/ImageView.js
--rw-r--r--   0 root         (0) root         (0)      183 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/index.js
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)     3436 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/itemList.js
--rw-r--r--   0 root         (0) root         (0)     2375 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/itemPage.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.564483 histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/HeaderAnalysesView.js
--rw-r--r--   0 root         (0) root         (0)     2861 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/HeaderImageView.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/HeaderUserView.js
--rw-r--r--   0 root         (0) root         (0)     1621 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/HeaderView.js
--rw-r--r--   0 root         (0) root         (0)      134 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.568483 histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/
--rw-r--r--   0 root         (0) root         (0)     4493 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/AnnotationContextMenu.js
--rw-r--r--   0 root         (0) root         (0)    10799 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/AnnotationPopover.js
--rw-r--r--   0 root         (0) root         (0)     1231 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/PixelmapContextMenu.js
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/index.js
--rw-r--r--   0 root         (0) root         (0)     2847 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/views/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.544483 histomicsui-1.4.3.dev5/histomicsui/web_client/vue/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.568483 histomicsui-1.4.3.dev5/histomicsui/web_client/vue/components/
--rw-r--r--   0 root         (0) root         (0)     2777 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/vue/components/ColorPickerInput.vue
--rw-r--r--   0 root         (0) root         (0)    12624 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
--rw-r--r--   0 root         (0) root         (0)      814 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
--rw-r--r--   0 root         (0) root         (0)      947 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/web_client/webpack.helper.js
--rw-r--r--   0 root         (0) root         (0)     1538 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/histomicsui/webroot.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.548483 histomicsui-1.4.3.dev5/histomicsui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6974 2023-04-07 20:32:29.000000 histomicsui-1.4.3.dev5/histomicsui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7281 2023-04-07 20:32:29.000000 histomicsui-1.4.3.dev5/histomicsui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 20:32:29.000000 histomicsui-1.4.3.dev5/histomicsui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-07 20:32:29.000000 histomicsui-1.4.3.dev5/histomicsui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 20:31:36.000000 histomicsui-1.4.3.dev5/histomicsui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-07 20:32:29.000000 histomicsui-1.4.3.dev5/histomicsui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-07 20:32:29.000000 histomicsui-1.4.3.dev5/histomicsui.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-07 20:32:29.576483 histomicsui-1.4.3.dev5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2289 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.568483 histomicsui-1.4.3.dev5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/datastore.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/girder_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.572483 histomicsui-1.4.3.dev5/tests/test_files/
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_files/.histomicsui_config.yaml
--rw-r--r--   0 root         (0) root         (0)      424 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_files/sample.anot
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_files/sample.meta
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_files/sample_girder_id.anot
--rw-r--r--   0 root         (0) root         (0)     8928 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_files/test_analysis_detection.xml
--rw-r--r--   0 root         (0) root         (0)    12017 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_files/test_analysis_features.xml
--rw-r--r--   0 root         (0) root         (0)     5257 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_handlers.py
--rw-r--r--   0 root         (0) root         (0)    19443 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_hui_rest.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_image_browse_endpoints.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)    32496 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_tcga.py
--rw-r--r--   0 root         (0) root         (0)     5993 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:32:29.576483 histomicsui-1.4.3.dev5/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      237 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     6591 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/analysisSpec.js
--rw-r--r--   0 root         (0) root         (0)    81677 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/annotationSpec.js
--rw-r--r--   0 root         (0) root         (0)     1923 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/girderUISpec.js
--rw-r--r--   0 root         (0) root         (0)     4037 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/huiSpec.js
--rw-r--r--   0 root         (0) root         (0)     4336 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/huiTest.js
--rw-r--r--   0 root         (0) root         (0)     4387 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/itemSpec.js
--rw-r--r--   0 root         (0) root         (0)     4390 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/metadataPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     6526 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/metadataPlotSpec.js
--rw-r--r--   0 root         (0) root         (0)     6175 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/overviewPanelSpec.js
--rw-r--r--   0 root         (0) root         (0)     2917 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/panelLayoutSpec.js
--rw-r--r--   0 root         (0) root         (0)    13890 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tests/web_client_specs/pixelmapCategorySpec.js
--rw-r--r--   0 root         (0) root         (0)     2944 2023-04-07 20:31:22.000000 histomicsui-1.4.3.dev5/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      303 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.git-blame-ignore-revs
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      690 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)    10173 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      585 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/README.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/docs/
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/config_options.rst
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/controls.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/docs/images/
+-rwxr-xr-x   0 root         (0) root         (0)   133796 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/difference.gif
+-rwxr-xr-x   0 root         (0) root         (0)   133603 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/intersect.gif
+-rwxr-xr-x   0 root         (0) root         (0)   154141 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/union.gif
+-rwxr-xr-x   0 root         (0) root         (0)   168255 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/docs/images/xor.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.873448 histomicsui-1.4.3.dev8/histomicsui/
+-rw-r--r--   0 root         (0) root         (0)    17578 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/case.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/cohort.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/image.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/meta.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/pathology.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/models/slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui/rest/
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3728 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/aperio.py
+-rw-r--r--   0 root         (0) root         (0)     9313 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/hui_resource.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/image_browse_resource.py
+-rw-r--r--   0 root         (0) root         (0)    15298 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/system.py
+-rw-r--r--   0 root         (0) root         (0)    28968 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/rest/tcga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui/web_client/
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/app.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/collections/StyleCollection.js
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/collections/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/confirmDialog.js
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editElement.js
+-rw-r--r--   0 root         (0) root         (0)     6663 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js
+-rw-r--r--   0 root         (0) root         (0)    11184 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editStyleGroups.js
+-rw-r--r--   0 root         (0) root         (0)      478 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/index.js
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/metadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)     4936 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openImage.js
+-rw-r--r--   0 root         (0) root         (0)    22740 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/saveAnnotation.js
+-rw-r--r--   0 root         (0) root         (0)       78 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      787 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/models/StyleModel.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     5686 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/
+-rw-r--r--   0 root         (0) root         (0)    23413 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/AnnotationSelector.js
+-rw-r--r--   0 root         (0) root         (0)    43398 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/DrawWidget.js
+-rw-r--r--   0 root         (0) root         (0)    14204 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataPlot.js
+-rw-r--r--   0 root         (0) root         (0)    22033 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataWidget.js
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/OverviewWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/RegionSelector.js
+-rw-r--r--   0 root         (0) root         (0)     9946 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/ZoomWidget.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/panels/index.js
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/router.js
+-rw-r--r--   0 root         (0) root         (0)      292 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/static/
+-rwxr-xr-x   0 root         (0) root         (0)     5072 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/static/favicon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.869448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.881448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/configView.styl
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/frontPage.styl
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/image.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/editStyleGroups.styl
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/openAnnotatedImage.styl
+-rw-r--r--   0 root         (0) root         (0)      769 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/
+-rw-r--r--   0 root         (0) root         (0)      976 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/header.styl
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/headerAnalyses.styl
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/headerImage.styl
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/layout.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/metadataPlot.styl
+-rw-r--r--   0 root         (0) root         (0)      865 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/overviewWidget.styl
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/regionSelector.styl
+-rw-r--r--   0 root         (0) root         (0)      877 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/annotationContextMenu.styl
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/views/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/views/itemList.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.869448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.885448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/configView.pug
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/frontPage.pug
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/image.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/annotatedImageList.pug
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/confirmDialog.pug
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editElement.pug
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/openImage.pug
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/
+-rw-r--r--   0 root         (0) root         (0)      925 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/header.pug
+-rw-r--r--   0 root         (0) root         (0)      865 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerImage.pug
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerUser.pug
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/layout.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/metadataPlot.pug
+-rw-r--r--   0 root         (0) root         (0)      815 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/metadataWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/overviewWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/regionSelector.pug
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/
+-rw-r--r--   0 root         (0) root         (0)      576 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug
+-rw-r--r--   0 root         (0) root         (0)      204 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/pixelmapContextMenu.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.889448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/View.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)      776 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/FrontPageView.js
+-rw-r--r--   0 root         (0) root         (0)    68106 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ImageView.js
+-rw-r--r--   0 root         (0) root         (0)      183 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/index.js
+-rw-r--r--   0 root         (0) root         (0)      190 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)     3436 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemList.js
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemPage.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderImageView.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderUserView.js
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderView.js
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/
+-rw-r--r--   0 root         (0) root         (0)     4493 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)    10799 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/index.js
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/views/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.869448 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue
+-rw-r--r--   0 root         (0) root         (0)    12531 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue
+-rw-r--r--   0 root         (0) root         (0)      745 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue
+-rw-r--r--   0 root         (0) root         (0)      947 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/web_client/webpack.helper.js
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/histomicsui/webroot.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.877448 histomicsui-1.4.3.dev8/histomicsui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7281 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:12:29.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 17:13:22.000000 histomicsui-1.4.3.dev8/histomicsui.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.893448 histomicsui-1.4.3.dev8/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/datastore.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/girder_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/tests/test_files/
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/.histomicsui_config.yaml
+-rw-r--r--   0 root         (0) root         (0)      424 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/sample.anot
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/sample.meta
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/sample_girder_id.anot
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/test_analysis_detection.xml
+-rw-r--r--   0 root         (0) root         (0)    12017 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_files/test_analysis_features.xml
+-rw-r--r--   0 root         (0) root         (0)     5257 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_handlers.py
+-rw-r--r--   0 root         (0) root         (0)    19443 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_hui_rest.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_image_browse_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)    32496 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_tcga.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:13:22.897448 histomicsui-1.4.3.dev8/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/analysisSpec.js
+-rw-r--r--   0 root         (0) root         (0)    81677 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/annotationSpec.js
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/girderUISpec.js
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/huiSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4336 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/huiTest.js
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/itemSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4390 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6526 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPlotSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6175 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/overviewPanelSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/panelLayoutSpec.js
+-rw-r--r--   0 root         (0) root         (0)    13890 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tests/web_client_specs/pixelmapCategorySpec.js
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-04-11 17:12:14.000000 histomicsui-1.4.3.dev8/tox.ini
```

### Comparing `histomicsui-1.4.3.dev5/.circleci/config.yml` & `histomicsui-1.4.3.dev8/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/.gitignore` & `histomicsui-1.4.3.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/.travis.yml` & `histomicsui-1.4.3.dev8/.travis.yml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/LICENSE` & `histomicsui-1.4.3.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/NOTICE` & `histomicsui-1.4.3.dev8/NOTICE`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/PKG-INFO` & `histomicsui-1.4.3.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.3.dev5
+Version: 1.4.3.dev8
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.3.dev5/README.rst` & `histomicsui-1.4.3.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/docs/config_options.rst` & `histomicsui-1.4.3.dev8/docs/config_options.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/docs/controls.rst` & `histomicsui-1.4.3.dev8/docs/controls.rst`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/docs/images/difference.gif` & `histomicsui-1.4.3.dev8/docs/images/difference.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/docs/images/intersect.gif` & `histomicsui-1.4.3.dev8/docs/images/intersect.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/docs/images/union.gif` & `histomicsui-1.4.3.dev8/docs/images/union.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/docs/images/xor.gif` & `histomicsui-1.4.3.dev8/docs/images/xor.gif`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/__init__.py` & `histomicsui-1.4.3.dev8/histomicsui/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/constants.py` & `histomicsui-1.4.3.dev8/histomicsui/constants.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/handlers.py` & `histomicsui-1.4.3.dev8/histomicsui/handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/models/aperio.py` & `histomicsui-1.4.3.dev8/histomicsui/models/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/models/case.py` & `histomicsui-1.4.3.dev8/histomicsui/models/case.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/models/cohort.py` & `histomicsui-1.4.3.dev8/histomicsui/models/cohort.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/models/image.py` & `histomicsui-1.4.3.dev8/histomicsui/models/image.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/models/meta.py` & `histomicsui-1.4.3.dev8/histomicsui/models/meta.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/models/pathology.py` & `histomicsui-1.4.3.dev8/histomicsui/models/pathology.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/models/slide.py` & `histomicsui-1.4.3.dev8/histomicsui/models/slide.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/rest/__init__.py` & `histomicsui-1.4.3.dev8/histomicsui/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/rest/aperio.py` & `histomicsui-1.4.3.dev8/histomicsui/rest/aperio.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/rest/hui_resource.py` & `histomicsui-1.4.3.dev8/histomicsui/rest/hui_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/rest/image_browse_resource.py` & `histomicsui-1.4.3.dev8/histomicsui/rest/image_browse_resource.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/rest/system.py` & `histomicsui-1.4.3.dev8/histomicsui/rest/system.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/rest/tcga.py` & `histomicsui-1.4.3.dev8/histomicsui/rest/tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/app.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/app.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/confirmDialog.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/confirmDialog.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/editElement.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editElement.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/editRegionOfInterest.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editRegionOfInterest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/editStyleGroups.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/editStyleGroups.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/metadataPlot.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/metadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/openAnnotatedImage.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openAnnotatedImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/openImage.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/openImage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/dialogs/saveAnnotation.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/dialogs/saveAnnotation.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/main.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/main.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/package.json` & `histomicsui-1.4.3.dev8/histomicsui/web_client/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9862132352941176%*

 * *Differences: {"'devDependencies'": "{'eslint-plugin-vue': '^9.10.0'}",*

 * * "'eslintConfig'": "{'extends': ['@girder', 'plugin:vue/recommended'], 'rules': "*

 * *                   "{'vue/require-prop-types': 'off'}, 'overrides': [OrderedDict([('files', "*

 * *                   "['*.js', '*.vue'])])]}"}*

```diff
@@ -24,19 +24,31 @@
         "eslint": "^8.20.0",
         "eslint-config-semistandard": "^17.0.0",
         "eslint-config-standard": "^17.0.0",
         "eslint-plugin-backbone": "^2.1.1",
         "eslint-plugin-import": "^2.25.3",
         "eslint-plugin-n": "^15.2.4",
         "eslint-plugin-promise": "^6.0.0",
+        "eslint-plugin-vue": "^9.10.0",
         "pug-lint": "^2",
         "stylint": "^2"
     },
     "eslintConfig": {
-        "extends": "@girder",
+        "extends": [
+            "@girder",
+            "plugin:vue/recommended"
+        ],
+        "overrides": [
+            {
+                "files": [
+                    "*.js",
+                    "*.vue"
+                ]
+            }
+        ],
         "root": true,
         "rules": {
             "for-direction": "error",
             "getter-return": "error",
             "import/exports-last": "error",
             "multiline-ternary": [
                 "error",
@@ -47,15 +59,16 @@
             "object-curly-spacing": [
                 "error",
                 "never"
             ],
             "promise/no-native": "error",
             "promise/no-return-in-finally": "error",
             "promise/no-return-wrap": "error",
-            "switch-colon-spacing": "error"
+            "switch-colon-spacing": "error",
+            "vue/require-prop-types": "off"
         }
     },
     "girderPlugin": {
         "dependencies": [
             "large_image",
             "large_image_annotation",
             "slicer_cli_web"
```

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/panels/AnnotationSelector.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/AnnotationSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/panels/DrawWidget.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/DrawWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/panels/MetadataPlot.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataPlot.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/panels/MetadataWidget.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/panels/OverviewWidget.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/OverviewWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/panels/RegionSelector.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/RegionSelector.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/panels/ZoomWidget.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/panels/ZoomWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/router.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/router.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/static/favicon.png` & `histomicsui-1.4.3.dev8/histomicsui/web_client/static/favicon.png`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/body/frontPage.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/frontPage.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/body/image.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/body/image.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/dialogs/saveAnnotation.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/layout/header.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/header.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/layout/layout.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/annotationSelector.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/annotationSelector.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/drawWidget.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/drawWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/metadataWidget.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/panels/zoomWidget.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/panels/zoomWidget.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/stylesheets/popover/annotationPopover.styl` & `histomicsui-1.4.3.dev8/histomicsui/web_client/stylesheets/popover/annotationPopover.styl`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/body/configView.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/configView.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/body/image.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/body/image.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/editElement.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editRegionOfInterest.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/editStyleGroups.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/editStyleGroups.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/metadataPlot.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/metadataPlot.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/openAnnotatedImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/dialogs/saveAnnotation.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/dialogs/saveAnnotation.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/header.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/header.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/headerAnalyses.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerAnalyses.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/headerImage.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerImage.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/layout/headerUser.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/layout/headerUser.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/annotationSelector.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/annotationSelector.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/drawWidget.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/drawWidgetElement.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/drawWidgetElement.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/metadataWidget.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/metadataWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/panels/zoomWidget.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/panels/zoomWidget.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/popover/annotationContextMenu.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationContextMenu.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/templates/popover/annotationPopover.pug` & `histomicsui-1.4.3.dev8/histomicsui/web_client/templates/popover/annotationPopover.pug`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/HierarchyWidget.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/View.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/View.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/ConfigView.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ConfigView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/FrontPageView.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/body/ImageView.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/body/ImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/itemList.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemList.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/itemPage.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/itemPage.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/HeaderAnalysesView.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderAnalysesView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/HeaderImageView.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderImageView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/layout/HeaderView.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/AnnotationContextMenu.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/AnnotationPopover.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/AnnotationPopover.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/popover/PixelmapContextMenu.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/popover/PixelmapContextMenu.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/views/utils.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/vue/components/ColorPickerInput.vue` & `histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/ColorPickerInput.vue`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 <script>
-import { Chrome } from 'vue-color';
+import {Chrome} from 'vue-color';
 import tinycolor from 'tinycolor2';
 
 export default {
-    props: ['color'],
     components: {
         'chrome-picker': Chrome
     },
+    props: ['color'],
     data() {
         return {
             pickerColor: this.color,
             colorValue: this.color,
             displayPicker: false
+        };
+    },
+    watch: {
+        colorValue(val) {
+            if (val) {
+                this.updatePickerColor(val);
+                this.$emit('input', val);
+            }
         }
     },
     mounted() {
         this.setColor(this.color || '#000000');
     },
     methods: {
         setColor(color) {
@@ -44,52 +52,50 @@
         },
         documentClick(e) {
             const picker = this.$refs.colorpicker;
             if (picker && picker !== e.target && !picker.contains(e.target)) {
                 this.hidePicker();
             }
         }
-    },
-    watch: {
-        colorValue(val) {
-            if (val) {
-                this.updatePickerColor(val);
-                this.$emit('input', val);
-            }
-        }
     }
-}
+};
 </script>
 
 <template>
-    <div class="input-group color-picker" ref="colorpicker">
-        <input
-            type="text"
-            class="form-control"
-            v-model="colorValue"
-            @focus="showPicker"
-            @input="updateFromInput"
-        />
-        <span v-if="colorValue" class="input-group-addon color-picker-container">
-            <span
-                class="current-color"
-                :style="{ 'background-color': colorValue }"
-                @click="togglePicker"
-            >
-                <i :style="{ 'background-color': colorValue }"></i>
-            </span>
-            <chrome-picker
-                class="picker-offset"
-                ref="colorPicker"
-                :value="pickerColor"
-                @input="updateFromPicker"
-                v-if="displayPicker"
-            />
-        </span>
-    </div>
+  <div
+    ref="colorpicker"
+    class="input-group color-picker"
+  >
+    <input
+      v-model="colorValue"
+      type="text"
+      class="form-control"
+      @focus="showPicker"
+      @input="updateFromInput"
+    >
+    <span
+      v-if="colorValue"
+      class="input-group-addon color-picker-container"
+    >
+      <span
+        class="current-color"
+        :style="{ 'background-color': colorValue }"
+        @click="togglePicker"
+      >
+        <i :style="{ 'background-color': colorValue }" />
+      </span>
+      <chrome-picker
+        v-if="displayPicker"
+        ref="colorPicker"
+        class="picker-offset"
+        :value="pickerColor"
+        @input="updateFromPicker"
+      />
+    </span>
+  </div>
 </template>
 
 <style scoped>
 .current-color {
     display: inline-block;
     width: 16px;
     height: 16px;
```

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue` & `histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridData.vue`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 <script>
 import tinycolor from 'tinycolor2';
 import _ from 'underscore';
+
 import ColorPickerInput from './ColorPickerInput.vue';
 export default {
-    props: ['elementData'],
-    emits: ['submit', 'cancel'],
     components: {
         ColorPickerInput
     },
+    props: ['elementData'],
+    emits: ['submit', 'cancel'],
     data() {
         return {
             type: this.elementData.type,
             interpretation: this.elementData.interpretation,
             radius: this.elementData.radius,
             normalizeRange: this.elementData.normalizeRange === undefined ? true : this.elementData.normalizeRange,
             colorRange: _.clone(this.elementData.colorRange || []),
@@ -28,14 +29,34 @@
         headerMessage() {
             if (this.type === 'heatmap') {
                 return 'Edit Heatmap Element';
             }
             return 'Edit Grid Data Element';
         }
     },
+    mounted() {
+        if (this.colorRange) {
+            _.forEach(this.colorRange, (color, index) => {
+                this.colorRangeData.push({
+                    colorString: color,
+                    value: this.rangeValues[index]
+                });
+            });
+        }
+        if (this.type === 'griddata' && !this.minColor && !this.maxColor) {
+            if (this.colorRange.length > 0) {
+                this.minColor = this.colorRange[0];
+                this.maxColor = this.colorRange[this.colorRange.length - 1];
+            } else {
+                this.minColor = 'rgba(0, 0, 0, 0)';
+                this.maxColor = 'rgba(255, 0, 0, 1)';
+            }
+        }
+        this.updateRangeDataKeys();
+    },
     methods: {
         getColorString(color) {
             return tinycolor(color).toString();
         },
         addNewFirstColor() {
             let newFirstColor;
             if (this.colorRangeData.length > 0) {
@@ -61,23 +82,23 @@
                     g: (lowerColorRgb.g + higherColorRgb.g) / 2,
                     b: (lowerColorRgb.b + higherColorRgb.b) / 2,
                     a: (lowerColorRgb.a + higherColorRgb.a) / 2
                 }).toString();
                 const newEntry = {
                     colorString: newColorString,
                     value: (lowerRecord.value + higherRecord.value) / 2
-                }
+                };
                 this.colorRangeData.splice(index + 1, 0, newEntry);
             } else {
                 const newColor = _.clone(lowerColorRgb);
                 newColor.a = 1.0;
                 const newEntry = {
                     value: lowerRecord.value < 1 ? 1 : lowerRecord.value,
                     colorString: tinycolor(newColor).toString()
-                }
+                };
                 this.colorRangeData.push(newEntry);
             }
             this.updateRangeDataKeys();
         },
         removeColor(index) {
             this.colorRangeData.splice(index, 1);
             this.updateRangeDataKeys();
@@ -140,16 +161,14 @@
         notifySubmit() {
             this.colorRangeData.sort((entry1, entry2) => entry1.value - entry2.value);
             const propsToSave = {
                 rangeValues: this.colorRangeData.map((entry) => parseFloat(entry.value)),
                 colorRange: this.colorRangeData.map((entry) => entry.colorString),
                 normalizeRange: this.normalizeRange
             };
-            if (this.colorRangeData.length) {
-            }
             if (this.type === 'heatmap') {
                 propsToSave.radius = parseFloat(this.radius);
                 propsToSave.scaleWithZoom = this.scaleWithZoom;
             } else {
                 // griddata
                 propsToSave.minColor = tinycolor(this.minColor).toString();
                 propsToSave.maxColor = tinycolor(this.maxColor).toString();
@@ -158,124 +177,182 @@
                 }
             }
             this.$emit('submit', propsToSave);
         },
         cancelDialog() {
             this.$emit('cancel');
         }
-    },
-    mounted() {
-        if (this.colorRange) {
-            _.forEach(this.colorRange, (color, index) => {
-                this.colorRangeData.push({
-                    colorString: color,
-                    value: this.rangeValues[index]
-                });
-            });
-        }
-        if (this.type === 'griddata' && !this.minColor && !this.maxColor) {
-            if (this.colorRange.length > 0) {
-                this.minColor = this.colorRange[0];
-                this.maxColor = this.colorRange[this.colorRange.length - 1];
-            } else {
-                this.minColor = 'rgba(0, 0, 0, 0)';
-                this.maxColor = 'rgba(255, 0, 0, 1)';
-            }
-        }
-        this.updateRangeDataKeys();
     }
-}
+};
 </script>
 
 <template>
-    <div class="modal-dialog" v-if="this.colorRangeData">
-        <div class="modal-content">
-            <form class="modal-form">
-                <div class="modal-header">
-                    <button type="button" class="close"  @click="cancelDialog()" ref="close">
-                        <span>&times;</span>
-                    </button>
-                    <h4>{{ headerMessage }}</h4>
-                </div>
-                <div class="modal-body">
-                    <div class="errors" v-if="validationErrors.length > 0">
-                        <p>Errors</p>
-                        <ul>
-                            <li v-for="error in this.validationErrors" :key="error">{{ error }}</li>
-                        </ul>
-                    </div>
-                    <div class="form-group" v-if="this.type === 'heatmap'">
-                        <label for="h-griddata-radius">Radius</label>
-                        <input id="h-griddata-radius" class="input-sm form-control" type="number" min="1" v-model="radius">
-                    </div>
-                    <div class="form-group">
-                        <label for="h-griddata-range">Range Colors</label>
-                        <table id="h-griddata-range" class="table table-bordered table-condensed">
-                            <thead>
-                                <tr>
-                                    <th>Value</th>
-                                    <th>Color</th>
-                                    <th>
-                                        <a @click.prevent="addNewFirstColor">
-                                            <span class="icon-plus" title="Add new first color"></span>
-                                        </a>
-                                    </th>
-                                </tr>
-                            </thead>
-                            <tbody>
-                            <tr v-if="this.type === 'griddata'">
-                                <td title="The color of values below the lowest range value">
-                                    Minimum color
-                                </td>
-                                <td>
-                                    <color-picker-input :color="minColor" v-model="minColor"></color-picker-input>
-                                </td>
-                            </tr>
-                            <tr v-for="(entry, index) in colorRangeData" :key="entry.key">
-                                <td>
-                                    <input class="input-sm form-control" type="number" step="0.1" v-model="entry.value">
-                                </td>
-                                <td>
-                                    <color-picker-input :color="entry.colorString" v-model="entry.colorString"></color-picker-input>
-                                </td>
-                                <td>
-                                    <a @click.prevent="addColor(index)">
-                                        <span class="icon-plus" title="Add row below"></span>
-                                    </a>
-                                    <a @click.prevent="removeColor(index)">
-                                        <span class="icon-minus" title="Remove this row"></span>
-                                    </a>
-                                </td>
-                            </tr>
-                            <tr v-if="this.type === 'griddata'">
-                                <td title="The color of values above the highest range value">
-                                    Maximum color
-                                </td>
-                                <td>
-                                    <color-picker-input :color="maxColor" v-model="maxColor"></color-picker-input>
-                                </td>
-                            </tr>
-                            </tbody>
-                        </table>
-                    </div>
-                    <div class="checkbox">
-                        <label><input type="checkbox" v-model="normalizeRange"> <b>Normalize Range</b></label>
-                    </div>
-                    <div v-if="this.type === 'heatmap'" class="checkbox">
-                        <label><input type="checkbox" v-model="scaleWithZoom"> <b>Scale With Zoom</b></label>
-                    </div>
-                    <div v-if="this.interpretation === 'contour' || this.interpretation === 'chloropleth'" class="checkbox">
-                        <label><input type="checkbox" v-model="stepped"> <b>Stepped</b></label>
-                    </div>
-                </div>
-                <div class="modal-footer">
-                    <button type="button" class="btn btn-default" @click.prevent="cancelDialog()" id="close">
-                        Cancel
-                    </button>
-                    <button type="button" class="btn btn-primary" @click.prevent="submitClicked()">
-                        Submit
-                    </button>
-                </div>
-            </form>
+  <div
+    v-if="colorRangeData"
+    class="modal-dialog"
+  >
+    <div class="modal-content">
+      <form class="modal-form">
+        <div class="modal-header">
+          <button
+            ref="close"
+            type="button"
+            class="close"
+            @click="cancelDialog()"
+          >
+            <span>&times;</span>
+          </button>
+          <h4>{{ headerMessage }}</h4>
+        </div>
+        <div class="modal-body">
+          <div
+            v-if="validationErrors.length > 0"
+            class="errors"
+          >
+            <p>Errors</p>
+            <ul>
+              <li
+                v-for="error in validationErrors"
+                :key="error"
+              >
+                {{ error }}
+              </li>
+            </ul>
+          </div>
+          <div
+            v-if="type === 'heatmap'"
+            class="form-group"
+          >
+            <label for="h-griddata-radius">Radius</label>
+            <input
+              id="h-griddata-radius"
+              v-model="radius"
+              class="input-sm form-control"
+              type="number"
+              min="1"
+            >
+          </div>
+          <div class="form-group">
+            <label for="h-griddata-range">Range Colors</label>
+            <table
+              id="h-griddata-range"
+              class="table table-bordered table-condensed"
+            >
+              <thead>
+                <tr>
+                  <th>Value</th>
+                  <th>Color</th>
+                  <th>
+                    <a @click.prevent="addNewFirstColor">
+                      <span
+                        class="icon-plus"
+                        title="Add new first color"
+                      />
+                    </a>
+                  </th>
+                </tr>
+              </thead>
+              <tbody>
+                <tr v-if="type === 'griddata'">
+                  <td title="The color of values below the lowest range value">
+                    Minimum color
+                  </td>
+                  <td>
+                    <color-picker-input
+                      v-model="minColor"
+                      :color="minColor"
+                    />
+                  </td>
+                </tr>
+                <tr
+                  v-for="(entry, index) in colorRangeData"
+                  :key="entry.key"
+                >
+                  <td>
+                    <input
+                      v-model="entry.value"
+                      class="input-sm form-control"
+                      type="number"
+                      step="0.1"
+                    >
+                  </td>
+                  <td>
+                    <color-picker-input
+                      v-model="entry.colorString"
+                      :color="entry.colorString"
+                    />
+                  </td>
+                  <td>
+                    <a @click.prevent="addColor(index)">
+                      <span
+                        class="icon-plus"
+                        title="Add row below"
+                      />
+                    </a>
+                    <a @click.prevent="removeColor(index)">
+                      <span
+                        class="icon-minus"
+                        title="Remove this row"
+                      />
+                    </a>
+                  </td>
+                </tr>
+                <tr v-if="type === 'griddata'">
+                  <td title="The color of values above the highest range value">
+                    Maximum color
+                  </td>
+                  <td>
+                    <color-picker-input
+                      v-model="maxColor"
+                      :color="maxColor"
+                    />
+                  </td>
+                </tr>
+              </tbody>
+            </table>
+          </div>
+          <div class="checkbox">
+            <label><input
+              v-model="normalizeRange"
+              type="checkbox"
+            > <b>Normalize Range</b></label>
+          </div>
+          <div
+            v-if="type === 'heatmap'"
+            class="checkbox"
+          >
+            <label><input
+              v-model="scaleWithZoom"
+              type="checkbox"
+            > <b>Scale With Zoom</b></label>
+          </div>
+          <div
+            v-if="interpretation === 'contour' || interpretation === 'chloropleth'"
+            class="checkbox"
+          >
+            <label><input
+              v-model="stepped"
+              type="checkbox"
+            > <b>Stepped</b></label>
+          </div>
+        </div>
+        <div class="modal-footer">
+          <button
+            id="close"
+            type="button"
+            class="btn btn-default"
+            @click.prevent="cancelDialog()"
+          >
+            Cancel
+          </button>
+          <button
+            type="button"
+            class="btn btn-primary"
+            @click.prevent="submitClicked()"
+          >
+            Submit
+          </button>
         </div>
+      </form>
     </div>
+  </div>
 </template>
```

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue` & `histomicsui-1.4.3.dev8/histomicsui/web_client/vue/components/EditHeatmapOrGridDataContainer.vue`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 <script>
 import _ from 'underscore';
 import Vue from 'vue';
 
 import EditHeatmapOrGridData from './EditHeatmapOrGridData.vue';
 export default Vue.extend({
+    components: {
+        EditHeatmapOrGridData
+    },
     props: ['element', 'parentView'],
     data() {
         return {
             attributes: _.clone(this.element.attributes || {})
         };
     },
     methods: {
         handleSubmit(propsToSave) {
             this.element.set(propsToSave);
             this.close();
         },
         close() {
             this.parentView.closeVueModal();
         }
-    },
-    components: {
-        EditHeatmapOrGridData
     }
-})
+});
 </script>
 
 <template>
-    <div>
-        <edit-heatmap-or-grid-data
-            :elementData="this.attributes"
-            @submit="handleSubmit"
-            @cancel="close"
-        >
-        </edit-heatmap-or-grid-data>
-    </div>
+  <div>
+    <edit-heatmap-or-grid-data
+      :element-data="attributes"
+      @submit="handleSubmit"
+      @cancel="close"
+    />
+  </div>
 </template>
```

### Comparing `histomicsui-1.4.3.dev5/histomicsui/web_client/webpack.helper.js` & `histomicsui-1.4.3.dev8/histomicsui/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui/webroot.mako` & `histomicsui-1.4.3.dev8/histomicsui/webroot.mako`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/histomicsui.egg-info/PKG-INFO` & `histomicsui-1.4.3.dev8/histomicsui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicsui
-Version: 1.4.3.dev5
+Version: 1.4.3.dev8
 Summary: Organize, visualize, and analyze histology images.
 Home-page: https://github.com/DigitalSlideArchive/histomicsui
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,histomicsui
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicsui-1.4.3.dev5/histomicsui.egg-info/SOURCES.txt` & `histomicsui-1.4.3.dev8/histomicsui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/setup.py` & `histomicsui-1.4.3.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/datastore.py` & `histomicsui-1.4.3.dev8/tests/datastore.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/girder_utilities.py` & `histomicsui-1.4.3.dev8/tests/girder_utilities.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_files/.histomicsui_config.yaml` & `histomicsui-1.4.3.dev8/tests/test_files/.histomicsui_config.yaml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_files/test_analysis_detection.xml` & `histomicsui-1.4.3.dev8/tests/test_files/test_analysis_detection.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_files/test_analysis_features.xml` & `histomicsui-1.4.3.dev8/tests/test_files/test_analysis_features.xml`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_handlers.py` & `histomicsui-1.4.3.dev8/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_hui_rest.py` & `histomicsui-1.4.3.dev8/tests/test_hui_rest.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_image_browse_endpoints.py` & `histomicsui-1.4.3.dev8/tests/test_image_browse_endpoints.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_tcga.py` & `histomicsui-1.4.3.dev8/tests/test_tcga.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/test_web_client.py` & `histomicsui-1.4.3.dev8/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/analysisSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/analysisSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/annotationSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/annotationSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/girderUISpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/girderUISpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/huiSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/huiSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/huiTest.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/huiTest.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/itemSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/itemSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/metadataPanelSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/metadataPlotSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/metadataPlotSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/overviewPanelSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/overviewPanelSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/panelLayoutSpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/panelLayoutSpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tests/web_client_specs/pixelmapCategorySpec.js` & `histomicsui-1.4.3.dev8/tests/web_client_specs/pixelmapCategorySpec.js`

 * *Files identical despite different names*

### Comparing `histomicsui-1.4.3.dev5/tox.ini` & `histomicsui-1.4.3.dev8/tox.ini`

 * *Files identical despite different names*

