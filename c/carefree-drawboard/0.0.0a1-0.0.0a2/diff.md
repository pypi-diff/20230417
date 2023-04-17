# Comparing `tmp/carefree-drawboard-0.0.0a1.tar.gz` & `tmp/carefree-drawboard-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-drawboard-0.0.0a1.tar", last modified: Mon Apr 17 02:59:31 2023, max compression
+gzip compressed data, was "carefree-drawboard-0.0.0a2.tar", last modified: Mon Apr 17 03:19:32 2023, max compression
```

## Comparing `carefree-drawboard-0.0.0a1.tar` & `carefree-drawboard-0.0.0a2.tar`

### file list

```diff
@@ -1,186 +1,188 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.423367 carefree-drawboard-0.0.0a1/
--rw-rw-rw-   0        0        0      119 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/.env
--rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a1/LICENSE
--rw-rw-rw-   0        0        0      202 2023-04-17 02:58:27.000000 carefree-drawboard-0.0.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     8807 2023-04-17 02:59:31.423367 carefree-drawboard-0.0.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     8524 2023-04-17 02:49:50.000000 carefree-drawboard-0.0.0a1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.373603 carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/
--rw-rw-rw-   0        0        0     8807 2023-04-17 02:59:31.000000 carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3978 2023-04-17 02:59:31.000000 carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:59:31.000000 carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 02:59:31.000000 carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      147 2023-04-17 02:59:31.000000 carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 02:59:31.000000 carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.375599 carefree-drawboard-0.0.0a1/cfdraw/
--rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a1/cfdraw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.376596 carefree-drawboard-0.0.0a1/cfdraw/app/
--rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/app/__init__.py
--rw-rw-rw-   0        0        0     2905 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/app/app.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.379070 carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/
--rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/__init__.py
--rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/base.py
--rw-rw-rw-   0        0        0     1907 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/plugins.py
--rw-rw-rw-   0        0        0     5653 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/project.py
--rw-rw-rw-   0        0        0     1813 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/upload.py
--rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/websocket.py
--rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/app/schema.py
--rw-rw-rw-   0        0        0     2569 2023-04-16 17:34:51.000000 carefree-drawboard-0.0.0a1/cfdraw/cli.py
--rw-rw-rw-   0        0        0     1459 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/config.py
--rw-rw-rw-   0        0        0      962 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.380066 carefree-drawboard-0.0.0a1/cfdraw/parsers/
--rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a1/cfdraw/parsers/__init__.py
--rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a1/cfdraw/parsers/chakra.py
--rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/parsers/noli.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.382469 carefree-drawboard-0.0.0a1/cfdraw/plugins/
--rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/base.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.382469 carefree-drawboard-0.0.0a1/cfdraw/plugins/community/
--rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/community/__init__.py
--rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/factory.py
--rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/meta.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.383471 carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/
--rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/fields.py
--rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/text_area.py
--rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/timer.py
--rw-rw-rw-   0        0        0     1090 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/plugins/sync.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.384468 carefree-drawboard-0.0.0a1/cfdraw/schema/
--rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a1/cfdraw/schema/__init__.py
--rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a1/cfdraw/schema/fields.py
--rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/schema/plugins.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.387458 carefree-drawboard-0.0.0a1/cfdraw/utils/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/cache.py
--rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/console.py
--rw-rw-rw-   0        0        0     1220 2023-04-16 15:33:22.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/exec.py
--rw-rw-rw-   0        0        0      636 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/prerequisites.py
--rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/processes.py
--rw-rw-rw-   0        0        0     3667 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/server.py
--rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/cfdraw/utils/template.py
--rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a1/index.html
--rw-rw-rw-   0        0        0     1526 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a1/package.json
--rw-rw-rw-   0        0        0      113 2023-04-17 02:59:31.426357 carefree-drawboard-0.0.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-04-17 02:59:02.000000 carefree-drawboard-0.0.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.389584 carefree-drawboard-0.0.0a1/src/
--rw-rw-rw-   0        0        0      901 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a1/src/App.tsx
--rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/_settings.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.392573 carefree-drawboard-0.0.0a1/src/actions/
--rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/addImage.ts
--rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/addText.ts
--rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/arrange.ts
--rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/download.ts
--rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/export.ts
--rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/importMeta.ts
--rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/actions/managePlugins.ts
--rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/manageProjects.ts
--rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/update.ts
--rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/actions/uploadImage.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.351111 carefree-drawboard-0.0.0a1/src/assets/
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.393995 carefree-drawboard-0.0.0a1/src/assets/icons/
--rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a1/src/assets/icons/arrow-down.svg
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.393995 carefree-drawboard-0.0.0a1/src/board/
--rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/board/BoardPanel.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.396988 carefree-drawboard-0.0.0a1/src/components/
--rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFButton.tsx
--rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFDivider.tsx
--rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFHeading.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.397985 carefree-drawboard-0.0.0a1/src/components/CFIcon/
--rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a1/src/components/CFIcon/index.scss
--rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFIcon/index.tsx
--rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/components/CFImageUploader.tsx
--rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFInput.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.397985 carefree-drawboard-0.0.0a1/src/components/CFSelect/
--rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a1/src/components/CFSelect/index.scss
--rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFSelect/index.tsx
--rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFSlider.tsx
--rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/components/CFSwitch.tsx
--rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/components/CFText.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.399978 carefree-drawboard-0.0.0a1/src/hooks/
--rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/hooks/useFileDropper.ts
--rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/hooks/useGridLines.ts
--rw-rw-rw-   0        0        0     3048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/hooks/useInitBoard.ts
--rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a1/src/hooks/usePreventDefaults.ts
--rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/hooks/usePython.ts
--rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/hooks/useUndoRedo.ts
--rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a1/src/index.scss
--rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a1/src/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.403965 carefree-drawboard-0.0.0a1/src/lang/
--rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/add.ts
--rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/brush.ts
--rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/download.ts
--rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/index.ts
--rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/nodeEditor.ts
--rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/plugins.ts
--rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/projects.ts
--rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/settings.ts
--rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/toast.ts
--rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/lang/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.407951 carefree-drawboard-0.0.0a1/src/plugins/
--rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/AddPlugin.tsx
--rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/ArrangePlugin.tsx
--rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/BrushPlugin.tsx
--rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/DeletePlugin.tsx
--rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/DownloadPlugin.tsx
--rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/GroupPlugin.tsx
--rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/LinksPlugin.tsx
--rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/ProjectPlugin.tsx
--rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/SettingsPlugin.tsx
--rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/TextEditorPlugin.tsx
--rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/UndoRedoPlugin.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.409945 carefree-drawboard-0.0.0a1/src/plugins/_python/
--rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/_python/HttpFieldsPlugin.tsx
--rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/_python/HttpPluginWithSubmit.tsx
--rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/_python/HttpQAPlugin.tsx
--rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/_python/HttpTextAreaPlugin.tsx
--rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a1/src/plugins/_python/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.411400 carefree-drawboard-0.0.0a1/src/plugins/components/
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.413401 carefree-drawboard-0.0.0a1/src/plugins/components/Fields/
--rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Fields/NumberField.tsx
--rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Fields/SelectField.tsx
--rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Fields/TextField.tsx
--rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Fields/index.tsx
--rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Fields/utils.ts
--rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Floating.tsx
--rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Link.tsx
--rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/components/Render.tsx
--rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/index.tsx
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.414397 carefree-drawboard-0.0.0a1/src/plugins/utils/
--rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/utils/factory.ts
--rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/plugins/utils/renderFilters.ts
--rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a1/src/react-app-env.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.414397 carefree-drawboard-0.0.0a1/src/requests/
--rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a1/src/requests/actions.ts
--rw-rw-rw-   0        0        0     3411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/requests/hooks.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.415394 carefree-drawboard-0.0.0a1/src/requests/interceptors/
--rw-rw-rw-   0        0        0      824 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/requests/interceptors/_python.ts
--rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a1/src/requests/interceptors/index.ts
--rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a1/src/reset.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.417387 carefree-drawboard-0.0.0a1/src/schema/
--rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/schema/_python.ts
--rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/schema/meta.ts
--rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/schema/metaFields.ts
--rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a1/src/schema/misc.ts
--rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/schema/plugins.ts
--rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a1/src/schema/requests.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.421374 carefree-drawboard-0.0.0a1/src/stores/
--rw-rw-rw-   0        0        0     1431 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/_python.ts
--rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/gridLines.ts
--rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/hooks.ts
--rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/init.ts
--rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/meta.ts
--rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/plugins.ts
--rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/projects.ts
--rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/theme.ts
--rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a1/src/stores/ui.ts
-drwxrwxrwx   0        0        0        0 2023-04-17 02:59:31.423367 carefree-drawboard-0.0.0a1/src/utils/
--rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a1/src/utils/bem.ts
--rw-rw-rw-   0        0        0      546 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a1/src/utils/constants.ts
--rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a1/src/utils/event.ts
--rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a1/src/utils/misc.ts
--rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a1/src/utils/toast.ts
--rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a1/src/vite-env.d.ts
--rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a1/tsconfig.json
--rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a1/tsconfig.node.json
--rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a1/tsconfig.paths.json
--rw-rw-rw-   0        0        0      594 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a1/vite.config.ts
--rw-rw-rw-   0        0        0   210103 2023-04-16 17:37:05.000000 carefree-drawboard-0.0.0a1/yarn.lock
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.056273 carefree-drawboard-0.0.0a2/
+-rw-rw-rw-   0        0        0    11557 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a2/LICENSE
+-rw-rw-rw-   0        0        0       63 2023-04-17 03:16:55.000000 carefree-drawboard-0.0.0a2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8807 2023-04-17 03:19:32.056273 carefree-drawboard-0.0.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0     8524 2023-04-17 02:49:50.000000 carefree-drawboard-0.0.0a2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.001106 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/
+-rw-rw-rw-   0        0        0     8807 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-04-17 03:19:31.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      147 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 03:19:30.000000 carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.003449 carefree-drawboard-0.0.0a2/cfdraw/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.006439 carefree-drawboard-0.0.0a2/cfdraw/.web/
+-rw-rw-rw-   0        0        0      119 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/.env
+-rw-rw-rw-   0        0        0      143 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/.prettierrc
+-rw-rw-rw-   0        0        0      323 2023-04-13 08:34:20.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/index.html
+-rw-rw-rw-   0        0        0     1526 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/package.json
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.009429 carefree-drawboard-0.0.0a2/cfdraw/.web/src/
+-rw-rw-rw-   0        0        0      901 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/App.tsx
+-rw-rw-rw-   0        0        0     5434 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/_settings.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.013415 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/
+-rw-rw-rw-   0        0        0     2263 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addImage.ts
+-rw-rw-rw-   0        0        0      960 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addText.ts
+-rw-rw-rw-   0        0        0     9573 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/arrange.ts
+-rw-rw-rw-   0        0        0     1930 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/download.ts
+-rw-rw-rw-   0        0        0     2174 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/export.ts
+-rw-rw-rw-   0        0        0     5947 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/importMeta.ts
+-rw-rw-rw-   0        0        0     1286 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/managePlugins.ts
+-rw-rw-rw-   0        0        0     3528 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/manageProjects.ts
+-rw-rw-rw-   0        0        0      272 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/update.ts
+-rw-rw-rw-   0        0        0     1175 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/uploadImage.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:31.981040 carefree-drawboard-0.0.0a2/cfdraw/.web/src/assets/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.013415 carefree-drawboard-0.0.0a2/cfdraw/.web/src/assets/icons/
+-rw-rw-rw-   0        0        0      257 2022-10-23 15:19:01.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/assets/icons/arrow-down.svg
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.014413 carefree-drawboard-0.0.0a2/cfdraw/.web/src/board/
+-rw-rw-rw-   0        0        0     1453 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/board/BoardPanel.tsx
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.017402 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/
+-rw-rw-rw-   0        0        0      353 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFButton.tsx
+-rw-rw-rw-   0        0        0      359 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFDivider.tsx
+-rw-rw-rw-   0        0        0      243 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFHeading.tsx
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.017402 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/
+-rw-rw-rw-   0        0        0      546 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.scss
+-rw-rw-rw-   0        0        0     1568 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.tsx
+-rw-rw-rw-   0        0        0     1568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFImageUploader.tsx
+-rw-rw-rw-   0        0        0      346 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFInput.tsx
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.018400 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/
+-rw-rw-rw-   0        0        0       70 2023-04-07 06:01:04.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/index.scss
+-rw-rw-rw-   0        0        0     3483 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/index.tsx
+-rw-rw-rw-   0        0        0     4606 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSlider.tsx
+-rw-rw-rw-   0        0        0     1644 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSwitch.tsx
+-rw-rw-rw-   0        0        0      324 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFText.tsx
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.020392 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/
+-rw-rw-rw-   0        0        0     3110 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useFileDropper.ts
+-rw-rw-rw-   0        0        0     4289 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useGridLines.ts
+-rw-rw-rw-   0        0        0     3048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useInitBoard.ts
+-rw-rw-rw-   0        0        0      445 2023-04-11 05:03:17.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/usePreventDefaults.ts
+-rw-rw-rw-   0        0        0     5003 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/usePython.ts
+-rw-rw-rw-   0        0        0      394 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useUndoRedo.ts
+-rw-rw-rw-   0        0        0      131 2023-04-07 08:12:13.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/index.scss
+-rw-rw-rw-   0        0        0      345 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.024379 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/
+-rw-rw-rw-   0        0        0      792 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/add.ts
+-rw-rw-rw-   0        0        0      849 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/brush.ts
+-rw-rw-rw-   0        0        0     1148 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/download.ts
+-rw-rw-rw-   0        0        0     1436 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/index.ts
+-rw-rw-rw-   0        0        0      404 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/nodeEditor.ts
+-rw-rw-rw-   0        0        0     2283 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/plugins.ts
+-rw-rw-rw-   0        0        0     1746 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/projects.ts
+-rw-rw-rw-   0        0        0      896 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/settings.ts
+-rw-rw-rw-   0        0        0     6568 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/toast.ts
+-rw-rw-rw-   0        0        0     1472 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.029363 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/
+-rw-rw-rw-   0        0        0     2839 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/AddPlugin.tsx
+-rw-rw-rw-   0        0        0      870 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ArrangePlugin.tsx
+-rw-rw-rw-   0        0        0     4801 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/BrushPlugin.tsx
+-rw-rw-rw-   0        0        0      879 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DeletePlugin.tsx
+-rw-rw-rw-   0        0        0     3545 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DownloadPlugin.tsx
+-rw-rw-rw-   0        0        0     1067 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/GroupPlugin.tsx
+-rw-rw-rw-   0        0        0     1101 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/LinksPlugin.tsx
+-rw-rw-rw-   0        0        0     6511 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ProjectPlugin.tsx
+-rw-rw-rw-   0        0        0     5093 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/SettingsPlugin.tsx
+-rw-rw-rw-   0        0        0     2366 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/TextEditorPlugin.tsx
+-rw-rw-rw-   0        0        0      906 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.031355 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/
+-rw-rw-rw-   0        0        0     3607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx
+-rw-rw-rw-   0        0        0     2064 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx
+-rw-rw-rw-   0        0        0     1951 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx
+-rw-rw-rw-   0        0        0     1602 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx
+-rw-rw-rw-   0        0        0      258 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.032352 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.034346 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/
+-rw-rw-rw-   0        0        0     1411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx
+-rw-rw-rw-   0        0        0      693 2023-04-13 06:08:57.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx
+-rw-rw-rw-   0        0        0      854 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/TextField.tsx
+-rw-rw-rw-   0        0        0     1133 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/index.tsx
+-rw-rw-rw-   0        0        0      614 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/utils.ts
+-rw-rw-rw-   0        0        0     7481 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Floating.tsx
+-rw-rw-rw-   0        0        0      307 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Link.tsx
+-rw-rw-rw-   0        0        0     7048 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Render.tsx
+-rw-rw-rw-   0        0        0     2318 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/index.tsx
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.035343 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/
+-rw-rw-rw-   0        0        0     1575 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/factory.ts
+-rw-rw-rw-   0        0        0      583 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/renderFilters.ts
+-rw-rw-rw-   0        0        0      841 2023-04-06 03:20:54.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/react-app-env.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.035343 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/
+-rw-rw-rw-   0        0        0      922 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/actions.ts
+-rw-rw-rw-   0        0        0     3411 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/hooks.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.036339 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/
+-rw-rw-rw-   0        0        0      824 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/_python.ts
+-rw-rw-rw-   0        0        0      752 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/index.ts
+-rw-rw-rw-   0        0        0       38 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/reset.d.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.038332 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/
+-rw-rw-rw-   0        0        0     3348 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/_python.ts
+-rw-rw-rw-   0        0        0     1607 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/meta.ts
+-rw-rw-rw-   0        0        0     1169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/metaFields.ts
+-rw-rw-rw-   0        0        0      289 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/misc.ts
+-rw-rw-rw-   0        0        0     3169 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/plugins.ts
+-rw-rw-rw-   0        0        0      850 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/requests.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.041322 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/
+-rw-rw-rw-   0        0        0     1431 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/_python.ts
+-rw-rw-rw-   0        0        0     1495 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/gridLines.ts
+-rw-rw-rw-   0        0        0      578 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/hooks.ts
+-rw-rw-rw-   0        0        0      468 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/init.ts
+-rw-rw-rw-   0        0        0     1107 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/meta.ts
+-rw-rw-rw-   0        0        0     1561 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/plugins.ts
+-rw-rw-rw-   0        0        0     1704 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/projects.ts
+-rw-rw-rw-   0        0        0     3285 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/theme.ts
+-rw-rw-rw-   0        0        0     2025 2023-04-16 17:25:23.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/ui.ts
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.043316 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/
+-rw-rw-rw-   0        0        0      467 2023-04-07 05:25:36.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/bem.ts
+-rw-rw-rw-   0        0        0      546 2023-04-16 14:44:15.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/constants.ts
+-rw-rw-rw-   0        0        0      934 2023-04-06 06:11:04.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/event.ts
+-rw-rw-rw-   0        0        0     1025 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/misc.ts
+-rw-rw-rw-   0        0        0      633 2023-04-14 05:06:48.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/toast.ts
+-rw-rw-rw-   0        0        0       39 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/src/vite-env.d.ts
+-rw-rw-rw-   0        0        0      656 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.node.json
+-rw-rw-rw-   0        0        0      103 2023-04-06 01:57:35.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.paths.json
+-rw-rw-rw-   0        0        0      594 2023-04-16 17:25:21.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/vite.config.ts
+-rw-rw-rw-   0        0        0   210103 2023-04-16 17:37:05.000000 carefree-drawboard-0.0.0a2/cfdraw/.web/yarn.lock
+-rw-rw-rw-   0        0        0      405 2023-04-13 06:43:12.000000 carefree-drawboard-0.0.0a2/cfdraw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.044313 carefree-drawboard-0.0.0a2/cfdraw/app/
+-rw-rw-rw-   0        0        0       20 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/__init__.py
+-rw-rw-rw-   0        0        0     2905 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/app.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.047303 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/
+-rw-rw-rw-   0        0        0      118 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/base.py
+-rw-rw-rw-   0        0        0     1907 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/plugins.py
+-rw-rw-rw-   0        0        0     5653 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/project.py
+-rw-rw-rw-   0        0        0     1813 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/upload.py
+-rw-rw-rw-   0        0        0     2974 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/websocket.py
+-rw-rw-rw-   0        0        0      519 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/app/schema.py
+-rw-rw-rw-   0        0        0     2569 2023-04-16 17:34:51.000000 carefree-drawboard-0.0.0a2/cfdraw/cli.py
+-rw-rw-rw-   0        0        0     1459 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/config.py
+-rw-rw-rw-   0        0        0      955 2023-04-17 03:06:49.000000 carefree-drawboard-0.0.0a2/cfdraw/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.048299 carefree-drawboard-0.0.0a2/cfdraw/parsers/
+-rw-rw-rw-   0        0        0       44 2023-04-09 01:57:56.000000 carefree-drawboard-0.0.0a2/cfdraw/parsers/__init__.py
+-rw-rw-rw-   0        0        0      609 2023-04-12 06:16:04.000000 carefree-drawboard-0.0.0a2/cfdraw/parsers/chakra.py
+-rw-rw-rw-   0        0        0     6203 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/parsers/noli.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.050292 carefree-drawboard-0.0.0a2/cfdraw/plugins/
+-rw-rw-rw-   0        0        0      113 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4367 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/base.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.050292 carefree-drawboard-0.0.0a2/cfdraw/plugins/community/
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:16:37.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/community/__init__.py
+-rw-rw-rw-   0        0        0     2407 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/factory.py
+-rw-rw-rw-   0        0        0     1956 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/meta.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.052286 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/
+-rw-rw-rw-   0        0        0       71 2023-04-13 03:23:59.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/fields.py
+-rw-rw-rw-   0        0        0      671 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/text_area.py
+-rw-rw-rw-   0        0        0      795 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/timer.py
+-rw-rw-rw-   0        0        0     1090 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/plugins/sync.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.053282 carefree-drawboard-0.0.0a2/cfdraw/schema/
+-rw-rw-rw-   0        0        0       47 2023-04-13 15:19:11.000000 carefree-drawboard-0.0.0a2/cfdraw/schema/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-04-13 06:12:19.000000 carefree-drawboard-0.0.0a2/cfdraw/schema/fields.py
+-rw-rw-rw-   0        0        0     9673 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/schema/plugins.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:19:32.056273 carefree-drawboard-0.0.0a2/cfdraw/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:23:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/cache.py
+-rw-rw-rw-   0        0        0      875 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/console.py
+-rw-rw-rw-   0        0        0     1222 2023-04-17 03:07:11.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/exec.py
+-rw-rw-rw-   0        0        0      638 2023-04-17 03:07:08.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/prerequisites.py
+-rw-rw-rw-   0        0        0     1766 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/processes.py
+-rw-rw-rw-   0        0        0     3667 2023-04-17 02:32:05.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/server.py
+-rw-rw-rw-   0        0        0     2733 2023-04-16 14:44:14.000000 carefree-drawboard-0.0.0a2/cfdraw/utils/template.py
+-rw-rw-rw-   0        0        0      113 2023-04-17 03:19:32.057269 carefree-drawboard-0.0.0a2/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2023-04-17 03:12:52.000000 carefree-drawboard-0.0.0a2/setup.py
```

### Comparing `carefree-drawboard-0.0.0a1/LICENSE` & `carefree-drawboard-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/PKG-INFO` & `carefree-drawboard-0.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `carefree-drawboard-0.0.0a1/README.md` & `carefree-drawboard-0.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/carefree_drawboard.egg-info/PKG-INFO` & `carefree-drawboard-0.0.0a2/carefree_drawboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-drawboard
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: 🎨 Infinite Drawboard in Python
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn drawboard
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/app/app.py` & `carefree-drawboard-0.0.0a2/cfdraw/app/app.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/plugins.py` & `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/plugins.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/project.py` & `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/upload.py` & `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/upload.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/app/endpoints/websocket.py` & `carefree-drawboard-0.0.0a2/cfdraw/app/endpoints/websocket.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/app/schema.py` & `carefree-drawboard-0.0.0a2/cfdraw/app/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/cli.py` & `carefree-drawboard-0.0.0a2/cfdraw/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/config.py` & `carefree-drawboard-0.0.0a2/cfdraw/config.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/constants.py` & `carefree-drawboard-0.0.0a2/cfdraw/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,13 +38,13 @@
     ERROR = "error"
     CRITICAL = "critical"
 
 
 # directories
 ## common
 ROOT = Path(os.path.dirname(__file__))
-PARENT = ROOT.parent.absolute()
+WEB_ROOT = ROOT / ".web"
 ## upload
 UPLOAD_ROOT = Path("~").expanduser() / ".cache" / "carefree-draw"
 UPLOAD_IMAGE_FOLDER_NAME = ".images"
 UPLOAD_PROJECT_FOLDER_NAME = ".projects"
 PROJECT_META_FILE = "_meta.json"
```

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/parsers/chakra.py` & `carefree-drawboard-0.0.0a2/cfdraw/parsers/chakra.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/parsers/noli.py` & `carefree-drawboard-0.0.0a2/cfdraw/parsers/noli.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/plugins/base.py` & `carefree-drawboard-0.0.0a2/cfdraw/plugins/base.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/plugins/factory.py` & `carefree-drawboard-0.0.0a2/cfdraw/plugins/factory.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/plugins/meta.py` & `carefree-drawboard-0.0.0a2/cfdraw/plugins/meta.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/fields.py` & `carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/text_area.py` & `carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/text_area.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/plugins/middlewares/timer.py` & `carefree-drawboard-0.0.0a2/cfdraw/plugins/middlewares/timer.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/plugins/sync.py` & `carefree-drawboard-0.0.0a2/cfdraw/plugins/sync.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/schema/fields.py` & `carefree-drawboard-0.0.0a2/cfdraw/schema/fields.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/schema/plugins.py` & `carefree-drawboard-0.0.0a2/cfdraw/schema/plugins.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/utils/cache.py` & `carefree-drawboard-0.0.0a2/cfdraw/utils/cache.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/utils/console.py` & `carefree-drawboard-0.0.0a2/cfdraw/utils/console.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/utils/exec.py` & `carefree-drawboard-0.0.0a2/cfdraw/utils/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     prerequisites.install_frontend_packages()
     console.rule("[bold green]Launching App")
     os.environ["CFDRAW_FE_PORT"] = fe_port
     os.environ["CFDRAW_BE_PORT"] = be_port
     print_info(f"Your app will be ready at http://localhost:{fe_port}")
     subprocess.Popen(
         [prerequisites.get_yarn(), "dev", "--force"],
-        cwd=constants.PARENT,
+        cwd=constants.WEB_ROOT,
         env=os.environ,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.STDOUT,
     )
 
 
 def run_backend(
```

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/utils/prerequisites.py` & `carefree-drawboard-0.0.0a2/cfdraw/utils/prerequisites.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     if yarn_path is None:
         raise FileNotFoundError("cfdraw requires yarn to be installed.")
     return yarn_path
 
 
 def install_frontend_packages(*, verbose: bool = False) -> None:
     console.rule("[bold]Installing frontend packages")
-    kw: Dict[str, Any] = dict(cwd=constants.PARENT)
+    kw: Dict[str, Any] = dict(cwd=constants.WEB_ROOT)
     if not verbose:
         kw["stdout"] = subprocess.PIPE
     subprocess.run([get_yarn()], **kw)  # type: ignore
```

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/utils/processes.py` & `carefree-drawboard-0.0.0a2/cfdraw/utils/processes.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/utils/server.py` & `carefree-drawboard-0.0.0a2/cfdraw/utils/server.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/cfdraw/utils/template.py` & `carefree-drawboard-0.0.0a2/cfdraw/utils/template.py`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/package.json` & `carefree-drawboard-0.0.0a2/cfdraw/.web/package.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/setup.py` & `carefree-drawboard-0.0.0a2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.0-alpha.1"
+VERSION = "0.0.0-alpha.2"
 PACKAGE_NAME = "carefree-drawboard"
 
 DESCRIPTION = "🎨 Infinite Drawboard in Python"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

### Comparing `carefree-drawboard-0.0.0a1/src/App.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/App.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/_settings.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/_settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/addImage.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/addText.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/addText.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/arrange.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/arrange.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/download.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/export.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/export.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/importMeta.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/importMeta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/managePlugins.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/managePlugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/manageProjects.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/manageProjects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/actions/uploadImage.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/actions/uploadImage.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/board/BoardPanel.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/board/BoardPanel.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/components/CFIcon/index.scss` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.scss`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/components/CFIcon/index.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFIcon/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/components/CFImageUploader.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFImageUploader.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/components/CFSelect/index.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSelect/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/components/CFSlider.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSlider.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/components/CFSwitch.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/components/CFSwitch.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/hooks/useFileDropper.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useFileDropper.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/hooks/useGridLines.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useGridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/hooks/useInitBoard.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/useInitBoard.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/hooks/usePython.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/hooks/usePython.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/add.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/add.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/brush.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/brush.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/download.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/download.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/index.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/plugins.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/projects.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/settings.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/settings.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/toast.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/lang/ui.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/lang/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/AddPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/AddPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/ArrangePlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ArrangePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/BrushPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/BrushPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/DeletePlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DeletePlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/DownloadPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/DownloadPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/GroupPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/GroupPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/LinksPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/LinksPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/ProjectPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/ProjectPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/SettingsPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/SettingsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/TextEditorPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/TextEditorPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/UndoRedoPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/UndoRedoPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/_python/HttpFieldsPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpFieldsPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/_python/HttpPluginWithSubmit.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpPluginWithSubmit.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/_python/HttpQAPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpQAPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/_python/HttpTextAreaPlugin.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/_python/HttpTextAreaPlugin.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/components/Fields/NumberField.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/NumberField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/components/Fields/SelectField.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/SelectField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/components/Fields/TextField.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/TextField.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/components/Fields/index.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/components/Fields/utils.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Fields/utils.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/components/Floating.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Floating.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/components/Render.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/components/Render.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/index.tsx` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/index.tsx`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/utils/factory.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/factory.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/plugins/utils/renderFilters.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/plugins/utils/renderFilters.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/react-app-env.d.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/react-app-env.d.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/requests/actions.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/actions.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/requests/hooks.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/requests/interceptors/_python.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/requests/interceptors/index.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/requests/interceptors/index.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/schema/_python.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/schema/meta.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/schema/metaFields.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/metaFields.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/schema/plugins.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/schema/requests.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/schema/requests.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/_python.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/_python.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/gridLines.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/gridLines.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/hooks.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/hooks.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/meta.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/meta.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/plugins.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/plugins.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/projects.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/projects.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/theme.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/theme.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/stores/ui.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/stores/ui.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/utils/constants.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/constants.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/utils/event.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/event.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/utils/misc.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/misc.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/src/utils/toast.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/src/utils/toast.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/tsconfig.json` & `carefree-drawboard-0.0.0a2/cfdraw/.web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/vite.config.ts` & `carefree-drawboard-0.0.0a2/cfdraw/.web/vite.config.ts`

 * *Files identical despite different names*

### Comparing `carefree-drawboard-0.0.0a1/yarn.lock` & `carefree-drawboard-0.0.0a2/cfdraw/.web/yarn.lock`

 * *Files identical despite different names*

