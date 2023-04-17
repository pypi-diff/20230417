# Comparing `tmp/pyTermTk-0.9.0a56.tar.gz` & `tmp/pyTermTk-0.9.0a62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTermTk-0.9.0a56.tar", last modified: Wed May 18 09:20:34 2022, max compression
+gzip compressed data, was "pyTermTk-0.9.0a62.tar", last modified: Thu Jun  9 11:08:40 2022, max compression
```

## Comparing `pyTermTk-0.9.0a56.tar` & `pyTermTk-0.9.0a62.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.269006 pyTermTk-0.9.0a56/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/LICENSE
--rw-rw-r--   0 one       (1000) one       (1000)     6382 2022-05-18 09:20:34.269006 pyTermTk-0.9.0a56/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     5652 2022-05-17 21:18:14.000000 pyTermTk-0.9.0a56/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2022-05-18 09:20:34.269006 pyTermTk-0.9.0a56/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1276 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.253006 pyTermTk-0.9.0a56/tmp/
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.253006 pyTermTk-0.9.0a56/tmp/TermTk/
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.257006 pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/
--rw-rw-r--   0 one       (1000) one       (1000)       67 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1416 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/abstractitemmodel.py
--rw-rw-r--   0 one       (1000) one       (1000)     5194 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/abstractscrollarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     3377 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/abstractscrollview.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.257006 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.257006 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/
--rw-rw-r--   0 one       (1000) one       (1000)      163 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     2158 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/colors.py
--rw-rw-r--   0 one       (1000) one       (1000)     5936 2022-05-18 09:19:09.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/input.py
--rw-rw-r--   0 one       (1000) one       (1000)    43749 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/inputkey.py
--rw-rw-r--   0 one       (1000) one       (1000)     4663 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/inputmouse.py
--rw-rw-r--   0 one       (1000) one       (1000)     2415 2022-05-18 09:09:22.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/readinputlinux.py
--rw-rw-r--   0 one       (1000) one       (1000)     5906 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/term.py
--rw-rw-r--   0 one       (1000) one       (1000)      254 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)    26500 2022-04-19 13:53:21.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/canvas.py
--rw-rw-r--   0 one       (1000) one       (1000)     1453 2022-05-18 09:20:28.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)    10786 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/color.py
--rw-rw-r--   0 one       (1000) one       (1000)    35175 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/constant.py
--rw-rw-r--   0 one       (1000) one       (1000)     3608 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/drag.py
--rw-rw-r--   0 one       (1000) one       (1000)     1182 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/draw.py
--rw-rw-r--   0 one       (1000) one       (1000)     6292 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/filebuffer.py
--rw-rw-r--   0 one       (1000) one       (1000)    15115 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/helper.py
--rw-rw-r--   0 one       (1000) one       (1000)     3893 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/log.py
--rw-rw-r--   0 one       (1000) one       (1000)     6460 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/signal.py
--rw-rw-r--   0 one       (1000) one       (1000)    15235 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/string.py
--rw-rw-r--   0 one       (1000) one       (1000)     2702 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/timer.py
--rw-rw-r--   0 one       (1000) one       (1000)    10745 2022-05-18 09:03:46.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/ttk.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.261006 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/
--rw-rw-r--   0 one       (1000) one       (1000)       20 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     4088 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/draw_ascii.py
--rw-rw-r--   0 one       (1000) one       (1000)    10632 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/draw_utf8.py
--rw-rw-r--   0 one       (1000) one       (1000)     1339 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/fileicon_ascii.py
--rw-rw-r--   0 one       (1000) one       (1000)     9267 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/fileicon_nerd.py
--rw-rw-r--   0 one       (1000) one       (1000)     1345 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/fileicon_utf8.py
--rw-rw-r--   0 one       (1000) one       (1000)    10579 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/theme.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.261006 pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/
--rw-rw-r--   0 one       (1000) one       (1000)      140 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     3074 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/boxlayout.py
--rw-rw-r--   0 one       (1000) one       (1000)    14538 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/gridlayout.py
--rw-rw-r--   0 one       (1000) one       (1000)    13904 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/layout.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.261006 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/
--rw-rw-r--   0 one       (1000) one       (1000)        0 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1675 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/color.py
--rw-rw-r--   0 one       (1000) one       (1000)     1551 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/data.py
--rw-rw-r--   0 one       (1000) one       (1000)     2928 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/dragevents.py
--rw-rw-r--   0 one       (1000) one       (1000)     2552 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/keyevents.py
--rw-rw-r--   0 one       (1000) one       (1000)     5313 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/mouseevents.py
--rw-rw-r--   0 one       (1000) one       (1000)     1551 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/text.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.261006 pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/
--rw-rw-r--   0 one       (1000) one       (1000)       83 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     4329 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/logviewer.py
--rw-rw-r--   0 one       (1000) one       (1000)     4828 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/testwidget.py
--rw-rw-r--   0 one       (1000) one       (1000)     2199 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/testwidgetsizes.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.261006 pyTermTk-0.9.0a56/tmp/TermTk/TTkTypes/
--rw-rw-r--   0 one       (1000) one       (1000)       23 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTypes/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)        0 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkTypes/viewitem.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.265006 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.265006 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/
--rw-rw-r--   0 one       (1000) one       (1000)      186 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     2581 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/table.py
--rw-rw-r--   0 one       (1000) one       (1000)    15087 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/tableview.py
--rw-rw-r--   0 one       (1000) one       (1000)     2732 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/tree.py
--rw-rw-r--   0 one       (1000) one       (1000)     1777 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/treeview.py
--rw-rw-r--   0 one       (1000) one       (1000)     6778 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/treewidget.py
--rw-rw-r--   0 one       (1000) one       (1000)     2476 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/treewidgetitem.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.269006 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/
--rw-rw-r--   0 one       (1000) one       (1000)      291 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     2770 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/filetree.py
--rw-rw-r--   0 one       (1000) one       (1000)     7793 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/filetreewidget.py
--rw-rw-r--   0 one       (1000) one       (1000)     2715 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/filetreewidgetitem.py
--rw-rw-r--   0 one       (1000) one       (1000)     3133 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/tree.py
--rw-rw-r--   0 one       (1000) one       (1000)    11843 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/treewidget.py
--rw-rw-r--   0 one       (1000) one       (1000)     6374 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/treewidgetitem.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.269006 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/
--rw-rw-r--   0 one       (1000) one       (1000)       52 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)    21093 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/colorpicker.py
--rw-rw-r--   0 one       (1000) one       (1000)     1182 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/dateTimePicker.py
--rw-rw-r--   0 one       (1000) one       (1000)    10701 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/filepicker.py
--rw-rw-r--   0 one       (1000) one       (1000)      820 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)    10075 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     7238 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/button.py
--rw-rw-r--   0 one       (1000) one       (1000)     5179 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/checkbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     8119 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/combobox.py
--rw-rw-r--   0 one       (1000) one       (1000)     4736 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/frame.py
--rw-rw-r--   0 one       (1000) one       (1000)     3481 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/graph.py
--rw-rw-r--   0 one       (1000) one       (1000)     5999 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/image.py
--rw-rw-r--   0 one       (1000) one       (1000)     2376 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/label.py
--rw-rw-r--   0 one       (1000) one       (1000)     9223 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/lineedit.py
--rw-rw-r--   0 one       (1000) one       (1000)     3123 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/list_.py
--rw-rw-r--   0 one       (1000) one       (1000)    10404 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/listwidget.py
--rw-rw-r--   0 one       (1000) one       (1000)     8438 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/menubar.py
--rw-rw-r--   0 one       (1000) one       (1000)     4912 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/radiobutton.py
--rw-rw-r--   0 one       (1000) one       (1000)     3493 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/resizableframe.py
--rw-rw-r--   0 one       (1000) one       (1000)     2521 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/scrollarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     9296 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/scrollbar.py
--rw-rw-r--   0 one       (1000) one       (1000)     1462 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/spacer.py
--rw-rw-r--   0 one       (1000) one       (1000)     4224 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/spinbox.py
--rw-rw-r--   0 one       (1000) one       (1000)    12649 2022-04-10 12:37:02.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/splitter.py
--rw-rw-r--   0 one       (1000) one       (1000)    24792 2022-04-18 16:30:48.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/tabwidget.py
--rw-rw-r--   0 one       (1000) one       (1000)    20581 2022-04-11 20:15:58.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/texedit.py
--rw-rw-r--   0 one       (1000) one       (1000)    24102 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/widget.py
--rw-rw-r--   0 one       (1000) one       (1000)     3476 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/window.py
--rw-rw-r--   0 one       (1000) one       (1000)      177 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a56/tmp/TermTk/__init__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-05-18 09:20:34.269006 pyTermTk-0.9.0a56/tmp/pyTermTk.egg-info/
--rw-rw-r--   0 one       (1000) one       (1000)     6382 2022-05-18 09:20:33.000000 pyTermTk-0.9.0a56/tmp/pyTermTk.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     3493 2022-05-18 09:20:34.000000 pyTermTk-0.9.0a56/tmp/pyTermTk.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2022-05-18 09:20:33.000000 pyTermTk-0.9.0a56/tmp/pyTermTk.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)        7 2022-05-18 09:20:34.000000 pyTermTk-0.9.0a56/tmp/pyTermTk.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.846269 pyTermTk-0.9.0a62/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2022-06-09 11:08:35.000000 pyTermTk-0.9.0a62/LICENSE
+-rw-rw-r--   0 one       (1000) one       (1000)     6382 2022-06-09 11:08:40.846269 pyTermTk-0.9.0a62/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     5652 2022-06-09 11:08:35.000000 pyTermTk-0.9.0a62/README.md
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.830269 pyTermTk-0.9.0a62/TermTk/
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.834269 pyTermTk-0.9.0a62/TermTk/TTkAbstract/
+-rw-rw-r--   0 one       (1000) one       (1000)       67 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkAbstract/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1416 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkAbstract/abstractitemmodel.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5194 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkAbstract/abstractscrollarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3377 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkAbstract/abstractscrollview.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.834269 pyTermTk-0.9.0a62/TermTk/TTkCore/
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.834269 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/
+-rw-rw-r--   0 one       (1000) one       (1000)      163 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2158 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/colors.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5878 2022-05-18 10:13:06.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/input.py
+-rw-rw-r--   0 one       (1000) one       (1000)    43749 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/inputkey.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4663 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/inputmouse.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2415 2022-05-18 09:09:22.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/readinputlinux.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5906 2022-06-09 10:28:34.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/term.py
+-rw-rw-r--   0 one       (1000) one       (1000)      234 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)    26500 2022-04-19 13:53:21.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/canvas.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1453 2022-06-09 11:08:35.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10786 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/color.py
+-rw-rw-r--   0 one       (1000) one       (1000)    35175 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/constant.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1182 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/draw.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6292 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/filebuffer.py
+-rw-rw-r--   0 one       (1000) one       (1000)    15115 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/helper.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3893 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/log.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6460 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/signal.py
+-rw-rw-r--   0 one       (1000) one       (1000)    15235 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/string.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2702 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/timer.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10747 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkCore/ttk.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.834269 pyTermTk-0.9.0a62/TermTk/TTkGui/
+-rw-rw-r--   0 one       (1000) one       (1000)       20 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkGui/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3561 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkGui/drag.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.838269 pyTermTk-0.9.0a62/TermTk/TTkLayouts/
+-rw-rw-r--   0 one       (1000) one       (1000)      140 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkLayouts/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3074 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkLayouts/boxlayout.py
+-rw-rw-r--   0 one       (1000) one       (1000)    14538 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkLayouts/gridlayout.py
+-rw-rw-r--   0 one       (1000) one       (1000)    13904 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkLayouts/layout.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.838269 pyTermTk-0.9.0a62/TermTk/TTkTemplates/
+-rw-rw-r--   0 one       (1000) one       (1000)        0 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTemplates/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1675 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTemplates/color.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1551 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTemplates/data.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2924 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkTemplates/dragevents.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2552 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTemplates/keyevents.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5313 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTemplates/mouseevents.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1551 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTemplates/text.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.838269 pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/
+-rw-rw-r--   0 one       (1000) one       (1000)       83 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4329 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/logviewer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4828 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/testwidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2199 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/testwidgetsizes.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.838269 pyTermTk-0.9.0a62/TermTk/TTkTheme/
+-rw-rw-r--   0 one       (1000) one       (1000)       20 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkTheme/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4088 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkTheme/draw_ascii.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10632 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkTheme/draw_utf8.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1339 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkTheme/fileicon_ascii.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9267 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkTheme/fileicon_nerd.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1345 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkTheme/fileicon_utf8.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10591 2022-06-09 10:47:16.000000 pyTermTk-0.9.0a62/TermTk/TTkTheme/theme.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.838269 pyTermTk-0.9.0a62/TermTk/TTkTypes/
+-rw-rw-r--   0 one       (1000) one       (1000)       23 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTypes/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)        0 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkTypes/viewitem.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.842269 pyTermTk-0.9.0a62/TermTk/TTkWidgets/
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.842269 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/
+-rw-rw-r--   0 one       (1000) one       (1000)      186 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2581 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/table.py
+-rw-rw-r--   0 one       (1000) one       (1000)    15087 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/tableview.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2732 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/tree.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1777 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/treeview.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6778 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/treewidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2476 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/treewidgetitem.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.846269 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/
+-rw-rw-r--   0 one       (1000) one       (1000)      291 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2770 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/filetree.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7793 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/filetreewidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2715 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/filetreewidgetitem.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3133 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/tree.py
+-rw-rw-r--   0 one       (1000) one       (1000)    11843 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/treewidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6374 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/treewidgetitem.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.846269 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/
+-rw-rw-r--   0 one       (1000) one       (1000)       52 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)    21093 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/colorpicker.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1182 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/dateTimePicker.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10701 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/filepicker.py
+-rw-rw-r--   0 one       (1000) one       (1000)      820 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10075 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7242 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/button.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5179 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/checkbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8119 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/combobox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4736 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/frame.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3481 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/graph.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5999 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/image.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2376 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/label.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9223 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/lineedit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3123 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/list_.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10404 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/listwidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8438 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/menubar.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4912 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/radiobutton.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3493 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/resizableframe.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2521 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/scrollarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9296 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/scrollbar.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1462 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/spacer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4224 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/spinbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12649 2022-04-10 12:37:02.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/splitter.py
+-rw-rw-r--   0 one       (1000) one       (1000)    24838 2022-06-09 10:09:26.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/tabwidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)    20581 2022-04-11 20:15:58.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/texedit.py
+-rw-rw-r--   0 one       (1000) one       (1000)    24102 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/widget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3476 2022-04-06 21:47:33.000000 pyTermTk-0.9.0a62/TermTk/TTkWidgets/window.py
+-rw-rw-r--   0 one       (1000) one       (1000)      218 2022-05-24 08:05:25.000000 pyTermTk-0.9.0a62/TermTk/__init__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2022-06-09 11:08:40.846269 pyTermTk-0.9.0a62/pyTermTk.egg-info/
+-rw-rw-r--   0 one       (1000) one       (1000)     6382 2022-06-09 11:08:40.000000 pyTermTk-0.9.0a62/pyTermTk.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     3334 2022-06-09 11:08:40.000000 pyTermTk-0.9.0a62/pyTermTk.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2022-06-09 11:08:40.000000 pyTermTk-0.9.0a62/pyTermTk.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        7 2022-06-09 11:08:40.000000 pyTermTk-0.9.0a62/pyTermTk.egg-info/top_level.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2022-06-09 11:08:40.846269 pyTermTk-0.9.0a62/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     1269 2022-06-09 11:08:35.000000 pyTermTk-0.9.0a62/setup.py
```

### Comparing `pyTermTk-0.9.0a56/LICENSE` & `pyTermTk-0.9.0a62/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/PKG-INFO` & `pyTermTk-0.9.0a62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTermTk
-Version: 0.9.0a56
+Version: 0.9.0a62
 Summary: Python Terminal Toolkit
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyTermTk-0.9.0a56/README.md` & `pyTermTk-0.9.0a62/README.md`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/setup.py` & `pyTermTk-0.9.0a62/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools, os
-from tmp.TermTk.TTkCore.cfg import TTkCfg
+from TermTk.TTkCore.cfg import TTkCfg
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 print(f"Version: {TTkCfg.version}")
 print(f"Name: {TTkCfg.name}")
 
@@ -27,11 +27,11 @@
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Topic :: Terminals",
         "Topic :: Software Development :: User Interfaces"],
     # packages=setuptools.find_packages(),
-    packages = setuptools.find_packages(where="tmp"),
-    package_dir = {"":"tmp"},
+    packages = setuptools.find_packages(where="."),
+    package_dir = {"":"."},
     python_requires=">=3.8",
-)
+)
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/abstractitemmodel.py` & `pyTermTk-0.9.0a62/TermTk/TTkAbstract/abstractitemmodel.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/abstractscrollarea.py` & `pyTermTk-0.9.0a62/TermTk/TTkAbstract/abstractscrollarea.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkAbstract/abstractscrollview.py` & `pyTermTk-0.9.0a62/TermTk/TTkAbstract/abstractscrollview.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/colors.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/colors.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/input.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,15 @@
         self._rightTap = 0
 
     def close(self):
         self._readInput.close()
 
     def get_key(self, callback=None):
         mouse_re = re.compile(r"\033\[<(\d+);(\d+);(\d+)([mM])")
-        while True:
-            if not (stdinRead := self._readInput.read()):
-                TTkLog.debug("Close TTkInput")
-                break
-
+        while stdinRead := self._readInput.read():
             mevt = None
             kevt = TTkKeyEvent.parse(stdinRead)
             if kevt is None and \
                stdinRead.startswith("\033[<"):
                 # Mouse Event
                 m = mouse_re.match(stdinRead)
                 if not m:
@@ -123,14 +119,15 @@
 
             if kevt is None and mevt is None:
                 TTkLog.error("UNHANDLED: "+stdinRead.replace("\033","<ESC>"))
 
             if callback is not None:
                 if not callback(kevt, mevt):
                     break
+        TTkLog.debug("Close TTkInput")
 
 def main():
     print("Retrieve Keyboard, Mouse press/drag/wheel Events")
     print("Press q or <ESC> to exit")
     from term import TTkTerm
 
     TTkTerm.push(TTkTerm.Mouse.ON)
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/inputkey.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/inputkey.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/inputmouse.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/inputmouse.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/readinputlinux.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/readinputlinux.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/TTkTerm/term.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/TTkTerm/term.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/canvas.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/canvas.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/cfg.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/cfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from TermTk.TTkCore.constant import TTkK
 class TTkCfg:
-    version="0.9.0a56"
+    version="0.9.0a62"
     name="pyTermTk"
 
     color_depth: int = TTkK.DEP_24
 
     maxFps = 35
     doubleBuffer = True
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/color.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/color.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/constant.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/constant.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/drag.py` & `pyTermTk-0.9.0a62/TermTk/TTkGui/drag.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from TermTk.TTkCore.string    import TTkString
 from TermTk.TTkCore.helper    import TTkHelper
 from TermTk.TTkCore.canvas    import TTkCanvas
 from TermTk.TTkWidgets.widget import TTkWidget
 
 class _TTkDragDisplayWidget(TTkWidget):
     __slots__ = ('_pixmap')
     def __init__(self, *args, **kwargs):
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/draw.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/draw.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/filebuffer.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/filebuffer.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/helper.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/helper.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/log.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/log.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/signal.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/signal.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/string.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/string.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/timer.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/timer.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkCore/ttk.py` & `pyTermTk-0.9.0a62/TermTk/TTkCore/ttk.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from TermTk.TTkCore.TTkTerm.input import TTkInput
 from TermTk.TTkCore.TTkTerm.term import TTkTerm
 from TermTk.TTkCore.constant import TTkK
 from TermTk.TTkCore.log import TTkLog
 from TermTk.TTkCore.signal import pyTTkSlot, pyTTkSignal
 from TermTk.TTkCore.cfg import *
 from TermTk.TTkCore.timer import *
-from TermTk.TTkGui.theme import TTkTheme
+from TermTk.TTkTheme.theme import TTkTheme
 from TermTk.TTkLayouts.layout import TTkLayout
 from TermTk.TTkWidgets.widget import *
 
 class TTk(TTkWidget):
     __slots__ = ('_name', '_running', '_input', '_events', '_key_events', '_mouse_events', '_screen_events', '_title' )
 
     def __init__(self, *args, **kwargs):
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/draw_ascii.py` & `pyTermTk-0.9.0a62/TermTk/TTkTheme/draw_ascii.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/draw_utf8.py` & `pyTermTk-0.9.0a62/TermTk/TTkTheme/draw_utf8.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/fileicon_ascii.py` & `pyTermTk-0.9.0a62/TermTk/TTkTheme/fileicon_ascii.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/fileicon_nerd.py` & `pyTermTk-0.9.0a62/TermTk/TTkTheme/fileicon_nerd.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/fileicon_utf8.py` & `pyTermTk-0.9.0a62/TermTk/TTkTheme/fileicon_utf8.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkGui/theme.py` & `pyTermTk-0.9.0a62/TermTk/TTkTheme/theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from TermTk.TTkCore.color import TTkColor
 from TermTk.TTkCore.helper import TTkHelper
-from TermTk.TTkCore.string import TTkString
-import TermTk.TTkGui.fileicon_nerd  as fi_nerd
-import TermTk.TTkGui.fileicon_utf8  as fi_utf8
-import TermTk.TTkGui.fileicon_ascii as fi_ascii
-import TermTk.TTkGui.draw_utf8      as draw_utf8
-import TermTk.TTkGui.draw_ascii     as draw_ascii
+# from TermTk.TTkCore.string import TTkString
+import TermTk.TTkTheme.fileicon_nerd  as fi_nerd
+import TermTk.TTkTheme.fileicon_utf8  as fi_utf8
+import TermTk.TTkTheme.fileicon_ascii as fi_ascii
+import TermTk.TTkTheme.draw_utf8      as draw_utf8
+import TermTk.TTkTheme.draw_ascii     as draw_ascii
 
 
 class TTkTheme():
     '''Default Theme Class
     This class can be reimplemented/extended to include new themes and default colors
     '''
     NERD  = {'file':fi_nerd,  'draw':draw_utf8}
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/boxlayout.py` & `pyTermTk-0.9.0a62/TermTk/TTkLayouts/boxlayout.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/gridlayout.py` & `pyTermTk-0.9.0a62/TermTk/TTkLayouts/gridlayout.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkLayouts/layout.py` & `pyTermTk-0.9.0a62/TermTk/TTkLayouts/layout.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/color.py` & `pyTermTk-0.9.0a62/TermTk/TTkTemplates/color.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/data.py` & `pyTermTk-0.9.0a62/TermTk/TTkTemplates/data.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/dragevents.py` & `pyTermTk-0.9.0a62/TermTk/TTkTemplates/dragevents.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,55 +26,55 @@
     def dragEnterEvent(self, evt)  -> bool:
         '''
         This event handler, can be reimplemented in a subclass to receive drag events for the widget.
 
         .. note:: Reimplement this function to handle this event
 
         :param evt: The drop event
-        :type evt: :class:`~TermTk.TTkCore.drag.TTkDropEvent`
+        :type evt: :class:`~TermTk.TTkGui.drag.TTkDropEvent`
 
         :return: **True** if the event has been handled
         :rtype: bool
         '''
         return False
 
     def dragLeaveEvent(self, evt) -> bool:
         '''
         This event handler, can be reimplemented in a subclass to receive drag events for the widget.
 
         .. note:: Reimplement this function to handle this event
 
         :param evt: The drop event
-        :type evt: :class:`~TermTk.TTkCore.drag.TTkDropEvent`
+        :type evt: :class:`~TermTk.TTkGui.drag.TTkDropEvent`
 
         :return: **True** if the event has been handled
         :rtype: bool
         '''
         return False
 
     def dragMoveEvent(self, evt) -> bool:
         '''
         This event handler, can be reimplemented in a subclass to receive drag events for the widget.
 
         .. note:: Reimplement this function to handle this event
 
         :param evt: The drop event
-        :type evt: :class:`~TermTk.TTkCore.drag.TTkDropEvent`
+        :type evt: :class:`~TermTk.TTkGui.drag.TTkDropEvent`
 
         :return: **True** if the event has been handled
         :rtype: bool
         '''
         return False
 
     def dropEvent(self, evt) -> bool:
         '''
         This event handler, can be reimplemented in a subclass to receive drag events for the widget.
 
         .. note:: Reimplement this function to handle this event
 
         :param evt: The drop event
-        :type evt: :class:`~TermTk.TTkCore.drag.TTkDropEvent`
+        :type evt: :class:`~TermTk.TTkGui.drag.TTkDropEvent`
 
         :return: **True** if the event has been handled
         :rtype: bool
         '''
         return False
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/keyevents.py` & `pyTermTk-0.9.0a62/TermTk/TTkTemplates/keyevents.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/mouseevents.py` & `pyTermTk-0.9.0a62/TermTk/TTkTemplates/mouseevents.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTemplates/text.py` & `pyTermTk-0.9.0a62/TermTk/TTkTemplates/text.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/logviewer.py` & `pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/logviewer.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/testwidget.py` & `pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/testwidget.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkTestWidgets/testwidgetsizes.py` & `pyTermTk-0.9.0a62/TermTk/TTkTestWidgets/testwidgetsizes.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/table.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/table.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/tableview.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/tableview.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/tree.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/tree.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/treeview.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/treeview.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/treewidget.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/treewidget.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/Fancy/treewidgetitem.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/Fancy/treewidgetitem.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/filetree.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/filetree.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/filetreewidget.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/filetreewidget.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/filetreewidgetitem.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/filetreewidgetitem.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/tree.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/tree.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/treewidget.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/treewidget.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkModelView/treewidgetitem.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkModelView/treewidgetitem.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/colorpicker.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/colorpicker.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/dateTimePicker.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/dateTimePicker.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/TTkPickers/filepicker.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/TTkPickers/filepicker.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/__init__.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/about.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/about.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/button.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
     Demo: `formwidgets.py <https://github.com/ceccopierangiolieugenio/pyTermTk/blob/main/demo/showcase/formwidgets.py>`_
 
     :param str text: the text shown on the button, defaults to ""
     :type text: str, optional
     :param bool border: the border of the button, defaults to "False"
     :type border: bool, optional
-    :param TTkColor color: the color of the border of the button, defaults to :class:`~TermTk.TTkGui.theme.TTkTheme.buttonTextColor`
+    :param TTkColor color: the color of the border of the button, defaults to :class:`~TermTk.TTkTheme.theme.TTkTheme.buttonTextColor`
     :type color: :class:`~TermTk.TTkCore.color.TTkColor`, optional
-    :param TTkColor borderColor: the color of the border of the button, defaults to :class:`~TermTk.TTkGui.theme.TTkTheme.buttonBorderColor`
+    :param TTkColor borderColor: the color of the border of the button, defaults to :class:`~TermTk.TTkTheme.theme.TTkTheme.buttonBorderColor`
     :type borderColor: :class:`~TermTk.TTkCore.color.TTkColor`, optional
 
     +-----------------------------------------------------------------------------------------------+
     | `Signals <https://ceccopierangiolieugenio.github.io/pyTermTk/tutorial/003-signalslots.html>`_ |
     +-----------------------------------------------------------------------------------------------+
 
         .. py:method:: clicked()
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/checkbox.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/combobox.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/combobox.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/frame.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/frame.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/graph.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/graph.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/image.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/image.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/label.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/label.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/lineedit.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/lineedit.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/list_.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/list_.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/listwidget.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/listwidget.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/menubar.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/menubar.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/radiobutton.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/radiobutton.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/resizableframe.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/resizableframe.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/scrollarea.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/scrollarea.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/scrollbar.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/scrollbar.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/spacer.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/spacer.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/spinbox.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/splitter.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/splitter.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/tabwidget.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/tabwidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from turtle import isvisible
 from TermTk.TTkCore.constant import TTkConstant, TTkK
 from TermTk.TTkCore.helper import TTkHelper
 from TermTk.TTkCore.log import TTkLog
 from TermTk.TTkCore.cfg import *
 from TermTk.TTkCore.string import TTkString
-from TermTk.TTkCore.drag import TTkDrag
+from TermTk.TTkGui.drag import TTkDrag
 from TermTk.TTkCore.signal import pyTTkSlot, pyTTkSignal
 from TermTk.TTkWidgets.widget import TTkWidget
 from TermTk.TTkWidgets.spacer import TTkSpacer
 from TermTk.TTkWidgets.frame import TTkFrame
 from TermTk.TTkWidgets.button import TTkButton
 from TermTk.TTkWidgets.menubar import TTkMenuButton
 from TermTk.TTkLayouts.boxlayout import TTkHBoxLayout
@@ -269,14 +268,16 @@
         self._leftScroller.setSideEnd(sideEnd&TTkK.LEFT)
         self._updateTabs()
 
     def addTab(self, label, data=None):
         self.insertTab(len(self._tabButtons), label, data)
 
     def insertTab(self, index, label, data=None):
+        if index <= self._currentIndex:
+            self._currentIndex += 1
         button = TTkTabButton(parent=self, text=label, border=not self._small, closable=self._tabClosable)
         button._borderColor = self._borderColor
         self._tabButtons.insert(index,button)
         self._tabData.insert(index,data)
         button.clicked.connect(lambda :self.setCurrentIndex(self._tabButtons.index(button)))
         button.closeClicked.connect(lambda :self.tabCloseRequested.emit(self._tabButtons.index(button)))
         self._updateTabs()
```

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/texedit.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/texedit.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/widget.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/widget.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/TermTk/TTkWidgets/window.py` & `pyTermTk-0.9.0a62/TermTk/TTkWidgets/window.py`

 * *Files identical despite different names*

### Comparing `pyTermTk-0.9.0a56/tmp/pyTermTk.egg-info/PKG-INFO` & `pyTermTk-0.9.0a62/pyTermTk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTermTk
-Version: 0.9.0a56
+Version: 0.9.0a62
 Summary: Python Terminal Toolkit
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyTermTk-0.9.0a56/tmp/pyTermTk.egg-info/SOURCES.txt` & `pyTermTk-0.9.0a62/pyTermTk.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,100 @@
 LICENSE
 README.md
 setup.py
-tmp/TermTk/__init__.py
-tmp/TermTk/TTkAbstract/__init__.py
-tmp/TermTk/TTkAbstract/abstractitemmodel.py
-tmp/TermTk/TTkAbstract/abstractscrollarea.py
-tmp/TermTk/TTkAbstract/abstractscrollview.py
-tmp/TermTk/TTkCore/__init__.py
-tmp/TermTk/TTkCore/canvas.py
-tmp/TermTk/TTkCore/cfg.py
-tmp/TermTk/TTkCore/color.py
-tmp/TermTk/TTkCore/constant.py
-tmp/TermTk/TTkCore/drag.py
-tmp/TermTk/TTkCore/draw.py
-tmp/TermTk/TTkCore/filebuffer.py
-tmp/TermTk/TTkCore/helper.py
-tmp/TermTk/TTkCore/log.py
-tmp/TermTk/TTkCore/signal.py
-tmp/TermTk/TTkCore/string.py
-tmp/TermTk/TTkCore/timer.py
-tmp/TermTk/TTkCore/ttk.py
-tmp/TermTk/TTkCore/TTkTerm/__init__.py
-tmp/TermTk/TTkCore/TTkTerm/colors.py
-tmp/TermTk/TTkCore/TTkTerm/input.py
-tmp/TermTk/TTkCore/TTkTerm/inputkey.py
-tmp/TermTk/TTkCore/TTkTerm/inputmouse.py
-tmp/TermTk/TTkCore/TTkTerm/readinputlinux.py
-tmp/TermTk/TTkCore/TTkTerm/term.py
-tmp/TermTk/TTkGui/__init__.py
-tmp/TermTk/TTkGui/draw_ascii.py
-tmp/TermTk/TTkGui/draw_utf8.py
-tmp/TermTk/TTkGui/fileicon_ascii.py
-tmp/TermTk/TTkGui/fileicon_nerd.py
-tmp/TermTk/TTkGui/fileicon_utf8.py
-tmp/TermTk/TTkGui/theme.py
-tmp/TermTk/TTkLayouts/__init__.py
-tmp/TermTk/TTkLayouts/boxlayout.py
-tmp/TermTk/TTkLayouts/gridlayout.py
-tmp/TermTk/TTkLayouts/layout.py
-tmp/TermTk/TTkTemplates/__init__.py
-tmp/TermTk/TTkTemplates/color.py
-tmp/TermTk/TTkTemplates/data.py
-tmp/TermTk/TTkTemplates/dragevents.py
-tmp/TermTk/TTkTemplates/keyevents.py
-tmp/TermTk/TTkTemplates/mouseevents.py
-tmp/TermTk/TTkTemplates/text.py
-tmp/TermTk/TTkTestWidgets/__init__.py
-tmp/TermTk/TTkTestWidgets/logviewer.py
-tmp/TermTk/TTkTestWidgets/testwidget.py
-tmp/TermTk/TTkTestWidgets/testwidgetsizes.py
-tmp/TermTk/TTkTypes/__init__.py
-tmp/TermTk/TTkTypes/viewitem.py
-tmp/TermTk/TTkWidgets/__init__.py
-tmp/TermTk/TTkWidgets/about.py
-tmp/TermTk/TTkWidgets/button.py
-tmp/TermTk/TTkWidgets/checkbox.py
-tmp/TermTk/TTkWidgets/combobox.py
-tmp/TermTk/TTkWidgets/frame.py
-tmp/TermTk/TTkWidgets/graph.py
-tmp/TermTk/TTkWidgets/image.py
-tmp/TermTk/TTkWidgets/label.py
-tmp/TermTk/TTkWidgets/lineedit.py
-tmp/TermTk/TTkWidgets/list_.py
-tmp/TermTk/TTkWidgets/listwidget.py
-tmp/TermTk/TTkWidgets/menubar.py
-tmp/TermTk/TTkWidgets/radiobutton.py
-tmp/TermTk/TTkWidgets/resizableframe.py
-tmp/TermTk/TTkWidgets/scrollarea.py
-tmp/TermTk/TTkWidgets/scrollbar.py
-tmp/TermTk/TTkWidgets/spacer.py
-tmp/TermTk/TTkWidgets/spinbox.py
-tmp/TermTk/TTkWidgets/splitter.py
-tmp/TermTk/TTkWidgets/tabwidget.py
-tmp/TermTk/TTkWidgets/texedit.py
-tmp/TermTk/TTkWidgets/widget.py
-tmp/TermTk/TTkWidgets/window.py
-tmp/TermTk/TTkWidgets/Fancy/__init__.py
-tmp/TermTk/TTkWidgets/Fancy/table.py
-tmp/TermTk/TTkWidgets/Fancy/tableview.py
-tmp/TermTk/TTkWidgets/Fancy/tree.py
-tmp/TermTk/TTkWidgets/Fancy/treeview.py
-tmp/TermTk/TTkWidgets/Fancy/treewidget.py
-tmp/TermTk/TTkWidgets/Fancy/treewidgetitem.py
-tmp/TermTk/TTkWidgets/TTkModelView/__init__.py
-tmp/TermTk/TTkWidgets/TTkModelView/filetree.py
-tmp/TermTk/TTkWidgets/TTkModelView/filetreewidget.py
-tmp/TermTk/TTkWidgets/TTkModelView/filetreewidgetitem.py
-tmp/TermTk/TTkWidgets/TTkModelView/tree.py
-tmp/TermTk/TTkWidgets/TTkModelView/treewidget.py
-tmp/TermTk/TTkWidgets/TTkModelView/treewidgetitem.py
-tmp/TermTk/TTkWidgets/TTkPickers/__init__.py
-tmp/TermTk/TTkWidgets/TTkPickers/colorpicker.py
-tmp/TermTk/TTkWidgets/TTkPickers/dateTimePicker.py
-tmp/TermTk/TTkWidgets/TTkPickers/filepicker.py
-tmp/pyTermTk.egg-info/PKG-INFO
-tmp/pyTermTk.egg-info/SOURCES.txt
-tmp/pyTermTk.egg-info/dependency_links.txt
-tmp/pyTermTk.egg-info/top_level.txt
+./TermTk/__init__.py
+./TermTk/TTkAbstract/__init__.py
+./TermTk/TTkAbstract/abstractitemmodel.py
+./TermTk/TTkAbstract/abstractscrollarea.py
+./TermTk/TTkAbstract/abstractscrollview.py
+./TermTk/TTkCore/__init__.py
+./TermTk/TTkCore/canvas.py
+./TermTk/TTkCore/cfg.py
+./TermTk/TTkCore/color.py
+./TermTk/TTkCore/constant.py
+./TermTk/TTkCore/draw.py
+./TermTk/TTkCore/filebuffer.py
+./TermTk/TTkCore/helper.py
+./TermTk/TTkCore/log.py
+./TermTk/TTkCore/signal.py
+./TermTk/TTkCore/string.py
+./TermTk/TTkCore/timer.py
+./TermTk/TTkCore/ttk.py
+./TermTk/TTkCore/TTkTerm/__init__.py
+./TermTk/TTkCore/TTkTerm/colors.py
+./TermTk/TTkCore/TTkTerm/input.py
+./TermTk/TTkCore/TTkTerm/inputkey.py
+./TermTk/TTkCore/TTkTerm/inputmouse.py
+./TermTk/TTkCore/TTkTerm/readinputlinux.py
+./TermTk/TTkCore/TTkTerm/term.py
+./TermTk/TTkGui/__init__.py
+./TermTk/TTkGui/drag.py
+./TermTk/TTkLayouts/__init__.py
+./TermTk/TTkLayouts/boxlayout.py
+./TermTk/TTkLayouts/gridlayout.py
+./TermTk/TTkLayouts/layout.py
+./TermTk/TTkTemplates/__init__.py
+./TermTk/TTkTemplates/color.py
+./TermTk/TTkTemplates/data.py
+./TermTk/TTkTemplates/dragevents.py
+./TermTk/TTkTemplates/keyevents.py
+./TermTk/TTkTemplates/mouseevents.py
+./TermTk/TTkTemplates/text.py
+./TermTk/TTkTestWidgets/__init__.py
+./TermTk/TTkTestWidgets/logviewer.py
+./TermTk/TTkTestWidgets/testwidget.py
+./TermTk/TTkTestWidgets/testwidgetsizes.py
+./TermTk/TTkTheme/__init__.py
+./TermTk/TTkTheme/draw_ascii.py
+./TermTk/TTkTheme/draw_utf8.py
+./TermTk/TTkTheme/fileicon_ascii.py
+./TermTk/TTkTheme/fileicon_nerd.py
+./TermTk/TTkTheme/fileicon_utf8.py
+./TermTk/TTkTheme/theme.py
+./TermTk/TTkTypes/__init__.py
+./TermTk/TTkTypes/viewitem.py
+./TermTk/TTkWidgets/__init__.py
+./TermTk/TTkWidgets/about.py
+./TermTk/TTkWidgets/button.py
+./TermTk/TTkWidgets/checkbox.py
+./TermTk/TTkWidgets/combobox.py
+./TermTk/TTkWidgets/frame.py
+./TermTk/TTkWidgets/graph.py
+./TermTk/TTkWidgets/image.py
+./TermTk/TTkWidgets/label.py
+./TermTk/TTkWidgets/lineedit.py
+./TermTk/TTkWidgets/list_.py
+./TermTk/TTkWidgets/listwidget.py
+./TermTk/TTkWidgets/menubar.py
+./TermTk/TTkWidgets/radiobutton.py
+./TermTk/TTkWidgets/resizableframe.py
+./TermTk/TTkWidgets/scrollarea.py
+./TermTk/TTkWidgets/scrollbar.py
+./TermTk/TTkWidgets/spacer.py
+./TermTk/TTkWidgets/spinbox.py
+./TermTk/TTkWidgets/splitter.py
+./TermTk/TTkWidgets/tabwidget.py
+./TermTk/TTkWidgets/texedit.py
+./TermTk/TTkWidgets/widget.py
+./TermTk/TTkWidgets/window.py
+./TermTk/TTkWidgets/Fancy/__init__.py
+./TermTk/TTkWidgets/Fancy/table.py
+./TermTk/TTkWidgets/Fancy/tableview.py
+./TermTk/TTkWidgets/Fancy/tree.py
+./TermTk/TTkWidgets/Fancy/treeview.py
+./TermTk/TTkWidgets/Fancy/treewidget.py
+./TermTk/TTkWidgets/Fancy/treewidgetitem.py
+./TermTk/TTkWidgets/TTkModelView/__init__.py
+./TermTk/TTkWidgets/TTkModelView/filetree.py
+./TermTk/TTkWidgets/TTkModelView/filetreewidget.py
+./TermTk/TTkWidgets/TTkModelView/filetreewidgetitem.py
+./TermTk/TTkWidgets/TTkModelView/tree.py
+./TermTk/TTkWidgets/TTkModelView/treewidget.py
+./TermTk/TTkWidgets/TTkModelView/treewidgetitem.py
+./TermTk/TTkWidgets/TTkPickers/__init__.py
+./TermTk/TTkWidgets/TTkPickers/colorpicker.py
+./TermTk/TTkWidgets/TTkPickers/dateTimePicker.py
+./TermTk/TTkWidgets/TTkPickers/filepicker.py
+pyTermTk.egg-info/PKG-INFO
+pyTermTk.egg-info/SOURCES.txt
+pyTermTk.egg-info/dependency_links.txt
+pyTermTk.egg-info/top_level.txt
```

