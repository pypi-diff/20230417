# Comparing `tmp/maptasker-1.3.2.tar.gz` & `tmp/maptasker-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maptasker-1.3.2.tar", max compression
+gzip compressed data, was "maptasker-1.3.3.tar", max compression
```

## Comparing `maptasker-1.3.2.tar` & `maptasker-1.3.3.tar`

### file list

```diff
@@ -1,94 +1,98 @@
--rw-r--r--   0        0        0    35149 2023-02-10 17:49:08.224000 maptasker-1.3.2/LICENSE.txt
--rw-r--r--   0        0        0      296 2023-03-16 14:54:53.454155 maptasker-1.3.2/README_PyPl.md
--rw-r--r--   0        0        0     8196 2023-02-27 17:44:14.167143 maptasker-1.3.2/maptasker/.DS_Store
--rw-r--r--   0        0        0        0 2023-02-15 21:09:13.241439 maptasker-1.3.2/maptasker/__init__.py
--rw-r--r--   0        0        0      169 2023-03-11 17:11:25.837533 maptasker-1.3.2/maptasker/main.py
--rw-r--r--   0        0        0     6148 2023-02-27 16:37:40.000000 maptasker-1.3.2/maptasker/src/.DS_Store
--rw-r--r--   0        0        0     1159 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/MainItem.py
--rw-r--r--   0        0        0        0 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/__init__.py
--rw-r--r--   0        0        0      212 2023-03-23 17:49:08.090530 maptasker-1.3.2/maptasker/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3112 2023-03-23 17:49:08.129098 maptasker-1.3.2/maptasker/src/__pycache__/actargs.cpython-310.pyc
--rw-r--r--   0        0        0     5777 2023-04-04 15:04:43.335513 maptasker-1.3.2/maptasker/src/__pycache__/action.cpython-310.pyc
--rw-r--r--   0        0        0   107715 2023-03-23 17:49:08.156251 maptasker-1.3.2/maptasker/src/__pycache__/actionc.cpython-310.pyc
--rw-r--r--   0        0        0     2586 2023-03-23 17:49:08.130230 maptasker-1.3.2/maptasker/src/__pycache__/actiond.cpython-310.pyc
--rw-r--r--   0        0        0     4092 2023-04-04 17:31:32.000823 maptasker-1.3.2/maptasker/src/__pycache__/actione.cpython-310.pyc
--rw-r--r--   0        0        0     3113 2023-03-31 16:38:58.765668 maptasker-1.3.2/maptasker/src/__pycache__/actionr.cpython-310.pyc
--rw-r--r--   0        0        0    14483 2023-03-23 17:49:08.400678 maptasker-1.3.2/maptasker/src/__pycache__/actiont.cpython-310.pyc
--rw-r--r--   0        0        0     1005 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/__pycache__/argsdict.cpython-310.pyc
--rw-r--r--   0        0        0     1847 2023-04-04 15:34:28.525854 maptasker-1.3.2/maptasker/src/__pycache__/caveats.cpython-310.pyc
--rw-r--r--   0        0        0     4400 2023-03-23 17:49:08.182225 maptasker-1.3.2/maptasker/src/__pycache__/colors.cpython-310.pyc
--rw-r--r--   0        0        0     1726 2023-03-31 16:03:07.520328 maptasker-1.3.2/maptasker/src/__pycache__/colrmode.cpython-310.pyc
--rw-r--r--   0        0        0     3848 2023-03-23 17:49:08.203819 maptasker-1.3.2/maptasker/src/__pycache__/condition.cpython-310.pyc
--rw-r--r--   0        0        0      314 2023-03-23 17:49:08.122336 maptasker-1.3.2/maptasker/src/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-03-27 15:29:00.454256 maptasker-1.3.2/maptasker/src/__pycache__/debug.cpython-310.pyc
--rw-r--r--   0        0        0      351 2023-03-23 17:49:08.397467 maptasker-1.3.2/maptasker/src/__pycache__/depricated.cpython-310.pyc
--rw-r--r--   0        0        0     1379 2023-04-04 17:24:36.764246 maptasker-1.3.2/maptasker/src/__pycache__/getids.cpython-310.pyc
--rw-r--r--   0        0        0      969 2023-03-23 17:49:08.182943 maptasker-1.3.2/maptasker/src/__pycache__/getputarg.cpython-310.pyc
--rw-r--r--   0        0        0      754 2023-03-23 17:49:08.190511 maptasker-1.3.2/maptasker/src/__pycache__/initparg.cpython-310.pyc
--rw-r--r--   0        0        0     1223 2023-03-23 17:49:08.206563 maptasker-1.3.2/maptasker/src/__pycache__/kidapp.cpython-310.pyc
--rw-r--r--   0        0        0     5188 2023-04-04 17:33:48.583248 maptasker-1.3.2/maptasker/src/__pycache__/mapit.cpython-310.pyc
--rw-r--r--   0        0        0     3748 2023-04-04 14:44:36.346643 maptasker-1.3.2/maptasker/src/__pycache__/outputl.cpython-310.pyc
--rw-r--r--   0        0        0     4396 2023-03-23 17:49:08.186264 maptasker-1.3.2/maptasker/src/__pycache__/parsearg.cpython-310.pyc
--rw-r--r--   0        0        0     3864 2023-03-30 18:39:13.650737 maptasker-1.3.2/maptasker/src/__pycache__/prefers.cpython-310.pyc
--rw-r--r--   0        0        0      773 2023-03-23 17:49:08.204379 maptasker-1.3.2/maptasker/src/__pycache__/priority.cpython-310.pyc
--rw-r--r--   0        0        0     2083 2023-04-03 19:11:00.966898 maptasker-1.3.2/maptasker/src/__pycache__/proclist.cpython-310.pyc
--rw-r--r--   0        0        0     4581 2023-04-04 17:24:36.763063 maptasker-1.3.2/maptasker/src/__pycache__/profiles.cpython-310.pyc
--rw-r--r--   0        0        0      678 2023-03-23 17:49:08.179364 maptasker-1.3.2/maptasker/src/__pycache__/progargs.cpython-310.pyc
--rw-r--r--   0        0        0     6079 2023-03-30 17:50:55.588405 maptasker-1.3.2/maptasker/src/__pycache__/proginit.cpython-310.pyc
--rw-r--r--   0        0        0     7395 2023-04-04 17:27:48.326254 maptasker-1.3.2/maptasker/src/__pycache__/projects.cpython-310.pyc
--rw-r--r--   0        0        0     4273 2023-03-23 17:49:08.181004 maptasker-1.3.2/maptasker/src/__pycache__/runcli.cpython-310.pyc
--rw-r--r--   0        0        0     1601 2023-03-23 17:49:08.189915 maptasker-1.3.2/maptasker/src/__pycache__/rungui.cpython-310.pyc
--rw-r--r--   0        0        0     4247 2023-04-04 14:48:58.901070 maptasker-1.3.2/maptasker/src/__pycache__/scenes.cpython-310.pyc
--rw-r--r--   0        0        0     8098 2023-03-23 17:49:08.215471 maptasker-1.3.2/maptasker/src/__pycache__/servicec.cpython-310.pyc
--rw-r--r--   0        0        0     2046 2023-04-04 14:24:20.204824 maptasker-1.3.2/maptasker/src/__pycache__/share.cpython-310.pyc
--rw-r--r--   0        0        0      998 2023-03-23 17:49:08.120911 maptasker-1.3.2/maptasker/src/__pycache__/shellsort.cpython-310.pyc
--rw-r--r--   0        0        0     2376 2023-04-04 17:43:19.909562 maptasker-1.3.2/maptasker/src/__pycache__/sysconst.cpython-310.pyc
--rw-r--r--   0        0        0     2374 2023-04-03 19:11:00.967760 maptasker-1.3.2/maptasker/src/__pycache__/taskactn.cpython-310.pyc
--rw-r--r--   0        0        0     1331 2023-03-23 17:49:08.199590 maptasker-1.3.2/maptasker/src/__pycache__/taskerd.cpython-310.pyc
--rw-r--r--   0        0        0     7944 2023-04-04 16:03:53.668918 maptasker-1.3.2/maptasker/src/__pycache__/tasks.cpython-310.pyc
--rw-r--r--   0        0        0     3427 2023-04-04 17:52:29.735433 maptasker-1.3.2/maptasker/src/__pycache__/taskuniq.cpython-310.pyc
--rw-r--r--   0        0        0    13296 2023-04-04 17:53:27.430394 maptasker-1.3.2/maptasker/src/__pycache__/userintr.cpython-310.pyc
--rw-r--r--   0        0        0     2504 2023-04-04 14:19:09.456115 maptasker-1.3.2/maptasker/src/__pycache__/xmldata.cpython-310.pyc
--rw-r--r--   0        0        0     6328 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/actargs.py
--rw-r--r--   0        0        0    14801 2023-04-04 15:04:43.263794 maptasker-1.3.2/maptasker/src/action.py
--rw-r--r--   0        0        0   150799 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/actionc.py
--rw-r--r--   0        0        0     6713 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/actiond.py
--rw-r--r--   0        0        0     9670 2023-04-04 17:31:26.510616 maptasker-1.3.2/maptasker/src/actione.py
--rw-r--r--   0        0        0     7541 2023-03-31 16:38:58.724693 maptasker-1.3.2/maptasker/src/actionr.py
--rw-r--r--   0        0        0    17381 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/actiont.py
--rw-r--r--   0        0        0     3401 2023-04-04 15:26:45.790042 maptasker-1.3.2/maptasker/src/caveats.py
--rw-r--r--   0        0        0     8220 2023-03-23 17:42:41.450000 maptasker-1.3.2/maptasker/src/colors.py
--rw-r--r--   0        0        0     3285 2023-03-31 16:03:07.377591 maptasker-1.3.2/maptasker/src/colrmode.py
--rw-r--r--   0        0        0     9131 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/condition.py
--rw-r--r--   0        0        0     2318 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/config.py
--rw-r--r--   0        0        0     2440 2023-03-27 15:29:00.384399 maptasker-1.3.2/maptasker/src/debug.py
--rw-r--r--   0        0        0      342 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/depricated.py
--rw-r--r--   0        0        0     2463 2023-04-04 17:24:36.654348 maptasker-1.3.2/maptasker/src/getids.py
--rw-r--r--   0        0        0     2142 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/getputarg.py
--rw-r--r--   0        0        0     2366 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/initparg.py
--rw-r--r--   0        0        0     2397 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/kidapp.py
--rw-r--r--   0        0        0    15342 2023-04-04 17:33:48.564468 maptasker-1.3.2/maptasker/src/mapit.py
--rw-r--r--   0        0        0     9854 2023-04-04 14:42:44.210128 maptasker-1.3.2/maptasker/src/outputl.py
--rw-r--r--   0        0        0     8092 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/parsearg.py
--rw-r--r--   0        0        0     7310 2023-03-30 18:39:13.574286 maptasker-1.3.2/maptasker/src/prefers.py
--rw-r--r--   0        0        0     1649 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/priority.py
--rw-r--r--   0        0        0     4688 2023-04-03 19:11:00.841847 maptasker-1.3.2/maptasker/src/proclist.py
--rw-r--r--   0        0        0    10484 2023-04-04 17:24:36.651496 maptasker-1.3.2/maptasker/src/profiles.py
--rw-r--r--   0        0        0     1947 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/progargs.py
--rw-r--r--   0        0        0    10459 2023-03-30 17:50:55.543478 maptasker-1.3.2/maptasker/src/proginit.py
--rw-r--r--   0        0        0    15015 2023-04-04 17:27:48.225904 maptasker-1.3.2/maptasker/src/projects.py
--rw-r--r--   0        0        0     8999 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/runcli.py
--rw-r--r--   0        0        0     4154 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/rungui.py
--rw-r--r--   0        0        0     7762 2023-04-04 14:44:36.436998 maptasker-1.3.2/maptasker/src/scenes.py
--rw-r--r--   0        0        0    14219 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/servicec.py
--rw-r--r--   0        0        0     4300 2023-04-04 14:24:15.779355 maptasker-1.3.2/maptasker/src/share.py
--rw-r--r--   0        0        0     3354 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/shellsort.py
--rw-r--r--   0        0        0     4082 2023-04-04 17:43:19.871730 maptasker-1.3.2/maptasker/src/sysconst.py
--rw-r--r--   0        0        0     5247 2023-04-03 19:11:00.837179 maptasker-1.3.2/maptasker/src/taskactn.py
--rw-r--r--   0        0        0     3107 2023-03-23 17:42:41.413000 maptasker-1.3.2/maptasker/src/taskerd.py
--rw-r--r--   0        0        0    15228 2023-04-04 15:44:52.485008 maptasker-1.3.2/maptasker/src/tasks.py
--rw-r--r--   0        0        0     9526 2023-04-04 17:52:29.653958 maptasker-1.3.2/maptasker/src/taskuniq.py
--rw-r--r--   0        0        0    28690 2023-03-23 17:42:41.454000 maptasker-1.3.2/maptasker/src/userintr.py
--rw-r--r--   0        0        0     6623 2023-04-04 13:54:26.475440 maptasker-1.3.2/maptasker/src/xmldata.py
--rw-r--r--   0        0        0     1157 2023-03-19 17:43:40.831675 maptasker-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 maptasker-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-10 17:49:08.224000 maptasker-1.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      296 2023-03-16 14:54:53.454155 maptasker-1.3.3/README_PyPl.md
+-rw-r--r--   0        0        0     8196 2023-02-27 17:44:14.167143 maptasker-1.3.3/maptasker/.DS_Store
+-rw-r--r--   0        0        0      220 2023-04-12 16:31:10.132958 maptasker-1.3.3/maptasker/.MapTasker_arguments.json
+-rw-r--r--   0        0        0        0 2023-02-15 21:09:13.241439 maptasker-1.3.3/maptasker/__init__.py
+-rw-r--r--   0        0        0      169 2023-03-11 17:11:25.837533 maptasker-1.3.3/maptasker/main.py
+-rw-r--r--   0        0        0     6148 2023-02-27 16:37:40.000000 maptasker-1.3.3/maptasker/src/.DS_Store
+-rw-r--r--   0        0        0        0 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/__init__.py
+-rw-r--r--   0        0        0      212 2023-03-23 17:49:08.090530 maptasker-1.3.3/maptasker/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3135 2023-04-09 16:37:37.154363 maptasker-1.3.3/maptasker/src/__pycache__/actargs.cpython-310.pyc
+-rw-r--r--   0        0        0     5461 2023-04-13 17:51:08.803769 maptasker-1.3.3/maptasker/src/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0   107715 2023-03-23 17:49:08.156251 maptasker-1.3.3/maptasker/src/__pycache__/actionc.cpython-310.pyc
+-rw-r--r--   0        0        0     2565 2023-04-09 16:37:37.155274 maptasker-1.3.3/maptasker/src/__pycache__/actiond.cpython-310.pyc
+-rw-r--r--   0        0        0     4096 2023-04-14 13:57:38.116885 maptasker-1.3.3/maptasker/src/__pycache__/actione.cpython-310.pyc
+-rw-r--r--   0        0        0     2992 2023-04-13 17:32:39.155638 maptasker-1.3.3/maptasker/src/__pycache__/actionr.cpython-310.pyc
+-rw-r--r--   0        0        0    14483 2023-03-23 17:49:08.400678 maptasker-1.3.3/maptasker/src/__pycache__/actiont.cpython-310.pyc
+-rw-r--r--   0        0        0     1005 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/__pycache__/argsdict.cpython-310.pyc
+-rw-r--r--   0        0        0     1885 2023-04-16 16:38:35.415407 maptasker-1.3.3/maptasker/src/__pycache__/caveats.cpython-310.pyc
+-rw-r--r--   0        0        0     4400 2023-03-23 17:49:08.182225 maptasker-1.3.3/maptasker/src/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0     1717 2023-04-16 15:45:05.862632 maptasker-1.3.3/maptasker/src/__pycache__/colrmode.cpython-310.pyc
+-rw-r--r--   0        0        0     3848 2023-03-23 17:49:08.203819 maptasker-1.3.3/maptasker/src/__pycache__/condition.cpython-310.pyc
+-rw-r--r--   0        0        0      290 2023-04-13 16:13:11.506371 maptasker-1.3.3/maptasker/src/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1135 2023-04-11 19:03:07.815707 maptasker-1.3.3/maptasker/src/__pycache__/debug.cpython-310.pyc
+-rw-r--r--   0        0        0      351 2023-03-23 17:49:08.397467 maptasker-1.3.3/maptasker/src/__pycache__/depricated.cpython-310.pyc
+-rw-r--r--   0        0        0     1232 2023-04-13 16:38:33.007320 maptasker-1.3.3/maptasker/src/__pycache__/frmthtml.cpython-310.pyc
+-rw-r--r--   0        0        0     1348 2023-04-10 14:44:42.113922 maptasker-1.3.3/maptasker/src/__pycache__/getids.cpython-310.pyc
+-rw-r--r--   0        0        0     1636 2023-04-10 14:52:10.413906 maptasker-1.3.3/maptasker/src/__pycache__/getputarg.cpython-310.pyc
+-rw-r--r--   0        0        0      754 2023-03-23 17:49:08.190511 maptasker-1.3.3/maptasker/src/__pycache__/initparg.cpython-310.pyc
+-rw-r--r--   0        0        0     1267 2023-04-09 16:33:30.097241 maptasker-1.3.3/maptasker/src/__pycache__/kidapp.cpython-310.pyc
+-rw-r--r--   0        0        0     5236 2023-04-17 15:14:53.838375 maptasker-1.3.3/maptasker/src/__pycache__/mapit.cpython-310.pyc
+-rw-r--r--   0        0        0     1727 2023-04-10 14:52:10.410513 maptasker-1.3.3/maptasker/src/__pycache__/migrate.cpython-310.pyc
+-rw-r--r--   0        0        0     4219 2023-04-17 15:38:49.141755 maptasker-1.3.3/maptasker/src/__pycache__/outputl.cpython-310.pyc
+-rw-r--r--   0        0        0     4396 2023-03-23 17:49:08.186264 maptasker-1.3.3/maptasker/src/__pycache__/parsearg.cpython-310.pyc
+-rw-r--r--   0        0        0     3872 2023-04-11 16:27:41.747208 maptasker-1.3.3/maptasker/src/__pycache__/prefers.cpython-310.pyc
+-rw-r--r--   0        0        0      811 2023-04-11 19:20:37.385389 maptasker-1.3.3/maptasker/src/__pycache__/priority.cpython-310.pyc
+-rw-r--r--   0        0        0     2104 2023-04-09 16:37:37.296644 maptasker-1.3.3/maptasker/src/__pycache__/proclist.cpython-310.pyc
+-rw-r--r--   0        0        0     4733 2023-04-17 14:57:19.160832 maptasker-1.3.3/maptasker/src/__pycache__/profiles.cpython-310.pyc
+-rw-r--r--   0        0        0      678 2023-03-23 17:49:08.179364 maptasker-1.3.3/maptasker/src/__pycache__/progargs.cpython-310.pyc
+-rw-r--r--   0        0        0     5827 2023-04-12 16:13:37.277181 maptasker-1.3.3/maptasker/src/__pycache__/proginit.cpython-310.pyc
+-rw-r--r--   0        0        0     7211 2023-04-16 16:33:54.842749 maptasker-1.3.3/maptasker/src/__pycache__/projects.cpython-310.pyc
+-rw-r--r--   0        0        0     4273 2023-03-23 17:49:08.181004 maptasker-1.3.3/maptasker/src/__pycache__/runcli.cpython-310.pyc
+-rw-r--r--   0        0        0     1578 2023-04-10 15:06:22.084248 maptasker-1.3.3/maptasker/src/__pycache__/rungui.cpython-310.pyc
+-rw-r--r--   0        0        0     4362 2023-04-11 16:47:22.438398 maptasker-1.3.3/maptasker/src/__pycache__/scenes.cpython-310.pyc
+-rw-r--r--   0        0        0     8098 2023-03-23 17:49:08.215471 maptasker-1.3.3/maptasker/src/__pycache__/servicec.cpython-310.pyc
+-rw-r--r--   0        0        0     1976 2023-04-16 19:09:38.125947 maptasker-1.3.3/maptasker/src/__pycache__/share.cpython-310.pyc
+-rw-r--r--   0        0        0      998 2023-03-23 17:49:08.120911 maptasker-1.3.3/maptasker/src/__pycache__/shellsort.cpython-310.pyc
+-rw-r--r--   0        0        0     2362 2023-04-13 16:19:33.935300 maptasker-1.3.3/maptasker/src/__pycache__/sysconst.cpython-310.pyc
+-rw-r--r--   0        0        0     2471 2023-04-13 17:22:06.645489 maptasker-1.3.3/maptasker/src/__pycache__/taskactn.cpython-310.pyc
+-rw-r--r--   0        0        0     1329 2023-04-10 15:03:06.565941 maptasker-1.3.3/maptasker/src/__pycache__/taskerd.cpython-310.pyc
+-rw-r--r--   0        0        0     8012 2023-04-17 14:57:19.157983 maptasker-1.3.3/maptasker/src/__pycache__/tasks.cpython-310.pyc
+-rw-r--r--   0        0        0     3387 2023-04-16 16:28:05.704058 maptasker-1.3.3/maptasker/src/__pycache__/taskuniq.cpython-310.pyc
+-rw-r--r--   0        0        0    14185 2023-04-10 14:44:20.491744 maptasker-1.3.3/maptasker/src/__pycache__/userintr.cpython-310.pyc
+-rw-r--r--   0        0        0     2538 2023-04-10 19:05:04.241243 maptasker-1.3.3/maptasker/src/__pycache__/xmldata.cpython-310.pyc
+-rw-r--r--   0        0        0     6363 2023-04-09 16:37:34.662793 maptasker-1.3.3/maptasker/src/actargs.py
+-rw-r--r--   0        0        0    14351 2023-04-13 17:51:08.762301 maptasker-1.3.3/maptasker/src/action.py
+-rw-r--r--   0        0        0   150799 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/actionc.py
+-rw-r--r--   0        0        0     6754 2023-04-09 16:37:34.640363 maptasker-1.3.3/maptasker/src/actiond.py
+-rw-r--r--   0        0        0     9805 2023-04-13 19:15:57.876035 maptasker-1.3.3/maptasker/src/actione.py
+-rw-r--r--   0        0        0     7252 2023-04-13 17:32:39.100785 maptasker-1.3.3/maptasker/src/actionr.py
+-rw-r--r--   0        0        0    17381 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/actiont.py
+-rw-r--r--   0        0        0     3397 2023-04-16 16:35:22.994038 maptasker-1.3.3/maptasker/src/caveats.py
+-rw-r--r--   0        0        0     8220 2023-03-23 17:42:41.450000 maptasker-1.3.3/maptasker/src/colors.py
+-rw-r--r--   0        0        0     3276 2023-04-14 15:43:15.116427 maptasker-1.3.3/maptasker/src/colrmode.py
+-rw-r--r--   0        0        0     9131 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/condition.py
+-rw-r--r--   0        0        0     2303 2023-04-13 16:10:32.286658 maptasker-1.3.3/maptasker/src/config.py
+-rw-r--r--   0        0        0     2527 2023-04-11 18:04:19.248727 maptasker-1.3.3/maptasker/src/debug.py
+-rw-r--r--   0        0        0      342 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/depricated.py
+-rw-r--r--   0        0        0     2017 2023-04-13 16:38:32.954840 maptasker-1.3.3/maptasker/src/frmthtml.py
+-rw-r--r--   0        0        0     2441 2023-04-10 14:44:41.937204 maptasker-1.3.3/maptasker/src/getids.py
+-rw-r--r--   0        0        0     3042 2023-04-10 14:52:10.334081 maptasker-1.3.3/maptasker/src/getputarg.py
+-rw-r--r--   0        0        0     2366 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/initparg.py
+-rw-r--r--   0        0        0     2463 2023-04-09 16:33:24.154727 maptasker-1.3.3/maptasker/src/kidapp.py
+-rw-r--r--   0        0        0    15473 2023-04-17 15:14:53.760673 maptasker-1.3.3/maptasker/src/mapit.py
+-rw-r--r--   0        0        0     3459 2023-04-10 14:52:10.335844 maptasker-1.3.3/maptasker/src/migrate.py
+-rw-r--r--   0        0        0     9892 2023-04-17 15:38:49.066257 maptasker-1.3.3/maptasker/src/outputl.py
+-rw-r--r--   0        0        0     8092 2023-03-23 17:42:41.413000 maptasker-1.3.3/maptasker/src/parsearg.py
+-rw-r--r--   0        0        0     7786 2023-04-11 16:25:21.280491 maptasker-1.3.3/maptasker/src/prefers.py
+-rw-r--r--   0        0        0     1684 2023-04-11 19:20:37.207118 maptasker-1.3.3/maptasker/src/priority.py
+-rw-r--r--   0        0        0     4706 2023-04-09 16:37:34.668518 maptasker-1.3.3/maptasker/src/proclist.py
+-rw-r--r--   0        0        0    10653 2023-04-16 19:14:51.915412 maptasker-1.3.3/maptasker/src/profiles.py
+-rw-r--r--   0        0        0     1947 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/progargs.py
+-rw-r--r--   0        0        0    10342 2023-04-12 16:13:37.228970 maptasker-1.3.3/maptasker/src/proginit.py
+-rw-r--r--   0        0        0    15066 2023-04-16 16:33:54.739972 maptasker-1.3.3/maptasker/src/projects.py
+-rw-r--r--   0        0        0     8999 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/runcli.py
+-rw-r--r--   0        0        0     4149 2023-04-10 15:06:22.010146 maptasker-1.3.3/maptasker/src/rungui.py
+-rw-r--r--   0        0        0     7934 2023-04-11 16:43:39.790321 maptasker-1.3.3/maptasker/src/scenes.py
+-rw-r--r--   0        0        0    14219 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/servicec.py
+-rw-r--r--   0        0        0     4290 2023-04-16 19:08:14.858448 maptasker-1.3.3/maptasker/src/share.py
+-rw-r--r--   0        0        0     3354 2023-03-23 17:42:41.454000 maptasker-1.3.3/maptasker/src/shellsort.py
+-rw-r--r--   0        0        0     4056 2023-04-17 15:44:26.479132 maptasker-1.3.3/maptasker/src/sysconst.py
+-rw-r--r--   0        0        0     5820 2023-04-13 17:20:50.341670 maptasker-1.3.3/maptasker/src/taskactn.py
+-rw-r--r--   0        0        0     3100 2023-04-10 15:03:06.364934 maptasker-1.3.3/maptasker/src/taskerd.py
+-rw-r--r--   0        0        0    15369 2023-04-16 19:14:51.911035 maptasker-1.3.3/maptasker/src/tasks.py
+-rw-r--r--   0        0        0     9713 2023-04-16 16:23:58.449719 maptasker-1.3.3/maptasker/src/taskuniq.py
+-rw-r--r--   0        0        0    30601 2023-04-10 14:44:20.412620 maptasker-1.3.3/maptasker/src/userintr.py
+-rw-r--r--   0        0        0     6769 2023-04-10 19:04:43.346454 maptasker-1.3.3/maptasker/src/xmldata.py
+-rw-r--r--   0        0        0     1179 2023-04-09 16:07:12.762776 maptasker-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 maptasker-1.3.3/PKG-INFO
```

### Comparing `maptasker-1.3.2/LICENSE.txt` & `maptasker-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/.DS_Store` & `maptasker-1.3.3/maptasker/.DS_Store`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/.DS_Store` & `maptasker-1.3.3/maptasker/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/actargs.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/actargs.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 23 17:42:41 2023 UTC, .py size: 6328 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,195 +1,196 @@
-00000000: 6f0d 0d0a 0000 0000 918f 1c64 b818 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 cee9 3264 db18 0000  o.........2d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
+00000020: 0012 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a05 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c06 6d07 0200 0100 6d08 5a09 0100  d.l.m.....m.Z...
 00000060: 6404 650a 6405 650b 6406 650c 6407 650c  d.e.d.e.d.e.d.e.
-00000070: 6408 6505 6a0d 6409 6505 6a0d 640a 650a  d.e.j.d.e.j.d.e.
-00000080: 640b 650a 640c 650a 6612 640d 640e 8404  d.e.d.e.f.d.d...
-00000090: 5a0e 640f 6410 8400 5a0f 6403 5300 2911  Z.d.d...Z.d.S.).
-000000a0: e900 0000 0029 01da 1670 726f 6365 7373  .....)...process
-000000b0: 5f63 6f6e 6469 7469 6f6e 5f6c 6973 7429  _condition_list)
-000000c0: 01da 066c 6f67 6765 724e da11 6576 616c  ...loggerN..eval
-000000d0: 7561 7465 645f 7265 7375 6c74 73da 0361  uated_results..a
-000000e0: 7267 da07 6172 6765 7661 6cda 0761 7267  rg..argeval..arg
-000000f0: 7479 7065 da0b 636f 6465 5f61 6374 696f  type..code_actio
-00000100: 6eda 0b61 6374 696f 6e5f 7479 7065 da08  n..action_type..
-00000110: 636f 6c6f 726d 6170 da0c 7072 6f67 7261  colormap..progra
-00000120: 6d5f 6172 6773 da06 7265 7475 726e 6308  m_args..returnc.
-00000130: 0000 0000 0000 0000 0000 0018 0000 0007  ................
-00000140: 0000 0043 0000 0073 f202 0000 7c03 0400  ...C...s....|...
-00000150: 6401 6b02 7223 0100 6402 7c00 6403 3c00  d.k.r#..d.|.d.<.
-00000160: 7c00 6404 1900 a000 6405 7401 7c01 8301  |.d.....d.t.|...
-00000170: 9b00 9d02 a101 0100 7c00 6406 1900 a000  ........|.d.....
-00000180: 7c02 a101 0100 6402 7c00 6407 3c00 7c00  |.....d.|.d.<.|.
-00000190: 5300 0400 6408 6b02 7245 0100 6402 7c00  S...d.k.rE..d.|.
-000001a0: 6403 3c00 7c00 6409 1900 a000 6405 7401  d.<.|.d.....d.t.
-000001b0: 7c01 8301 9b00 9d02 a101 0100 7c00 640a  |...........|.d.
-000001c0: 1900 a000 7c02 a101 0100 6402 7c00 6407  ....|.....d.|.d.
-000001d0: 3c00 7c00 5300 0400 640b 6b02 727e 0100  <.|.S...d.k.r~..
-000001e0: 7c00 6404 1900 a000 6405 7401 7c01 8301  |.d.....d.t.|...
-000001f0: 9b00 9d02 a101 0100 7c00 6406 1900 a000  ........|.d.....
-00000200: 7c02 a101 0100 7402 a003 7c04 7c05 7c06  |.....t...|.|.|.
-00000210: 7c07 a104 5c04 7d08 7d09 7d0a 7d0b 7c00  |...\.}.}.}.}.|.
-00000220: 640c 1900 a000 7c08 9b00 640d 7c09 9b00  d.....|...d.|...
-00000230: 640d 7c0a 9b00 9d05 a101 0100 6402 7c00  d.|.........d.|.
-00000240: 6407 3c00 7c00 5300 0400 640e 6b02 72d7  d.<.|.S...d.k.r.
-00000250: 0100 7c00 6404 1900 a000 6405 7401 7c01  ..|.d.....d.t.|.
-00000260: 8301 9b00 9d02 a101 0100 7c00 6406 1900  ..........|.d...
-00000270: a000 7c02 a101 0100 640f 7d0c 7404 7c04  ..|.....d.}.t.|.
-00000280: 8301 5c02 7d0d 7d0e 7405 7c0d 8301 4400  ..\.}.}.t.|...D.
-00000290: 5d27 5c02 7d0f 7d10 7c0c 9b00 6410 7c10  ]'\.}.}.|...d.|.
-000002a0: 6411 1900 9b00 7c10 6412 1900 9b00 7c10  d.....|.d.....|.
-000002b0: 6413 1900 9b00 9d05 7d0c 7c0e 72c9 7406  d.......}.|.r.t.
-000002c0: 7c0e 8301 7c0f 6b04 72c9 7c0c 9b00 6410  |...|.k.r.|...d.
-000002d0: 7c0e 7c0f 1900 9b00 6410 9d04 7d0c 71a2  |.|.....d...}.q.
-000002e0: 7c00 6414 1900 a000 7c0c a101 0100 6402  |.d.....|.....d.
-000002f0: 7c00 6407 3c00 7c00 5300 0400 6415 6b02  |.d.<.|.S...d.k.
-00000300: 9001 722f 0100 6416 5c02 7d11 7d12 7c04  ..r/..d.\.}.}.|.
-00000310: a007 6415 a101 7d13 7c13 a007 6417 a101  ..d...}.|...d...
-00000320: 6418 7501 72f3 7c13 a007 6417 a101 6a08  d.u.r.|...d...j.
-00000330: 7d11 7c13 a007 6419 a101 6418 7501 9001  }.|...d...d.u...
-00000340: 7204 641a 7c13 a007 6419 a101 6a08 1700  r.d.|...d...j...
-00000350: 7d12 6e0e 7c13 a007 641b a101 6418 7501  }.n.|...d...d.u.
-00000360: 9001 7212 7c13 a007 641b a101 6a08 7d11  ..r.|...d...j.}.
-00000370: 7c11 9001 7226 7c00 641c 1900 a000 7c02  |...r&|.d.....|.
-00000380: 7c11 1700 7c12 1700 a101 0100 6402 7c00  |...|.......d.|.
-00000390: 6407 3c00 7c00 5300 7c00 641c 1900 a000  d.<.|.S.|.d.....
-000003a0: 6410 a101 0100 7c00 5300 641d 6b02 9001  d.....|.S.d.k...
-000003b0: 726d 7c04 a007 641d a101 7d14 7c14 a007  rm|...d...}.|...
-000003c0: 641e a101 7d15 7c15 a007 641f a101 7d16  d...}.|...d...}.
-000003d0: 7c16 6418 7501 9001 726b 7c16 6a08 6418  |.d.u...rk|.j.d.
-000003e0: 7501 9001 726b 7c16 6a08 a009 6420 6421  u...rk|.j...d d!
-000003f0: a102 7d17 7c17 a009 6422 6423 a102 7d17  ..}.|...d"d#..}.
-00000400: 7c17 a009 6424 6425 a102 7d17 7c00 6426  |...d$d%..}.|.d&
-00000410: 1900 a000 7c17 a101 0100 6402 7c00 6407  ....|.....d.|.d.
-00000420: 3c00 7c00 5300 0900 740a a00b 6427 7c03  <.|.S...t...d'|.
-00000430: 1700 6428 1700 a101 0100 7c00 5300 2929  ..d(......|.S.))
-00000440: 6199 0100 000a 0a20 2020 203a 7061 7261  a......    :para
-00000450: 6d20 6576 616c 7561 7465 645f 7265 7375  m evaluated_resu
-00000460: 6c74 733a 2061 6c6c 2074 6865 2041 6374  lts: all the Act
-00000470: 696f 6e20 6172 6775 6d65 6e74 2022 7479  ion argument "ty
-00000480: 7065 7322 2061 6e64 2022 6172 6775 6d65  pes" and "argume
-00000490: 6e74 7322 0a20 2020 203a 7061 7261 6d20  nts".    :param 
-000004a0: 6172 673a 2074 6865 2069 6e63 6f6d 696e  arg: the incomin
-000004b0: 6720 6172 6775 6d65 6e74 0a20 2020 203a  g argument.    :
-000004c0: 7061 7261 6d20 6172 6765 7661 6c3a 2074  param argeval: t
-000004d0: 6865 2065 7661 6c75 6174 696f 6e20 6172  he evaluation ar
-000004e0: 6775 6d65 6e74 0a20 2020 203a 7061 7261  gument.    :para
-000004f0: 6d20 6172 6774 7970 653a 2074 6865 2061  m argtype: the a
-00000500: 7267 756d 656e 7420 2274 7970 6522 0a20  rgument "type". 
-00000510: 2020 203a 7061 7261 6d20 636f 6465 5f61     :param code_a
-00000520: 6374 696f 6e3a 2074 6865 2041 6374 696f  ction: the Actio
-00000530: 6e20 636f 6465 0a20 2020 203a 7061 7261  n code.    :para
-00000540: 6d20 6163 7469 6f6e 5f74 7970 653a 2074  m action_type: t
-00000550: 6865 2041 6374 696f 6e20 7479 7065 0a20  he Action type. 
-00000560: 2020 203a 7061 7261 6d20 636f 6c6f 726d     :param colorm
-00000570: 6170 3a20 636f 6c6f 7273 2074 6f20 7573  ap: colors to us
-00000580: 6520 696e 206f 7574 7075 740a 2020 2020  e in output.    
-00000590: 3a70 6172 616d 2070 726f 6772 616d 5f61  :param program_a
-000005a0: 7267 733a 2072 756e 7469 6d65 2061 7267  rgs: runtime arg
-000005b0: 756d 656e 7473 0a20 2020 203a 7265 7475  uments.    :retu
-000005c0: 726e 3a20 6469 6374 696f 6e61 7279 206f  rn: dictionary o
-000005d0: 6620 7265 7375 6c74 730a 2020 2020 da03  f results.    ..
-000005e0: 5374 7254 da0c 6765 745f 786d 6c5f 666c  StrT..get_xml_fl
-000005f0: 6167 da07 7374 7261 7267 7372 0500 0000  ag..strargsr....
-00000600: da07 7374 7265 7661 6cda 1372 6574 7572  ..streval..retur
-00000610: 6e69 6e67 5f73 6f6d 6574 6869 6e67 da03  ning_something..
-00000620: 496e 74da 0769 6e74 6172 6773 da07 696e  Int..intargs..in
-00000630: 7465 7661 6cda 0341 7070 da0a 7265 7375  teval..App..resu
-00000640: 6c74 5f61 7070 7a02 2c20 da0d 436f 6e64  lt_appz., ..Cond
-00000650: 6974 696f 6e4c 6973 74da 00fa 0120 7201  itionList.... r.
-00000660: 0000 00e9 0100 0000 e902 0000 00da 0a72  ...............r
-00000670: 6573 756c 745f 636f 6eda 0349 6d67 2902  esult_con..Img).
-00000680: 7218 0000 0072 1800 0000 5a03 6e6d 654e  r....r....Z.nmeN
-00000690: 5a03 706b 677a 0a2c 2050 6163 6b61 6765  Z.pkgz., Package
-000006a0: 3ada 0376 6172 da0a 7265 7375 6c74 5f69  :..var..result_i
-000006b0: 6d67 da06 4275 6e64 6c65 5a04 5661 6c73  mg..BundleZ.Vals
-000006c0: 7a2c 636f 6d2e 7477 6f66 6f72 7479 666f  z,com.twofortyfo
-000006d0: 7572 616d 2e6c 6f63 616c 652e 696e 7465  uram.locale.inte
-000006e0: 6e74 2e65 7874 7261 2e42 4c55 5242 7a0f  nt.extra.BLURBz.
-000006f0: 3c2f 666f 6e74 3e3c 6272 3e3c 6272 3e7a  </font><br><br>z
-00000700: 083c 6272 3e3c 6272 3e7a 0426 6c74 3bfa  .<br><br>z.&lt;.
-00000710: 013c 7a04 2667 743b fa01 3eda 0a72 6573  .<z.&gt;..>..res
-00000720: 756c 745f 6275 6e7a 2467 6574 5f61 6374  ult_bunz$get_act
-00000730: 696f 6e5f 7265 7375 6c74 733a 2075 6e6b  ion_results: unk
-00000740: 6e6f 776e 2061 7267 7479 7065 3a7a 0521  nown argtype:z.!
-00000750: 2121 2121 290c da06 6170 7065 6e64 da03  !!!!)...append..
-00000760: 7374 72da 0a67 6574 5f61 6374 696f 6eda  str..get_action.
-00000770: 0f67 6574 5f61 7070 5f64 6574 6169 6c73  .get_app_details
-00000780: 7202 0000 00da 0965 6e75 6d65 7261 7465  r......enumerate
-00000790: da03 6c65 6eda 0466 696e 64da 0474 6578  ..len..find..tex
-000007a0: 74da 0772 6570 6c61 6365 7203 0000 00da  t..replacer.....
-000007b0: 0564 6562 7567 2918 7204 0000 0072 0500  .debug).r....r..
-000007c0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000007d0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-000007e0: da09 6170 705f 636c 6173 73da 0761 7070  ..app_class..app
-000007f0: 5f70 6b67 da03 6170 70da 0565 7874 7261  _pkg..app..extra
-00000800: 5a10 6669 6e61 6c5f 636f 6e64 6974 696f  Z.final_conditio
-00000810: 6e73 5a0e 636f 6e64 6974 696f 6e5f 6c69  nsZ.condition_li
-00000820: 7374 5a0c 626f 6f6c 6561 6e5f 6c69 7374  stZ.boolean_list
-00000830: 5a04 6e75 6d78 5a09 636f 6e64 6974 696f  Z.numxZ.conditio
-00000840: 6e5a 0569 6d61 6765 da07 7061 636b 6167  nZ.image..packag
-00000850: 65da 0563 6869 6c64 5a06 6368 696c 6431  e..childZ.child1
-00000860: 5a06 6368 696c 6432 5a06 6368 696c 6433  Z.child2Z.child3
-00000870: 5a0c 636c 6561 6e5f 7374 7269 6e67 a900  Z.clean_string..
-00000880: 7234 0000 00fa 762f 5573 6572 732f 6d69  r4....v/Users/mi
-00000890: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
-000008a0: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
-000008b0: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
-000008c0: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
-000008d0: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
-000008e0: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
-000008f0: 7263 2f61 6374 6172 6773 2e70 79da 1467  rc/actargs.py..g
-00000900: 6574 5f61 6374 696f 6e5f 6172 6775 6d65  et_action_argume
-00000910: 6e74 7313 0000 0073 8a00 0000 0216 0a01  nts....s........
-00000920: 0801 1801 0e01 0801 043b 0ac6 0801 1801  .........;......
-00000930: 0e01 0801 0436 0acb 1801 0e01 0401 0801  .....6..........
-00000940: 0cff 1e03 0801 042e 0ad3 1801 0e01 0401  ................
-00000950: 0c01 1002 2002 02ff 1003 1401 0280 0e01  .... ...........
-00000960: 0801 0420 0ce1 0801 0a01 0e01 0c01 1001  ... ............
-00000970: 1201 1001 0c01 0601 1601 0801 0414 0eee  ................
-00000980: 0412 08ef 0a01 0a01 0401 0201 04ff 1603  ................
-00000990: 0e02 0c01 0c01 0e01 0801 0405 02fc 0401  ................
-000009a0: 0a01 04ff 0403 7236 0000 0063 0900 0000  ......r6...c....
-000009b0: 0000 0000 0000 0000 0e00 0000 0a00 0000  ................
-000009c0: 4300 0000 7370 0000 0074 007c 0083 0144  C...sp...t.|...D
-000009d0: 005d 315c 027d 097d 0a7c 0a64 016b 0272  .]1\.}.}.|.d.k.r
-000009e0: 0e7c 096e 087c 027c 0119 0064 0219 00a0  .|.n.|.|...d....
-000009f0: 017c 0aa1 017d 0b7c 037c 0919 007d 0c7c  .|...}.|.|...}.|
-00000a00: 027c 0119 0064 0319 007c 0b19 007d 0d7c  .|...d...|...}.|
-00000a10: 0864 0419 00a0 027c 0da1 0101 0074 037c  .d.....|.....t.|
-00000a20: 087c 0a7c 0c7c 0d7c 047c 057c 067c 0783  .|.|.|.|.|.|.|..
-00000a30: 087d 0871 047c 0853 0029 054e da02 6966  .}.q.|.S.).N..if
-00000a40: da04 6172 6773 da05 7479 7065 73da 1170  ..args..types..p
-00000a50: 6f73 6974 696f 6e5f 6172 675f 7479 7065  osition_arg_type
-00000a60: 2904 7228 0000 00da 0569 6e64 6578 7224  ).r(.....indexr$
-00000a70: 0000 0072 3600 0000 290e da08 6172 675f  ...r6...)...arg_
-00000a80: 6c69 7374 da09 6469 6374 5f63 6f64 65da  list..dict_code.
-00000a90: 116c 6f6f 6b75 705f 636f 6465 5f65 6e74  .lookup_code_ent
-00000aa0: 7279 da0d 6576 616c 7561 7465 5f6c 6973  ry..evaluate_lis
-00000ab0: 7472 0800 0000 7209 0000 0072 0a00 0000  tr....r....r....
-00000ac0: 720b 0000 0072 0400 0000 5a03 6e75 6d72  r....r....Z.numr
-00000ad0: 0500 0000 723b 0000 0072 0600 0000 7207  ....r;...r....r.
-00000ae0: 0000 0072 3400 0000 7234 0000 0072 3500  ...r4...r4...r5.
-00000af0: 0000 da0b 6163 7469 6f6e 5f61 7267 736f  ....action_argso
-00000b00: 0000 0073 2000 0000 100b 1e02 0802 1001  ...s ...........
-00000b10: 0e01 0201 0201 0201 0201 0201 0201 0201  ................
-00000b20: 0201 0201 06f8 040b 7240 0000 0029 105a  ........r@...).Z
-00000b30: 156d 6170 7461 736b 6572 2e73 7263 2e61  .maptasker.src.a
-00000b40: 6374 696f 6e64 7202 0000 00da 166d 6170  ctiondr......map
-00000b50: 7461 736b 6572 2e73 7263 2e73 7973 636f  tasker.src.sysco
-00000b60: 6e73 7472 0300 0000 da15 786d 6c2e 6574  nstr......xml.et
-00000b70: 7265 652e 456c 656d 656e 7454 7265 65da  ree.ElementTree.
-00000b80: 0378 6d6c da14 6d61 7074 6173 6b65 722e  .xml..maptasker.
-00000b90: 7372 632e 6163 7469 6f6e da03 7372 63da  src.action..src.
-00000ba0: 0661 6374 696f 6e72 2600 0000 da04 6469  .actionr&.....di
-00000bb0: 6374 da06 6f62 6a65 6374 da04 6c69 7374  ct..object..list
-00000bc0: da05 6574 7265 6572 3600 0000 7240 0000  ..etreer6...r@..
-00000bd0: 0072 3400 0000 7234 0000 0072 3400 0000  .r4...r4...r4...
-00000be0: 7235 0000 00da 083c 6d6f 6475 6c65 3e01  r5.....<module>.
-00000bf0: 0000 0073 3000 0000 0c0c 0c01 0801 1201  ...s0...........
-00000c00: 0203 0201 02ff 0202 02fe 0203 02fd 0204  ................
-00000c10: 02fc 0405 02fb 0406 02fa 0207 02f9 0208  ................
-00000c20: 02f8 0209 0af7 0c5c                      .......\
+00000070: 6408 6505 6a0d 6a0e 6409 6505 6a0d 6a0e  d.e.j.j.d.e.j.j.
+00000080: 640a 650a 640b 650a 640c 650a 6612 640d  d.e.d.e.d.e.f.d.
+00000090: 640e 8404 5a0f 640f 6410 8400 5a10 6403  d...Z.d.d...Z.d.
+000000a0: 5300 2911 e900 0000 0029 01da 1670 726f  S.)......)...pro
+000000b0: 6365 7373 5f63 6f6e 6469 7469 6f6e 5f6c  cess_condition_l
+000000c0: 6973 7429 01da 066c 6f67 6765 724e da11  ist)...loggerN..
+000000d0: 6576 616c 7561 7465 645f 7265 7375 6c74  evaluated_result
+000000e0: 73da 0361 7267 da07 6172 6765 7661 6cda  s..arg..argeval.
+000000f0: 0761 7267 7479 7065 da0b 636f 6465 5f61  .argtype..code_a
+00000100: 6374 696f 6eda 0b61 6374 696f 6e5f 7479  ction..action_ty
+00000110: 7065 da08 636f 6c6f 726d 6170 da0c 7072  pe..colormap..pr
+00000120: 6f67 7261 6d5f 6172 6773 da06 7265 7475  ogram_args..retu
+00000130: 726e 6308 0000 0000 0000 0000 0000 0018  rnc.............
+00000140: 0000 0007 0000 0043 0000 0073 f202 0000  .......C...s....
+00000150: 7c03 0400 6401 6b02 7223 0100 6402 7c00  |...d.k.r#..d.|.
+00000160: 6403 3c00 7c00 6404 1900 a000 6405 7401  d.<.|.d.....d.t.
+00000170: 7c01 8301 9b00 9d02 a101 0100 7c00 6406  |...........|.d.
+00000180: 1900 a000 7c02 a101 0100 6402 7c00 6407  ....|.....d.|.d.
+00000190: 3c00 7c00 5300 0400 6408 6b02 7245 0100  <.|.S...d.k.rE..
+000001a0: 6402 7c00 6403 3c00 7c00 6409 1900 a000  d.|.d.<.|.d.....
+000001b0: 6405 7401 7c01 8301 9b00 9d02 a101 0100  d.t.|...........
+000001c0: 7c00 640a 1900 a000 7c02 a101 0100 6402  |.d.....|.....d.
+000001d0: 7c00 6407 3c00 7c00 5300 0400 640b 6b02  |.d.<.|.S...d.k.
+000001e0: 727e 0100 7c00 6404 1900 a000 6405 7401  r~..|.d.....d.t.
+000001f0: 7c01 8301 9b00 9d02 a101 0100 7c00 6406  |...........|.d.
+00000200: 1900 a000 7c02 a101 0100 7402 a003 7c04  ....|.....t...|.
+00000210: 7c05 7c06 7c07 a104 5c04 7d08 7d09 7d0a  |.|.|...\.}.}.}.
+00000220: 7d0b 7c00 640c 1900 a000 7c08 9b00 640d  }.|.d.....|...d.
+00000230: 7c09 9b00 640d 7c0a 9b00 9d05 a101 0100  |...d.|.........
+00000240: 6402 7c00 6407 3c00 7c00 5300 0400 640e  d.|.d.<.|.S...d.
+00000250: 6b02 72d7 0100 7c00 6404 1900 a000 6405  k.r...|.d.....d.
+00000260: 7401 7c01 8301 9b00 9d02 a101 0100 7c00  t.|...........|.
+00000270: 6406 1900 a000 7c02 a101 0100 640f 7d0c  d.....|.....d.}.
+00000280: 7404 7c04 8301 5c02 7d0d 7d0e 7405 7c0d  t.|...\.}.}.t.|.
+00000290: 8301 4400 5d27 5c02 7d0f 7d10 7c0c 9b00  ..D.]'\.}.}.|...
+000002a0: 6410 7c10 6411 1900 9b00 7c10 6412 1900  d.|.d.....|.d...
+000002b0: 9b00 7c10 6413 1900 9b00 9d05 7d0c 7c0e  ..|.d.......}.|.
+000002c0: 72c9 7406 7c0e 8301 7c0f 6b04 72c9 7c0c  r.t.|...|.k.r.|.
+000002d0: 9b00 6410 7c0e 7c0f 1900 9b00 6410 9d04  ..d.|.|.....d...
+000002e0: 7d0c 71a2 7c00 6414 1900 a000 7c0c a101  }.q.|.d.....|...
+000002f0: 0100 6402 7c00 6407 3c00 7c00 5300 0400  ..d.|.d.<.|.S...
+00000300: 6415 6b02 9001 722f 0100 6416 5c02 7d11  d.k...r/..d.\.}.
+00000310: 7d12 7c04 a007 6415 a101 7d13 7c13 a007  }.|...d...}.|...
+00000320: 6417 a101 6418 7501 72f3 7c13 a007 6417  d...d.u.r.|...d.
+00000330: a101 6a08 7d11 7c13 a007 6419 a101 6418  ..j.}.|...d...d.
+00000340: 7501 9001 7204 641a 7c13 a007 6419 a101  u...r.d.|...d...
+00000350: 6a08 1700 7d12 6e0e 7c13 a007 641b a101  j...}.n.|...d...
+00000360: 6418 7501 9001 7212 7c13 a007 641b a101  d.u...r.|...d...
+00000370: 6a08 7d11 7c11 9001 7226 7c00 641c 1900  j.}.|...r&|.d...
+00000380: a000 7c02 7c11 1700 7c12 1700 a101 0100  ..|.|...|.......
+00000390: 6402 7c00 6407 3c00 7c00 5300 7c00 641c  d.|.d.<.|.S.|.d.
+000003a0: 1900 a000 6410 a101 0100 7c00 5300 641d  ....d.....|.S.d.
+000003b0: 6b02 9001 726d 7c04 a007 641d a101 7d14  k...rm|...d...}.
+000003c0: 7c14 a007 641e a101 7d15 7c15 a007 641f  |...d...}.|...d.
+000003d0: a101 7d16 7c16 6418 7501 9001 726b 7c16  ..}.|.d.u...rk|.
+000003e0: 6a08 6418 7501 9001 726b 7c16 6a08 a009  j.d.u...rk|.j...
+000003f0: 6420 6421 a102 7d17 7c17 a009 6422 6423  d d!..}.|...d"d#
+00000400: a102 7d17 7c17 a009 6424 6425 a102 7d17  ..}.|...d$d%..}.
+00000410: 7c00 6426 1900 a000 7c17 a101 0100 6402  |.d&....|.....d.
+00000420: 7c00 6407 3c00 7c00 5300 0900 740a a00b  |.d.<.|.S...t...
+00000430: 6427 7c03 1700 6428 1700 a101 0100 7c00  d'|...d(......|.
+00000440: 5300 2929 6199 0100 000a 0a20 2020 203a  S.))a......    :
+00000450: 7061 7261 6d20 6576 616c 7561 7465 645f  param evaluated_
+00000460: 7265 7375 6c74 733a 2061 6c6c 2074 6865  results: all the
+00000470: 2041 6374 696f 6e20 6172 6775 6d65 6e74   Action argument
+00000480: 2022 7479 7065 7322 2061 6e64 2022 6172   "types" and "ar
+00000490: 6775 6d65 6e74 7322 0a20 2020 203a 7061  guments".    :pa
+000004a0: 7261 6d20 6172 673a 2074 6865 2069 6e63  ram arg: the inc
+000004b0: 6f6d 696e 6720 6172 6775 6d65 6e74 0a20  oming argument. 
+000004c0: 2020 203a 7061 7261 6d20 6172 6765 7661     :param argeva
+000004d0: 6c3a 2074 6865 2065 7661 6c75 6174 696f  l: the evaluatio
+000004e0: 6e20 6172 6775 6d65 6e74 0a20 2020 203a  n argument.    :
+000004f0: 7061 7261 6d20 6172 6774 7970 653a 2074  param argtype: t
+00000500: 6865 2061 7267 756d 656e 7420 2274 7970  he argument "typ
+00000510: 6522 0a20 2020 203a 7061 7261 6d20 636f  e".    :param co
+00000520: 6465 5f61 6374 696f 6e3a 2074 6865 2041  de_action: the A
+00000530: 6374 696f 6e20 636f 6465 0a20 2020 203a  ction code.    :
+00000540: 7061 7261 6d20 6163 7469 6f6e 5f74 7970  param action_typ
+00000550: 653a 2074 6865 2041 6374 696f 6e20 7479  e: the Action ty
+00000560: 7065 0a20 2020 203a 7061 7261 6d20 636f  pe.    :param co
+00000570: 6c6f 726d 6170 3a20 636f 6c6f 7273 2074  lormap: colors t
+00000580: 6f20 7573 6520 696e 206f 7574 7075 740a  o use in output.
+00000590: 2020 2020 3a70 6172 616d 2070 726f 6772      :param progr
+000005a0: 616d 5f61 7267 733a 2072 756e 7469 6d65  am_args: runtime
+000005b0: 2061 7267 756d 656e 7473 0a20 2020 203a   arguments.    :
+000005c0: 7265 7475 726e 3a20 6469 6374 696f 6e61  return: dictiona
+000005d0: 7279 206f 6620 7265 7375 6c74 730a 2020  ry of results.  
+000005e0: 2020 da03 5374 7254 da0c 6765 745f 786d    ..StrT..get_xm
+000005f0: 6c5f 666c 6167 da07 7374 7261 7267 7372  l_flag..strargsr
+00000600: 0500 0000 da07 7374 7265 7661 6cda 1372  ......streval..r
+00000610: 6574 7572 6e69 6e67 5f73 6f6d 6574 6869  eturning_somethi
+00000620: 6e67 da03 496e 74da 0769 6e74 6172 6773  ng..Int..intargs
+00000630: da07 696e 7465 7661 6cda 0341 7070 da0a  ..inteval..App..
+00000640: 7265 7375 6c74 5f61 7070 7a02 2c20 da0d  result_appz., ..
+00000650: 436f 6e64 6974 696f 6e4c 6973 74da 00fa  ConditionList...
+00000660: 0120 7201 0000 00e9 0100 0000 e902 0000  . r.............
+00000670: 00da 0a72 6573 756c 745f 636f 6eda 0349  ...result_con..I
+00000680: 6d67 2902 7218 0000 0072 1800 0000 5a03  mg).r....r....Z.
+00000690: 6e6d 654e 5a03 706b 677a 0a2c 2050 6163  nmeNZ.pkgz., Pac
+000006a0: 6b61 6765 3ada 0376 6172 da0a 7265 7375  kage:..var..resu
+000006b0: 6c74 5f69 6d67 da06 4275 6e64 6c65 5a04  lt_img..BundleZ.
+000006c0: 5661 6c73 7a2c 636f 6d2e 7477 6f66 6f72  Valsz,com.twofor
+000006d0: 7479 666f 7572 616d 2e6c 6f63 616c 652e  tyfouram.locale.
+000006e0: 696e 7465 6e74 2e65 7874 7261 2e42 4c55  intent.extra.BLU
+000006f0: 5242 7a0f 3c2f 666f 6e74 3e3c 6272 3e3c  RBz.</font><br><
+00000700: 6272 3e7a 083c 6272 3e3c 6272 3e7a 0426  br>z.<br><br>z.&
+00000710: 6c74 3bfa 013c 7a04 2667 743b fa01 3eda  lt;..<z.&gt;..>.
+00000720: 0a72 6573 756c 745f 6275 6e7a 2467 6574  .result_bunz$get
+00000730: 5f61 6374 696f 6e5f 7265 7375 6c74 733a  _action_results:
+00000740: 2075 6e6b 6e6f 776e 2061 7267 7479 7065   unknown argtype
+00000750: 3a7a 0521 2121 2121 290c da06 6170 7065  :z.!!!!!)...appe
+00000760: 6e64 da03 7374 72da 0a67 6574 5f61 6374  nd..str..get_act
+00000770: 696f 6eda 0f67 6574 5f61 7070 5f64 6574  ion..get_app_det
+00000780: 6169 6c73 7202 0000 00da 0965 6e75 6d65  ailsr......enume
+00000790: 7261 7465 da03 6c65 6eda 0466 696e 64da  rate..len..find.
+000007a0: 0474 6578 74da 0772 6570 6c61 6365 7203  .text..replacer.
+000007b0: 0000 00da 0564 6562 7567 2918 7204 0000  .....debug).r...
+000007c0: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+000007d0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000007e0: 0b00 0000 da09 6170 705f 636c 6173 73da  ......app_class.
+000007f0: 0761 7070 5f70 6b67 da03 6170 70da 0565  .app_pkg..app..e
+00000800: 7874 7261 5a10 6669 6e61 6c5f 636f 6e64  xtraZ.final_cond
+00000810: 6974 696f 6e73 5a0e 636f 6e64 6974 696f  itionsZ.conditio
+00000820: 6e5f 6c69 7374 5a0c 626f 6f6c 6561 6e5f  n_listZ.boolean_
+00000830: 6c69 7374 5a04 6e75 6d78 5a09 636f 6e64  listZ.numxZ.cond
+00000840: 6974 696f 6e5a 0569 6d61 6765 da07 7061  itionZ.image..pa
+00000850: 636b 6167 65da 0563 6869 6c64 5a06 6368  ckage..childZ.ch
+00000860: 696c 6431 5a06 6368 696c 6432 5a06 6368  ild1Z.child2Z.ch
+00000870: 696c 6433 5a0c 636c 6561 6e5f 7374 7269  ild3Z.clean_stri
+00000880: 6e67 a900 7234 0000 00fa 762f 5573 6572  ng..r4....v/User
+00000890: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
+000008a0: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
+000008b0: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
+000008c0: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
+000008d0: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
+000008e0: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
+000008f0: 6572 2f73 7263 2f61 6374 6172 6773 2e70  er/src/actargs.p
+00000900: 79da 1467 6574 5f61 6374 696f 6e5f 6172  y..get_action_ar
+00000910: 6775 6d65 6e74 7313 0000 0073 8a00 0000  guments....s....
+00000920: 0216 0a01 0801 1801 0e01 0801 043b 0ac6  .............;..
+00000930: 0801 1801 0e01 0801 0436 0acb 1801 0e01  .........6......
+00000940: 0401 0801 0cff 1e03 0801 042e 0ad3 1801  ................
+00000950: 0e01 0401 0c01 1002 2002 02ff 1003 1401  ........ .......
+00000960: 0280 0e01 0801 0420 0ce1 0801 0a01 0e01  ....... ........
+00000970: 0c01 1001 1201 1001 0c01 0601 1601 0801  ................
+00000980: 0414 0eee 0412 08ef 0a01 0a01 0401 0201  ................
+00000990: 04ff 1603 0e02 0c01 0c01 0e01 0801 0405  ................
+000009a0: 02fc 0401 0a01 04ff 0403 7236 0000 0063  ..........r6...c
+000009b0: 0900 0000 0000 0000 0000 0000 0e00 0000  ................
+000009c0: 0a00 0000 4300 0000 7370 0000 0074 007c  ....C...sp...t.|
+000009d0: 0083 0144 005d 315c 027d 097d 0a7c 0a64  ...D.]1\.}.}.|.d
+000009e0: 016b 0272 0e7c 096e 087c 027c 0119 0064  .k.r.|.n.|.|...d
+000009f0: 0219 00a0 017c 0aa1 017d 0b7c 037c 0919  .....|...}.|.|..
+00000a00: 007d 0c7c 027c 0119 0064 0319 007c 0b19  .}.|.|...d...|..
+00000a10: 007d 0d7c 0864 0419 00a0 027c 0da1 0101  .}.|.d.....|....
+00000a20: 0074 037c 087c 0a7c 0c7c 0d7c 047c 057c  .t.|.|.|.|.|.|.|
+00000a30: 067c 0783 087d 0871 047c 0853 0029 054e  .|...}.q.|.S.).N
+00000a40: da02 6966 da04 6172 6773 da05 7479 7065  ..if..args..type
+00000a50: 73da 1170 6f73 6974 696f 6e5f 6172 675f  s..position_arg_
+00000a60: 7479 7065 2904 7228 0000 00da 0569 6e64  type).r(.....ind
+00000a70: 6578 7224 0000 0072 3600 0000 290e da08  exr$...r6...)...
+00000a80: 6172 675f 6c69 7374 da09 6469 6374 5f63  arg_list..dict_c
+00000a90: 6f64 65da 116c 6f6f 6b75 705f 636f 6465  ode..lookup_code
+00000aa0: 5f65 6e74 7279 da0d 6576 616c 7561 7465  _entry..evaluate
+00000ab0: 5f6c 6973 7472 0800 0000 7209 0000 0072  _listr....r....r
+00000ac0: 0a00 0000 720b 0000 0072 0400 0000 5a03  ....r....r....Z.
+00000ad0: 6e75 6d72 0500 0000 723b 0000 0072 0600  numr....r;...r..
+00000ae0: 0000 7207 0000 0072 3400 0000 7234 0000  ..r....r4...r4..
+00000af0: 0072 3500 0000 da0b 6163 7469 6f6e 5f61  .r5.....action_a
+00000b00: 7267 736f 0000 0073 2000 0000 100b 1e02  rgso...s .......
+00000b10: 0802 1001 0e01 0201 0201 0201 0201 0201  ................
+00000b20: 0201 0201 0201 0201 06f8 040b 7240 0000  ............r@..
+00000b30: 0029 115a 156d 6170 7461 736b 6572 2e73  .).Z.maptasker.s
+00000b40: 7263 2e61 6374 696f 6e64 7202 0000 00da  rc.actiondr.....
+00000b50: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
+00000b60: 7973 636f 6e73 7472 0300 0000 da16 6465  ysconstr......de
+00000b70: 6675 7365 6478 6d6c 2e45 6c65 6d65 6e74  fusedxml.Element
+00000b80: 5472 6565 da0a 6465 6675 7365 6478 6d6c  Tree..defusedxml
+00000b90: da14 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+00000ba0: 6163 7469 6f6e da03 7372 63da 0661 6374  action..src..act
+00000bb0: 696f 6e72 2600 0000 da04 6469 6374 da06  ionr&.....dict..
+00000bc0: 6f62 6a65 6374 da04 6c69 7374 da0b 456c  object..list..El
+00000bd0: 656d 656e 7454 7265 65da 0358 4d4c 7236  ementTree..XMLr6
+00000be0: 0000 0072 4000 0000 7234 0000 0072 3400  ...r@...r4...r4.
+00000bf0: 0000 7234 0000 0072 3500 0000 da08 3c6d  ..r4...r5.....<m
+00000c00: 6f64 756c 653e 0100 0000 7330 0000 000c  odule>....s0....
+00000c10: 0c0c 0108 0112 0102 0302 0102 ff02 0202  ................
+00000c20: fe02 0302 fd02 0402 fc06 0502 fb06 0602  ................
+00000c30: fa02 0702 f902 0802 f802 090a f70c 5c    ..............\
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/action.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/action.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 15:04:43 2023 UTC, .py size: 14801 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,362 +1,342 @@
-00000000: 6f0d 0d0a 0000 0000 8b3c 2c64 d139 0000  o........<,d.9..
+00000000: 6f0d 0d0a 0000 0000 0c41 3864 0f38 0000  o........A8d.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c03 6d05 5a05 0100 6405 6406 8400  d.l.m.Z...d.d...
-00000060: 5a06 6407 6408 8400 5a07 6409 640a 8400  Z.d.d...Z.d.d...
-00000070: 5a08 640b 640c 8400 5a09 640d 640e 8400  Z.d.d...Z.d.d...
-00000080: 5a0a 640f 6410 8400 5a0b 6411 6412 8400  Z.d.d...Z.d.d...
-00000090: 5a0c 6413 6414 8400 5a0d 6415 6416 8400  Z.d.d...Z.d.d...
-000000a0: 5a0e 6417 6418 8400 5a0f 6401 5300 2919  Z.d.d...Z.d.S.).
-000000b0: e900 0000 004e 2901 da0a 7368 656c 6c5f  .....N)...shell_
-000000c0: 736f 7274 2901 da06 6c6f 6767 6572 2901  sort)...logger).
-000000d0: da0b 464f 4e54 5f54 4f5f 5553 4563 0200  ..FONT_TO_USEc..
-000000e0: 0000 0000 0000 0000 0000 0800 0000 0600  ................
-000000f0: 0000 4300 0000 739e 0000 0067 0067 0067  ..C...s....g.g.g
-00000100: 0003 0302 037d 027d 037d 0464 017d 057c  .....}.}.}.d.}.|
-00000110: 0044 005d 187d 067c 066a 007c 0176 0072  .D.].}.|.j.|.v.r
-00000120: 1471 0c7c 066a 01a0 0264 02a1 017d 077c  .q.|.j...d...}.|
-00000130: 0764 0075 0072 1f71 0c7c 04a0 037c 06a1  .d.u.r.q.|...|..
-00000140: 0101 0071 0c7c 0472 4a74 047c 0464 0364  ...q.|.rJt.|.d.d
-00000150: 0483 0301 007c 0444 005d 117d 067c 03a0  .....|.D.].}.|..
-00000160: 037c 066a 00a1 0101 007c 02a0 037c 066a  .|.j.....|...|.j
-00000170: 01a0 0264 02a1 01a1 0101 0071 2f64 0564  ...d.......q/d.d
-00000180: 0684 0074 057c 0283 0144 0083 017d 057c  ...t.|...D...}.|
-00000190: 027c 037c 0566 0353 0029 074e 7201 0000  .|.|.f.S.).Nr...
-000001a0: 00da 0273 7254 4663 0100 0000 0000 0000  ...srTFc........
-000001b0: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
-000001c0: 7318 0000 0067 007c 005d 085c 027d 017d  s....g.|.].\.}.}
-000001d0: 0274 007c 0183 0191 0271 0253 00a9 0029  .t.|.....q.S...)
-000001e0: 01da 0373 7472 2903 da02 2e30 5a03 696e  ...str)....0Z.in
-000001f0: 64da 0178 7206 0000 0072 0600 0000 fa75  d..xr....r.....u
-00000200: 2f55 7365 7273 2f6d 696b 7275 6269 6e2f  /Users/mikrubin/
-00000210: 4c69 6272 6172 792f 436c 6f75 6453 746f  Library/CloudSto
-00000220: 7261 6765 2f47 6f6f 676c 6544 7269 7665  rage/GoogleDrive
-00000230: 2d6d 696b 7275 6269 6e40 676d 6169 6c2e  -mikrubin@gmail.
-00000240: 636f 6d2f 4d79 2044 7269 7665 2f50 7974  com/My Drive/Pyt
-00000250: 686f 6e2f 6d61 7074 6173 6b65 722f 6d61  hon/maptasker/ma
-00000260: 7074 6173 6b65 722f 7372 632f 6163 7469  ptasker/src/acti
-00000270: 6f6e 2e70 79da 0a3c 6c69 7374 636f 6d70  on.py..<listcomp
-00000280: 3e32 0000 0073 0600 0000 0600 0c01 06ff  >2...s..........
-00000290: 7a1c 6765 745f 6172 6773 2e3c 6c6f 6361  z.get_args.<loca
-000002a0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2906  ls>.<listcomp>).
-000002b0: da03 7461 67da 0661 7474 7269 62da 0367  ..tag..attrib..g
-000002c0: 6574 da06 6170 7065 6e64 7202 0000 00da  et..appendr.....
-000002d0: 0965 6e75 6d65 7261 7465 2908 da06 6163  .enumerate)...ac
-000002e0: 7469 6f6e 5a0b 6967 6e6f 7265 5f6c 6973  tionZ.ignore_lis
-000002f0: 74da 0861 7267 5f6c 6973 745a 0974 7970  t..arg_listZ.typ
-00000300: 655f 6c69 7374 5a0b 6d61 7374 6572 5f6c  e_listZ.master_l
-00000310: 6973 745a 0861 7267 5f6e 756d 73da 0563  istZ.arg_nums..c
-00000320: 6869 6c64 5a0a 6163 7469 6f6e 5f61 7267  hildZ.action_arg
-00000330: 7206 0000 0072 0600 0000 720a 0000 00da  r....r....r.....
-00000340: 0867 6574 5f61 7267 7320 0000 0073 2400  .get_args ...s$.
-00000350: 0000 1001 0401 0801 0a01 0201 0c01 0801  ................
-00000360: 0201 0c02 0402 0c02 0801 0c01 1401 0601  ................
-00000370: 0601 06ff 0a04 7214 0000 0063 0300 0000  ......r....c....
-00000380: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00000390: 4300 0000 7310 0000 007c 0064 016b 0272  C...s....|.d.k.r
-000003a0: 067c 0153 007c 0253 0029 024e da01 3072  .|.S.|.S.).N..0r
-000003b0: 0600 0000 2903 5a09 7468 655f 7661 6c75  ....).Z.the_valu
-000003c0: 655a 0e69 665f 7a65 726f 5f73 7472 696e  eZ.if_zero_strin
-000003d0: 675a 1269 665f 6e6f 745f 7a65 726f 5f73  gZ.if_not_zero_s
-000003e0: 7472 696e 6772 0600 0000 7206 0000 0072  tringr....r....r
-000003f0: 0a00 0000 da0c 6966 5f7a 6572 6f5f 656c  ......if_zero_el
-00000400: 7365 3c00 0000 7302 0000 0010 0172 1600  se<...s......r..
-00000410: 0000 6301 0000 0000 0000 0000 0000 0006  ..c.............
-00000420: 0000 000d 0000 0043 0000 0073 7200 0000  .......C...sr...
-00000430: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
-00000440: 6401 6409 640a 640b 640c 9c0c 7d01 7c00  d.d.d.d.d...}.|.
-00000450: a000 640d a101 6a01 7d02 7c00 a000 640e  ..d...j.}.|...d.
-00000460: a101 6a01 7d03 7c01 7c03 1900 7d04 640f  ..j.}.|.|...}.d.
-00000470: 7c04 7601 7232 7c00 a000 6410 a101 6a01  |.v.r2|...d...j.
-00000480: 6400 7501 7232 7c00 a000 6410 a101 6a01  d.u.r2|...d...j.
-00000490: 7d05 6e02 6411 7d05 7c02 7c04 7c05 6603  }.n.d.}.|.|.|.f.
-000004a0: 5300 2912 4e7a 0320 3d20 7a05 204e 4551  S.).Nz. = z. NEQ
-000004b0: 207a 0320 7e20 7a04 2021 7e20 7a05 2021   z. ~ z. !~ z. !
-000004c0: 7e52 207a 0420 7e52 207a 0320 3c20 7a03  ~R z. ~R z. < z.
-000004d0: 203e 207a 0420 213d 207a 0720 6973 2073   > z. != z. is s
-000004e0: 6574 7a08 206e 6f74 2073 6574 290c 7215  etz. not set).r.
-000004f0: 0000 00da 0131 da01 32da 0133 da01 34da  .....1..2..3..4.
-00000500: 0135 da01 36da 0137 da01 38da 0139 5a02  .5..6..7..8..9Z.
-00000510: 3132 5a02 3133 5a03 6c68 73da 026f 70da  12Z.13Z.lhs..op.
-00000520: 0373 6574 5a03 7268 73da 0029 02da 0466  .setZ.rhs..)...f
-00000530: 696e 64da 0474 6578 7429 0672 1300 0000  ind..text).r....
-00000540: 5a0e 7468 655f 6f70 6572 6174 696f 6e73  Z.the_operations
-00000550: 5a0c 6669 7273 745f 7374 7269 6e67 5a09  Z.first_stringZ.
-00000560: 6f70 6572 6174 696f 6e5a 0d74 6865 5f6f  operationZ.the_o
-00000570: 7065 7261 7469 6f6e 5a0d 7365 636f 6e64  perationZ.second
-00000580: 5f73 7472 696e 6772 0600 0000 7206 0000  _stringr....r...
-00000590: 0072 0a00 0000 da12 6576 616c 7561 7465  .r......evaluate
-000005a0: 5f63 6f6e 6469 7469 6f6e 4300 0000 7328  _conditionC...s(
-000005b0: 0000 0002 0202 0102 0102 0102 0102 0102  ................
-000005c0: 0102 0102 0102 0102 0102 0106 f40c 0f0c  ................
-000005d0: 0108 0118 020e 0204 020a 0272 2500 0000  ...........r%...
-000005e0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000005f0: 0005 0000 0043 0000 0073 7400 0000 7400  .....C...st...t.
-00000600: 7c00 8301 6401 1800 7d01 7c01 6402 6b04  |...d...}.|.d.k.
-00000610: 7238 7401 7c00 8301 4400 5d29 7d02 7c02  r8t.|...D.])}.|.
-00000620: 6403 6b02 7219 7c01 6401 1800 7d01 710e  d.k.r.|.d...}.q.
-00000630: 7c02 7400 7c02 8301 6404 1800 6400 8502  |.t.|...d...d...
-00000640: 1900 6405 6b02 7235 7c02 6400 7400 7c02  ..d.k.r5|.d.t.|.
-00000650: 8301 6404 1800 8502 1900 7c00 7c01 3c00  ..d.......|.|.<.
-00000660: 7c00 0200 0100 5300 0100 7c00 5300 7c00  |.....S...|.S.|.
-00000670: 5300 2906 4ee9 0100 0000 7201 0000 0072  S.).N.....r....r
-00000680: 2200 0000 e902 0000 00fa 022c 2029 02da  ".........., )..
-00000690: 036c 656e da08 7265 7665 7273 6564 2903  .len..reversed).
-000006a0: da0d 6d61 7463 685f 7265 7375 6c74 735a  ..match_resultsZ
-000006b0: 106c 6173 745f 7661 6c69 645f 656e 7472  .last_valid_entr
-000006c0: 79da 0469 7465 6d72 0600 0000 7206 0000  y..itemr....r...
-000006d0: 0072 0a00 0000 da13 6472 6f70 5f74 7261  .r......drop_tra
-000006e0: 696c 696e 675f 636f 6d6d 6163 0000 0073  iling_commac...s
-000006f0: 1400 0000 0c01 0801 0c01 0801 0a01 1801  ................
-00000700: 1801 0801 0202 0801 722d 0000 0063 0000  ........r-...c..
-00000710: 0000 0000 0000 0000 0000 0300 0000 0600  ................
-00000720: 0000 4700 0000 736c 0000 0067 007d 017c  ..G...sl...g.}.|
-00000730: 0044 005d 2f7d 027c 0264 0119 0072 1c7c  .D.]/}.|.d...r.|
-00000740: 0264 0219 0064 036b 0372 1c7c 01a0 007c  .d...d.k.r.|...|
-00000750: 0264 0419 007c 0264 0219 0017 00a1 0101  .d...|.d........
-00000760: 0071 047c 0264 0119 0073 267c 0264 0219  .q.|.d...s&|.d..
-00000770: 0064 056b 0372 2c7c 01a0 0064 03a1 0101  .d.k.r,|...d....
-00000780: 0071 047c 01a0 007c 0264 0419 00a1 0101  .q.|...|.d......
-00000790: 0071 047c 0153 0029 064e 7201 0000 0072  .q.|.S.).Nr....r
-000007a0: 2600 0000 7222 0000 0072 2700 0000 7217  &...r"...r'...r.
-000007b0: 0000 0029 0172 0f00 0000 2903 da04 6172  ...).r....)...ar
-000007c0: 6773 da07 7265 7375 6c74 7372 2c00 0000  gs..resultsr,...
-000007d0: 7206 0000 0072 0600 0000 720a 0000 00da  r....r....r.....
-000007e0: 1765 7661 6c75 6174 655f 6163 7469 6f6e  .evaluate_action
-000007f0: 5f73 6574 7469 6e67 7900 0000 7310 0000  _settingy...s...
-00000800: 0004 0108 0214 0118 0114 010c 0110 0204  ................
-00000810: 0172 3000 0000 6305 0000 0000 0000 0000  .r0...c.........
-00000820: 0000 000f 0000 0004 0000 0043 0000 0073  ...........C...s
-00000830: a601 0000 6401 6402 6c00 6d01 7d05 0100  ....d.d.l.m.}...
-00000840: 7c00 7c01 1900 7d06 7c06 6401 1900 7d07  |.|...}.|.d...}.
-00000850: 6401 7d08 6403 7d09 7c09 72d1 7c08 6404  d.}.d.}.|.r.|.d.
-00000860: 1700 7402 7c06 8301 1600 7d08 7c06 7c08  ..t.|.....}.|.|.
-00000870: 1900 7d0a 7c0a a003 a100 724a 7c08 6404  ..}.|.....rJ|.d.
+00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6406 6407 8400 5a09 6408  m.Z...d.d...Z.d.
+00000070: 6409 8400 5a0a 640a 640b 8400 5a0b 640c  d...Z.d.d...Z.d.
+00000080: 640d 8400 5a0c 640e 640f 8400 5a0d 6410  d...Z.d.d...Z.d.
+00000090: 6411 8400 5a0e 6412 6413 8400 5a0f 6414  d...Z.d.d...Z.d.
+000000a0: 6415 8400 5a10 6416 6417 8400 5a11 6418  d...Z.d.d...Z.d.
+000000b0: 6419 8400 5a12 6401 5300 291a e900 0000  d...Z.d.S.).....
+000000c0: 004e 2901 da0a 7368 656c 6c5f 736f 7274  .N)...shell_sort
+000000d0: 2901 da0b 666f 726d 6174 5f68 746d 6c29  )...format_html)
+000000e0: 01da 1072 656d 6f76 655f 6874 6d6c 5f74  ...remove_html_t
+000000f0: 6167 7329 01da 066c 6f67 6765 7263 0200  ags)...loggerc..
+00000100: 0000 0000 0000 0000 0000 0800 0000 0600  ................
+00000110: 0000 4300 0000 739e 0000 0067 0067 0067  ..C...s....g.g.g
+00000120: 0003 0302 037d 027d 037d 0464 017d 057c  .....}.}.}.d.}.|
+00000130: 0044 005d 187d 067c 066a 007c 0176 0072  .D.].}.|.j.|.v.r
+00000140: 1471 0c7c 066a 01a0 0264 02a1 017d 077c  .q.|.j...d...}.|
+00000150: 0764 0075 0072 1f71 0c7c 04a0 037c 06a1  .d.u.r.q.|...|..
+00000160: 0101 0071 0c7c 0472 4a74 047c 0464 0364  ...q.|.rJt.|.d.d
+00000170: 0483 0301 007c 0444 005d 117d 067c 03a0  .....|.D.].}.|..
+00000180: 037c 066a 00a1 0101 007c 02a0 037c 066a  .|.j.....|...|.j
+00000190: 01a0 0264 02a1 01a1 0101 0071 2f64 0564  ...d.......q/d.d
+000001a0: 0684 0074 057c 0283 0144 0083 017d 057c  ...t.|...D...}.|
+000001b0: 027c 037c 0566 0353 0029 074e 7201 0000  .|.|.f.S.).Nr...
+000001c0: 00da 0273 7254 4663 0100 0000 0000 0000  ...srTFc........
+000001d0: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
+000001e0: 7318 0000 0067 007c 005d 085c 027d 017d  s....g.|.].\.}.}
+000001f0: 0274 007c 0183 0191 0271 0253 00a9 0029  .t.|.....q.S...)
+00000200: 01da 0373 7472 2903 da02 2e30 5a03 696e  ...str)....0Z.in
+00000210: 64da 0178 7207 0000 0072 0700 0000 fa75  d..xr....r.....u
+00000220: 2f55 7365 7273 2f6d 696b 7275 6269 6e2f  /Users/mikrubin/
+00000230: 4c69 6272 6172 792f 436c 6f75 6453 746f  Library/CloudSto
+00000240: 7261 6765 2f47 6f6f 676c 6544 7269 7665  rage/GoogleDrive
+00000250: 2d6d 696b 7275 6269 6e40 676d 6169 6c2e  -mikrubin@gmail.
+00000260: 636f 6d2f 4d79 2044 7269 7665 2f50 7974  com/My Drive/Pyt
+00000270: 686f 6e2f 6d61 7074 6173 6b65 722f 6d61  hon/maptasker/ma
+00000280: 7074 6173 6b65 722f 7372 632f 6163 7469  ptasker/src/acti
+00000290: 6f6e 2e70 79da 0a3c 6c69 7374 636f 6d70  on.py..<listcomp
+000002a0: 3e35 0000 0073 0600 0000 0600 0c01 06ff  >5...s..........
+000002b0: 7a1c 6765 745f 6172 6773 2e3c 6c6f 6361  z.get_args.<loca
+000002c0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2906  ls>.<listcomp>).
+000002d0: da03 7461 67da 0661 7474 7269 62da 0367  ..tag..attrib..g
+000002e0: 6574 da06 6170 7065 6e64 7202 0000 00da  et..appendr.....
+000002f0: 0965 6e75 6d65 7261 7465 2908 da06 6163  .enumerate)...ac
+00000300: 7469 6f6e 5a0b 6967 6e6f 7265 5f6c 6973  tionZ.ignore_lis
+00000310: 74da 0861 7267 5f6c 6973 745a 0974 7970  t..arg_listZ.typ
+00000320: 655f 6c69 7374 5a0b 6d61 7374 6572 5f6c  e_listZ.master_l
+00000330: 6973 745a 0861 7267 5f6e 756d 73da 0563  istZ.arg_nums..c
+00000340: 6869 6c64 5a0a 6163 7469 6f6e 5f61 7267  hildZ.action_arg
+00000350: 7207 0000 0072 0700 0000 720b 0000 00da  r....r....r.....
+00000360: 0867 6574 5f61 7267 7321 0000 0073 2400  .get_args!...s$.
+00000370: 0000 1001 0401 0801 0a01 0201 0c01 0801  ................
+00000380: 0201 0c02 0402 0c02 0802 0c01 1401 0602  ................
+00000390: 0601 06ff 0a04 7215 0000 0063 0300 0000  ......r....c....
+000003a0: 0000 0000 0000 0000 0300 0000 0200 0000  ................
+000003b0: 4300 0000 7310 0000 007c 0064 016b 0272  C...s....|.d.k.r
+000003c0: 067c 0153 007c 0253 0029 024e da01 3072  .|.S.|.S.).N..0r
+000003d0: 0700 0000 2903 5a09 7468 655f 7661 6c75  ....).Z.the_valu
+000003e0: 655a 0e69 665f 7a65 726f 5f73 7472 696e  eZ.if_zero_strin
+000003f0: 675a 1269 665f 6e6f 745f 7a65 726f 5f73  gZ.if_not_zero_s
+00000400: 7472 696e 6772 0700 0000 7207 0000 0072  tringr....r....r
+00000410: 0b00 0000 da0c 6966 5f7a 6572 6f5f 656c  ......if_zero_el
+00000420: 7365 3f00 0000 7302 0000 0010 0172 1700  se?...s......r..
+00000430: 0000 6301 0000 0000 0000 0000 0000 0006  ..c.............
+00000440: 0000 000d 0000 0043 0000 0073 7200 0000  .......C...sr...
+00000450: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
+00000460: 6401 6409 640a 640b 640c 9c0c 7d01 7c00  d.d.d.d.d...}.|.
+00000470: a000 640d a101 6a01 7d02 7c00 a000 640e  ..d...j.}.|...d.
+00000480: a101 6a01 7d03 7c01 7c03 1900 7d04 640f  ..j.}.|.|...}.d.
+00000490: 7c04 7601 7232 7c00 a000 6410 a101 6a01  |.v.r2|...d...j.
+000004a0: 6400 7501 7232 7c00 a000 6410 a101 6a01  d.u.r2|...d...j.
+000004b0: 7d05 6e02 6411 7d05 7c02 7c04 7c05 6603  }.n.d.}.|.|.|.f.
+000004c0: 5300 2912 4e7a 0320 3d20 7a05 204e 4551  S.).Nz. = z. NEQ
+000004d0: 207a 0320 7e20 7a04 2021 7e20 7a05 2021   z. ~ z. !~ z. !
+000004e0: 7e52 207a 0420 7e52 207a 0320 3c20 7a03  ~R z. ~R z. < z.
+000004f0: 203e 207a 0420 213d 207a 0720 6973 2073   > z. != z. is s
+00000500: 6574 7a08 206e 6f74 2073 6574 290c 7216  etz. not set).r.
+00000510: 0000 00da 0131 da01 32da 0133 da01 34da  .....1..2..3..4.
+00000520: 0135 da01 36da 0137 da01 38da 0139 5a02  .5..6..7..8..9Z.
+00000530: 3132 5a02 3133 5a03 6c68 73da 026f 70da  12Z.13Z.lhs..op.
+00000540: 0373 6574 5a03 7268 73da 0029 02da 0466  .setZ.rhs..)...f
+00000550: 696e 64da 0474 6578 7429 0672 1400 0000  ind..text).r....
+00000560: 5a0e 7468 655f 6f70 6572 6174 696f 6e73  Z.the_operations
+00000570: 5a0c 6669 7273 745f 7374 7269 6e67 5a09  Z.first_stringZ.
+00000580: 6f70 6572 6174 696f 6e5a 0d74 6865 5f6f  operationZ.the_o
+00000590: 7065 7261 7469 6f6e 5a0d 7365 636f 6e64  perationZ.second
+000005a0: 5f73 7472 696e 6772 0700 0000 7207 0000  _stringr....r...
+000005b0: 0072 0b00 0000 da12 6576 616c 7561 7465  .r......evaluate
+000005c0: 5f63 6f6e 6469 7469 6f6e 4600 0000 7328  _conditionF...s(
+000005d0: 0000 0002 0202 0102 0102 0102 0102 0102  ................
+000005e0: 0102 0102 0102 0102 0102 0106 f40c 0f0c  ................
+000005f0: 0108 0118 020e 0204 020a 0272 2600 0000  ...........r&...
+00000600: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000610: 0005 0000 0043 0000 0073 7400 0000 7400  .....C...st...t.
+00000620: 7c00 8301 6401 1800 7d01 7c01 6402 6b04  |...d...}.|.d.k.
+00000630: 7238 7401 7c00 8301 4400 5d29 7d02 7c02  r8t.|...D.])}.|.
+00000640: 6403 6b02 7219 7c01 6401 1800 7d01 710e  d.k.r.|.d...}.q.
+00000650: 7c02 7400 7c02 8301 6404 1800 6400 8502  |.t.|...d...d...
+00000660: 1900 6405 6b02 7235 7c02 6400 7400 7c02  ..d.k.r5|.d.t.|.
+00000670: 8301 6404 1800 8502 1900 7c00 7c01 3c00  ..d.......|.|.<.
+00000680: 7c00 0200 0100 5300 0100 7c00 5300 7c00  |.....S...|.S.|.
+00000690: 5300 2906 4ee9 0100 0000 7201 0000 0072  S.).N.....r....r
+000006a0: 2300 0000 e902 0000 00fa 022c 2029 02da  #.........., )..
+000006b0: 036c 656e da08 7265 7665 7273 6564 2903  .len..reversed).
+000006c0: da0d 6d61 7463 685f 7265 7375 6c74 735a  ..match_resultsZ
+000006d0: 106c 6173 745f 7661 6c69 645f 656e 7472  .last_valid_entr
+000006e0: 79da 0469 7465 6d72 0700 0000 7207 0000  y..itemr....r...
+000006f0: 0072 0b00 0000 da13 6472 6f70 5f74 7261  .r......drop_tra
+00000700: 696c 696e 675f 636f 6d6d 6166 0000 0073  iling_commaf...s
+00000710: 1400 0000 0c01 0801 0c01 0801 0a01 1801  ................
+00000720: 1801 0801 0202 0801 722e 0000 0063 0000  ........r....c..
+00000730: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00000740: 0000 4700 0000 736c 0000 0067 007d 017c  ..G...sl...g.}.|
+00000750: 0044 005d 2f7d 027c 0264 0119 0072 1c7c  .D.]/}.|.d...r.|
+00000760: 0264 0219 0064 036b 0372 1c7c 01a0 007c  .d...d.k.r.|...|
+00000770: 0264 0419 007c 0264 0219 0017 00a1 0101  .d...|.d........
+00000780: 0071 047c 0264 0119 0073 267c 0264 0219  .q.|.d...s&|.d..
+00000790: 0064 056b 0372 2c7c 01a0 0064 03a1 0101  .d.k.r,|...d....
+000007a0: 0071 047c 01a0 007c 0264 0419 00a1 0101  .q.|...|.d......
+000007b0: 0071 047c 0153 0029 064e 7201 0000 0072  .q.|.S.).Nr....r
+000007c0: 2700 0000 7223 0000 0072 2800 0000 7218  '...r#...r(...r.
+000007d0: 0000 0029 0172 1000 0000 2903 da04 6172  ...).r....)...ar
+000007e0: 6773 da07 7265 7375 6c74 7372 2d00 0000  gs..resultsr-...
+000007f0: 7207 0000 0072 0700 0000 720b 0000 00da  r....r....r.....
+00000800: 1765 7661 6c75 6174 655f 6163 7469 6f6e  .evaluate_action
+00000810: 5f73 6574 7469 6e67 7c00 0000 7310 0000  _setting|...s...
+00000820: 0004 0108 0214 0118 0114 010c 0110 0204  ................
+00000830: 0172 3100 0000 6305 0000 0000 0000 0000  .r1...c.........
+00000840: 0000 000f 0000 0004 0000 0043 0000 0073  ...........C...s
+00000850: a601 0000 6401 6402 6c00 6d01 7d05 0100  ....d.d.l.m.}...
+00000860: 7c00 7c01 1900 7d06 7c06 6401 1900 7d07  |.|...}.|.d...}.
+00000870: 6401 7d08 6403 7d09 7c09 72d1 7c08 6404  d.}.d.}.|.r.|.d.
 00000880: 1700 7402 7c06 8301 1600 7d08 7c06 7c08  ..t.|.....}.|.|.
-00000890: 1900 7d0b 7c0a 7c02 6b02 7240 7c03 a004  ..}.|.|.k.r@|...
-000008a0: 7c07 7c0b 1700 6405 1700 a101 0100 0900  |.|...d.........
-000008b0: 6400 5300 7c08 7402 7c06 8301 6b04 7249  d.S.|.t.|...k.rI
-000008c0: 0900 6400 5300 6e85 7c0a 6406 7600 7270  ..d.S.n.|.d.v.rp
-000008d0: 7c08 6404 1700 7402 7c06 8301 1600 7d08  |.d...t.|.....}.
-000008e0: 7c06 7c08 1900 7d0b 7405 6407 7c02 7c0b  |.|...}.t.d.|.|.
-000008f0: 6703 8301 7d0c 7c0c 6401 1900 9b00 6405  g...}.|.d.....d.
-00000900: 9d02 7d0c 7c03 a004 7c0c a101 0100 0900  ..}.|...|.......
-00000910: 6400 5300 7c0a 6408 6b02 72bc 7c08 6404  d.S.|.d.k.r.|.d.
-00000920: 1700 7402 7c06 8301 1600 7d08 7c06 7c08  ..t.|.....}.|.|.
-00000930: 1900 7c05 7600 72a1 7c05 7c06 7c08 1900  ..|.v.r.|.|.|...
-00000940: 1900 7406 7c02 8301 1900 6701 7d0c 7c06  ..t.|.....g.}.|.
-00000950: 7c08 6409 1800 1900 7c0c 6401 1900 1700  |.d.....|.d.....
-00000960: 6405 1700 7d0c 7c03 a004 7c0c a101 0100  d...}.|...|.....
-00000970: 0900 6400 5300 640a 7c06 7c08 1900 9b00  ..d.S.d.|.|.....
-00000980: 640b 7c00 9b00 9d04 7d0d 7407 a008 7c0d  d.|.....}.t...|.
-00000990: a101 0100 7409 7c0d 8301 0100 740a a00b  ....t.|.....t...
-000009a0: 6404 a101 0100 0900 6400 5300 640c 7c0a  d.......d.S.d.|.
-000009b0: 9b00 640d 7c04 9b00 9d04 7c00 6602 7d0e  ..d.|.....|.f.}.
-000009c0: 7407 a008 7c0e a101 0100 740b 640e 8301  t...|.....t.d...
-000009d0: 0100 7c09 7314 6400 5300 290f 4e72 0100  ..|.s.d.S.).Nr..
-000009e0: 0000 2901 da0d 6c6f 6f6b 7570 5f76 616c  ..)...lookup_val
-000009f0: 7565 7354 7226 0000 0072 2800 0000 2902  uesTr&...r(...).
-00000a00: da01 65da 0269 6646 da01 6c72 2700 0000  ..e..ifF..lr'...
-00000a10: 7a0f 5072 6f67 7261 6d20 6572 726f 723a  z.Program error:
-00000a20: 207a 2b20 6973 206e 6f74 2069 6e20 6163   z+ is not in ac
-00000a30: 7469 6f6e 7420 286c 6f6f 6b75 7020 7461  tiont (lookup ta
-00000a40: 626c 6529 2066 6f72 206e 616d 653a 7a33  ble) for name:z3
-00000a50: 6765 745f 786d 6c5f 696e 745f 6172 6775  get_xml_int_argu
-00000a60: 6d65 6e74 5f74 6f5f 7661 6c75 6520 6661  ment_to_value fa
-00000a70: 696c 6564 2d20 7468 6973 5f65 6c65 6d65  iled- this_eleme
-00000a80: 6e74 3afa 0120 e908 0000 0029 0c5a 156d  nt:.. .....).Z.m
-00000a90: 6170 7461 736b 6572 2e73 7263 2e61 6374  aptasker.src.act
-00000aa0: 696f 6e74 7231 0000 0072 2900 0000 da07  iontr1...r).....
-00000ab0: 6973 6469 6769 7472 0f00 0000 7230 0000  isdigitr....r0..
-00000ac0: 00da 0369 6e74 7203 0000 00da 0564 6562  ...intr......deb
-00000ad0: 7567 da05 7072 696e 74da 0373 7973 da04  ug..print..sys..
-00000ae0: 6578 6974 290f da05 6e61 6d65 735a 0c61  exit)...namesZ.a
-00000af0: 7267 5f6c 6f63 6174 696f 6e5a 0d74 6865  rg_locationZ.the
-00000b00: 5f69 6e74 5f76 616c 7565 722b 0000 00da  _int_valuer+....
-00000b10: 0961 7267 756d 656e 7473 7231 0000 005a  .argumentsr1...Z
-00000b20: 0874 6865 5f6c 6973 745a 0974 6865 5f74  .the_listZ.the_t
-00000b30: 6974 6c65 da03 6964 78da 0772 756e 6e69  itle..idx..runni
-00000b40: 6e67 5a0c 7468 6973 5f65 6c65 6d65 6e74  ngZ.this_element
-00000b50: 5a0c 6e65 7874 5f65 6c65 6d65 6e74 5a0f  Z.next_elementZ.
-00000b60: 6576 616c 7561 7465 645f 7661 6c75 65da  evaluated_value.
-00000b70: 0965 7272 6f72 5f6d 7367 da03 6d73 6772  .error_msg..msgr
-00000b80: 0600 0000 7206 0000 0072 0a00 0000 da10  ....r....r......
-00000b90: 7072 6f63 6573 735f 786d 6c5f 6c69 7374  process_xml_list
-00000ba0: 8e00 0000 7372 0000 000c 0208 0208 0104  ....sr..........
-00000bb0: 0104 0104 0310 0108 0108 0110 0208 0108  ................
-00000bc0: 0112 0102 0104 270c db02 0104 2402 db08  ......'.....$...
-00000bd0: 0210 0108 0102 0108 0104 ff0e 030a 0102  ................
-00000be0: 0104 1b08 e610 010c 0216 0118 010a 0102  ................
-00000bf0: 0904 0b0c ef02 0104 ff02 ff0a 0408 010a  ................
-00000c00: 0102 0104 0b02 f902 0104 ff02 0104 ff02  ................
-00000c10: 0304 fb0a 0708 0104 d104 3072 4300 0000  ..........0rC...
-00000c20: 6302 0000 0000 0000 0000 0000 000f 0000  c...............
-00000c30: 000b 0000 0043 0000 0073 3a01 0000 6401  .....C...s:...d.
-00000c40: 7c01 6402 1900 1700 7400 1700 6403 1700  |.d.....t...d...
-00000c50: 7d02 6404 7d03 6404 7d04 7c00 a001 6405  }.d.}.d.}.|...d.
-00000c60: a101 6a02 7d05 7c00 a001 6406 a101 6400  ..j.}.|...d...d.
-00000c70: 7501 722a 7c00 a001 6406 a101 6a02 7d06  u.r*|...d...j.}.
-00000c80: 7c06 6407 7601 722a 7403 7c06 7c01 8302  |.d.v.r*t.|.|...
-00000c90: 7d03 7c00 a001 6408 a101 6400 7501 7233  }.|...d...d.u.r3
-00000ca0: 7c02 6e01 6404 7d07 7c00 a001 6409 a101  |.n.d.}.|...d...
-00000cb0: 6400 7501 7297 640a 7d08 6404 7d09 6700  d.u.r.d.}.d.}.g.
-00000cc0: 7d0a 7c00 a001 6409 a101 4400 5d45 7d0b  }.|...d...D.]E}.
-00000cd0: 640b 7c0b 6a04 7600 7255 7c0a a005 7c0b  d.|.j.v.rU|...|.
-00000ce0: 6a02 a101 0100 7147 7c0b 6a04 640c 6b02  j.....qG|.j.d.k.
-00000cf0: 728c 7c05 640d 6b03 728c 7406 7c0b 8301  r.|.d.k.r.t.|...
-00000d00: 5c03 7d0c 7d0d 7d0e 7c08 640a 6b03 7274  \.}.}.}.|.d.k.rt
-00000d10: 7c0a 7c08 640e 1800 1900 a007 a100 9b00  |.|.d...........
-00000d20: 640f 9d02 7d09 7c04 9b00 6410 7c01 6411  d...}.|...d.|.d.
-00000d30: 1900 9b00 6412 7c09 9b00 6413 7c0c 9b00  ....d.|...d.|...
-00000d40: 7c0d 9b00 7c0e 9b00 6414 9d0a 7d04 7c08  |...|...d...}.|.
-00000d50: 640e 3700 7d08 7147 7c05 6415 6b02 7297  d.7.}.qG|.d.k.r.
-00000d60: 7c04 a008 6416 6417 a102 7d04 7c04 7c07  |...d.d...}.|.|.
-00000d70: 1700 7c03 1700 5300 2918 4e7a 1b20 3c2f  ..|...S.).Nz. </
-00000d80: 7370 616e 3e3c 7370 616e 2073 7479 6c65  span><span style
-00000d90: 3d22 636f 6c6f 723a 5a15 6469 7361 626c  ="color:Z.disabl
-00000da0: 6564 5f61 6374 696f 6e5f 636f 6c6f 727a  ed_action_colorz
-00000db0: 123e 5b44 4953 4142 4c45 445d 3c2f 7370  .>[DISABLED]</sp
-00000dc0: 616e 3e72 2200 0000 da04 636f 6465 da05  an>r".....code..
-00000dd0: 6c61 6265 6c29 0272 2200 0000 da01 0a5a  label).r"......Z
-00000de0: 026f 6eda 0d43 6f6e 6469 7469 6f6e 4c69  .on..ConditionLi
-00000df0: 7374 7201 0000 00da 0462 6f6f 6cda 0943  str......bool..C
-00000e00: 6f6e 6469 7469 6f6e 5a02 3337 7226 0000  onditionZ.37r&..
-00000e10: 0072 3500 0000 7a15 203c 7370 616e 2073  .r5...z. <span s
-00000e20: 7479 6c65 3d20 2263 6f6c 6f72 3a5a 1661  tyle= "color:Z.a
-00000e30: 6374 696f 6e5f 636f 6e64 6974 696f 6e5f  ction_condition_
-00000e40: 636f 6c6f 727a 0b22 3e3c 2f73 7061 6e3e  colorz."></span>
-00000e50: 2028 7a0f 636f 6e64 6974 696f 6e3a 2020   (z.condition:  
-00000e60: 4966 20fa 0129 5a02 3335 7a0e 636f 6e64  If ..)Z.35z.cond
-00000e70: 6974 696f 6e3a 2020 4966 7a0e 3c65 6d3e  ition:  Ifz.<em>
-00000e80: 554e 5449 4c3c 2f65 6d3e 2909 7204 0000  UNTIL</em>).r...
-00000e90: 0072 2300 0000 7224 0000 00da 0b63 6c65  .r#...r$.....cle
-00000ea0: 616e 5f6c 6162 656c 720c 0000 0072 0f00  an_labelr....r..
-00000eb0: 0000 7225 0000 00da 0575 7070 6572 da07  ..r%.....upper..
-00000ec0: 7265 706c 6163 6529 0f72 1300 0000 da08  replace).r......
-00000ed0: 636f 6c6f 726d 6170 5a14 6469 7361 626c  colormapZ.disabl
-00000ee0: 6564 5f61 6374 696f 6e5f 6874 6d6c 5a0a  ed_action_htmlZ.
-00000ef0: 7461 736b 5f6c 6162 656c 5a0f 7461 736b  task_labelZ.task
-00000f00: 5f63 6f6e 6469 7469 6f6e 735a 0f74 6865  _conditionsZ.the
-00000f10: 5f61 6374 696f 6e5f 636f 6465 da03 6c62  _action_code..lb
-00000f20: 6c5a 0f61 6374 696f 6e5f 6469 7361 626c  lZ.action_disabl
-00000f30: 6564 5a0f 636f 6e64 6974 696f 6e5f 636f  edZ.condition_co
-00000f40: 756e 745a 1162 6f6f 6c65 616e 5f74 6f5f  untZ.boolean_to_
-00000f50: 696e 6a65 6374 5a08 626f 6f6c 6561 6e73  injectZ.booleans
-00000f60: da08 6368 696c 6472 656e 5a07 7374 7269  ..childrenZ.stri
-00000f70: 6e67 31da 086f 7065 7261 746f 725a 0773  ng1..operatorZ.s
-00000f80: 7472 696e 6732 7206 0000 0072 0600 0000  tring2r....r....
-00000f90: 720a 0000 00da 1c67 6574 5f6c 6162 656c  r......get_label
-00000fa0: 5f64 6973 6162 6c65 645f 636f 6e64 6974  _disabled_condit
-00000fb0: 696f 6ece 0000 0073 5c00 0000 0202 0601  ion....s\.......
-00000fc0: 02ff 0202 02fe 0203 02fd 02ff 0407 0401  ................
-00000fd0: 0c01 0e01 0c01 0803 0a01 1602 0e01 0401  ................
-00000fe0: 0401 0401 0e01 0a01 0e01 1201 0e01 0801  ................
-00000ff0: 1601 0602 0601 04ff 0202 04fe 0202 02fe  ................
-00001000: 0202 02fe 0202 06fe 02ff 0805 0280 0801  ................
-00001010: 0401 0401 04ff 0c04 7252 0000 0063 0200  ........rR...c..
-00001020: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-00001030: 0000 4300 0000 737e 0000 007c 00a0 0064  ..C...s~...|...d
-00001040: 0164 02a1 027d 007c 00a0 0064 0364 02a1  .d...}.|...d.d..
-00001050: 027d 007c 00a0 0064 0464 02a1 027d 007c  .}.|...d.d...}.|
-00001060: 00a0 0064 0564 03a1 027d 007c 00a0 0164  ...d.d...}.|...d
-00001070: 06a1 017d 027c 0264 076b 0472 347c 00a0  ...}.|.d.k.r4|..
-00001080: 0164 08a1 017d 037c 027c 036b 0472 347c  .d...}.|.|.k.r4|
-00001090: 009b 0064 097c 0164 0a19 009b 0064 0b9d  ...d.|.d.....d..
-000010a0: 047d 0064 0c7c 0164 0a19 009b 0064 0d7c  .}.d.|.d.....d.|
-000010b0: 009b 0064 0e9d 0553 0029 0f4e 7246 0000  ...d...S.).NrF..
-000010c0: 0072 2200 0000 fa07 3c2f 666f 6e74 3e7a  .r".....</font>z
-000010d0: 063c 2f62 6967 3e7a 0e3c 2f66 6f6e 743e  .</big>z.</font>
-000010e0: 3c2f 666f 6e74 3efa 053c 666f 6e74 7201  </font>..<fontr.
-000010f0: 0000 007a 052f 666f 6e74 7a13 3c73 7061  ...z./fontz.<spa
-00001100: 6e20 7374 796c 653d 2263 6f6c 6f72 3ada  n style="color:.
-00001110: 1261 6374 696f 6e5f 6c61 6265 6c5f 636f  .action_label_co
-00001120: 6c6f 72fa 0122 7a14 203c 7370 616e 2073  lor.."z. <span s
-00001130: 7479 6c65 3d22 636f 6c6f 723a 7a11 223e  tyle="color:z.">
-00001140: 2e2e 2e77 6974 6820 6c61 6265 6c3a 207a  ...with label: z
-00001150: 0b3c 2f73 7061 6e3e 3c2f 623e 2902 724d  .</span></b>).rM
-00001160: 0000 00da 0563 6f75 6e74 2904 724f 0000  .....count).rO..
-00001170: 0072 4e00 0000 5a0a 666f 6e74 5f63 6f75  .rN...Z.font_cou
-00001180: 6e74 5a0e 656e 645f 666f 6e74 5f63 6f75  ntZ.end_font_cou
-00001190: 6e74 7206 0000 0072 0600 0000 720a 0000  ntr....r....r...
-000011a0: 0072 4b00 0000 fd00 0000 731a 0000 000c  .rK.......s.....
-000011b0: 020c 010c 010c 010a 0108 020a 0208 0114  ................
-000011c0: 010c 0302 0106 ff02 ff72 4b00 0000 6304  .........rK...c.
-000011d0: 0000 0000 0000 0000 0000 0006 0000 0004  ................
-000011e0: 0000 0043 0000 0073 bc00 0000 7c01 722f  ...C...s....|.r/
-000011f0: 7400 7c00 7c02 8302 7d04 6401 7c04 7600  t.|.|...}.d.|.v.
-00001200: 7214 6402 7c04 7601 7214 7c04 9b00 6402  r.d.|.v.r.|...d.
-00001210: 9d02 7d04 6403 7c04 7600 7221 6404 7c04  ..}.d.|.v.r!d.|.
-00001220: 7601 7221 7c04 9b00 6402 9d02 7d04 6405  v.r!|...d...}.d.
-00001230: 7c04 7600 722e 6406 7c04 7601 722e 7c04  |.v.r.d.|.v.r.|.
-00001240: 9b00 6406 9d02 7d04 6e02 6407 7d04 7c03  ..d...}.n.d.}.|.
-00001250: 6408 1900 7249 7c01 7249 7c04 9b00 6409  d...rI|.rI|...d.
-00001260: 7c03 640a 1900 9b00 640b 9d04 7c00 a001  |.d.....d...|...
-00001270: 640c a101 6a02 1700 640d 1700 7d04 7c00  d...j...d...}.|.
-00001280: a001 640e a101 7d05 7c05 6400 7501 725c  ..d...}.|.d.u.r\
-00001290: 7c05 6a02 640f 6b02 725c 6410 7c04 9b00  |.j.d.k.r\d.|...
-000012a0: 9d02 7d04 7c04 5300 2911 4e72 5400 0000  ..}.|.S.).NrT...
-000012b0: 7253 0000 007a 0826 6c74 3b66 6f6e 747a  rS...z.&lt;fontz
-000012c0: 0d26 6c74 3b2f 666f 6e74 2667 743b 7a03  .&lt;/font&gt;z.
-000012d0: 3c62 3e7a 043c 2f62 3e72 2200 0000 7239  <b>z.</b>r"...r9
-000012e0: 0000 007a 1d3c 2f73 7061 6e3e 3c73 7061  ...z.</span><spa
-000012f0: 6e20 7374 796c 653d 2263 6f6c 6f72 3a52  n style="color:R
-00001300: 6564 da0b 666f 6e74 5f74 6f5f 7573 657a  ed..font_to_usez
-00001310: 123e 266e 6273 703b 266e 6273 703b 636f  .>&nbsp;&nbsp;co
-00001320: 6465 3a72 4400 0000 fa01 2d5a 0273 655a  de:rD.....-Z.seZ
-00001330: 0566 616c 7365 7a1c 205b 436f 6e74 696e  .falsez. [Contin
-00001340: 7565 2054 6173 6b20 4166 7465 7220 4572  ue Task After Er
-00001350: 726f 725d 2903 7252 0000 0072 2300 0000  ror]).rR...r#...
-00001360: 7224 0000 0029 06da 0b63 6f64 655f 6163  r$...)...code_ac
-00001370: 7469 6f6e da0b 6163 7469 6f6e 5f74 7970  tion..action_typ
-00001380: 6572 4e00 0000 da0c 7072 6f67 7261 6d5f  erN.....program_
-00001390: 6172 6773 da0b 6578 7472 615f 7374 7566  args..extra_stuf
-000013a0: 6672 1300 0000 7206 0000 0072 0600 0000  fr....r....r....
-000013b0: 720a 0000 00da 0f67 6574 5f65 7874 7261  r......get_extra
-000013c0: 5f73 7475 6666 1601 0000 733a 0000 0002  _stuff....s:....
-000013d0: 0202 ff02 0304 0104 ff10 040a 0210 020a  ................
-000013e0: 0210 020a 0202 8004 0206 0202 ff02 0102  ................
-000013f0: ff06 0406 0106 ff0a 0202 fe02 0302 fd02  ................
-00001400: ff0a 0812 010a 0104 0172 5e00 0000 6304  .........r^...c.
-00001410: 0000 0000 0000 0000 0000 0009 0000 0005  ................
-00001420: 0000 0043 0000 0073 ba00 0000 7400 7c00  ...C...s....t.|.
-00001430: 7c01 7c02 7c03 8304 7d04 6401 5c03 7d05  |.|.|...}.d.\.}.
-00001440: 7d06 7d07 7c00 a001 6402 a101 7d08 7c08  }.}.|...d...}.|.
-00001450: 6400 7501 7257 7c08 6a02 6402 6b02 7257  d.u.rW|.j.d.k.rW
-00001460: 7c08 a001 6403 a101 6400 7500 7227 6404  |...d...d.u.r'd.
-00001470: 6404 6404 7c04 6604 5300 7c08 a001 6403  d.d.|.f.S.|...d.
-00001480: a101 6a03 6400 7501 7237 6405 7c08 a001  ..j.d.u.r7d.|...
-00001490: 6403 a101 6a03 1700 7d05 7c08 a001 6406  d...j...}.|...d.
-000014a0: a101 6a03 6400 7501 7247 6407 7c08 a001  ..j.d.u.rGd.|...
-000014b0: 6406 a101 6a03 1700 7d06 7c08 a001 6408  d...j...}.|...d.
-000014c0: a101 6a03 6400 7501 7257 6409 7c08 a001  ..j.d.u.rWd.|...
-000014d0: 6408 a101 6a03 1700 7d07 7c05 7c06 7c07  d...j...}.|.|.|.
-000014e0: 7c04 6604 5300 290a 4e29 0372 2200 0000  |.f.S.).N).r"...
-000014f0: 7222 0000 0072 2200 0000 da03 4170 705a  r"...r".....AppZ
-00001500: 0861 7070 436c 6173 7372 2200 0000 7a06  .appClassr"...z.
-00001510: 436c 6173 733a 5a06 6170 7050 6b67 7a0a  Class:Z.appPkgz.
-00001520: 2c20 5061 636b 6167 653a 7245 0000 007a  , Package:rE...z
-00001530: 062c 2041 7070 3a29 0472 5e00 0000 7223  ., App:).r^...r#
-00001540: 0000 0072 0c00 0000 7224 0000 0029 09da  ...r....r$...)..
-00001550: 0a63 6f64 655f 6368 696c 6472 5b00 0000  .code_childr[...
-00001560: 724e 0000 0072 5c00 0000 725d 0000 005a  rN...r\...r]...Z
-00001570: 0961 7070 5f63 6c61 7373 5a07 6170 705f  .app_classZ.app_
-00001580: 706b 675a 0361 7070 7213 0000 0072 0600  pkgZ.appr....r..
-00001590: 0000 7206 0000 0072 0a00 0000 da0f 6765  ..r....r......ge
-000015a0: 745f 6170 705f 6465 7461 696c 733f 0100  t_app_details?..
-000015b0: 0073 1a00 0000 0e01 0a01 0a01 1201 0e01  .s..............
-000015c0: 0c01 1001 1001 1001 1001 1001 1001 0c01  ................
-000015d0: 7261 0000 0029 1072 3b00 0000 5a17 6d61  ra...).r;...Z.ma
-000015e0: 7074 6173 6b65 722e 7372 632e 7368 656c  ptasker.src.shel
-000015f0: 6c73 6f72 7472 0200 0000 da16 6d61 7074  lsortr......mapt
-00001600: 6173 6b65 722e 7372 632e 7379 7363 6f6e  asker.src.syscon
-00001610: 7374 7203 0000 0072 0400 0000 7214 0000  str....r....r...
-00001620: 0072 1600 0000 7225 0000 0072 2d00 0000  .r....r%...r-...
-00001630: 7230 0000 0072 4300 0000 7252 0000 0072  r0...rC...rR...r
-00001640: 4b00 0000 725e 0000 0072 6100 0000 7206  K...r^...ra...r.
-00001650: 0000 0072 0600 0000 7206 0000 0072 0a00  ...r....r....r..
-00001660: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001670: 731c 0000 0008 0d0c 020c 010c 0108 0e08  s...............
-00001680: 1c08 0708 2008 1608 1508 4008 2f08 190c  .... .....@./...
-00001690: 29                                       )
+00000890: 1900 7d0a 7c0a a003 a100 724a 7c08 6404  ..}.|.....rJ|.d.
+000008a0: 1700 7402 7c06 8301 1600 7d08 7c06 7c08  ..t.|.....}.|.|.
+000008b0: 1900 7d0b 7c0a 7c02 6b02 7240 7c03 a004  ..}.|.|.k.r@|...
+000008c0: 7c07 7c0b 1700 6405 1700 a101 0100 0900  |.|...d.........
+000008d0: 6400 5300 7c08 7402 7c06 8301 6b04 7249  d.S.|.t.|...k.rI
+000008e0: 0900 6400 5300 6e85 7c0a 6406 7600 7270  ..d.S.n.|.d.v.rp
+000008f0: 7c08 6404 1700 7402 7c06 8301 1600 7d08  |.d...t.|.....}.
+00000900: 7c06 7c08 1900 7d0b 7405 6407 7c02 7c0b  |.|...}.t.d.|.|.
+00000910: 6703 8301 7d0c 7c0c 6401 1900 9b00 6405  g...}.|.d.....d.
+00000920: 9d02 7d0c 7c03 a004 7c0c a101 0100 0900  ..}.|...|.......
+00000930: 6400 5300 7c0a 6408 6b02 72bc 7c08 6404  d.S.|.d.k.r.|.d.
+00000940: 1700 7402 7c06 8301 1600 7d08 7c06 7c08  ..t.|.....}.|.|.
+00000950: 1900 7c05 7600 72a1 7c05 7c06 7c08 1900  ..|.v.r.|.|.|...
+00000960: 1900 7406 7c02 8301 1900 6701 7d0c 7c06  ..t.|.....g.}.|.
+00000970: 7c08 6409 1800 1900 7c0c 6401 1900 1700  |.d.....|.d.....
+00000980: 6405 1700 7d0c 7c03 a004 7c0c a101 0100  d...}.|...|.....
+00000990: 0900 6400 5300 640a 7c06 7c08 1900 9b00  ..d.S.d.|.|.....
+000009a0: 640b 7c00 9b00 9d04 7d0d 7407 a008 7c0d  d.|.....}.t...|.
+000009b0: a101 0100 7409 7c0d 8301 0100 740a a00b  ....t.|.....t...
+000009c0: 6404 a101 0100 0900 6400 5300 640c 7c0a  d.......d.S.d.|.
+000009d0: 9b00 640d 7c04 9b00 9d04 7c00 6602 7d0e  ..d.|.....|.f.}.
+000009e0: 7407 a008 7c0e a101 0100 740b 640e 8301  t...|.....t.d...
+000009f0: 0100 7c09 7314 6400 5300 290f 4e72 0100  ..|.s.d.S.).Nr..
+00000a00: 0000 2901 da0d 6c6f 6f6b 7570 5f76 616c  ..)...lookup_val
+00000a10: 7565 7354 7227 0000 0072 2900 0000 2902  uesTr'...r)...).
+00000a20: da01 65da 0269 6646 da01 6c72 2800 0000  ..e..ifF..lr(...
+00000a30: 7a0f 5072 6f67 7261 6d20 6572 726f 723a  z.Program error:
+00000a40: 207a 2b20 6973 206e 6f74 2069 6e20 6163   z+ is not in ac
+00000a50: 7469 6f6e 7420 286c 6f6f 6b75 7020 7461  tiont (lookup ta
+00000a60: 626c 6529 2066 6f72 206e 616d 653a 7a33  ble) for name:z3
+00000a70: 6765 745f 786d 6c5f 696e 745f 6172 6775  get_xml_int_argu
+00000a80: 6d65 6e74 5f74 6f5f 7661 6c75 6520 6661  ment_to_value fa
+00000a90: 696c 6564 2d20 7468 6973 5f65 6c65 6d65  iled- this_eleme
+00000aa0: 6e74 3afa 0120 e908 0000 0029 0c5a 156d  nt:.. .....).Z.m
+00000ab0: 6170 7461 736b 6572 2e73 7263 2e61 6374  aptasker.src.act
+00000ac0: 696f 6e74 7232 0000 0072 2a00 0000 da07  iontr2...r*.....
+00000ad0: 6973 6469 6769 7472 1000 0000 7231 0000  isdigitr....r1..
+00000ae0: 00da 0369 6e74 7205 0000 00da 0564 6562  ...intr......deb
+00000af0: 7567 da05 7072 696e 74da 0373 7973 da04  ug..print..sys..
+00000b00: 6578 6974 290f da05 6e61 6d65 735a 0c61  exit)...namesZ.a
+00000b10: 7267 5f6c 6f63 6174 696f 6e5a 0d74 6865  rg_locationZ.the
+00000b20: 5f69 6e74 5f76 616c 7565 722c 0000 005a  _int_valuer,...Z
+00000b30: 0961 7267 756d 656e 7473 7232 0000 005a  .argumentsr2...Z
+00000b40: 0874 6865 5f6c 6973 745a 0974 6865 5f74  .the_listZ.the_t
+00000b50: 6974 6c65 da03 6964 785a 0772 756e 6e69  itle..idxZ.runni
+00000b60: 6e67 5a0c 7468 6973 5f65 6c65 6d65 6e74  ngZ.this_element
+00000b70: 5a0c 6e65 7874 5f65 6c65 6d65 6e74 5a0f  Z.next_elementZ.
+00000b80: 6576 616c 7561 7465 645f 7661 6c75 65da  evaluated_value.
+00000b90: 0965 7272 6f72 5f6d 7367 da03 6d73 6772  .error_msg..msgr
+00000ba0: 0700 0000 7207 0000 0072 0b00 0000 da10  ....r....r......
+00000bb0: 7072 6f63 6573 735f 786d 6c5f 6c69 7374  process_xml_list
+00000bc0: 9100 0000 7372 0000 000c 0208 0208 0104  ....sr..........
+00000bd0: 0104 0104 0310 0108 0108 0110 0208 0108  ................
+00000be0: 0112 0102 0104 270c db02 0104 2402 db08  ......'.....$...
+00000bf0: 0210 0108 0102 0108 0104 ff0e 030a 0102  ................
+00000c00: 0104 1b08 e610 010c 0216 0118 010a 0102  ................
+00000c10: 0904 0b0c ef02 0104 ff02 ff0a 0408 010a  ................
+00000c20: 0102 0104 0b02 f902 0104 ff02 0104 ff02  ................
+00000c30: 0304 fb0a 0708 0104 d104 3072 4200 0000  ..........0rB...
+00000c40: 6302 0000 0000 0000 0000 0000 000e 0000  c...............
+00000c50: 000c 0000 0043 0000 0073 2801 0000 6401  .....C...s(...d.
+00000c60: 7d02 6401 7d03 7c00 a000 6402 a101 6a01  }.d.}.|...d...j.
+00000c70: 7d04 7c00 a000 6403 a101 6400 7501 721c  }.|...d...d.u.r.
+00000c80: 7c00 a000 6403 a101 6a01 7d05 7402 7c05  |...d...j.}.t.|.
+00000c90: 7c01 8302 7d02 7c00 a000 6404 a101 6400  |...}.|...d...d.
+00000ca0: 7501 722b 7403 7c01 6405 6401 6406 6407  u.r+t.|.d.d.d.d.
+00000cb0: 8305 6e01 6401 7d06 7c00 a000 6408 a101  ..n.d.}.|...d...
+00000cc0: 6400 7501 728e 6409 7d07 6401 7d08 6700  d.u.r.d.}.d.}.g.
+00000cd0: 7d09 7c00 a000 6408 a101 4400 5d44 7d0a  }.|...d...D.]D}.
+00000ce0: 640a 7c0a 6a04 7600 724d 7c09 a005 7c0a  d.|.j.v.rM|...|.
+00000cf0: 6a01 a101 0100 713f 7c0a 6a04 640b 6b02  j.....q?|.j.d.k.
+00000d00: 7283 7c04 640c 6b03 7283 7406 7c0a 8301  r.|.d.k.r.t.|...
+00000d10: 5c03 7d0b 7d0c 7d0d 7c07 6409 6b03 726c  \.}.}.}.|.d.k.rl
+00000d20: 7c09 7c07 640d 1800 1900 a007 a100 9b00  |.|.d...........
+00000d30: 640e 9d02 7d08 7403 7c01 640f 6401 6410  d...}.t.|.d.d.d.
+00000d40: 7c08 9b00 6411 7c0b 9b00 7c0c 9b00 7c0d  |...d.|...|...|.
+00000d50: 9b00 6412 9d07 6407 8305 7d03 7c07 640d  ..d...d...}.|.d.
+00000d60: 3700 7d07 713f 7c04 6413 6b02 728e 7c03  7.}.q?|.d.k.r.|.
+00000d70: a008 6414 6415 a102 7d03 7c03 7c06 1700  ..d.d...}.|.|...
+00000d80: 7c02 1700 5300 2916 4e72 2300 0000 da04  |...S.).Nr#.....
+00000d90: 636f 6465 da05 6c61 6265 6c5a 026f 6e5a  code..labelZ.onZ
+00000da0: 1564 6973 6162 6c65 645f 6163 7469 6f6e  .disabled_action
+00000db0: 5f63 6f6c 6f72 7a0b 205b 4449 5341 424c  _colorz. [DISABL
+00000dc0: 4544 5d54 da0d 436f 6e64 6974 696f 6e4c  ED]T..ConditionL
+00000dd0: 6973 7472 0100 0000 da04 626f 6f6c da09  istr......bool..
+00000de0: 436f 6e64 6974 696f 6e5a 0233 3772 2700  ConditionZ.37r'.
+00000df0: 0000 7236 0000 005a 1661 6374 696f 6e5f  ..r6...Z.action_
+00000e00: 636f 6e64 6974 696f 6e5f 636f 6c6f 727a  condition_colorz
+00000e10: 0220 287a 0f63 6f6e 6469 7469 6f6e 3a20  . (z.condition: 
+00000e20: 2049 6620 fa01 295a 0233 357a 0e63 6f6e   If ..)Z.35z.con
+00000e30: 6469 7469 6f6e 3a20 2049 667a 0e3c 656d  dition:  Ifz.<em
+00000e40: 3e55 4e54 494c 3c2f 656d 3e29 0972 2400  >UNTIL</em>).r$.
+00000e50: 0000 7225 0000 00da 0b63 6c65 616e 5f6c  ..r%.....clean_l
+00000e60: 6162 656c 7203 0000 0072 0d00 0000 7210  abelr....r....r.
+00000e70: 0000 0072 2600 0000 da05 7570 7065 72da  ...r&.....upper.
+00000e80: 0772 6570 6c61 6365 290e 7214 0000 00da  .replace).r.....
+00000e90: 0863 6f6c 6f72 6d61 705a 0a74 6173 6b5f  .colormapZ.task_
+00000ea0: 6c61 6265 6c5a 0f74 6173 6b5f 636f 6e64  labelZ.task_cond
+00000eb0: 6974 696f 6e73 5a0f 7468 655f 6163 7469  itionsZ.the_acti
+00000ec0: 6f6e 5f63 6f64 65da 036c 626c 5a0f 6163  on_code..lblZ.ac
+00000ed0: 7469 6f6e 5f64 6973 6162 6c65 645a 0f63  tion_disabledZ.c
+00000ee0: 6f6e 6469 7469 6f6e 5f63 6f75 6e74 5a11  ondition_countZ.
+00000ef0: 626f 6f6c 6561 6e5f 746f 5f69 6e6a 6563  boolean_to_injec
+00000f00: 745a 0862 6f6f 6c65 616e 73da 0863 6869  tZ.booleans..chi
+00000f10: 6c64 7265 6e5a 0773 7472 696e 6731 da08  ldrenZ.string1..
+00000f20: 6f70 6572 6174 6f72 5a07 7374 7269 6e67  operatorZ.string
+00000f30: 3272 0700 0000 7207 0000 0072 0b00 0000  2r....r....r....
+00000f40: da1c 6765 745f 6c61 6265 6c5f 6469 7361  ..get_label_disa
+00000f50: 626c 6564 5f63 6f6e 6469 7469 6f6e d100  bled_condition..
+00000f60: 0000 7352 0000 0004 0104 010c 010e 010c  ..sR............
+00000f70: 010a 020e 0410 ff02 0202 fd0e 0504 0104  ................
+00000f80: 0104 010e 010a 010e 0112 010e 0108 0116  ................
+00000f90: 0102 0102 0102 0102 0108 0202 0102 ff02  ................
+00000fa0: 0102 ff02 0206 fe02 0404 f708 0b02 8008  ................
+00000fb0: 0104 0104 0104 ff0c 0472 5000 0000 6302  .........rP...c.
+00000fc0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00000fd0: 0000 0043 0000 0073 2000 0000 7400 7c00  ...C...s ...t.|.
+00000fe0: 6401 8302 7d00 7401 7c01 6402 6401 6403  d...}.t.|.d.d.d.
+00000ff0: 7c00 9b00 9d02 6404 8305 5300 2905 4e72  |.....d...S.).Nr
+00001000: 2300 0000 5a12 6163 7469 6f6e 5f6c 6162  #...Z.action_lab
+00001010: 656c 5f63 6f6c 6f72 7a10 202e 2e2e 7769  el_colorz. ...wi
+00001020: 7468 206c 6162 656c 3a20 5429 0272 0400  th label: T).r..
+00001030: 0000 7203 0000 0029 0272 4d00 0000 724c  ..r....).rM...rL
+00001040: 0000 0072 0700 0000 7207 0000 0072 0b00  ...r....r....r..
+00001050: 0000 7249 0000 0001 0100 0073 0800 0000  ..rI.......s....
+00001060: 0a02 0202 1001 04ff 7249 0000 0063 0400  ........rI...c..
+00001070: 0000 0000 0000 0000 0000 0600 0000 0800  ................
+00001080: 0000 4300 0000 73be 0000 007c 0172 2f74  ..C...s....|.r/t
+00001090: 007c 007c 0283 027d 0464 017c 0476 0072  .|.|...}.d.|.v.r
+000010a0: 1464 027c 0476 0172 147c 049b 0064 029d  .d.|.v.r.|...d..
+000010b0: 027d 0464 037c 0476 0072 2164 047c 0476  .}.d.|.v.r!d.|.v
+000010c0: 0172 217c 049b 0064 029d 027d 0464 057c  .r!|...d...}.d.|
+000010d0: 0476 0072 2e64 067c 0476 0172 2e7c 049b  .v.r.d.|.v.r.|..
+000010e0: 0064 069d 027d 046e 0264 077d 047c 0364  .d...}.n.d.}.|.d
+000010f0: 0819 0072 477c 0172 4774 017c 0264 0964  ...rG|.rGt.|.d.d
+00001100: 0764 0a7c 00a0 0264 0ba1 016a 039b 0064  .d.|...d...j...d
+00001110: 0c9d 0364 0d83 057d 047c 00a0 0264 0ea1  ...d...}.|...d..
+00001120: 017d 057c 0564 0075 0172 5a7c 056a 0364  .}.|.d.u.rZ|.j.d
+00001130: 0f6b 0272 5a64 107c 049b 009d 027d 047c  .k.rZd.|.....}.|
+00001140: 049b 0064 119d 0253 0029 124e 7a05 3c66  ...d...S.).Nz.<f
+00001150: 6f6e 747a 073c 2f66 6f6e 743e 7a08 266c  ontz.</font>z.&l
+00001160: 743b 666f 6e74 7a0d 266c 743b 2f66 6f6e  t;fontz.&lt;/fon
+00001170: 7426 6774 3b7a 033c 623e 7a04 3c2f 623e  t&gt;z.<b>z.</b>
+00001180: 7223 0000 0072 3a00 0000 5a06 5965 6c6c  r#...r:...Z.Yell
+00001190: 6f77 7a12 266e 6273 703b 266e 6273 703b  owz.&nbsp;&nbsp;
+000011a0: 636f 6465 3a20 7243 0000 00fa 012d 465a  code: rC.....-FZ
+000011b0: 0273 655a 0566 616c 7365 7a1c 205b 436f  .seZ.falsez. [Co
+000011c0: 6e74 696e 7565 2054 6173 6b20 4166 7465  ntinue Task Afte
+000011d0: 7220 4572 726f 725d 7a07 3c2f 7370 616e  r Error]z.</span
+000011e0: 3e29 0472 5000 0000 7203 0000 0072 2400  >).rP...r....r$.
+000011f0: 0000 7225 0000 0029 06da 0b63 6f64 655f  ..r%...)...code_
+00001200: 6163 7469 6f6e da0b 6163 7469 6f6e 5f74  action..action_t
+00001210: 7970 6572 4c00 0000 da0c 7072 6f67 7261  yperL.....progra
+00001220: 6d5f 6172 6773 da0b 6578 7472 615f 7374  m_args..extra_st
+00001230: 7566 6672 1400 0000 7207 0000 0072 0700  uffr....r....r..
+00001240: 0000 720b 0000 00da 0f67 6574 5f65 7874  ..r......get_ext
+00001250: 7261 5f73 7475 6666 0f01 0000 7336 0000  ra_stuff....s6..
+00001260: 0004 0202 0104 0104 ff10 040a 0210 020a  ................
+00001270: 0210 020a 0202 8004 0206 0202 ff02 0102  ................
+00001280: ff02 0302 0102 0102 0112 0102 0104 fb0a  ................
+00001290: 0912 010a 010a 0172 5600 0000 6304 0000  .......rV...c...
+000012a0: 0000 0000 0000 0000 0009 0000 0005 0000  ................
+000012b0: 0043 0000 0073 ba00 0000 7400 7c00 7c01  .C...s....t.|.|.
+000012c0: 7c02 7c03 8304 7d04 6401 5c03 7d05 7d06  |.|...}.d.\.}.}.
+000012d0: 7d07 7c00 a001 6402 a101 7d08 7c08 6400  }.|...d...}.|.d.
+000012e0: 7501 7257 7c08 6a02 6402 6b02 7257 7c08  u.rW|.j.d.k.rW|.
+000012f0: a001 6403 a101 6400 7500 7227 6404 6404  ..d...d.u.r'd.d.
+00001300: 6404 7c04 6604 5300 7c08 a001 6403 a101  d.|.f.S.|...d...
+00001310: 6a03 6400 7501 7237 6405 7c08 a001 6403  j.d.u.r7d.|...d.
+00001320: a101 6a03 1700 7d05 7c08 a001 6406 a101  ..j...}.|...d...
+00001330: 6a03 6400 7501 7247 6407 7c08 a001 6406  j.d.u.rGd.|...d.
+00001340: a101 6a03 1700 7d06 7c08 a001 6408 a101  ..j...}.|...d...
+00001350: 6a03 6400 7501 7257 6409 7c08 a001 6408  j.d.u.rWd.|...d.
+00001360: a101 6a03 1700 7d07 7c05 7c06 7c07 7c04  ..j...}.|.|.|.|.
+00001370: 6604 5300 290a 4e29 0372 2300 0000 7223  f.S.).N).r#...r#
+00001380: 0000 0072 2300 0000 da03 4170 705a 0861  ...r#.....AppZ.a
+00001390: 7070 436c 6173 7372 2300 0000 7a06 436c  ppClassr#...z.Cl
+000013a0: 6173 733a 5a06 6170 7050 6b67 7a0a 2c20  ass:Z.appPkgz., 
+000013b0: 5061 636b 6167 653a 7244 0000 007a 062c  Package:rD...z.,
+000013c0: 2041 7070 3a29 0472 5600 0000 7224 0000   App:).rV...r$..
+000013d0: 0072 0d00 0000 7225 0000 0029 09da 0a63  .r....r%...)...c
+000013e0: 6f64 655f 6368 696c 6472 5300 0000 724c  ode_childrS...rL
+000013f0: 0000 0072 5400 0000 7255 0000 005a 0961  ...rT...rU...Z.a
+00001400: 7070 5f63 6c61 7373 5a07 6170 705f 706b  pp_classZ.app_pk
+00001410: 675a 0361 7070 7214 0000 0072 0700 0000  gZ.appr....r....
+00001420: 7207 0000 0072 0b00 0000 da0f 6765 745f  r....r......get_
+00001430: 6170 705f 6465 7461 696c 7338 0100 0073  app_details8...s
+00001440: 1a00 0000 0e01 0a01 0a01 1201 0e01 0c01  ................
+00001450: 1001 1001 1001 1001 1001 1001 0c01 7259  ..............rY
+00001460: 0000 0029 1372 3c00 0000 5a17 6d61 7074  ...).r<...Z.mapt
+00001470: 6173 6b65 722e 7372 632e 7368 656c 6c73  asker.src.shells
+00001480: 6f72 7472 0200 0000 da16 6d61 7074 6173  ortr......maptas
+00001490: 6b65 722e 7372 632e 6672 6d74 6874 6d6c  ker.src.frmthtml
+000014a0: 7203 0000 00da 156d 6170 7461 736b 6572  r......maptasker
+000014b0: 2e73 7263 2e78 6d6c 6461 7461 7204 0000  .src.xmldatar...
+000014c0: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+000014d0: 2e73 7973 636f 6e73 7472 0500 0000 7215  .sysconstr....r.
+000014e0: 0000 0072 1700 0000 7226 0000 0072 2e00  ...r....r&...r..
+000014f0: 0000 7231 0000 0072 4200 0000 7250 0000  ..r1...rB...rP..
+00001500: 0072 4900 0000 7256 0000 0072 5900 0000  .rI...rV...rY...
+00001510: 7207 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
+00001520: 0b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00001530: 0000 731e 0000 0008 0d0c 020c 010c 010c  ..s.............
+00001540: 0108 0e08 1e08 0708 2008 1608 1508 4008  ........ .....@.
+00001550: 3008 0e0c 29                             0...)
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/actionc.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/actionc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/actiond.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/actiond.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 23 17:42:41 2023 UTC, .py size: 6713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,162 +1,161 @@
-00000000: 6f0d 0d0a 0000 0000 918f 1c64 391a 0000  o..........d9...
+00000000: 6f0d 0d0a 0000 0000 cee9 3264 621a 0000  o.........2db...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 2001 0000 6400  .....@...s ...d.
+00000020: 000a 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c04 6d05 0200 0100 6d06  ..d.d.l.m.....m.
 00000050: 5a07 0100 6400 6403 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6400 6404 6c0a 6d0b 5a0b 0100 6700 6405  d.d.l.m.Z...g.d.
-00000070: a201 5a0c 6406 6501 6a0d 6a0e 6602 6407  ..Z.d.e.j.j.f.d.
-00000080: 6408 8404 5a0f 6409 6501 6a0d 6a0e 640a  d...Z.d.e.j.j.d.
-00000090: 6501 6a0d 6a0e 6406 6501 6a0d 6a0e 6606  e.j.j.d.e.j.j.f.
-000000a0: 640b 640c 8404 5a10 6409 6501 6a0d 6a0e  d.d...Z.d.e.j.j.
-000000b0: 640a 6501 6a0d 6a0e 6406 6501 6a0d 6a0e  d.e.j.j.d.e.j.j.
-000000c0: 6606 640d 640e 8404 5a11 640f 6501 6a0d  f.d.d...Z.d.e.j.
-000000d0: 6a0e 6409 6501 6a0d 6a0e 6410 6501 6a0d  j.d.e.j.j.d.e.j.
-000000e0: 6a0e 6411 6501 6a0d 6a0e 6406 6501 6a0d  j.d.e.j.j.d.e.j.
-000000f0: 6a0e 660a 6412 6413 8404 5a12 640a 6501  j.f.d.d...Z.d.e.
-00000100: 6a0d 6a0e 6414 6501 6a0d 6a0e 6406 6501  j.j.d.e.j.j.d.e.
-00000110: 6a0d 6a0e 6606 6415 6416 8404 5a13 6417  j.j.f.d.d...Z.d.
-00000120: 6501 6a0d 6a0e 6a14 6406 6515 6516 6516  e.j.j.j.d.e.e.e.
-00000130: 6503 1900 1900 6516 6517 1900 6602 1900  e.....e.e...f...
-00000140: 6604 6418 6419 8404 5a18 6401 5300 291a  f.d.d...Z.d.S.).
-00000150: e900 0000 004e 2901 da03 416e 7929 01da  .....N)...Any)..
-00000160: 066c 6f67 6765 72a9 01da 0c61 6374 696f  .logger....actio
-00000170: 6e5f 636f 6465 7329 07da 0463 6f64 65da  n_codes)...code.
-00000180: 056c 6162 656c da02 7365 da02 6f6e 5a0f  .label..se..onZ.
-00000190: 4c69 7374 456c 656d 656e 7449 7465 6d5a  ListElementItemZ
-000001a0: 0370 7269 5a03 7069 6eda 0672 6574 7572  .priZ.pin..retur
-000001b0: 6e63 0000 0000 0000 0000 0000 0000 0000  nc..............
-000001c0: 0000 0100 0000 4300 0000 7304 0000 0074  ......C...s....t
-000001d0: 0053 0029 014e 7204 0000 00a9 0072 0b00  .S.).Nr......r..
-000001e0: 0000 720b 0000 00fa 762f 5573 6572 732f  ..r.....v/Users/
-000001f0: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
-00000200: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
-00000210: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
-00000220: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
-00000230: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
-00000240: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
-00000250: 2f73 7263 2f61 6374 696f 6e64 2e70 79da  /src/actiond.py.
-00000260: 0867 6574 5f64 6963 741b 0000 0073 0200  .get_dict....s..
-00000270: 0000 0401 720d 0000 00da 0661 6374 696f  ....r......actio
-00000280: 6eda 0964 6963 745f 636f 6465 6302 0000  n..dict_codec...
-00000290: 0000 0000 0000 0000 0006 0000 0008 0000  ................
-000002a0: 0043 0000 0073 7000 0000 7400 a001 7c00  .C...sp...t...|.
-000002b0: 7402 a102 5c03 7d02 7d03 7d04 7403 7c02  t...\.}.}.}.t.|.
-000002c0: 8301 7d05 7c05 7404 7c01 1900 6401 1900  ..}.|.t.|...d...
-000002d0: 6b04 7236 7c05 7404 7c01 1900 6401 3c00  k.r6|.t.|...d.<.
-000002e0: 7c04 7404 7c01 1900 6402 3c00 7c03 7404  |.t.|...d.<.|.t.
-000002f0: 7c01 1900 6403 3c00 7405 a006 6404 7c01  |...d.<.t...d.|.
-00000300: 9b00 6405 7407 7404 7c01 1900 8301 9b00  ..d.t.t.|.......
-00000310: 9d04 a101 0100 6400 5300 2906 4eda 076e  ......d.S.).N..n
-00000320: 756d 6172 6773 da04 6172 6773 da05 7479  umargs..args..ty
-00000330: 7065 737a 1575 7064 6174 655f 6163 7469  pesz.update_acti
-00000340: 6f6e 5f63 6f64 6573 3a20 fa01 2029 08da  on_codes: .. )..
-00000350: 0a67 6574 5f61 6374 696f 6eda 0867 6574  .get_action..get
-00000360: 5f61 7267 73da 0b69 676e 6f72 655f 6c69  _args..ignore_li
-00000370: 7374 da03 6c65 6e72 0500 0000 7203 0000  st..lenr....r...
-00000380: 00da 0564 6562 7567 da03 7374 72a9 0672  ...debug..str..r
-00000390: 0e00 0000 720f 0000 00da 0861 7267 5f6c  ....r......arg_l
-000003a0: 6973 74da 0974 7970 655f 6c69 7374 da08  ist..type_list..
-000003b0: 6172 675f 6e75 6d73 5a09 6172 675f 636f  arg_numsZ.arg_co
-000003c0: 756e 7472 0b00 0000 720b 0000 0072 0c00  untr....r....r..
-000003d0: 0000 da13 7570 6461 7465 5f61 6374 696f  ....update_actio
-000003e0: 6e5f 636f 6465 7322 0000 0073 1000 0000  n_codes"...s....
-000003f0: 1209 0801 1003 0c02 0c01 0c01 1e01 0401  ................
-00000400: 721e 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00000410: 0000 0600 0000 0400 0000 4300 0000 733e  ..........C...s>
-00000420: 0000 0074 00a0 0164 017c 019b 009d 02a1  ...t...d.|......
-00000430: 0101 0074 02a0 037c 0074 04a1 025c 037d  ...t...|.t...\.}
-00000440: 027d 037d 0474 057c 0283 017d 057c 057c  .}.}.t.|...}.|.|
-00000450: 047c 0364 029c 0374 067c 013c 0064 0053  .|.d...t.|.<.d.S
-00000460: 0029 034e 7a07 2e2e 2e66 6f72 2029 0372  .).Nz....for ).r
-00000470: 1000 0000 7211 0000 0072 1200 0000 2907  ....r....r....).
-00000480: 7203 0000 00da 0469 6e66 6f72 1400 0000  r......infor....
-00000490: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-000004a0: 0500 0000 721a 0000 0072 0b00 0000 720b  ....r....r....r.
-000004b0: 0000 0072 0c00 0000 da16 6275 696c 645f  ...r......build_
-000004c0: 6e65 775f 6163 7469 6f6e 5f63 6f64 6573  new_action_codes
-000004d0: 3b00 0000 7310 0000 0010 0312 0708 0102  ;...s...........
-000004e0: 0202 0102 010a fd04 0572 2000 0000 da05  .........r .....
-000004f0: 6368 696c 64da 0561 6464 6572 da0c 7072  child..adder..pr
-00000500: 6f67 7261 6d5f 6172 6773 6304 0000 0000  ogram_argsc.....
-00000510: 0000 0000 0000 0005 0000 0006 0000 0043  ...............C
-00000520: 0000 0073 6000 0000 7c00 6a00 7c02 1700  ...s`...|.j.|...
-00000530: 7d04 7c04 7401 7601 7229 7402 7c01 7c04  }.|.t.v.r)t.|.|.
-00000540: 8302 0100 7403 a004 6401 7c04 9b00 6402  ....t...d.|...d.
-00000550: 9d03 7401 7c04 1900 a102 0100 7c03 6403  ..t.|.......|.d.
-00000560: 1900 7227 7405 6401 7c04 6402 7401 7c04  ..r't.d.|.d.t.|.
-00000570: 1900 8304 0100 6400 5300 7406 7c01 7c04  ......d.S.t.|.|.
-00000580: 8302 0100 6400 5300 2904 4e7a 1862 7569  ....d.S.).Nz.bui
-00000590: 6c64 5f6e 6577 5f61 6374 696f 6e5f 636f  ld_new_action_co
-000005a0: 6465 733a 2072 1300 0000 7218 0000 0029  des: r....r....)
-000005b0: 07da 0474 6578 7472 0500 0000 7220 0000  ...textr....r ..
-000005c0: 0072 0300 0000 7218 0000 00da 0570 7269  .r....r......pri
-000005d0: 6e74 721e 0000 0029 0572 2100 0000 720e  ntr....).r!...r.
-000005e0: 0000 0072 2200 0000 7223 0000 0072 0f00  ...r"...r#...r..
-000005f0: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000600: 00da 1262 7569 6c64 5f61 6374 696f 6e5f  ...build_action_
-00000610: 636f 6465 7355 0000 0073 1200 0000 0a07  codesU...s......
-00000620: 0802 0a02 1801 0801 1201 0403 0aff 0401  ................
-00000630: 7226 0000 00da 0c64 6973 706c 6179 5f6e  r&.....display_n
-00000640: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
-00000650: 0200 0000 0300 0000 4300 0000 732e 0000  ........C...s...
-00000660: 007c 0074 0076 0172 0974 0164 017c 0083  .|.t.v.r.t.d.|..
-00000670: 0201 007c 0174 007c 0019 0076 0172 157c  ...|.t.|...v.r.|
-00000680: 0174 007c 0019 0064 023c 0064 0053 0029  .t.|...d.<.d.S.)
-00000690: 034e da00 da07 6469 7370 6c61 7929 0272  .N....display).r
-000006a0: 0500 0000 7220 0000 0029 0272 0f00 0000  ....r ...).r....
-000006b0: 7227 0000 0072 0b00 0000 720b 0000 0072  r'...r....r....r
-000006c0: 0c00 0000 da18 6164 645f 6e61 6d65 5f74  ......add_name_t
-000006d0: 6f5f 6163 7469 6f6e 5f63 6f64 6573 6c00  o_action_codesl.
-000006e0: 0000 730a 0000 0008 030a 010c 010c 0104  ..s.............
-000006f0: 0172 2a00 0000 da0b 636f 6465 5f61 6374  .r*.....code_act
-00000700: 696f 6e63 0100 0000 0000 0000 0000 0000  ionc............
-00000710: 0900 0000 0600 0000 4300 0000 7378 0000  ........C...sx..
-00000720: 0067 0067 0002 027d 017d 027c 00a0 0064  .g.g...}.}.|...d
-00000730: 01a1 017d 037c 0364 0075 0172 387c 0344  ...}.|.d.u.r8|.D
-00000740: 005d 277d 0464 027c 046a 0176 0072 227c  .]'}.d.|.j.v.r"|
-00000750: 046a 02a0 03a1 007d 057c 02a0 047c 05a1  .j.....}.|...|..
-00000760: 0101 0071 107c 046a 0164 036b 0272 3774  ...q.|.j.d.k.r7t
-00000770: 05a0 067c 04a1 015c 037d 067d 077d 087c  ...|...\.}.}.}.|
-00000780: 01a0 047c 067c 077c 0867 03a1 0101 0071  ...|.|.|.g.....q
-00000790: 107c 017c 0266 0253 0029 044e da0d 436f  .|.|.f.S.).N..Co
-000007a0: 6e64 6974 696f 6e4c 6973 74da 0462 6f6f  nditionList..boo
-000007b0: 6cda 0943 6f6e 6469 7469 6f6e 2907 da04  l..Condition)...
-000007c0: 6669 6e64 da03 7461 6772 2400 0000 da05  find..tagr$.....
-000007d0: 7570 7065 72da 0661 7070 656e 6472 1400  upper..appendr..
-000007e0: 0000 da12 6576 616c 7561 7465 5f63 6f6e  ....evaluate_con
-000007f0: 6469 7469 6f6e 2909 722b 0000 00da 0e63  dition).r+.....c
-00000800: 6f6e 6469 7469 6f6e 5f6c 6973 74da 0c62  ondition_list..b
-00000810: 6f6f 6c65 616e 5f6c 6973 745a 1263 6f6e  oolean_listZ.con
-00000820: 6469 7469 6f6e 5f6c 6973 745f 7374 7272  dition_list_strr
-00000830: 2100 0000 da09 6f70 6572 6174 696f 6eda  !.....operation.
-00000840: 0c66 6972 7374 5f73 7472 696e 67da 0d74  .first_string..t
-00000850: 6865 5f6f 7065 7261 7469 6f6e da0d 7365  he_operation..se
-00000860: 636f 6e64 5f73 7472 696e 6772 0b00 0000  cond_stringr....
-00000870: 720b 0000 0072 0c00 0000 da16 7072 6f63  r....r......proc
-00000880: 6573 735f 636f 6e64 6974 696f 6e5f 6c69  ess_condition_li
-00000890: 7374 7a00 0000 7320 0000 000a 030a 0108  stz...s ........
-000008a0: 0108 010a 010a 010c 010a 0108 0502 fc02  ................
-000008b0: 0102 0102 0110 0202 8008 0172 3a00 0000  ...........r:...
-000008c0: 2919 da15 786d 6c2e 6574 7265 652e 456c  )...xml.etree.El
-000008d0: 656d 656e 7454 7265 65da 0378 6d6c da06  ementTree..xml..
-000008e0: 7479 7069 6e67 7202 0000 00da 146d 6170  typingr......map
-000008f0: 7461 736b 6572 2e73 7263 2e61 6374 696f  tasker.src.actio
-00000900: 6eda 0373 7263 720e 0000 0072 1400 0000  n..srcr....r....
-00000910: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
-00000920: 7379 7363 6f6e 7374 7203 0000 00da 156d  sysconstr......m
-00000930: 6170 7461 736b 6572 2e73 7263 2e61 6374  aptasker.src.act
-00000940: 696f 6e63 7205 0000 0072 1600 0000 da05  ioncr....r......
-00000950: 6574 7265 65da 0b45 6c65 6d65 6e74 5472  etree..ElementTr
-00000960: 6565 720d 0000 0072 1e00 0000 7220 0000  eer....r....r ..
-00000970: 0072 2600 0000 722a 0000 00da 0745 6c65  .r&...r*.....Ele
-00000980: 6d65 6e74 da05 7475 706c 65da 046c 6973  ment..tuple..lis
-00000990: 7472 1900 0000 723a 0000 0072 0b00 0000  tr....r:...r....
-000009a0: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-000009b0: 083c 6d6f 6475 6c65 3e01 0000 0073 5800  .<module>....sX.
-000009c0: 0000 080d 0c01 1202 0c01 0c01 0802 1206  ................
-000009d0: 0207 0601 02ff 0601 02ff 0602 0afe 0219  ................
-000009e0: 0601 02ff 0601 02ff 0602 0afe 021a 0601  ................
-000009f0: 02ff 0602 02fe 0603 02fd 0604 02fc 0605  ................
-00000a00: 0afb 0217 0601 02ff 0601 02ff 0602 0afe  ................
-00000a10: 020e 0801 02ff 1602 0efe                 ..........
+00000070: a201 5a0c 6406 6501 6a0d 6602 6407 6408  ..Z.d.e.j.f.d.d.
+00000080: 8404 5a0e 6409 6501 6a0d 6a0f 640a 6501  ..Z.d.e.j.j.d.e.
+00000090: 6a0d 6406 6501 6a0d 6606 640b 640c 8404  j.d.e.j.f.d.d...
+000000a0: 5a10 6409 6501 6a0d 6a0f 640a 6501 6a0d  Z.d.e.j.j.d.e.j.
+000000b0: 6406 6501 6a0d 6606 640d 640e 8404 5a11  d.e.j.f.d.d...Z.
+000000c0: 640f 6501 6a0d 6a0f 6409 6501 6a0d 6a0f  d.e.j.j.d.e.j.j.
+000000d0: 6410 6501 6a0d 6a0f 6411 6501 6a0d 6a0f  d.e.j.j.d.e.j.j.
+000000e0: 6406 6501 6a0d 660a 6412 6413 8404 5a12  d.e.j.f.d.d...Z.
+000000f0: 640a 6501 6a0d 6a0f 6414 6501 6a0d 6406  d.e.j.j.d.e.j.d.
+00000100: 6501 6a0d 6606 6415 6416 8404 5a13 6417  e.j.f.d.d...Z.d.
+00000110: 6501 6a0d 6a0f 6406 6514 6515 6515 6503  e.j.j.d.e.e.e.e.
+00000120: 1900 1900 6515 6516 1900 6602 1900 6604  ....e.e...f...f.
+00000130: 6418 6419 8404 5a17 6401 5300 291a e900  d.d...Z.d.S.)...
+00000140: 0000 004e 2901 da03 416e 7929 01da 066c  ...N)...Any)...l
+00000150: 6f67 6765 72a9 01da 0c61 6374 696f 6e5f  ogger....action_
+00000160: 636f 6465 7329 07da 0463 6f64 65da 056c  codes)...code..l
+00000170: 6162 656c da02 7365 da02 6f6e 5a0f 4c69  abel..se..onZ.Li
+00000180: 7374 456c 656d 656e 7449 7465 6d5a 0370  stElementItemZ.p
+00000190: 7269 5a03 7069 6eda 0672 6574 7572 6e63  riZ.pin..returnc
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0100 0000 4300 0000 7304 0000 0074 0053  ....C...s....t.S
+000001c0: 0029 014e 7204 0000 00a9 0072 0b00 0000  .).Nr......r....
+000001d0: 720b 0000 00fa 762f 5573 6572 732f 6d69  r.....v/Users/mi
+000001e0: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
+000001f0: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
+00000200: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
+00000210: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
+00000220: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
+00000230: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
+00000240: 7263 2f61 6374 696f 6e64 2e70 79da 0867  rc/actiond.py..g
+00000250: 6574 5f64 6963 741b 0000 0073 0200 0000  et_dict....s....
+00000260: 0401 720d 0000 00da 0661 6374 696f 6eda  ..r......action.
+00000270: 0964 6963 745f 636f 6465 6302 0000 0000  .dict_codec.....
+00000280: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00000290: 0000 0073 7000 0000 7400 a001 7c00 7402  ...sp...t...|.t.
+000002a0: a102 5c03 7d02 7d03 7d04 7403 7c02 8301  ..\.}.}.}.t.|...
+000002b0: 7d05 7c05 7404 7c01 1900 6401 1900 6b04  }.|.t.|...d...k.
+000002c0: 7236 7c05 7404 7c01 1900 6401 3c00 7c04  r6|.t.|...d.<.|.
+000002d0: 7404 7c01 1900 6402 3c00 7c03 7404 7c01  t.|...d.<.|.t.|.
+000002e0: 1900 6403 3c00 7405 a006 6404 7c01 9b00  ..d.<.t...d.|...
+000002f0: 6405 7407 7404 7c01 1900 8301 9b00 9d04  d.t.t.|.........
+00000300: a101 0100 6400 5300 2906 4eda 076e 756d  ....d.S.).N..num
+00000310: 6172 6773 da04 6172 6773 da05 7479 7065  args..args..type
+00000320: 737a 1575 7064 6174 655f 6163 7469 6f6e  sz.update_action
+00000330: 5f63 6f64 6573 3a20 fa01 2029 08da 0a67  _codes: .. )...g
+00000340: 6574 5f61 6374 696f 6eda 0867 6574 5f61  et_action..get_a
+00000350: 7267 73da 0b69 676e 6f72 655f 6c69 7374  rgs..ignore_list
+00000360: da03 6c65 6e72 0500 0000 7203 0000 00da  ..lenr....r.....
+00000370: 0564 6562 7567 da03 7374 72a9 0672 0e00  .debug..str..r..
+00000380: 0000 720f 0000 00da 0861 7267 5f6c 6973  ..r......arg_lis
+00000390: 74da 0974 7970 655f 6c69 7374 da08 6172  t..type_list..ar
+000003a0: 675f 6e75 6d73 5a09 6172 675f 636f 756e  g_numsZ.arg_coun
+000003b0: 7472 0b00 0000 720b 0000 0072 0c00 0000  tr....r....r....
+000003c0: da13 7570 6461 7465 5f61 6374 696f 6e5f  ..update_action_
+000003d0: 636f 6465 7322 0000 0073 1000 0000 1209  codes"...s......
+000003e0: 0801 1003 0c02 0c01 0c01 1e01 0401 721e  ..............r.
+000003f0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000400: 0600 0000 0400 0000 4300 0000 733e 0000  ........C...s>..
+00000410: 0074 00a0 0164 017c 019b 009d 02a1 0101  .t...d.|........
+00000420: 0074 02a0 037c 0074 04a1 025c 037d 027d  .t...|.t...\.}.}
+00000430: 037d 0474 057c 0283 017d 057c 057c 047c  .}.t.|...}.|.|.|
+00000440: 0364 029c 0374 067c 013c 0064 0053 0029  .d...t.|.<.d.S.)
+00000450: 034e 7a07 2e2e 2e66 6f72 2029 0372 1000  .Nz....for ).r..
+00000460: 0000 7211 0000 0072 1200 0000 2907 7203  ..r....r....).r.
+00000470: 0000 00da 0469 6e66 6f72 1400 0000 7215  .....infor....r.
+00000480: 0000 0072 1600 0000 7217 0000 0072 0500  ...r....r....r..
+00000490: 0000 721a 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+000004a0: 0072 0c00 0000 da16 6275 696c 645f 6e65  .r......build_ne
+000004b0: 775f 6163 7469 6f6e 5f63 6f64 6573 3b00  w_action_codes;.
+000004c0: 0000 7310 0000 0010 0312 0708 0102 0202  ..s.............
+000004d0: 0102 010a fd04 0572 2000 0000 da05 6368  .......r .....ch
+000004e0: 696c 64da 0561 6464 6572 da0c 7072 6f67  ild..adder..prog
+000004f0: 7261 6d5f 6172 6773 6304 0000 0000 0000  ram_argsc.......
+00000500: 0000 0000 0005 0000 0006 0000 0043 0000  .............C..
+00000510: 0073 6000 0000 7c00 6a00 7c02 1700 7d04  .s`...|.j.|...}.
+00000520: 7c04 7401 7601 7229 7402 7c01 7c04 8302  |.t.v.r)t.|.|...
+00000530: 0100 7403 a004 6401 7c04 9b00 6402 9d03  ..t...d.|...d...
+00000540: 7401 7c04 1900 a102 0100 7c03 6403 1900  t.|.......|.d...
+00000550: 7227 7405 6401 7c04 6402 7401 7c04 1900  r't.d.|.d.t.|...
+00000560: 8304 0100 6400 5300 7406 7c01 7c04 8302  ....d.S.t.|.|...
+00000570: 0100 6400 5300 2904 4e7a 1862 7569 6c64  ..d.S.).Nz.build
+00000580: 5f6e 6577 5f61 6374 696f 6e5f 636f 6465  _new_action_code
+00000590: 733a 2072 1300 0000 7218 0000 0029 07da  s: r....r....)..
+000005a0: 0474 6578 7472 0500 0000 7220 0000 0072  .textr....r ...r
+000005b0: 0300 0000 7218 0000 00da 0570 7269 6e74  ....r......print
+000005c0: 721e 0000 0029 0572 2100 0000 720e 0000  r....).r!...r...
+000005d0: 0072 2200 0000 7223 0000 0072 0f00 0000  .r"...r#...r....
+000005e0: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+000005f0: 1262 7569 6c64 5f61 6374 696f 6e5f 636f  .build_action_co
+00000600: 6465 7355 0000 0073 1200 0000 0a07 0802  desU...s........
+00000610: 0a02 1801 0801 1201 0403 0aff 0401 7226  ..............r&
+00000620: 0000 00da 0c64 6973 706c 6179 5f6e 616d  .....display_nam
+00000630: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
+00000640: 0000 0300 0000 4300 0000 732e 0000 007c  ......C...s....|
+00000650: 0074 0076 0172 0974 0164 017c 0083 0201  .t.v.r.t.d.|....
+00000660: 007c 0174 007c 0019 0076 0172 157c 0174  .|.t.|...v.r.|.t
+00000670: 007c 0019 0064 023c 0064 0053 0029 034e  .|...d.<.d.S.).N
+00000680: da00 da07 6469 7370 6c61 7929 0272 0500  ....display).r..
+00000690: 0000 7220 0000 0029 0272 0f00 0000 7227  ..r ...).r....r'
+000006a0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+000006b0: 0000 da18 6164 645f 6e61 6d65 5f74 6f5f  ....add_name_to_
+000006c0: 6163 7469 6f6e 5f63 6f64 6573 6c00 0000  action_codesl...
+000006d0: 730a 0000 0008 030a 010c 010c 0104 0172  s..............r
+000006e0: 2a00 0000 da0b 636f 6465 5f61 6374 696f  *.....code_actio
+000006f0: 6e63 0100 0000 0000 0000 0000 0000 0900  nc..............
+00000700: 0000 0600 0000 4300 0000 7378 0000 0067  ......C...sx...g
+00000710: 0067 0002 027d 017d 027c 00a0 0064 01a1  .g...}.}.|...d..
+00000720: 017d 037c 0364 0075 0172 387c 0344 005d  .}.|.d.u.r8|.D.]
+00000730: 277d 0464 027c 046a 0176 0072 227c 046a  '}.d.|.j.v.r"|.j
+00000740: 02a0 03a1 007d 057c 02a0 047c 05a1 0101  .....}.|...|....
+00000750: 0071 107c 046a 0164 036b 0272 3774 05a0  .q.|.j.d.k.r7t..
+00000760: 067c 04a1 015c 037d 067d 077d 087c 01a0  .|...\.}.}.}.|..
+00000770: 047c 067c 077c 0867 03a1 0101 0071 107c  .|.|.|.g.....q.|
+00000780: 017c 0266 0253 0029 044e da0d 436f 6e64  .|.f.S.).N..Cond
+00000790: 6974 696f 6e4c 6973 74da 0462 6f6f 6cda  itionList..bool.
+000007a0: 0943 6f6e 6469 7469 6f6e 2907 da04 6669  .Condition)...fi
+000007b0: 6e64 da03 7461 6772 2400 0000 da05 7570  nd..tagr$.....up
+000007c0: 7065 72da 0661 7070 656e 6472 1400 0000  per..appendr....
+000007d0: da12 6576 616c 7561 7465 5f63 6f6e 6469  ..evaluate_condi
+000007e0: 7469 6f6e 2909 722b 0000 00da 0e63 6f6e  tion).r+.....con
+000007f0: 6469 7469 6f6e 5f6c 6973 74da 0c62 6f6f  dition_list..boo
+00000800: 6c65 616e 5f6c 6973 745a 1263 6f6e 6469  lean_listZ.condi
+00000810: 7469 6f6e 5f6c 6973 745f 7374 7272 2100  tion_list_strr!.
+00000820: 0000 da09 6f70 6572 6174 696f 6eda 0c66  ....operation..f
+00000830: 6972 7374 5f73 7472 696e 67da 0d74 6865  irst_string..the
+00000840: 5f6f 7065 7261 7469 6f6e da0d 7365 636f  _operation..seco
+00000850: 6e64 5f73 7472 696e 6772 0b00 0000 720b  nd_stringr....r.
+00000860: 0000 0072 0c00 0000 da16 7072 6f63 6573  ...r......proces
+00000870: 735f 636f 6e64 6974 696f 6e5f 6c69 7374  s_condition_list
+00000880: 7a00 0000 7320 0000 000a 030a 0108 0108  z...s ..........
+00000890: 010a 010a 010c 010a 0108 0502 fc02 0102  ................
+000008a0: 0102 0110 0202 8008 0172 3a00 0000 2918  .........r:...).
+000008b0: da16 6465 6675 7365 6478 6d6c 2e45 6c65  ..defusedxml.Ele
+000008c0: 6d65 6e74 5472 6565 da0a 6465 6675 7365  mentTree..defuse
+000008d0: 6478 6d6c da06 7479 7069 6e67 7202 0000  dxml..typingr...
+000008e0: 00da 146d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+000008f0: 2e61 6374 696f 6eda 0373 7263 720e 0000  .action..srcr...
+00000900: 0072 1400 0000 da16 6d61 7074 6173 6b65  .r......maptaske
+00000910: 722e 7372 632e 7379 7363 6f6e 7374 7203  r.src.sysconstr.
+00000920: 0000 00da 156d 6170 7461 736b 6572 2e73  .....maptasker.s
+00000930: 7263 2e61 6374 696f 6e63 7205 0000 0072  rc.actioncr....r
+00000940: 1600 0000 da0b 456c 656d 656e 7454 7265  ......ElementTre
+00000950: 6572 0d00 0000 da03 584d 4c72 1e00 0000  er......XMLr....
+00000960: 7220 0000 0072 2600 0000 722a 0000 00da  r ...r&...r*....
+00000970: 0574 7570 6c65 da04 6c69 7374 7219 0000  .tuple..listr...
+00000980: 0072 3a00 0000 720b 0000 0072 0b00 0000  .r:...r....r....
+00000990: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+000009a0: 756c 653e 0100 0000 7358 0000 0008 0d0c  ule>....sX......
+000009b0: 0112 020c 010c 0108 0210 0602 0706 0102  ................
+000009c0: ff04 0102 ff04 020a fe02 1906 0102 ff04  ................
+000009d0: 0102 ff04 020a fe02 1a06 0102 ff06 0202  ................
+000009e0: fe06 0302 fd06 0402 fc04 050a fb02 1706  ................
+000009f0: 0102 ff04 0102 ff04 020a fe02 0e06 0102  ................
+00000a00: ff16 020e fe                             .....
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/actione.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/actione.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 17:31:26 2023 UTC, .py size: 9670 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-00000000: 6f0d 0d0a 0000 0000 ee5e 2c64 c625 0000  o........^,d.%..
+00000000: 6f0d 0d0a 0000 0000 ed54 3864 4d26 0000  o........T8dM&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 6d05 0200  d.l.Z.d.d.l.m...
 00000050: 0100 6d06 5a07 0100 6400 6402 6c08 6d09  ..m.Z...d.d.l.m.
 00000060: 5a09 0100 6400 6403 6c0a 6d0b 5a0b 0100  Z...d.d.l.m.Z...
 00000070: 6400 6404 6c0c 6d0d 5a0d 0100 6400 6405  d.d.l.m.Z...d.d.
 00000080: 6c0e 6d0f 5a0f 0100 6400 6406 6c0e 6d10  l.m.Z...d.d.l.m.
 00000090: 5a10 0100 6501 a011 6407 a101 5a12 6408  Z...e...d...Z.d.
 000000a0: 6409 8400 5a13 640a 640b 8400 5a14 640c  d...Z.d.d...Z.d.
 000000b0: 640d 8400 5a15 640e 6503 6a16 6a17 640f  d...Z.d.e.j.j.d.
 000000c0: 6503 6a16 6a17 6410 6518 6411 6519 6412  e.j.j.d.e.d.e.d.
 000000d0: 651a 6413 6519 6414 651a 660e 6415 6416  e.d.e.d.e.f.d.d.
 000000e0: 8404 5a1b 6417 6418 8400 5a1c 6401 5300  ..Z.d.d...Z.d.S.
-000000f0: 2919 e900 0000 004e 2901 da0e 434f 4e54  )......N)...CONT
-00000100: 494e 5545 5f4c 494d 4954 2901 da0f 6765  INUE_LIMIT)...ge
-00000110: 745f 6578 7472 615f 7374 7566 6629 01da  t_extra_stuff)..
-00000120: 0c61 6374 696f 6e5f 636f 6465 7329 01da  .action_codes)..
-00000130: 066c 6f67 6765 7229 01da 0b46 4f4e 545f  .logger)...FONT_
-00000140: 544f 5f55 5345 7a06 2c5b 2c20 5d2b 6301  TO_USEz.,[, ]+c.
-00000150: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000160: 0000 0043 0000 0073 9400 0000 7c00 a000  ...C...s....|...
-00000170: 6401 6402 a102 7d00 7c00 a000 6403 6404  d.d...}.|...d.d.
-00000180: a102 7d00 7401 a002 6405 7c00 a102 7d00  ..}.t...d.|...}.
-00000190: 7c00 a000 6406 6407 a102 7d00 7c00 a000  |...d.d...}.|...
-000001a0: 6408 6409 a102 7d00 7c00 a000 640a 6404  d.d...}.|...d.d.
-000001b0: a102 7d00 7c00 a000 640b 6404 a102 7d00  ..}.|...d.d...}.
-000001c0: 7c00 a000 640c 6404 a102 7d00 7c00 a000  |...d.d...}.|...
-000001d0: 640d 6404 a102 7d00 7c00 a000 640e 6404  d.d...}.|...d.d.
-000001e0: a102 7d00 7c00 a000 640f 6404 a102 7d00  ..}.|...d.d...}.
-000001f0: 7c00 a000 6410 6411 a102 7d00 7c00 5300  |...d.d...}.|.S.
-00000200: 2912 4e7a 092c 2020 3c66 6f6e 743e 7a06  ).Nz.,  <font>z.
-00000210: 3c66 6f6e 743e 7a03 2c20 28da 007a 022c  <font>z., (..z.,
-00000220: 207a 072c 203c 7370 616e 7a05 3c73 7061   z., <spanz.<spa
-00000230: 6e7a 082c 2020 3c73 7061 6e7a 0720 203c  nz.,  <spanz.  <
-00000240: 7370 616e 7a07 2c20 636f 6465 3a7a 053c  spanz., code:z.<
-00000250: 6269 673e 7a07 3c73 6d61 6c6c 3e7a 043c  big>z.<small>z.<
-00000260: 7474 3e7a 033c 693e 7a03 3c75 3e7a 072c  tt>z.<i>z.<u>z.,
-00000270: 203c 666f 6e74 7a05 3c66 6f6e 7429 03da   <fontz.<font)..
-00000280: 0772 6570 6c61 6365 da07 7061 7474 6572  .replace..patter
-00000290: 6eda 0373 7562 2901 da07 7265 7375 6c74  n..sub)...result
-000002a0: 73a9 0072 0c00 0000 fa76 2f55 7365 7273  s..r.....v/Users
-000002b0: 2f6d 696b 7275 6269 6e2f 4c69 6272 6172  /mikrubin/Librar
-000002c0: 792f 436c 6f75 6453 746f 7261 6765 2f47  y/CloudStorage/G
-000002d0: 6f6f 676c 6544 7269 7665 2d6d 696b 7275  oogleDrive-mikru
-000002e0: 6269 6e40 676d 6169 6c2e 636f 6d2f 4d79  bin@gmail.com/My
-000002f0: 2044 7269 7665 2f50 7974 686f 6e2f 6d61   Drive/Python/ma
-00000300: 7074 6173 6b65 722f 6d61 7074 6173 6b65  ptasker/maptaske
-00000310: 722f 7372 632f 6163 7469 6f6e 652e 7079  r/src/actione.py
-00000320: da12 636c 6561 6e75 705f 7468 655f 7265  ..cleanup_the_re
-00000330: 7375 6c74 1f00 0000 731e 0000 0004 0304  sult....s.......
-00000340: 0104 ff0c 030c 010c 010c 010c 010c 010c  ................
-00000350: 010c 010c 010c 010c 0104 0172 0e00 0000  ...........r....
-00000360: 6300 0000 0000 0000 0000 0000 0005 0000  c...............
-00000370: 0005 0000 0043 0000 0073 9c00 0000 6401  .....C...s....d.
-00000380: 7d00 7400 4400 5d3f 7d01 7400 7c01 1900  }.t.D.]?}.t.|...
-00000390: 7d02 7c02 6402 1900 7d03 7c03 6403 6b04  }.|.d...}.|.d.k.
-000003a0: 722a 6404 7c02 7601 722a 6405 7c01 9b00  r*d.|.v.r*d.|...
-000003b0: 6406 7c03 9b00 9d04 7d04 7401 7c04 8301  d.|.....}.t.|...
-000003c0: 0100 7402 a003 7c04 9b00 a101 0100 6407  ..t...|.......d.
-000003d0: 7d00 6408 7c02 7601 7243 6405 7c01 9b00  }.d.|.v.rCd.|...
-000003e0: 6409 9d03 7d04 7401 7c04 8301 0100 7402  d...}.t.|.....t.
-000003f0: a003 7c04 a101 0100 640a 7c02 6408 3c00  ..|.....d.|.d.<.
-00000400: 6407 7d00 7104 7c00 724c 7404 640b 8301  d.}.q.|.rLt.d...
-00000410: 0100 6400 5300 6400 5300 290c 4e46 da07  ..d.S.d.S.).NF..
-00000420: 6e75 6d61 7267 7372 0100 0000 da07 7265  numargsr......re
-00000430: 7161 7267 737a 1145 7272 6f72 3a20 6469  qargsz.Error: di
-00000440: 6374 5f63 6f64 6520 7a1b 206d 6973 7369  ct_code z. missi
-00000450: 6e67 2072 6571 6172 6773 2120 206e 756d  ng reqargs!  num
-00000460: 6172 6773 3a54 da07 6469 7370 6c61 797a  args:T..displayz
-00000470: 1320 6d69 7373 696e 6720 2264 6973 706c  . missing "displ
-00000480: 6179 2221 5a08 756e 6d61 7070 6564 e963  ay"!Z.unmapped.c
-00000490: 0000 0029 0572 0400 0000 da05 7072 696e  ...).r......prin
-000004a0: 7472 0500 0000 da05 6465 6275 67da 0465  tr......debug..e
-000004b0: 7869 7429 05da 0466 6c61 67da 0469 7465  xit)...flag..ite
-000004c0: 6dda 0565 6e74 7279 720f 0000 00da 0965  m..entryr......e
-000004d0: 7272 6f72 5f6d 7367 720c 0000 0072 0c00  rror_msgr....r..
-000004e0: 0000 720d 0000 00da 146c 6f6f 6b5f 666f  ..r......look_fo
-000004f0: 725f 6d69 7373 696e 675f 7265 7136 0000  r_missing_req6..
-00000500: 0073 2600 0000 0401 0801 0801 0801 1001  .s&.............
-00000510: 1001 0801 0c01 0401 0801 0c01 0801 0a01  ................
-00000520: 0801 0401 0280 0401 0c01 04ff 721a 0000  ............r...
-00000530: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
-00000540: 0000 0300 0000 4300 0000 7344 0000 0064  ......C...sD...d
-00000550: 0164 026c 006d 017d 0101 007c 0064 0064  .d.l.m.}...|.d.d
-00000560: 0385 0219 007d 027c 027c 0176 0072 207c  .....}.|.|.v.r |
-00000570: 0074 0276 0072 2064 0474 027c 0019 0064  .t.v.r d.t.|...d
-00000580: 0419 0064 0517 0069 0174 027c 003c 0064  ...d...i.t.|.<.d
-00000590: 0053 0029 064e 7201 0000 0029 01da 0a64  .S.).Nr....)...d
-000005a0: 6570 7269 6361 7465 64e9 ffff ffff 7211  epricated.....r.
-000005b0: 0000 007a 1a3c 656d 3e20 2849 7320 4465  ...z.<em> (Is De
-000005c0: 7072 6563 6174 6564 293c 2f65 6d3e 2029  precated)</em> )
-000005d0: 035a 186d 6170 7461 736b 6572 2e73 7263  .Z.maptasker.src
-000005e0: 2e64 6570 7269 6361 7465 6472 1b00 0000  .depricatedr....
-000005f0: 7204 0000 0029 03da 0964 6963 745f 636f  r....)...dict_co
-00000600: 6465 721b 0000 00da 066c 6f6f 6b75 7072  der......lookupr
-00000610: 0c00 0000 720c 0000 0072 0d00 0000 da15  ....r....r......
-00000620: 6368 6563 6b5f 666f 725f 6465 7072 6563  check_for_deprec
-00000630: 6174 696f 6e4d 0000 0073 0c00 0000 0c01  ationM...s......
-00000640: 0c02 1001 1002 08ff 0403 721f 0000 00da  ..........r.....
-00000650: 0a63 6f64 655f 6368 696c 64da 0b63 6f64  .code_child..cod
-00000660: 655f 6163 7469 6f6e da0b 6163 7469 6f6e  e_action..action
-00000670: 5f74 7970 65da 0863 6f6c 6f72 6d61 70da  _type..colormap.
-00000680: 0963 6f64 655f 7479 7065 da0c 7072 6f67  .code_type..prog
-00000690: 7261 6d5f 6172 6773 da06 7265 7475 726e  ram_args..return
-000006a0: 6306 0000 0000 0000 0000 0000 000c 0000  c...............
-000006b0: 000a 0000 0043 0000 0073 6801 0000 7400  .....C...sh...t.
-000006c0: a001 6401 7c00 6a02 9b00 7c04 9b00 9d03  ..d.|.j...|.....
-000006d0: a101 0100 7c00 6a02 7c04 1700 7d06 7403  ....|.j.|...}.t.
-000006e0: 7c06 8301 0100 7c06 7404 7601 731e 6402  |.....|.t.v.s.d.
-000006f0: 7404 7c06 1900 7601 7235 6403 7c06 9b00  t.|...v.r5d.|...
-00000700: 6404 7405 7c01 7c02 7c03 7c05 8304 9b00  d.t.|.|.|.|.....
-00000710: 9d04 7d07 7400 a001 6405 7c06 9b00 6406  ..}.t...d.|...d.
-00000720: 9d03 a101 0100 6e79 6407 7c03 6408 1900  ......nyd.|.d...
-00000730: 1700 7c05 6409 1900 1700 640a 1700 7404  ..|.d.....d...t.
-00000740: 7c06 1900 6402 1900 1700 640b 1700 7d07  |...d.....d...}.
-00000750: 640c 7404 7c06 1900 7600 7256 7404 7c06  d.t.|...v.rVt.|.
-00000760: 1900 640c 1900 7d08 6e02 640d 7d08 7c08  ..d...}.n.d.}.|.
-00000770: 640d 6b03 7276 640e 7404 7c06 1900 7600  d.k.rvd.t.|...v.
-00000780: 7276 7406 a007 7c06 7404 7c01 7c02 7c03  rvt...|.t.|.|.|.
-00000790: 7404 7c06 1900 640e 1900 7404 7c06 1900  t.|...d...t.|...
-000007a0: 640f 1900 7c05 a108 7d07 6410 7404 7c06  d...|...}.d.t.|.
-000007b0: 1900 7600 72ae 7404 7c06 1900 6410 1900  ..v.r.t.|...d...
-000007c0: 640d 1900 7d09 7c06 7408 a009 7404 7c09  d...}.|.t...t.|.
-000007d0: 1900 a101 6901 7d0a 7404 7c06 1900 6402  ....i.}.t.|...d.
-000007e0: 1900 7d0b 7408 a009 7c0b a101 7c0a 6402  ..}.t...|...|.d.
-000007f0: 3c00 7406 a007 7c06 7c0a 7c01 7c02 7c03  <.t...|.|.|.|.|.
-00000800: 7c0a 7c06 1900 640e 1900 7c0a 7c06 1900  |.|...d...|.|...
-00000810: 640f 1900 7c05 a108 7d07 740a 7c07 8301  d...|...}.t.|...
-00000820: 7d07 7c07 5300 2911 6195 0100 000a 2020  }.|.S.).a.....  
-00000830: 2020 4769 7665 6e20 616e 2061 6374 696f    Given an actio
-00000840: 6e20 636f 6465 2c20 6576 616c 7561 7465  n code, evaluate
-00000850: 2069 7420 666f 7220 6469 7370 6c61 790a   it for display.
-00000860: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-00000870: 6f64 655f 6368 696c 643a 2078 6d6c 2065  ode_child: xml e
-00000880: 6c65 6d65 6e74 206f 6620 7468 6520 3c63  lement of the <c
-00000890: 6f64 653e 0a20 2020 2020 2020 203a 7061  ode>.        :pa
-000008a0: 7261 6d20 636f 6465 5f61 6374 696f 6e3a  ram code_action:
-000008b0: 2076 616c 7565 206f 6620 3c63 6f64 653e   value of <code>
-000008c0: 2028 652e 672e 2022 3534 3922 290a 2020   (e.g. "549").  
-000008d0: 2020 2020 2020 3a70 6172 616d 2061 6374        :param act
-000008e0: 696f 6e5f 7479 7065 3a0a 2020 2020 2020  ion_type:.      
-000008f0: 2020 3a70 6172 616d 2063 6f6c 6f72 6d61    :param colorma
-00000900: 703a 2063 6f6c 6f72 7320 746f 2075 7365  p: colors to use
-00000910: 2069 6e20 6f75 7470 7574 0a20 2020 2020   in output.     
-00000920: 2020 203a 7061 7261 6d20 636f 6465 5f74     :param code_t
-00000930: 7970 653a 2027 6527 3d65 7665 6e74 2c20  ype: 'e'=event, 
-00000940: 2773 273d 7374 6174 652c 2027 7427 3d74  's'=state, 't'=t
-00000950: 6173 6b0a 2020 2020 2020 2020 3a70 6172  ask.        :par
-00000960: 616d 2070 726f 6772 616d 5f61 7267 733a  am program_args:
-00000970: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
-00000980: 7473 0a20 2020 2020 2020 203a 7265 7475  ts.        :retu
-00000990: 726e 3a20 666f 726d 6174 7465 6420 6f75  rn: formatted ou
-000009a0: 7470 7574 206c 696e 6520 7769 7468 2061  tput line with a
-000009b0: 6374 696f 6e20 6465 7461 696c 730a 2020  ction details.  
-000009c0: 2020 7a08 6765 7463 6f64 653a 7211 0000    z.getcode:r...
-000009d0: 007a 0543 6f64 6520 7a0f 206e 6f74 2079  .z.Code z. not y
-000009e0: 6574 206d 6170 7065 647a 1475 6e6d 6170  et mappedz.unmap
-000009f0: 7065 6420 7461 736b 2063 6f64 653a 20fa  ped task code: .
-00000a00: 0120 7a13 3c73 7061 6e20 7374 796c 653d  . z.<span style=
-00000a10: 2263 6f6c 6f72 3a5a 1161 6374 696f 6e5f  "color:Z.action_
-00000a20: 6e61 6d65 5f63 6f6c 6f72 da0b 666f 6e74  name_color..font
-00000a30: 5f74 6f5f 7573 65fa 013e 7a07 3c2f 7370  _to_use..>z.</sp
-00000a40: 616e 3e72 0f00 0000 7201 0000 0072 1000  an>r....r....r..
-00000a50: 0000 5a08 6576 616c 6172 6773 5a08 7265  ..Z.evalargsZ.re
-00000a60: 6469 7265 6374 290b 7205 0000 0072 1400  direct).r....r..
-00000a70: 0000 da04 7465 7874 721f 0000 0072 0400  ....textr....r..
-00000a80: 0000 7203 0000 00da 0e61 6374 696f 6e5f  ..r......action_
-00000a90: 7265 7375 6c74 735a 1267 6574 5f61 6374  resultsZ.get_act
-00000aa0: 696f 6e5f 7265 7375 6c74 73da 0463 6f70  ion_results..cop
-00000ab0: 79da 0864 6565 7063 6f70 7972 0e00 0000  y..deepcopyr....
-00000ac0: 290c 7220 0000 0072 2100 0000 7222 0000  ).r ...r!...r"..
-00000ad0: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-00000ae0: 721d 0000 005a 0a74 6865 5f72 6573 756c  r....Z.the_resul
-00000af0: 7472 0f00 0000 5a08 7265 6665 7272 616c  tr....Z.referral
-00000b00: 5a11 7465 6d70 5f6c 6f6f 6b75 705f 636f  Z.temp_lookup_co
-00000b10: 6465 735a 0c64 6973 706c 6179 5f6e 616d  desZ.display_nam
-00000b20: 6572 0c00 0000 720c 0000 0072 0d00 0000  er....r....r....
-00000b30: da0f 6765 745f 6163 7469 6f6e 5f63 6f64  ..get_action_cod
-00000b40: 655b 0000 0073 7000 0000 1612 0a01 0802  e[...sp.........
-00000b50: 1402 0802 0c01 04ff 02ff 1404 0205 0601  ................
-00000b60: 02ff 0602 02fe 0203 02fd 0a04 02fc 0205  ................
-00000b70: 02fb 02ff 0c08 0e01 0402 1402 0401 0201  ................
-00000b80: 0201 0201 0201 0201 0a01 0a01 0201 04f8  ................
-00000b90: 0c0c 0a01 0201 04ff 1203 0601 0201 04ff  ................
-00000ba0: 0e03 0402 0201 0201 0201 0201 0201 0a01  ................
-00000bb0: 0a01 0201 04f8 080b 0401 722e 0000 0063  ..........r....c
-00000bc0: 0500 0000 0000 0000 0000 0000 0a00 0000  ................
-00000bd0: 0600 0000 4300 0000 73fa 0000 007c 037d  ....C...s....|.}
-00000be0: 057c 0564 016b 0372 177c 01a0 0074 019b  .|.d.k.r.|...t..
-00000bf0: 0064 029d 0274 019b 0064 027c 049b 009d  .d...t...d.|....
-00000c00: 0364 03a1 037d 0164 017d 057c 0564 016b  .d...}.d.}.|.d.k
-00000c10: 0072 1f7c 047c 0117 007d 017c 0164 046b  .r.|.|...}.|.d.k
-00000c20: 0372 717c 01a0 0264 05a1 017d 0674 037c  .rq|...d...}.t.|
-00000c30: 0183 017d 077c 0664 066b 0272 3b7c 0764  ...}.|.d.k.r;|.d
-00000c40: 076b 0472 3b7c 00a0 047c 01a1 0101 0064  .k.r;|...|.....d
-00000c50: 0053 007c 01a0 0564 05a1 017d 0864 017d  .S.|...d...}.d.}
-00000c60: 057c 0844 005d 2a7d 097c 0564 016b 0272  .|.D.]*}.|.d.k.r
-00000c70: 507c 00a0 047c 09a1 0101 006e 087c 00a0  P|...|.....n.|..
-00000c80: 0464 087c 099b 009d 02a1 0101 007c 0564  .d.|.........|.d
-00000c90: 0337 007d 057c 0574 066b 0272 6e7c 00a0  .7.}.|.t.k.rn|..
-00000ca0: 0464 0974 0774 0683 019b 0064 0a9d 03a1  .d.t.t.....d....
-00000cb0: 0101 0001 0064 0053 0071 4464 0053 007c  .....d.S.qDd.S.|
-00000cc0: 00a0 0464 0b7c 026a 089b 0064 0c9d 03a1  ...d.|.j...d....
-00000cd0: 0101 0064 0053 0029 0d4e 7201 0000 0072  ...d.S.).Nr....r
-00000ce0: 2900 0000 e901 0000 0072 0700 0000 da01  )........r......
-00000cf0: 0a72 1c00 0000 e950 0000 007a 032e 2e2e  .r.....P...z....
-00000d00: 7a2f 3c73 7061 6e20 7374 796c 653d 2263  z/<span style="c
-00000d10: 6f6c 6f72 3a72 6564 223e 202e 2e2e 2063  olor:red"> ... c
-00000d20: 6f6e 7469 6e75 6520 6c69 6d69 7420 6f66  ontinue limit of
-00000d30: 207a 3c20 7265 6163 6865 642e 2020 5365   z< reached.  Se
-00000d40: 6520 2243 4f4e 5449 4e55 455f 4c49 4d49  e "CONTINUE_LIMI
-00000d50: 5420 3d22 2069 6e20 636f 6465 2066 6f72  T =" in code for
-00000d60: 2064 6574 6169 6c73 3c2f 7370 616e 3e7a   details</span>z
-00000d70: 0741 6374 696f 6e20 7a10 3a20 6e6f 7420  .Action z.: not 
-00000d80: 7965 7420 6d61 7070 6564 2909 7208 0000  yet mapped).r...
-00000d90: 0072 0600 0000 da04 6669 6e64 da03 6c65  .r......find..le
-00000da0: 6eda 0661 7070 656e 64da 0573 706c 6974  n..append..split
-00000db0: 7202 0000 00da 0373 7472 722a 0000 0029  r......strr*...)
-00000dc0: 0a5a 0561 6c69 7374 5a05 7463 6f64 655a  .Z.alistZ.tcodeZ
-00000dd0: 0c63 6f64 655f 656c 656d 656e 74da 0669  .code_element..i
-00000de0: 6e64 656e 745a 0a69 6e64 656e 745f 616d  ndentZ.indent_am
-00000df0: 74da 0563 6f75 6e74 da07 6e65 776c 696e  t..count..newlin
-00000e00: 655a 0974 636f 6465 5f6c 656e 5a0e 6172  eZ.tcode_lenZ.ar
-00000e10: 7261 795f 6f66 5f6c 696e 6573 7217 0000  ray_of_linesr...
-00000e20: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000e30: da0c 6275 696c 645f 6163 7469 6f6e b100  ..build_action..
-00000e40: 0000 733e 0000 0004 0208 011e 0104 0208  ..s>............
-00000e50: 0108 0108 030a 0108 0110 030a 0104 150a  ................
-00000e60: ed04 0108 0108 010c 0110 0208 0108 0204  ................
-00000e70: 0202 0106 0106 ff04 ff02 0504 0302 f604  ................
-00000e80: 0a14 ff04 0172 3a00 0000 291d 722c 0000  .....r:...).r,..
-00000e90: 00da 0272 65da 1578 6d6c 2e65 7472 6565  ...re..xml.etree
-00000ea0: 2e45 6c65 6d65 6e74 5472 6565 da03 786d  .ElementTree..xm
-00000eb0: 6c5a 156d 6170 7461 736b 6572 2e73 7263  lZ.maptasker.src
-00000ec0: 2e61 6374 696f 6e72 da03 7372 635a 0761  .actionr..srcZ.a
-00000ed0: 6374 696f 6e72 722b 0000 005a 146d 6170  ctionrr+...Z.map
-00000ee0: 7461 736b 6572 2e73 7263 2e63 6f6e 6669  tasker.src.confi
-00000ef0: 6772 0200 0000 5a14 6d61 7074 6173 6b65  gr....Z.maptaske
-00000f00: 722e 7372 632e 6163 7469 6f6e 7203 0000  r.src.actionr...
-00000f10: 005a 156d 6170 7461 736b 6572 2e73 7263  .Z.maptasker.src
-00000f20: 2e61 6374 696f 6e63 7204 0000 00da 166d  .actioncr......m
-00000f30: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
-00000f40: 636f 6e73 7472 0500 0000 7206 0000 00da  constr....r.....
-00000f50: 0763 6f6d 7069 6c65 7209 0000 0072 0e00  .compiler....r..
-00000f60: 0000 721a 0000 0072 1f00 0000 da05 6574  ..r....r......et
-00000f70: 7265 65da 0b45 6c65 6d65 6e74 5472 6565  ree..ElementTree
-00000f80: da04 626f 6f6c da04 6469 6374 7236 0000  ..bool..dictr6..
-00000f90: 0072 2e00 0000 723a 0000 0072 0c00 0000  .r....r:...r....
-00000fa0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000fb0: 083c 6d6f 6475 6c65 3e01 0000 0073 3a00  .<module>....s:.
-00000fc0: 0000 080c 0801 0801 1202 0c01 0c01 0c01  ................
-00000fd0: 0c01 0c01 0a02 0807 0817 0817 020e 0601  ................
-00000fe0: 02ff 0602 02fe 0203 02fd 0204 02fc 0205  ................
-00000ff0: 02fb 0206 02fa 0207 0af9 0c56            ...........V
+000000f0: 2919 e900 0000 004e 2901 da0f 6765 745f  )......N)...get_
+00000100: 6578 7472 615f 7374 7566 6629 01da 0b66  extra_stuff)...f
+00000110: 6f72 6d61 745f 6874 6d6c 2901 da0c 6163  ormat_html)...ac
+00000120: 7469 6f6e 5f63 6f64 6573 2901 da06 6c6f  tion_codes)...lo
+00000130: 6767 6572 2901 da0b 464f 4e54 5f54 4f5f  gger)...FONT_TO_
+00000140: 5553 457a 062c 5b2c 205d 2b63 0100 0000  USEz.,[, ]+c....
+00000150: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000160: 4300 0000 7394 0000 007c 00a0 0064 0164  C...s....|...d.d
+00000170: 02a1 027d 007c 00a0 0064 0364 04a1 027d  ...}.|...d.d...}
+00000180: 0074 01a0 0264 057c 00a1 027d 007c 00a0  .t...d.|...}.|..
+00000190: 0064 0664 07a1 027d 007c 00a0 0064 0864  .d.d...}.|...d.d
+000001a0: 09a1 027d 007c 00a0 0064 0a64 04a1 027d  ...}.|...d.d...}
+000001b0: 007c 00a0 0064 0b64 04a1 027d 007c 00a0  .|...d.d...}.|..
+000001c0: 0064 0c64 04a1 027d 007c 00a0 0064 0d64  .d.d...}.|...d.d
+000001d0: 04a1 027d 007c 00a0 0064 0e64 04a1 027d  ...}.|...d.d...}
+000001e0: 007c 00a0 0064 0f64 04a1 027d 007c 00a0  .|...d.d...}.|..
+000001f0: 0064 1064 11a1 027d 007c 0053 0029 124e  .d.d...}.|.S.).N
+00000200: 7a09 2c20 203c 666f 6e74 3e7a 063c 666f  z.,  <font>z.<fo
+00000210: 6e74 3e7a 032c 2028 da00 7a02 2c20 7a07  nt>z., (..z., z.
+00000220: 2c20 3c73 7061 6e7a 053c 7370 616e 7a08  , <spanz.<spanz.
+00000230: 2c20 203c 7370 616e 7a07 2020 3c73 7061  ,  <spanz.  <spa
+00000240: 6e7a 072c 2063 6f64 653a 7a05 3c62 6967  nz., code:z.<big
+00000250: 3e7a 073c 736d 616c 6c3e 7a04 3c74 743e  >z.<small>z.<tt>
+00000260: 7a03 3c69 3e7a 033c 753e 7a07 2c20 3c66  z.<i>z.<u>z., <f
+00000270: 6f6e 747a 053c 666f 6e74 2903 da07 7265  ontz.<font)...re
+00000280: 706c 6163 65da 0770 6174 7465 726e da03  place..pattern..
+00000290: 7375 6229 01da 0772 6573 756c 7473 a900  sub)...results..
+000002a0: 720c 0000 00fa 762f 5573 6572 732f 6d69  r.....v/Users/mi
+000002b0: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
+000002c0: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
+000002d0: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
+000002e0: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
+000002f0: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
+00000300: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
+00000310: 7263 2f61 6374 696f 6e65 2e70 79da 1263  rc/actione.py..c
+00000320: 6c65 616e 7570 5f74 6865 5f72 6573 756c  leanup_the_resul
+00000330: 7422 0000 0073 1e00 0000 0403 0401 04ff  t"...s..........
+00000340: 0c03 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000350: 0c01 0c01 0c01 0401 720e 0000 0063 0000  ........r....c..
+00000360: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+00000370: 0000 4300 0000 739c 0000 0064 017d 0074  ..C...s....d.}.t
+00000380: 0044 005d 3f7d 0174 007c 0119 007d 027c  .D.]?}.t.|...}.|
+00000390: 0264 0219 007d 037c 0364 036b 0472 2a64  .d...}.|.d.k.r*d
+000003a0: 047c 0276 0172 2a64 057c 019b 0064 067c  .|.v.r*d.|...d.|
+000003b0: 039b 009d 047d 0474 017c 0483 0101 0074  .....}.t.|.....t
+000003c0: 02a0 037c 049b 00a1 0101 0064 077d 0064  ...|.......d.}.d
+000003d0: 087c 0276 0172 4364 057c 019b 0064 099d  .|.v.rCd.|...d..
+000003e0: 037d 0474 017c 0483 0101 0074 02a0 037c  .}.t.|.....t...|
+000003f0: 04a1 0101 0064 0a7c 0264 083c 0064 077d  .....d.|.d.<.d.}
+00000400: 0071 047c 0072 4c74 0464 0b83 0101 0064  .q.|.rLt.d.....d
+00000410: 0053 0064 0053 0029 0c4e 46da 076e 756d  .S.d.S.).NF..num
+00000420: 6172 6773 7201 0000 00da 0772 6571 6172  argsr......reqar
+00000430: 6773 7a11 4572 726f 723a 2064 6963 745f  gsz.Error: dict_
+00000440: 636f 6465 207a 1b20 6d69 7373 696e 6720  code z. missing 
+00000450: 7265 7161 7267 7321 2020 6e75 6d61 7267  reqargs!  numarg
+00000460: 733a 54da 0764 6973 706c 6179 7a13 206d  s:T..displayz. m
+00000470: 6973 7369 6e67 2022 6469 7370 6c61 7922  issing "display"
+00000480: 215a 0875 6e6d 6170 7065 64e9 6300 0000  !Z.unmapped.c...
+00000490: 2905 7204 0000 00da 0570 7269 6e74 7205  ).r......printr.
+000004a0: 0000 00da 0564 6562 7567 da04 6578 6974  .....debug..exit
+000004b0: 2905 da04 666c 6167 da04 6974 656d da05  )...flag..item..
+000004c0: 656e 7472 7972 0f00 0000 da09 6572 726f  entryr......erro
+000004d0: 725f 6d73 6772 0c00 0000 720c 0000 0072  r_msgr....r....r
+000004e0: 0d00 0000 da14 6c6f 6f6b 5f66 6f72 5f6d  ......look_for_m
+000004f0: 6973 7369 6e67 5f72 6571 3900 0000 7326  issing_req9...s&
+00000500: 0000 0004 0108 0108 0108 0110 0110 0108  ................
+00000510: 010c 0104 0108 010c 0108 010a 0108 0104  ................
+00000520: 0102 8004 010c 0104 ff72 1a00 0000 6301  .........r....c.
+00000530: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00000540: 0000 0043 0000 0073 4400 0000 6401 6402  ...C...sD...d.d.
+00000550: 6c00 6d01 7d01 0100 7c00 6400 6403 8502  l.m.}...|.d.d...
+00000560: 1900 7d02 7c02 7c01 7600 7220 7c00 7402  ..}.|.|.v.r |.t.
+00000570: 7600 7220 6404 7402 7c00 1900 6404 1900  v.r d.t.|...d...
+00000580: 6405 1700 6901 7402 7c00 3c00 6400 5300  d...i.t.|.<.d.S.
+00000590: 2906 4e72 0100 0000 2901 da0a 6465 7072  ).Nr....)...depr
+000005a0: 6963 6174 6564 e9ff ffff ff72 1100 0000  icated.....r....
+000005b0: 7a1a 3c65 6d3e 2028 4973 2044 6570 7265  z.<em> (Is Depre
+000005c0: 6361 7465 6429 3c2f 656d 3e20 2903 5a18  cated)</em> ).Z.
+000005d0: 6d61 7074 6173 6b65 722e 7372 632e 6465  maptasker.src.de
+000005e0: 7072 6963 6174 6564 721b 0000 0072 0400  pricatedr....r..
+000005f0: 0000 2903 da09 6469 6374 5f63 6f64 6572  ..)...dict_coder
+00000600: 1b00 0000 da06 6c6f 6f6b 7570 720c 0000  ......lookupr...
+00000610: 0072 0c00 0000 720d 0000 00da 1563 6865  .r....r......che
+00000620: 636b 5f66 6f72 5f64 6570 7265 6361 7469  ck_for_deprecati
+00000630: 6f6e 5000 0000 730c 0000 000c 010c 0210  onP...s.........
+00000640: 0110 0208 ff04 0372 1f00 0000 da0a 636f  .......r......co
+00000650: 6465 5f63 6869 6c64 da0b 636f 6465 5f61  de_child..code_a
+00000660: 6374 696f 6eda 0b61 6374 696f 6e5f 7479  ction..action_ty
+00000670: 7065 da08 636f 6c6f 726d 6170 da09 636f  pe..colormap..co
+00000680: 6465 5f74 7970 65da 0c70 726f 6772 616d  de_type..program
+00000690: 5f61 7267 73da 0672 6574 7572 6e63 0600  _args..returnc..
+000006a0: 0000 0000 0000 0000 0000 0c00 0000 0a00  ................
+000006b0: 0000 4300 0000 7358 0100 0074 00a0 0164  ..C...sX...t...d
+000006c0: 017c 006a 029b 007c 049b 009d 03a1 0101  .|.j...|........
+000006d0: 007c 006a 027c 0417 007d 0674 037c 0683  .|.j.|...}.t.|..
+000006e0: 0101 007c 0674 0476 0173 1e64 0274 047c  ...|.t.v.s.d.t.|
+000006f0: 0619 0076 0172 3564 037c 069b 0064 0474  ...v.r5d.|...d.t
+00000700: 057c 017c 027c 037c 0583 049b 009d 047d  .|.|.|.|.......}
+00000710: 0774 00a0 0164 057c 069b 0064 069d 03a1  .t...d.|...d....
+00000720: 0101 006e 7174 067c 0364 0764 0874 047c  ...nqt.|.d.d.t.|
+00000730: 0619 0064 0219 0064 0983 057d 0764 0a74  ...d...d...}.d.t
+00000740: 047c 0619 0076 0072 4e74 047c 0619 0064  .|...v.rNt.|...d
+00000750: 0a19 007d 086e 0264 0b7d 087c 0864 0b6b  ...}.n.d.}.|.d.k
+00000760: 0372 6e64 0c74 047c 0619 0076 0072 6e74  .rnd.t.|...v.rnt
+00000770: 07a0 087c 0674 047c 017c 027c 0374 047c  ...|.t.|.|.|.t.|
+00000780: 0619 0064 0c19 0074 047c 0619 0064 0d19  ...d...t.|...d..
+00000790: 007c 05a1 087d 0764 0e74 047c 0619 0076  .|...}.d.t.|...v
+000007a0: 0072 a674 047c 0619 0064 0e19 0064 0b19  .r.t.|...d...d..
+000007b0: 007d 097c 0674 09a0 0a74 047c 0919 00a1  .}.|.t...t.|....
+000007c0: 0169 017d 0a74 047c 0619 0064 0219 007d  .i.}.t.|...d...}
+000007d0: 0b74 09a0 0a7c 0ba1 017c 0a64 023c 0074  .t...|...|.d.<.t
+000007e0: 07a0 087c 067c 0a7c 017c 027c 037c 0a7c  ...|.|.|.|.|.|.|
+000007f0: 0619 0064 0c19 007c 0a7c 0619 0064 0d19  ...d...|.|...d..
+00000800: 007c 05a1 087d 0774 0b7c 0783 017d 077c  .|...}.t.|...}.|
+00000810: 0753 0029 0f61 9501 0000 0a20 2020 2047  .S.).a.....    G
+00000820: 6976 656e 2061 6e20 6163 7469 6f6e 2063  iven an action c
+00000830: 6f64 652c 2065 7661 6c75 6174 6520 6974  ode, evaluate it
+00000840: 2066 6f72 2064 6973 706c 6179 0a20 2020   for display.   
+00000850: 2020 2020 203a 7061 7261 6d20 636f 6465       :param code
+00000860: 5f63 6869 6c64 3a20 786d 6c20 656c 656d  _child: xml elem
+00000870: 656e 7420 6f66 2074 6865 203c 636f 6465  ent of the <code
+00000880: 3e0a 2020 2020 2020 2020 3a70 6172 616d  >.        :param
+00000890: 2063 6f64 655f 6163 7469 6f6e 3a20 7661   code_action: va
+000008a0: 6c75 6520 6f66 203c 636f 6465 3e20 2865  lue of <code> (e
+000008b0: 2e67 2e20 2235 3439 2229 0a20 2020 2020  .g. "549").     
+000008c0: 2020 203a 7061 7261 6d20 6163 7469 6f6e     :param action
+000008d0: 5f74 7970 653a 0a20 2020 2020 2020 203a  _type:.        :
+000008e0: 7061 7261 6d20 636f 6c6f 726d 6170 3a20  param colormap: 
+000008f0: 636f 6c6f 7273 2074 6f20 7573 6520 696e  colors to use in
+00000900: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
+00000910: 3a70 6172 616d 2063 6f64 655f 7479 7065  :param code_type
+00000920: 3a20 2765 273d 6576 656e 742c 2027 7327  : 'e'=event, 's'
+00000930: 3d73 7461 7465 2c20 2774 273d 7461 736b  =state, 't'=task
+00000940: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000950: 7072 6f67 7261 6d5f 6172 6773 3a20 7275  program_args: ru
+00000960: 6e74 696d 6520 6172 6775 6d65 6e74 730a  ntime arguments.
+00000970: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00000980: 2066 6f72 6d61 7474 6564 206f 7574 7075   formatted outpu
+00000990: 7420 6c69 6e65 2077 6974 6820 6163 7469  t line with acti
+000009a0: 6f6e 2064 6574 6169 6c73 0a20 2020 207a  on details.    z
+000009b0: 0867 6574 636f 6465 3a72 1100 0000 7a05  .getcode:r....z.
+000009c0: 436f 6465 207a 0f20 6e6f 7420 7965 7420  Code z. not yet 
+000009d0: 6d61 7070 6564 7a14 756e 6d61 7070 6564  mappedz.unmapped
+000009e0: 2074 6173 6b20 636f 6465 3a20 fa01 205a   task code: .. Z
+000009f0: 1161 6374 696f 6e5f 6e61 6d65 5f63 6f6c  .action_name_col
+00000a00: 6f72 7207 0000 0054 720f 0000 0072 0100  orr....Tr....r..
+00000a10: 0000 7210 0000 005a 0865 7661 6c61 7267  ..r....Z.evalarg
+00000a20: 735a 0872 6564 6972 6563 7429 0c72 0500  sZ.redirect).r..
+00000a30: 0000 7214 0000 00da 0474 6578 7472 1f00  ..r......textr..
+00000a40: 0000 7204 0000 0072 0200 0000 7203 0000  ..r....r....r...
+00000a50: 00da 0e61 6374 696f 6e5f 7265 7375 6c74  ...action_result
+00000a60: 735a 1267 6574 5f61 6374 696f 6e5f 7265  sZ.get_action_re
+00000a70: 7375 6c74 73da 0463 6f70 79da 0864 6565  sults..copy..dee
+00000a80: 7063 6f70 7972 0e00 0000 290c 7220 0000  pcopyr....).r ..
+00000a90: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
+00000aa0: 7224 0000 0072 2500 0000 721d 0000 005a  r$...r%...r....Z
+00000ab0: 0a74 6865 5f72 6573 756c 7472 0f00 0000  .the_resultr....
+00000ac0: 5a08 7265 6665 7272 616c 5a11 7465 6d70  Z.referralZ.temp
+00000ad0: 5f6c 6f6f 6b75 705f 636f 6465 735a 0c64  _lookup_codesZ.d
+00000ae0: 6973 706c 6179 5f6e 616d 6572 0c00 0000  isplay_namer....
+00000af0: 720c 0000 0072 0d00 0000 da0f 6765 745f  r....r......get_
+00000b00: 6163 7469 6f6e 5f63 6f64 655e 0000 0073  action_code^...s
+00000b10: 5e00 0000 1612 0a01 0802 1402 0802 0c01  ^...............
+00000b20: 04ff 02ff 1404 0204 1201 04ff 0c04 0e01  ................
+00000b30: 0402 1402 0401 0201 0201 0201 0201 0201  ................
+00000b40: 0a01 0a01 0201 04f8 0c0c 0a01 0201 04ff  ................
+00000b50: 1203 0601 0201 04ff 0e03 0402 0201 0201  ................
+00000b60: 0201 0201 0201 0a01 0a01 0201 04f8 080b  ................
+00000b70: 0401 722c 0000 0063 0600 0000 0000 0000  ..r,...c........
+00000b80: 0000 0000 0c00 0000 0a00 0000 4300 0000  ............C...
+00000b90: 7312 0100 0064 0164 026c 006d 017d 0601  s....d.d.l.m.}..
+00000ba0: 007c 047d 077c 0764 016b 0372 1d7c 02a0  .|.}.|.d.k.r.|..
+00000bb0: 0274 039b 0064 039d 0274 039b 0064 037c  .t...d...t...d.|
+00000bc0: 059b 009d 0364 04a1 037d 0264 017d 077c  .....d...}.d.}.|
+00000bd0: 0764 016b 0072 257c 057c 0217 007d 027c  .d.k.r%|.|...}.|
+00000be0: 0264 056b 0372 7d7c 02a0 0464 06a1 017d  .d.k.r}|...d...}
+00000bf0: 0874 057c 0283 017d 097c 0864 076b 0272  .t.|...}.|.d.k.r
+00000c00: 417c 0964 086b 0472 417c 01a0 067c 02a1  A|.d.k.rA|...|..
+00000c10: 0101 0064 0053 007c 02a0 0764 06a1 017d  ...d.S.|...d...}
+00000c20: 0a64 017d 077c 0a44 005d 307d 0b7c 0764  .d.}.|.D.]0}.|.d
+00000c30: 016b 0272 567c 01a0 067c 0ba1 0101 006e  .k.rV|...|.....n
+00000c40: 087c 01a0 0664 097c 0b9b 009d 02a1 0101  .|...d.|........
+00000c50: 007c 0764 0437 007d 077c 077c 066b 0272  .|.d.7.}.|.|.k.r
+00000c60: 7a7c 01a0 0674 087c 0064 0a64 0564 0b74  z|...t.|.d.d.d.t
+00000c70: 097c 0683 019b 0064 0c9d 0364 0d83 05a1  .|.....d...d....
+00000c80: 0101 0001 0064 0053 0071 4a64 0053 007c  .....d.S.qJd.S.|
+00000c90: 01a0 0664 0e7c 036a 0a9b 0064 0f9d 03a1  ...d.|.j...d....
+00000ca0: 0101 0064 0053 0029 104e 7201 0000 0029  ...d.S.).Nr....)
+00000cb0: 01da 0e43 4f4e 5449 4e55 455f 4c49 4d49  ...CONTINUE_LIMI
+00000cc0: 547a 0222 3ee9 0100 0000 7207 0000 00da  Tz.">.....r.....
+00000cd0: 010a 721c 0000 00e9 5000 0000 7a03 2e2e  ..r.....P...z...
+00000ce0: 2e5a 0352 6564 7a17 202e 2e2e 2063 6f6e  .Z.Redz. ... con
+00000cf0: 7469 6e75 6520 6c69 6d69 7420 6f66 207a  tinue limit of z
+00000d00: 3a20 7265 6163 6865 642e 2020 5365 6520  : reached.  See 
+00000d10: 2243 4f4e 5449 4e55 455f 4c49 4d49 5420  "CONTINUE_LIMIT 
+00000d20: 3d22 2069 6e20 636f 6e66 6967 2e70 7920  =" in config.py 
+00000d30: 666f 7220 6465 7461 696c 7354 7a07 4163  for detailsTz.Ac
+00000d40: 7469 6f6e 207a 103a 206e 6f74 2079 6574  tion z.: not yet
+00000d50: 206d 6170 7065 6429 0b5a 146d 6170 7461   mapped).Z.mapta
+00000d60: 736b 6572 2e73 7263 2e63 6f6e 6669 6772  sker.src.configr
+00000d70: 2d00 0000 7208 0000 0072 0600 0000 da04  -...r....r......
+00000d80: 6669 6e64 da03 6c65 6eda 0661 7070 656e  find..len..appen
+00000d90: 64da 0573 706c 6974 7203 0000 00da 0373  d..splitr......s
+00000da0: 7472 7228 0000 0029 0c72 2300 0000 5a05  trr(...).r#...Z.
+00000db0: 616c 6973 745a 0574 636f 6465 5a0c 636f  alistZ.tcodeZ.co
+00000dc0: 6465 5f65 6c65 6d65 6e74 da06 696e 6465  de_element..inde
+00000dd0: 6e74 5a0a 696e 6465 6e74 5f61 6d74 722d  ntZ.indent_amtr-
+00000de0: 0000 00da 0563 6f75 6e74 da07 6e65 776c  .....count..newl
+00000df0: 696e 655a 0974 636f 6465 5f6c 656e 5a0e  ineZ.tcode_lenZ.
+00000e00: 6172 7261 795f 6f66 5f6c 696e 6573 7217  array_of_linesr.
+00000e10: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000e20: 0000 da0c 6275 696c 645f 6163 7469 6f6e  ....build_action
+00000e30: b000 0000 7348 0000 000c 0104 0308 011e  ....sH..........
+00000e40: 0104 0108 0108 0108 030a 0108 0110 030a  ................
+00000e50: 0104 1c0a e604 0108 0108 010c 0110 0208  ................
+00000e60: 0108 0204 0102 0102 0102 0102 010e 0202  ................
+00000e70: 0402 f704 ff02 0d04 0302 ef04 1114 ff04  ................
+00000e80: 0172 3900 0000 291d 722a 0000 00da 0272  .r9...).r*.....r
+00000e90: 65da 1664 6566 7573 6564 786d 6c2e 456c  e..defusedxml.El
+00000ea0: 656d 656e 7454 7265 65da 0a64 6566 7573  ementTree..defus
+00000eb0: 6564 786d 6c5a 156d 6170 7461 736b 6572  edxmlZ.maptasker
+00000ec0: 2e73 7263 2e61 6374 696f 6e72 da03 7372  .src.actionr..sr
+00000ed0: 635a 0761 6374 696f 6e72 7229 0000 005a  cZ.actionrr)...Z
+00000ee0: 146d 6170 7461 736b 6572 2e73 7263 2e61  .maptasker.src.a
+00000ef0: 6374 696f 6e72 0200 0000 5a16 6d61 7074  ctionr....Z.mapt
+00000f00: 6173 6b65 722e 7372 632e 6672 6d74 6874  asker.src.frmtht
+00000f10: 6d6c 7203 0000 005a 156d 6170 7461 736b  mlr....Z.maptask
+00000f20: 6572 2e73 7263 2e61 6374 696f 6e63 7204  er.src.actioncr.
+00000f30: 0000 00da 166d 6170 7461 736b 6572 2e73  .....maptasker.s
+00000f40: 7263 2e73 7973 636f 6e73 7472 0500 0000  rc.sysconstr....
+00000f50: 7206 0000 00da 0763 6f6d 7069 6c65 7209  r......compiler.
+00000f60: 0000 0072 0e00 0000 721a 0000 0072 1f00  ...r....r....r..
+00000f70: 0000 da0b 456c 656d 656e 7454 7265 65da  ....ElementTree.
+00000f80: 0358 4d4c da04 626f 6f6c da04 6469 6374  .XML..bool..dict
+00000f90: 7235 0000 0072 2c00 0000 7239 0000 0072  r5...r,...r9...r
+00000fa0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+00000fb0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000fc0: 0073 3a00 0000 080c 0801 0801 1202 0c02  .s:.............
+00000fd0: 0c01 0c01 0c01 0c01 0a02 0809 0817 0817  ................
+00000fe0: 020e 0601 02ff 0602 02fe 0203 02fd 0204  ................
+00000ff0: 02fc 0205 02fb 0206 02fa 0207 0af9 0c52  ...............R
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/actionr.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/actionr.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar 31 16:38:58 2023 UTC, .py size: 7541 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,195 +1,187 @@
-00000000: 6f0d 0d0a 0000 0000 a20c 2764 751d 0000  o.........'du...
+00000000: 6f0d 0d0a 0000 0000 b73c 3864 541c 0000  o........<8dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0014 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c03 6d04 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
+00000020: 0014 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6401 6c03 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 0200 0100 6d07 5a08 0100 6400 6403  m.....m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0d 6d0e 5a0e 0100  Z...d.d.l.m.Z...
 00000080: 6400 6406 6c0f 6d10 5a10 0100 6400 6407  d.d.l.m.Z...d.d.
-00000090: 6c0f 6d11 5a11 0100 6408 6512 6409 6513  l.m.Z...d.e.d.e.
-000000a0: 6604 640a 640b 8404 5a14 640c 6502 6a15  f.d.d...Z.d.e.j.
-000000b0: 6a16 640d 6517 640e 6502 6a15 6a16 640f  j.d.e.d.e.j.j.d.
-000000c0: 6518 6410 6512 6411 6512 6412 6512 6413  e.d.e.d.e.d.e.d.
-000000d0: 6517 6408 6512 6409 6519 6614 6414 6415  e.d.e.d.e.f.d.d.
-000000e0: 8404 5a1a 640c 6513 6412 6502 6a15 6a16  ..Z.d.e.d.e.j.j.
-000000f0: 640e 6502 6a15 6a16 640f 6518 6410 6502  d.e.j.j.d.e.d.e.
-00000100: 6a15 6a16 640d 6517 6513 1900 6413 6517  j.j.d.e.e...d.e.
-00000110: 6513 1900 6411 6502 6a15 6a16 6409 6513  e...d.e.j.j.d.e.
-00000120: 6612 6416 6417 8404 5a1b 6401 5300 2918  f.d.d...Z.d.S.).
-00000130: e900 0000 004e 2901 da0b 6465 6661 756c  .....N)...defaul
-00000140: 7464 6963 7429 01da 0b61 6374 696f 6e5f  tdict)...action_
-00000150: 6172 6773 2901 da0c 6163 7469 6f6e 5f63  args)...action_c
-00000160: 6f64 6573 2901 da06 6c6f 6767 6572 2901  odes)...logger).
-00000170: da1d 6765 745f 786d 6c5f 696e 745f 6172  ..get_xml_int_ar
-00000180: 6775 6d65 6e74 5f74 6f5f 7661 6c75 6529  gument_to_value)
-00000190: 01da 1d67 6574 5f78 6d6c 5f73 7472 5f61  ...get_xml_str_a
-000001a0: 7267 756d 656e 745f 746f 5f76 616c 7565  rgument_to_value
-000001b0: da11 6576 616c 7561 7465 645f 7265 7375  ..evaluated_resu
-000001c0: 6c74 73da 0672 6574 7572 6e63 0100 0000  lts..returnc....
-000001d0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-000001e0: 4300 0000 7356 0100 0064 017d 017c 0064  C...sV...d.}.|.d
-000001f0: 0219 0044 005d a27d 0264 017d 037c 0204  ...D.].}.d.}.|..
-00000200: 0064 036b 0272 2201 007c 0064 0419 0072  .d.k.r"..|.d...r
-00000210: 217c 0064 0419 0064 0519 007d 037c 0064  !|.d...d...}.|.d
-00000220: 0419 00a0 0064 05a1 0101 006e 7f04 0064  .....d.....n...d
-00000230: 066b 0272 3901 007c 0064 0719 0072 387c  .k.r9..|.d...r8|
-00000240: 0064 0719 0064 0519 007d 037c 0064 0719  .d...d...}.|.d..
-00000250: 00a0 0064 05a1 0101 006e 6804 0064 086b  ...d.....nh..d.k
-00000260: 0272 5001 007c 0064 0919 0072 4f7c 0064  .rP..|.d...rO|.d
-00000270: 0919 0064 0519 007d 037c 0064 0919 00a0  ...d...}.|.d....
-00000280: 0064 05a1 0101 006e 5104 0064 0a6b 0272  .d.....nQ..d.k.r
-00000290: 6701 007c 0064 0b19 0072 667c 0064 0b19  g..|.d...rf|.d..
-000002a0: 0064 0519 007d 037c 0064 0b19 00a0 0064  .d...}.|.d.....d
-000002b0: 05a1 0101 006e 3a04 0064 0c6b 0272 7e01  .....n:..d.k.r~.
-000002c0: 007c 0064 0d19 0072 7d7c 0064 0d19 0064  .|.d...r}|.d...d
-000002d0: 0519 007d 037c 0064 0d19 00a0 0064 05a1  ...}.|.d.....d..
-000002e0: 0101 006e 2364 0e6b 0272 937c 0064 0f19  ...n#d.k.r.|.d..
-000002f0: 0072 927c 0064 0f19 0064 0519 007d 037c  .r.|.d...d...}.|
-00000300: 0064 0f19 00a0 0064 05a1 0101 006e 0e09  .d.....d.....n..
-00000310: 0074 01a0 0264 107c 029b 009d 02a1 0101  .t...d.|........
-00000320: 0074 03a0 0464 11a1 0101 007c 019b 0064  .t...d.....|...d
-00000330: 127c 039b 009d 037d 0171 067c 0153 0029  .|.....}.q.|.S.)
-00000340: 134e da00 5a11 706f 7369 7469 6f6e 5f61  .N..Z.position_a
-00000350: 7267 5f74 7970 655a 0353 7472 da0a 7265  rg_typeZ.Str..re
-00000360: 7375 6c74 5f73 7472 7201 0000 005a 0349  sult_strr....Z.I
-00000370: 6e74 da0a 7265 7375 6c74 5f69 6e74 5a03  nt..result_intZ.
-00000380: 4170 705a 0a72 6573 756c 745f 6170 705a  AppZ.result_appZ
-00000390: 0d43 6f6e 6469 7469 6f6e 4c69 7374 5a0a  .ConditionListZ.
-000003a0: 7265 7375 6c74 5f63 6f6e 5a03 496d 675a  result_conZ.ImgZ
-000003b0: 0a72 6573 756c 745f 696d 675a 0642 756e  .result_imgZ.Bun
-000003c0: 646c 655a 0a72 6573 756c 745f 6275 6e7a  dleZ.result_bunz
-000003d0: 3646 756e 6374 696f 6e20 6765 745f 7265  6Function get_re
-000003e0: 7375 6c74 735f 696e 5f61 7267 5f6f 7264  sults_in_arg_ord
-000003f0: 6572 3a20 6e6f 206d 6174 6368 2066 6f72  er: no match for
-00000400: 2022 6172 6722 3ae9 0800 0000 fa01 2029   "arg":....... )
-00000410: 05da 0370 6f70 7205 0000 00da 0564 6562  ...popr......deb
-00000420: 7567 da03 7379 73da 0465 7869 7429 0472  ug..sys..exit).r
-00000430: 0800 0000 5a0d 7265 7475 726e 5f72 6573  ....Z.return_res
-00000440: 756c 74da 0361 7267 5a08 7468 655f 6974  ult..argZ.the_it
-00000450: 656d a900 7214 0000 00fa 762f 5573 6572  em..r.....v/User
-00000460: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
-00000470: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
-00000480: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
-00000490: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
-000004a0: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
-000004b0: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
-000004c0: 6572 2f73 7263 2f61 6374 696f 6e72 2e70  er/src/actionr.p
-000004d0: 79da 1867 6574 5f72 6573 756c 7473 5f69  y..get_results_i
-000004e0: 6e5f 6172 675f 6f72 6465 721c 0000 0073  n_arg_order....s
-000004f0: 5600 0000 0401 0c01 0401 0201 0a01 0801  V...............
-00000500: 0c01 0801 0201 04ff 0280 0a03 0801 0c01  ................
-00000510: 0e01 0280 0a01 0801 0c01 0e01 0280 0a01  ................
-00000520: 0801 0c01 0e01 0280 0a01 0801 0c01 0e01  ................
-00000530: 0280 0601 0801 0c01 0e01 0280 0201 0401  ................
-00000540: 0801 04ff 0a03 1001 0401 7216 0000 00da  ..........r.....
-00000550: 0964 6963 745f 636f 6465 da08 6172 675f  .dict_code..arg_
-00000560: 6c69 7374 da0b 636f 6465 5f61 6374 696f  list..code_actio
-00000570: 6eda 0b61 6374 696f 6e5f 7479 7065 da08  n..action_type..
-00000580: 636f 6c6f 726d 6170 da0c 7072 6f67 7261  colormap..progra
-00000590: 6d5f 6172 6773 da11 6c6f 6f6b 7570 5f63  m_args..lookup_c
-000005a0: 6f64 655f 656e 7472 79da 0d65 7661 6c75  ode_entry..evalu
-000005b0: 6174 655f 6c69 7374 6309 0000 0000 0000  ate_listc.......
-000005c0: 0000 0000 0009 0000 000a 0000 0043 0000  .............C..
-000005d0: 0073 6400 0000 7400 7c01 7c00 7c06 7c07  .sd...t.|.|.|.|.
-000005e0: 7c02 7c03 7c04 7c05 7c08 8309 7d08 7c08  |.|.|.|.|...}.|.
-000005f0: 6401 1900 7230 7c08 6402 1900 7220 7401  d...r0|.d...r t.
-00000600: 7c02 7c08 6402 1900 7c08 6403 1900 8303  |.|.d...|.d.....
-00000610: 7c08 6404 3c00 7c08 6405 1900 7230 7402  |.d.<.|.d...r0t.
-00000620: 7c02 7c08 6405 1900 7c08 6406 1900 8303  |.|.d...|.d.....
-00000630: 7c08 6407 3c00 7c08 5300 2908 4e5a 0c67  |.d.<.|.S.).NZ.g
-00000640: 6574 5f78 6d6c 5f66 6c61 675a 0773 7472  et_xml_flagZ.str
-00000650: 6172 6773 5a07 7374 7265 7661 6c72 0b00  argsZ.strevalr..
-00000660: 0000 5a07 696e 7461 7267 735a 0769 6e74  ..Z.intargsZ.int
-00000670: 6576 616c 720c 0000 0029 0372 0300 0000  evalr....).r....
-00000680: 7207 0000 0072 0600 0000 2909 7217 0000  r....r....).r...
-00000690: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-000006a0: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-000006b0: 1e00 0000 7208 0000 0072 1400 0000 7214  ....r....r....r.
-000006c0: 0000 0072 1500 0000 da14 6576 616c 7561  ...r......evalua
-000006d0: 7465 5f61 6374 696f 6e5f 6172 6773 4800  te_action_argsH.
-000006e0: 0000 732a 0000 0002 0c02 0102 0102 0102  ..s*............
-000006f0: 0102 0102 0102 0102 0102 0104 f708 0c08  ................
-00000700: 0102 010e 0108 ff08 0302 010e 0108 ff04  ................
-00000710: 0472 1f00 0000 6308 0000 0000 0000 0000  .r....c.........
-00000720: 0000 000d 0000 000a 0000 0043 0000 0073  ...........C...s
-00000730: da00 0000 7400 6401 6402 8400 8301 7d08  ....t.d.d.....}.
-00000740: 6403 7d09 6404 7d0a 6405 7c00 7600 7312  d.}.d.}.d.|.v.s.
-00000750: 6406 7c00 7600 7217 6404 7d0b 6404 7d0c  d.|.v.r.d.}.d.}.
-00000760: 6e18 6407 7c04 6408 1900 1700 7c07 6409  n.d.|.d.....|.d.
-00000770: 1900 1700 640a 1700 7d0b 640b 7c04 640c  ....d...}.d.|.d.
-00000780: 1900 1700 7c07 6409 1900 1700 640a 1700  ....|.d.....d...
-00000790: 7d0c 7c05 7c01 7c00 1900 640d 3c00 7c06  }.|.|.|...d.<.|.
-000007a0: 7c01 7c00 1900 640e 3c00 7c05 724f 7c07  |.|...d.<.|.rO|.
-000007b0: 640f 1900 6410 6b03 724f 7401 7c00 7c05  d...d.k.rOt.|.|.
-000007c0: 7c02 7c03 7c04 7c07 7c01 7c06 7c08 8309  |.|.|.|.|.|.|...
-000007d0: 7d08 7c08 6411 1900 7257 7402 7c08 8301  }.|.d...rWt.|...
-000007e0: 7d0a 7c0b 7403 7c00 1900 6412 1900 1700  }.|.t.|...d.....
-000007f0: 7c0c 1700 7c09 1700 7c0a 1700 7404 a005  |...|...|...t...
-00000800: 7c02 7c03 7c04 7c07 a104 1700 5300 2913  |.|.|.|.....S.).
-00000810: 4e63 0000 0000 0000 0000 0000 0000 0000  Nc..............
-00000820: 0000 0100 0000 5300 0000 7304 0000 0067  ......S...s....g
-00000830: 0053 0029 014e 7214 0000 0072 1400 0000  .S.).Nr....r....
-00000840: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000850: 083c 6c61 6d62 6461 3e7c 0000 0073 0200  .<lambda>|...s..
-00000860: 0000 0400 7a24 6765 745f 6163 7469 6f6e  ....z$get_action
-00000870: 5f72 6573 756c 7473 2e3c 6c6f 6361 6c73  _results.<locals
-00000880: 3e2e 3c6c 616d 6264 613e 7a0c 266e 6273  >.<lambda>z.&nbs
-00000890: 703b 266e 6273 703b 720a 0000 00da 0173  p;&nbsp;r......s
-000008a0: da01 657a 133c 7370 616e 2073 7479 6c65  ..ez.<span style
-000008b0: 3d22 636f 6c6f 723a da11 6163 7469 6f6e  ="color:..action
-000008c0: 5f6e 616d 655f 636f 6c6f 72da 0b66 6f6e  _name_color..fon
-000008d0: 745f 746f 5f75 7365 fa01 3e7a 1a3c 2f73  t_to_use..>z.</s
-000008e0: 7061 6e3e 3c73 7061 6e20 7374 796c 653d  pan><span style=
-000008f0: 2263 6f6c 6f72 3ada 0c61 6374 696f 6e5f  "color:..action_
-00000900: 636f 6c6f 72da 0772 6571 6172 6773 da08  color..reqargs..
-00000910: 6576 616c 6172 6773 5a14 6469 7370 6c61  evalargsZ.displa
-00000920: 795f 6465 7461 696c 5f6c 6576 656c e902  y_detail_level..
-00000930: 0000 005a 1372 6574 7572 6e69 6e67 5f73  ...Z.returning_s
-00000940: 6f6d 6574 6869 6e67 da07 6469 7370 6c61  omething..displa
-00000950: 7929 0672 0200 0000 721f 0000 0072 1600  y).r....r....r..
-00000960: 0000 7204 0000 00da 0a67 6574 5f61 6374  ..r......get_act
-00000970: 696f 6eda 0f67 6574 5f65 7874 7261 5f73  ion..get_extra_s
-00000980: 7475 6666 290d 7217 0000 0072 1d00 0000  tuff).r....r....
-00000990: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000009a0: 1800 0000 721e 0000 0072 1c00 0000 7208  ....r....r....r.
-000009b0: 0000 005a 0a74 776f 5f62 6c61 6e6b 73da  ...Z.two_blanks.
-000009c0: 0672 6573 756c 745a 1264 6973 706c 6179  .resultZ.display
-000009d0: 5f6e 616d 655f 636f 6c6f 725a 1464 6973  _name_colorZ.dis
-000009e0: 706c 6179 5f64 6574 6169 6c5f 636f 6c6f  play_detail_colo
-000009f0: 7272 1400 0000 7214 0000 0072 1500 0000  rr....r....r....
-00000a00: da12 6765 745f 6163 7469 6f6e 5f72 6573  ..get_action_res
-00000a10: 756c 7473 7100 0000 7368 0000 0002 0a06  ultsq...sh......
-00000a20: 0104 ff04 0304 0110 0104 0106 0102 0306  ................
-00000a30: 0102 ff06 0202 fe02 0302 fd02 ff02 0706  ................
-00000a40: 0102 ff06 0202 fe02 0302 fd02 ff0c 090c  ................
-00000a50: 0110 0202 0202 0102 0102 0102 0102 0102  ................
-00000a60: 0102 0102 0102 0104 f708 0e08 0102 020a  ................
-00000a70: 0102 ff02 0202 fe02 0302 fd02 0402 fc0e  ................
-00000a80: 0502 fb02 ff72 2e00 0000 291c 7211 0000  .....r....).r...
-00000a90: 00da 1578 6d6c 2e65 7472 6565 2e45 6c65  ...xml.etree.Ele
-00000aa0: 6d65 6e74 5472 6565 da03 786d 6cda 0b63  mentTree..xml..c
-00000ab0: 6f6c 6c65 6374 696f 6e73 7202 0000 00da  ollectionsr.....
-00000ac0: 146d 6170 7461 736b 6572 2e73 7263 2e61  .maptasker.src.a
-00000ad0: 6374 696f 6eda 0373 7263 da06 6163 7469  ction..src..acti
-00000ae0: 6f6e 722b 0000 005a 156d 6170 7461 736b  onr+...Z.maptask
-00000af0: 6572 2e73 7263 2e61 6374 6172 6773 7203  er.src.actargsr.
-00000b00: 0000 00da 156d 6170 7461 736b 6572 2e73  .....maptasker.s
-00000b10: 7263 2e61 6374 696f 6e63 7204 0000 00da  rc.actioncr.....
-00000b20: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
-00000b30: 7973 636f 6e73 7472 0500 0000 5a15 6d61  ysconstr....Z.ma
-00000b40: 7074 6173 6b65 722e 7372 632e 786d 6c64  ptasker.src.xmld
-00000b50: 6174 6172 0600 0000 7207 0000 00da 0464  atar....r......d
-00000b60: 6963 74da 0373 7472 7216 0000 00da 0565  ict..strr......e
-00000b70: 7472 6565 da0b 456c 656d 656e 7454 7265  tree..ElementTre
-00000b80: 65da 046c 6973 74da 0462 6f6f 6cda 0574  e..list..bool..t
-00000b90: 7570 6c65 721f 0000 0072 2e00 0000 7214  upler....r....r.
-00000ba0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00000bb0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000bc0: 7364 0000 0008 0c08 010c 0112 020c 010c  sd..............
-00000bd0: 010c 010c 010c 0112 0602 2c06 0102 ff02  ..........,.....
-00000be0: 0202 fe06 0302 fd02 0402 fc02 0502 fb02  ................
-00000bf0: 0602 fa02 0702 f902 0802 f802 0902 f702  ................
-00000c00: 0a0a f602 2902 0102 ff06 0202 fe06 0302  ....)...........
-00000c10: fd02 0402 fc06 0502 fb06 0602 fa06 0702  ................
-00000c20: f906 0802 f802 090e f7                   .........
+00000090: 6c11 6d12 5a12 0100 6400 6408 6c11 6d13  l.m.Z...d.d.l.m.
+000000a0: 5a13 0100 6409 6514 640a 6515 6604 640b  Z...d.e.d.e.f.d.
+000000b0: 640c 8404 5a16 640d 6504 6a17 6a18 640e  d...Z.d.e.j.j.d.
+000000c0: 6519 640f 6504 6a17 6a18 6410 651a 6411  e.d.e.j.j.d.e.d.
+000000d0: 6514 6412 6514 6413 6514 6414 6519 6409  e.d.e.d.e.d.e.d.
+000000e0: 6514 640a 651b 6614 6415 6416 8404 5a1c  e.d.e.f.d.d...Z.
+000000f0: 640d 6515 6413 6504 6a17 6a18 640f 6504  d.e.d.e.j.j.d.e.
+00000100: 6a17 6a18 6410 651a 6411 6504 6a17 6a18  j.j.d.e.d.e.j.j.
+00000110: 640e 6519 6515 1900 6414 6519 6515 1900  d.e.e...d.e.e...
+00000120: 6412 6504 6a17 6a18 640a 6515 6612 6417  d.e.j.j.d.e.f.d.
+00000130: 6418 8404 5a1d 6401 5300 2919 e900 0000  d...Z.d.S.).....
+00000140: 004e 2901 da0b 6465 6661 756c 7464 6963  .N)...defaultdic
+00000150: 7429 01da 0b61 6374 696f 6e5f 6172 6773  t)...action_args
+00000160: 2901 da0c 6163 7469 6f6e 5f63 6f64 6573  )...action_codes
+00000170: 2901 da0b 666f 726d 6174 5f68 746d 6c29  )...format_html)
+00000180: 01da 066c 6f67 6765 7229 01da 1d67 6574  ...logger)...get
+00000190: 5f78 6d6c 5f69 6e74 5f61 7267 756d 656e  _xml_int_argumen
+000001a0: 745f 746f 5f76 616c 7565 2901 da1d 6765  t_to_value)...ge
+000001b0: 745f 786d 6c5f 7374 725f 6172 6775 6d65  t_xml_str_argume
+000001c0: 6e74 5f74 6f5f 7661 6c75 65da 1165 7661  nt_to_value..eva
+000001d0: 6c75 6174 6564 5f72 6573 756c 7473 da06  luated_results..
+000001e0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+000001f0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+00000200: 5601 0000 6401 7d01 7c00 6402 1900 4400  V...d.}.|.d...D.
+00000210: 5da2 7d02 6401 7d03 7c02 0400 6403 6b02  ].}.d.}.|...d.k.
+00000220: 7222 0100 7c00 6404 1900 7221 7c00 6404  r"..|.d...r!|.d.
+00000230: 1900 6405 1900 7d03 7c00 6404 1900 a000  ..d...}.|.d.....
+00000240: 6405 a101 0100 6e7f 0400 6406 6b02 7239  d.....n...d.k.r9
+00000250: 0100 7c00 6407 1900 7238 7c00 6407 1900  ..|.d...r8|.d...
+00000260: 6405 1900 7d03 7c00 6407 1900 a000 6405  d...}.|.d.....d.
+00000270: a101 0100 6e68 0400 6408 6b02 7250 0100  ....nh..d.k.rP..
+00000280: 7c00 6409 1900 724f 7c00 6409 1900 6405  |.d...rO|.d...d.
+00000290: 1900 7d03 7c00 6409 1900 a000 6405 a101  ..}.|.d.....d...
+000002a0: 0100 6e51 0400 640a 6b02 7267 0100 7c00  ..nQ..d.k.rg..|.
+000002b0: 640b 1900 7266 7c00 640b 1900 6405 1900  d...rf|.d...d...
+000002c0: 7d03 7c00 640b 1900 a000 6405 a101 0100  }.|.d.....d.....
+000002d0: 6e3a 0400 640c 6b02 727e 0100 7c00 640d  n:..d.k.r~..|.d.
+000002e0: 1900 727d 7c00 640d 1900 6405 1900 7d03  ..r}|.d...d...}.
+000002f0: 7c00 640d 1900 a000 6405 a101 0100 6e23  |.d.....d.....n#
+00000300: 640e 6b02 7293 7c00 640f 1900 7292 7c00  d.k.r.|.d...r.|.
+00000310: 640f 1900 6405 1900 7d03 7c00 640f 1900  d...d...}.|.d...
+00000320: a000 6405 a101 0100 6e0e 0900 7401 a002  ..d.....n...t...
+00000330: 6410 7c02 9b00 9d02 a101 0100 7403 a004  d.|.........t...
+00000340: 6411 a101 0100 7c01 9b00 6412 7c03 9b00  d.....|...d.|...
+00000350: 9d03 7d01 7106 7c01 5300 2913 4eda 005a  ..}.q.|.S.).N..Z
+00000360: 1170 6f73 6974 696f 6e5f 6172 675f 7479  .position_arg_ty
+00000370: 7065 5a03 5374 72da 0a72 6573 756c 745f  peZ.Str..result_
+00000380: 7374 7272 0100 0000 5a03 496e 74da 0a72  strr....Z.Int..r
+00000390: 6573 756c 745f 696e 745a 0341 7070 5a0a  esult_intZ.AppZ.
+000003a0: 7265 7375 6c74 5f61 7070 5a0d 436f 6e64  result_appZ.Cond
+000003b0: 6974 696f 6e4c 6973 745a 0a72 6573 756c  itionListZ.resul
+000003c0: 745f 636f 6e5a 0349 6d67 5a0a 7265 7375  t_conZ.ImgZ.resu
+000003d0: 6c74 5f69 6d67 5a06 4275 6e64 6c65 5a0a  lt_imgZ.BundleZ.
+000003e0: 7265 7375 6c74 5f62 756e 7a36 4675 6e63  result_bunz6Func
+000003f0: 7469 6f6e 2067 6574 5f72 6573 756c 7473  tion get_results
+00000400: 5f69 6e5f 6172 675f 6f72 6465 723a 206e  _in_arg_order: n
+00000410: 6f20 6d61 7463 6820 666f 7220 2261 7267  o match for "arg
+00000420: 223a e908 0000 00fa 0120 2905 da03 706f  ":....... )...po
+00000430: 7072 0600 0000 da05 6465 6275 67da 0373  pr......debug..s
+00000440: 7973 da04 6578 6974 2904 7209 0000 005a  ys..exit).r....Z
+00000450: 0d72 6574 7572 6e5f 7265 7375 6c74 da03  .return_result..
+00000460: 6172 675a 0874 6865 5f69 7465 6da9 0072  argZ.the_item..r
+00000470: 1500 0000 fa76 2f55 7365 7273 2f6d 696b  .....v/Users/mik
+00000480: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
+00000490: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
+000004a0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
+000004b0: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
+000004c0: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
+000004d0: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
+000004e0: 632f 6163 7469 6f6e 722e 7079 da18 6765  c/actionr.py..ge
+000004f0: 745f 7265 7375 6c74 735f 696e 5f61 7267  t_results_in_arg
+00000500: 5f6f 7264 6572 1e00 0000 7356 0000 0004  _order....sV....
+00000510: 010c 0104 0102 010a 0108 010c 0108 0102  ................
+00000520: 0104 ff02 800a 0308 010c 010e 0102 800a  ................
+00000530: 0108 010c 010e 0102 800a 0108 010c 010e  ................
+00000540: 0102 800a 0108 010c 010e 0102 8006 0108  ................
+00000550: 010c 010e 0102 8002 0104 0108 0104 ff0a  ................
+00000560: 0310 0104 0172 1700 0000 da09 6469 6374  .....r......dict
+00000570: 5f63 6f64 65da 0861 7267 5f6c 6973 74da  _code..arg_list.
+00000580: 0b63 6f64 655f 6163 7469 6f6e da0b 6163  .code_action..ac
+00000590: 7469 6f6e 5f74 7970 65da 0863 6f6c 6f72  tion_type..color
+000005a0: 6d61 70da 0c70 726f 6772 616d 5f61 7267  map..program_arg
+000005b0: 73da 116c 6f6f 6b75 705f 636f 6465 5f65  s..lookup_code_e
+000005c0: 6e74 7279 da0d 6576 616c 7561 7465 5f6c  ntry..evaluate_l
+000005d0: 6973 7463 0900 0000 0000 0000 0000 0000  istc............
+000005e0: 0900 0000 0a00 0000 4300 0000 7364 0000  ........C...sd..
+000005f0: 0074 007c 017c 007c 067c 077c 027c 037c  .t.|.|.|.|.|.|.|
+00000600: 047c 057c 0883 097d 087c 0864 0119 0072  .|.|...}.|.d...r
+00000610: 307c 0864 0219 0072 2074 017c 027c 0864  0|.d...r t.|.|.d
+00000620: 0219 007c 0864 0319 0083 037c 0864 043c  ...|.d.....|.d.<
+00000630: 007c 0864 0519 0072 3074 027c 027c 0864  .|.d...r0t.|.|.d
+00000640: 0519 007c 0864 0619 0083 037c 0864 073c  ...|.d.....|.d.<
+00000650: 007c 0853 0029 084e 5a0c 6765 745f 786d  .|.S.).NZ.get_xm
+00000660: 6c5f 666c 6167 5a07 7374 7261 7267 735a  l_flagZ.strargsZ
+00000670: 0773 7472 6576 616c 720c 0000 005a 0769  .strevalr....Z.i
+00000680: 6e74 6172 6773 5a07 696e 7465 7661 6c72  ntargsZ.intevalr
+00000690: 0d00 0000 2903 7203 0000 0072 0800 0000  ....).r....r....
+000006a0: 7207 0000 0029 0972 1800 0000 7219 0000  r....).r....r...
+000006b0: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+000006c0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+000006d0: 0900 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+000006e0: 0000 00da 1465 7661 6c75 6174 655f 6163  .....evaluate_ac
+000006f0: 7469 6f6e 5f61 7267 734a 0000 0073 2a00  tion_argsJ...s*.
+00000700: 0000 020c 0201 0201 0201 0201 0201 0201  ................
+00000710: 0201 0201 0201 04f7 080c 0801 0201 0e01  ................
+00000720: 08ff 0803 0201 0e01 08ff 0404 7220 0000  ............r ..
+00000730: 0063 0800 0000 0000 0000 0000 0000 0b00  .c..............
+00000740: 0000 0e00 0000 4300 0000 73a6 0000 0074  ......C...s....t
+00000750: 0064 0164 0284 0083 017d 0864 037d 0964  .d.d.....}.d.}.d
+00000760: 047d 0a7c 057c 017c 0019 0064 053c 007c  .}.|.|.|...d.<.|
+00000770: 067c 017c 0019 0064 063c 007c 0572 2a7c  .|.|...d.<.|.r*|
+00000780: 0764 0719 0064 086b 0372 2a74 017c 007c  .d...d.k.r*t.|.|
+00000790: 057c 027c 037c 047c 077c 017c 067c 0883  .|.|.|.|.|.|.|..
+000007a0: 097d 087c 0864 0919 0072 3274 027c 0883  .}.|.d...r2t.|..
+000007b0: 017d 0a74 037c 0464 0a64 0474 047c 0019  .}.t.|.d.d.t.|..
+000007c0: 0064 0b19 0064 0c83 0574 037c 0464 0d64  .d...d...t.|.d.d
+000007d0: 047c 099b 007c 0a9b 0064 0e74 05a0 067c  .|...|...d.t...|
+000007e0: 027c 037c 047c 07a1 049b 009d 0464 0f83  .|.|.|.......d..
+000007f0: 0517 0053 0029 104e 6300 0000 0000 0000  ...S.).Nc.......
+00000800: 0000 0000 0000 0000 0001 0000 0053 0000  .............S..
+00000810: 0073 0400 0000 6700 5300 2901 4e72 1500  .s....g.S.).Nr..
+00000820: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
+00000830: 0072 1600 0000 da08 3c6c 616d 6264 613e  .r......<lambda>
+00000840: 7e00 0000 7302 0000 0004 007a 2467 6574  ~...s......z$get
+00000850: 5f61 6374 696f 6e5f 7265 7375 6c74 732e  _action_results.
+00000860: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00000870: 3e7a 0c26 6e62 7370 3b26 6e62 7370 3b72  >z.&nbsp;&nbsp;r
+00000880: 0b00 0000 da07 7265 7161 7267 73da 0865  ......reqargs..e
+00000890: 7661 6c61 7267 735a 1464 6973 706c 6179  valargsZ.display
+000008a0: 5f64 6574 6169 6c5f 6c65 7665 6ce9 0200  _detail_level...
+000008b0: 0000 5a13 7265 7475 726e 696e 675f 736f  ..Z.returning_so
+000008c0: 6d65 7468 696e 67da 1161 6374 696f 6e5f  mething..action_
+000008d0: 6e61 6d65 5f63 6f6c 6f72 da07 6469 7370  name_color..disp
+000008e0: 6c61 7954 da0c 6163 7469 6f6e 5f63 6f6c  layT..action_col
+000008f0: 6f72 7a07 3c2f 7370 616e 3e46 2907 7202  orz.</span>F).r.
+00000900: 0000 0072 2000 0000 7217 0000 0072 0500  ...r ...r....r..
+00000910: 0000 7204 0000 00da 0a67 6574 5f61 6374  ..r......get_act
+00000920: 696f 6eda 0f67 6574 5f65 7874 7261 5f73  ion..get_extra_s
+00000930: 7475 6666 290b 7218 0000 0072 1e00 0000  tuff).r....r....
+00000940: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000950: 1900 0000 721f 0000 0072 1d00 0000 7209  ....r....r....r.
+00000960: 0000 005a 0a74 776f 5f62 6c61 6e6b 73da  ...Z.two_blanks.
+00000970: 0672 6573 756c 7472 1500 0000 7215 0000  .resultr....r...
+00000980: 0072 1600 0000 da12 6765 745f 6163 7469  .r......get_acti
+00000990: 6f6e 5f72 6573 756c 7473 7300 0000 7344  on_resultss...sD
+000009a0: 0000 0002 0a06 0104 ff04 0304 010c 040c  ................
+000009b0: 0110 0202 0202 0102 0102 0102 0102 0102  ................
+000009c0: 0102 0102 0102 0104 f708 0d08 0102 0312  ................
+000009d0: 0102 ff02 0202 0102 0102 010a 020e 0104  ................
+000009e0: ff02 0302 f804 fe72 2b00 0000 291e 7212  .......r+...).r.
+000009f0: 0000 00da 0b63 6f6c 6c65 6374 696f 6e73  .....collections
+00000a00: 7202 0000 00da 1664 6566 7573 6564 786d  r......defusedxm
+00000a10: 6c2e 456c 656d 656e 7454 7265 65da 0a64  l.ElementTree..d
+00000a20: 6566 7573 6564 786d 6cda 146d 6170 7461  efusedxml..mapta
+00000a30: 736b 6572 2e73 7263 2e61 6374 696f 6eda  sker.src.action.
+00000a40: 0373 7263 da06 6163 7469 6f6e 7228 0000  .src..actionr(..
+00000a50: 005a 156d 6170 7461 736b 6572 2e73 7263  .Z.maptasker.src
+00000a60: 2e61 6374 6172 6773 7203 0000 00da 156d  .actargsr......m
+00000a70: 6170 7461 736b 6572 2e73 7263 2e61 6374  aptasker.src.act
+00000a80: 696f 6e63 7204 0000 00da 166d 6170 7461  ioncr......mapta
+00000a90: 736b 6572 2e73 7263 2e66 726d 7468 746d  sker.src.frmthtm
+00000aa0: 6c72 0500 0000 da16 6d61 7074 6173 6b65  lr......maptaske
+00000ab0: 722e 7372 632e 7379 7363 6f6e 7374 7206  r.src.sysconstr.
+00000ac0: 0000 005a 156d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
+00000ad0: 7263 2e78 6d6c 6461 7461 7207 0000 0072  rc.xmldatar....r
+00000ae0: 0800 0000 da04 6469 6374 da03 7374 7272  ......dict..strr
+00000af0: 1700 0000 da0b 456c 656d 656e 7454 7265  ......ElementTre
+00000b00: 65da 0358 4d4c da04 6c69 7374 da04 626f  e..XML..list..bo
+00000b10: 6f6c da05 7475 706c 6572 2000 0000 722b  ol..tupler ...r+
+00000b20: 0000 0072 1500 0000 7215 0000 0072 1500  ...r....r....r..
+00000b30: 0000 7216 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000b40: 3e01 0000 0073 6600 0000 080c 0c01 0802  >....sf.........
+00000b50: 1202 0c01 0c01 0c01 0c01 0c01 0c01 1206  ................
+00000b60: 022c 0601 02ff 0202 02fe 0603 02fd 0204  .,..............
+00000b70: 02fc 0205 02fb 0206 02fa 0207 02f9 0208  ................
+00000b80: 02f8 0209 02f7 020a 0af6 0229 0201 02ff  ...........)....
+00000b90: 0602 02fe 0603 02fd 0204 02fc 0605 02fb  ................
+00000ba0: 0606 02fa 0607 02f9 0608 02f8 0209 0ef7  ................
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/actiont.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/actiont.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/argsdict.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/argsdict.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/caveats.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/caveats.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 15:26:45 2023 UTC, .py size: 3401 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,118 @@
-00000000: 6f0d 0d0a 0000 0000 b541 2c64 490d 0000  o........A,dI...
+00000000: 6f0d 0d0a 0000 0000 ca23 3c64 450d 0000  o........#<dE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
+00000020: 0008 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 0200 0100 6d02 5a03 0100  d.l.m.....m.Z...
-00000040: 6402 6504 6505 1900 6403 6506 6404 6506  d.e.e...d.e.d.e.
-00000050: 6405 6401 6608 6406 6407 8404 5a07 6401  d.d.f.d.d...Z.d.
-00000060: 5300 2908 e900 0000 004e da0b 6f75 7470  S.)......N..outp
-00000070: 7574 5f6c 6973 74da 0c70 726f 6772 616d  ut_list..program
-00000080: 5f61 7267 73da 0863 6f6c 6f72 6d61 70da  _args..colormap.
-00000090: 0672 6574 7572 6e63 0300 0000 0000 0000  .returnc........
-000000a0: 0000 0000 0900 0000 0700 0000 4300 0000  ............C...
-000000b0: 73c8 0000 0064 017c 0264 0219 009b 009d  s....d.|.d......
-000000c0: 027c 0164 0319 0017 0064 0417 007d 0364  .|.d.....d...}.d
-000000d0: 057d 0464 067d 0564 077d 0674 00a0 017c  .}.d.}.d.}.t...|
-000000e0: 027c 017c 0064 0864 09a1 0501 0074 00a0  .|.|.d.d.....t..
-000000f0: 017c 027c 017c 0064 0a7c 03a1 0501 007c  .|.|.|.d.|.....|
-00000100: 0164 0b19 0064 086b 0472 3664 0c7d 0774  .d...d.k.r6d.}.t
-00000110: 00a0 017c 027c 017c 0064 0a7c 07a1 0501  ...|.|.|.d.|....
-00000120: 0074 00a0 017c 027c 017c 0064 0a7c 04a1  .t...|.|.|.d.|..
-00000130: 0501 0074 00a0 017c 027c 017c 0064 0a7c  ...t...|.|.|.d.|
-00000140: 05a1 0501 007c 0164 0b19 0064 086b 0272  .....|.d...d.k.r
-00000150: 5964 0d7d 0874 00a0 017c 027c 017c 0064  Yd.}.t...|.|.|.d
-00000160: 0a7c 08a1 0501 0074 00a0 017c 027c 017c  .|.....t...|.|.|
-00000170: 0064 0a7c 06a1 0501 0064 0e53 0029 0f61  .d.|.....d.S.).a
-00000180: 3001 0000 6f75 7470 7574 2074 6865 2070  0...output the p
-00000190: 726f 6772 616d 2063 6176 6561 7473 0a20  rogram caveats. 
-000001a0: 2020 204f 7574 7075 7420 7468 6520 7072     Output the pr
-000001b0: 6f67 7261 6d20 6361 7665 6174 7320 6174  ogram caveats at
-000001c0: 2074 6865 2076 6572 7920 656e 640a 2020   the very end.  
-000001d0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000001e0: 3a20 6c69 7374 2069 6e74 6f20 7768 6963  : list into whic
-000001f0: 6820 616c 6c20 6f75 7470 7574 2068 6173  h all output has
-00000200: 2062 6565 6e20 6164 6465 642c 2074 6865   been added, the
-00000210: 2070 726f 6772 616d 2072 756e 7469 6d65   program runtime
-00000220: 2061 7267 756d 656e 7473 2c0a 2020 2020   arguments,.    
-00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000240: 7468 6520 6469 6374 696f 6e61 7279 206f  the dictionary o
-00000250: 6620 636f 6c6f 7273 2074 6f20 7573 650a  f colors to use.
-00000260: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00000270: 3a20 7468 6520 636f 756e 7420 6f66 2074  : the count of t
-00000280: 6865 206e 756d 6265 7220 6f66 2074 696d  he number of tim
-00000290: 6573 2074 6865 2070 726f 6772 616d 2068  es the program h
-000002a0: 6173 2062 6565 6e20 6361 6c6c 6564 0a0a  as been called..
-000002b0: 2020 2020 7a13 3c73 7061 6e20 7374 796c      z.<span styl
-000002c0: 653d 2263 6f6c 6f72 3ada 1774 7261 696c  e="color:..trail
-000002d0: 696e 675f 636f 6d6d 656e 7473 5f63 6f6c  ing_comments_col
-000002e0: 6f72 da0b 666f 6e74 5f74 6f5f 7573 657a  or..font_to_usez
-000002f0: 0a3e 4341 5645 4154 533a 0a7a 7c2d 2054  .>CAVEATS:.z|- T
-00000300: 6869 7320 6861 7320 6f6e 6c79 2062 6565  his has only bee
-00000310: 6e20 7465 7374 6564 206f 6e20 6d79 206f  n tested on my o
-00000320: 776e 2062 6163 6b75 702e 786d 6c20 6669  wn backup.xml fi
-00000330: 6c65 2e20 2046 6f72 2070 726f 626c 656d  le.  For problem
-00000340: 732c 2072 6570 6f72 7420 7468 656d 206f  s, report them o
-00000350: 6e20 6874 7470 733a 2f2f 6769 7468 7562  n https://github
-00000360: 2e63 6f6d 2f6d 6374 696e 6b65 722f 4d61  .com/mctinker/Ma
-00000370: 702d 5461 736b 6572 2e7a 5e2d 2054 6173  p-Tasker.z^- Tas
-00000380: 6b73 2074 6861 7420 6172 6520 6964 656e  ks that are iden
-00000390: 7469 6669 6564 2061 7320 2255 6e6e 616d  tified as "Unnam
-000003a0: 6564 2f41 6e6f 6e79 6d6f 7573 2220 6861  ed/Anonymous" ha
-000003b0: 7665 206e 6f20 6e61 6d65 2061 6e64 2061  ve no name and a
-000003c0: 7265 2063 6f6e 7369 6465 7265 6420 416e  re considered An
-000003d0: 6f6e 796d 6f75 732e 0a7a 802d 2054 6173  onymous..z.- Tas
-000003e0: 6b65 7220 6669 656c 6473 2074 6861 7420  ker fields that 
-000003f0: 6861 7665 2065 6d62 6564 6465 6420 4854  have embedded HT
-00000400: 4d4c 2028 652e 672e 2063 6f6c 6f72 3d2e  ML (e.g. color=.
-00000410: 2e2e 3e22 2920 7769 6c6c 2072 6573 756c  ..>") will resul
-00000420: 7420 696e 2074 6865 2072 656d 6169 6e69  t in the remaini
-00000430: 6e67 206c 6162 656c 2064 6973 706c 6179  ng label display
-00000440: 6564 2069 6e20 7468 6174 2073 616d 6520  ed in that same 
-00000450: 636f 6c6f 722f 666f 6e74 2e72 0100 0000  color/font.r....
-00000460: 7a04 3c68 723e e904 0000 00da 1464 6973  z.<hr>.......dis
-00000470: 706c 6179 5f64 6574 6169 6c5f 6c65 7665  play_detail_leve
-00000480: 6c7a 812d 204d 6f73 7420 6275 7420 6e6f  lz.- Most but no
-00000490: 7420 616c 6c20 5461 736b 2061 6374 696f  t all Task actio
-000004a0: 6e73 2068 6176 6520 6265 656e 206d 6170  ns have been map
-000004b0: 7065 6420 616e 6420 7769 6c6c 2064 6973  ped and will dis
-000004c0: 706c 6179 2061 7320 7375 6368 2e20 204c  play as such.  L
-000004d0: 696b 6577 6973 6520 666f 7220 5072 6f66  ikewise for Prof
-000004e0: 696c 6520 636f 6e64 6974 696f 6e73 2061  ile conditions a
-000004f0: 6e64 2050 6c75 672d 696e 732e 0a3c 2f73  nd Plug-ins..</s
-00000500: 7061 6e3e 7a87 2d20 466f 7220 6f70 7469  pan>z.- For opti
-00000510: 6f6e 202d 6430 2c20 5461 736b 7320 7468  on -d0, Tasks th
-00000520: 6174 2061 7265 2069 6465 6e74 6966 6965  at are identifie
-00000530: 6420 6173 2022 556e 6e61 6d65 642f 416e  d as "Unnamed/An
-00000540: 6f6e 796d 6f75 7322 2077 696c 6c20 6861  onymous" will ha
-00000550: 7665 2074 6865 6972 2066 6972 7374 2054  ve their first T
-00000560: 6173 6b20 6f6e 6c79 206c 6973 7465 642e  ask only listed.
-00000570: 2e2e 2e0a 2020 6a75 7374 206c 696b 6520  ....  just like 
-00000580: 5461 736b 6572 2064 6f65 732e 0a4e 2902  Tasker does..N).
-00000590: da0c 6275 696c 645f 6f75 7470 7574 da09  ..build_output..
-000005a0: 6d79 5f6f 7574 7075 7429 0972 0200 0000  my_output).r....
-000005b0: 7203 0000 0072 0400 0000 5a07 6361 7665  r....r....Z.cave
-000005c0: 6174 315a 0763 6176 6561 7433 5a07 6361  at1Z.caveat3Z.ca
-000005d0: 7665 6174 345a 0763 6176 6561 7436 5a07  veat4Z.caveat6Z.
-000005e0: 6361 7665 6174 325a 0763 6176 6561 7435  caveat2Z.caveat5
-000005f0: a900 720c 0000 00fa 762f 5573 6572 732f  ..r.....v/Users/
-00000600: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
-00000610: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
-00000620: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
-00000630: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
-00000640: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
-00000650: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
-00000660: 2f73 7263 2f63 6176 6561 7473 2e70 79da  /src/caveats.py.
-00000670: 0f64 6973 706c 6179 5f63 6176 6561 7473  .display_caveats
-00000680: 1100 0000 733c 0000 000c 0a06 0102 ff02  ....s<..........
-00000690: 0202 fe02 ff02 0602 ff02 0502 ff02 0502  ................
-000006a0: ff12 0412 010c 0102 0202 ff04 040a 0104  ................
-000006b0: ff12 0312 010c 0202 0302 ff04 040a 0104  ................
-000006c0: ff12 0304 0172 0e00 0000 2908 da15 6d61  .....r....)...ma
-000006d0: 7074 6173 6b65 722e 7372 632e 6f75 7470  ptasker.src.outp
-000006e0: 7574 6cda 0373 7263 da07 6f75 7470 7574  utl..src..output
-000006f0: 6c72 0a00 0000 da04 6c69 7374 da03 7374  lr......list..st
-00000700: 72da 0464 6963 7472 0e00 0000 720c 0000  r..dictr....r...
-00000710: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000720: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
-00000730: 0000 0012 0d22 03                        .....".
+00000040: 6400 6402 6c04 6d05 5a05 0100 6403 6506  d.d.l.m.Z...d.e.
+00000050: 6507 1900 6404 6508 6405 6508 6406 6401  e...d.e.d.e.d.d.
+00000060: 6608 6407 6408 8404 5a09 6401 5300 2909  f.d.d...Z.d.S.).
+00000070: e900 0000 004e 2901 da0b 666f 726d 6174  .....N)...format
+00000080: 5f68 746d 6cda 0b6f 7574 7075 745f 6c69  _html..output_li
+00000090: 7374 da0c 7072 6f67 7261 6d5f 6172 6773  st..program_args
+000000a0: da08 636f 6c6f 726d 6170 da06 7265 7475  ..colormap..retu
+000000b0: 726e 6303 0000 0000 0000 0000 0000 0009  rnc.............
+000000c0: 0000 0008 0000 0043 0000 0073 c400 0000  .......C...s....
+000000d0: 7400 7c02 6401 6402 6403 6404 8305 7d03  t.|.d.d.d.d...}.
+000000e0: 6405 7d04 6406 7d05 6407 7d06 7401 a002  d.}.d.}.d.}.t...
+000000f0: 7c02 7c01 7c00 6408 6409 a105 0100 7401  |.|.|.d.d.....t.
+00000100: a002 7c02 7c01 7c00 640a 7c03 a105 0100  ..|.|.|.d.|.....
+00000110: 7c01 640b 1900 6408 6b04 7231 640c 7d07  |.d...d.k.r1d.}.
+00000120: 7401 a002 7c02 7c01 7c00 640a 7c07 a105  t...|.|.|.d.|...
+00000130: 0100 7401 a002 7c02 7c01 7c00 640a 7c04  ..t...|.|.|.d.|.
+00000140: a105 0100 7401 a002 7c02 7c01 7c00 640a  ....t...|.|.|.d.
+00000150: 7c05 a105 0100 7c01 640b 1900 6408 6b02  |.....|.d...d.k.
+00000160: 7254 640d 7d08 7401 a002 7c02 7c01 7c00  rTd.}.t...|.|.|.
+00000170: 640a 7c08 a105 0100 7401 a002 7c02 7c01  d.|.....t...|.|.
+00000180: 7c00 640a 7c06 9b00 640e 9d02 a105 0100  |.d.|...d.......
+00000190: 640f 5300 2910 6130 0100 006f 7574 7075  d.S.).a0...outpu
+000001a0: 7420 7468 6520 7072 6f67 7261 6d20 6361  t the program ca
+000001b0: 7665 6174 730a 2020 2020 4f75 7470 7574  veats.    Output
+000001c0: 2074 6865 2070 726f 6772 616d 2063 6176   the program cav
+000001d0: 6561 7473 2061 7420 7468 6520 7665 7279  eats at the very
+000001e0: 2065 6e64 0a20 2020 2020 2020 2050 6172   end.        Par
+000001f0: 616d 6574 6572 733a 206c 6973 7420 696e  ameters: list in
+00000200: 746f 2077 6869 6368 2061 6c6c 206f 7574  to which all out
+00000210: 7075 7420 6861 7320 6265 656e 2061 6464  put has been add
+00000220: 6564 2c20 7468 6520 7072 6f67 7261 6d20  ed, the program 
+00000230: 7275 6e74 696d 6520 6172 6775 6d65 6e74  runtime argument
+00000240: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00000250: 2020 2020 2020 2074 6865 2064 6963 7469         the dicti
+00000260: 6f6e 6172 7920 6f66 2063 6f6c 6f72 7320  onary of colors 
+00000270: 746f 2075 7365 0a0a 2020 2020 2020 2020  to use..        
+00000280: 5265 7475 726e 733a 2074 6865 2063 6f75  Returns: the cou
+00000290: 6e74 206f 6620 7468 6520 6e75 6d62 6572  nt of the number
+000002a0: 206f 6620 7469 6d65 7320 7468 6520 7072   of times the pr
+000002b0: 6f67 7261 6d20 6861 7320 6265 656e 2063  ogram has been c
+000002c0: 616c 6c65 640a 0a20 2020 20da 1774 7261  alled..    ..tra
+000002d0: 696c 696e 675f 636f 6d6d 656e 7473 5f63  iling_comments_c
+000002e0: 6f6c 6f72 da00 7a09 4341 5645 4154 533a  olor..z.CAVEATS:
+000002f0: 0a46 7a7c 2d20 5468 6973 2068 6173 206f  .Fz|- This has o
+00000300: 6e6c 7920 6265 656e 2074 6573 7465 6420  nly been tested 
+00000310: 6f6e 206d 7920 6f77 6e20 6261 636b 7570  on my own backup
+00000320: 2e78 6d6c 2066 696c 652e 2020 466f 7220  .xml file.  For 
+00000330: 7072 6f62 6c65 6d73 2c20 7265 706f 7274  problems, report
+00000340: 2074 6865 6d20 6f6e 2068 7474 7073 3a2f   them on https:/
+00000350: 2f67 6974 6875 622e 636f 6d2f 6d63 7469  /github.com/mcti
+00000360: 6e6b 6572 2f4d 6170 2d54 6173 6b65 722e  nker/Map-Tasker.
+00000370: 7a5e 2d20 5461 736b 7320 7468 6174 2061  z^- Tasks that a
+00000380: 7265 2069 6465 6e74 6966 6965 6420 6173  re identified as
+00000390: 2022 556e 6e61 6d65 642f 416e 6f6e 796d   "Unnamed/Anonym
+000003a0: 6f75 7322 2068 6176 6520 6e6f 206e 616d  ous" have no nam
+000003b0: 6520 616e 6420 6172 6520 636f 6e73 6964  e and are consid
+000003c0: 6572 6564 2041 6e6f 6e79 6d6f 7573 2e0a  ered Anonymous..
+000003d0: 7a91 2d20 416c 6c20 6174 7465 6d70 7473  z.- All attempts
+000003e0: 2061 7265 206d 6164 6520 746f 2072 6574   are made to ret
+000003f0: 6169 6e20 656d 6265 6464 6564 2048 544d  ain embedded HTM
+00000400: 4c20 2865 2e67 2e20 636f 6c6f 723d 2e2e  L (e.g. color=..
+00000410: 2e3e 2229 2069 6e20 5461 736b 6572 2066  .>") in Tasker f
+00000420: 6965 6c64 732c 2062 7574 2069 7320 7374  ields, but is st
+00000430: 7269 7070 6564 206f 7574 206f 6620 4163  ripped out of Ac
+00000440: 7469 6f6e 206c 6162 656c 7320 616e 6420  tion labels and 
+00000450: 5461 736b 6572 4e65 7420 636f 6d6d 656e  TaskerNet commen
+00000460: 7473 2e72 0100 0000 7a04 3c68 723e e904  ts.r....z.<hr>..
+00000470: 0000 00da 1464 6973 706c 6179 5f64 6574  .....display_det
+00000480: 6169 6c5f 6c65 7665 6c7a 7a2d 204d 6f73  ail_levelzz- Mos
+00000490: 7420 6275 7420 6e6f 7420 616c 6c20 5461  t but not all Ta
+000004a0: 736b 2061 6374 696f 6e73 2068 6176 6520  sk actions have 
+000004b0: 6265 656e 206d 6170 7065 6420 616e 6420  been mapped and 
+000004c0: 7769 6c6c 2064 6973 706c 6179 2061 7320  will display as 
+000004d0: 7375 6368 2e20 204c 696b 6577 6973 6520  such.  Likewise 
+000004e0: 666f 7220 5072 6f66 696c 6520 636f 6e64  for Profile cond
+000004f0: 6974 696f 6e73 2061 6e64 2050 6c75 672d  itions and Plug-
+00000500: 696e 732e 0a7a 892d 2046 6f72 206f 7074  ins..z.- For opt
+00000510: 696f 6e20 2d64 302c 2054 6173 6b73 2074  ion -d0, Tasks t
+00000520: 6861 7420 6172 6520 6964 656e 7469 6669  hat are identifi
+00000530: 6564 2061 7320 2255 6e6e 616d 6564 2f41  ed as "Unnamed/A
+00000540: 6e6f 6e79 6d6f 7573 2220 7769 6c6c 2068  nonymous" will h
+00000550: 6176 6520 7468 6569 7220 6669 7273 7420  ave their first 
+00000560: 4163 7469 6f6e 206f 6e6c 7920 6c69 7374  Action only list
+00000570: 6564 2e2e 2e2e 0a20 206a 7573 7420 6c69  ed.....  just li
+00000580: 6b65 2054 6173 6b65 7220 646f 6573 2e0a  ke Tasker does..
+00000590: 7a07 3c2f 7370 616e 3e4e 2903 7202 0000  z.</span>N).r...
+000005a0: 00da 0c62 7569 6c64 5f6f 7574 7075 74da  ...build_output.
+000005b0: 096d 795f 6f75 7470 7574 2909 7203 0000  .my_output).r...
+000005c0: 0072 0400 0000 7205 0000 005a 0763 6176  .r....r....Z.cav
+000005d0: 6561 7431 5a07 6361 7665 6174 335a 0763  eat1Z.caveat3Z.c
+000005e0: 6176 6561 7434 5a07 6361 7665 6174 365a  aveat4Z.caveat6Z
+000005f0: 0763 6176 6561 7432 5a07 6361 7665 6174  .caveat2Z.caveat
+00000600: 35a9 0072 0d00 0000 fa76 2f55 7365 7273  5..r.....v/Users
+00000610: 2f6d 696b 7275 6269 6e2f 4c69 6272 6172  /mikrubin/Librar
+00000620: 792f 436c 6f75 6453 746f 7261 6765 2f47  y/CloudStorage/G
+00000630: 6f6f 676c 6544 7269 7665 2d6d 696b 7275  oogleDrive-mikru
+00000640: 6269 6e40 676d 6169 6c2e 636f 6d2f 4d79  bin@gmail.com/My
+00000650: 2044 7269 7665 2f50 7974 686f 6e2f 6d61   Drive/Python/ma
+00000660: 7074 6173 6b65 722f 6d61 7074 6173 6b65  ptasker/maptaske
+00000670: 722f 7372 632f 6361 7665 6174 732e 7079  r/src/caveats.py
+00000680: da0f 6469 7370 6c61 795f 6361 7665 6174  ..display_caveat
+00000690: 7312 0000 0073 3200 0000 1009 0202 02ff  s....s2.........
+000006a0: 0205 02ff 0205 02ff 1204 1201 0c01 0202  ................
+000006b0: 02ff 0404 0a01 04ff 1203 1201 0c02 0203  ................
+000006c0: 02ff 0404 0a01 04ff 1803 0401 720f 0000  ............r...
+000006d0: 0029 0ada 156d 6170 7461 736b 6572 2e73  .)...maptasker.s
+000006e0: 7263 2e6f 7574 7075 746c da03 7372 63da  rc.outputl..src.
+000006f0: 076f 7574 7075 746c 720b 0000 00da 166d  .outputlr......m
+00000700: 6170 7461 736b 6572 2e73 7263 2e66 726d  aptasker.src.frm
+00000710: 7468 746d 6c72 0200 0000 da04 6c69 7374  thtmlr......list
+00000720: da03 7374 72da 0464 6963 7472 0f00 0000  ..str..dictr....
+00000730: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000740: 0e00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000750: 0000 7306 0000 0012 0d0c 0122 03         ..s........".
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/colors.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/colors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/colrmode.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/colrmode.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar 31 16:03:07 2023 UTC, .py size: 3285 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3b04 2764 d50c 0000  o.......;.'d....
+00000000: 6f0d 0d0a 0000 0000 9374 3964 cc0c 0000  o........t9d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 5a00 6402 6501 6403 6502 6404  d.l.Z.d.e.d.e.d.
 00000040: 6502 6606 6405 6406 8404 5a03 6401 5300  e.f.d.d...Z.d.S.
 00000050: 2907 e900 0000 004e da0f 6170 7065 6172  )......N..appear
 00000060: 616e 6365 5f6d 6f64 65da 0863 6f6c 6f72  ance_mode..color
 00000070: 6d61 70da 0672 6574 7572 6e63 0200 0000  map..returnc....
@@ -48,61 +48,61 @@
 000002f0: 725f 7461 736b 5f63 6f6c 6f72 da0b 4772  r_task_color..Gr
 00000300: 6565 6e59 656c 6c6f 77da 0a74 6173 6b5f  eenYellow..task_
 00000310: 636f 6c6f 72da 0659 656c 6c6f 77da 1275  color..Yellow..u
 00000320: 6e6b 6e6f 776e 5f74 6173 6b5f 636f 6c6f  nknown_task_colo
 00000330: 72da 0b73 6365 6e65 5f63 6f6c 6f72 da04  r..scene_color..
 00000340: 4c69 6d65 da0c 6275 6c6c 6574 5f63 6f6c  Lime..bullet_col
 00000350: 6f72 da11 6163 7469 6f6e 5f6e 616d 655f  or..action_name_
-00000360: 636f 6c6f 72da 0d50 616c 6547 6f6c 6465  color..PaleGolde
-00000370: 6e72 6f64 da0c 6163 7469 6f6e 5f63 6f6c  nrod..action_col
-00000380: 6f72 da0a 4461 726b 4f72 616e 6765 da12  or..DarkOrange..
-00000390: 6163 7469 6f6e 5f6c 6162 656c 5f63 6f6c  action_label_col
-000003a0: 6f72 da07 4d61 6765 6e74 61da 1661 6374  or..Magenta..act
-000003b0: 696f 6e5f 636f 6e64 6974 696f 6e5f 636f  ion_condition_co
-000003c0: 6c6f 72da 0a50 6170 6179 6157 6869 70da  lor..PapayaWhip.
-000003d0: 1564 6973 6162 6c65 645f 6163 7469 6f6e  .disabled_action
-000003e0: 5f63 6f6c 6f72 da07 4372 696d 736f 6eda  _color..Crimson.
-000003f0: 1770 726f 6669 6c65 5f63 6f6e 6469 7469  .profile_conditi
-00000400: 6f6e 5f63 6f6c 6f72 da08 4c61 7665 6e64  on_color..Lavend
-00000410: 6572 da10 6261 636b 6772 6f75 6e64 5f63  er..background_c
-00000420: 6f6c 6f72 da08 4461 726b 426c 7565 da17  olor..DarkBlue..
-00000430: 7472 6169 6c69 6e67 5f63 6f6d 6d65 6e74  trailing_comment
-00000440: 735f 636f 6c6f 72da 0950 6561 6368 5075  s_color..PeachPu
-00000450: 6666 da0f 7461 736b 6572 6e65 745f 636f  ff..taskernet_co
-00000460: 6c6f 72da 094c 6967 6874 5069 6e6b da11  lor..LightPink..
-00000470: 7072 6566 6572 656e 6365 735f 636f 6c6f  preferences_colo
-00000480: 72da 0542 6c61 636b da07 4461 726b 5265  r..Black..DarkRe
-00000490: 64da 094c 6177 6e47 7265 656e da09 4461  d..LawnGreen..Da
-000004a0: 726b 4772 6565 6eda 0f4d 6564 6975 6d56  rkGreen..MediumV
-000004b0: 696f 6c65 7452 6564 da06 5075 7270 6c65  ioletRed..Purple
-000004c0: da0d 4461 726b 536c 6174 6547 7261 79da  ..DarkSlateGray.
-000004d0: 0649 6e64 6967 6fda 0c4d 6564 6975 6d4f  .Indigo..MediumO
-000004e0: 7263 6869 64da 0542 726f 776e da09 496e  rchid..Brown..In
-000004f0: 6469 616e 5265 64da 0654 6f6d 6174 6fda  dianRed..Tomato.
-00000500: 0952 6f79 616c 426c 7565 da0a 446f 6467  .RoyalBlue..Dodg
-00000510: 6572 426c 7565 2902 da0a 6461 726b 6465  erBlue)...darkde
-00000520: 7465 6374 5a06 6973 4461 726b 2903 7202  tectZ.isDark).r.
-00000530: 0000 0072 0300 0000 da04 6d6f 6465 a900  ...r......mode..
-00000540: 7238 0000 00fa 772f 5573 6572 732f 6d69  r8....w/Users/mi
-00000550: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
-00000560: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
-00000570: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
-00000580: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
-00000590: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
-000005a0: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
-000005b0: 7263 2f63 6f6c 726d 6f64 652e 7079 da0e  rc/colrmode.py..
-000005c0: 7365 745f 636f 6c6f 725f 6d6f 6465 1100  set_color_mode..
-000005d0: 0000 73a0 0000 0008 0912 0104 0208 0202  ..s.............
-000005e0: 0104 0102 ff04 0202 fe04 0302 fd04 0402  ................
-000005f0: fc04 0502 fb04 0602 fa04 0702 f904 0802  ................
-00000600: f804 0902 f704 0a02 f604 0b02 f504 0c02  ................
-00000610: f404 0d02 f304 0e02 f204 0f02 f104 1002  ................
-00000620: f004 1102 ef04 1206 ee04 2a02 eb04 0102  ..........*.....
-00000630: ff04 0202 fe04 0302 fd04 0402 fc04 0502  ................
-00000640: fb04 0602 fa04 0702 f904 0802 f804 0902  ................
-00000650: f704 0a02 f604 0b02 f504 0c02 f404 0d02  ................
-00000660: f304 0e02 f204 0f02 f104 1002 f004 1102  ................
-00000670: ef04 1206 ee04 1572 3a00 0000 2904 7236  .......r:...).r6
-00000680: 0000 00da 0373 7472 da04 6469 6374 723a  .....str..dictr:
-00000690: 0000 0072 3800 0000 7238 0000 0072 3800  ...r8...r8...r8.
-000006a0: 0000 7239 0000 00da 083c 6d6f 6475 6c65  ..r9.....<module
-000006b0: 3e01 0000 0073 0400 0000 080d 1a03       >....s........
+00000360: 636f 6c6f 72da 0447 6f6c 64da 0c61 6374  color..Gold..act
+00000370: 696f 6e5f 636f 6c6f 72da 0a44 6172 6b4f  ion_color..DarkO
+00000380: 7261 6e67 65da 1261 6374 696f 6e5f 6c61  range..action_la
+00000390: 6265 6c5f 636f 6c6f 72da 074d 6167 656e  bel_color..Magen
+000003a0: 7461 da16 6163 7469 6f6e 5f63 6f6e 6469  ta..action_condi
+000003b0: 7469 6f6e 5f63 6f6c 6f72 da0a 5061 7061  tion_color..Papa
+000003c0: 7961 5768 6970 da15 6469 7361 626c 6564  yaWhip..disabled
+000003d0: 5f61 6374 696f 6e5f 636f 6c6f 72da 0743  _action_color..C
+000003e0: 7269 6d73 6f6e da17 7072 6f66 696c 655f  rimson..profile_
+000003f0: 636f 6e64 6974 696f 6e5f 636f 6c6f 72da  condition_color.
+00000400: 084c 6176 656e 6465 72da 1062 6163 6b67  .Lavender..backg
+00000410: 726f 756e 645f 636f 6c6f 72da 0844 6172  round_color..Dar
+00000420: 6b42 6c75 65da 1774 7261 696c 696e 675f  kBlue..trailing_
+00000430: 636f 6d6d 656e 7473 5f63 6f6c 6f72 da09  comments_color..
+00000440: 5065 6163 6850 7566 66da 0f74 6173 6b65  PeachPuff..taske
+00000450: 726e 6574 5f63 6f6c 6f72 da09 4c69 6768  rnet_color..Ligh
+00000460: 7450 696e 6bda 1170 7265 6665 7265 6e63  tPink..preferenc
+00000470: 6573 5f63 6f6c 6f72 da05 426c 6163 6bda  es_color..Black.
+00000480: 0744 6172 6b52 6564 da09 4c61 776e 4772  .DarkRed..LawnGr
+00000490: 6565 6eda 0944 6172 6b47 7265 656e da0f  een..DarkGreen..
+000004a0: 4d65 6469 756d 5669 6f6c 6574 5265 64da  MediumVioletRed.
+000004b0: 0650 7572 706c 65da 0d44 6172 6b53 6c61  .Purple..DarkSla
+000004c0: 7465 4772 6179 da06 496e 6469 676f da0c  teGray..Indigo..
+000004d0: 4d65 6469 756d 4f72 6368 6964 da05 4272  MediumOrchid..Br
+000004e0: 6f77 6eda 0949 6e64 6961 6e52 6564 da06  own..IndianRed..
+000004f0: 546f 6d61 746f da09 526f 7961 6c42 6c75  Tomato..RoyalBlu
+00000500: 65da 0a44 6f64 6765 7242 6c75 6529 02da  e..DodgerBlue)..
+00000510: 0a64 6172 6b64 6574 6563 745a 0669 7344  .darkdetectZ.isD
+00000520: 6172 6b29 0372 0200 0000 7203 0000 00da  ark).r....r.....
+00000530: 046d 6f64 65a9 0072 3800 0000 fa77 2f55  .mode..r8....w/U
+00000540: 7365 7273 2f6d 696b 7275 6269 6e2f 4c69  sers/mikrubin/Li
+00000550: 6272 6172 792f 436c 6f75 6453 746f 7261  brary/CloudStora
+00000560: 6765 2f47 6f6f 676c 6544 7269 7665 2d6d  ge/GoogleDrive-m
+00000570: 696b 7275 6269 6e40 676d 6169 6c2e 636f  ikrubin@gmail.co
+00000580: 6d2f 4d79 2044 7269 7665 2f50 7974 686f  m/My Drive/Pytho
+00000590: 6e2f 6d61 7074 6173 6b65 722f 6d61 7074  n/maptasker/mapt
+000005a0: 6173 6b65 722f 7372 632f 636f 6c72 6d6f  asker/src/colrmo
+000005b0: 6465 2e70 79da 0e73 6574 5f63 6f6c 6f72  de.py..set_color
+000005c0: 5f6d 6f64 6511 0000 0073 a000 0000 0809  _mode....s......
+000005d0: 1201 0402 0802 0201 0401 02ff 0402 02fe  ................
+000005e0: 0403 02fd 0404 02fc 0405 02fb 0406 02fa  ................
+000005f0: 0407 02f9 0408 02f8 0409 02f7 040a 02f6  ................
+00000600: 040b 02f5 040c 02f4 040d 02f3 040e 02f2  ................
+00000610: 040f 02f1 0410 02f0 0411 02ef 0412 06ee  ................
+00000620: 042a 02eb 0401 02ff 0402 02fe 0403 02fd  .*..............
+00000630: 0404 02fc 0405 02fb 0406 02fa 0407 02f9  ................
+00000640: 0408 02f8 0409 02f7 040a 02f6 040b 02f5  ................
+00000650: 040c 02f4 040d 02f3 040e 02f2 040f 02f1  ................
+00000660: 0410 02f0 0411 02ef 0412 06ee 0415 723a  ..............r:
+00000670: 0000 0029 0472 3600 0000 da03 7374 72da  ...).r6.....str.
+00000680: 0464 6963 7472 3a00 0000 7238 0000 0072  .dictr:...r8...r
+00000690: 3800 0000 7238 0000 0072 3900 0000 da08  8...r8...r9.....
+000006a0: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
+000006b0: 0008 0d1a 03                             .....
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/condition.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/condition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/debug.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/debug.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar 27 15:29:00 2023 UTC, .py size: 2440 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-00000000: 6f0d 0d0a 0000 0000 3cb6 2164 8809 0000  o.......<.!d....
+00000000: 6f0d 0d0a 0000 0000 23a1 3564 df09 0000  o.......#.5d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000020: 0008 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 6d02 0200  d.l.Z.d.d.l.m...
-00000040: 0100 6d03 5a04 0100 6402 5a05 6403 6506  ..m.Z...d.Z.d.e.
-00000050: 6404 6506 6405 6507 6406 6401 6608 6407  d.e.d.e.d.d.f.d.
-00000060: 6408 8404 5a08 6401 5300 2909 e900 0000  d...Z.d.S.).....
-00000070: 004e 7a2e 3c73 7061 6e20 7374 796c 653d  .Nz.<span style=
-00000080: 2263 6f6c 6f72 3a57 6869 7465 3b66 6f6e  "color:White;fon
-00000090: 742d 6661 6d69 6c79 3a43 6f75 7269 6572  t-family:Courier
-000000a0: 223e da08 636f 6c6f 726d 6170 da0c 7072  ">..colormap..pr
-000000b0: 6f67 7261 6d5f 6172 6773 da0b 6f75 7470  ogram_args..outp
-000000c0: 7574 5f6c 6973 74da 0672 6574 7572 6e63  ut_list..returnc
-000000d0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-000000e0: 0d00 0000 4300 0000 73c8 0000 0074 00a0  ....C...s....t..
-000000f0: 017c 007c 017c 0264 0174 029b 0064 0274  .|.|.|.d.t...d.t
-00000100: 0374 046a 0583 019b 0064 039d 04a1 0501  .t.j.....d......
-00000110: 0074 00a0 017c 007c 017c 0264 0164 04a1  .t...|.|.|.d.d..
-00000120: 0501 007c 01a0 06a1 0044 005d 155c 027d  ...|.....D.].\.}
-00000130: 037d 0474 00a0 017c 007c 017c 0264 0174  .}.t...|.|.|.d.t
-00000140: 029b 007c 039b 0064 057c 049b 0064 039d  ...|...d.|...d..
-00000150: 05a1 0501 0071 1f74 00a0 017c 007c 017c  .....q.t...|.|.|
-00000160: 0264 0164 04a1 0501 007c 00a0 06a1 0044  .d.d.....|.....D
-00000170: 005d 165c 027d 037d 0474 00a0 017c 007c  .].\.}.}.t...|.|
-00000180: 017c 0264 0174 029b 0064 067c 039b 0064  .|.d.t...d.|...d
-00000190: 077c 049b 0064 039d 06a1 0501 0071 4274  .|...d.......qBt
-000001a0: 00a0 017c 007c 017c 0264 0164 04a1 0501  ...|.|.|.d.d....
-000001b0: 0064 0853 0029 097a b40a 2020 2020 4f75  .d.S.).z..    Ou
-000001c0: 7470 7574 206f 7572 2072 756e 7469 6d65  tput our runtime
-000001d0: 2061 7267 756d 656e 7473 0a20 2020 2020   arguments.     
-000001e0: 2020 203a 7061 7261 6d20 636f 6c6f 726d     :param colorm
-000001f0: 6170 3a20 636f 6c6f 7273 2074 6f20 7573  ap: colors to us
-00000200: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
-00000210: 2070 726f 6772 616d 5f61 7267 733a 206f   program_args: o
-00000220: 7468 6572 2072 756e 7469 6d65 2061 7267  ther runtime arg
-00000230: 756d 656e 7473 0a20 2020 2020 2020 203a  uments.        :
-00000240: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
-00000250: 743a 2077 6865 7265 2074 6865 206f 7574  t: where the out
-00000260: 7075 7420 676f 6573 0a20 2020 20e9 0400  put goes.    ...
-00000270: 0000 7a09 7379 732e 6172 6776 3a7a 073c  ..z.sys.argv:z.<
-00000280: 2f73 7061 6e3e da00 7a02 3a20 7a0d 636f  /span>..z.: z.co
-00000290: 6c6f 726d 6170 2066 6f72 207a 0820 7365  lormap for z. se
-000002a0: 7420 746f 204e 2907 da0c 6275 696c 645f  t to N)...build_
-000002b0: 6f75 7470 7574 da09 6d79 5f6f 7574 7075  output..my_outpu
-000002c0: 74da 0b64 6562 7567 5f73 7479 6c65 da03  t..debug_style..
-000002d0: 7374 72da 0373 7973 da04 6172 6776 da05  str..sys..argv..
-000002e0: 6974 656d 7329 0572 0200 0000 7203 0000  items).r....r...
-000002f0: 0072 0400 0000 da03 6b65 79da 0576 616c  .r......key..val
-00000300: 7565 a900 7211 0000 00fa 742f 5573 6572  ue..r.....t/User
-00000310: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
-00000320: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
-00000330: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
-00000340: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
-00000350: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
-00000360: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
-00000370: 6572 2f73 7263 2f64 6562 7567 2e70 79da  er/src/debug.py.
-00000380: 0664 6562 7567 3114 0000 0073 5800 0000  .debug1....sX...
-00000390: 0407 0201 0201 0201 0201 1401 04fb 0407  ................
-000003a0: 0201 0201 0201 0201 0201 04fb 1007 0401  ................
-000003b0: 0201 0201 0201 0201 1201 06fb 0407 0201  ................
-000003c0: 0201 0201 0201 0201 04fb 1007 0401 0201  ................
-000003d0: 0201 0201 0201 1401 06fb 0407 0201 0201  ................
-000003e0: 0201 0201 0201 08fb 7213 0000 0029 0972  ........r....).r
-000003f0: 0c00 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
-00000400: 7372 632e 6f75 7470 7574 6cda 0373 7263  src.outputl..src
-00000410: da07 6f75 7470 7574 6c72 0800 0000 720a  ..outputlr....r.
-00000420: 0000 00da 0464 6963 74da 046c 6973 7472  .....dict..listr
-00000430: 1300 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
-00000440: 0000 0072 1200 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000450: 653e 0100 0000 7308 0000 0008 0d12 0104  e>....s.........
-00000460: 021e 03                                  ...
+00000040: 0100 6d03 5a04 0100 6400 6402 6c05 6d06  ..m.Z...d.d.l.m.
+00000050: 5a06 0100 6403 6507 6404 6507 6405 6508  Z...d.e.d.e.d.e.
+00000060: 6406 6401 6608 6407 6408 8404 5a09 6401  d.d.f.d.d...Z.d.
+00000070: 5300 2909 e900 0000 004e 2901 da0b 666f  S.)......N)...fo
+00000080: 726d 6174 5f68 746d 6cda 0863 6f6c 6f72  rmat_html..color
+00000090: 6d61 70da 0c70 726f 6772 616d 5f61 7267  map..program_arg
+000000a0: 73da 0b6f 7574 7075 745f 6c69 7374 da06  s..output_list..
+000000b0: 7265 7475 726e 6303 0000 0000 0000 0000  returnc.........
+000000c0: 0000 0005 0000 000f 0000 0043 0000 0073  ...........C...s
+000000d0: da00 0000 7400 a001 7c00 7c01 7c02 6401  ....t...|.|.|.d.
+000000e0: 7402 7c00 6402 6403 6404 7403 7404 6a05  t.|.d.d.d.t.t.j.
+000000f0: 8301 9b00 9d02 6405 8305 a105 0100 7400  ......d.......t.
+00000100: a001 7c00 7c01 7c02 6401 6403 a105 0100  ..|.|.|.d.d.....
+00000110: 7c01 a006 a100 4400 5d18 5c02 7d03 7d04  |.....D.].\.}.}.
+00000120: 7400 a001 7c00 7c01 7c02 6401 7402 7c00  t...|.|.|.d.t.|.
+00000130: 6402 6403 7c03 9b00 6406 7c04 9b00 9d03  d.d.|...d.|.....
+00000140: 6405 8305 a105 0100 7122 7400 a001 7c00  d.......q"t...|.
+00000150: 7c01 7c02 6401 6403 a105 0100 7c00 a006  |.|.d.d.....|...
+00000160: a100 4400 5d19 5c02 7d03 7d04 7400 a001  ..D.].\.}.}.t...
+00000170: 7c00 7c01 7c02 6401 7402 7c00 6402 6403  |.|.|.d.t.|.d.d.
+00000180: 6407 7c03 9b00 6408 7c04 9b00 9d04 6405  d.|...d.|.....d.
+00000190: 8305 a105 0100 7148 7400 a001 7c00 7c01  ......qHt...|.|.
+000001a0: 7c02 6401 6403 a105 0100 6409 5300 290a  |.d.d.....d.S.).
+000001b0: 7ab4 0a20 2020 204f 7574 7075 7420 6f75  z..    Output ou
+000001c0: 7220 7275 6e74 696d 6520 6172 6775 6d65  r runtime argume
+000001d0: 6e74 730a 2020 2020 2020 2020 3a70 6172  nts.        :par
+000001e0: 616d 2063 6f6c 6f72 6d61 703a 2063 6f6c  am colormap: col
+000001f0: 6f72 7320 746f 2075 7365 0a20 2020 2020  ors to use.     
+00000200: 2020 203a 7061 7261 6d20 7072 6f67 7261     :param progra
+00000210: 6d5f 6172 6773 3a20 6f74 6865 7220 7275  m_args: other ru
+00000220: 6e74 696d 6520 6172 6775 6d65 6e74 730a  ntime arguments.
+00000230: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00000240: 7574 7075 745f 6c69 7374 3a20 7768 6572  utput_list: wher
+00000250: 6520 7468 6520 6f75 7470 7574 2067 6f65  e the output goe
+00000260: 730a 2020 2020 e904 0000 005a 0557 6869  s.    .....Z.Whi
+00000270: 7465 da00 7a09 7379 732e 6172 6776 3a54  te..z.sys.argv:T
+00000280: 7a02 3a20 7a0d 636f 6c6f 726d 6170 2066  z.: z.colormap f
+00000290: 6f72 207a 0820 7365 7420 746f 204e 2907  or z. set to N).
+000002a0: da0c 6275 696c 645f 6f75 7470 7574 da09  ..build_output..
+000002b0: 6d79 5f6f 7574 7075 7472 0200 0000 da03  my_outputr......
+000002c0: 7374 72da 0373 7973 da04 6172 6776 da05  str..sys..argv..
+000002d0: 6974 656d 7329 0572 0300 0000 7204 0000  items).r....r...
+000002e0: 0072 0500 0000 da03 6b65 79da 0576 616c  .r......key..val
+000002f0: 7565 a900 7211 0000 00fa 742f 5573 6572  ue..r.....t/User
+00000300: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
+00000310: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
+00000320: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
+00000330: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
+00000340: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
+00000350: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
+00000360: 6572 2f73 7263 2f64 6562 7567 2e70 79da  er/src/debug.py.
+00000370: 0664 6562 7567 3113 0000 0073 5c00 0000  .debug1....s\...
+00000380: 0407 0201 0201 0201 0201 1a01 04fb 0408  ................
+00000390: 0201 0201 0201 0201 0201 04fb 1007 0401  ................
+000003a0: 0201 0201 0201 0201 1801 06fb 0407 0201  ................
+000003b0: 0201 0201 0201 0201 04fb 1007 0401 0201  ................
+000003c0: 0201 0201 0201 0201 1601 02ff 06fb 0409  ................
+000003d0: 0201 0201 0201 0201 0201 08fb 7213 0000  ............r...
+000003e0: 0029 0a72 0c00 0000 da15 6d61 7074 6173  .).r......maptas
+000003f0: 6b65 722e 7372 632e 6f75 7470 7574 6cda  ker.src.outputl.
+00000400: 0373 7263 da07 6f75 7470 7574 6c72 0900  .src..outputlr..
+00000410: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
+00000420: 632e 6672 6d74 6874 6d6c 7202 0000 00da  c.frmthtmlr.....
+00000430: 0464 6963 74da 046c 6973 7472 1300 0000  .dict..listr....
+00000440: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000450: 1200 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000460: 0000 7308 0000 0008 0d12 010c 011e 03    ..s............
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/initparg.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/initparg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/kidapp.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/kidapp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 23 17:42:41 2023 UTC, .py size: 2397 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 918f 1c64 5d09 0000  o..........d]...
+00000000: 6f0d 0d0a 0000 0000 d4e8 3264 9f09 0000  o.........2d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 5a01 6402 6501 6a02 6403 6503  d.l.Z.d.e.j.d.e.
 00000040: 6604 6404 6405 8404 5a04 6401 5300 2906  f.d.d...Z.d.S.).
 00000050: e900 0000 004e da07 656c 656d 656e 74da  .....N..element.
 00000060: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
 00000070: 0000 0000 0b00 0000 0b00 0000 4300 0000  ............C...
@@ -21,57 +21,60 @@
 00000140: 0971 2d7c 0372 7164 0f7c 059b 0064 107c  .q-|.rqd.|...d.|
 00000150: 0364 0474 037c 0383 0164 1118 0085 0219  .d.t.|...d......
 00000160: 009b 009d 047d 037c 0472 8364 0f7c 059b  .....}.|.r.d.|..
 00000170: 0064 127c 0464 0474 037c 0483 0164 1118  .d.|.d.t.|...d..
 00000180: 0085 0219 009b 009d 047d 0464 137c 019b  .........}.d.|..
 00000190: 0064 147c 029b 0064 157c 079b 0064 0a7c  .d.|...d.|...d.|
 000001a0: 039b 0064 0a7c 049b 0064 169d 0b53 0029  ...d.|...d...S.)
-000001b0: 177a 8e0a 4765 7420 616e 7920 6173 736f  .z..Get any asso
-000001c0: 6369 6174 6564 204b 6964 2041 7070 6c69  ciated Kid Appli
-000001d0: 6361 7469 6f6e 2069 6e66 6f20 616e 6420  cation info and 
-000001e0: 7265 7475 726e 2069 740a 2020 2020 3a70  return it.    :p
-000001f0: 6172 616d 2065 6c65 6d65 6e74 3a20 726f  aram element: ro
-00000200: 6f74 2065 6c65 6d65 6e74 2074 6f20 7365  ot element to se
-00000210: 6172 6368 2066 6f72 203c 4b69 643e 0a20  arch for <Kid>. 
-00000220: 2020 203a 7265 7475 726e 3a20 7468 6520     :return: the 
-00000230: 4b69 6420 4170 7020 696e 666f 0a20 2020  Kid App info.   
-00000240: 20da 007a 1826 6e62 7370 3b26 6e62 7370   ..z.&nbsp;&nbsp
-00000250: 3b26 6e62 7370 3b26 6e62 7370 3b5a 034b  ;&nbsp;&nbsp;Z.K
-00000260: 6964 4eda 0370 6b67 5a04 766e 6d65 5a05  idN..pkgZ.vnmeZ.
-00000270: 7654 6172 6772 0100 0000 5a04 6665 6174  vTargr....Z.feat
-00000280: fa01 20e9 0100 0000 fa01 3d7a 022c 205a  .. .......=z., Z
-00000290: 056d 706c 7567 7a04 3c62 723e 7a09 4665  .mplugz.<br>z.Fe
-000002a0: 6174 7572 6573 3ae9 0200 0000 7a08 506c  atures:.....z.Pl
-000002b0: 7567 696e 733a 7a28 3c62 723e 266e 6273  ugins:z(<br>&nbs
-000002c0: 703b 266e 6273 703b 266e 6273 703b 5b4b  p;&nbsp;&nbsp;[K
-000002d0: 6964 2041 7070 3a20 5061 636b 6167 653a  id App: Package:
-000002e0: 7a0f 2c20 5665 7273 696f 6e20 4e61 6d65  z., Version Name
-000002f0: 3a7a 192c 2054 6172 6765 7420 416e 6472  :z., Target Andr
-00000300: 6f69 6420 5665 7273 696f 6e3a fa01 5d29  oid Version:..])
-00000310: 04da 0466 696e 64da 0474 6578 74da 0374  ...find..text..t
-00000320: 6167 da03 6c65 6e29 0b72 0200 0000 5a0b  ag..len).r....Z.
-00000330: 6b69 645f 7061 636b 6167 655a 0b6b 6964  kid_packageZ.kid
-00000340: 5f76 6572 7369 6f6e 5a0c 6b69 645f 6665  _versionZ.kid_fe
-00000350: 6174 7572 6573 5a0b 6b69 645f 706c 7567  aturesZ.kid_plug
-00000360: 696e 735a 0b66 6f75 725f 7370 6163 6573  insZ.four_spaces
-00000370: 5a0b 6b69 645f 656c 656d 656e 745a 0a6b  Z.kid_elementZ.k
-00000380: 6964 5f74 6172 6765 745a 0b6e 756d 5f66  id_targetZ.num_f
-00000390: 6561 7475 7265 5a0a 6e75 6d5f 706c 7567  eatureZ.num_plug
-000003a0: 696e da04 6974 656d a900 7210 0000 00fa  in..item..r.....
-000003b0: 752f 5573 6572 732f 6d69 6b72 7562 696e  u/Users/mikrubin
-000003c0: 2f4c 6962 7261 7279 2f43 6c6f 7564 5374  /Library/CloudSt
-000003d0: 6f72 6167 652f 476f 6f67 6c65 4472 6976  orage/GoogleDriv
-000003e0: 652d 6d69 6b72 7562 696e 4067 6d61 696c  e-mikrubin@gmail
-000003f0: 2e63 6f6d 2f4d 7920 4472 6976 652f 5079  .com/My Drive/Py
-00000400: 7468 6f6e 2f6d 6170 7461 736b 6572 2f6d  thon/maptasker/m
-00000410: 6170 7461 736b 6572 2f73 7263 2f6b 6964  aptasker/src/kid
-00000420: 6170 702e 7079 da0b 6765 745f 6b69 645f  app.py..get_kid_
-00000430: 6170 7011 0000 0073 2c00 0000 1006 0401  app....s,.......
-00000440: 0a01 0801 0401 0c02 0c01 0c01 0801 0802  ................
-00000450: 0a01 1c01 0a01 0a01 1c01 0801 0280 0401  ................
-00000460: 2001 0401 2001 2402 7212 0000 0029 05da   ... .$.r....)..
-00000470: 1578 6d6c 2e65 7472 6565 2e45 6c65 6d65  .xml.etree.Eleme
-00000480: 6e74 5472 6565 da03 786d 6cda 0565 7472  ntTree..xml..etr
-00000490: 6565 da03 7374 7272 1200 0000 7210 0000  ee..strr....r...
-000004a0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-000004b0: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
-000004c0: 0000 0008 0d18 03                        .......
+000001b0: 177a 9a0a 2020 2020 4765 7420 616e 7920  .z..    Get any 
+000001c0: 6173 736f 6369 6174 6564 204b 6964 2041  associated Kid A
+000001d0: 7070 6c69 6361 7469 6f6e 2069 6e66 6f20  pplication info 
+000001e0: 616e 6420 7265 7475 726e 2069 740a 2020  and return it.  
+000001f0: 2020 2020 2020 3a70 6172 616d 2065 6c65        :param ele
+00000200: 6d65 6e74 3a20 726f 6f74 2065 6c65 6d65  ment: root eleme
+00000210: 6e74 2074 6f20 7365 6172 6368 2066 6f72  nt to search for
+00000220: 203c 4b69 643e 0a20 2020 2020 2020 203a   <Kid>.        :
+00000230: 7265 7475 726e 3a20 7468 6520 4b69 6420  return: the Kid 
+00000240: 4170 7020 696e 666f 0a20 2020 20da 007a  App info.    ..z
+00000250: 1826 6e62 7370 3b26 6e62 7370 3b26 6e62  .&nbsp;&nbsp;&nb
+00000260: 7370 3b26 6e62 7370 3b5a 034b 6964 4eda  sp;&nbsp;Z.KidN.
+00000270: 0370 6b67 5a04 766e 6d65 5a05 7654 6172  .pkgZ.vnmeZ.vTar
+00000280: 6772 0100 0000 5a04 6665 6174 fa01 20e9  gr....Z.feat.. .
+00000290: 0100 0000 fa01 3d7a 022c 205a 056d 706c  ......=z., Z.mpl
+000002a0: 7567 7a04 3c62 723e 7a09 4665 6174 7572  ugz.<br>z.Featur
+000002b0: 6573 3ae9 0200 0000 7a08 506c 7567 696e  es:.....z.Plugin
+000002c0: 733a 7a28 3c62 723e 266e 6273 703b 266e  s:z(<br>&nbsp;&n
+000002d0: 6273 703b 266e 6273 703b 5b4b 6964 2041  bsp;&nbsp;[Kid A
+000002e0: 7070 3a20 5061 636b 6167 653a 7a0f 2c20  pp: Package:z., 
+000002f0: 5665 7273 696f 6e20 4e61 6d65 3a7a 192c  Version Name:z.,
+00000300: 2054 6172 6765 7420 416e 6472 6f69 6420   Target Android 
+00000310: 5665 7273 696f 6e3a fa01 5d29 04da 0466  Version:..])...f
+00000320: 696e 64da 0474 6578 74da 0374 6167 da03  ind..text..tag..
+00000330: 6c65 6e29 0b72 0200 0000 5a0b 6b69 645f  len).r....Z.kid_
+00000340: 7061 636b 6167 655a 0b6b 6964 5f76 6572  packageZ.kid_ver
+00000350: 7369 6f6e 5a0c 6b69 645f 6665 6174 7572  sionZ.kid_featur
+00000360: 6573 5a0b 6b69 645f 706c 7567 696e 735a  esZ.kid_pluginsZ
+00000370: 0b66 6f75 725f 7370 6163 6573 5a0b 6b69  .four_spacesZ.ki
+00000380: 645f 656c 656d 656e 745a 0a6b 6964 5f74  d_elementZ.kid_t
+00000390: 6172 6765 745a 0b6e 756d 5f66 6561 7475  argetZ.num_featu
+000003a0: 7265 5a0a 6e75 6d5f 706c 7567 696e da04  reZ.num_plugin..
+000003b0: 6974 656d a900 7210 0000 00fa 752f 5573  item..r.....u/Us
+000003c0: 6572 732f 6d69 6b72 7562 696e 2f4c 6962  ers/mikrubin/Lib
+000003d0: 7261 7279 2f43 6c6f 7564 5374 6f72 6167  rary/CloudStorag
+000003e0: 652f 476f 6f67 6c65 4472 6976 652d 6d69  e/GoogleDrive-mi
+000003f0: 6b72 7562 696e 4067 6d61 696c 2e63 6f6d  krubin@gmail.com
+00000400: 2f4d 7920 4472 6976 652f 5079 7468 6f6e  /My Drive/Python
+00000410: 2f6d 6170 7461 736b 6572 2f6d 6170 7461  /maptasker/mapta
+00000420: 736b 6572 2f73 7263 2f6b 6964 6170 702e  sker/src/kidapp.
+00000430: 7079 da0b 6765 745f 6b69 645f 6170 7011  py..get_kid_app.
+00000440: 0000 0073 3e00 0000 1006 0401 0a01 0801  ...s>...........
+00000450: 0401 0c02 0c01 0c01 0801 0802 0a01 1c01  ................
+00000460: 0a01 0a01 1c01 0801 0280 0401 2001 0401  ............ ...
+00000470: 2001 0803 0201 04ff 0202 04fe 0202 04fe   ...............
+00000480: 0202 06fe 02ff 7212 0000 0029 05da 1664  ......r....)...d
+00000490: 6566 7573 6564 786d 6c2e 456c 656d 656e  efusedxml.Elemen
+000004a0: 7454 7265 65da 0a64 6566 7573 6564 786d  tTree..defusedxm
+000004b0: 6cda 0b45 6c65 6d65 6e74 5472 6565 da03  l..ElementTree..
+000004c0: 7374 7272 1200 0000 7210 0000 0072 1000  strr....r....r..
+000004d0: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
+000004e0: 6f64 756c 653e 0100 0000 7304 0000 0008  odule>....s.....
+000004f0: 0d18 03                                  ...
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/mapit.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/mapit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 17:33:48 2023 UTC, .py size: 15342 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,325 +1,328 @@
-00000000: 6f0d 0d0a 0000 0000 7c5f 2c64 ee3b 0000  o.......|_,d.;..
+00000000: 6f0d 0d0a 0000 0000 6d62 3d64 713c 0000  o.......mb=dq<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000e 0000 0040 0000 0073 3c01 0000 6400  .....@...s<...d.
+00000020: 000e 0000 0040 0000 0073 3a01 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6401 6c09 6d0a 0200 0100 6d0b  ..d.d.l.m.....m.
 00000070: 5a0c 0100 6400 6401 6c0d 6d0a 0200 0100  Z...d.d.l.m.....
 00000080: 6d0e 5a0f 0100 6400 6401 6c10 6d0a 0200  m.Z...d.d.l.m...
 00000090: 0100 6d11 5a11 0100 6400 6401 6c12 6d0a  ..m.Z...d.d.l.m.
 000000a0: 0200 0100 6d13 5a14 0100 6400 6404 6c15  ....m.Z...d.d.l.
 000000b0: 6d16 5a16 0100 6400 6405 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
 000000c0: 0100 6400 6406 6c19 6d1a 5a1a 0100 6407  ..d.d.l.m.Z...d.
-000000d0: 6503 6a1b 6a1c 6a1c 6408 6503 6a1b 6a1c  e.j.j.j.d.e.j.j.
-000000e0: 6a1d 6409 6507 651e 1900 640a 6508 651e  j.d.e.e...d.e.e.
-000000f0: 6507 6503 6a1b 6a1c 6a1d 1900 6602 1900  e.e.j.j.j...f...
-00000100: 640b 6401 660a 640c 640d 8404 5a1f 6409  d.d.f.d.d...Z.d.
-00000110: 6507 651e 1900 640e 651e 640f 651e 640b  e.e...d.e.d.e.d.
-00000120: 6401 6608 6410 6411 8404 5a20 6412 651e  d.f.d.d...Z d.e.
-00000130: 6413 651e 6407 6503 6a1b 6408 6503 6a1b  d.e.d.e.j.d.e.j.
-00000140: 6409 6521 640a 6522 640b 6401 660e 6414  d.e!d.e"d.d.f.d.
-00000150: 6415 8404 5a23 0900 640b 6524 6602 6416  d...Z#..d.e$f.d.
-00000160: 6417 8404 5a25 6401 5300 2918 e900 0000  d...Z%d.S.).....
-00000170: 004e 2901 da06 6765 7463 7764 2902 da04  .N)...getcwd)...
-00000180: 4c69 7374 da04 4469 6374 2901 da0f 6469  List..Dict)...di
-00000190: 7370 6c61 795f 6361 7665 6174 7329 01da  splay_caveats)..
-000001a0: 0f67 6574 5f70 7265 6665 7265 6e63 6573  .get_preferences
-000001b0: 2901 da06 6c6f 6767 6572 da04 7472 6565  )...logger..tree
-000001c0: da04 726f 6f74 da0b 6f75 7470 7574 5f6c  ..root..output_l
-000001d0: 6973 74da 1061 6c6c 5f74 6173 6b65 725f  ist..all_tasker_
-000001e0: 6974 656d 73da 0672 6574 7572 6e63 0400  items..returnc..
-000001f0: 0000 0000 0000 0000 0000 0500 0000 0300  ................
-00000200: 0000 4300 0000 735a 0000 007c 00a0 00a1  ..C...sZ...|....
-00000210: 0044 005d 067d 047c 04a0 01a1 0001 0071  .D.].}.|.......q
-00000220: 047c 0364 0119 00a0 01a1 0001 007c 0364  .|.d.........|.d
-00000230: 0219 00a0 01a1 0001 007c 0364 0319 00a0  .........|.d....
-00000240: 01a1 0001 007c 0364 0419 00a0 01a1 0001  .....|.d........
-00000250: 007c 01a0 01a1 0001 007c 02a0 01a1 0001  .|.......|......
-00000260: 0064 0553 0029 0661 1701 0000 0a20 2020  .d.S.).a.....   
-00000270: 2043 6c65 616e 2075 7020 6f75 7220 6d65   Clean up our me
-00000280: 6d6f 7279 2068 6f67 730a 2020 2020 2020  mory hogs.      
-00000290: 2020 3a70 6172 616d 2074 7265 653a 2078    :param tree: x
-000002a0: 6d6c 2074 7265 6520 746f 2065 6d70 7479  ml tree to empty
-000002b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000002c0: 726f 6f74 3a20 726f 6f74 2078 6d6c 2074  root: root xml t
-000002d0: 6861 7420 7761 7320 7061 7273 6564 2066  hat was parsed f
-000002e0: 726f 6d20 6261 636b 7570 2066 696c 650a  rom backup file.
-000002f0: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-00000300: 7574 7075 745f 6c69 7374 3a20 6c69 7374  utput_list: list
-00000310: 206f 6620 6f75 7470 7574 206c 696e 6573   of output lines
-00000320: 2074 6f20 636c 6561 720a 2020 2020 2020   to clear.      
-00000330: 2020 3a70 6172 616d 2061 6c6c 5f74 6173    :param all_tas
-00000340: 6b65 725f 6974 656d 733a 2041 6c6c 2050  ker_items: All P
-00000350: 726f 6a65 6374 732f 5072 6f66 696c 6573  rojects/Profiles
-00000360: 2f54 6173 6b73 2f53 6365 6e65 730a 2020  /Tasks/Scenes.  
-00000370: 2020 2020 2020 3a72 6574 7572 6e3a 0a20        :return:. 
-00000380: 2020 205a 0c61 6c6c 5f70 726f 6a65 6374     Z.all_project
-00000390: 735a 0c61 6c6c 5f70 726f 6669 6c65 735a  sZ.all_profilesZ
-000003a0: 0961 6c6c 5f74 6173 6b73 5a0a 616c 6c5f  .all_tasksZ.all_
-000003b0: 7363 656e 6573 4e29 02da 0469 7465 72da  scenesN)...iter.
-000003c0: 0563 6c65 6172 2905 7208 0000 0072 0900  .clear).r....r..
-000003d0: 0000 720a 0000 0072 0b00 0000 da04 656c  ..r....r......el
-000003e0: 656d a900 7210 0000 00fa 742f 5573 6572  em..r.....t/User
-000003f0: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
-00000400: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
-00000410: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
-00000420: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
-00000430: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
-00000440: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
-00000450: 6572 2f73 7263 2f6d 6170 6974 2e70 79da  er/src/mapit.py.
-00000460: 0f63 6c65 616e 5f75 705f 6d65 6d6f 7279  .clean_up_memory
-00000470: 3700 0000 7312 0000 000c 0e0a 010c 010c  7...s...........
-00000480: 010c 010c 0108 0108 0104 0172 1200 0000  ...........r....
-00000490: da0d 6d79 5f6f 7574 7075 745f 6469 72da  ..my_output_dir.
-000004a0: 0c6d 795f 6669 6c65 5f6e 616d 6563 0300  .my_file_namec..
-000004b0: 0000 0000 0000 0000 0000 0a00 0000 0800  ................
-000004c0: 0000 4300 0000 73c6 0000 0074 00a0 0164  ..C...s....t...d
-000004d0: 017c 019b 009d 02a1 0101 0074 027c 017c  .|.........t.|.|
-000004e0: 0217 0064 0283 028f 457d 037c 0044 005d  ...d....E}.|.D.]
-000004f0: 3a7d 047c 04a0 0364 03a1 017d 057c 0564  :}.|...d...}.|.d
-00000500: 046b 0372 457c 047c 0564 0517 0064 0685  .k.rE|.|.d...d..
-00000510: 0219 00a0 0464 07a1 017d 067c 0664 0819  .....d...}.|.d..
-00000520: 007d 077c 0464 067c 0585 0219 007c 0717  .}.|.d.|.....|..
-00000530: 0064 0917 007c 047c 0564 0517 0074 057c  .d...|.|.d...t.|
-00000540: 0783 0117 0064 0685 0219 0017 007d 087c  .....d.......}.|
-00000550: 087d 096e 027c 047d 097c 03a0 067c 09a1  .}.n.|.}.|...|..
-00000560: 0101 0071 1257 0064 0604 0004 0083 0301  ...q.W.d........
-00000570: 006e 0831 0073 5777 0101 0001 0001 0059  .n.1.sWw.......Y
-00000580: 0001 0074 00a0 0164 0aa1 0101 0064 0653  ...t...d.....d.S
-00000590: 0029 0b61 0c01 0000 0a20 2020 2077 7269  .).a.....    wri
-000005a0: 7465 5f6f 7574 5f74 6865 5f66 696c 653a  te_out_the_file:
-000005b0: 2077 6520 6861 7665 2061 206c 6973 7420   we have a list 
-000005c0: 6f66 206f 7574 7075 7420 6c69 6e65 732e  of output lines.
-000005d0: 2020 5772 6974 6520 7468 656d 206f 7574    Write them out
-000005e0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000005f0: 206f 7574 7075 745f 6c69 7374 3a20 6c69   output_list: li
-00000600: 7374 206f 6620 616c 6c20 6f75 7470 7574  st of all output
-00000610: 206c 696e 6573 2067 656e 6572 6174 6564   lines generated
-00000620: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000630: 6d79 5f6f 7574 7075 745f 6469 723a 2064  my_output_dir: d
-00000640: 6972 6563 746f 7279 2074 6f20 6f75 7470  irectory to outp
-00000650: 7574 2074 6f0a 2020 2020 2020 2020 3a70  ut to.        :p
-00000660: 6172 616d 206d 795f 6669 6c65 5f6e 616d  aram my_file_nam
-00000670: 653a 206e 616d 6520 6f66 2066 696c 6520  e: name of file 
-00000680: 746f 2075 7365 0a20 2020 2020 2020 203a  to use.        :
-00000690: 7265 7475 726e 3a20 6e6f 7468 696e 670a  return: nothing.
-000006a0: 2020 2020 7a27 4675 6e63 7469 6f6e 2045      z'Function E
-000006b0: 6e74 7279 3a20 7772 6974 655f 6f75 745f  ntry: write_out_
-000006c0: 7468 655f 6669 6c65 2064 6972 3ada 0177  the_file dir:..w
-000006d0: 7a08 4163 7469 6f6e 3a20 e9ff ffff ffe9  z.Action: ......
-000006e0: 0800 0000 4efa 0120 7201 0000 00fa 013a  ....N.. r......:
-000006f0: 7a21 4675 6e63 7469 6f6e 2045 7869 743a  z!Function Exit:
-00000700: 2077 7269 7465 5f6f 7574 5f74 6865 5f66   write_out_the_f
-00000710: 696c 6529 0772 0700 0000 da04 696e 666f  ile).r......info
-00000720: da04 6f70 656e da04 6669 6e64 da05 7370  ..open..find..sp
-00000730: 6c69 74da 036c 656e da05 7772 6974 6529  lit..len..write)
-00000740: 0a72 0a00 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000750: 5a08 6f75 745f 6669 6c65 da04 6974 656d  Z.out_file..item
-00000760: 5a0f 6163 7469 6f6e 5f70 6f73 6974 696f  Z.action_positio
-00000770: 6e5a 1261 6374 696f 6e5f 6e75 6d62 6572  nZ.action_number
-00000780: 5f6c 6973 745a 0d61 6374 696f 6e5f 6e75  _listZ.action_nu
-00000790: 6d62 6572 5a04 7465 6d70 5a0b 6f75 7470  mberZ.tempZ.outp
-000007a0: 7574 5f6c 696e 6572 1000 0000 7210 0000  ut_liner....r...
-000007b0: 0072 1100 0000 da12 7772 6974 655f 6f75  .r......write_ou
-000007c0: 745f 7468 655f 6669 6c65 5300 0000 732c  t_the_fileS...s,
-000007d0: 0000 0010 0a10 0108 010a 0208 0116 0108  ................
-000007e0: 010a 0202 0102 ff02 0202 fe16 0302 fd02  ................
-000007f0: ff06 0604 020c 0102 f11c ff0a 1104 0172  ...............r
-00000800: 2100 0000 da04 6e61 6d65 da14 7072 6f66  !.....name..prof
-00000810: 696c 655f 6f72 5f74 6173 6b5f 6e61 6d65  ile_or_task_name
-00000820: 6306 0000 0000 0000 0000 0000 0007 0000  c...............
-00000830: 0005 0000 0043 0000 0073 4600 0000 7c04  .....C...sF...|.
-00000840: a000 a100 0100 7c00 9b00 6401 7c01 9b00  ......|...d.|...
-00000850: 6402 9d04 7d06 7401 7c06 8301 0100 7402  d...}.t.|.....t.
-00000860: a003 7c06 a101 0100 7404 7c02 7c03 7c04  ..|.....t.|.|.|.
-00000870: 7c05 8304 0100 7405 a006 6403 a101 0100  |.....t...d.....
-00000880: 6404 5300 2905 61f6 0100 000a 2020 2020  d.S.).a.....    
-00000890: 436c 6561 6e75 7020 6d65 6d6f 7279 2061  Cleanup memory a
-000008a0: 6e64 206c 6574 2075 7365 7220 6b6e 6f77  nd let user know
-000008b0: 2074 6865 7265 2077 6173 206e 6f20 6d61   there was no ma
-000008c0: 7463 6820 666f 756e 6420 666f 7220 5461  tch found for Ta
-000008d0: 736b 2f50 726f 6669 6c65 0a20 2020 2020  sk/Profile.     
-000008e0: 2020 203a 7061 7261 6d20 6e61 6d65 3a20     :param name: 
-000008f0: 7468 6520 6e61 6d65 2074 6f20 6164 6420  the name to add 
-00000900: 746f 2074 6865 206c 6f67 2f70 7269 6e74  to the log/print
-00000910: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
-00000920: 3a70 6172 616d 2070 726f 6669 6c65 5f6f  :param profile_o
-00000930: 725f 7461 736b 5f6e 616d 653a 206e 616d  r_task_name: nam
-00000940: 6520 6f66 2074 6865 2050 726f 6669 6c65  e of the Profile
-00000950: 206f 7220 5461 736b 2074 6f20 636c 6561   or Task to clea
-00000960: 6e0a 2020 2020 2020 2020 3a70 6172 616d  n.        :param
-00000970: 2074 7265 653a 2078 6d6c 2074 7265 6520   tree: xml tree 
-00000980: 746f 2063 6c65 6172 0a20 2020 2020 2020  to clear.       
-00000990: 203a 7061 7261 6d20 726f 6f74 3a20 726f   :param root: ro
-000009a0: 6f74 206f 6620 786d 6c20 7061 7273 6564  ot of xml parsed
-000009b0: 2066 726f 6d20 6669 6c65 2074 6f20 636c   from file to cl
-000009c0: 6561 720a 2020 2020 2020 2020 3a70 6172  ear.        :par
-000009d0: 616d 206f 7574 7075 745f 6c69 7374 3a20  am output_list: 
-000009e0: 6c69 7374 206f 6620 6f75 7470 7574 206c  list of output l
-000009f0: 696e 6573 2074 6f20 656d 7074 790a 2020  ines to empty.  
-00000a00: 2020 2020 2020 3a70 6172 616d 2061 6c6c        :param all
-00000a10: 5f74 6173 6b65 725f 6974 656d 733a 2061  _tasker_items: a
-00000a20: 6c6c 2054 6173 6b65 7220 5072 6f6a 6563  ll Tasker Projec
-00000a30: 7473 2f50 726f 6669 6c65 732f 5461 736b  ts/Profiles/Task
-00000a40: 732f 5363 656e 6573 2074 6f20 636c 6561  s/Scenes to clea
-00000a50: 720a 2020 2020 2020 2020 3a72 7479 7065  r.        :rtype
-00000a60: 3a20 636f 6c6f 7273 2c20 7275 6e74 696d  : colors, runtim
-00000a70: 6520 6172 6775 6d65 6e74 732c 0a20 2020  e arguments,.   
-00000a80: 2072 1800 0000 7a0c 206e 6f74 2066 6f75   r....z. not fou
-00000a90: 6e64 2121 e905 0000 004e 2907 720e 0000  nd!!.....N).r...
-00000aa0: 00da 0570 7269 6e74 7207 0000 00da 0564  ...printr......d
-00000ab0: 6562 7567 7212 0000 00da 0373 7973 da04  ebugr......sys..
-00000ac0: 6578 6974 2907 7222 0000 0072 2300 0000  exit).r"...r#...
-00000ad0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000ae0: 0b00 0000 5a0d 6572 726f 725f 6d65 7373  ....Z.error_mess
-00000af0: 6167 6572 1000 0000 7210 0000 0072 1100  ager....r....r..
-00000b00: 0000 da11 636c 6561 6e5f 7570 5f61 6e64  ....clean_up_and
-00000b10: 5f65 7869 7476 0000 0073 0c00 0000 0813  _exitv...s......
-00000b20: 1001 0801 0a01 0e01 0e01 7229 0000 0063  ..........r)...c
-00000b30: 0000 0000 0000 0000 0000 0000 1100 0000  ................
-00000b40: 0a00 0000 4300 0000 7338 0200 0067 0067  ....C...s8...g.g
-00000b50: 0067 0067 0066 045c 047d 007d 017d 027d  .g.g.f.\.}.}.}.}
-00000b60: 0374 00a0 017c 01a1 015c 097d 047d 057d  .t...|...\.}.}.}
-00000b70: 067d 077d 017d 087d 097d 0a7d 0b7c 0564  .}.}.}.}.}.}.|.d
-00000b80: 0119 0072 2374 027c 017c 057c 047c 0b83  ...r#t.|.|.|.|..
-00000b90: 0401 0074 03a0 047c 017c 007c 027c 057c  ...t...|.|.|.|.|
-00000ba0: 067c 077c 047c 0ba1 087d 007c 0564 0219  .|.|.|...}.|.d..
-00000bb0: 0072 427c 0664 0319 0073 4274 0564 047c  .rB|.d...sBt.d.|
-00000bc0: 0564 0219 007c 087c 097c 017c 0b83 0601  .d...|.|.|.|....
-00000bd0: 007c 0564 0519 0072 557c 0664 0619 0073  .|.d...rU|.d...s
-00000be0: 5574 0564 077c 0564 0519 007c 087c 097c  Ut.d.|.d...|.|.|
-00000bf0: 017c 0b83 0601 007c 0564 0819 0073 777c  .|.....|.d...sw|
-00000c00: 0564 0219 0073 777c 0564 0519 0073 7774  .d...sw|.d...swt
-00000c10: 06a0 077c 017c 037c 007c 057c 067c 077c  ...|.|.|.|.|.|.|
-00000c20: 047c 0ba1 0801 0074 06a0 087c 017c 037c  .|.....t...|.|.|
-00000c30: 027c 067c 047c 05a1 0601 007c 0564 0819  .|.|.|.....|.d..
-00000c40: 0072 9a7c 0664 0919 0073 9a7c 0564 0519  .r.|.d...s.|.d..
-00000c50: 0072 877c 0664 0619 0072 9a7c 0564 0219  .r.|.d...r.|.d..
-00000c60: 0072 8f7c 0664 0319 0072 9a74 0564 0a7c  .r.|.d...r.t.d.|
-00000c70: 0564 0819 007c 087c 097c 017c 0b83 0601  .d...|.|.|.|....
-00000c80: 0074 097c 017c 057c 0483 0301 0064 0b7d  .t.|.|.|.....d.}
-00000c90: 0c74 0aa0 0b7c 047c 057c 0164 0c7c 0ca1  .t...|.|.|.d.|..
-00000ca0: 0501 0074 0c83 007d 0d74 0da0 0e64 0d7c  ...t...}.t...d.|
-00000cb0: 0d9b 009d 02a1 0101 007c 0d64 0075 0072  .........|.d.u.r
-00000cc0: d164 0e7d 0c74 0da0 0e7c 0ca1 0101 0074  .d.}.t...|.....t
-00000cd0: 0f7c 0c83 0101 0074 107c 087c 097c 017c  .|.....t.|.|.|.|
-00000ce0: 0b83 0401 0074 11a0 1264 0fa1 0101 0064  .....t...d.....d
-00000cf0: 107d 0e74 137c 017c 0d7c 0e83 0301 0074  .}.t.|.|.|.....t
-00000d00: 107c 087c 097c 017c 0b83 0401 0074 0da0  .|.|.|.|.....t..
-00000d10: 0e64 11a1 0101 0064 0c7d 0f7a 0e74 146a  .d.....d.}.z.t.j
-00000d20: 1564 127c 0d9b 007c 0e9b 009d 0364 0f64  .d.|...|.....d.d
-00000d30: 138d 0201 0057 006e 2004 0074 1690 0179  .....W.n ..t...y
-00000d40: 1501 007d 1001 007a 1364 147d 0c74 0f7c  ...}...z.d.}.t.|
-00000d50: 0c83 0101 0074 0da0 0e7c 0ca1 0101 0064  .....t...|.....d
-00000d60: 157d 0f57 0059 0064 007d 107e 106e 0564  .}.W.Y.d.}.~.n.d
-00000d70: 007d 107e 1077 0177 0074 0f64 1683 0101  .}.~.w.w.t.d....
-00000d80: 007c 0f53 0029 174e 5a13 6469 7370 6c61  .|.S.).NZ.displa
-00000d90: 795f 7072 6566 6572 656e 6365 735a 1373  y_preferencesZ.s
-00000da0: 696e 676c 655f 7072 6f6a 6563 745f 6e61  ingle_project_na
-00000db0: 6d65 5a14 7369 6e67 6c65 5f70 726f 6a65  meZ.single_proje
-00000dc0: 6374 5f66 6f75 6e64 5a07 5072 6f6a 6563  ct_foundZ.Projec
-00000dd0: 745a 1373 696e 676c 655f 7072 6f66 696c  tZ.single_profil
-00000de0: 655f 6e61 6d65 5a14 7369 6e67 6c65 5f70  e_nameZ.single_p
-00000df0: 726f 6669 6c65 5f66 6f75 6e64 5a07 5072  rofile_foundZ.Pr
-00000e00: 6f66 696c 655a 1073 696e 676c 655f 7461  ofileZ.single_ta
-00000e10: 736b 5f6e 616d 655a 1173 696e 676c 655f  sk_nameZ.single_
-00000e20: 7461 736b 5f66 6f75 6e64 5a04 5461 736b  task_foundZ.Task
-00000e30: 7a0f 3c2f 626f 6479 3e0a 3c2f 6874 6d6c  z.</body>.</html
-00000e40: 3e72 0100 0000 7a11 6f75 7470 7574 2064  >r....z.output d
-00000e50: 6972 6563 746f 7279 3a7a 3c4d 6170 5461  irectory:z<MapTa
-00000e60: 736b 6572 2063 616e 6365 6c6c 6564 2e20  sker cancelled. 
-00000e70: 2041 6e20 6572 726f 7220 6f63 6375 7272   An error occurr
-00000e80: 6564 2e20 2050 726f 6772 616d 2063 616e  ed.  Program can
-00000e90: 6365 6c6c 6564 2ee9 0200 0000 7a0f 2f4d  celled......z./M
-00000ea0: 6170 5461 736b 6572 2e68 746d 6c7a 204d  apTasker.htmlz M
-00000eb0: 6170 5461 736b 6572 2070 726f 6772 616d  apTasker program
-00000ec0: 2065 6e64 6564 206e 6f72 6d61 6c6c 797a   ended normallyz
-00000ed0: 0766 696c 653a 2f2f 2901 da03 6e65 777a  .file://)...newz
-00000ee0: 4745 7272 6f72 3a20 4661 696c 6564 2074  GError: Failed t
-00000ef0: 6f20 6f70 656e 206f 7574 7075 7420 696e  o open output in
-00000f00: 2062 726f 7773 6572 3a20 796f 7572 2062   browser: your b
-00000f10: 726f 7773 6572 2069 7320 6e6f 7420 7375  rowser is not su
-00000f20: 7070 6f72 7465 642e e901 0000 007a 4259  pported......zBY
-00000f30: 6f75 2063 616e 2066 696e 6420 274d 6170  ou can find 'Map
-00000f40: 5461 736b 6572 2e68 746d 6c27 2069 6e20  Tasker.html' in 
-00000f50: 7468 6520 6375 7272 656e 7420 666f 6c64  the current fold
-00000f60: 6572 2e20 2050 726f 6772 616d 2065 6e64  er.  Program end
-00000f70: 2e29 17da 0a69 6e69 7469 616c 697a 655a  .)...initializeZ
-00000f80: 0873 7461 7274 5f75 7072 0600 0000 da08  .start_upr......
-00000f90: 7072 6f6a 6563 7473 5a23 7072 6f63 6573  projectsZ#proces
-00000fa0: 735f 7072 6f6a 6563 7473 5f61 6e64 5f74  s_projects_and_t
-00000fb0: 6865 6972 5f70 726f 6669 6c65 7372 2900  heir_profilesr).
-00000fc0: 0000 da0d 7370 6563 6961 6c5f 7461 736b  ....special_task
-00000fd0: 735a 2370 726f 6365 7373 5f74 6173 6b73  sZ#process_tasks
-00000fe0: 5f6e 6f74 5f63 616c 6c65 645f 6279 5f70  _not_called_by_p
-00000ff0: 726f 6669 6c65 5a22 7072 6f63 6573 735f  rofileZ"process_
-00001000: 6d69 7373 696e 675f 7461 736b 735f 616e  missing_tasks_an
-00001010: 645f 7072 6f66 696c 6573 7205 0000 00da  d_profilesr.....
-00001020: 0c62 7569 6c64 5f6f 7574 7075 745a 096d  .build_outputZ.m
-00001030: 795f 6f75 7470 7574 7202 0000 0072 0700  y_outputr....r..
-00001040: 0000 7226 0000 0072 2500 0000 7212 0000  ..r&...r%...r...
-00001050: 0072 2700 0000 7228 0000 0072 2100 0000  .r'...r(...r!...
-00001060: da0a 7765 6262 726f 7773 6572 721b 0000  ..webbrowserr...
-00001070: 00da 0945 7863 6570 7469 6f6e 2911 5a0b  ...Exception).Z.
-00001080: 666f 756e 645f 7461 736b 7372 0a00 0000  found_tasksr....
-00001090: 5a19 7072 6f6a 6563 7473 5f77 6974 686f  Z.projects_witho
-000010a0: 7574 5f70 726f 6669 6c65 735a 1670 726f  ut_profilesZ.pro
-000010b0: 6a65 6374 735f 7769 7468 5f6e 6f5f 7461  jects_with_no_ta
-000010c0: 736b 735a 0863 6f6c 6f72 6d61 705a 0c70  sksZ.colormapZ.p
-000010d0: 726f 6772 616d 5f61 7267 735a 0b66 6f75  rogram_argsZ.fou
-000010e0: 6e64 5f69 7465 6d73 5a07 6865 6164 696e  nd_itemsZ.headin
-000010f0: 6772 0800 0000 7209 0000 00da 0866 696c  gr....r......fil
-00001100: 656e 616d 6572 0b00 0000 5a09 6572 726f  enamer....Z.erro
-00001110: 725f 6d73 6772 1300 0000 7214 0000 005a  r_msgr....r....Z
-00001120: 056d 795f 7263 da01 6572 1000 0000 7210  .my_rc..er....r.
-00001130: 0000 0072 1100 0000 da09 6d61 7069 745f  ...r......mapit_
-00001140: 616c 6cc1 0000 0073 f600 0000 0203 0201  all....s........
-00001150: 0201 0201 0cfc 0812 02f6 0201 0201 0201  ................
-00001160: 0201 0201 0201 0201 0201 0201 080d 0201  ................
-00001170: 0201 0201 0201 0201 04fc 040a 0201 0201  ................
-00001180: 0201 0201 0201 0201 0201 0201 04f8 100c  ................
-00001190: 0201 0201 0601 0201 0201 0201 0201 04fa  ................
-000011a0: 1009 0201 0201 0601 0201 0201 0201 0201  ................
-000011b0: 04fa 060d 02ff 0602 02fe 0603 02fd 0405  ................
-000011c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000011d0: 04f8 040e 0201 0201 0201 0201 0201 0201  ................
-000011e0: 04fa 060b 02ff 0602 02fe 0604 02fc 0605  ................
-000011f0: 02fb 0608 02f8 0609 02f7 020c 0201 0601  ................
-00001200: 0201 0201 0201 0201 04fa 0c0d 0403 1201  ................
-00001210: 0604 1001 0801 0401 0a01 0801 0e01 0a01  ................
-00001220: 0402 0c02 0e03 0a03 0401 0201 1c01 1001  ................
-00001230: 0202 02ff 0803 0a01 1001 0880 02fa 0807  ................
-00001240: 0401 7235 0000 0029 2672 2700 0000 7231  ..r5...)&r'...r1
-00001250: 0000 005a 1578 6d6c 2e65 7472 6565 2e45  ...Z.xml.etree.E
-00001260: 6c65 6d65 6e74 5472 6565 5a03 786d 6cda  lementTreeZ.xml.
-00001270: 026f 7372 0200 0000 da06 7479 7069 6e67  .osr......typing
-00001280: 7203 0000 0072 0400 0000 5a15 6d61 7074  r....r....Z.mapt
-00001290: 6173 6b65 722e 7372 632e 6f75 7470 7574  asker.src.output
-000012a0: 6cda 0373 7263 5a07 6f75 7470 7574 6c72  l..srcZ.outputlr
-000012b0: 3000 0000 5a16 6d61 7074 6173 6b65 722e  0...Z.maptasker.
-000012c0: 7372 632e 7072 6f67 696e 6974 5a08 7072  src.proginitZ.pr
-000012d0: 6f67 696e 6974 722d 0000 005a 166d 6170  oginitr-...Z.map
-000012e0: 7461 736b 6572 2e73 7263 2e70 726f 6a65  tasker.src.proje
-000012f0: 6374 7372 2e00 0000 5a16 6d61 7074 6173  ctsr....Z.maptas
-00001300: 6b65 722e 7372 632e 7461 736b 756e 6971  ker.src.taskuniq
-00001310: 5a08 7461 736b 756e 6971 722f 0000 005a  Z.taskuniqr/...Z
-00001320: 156d 6170 7461 736b 6572 2e73 7263 2e63  .maptasker.src.c
-00001330: 6176 6561 7473 7205 0000 005a 156d 6170  aveatsr....Z.map
-00001340: 7461 736b 6572 2e73 7263 2e70 7265 6665  tasker.src.prefe
-00001350: 7273 7206 0000 005a 166d 6170 7461 736b  rsr....Z.maptask
-00001360: 6572 2e73 7263 2e73 7973 636f 6e73 7472  er.src.sysconstr
-00001370: 0700 0000 5a05 6574 7265 655a 0b45 6c65  ....Z.etreeZ.Ele
-00001380: 6d65 6e74 5472 6565 5a07 456c 656d 656e  mentTreeZ.Elemen
-00001390: 74da 0373 7472 7212 0000 0072 2100 0000  t..strr....r!...
-000013a0: da04 6c69 7374 da04 6469 6374 7229 0000  ..list..dictr)..
-000013b0: 00da 0369 6e74 7235 0000 0072 1000 0000  ...intr5...r....
-000013c0: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-000013d0: 083c 6d6f 6475 6c65 3e01 0000 0073 6200  .<module>....sb.
-000013e0: 0000 0820 0801 0801 0c01 1001 1202 1201  ... ............
-000013f0: 1201 1201 0c01 0c01 0c01 020a 0801 02ff  ................
-00001400: 0802 02fe 0603 02fd 1404 02fc 0205 0afb  ................
-00001410: 021c 0601 02ff 0201 02ff 0201 02ff 0202  ................
-00001420: 0afe 0223 0201 02ff 0202 02fe 0403 02fd  ...#............
-00001430: 0404 02fc 0205 02fb 0206 02fa 0207 0af9  ................
-00001440: 0220 122b                                . .+
+000000d0: 6503 6a1b 6a1c 6408 6503 6a1b 6a1c 6409  e.j.j.d.e.j.j.d.
+000000e0: 6507 651d 1900 640a 6508 651d 6507 6503  e.e...d.e.e.e.e.
+000000f0: 6a1b 6a1c 1900 6602 1900 640b 6401 660a  j.j...f...d.d.f.
+00000100: 640c 640d 8404 5a1e 6409 6507 651d 1900  d.d...Z.d.e.e...
+00000110: 640e 651d 640f 651d 640b 6401 6608 6410  d.e.d.e.d.d.f.d.
+00000120: 6411 8404 5a1f 6412 651d 6413 651d 6407  d...Z.d.e.d.e.d.
+00000130: 6503 6a1b 6a1c 6408 6503 6a1b 6a1c 6409  e.j.j.d.e.j.j.d.
+00000140: 6520 640a 6521 640b 6401 660e 6414 6415  e d.e!d.d.f.d.d.
+00000150: 8404 5a22 0900 640b 6523 6602 6416 6417  ..Z"..d.e#f.d.d.
+00000160: 8404 5a24 6401 5300 2918 e900 0000 004e  ..Z$d.S.)......N
+00000170: 2901 da06 6765 7463 7764 2902 da04 4c69  )...getcwd)...Li
+00000180: 7374 da04 4469 6374 2901 da0f 6469 7370  st..Dict)...disp
+00000190: 6c61 795f 6361 7665 6174 7329 01da 0f67  lay_caveats)...g
+000001a0: 6574 5f70 7265 6665 7265 6e63 6573 2901  et_preferences).
+000001b0: da06 6c6f 6767 6572 da04 7472 6565 da04  ..logger..tree..
+000001c0: 726f 6f74 da0b 6f75 7470 7574 5f6c 6973  root..output_lis
+000001d0: 74da 1061 6c6c 5f74 6173 6b65 725f 6974  t..all_tasker_it
+000001e0: 656d 73da 0672 6574 7572 6e63 0400 0000  ems..returnc....
+000001f0: 0000 0000 0000 0000 0500 0000 0300 0000  ................
+00000200: 4300 0000 735a 0000 007c 00a0 00a1 0044  C...sZ...|.....D
+00000210: 005d 067d 047c 04a0 01a1 0001 0071 047c  .].}.|.......q.|
+00000220: 0364 0119 00a0 01a1 0001 007c 0364 0219  .d.........|.d..
+00000230: 00a0 01a1 0001 007c 0364 0319 00a0 01a1  .......|.d......
+00000240: 0001 007c 0364 0419 00a0 01a1 0001 007c  ...|.d.........|
+00000250: 01a0 01a1 0001 007c 02a0 01a1 0001 0064  .......|.......d
+00000260: 0553 0029 0661 1701 0000 0a20 2020 2043  .S.).a.....    C
+00000270: 6c65 616e 2075 7020 6f75 7220 6d65 6d6f  lean up our memo
+00000280: 7279 2068 6f67 730a 2020 2020 2020 2020  ry hogs.        
+00000290: 3a70 6172 616d 2074 7265 653a 2078 6d6c  :param tree: xml
+000002a0: 2074 7265 6520 746f 2065 6d70 7479 0a20   tree to empty. 
+000002b0: 2020 2020 2020 203a 7061 7261 6d20 726f         :param ro
+000002c0: 6f74 3a20 726f 6f74 2078 6d6c 2074 6861  ot: root xml tha
+000002d0: 7420 7761 7320 7061 7273 6564 2066 726f  t was parsed fro
+000002e0: 6d20 6261 636b 7570 2066 696c 650a 2020  m backup file.  
+000002f0: 2020 2020 2020 3a70 6172 616d 206f 7574        :param out
+00000300: 7075 745f 6c69 7374 3a20 6c69 7374 206f  put_list: list o
+00000310: 6620 6f75 7470 7574 206c 696e 6573 2074  f output lines t
+00000320: 6f20 636c 6561 720a 2020 2020 2020 2020  o clear.        
+00000330: 3a70 6172 616d 2061 6c6c 5f74 6173 6b65  :param all_taske
+00000340: 725f 6974 656d 733a 2041 6c6c 2050 726f  r_items: All Pro
+00000350: 6a65 6374 732f 5072 6f66 696c 6573 2f54  jects/Profiles/T
+00000360: 6173 6b73 2f53 6365 6e65 730a 2020 2020  asks/Scenes.    
+00000370: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
+00000380: 205a 0c61 6c6c 5f70 726f 6a65 6374 735a   Z.all_projectsZ
+00000390: 0c61 6c6c 5f70 726f 6669 6c65 73da 0961  .all_profiles..a
+000003a0: 6c6c 5f74 6173 6b73 5a0a 616c 6c5f 7363  ll_tasksZ.all_sc
+000003b0: 656e 6573 4e29 02da 0469 7465 72da 0563  enesN)...iter..c
+000003c0: 6c65 6172 2905 7208 0000 0072 0900 0000  lear).r....r....
+000003d0: 720a 0000 0072 0b00 0000 da04 656c 656d  r....r......elem
+000003e0: a900 7211 0000 00fa 742f 5573 6572 732f  ..r.....t/Users/
+000003f0: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
+00000400: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
+00000410: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
+00000420: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
+00000430: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
+00000440: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
+00000450: 2f73 7263 2f6d 6170 6974 2e70 79da 0f63  /src/mapit.py..c
+00000460: 6c65 616e 5f75 705f 6d65 6d6f 7279 3800  lean_up_memory8.
+00000470: 0000 7312 0000 000c 0e0a 010c 010c 010c  ..s.............
+00000480: 010c 0108 0108 0104 0172 1300 0000 da0d  .........r......
+00000490: 6d79 5f6f 7574 7075 745f 6469 72da 0c6d  my_output_dir..m
+000004a0: 795f 6669 6c65 5f6e 616d 6563 0300 0000  y_file_namec....
+000004b0: 0000 0000 0000 0000 0a00 0000 0800 0000  ................
+000004c0: 4300 0000 73de 0000 0074 00a0 0164 017c  C...s....t...d.|
+000004d0: 019b 009d 02a1 0101 0074 027c 017c 0217  .........t.|.|..
+000004e0: 0064 0283 028f 517d 037c 0044 005d 467d  .d....Q}.|.D.]F}
+000004f0: 047c 04a0 0364 03a1 017d 057c 0564 046b  .|...d...}.|.d.k
+00000500: 0372 457c 047c 0564 0517 0064 0685 0219  .rE|.|.d...d....
+00000510: 00a0 0464 07a1 017d 067c 0664 0819 007d  ...d...}.|.d...}
+00000520: 077c 0464 067c 0585 0219 007c 0717 0064  .|.d.|.....|...d
+00000530: 0917 007c 047c 0564 0517 0074 057c 0783  ...|.|.d...t.|..
+00000540: 0117 0064 0685 0219 0017 007d 087c 087d  ...d.......}.|.}
+00000550: 096e 027c 047d 097c 09a0 0664 0a64 0ba1  .n.|.}.|...d.d..
+00000560: 027d 097c 09a0 0664 0c64 0da1 027d 097c  .}.|...d.d...}.|
+00000570: 03a0 077c 09a1 0101 0071 1257 0064 0604  ...|.....q.W.d..
+00000580: 0004 0083 0301 006e 0831 0073 6377 0101  .......n.1.scw..
+00000590: 0001 0001 0059 0001 0074 00a0 0164 0ea1  .....Y...t...d..
+000005a0: 0101 0064 0653 0029 0f61 0c01 0000 0a20  ...d.S.).a..... 
+000005b0: 2020 2077 7269 7465 5f6f 7574 5f74 6865     write_out_the
+000005c0: 5f66 696c 653a 2077 6520 6861 7665 2061  _file: we have a
+000005d0: 206c 6973 7420 6f66 206f 7574 7075 7420   list of output 
+000005e0: 6c69 6e65 732e 2020 5772 6974 6520 7468  lines.  Write th
+000005f0: 656d 206f 7574 2e0a 2020 2020 2020 2020  em out..        
+00000600: 3a70 6172 616d 206f 7574 7075 745f 6c69  :param output_li
+00000610: 7374 3a20 6c69 7374 206f 6620 616c 6c20  st: list of all 
+00000620: 6f75 7470 7574 206c 696e 6573 2067 656e  output lines gen
+00000630: 6572 6174 6564 0a20 2020 2020 2020 203a  erated.        :
+00000640: 7061 7261 6d20 6d79 5f6f 7574 7075 745f  param my_output_
+00000650: 6469 723a 2064 6972 6563 746f 7279 2074  dir: directory t
+00000660: 6f20 6f75 7470 7574 2074 6f0a 2020 2020  o output to.    
+00000670: 2020 2020 3a70 6172 616d 206d 795f 6669      :param my_fi
+00000680: 6c65 5f6e 616d 653a 206e 616d 6520 6f66  le_name: name of
+00000690: 2066 696c 6520 746f 2075 7365 0a20 2020   file to use.   
+000006a0: 2020 2020 203a 7265 7475 726e 3a20 6e6f       :return: no
+000006b0: 7468 696e 670a 2020 2020 7a27 4675 6e63  thing.    z'Func
+000006c0: 7469 6f6e 2045 6e74 7279 3a20 7772 6974  tion Entry: writ
+000006d0: 655f 6f75 745f 7468 655f 6669 6c65 2064  e_out_the_file d
+000006e0: 6972 3ada 0177 7a08 4163 7469 6f6e 3a20  ir:..wz.Action: 
+000006f0: e9ff ffff ffe9 0800 0000 4efa 0120 7201  ..........N.. r.
+00000700: 0000 00fa 013a 7a0e 3c2f 7370 616e 3e3c  .....:z.</span><
+00000710: 2f73 7061 6e3e 7a07 3c2f 7370 616e 3e7a  /span>z.</span>z
+00000720: 083c 2f70 3e3c 2f70 3e7a 043c 2f70 3e7a  .</p></p>z.</p>z
+00000730: 2146 756e 6374 696f 6e20 4578 6974 3a20  !Function Exit: 
+00000740: 7772 6974 655f 6f75 745f 7468 655f 6669  write_out_the_fi
+00000750: 6c65 2908 7207 0000 00da 0469 6e66 6fda  le).r......info.
+00000760: 046f 7065 6eda 0466 696e 64da 0573 706c  .open..find..spl
+00000770: 6974 da03 6c65 6eda 0772 6570 6c61 6365  it..len..replace
+00000780: da05 7772 6974 6529 0a72 0a00 0000 7214  ..write).r....r.
+00000790: 0000 0072 1500 0000 5a08 6f75 745f 6669  ...r....Z.out_fi
+000007a0: 6c65 da04 6974 656d 5a0f 6163 7469 6f6e  le..itemZ.action
+000007b0: 5f70 6f73 6974 696f 6e5a 1261 6374 696f  _positionZ.actio
+000007c0: 6e5f 6e75 6d62 6572 5f6c 6973 745a 0d61  n_number_listZ.a
+000007d0: 6374 696f 6e5f 6e75 6d62 6572 5a04 7465  ction_numberZ.te
+000007e0: 6d70 5a0b 6f75 7470 7574 5f6c 696e 6572  mpZ.output_liner
+000007f0: 1100 0000 7211 0000 0072 1200 0000 da12  ....r....r......
+00000800: 7772 6974 655f 6f75 745f 7468 655f 6669  write_out_the_fi
+00000810: 6c65 5400 0000 7330 0000 0010 0a10 0108  leT...s0........
+00000820: 010a 0208 0116 0108 010a 0202 0102 ff02  ................
+00000830: 0202 fe16 0302 fd02 ff06 0604 020c 010c  ................
+00000840: 010c 0102 ef1c ff0a 1304 0172 2300 0000  ...........r#...
+00000850: da04 6e61 6d65 da14 7072 6f66 696c 655f  ..name..profile_
+00000860: 6f72 5f74 6173 6b5f 6e61 6d65 6306 0000  or_task_namec...
+00000870: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+00000880: 0043 0000 0073 4600 0000 7c04 a000 a100  .C...sF...|.....
+00000890: 0100 7c00 9b00 6401 7c01 9b00 6402 9d04  ..|...d.|...d...
+000008a0: 7d06 7401 7c06 8301 0100 7402 a003 7c06  }.t.|.....t...|.
+000008b0: a101 0100 7404 7c02 7c03 7c04 7c05 8304  ....t.|.|.|.|...
+000008c0: 0100 7405 a006 6403 a101 0100 6404 5300  ..t...d.....d.S.
+000008d0: 2905 61f6 0100 000a 2020 2020 436c 6561  ).a.....    Clea
+000008e0: 6e75 7020 6d65 6d6f 7279 2061 6e64 206c  nup memory and l
+000008f0: 6574 2075 7365 7220 6b6e 6f77 2074 6865  et user know the
+00000900: 7265 2077 6173 206e 6f20 6d61 7463 6820  re was no match 
+00000910: 666f 756e 6420 666f 7220 5461 736b 2f50  found for Task/P
+00000920: 726f 6669 6c65 0a20 2020 2020 2020 203a  rofile.        :
+00000930: 7061 7261 6d20 6e61 6d65 3a20 7468 6520  param name: the 
+00000940: 6e61 6d65 2074 6f20 6164 6420 746f 2074  name to add to t
+00000950: 6865 206c 6f67 2f70 7269 6e74 206f 7574  he log/print out
+00000960: 7075 740a 2020 2020 2020 2020 3a70 6172  put.        :par
+00000970: 616d 2070 726f 6669 6c65 5f6f 725f 7461  am profile_or_ta
+00000980: 736b 5f6e 616d 653a 206e 616d 6520 6f66  sk_name: name of
+00000990: 2074 6865 2050 726f 6669 6c65 206f 7220   the Profile or 
+000009a0: 5461 736b 2074 6f20 636c 6561 6e0a 2020  Task to clean.  
+000009b0: 2020 2020 2020 3a70 6172 616d 2074 7265        :param tre
+000009c0: 653a 2078 6d6c 2074 7265 6520 746f 2063  e: xml tree to c
+000009d0: 6c65 6172 0a20 2020 2020 2020 203a 7061  lear.        :pa
+000009e0: 7261 6d20 726f 6f74 3a20 726f 6f74 206f  ram root: root o
+000009f0: 6620 786d 6c20 7061 7273 6564 2066 726f  f xml parsed fro
+00000a00: 6d20 6669 6c65 2074 6f20 636c 6561 720a  m file to clear.
+00000a10: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00000a20: 7574 7075 745f 6c69 7374 3a20 6c69 7374  utput_list: list
+00000a30: 206f 6620 6f75 7470 7574 206c 696e 6573   of output lines
+00000a40: 2074 6f20 656d 7074 790a 2020 2020 2020   to empty.      
+00000a50: 2020 3a70 6172 616d 2061 6c6c 5f74 6173    :param all_tas
+00000a60: 6b65 725f 6974 656d 733a 2061 6c6c 2054  ker_items: all T
+00000a70: 6173 6b65 7220 5072 6f6a 6563 7473 2f50  asker Projects/P
+00000a80: 726f 6669 6c65 732f 5461 736b 732f 5363  rofiles/Tasks/Sc
+00000a90: 656e 6573 2074 6f20 636c 6561 720a 2020  enes to clear.  
+00000aa0: 2020 2020 2020 3a72 7479 7065 3a20 636f        :rtype: co
+00000ab0: 6c6f 7273 2c20 7275 6e74 696d 6520 6172  lors, runtime ar
+00000ac0: 6775 6d65 6e74 732c 0a20 2020 2072 1900  guments,.    r..
+00000ad0: 0000 7a0c 206e 6f74 2066 6f75 6e64 2121  ..z. not found!!
+00000ae0: e905 0000 004e 2907 720f 0000 00da 0570  .....N).r......p
+00000af0: 7269 6e74 7207 0000 00da 0564 6562 7567  rintr......debug
+00000b00: 7213 0000 00da 0373 7973 da04 6578 6974  r......sys..exit
+00000b10: 2907 7224 0000 0072 2500 0000 7208 0000  ).r$...r%...r...
+00000b20: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000b30: da0d 6572 726f 725f 6d65 7373 6167 6572  ..error_messager
+00000b40: 1100 0000 7211 0000 0072 1200 0000 da11  ....r....r......
+00000b50: 636c 6561 6e5f 7570 5f61 6e64 5f65 7869  clean_up_and_exi
+00000b60: 7479 0000 0073 0c00 0000 0813 1001 0801  ty...s..........
+00000b70: 0a01 0e01 0e01 722c 0000 0063 0000 0000  ......r,...c....
+00000b80: 0000 0000 0000 0000 1000 0000 0a00 0000  ................
+00000b90: 4300 0000 7328 0200 0067 0067 0067 0067  C...s(...g.g.g.g
+00000ba0: 0066 045c 047d 007d 017d 027d 0374 00a0  .f.\.}.}.}.}.t..
+00000bb0: 017c 01a1 015c 097d 047d 057d 067d 077d  .|...\.}.}.}.}.}
+00000bc0: 017d 087d 097d 0a7d 0b7c 0564 0119 0072  .}.}.}.}.|.d...r
+00000bd0: 2374 027c 017c 057c 047c 0b83 0401 0074  #t.|.|.|.|.....t
+00000be0: 03a0 047c 017c 007c 027c 057c 067c 077c  ...|.|.|.|.|.|.|
+00000bf0: 047c 0ba1 087d 007c 0564 0219 0072 427c  .|...}.|.d...rB|
+00000c00: 0664 0319 0073 4274 0564 047c 0564 0219  .d...sBt.d.|.d..
+00000c10: 007c 087c 097c 017c 0b83 0601 007c 0564  .|.|.|.|.....|.d
+00000c20: 0519 0072 557c 0664 0619 0073 5574 0564  ...rU|.d...sUt.d
+00000c30: 077c 0564 0519 007c 087c 097c 017c 0b83  .|.d...|.|.|.|..
+00000c40: 0601 007c 0564 0819 0073 777c 0564 0219  ...|.d...sw|.d..
+00000c50: 0073 777c 0564 0519 0073 7774 06a0 077c  .sw|.d...swt...|
+00000c60: 017c 037c 007c 057c 067c 077c 047c 0ba1  .|.|.|.|.|.|.|..
+00000c70: 0801 0074 06a0 087c 017c 037c 027c 067c  ...t...|.|.|.|.|
+00000c80: 047c 05a1 0601 007c 0564 0819 0072 9a7c  .|.....|.d...r.|
+00000c90: 0664 0919 0073 9a7c 0564 0519 0072 877c  .d...s.|.d...r.|
+00000ca0: 0664 0619 0072 9a7c 0564 0219 0072 8f7c  .d...r.|.d...r.|
+00000cb0: 0664 0319 0072 9a74 0564 0a7c 0564 0819  .d...r.t.d.|.d..
+00000cc0: 007c 087c 097c 017c 0b83 0601 0074 097c  .|.|.|.|.....t.|
+00000cd0: 017c 057c 0483 0301 0064 0b7d 0c74 0aa0  .|.|.....d.}.t..
+00000ce0: 0b7c 047c 057c 0164 0c7c 0ca1 0501 0074  .|.|.|.d.|.....t
+00000cf0: 0c83 007d 0d74 0da0 0e64 0d7c 0d9b 009d  ...}.t...d.|....
+00000d00: 02a1 0101 007c 0d64 0075 0072 d164 0e7d  .....|.d.u.r.d.}
+00000d10: 0c74 0da0 0e7c 0ca1 0101 0074 0f7c 0c83  .t...|.....t.|..
+00000d20: 0101 0074 107c 087c 097c 017c 0b83 0401  ...t.|.|.|.|....
+00000d30: 0074 11a0 1264 0fa1 0101 0064 107d 0e74  .t...d.....d.}.t
+00000d40: 137c 017c 0d7c 0e83 0301 0074 107c 087c  .|.|.|.....t.|.|
+00000d50: 097c 017c 0b83 0401 0074 0da0 0e64 11a1  .|.|.....t...d..
+00000d60: 0101 0064 0c7d 0f7a 0e74 146a 1564 127c  ...d.}.z.t.j.d.|
+00000d70: 0d9b 007c 0e9b 009d 0364 0f64 138d 0201  ...|.....d.d....
+00000d80: 0057 006e 1804 0074 146a 1690 0179 0d01  .W.n...t.j...y..
+00000d90: 0001 0001 0064 147d 0c74 0f7c 0c83 0101  .....d.}.t.|....
+00000da0: 0074 0da0 0e7c 0ca1 0101 0064 157d 0f59  .t...|.....d.}.Y
+00000db0: 006e 0177 0074 0f64 1683 0101 007c 0f53  .n.w.t.d.....|.S
+00000dc0: 0029 174e 5a13 6469 7370 6c61 795f 7072  .).NZ.display_pr
+00000dd0: 6566 6572 656e 6365 735a 1373 696e 676c  eferencesZ.singl
+00000de0: 655f 7072 6f6a 6563 745f 6e61 6d65 5a14  e_project_nameZ.
+00000df0: 7369 6e67 6c65 5f70 726f 6a65 6374 5f66  single_project_f
+00000e00: 6f75 6e64 5a07 5072 6f6a 6563 745a 1373  oundZ.ProjectZ.s
+00000e10: 696e 676c 655f 7072 6f66 696c 655f 6e61  ingle_profile_na
+00000e20: 6d65 5a14 7369 6e67 6c65 5f70 726f 6669  meZ.single_profi
+00000e30: 6c65 5f66 6f75 6e64 5a07 5072 6f66 696c  le_foundZ.Profil
+00000e40: 655a 1073 696e 676c 655f 7461 736b 5f6e  eZ.single_task_n
+00000e50: 616d 655a 1173 696e 676c 655f 7461 736b  ameZ.single_task
+00000e60: 5f66 6f75 6e64 da04 5461 736b 7a0f 3c2f  _found..Taskz.</
+00000e70: 626f 6479 3e0a 3c2f 6874 6d6c 3e72 0100  body>.</html>r..
+00000e80: 0000 7a11 6f75 7470 7574 2064 6972 6563  ..z.output direc
+00000e90: 746f 7279 3a7a 3c4d 6170 5461 736b 6572  tory:z<MapTasker
+00000ea0: 2063 616e 6365 6c6c 6564 2e20 2041 6e20   cancelled.  An 
+00000eb0: 6572 726f 7220 6f63 6375 7272 6564 2e20  error occurred. 
+00000ec0: 2050 726f 6772 616d 2063 616e 6365 6c6c   Program cancell
+00000ed0: 6564 2ee9 0200 0000 7a0f 2f4d 6170 5461  ed......z./MapTa
+00000ee0: 736b 6572 2e68 746d 6c7a 204d 6170 5461  sker.htmlz MapTa
+00000ef0: 736b 6572 2070 726f 6772 616d 2065 6e64  sker program end
+00000f00: 6564 206e 6f72 6d61 6c6c 797a 0766 696c  ed normallyz.fil
+00000f10: 653a 2f2f 2901 da03 6e65 777a 4745 7272  e://)...newzGErr
+00000f20: 6f72 3a20 4661 696c 6564 2074 6f20 6f70  or: Failed to op
+00000f30: 656e 206f 7574 7075 7420 696e 2062 726f  en output in bro
+00000f40: 7773 6572 3a20 796f 7572 2062 726f 7773  wser: your brows
+00000f50: 6572 2069 7320 6e6f 7420 7375 7070 6f72  er is not suppor
+00000f60: 7465 642e e901 0000 007a 4259 6f75 2063  ted......zBYou c
+00000f70: 616e 2066 696e 6420 274d 6170 5461 736b  an find 'MapTask
+00000f80: 6572 2e68 746d 6c27 2069 6e20 7468 6520  er.html' in the 
+00000f90: 6375 7272 656e 7420 666f 6c64 6572 2e20  current folder. 
+00000fa0: 2050 726f 6772 616d 2065 6e64 2e29 17da   Program end.)..
+00000fb0: 0a69 6e69 7469 616c 697a 655a 0873 7461  .initializeZ.sta
+00000fc0: 7274 5f75 7072 0600 0000 da08 7072 6f6a  rt_upr......proj
+00000fd0: 6563 7473 5a23 7072 6f63 6573 735f 7072  ectsZ#process_pr
+00000fe0: 6f6a 6563 7473 5f61 6e64 5f74 6865 6972  ojects_and_their
+00000ff0: 5f70 726f 6669 6c65 7372 2c00 0000 da0d  _profilesr,.....
+00001000: 7370 6563 6961 6c5f 7461 736b 735a 2370  special_tasksZ#p
+00001010: 726f 6365 7373 5f74 6173 6b73 5f6e 6f74  rocess_tasks_not
+00001020: 5f63 616c 6c65 645f 6279 5f70 726f 6669  _called_by_profi
+00001030: 6c65 5a22 7072 6f63 6573 735f 6d69 7373  leZ"process_miss
+00001040: 696e 675f 7461 736b 735f 616e 645f 7072  ing_tasks_and_pr
+00001050: 6f66 696c 6573 7205 0000 00da 0c62 7569  ofilesr......bui
+00001060: 6c64 5f6f 7574 7075 745a 096d 795f 6f75  ld_outputZ.my_ou
+00001070: 7470 7574 7202 0000 0072 0700 0000 7228  tputr....r....r(
+00001080: 0000 0072 2700 0000 7213 0000 0072 2900  ...r'...r....r).
+00001090: 0000 722a 0000 0072 2300 0000 da0a 7765  ..r*...r#.....we
+000010a0: 6262 726f 7773 6572 721c 0000 00da 0545  bbrowserr......E
+000010b0: 7272 6f72 2910 5a0b 666f 756e 645f 7461  rror).Z.found_ta
+000010c0: 736b 7372 0a00 0000 5a19 7072 6f6a 6563  sksr....Z.projec
+000010d0: 7473 5f77 6974 686f 7574 5f70 726f 6669  ts_without_profi
+000010e0: 6c65 735a 1670 726f 6a65 6374 735f 7769  lesZ.projects_wi
+000010f0: 7468 5f6e 6f5f 7461 736b 735a 0863 6f6c  th_no_tasksZ.col
+00001100: 6f72 6d61 705a 0c70 726f 6772 616d 5f61  ormapZ.program_a
+00001110: 7267 735a 0b66 6f75 6e64 5f69 7465 6d73  rgsZ.found_items
+00001120: da07 6865 6164 696e 6772 0800 0000 7209  ..headingr....r.
+00001130: 0000 00da 0866 696c 656e 616d 6572 0b00  .....filenamer..
+00001140: 0000 5a09 6572 726f 725f 6d73 6772 1400  ..Z.error_msgr..
+00001150: 0000 7215 0000 005a 056d 795f 7263 7211  ..r....Z.my_rcr.
+00001160: 0000 0072 1100 0000 7212 0000 00da 096d  ...r....r......m
+00001170: 6170 6974 5f61 6c6c c400 0000 73f4 0000  apit_all....s...
+00001180: 0002 0302 0102 0102 010c fc08 1202 f602  ................
+00001190: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+000011a0: 0108 0c02 0102 0102 0102 0102 0104 fc04  ................
+000011b0: 0a02 0102 0102 0102 0102 0102 0102 0102  ................
+000011c0: 0104 f810 0c02 0102 0106 0102 0102 0102  ................
+000011d0: 0102 0104 fa10 0902 0102 0106 0102 0102  ................
+000011e0: 0102 0102 0104 fa06 0d02 ff06 0202 fe06  ................
+000011f0: 0302 fd04 0502 0102 0102 0102 0102 0102  ................
+00001200: 0102 0102 0104 f804 0e02 0102 0102 0102  ................
+00001210: 0102 0102 0104 fa06 0b02 ff06 0202 fe06  ................
+00001220: 0402 fc06 0502 fb06 0802 f806 0902 f702  ................
+00001230: 0c02 0106 0102 0102 0102 0102 0104 fa0c  ................
+00001240: 0d04 0312 0106 0410 0108 0104 010a 0108  ................
+00001250: 010e 010a 0104 020c 020e 030a 0304 0102  ................
+00001260: 011c 0110 0102 0202 ff08 030a 0108 0102  ................
+00001270: fa08 0704 0172 3900 0000 2925 7229 0000  .....r9...)%r)..
+00001280: 0072 3500 0000 5a16 6465 6675 7365 6478  .r5...Z.defusedx
+00001290: 6d6c 2e45 6c65 6d65 6e74 5472 6565 5a0a  ml.ElementTreeZ.
+000012a0: 6465 6675 7365 6478 6d6c da02 6f73 7202  defusedxml..osr.
+000012b0: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
+000012c0: 7204 0000 005a 156d 6170 7461 736b 6572  r....Z.maptasker
+000012d0: 2e73 7263 2e6f 7574 7075 746c da03 7372  .src.outputl..sr
+000012e0: 635a 076f 7574 7075 746c 7234 0000 005a  cZ.outputlr4...Z
+000012f0: 166d 6170 7461 736b 6572 2e73 7263 2e70  .maptasker.src.p
+00001300: 726f 6769 6e69 745a 0870 726f 6769 6e69  roginitZ.progini
+00001310: 7472 3100 0000 5a16 6d61 7074 6173 6b65  tr1...Z.maptaske
+00001320: 722e 7372 632e 7072 6f6a 6563 7473 7232  r.src.projectsr2
+00001330: 0000 005a 166d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
+00001340: 7263 2e74 6173 6b75 6e69 715a 0874 6173  rc.taskuniqZ.tas
+00001350: 6b75 6e69 7172 3300 0000 5a15 6d61 7074  kuniqr3...Z.mapt
+00001360: 6173 6b65 722e 7372 632e 6361 7665 6174  asker.src.caveat
+00001370: 7372 0500 0000 5a15 6d61 7074 6173 6b65  sr....Z.maptaske
+00001380: 722e 7372 632e 7072 6566 6572 7372 0600  r.src.prefersr..
+00001390: 0000 5a16 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
+000013a0: 632e 7379 7363 6f6e 7374 7207 0000 005a  c.sysconstr....Z
+000013b0: 0b45 6c65 6d65 6e74 5472 6565 5a03 584d  .ElementTreeZ.XM
+000013c0: 4cda 0373 7472 7213 0000 0072 2300 0000  L..strr....r#...
+000013d0: da04 6c69 7374 da04 6469 6374 722c 0000  ..list..dictr,..
+000013e0: 00da 0369 6e74 7239 0000 0072 1100 0000  ...intr9...r....
+000013f0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00001400: 083c 6d6f 6475 6c65 3e01 0000 0073 6200  .<module>....sb.
+00001410: 0000 0820 0801 0801 0c01 1001 1202 1201  ... ............
+00001420: 1201 1201 0c01 0c01 0c01 020b 0601 02ff  ................
+00001430: 0602 02fe 0603 02fd 1204 02fc 0205 0afb  ................
+00001440: 021c 0601 02ff 0201 02ff 0201 02ff 0202  ................
+00001450: 0afe 0225 0201 02ff 0202 02fe 0603 02fd  ...%............
+00001460: 0604 02fc 0205 02fb 0206 02fa 0207 0af9  ................
+00001470: 0220 122b                                . .+
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/outputl.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/outputl.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 14:42:44 2023 UTC, .py size: 9854 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,235 +1,264 @@
-00000000: 6f0d 0d0a 0000 0000 6437 2c64 7e26 0000  o.......d7,d~&..
+00000000: 6f0d 0d0a 0000 0000 0968 3d64 a426 0000  o........h=d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0010 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
+00000020: 0010 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6403 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
-00000060: 6400 6404 6c08 6d0a 5a0a 0100 6400 6405  d.d.l.m.Z...d.d.
-00000070: 6c08 6d0b 5a0b 0100 6400 6406 6c08 6d0c  l.m.Z...d.d.l.m.
-00000080: 5a0c 0100 6407 650d 6408 650e 6409 650f  Z...d.e.d.e.d.e.
-00000090: 640a 650f 640b 650f 640c 6510 640d 6510  d.e.d.e.d.e.d.e.
-000000a0: 640e 6401 6610 640f 6410 8404 5a11 6411  d.d.f.d.d...Z.d.
-000000b0: 6510 640e 650f 6604 6412 6413 8404 5a12  e.d.e.f.d.d...Z.
-000000c0: 6414 6501 6a13 640c 6510 6415 650f 640e  d.e.j.d.e.d.e.d.
-000000d0: 650f 6608 6416 6417 8404 5a14 6418 6419  e.f.d.d...Z.d.d.
-000000e0: 8400 5a15 641a 641b 8400 5a16 6401 5300  ..Z.d.d...Z.d.S.
-000000f0: 291c e900 0000 004e 2901 da06 6465 6275  )......N)...debu
-00000100: 6731 2901 da0b 464f 4e54 5f54 4f5f 5553  g1)...FONT_TO_US
-00000110: 4529 01da 1155 4e4b 4e4f 574e 5f54 4153  E)...UNKNOWN_TAS
-00000120: 4b5f 4e41 4d45 2901 da09 6465 6275 675f  K_NAME)...debug_
-00000130: 6f75 7429 01da 066c 6f67 6765 72da 1369  out)...logger..i
-00000140: 6e63 6c75 6465 5f74 6865 5f70 726f 6669  nclude_the_profi
-00000150: 6c65 da0b 6f75 7470 7574 5f6c 6973 74da  le..output_list.
-00000160: 0c70 726f 6a65 6374 5f6e 616d 65da 0c70  .project_name..p
-00000170: 726f 6669 6c65 5f6e 616d 65da 0768 6561  rofile_name..hea
-00000180: 6469 6e67 da08 636f 6c6f 726d 6170 da0c  ding..colormap..
-00000190: 7072 6f67 7261 6d5f 6172 6773 da06 7265  program_args..re
-000001a0: 7475 726e 6307 0000 0000 0000 0000 0000  turnc...........
-000001b0: 0007 0000 0007 0000 0043 0000 0073 9400  .........C...s..
-000001c0: 0000 7c01 a000 a100 0100 7401 7c05 7c06  ..|.......t.|.|.
-000001d0: 7c01 6401 7402 7c04 1700 8305 0100 7c06  |.d.t.|.......|.
-000001e0: 6402 1900 7218 7403 7c05 7c06 7c01 8303  d...r.t.|.|.|...
-000001f0: 0100 7401 7c05 7c06 7c01 6403 6404 8305  ..t.|.|.|.d.d...
-00000200: 0100 7401 7c05 7c06 7c01 6405 6406 7c02  ..t.|.|.|.d.d.|.
-00000210: 9b00 9d02 8305 0100 7c00 7248 7401 7c05  ........|.rHt.|.
-00000220: 7c06 7c01 6403 6404 8305 0100 7401 7c05  |.|.d.d.....t.|.
-00000230: 7c06 7c01 6405 6407 7c03 9b00 9d02 8305  |.|.d.d.|.......
-00000240: 0100 7401 7c05 7c06 7c01 6403 6404 8305  ..t.|.|.|.d.d...
-00000250: 0100 6400 5300 2908 4e72 0100 0000 da05  ..d.S.).Nr......
-00000260: 6465 6275 67e9 0100 0000 da00 e902 0000  debug...........
-00000270: 007a 0950 726f 6a65 6374 3a20 7a09 5072  .z.Project: z.Pr
-00000280: 6f66 696c 653a 2029 04da 0563 6c65 6172  ofile: )...clear
-00000290: da09 6d79 5f6f 7574 7075 7472 0300 0000  ..my_outputr....
-000002a0: 7202 0000 0029 0772 0700 0000 7208 0000  r....).r....r...
-000002b0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-000002c0: 720c 0000 0072 0d00 0000 a900 7215 0000  r....r......r...
-000002d0: 00fa 762f 5573 6572 732f 6d69 6b72 7562  ..v/Users/mikrub
-000002e0: 696e 2f4c 6962 7261 7279 2f43 6c6f 7564  in/Library/Cloud
-000002f0: 5374 6f72 6167 652f 476f 6f67 6c65 4472  Storage/GoogleDr
-00000300: 6976 652d 6d69 6b72 7562 696e 4067 6d61  ive-mikrubin@gma
-00000310: 696c 2e63 6f6d 2f4d 7920 4472 6976 652f  il.com/My Drive/
-00000320: 5079 7468 6f6e 2f6d 6170 7461 736b 6572  Python/maptasker
-00000330: 2f6d 6170 7461 736b 6572 2f73 7263 2f6f  /maptasker/src/o
-00000340: 7574 7075 746c 2e70 79da 1272 6566 7265  utputl.py..refre
-00000350: 7368 5f6f 7572 5f6f 7574 7075 741c 0000  sh_our_output...
-00000360: 0073 1600 0000 0809 1402 0802 0c01 1001  .s..............
-00000370: 1601 0401 1001 1601 1001 0401 7217 0000  ............r...
-00000380: 00da 0d73 7479 6c65 5f64 6574 6169 6c73  ...style_details
-00000390: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000003a0: 0008 0000 0043 0000 0073 7c00 0000 6401  .....C...s|...d.
-000003b0: 7d01 7c00 6402 1900 721e 6403 7c00 6404  }.|.d...r.d.|.d.
-000003c0: 1900 9b00 6405 7c00 6406 1900 9b00 7c00  ....d.|.d.....|.
-000003d0: 6407 1900 9b00 6408 7c00 6409 1900 9b00  d.....d.|.d.....
-000003e0: 640a 9d08 7d01 7c01 5300 7c00 640b 1900  d...}.|.S.|.d...
-000003f0: 723c 640c 7c00 6406 1900 9b00 7400 9b00  r<d.|.d.....t...
-00000400: 6408 7c00 6409 1900 9b00 640d 7c00 6404  d.|.d.....d.|.d.
-00000410: 1900 9b00 640e 9d08 7d01 7c01 a001 640f  ....d...}.|...d.
-00000420: 6401 a102 7d01 7c01 5300 2910 7abc 0a20  d...}.|.S.).z.. 
-00000430: 2020 2041 6464 2061 7070 726f 7072 6961     Add appropria
-00000440: 7465 2048 544d 4c20 7374 796c 6520 7461  te HTML style ta
-00000450: 6773 2062 6173 6564 206f 6e20 7061 7261  gs based on para
-00000460: 6d65 7465 7273 2069 6e20 6469 6374 696f  meters in dictio
-00000470: 6e61 7279 2070 6173 7365 6420 696e 0a20  nary passed in. 
-00000480: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-00000490: 796c 655f 6465 7461 696c 733a 2064 6963  yle_details: dic
-000004a0: 7469 6f6e 6172 790a 2020 2020 2020 2020  tionary.        
-000004b0: 3a72 6574 7572 6e3a 2075 7064 6174 6564  :return: updated
-000004c0: 206f 7574 7075 7420 6c69 6e65 2077 6974   output line wit
-000004d0: 6820 7374 796c 6520 6465 7461 696c 7320  h style details 
-000004e0: 6164 6465 640a 2020 2020 7211 0000 00da  added.    r.....
-000004f0: 0769 735f 6c69 7374 7a11 3c6c 6920 7374  .is_listz.<li st
-00000500: 796c 653d 2263 6f6c 6f72 3ada 0663 6f6c  yle="color:..col
-00000510: 6f72 317a 1522 3e3c 7370 616e 2073 7479  or1z."><span sty
-00000520: 6c65 3d22 636f 6c6f 723a da06 636f 6c6f  le="color:..colo
-00000530: 7232 da04 666f 6e74 fa01 3eda 0765 6c65  r2..font..>..ele
-00000540: 6d65 6e74 7a0d 3c2f 7370 616e 3e3c 2f6c  mentz.</span></l
-00000550: 693e 0ada 0c69 735f 7461 736b 6572 6e65  i>...is_taskerne
-00000560: 747a 3f3c 7020 7374 796c 653d 226d 6172  tz?<p style="mar
-00000570: 6769 6e2d 6c65 6674 3a32 3070 783b 6d61  gin-left:20px;ma
-00000580: 7267 696e 2d72 6967 6874 3a35 3070 783b  rgin-right:50px;
-00000590: 223e 3c70 2073 7479 6c65 3d22 636f 6c6f  "><p style="colo
-000005a0: 723a 7a15 3c2f 703e 0a3c 7020 7374 796c  r:z.</p>.<p styl
-000005b0: 653d 2263 6f6c 6f72 3a7a 0222 3e7a 0d3c  e="color:z.">z.<
-000005c0: 7370 616e 3e3c 2f73 7061 6e3e 2902 7203  span></span>).r.
-000005d0: 0000 00da 0772 6570 6c61 6365 2902 7218  .....replace).r.
-000005e0: 0000 005a 0f6c 696e 655f 7769 7468 5f73  ...Z.line_with_s
-000005f0: 7479 6c65 7215 0000 0072 1500 0000 7216  tyler....r....r.
-00000600: 0000 00da 0970 7574 5f73 7479 6c65 3e00  .....put_style>.
-00000610: 0000 7330 0000 0004 0608 010c 0206 0102  ..s0............
-00000620: ff06 0104 ff06 0206 fe02 ff04 0f08 f702  ................
-00000630: 0206 0102 ff02 0104 ff06 0204 fe06 0306  ................
-00000640: fd02 ff0c 0604 0272 2100 0000 721e 0000  .......r!...r...
-00000650: 00da 0b66 6f6e 745f 746f 5f75 7365 6303  ...font_to_usec.
-00000660: 0000 0000 0000 0000 0000 0004 0000 0008  ................
-00000670: 0000 0043 0000 0073 9a01 0000 7c00 6400  ...C...s....|.d.
-00000680: 6401 8502 1900 6402 6b02 7217 7400 6403  d.....d.k.r.t.d.
-00000690: 7c01 6404 1900 7c01 6405 1900 7c02 7c00  |.d...|.d...|.|.
-000006a0: 6406 9c05 6407 8d01 5300 7c00 6400 6401  d...d...S.|.d.d.
-000006b0: 8502 1900 6408 6b02 722e 7400 6403 7c01  ....d.k.r.t.d.|.
-000006c0: 6404 1900 7c01 6409 1900 7c02 7c00 6406  d...|.d...|.|.d.
-000006d0: 9c05 6407 8d01 5300 7c00 6400 640a 8502  ..d...S.|.d.d...
-000006e0: 1900 640b 6b02 733a 640c 7c00 7600 725c  ..d.k.s:d.|.v.r\
-000006f0: 7401 7c00 7600 724d 7400 6403 7c01 6404  t.|.v.rMt.d.|.d.
-00000700: 1900 7c01 640d 1900 7c02 7c00 6406 9c05  ..|.d...|.|.d...
-00000710: 6407 8d01 5300 7400 6403 7c01 6404 1900  d...S.t.d.|.d...
-00000720: 7c01 640e 1900 7c02 7c00 6406 9c05 6407  |.d...|.|.d...d.
-00000730: 8d01 5300 7c00 6400 640f 8502 1900 6410  ..S.|.d.d.....d.
-00000740: 6b02 7273 7400 6403 7c01 6404 1900 7c01  k.rst.d.|.d...|.
-00000750: 6411 1900 7c02 7c00 6406 9c05 6407 8d01  d...|.|.d...d...
-00000760: 5300 6412 7c00 7600 729f 6413 7c00 7600  S.d.|.v.r.d.|.v.
-00000770: 7290 7c00 6414 6400 8502 1900 6415 6b02  r.|.d.d.....d.k.
-00000780: 7285 6415 5300 7402 a003 7c00 a004 6413  r.d.S.t...|...d.
-00000790: 6416 a102 a101 7d03 7c03 7d00 7400 6403  d.....}.|.}.t.d.
-000007a0: 7c01 6404 1900 7c01 6417 1900 7c02 7c00  |.d...|.d...|.|.
-000007b0: 6406 9c05 6407 8d01 5300 6418 7c00 7600  d...d...S.d.|.v.
-000007c0: 72b2 7400 6403 7c01 6404 1900 7c01 6419  r.t.d.|.d...|.d.
-000007d0: 1900 7c02 7c00 6406 9c05 6407 8d01 5300  ..|.|.d...d...S.
-000007e0: 641a 7c00 7600 72c6 7400 641b 7c01 6404  d.|.v.r.t.d.|.d.
-000007f0: 1900 7c01 641c 1900 7c02 7c00 6403 641d  ..|.d...|.|.d.d.
-00000800: 9c06 6407 8d01 5300 641e 7c00 9b00 9d02  ..d...S.d.|.....
-00000810: 641f 1700 5300 2920 4ee9 0700 0000 da07  d...S.) N.......
-00000820: 5072 6f6a 6563 7454 5a0c 6275 6c6c 6574  ProjectTZ.bullet
-00000830: 5f63 6f6c 6f72 5a0d 7072 6f6a 6563 745f  _colorZ.project_
-00000840: 636f 6c6f 7229 0572 1900 0000 721a 0000  color).r....r...
-00000850: 0072 1b00 0000 721c 0000 0072 1e00 0000  .r....r....r....
-00000860: 2901 7218 0000 00da 0750 726f 6669 6c65  ).r......Profile
-00000870: 5a0d 7072 6f66 696c 655f 636f 6c6f 72e9  Z.profile_color.
-00000880: 0500 0000 7a05 5461 736b 3a7a 0f26 2334  ....z.Task:z.&#4
-00000890: 353b 2623 3435 3b54 6173 6b3a 5a12 756e  5;&#45;Task:Z.un
-000008a0: 6b6e 6f77 6e5f 7461 736b 5f63 6f6c 6f72  known_task_color
-000008b0: 5a0a 7461 736b 5f63 6f6c 6f72 e906 0000  Z.task_color....
-000008c0: 007a 0653 6365 6e65 3a5a 0b73 6365 6e65  .z.Scene:Z.scene
-000008d0: 5f63 6f6c 6f72 7a07 4163 7469 6f6e 3a7a  _colorz.Action:z
-000008e0: 0b41 6374 696f 6e3a 202e 2e2e e90b 0000  .Action: .......
-000008f0: 0072 1100 0000 7a1a 266e 6273 703b 266e  .r....z.&nbsp;&n
-00000900: 6273 703b 636f 6e74 696e 7565 6420 3e3e  bsp;continued >>
-00000910: 3e20 5a0c 6163 7469 6f6e 5f63 6f6c 6f72  > Z.action_color
-00000920: 7a09 4c61 6265 6c20 666f 725a 1261 6374  z.Label forZ.act
-00000930: 696f 6e5f 6c61 6265 6c5f 636f 6c6f 727a  ion_label_colorz
-00000940: 0a54 6173 6b65 724e 6574 2046 5a0f 7461  .TaskerNet FZ.ta
-00000950: 736b 6572 6e65 745f 636f 6c6f 7229 0672  skernet_color).r
-00000960: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
-00000970: 0000 0072 1e00 0000 721f 0000 007a 043c  ...r....r....z.<
-00000980: 6c69 207a 063c 2f6c 693e 0a29 0572 2100  li z.</li>.).r!.
-00000990: 0000 7204 0000 00da 0f61 6374 696f 6e5f  ..r......action_
-000009a0: 6576 616c 7561 7465 5a12 636c 6561 6e75  evaluateZ.cleanu
-000009b0: 705f 7468 655f 7265 7375 6c74 7220 0000  p_the_resultr ..
-000009c0: 0029 0472 1e00 0000 720c 0000 0072 2200  .).r....r....r".
-000009d0: 0000 da03 746d 7072 1500 0000 7215 0000  ....tmpr....r...
-000009e0: 0072 1600 0000 da0f 756c 6966 795f 6c69  .r......ulify_li
-000009f0: 7374 5f69 7465 6d5c 0000 0073 a600 0000  st_item\...s....
-00000a00: 1001 0201 0202 0601 0601 0201 0201 04fb  ................
-00000a10: 06ff 1009 0201 0202 0601 0601 0201 0201  ................
-00000a20: 04fb 06ff 180a 080c 02f7 0202 0601 0601  ................
-00000a30: 0201 0201 04fb 04ff 02ff 020b 0202 0601  ................
-00000a40: 0601 0201 0201 04fb 04ff 02f5 1015 0201  ................
-00000a50: 0202 0601 0601 0201 0201 04fb 06ff 0809  ................
-00000a60: 0802 1002 0401 0401 0a01 04ff 0403 0201  ................
-00000a70: 0202 0601 0601 0201 0201 04fb 06ff 0809  ................
-00000a80: 0201 0202 0601 0601 0201 0201 04fb 06ff  ................
-00000a90: 0809 0201 0202 0601 0601 0201 0201 0201  ................
-00000aa0: 04fa 06ff 0e0b 722b 0000 0063 0400 0000  ......r+...c....
-00000ab0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00000ac0: 4300 0000 73a0 0000 0064 017d 047c 0104  C...s....d.}.|..
-00000ad0: 0064 026b 0272 2101 007c 0064 0064 0385  .d.k.r!..|.d.d..
-00000ae0: 0219 0064 046b 0272 187c 009b 0064 0517  ...d.k.r.|...d..
-00000af0: 007d 0409 007c 0453 0064 067c 009b 009d  .}...|.S.d.|....
-00000b00: 0264 0717 007d 047c 0453 0004 0064 086b  .d...}.|.S...d.k
-00000b10: 0272 2f01 0064 097c 009b 009d 0264 0a17  .r/..d.|.....d..
-00000b20: 007d 047c 0453 0004 0064 0b6b 0272 3c01  .}.|.S...d.k.r<.
-00000b30: 0074 007c 007c 027c 0383 037d 047c 0453  .t.|.|.|...}.|.S
-00000b40: 0004 0064 0c6b 0272 4501 0064 0d7d 047c  ...d.k.rE..d.}.|
-00000b50: 0453 0064 0e6b 0272 4e7c 0064 0517 007d  .S.d.k.rN|.d...}
-00000b60: 047c 0453 007c 0453 0029 0f4e 7211 0000  .|.S.|.S.).Nr...
-00000b70: 0072 0100 0000 7227 0000 007a 063c 6874  .r....r'...z.<ht
-00000b80: 6d6c 3e7a 053c 6272 3e0a 7a03 3c62 3e7a  ml>z.<br>.z.<b>z
-00000b90: 093c 2f62 3e3c 6272 3e0a 7210 0000 007a  .</b><br>.r....z
-00000ba0: 043c 756c 3eda 010a 7212 0000 00e9 0300  .<ul>...r.......
-00000bb0: 0000 7a05 3c2f 756c 3ee9 0400 0000 2901  ..z.</ul>.....).
-00000bc0: 722b 0000 0029 0572 1e00 0000 5a03 6c76  r+...).r....Z.lv
-00000bd0: 6c72 0c00 0000 7222 0000 00da 0673 7472  lr....r".....str
-00000be0: 696e 6772 1500 0000 7215 0000 0072 1600  ingr....r....r..
-00000bf0: 0000 da05 756c 6966 79c3 0000 0073 2a00  ....ulify....s*.
-00000c00: 0000 0402 0201 0a01 1002 0a01 0202 0409  ................
-00000c10: 0ef7 0409 0af8 0e01 0407 0afa 0c01 0405  ................
-00000c20: 0afc 0401 0403 06fe 0801 0801 7230 0000  ............r0..
-00000c30: 0063 0500 0000 0000 0000 0000 0000 0700  .c..............
-00000c40: 0000 0800 0000 4300 0000 7366 0000 0064  ......C...sf...d
-00000c50: 017c 0476 0072 137c 0164 0219 0064 0375  .|.v.r.|.d...d.u
-00000c60: 0072 137c 04a0 0064 01a1 017d 057c 0564  .r.|...d...}.|.d
-00000c70: 0419 007d 047c 02a0 0174 027c 047c 037c  ...}.|...t.|.|.|
-00000c80: 007c 0164 0519 0083 04a1 0101 0074 0372  .|.d.........t.r
-00000c90: 3164 0674 027c 047c 037c 007c 0164 0519  1d.t.|.|.|.|.d..
-00000ca0: 0083 0466 027d 0674 04a0 057c 06a1 0101  ...f.}.t...|....
-00000cb0: 0064 0053 0029 074e 7a08 5461 736b 2049  .d.S.).Nz.Task I
-00000cc0: 443a 720f 0000 0046 7201 0000 0072 2200  D:r....Fr....r".
-00000cd0: 0000 7a0b 6f75 745f 7374 7269 6e67 3a29  ..z.out_string:)
-00000ce0: 06da 0573 706c 6974 da06 6170 7065 6e64  ...split..append
-00000cf0: 7230 0000 0072 0500 0000 7206 0000 0072  r0...r....r....r
-00000d00: 0f00 0000 2907 720c 0000 0072 0d00 0000  ....).r....r....
-00000d10: 7208 0000 005a 0a6c 6973 745f 6c65 7665  r....Z.list_leve
-00000d20: 6c5a 0a6f 7574 5f73 7472 696e 675a 0c74  lZ.out_stringZ.t
-00000d30: 656d 705f 656c 656d 656e 745a 0964 6562  emp_elementZ.deb
-00000d40: 7567 5f6d 7367 7215 0000 0072 1500 0000  ug_msgr....r....
-00000d50: 7216 0000 0072 1400 0000 db00 0000 7318  r....r........s.
-00000d60: 0000 0014 020a 0208 0104 0110 0104 ff04  ................
-00000d70: 0404 010c 0106 ff0a 0304 0172 1400 0000  ...........r....
-00000d80: 2917 da15 786d 6c2e 6574 7265 652e 456c  )...xml.etree.El
-00000d90: 656d 656e 7454 7265 65da 0378 6d6c 5a15  ementTree..xmlZ.
-00000da0: 6d61 7074 6173 6b65 722e 7372 632e 6163  maptasker.src.ac
-00000db0: 7469 6f6e 65da 0373 7263 5a07 6163 7469  tione..srcZ.acti
-00000dc0: 6f6e 6572 2900 0000 5a13 6d61 7074 6173  oner)...Z.maptas
-00000dd0: 6b65 722e 7372 632e 6465 6275 6772 0200  ker.src.debugr..
-00000de0: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
-00000df0: 632e 7379 7363 6f6e 7374 7203 0000 0072  c.sysconstr....r
-00000e00: 0400 0000 7205 0000 0072 0600 0000 da04  ....r....r......
-00000e10: 626f 6f6c da04 6c69 7374 da03 7374 72da  bool..list..str.
-00000e20: 0464 6963 7472 1700 0000 7221 0000 00da  .dictr....r!....
-00000e30: 0565 7472 6565 722b 0000 0072 3000 0000  .etreer+...r0...
-00000e40: 7214 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00000e50: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-00000e60: 6c65 3e01 0000 0073 3800 0000 080e 1202  le>....s8.......
-00000e70: 0c01 0c01 0c01 0c01 0c01 0206 0201 02ff  ................
-00000e80: 0202 02fe 0203 02fd 0204 02fc 0205 02fb  ................
-00000e90: 0206 02fa 0207 02f9 0208 0af8 1222 1c1e  ............."..
-00000ea0: 0867 0c18                                .g..
+00000060: 6400 6404 6c0a 6d0b 5a0b 0100 6400 6405  d.d.l.m.Z...d.d.
+00000070: 6c0a 6d0c 5a0c 0100 6400 6406 6c0a 6d0d  l.m.Z...d.d.l.m.
+00000080: 5a0d 0100 6400 6407 6c0a 6d0e 5a0e 0100  Z...d.d.l.m.Z...
+00000090: 6408 650f 6409 6510 640a 6511 640b 6511  d.e.d.e.d.e.d.e.
+000000a0: 640c 6511 640d 6512 640e 6512 640f 6401  d.e.d.e.d.e.d.d.
+000000b0: 6610 6410 6411 8404 5a13 6412 6512 640f  f.d.d...Z.d.e.d.
+000000c0: 6511 6604 6413 6414 8404 5a14 6415 6501  e.f.d.d...Z.d.e.
+000000d0: 6a15 6a16 640d 6512 6416 6511 640f 6511  j.j.d.e.d.e.d.e.
+000000e0: 6608 6417 6418 8404 5a17 6419 641a 8400  f.d.d...Z.d.d...
+000000f0: 5a18 640d 6512 640e 6512 6409 6510 641b  Z.d.e.d.e.d.e.d.
+00000100: 6519 641c 6511 640f 6401 660c 641d 641e  e.d.e.d.d.f.d.d.
+00000110: 8404 5a1a 6401 5300 291f e900 0000 004e  ..Z.d.S.)......N
+00000120: 2901 da06 6465 6275 6731 2901 da0b 666f  )...debug1)...fo
+00000130: 726d 6174 5f68 746d 6c29 01da 0b46 4f4e  rmat_html)...FON
+00000140: 545f 544f 5f55 5345 2901 da11 554e 4b4e  T_TO_USE)...UNKN
+00000150: 4f57 4e5f 5441 534b 5f4e 414d 4529 01da  OWN_TASK_NAME)..
+00000160: 0964 6562 7567 5f6f 7574 2901 da06 6c6f  .debug_out)...lo
+00000170: 6767 6572 da13 696e 636c 7564 655f 7468  gger..include_th
+00000180: 655f 7072 6f66 696c 65da 0b6f 7574 7075  e_profile..outpu
+00000190: 745f 6c69 7374 da0c 7072 6f6a 6563 745f  t_list..project_
+000001a0: 6e61 6d65 da0c 7072 6f66 696c 655f 6e61  name..profile_na
+000001b0: 6d65 da07 6865 6164 696e 67da 0863 6f6c  me..heading..col
+000001c0: 6f72 6d61 70da 0c70 726f 6772 616d 5f61  ormap..program_a
+000001d0: 7267 73da 0672 6574 7572 6e63 0700 0000  rgs..returnc....
+000001e0: 0000 0000 0000 0000 0700 0000 0b00 0000  ................
+000001f0: 4300 0000 73ac 0000 007c 01a0 00a1 0001  C...s....|......
+00000200: 0074 017c 057c 067c 0164 0174 027c 0417  .t.|.|.|.d.t.|..
+00000210: 0083 0501 007c 0664 0219 0072 1874 037c  .....|.d...r.t.|
+00000220: 057c 067c 0183 0301 0074 017c 057c 067c  .|.|.....t.|.|.|
+00000230: 0164 0364 0483 0501 0074 017c 057c 067c  .d.d.....t.|.|.|
+00000240: 0164 0574 047c 0564 0664 0464 077c 029b  .d.t.|.d.d.d.|..
+00000250: 009d 0264 0883 0583 0501 007c 0072 5474  ...d.......|.rTt
+00000260: 017c 057c 067c 0164 0364 0483 0501 0074  .|.|.|.d.d.....t
+00000270: 017c 057c 067c 0164 0574 047c 0564 0964  .|.|.|.d.t.|.d.d
+00000280: 0464 0a7c 039b 009d 0264 0883 0583 0501  .d.|.....d......
+00000290: 0074 017c 057c 067c 0164 0364 0483 0501  .t.|.|.|.d.d....
+000002a0: 0064 0053 0029 0b4e 7201 0000 00da 0564  .d.S.).Nr......d
+000002b0: 6562 7567 e901 0000 00da 00e9 0200 0000  ebug............
+000002c0: 5a0d 7072 6f6a 6563 745f 636f 6c6f 727a  Z.project_colorz
+000002d0: 0950 726f 6a65 6374 3a20 545a 0d70 726f  .Project: TZ.pro
+000002e0: 6669 6c65 5f63 6f6c 6f72 7a09 5072 6f66  file_colorz.Prof
+000002f0: 696c 653a 2029 05da 0563 6c65 6172 da09  ile: )...clear..
+00000300: 6d79 5f6f 7574 7075 7472 0400 0000 7202  my_outputr....r.
+00000310: 0000 0072 0300 0000 2907 7208 0000 0072  ...r....).r....r
+00000320: 0900 0000 720a 0000 0072 0b00 0000 720c  ....r....r....r.
+00000330: 0000 0072 0d00 0000 720e 0000 00a9 0072  ...r....r......r
+00000340: 1600 0000 fa76 2f55 7365 7273 2f6d 696b  .....v/Users/mik
+00000350: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
+00000360: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
+00000370: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
+00000380: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
+00000390: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
+000003a0: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
+000003b0: 632f 6f75 7470 7574 6c2e 7079 da12 7265  c/outputl.py..re
+000003c0: 6672 6573 685f 6f75 725f 6f75 7470 7574  fresh_our_output
+000003d0: 1d00 0000 7332 0000 0008 0914 0308 020c  ....s2..........
+000003e0: 0110 0302 0202 0102 0102 0102 0114 0104  ................
+000003f0: fb04 0910 0202 0102 0102 0102 0102 0102  ................
+00000400: 0110 0102 ff04 fb10 0904 0172 1800 0000  ...........r....
+00000410: da0d 7374 796c 655f 6465 7461 696c 7363  ..style_detailsc
+00000420: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000430: 0800 0000 4300 0000 737c 0000 0064 017d  ....C...s|...d.}
+00000440: 017c 0064 0219 0072 1e64 037c 0064 0419  .|.d...r.d.|.d..
+00000450: 009b 0064 057c 0064 0619 009b 007c 0064  ...d.|.d.....|.d
+00000460: 0719 009b 0064 087c 0064 0919 009b 0064  .....d.|.d.....d
+00000470: 0a9d 087d 017c 0153 007c 0064 0b19 0072  ...}.|.S.|.d...r
+00000480: 3c64 0c7c 0064 0619 009b 0074 009b 0064  <d.|.d.....t...d
+00000490: 087c 0064 0919 009b 0064 0d7c 0064 0419  .|.d.....d.|.d..
+000004a0: 009b 0064 089d 087d 017c 01a0 0164 0e64  ...d...}.|...d.d
+000004b0: 01a1 027d 017c 0153 0029 0f7a e60a 2020  ...}.|.S.).z..  
+000004c0: 2020 4164 6420 6170 7072 6f70 7269 6174    Add appropriat
+000004d0: 6520 4854 4d4c 2073 7479 6c65 2074 6167  e HTML style tag
+000004e0: 7320 6261 7365 6420 6f6e 2070 6172 616d  s based on param
+000004f0: 6574 6572 7320 696e 2064 6963 7469 6f6e  eters in diction
+00000500: 6172 7920 7061 7373 6564 2069 6e0a 2020  ary passed in.  
+00000510: 2020 2020 2020 3a70 6172 616d 2073 7479        :param sty
+00000520: 6c65 5f64 6574 6169 6c73 3a20 5472 7565  le_details: True
+00000530: 2069 6620 7765 2061 7265 2074 6f20 6f75   if we are to ou
+00000540: 7470 7574 2061 206c 6973 7420 283c 6c69  tput a list (<li
+00000550: 3e29 2c20 4661 6c73 6520 6966 206e 6f74  >), False if not
+00000560: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00000570: 3a20 7570 6461 7465 6420 6f75 7470 7574  : updated output
+00000580: 206c 696e 6520 7769 7468 2073 7479 6c65   line with style
+00000590: 2064 6574 6169 6c73 2061 6464 6564 0a20   details added. 
+000005a0: 2020 2072 1200 0000 da07 6973 5f6c 6973     r......is_lis
+000005b0: 747a 113c 6c69 2073 7479 6c65 3d22 636f  tz.<li style="co
+000005c0: 6c6f 723a da06 636f 6c6f 7231 7a15 223e  lor:..color1z.">
+000005d0: 3c73 7061 6e20 7374 796c 653d 2263 6f6c  <span style="col
+000005e0: 6f72 3ada 0663 6f6c 6f72 32da 0466 6f6e  or:..color2..fon
+000005f0: 747a 0222 3eda 0765 6c65 6d65 6e74 fa0d  tz.">..element..
+00000600: 3c2f 7370 616e 3e3c 2f6c 693e 0ada 0c69  </span></li>...i
+00000610: 735f 7461 736b 6572 6e65 747a 333c 7020  s_taskernetz3<p 
+00000620: 7374 796c 653d 226d 6172 6769 6e2d 6c65  style="margin-le
+00000630: 6674 3a32 3070 783b 6d61 7267 696e 2d72  ft:20px;margin-r
+00000640: 6967 6874 3a35 3070 783b 636f 6c6f 723a  ight:50px;color:
+00000650: 7a15 3c2f 703e 0a3c 7020 7374 796c 653d  z.</p>.<p style=
+00000660: 2263 6f6c 6f72 3a7a 0d3c 7370 616e 3e3c  "color:z.<span><
+00000670: 2f73 7061 6e3e 2902 7204 0000 00da 0772  /span>).r......r
+00000680: 6570 6c61 6365 2902 7219 0000 005a 0f6c  eplace).r....Z.l
+00000690: 696e 655f 7769 7468 5f73 7479 6c65 7216  ine_with_styler.
+000006a0: 0000 0072 1600 0000 7217 0000 00da 0970  ...r....r......p
+000006b0: 7574 5f73 7479 6c65 5400 0000 7330 0000  ut_styleT...s0..
+000006c0: 0004 0608 010c 0206 0102 ff06 0104 ff06  ................
+000006d0: 0206 fe02 ff04 0f08 f702 0206 0102 ff02  ................
+000006e0: 0104 ff06 0204 fe06 0306 fd02 ff0c 0604  ................
+000006f0: 0272 2200 0000 721e 0000 00da 0b66 6f6e  .r"...r......fon
+00000700: 745f 746f 5f75 7365 6303 0000 0000 0000  t_to_usec.......
+00000710: 0000 0000 0004 0000 0008 0000 0043 0000  .............C..
+00000720: 0073 6001 0000 7c02 9b00 6401 9d02 7c00  .s`...|...d...|.
+00000730: 7600 730b 6402 7c00 7600 7216 6403 7c01  v.s.d.|.v.r.d.|.
+00000740: 6404 1900 9b00 6405 7c00 9b00 6406 9d05  d.....d.|...d...
+00000750: 5300 7c02 9b00 6407 9d02 7c00 7600 7228  S.|...d...|.v.r(
+00000760: 6403 7c01 6404 1900 9b00 6405 7c00 9b00  d.|.d.....d.|...
+00000770: 6406 9d05 5300 7c00 6400 6408 8502 1900  d...S.|.d.d.....
+00000780: 6409 6b02 7334 640a 7c00 7600 7256 7400  d.k.s4d.|.v.rVt.
+00000790: 7c00 7600 7247 7401 640b 7c01 6404 1900  |.v.rGt.d.|.d...
+000007a0: 7c01 640c 1900 7c02 7c00 640d 9c05 640e  |.d...|.|.d...d.
+000007b0: 8d01 5300 7401 640b 7c01 6404 1900 7c01  ..S.t.d.|.d...|.
+000007c0: 640f 1900 7c02 7c00 640d 9c05 640e 8d01  d...|.|.d...d...
+000007d0: 5300 7c00 6400 6410 8502 1900 6411 6b02  S.|.d.d.....d.k.
+000007e0: 726d 7401 640b 7c01 6404 1900 7c01 6412  rmt.d.|.d...|.d.
+000007f0: 1900 7c02 7c00 640d 9c05 640e 8d01 5300  ..|.|.d...d...S.
+00000800: 6413 7c00 7600 7295 6414 7c00 7600 728a  d.|.v.r.d.|.v.r.
+00000810: 7c00 6415 6400 8502 1900 6416 6b02 727f  |.d.d.....d.k.r.
+00000820: 6416 5300 7402 a003 7c00 a004 6414 6417  d.S.t...|...d.d.
+00000830: a102 a101 7d03 7c03 7d00 6403 7c01 6404  ....}.|.}.d.|.d.
+00000840: 1900 9b00 6405 7c00 9b00 6406 9d05 5300  ....d.|...d...S.
+00000850: 6418 7c00 7600 72a9 7401 6419 7c01 6404  d.|.v.r.t.d.|.d.
+00000860: 1900 7c01 641a 1900 7c02 7c00 640b 641b  ..|.d...|.|.d.d.
+00000870: 9c06 640e 8d01 5300 641c 7c00 9b00 9d02  ..d...S.d.|.....
+00000880: 6406 1700 5300 291d 4e7a 0a22 3e50 726f  d...S.).Nz.">Pro
+00000890: 6a65 6374 3a7a 1750 726f 6a65 6374 2068  ject:z.Project h
+000008a0: 6173 206e 6f20 5072 6f66 696c 6573 7a10  as no Profilesz.
+000008b0: 3c6c 6920 7374 796c 653d 636f 6c6f 723a  <li style=color:
+000008c0: 5a0c 6275 6c6c 6574 5f63 6f6c 6f72 fa01  Z.bullet_color..
+000008d0: 3e72 1f00 0000 7a0a 223e 5072 6f66 696c  >r....z.">Profil
+000008e0: 653a e905 0000 007a 0554 6173 6b3a 7a0f  e:.....z.Task:z.
+000008f0: 2623 3435 3b26 2334 353b 5461 736b 3a54  &#45;&#45;Task:T
+00000900: 5a12 756e 6b6e 6f77 6e5f 7461 736b 5f63  Z.unknown_task_c
+00000910: 6f6c 6f72 2905 721a 0000 0072 1b00 0000  olor).r....r....
+00000920: 721c 0000 0072 1d00 0000 721e 0000 0029  r....r....r....)
+00000930: 0172 1900 0000 5a0a 7461 736b 5f63 6f6c  .r....Z.task_col
+00000940: 6f72 e906 0000 007a 0653 6365 6e65 3a5a  or.....z.Scene:Z
+00000950: 0b73 6365 6e65 5f63 6f6c 6f72 7a07 4163  .scene_colorz.Ac
+00000960: 7469 6f6e 3a7a 0b41 6374 696f 6e3a 202e  tion:z.Action: .
+00000970: 2e2e e90b 0000 0072 1200 0000 7a1a 266e  .......r....z.&n
+00000980: 6273 703b 266e 6273 703b 636f 6e74 696e  bsp;&nbsp;contin
+00000990: 7565 6420 3e3e 3e20 7a0a 5461 736b 6572  ued >>> z.Tasker
+000009a0: 4e65 7420 465a 0f74 6173 6b65 726e 6574  Net FZ.taskernet
+000009b0: 5f63 6f6c 6f72 2906 721a 0000 0072 1b00  _color).r....r..
+000009c0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000009d0: 0072 2000 0000 7a04 3c6c 6920 2905 7205  .r ...z.<li ).r.
+000009e0: 0000 0072 2200 0000 da0f 6163 7469 6f6e  ...r".....action
+000009f0: 5f65 7661 6c75 6174 655a 1263 6c65 616e  _evaluateZ.clean
+00000a00: 7570 5f74 6865 5f72 6573 756c 7472 2100  up_the_resultr!.
+00000a10: 0000 2904 721e 0000 0072 0d00 0000 7223  ..).r....r....r#
+00000a20: 0000 00da 0374 6d70 7216 0000 0072 1600  .....tmpr....r..
+00000a30: 0000 7217 0000 00da 0f75 6c69 6679 5f6c  ..r......ulify_l
+00000a40: 6973 745f 6974 656d 7200 0000 736a 0000  ist_itemr...sj..
+00000a50: 0016 0416 020e 0116 0118 0208 0c02 f702  ................
+00000a60: 0206 0106 0102 0102 0104 fb04 ff02 ff02  ................
+00000a70: 0b02 0206 0106 0102 0102 0104 fb04 ff02  ................
+00000a80: f510 1502 0102 0206 0106 0102 0102 0104  ................
+00000a90: fb06 ff08 0908 0210 0204 0104 010a 0104  ................
+00000aa0: ff04 0316 0108 0102 0102 0206 0106 0102  ................
+00000ab0: 0102 0102 0104 fa06 ff0e 0b72 2a00 0000  ...........r*...
+00000ac0: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
+00000ad0: 0004 0000 0043 0000 0073 a000 0000 6401  .....C...s....d.
+00000ae0: 7d04 7c01 0400 6402 6b02 7221 0100 7c00  }.|...d.k.r!..|.
+00000af0: 6400 6403 8502 1900 6404 6b02 7218 7c00  d.d.....d.k.r.|.
+00000b00: 9b00 6405 1700 7d04 0900 7c04 5300 6406  ..d...}...|.S.d.
+00000b10: 7c00 9b00 9d02 6407 1700 7d04 7c04 5300  |.....d...}.|.S.
+00000b20: 0400 6408 6b02 722f 0100 6409 7c00 9b00  ..d.k.r/..d.|...
+00000b30: 9d02 640a 1700 7d04 7c04 5300 0400 640b  ..d...}.|.S...d.
+00000b40: 6b02 723c 0100 7400 7c00 7c02 7c03 8303  k.r<..t.|.|.|...
+00000b50: 7d04 7c04 5300 0400 640c 6b02 7245 0100  }.|.S...d.k.rE..
+00000b60: 640d 7d04 7c04 5300 640e 6b02 724e 7c00  d.}.|.S.d.k.rN|.
+00000b70: 6405 1700 7d04 7c04 5300 7c04 5300 290f  d...}.|.S.|.S.).
+00000b80: 4e72 1200 0000 7201 0000 0072 2600 0000  Nr....r....r&...
+00000b90: 7a06 3c68 746d 6c3e 7a05 3c62 723e 0a7a  z.<html>z.<br>.z
+00000ba0: 033c 623e 7a09 3c2f 623e 3c62 723e 0a72  .<b>z.</b><br>.r
+00000bb0: 1100 0000 7a04 3c75 6c3e da01 0a72 1300  ....z.<ul>...r..
+00000bc0: 0000 e903 0000 007a 053c 2f75 6c3e e904  .......z.</ul>..
+00000bd0: 0000 0029 0172 2a00 0000 2905 721e 0000  ...).r*...).r...
+00000be0: 005a 036c 766c 720d 0000 0072 2300 0000  .Z.lvlr....r#...
+00000bf0: da06 7374 7269 6e67 7216 0000 0072 1600  ..stringr....r..
+00000c00: 0000 7217 0000 00da 0575 6c69 6679 bb00  ..r......ulify..
+00000c10: 0000 732a 0000 0004 0202 010a 0110 020a  ..s*............
+00000c20: 0102 0204 090e f704 090a f80e 0104 070a  ................
+00000c30: fa0c 0104 050a fc04 0104 0306 fe08 0108  ................
+00000c40: 0172 2f00 0000 da0a 6c69 7374 5f6c 6576  .r/.....list_lev
+00000c50: 656c da0a 6f75 745f 7374 7269 6e67 6305  el..out_stringc.
+00000c60: 0000 0000 0000 0000 0000 0007 0000 0008  ................
+00000c70: 0000 0043 0000 0073 6600 0000 6401 7c04  ...C...sf...d.|.
+00000c80: 7600 7213 7c01 6402 1900 6403 7500 7213  v.r.|.d...d.u.r.
+00000c90: 7c04 a000 6401 a101 7d05 7c05 6404 1900  |...d...}.|.d...
+00000ca0: 7d04 7c02 a001 7402 7c04 7c03 7c00 7c01  }.|...t.|.|.|.|.
+00000cb0: 6405 1900 8304 a101 0100 7403 7231 6406  d.........t.r1d.
+00000cc0: 7402 7c04 7c03 7c00 7c01 6405 1900 8304  t.|.|.|.|.d.....
+00000cd0: 6602 7d06 7404 a005 7c06 a101 0100 6407  f.}.t...|.....d.
+00000ce0: 5300 2908 6154 0100 000a 2020 2020 4164  S.).aT....    Ad
+00000cf0: 6420 6c69 6e65 2074 6f20 7468 6520 6c69  d line to the li
+00000d00: 7374 206f 6620 6f75 7470 7574 206c 696e  st of output lin
+00000d10: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
+00000d20: 6d20 636f 6c6f 726d 6170 3a20 636f 6c6f  m colormap: colo
+00000d30: 7273 2074 6f20 7573 6520 696e 2074 6865  rs to use in the
+00000d40: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
+00000d50: 3a70 6172 616d 2070 726f 6772 616d 5f61  :param program_a
+00000d60: 7267 733a 2072 756e 7469 6d65 2061 7267  rgs: runtime arg
+00000d70: 756d 656e 7473 0a20 2020 2020 2020 203a  uments.        :
+00000d80: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
+00000d90: 743a 206c 6973 7420 6f66 2061 6c6c 206f  t: list of all o
+00000da0: 7574 7075 7420 6c69 6e65 7320 7468 7573  utput lines thus
+00000db0: 2066 6172 0a20 2020 2020 2020 203a 7061   far.        :pa
+00000dc0: 7261 6d20 6c69 7374 5f6c 6576 656c 3a20  ram list_level: 
+00000dd0: 6c65 7665 6c20 7765 2061 7265 206f 7574  level we are out
+00000de0: 7075 7474 696e 670a 2020 2020 2020 2020  putting.        
+00000df0: 3a70 6172 616d 206f 7574 5f73 7472 696e  :param out_strin
+00000e00: 673a 2074 6865 2073 7472 696e 6720 746f  g: the string to
+00000e10: 2061 6464 2074 6f20 7468 6520 6f75 7470   add to the outp
+00000e20: 7574 0a20 2020 2020 2020 203a 7265 7475  ut.        :retu
+00000e30: 726e 3a20 6e6f 6e65 0a20 2020 207a 0854  rn: none.    z.T
+00000e40: 6173 6b20 4944 3a72 1000 0000 4672 0100  ask ID:r....Fr..
+00000e50: 0000 7223 0000 007a 0b6f 7574 5f73 7472  ..r#...z.out_str
+00000e60: 696e 673a 4e29 06da 0573 706c 6974 da06  ing:N)...split..
+00000e70: 6170 7065 6e64 722f 0000 0072 0600 0000  appendr/...r....
+00000e80: 7207 0000 0072 1000 0000 2907 720d 0000  r....r....).r...
+00000e90: 0072 0e00 0000 7209 0000 0072 3000 0000  .r....r....r0...
+00000ea0: 7231 0000 005a 0c74 656d 705f 656c 656d  r1...Z.temp_elem
+00000eb0: 656e 745a 0964 6562 7567 5f6d 7367 7216  entZ.debug_msgr.
+00000ec0: 0000 0072 1600 0000 7217 0000 0072 1500  ...r....r....r..
+00000ed0: 0000 d300 0000 7318 0000 0014 110a 0208  ......s.........
+00000ee0: 0104 0110 0104 ff04 0404 010c 0106 ff0a  ................
+00000ef0: 0304 0172 1500 0000 291b da16 6465 6675  ...r....)...defu
+00000f00: 7365 6478 6d6c 2e45 6c65 6d65 6e74 5472  sedxml.ElementTr
+00000f10: 6565 da0a 6465 6675 7365 6478 6d6c 5a15  ee..defusedxmlZ.
+00000f20: 6d61 7074 6173 6b65 722e 7372 632e 6163  maptasker.src.ac
+00000f30: 7469 6f6e 65da 0373 7263 5a07 6163 7469  tione..srcZ.acti
+00000f40: 6f6e 6572 2800 0000 5a13 6d61 7074 6173  oner(...Z.maptas
+00000f50: 6b65 722e 7372 632e 6465 6275 6772 0200  ker.src.debugr..
+00000f60: 0000 5a16 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
+00000f70: 632e 6672 6d74 6874 6d6c 7203 0000 00da  c.frmthtmlr.....
+00000f80: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
+00000f90: 7973 636f 6e73 7472 0400 0000 7205 0000  ysconstr....r...
+00000fa0: 0072 0600 0000 7207 0000 00da 0462 6f6f  .r....r......boo
+00000fb0: 6cda 046c 6973 74da 0373 7472 da04 6469  l..list..str..di
+00000fc0: 6374 7218 0000 0072 2200 0000 da0b 456c  ctr....r".....El
+00000fd0: 656d 656e 7454 7265 65da 0358 4d4c 722a  ementTree..XMLr*
+00000fe0: 0000 0072 2f00 0000 da03 696e 7472 1500  ...r/.....intr..
+00000ff0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00001000: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001010: 0100 0000 7362 0000 0008 0e12 020c 010c  ....sb..........
+00001020: 010c 010c 010c 010c 0102 0602 0102 ff02  ................
+00001030: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
+00001040: 0602 fa02 0702 f902 080a f812 3702 1e06  ............7...
+00001050: 0102 ff02 0102 ff02 0102 ff02 020a fe08  ................
+00001060: 4902 1802 0102 ff02 0202 fe02 0302 fd02  I...............
+00001070: 0402 fc02 0502 fb02 060e fa              ...........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/parsearg.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/parsearg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/prefers.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/prefers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 18:39:13 2023 UTC, .py size: 7310 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-00000000: 6f0d 0d0a 0000 0000 51d7 2564 8e1c 0000  o.......Q.%d....
+00000000: 6f0d 0d0a 0000 0000 f189 3564 6a1e 0000  o.........5dj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 650a 6407 650b 6408 650b 6409 650c 640a  e.d.e.d.e.d.e.d.
 00000080: 6401 660a 640b 640c 8404 5a0d 640d 650c  d.f.d.d...Z.d.e.
 00000090: 640e 650a 6406 650a 640f 650a 640a 6401  d.e.d.e.d.e.d.d.
 000000a0: 660a 6410 6411 8404 5a0e 6401 5300 2912  f.d.d...Z.d.S.).
 000000b0: e900 0000 004e 2901 da0a 6974 656d 6765  .....N)...itemge
 000000c0: 7474 6572 2901 da09 6d79 5f6f 7574 7075  tter)...my_outpu
-000000d0: 7429 01da 0d73 6572 7669 6365 5f63 6f64  t)...service_cod
-000000e0: 6573 2901 da0b 464f 4e54 5f54 4f5f 5553  es)...FONT_TO_US
-000000f0: 45da 0863 6f6c 6f72 6d61 70da 0c73 6572  E..colormap..ser
+000000d0: 7429 01da 0b66 6f72 6d61 745f 6874 6d6c  t)...format_html
+000000e0: 2901 da0d 7365 7276 6963 655f 636f 6465  )...service_code
+000000f0: 73da 0863 6f6c 6f72 6d61 70da 0c73 6572  s..colormap..ser
 00000100: 7669 6365 5f6e 616d 65da 0d73 6572 7669  vice_name..servi
 00000110: 6365 5f76 616c 7565 da0c 6f75 7470 7574  ce_value..output
 00000120: 5f6c 696e 6573 da06 7265 7475 726e 6304  _lines..returnc.
-00000130: 0000 0000 0000 0000 0000 000c 0000 0009  ................
-00000140: 0000 0043 0000 0073 0a01 0000 6401 7c00  ...C...s....d.|.
-00000150: 6402 1900 1700 7400 1700 6403 1700 7d04  d.....t...d...}.
-00000160: 6404 7d05 7401 7c01 1900 6405 1900 7d06  d.}.t.|...d...}.
-00000170: 7c06 a002 6406 6407 a102 7d06 6408 7401  |...d.d...}.d.t.
-00000180: 7c01 1900 7600 7228 7401 7c01 1900 6408  |...v.r(t.|...d.
-00000190: 1900 7403 7c02 8301 1900 7d02 7c02 6409  ..t.|.....}.|.d.
-000001a0: 6b02 722f 640a 7d02 6e3a 7c01 640b 6b02  k.r/d.}.n:|.d.k.
-000001b0: 7269 640c 7d07 640d 640e 8400 7404 a005  rid.}.d.d...t...
-000001c0: 640f 7c02 a102 4400 8301 7d08 6410 640e  d.|...D...}.d.d.
-000001d0: 8400 7404 a005 6411 7c02 a102 4400 8301  ..t...d.|...D...
-000001e0: 7d09 7406 7c08 8301 4400 5d17 5c02 7d0a  }.t.|...D.].\.}.
-000001f0: 7d0b 7c07 9b00 6412 7c05 6413 1400 9b00  }.|...d.|.d.....
-00000200: 7c02 7c0b 6414 1700 7c09 7c0a 1900 8502  |.|.d...|.|.....
-00000210: 1900 9b00 9d04 7d07 714f 7c07 7d02 7c03  ......}.qO|.}.|.
-00000220: a007 7401 7c01 1900 6415 1900 7c04 9b00  ..t.|...d...|...
-00000230: 7c05 6416 1400 9b00 7c06 9b00 7c05 6417  |.d.....|...|.d.
-00000240: 1400 9b00 7c02 9b00 6418 9d06 6702 a101  ....|...d...g...
-00000250: 0100 6419 5300 291a 616c 0100 000a 2020  ..d.S.).al....  
-00000260: 2020 5765 2068 6176 6520 6120 7365 7276    We have a serv
-00000270: 6963 6520 786d 6c20 656c 656d 656e 7420  ice xml element 
-00000280: 7468 6174 2077 6520 6861 7665 206d 6170  that we have map
-00000290: 7065 6420 6173 2061 2070 7265 6665 7265  ped as a prefere
-000002a0: 6e63 652e 2020 5072 6f63 6573 7320 6974  nce.  Process it
-000002b0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000002c0: 2063 6f6c 6f72 6d61 703a 2063 6f6c 6f72   colormap: color
-000002d0: 7320 746f 2075 7365 2069 6e20 6f75 7470  s to use in outp
-000002e0: 7574 0a20 2020 2020 2020 203a 7061 7261  ut.        :para
-000002f0: 6d20 7365 7276 6963 655f 6e61 6d65 3a20  m service_name: 
-00000300: 6e61 6d65 206f 6620 7468 6520 7072 6566  name of the pref
-00000310: 6572 656e 6365 2069 6e20 3c53 6572 7669  erence in <Servi
-00000320: 6365 2078 6d6c 0a20 2020 2020 2020 203a  ce xml.        :
-00000330: 7061 7261 6d20 7365 7276 6963 655f 7661  param service_va
-00000340: 6c75 653a 2076 616c 7565 206f 6620 7468  lue: value of th
-00000350: 6520 7072 6566 6572 656e 6365 2069 6e20  e preference in 
-00000360: 3c53 6572 7669 6365 2078 6d6c 0a20 2020  <Service xml.   
-00000370: 2020 2020 203a 7061 7261 6d20 6f75 7470       :param outp
-00000380: 7574 5f6c 696e 6573 3a20 6163 6375 6d75  ut_lines: accumu
-00000390: 6c61 7465 6420 6f75 7470 7574 206c 696e  lated output lin
-000003a0: 6573 2067 656e 6572 6174 6564 2074 6875  es generated thu
-000003b0: 7320 6661 7220 2874 6f20 6170 7065 6e64  s far (to append
-000003c0: 2074 6f29 0a20 2020 20fa 1420 3c73 7061   to).    .. <spa
-000003d0: 6e20 7374 796c 653d 2263 6f6c 6f72 3ada  n style="color:.
-000003e0: 1170 7265 6665 7265 6e63 6573 5f63 6f6c  .preferences_col
-000003f0: 6f72 fa01 3efa 0626 6e62 7370 3bda 0764  or..>..&nbsp;..d
-00000400: 6973 706c 6179 e92d 0000 00da 012e da06  isplay.-........
-00000410: 7661 6c75 6573 5a11 6375 7374 5f6e 6f74  valuesZ.cust_not
-00000420: 6966 6963 6174 696f 6e5a 0744 6566 6175  ificationZ.Defau
-00000430: 6c74 5a28 5052 4546 5f4b 4545 505f 4143  ltZ(PREF_KEEP_AC
-00000440: 4345 5353 4942 494c 4954 595f 5345 5256  CESSIBILITY_SERV
-00000450: 4943 4553 5f52 554e 4e49 4e47 da00 6301  ICES_RUNNING..c.
-00000460: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000470: 0000 0053 0000 00f3 1400 0000 6700 7c00  ...S........g.|.
-00000480: 5d06 7d01 7c01 a000 a100 9102 7102 5300  ].}.|.......q.S.
-00000490: a900 a901 da05 7374 6172 74a9 02da 022e  ......start.....
-000004a0: 30da 016d 7215 0000 0072 1500 0000 fa76  0..mr....r.....v
-000004b0: 2f55 7365 7273 2f6d 696b 7275 6269 6e2f  /Users/mikrubin/
-000004c0: 4c69 6272 6172 792f 436c 6f75 6453 746f  Library/CloudSto
-000004d0: 7261 6765 2f47 6f6f 676c 6544 7269 7665  rage/GoogleDrive
-000004e0: 2d6d 696b 7275 6269 6e40 676d 6169 6c2e  -mikrubin@gmail.
-000004f0: 636f 6d2f 4d79 2044 7269 7665 2f50 7974  com/My Drive/Pyt
-00000500: 686f 6e2f 6d61 7074 6173 6b65 722f 6d61  hon/maptasker/ma
-00000510: 7074 6173 6b65 722f 7372 632f 7072 6566  ptasker/src/pref
-00000520: 6572 732e 7079 da0a 3c6c 6973 7463 6f6d  ers.py..<listcom
-00000530: 703e 3600 0000 f302 0000 0014 007a 2370  p>6..........z#p
-00000540: 726f 6365 7373 5f73 6572 7669 6365 2e3c  rocess_service.<
-00000550: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000560: 703e 7a0e 2270 6163 6b61 6765 4e61 6d65  p>z."packageName
-00000570: 223a 6301 0000 0000 0000 0000 0000 0002  ":c.............
-00000580: 0000 0004 0000 0053 0000 0072 1400 0000  .......S...r....
-00000590: 7215 0000 0072 1600 0000 7218 0000 0072  r....r....r....r
-000005a0: 1500 0000 7215 0000 0072 1b00 0000 721c  ....r....r....r.
-000005b0: 0000 0037 0000 0072 1d00 0000 da01 7dfa  ...7...r......}.
-000005c0: 043c 6272 3ee9 3200 0000 e90e 0000 00da  .<br>.2.........
-000005d0: 036e 756d e902 0000 00e9 0400 0000 fa07  .num............
-000005e0: 3c2f 7370 616e 3e4e 2908 7205 0000 0072  </span>N).r....r
-000005f0: 0400 0000 da05 6c6a 7573 74da 0369 6e74  ......ljust..int
-00000600: da02 7265 da08 6669 6e64 6974 6572 da09  ..re..finditer..
-00000610: 656e 756d 6572 6174 65da 0661 7070 656e  enumerate..appen
-00000620: 6429 0c72 0600 0000 7207 0000 0072 0800  d).r....r....r..
-00000630: 0000 7209 0000 00da 1070 7265 6665 7265  ..r......prefere
-00000640: 6e63 6573 5f68 746d 6cda 0562 6c61 6e6b  nces_html..blank
-00000650: 5a13 6f75 7470 7574 5f73 6572 7669 6365  Z.output_service
-00000660: 5f6e 616d 655a 0d70 6163 6b61 6765 5f6e  _nameZ.package_n
-00000670: 616d 6573 5a08 7061 636b 6167 6573 5a0c  amesZ.packagesZ.
-00000680: 7061 636b 6167 6573 5f65 6e64 da06 6e75  packages_end..nu
-00000690: 6d62 6572 da08 706f 7369 7469 6f6e 7215  mber..positionr.
-000006a0: 0000 0072 1500 0000 721b 0000 00da 0f70  ...r....r......p
-000006b0: 726f 6365 7373 5f73 6572 7669 6365 1700  rocess_service..
-000006c0: 0000 732c 0000 0012 0b02 ff04 030c 030c  ..s,............
-000006d0: 020c 0314 0108 0406 0108 0204 0116 0116  ................
-000006e0: 0110 0124 0204 ff04 0304 030a 0220 0202  ...$......... ..
-000006f0: fd08 ff72 3000 0000 da0b 6f75 7470 7574  ...r0.....output
-00000700: 5f6c 6973 74da 0c70 726f 6772 616d 5f61  _list..program_a
-00000710: 7267 73da 1061 6c6c 5f74 6173 6b65 725f  rgs..all_tasker_
-00000720: 6974 656d 7363 0400 0000 0000 0000 0000  itemsc..........
-00000730: 0000 1300 0000 0e00 0000 4300 0000 73be  ..........C...s.
-00000740: 0100 0067 0064 01a2 017d 0467 007d 0564  ...g.d...}.g.}.d
-00000750: 027c 0264 0319 0017 0074 0017 0064 0417  .|.d.....t...d..
-00000760: 007d 0664 057d 0764 067d 0874 017c 027c  .}.d.}.d.}.t.|.|
-00000770: 017c 0064 077c 069b 0064 089d 0283 0501  .|.d.|...d......
-00000780: 0064 097d 0964 0a7d 0a7c 0364 0b19 0044  .d.}.d.}.|.d...D
-00000790: 005d 4e7d 0b7c 0ba0 0264 0ca1 016a 037d  .]N}.|...d...j.}
-000007a0: 0c7c 0ba0 0264 0da1 016a 037d 0d7c 0ba0  .|...d...j.}.|..
-000007b0: 0264 0ea1 016a 037d 0e7c 0c74 0476 0072  .d...j.}.|.t.v.r
-000007c0: 4774 057c 027c 0c7c 0e7c 0583 0401 0071  Gt.|.|.|.|.....q
-000007d0: 277c 0164 0f19 0072 757c 0872 5664 107d  '|.d...ru|.rVd.}
-000007e0: 087c 05a0 067c 0a64 1167 02a1 0101 007c  .|...|.d.g.....|
-000007f0: 05a0 067c 0a7c 069b 0064 127c 0c9b 007c  ...|.|...d.|...|
-00000800: 0764 0714 009b 0064 137c 0d9b 007c 0764  .d.....d.|...|.d
-00000810: 0714 009b 0064 147c 0e9b 0064 159d 0a67  .....d.|...d...g
-00000820: 02a1 0101 007c 0a64 1637 007d 0a71 2774  .....|.d.7.}.q't
-00000830: 077c 0574 0864 1783 0164 188d 027d 0f7c  .|.t.d...d...}.|
-00000840: 0f44 005d 427d 107c 1064 1719 007d 1174  .D.]B}.|.d...}.t
-00000850: 04a0 09a1 0044 005d 2d7d 127c 1264 1619  .....D.]-}.|.d..
-00000860: 0064 1919 007c 116b 0272 b77c 097c 1264  .d...|.k.r.|.|.d
-00000870: 1619 0064 1a19 006b 0372 b774 017c 027c  ...d...k.r.t.|.|
-00000880: 017c 0064 0764 117c 069b 0064 1b7c 047c  .|.d.d.|...d.|.|
-00000890: 1264 1619 0064 1a19 0019 009b 0064 159d  .d...d.......d..
-000008a0: 0583 0501 007c 1264 1619 0064 1a19 007d  .....|.d...d...}
-000008b0: 0971 8a74 017c 027c 017c 0064 077c 1064  .q.t.|.|.|.d.|.d
-000008c0: 1619 0083 0501 0071 8074 017c 027c 017c  .......q.t.|.|.|
-000008d0: 0064 077c 069b 0064 1c9d 0283 0501 0074  .d.|...d.......t
-000008e0: 017c 027c 017c 0064 0764 1d83 0501 007c  .|.|.|.d.d.....|
-000008f0: 0364 0b3d 0074 0aa0 0ba1 0001 0064 1e53  .d.=.t.......d.S
-00000900: 0029 1f61 2b01 0000 0a20 2020 2047 6574  .).a+....    Get
-00000910: 2054 6173 6b65 7220 2770 7265 6665 7265   Tasker 'prefere
-00000920: 6e63 6573 2720 616e 6420 6f75 7470 7574  nces' and output
-00000930: 2074 6865 6d0a 2020 2020 2020 2020 3a70   them.        :p
-00000940: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
-00000950: 3a20 6c69 7374 206f 6620 6f75 7470 7574  : list of output
-00000960: 206c 696e 6573 2067 656e 6572 6174 6564   lines generated
-00000970: 2074 6875 7320 6661 720a 2020 2020 2020   thus far.      
-00000980: 2020 3a70 6172 616d 2070 726f 6772 616d    :param program
-00000990: 5f61 7267 733a 2072 756e 7469 6d65 2061  _args: runtime a
-000009a0: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-000009b0: 203a 7061 7261 6d20 636f 6c6f 726d 6170   :param colormap
-000009c0: 3a20 636f 6c6f 7273 2074 6f20 7573 6520  : colors to use 
-000009d0: 696e 2070 7574 7075 740a 2020 2020 2020  in putput.      
-000009e0: 2020 3a70 6172 616d 2061 6c6c 5f74 6173    :param all_tas
-000009f0: 6b65 725f 6974 656d 733a 2061 6c6c 2050  ker_items: all P
-00000a00: 726f 6a65 6374 2f50 726f 6669 6c65 2f54  roject/Profile/T
-00000a10: 6173 6b2f 5363 656e 652f 5365 7276 6963  ask/Scene/Servic
-00000a20: 6520 786d 6c20 656c 656d 656e 7473 0a20  e xml elements. 
-00000a30: 2020 2029 0e7a 0c55 4920 3e20 4765 6e65     ).z.UI > Gene
-00000a40: 7261 6c7a 1055 4920 3e20 4d61 696e 2053  ralz.UI > Main S
-00000a50: 6372 6565 6e7a 0c55 4920 3e20 5549 204c  creenz.UI > UI L
-00000a60: 6f63 6b7a 1155 4920 3e20 4c6f 6361 6c69  ockz.UI > Locali
-00000a70: 7a61 7469 6f6e 7a11 4d6f 6e69 746f 7220  zationz.Monitor 
-00000a80: 3e20 4765 6e65 7261 6c7a 1f4d 6f6e 6974  > Generalz.Monit
-00000a90: 6f72 203e 2044 6973 706c 6179 204f 6e20  or > Display On 
-00000aa0: 4d6f 6e69 746f 7269 6e67 7a20 4d6f 6e69  Monitoringz Moni
-00000ab0: 746f 7220 3e20 4469 7370 6c61 7920 4f66  tor > Display Of
-00000ac0: 6620 4d6f 6e69 746f 7269 6e67 7a1c 4d6f  f Monitoringz.Mo
-00000ad0: 6e69 746f 7220 3e20 4765 6e65 7261 6c20  nitor > General 
-00000ae0: 4d6f 6e69 746f 7269 6e67 7a13 4d6f 6e69  Monitoringz.Moni
-00000af0: 746f 7220 3e20 4361 6c69 6272 6174 65da  tor > Calibrate.
-00000b00: 0641 6374 696f 6e7a 2241 6374 696f 6e20  .Actionz"Action 
-00000b10: 3e20 5265 7365 7420 4572 726f 7220 4e6f  > Reset Error No
-00000b20: 7469 6669 6361 7469 6f6e 73da 044d 6973  tifications..Mis
-00000b30: 637a 104d 6973 6320 3e20 4465 6275 6767  cz.Misc > Debugg
-00000b40: 696e 677a 1d55 6e6c 6973 7465 6420 2850  ingz.Unlisted (P
-00000b50: 6572 6861 7073 2044 6570 7265 6361 7465  erhaps Deprecate
-00000b60: 6429 720b 0000 0072 0c00 0000 720d 0000  d)r....r....r...
-00000b70: 0072 0e00 0000 5472 2400 0000 7a42 5461  .r....Tr$...zBTa
+00000130: 0000 0000 0000 0000 0000 000c 0000 000c  ................
+00000140: 0000 0043 0000 0073 1001 0000 7400 7c00  ...C...s....t.|.
+00000150: 6401 6402 6402 6403 8305 7d04 6404 7d05  d.d.d.d...}.d.}.
+00000160: 7401 7c01 1900 6405 1900 7d06 7c06 a002  t.|...d...}.|...
+00000170: 6406 6407 a102 7d06 6408 7401 7c01 1900  d.d...}.d.t.|...
+00000180: 7600 7226 7401 7c01 1900 6408 1900 7403  v.r&t.|...d...t.
+00000190: 7c02 8301 1900 7d02 7c02 6409 6b02 722d  |.....}.|.d.k.r-
+000001a0: 640a 7d02 6e3a 7c01 640b 6b02 7267 6402  d.}.n:|.d.k.rgd.
+000001b0: 7d07 640c 640d 8400 7404 a005 640e 7c02  }.d.d...t...d.|.
+000001c0: a102 4400 8301 7d08 640f 640d 8400 7404  ..D...}.d.d...t.
+000001d0: a005 6410 7c02 a102 4400 8301 7d09 7406  ..d.|...D...}.t.
+000001e0: 7c08 8301 4400 5d17 5c02 7d0a 7d0b 7c07  |...D.].\.}.}.|.
+000001f0: 9b00 6411 7c05 6412 1400 9b00 7c02 7c0b  ..d.|.d.....|.|.
+00000200: 6413 1700 7c09 7c0a 1900 8502 1900 9b00  d...|.|.........
+00000210: 9d04 7d07 714d 7c07 7d02 7c03 a007 7401  ..}.qM|.}.|...t.
+00000220: 7c01 1900 6414 1900 7400 7c00 6401 6402  |...d...t.|.d.d.
+00000230: 7c04 9b00 7c05 6415 1400 9b00 7c06 9b00  |...|.d.....|...
+00000240: 7c05 6416 1400 9b00 7c02 9b00 9d05 6417  |.d.....|.....d.
+00000250: 8305 6702 a101 0100 6418 5300 2919 616c  ..g.....d.S.).al
+00000260: 0100 000a 2020 2020 5765 2068 6176 6520  ....    We have 
+00000270: 6120 7365 7276 6963 6520 786d 6c20 656c  a service xml el
+00000280: 656d 656e 7420 7468 6174 2077 6520 6861  ement that we ha
+00000290: 7665 206d 6170 7065 6420 6173 2061 2070  ve mapped as a p
+000002a0: 7265 6665 7265 6e63 652e 2020 5072 6f63  reference.  Proc
+000002b0: 6573 7320 6974 2e0a 2020 2020 2020 2020  ess it..        
+000002c0: 3a70 6172 616d 2063 6f6c 6f72 6d61 703a  :param colormap:
+000002d0: 2063 6f6c 6f72 7320 746f 2075 7365 2069   colors to use i
+000002e0: 6e20 6f75 7470 7574 0a20 2020 2020 2020  n output.       
+000002f0: 203a 7061 7261 6d20 7365 7276 6963 655f   :param service_
+00000300: 6e61 6d65 3a20 6e61 6d65 206f 6620 7468  name: name of th
+00000310: 6520 7072 6566 6572 656e 6365 2069 6e20  e preference in 
+00000320: 3c53 6572 7669 6365 2078 6d6c 0a20 2020  <Service xml.   
+00000330: 2020 2020 203a 7061 7261 6d20 7365 7276       :param serv
+00000340: 6963 655f 7661 6c75 653a 2076 616c 7565  ice_value: value
+00000350: 206f 6620 7468 6520 7072 6566 6572 656e   of the preferen
+00000360: 6365 2069 6e20 3c53 6572 7669 6365 2078  ce in <Service x
+00000370: 6d6c 0a20 2020 2020 2020 203a 7061 7261  ml.        :para
+00000380: 6d20 6f75 7470 7574 5f6c 696e 6573 3a20  m output_lines: 
+00000390: 6163 6375 6d75 6c61 7465 6420 6f75 7470  accumulated outp
+000003a0: 7574 206c 696e 6573 2067 656e 6572 6174  ut lines generat
+000003b0: 6564 2074 6875 7320 6661 7220 2874 6f20  ed thus far (to 
+000003c0: 6170 7065 6e64 2074 6f29 0a20 2020 20da  append to).    .
+000003d0: 1170 7265 6665 7265 6e63 6573 5f63 6f6c  .preferences_col
+000003e0: 6f72 da00 46fa 0626 6e62 7370 3bda 0764  or..F..&nbsp;..d
+000003f0: 6973 706c 6179 e92d 0000 00da 012e da06  isplay.-........
+00000400: 7661 6c75 6573 5a11 6375 7374 5f6e 6f74  valuesZ.cust_not
+00000410: 6966 6963 6174 696f 6e5a 0744 6566 6175  ificationZ.Defau
+00000420: 6c74 5a28 5052 4546 5f4b 4545 505f 4143  ltZ(PREF_KEEP_AC
+00000430: 4345 5353 4942 494c 4954 595f 5345 5256  CESSIBILITY_SERV
+00000440: 4943 4553 5f52 554e 4e49 4e47 6301 0000  ICES_RUNNINGc...
+00000450: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000460: 0053 0000 00f3 1400 0000 6700 7c00 5d06  .S........g.|.].
+00000470: 7d01 7c01 a000 a100 9102 7102 5300 a900  }.|.......q.S...
+00000480: a901 da05 7374 6172 74a9 02da 022e 30da  ....start.....0.
+00000490: 016d 7213 0000 0072 1300 0000 fa76 2f55  .mr....r.....v/U
+000004a0: 7365 7273 2f6d 696b 7275 6269 6e2f 4c69  sers/mikrubin/Li
+000004b0: 6272 6172 792f 436c 6f75 6453 746f 7261  brary/CloudStora
+000004c0: 6765 2f47 6f6f 676c 6544 7269 7665 2d6d  ge/GoogleDrive-m
+000004d0: 696b 7275 6269 6e40 676d 6169 6c2e 636f  ikrubin@gmail.co
+000004e0: 6d2f 4d79 2044 7269 7665 2f50 7974 686f  m/My Drive/Pytho
+000004f0: 6e2f 6d61 7074 6173 6b65 722f 6d61 7074  n/maptasker/mapt
+00000500: 6173 6b65 722f 7372 632f 7072 6566 6572  asker/src/prefer
+00000510: 732e 7079 da0a 3c6c 6973 7463 6f6d 703e  s.py..<listcomp>
+00000520: 3400 0000 f302 0000 0014 007a 2370 726f  4..........z#pro
+00000530: 6365 7373 5f73 6572 7669 6365 2e3c 6c6f  cess_service.<lo
+00000540: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00000550: 7a0e 2270 6163 6b61 6765 4e61 6d65 223a  z."packageName":
+00000560: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000570: 0004 0000 0053 0000 0072 1200 0000 7213  .....S...r....r.
+00000580: 0000 0072 1400 0000 7216 0000 0072 1300  ...r....r....r..
+00000590: 0000 7213 0000 0072 1900 0000 721a 0000  ..r....r....r...
+000005a0: 0035 0000 0072 1b00 0000 da01 7dfa 043c  .5...r......}..<
+000005b0: 6272 3ee9 3200 0000 e90e 0000 00da 036e  br>.2..........n
+000005c0: 756d e902 0000 00e9 0400 0000 544e 2908  um..........TN).
+000005d0: 7204 0000 0072 0500 0000 da05 6c6a 7573  r....r......ljus
+000005e0: 74da 0369 6e74 da02 7265 da08 6669 6e64  t..int..re..find
+000005f0: 6974 6572 da09 656e 756d 6572 6174 65da  iter..enumerate.
+00000600: 0661 7070 656e 6429 0c72 0600 0000 7207  .append).r....r.
+00000610: 0000 0072 0800 0000 7209 0000 00da 1070  ...r....r......p
+00000620: 7265 6665 7265 6e63 6573 5f68 746d 6cda  references_html.
+00000630: 0562 6c61 6e6b 5a13 6f75 7470 7574 5f73  .blankZ.output_s
+00000640: 6572 7669 6365 5f6e 616d 655a 0d70 6163  ervice_nameZ.pac
+00000650: 6b61 6765 5f6e 616d 6573 da08 7061 636b  kage_names..pack
+00000660: 6167 6573 5a0c 7061 636b 6167 6573 5f65  agesZ.packages_e
+00000670: 6e64 da06 6e75 6d62 6572 da08 706f 7369  nd..number..posi
+00000680: 7469 6f6e 7213 0000 0072 1300 0000 7219  tionr....r....r.
+00000690: 0000 00da 0f70 726f 6365 7373 5f73 6572  .....process_ser
+000006a0: 7669 6365 1700 0000 7336 0000 0010 0a04  vice....s6......
+000006b0: 010c 030c 020c 0314 0108 0406 0108 0204  ................
+000006c0: 0116 0116 0110 0124 0204 ff04 0304 020a  .......$........
+000006d0: 0202 0202 0102 0102 011e 0202 0202 f902  ................
+000006e0: fd08 ff72 2e00 0000 da0b 6f75 7470 7574  ...r......output
+000006f0: 5f6c 6973 74da 0c70 726f 6772 616d 5f61  _list..program_a
+00000700: 7267 73da 1061 6c6c 5f74 6173 6b65 725f  rgs..all_tasker_
+00000710: 6974 656d 7363 0400 0000 0000 0000 0000  itemsc..........
+00000720: 0000 1300 0000 1100 0000 4300 0000 73d2  ..........C...s.
+00000730: 0100 0067 0064 01a2 017d 0467 007d 0574  ...g.d...}.g.}.t
+00000740: 007c 0264 0264 0364 0364 0483 057d 0664  .|.d.d.d.d...}.d
+00000750: 057d 0764 067d 0874 017c 027c 017c 0064  .}.d.}.t.|.|.|.d
+00000760: 0774 007c 0264 0264 0364 0864 0683 0583  .t.|.d.d.d.d....
+00000770: 0501 0064 097d 0964 0a7d 0a7c 0364 0b19  ...d.}.d.}.|.d..
+00000780: 0044 005d 557d 0b7c 0ba0 0264 0ca1 016a  .D.]U}.|...d...j
+00000790: 037d 0c7c 0ba0 0264 0da1 016a 037d 0d7c  .}.|...d...j.}.|
+000007a0: 0ba0 0264 0ea1 016a 037d 0e7c 0c74 0476  ...d...j.}.|.t.v
+000007b0: 0072 4874 057c 027c 0c7c 0e7c 0583 0401  .rHt.|.|.|.|....
+000007c0: 0071 287c 0164 0f19 0072 7d7c 0872 5764  .q(|.d...r}|.rWd
+000007d0: 047d 087c 05a0 067c 0a64 1067 02a1 0101  .}.|...|.d.g....
+000007e0: 007c 05a0 067c 0a74 007c 0264 0264 037c  .|...|.t.|.d.d.|
+000007f0: 0764 1114 009b 0064 127c 0c9b 007c 0764  .d.....d.|...|.d
+00000800: 0714 009b 0064 137c 0d9b 007c 0764 0714  .....d.|...|.d..
+00000810: 009b 0064 147c 0e9b 009d 0964 0683 0567  ...d.|.....d...g
+00000820: 02a1 0101 007c 0a64 1537 007d 0a71 2874  .....|.d.7.}.q(t
+00000830: 077c 0574 0864 1683 0164 178d 027d 0f7c  .|.t.d...d...}.|
+00000840: 0f44 005d 447d 107c 1064 1619 007d 1174  .D.]D}.|.d...}.t
+00000850: 04a0 09a1 0044 005d 2f7d 127c 1264 1519  .....D.]/}.|.d..
+00000860: 0064 1819 007c 116b 0272 c17c 097c 1264  .d...|.k.r.|.|.d
+00000870: 1519 0064 1919 006b 0372 c174 017c 027c  ...d...k.r.t.|.|
+00000880: 017c 0064 0774 007c 0264 0264 0364 1a7c  .|.d.t.|.d.d.d.|
+00000890: 047c 1264 1519 0064 1919 0019 009b 009d  .|.d...d........
+000008a0: 0264 0683 0583 0501 007c 1264 1519 0064  .d.......|.d...d
+000008b0: 1919 007d 0971 9274 017c 027c 017c 0064  ...}.q.t.|.|.|.d
+000008c0: 077c 1064 1519 0083 0501 0071 8874 017c  .|.d.......q.t.|
+000008d0: 027c 017c 0064 077c 069b 0064 1b9d 0283  .|.|.d.|...d....
+000008e0: 0501 0074 017c 027c 017c 0064 0764 0383  ...t.|.|.|.d.d..
+000008f0: 0501 007c 0364 0b3d 0074 0aa0 0ba1 0001  ...|.d.=.t......
+00000900: 0064 1c53 0029 1d61 2b01 0000 0a20 2020  .d.S.).a+....   
+00000910: 2047 6574 2054 6173 6b65 7220 2770 7265   Get Tasker 'pre
+00000920: 6665 7265 6e63 6573 2720 616e 6420 6f75  ferences' and ou
+00000930: 7470 7574 2074 6865 6d0a 2020 2020 2020  tput them.      
+00000940: 2020 3a70 6172 616d 206f 7574 7075 745f    :param output_
+00000950: 6c69 7374 3a20 6c69 7374 206f 6620 6f75  list: list of ou
+00000960: 7470 7574 206c 696e 6573 2067 656e 6572  tput lines gener
+00000970: 6174 6564 2074 6875 7320 6661 720a 2020  ated thus far.  
+00000980: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
+00000990: 6772 616d 5f61 7267 733a 2072 756e 7469  gram_args: runti
+000009a0: 6d65 2061 7267 756d 656e 7473 0a20 2020  me arguments.   
+000009b0: 2020 2020 203a 7061 7261 6d20 636f 6c6f       :param colo
+000009c0: 726d 6170 3a20 636f 6c6f 7273 2074 6f20  rmap: colors to 
+000009d0: 7573 6520 696e 2070 7574 7075 740a 2020  use in putput.  
+000009e0: 2020 2020 2020 3a70 6172 616d 2061 6c6c        :param all
+000009f0: 5f74 6173 6b65 725f 6974 656d 733a 2061  _tasker_items: a
+00000a00: 6c6c 2050 726f 6a65 6374 2f50 726f 6669  ll Project/Profi
+00000a10: 6c65 2f54 6173 6b2f 5363 656e 652f 5365  le/Task/Scene/Se
+00000a20: 7276 6963 6520 786d 6c20 656c 656d 656e  rvice xml elemen
+00000a30: 7473 0a20 2020 2029 0e7a 0c55 4920 3e20  ts.    ).z.UI > 
+00000a40: 4765 6e65 7261 6c7a 1055 4920 3e20 4d61  Generalz.UI > Ma
+00000a50: 696e 2053 6372 6565 6e7a 0c55 4920 3e20  in Screenz.UI > 
+00000a60: 5549 204c 6f63 6b7a 1155 4920 3e20 4c6f  UI Lockz.UI > Lo
+00000a70: 6361 6c69 7a61 7469 6f6e 7a11 4d6f 6e69  calizationz.Moni
+00000a80: 746f 7220 3e20 4765 6e65 7261 6c7a 1f4d  tor > Generalz.M
+00000a90: 6f6e 6974 6f72 203e 2044 6973 706c 6179  onitor > Display
+00000aa0: 204f 6e20 4d6f 6e69 746f 7269 6e67 7a20   On Monitoringz 
+00000ab0: 4d6f 6e69 746f 7220 3e20 4469 7370 6c61  Monitor > Displa
+00000ac0: 7920 4f66 6620 4d6f 6e69 746f 7269 6e67  y Off Monitoring
+00000ad0: 7a1c 4d6f 6e69 746f 7220 3e20 4765 6e65  z.Monitor > Gene
+00000ae0: 7261 6c20 4d6f 6e69 746f 7269 6e67 7a13  ral Monitoringz.
+00000af0: 4d6f 6e69 746f 7220 3e20 4361 6c69 6272  Monitor > Calibr
+00000b00: 6174 65da 0641 6374 696f 6e7a 2241 6374  ate..Actionz"Act
+00000b10: 696f 6e20 3e20 5265 7365 7420 4572 726f  ion > Reset Erro
+00000b20: 7220 4e6f 7469 6669 6361 7469 6f6e 73da  r Notifications.
+00000b30: 044d 6973 637a 104d 6973 6320 3e20 4465  .Miscz.Misc > De
+00000b40: 6275 6767 696e 677a 1d55 6e6c 6973 7465  buggingz.Unliste
+00000b50: 6420 2850 6572 6861 7073 2044 6570 7265  d (Perhaps Depre
+00000b60: 6361 7465 6429 720b 0000 0072 0c00 0000  cated)r....r....
+00000b70: 4672 0d00 0000 5472 2200 0000 7a3b 5461  Fr....Tr"...z;Ta
 00000b80: 736b 6572 2050 7265 6665 7265 6e63 6573  sker Preferences
 00000b90: 203e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e   >>>>>>>>>>>>>>>
 00000ba0: 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e 3e3e  >>>>>>>>>>>>>>>>
-00000bb0: 3e3e 3e3e 3e3e 3e3e 3e3c 2f73 7061 6e3e  >>>>>>>>></span>
-00000bc0: 69e7 0300 00e9 6400 0000 da0c 616c 6c5f  i.....d.....all_
-00000bd0: 7365 7276 6963 6573 da01 6eda 0174 da01  services..n..t..
-00000be0: 76da 0564 6562 7567 4672 1f00 0000 7a1c  v..debugFr....z.
-00000bf0: 266e 6273 703b 266e 6273 703b 4e6f 7420  &nbsp;&nbsp;Not 
-00000c00: 7965 7420 6d61 7070 6564 3a20 7a05 7479  yet mapped: z.ty
-00000c10: 7065 3a7a 0676 616c 7565 3a72 2500 0000  pe:z.value:r%...
-00000c20: e901 0000 0072 0100 0000 2901 da03 6b65  .....r....)...ke
-00000c30: 7972 2200 0000 da07 7365 6374 696f 6e7a  yr".....sectionz
-00000c40: 0f26 6e62 7370 3b53 6563 7469 6f6e 3a20  .&nbsp;Section: 
-00000c50: 7a36 3c62 723e 266e 6273 703b 5468 6520  z6<br>&nbsp;The 
-00000c60: 7265 6d61 696e 696e 6720 7072 6566 6572  remaining prefer
-00000c70: 656e 6365 7320 6172 6520 6e6f 7420 7965  ences are not ye
-00000c80: 7420 6d61 7070 6564 7213 0000 004e 290c  t mappedr....N).
-00000c90: 7205 0000 0072 0300 0000 da04 6669 6e64  r....r......find
-00000ca0: da04 7465 7874 7204 0000 0072 3000 0000  ..textr....r0...
-00000cb0: 722b 0000 00da 0673 6f72 7465 6472 0200  r+.....sortedr..
-00000cc0: 0000 da05 6974 656d 73da 0267 635a 0763  ....items..gcZ.c
-00000cd0: 6f6c 6c65 6374 2913 7231 0000 0072 3200  ollect).r1...r2.
-00000ce0: 0000 7206 0000 0072 3300 0000 5a0d 7365  ..r....r3...Z.se
-00000cf0: 6374 696f 6e5f 6e61 6d65 7372 0900 0000  ction_namesr....
-00000d00: 722c 0000 0072 2d00 0000 5a0a 6669 7273  r,...r-...Z.firs
-00000d10: 745f 7469 6d65 5a0f 6375 7272 656e 745f  t_timeZ.current_
-00000d20: 7365 6374 696f 6e5a 0964 756d 6d79 5f6e  sectionZ.dummy_n
-00000d30: 756d 5a07 7365 7276 6963 6572 0700 0000  umZ.servicer....
-00000d40: 5a0c 7365 7276 6963 655f 7479 7065 7208  Z.service_typer.
-00000d50: 0000 005a 0d73 6f72 7465 645f 6f75 7470  ...Z.sorted_outp
-00000d60: 7574 da04 6c69 6e65 7222 0000 00da 0469  ut..liner".....i
-00000d70: 7465 6d72 1500 0000 7215 0000 0072 1b00  temr....r....r..
-00000d80: 0000 da0f 6765 745f 7072 6566 6572 656e  ....get_preferen
-00000d90: 6365 7349 0000 0073 8c00 0000 080b 0410  cesI...s........
-00000da0: 1202 02ff 0403 0401 0203 0201 0201 0201  ................
-00000db0: 0201 0802 04fa 040c 0401 0c01 0c01 0c01  ................
-00000dc0: 0c01 0802 1002 0803 0402 0401 0e01 0402  ................
-00000dd0: 0202 0602 0201 02ff 0601 04ff 0201 02ff  ................
-00000de0: 0601 04ff 0201 06ff 02fd 04ff 0809 0280  ................
+00000bb0: 3e3e 3e3e 3e3e 3e3e 3e69 e703 0000 e964  >>>>>>>>>i.....d
+00000bc0: 0000 00da 0c61 6c6c 5f73 6572 7669 6365  .....all_service
+00000bd0: 73da 016e da01 74da 0176 da05 6465 6275  s..n..t..v..debu
+00000be0: 6772 1d00 0000 7221 0000 007a 0f4e 6f74  gr....r!...z.Not
+00000bf0: 2079 6574 206d 6170 7065 643a 7a05 7479   yet mapped:z.ty
+00000c00: 7065 3a7a 0676 616c 7565 3ae9 0100 0000  pe:z.value:.....
+00000c10: 7201 0000 0029 01da 036b 6579 7220 0000  r....)...keyr ..
+00000c20: 00da 0773 6563 7469 6f6e 7a13 3c62 723e  ...sectionz.<br>
+00000c30: 266e 6273 703b 5365 6374 696f 6e3a 207a  &nbsp;Section: z
+00000c40: 363c 6272 3e26 6e62 7370 3b54 6865 2072  6<br>&nbsp;The r
+00000c50: 656d 6169 6e69 6e67 2070 7265 6665 7265  emaining prefere
+00000c60: 6e63 6573 2061 7265 206e 6f74 2079 6574  nces are not yet
+00000c70: 206d 6170 7065 644e 290c 7204 0000 0072   mappedN).r....r
+00000c80: 0300 0000 da04 6669 6e64 da04 7465 7874  ......find..text
+00000c90: 7205 0000 0072 2e00 0000 7228 0000 00da  r....r....r(....
+00000ca0: 0673 6f72 7465 6472 0200 0000 da05 6974  .sortedr......it
+00000cb0: 656d 73da 0267 635a 0763 6f6c 6c65 6374  ems..gcZ.collect
+00000cc0: 2913 722f 0000 0072 3000 0000 7206 0000  ).r/...r0...r...
+00000cd0: 0072 3100 0000 5a0d 7365 6374 696f 6e5f  .r1...Z.section_
+00000ce0: 6e61 6d65 7372 0900 0000 7229 0000 0072  namesr....r)...r
+00000cf0: 2a00 0000 da0a 6669 7273 745f 7469 6d65  *.....first_time
+00000d00: 5a0f 6375 7272 656e 745f 7365 6374 696f  Z.current_sectio
+00000d10: 6e5a 0964 756d 6d79 5f6e 756d 5a07 7365  nZ.dummy_numZ.se
+00000d20: 7276 6963 6572 0700 0000 5a0c 7365 7276  rvicer....Z.serv
+00000d30: 6963 655f 7479 7065 7208 0000 005a 0d73  ice_typer....Z.s
+00000d40: 6f72 7465 645f 6f75 7470 7574 da04 6c69  orted_output..li
+00000d50: 6e65 7220 0000 00da 0469 7465 6d72 1300  ner .....itemr..
+00000d60: 0000 7213 0000 0072 1900 0000 da0f 6765  ..r....r......ge
+00000d70: 745f 7072 6566 6572 656e 6365 734e 0000  t_preferencesN..
+00000d80: 0073 aa00 0000 080b 0410 1001 0401 0401  .s..............
+00000d90: 0203 0201 0201 0201 0201 0202 0201 0201  ................
+00000da0: 0201 0201 0201 02fb 04fa 0411 0401 0c01  ................
+00000db0: 0c01 0c01 0c01 0802 1002 0803 0402 0401  ................
+00000dc0: 0e01 0402 0202 0201 0201 0201 0201 0a02  ................
+00000dd0: 0201 02ff 0601 04ff 0201 02ff 0601 04ff  ................
+00000de0: 0201 04ff 0203 02f8 02fe 04ff 080f 0280  ................
 00000df0: 1004 0803 0802 0c02 2001 0202 0201 0201  ........ .......
-00000e00: 0201 0201 0802 0e01 06ff 04fa 0c0a 0280  ................
-00000e10: 1601 0202 0201 0201 0201 0201 0801 04fb  ................
-00000e20: 1007 0603 0801 0401 7246 0000 0029 0f72  ........rF...).r
-00000e30: 4300 0000 7228 0000 00da 086f 7065 7261  C...r(.....opera
-00000e40: 746f 7272 0200 0000 da15 6d61 7074 6173  torr......maptas
-00000e50: 6b65 722e 7372 632e 6f75 7470 7574 6c72  ker.src.outputlr
-00000e60: 0300 0000 5a16 6d61 7074 6173 6b65 722e  ....Z.maptasker.
-00000e70: 7372 632e 7365 7276 6963 6563 7204 0000  src.servicecr...
-00000e80: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
-00000e90: 2e73 7973 636f 6e73 7472 0500 0000 da04  .sysconstr......
-00000ea0: 6469 6374 da03 7374 72da 046c 6973 7472  dict..str..listr
-00000eb0: 3000 0000 7246 0000 0072 1500 0000 7215  0...rF...r....r.
-00000ec0: 0000 0072 1500 0000 721b 0000 00da 083c  ...r....r......<
-00000ed0: 6d6f 6475 6c65 3e01 0000 0073 3800 0000  module>....s8...
-00000ee0: 080d 0801 0c01 0c02 0c01 0c01 0203 0201  ................
-00000ef0: 02ff 0201 02ff 0201 02ff 0201 02ff 0202  ................
-00000f00: 0afe 0232 0201 02ff 0201 02ff 0201 02ff  ...2............
-00000f10: 0201 02ff 0202 0efe                      ........
+00000e00: 0201 0201 0201 0201 0201 0201 1401 0201  ................
+00000e10: 02fb 04fb 0c0d 0280 1601 0202 0201 0201  ................
+00000e20: 0201 0201 0801 04fb 1007 0603 0801 0401  ................
+00000e30: 7245 0000 0029 0f72 4100 0000 7225 0000  rE...).rA...r%..
+00000e40: 00da 086f 7065 7261 746f 7272 0200 0000  ...operatorr....
+00000e50: da15 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+00000e60: 6f75 7470 7574 6c72 0300 0000 da16 6d61  outputlr......ma
+00000e70: 7074 6173 6b65 722e 7372 632e 6672 6d74  ptasker.src.frmt
+00000e80: 6874 6d6c 7204 0000 005a 166d 6170 7461  htmlr....Z.mapta
+00000e90: 736b 6572 2e73 7263 2e73 6572 7669 6365  sker.src.service
+00000ea0: 6372 0500 0000 da04 6469 6374 da03 7374  cr......dict..st
+00000eb0: 72da 046c 6973 7472 2e00 0000 7245 0000  r..listr....rE..
+00000ec0: 0072 1300 0000 7213 0000 0072 1300 0000  .r....r....r....
+00000ed0: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000ee0: 0000 0073 3800 0000 080d 0801 0c01 0c02  ...s8...........
+00000ef0: 0c01 0c01 0203 0201 02ff 0201 02ff 0201  ................
+00000f00: 02ff 0201 02ff 0202 0afe 0237 0201 02ff  ...........7....
+00000f10: 0201 02ff 0201 02ff 0201 02ff 0202 0efe  ................
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/proclist.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/proclist.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  3 19:11:00 2023 UTC, .py size: 4688 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,131 +1,132 @@
-00000000: 6f0d 0d0a 0000 0000 c424 2b64 5012 0000  o........$+dP...
+00000000: 6f0d 0d0a 0000 0000 cee9 3264 6212 0000  o.........2db...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
+00000020: 0012 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6406 6509 6407 650a 6408  m.Z...d.e.d.e.d.
-00000070: 650a 6409 6501 6a0b 640a 650a 640b 650c  e.d.e.j.d.e.d.e.
-00000080: 640c 650c 640d 650c 640e 6401 6612 640f  d.e.d.e.d.d.f.d.
-00000090: 6410 8404 5a0d 6401 5300 2911 e900 0000  d...Z.d.S.).....
-000000a0: 004e 2901 da09 6d79 5f6f 7574 7075 7429  .N)...my_output)
-000000b0: 01da 1b67 6574 5f74 6173 6b5f 6163 7469  ...get_task_acti
-000000c0: 6f6e 735f 616e 645f 6f75 7470 7574 2901  ons_and_output).
-000000d0: da06 6c6f 6767 6572 2901 da11 554e 4b4e  ..logger)...UNKN
-000000e0: 4f57 4e5f 5441 534b 5f4e 414d 45da 096c  OWN_TASK_NAME..l
-000000f0: 6973 745f 7479 7065 da0b 6f75 7470 7574  ist_type..output
-00000100: 5f6c 6973 74da 0874 6865 5f6c 6973 74da  _list..the_list.
-00000110: 0874 6865 5f74 6173 6bda 0b74 6173 6b73  .the_task..tasks
-00000120: 5f66 6f75 6e64 da0c 7072 6f67 7261 6d5f  _found..program_
-00000130: 6172 6773 da08 636f 6c6f 726d 6170 da10  args..colormap..
-00000140: 616c 6c5f 7461 736b 6572 5f69 7465 6d73  all_tasker_items
-00000150: da06 7265 7475 726e 6308 0000 0000 0000  ..returnc.......
-00000160: 0000 0000 000e 0000 000b 0000 0043 0000  .............C..
-00000170: 0073 1c01 0000 6401 6402 6c00 6d01 7d08  .s....d.d.l.m.}.
-00000180: 0100 7402 7c02 8301 4400 5d81 5c02 7d09  ..t.|...D.].\.}.
-00000190: 7d0a 6403 7d0b 6403 7d0c 7c05 6404 1900  }.d.}.d.}.|.d...
-000001a0: 7226 7403 a004 6405 7405 7c0a 8301 9b00  r&t...d.t.|.....
-000001b0: 6406 7c02 9b00 6407 7c00 9b00 9d06 a101  d.|...d.|.......
-000001c0: 0100 6408 7c00 7600 7245 7c0a 7d0b 7c00  ..d.|.v.rE|.}.|.
-000001d0: 7d0c 6403 7d0a 7c05 6404 1900 7245 7c00  }.d.}.|.d...rE|.
-000001e0: a006 6409 a101 7d0d 7c0d 640a 6b03 7245  ..d...}.|.d.k.rE
-000001f0: 7c00 9b00 7405 7c0d 8301 9b00 9d02 7d00  |...t.|.......}.
-00000200: 7407 7c06 7c05 7c01 640b 7c00 9b00 640c  t.|.|.|.d.|...d.
-00000210: 7c0a 9b00 9d03 8305 0100 7c0b 7258 7c0b  |.........|.rX|.
-00000220: 7d0a 7c0c 7d00 7c03 7262 640d 7c00 7600  }.|.}.|.rbd.|.v.
-00000230: 7262 7408 7c0a 7600 7366 640d 7c00 7600  rbt.|.v.sfd.|.v.
-00000240: 7278 640e 7c0a 7601 7278 7409 7c03 7c01  rxd.|.v.rxt.|.|.
-00000250: 7c05 7c00 7c0a 7c04 7c06 7c07 640f 1900  |.|.|.|.|.|.d...
-00000260: 8308 0100 710a 7c00 6410 6b02 728b 7c05  ....q.|.d.k.r.|.
-00000270: 6411 1900 6412 6b04 728b 7c08 7c0a 7c01  d...d.k.r.|.|.|.
-00000280: 7c04 7c05 7c06 7c07 8306 0100 710a 6413  |.|.|.|.....q.d.
-00000290: 5300 2914 6129 0200 000a 2020 2020 5072  S.).a)....    Pr
-000002a0: 6f63 6573 7320 5461 736b 2f53 6365 6e65  ocess Task/Scene
-000002b0: 2074 6578 742f 6c69 6e65 2069 7465 6d3a   text/line item:
-000002c0: 2063 616c 6c20 7265 6375 7273 6976 656c   call recursivel
-000002d0: 7920 666f 7220 5461 736b 7320 7769 7468  y for Tasks with
-000002e0: 696e 2053 6365 6e65 730a 2020 2020 2020  in Scenes.      
-000002f0: 2020 3a70 6172 616d 206c 6973 745f 7479    :param list_ty
-00000300: 7065 3a20 5461 736b 206f 7220 5363 656e  pe: Task or Scen
-00000310: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
-00000320: 206f 7574 7075 745f 6c69 7374 3a20 6c69   output_list: li
-00000330: 7374 206f 6620 6f75 7470 7574 206c 696e  st of output lin
-00000340: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
-00000350: 6d20 7468 655f 6c69 7374 3a20 6c69 7374  m the_list: list
-00000360: 206f 6620 5461 736b 206e 616d 6573 2074   of Task names t
-00000370: 726f 2070 726f 6365 7373 0a20 2020 2020  ro process.     
-00000380: 2020 203a 7061 7261 6d20 7468 655f 7461     :param the_ta
-00000390: 736b 3a20 5461 736b 2f53 6365 6e65 2078  sk: Task/Scene x
-000003a0: 6d6c 2065 6c65 6d65 6e74 0a20 2020 2020  ml element.     
-000003b0: 2020 203a 7061 7261 6d20 7461 736b 735f     :param tasks_
-000003c0: 666f 756e 643a 206c 6973 7420 6f66 2054  found: list of T
-000003d0: 6173 6b73 2066 6f75 6e64 2073 6f20 6661  asks found so fa
-000003e0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
-000003f0: 2070 726f 6772 616d 5f61 7267 733a 2064   program_args: d
-00000400: 6963 7469 6f6e 6172 7920 6f66 2072 756e  ictionary of run
-00000410: 7469 6d65 2061 7267 756d 656e 7473 0a20  time arguments. 
-00000420: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
-00000430: 6c6f 726d 6170 3a20 6469 6374 696f 6e61  lormap: dictiona
-00000440: 7279 206f 6620 636f 6c6f 7273 2074 6f20  ry of colors to 
-00000450: 7573 650a 2020 2020 2020 2020 3a70 6172  use.        :par
-00000460: 616d 2061 6c6c 5f74 6173 6b65 725f 6974  am all_tasker_it
-00000470: 656d 733a 2064 6963 7469 6f6e 6172 7920  ems: dictionary 
-00000480: 6f66 2061 6c6c 2054 6173 6b65 7220 5072  of all Tasker Pr
-00000490: 6f6a 6563 7473 2f50 726f 6669 6c65 732f  ojects/Profiles/
-000004a0: 5461 736b 732f 5363 656e 6573 0a20 2020  Tasks/Scenes.   
-000004b0: 2020 2020 203a 7265 7475 726e 3a0a 2020       :return:.  
-000004c0: 2020 7201 0000 0029 01da 0d70 726f 6365    r....)...proce
-000004d0: 7373 5f73 6365 6e65 da00 da05 6465 6275  ss_scene....debu
-000004e0: 677a 1770 726f 6365 7373 5f6c 6973 7420  gz.process_list 
-000004f0: 2074 6865 5f69 7465 6d3a 7a0a 2074 6865   the_item:z. the
-00000500: 5f6c 6973 743a 7a0b 206c 6973 745f 7479  _list:z. list_ty
-00000510: 7065 3a7a 0f26 2334 353b 2623 3435 3b54  pe:z.&#45;&#45;T
-00000520: 6173 6b3a 7a03 4944 3ae9 ffff ffff e902  ask:z.ID:.......
-00000530: 0000 007a 0626 6e62 7370 3b7a 0554 6173  ...z.&nbsp;z.Tas
-00000540: 6b3a 7a0e 3c65 6d3e 4e6f 2050 726f 6669  k:z.<em>No Profi
-00000550: 6c65 da09 616c 6c5f 7461 736b 737a 0653  le..all_tasksz.S
-00000560: 6365 6e65 3ada 1464 6973 706c 6179 5f64  cene:..display_d
-00000570: 6574 6169 6c5f 6c65 7665 6ce9 0100 0000  etail_level.....
-00000580: 4e29 0ada 146d 6170 7461 736b 6572 2e73  N)...maptasker.s
-00000590: 7263 2e73 6365 6e65 7372 0f00 0000 da09  rc.scenesr......
-000005a0: 656e 756d 6572 6174 6572 0400 0000 7211  enumerater....r.
-000005b0: 0000 00da 0373 7472 da04 6669 6e64 7202  .....str..findr.
-000005c0: 0000 0072 0500 0000 7203 0000 0029 0e72  ...r....r....).r
-000005d0: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
-000005e0: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-000005f0: 0000 720d 0000 0072 0f00 0000 5a08 6d79  ..r....r....Z.my
-00000600: 5f63 6f75 6e74 da08 7468 655f 6974 656d  _count..the_item
-00000610: 5a09 7465 6d70 5f69 7465 6d5a 0974 656d  Z.temp_itemZ.tem
-00000620: 705f 6c69 7374 5a06 6964 5f6c 6f63 a900  p_listZ.id_loc..
-00000630: 721c 0000 00fa 772f 5573 6572 732f 6d69  r.....w/Users/mi
-00000640: 6b72 7562 696e 2f4c 6962 7261 7279 2f43  krubin/Library/C
-00000650: 6c6f 7564 5374 6f72 6167 652f 476f 6f67  loudStorage/Goog
-00000660: 6c65 4472 6976 652d 6d69 6b72 7562 696e  leDrive-mikrubin
-00000670: 4067 6d61 696c 2e63 6f6d 2f4d 7920 4472  @gmail.com/My Dr
-00000680: 6976 652f 5079 7468 6f6e 2f6d 6170 7461  ive/Python/mapta
-00000690: 736b 6572 2f6d 6170 7461 736b 6572 2f73  sker/maptasker/s
-000006a0: 7263 2f70 726f 636c 6973 742e 7079 da0c  rc/proclist.py..
-000006b0: 7072 6f63 6573 735f 6c69 7374 1a00 0000  process_list....
-000006c0: 736c 0000 000c 1810 0304 0104 0108 0104  sl..............
-000006d0: 0102 0106 0104 ff02 0104 ff02 0104 ff04  ................
-000006e0: ff08 0604 0104 0104 0108 010a 0108 0110  ................
-000006f0: 0102 0414 0104 ff04 0304 0104 0102 0602  ................
-00000700: ff10 0108 0108 0102 0102 0102 0102 0102  ................
-00000710: 0102 0102 0102 0106 0106 f814 0a02 0202  ................
-00000720: 0102 0102 0102 0102 0102 0104 fa02 8004  ................
-00000730: 0972 1e00 0000 290e da15 786d 6c2e 6574  .r....)...xml.et
-00000740: 7265 652e 456c 656d 656e 7454 7265 65da  ree.ElementTree.
-00000750: 0378 6d6c da15 6d61 7074 6173 6b65 722e  .xml..maptasker.
-00000760: 7372 632e 6f75 7470 7574 6c72 0200 0000  src.outputlr....
-00000770: 5a16 6d61 7074 6173 6b65 722e 7372 632e  Z.maptasker.src.
-00000780: 7461 736b 6163 746e 7203 0000 00da 166d  taskactnr......m
-00000790: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
-000007a0: 636f 6e73 7472 0400 0000 7205 0000 0072  constr....r....r
-000007b0: 1900 0000 da04 6c69 7374 da05 6574 7265  ......list..etre
-000007c0: 65da 0464 6963 7472 1e00 0000 721c 0000  e..dictr....r...
-000007d0: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-000007e0: da08 3c6d 6f64 756c 653e 0100 0000 7330  ..<module>....s0
-000007f0: 0000 0008 0d0c 020c 020c 010c 0102 0602  ................
-00000800: 0102 ff02 0202 fe02 0302 fd04 0402 fc02  ................
-00000810: 0502 fb02 0602 fa02 0702 f902 0802 f802  ................
-00000820: 090e f7                                  ...
+00000070: 650a 6409 6501 6a0b 6a0c 640a 650a 640b  e.d.e.j.j.d.e.d.
+00000080: 650d 640c 650d 640d 650d 640e 6401 6612  e.d.e.d.e.d.d.f.
+00000090: 640f 6410 8404 5a0e 6401 5300 2911 e900  d.d...Z.d.S.)...
+000000a0: 0000 004e 2901 da09 6d79 5f6f 7574 7075  ...N)...my_outpu
+000000b0: 7429 01da 1b67 6574 5f74 6173 6b5f 6163  t)...get_task_ac
+000000c0: 7469 6f6e 735f 616e 645f 6f75 7470 7574  tions_and_output
+000000d0: 2901 da06 6c6f 6767 6572 2901 da11 554e  )...logger)...UN
+000000e0: 4b4e 4f57 4e5f 5441 534b 5f4e 414d 45da  KNOWN_TASK_NAME.
+000000f0: 096c 6973 745f 7479 7065 da0b 6f75 7470  .list_type..outp
+00000100: 7574 5f6c 6973 74da 0874 6865 5f6c 6973  ut_list..the_lis
+00000110: 74da 0874 6865 5f74 6173 6bda 0b74 6173  t..the_task..tas
+00000120: 6b73 5f66 6f75 6e64 da0c 7072 6f67 7261  ks_found..progra
+00000130: 6d5f 6172 6773 da08 636f 6c6f 726d 6170  m_args..colormap
+00000140: da10 616c 6c5f 7461 736b 6572 5f69 7465  ..all_tasker_ite
+00000150: 6d73 da06 7265 7475 726e 6308 0000 0000  ms..returnc.....
+00000160: 0000 0000 0000 000e 0000 000b 0000 0043  ...............C
+00000170: 0000 0073 1c01 0000 6401 6402 6c00 6d01  ...s....d.d.l.m.
+00000180: 7d08 0100 7402 7c02 8301 4400 5d81 5c02  }...t.|...D.].\.
+00000190: 7d09 7d0a 6403 7d0b 6403 7d0c 7c05 6404  }.}.d.}.d.}.|.d.
+000001a0: 1900 7226 7403 a004 6405 7405 7c0a 8301  ..r&t...d.t.|...
+000001b0: 9b00 6406 7c02 9b00 6407 7c00 9b00 9d06  ..d.|...d.|.....
+000001c0: a101 0100 6408 7c00 7600 7245 7c0a 7d0b  ....d.|.v.rE|.}.
+000001d0: 7c00 7d0c 6403 7d0a 7c05 6404 1900 7245  |.}.d.}.|.d...rE
+000001e0: 7c00 a006 6409 a101 7d0d 7c0d 640a 6b03  |...d...}.|.d.k.
+000001f0: 7245 7c00 9b00 7405 7c0d 8301 9b00 9d02  rE|...t.|.......
+00000200: 7d00 7407 7c06 7c05 7c01 640b 7c00 9b00  }.t.|.|.|.d.|...
+00000210: 640c 7c0a 9b00 9d03 8305 0100 7c0b 7258  d.|.........|.rX
+00000220: 7c0b 7d0a 7c0c 7d00 7c03 7262 640d 7c00  |.}.|.}.|.rbd.|.
+00000230: 7600 7262 7408 7c0a 7600 7366 640d 7c00  v.rbt.|.v.sfd.|.
+00000240: 7600 7278 640e 7c0a 7601 7278 7409 7c03  v.rxd.|.v.rxt.|.
+00000250: 7c01 7c05 7c00 7c0a 7c04 7c06 7c07 640f  |.|.|.|.|.|.|.d.
+00000260: 1900 8308 0100 710a 7c00 6410 6b02 728b  ......q.|.d.k.r.
+00000270: 7c05 6411 1900 6412 6b04 728b 7c08 7c0a  |.d...d.k.r.|.|.
+00000280: 7c01 7c04 7c05 7c06 7c07 8306 0100 710a  |.|.|.|.|.....q.
+00000290: 6413 5300 2914 6129 0200 000a 2020 2020  d.S.).a)....    
+000002a0: 5072 6f63 6573 7320 5461 736b 2f53 6365  Process Task/Sce
+000002b0: 6e65 2074 6578 742f 6c69 6e65 2069 7465  ne text/line ite
+000002c0: 6d3a 2063 616c 6c20 7265 6375 7273 6976  m: call recursiv
+000002d0: 656c 7920 666f 7220 5461 736b 7320 7769  ely for Tasks wi
+000002e0: 7468 696e 2053 6365 6e65 730a 2020 2020  thin Scenes.    
+000002f0: 2020 2020 3a70 6172 616d 206c 6973 745f      :param list_
+00000300: 7479 7065 3a20 5461 736b 206f 7220 5363  type: Task or Sc
+00000310: 656e 650a 2020 2020 2020 2020 3a70 6172  ene.        :par
+00000320: 616d 206f 7574 7075 745f 6c69 7374 3a20  am output_list: 
+00000330: 6c69 7374 206f 6620 6f75 7470 7574 206c  list of output l
+00000340: 696e 6573 0a20 2020 2020 2020 203a 7061  ines.        :pa
+00000350: 7261 6d20 7468 655f 6c69 7374 3a20 6c69  ram the_list: li
+00000360: 7374 206f 6620 5461 736b 206e 616d 6573  st of Task names
+00000370: 2074 726f 2070 726f 6365 7373 0a20 2020   tro process.   
+00000380: 2020 2020 203a 7061 7261 6d20 7468 655f       :param the_
+00000390: 7461 736b 3a20 5461 736b 2f53 6365 6e65  task: Task/Scene
+000003a0: 2078 6d6c 2065 6c65 6d65 6e74 0a20 2020   xml element.   
+000003b0: 2020 2020 203a 7061 7261 6d20 7461 736b       :param task
+000003c0: 735f 666f 756e 643a 206c 6973 7420 6f66  s_found: list of
+000003d0: 2054 6173 6b73 2066 6f75 6e64 2073 6f20   Tasks found so 
+000003e0: 6661 720a 2020 2020 2020 2020 3a70 6172  far.        :par
+000003f0: 616d 2070 726f 6772 616d 5f61 7267 733a  am program_args:
+00000400: 2064 6963 7469 6f6e 6172 7920 6f66 2072   dictionary of r
+00000410: 756e 7469 6d65 2061 7267 756d 656e 7473  untime arguments
+00000420: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000430: 636f 6c6f 726d 6170 3a20 6469 6374 696f  colormap: dictio
+00000440: 6e61 7279 206f 6620 636f 6c6f 7273 2074  nary of colors t
+00000450: 6f20 7573 650a 2020 2020 2020 2020 3a70  o use.        :p
+00000460: 6172 616d 2061 6c6c 5f74 6173 6b65 725f  aram all_tasker_
+00000470: 6974 656d 733a 2064 6963 7469 6f6e 6172  items: dictionar
+00000480: 7920 6f66 2061 6c6c 2054 6173 6b65 7220  y of all Tasker 
+00000490: 5072 6f6a 6563 7473 2f50 726f 6669 6c65  Projects/Profile
+000004a0: 732f 5461 736b 732f 5363 656e 6573 0a20  s/Tasks/Scenes. 
+000004b0: 2020 2020 2020 203a 7265 7475 726e 3a0a         :return:.
+000004c0: 2020 2020 7201 0000 0029 01da 0d70 726f      r....)...pro
+000004d0: 6365 7373 5f73 6365 6e65 da00 da05 6465  cess_scene....de
+000004e0: 6275 677a 1770 726f 6365 7373 5f6c 6973  bugz.process_lis
+000004f0: 7420 2074 6865 5f69 7465 6d3a 7a0a 2074  t  the_item:z. t
+00000500: 6865 5f6c 6973 743a 7a0b 206c 6973 745f  he_list:z. list_
+00000510: 7479 7065 3a7a 0f26 2334 353b 2623 3435  type:z.&#45;&#45
+00000520: 3b54 6173 6b3a 7a03 4944 3ae9 ffff ffff  ;Task:z.ID:.....
+00000530: e902 0000 007a 0626 6e62 7370 3b7a 0554  .....z.&nbsp;z.T
+00000540: 6173 6b3a 7a0e 3c65 6d3e 4e6f 2050 726f  ask:z.<em>No Pro
+00000550: 6669 6c65 da09 616c 6c5f 7461 736b 737a  file..all_tasksz
+00000560: 0653 6365 6e65 3ada 1464 6973 706c 6179  .Scene:..display
+00000570: 5f64 6574 6169 6c5f 6c65 7665 6ce9 0100  _detail_level...
+00000580: 0000 4e29 0ada 146d 6170 7461 736b 6572  ..N)...maptasker
+00000590: 2e73 7263 2e73 6365 6e65 7372 0f00 0000  .src.scenesr....
+000005a0: da09 656e 756d 6572 6174 6572 0400 0000  ..enumerater....
+000005b0: 7211 0000 00da 0373 7472 da04 6669 6e64  r......str..find
+000005c0: 7202 0000 0072 0500 0000 7203 0000 0029  r....r....r....)
+000005d0: 0e72 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
+000005e0: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+000005f0: 0c00 0000 720d 0000 0072 0f00 0000 5a08  ....r....r....Z.
+00000600: 6d79 5f63 6f75 6e74 da08 7468 655f 6974  my_count..the_it
+00000610: 656d 5a09 7465 6d70 5f69 7465 6d5a 0974  emZ.temp_itemZ.t
+00000620: 656d 705f 6c69 7374 5a06 6964 5f6c 6f63  emp_listZ.id_loc
+00000630: a900 721c 0000 00fa 772f 5573 6572 732f  ..r.....w/Users/
+00000640: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
+00000650: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
+00000660: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
+00000670: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
+00000680: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
+00000690: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
+000006a0: 2f73 7263 2f70 726f 636c 6973 742e 7079  /src/proclist.py
+000006b0: da0c 7072 6f63 6573 735f 6c69 7374 1a00  ..process_list..
+000006c0: 0000 736c 0000 000c 1810 0304 0104 0108  ..sl............
+000006d0: 0104 0102 0106 0104 ff02 0104 ff02 0104  ................
+000006e0: ff04 ff08 0604 0104 0104 0108 010a 0108  ................
+000006f0: 0110 0102 0414 0104 ff04 0304 0104 0102  ................
+00000700: 0602 ff10 0108 0108 0102 0102 0102 0102  ................
+00000710: 0102 0102 0102 0102 0106 0106 f814 0a02  ................
+00000720: 0202 0102 0102 0102 0102 0102 0104 fa02  ................
+00000730: 8004 0972 1e00 0000 290f da16 6465 6675  ...r....)...defu
+00000740: 7365 6478 6d6c 2e45 6c65 6d65 6e74 5472  sedxml.ElementTr
+00000750: 6565 da0a 6465 6675 7365 6478 6d6c da15  ee..defusedxml..
+00000760: 6d61 7074 6173 6b65 722e 7372 632e 6f75  maptasker.src.ou
+00000770: 7470 7574 6c72 0200 0000 5a16 6d61 7074  tputlr....Z.mapt
+00000780: 6173 6b65 722e 7372 632e 7461 736b 6163  asker.src.taskac
+00000790: 746e 7203 0000 00da 166d 6170 7461 736b  tnr......maptask
+000007a0: 6572 2e73 7263 2e73 7973 636f 6e73 7472  er.src.sysconstr
+000007b0: 0400 0000 7205 0000 0072 1900 0000 da04  ....r....r......
+000007c0: 6c69 7374 da0b 456c 656d 656e 7454 7265  list..ElementTre
+000007d0: 65da 0358 4d4c da04 6469 6374 721e 0000  e..XML..dictr...
+000007e0: 0072 1c00 0000 721c 0000 0072 1c00 0000  .r....r....r....
+000007f0: 721d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000800: 0000 0073 3000 0000 080d 0c02 0c02 0c01  ...s0...........
+00000810: 0c01 0206 0201 02ff 0202 02fe 0203 02fd  ................
+00000820: 0604 02fc 0205 02fb 0206 02fa 0207 02f9  ................
+00000830: 0208 02f8 0209 0ef7                      ........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/profiles.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/profiles.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 17:24:36 2023 UTC, .py size: 10484 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,287 +1,296 @@
-00000000: 6f0d 0d0a 0000 0000 545d 2c64 f428 0000  o.......T],d.(..
+00000000: 6f0d 0d0a 0000 0000 2b49 3c64 9d29 0000  o.......+I<d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0016 0000 0040 0000 0073 f200 0000 6400  .....@...s....d.
+00000020: 0016 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a04 0100 6400 6401 6c05 6d03  ..m.Z...d.d.l.m.
 00000050: 0200 0100 6d06 5a06 0100 6400 6402 6c07  ....m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6403 6c07 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6405 6c0c 6d0d 5a0d 0100 6406 6501 6a0e  d.l.m.Z...d.e.j.
-00000090: 6407 650f 6408 650f 6409 6510 640a 6510  d.e.d.e.d.e.d.e.
-000000a0: 640b 6510 640c 6511 6501 6a0e 6512 6602  d.e.d.e.e.j.e.f.
-000000b0: 1900 660e 640d 640e 8404 5a13 640f 6501  ..f.d.d...Z.d.e.
-000000c0: 6a0e 6410 6501 6a0e 6411 650f 6409 6510  j.d.e.j.d.e.d.e.
-000000d0: 6412 6510 640c 6511 660c 6413 6414 8404  d.e.d.e.f.d.d...
-000000e0: 5a14 6411 650f 640f 6501 6a0e 6415 6512  Z.d.e.d.e.j.d.e.
-000000f0: 6416 650f 6417 650f 6409 6510 6418 6512  d.e.d.e.d.e.d.e.
-00000100: 6412 6510 6419 6510 640b 6510 640c 6501  d.e.d.e.d.e.d.e.
-00000110: 6a0e 6616 641a 641b 8404 5a15 6401 5300  j.f.d.d...Z.d.S.
-00000120: 291c e900 0000 004e 2901 da09 6d79 5f6f  )......N)...my_o
-00000130: 7574 7075 7429 01da 1272 6566 7265 7368  utput)...refresh
-00000140: 5f6f 7572 5f6f 7574 7075 7429 01da 0573  _our_output)...s
-00000150: 6861 7265 2901 da0a 4e4f 5f50 524f 4649  hare)...NO_PROFI
-00000160: 4c45 da0b 7468 655f 7072 6f66 696c 65da  LE..the_profile.
-00000170: 1066 6f75 6e64 5f74 6173 6b73 5f6c 6973  .found_tasks_lis
-00000180: 74da 1074 6173 6b5f 6f75 7470 7574 5f6c  t..task_output_l
-00000190: 696e 65da 0c70 726f 6772 616d 5f61 7267  ine..program_arg
-000001a0: 73da 0961 6c6c 5f74 6173 6b73 da0b 666f  s..all_tasks..fo
-000001b0: 756e 645f 6974 656d 73da 0672 6574 7572  und_items..retur
-000001c0: 6e63 0600 0000 0000 0000 0000 0000 0c00  nc..............
-000001d0: 0000 0800 0000 4300 0000 73a2 0000 0067  ......C...s....g
-000001e0: 0064 01a2 017d 0664 025c 027d 077d 087c  .d...}.d.\.}.}.|
-000001f0: 0044 005d 427d 097c 096a 007c 0676 0072  .D.]B}.|.j.|.v.r
-00000200: 1271 0a64 037c 096a 0076 0072 4264 047d  .q.d.|.j.v.rBd.}
-00000210: 0a7c 096a 0064 056b 0272 2064 067d 0a7c  .|.j.d.k.r d.}.|
-00000220: 096a 017d 0b74 02a0 037c 0b7c 017c 027c  .j.}.t...|.|.|.|
-00000230: 0a7c 04a1 055c 027d 077d 087c 0364 0719  .|...\.}.}.|.d..
-00000240: 0072 417c 0364 0719 007c 086b 0272 4164  .rA|.d...|.k.rAd
-00000250: 087c 0564 093c 0001 007c 077c 0866 0253  .|.d.<...|.|.f.S
-00000260: 0071 0a7c 096a 0064 0a6b 0272 4c01 007c  .q.|.j.d.k.rL..|
-00000270: 077c 0866 0253 0071 0a7c 077c 0866 0253  .|.f.S.q.|.|.f.S
-00000280: 0029 0b4e 2904 5a05 6364 6174 655a 0565  .).N).Z.cdateZ.e
-00000290: 6461 7465 da05 666c 6167 73da 0269 6429  date..flags..id)
-000002a0: 02da 0072 0f00 0000 5a03 6d69 64da 0545  ...r....Z.mid..E
-000002b0: 6e74 7279 5a04 6d69 6431 5a04 4578 6974  ntryZ.mid1Z.Exit
-000002c0: da10 7369 6e67 6c65 5f74 6173 6b5f 6e61  ..single_task_na
-000002d0: 6d65 54da 1173 696e 676c 655f 7461 736b  meT..single_task
-000002e0: 5f66 6f75 6e64 da03 6e6d 6529 04da 0374  _found..nme)...t
-000002f0: 6167 da04 7465 7874 da05 7461 736b 73da  ag..text..tasks.
-00000300: 0d67 6574 5f74 6173 6b5f 6e61 6d65 290c  .get_task_name).
-00000310: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000320: 0900 0000 720a 0000 0072 0b00 0000 5a11  ....r....r....Z.
-00000330: 6b65 7973 5f77 655f 646f 6e74 5f77 616e  keys_we_dont_wan
-00000340: 745a 1074 6865 5f74 6173 6b5f 656c 656d  tZ.the_task_elem
-00000350: 656e 745a 0d74 6865 5f74 6173 6b5f 6e61  entZ.the_task_na
-00000360: 6d65 da05 6368 696c 645a 0974 6173 6b5f  me..childZ.task_
-00000370: 7479 7065 5a07 7461 736b 5f69 64a9 0072  typeZ.task_id..r
-00000380: 1900 0000 fa77 2f55 7365 7273 2f6d 696b  .....w/Users/mik
-00000390: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
-000003a0: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
-000003b0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
-000003c0: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
-000003d0: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
-000003e0: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
-000003f0: 632f 7072 6f66 696c 6573 2e70 79da 1167  c/profiles.py..g
-00000400: 6574 5f70 726f 6669 6c65 5f74 6173 6b73  et_profile_tasks
-00000410: 1e00 0000 7332 0000 0008 0808 0108 020a  ....s2..........
-00000420: 0102 010a 0104 010a 0104 0106 0104 010a  ................
-00000430: 0108 ff06 0402 ff0c 0208 0202 0108 0502  ................
-00000440: 800a fd02 0208 0102 fd08 0372 1b00 0000  ...........r....
-00000450: da07 7072 6f6a 6563 74da 0770 726f 6669  ..project..profi
-00000460: 6c65 da0b 6f75 7470 7574 5f6c 6973 74da  le..output_list.
-00000470: 0863 6f6c 6f72 6d61 7063 0500 0000 0000  .colormapc......
-00000480: 0000 0000 0000 1200 0000 0d00 0000 4300  ..............C.
-00000490: 0000 7302 0200 0064 017c 0464 0219 0017  ..s....d.|.d....
-000004a0: 007c 0364 0319 0017 0064 0417 007d 0564  .|.d.....d...}.d
-000004b0: 017c 0464 0519 0017 007c 0364 0319 0017  .|.d.....|.d....
-000004c0: 0064 0617 007d 0664 077c 0464 0819 0017  .d...}.d.|.d....
-000004d0: 0064 0917 007c 0517 007d 0764 017c 0464  .d...|...}.d.|.d
-000004e0: 0a19 0017 007c 0364 0319 0017 0064 0b17  .....|.d.....d..
-000004f0: 007d 0864 0c7d 097c 01a0 0064 0da1 017d  .}.d.}.|...d...}
-00000500: 0a7c 0a64 0075 0172 417c 0a6a 0164 0e6b  .|.d.u.rA|.j.d.k
-00000510: 0272 417c 067d 0b6e 0264 0c7d 0b7c 00a0  .rA|.}.n.d.}.|..
-00000520: 0064 0fa1 017d 0c7c 0c64 0075 0172 4e7c  .d...}.|.d.u.rN|
-00000530: 076e 0164 0c7d 0d64 0c7d 0e7c 0364 1019  .n.d.}.d.}.|.d..
-00000540: 0072 707c 01a0 0064 11a1 017d 0e7c 0e64  .rp|...d...}.|.d
-00000550: 0075 0172 7064 127c 0364 0319 009b 0064  .u.rpd.|.d.....d
-00000560: 137c 0e6a 019b 0064 147c 0364 0319 009b  .|.j...d.|.d....
-00000570: 0064 0b9d 077d 0e64 0c7d 0f7c 0364 1519  .d...}.d.}.|.d..
-00000580: 0072 9174 02a0 037c 017c 047c 03a1 037d  .r.t...|.|.|...}
-00000590: 097c 0972 917c 089b 0064 167c 099b 0064  .|.r.|...d.|...d
-000005a0: 177c 0f9b 007c 0d9b 007c 0b9b 0064 187c  .|...|...|...d.|
-000005b0: 0e9b 0064 199d 0a7d 0f7a 0a7c 01a0 0064  ...d...}.z.|...d
-000005c0: 1aa1 016a 017c 0f17 007d 0f57 006e 4304  ...j.|...}.W.nC.
-000005d0: 0074 0479 de01 007d 1001 007a 377c 0364  .t.y...}...z7|.d
-000005e0: 1519 0072 cc74 02a0 037c 017c 047c 03a1  ...r.t...|.|.|..
-000005f0: 037d 097c 0972 c374 059b 0064 197c 089b  .}.|.r.t...d.|..
-00000600: 0064 167c 099b 0064 177c 059b 007c 0d9b  .d.|...d.|...|..
-00000610: 007c 0b9b 007c 0e9b 009d 0a6e 077c 0f74  .|...|.....n.|.t
-00000620: 0517 007c 0d17 007c 0b17 007d 0f6e 087c  ...|...|...}.n.|
-00000630: 0f74 0517 007c 0d17 007c 0b17 007d 0f57  .t...|...|...}.W
-00000640: 0059 0064 007d 107e 106e 0564 007d 107e  .Y.d.}.~.n.d.}.~
-00000650: 1077 0177 007c 0364 1019 0072 f07c 01a0  .w.w.|.d...r.|..
-00000660: 0064 1ba1 016a 017d 117c 0f9b 0064 1c7c  .d...j.}.|...d.|
-00000670: 119b 009d 037d 0f74 067c 047c 037c 0264  .....}.t.|.|.|.d
-00000680: 1d64 1e7c 0f9b 009d 0283 0501 007c 0a7c  .d.|.........|.|
-00000690: 0d7c 097c 0f66 0453 0029 1f4e 7a13 3c73  .|.|.f.S.).Nz.<s
-000006a0: 7061 6e20 7374 796c 653d 2263 6f6c 6f72  pan style="color
-000006b0: 3ada 0d70 726f 6669 6c65 5f63 6f6c 6f72  :..profile_color
-000006c0: da0b 666f 6e74 5f74 6f5f 7573 657a 083e  ..font_to_usez.>
-000006d0: 3c2f 7370 616e 3eda 1664 6973 6162 6c65  </span>..disable
-000006e0: 645f 7072 6f66 696c 655f 636f 6c6f 727a  d_profile_colorz
-000006f0: 123e 5b44 4953 4142 4c45 445d 3c2f 7370  .>[DISABLED]</sp
-00000700: 616e 3e7a 0f20 2073 7479 6c65 3d22 636f  an>z.  style="co
-00000710: 6c6f 723a da13 6c61 756e 6368 6572 5f74  lor:..launcher_t
-00000720: 6173 6b5f 636f 6c6f 727a 1022 5b4c 6175  ask_colorz."[Lau
-00000730: 6e63 6865 7220 5461 736b 5dda 1770 726f  ncher Task]..pro
-00000740: 6669 6c65 5f63 6f6e 6469 7469 6f6e 5f63  file_condition_c
-00000750: 6f6c 6f72 fa01 3e72 0f00 0000 da05 6c69  olor..>r......li
-00000760: 6d69 74da 0474 7275 655a 0f50 726f 6669  mit..trueZ.Profi
-00000770: 6c65 5661 7269 6162 6c65 da05 6465 6275  leVariable..debu
-00000780: 6772 0d00 0000 7a1f 203c 7370 616e 2073  gr....z. <span s
-00000790: 7479 6c65 3d22 636f 6c6f 723a 4772 6565  tyle="color:Gree
-000007a0: 6e59 656c 6c6f 777a 083e 666c 6167 733a  nYellowz.>flags:
-000007b0: 207a 1d3c 2f73 7061 6e3e 3c73 7061 6e20   z.</span><span 
-000007c0: 7374 796c 653d 2263 6f6c 6f72 3a52 6564  style="color:Red
-000007d0: da1a 6469 7370 6c61 795f 7072 6f66 696c  ..display_profil
-000007e0: 655f 636f 6e64 6974 696f 6e73 7a02 2028  e_conditionsz. (
-000007f0: 7a09 293c 2f73 7061 6e3e 20fa 0120 7a07  z.)</span> .. z.
-00000800: 3c2f 7370 616e 3e72 1300 0000 720e 0000  </span>r....r...
-00000810: 007a 0420 4944 3ae9 0200 0000 7a09 5072  .z. ID:.....z.Pr
-00000820: 6f66 696c 653a 2029 07da 0466 696e 6472  ofile: )...findr
-00000830: 1500 0000 da09 636f 6e64 6974 696f 6e5a  ......conditionZ
-00000840: 1770 6172 7365 5f70 726f 6669 6c65 5f63  .parse_profile_c
-00000850: 6f6e 6469 7469 6f6e da09 4578 6365 7074  ondition..Except
-00000860: 696f 6e72 0500 0000 7202 0000 0029 1272  ionr....r....).r
-00000870: 1c00 0000 721d 0000 0072 1e00 0000 7209  ....r....r....r.
-00000880: 0000 0072 1f00 0000 5a12 7072 6f66 696c  ...r....Z.profil
-00000890: 655f 636f 6c6f 725f 6874 6d6c 5a15 6469  e_color_htmlZ.di
-000008a0: 7361 626c 6564 5f70 726f 6669 6c65 5f68  sabled_profile_h
-000008b0: 746d 6c5a 126c 6175 6e63 6865 725f 7461  tmlZ.launcher_ta
-000008c0: 736b 5f68 746d 6c5a 1463 6f6e 6469 7469  sk_htmlZ.conditi
-000008d0: 6f6e 5f63 6f6c 6f72 5f68 746d 6cda 1170  on_color_html..p
-000008e0: 726f 6669 6c65 5f63 6f6e 6469 7469 6f6e  rofile_condition
-000008f0: 7226 0000 00da 0864 6973 6162 6c65 645a  r&.....disabledZ
-00000900: 0c6c 6175 6e63 6865 725f 786d 6cda 086c  .launcher_xml..l
-00000910: 6175 6e63 6865 7272 0d00 0000 da0c 7072  auncherr......pr
-00000920: 6f66 696c 655f 6e61 6d65 da01 655a 0a70  ofile_name..eZ.p
-00000930: 726f 6669 6c65 5f69 6472 1900 0000 7219  rofile_idr....r.
-00000940: 0000 0072 1a00 0000 da12 6275 696c 645f  ...r......build_
-00000950: 7072 6f66 696c 655f 6c69 6e65 4400 0000  profile_lineD...
-00000960: 73c8 0000 0002 0906 0102 ff06 0202 fe02  s...............
-00000970: 0302 fd02 ff02 0706 0102 ff06 0202 fe02  ................
-00000980: 0302 fd02 ff02 0706 0102 ff02 0202 fe02  ................
-00000990: 0302 fd02 ff02 0706 0102 ff06 0202 fe02  ................
-000009a0: 0302 fd02 ff04 060a 0312 0106 0104 0204  ................
-000009b0: 0102 0104 ff10 0304 0908 010a 0108 010c  ................
-000009c0: 0204 0104 ff06 0206 fe02 ff04 0708 0104  ................
-000009d0: 0106 0104 ff04 030c 0202 0102 ff02 0102  ................
-000009e0: ff02 0104 ff02 0106 ff02 ff02 0614 010e  ................
-000009f0: 0108 0104 0106 0104 ff02 0614 fe02 0102  ................
-00000a00: ff02 0102 ff02 0102 ff02 0106 ff0e 0304  ................
-00000a10: fc10 0714 8002 f408 0e0c 010e 0102 0202  ................
-00000a20: 0102 0102 0102 0108 0104 fb0c 0772 3400  .............r4.
-00000a30: 0000 da0c 7072 6f6a 6563 745f 6e61 6d65  ....project_name
-00000a40: da0b 7072 6f66 696c 655f 6964 73da 136c  ..profile_ids..l
-00000a50: 6973 745f 6f66 5f66 6f75 6e64 5f74 6173  ist_of_found_tas
-00000a60: 6b73 da07 6865 6164 696e 67da 1061 6c6c  ks..heading..all
-00000a70: 5f74 6173 6b65 725f 6974 656d 7363 0a00  _tasker_itemsc..
-00000a80: 0000 0000 0000 0000 0000 1600 0000 1000  ................
-00000a90: 0000 4300 0000 7334 0100 0064 017d 0a7c  ..C...s4...d.}.|
-00000aa0: 0344 005d 937d 0b7c 0864 0219 007c 0b19  .D.].}.|.d...|..
-00000ab0: 007d 0c7c 0c64 0375 0072 1301 0064 0353  .}.|.d.u.r...d.S
-00000ac0: 007c 0564 0419 0072 487a 1e7c 0ca0 0064  .|.d...rHz.|...d
-00000ad0: 05a1 016a 017d 0d7c 0564 0419 007c 0d6b  ...j.}.|.d...|.k
-00000ae0: 0372 2657 0071 0464 067c 0964 073c 0074  .r&W.q.d.|.d.<.t
-00000af0: 0264 087c 007c 0264 017c 067c 077c 0583  .d.|.|.d.|.|.|..
-00000b00: 0701 0057 006e 1204 0074 0379 4701 007d  ...W.n...t.yG..}
-00000b10: 0e01 007a 0657 0059 0064 037d 0e7e 0e71  ...z.W.Y.d.}.~.q
-00000b20: 0464 037d 0e7e 0e77 0177 0067 007d 0f64  .d.}.~.w.w.g.}.d
-00000b30: 097d 1074 047c 0c7c 047c 0f7c 057c 0864  .}.t.|.|.|.|.|.d
-00000b40: 0a19 007c 0983 065c 027d 0a7d 1174 057c  ...|...\.}.}.t.|
-00000b50: 017c 0c7c 007c 057c 0783 055c 047d 127d  .|.|.|.|...\.}.}
-00000b60: 137d 147d 0d7c 0564 0b19 0072 7074 067c  .}.}.|.d...rpt.|
-00000b70: 0c7c 077c 057c 0083 0401 0074 07a0 087c  .|.|.|.....t...|
-00000b80: 007c 117c 0a7c 0f7c 027c 0d7c 047c 067c  .|.|.|.|.|.|.|.|
-00000b90: 077c 057c 087c 0964 06a1 0d7d 157c 1572  .|.|.|.d...}.|.r
-00000ba0: 8b7c 0564 0c19 0072 8b7c 0964 0d19 0073  .|.d...r.|.d...s
-00000bb0: 917c 1573 947c 0964 0719 0072 9401 007c  .|.s.|.d...r...|
-00000bc0: 0a53 007c 1573 9771 0471 047c 0a53 0029  .S.|.s.q.q.|.S.)
-00000bd0: 0e61 9c02 0000 0a20 2020 2047 6f20 7468  .a.....    Go th
-00000be0: 726f 7567 6820 5072 6f6a 6563 7427 7320  rough Project's 
-00000bf0: 5072 6f66 696c 6573 2061 6e64 206f 7574  Profiles and out
-00000c00: 7075 7420 6561 6368 0a20 2020 2020 2020  put each.       
-00000c10: 203a 7061 7261 6d20 6f75 7470 7574 5f6c   :param output_l
-00000c20: 6973 743a 206c 6973 7420 6f66 2065 6163  ist: list of eac
-00000c30: 6820 6f75 7470 7574 206c 696e 6520 6765  h output line ge
-00000c40: 6e65 7261 7465 6420 736f 2066 6172 0a20  nerated so far. 
-00000c50: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
-00000c60: 6f6a 6563 743a 2050 726f 6a65 6374 2074  oject: Project t
-00000c70: 6f20 7072 6f63 6573 730a 2020 2020 2020  o process.      
-00000c80: 2020 3a70 6172 616d 2070 726f 6a65 6374    :param project
-00000c90: 5f6e 616d 653a 2050 726f 6a65 6374 2773  _name: Project's
-00000ca0: 206e 616d 650a 2020 2020 2020 2020 3a70   name.        :p
-00000cb0: 6172 616d 2070 726f 6669 6c65 5f69 6473  aram profile_ids
-00000cc0: 3a20 6c69 7374 206f 6620 5072 6f66 696c  : list of Profil
-00000cd0: 6573 2069 6e20 5072 6f6a 6563 740a 2020  es in Project.  
-00000ce0: 2020 2020 2020 3a70 6172 616d 206c 6973        :param lis
-00000cf0: 745f 6f66 5f66 6f75 6e64 5f74 6173 6b73  t_of_found_tasks
-00000d00: 3a20 6c69 7374 206f 6620 5461 736b 7320  : list of Tasks 
-00000d10: 666f 756e 640a 2020 2020 2020 2020 3a70  found.        :p
-00000d20: 6172 616d 2070 726f 6772 616d 5f61 7267  aram program_arg
-00000d30: 733a 2072 756e 7469 6d65 2061 7267 756d  s: runtime argum
-00000d40: 656e 7473 0a20 2020 2020 2020 203a 7061  ents.        :pa
-00000d50: 7261 6d20 6865 6164 696e 673a 2074 6865  ram heading: the
-00000d60: 206f 7574 7075 7420 6865 6164 696e 670a   output heading.
-00000d70: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-00000d80: 6f6c 6f72 6d61 703a 2074 6865 2063 6f6c  olormap: the col
-00000d90: 6f72 7320 746f 2075 7365 2069 6e20 6f75  ors to use in ou
-00000da0: 7075 740a 2020 2020 2020 2020 3a70 6172  put.        :par
-00000db0: 616d 2061 6c6c 5f74 6173 6b65 725f 6974  am all_tasker_it
-00000dc0: 656d 733a 2061 6c6c 2054 6173 6b65 7220  ems: all Tasker 
-00000dd0: 5072 6f6a 6563 7473 2f50 726f 6669 6c65  Projects/Profile
-00000de0: 732f 5461 736b 732f 5363 656e 6573 0a20  s/Tasks/Scenes. 
-00000df0: 2020 2020 2020 203a 7061 7261 6d20 666f         :param fo
-00000e00: 756e 645f 6974 656d 733a 2061 6c6c 2022  und_items: all "
-00000e10: 666f 756e 6422 2069 7465 6d73 2028 7369  found" items (si
-00000e20: 6e67 6c65 2050 726f 6a65 6374 2f50 726f  ngle Project/Pro
-00000e30: 6669 6c65 2f54 6173 6b29 206e 616d 6520  file/Task) name 
-00000e40: 616e 6420 666c 6167 0a20 2020 2020 2020  and flag.       
-00000e50: 203a 7265 7475 726e 3a20 786d 6c20 656c   :return: xml el
-00000e60: 656d 656e 7420 6f66 2054 6173 6b0a 2020  ement of Task.  
-00000e70: 2020 720f 0000 00da 0c61 6c6c 5f70 726f    r......all_pro
-00000e80: 6669 6c65 734e da13 7369 6e67 6c65 5f70  filesN..single_p
-00000e90: 726f 6669 6c65 5f6e 616d 6572 1300 0000  rofile_namer....
-00000ea0: 54da 1473 696e 676c 655f 7072 6f66 696c  T..single_profil
-00000eb0: 655f 666f 756e 6446 722a 0000 0072 0a00  e_foundFr*...r..
-00000ec0: 0000 da11 6469 7370 6c61 795f 7461 736b  ....display_task
-00000ed0: 6572 6e65 7472 1100 0000 7212 0000 0029  ernetr....r....)
-00000ee0: 0972 2c00 0000 7215 0000 0072 0300 0000  .r,...r....r....
-00000ef0: 722e 0000 0072 1b00 0000 7234 0000 0072  r....r....r4...r
-00000f00: 0400 0000 7216 0000 00da 0b6f 7574 7075  ....r......outpu
-00000f10: 745f 7461 736b 2916 721e 0000 0072 1c00  t_task).r....r..
-00000f20: 0000 7235 0000 0072 3600 0000 7237 0000  ..r5...r6...r7..
-00000f30: 0072 0900 0000 7238 0000 0072 1f00 0000  .r....r8...r....
-00000f40: 7239 0000 0072 0b00 0000 da10 6f75 725f  r9...r......our_
-00000f50: 7461 736b 5f65 6c65 6d65 6e74 da04 6974  task_element..it
-00000f60: 656d 721d 0000 0072 3200 0000 7233 0000  emr....r2...r3..
-00000f70: 00da 0974 6173 6b5f 6c69 7374 7208 0000  ...task_listr...
-00000f80: 00da 0d6f 7572 5f74 6173 6b5f 6e61 6d65  ...our_task_name
-00000f90: 7226 0000 0072 3100 0000 722f 0000 005a  r&...r1...r/...Z
-00000fa0: 0d73 7065 6369 6669 635f 7461 736b 7219  .specific_taskr.
-00000fb0: 0000 0072 1900 0000 721a 0000 00da 1070  ...r....r......p
-00000fc0: 726f 6365 7373 5f70 726f 6669 6c65 73b0  rocess_profiles.
-00000fd0: 0000 0073 8c00 0000 041a 0803 0c01 0801  ...s............
-00000fe0: 0601 0802 0201 0c01 0c01 0401 0801 0201  ................
-00000ff0: 0201 0201 0201 0201 0201 0201 0201 08f9  ................
-00001000: 0e09 0c01 0880 02ff 0402 0401 0201 0201  ................
-00001010: 0201 0201 0201 0601 0201 08fa 020a 0a01  ................
-00001020: 0cff 0805 0e01 0405 0201 0201 0201 0201  ................
-00001030: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001040: 0201 04f3 0212 02ff 0602 02fe 0603 02fd  ................
-00001050: 0204 02fc 0605 02fb 0207 0404 04fd 0201  ................
-00001060: 02ff 0403 7243 0000 0029 16da 1578 6d6c  ....rC...)...xml
-00001070: 2e65 7472 6565 2e45 6c65 6d65 6e74 5472  .etree.ElementTr
-00001080: 6565 da03 786d 6c5a 176d 6170 7461 736b  ee..xmlZ.maptask
-00001090: 6572 2e73 7263 2e63 6f6e 6469 7469 6f6e  er.src.condition
-000010a0: da03 7372 6372 2d00 0000 da13 6d61 7074  ..srcr-.....mapt
-000010b0: 6173 6b65 722e 7372 632e 7461 736b 7372  asker.src.tasksr
-000010c0: 1600 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
-000010d0: 7372 632e 6f75 7470 7574 6c72 0200 0000  src.outputlr....
-000010e0: 7203 0000 00da 136d 6170 7461 736b 6572  r......maptasker
-000010f0: 2e73 7263 2e73 6861 7265 7204 0000 00da  .src.sharer.....
-00001100: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
-00001110: 7973 636f 6e73 7472 0500 0000 da05 6574  ysconstr......et
-00001120: 7265 65da 046c 6973 74da 0464 6963 74da  ree..list..dict.
-00001130: 0574 7570 6c65 da03 7374 7272 1b00 0000  .tuple..strr....
-00001140: 7234 0000 0072 4300 0000 7219 0000 0072  r4...rC...r....r
-00001150: 1900 0000 7219 0000 0072 1a00 0000 da08  ....r....r......
-00001160: 3c6d 6f64 756c 653e 0100 0000 7374 0000  <module>....st..
-00001170: 0008 0d12 0212 010c 030c 010c 020c 0102  ................
-00001180: 0604 0102 ff02 0202 fe02 0302 fd02 0402  ................
-00001190: fc02 0502 fb02 0602 fa0c 070a f902 2604  ..............&.
-000011a0: 0102 ff04 0202 fe02 0302 fd02 0402 fc02  ................
-000011b0: 0502 fb02 060a fa02 6c02 0102 ff04 0202  ........l.......
-000011c0: fe02 0302 fd02 0402 fc02 0502 fb02 0602  ................
-000011d0: fa02 0702 f902 0802 f802 0902 f702 0a02  ................
-000011e0: f604 0b0e f5                             .....
+00000080: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
+00000090: 6d0f 5a0f 0100 6400 6407 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
+000000a0: 0100 6408 6501 6a12 6a13 6409 6514 640a  ..d.e.j.j.d.e.d.
+000000b0: 6514 640b 6515 640c 6515 640d 6515 640e  e.d.e.d.e.d.e.d.
+000000c0: 6516 6501 6a12 6a13 6517 6602 1900 660e  e.e.j.j.e.f...f.
+000000d0: 640f 6410 8404 5a18 6411 6501 6a12 6a13  d.d...Z.d.e.j.j.
+000000e0: 6412 6501 6a12 6a13 6413 6514 640b 6515  d.e.j.j.d.e.d.e.
+000000f0: 6414 6515 640e 6517 660c 6415 6416 8404  d.e.d.e.f.d.d...
+00000100: 5a19 6413 6514 6411 6501 6a12 6a13 6417  Z.d.e.d.e.j.j.d.
+00000110: 6517 6418 6514 6419 6514 640b 6515 641a  e.d.e.d.e.d.e.d.
+00000120: 6517 6414 6515 641b 6515 640d 6515 640e  e.d.e.d.e.d.e.d.
+00000130: 6501 6a12 6616 641c 641d 8404 5a1a 6401  e.j.f.d.d...Z.d.
+00000140: 5300 291e e900 0000 004e 2901 da09 6d79  S.)......N)...my
+00000150: 5f6f 7574 7075 7429 01da 1272 6566 7265  _output)...refre
+00000160: 7368 5f6f 7572 5f6f 7574 7075 7429 01da  sh_our_output)..
+00000170: 0b66 6f72 6d61 745f 6874 6d6c 2901 da10  .format_html)...
+00000180: 7265 6d6f 7665 5f68 746d 6c5f 7461 6773  remove_html_tags
+00000190: 2901 da05 7368 6172 6529 01da 0a4e 4f5f  )...share)...NO_
+000001a0: 5052 4f46 494c 45da 0b74 6865 5f70 726f  PROFILE..the_pro
+000001b0: 6669 6c65 da10 666f 756e 645f 7461 736b  file..found_task
+000001c0: 735f 6c69 7374 da10 7461 736b 5f6f 7574  s_list..task_out
+000001d0: 7075 745f 6c69 6e65 da0c 7072 6f67 7261  put_line..progra
+000001e0: 6d5f 6172 6773 da09 616c 6c5f 7461 736b  m_args..all_task
+000001f0: 73da 0b66 6f75 6e64 5f69 7465 6d73 da06  s..found_items..
+00000200: 7265 7475 726e 6306 0000 0000 0000 0000  returnc.........
+00000210: 0000 000c 0000 0008 0000 0043 0000 0073  ...........C...s
+00000220: a200 0000 6700 6401 a201 7d06 6402 5c02  ....g.d...}.d.\.
+00000230: 7d07 7d08 7c00 4400 5d42 7d09 7c09 6a00  }.}.|.D.]B}.|.j.
+00000240: 7c06 7600 7212 710a 6403 7c09 6a00 7600  |.v.r.q.d.|.j.v.
+00000250: 7242 6404 7d0a 7c09 6a00 6405 6b02 7220  rBd.}.|.j.d.k.r 
+00000260: 6406 7d0a 7c09 6a01 7d0b 7402 a003 7c0b  d.}.|.j.}.t...|.
+00000270: 7c01 7c02 7c0a 7c04 a105 5c02 7d07 7d08  |.|.|.|...\.}.}.
+00000280: 7c03 6407 1900 7241 7c03 6407 1900 7c08  |.d...rA|.d...|.
+00000290: 6b02 7241 6408 7c05 6409 3c00 0100 7c07  k.rAd.|.d.<...|.
+000002a0: 7c08 6602 5300 710a 7c09 6a00 640a 6b02  |.f.S.q.|.j.d.k.
+000002b0: 724c 0100 7c07 7c08 6602 5300 710a 7c07  rL..|.|.f.S.q.|.
+000002c0: 7c08 6602 5300 290b 4e29 045a 0563 6461  |.f.S.).N).Z.cda
+000002d0: 7465 5a05 6564 6174 65da 0566 6c61 6773  teZ.edate..flags
+000002e0: da02 6964 2902 da00 7211 0000 005a 036d  ..id)...r....Z.m
+000002f0: 6964 da05 456e 7472 795a 046d 6964 31da  id..EntryZ.mid1.
+00000300: 0445 7869 74da 1073 696e 676c 655f 7461  .Exit..single_ta
+00000310: 736b 5f6e 616d 6554 da11 7369 6e67 6c65  sk_nameT..single
+00000320: 5f74 6173 6b5f 666f 756e 64da 036e 6d65  _task_found..nme
+00000330: 2904 da03 7461 67da 0474 6578 74da 0574  )...tag..text..t
+00000340: 6173 6b73 da0d 6765 745f 7461 736b 5f6e  asks..get_task_n
+00000350: 616d 6529 0c72 0800 0000 7209 0000 0072  ame).r....r....r
+00000360: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
+00000370: 0000 005a 116b 6579 735f 7765 5f64 6f6e  ...Z.keys_we_don
+00000380: 745f 7761 6e74 5a10 7468 655f 7461 736b  t_wantZ.the_task
+00000390: 5f65 6c65 6d65 6e74 5a0d 7468 655f 7461  _elementZ.the_ta
+000003a0: 736b 5f6e 616d 65da 0563 6869 6c64 da09  sk_name..child..
+000003b0: 7461 736b 5f74 7970 655a 0774 6173 6b5f  task_typeZ.task_
+000003c0: 6964 a900 721d 0000 00fa 772f 5573 6572  id..r.....w/User
+000003d0: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
+000003e0: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
+000003f0: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
+00000400: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
+00000410: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
+00000420: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
+00000430: 6572 2f73 7263 2f70 726f 6669 6c65 732e  er/src/profiles.
+00000440: 7079 da11 6765 745f 7072 6f66 696c 655f  py..get_profile_
+00000450: 7461 736b 7320 0000 0073 3200 0000 0808  tasks ...s2.....
+00000460: 0801 0802 0a01 0201 0a01 0401 0a01 0401  ................
+00000470: 0601 0401 0a01 08ff 0604 02ff 0c02 0802  ................
+00000480: 0201 0805 0280 0afd 0202 0801 02fd 0803  ................
+00000490: 721f 0000 00da 0770 726f 6a65 6374 da07  r......project..
+000004a0: 7072 6f66 696c 65da 0b6f 7574 7075 745f  profile..output_
+000004b0: 6c69 7374 da08 636f 6c6f 726d 6170 6305  list..colormapc.
+000004c0: 0000 0000 0000 0000 0000 0011 0000 0008  ................
+000004d0: 0000 0043 0000 0073 8201 0000 6401 0400  ...C...s....d...
+000004e0: 7d05 7d06 7400 7c04 6402 6401 6403 6404  }.}.t.|.d.d.d.d.
+000004f0: 8305 7d07 7400 7c04 6405 6401 6406 6404  ..}.t.|.d.d.d.d.
+00000500: 8305 7d08 7c01 a001 6407 a101 7d09 7c09  ..}.|...d...}.|.
+00000510: 6408 7501 7225 7c09 6a02 6409 6b02 7225  d.u.r%|.j.d.k.r%
+00000520: 7c07 7d0a 6e02 6401 7d0a 7c00 a001 640a  |.}.n.d.}.|...d.
+00000530: a101 7d0b 7c0b 6408 7501 7232 7c08 6e01  ..}.|.d.u.r2|.n.
+00000540: 6401 7d0c 7c03 640b 1900 7250 7c01 a001  d.}.|.d...rP|...
+00000550: 640c a101 7d05 7c05 6408 7501 724e 7400  d...}.|.d.u.rNt.
+00000560: 7c04 640d 6401 640e 7c05 6a02 9b00 9d02  |.d.d.d.|.j.....
+00000570: 6404 8305 7d05 6e02 6401 7d05 7c03 640f  d...}.n.d.}.|.d.
+00000580: 1900 726e 7403 a004 7c01 7c04 7c03 a103  ..rnt...|.|.|...
+00000590: 0400 7d0d 726e 7405 7c0d 6401 8302 7d0d  ..}.rnt.|.d...}.
+000005a0: 7400 7c04 6410 6401 6411 7c0d 9b00 6412  t.|.d.d.d.|...d.
+000005b0: 9d03 6404 8305 7d06 7a08 7c01 a001 6413  ..d...}.z.|...d.
+000005c0: a101 6a02 7d0e 5700 6e0b 0400 7406 7981  ..j.}.W.n...t.y.
+000005d0: 0100 0100 0100 7407 7d0e 5900 6e01 7700  ......t.}.Y.n.w.
+000005e0: 7400 7c04 6414 6401 6415 7c0e 9b00 6416  t.|.d.d.d.|...d.
+000005f0: 9d03 6404 8305 7d0f 7c03 640b 1900 72a8  ..d...}.|.d...r.
+00000600: 7c01 a001 6417 a101 6a02 7d10 7c0f 9b00  |...d...j.}.|...
+00000610: 6416 7400 7c04 6418 6401 6419 7c10 9b00  d.t.|.d.d.d.|...
+00000620: 9d02 6404 8305 9b00 9d03 7d0f 7c0f 9b00  ..d.......}.|...
+00000630: 6416 7c06 9b00 6416 7c0c 9b00 7c0a 9b00  d.|...d.|...|...
+00000640: 6416 7c05 9b00 9d08 7d0f 7408 7c04 7c03  d.|.....}.t.|.|.
+00000650: 7c02 641a 7c0f 8305 0100 7c0e 5300 291b  |.d.|.....|.S.).
+00000660: 6180 0100 000a 2020 2020 4765 7420 7468  a.....    Get th
+00000670: 6520 5072 6f66 696c 6527 7320 6b65 7920  e Profile's key 
+00000680: 6174 7472 6962 7574 6573 3a20 6c69 6d69  attributes: limi
+00000690: 742c 206c 6175 6e63 6865 7220 7461 736b  t, launcher task
+000006a0: 2c20 7275 6e20 636f 6e64 6974 696f 6e73  , run conditions
+000006b0: 2061 6e64 206f 7574 7075 7420 6974 0a20   and output it. 
+000006c0: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
+000006d0: 6f6a 6563 743a 2074 6865 2050 726f 6a65  oject: the Proje
+000006e0: 6374 2078 6d6c 2065 6c65 6d65 6e74 0a20  ct xml element. 
+000006f0: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
+00000700: 6f66 696c 653a 2074 6865 2050 726f 6669  ofile: the Profi
+00000710: 6c65 2078 6d6c 2065 6c65 6d65 6e74 0a20  le xml element. 
+00000720: 2020 2020 2020 203a 7061 7261 6d20 6f75         :param ou
+00000730: 7470 7574 5f6c 6973 743a 2074 6865 206c  tput_list: the l
+00000740: 6973 7420 6f66 206f 7574 7075 7420 6c69  ist of output li
+00000750: 6e65 7320 6275 696c 7420 7468 7573 2066  nes built thus f
+00000760: 6172 0a20 2020 2020 2020 203a 7061 7261  ar.        :para
+00000770: 6d20 7072 6f67 7261 6d5f 6172 6773 3a20  m program_args: 
+00000780: 7275 6e74 696d 6520 6172 6775 6d65 6e74  runtime argument
+00000790: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
+000007a0: 2063 6f6c 6f72 6d61 703a 2063 6f6c 6f72   colormap: color
+000007b0: 7320 746f 2075 7365 2069 6e20 6f75 7470  s to use in outp
+000007c0: 7574 0a20 2020 2020 2020 203a 7265 7475  ut.        :retu
+000007d0: 726e 3a20 5072 6f66 696c 6520 6e61 6d65  rn: Profile name
+000007e0: 0a20 2020 2072 1100 0000 da16 6469 7361  .    r......disa
+000007f0: 626c 6564 5f70 726f 6669 6c65 5f63 6f6c  bled_profile_col
+00000800: 6f72 7a0a 5b44 4953 4142 4c45 445d 54da  orz.[DISABLED]T.
+00000810: 136c 6175 6e63 6865 725f 7461 736b 5f63  .launcher_task_c
+00000820: 6f6c 6f72 7a0f 5b4c 6175 6e63 6865 7220  olorz.[Launcher 
+00000830: 5461 736b 5dda 056c 696d 6974 4eda 0474  Task]..limitN..t
+00000840: 7275 655a 0f50 726f 6669 6c65 5661 7269  rueZ.ProfileVari
+00000850: 6162 6c65 da05 6465 6275 6772 0f00 0000  able..debugr....
+00000860: da0b 4772 6565 6e59 656c 6c6f 777a 0820  ..GreenYellowz. 
+00000870: 666c 6167 733a 20da 1a64 6973 706c 6179  flags: ..display
+00000880: 5f70 726f 6669 6c65 5f63 6f6e 6469 7469  _profile_conditi
+00000890: 6f6e 73da 1770 726f 6669 6c65 5f63 6f6e  ons..profile_con
+000008a0: 6469 7469 6f6e 5f63 6f6c 6f72 7a02 2028  dition_colorz. (
+000008b0: fa01 2972 1600 0000 da0d 7072 6f66 696c  ..)r......profil
+000008c0: 655f 636f 6c6f 727a 0950 726f 6669 6c65  e_colorz.Profile
+000008d0: 3a20 fa01 2072 1000 0000 da06 5965 6c6c  : .. r......Yell
+000008e0: 6f77 7a03 4944 3ae9 0200 0000 2909 7204  owz.ID:.....).r.
+000008f0: 0000 00da 0466 696e 6472 1800 0000 da09  .....findr......
+00000900: 636f 6e64 6974 696f 6e5a 1770 6172 7365  conditionZ.parse
+00000910: 5f70 726f 6669 6c65 5f63 6f6e 6469 7469  _profile_conditi
+00000920: 6f6e 7205 0000 00da 0e41 7474 7269 6275  onr......Attribu
+00000930: 7465 4572 726f 7272 0700 0000 7202 0000  teErrorr....r...
+00000940: 0029 1172 2000 0000 7221 0000 0072 2200  .).r ...r!...r".
+00000950: 0000 720b 0000 0072 2300 0000 720f 0000  ..r....r#...r...
+00000960: 005a 0e63 6f6e 6469 7469 6f6e 5f74 6578  .Z.condition_tex
+00000970: 745a 1564 6973 6162 6c65 645f 7072 6f66  tZ.disabled_prof
+00000980: 696c 655f 6874 6d6c 5a12 6c61 756e 6368  ile_htmlZ.launch
+00000990: 6572 5f74 6173 6b5f 6874 6d6c 7226 0000  er_task_htmlr&..
+000009a0: 00da 0864 6973 6162 6c65 645a 0c6c 6175  ...disabledZ.lau
+000009b0: 6e63 6865 725f 786d 6c5a 086c 6175 6e63  ncher_xmlZ.launc
+000009c0: 6865 725a 1270 726f 6669 6c65 5f63 6f6e  herZ.profile_con
+000009d0: 6469 7469 6f6e 735a 1074 6865 5f70 726f  ditionsZ.the_pro
+000009e0: 6669 6c65 5f6e 616d 65da 0c70 726f 6669  file_name..profi
+000009f0: 6c65 5f6e 616d 655a 0a70 726f 6669 6c65  le_nameZ.profile
+00000a00: 5f69 6472 1d00 0000 721d 0000 0072 1e00  _idr....r....r..
+00000a10: 0000 da12 6275 696c 645f 7072 6f66 696c  ....build_profil
+00000a20: 655f 6c69 6e65 4600 0000 736a 0000 0008  e_lineF...sj....
+00000a30: 1002 030a 0104 ff02 030a 0104 ff0a 0512  ................
+00000a40: 0106 0104 020a 0310 0108 090a 0108 0102  ................
+00000a50: 0112 0106 ff04 0408 0304 0106 0108 ff0a  ................
+00000a60: 0502 0102 0102 0102 010a 0102 0104 fb02  ................
+00000a70: 0910 010c 0108 0102 ff02 0412 0104 ff08  ................
+00000a80: 050c 011e 0202 ff1e 0502 0302 0102 0102  ................
+00000a90: 0102 0102 0104 fb04 0772 3600 0000 da0c  .........r6.....
+00000aa0: 7072 6f6a 6563 745f 6e61 6d65 da0b 7072  project_name..pr
+00000ab0: 6f66 696c 655f 6964 73da 136c 6973 745f  ofile_ids..list_
+00000ac0: 6f66 5f66 6f75 6e64 5f74 6173 6b73 da07  of_found_tasks..
+00000ad0: 6865 6164 696e 67da 1061 6c6c 5f74 6173  heading..all_tas
+00000ae0: 6b65 725f 6974 656d 7363 0a00 0000 0000  ker_itemsc......
+00000af0: 0000 0000 0000 1100 0000 1000 0000 4300  ..............C.
+00000b00: 0000 7326 0100 0064 017d 0a7c 0344 005d  ..s&...d.}.|.D.]
+00000b10: 8c7d 0b7c 0864 0219 007c 0b19 007d 0c7c  .}.|.d...|...}.|
+00000b20: 0c64 0375 0072 1301 0064 0353 007c 0564  .d.u.r...d.S.|.d
+00000b30: 0419 0072 477a 267c 0ca0 0064 05a1 016a  ...rGz&|...d...j
+00000b40: 017d 0d7c 0564 0419 007c 0d6b 0372 2657  .}.|.d...|.k.r&W
+00000b50: 0071 0464 067c 0964 073c 0074 0264 087c  .q.d.|.d.<.t.d.|
+00000b60: 007c 0264 017c 067c 077c 0583 0701 0074  .|.d.|.|.|.....t
+00000b70: 037c 077c 057c 0064 0964 0183 0501 0057  .|.|.|.d.d.....W
+00000b80: 006e 0904 0074 0479 4601 0001 0001 0059  .n...t.yF......Y
+00000b90: 0071 0477 0067 007d 0e74 057c 0c7c 047c  .q.w.g.}.t.|.|.|
+00000ba0: 0e7c 057c 0864 0a19 007c 0983 065c 027d  .|.|.d...|...\.}
+00000bb0: 0a7d 0f74 067c 017c 0c7c 007c 057c 0783  .}.t.|.|.|.|.|..
+00000bc0: 057d 0d7c 0564 0b19 0072 6974 077c 0c7c  .}.|.d...rit.|.|
+00000bd0: 077c 057c 0083 0401 0074 08a0 097c 007c  .|.|.....t...|.|
+00000be0: 0f7c 0a7c 0e7c 027c 0d7c 047c 067c 077c  .|.|.|.|.|.|.|.|
+00000bf0: 057c 087c 0964 06a1 0d7d 107c 1072 847c  .|.|.d...}.|.r.|
+00000c00: 0564 0c19 0072 847c 0964 0d19 0073 8a7c  .d...r.|.d...s.|
+00000c10: 1073 8d7c 0964 0719 0072 8d01 007c 0a53  .s.|.d...r...|.S
+00000c20: 007c 1073 9071 0471 047c 0a53 0029 0e61  .|.s.q.q.|.S.).a
+00000c30: 9c02 0000 0a20 2020 2047 6f20 7468 726f  .....    Go thro
+00000c40: 7567 6820 5072 6f6a 6563 7427 7320 5072  ugh Project's Pr
+00000c50: 6f66 696c 6573 2061 6e64 206f 7574 7075  ofiles and outpu
+00000c60: 7420 6561 6368 0a20 2020 2020 2020 203a  t each.        :
+00000c70: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
+00000c80: 743a 206c 6973 7420 6f66 2065 6163 6820  t: list of each 
+00000c90: 6f75 7470 7574 206c 696e 6520 6765 6e65  output line gene
+00000ca0: 7261 7465 6420 736f 2066 6172 0a20 2020  rated so far.   
+00000cb0: 2020 2020 203a 7061 7261 6d20 7072 6f6a       :param proj
+00000cc0: 6563 743a 2050 726f 6a65 6374 2074 6f20  ect: Project to 
+00000cd0: 7072 6f63 6573 730a 2020 2020 2020 2020  process.        
+00000ce0: 3a70 6172 616d 2070 726f 6a65 6374 5f6e  :param project_n
+00000cf0: 616d 653a 2050 726f 6a65 6374 2773 206e  ame: Project's n
+00000d00: 616d 650a 2020 2020 2020 2020 3a70 6172  ame.        :par
+00000d10: 616d 2070 726f 6669 6c65 5f69 6473 3a20  am profile_ids: 
+00000d20: 6c69 7374 206f 6620 5072 6f66 696c 6573  list of Profiles
+00000d30: 2069 6e20 5072 6f6a 6563 740a 2020 2020   in Project.    
+00000d40: 2020 2020 3a70 6172 616d 206c 6973 745f      :param list_
+00000d50: 6f66 5f66 6f75 6e64 5f74 6173 6b73 3a20  of_found_tasks: 
+00000d60: 6c69 7374 206f 6620 5461 736b 7320 666f  list of Tasks fo
+00000d70: 756e 640a 2020 2020 2020 2020 3a70 6172  und.        :par
+00000d80: 616d 2070 726f 6772 616d 5f61 7267 733a  am program_args:
+00000d90: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
+00000da0: 7473 0a20 2020 2020 2020 203a 7061 7261  ts.        :para
+00000db0: 6d20 6865 6164 696e 673a 2074 6865 206f  m heading: the o
+00000dc0: 7574 7075 7420 6865 6164 696e 670a 2020  utput heading.  
+00000dd0: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
+00000de0: 6f72 6d61 703a 2074 6865 2063 6f6c 6f72  ormap: the color
+00000df0: 7320 746f 2075 7365 2069 6e20 6f75 7075  s to use in oupu
+00000e00: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+00000e10: 2061 6c6c 5f74 6173 6b65 725f 6974 656d   all_tasker_item
+00000e20: 733a 2061 6c6c 2054 6173 6b65 7220 5072  s: all Tasker Pr
+00000e30: 6f6a 6563 7473 2f50 726f 6669 6c65 732f  ojects/Profiles/
+00000e40: 5461 736b 732f 5363 656e 6573 0a20 2020  Tasks/Scenes.   
+00000e50: 2020 2020 203a 7061 7261 6d20 666f 756e       :param foun
+00000e60: 645f 6974 656d 733a 2061 6c6c 2022 666f  d_items: all "fo
+00000e70: 756e 6422 2069 7465 6d73 2028 7369 6e67  und" items (sing
+00000e80: 6c65 2050 726f 6a65 6374 2f50 726f 6669  le Project/Profi
+00000e90: 6c65 2f54 6173 6b29 206e 616d 6520 616e  le/Task) name an
+00000ea0: 6420 666c 6167 0a20 2020 2020 2020 203a  d flag.        :
+00000eb0: 7265 7475 726e 3a20 786d 6c20 656c 656d  return: xml elem
+00000ec0: 656e 7420 6f66 2054 6173 6b0a 2020 2020  ent of Task.    
+00000ed0: 7211 0000 00da 0c61 6c6c 5f70 726f 6669  r......all_profi
+00000ee0: 6c65 734e da13 7369 6e67 6c65 5f70 726f  lesN..single_pro
+00000ef0: 6669 6c65 5f6e 616d 6572 1600 0000 54da  file_namer....T.
+00000f00: 1473 696e 676c 655f 7072 6f66 696c 655f  .single_profile_
+00000f10: 666f 756e 6446 e901 0000 0072 0c00 0000  foundF.....r....
+00000f20: da11 6469 7370 6c61 795f 7461 736b 6572  ..display_tasker
+00000f30: 6e65 7472 1400 0000 7215 0000 0029 0a72  netr....r....).r
+00000f40: 3100 0000 7218 0000 0072 0300 0000 7202  1...r....r....r.
+00000f50: 0000 0072 3300 0000 721f 0000 0072 3600  ...r3...r....r6.
+00000f60: 0000 7206 0000 0072 1900 0000 da0b 6f75  ..r....r......ou
+00000f70: 7470 7574 5f74 6173 6b29 1172 2200 0000  tput_task).r"...
+00000f80: 7220 0000 0072 3700 0000 7238 0000 0072  r ...r7...r8...r
+00000f90: 3900 0000 720b 0000 0072 3a00 0000 7223  9...r....r:...r#
+00000fa0: 0000 0072 3b00 0000 720d 0000 00da 106f  ...r;...r......o
+00000fb0: 7572 5f74 6173 6b5f 656c 656d 656e 74da  ur_task_element.
+00000fc0: 0469 7465 6d72 2100 0000 7235 0000 00da  .itemr!...r5....
+00000fd0: 0974 6173 6b5f 6c69 7374 da0d 6f75 725f  .task_list..our_
+00000fe0: 7461 736b 5f6e 616d 655a 0d73 7065 6369  task_nameZ.speci
+00000ff0: 6669 635f 7461 736b 721d 0000 0072 1d00  fic_taskr....r..
+00001000: 0000 721e 0000 00da 1070 726f 6365 7373  ..r......process
+00001010: 5f70 726f 6669 6c65 73ae 0000 0073 8a00  _profiles....s..
+00001020: 0000 041a 0803 0c01 0801 0601 0802 0201  ................
+00001030: 0c01 0c01 0401 0801 0202 0201 0201 0201  ................
+00001040: 0201 0201 0201 0201 04f9 140a 0c01 0401  ................
+00001050: 02ff 0403 0201 0201 0201 0201 0201 0601  ................
+00001060: 0201 08fa 020a 0a01 04ff 0805 0e01 0405  ................
+00001070: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001080: 0201 0201 0201 0201 0201 04f3 0212 02ff  ................
+00001090: 0602 02fe 0603 02fd 0204 02fc 0605 02fb  ................
+000010a0: 0207 0404 04fd 0201 02ff 0403 7246 0000  ............rF..
+000010b0: 0029 1bda 1664 6566 7573 6564 786d 6c2e  .)...defusedxml.
+000010c0: 456c 656d 656e 7454 7265 65da 0a64 6566  ElementTree..def
+000010d0: 7573 6564 786d 6c5a 176d 6170 7461 736b  usedxmlZ.maptask
+000010e0: 6572 2e73 7263 2e63 6f6e 6469 7469 6f6e  er.src.condition
+000010f0: da03 7372 6372 3200 0000 da13 6d61 7074  ..srcr2.....mapt
+00001100: 6173 6b65 722e 7372 632e 7461 736b 7372  asker.src.tasksr
+00001110: 1900 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
+00001120: 7372 632e 6f75 7470 7574 6c72 0200 0000  src.outputlr....
+00001130: 7203 0000 00da 166d 6170 7461 736b 6572  r......maptasker
+00001140: 2e73 7263 2e66 726d 7468 746d 6c72 0400  .src.frmthtmlr..
+00001150: 0000 da15 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
+00001160: 632e 786d 6c64 6174 6172 0500 0000 da13  c.xmldatar......
+00001170: 6d61 7074 6173 6b65 722e 7372 632e 7368  maptasker.src.sh
+00001180: 6172 6572 0600 0000 da16 6d61 7074 6173  arer......maptas
+00001190: 6b65 722e 7372 632e 7379 7363 6f6e 7374  ker.src.sysconst
+000011a0: 7207 0000 00da 0b45 6c65 6d65 6e74 5472  r......ElementTr
+000011b0: 6565 da03 584d 4cda 046c 6973 74da 0464  ee..XML..list..d
+000011c0: 6963 74da 0574 7570 6c65 da03 7374 7272  ict..tuple..strr
+000011d0: 1f00 0000 7236 0000 0072 4600 0000 721d  ....r6...rF...r.
+000011e0: 0000 0072 1d00 0000 721d 0000 0072 1e00  ...r....r....r..
+000011f0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001200: 7378 0000 0008 0d12 0212 010c 030c 010c  sx..............
+00001210: 010c 010c 020c 0102 0606 0102 ff02 0202  ................
+00001220: fe02 0302 fd02 0402 fc02 0502 fb02 0602  ................
+00001230: fa0e 070a f902 2606 0102 ff06 0202 fe02  ......&.........
+00001240: 0302 fd02 0402 fc02 0502 fb02 060a fa02  ................
+00001250: 6802 0102 ff06 0202 fe02 0302 fd02 0402  h...............
+00001260: fc02 0502 fb02 0602 fa02 0702 f902 0802  ................
+00001270: f802 0902 f702 0a02 f604 0b0e f5         .............
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/progargs.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/progargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/projects.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/projects.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 17:27:48 2023 UTC, .py size: 15015 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,463 +1,451 @@
-00000000: 6f0d 0d0a 0000 0000 145e 2c64 a73a 0000  o........^,d.:..
+00000000: 6f0d 0d0a 0000 0000 7223 3c64 da3a 0000  o.......r#<d.:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0014 0000 0040 0000 0073 7601 0000 6400  .....@...sv...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c02 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6408 6c0d 6d0e 5a0e 0100 6400 6409 6c0f  d.l.m.Z...d.d.l.
-00000090: 6d10 5a10 0100 6400 6401 6c11 6d12 0200  m.Z...d.d.l.m...
-000000a0: 0100 6d13 5a13 0100 6400 640a 6c14 6d15  ..m.Z...d.d.l.m.
-000000b0: 5a15 0100 6400 640b 6c14 6d16 5a16 0100  Z...d.d.l.m.Z...
-000000c0: 640c 6517 640d 6517 640e 6517 640f 6518  d.e.d.e.d.e.d.e.
-000000d0: 6410 6518 6411 6519 6412 6518 6413 6518  d.e.d.e.d.e.d.e.
-000000e0: 6414 6517 6612 6415 6416 8404 5a1a 6417  d.e.f.d.d...Z.d.
-000000f0: 6501 6a1b 6412 6518 6418 6519 6414 6519  e.j.d.e.d.e.d.e.
-00000100: 6608 6419 641a 8404 5a1c 641b 6517 640d  f.d.d...Z.d.e.d.
-00000110: 6517 640c 6517 641c 6519 6412 6518 640f  e.d.e.d.e.d.e.d.
-00000120: 6518 6411 6519 6413 6518 6410 6518 6414  e.d.e.d.e.d.e.d.
-00000130: 6401 6614 641d 641e 8404 5a1d 640f 6518  d.f.d.d...Z.d.e.
-00000140: 6412 6518 6417 6501 6a1b 641c 6519 6410  d.e.d.e.j.d.e.d.
-00000150: 6518 6411 6519 640c 6517 641f 6519 6414  e.d.e.d.e.d.e.d.
-00000160: 651e 6612 6420 6421 8404 5a1f 6410 6518  e.f.d d!..Z.d.e.
-00000170: 640c 6517 6411 6519 640e 6517 640d 6517  d.e.d.e.d.e.d.e.
-00000180: 6422 6501 6a1b 6412 6518 640f 6518 6413  d"e.j.d.e.d.e.d.
-00000190: 6518 6414 6517 6614 6423 6424 8404 5a20  e.d.e.f.d#d$..Z 
-000001a0: 6401 5300 2925 e900 0000 004e 2901 da09  d.S.)%.....N)...
-000001b0: 6d79 5f6f 7574 7075 7429 01da 1272 6566  my_output)...ref
-000001c0: 7265 7368 5f6f 7572 5f6f 7574 7075 7429  resh_our_output)
-000001d0: 01da 1070 726f 6365 7373 5f70 726f 6669  ...process_profi
-000001e0: 6c65 7329 01da 0573 6861 7265 2901 da0b  les)...share)...
-000001f0: 6765 745f 6b69 645f 6170 7029 01da 0c67  get_kid_app)...g
-00000200: 6574 5f70 7269 6f72 6974 7929 01da 0767  et_priority)...g
-00000210: 6574 5f69 6473 2901 da16 7072 6f63 6573  et_ids)...proces
-00000220: 735f 7072 6f6a 6563 745f 7363 656e 6573  s_project_scenes
-00000230: 2901 da0a 4e4f 5f50 524f 4649 4c45 2901  )...NO_PROFILE).
-00000240: da0b 464f 4e54 5f54 4f5f 5553 45da 0b6f  ..FONT_TO_USE..o
-00000250: 7574 7075 745f 6c69 7374 da0b 666f 756e  utput_list..foun
-00000260: 645f 7461 736b 73da 1970 726f 6a65 6374  d_tasks..project
-00000270: 735f 7769 7468 6f75 745f 7072 6f66 696c  s_without_profil
-00000280: 6573 da0c 7072 6f67 7261 6d5f 6172 6773  es..program_args
-00000290: da0b 666f 756e 645f 6974 656d 73da 0768  ..found_items..h
-000002a0: 6561 6469 6e67 da08 636f 6c6f 726d 6170  eading..colormap
-000002b0: da10 616c 6c5f 7461 736b 6572 5f69 7465  ..all_tasker_ite
-000002c0: 6d73 da06 7265 7475 726e 6308 0000 0000  ms..returnc.....
-000002d0: 0000 0000 0000 0009 0000 000a 0000 0043  ...............C
-000002e0: 0000 0073 3e00 0000 6401 7d08 7400 7c04  ...s>...d.}.t.|.
-000002f0: 7c00 7c05 7c02 7c01 7c08 7c06 7c03 7c07  |.|.|.|.|.|.|.|.
-00000300: 8309 0100 7401 7c06 7c03 7c00 6402 6401  ....t.|.|.|.d.d.
-00000310: 8305 0100 7402 7403 a004 7c01 a101 a005  ....t.t...|.....
-00000320: a100 8301 5300 2903 61cc 0200 000a 2020  ....S.).a.....  
-00000330: 2020 476f 2074 6872 6f75 6768 2061 6c6c    Go through all
-00000340: 2050 726f 6a65 6374 732c 2070 726f 6365   Projects, proce
-00000350: 7373 2074 6865 6d20 616e 6420 7468 6569  ss them and thei
-00000360: 7220 5072 6f66 696c 6573 2061 6e64 2054  r Profiles and T
-00000370: 6173 6b73 2028 616e 6420 6164 6420 746f  asks (and add to
-00000380: 206f 7572 206f 7574 7075 7420 6c69 7374   our output list
-00000390: 290a 2020 2020 2020 2020 3a70 6172 616d  ).        :param
-000003a0: 206f 7574 7075 745f 6c69 7374 3a20 6c69   output_list: li
-000003b0: 7374 206f 6620 6f75 7470 7574 206c 696e  st of output lin
-000003c0: 6573 2067 656e 6572 6174 6564 2074 6875  es generated thu
-000003d0: 7320 6661 720a 2020 2020 2020 2020 3a70  s far.        :p
-000003e0: 6172 616d 2066 6f75 6e64 5f74 6173 6b73  aram found_tasks
-000003f0: 3a20 6c69 7374 206f 6620 5461 736b 7320  : list of Tasks 
-00000400: 666f 756e 6420 7468 7573 2066 6172 0a20  found thus far. 
-00000410: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
-00000420: 6f6a 6563 7473 5f77 6974 686f 7574 5f70  ojects_without_p
-00000430: 726f 6669 6c65 733a 206c 6973 7420 6f66  rofiles: list of
-00000440: 2050 726f 6a65 6374 7320 7468 6174 2064   Projects that d
-00000450: 6f6e 2774 2068 6176 6520 616e 7920 5072  on't have any Pr
-00000460: 6f66 696c 6573 0a20 2020 2020 2020 203a  ofiles.        :
-00000470: 7061 7261 6d20 7072 6f67 7261 6d5f 6172  param program_ar
-00000480: 6773 3a20 7275 6e74 696d 6520 6172 6775  gs: runtime argu
-00000490: 6d65 6e74 730a 2020 2020 2020 2020 3a70  ments.        :p
-000004a0: 6172 616d 2066 6f75 6e64 5f69 7465 6d73  aram found_items
-000004b0: 3a20 6966 2073 6561 7263 6869 6e67 2066  : if searching f
-000004c0: 6f72 2061 2073 696e 676c 6520 5072 6f6a  or a single Proj
-000004d0: 6563 742f 5072 6f66 696c 652f 5461 736b  ect/Profile/Task
-000004e0: 2c20 6e61 6d65 206f 6620 7369 6e67 6c65  , name of single
-000004f0: 2069 7465 6d0a 2020 2020 2020 2020 3a70   item.        :p
-00000500: 6172 616d 2068 6561 6469 6e67 3a20 6865  aram heading: he
-00000510: 6164 696e 6720 7072 696e 7465 640a 2020  ading printed.  
-00000520: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
-00000530: 6f72 6d61 703a 2063 6f6c 6f72 7320 746f  ormap: colors to
-00000540: 2075 7365 2069 6e20 6f75 7470 7574 0a20   use in output. 
-00000550: 2020 2020 2020 203a 7061 7261 6d20 616c         :param al
-00000560: 6c5f 7461 736b 6572 5f69 7465 6d73 3a20  l_tasker_items: 
-00000570: 616c 6c20 5072 6f6a 6563 742f 5072 6f66  all Project/Prof
-00000580: 696c 652f 5461 736b 2f53 6365 6e65 2f50  ile/Task/Scene/P
-00000590: 7265 6665 7265 6e63 6520 5461 736b 6572  reference Tasker
-000005a0: 2078 6d6c 2065 6c65 6d65 6e74 730a 2020   xml elements.  
-000005b0: 2020 2020 2020 3a72 6574 7572 6e3a 206c        :return: l
-000005c0: 6973 7420 6f66 2054 6173 6b73 2066 6f75  ist of Tasks fou
-000005d0: 6e64 2074 6875 7320 6661 722c 2077 6974  nd thus far, wit
-000005e0: 6820 6475 706c 6963 6174 6573 2072 656d  h duplicates rem
-000005f0: 6f76 6564 0a20 2020 20da 00e9 0300 0000  oved.    .......
-00000600: 2906 da10 7072 6f63 6573 735f 7072 6f6a  )...process_proj
-00000610: 6563 7473 7202 0000 00da 046c 6973 74da  ectsr......list.
-00000620: 0464 6963 74da 0866 726f 6d6b 6579 73da  .dict..fromkeys.
-00000630: 046b 6579 7329 0972 0c00 0000 720d 0000  .keys).r....r...
-00000640: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000650: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000660: 106f 7572 5f74 6173 6b5f 656c 656d 656e  .our_task_elemen
-00000670: 74a9 0072 1d00 0000 fa77 2f55 7365 7273  t..r.....w/Users
-00000680: 2f6d 696b 7275 6269 6e2f 4c69 6272 6172  /mikrubin/Librar
-00000690: 792f 436c 6f75 6453 746f 7261 6765 2f47  y/CloudStorage/G
-000006a0: 6f6f 676c 6544 7269 7665 2d6d 696b 7275  oogleDrive-mikru
-000006b0: 6269 6e40 676d 6169 6c2e 636f 6d2f 4d79  bin@gmail.com/My
-000006c0: 2044 7269 7665 2f50 7974 686f 6e2f 6d61   Drive/Python/ma
-000006d0: 7074 6173 6b65 722f 6d61 7074 6173 6b65  ptasker/maptaske
-000006e0: 722f 7372 632f 7072 6f6a 6563 7473 2e70  r/src/projects.p
-000006f0: 79da 2370 726f 6365 7373 5f70 726f 6a65  y.#process_proje
-00000700: 6374 735f 616e 645f 7468 6569 725f 7072  cts_and_their_pr
-00000710: 6f66 696c 6573 2100 0000 731c 0000 0004  ofiles!...s.....
-00000720: 1602 0202 0102 0102 0102 0102 0102 0102  ................
-00000730: 0102 0102 0104 f710 0b12 0472 1f00 0000  ...........r....
-00000740: da07 7072 6f6a 6563 74da 1270 726f 6a65  ..project..proje
-00000750: 6374 5f63 6f6c 6f72 5f68 746d 6c63 0300  ct_color_htmlc..
-00000760: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-00000770: 0000 4300 0000 7358 0000 0064 017d 037c  ..C...sX...d.}.|
-00000780: 00a0 0064 02a1 017d 047c 0464 0375 0172  ...d...}.|.d.u.r
-00000790: 2a7c 04a0 0064 04a1 017d 057c 0564 0375  *|...d...}.|.d.u
-000007a0: 0172 2a7c 056a 0164 0375 0172 2a64 057c  .r*|.j.d.u.r*d.|
-000007b0: 0164 0619 0017 0074 0217 0064 077c 056a  .d.....t...d.|.j
-000007c0: 019b 0064 089d 0317 007c 0217 007d 037c  ...d.....|...}.|
-000007d0: 0353 0029 0961 1e01 0000 0a20 2020 2049  .S.).a.....    I
-000007e0: 6620 5072 6f6a 6563 7420 6861 7320 6120  f Project has a 
-000007f0: 6c61 756e 6368 6572 2054 6173 6b2c 2067  launcher Task, g
-00000800: 6574 2069 740a 2020 2020 2020 2020 3a70  et it.        :p
-00000810: 6172 616d 2070 726f 6a65 6374 3a20 786d  aram project: xm
-00000820: 6c20 656c 656d 656e 7420 6f66 2050 726f  l element of Pro
-00000830: 6a65 6374 2077 6520 6172 6520 7072 6f63  ject we are proc
-00000840: 6573 7369 6e67 0a20 2020 2020 2020 203a  essing.        :
-00000850: 7061 7261 6d20 636f 6c6f 726d 6170 3a20  param colormap: 
-00000860: 636f 6c6f 7273 2074 6f20 7573 6520 696e  colors to use in
-00000870: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
-00000880: 3a70 6172 616d 2070 726f 6a65 6374 5f63  :param project_c
-00000890: 6f6c 6f72 5f68 746d 6c3a 2068 746d 6c20  olor_html: html 
-000008a0: 746f 2075 7365 2074 6861 7420 6465 6669  to use that defi
-000008b0: 6e65 7320 7468 6520 636f 6c6f 720a 2020  nes the color.  
-000008c0: 2020 2020 2020 3a72 6574 7572 6e3a 2069        :return: i
-000008d0: 6e66 6f72 6d61 7469 6f6e 2072 656c 6174  nformation relat
-000008e0: 6564 2074 6f20 6c61 756e 6368 6572 2054  ed to launcher T
-000008f0: 6173 6b0a 2020 2020 7215 0000 005a 0553  ask.    r....Z.S
-00000900: 6861 7265 4eda 0174 fa1a 3c2f 7370 616e  hareN..t..</span
-00000910: 3e3c 7370 616e 2073 7479 6c65 3d22 636f  ><span style="co
-00000920: 6c6f 723a da13 6c61 756e 6368 6572 5f74  lor:..launcher_t
-00000930: 6173 6b5f 636f 6c6f 727a 113e 5b4c 6175  ask_colorz.>[Lau
-00000940: 6e63 6865 7220 5461 736b 3a20 7a09 5d3c  ncher Task: z.]<
-00000950: 2f73 7061 6e3e 2029 03da 0466 696e 64da  /span> )...find.
-00000960: 0474 6578 7472 0b00 0000 2906 7220 0000  .textr....).r ..
-00000970: 0072 1200 0000 7221 0000 00da 126c 6175  .r....r!.....lau
-00000980: 6e63 6865 725f 7461 736b 5f69 6e66 6f5a  ncher_task_infoZ
-00000990: 0d73 6861 7265 5f65 6c65 6d65 6e74 5a15  .share_elementZ.
-000009a0: 6c61 756e 6368 6572 5f74 6173 6b5f 656c  launcher_task_el
-000009b0: 656d 656e 7472 1d00 0000 721d 0000 0072  ementr....r....r
-000009c0: 1e00 0000 da11 6765 745f 6c61 756e 6368  ......get_launch
-000009d0: 6572 5f74 6173 6b4b 0000 0073 2000 0000  er_taskK...s ...
-000009e0: 040a 0a01 0801 0a01 1201 0202 0601 02ff  ................
-000009f0: 0202 02fe 0c03 02fd 0204 02fc 02ff 0407  ................
-00000a00: 7228 0000 00da 0874 6173 6b5f 6964 73da  r(.....task_ids.
-00000a10: 0c70 726f 6a65 6374 5f6e 616d 6563 0900  .project_namec..
-00000a20: 0000 0000 0000 0000 0000 0f00 0000 1000  ................
-00000a30: 0000 4300 0000 73ea 0000 0064 017d 097c  ..C...s....d.}.|
-00000a40: 0044 005d 667d 0a7c 0a7c 0176 0172 6a7c  .D.]f}.|.|.v.rj|
-00000a50: 0864 0219 0073 6a7c 0864 0319 0073 6a74  .d...sj|.d...sjt
-00000a60: 00a0 017c 0a7c 0167 0064 047c 0764 0519  ...|.|.g.d.|.d..
-00000a70: 00a1 055c 027d 0b7d 0c7c 01a0 027c 0aa1  ...\.}.}.|...|..
-00000a80: 0101 007c 0972 507c 0072 507c 0864 0219  ...|.rP|.rP|.d..
-00000a90: 0073 507c 0864 0319 0073 5074 037c 047c  .sP|.d...sPt.|.|
-00000aa0: 057c 0264 0664 077c 0464 0819 009b 0064  .|.d.d.|.d.....d
-00000ab0: 097c 0564 0a19 009b 0064 0b7c 039b 0064  .|.d.....d.|...d
-00000ac0: 0c9d 0783 0501 0074 037c 047c 057c 0264  .......t.|.|.|.d
-00000ad0: 0d64 0483 0501 0064 0e7d 097c 0c9b 0064  .d.....d.}.|...d
-00000ae0: 0f7c 039b 0064 109d 0467 017d 0d74 00a0  .|...d...g.}.t..
-00000af0: 047c 027c 0c7c 0b7c 0d7c 0374 057c 017c  .|.|.|.|.|.t.|.|
-00000b00: 067c 047c 057c 077c 0864 01a1 0d7d 0e71  .|.|.|.|.d...}.q
-00000b10: 0474 037c 047c 057c 0264 0664 0483 0501  .t.|.|.|.d.d....
-00000b20: 0064 1153 0029 1261 6602 0000 0a20 2020  .d.S.).af....   
-00000b30: 2050 726f 6365 7373 2061 6c6c 2054 6173   Process all Tas
-00000b40: 6b73 2069 6e20 5072 6f6a 6563 7420 7468  ks in Project th
-00000b50: 6174 2061 7265 206e 6f74 2072 6566 6572  at are not refer
-00000b60: 656e 6365 6420 6279 2061 2050 726f 6669  enced by a Profi
-00000b70: 6c65 0a20 2020 2020 2020 203a 7061 7261  le.        :para
-00000b80: 6d20 7461 736b 5f69 6473 3a20 4c69 7374  m task_ids: List
-00000b90: 206f 6620 5461 736b 2049 4473 0a20 2020   of Task IDs.   
-00000ba0: 2020 2020 203a 7061 7261 6d20 666f 756e       :param foun
-00000bb0: 645f 7461 736b 733a 206c 6973 7420 6f66  d_tasks: list of
-00000bc0: 2054 6173 6b73 2066 6f75 6e64 2074 6875   Tasks found thu
-00000bd0: 7320 6661 720a 2020 2020 2020 2020 3a70  s far.        :p
-00000be0: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
-00000bf0: 3a20 6f75 7470 7574 206c 696e 6573 2067  : output lines g
-00000c00: 656e 6572 6174 6564 2074 6875 7320 6661  enerated thus fa
-00000c10: 7220 6f6e 746f 2077 6869 6368 2077 6520  r onto which we 
-00000c20: 7769 6c6c 2061 7070 656e 6420 6d6f 7265  will append more
-00000c30: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000c40: 7072 6f6a 6563 745f 6e61 6d65 3a20 6e61  project_name: na
-00000c50: 6d65 206f 6620 6375 7272 656e 7420 5072  me of current Pr
-00000c60: 6f6a 6563 740a 2020 2020 2020 2020 3a70  oject.        :p
-00000c70: 6172 616d 2063 6f6c 6f72 6d61 703a 2063  aram colormap: c
-00000c80: 6f6c 6f72 7320 746f 2075 7365 2069 6e20  olors to use in 
-00000c90: 6f75 7470 7574 0a20 2020 2020 2020 203a  output.        :
-00000ca0: 7061 7261 6d20 7072 6f67 7261 6d5f 6172  param program_ar
-00000cb0: 6773 3a20 7275 6e74 696d 6520 6172 6775  gs: runtime argu
-00000cc0: 6d65 6e74 730a 2020 2020 2020 2020 3a70  ments.        :p
-00000cd0: 6172 616d 2068 6561 6469 6e67 3a20 6375  aram heading: cu
-00000ce0: 7272 656e 7420 6865 6164 696e 670a 2020  rrent heading.  
-00000cf0: 2020 2020 2020 3a70 6172 616d 2061 6c6c        :param all
-00000d00: 5f74 6173 6b65 725f 6974 656d 733a 2061  _tasker_items: a
-00000d10: 6c6c 2050 726f 6a65 6374 732f 5072 6f66  ll Projects/Prof
-00000d20: 696c 6573 2f54 6173 6b73 2f53 6365 6e65  iles/Tasks/Scene
-00000d30: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-00000d40: 2066 6f75 6e64 5f69 7465 6d73 3a20 7369   found_items: si
-00000d50: 6e67 6c65 2069 7465 6d20 6e61 6d65 2066  ngle item name f
-00000d60: 6f72 2050 726f 6a65 6374 2f50 726f 6669  or Project/Profi
-00000d70: 6c65 2f54 6173 6b0a 2020 2020 2020 2020  le/Task.        
-00000d80: 3a72 6574 7572 6e3a 206e 6f6e 650a 2020  :return: none.  
-00000d90: 2020 54da 1473 696e 676c 655f 7072 6f66    T..single_prof
-00000da0: 696c 655f 666f 756e 64da 1173 696e 676c  ile_found..singl
-00000db0: 655f 7461 736b 5f66 6f75 6e64 7215 0000  e_task_foundr...
-00000dc0: 00da 0961 6c6c 5f74 6173 6b73 e904 0000  ...all_tasks....
-00000dd0: 007a 173c 6272 3e3c 7370 616e 2073 7479  .z.<br><span sty
-00000de0: 6c65 3d22 636f 6c6f 723a da0a 7461 736b  le="color:..task
-00000df0: 5f63 6f6c 6f72 7a0d 3b66 6f6e 742d 6661  _colorz.;font-fa
-00000e00: 6d69 6c79 3ada 0b66 6f6e 745f 746f 5f75  mily:..font_to_u
-00000e10: 7365 7a32 3e26 6e62 7370 3b26 6e62 7370  sez2>&nbsp;&nbsp
-00000e20: 3b26 6e62 7370 3b54 6865 2066 6f6c 6c6f  ;&nbsp;The follo
-00000e30: 7769 6e67 2054 6173 6b73 2069 6e20 5072  wing Tasks in Pr
-00000e40: 6f6a 6563 7420 7a25 2061 7265 206e 6f74  oject z% are not
-00000e50: 2069 6e20 616e 7920 5072 6f66 696c 652e   in any Profile.
-00000e60: 2e2e 3c2f 7370 616e 3e3c 6272 3ee9 0100  ..</span><br>...
-00000e70: 0000 467a 2f20 3c65 6d3e 284e 6f74 2072  ..Fz/ <em>(Not r
-00000e80: 6566 6572 656e 6365 6420 6279 2061 6e79  eferenced by any
-00000e90: 2050 726f 6669 6c65 2069 6e20 5072 6f6a   Profile in Proj
-00000ea0: 6563 7420 7a06 293c 2f65 6d3e 4e29 06da  ect z.)</em>N)..
-00000eb0: 0574 6173 6b73 5a0d 6765 745f 7461 736b  .tasksZ.get_task
-00000ec0: 5f6e 616d 65da 0672 656d 6f76 6572 0200  _name..remover..
-00000ed0: 0000 5a0b 6f75 7470 7574 5f74 6173 6b72  ..Z.output_taskr
-00000ee0: 0a00 0000 290f 7229 0000 0072 0d00 0000  ....).r)...r....
-00000ef0: 720c 0000 0072 2a00 0000 7212 0000 0072  r....r*...r....r
-00000f00: 0f00 0000 7211 0000 0072 1300 0000 7210  ....r....r....r.
-00000f10: 0000 005a 126f 7574 7075 745f 7468 655f  ...Z.output_the_
-00000f20: 6865 6164 696e 675a 0674 6865 5f69 6472  headingZ.the_idr
-00000f30: 1c00 0000 5a0d 6f75 725f 7461 736b 5f6e  ....Z.our_task_n
-00000f40: 616d 655a 0974 6173 6b5f 6c69 7374 5a04  ameZ.task_listZ.
-00000f50: 6b61 6b61 721d 0000 0072 1d00 0000 721e  kakar....r....r.
-00000f60: 0000 00da 1574 6173 6b73 5f6e 6f74 5f69  .....tasks_not_i
-00000f70: 6e5f 7072 6f66 696c 6573 6700 0000 7372  n_profilesg...sr
-00000f80: 0000 0002 1a02 ff08 0508 0206 0202 fe06  ................
-00000f90: 0302 fd04 060e 0108 ff0a 0402 0402 ff02  ................
-00000fa0: 0202 fe06 0302 fd06 0402 fc02 0602 0102  ................
-00000fb0: 0102 0102 0102 0206 0104 ff06 0204 fe02  ................
-00000fc0: 0306 fd04 fa10 0d04 0106 0402 0106 ff04  ................
-00000fd0: ff04 0602 0102 0102 0102 0102 0102 0102  ................
-00000fe0: 0102 0102 0102 0102 0102 0102 0104 f302  ................
-00000ff0: 8010 1004 0172 3400 0000 7227 0000 0063  .....r4...r'...c
-00001000: 0800 0000 0000 0000 0000 0000 0a00 0000  ................
-00001010: 0b00 0000 4300 0000 7386 0000 0064 0104  ....C...s....d..
-00001020: 007d 087d 097c 0064 0219 0064 036b 0272  .}.}.|.d...d.k.r
-00001030: 1374 007c 0283 017d 0874 017c 0264 0483  .t.|...}.t.|.d..
-00001040: 027d 097c 0064 0519 0072 2f7c 037c 0064  .}.|.d...r/|.|.d
-00001050: 0519 006b 0372 1f64 0653 0064 067c 0464  ...k.r.d.S.d.|.d
-00001060: 073c 0074 0264 047c 067c 0364 017c 057c  .<.t.d.|.|.d.|.|
-00001070: 017c 0083 0701 0064 0453 0074 037c 017c  .|.....d.S.t.|.|
-00001080: 007c 0664 0864 097c 039b 0064 0a7c 079b  .|.d.d.|...d.|..
-00001090: 007c 099b 007c 089b 009d 0683 0501 0064  .|...|.........d
-000010a0: 0453 0029 0b61 6f02 0000 0a20 2020 2041  .S.).ao....    A
-000010b0: 6464 2065 7874 7261 2069 6e66 6f20 746f  dd extra info to
-000010c0: 2050 726f 6a65 6374 206f 7574 7075 7420   Project output 
-000010d0: 6c69 6e65 2061 7320 6170 7072 6f70 7269  line as appropri
-000010e0: 6174 6520 616e 6420 7468 656e 206f 7574  ate and then out
-000010f0: 7075 7420 6974 2e0a 2020 2020 2020 2020  put it..        
-00001100: 3a70 6172 616d 2070 726f 6772 616d 5f61  :param program_a
-00001110: 7267 733a 2072 756e 7469 6d65 2061 7267  rgs: runtime arg
-00001120: 756d 656e 7473 0a20 2020 2020 2020 203a  uments.        :
-00001130: 7061 7261 6d20 636f 6c6f 726d 6170 3a20  param colormap: 
-00001140: 636f 6c6f 7273 2074 6f20 7573 6520 696e  colors to use in
-00001150: 2070 7574 7075 740a 2020 2020 2020 2020   putput.        
-00001160: 3a70 6172 616d 2070 726f 6a65 6374 3a20  :param project: 
-00001170: 5072 6f6a 6563 7420 786d 6c20 656c 656d  Project xml elem
-00001180: 656e 740a 2020 2020 2020 2020 3a70 6172  ent.        :par
-00001190: 616d 2070 726f 6a65 6374 5f6e 616d 653a  am project_name:
-000011a0: 206e 616d 6520 6f66 2050 726f 6a65 6374   name of Project
-000011b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000011c0: 666f 756e 645f 6974 656d 733a 2073 696e  found_items: sin
-000011d0: 676c 6520 6e61 6d65 2066 6f72 2050 726f  gle name for Pro
-000011e0: 6a65 6374 2f50 726f 6669 6c65 2f54 6173  ject/Profile/Tas
-000011f0: 6b20 6966 2070 726f 7669 6465 640a 2020  k if provided.  
-00001200: 2020 2020 2020 3a70 6172 616d 2068 6561        :param hea
-00001210: 6469 6e67 3a20 6c61 7374 206f 7574 7075  ding: last outpu
-00001220: 7420 6865 6164 696e 670a 2020 2020 2020  t heading.      
-00001230: 2020 3a70 6172 616d 206f 7574 7075 745f    :param output_
-00001240: 6c69 7374 3a20 6c69 7374 206f 6620 6f75  list: list of ou
-00001250: 7470 7574 206c 696e 6573 2067 656e 6572  tput lines gener
-00001260: 6174 6564 2074 6875 7320 6661 720a 2020  ated thus far.  
-00001270: 2020 2020 2020 3a70 6172 616d 206c 6175        :param lau
-00001280: 6e63 6865 725f 7461 736b 5f69 6e66 6f3a  ncher_task_info:
-00001290: 2064 6574 6169 6c73 2061 626f 7574 2028   details about (
-000012a0: 616e 7929 206c 6175 6e63 6865 7220 5461  any) launcher Ta
-000012b0: 736b 0a20 2020 2020 2020 203a 7265 7475  sk.        :retu
-000012c0: 726e 3a20 5472 7565 2069 6620 7765 2061  rn: True if we a
-000012d0: 7265 206c 6f6f 6b69 6e67 2066 6f72 2061  re looking for a
-000012e0: 2073 696e 676c 6520 5072 6f6a 6563 7420   single Project 
-000012f0: 616e 6420 7468 6973 2069 736e 2774 2069  and this isn't i
-00001300: 742e 2020 4661 6c73 6520 6f74 6865 7277  t.  False otherw
-00001310: 6973 652e 0a20 2020 2072 1500 0000 da14  ise..    r......
-00001320: 6469 7370 6c61 795f 6465 7461 696c 5f6c  display_detail_l
-00001330: 6576 656c 7216 0000 0046 da13 7369 6e67  evelr....F..sing
-00001340: 6c65 5f70 726f 6a65 6374 5f6e 616d 6554  le_project_nameT
-00001350: da14 7369 6e67 6c65 5f70 726f 6a65 6374  ..single_project
-00001360: 5f66 6f75 6e64 e902 0000 007a 0950 726f  _found.....z.Pro
-00001370: 6a65 6374 3a20 fa01 2029 0472 0600 0000  ject: .. ).r....
-00001380: 7207 0000 0072 0300 0000 7202 0000 0029  r....r....r....)
-00001390: 0a72 0f00 0000 7212 0000 0072 2000 0000  .r....r....r ...
-000013a0: 722a 0000 0072 1000 0000 7211 0000 0072  r*...r....r....r
-000013b0: 0c00 0000 7227 0000 005a 0c6b 6964 5f61  ....r'...Z.kid_a
-000013c0: 7070 5f69 6e66 6fda 0870 7269 6f72 6974  pp_info..priorit
-000013d0: 7972 1d00 0000 721d 0000 0072 1e00 0000  yr....r....r....
-000013e0: da1c 6765 745f 6578 7472 615f 616e 645f  ..get_extra_and_
-000013f0: 6f75 7470 7574 5f70 726f 6a65 6374 c800  output_project..
-00001400: 0000 7328 0000 0008 170c 0108 010a 0108  ..s(............
-00001410: 030c 0104 0108 0202 010e 0104 ff04 0b02  ................
-00001420: f902 0102 0102 0102 0116 0104 fb04 0772  ...............r
-00001430: 3b00 0000 721c 0000 0063 0900 0000 0000  ;...r....c......
-00001440: 0000 0000 0000 0f00 0000 0c00 0000 4300  ..............C.
-00001450: 0000 7388 0100 0064 017c 0664 0219 0017  ..s....d.|.d....
-00001460: 007c 0764 0319 0017 0064 0417 007d 097c  .|.d.....d...}.|
-00001470: 0864 0519 0044 005d b17d 0a7c 0064 0619  .d...D.].}.|.d..
-00001480: 0073 1a7c 0064 0719 0072 1d01 0067 0053  .s.|.d...r...g.S
-00001490: 007c 0aa0 0064 08a1 016a 017d 0b74 027c  .|...d...j.}.t.|
-000014a0: 0a7c 067c 0983 037d 0c74 037c 077c 067c  .|.|...}.t.|.|.|
-000014b0: 0a7c 0b7c 007c 027c 017c 0c83 0872 3571  .|.|.|.|.|...r5q
-000014c0: 107c 0764 0919 0072 4074 047c 0a7c 067c  .|.d...r@t.|.|.|
-000014d0: 077c 0183 0401 0074 0564 0a7c 077c 067c  .|.....t.d.|.|.|
-000014e0: 017c 0a7c 0b7c 0383 0704 007d 0d72 6374  .|.|.|.....}.rct
-000014f0: 067c 017c 0a7c 0b7c 0d7c 047c 077c 027c  .|.|.|.|.|.|.|.|
-00001500: 067c 087c 0083 0a7d 057c 0764 0b19 0072  .|.|...}.|.d...r
-00001510: 627c 0064 0719 0073 6271 106e 1074 077c  b|.d...sbq.n.t.|
-00001520: 067c 077c 0164 0c64 0d7c 0664 0e19 0017  .|.|.d.d.|.d....
-00001530: 0074 0817 0064 0f17 0083 0501 0074 077c  .t...d.......t.|
-00001540: 067c 077c 0164 1064 1183 0501 0074 0564  .|.|.d.d.....t.d
-00001550: 1269 0069 0067 007c 0a7c 0b67 0083 0704  .i.i.g.|.|.g....
-00001560: 007d 0e72 9374 097c 0e7c 047c 017c 0b7c  .}.r.t.|.|.|.|.|
-00001570: 067c 077c 027c 087c 0083 0901 007c 0764  .|.|.|.|.....|.d
-00001580: 1319 0073 a174 0a7c 0a7c 067c 077c 017c  ...s.t.|.|.|.|.|
-00001590: 057c 047c 0883 0701 0074 077c 067c 077c  .|.|.....t.|.|.|
-000015a0: 0164 1064 1183 0501 007c 0064 1419 0073  .d.d.....|.d...s
-000015b0: b57c 0064 0719 0073 b57c 0064 0619 0072  .|.d...s.|.d...r
-000015c0: c174 077c 067c 077c 0164 1064 1183 0501  .t.|.|.|.d.d....
-000015d0: 007c 0402 0001 0053 0071 1067 0053 0029  .|.....S.q.g.S.)
-000015e0: 1561 6002 0000 0a20 2020 2047 6f20 7468  .a`....    Go th
-000015f0: 726f 7567 6820 616c 6c20 7468 6520 5072  rough all the Pr
-00001600: 6f6a 6563 7473 2c20 6765 7420 7468 6569  ojects, get thei
-00001610: 7220 6465 7461 696c 2061 6e64 206f 7574  r detail and out
-00001620: 7075 7420 6974 0a20 2020 2020 2020 203a  put it.        :
-00001630: 7061 7261 6d20 666f 756e 645f 6974 656d  param found_item
-00001640: 733a 2061 6c6c 2069 7465 6d73 2066 6f75  s: all items fou
-00001650: 6e64 2073 6f20 6661 720a 2020 2020 2020  nd so far.      
-00001660: 2020 3a70 6172 616d 206f 7574 7075 745f    :param output_
-00001670: 6c69 7374 3a20 6c69 7374 206f 6620 6f75  list: list of ou
-00001680: 7470 7574 206c 696e 6573 2067 656e 6572  tput lines gener
-00001690: 6174 6564 2073 6f20 6661 720a 2020 2020  ated so far.    
-000016a0: 2020 2020 3a70 6172 616d 2068 6561 6469      :param headi
-000016b0: 6e67 3a20 7468 6520 6f75 7470 7574 2068  ng: the output h
-000016c0: 6561 6469 6e67 0a20 2020 2020 2020 203a  eading.        :
-000016d0: 7061 7261 6d20 7072 6f6a 6563 7473 5f77  param projects_w
-000016e0: 6974 686f 7574 5f70 726f 6669 6c65 733a  ithout_profiles:
-000016f0: 206c 6973 7420 6f66 2050 726f 6a65 6374   list of Project
-00001700: 7320 7769 7468 206e 6f20 5072 6f66 696c  s with no Profil
-00001710: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
-00001720: 6d20 666f 756e 645f 7461 736b 733a 206c  m found_tasks: l
-00001730: 6973 7420 6f66 2054 6173 6b73 2066 6f75  ist of Tasks fou
-00001740: 6e64 0a20 2020 2020 2020 203a 7061 7261  nd.        :para
-00001750: 6d20 6f75 725f 7461 736b 5f65 6c65 6d65  m our_task_eleme
-00001760: 6e74 3a20 786d 6c20 656c 656d 656e 7420  nt: xml element 
-00001770: 6f66 206f 7572 2054 6173 6b0a 2020 2020  of our Task.    
-00001780: 2020 2020 3a70 6172 616d 2063 6f6c 6f72      :param color
-00001790: 6d61 703a 206f 7574 7075 7420 636f 6c6f  map: output colo
-000017a0: 7273 2074 6f20 7573 650a 2020 2020 2020  rs to use.      
-000017b0: 2020 3a70 6172 616d 2070 726f 6772 616d    :param program
-000017c0: 5f61 7267 733a 2072 756e 7469 6d65 2061  _args: runtime a
-000017d0: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-000017e0: 203a 7061 7261 6d20 616c 6c5f 7461 736b   :param all_task
-000017f0: 6572 5f69 7465 6d73 3a20 616c 6c20 5072  er_items: all Pr
-00001800: 6f6a 6563 7473 2f50 726f 6669 6c65 732f  ojects/Profiles/
-00001810: 5461 736b 732f 5363 656e 6573 0a20 2020  Tasks/Scenes.   
-00001820: 2020 2020 203a 7265 7475 726e 3a20 6c69       :return: li
-00001830: 7374 206f 6620 666f 756e 6420 5461 736b  st of found Task
-00001840: 730a 2020 2020 7a13 3c73 7061 6e20 7374  s.    z.<span st
-00001850: 796c 653d 2263 6f6c 6f72 3ada 0d70 726f  yle="color:..pro
-00001860: 6a65 6374 5f63 6f6c 6f72 7230 0000 00fa  ject_colorr0....
-00001870: 013e da0c 616c 6c5f 7072 6f6a 6563 7473  .>..all_projects
-00001880: 722c 0000 0072 2b00 0000 da04 6e61 6d65  r,...r+.....name
-00001890: da11 6469 7370 6c61 795f 7461 736b 6572  ..display_tasker
-000018a0: 6e65 7454 da13 7369 6e67 6c65 5f70 726f  netT..single_pro
-000018b0: 6669 6c65 5f6e 616d 6572 3800 0000 7223  file_namer8...r#
-000018c0: 0000 00da 0d70 726f 6669 6c65 5f63 6f6c  .....profile_col
-000018d0: 6f72 7a28 3e3c 656d 3e50 726f 6a65 6374  orz(><em>Project
-000018e0: 2068 6173 206e 6f20 5072 6f66 696c 6573   has no Profiles
-000018f0: 3c2f 656d 3e3c 2f73 7061 6e3e 7216 0000  </em></span>r...
-00001900: 0072 1500 0000 46da 1073 696e 676c 655f  .r....F..single_
-00001910: 7461 736b 5f6e 616d 6572 3700 0000 290b  task_namer7...).
-00001920: 7225 0000 0072 2600 0000 7228 0000 0072  r%...r&...r(...r
-00001930: 3b00 0000 7205 0000 0072 0800 0000 7204  ;...r....r....r.
-00001940: 0000 0072 0200 0000 720b 0000 0072 3400  ...r....r....r4.
-00001950: 0000 7209 0000 0029 0f72 1000 0000 720c  ..r....).r....r.
-00001960: 0000 0072 1100 0000 720e 0000 0072 0d00  ...r....r....r..
-00001970: 0000 721c 0000 0072 1200 0000 720f 0000  ..r....r....r...
-00001980: 0072 1300 0000 7221 0000 0072 2000 0000  .r....r!...r ...
-00001990: 722a 0000 0072 2700 0000 5a0b 7072 6f66  r*...r'...Z.prof
-000019a0: 696c 655f 6964 7372 2900 0000 721d 0000  ile_idsr)...r...
-000019b0: 0072 1d00 0000 721e 0000 0072 1700 0000  .r....r....r....
-000019c0: fb00 0000 73ca 0000 0002 1a06 0102 ff06  ....s...........
-000019d0: 0202 fe02 0302 fd02 ff0c 0710 0202 0104  ................
-000019e0: 670c 9a0c 0302 0302 0102 0102 0102 0102  g...............
-000019f0: 0102 0102 0102 0104 f802 0a08 030e 0102  ................
-00001a00: 0202 0102 0102 0102 0102 0102 0102 0108  ................
-00001a10: f902 0902 0102 0102 0102 0102 0102 0102  ................
-00001a20: 0102 0102 0102 0104 f606 0f02 ff06 0202  ................
-00001a30: fe02 0402 8002 0202 0102 0102 0102 0102  ................
-00001a40: 0206 0102 ff02 0202 fe02 0302 fd04 fa10  ................
-00001a50: 0c18 0302 0202 0102 0102 0102 0102 0102  ................
-00001a60: 0102 0102 0102 0104 f708 0d02 0102 0102  ................
-00001a70: 0102 0102 0102 0102 0102 0104 f910 0a06  ................
-00001a80: 0202 ff06 0202 fe06 0302 fd10 0508 0102  ................
-00001a90: fa04 0972 1700 0000 2921 da15 786d 6c2e  ...r....)!..xml.
-00001aa0: 6574 7265 652e 456c 656d 656e 7454 7265  etree.ElementTre
-00001ab0: 65da 0378 6d6c da15 6d61 7074 6173 6b65  e..xml..maptaske
-00001ac0: 722e 7372 632e 6f75 7470 7574 6c72 0200  r.src.outputlr..
-00001ad0: 0000 7203 0000 005a 166d 6170 7461 736b  ..r....Z.maptask
-00001ae0: 6572 2e73 7263 2e70 726f 6669 6c65 7372  er.src.profilesr
-00001af0: 0400 0000 5a13 6d61 7074 6173 6b65 722e  ....Z.maptasker.
-00001b00: 7372 632e 7368 6172 6572 0500 0000 5a14  src.sharer....Z.
-00001b10: 6d61 7074 6173 6b65 722e 7372 632e 6b69  maptasker.src.ki
-00001b20: 6461 7070 7206 0000 005a 166d 6170 7461  dappr....Z.mapta
-00001b30: 736b 6572 2e73 7263 2e70 7269 6f72 6974  sker.src.priorit
-00001b40: 7972 0700 0000 5a14 6d61 7074 6173 6b65  yr....Z.maptaske
-00001b50: 722e 7372 632e 6765 7469 6473 7208 0000  r.src.getidsr...
-00001b60: 005a 146d 6170 7461 736b 6572 2e73 7263  .Z.maptasker.src
-00001b70: 2e73 6365 6e65 7372 0900 0000 5a13 6d61  .scenesr....Z.ma
-00001b80: 7074 6173 6b65 722e 7372 632e 7461 736b  ptasker.src.task
-00001b90: 73da 0373 7263 7232 0000 00da 166d 6170  s..srcr2.....map
-00001ba0: 7461 736b 6572 2e73 7263 2e73 7973 636f  tasker.src.sysco
-00001bb0: 6e73 7472 0a00 0000 720b 0000 0072 1800  nstr....r....r..
-00001bc0: 0000 7219 0000 00da 0373 7472 721f 0000  ..r......strr...
-00001bd0: 00da 0565 7472 6565 7228 0000 0072 3400  ...etreer(...r4.
-00001be0: 0000 da04 626f 6f6c 723b 0000 0072 1700  ....boolr;...r..
-00001bf0: 0000 721d 0000 0072 1d00 0000 721d 0000  ..r....r....r...
-00001c00: 0072 1e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001c10: 0100 0000 73ca 0000 0008 0e0c 020c 010c  ....s...........
-00001c20: 010c 010c 010c 010c 010c 0112 010c 010c  ................
-00001c30: 0102 0602 0102 ff02 0202 fe02 0302 fd02  ................
-00001c40: 0402 fc02 0502 fb02 0602 fa02 0702 f902  ................
-00001c50: 0802 f802 090a f702 2a04 0102 ff02 0102  ........*.......
-00001c60: ff02 0102 ff02 020a fe02 1c02 0102 ff02  ................
-00001c70: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
-00001c80: 0602 fa02 0702 f902 0802 f802 0902 f702  ................
-00001c90: 0a0a f602 6102 0102 ff02 0202 fe04 0302  ....a...........
-00001ca0: fd02 0402 fc02 0502 fb02 0602 fa02 0702  ................
-00001cb0: f902 0802 f802 090a f702 3302 0102 ff02  ..........3.....
-00001cc0: 0202 fe02 0302 fd02 0402 fc02 0502 fb04  ................
-00001cd0: 0602 fa02 0702 f902 0802 f802 0902 f702  ................
-00001ce0: 0a0e f6                                  ...
+00000020: 0014 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
+00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
+00000040: 0100 6d04 5a04 0100 6400 6402 6c05 6d06  ..m.Z...d.d.l.m.
+00000050: 5a06 0100 6400 6403 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
+00000060: 6400 6404 6c09 6d0a 5a0a 0100 6400 6405  d.d.l.m.Z...d.d.
+00000070: 6c0b 6d0c 5a0c 0100 6400 6406 6c0b 6d0d  l.m.Z...d.d.l.m.
+00000080: 5a0d 0100 6400 6407 6c0e 6d0f 5a0f 0100  Z...d.d.l.m.Z...
+00000090: 6400 6408 6c10 6d11 5a11 0100 6400 6409  d.d.l.m.Z...d.d.
+000000a0: 6c12 6d13 5a13 0100 6400 640a 6c14 6d15  l.m.Z...d.d.l.m.
+000000b0: 5a15 0100 6400 640b 6c16 6d17 5a17 0100  Z...d.d.l.m.Z...
+000000c0: 640c 6518 640d 6518 640e 6518 640f 6519  d.e.d.e.d.e.d.e.
+000000d0: 6410 6519 6411 651a 6412 6519 6413 6519  d.e.d.e.d.e.d.e.
+000000e0: 6414 6518 6612 6415 6416 8404 5a1b 6417  d.e.f.d.d...Z.d.
+000000f0: 6501 6a1c 6a1d 6412 6519 6414 651a 6606  e.j.j.d.e.d.e.f.
+00000100: 6418 6419 8404 5a1e 641a 6518 640d 6518  d.d...Z.d.e.d.e.
+00000110: 640c 6518 641b 651a 6412 6519 640f 6519  d.e.d.e.d.e.d.e.
+00000120: 6411 651a 6413 6519 6410 6519 6414 6401  d.e.d.e.d.e.d.d.
+00000130: 6614 641c 641d 8404 5a1f 640f 6519 6412  f.d.d...Z.d.e.d.
+00000140: 6519 6417 6501 6a1c 6a1d 641b 651a 6410  e.d.e.j.j.d.e.d.
+00000150: 6519 6411 651a 640c 6518 641e 651a 6414  e.d.e.d.e.d.e.d.
+00000160: 6520 6612 641f 6420 8404 5a21 6410 6519  e f.d.d ..Z!d.e.
+00000170: 640c 6518 6411 651a 640e 6518 640d 6518  d.e.d.e.d.e.d.e.
+00000180: 6421 6501 6a1c 6a1d 6412 6519 640f 6519  d!e.j.j.d.e.d.e.
+00000190: 6413 6519 6414 6518 6614 6422 6423 8404  d.e.d.e.f.d"d#..
+000001a0: 5a22 6401 5300 2924 e900 0000 004e 2901  Z"d.S.)$.....N).
+000001b0: da0b 666f 726d 6174 5f68 746d 6c29 01da  ..format_html)..
+000001c0: 0767 6574 5f69 6473 2901 da0b 6765 745f  .get_ids)...get_
+000001d0: 6b69 645f 6170 7029 01da 096d 795f 6f75  kid_app)...my_ou
+000001e0: 7470 7574 2901 da12 7265 6672 6573 685f  tput)...refresh_
+000001f0: 6f75 725f 6f75 7470 7574 2901 da0c 6765  our_output)...ge
+00000200: 745f 7072 696f 7269 7479 2901 da10 7072  t_priority)...pr
+00000210: 6f63 6573 735f 7072 6f66 696c 6573 2901  ocess_profiles).
+00000220: da16 7072 6f63 6573 735f 7072 6f6a 6563  ..process_projec
+00000230: 745f 7363 656e 6573 2901 da05 7368 6172  t_scenes)...shar
+00000240: 6529 01da 0a4e 4f5f 5052 4f46 494c 45da  e)...NO_PROFILE.
+00000250: 0b6f 7574 7075 745f 6c69 7374 da0b 666f  .output_list..fo
+00000260: 756e 645f 7461 736b 73da 1970 726f 6a65  und_tasks..proje
+00000270: 6374 735f 7769 7468 6f75 745f 7072 6f66  cts_without_prof
+00000280: 696c 6573 da0c 7072 6f67 7261 6d5f 6172  iles..program_ar
+00000290: 6773 da0b 666f 756e 645f 6974 656d 73da  gs..found_items.
+000002a0: 0768 6561 6469 6e67 da08 636f 6c6f 726d  .heading..colorm
+000002b0: 6170 da10 616c 6c5f 7461 736b 6572 5f69  ap..all_tasker_i
+000002c0: 7465 6d73 da06 7265 7475 726e 6308 0000  tems..returnc...
+000002d0: 0000 0000 0000 0000 0009 0000 000a 0000  ................
+000002e0: 0043 0000 0073 3e00 0000 6401 7d08 7400  .C...s>...d.}.t.
+000002f0: 7c04 7c00 7c05 7c02 7c01 7c08 7c06 7c03  |.|.|.|.|.|.|.|.
+00000300: 7c07 8309 0100 7401 7c06 7c03 7c00 6402  |.....t.|.|.|.d.
+00000310: 6401 8305 0100 7402 7403 a004 7c01 a101  d.....t.t...|...
+00000320: a005 a100 8301 5300 2903 61cc 0200 000a  ......S.).a.....
+00000330: 2020 2020 476f 2074 6872 6f75 6768 2061      Go through a
+00000340: 6c6c 2050 726f 6a65 6374 732c 2070 726f  ll Projects, pro
+00000350: 6365 7373 2074 6865 6d20 616e 6420 7468  cess them and th
+00000360: 6569 7220 5072 6f66 696c 6573 2061 6e64  eir Profiles and
+00000370: 2054 6173 6b73 2028 616e 6420 6164 6420   Tasks (and add 
+00000380: 746f 206f 7572 206f 7574 7075 7420 6c69  to our output li
+00000390: 7374 290a 2020 2020 2020 2020 3a70 6172  st).        :par
+000003a0: 616d 206f 7574 7075 745f 6c69 7374 3a20  am output_list: 
+000003b0: 6c69 7374 206f 6620 6f75 7470 7574 206c  list of output l
+000003c0: 696e 6573 2067 656e 6572 6174 6564 2074  ines generated t
+000003d0: 6875 7320 6661 720a 2020 2020 2020 2020  hus far.        
+000003e0: 3a70 6172 616d 2066 6f75 6e64 5f74 6173  :param found_tas
+000003f0: 6b73 3a20 6c69 7374 206f 6620 5461 736b  ks: list of Task
+00000400: 7320 666f 756e 6420 7468 7573 2066 6172  s found thus far
+00000410: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000420: 7072 6f6a 6563 7473 5f77 6974 686f 7574  projects_without
+00000430: 5f70 726f 6669 6c65 733a 206c 6973 7420  _profiles: list 
+00000440: 6f66 2050 726f 6a65 6374 7320 7468 6174  of Projects that
+00000450: 2064 6f6e 2774 2068 6176 6520 616e 7920   don't have any 
+00000460: 5072 6f66 696c 6573 0a20 2020 2020 2020  Profiles.       
+00000470: 203a 7061 7261 6d20 7072 6f67 7261 6d5f   :param program_
+00000480: 6172 6773 3a20 7275 6e74 696d 6520 6172  args: runtime ar
+00000490: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
+000004a0: 3a70 6172 616d 2066 6f75 6e64 5f69 7465  :param found_ite
+000004b0: 6d73 3a20 6966 2073 6561 7263 6869 6e67  ms: if searching
+000004c0: 2066 6f72 2061 2073 696e 676c 6520 5072   for a single Pr
+000004d0: 6f6a 6563 742f 5072 6f66 696c 652f 5461  oject/Profile/Ta
+000004e0: 736b 2c20 6e61 6d65 206f 6620 7369 6e67  sk, name of sing
+000004f0: 6c65 2069 7465 6d0a 2020 2020 2020 2020  le item.        
+00000500: 3a70 6172 616d 2068 6561 6469 6e67 3a20  :param heading: 
+00000510: 6865 6164 696e 6720 7072 696e 7465 640a  heading printed.
+00000520: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+00000530: 6f6c 6f72 6d61 703a 2063 6f6c 6f72 7320  olormap: colors 
+00000540: 746f 2075 7365 2069 6e20 6f75 7470 7574  to use in output
+00000550: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000560: 616c 6c5f 7461 736b 6572 5f69 7465 6d73  all_tasker_items
+00000570: 3a20 616c 6c20 5072 6f6a 6563 742f 5072  : all Project/Pr
+00000580: 6f66 696c 652f 5461 736b 2f53 6365 6e65  ofile/Task/Scene
+00000590: 2f50 7265 6665 7265 6e63 6520 5461 736b  /Preference Task
+000005a0: 6572 2078 6d6c 2065 6c65 6d65 6e74 730a  er xml elements.
+000005b0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000005c0: 206c 6973 7420 6f66 2054 6173 6b73 2066   list of Tasks f
+000005d0: 6f75 6e64 2074 6875 7320 6661 722c 2077  ound thus far, w
+000005e0: 6974 6820 6475 706c 6963 6174 6573 2072  ith duplicates r
+000005f0: 656d 6f76 6564 0a20 2020 20da 00e9 0300  emoved.    .....
+00000600: 0000 2906 da10 7072 6f63 6573 735f 7072  ..)...process_pr
+00000610: 6f6a 6563 7473 7205 0000 00da 046c 6973  ojectsr......lis
+00000620: 74da 0464 6963 74da 0866 726f 6d6b 6579  t..dict..fromkey
+00000630: 73da 046b 6579 7329 0972 0c00 0000 720d  s..keys).r....r.
+00000640: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
+00000650: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000660: 00da 106f 7572 5f74 6173 6b5f 656c 656d  ...our_task_elem
+00000670: 656e 74a9 0072 1d00 0000 fa77 2f55 7365  ent..r.....w/Use
+00000680: 7273 2f6d 696b 7275 6269 6e2f 4c69 6272  rs/mikrubin/Libr
+00000690: 6172 792f 436c 6f75 6453 746f 7261 6765  ary/CloudStorage
+000006a0: 2f47 6f6f 676c 6544 7269 7665 2d6d 696b  /GoogleDrive-mik
+000006b0: 7275 6269 6e40 676d 6169 6c2e 636f 6d2f  rubin@gmail.com/
+000006c0: 4d79 2044 7269 7665 2f50 7974 686f 6e2f  My Drive/Python/
+000006d0: 6d61 7074 6173 6b65 722f 6d61 7074 6173  maptasker/maptas
+000006e0: 6b65 722f 7372 632f 7072 6f6a 6563 7473  ker/src/projects
+000006f0: 2e70 79da 2370 726f 6365 7373 5f70 726f  .py.#process_pro
+00000700: 6a65 6374 735f 616e 645f 7468 6569 725f  jects_and_their_
+00000710: 7072 6f66 696c 6573 2100 0000 731c 0000  profiles!...s...
+00000720: 0004 1602 0202 0102 0102 0102 0102 0102  ................
+00000730: 0102 0102 0102 0104 f710 0b12 0472 1f00  .............r..
+00000740: 0000 da07 7072 6f6a 6563 7463 0200 0000  ....projectc....
+00000750: 0000 0000 0000 0000 0500 0000 0700 0000  ................
+00000760: 4300 0000 7350 0000 0064 017d 027c 00a0  C...sP...d.}.|..
+00000770: 0064 02a1 017d 037c 0364 0375 0172 267c  .d...}.|.d.u.r&|
+00000780: 03a0 0064 04a1 017d 047c 0464 0375 0172  ...d...}.|.d.u.r
+00000790: 267c 046a 0164 0375 0172 2674 027c 0164  &|.j.d.u.r&t.|.d
+000007a0: 0564 0164 067c 046a 019b 0064 079d 0364  .d.d.|.j...d...d
+000007b0: 0883 057d 027c 0253 0029 097a d80a 2020  ...}.|.S.).z..  
+000007c0: 2020 4966 2050 726f 6a65 6374 2068 6173    If Project has
+000007d0: 2061 206c 6175 6e63 6865 7220 5461 736b   a launcher Task
+000007e0: 2c20 6765 7420 6974 0a20 2020 2020 2020  , get it.       
+000007f0: 203a 7061 7261 6d20 7072 6f6a 6563 743a   :param project:
+00000800: 2078 6d6c 2065 6c65 6d65 6e74 206f 6620   xml element of 
+00000810: 5072 6f6a 6563 7420 7765 2061 7265 2070  Project we are p
+00000820: 726f 6365 7373 696e 670a 2020 2020 2020  rocessing.      
+00000830: 2020 3a70 6172 616d 2063 6f6c 6f72 6d61    :param colorma
+00000840: 703a 2063 6f6c 6f72 7320 746f 2075 7365  p: colors to use
+00000850: 2069 6e20 6f75 7470 7574 0a20 2020 2020   in output.     
+00000860: 2020 203a 7265 7475 726e 3a20 696e 666f     :return: info
+00000870: 726d 6174 696f 6e20 7265 6c61 7465 6420  rmation related 
+00000880: 746f 206c 6175 6e63 6865 7220 5461 736b  to launcher Task
+00000890: 0a20 2020 2072 1500 0000 5a05 5368 6172  .    r....Z.Shar
+000008a0: 654e da01 74da 136c 6175 6e63 6865 725f  eN..t..launcher_
+000008b0: 7461 736b 5f63 6f6c 6f72 7a10 5b4c 6175  task_colorz.[Lau
+000008c0: 6e63 6865 7220 5461 736b 3a20 7a02 5d20  ncher Task: z.] 
+000008d0: 5429 03da 0466 696e 64da 0474 6578 7472  T)...find..textr
+000008e0: 0200 0000 2905 7220 0000 0072 1200 0000  ....).r ...r....
+000008f0: da12 6c61 756e 6368 6572 5f74 6173 6b5f  ..launcher_task_
+00000900: 696e 666f 5a0d 7368 6172 655f 656c 656d  infoZ.share_elem
+00000910: 656e 745a 156c 6175 6e63 6865 725f 7461  entZ.launcher_ta
+00000920: 736b 5f65 6c65 6d65 6e74 721d 0000 0072  sk_elementr....r
+00000930: 1d00 0000 721e 0000 00da 1167 6574 5f6c  ....r......get_l
+00000940: 6175 6e63 6865 725f 7461 736b 4b00 0000  auncher_taskK...
+00000950: 731a 0000 0004 070a 0108 010a 0112 0102  s...............
+00000960: 0102 0102 0102 010c 0102 0104 fb04 0772  ...............r
+00000970: 2600 0000 da08 7461 736b 5f69 6473 da0c  &.....task_ids..
+00000980: 7072 6f6a 6563 745f 6e61 6d65 6309 0000  project_namec...
+00000990: 0000 0000 0000 0000 000f 0000 0010 0000  ................
+000009a0: 0043 0000 0073 e200 0000 6401 7d09 7c00  .C...s....d.}.|.
+000009b0: 4400 5d62 7d0a 7c0a 7c01 7601 7266 7c08  D.]b}.|.|.v.rf|.
+000009c0: 6402 1900 7366 7c08 6403 1900 7366 7400  d...sf|.d...sft.
+000009d0: a001 7c0a 7c01 6700 6404 7c07 6405 1900  ..|.|.g.d.|.d...
+000009e0: a105 5c02 7d0b 7d0c 7c01 a002 7c0a a101  ..\.}.}.|...|...
+000009f0: 0100 7c09 724c 7c00 724c 7c08 6402 1900  ..|.rL|.rL|.d...
+00000a00: 734c 7c08 6403 1900 734c 7403 7c04 7c05  sL|.d...sLt.|.|.
+00000a10: 7c02 6406 7404 7c04 6407 6404 6408 7c03  |.d.t.|.d.d.d.|.
+00000a20: 9b00 6409 9d03 6401 8305 8305 0100 7403  ..d...d.......t.
+00000a30: 7c04 7c05 7c02 640a 6404 8305 0100 640b  |.|.|.d.d.....d.
+00000a40: 7d09 7c0c 9b00 640c 7c03 9b00 640d 9d04  }.|...d.|...d...
+00000a50: 6701 7d0d 7400 a005 7c02 7c0c 7c0b 7c0d  g.}.t...|.|.|.|.
+00000a60: 7c03 7406 7c01 7c06 7c04 7c05 7c07 7c08  |.t.|.|.|.|.|.|.
+00000a70: 6401 a10d 7d0e 7104 7403 7c04 7c05 7c02  d...}.q.t.|.|.|.
+00000a80: 6406 6404 8305 0100 640e 5300 290f 6166  d.d.....d.S.).af
+00000a90: 0200 000a 2020 2020 5072 6f63 6573 7320  ....    Process 
+00000aa0: 616c 6c20 5461 736b 7320 696e 2050 726f  all Tasks in Pro
+00000ab0: 6a65 6374 2074 6861 7420 6172 6520 6e6f  ject that are no
+00000ac0: 7420 7265 6665 7265 6e63 6564 2062 7920  t referenced by 
+00000ad0: 6120 5072 6f66 696c 650a 2020 2020 2020  a Profile.      
+00000ae0: 2020 3a70 6172 616d 2074 6173 6b5f 6964    :param task_id
+00000af0: 733a 204c 6973 7420 6f66 2054 6173 6b20  s: List of Task 
+00000b00: 4944 730a 2020 2020 2020 2020 3a70 6172  IDs.        :par
+00000b10: 616d 2066 6f75 6e64 5f74 6173 6b73 3a20  am found_tasks: 
+00000b20: 6c69 7374 206f 6620 5461 736b 7320 666f  list of Tasks fo
+00000b30: 756e 6420 7468 7573 2066 6172 0a20 2020  und thus far.   
+00000b40: 2020 2020 203a 7061 7261 6d20 6f75 7470       :param outp
+00000b50: 7574 5f6c 6973 743a 206f 7574 7075 7420  ut_list: output 
+00000b60: 6c69 6e65 7320 6765 6e65 7261 7465 6420  lines generated 
+00000b70: 7468 7573 2066 6172 206f 6e74 6f20 7768  thus far onto wh
+00000b80: 6963 6820 7765 2077 696c 6c20 6170 7065  ich we will appe
+00000b90: 6e64 206d 6f72 650a 2020 2020 2020 2020  nd more.        
+00000ba0: 3a70 6172 616d 2070 726f 6a65 6374 5f6e  :param project_n
+00000bb0: 616d 653a 206e 616d 6520 6f66 2063 7572  ame: name of cur
+00000bc0: 7265 6e74 2050 726f 6a65 6374 0a20 2020  rent Project.   
+00000bd0: 2020 2020 203a 7061 7261 6d20 636f 6c6f       :param colo
+00000be0: 726d 6170 3a20 636f 6c6f 7273 2074 6f20  rmap: colors to 
+00000bf0: 7573 6520 696e 206f 7574 7075 740a 2020  use in output.  
+00000c00: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
+00000c10: 6772 616d 5f61 7267 733a 2072 756e 7469  gram_args: runti
+00000c20: 6d65 2061 7267 756d 656e 7473 0a20 2020  me arguments.   
+00000c30: 2020 2020 203a 7061 7261 6d20 6865 6164       :param head
+00000c40: 696e 673a 2063 7572 7265 6e74 2068 6561  ing: current hea
+00000c50: 6469 6e67 0a20 2020 2020 2020 203a 7061  ding.        :pa
+00000c60: 7261 6d20 616c 6c5f 7461 736b 6572 5f69  ram all_tasker_i
+00000c70: 7465 6d73 3a20 616c 6c20 5072 6f6a 6563  tems: all Projec
+00000c80: 7473 2f50 726f 6669 6c65 732f 5461 736b  ts/Profiles/Task
+00000c90: 732f 5363 656e 6573 0a20 2020 2020 2020  s/Scenes.       
+00000ca0: 203a 7061 7261 6d20 666f 756e 645f 6974   :param found_it
+00000cb0: 656d 733a 2073 696e 676c 6520 6974 656d  ems: single item
+00000cc0: 206e 616d 6520 666f 7220 5072 6f6a 6563   name for Projec
+00000cd0: 742f 5072 6f66 696c 652f 5461 736b 0a20  t/Profile/Task. 
+00000ce0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00000cf0: 6e6f 6e65 0a20 2020 2054 da14 7369 6e67  none.    T..sing
+00000d00: 6c65 5f70 726f 6669 6c65 5f66 6f75 6e64  le_profile_found
+00000d10: da11 7369 6e67 6c65 5f74 6173 6b5f 666f  ..single_task_fo
+00000d20: 756e 6472 1500 0000 da09 616c 6c5f 7461  undr......all_ta
+00000d30: 736b 73e9 0400 0000 da0a 7461 736b 5f63  sks.......task_c
+00000d40: 6f6c 6f72 7a35 3c62 723e 266e 6273 703b  olorz5<br>&nbsp;
+00000d50: 266e 6273 703b 266e 6273 703b 5468 6520  &nbsp;&nbsp;The 
+00000d60: 666f 6c6c 6f77 696e 6720 5461 736b 7320  following Tasks 
+00000d70: 696e 2050 726f 6a65 6374 207a 1e20 6172  in Project z. ar
+00000d80: 6520 6e6f 7420 696e 2061 6e79 2050 726f  e not in any Pro
+00000d90: 6669 6c65 2e2e 2e3c 6272 3ee9 0100 0000  file...<br>.....
+00000da0: 467a 2f20 3c65 6d3e 284e 6f74 2072 6566  Fz/ <em>(Not ref
+00000db0: 6572 656e 6365 6420 6279 2061 6e79 2050  erenced by any P
+00000dc0: 726f 6669 6c65 2069 6e20 5072 6f6a 6563  rofile in Projec
+00000dd0: 7420 7a06 293c 2f65 6d3e 4e29 07da 0574  t z.)</em>N)...t
+00000de0: 6173 6b73 5a0d 6765 745f 7461 736b 5f6e  asksZ.get_task_n
+00000df0: 616d 65da 0672 656d 6f76 6572 0500 0000  ame..remover....
+00000e00: 7202 0000 005a 0b6f 7574 7075 745f 7461  r....Z.output_ta
+00000e10: 736b 720b 0000 0029 0f72 2700 0000 720d  skr....).r'...r.
+00000e20: 0000 0072 0c00 0000 7228 0000 0072 1200  ...r....r(...r..
+00000e30: 0000 720f 0000 0072 1100 0000 7213 0000  ..r....r....r...
+00000e40: 0072 1000 0000 5a12 6f75 7470 7574 5f74  .r....Z.output_t
+00000e50: 6865 5f68 6561 6469 6e67 5a06 7468 655f  he_headingZ.the_
+00000e60: 6964 721c 0000 005a 0d6f 7572 5f74 6173  idr....Z.our_tas
+00000e70: 6b5f 6e61 6d65 5a09 7461 736b 5f6c 6973  k_nameZ.task_lis
+00000e80: 745a 046b 616b 6172 1d00 0000 721d 0000  tZ.kakar....r...
+00000e90: 0072 1e00 0000 da15 7461 736b 735f 6e6f  .r......tasks_no
+00000ea0: 745f 696e 5f70 726f 6669 6c65 7364 0000  t_in_profilesd..
+00000eb0: 0073 7600 0000 021a 02ff 0805 0802 0602  .sv.............
+00000ec0: 02fe 0603 02fd 0406 0e01 08ff 0a04 0205  ................
+00000ed0: 02ff 0202 02fe 0603 02fd 0604 02fc 0206  ................
+00000ee0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000ef0: 0202 0201 06ff 0203 02f8 04fb 1010 0401  ................
+00000f00: 0604 0201 06ff 04ff 0406 0201 0201 0201  ................
+00000f10: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000f20: 0201 0201 04f3 0280 1010 0401 7231 0000  ............r1..
+00000f30: 0072 2500 0000 6308 0000 0000 0000 0000  .r%...c.........
+00000f40: 0000 000b 0000 000a 0000 0043 0000 0073  ...........C...s
+00000f50: ac00 0000 6401 0400 7d08 7d09 7c00 6402  ....d...}.}.|.d.
+00000f60: 1900 6403 6b02 7213 7400 7c02 8301 7d08  ..d.k.r.t.|...}.
+00000f70: 7401 7c02 6404 8302 7d09 7402 7c01 6405  t.|.d...}.t.|.d.
+00000f80: 6401 6406 7c03 9b00 9d02 6407 8305 7d0a  d.d.|.....d...}.
+00000f90: 7c00 6408 1900 7243 7c03 7c00 6408 1900  |.d...rC|.|.d...
+00000fa0: 6b03 722a 6407 5300 6407 7c04 6409 3c00  k.r*d.S.d.|.d.<.
+00000fb0: 7403 6404 7c06 7c0a 9b00 640a 7c07 9b00  t.d.|.|...d.|...
+00000fc0: 7c09 9b00 7c08 9b00 9d05 6401 7c05 7c01  |...|.....d.|.|.
+00000fd0: 7c00 8307 0100 6404 5300 7404 7c01 7c00  |.....d.S.t.|.|.
+00000fe0: 7c06 640b 7c0a 9b00 640a 7c07 9b00 7c09  |.d.|...d.|...|.
+00000ff0: 9b00 7c08 9b00 9d05 8305 0100 6404 5300  ..|.........d.S.
+00001000: 290c 616f 0200 000a 2020 2020 4164 6420  ).ao....    Add 
+00001010: 6578 7472 6120 696e 666f 2074 6f20 5072  extra info to Pr
+00001020: 6f6a 6563 7420 6f75 7470 7574 206c 696e  oject output lin
+00001030: 6520 6173 2061 7070 726f 7072 6961 7465  e as appropriate
+00001040: 2061 6e64 2074 6865 6e20 6f75 7470 7574   and then output
+00001050: 2069 742e 0a20 2020 2020 2020 203a 7061   it..        :pa
+00001060: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
+00001070: 3a20 7275 6e74 696d 6520 6172 6775 6d65  : runtime argume
+00001080: 6e74 730a 2020 2020 2020 2020 3a70 6172  nts.        :par
+00001090: 616d 2063 6f6c 6f72 6d61 703a 2063 6f6c  am colormap: col
+000010a0: 6f72 7320 746f 2075 7365 2069 6e20 7075  ors to use in pu
+000010b0: 7470 7574 0a20 2020 2020 2020 203a 7061  tput.        :pa
+000010c0: 7261 6d20 7072 6f6a 6563 743a 2050 726f  ram project: Pro
+000010d0: 6a65 6374 2078 6d6c 2065 6c65 6d65 6e74  ject xml element
+000010e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000010f0: 7072 6f6a 6563 745f 6e61 6d65 3a20 6e61  project_name: na
+00001100: 6d65 206f 6620 5072 6f6a 6563 740a 2020  me of Project.  
+00001110: 2020 2020 2020 3a70 6172 616d 2066 6f75        :param fou
+00001120: 6e64 5f69 7465 6d73 3a20 7369 6e67 6c65  nd_items: single
+00001130: 206e 616d 6520 666f 7220 5072 6f6a 6563   name for Projec
+00001140: 742f 5072 6f66 696c 652f 5461 736b 2069  t/Profile/Task i
+00001150: 6620 7072 6f76 6964 6564 0a20 2020 2020  f provided.     
+00001160: 2020 203a 7061 7261 6d20 6865 6164 696e     :param headin
+00001170: 673a 206c 6173 7420 6f75 7470 7574 2068  g: last output h
+00001180: 6561 6469 6e67 0a20 2020 2020 2020 203a  eading.        :
+00001190: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
+000011a0: 743a 206c 6973 7420 6f66 206f 7574 7075  t: list of outpu
+000011b0: 7420 6c69 6e65 7320 6765 6e65 7261 7465  t lines generate
+000011c0: 6420 7468 7573 2066 6172 0a20 2020 2020  d thus far.     
+000011d0: 2020 203a 7061 7261 6d20 6c61 756e 6368     :param launch
+000011e0: 6572 5f74 6173 6b5f 696e 666f 3a20 6465  er_task_info: de
+000011f0: 7461 696c 7320 6162 6f75 7420 2861 6e79  tails about (any
+00001200: 2920 6c61 756e 6368 6572 2054 6173 6b0a  ) launcher Task.
+00001210: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001220: 2054 7275 6520 6966 2077 6520 6172 6520   True if we are 
+00001230: 6c6f 6f6b 696e 6720 666f 7220 6120 7369  looking for a si
+00001240: 6e67 6c65 2050 726f 6a65 6374 2061 6e64  ngle Project and
+00001250: 2074 6869 7320 6973 6e27 7420 6974 2e20   this isn't it. 
+00001260: 2046 616c 7365 206f 7468 6572 7769 7365   False otherwise
+00001270: 2e0a 2020 2020 7215 0000 00da 1464 6973  ..    r......dis
+00001280: 706c 6179 5f64 6574 6169 6c5f 6c65 7665  play_detail_leve
+00001290: 6c72 1600 0000 46da 0d70 726f 6a65 6374  lr....F..project
+000012a0: 5f63 6f6c 6f72 7a09 5072 6f6a 6563 743a  _colorz.Project:
+000012b0: 2054 da13 7369 6e67 6c65 5f70 726f 6a65   T..single_proje
+000012c0: 6374 5f6e 616d 65da 1473 696e 676c 655f  ct_name..single_
+000012d0: 7072 6f6a 6563 745f 666f 756e 64fa 0120  project_found.. 
+000012e0: e902 0000 0029 0572 0400 0000 7207 0000  .....).r....r...
+000012f0: 0072 0200 0000 7206 0000 0072 0500 0000  .r....r....r....
+00001300: 290b 720f 0000 0072 1200 0000 7220 0000  ).r....r....r ..
+00001310: 0072 2800 0000 7210 0000 0072 1100 0000  .r(...r....r....
+00001320: 720c 0000 0072 2500 0000 5a0c 6b69 645f  r....r%...Z.kid_
+00001330: 6170 705f 696e 666f da08 7072 696f 7269  app_info..priori
+00001340: 7479 5a14 7072 6f6a 6563 745f 6e61 6d65  tyZ.project_name
+00001350: 5f64 6574 6169 6c73 721d 0000 0072 1d00  _detailsr....r..
+00001360: 0000 721e 0000 00da 1c67 6574 5f65 7874  ..r......get_ext
+00001370: 7261 5f61 6e64 5f6f 7574 7075 745f 7072  ra_and_output_pr
+00001380: 6f6a 6563 74c9 0000 0073 3a00 0000 0817  oject....s:.....
+00001390: 0c01 0801 0a01 0203 1001 04ff 0805 0c01  ................
+000013a0: 0401 0802 0201 0201 0201 1401 0201 0201  ................
+000013b0: 0201 0201 04f9 0411 02f9 0201 0201 0201  ................
+000013c0: 0201 1401 04fb 0407 7239 0000 0072 1c00  ........r9...r..
+000013d0: 0000 6309 0000 0000 0000 0000 0000 000e  ..c.............
+000013e0: 0000 000c 0000 0043 0000 0073 6a01 0000  .......C...sj...
+000013f0: 7c08 6401 1900 4400 5dae 7d09 7c00 6402  |.d...D.].}.|.d.
+00001400: 1900 730e 7c00 6403 1900 7211 0100 6700  ..s.|.d...r...g.
+00001410: 5300 7c09 a000 6404 a101 6a01 7d0a 7402  S.|...d...j.}.t.
+00001420: 7c09 7c06 8302 7d0b 7403 7c07 7c06 7c09  |.|...}.t.|.|.|.
+00001430: 7c0a 7c00 7c02 7c01 7c0b 8308 7228 7104  |.|.|.|.|...r(q.
+00001440: 7c07 6405 1900 7233 7404 7c09 7c06 7c07  |.d...r3t.|.|.|.
+00001450: 7c01 8304 0100 7405 6406 7c07 7c06 7c01  |.....t.d.|.|.|.
+00001460: 7c09 7c0a 7c03 8307 0400 7d0c 7256 7406  |.|.|.....}.rVt.
+00001470: 7c01 7c09 7c0a 7c0c 7c04 7c07 7c02 7c06  |.|.|.|.|.|.|.|.
+00001480: 7c08 7c00 830a 7d05 7c07 6407 1900 7255  |.|...}.|.d...rU
+00001490: 7c00 6403 1900 7355 7104 6e0e 7407 7c06  |.d...sUq.n.t.|.
+000014a0: 7c07 7c01 6408 7408 7c06 6409 640a 640b  |.|.d.t.|.d.d.d.
+000014b0: 640c 8305 8305 0100 7407 7c06 7c07 7c01  d.......t.|.|.|.
+000014c0: 640d 640a 8305 0100 7405 640c 6900 6900  d.d.....t.d.i.i.
+000014d0: 6700 7c09 7c0a 6700 8307 0400 7d0d 7284  g.|.|.g.....}.r.
+000014e0: 7409 7c0d 7c04 7c01 7c0a 7c06 7c07 7c02  t.|.|.|.|.|.|.|.
+000014f0: 7c08 7c00 8309 0100 7c07 640e 1900 7392  |.|.....|.d...s.
+00001500: 740a 7c09 7c06 7c07 7c01 7c05 7c04 7c08  t.|.|.|.|.|.|.|.
+00001510: 8307 0100 7407 7c06 7c07 7c01 640d 640a  ....t.|.|.|.d.d.
+00001520: 8305 0100 7c00 640f 1900 73a6 7c00 6403  ....|.d...s.|.d.
+00001530: 1900 73a6 7c00 6402 1900 72b2 7407 7c06  ..s.|.d...r.t.|.
+00001540: 7c07 7c01 640d 640a 8305 0100 7c04 0200  |.|.d.d.....|...
+00001550: 0100 5300 7104 6700 5300 2910 6160 0200  ..S.q.g.S.).a`..
+00001560: 000a 2020 2020 476f 2074 6872 6f75 6768  ..    Go through
+00001570: 2061 6c6c 2074 6865 2050 726f 6a65 6374   all the Project
+00001580: 732c 2067 6574 2074 6865 6972 2064 6574  s, get their det
+00001590: 6169 6c20 616e 6420 6f75 7470 7574 2069  ail and output i
+000015a0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+000015b0: 2066 6f75 6e64 5f69 7465 6d73 3a20 616c   found_items: al
+000015c0: 6c20 6974 656d 7320 666f 756e 6420 736f  l items found so
+000015d0: 2066 6172 0a20 2020 2020 2020 203a 7061   far.        :pa
+000015e0: 7261 6d20 6f75 7470 7574 5f6c 6973 743a  ram output_list:
+000015f0: 206c 6973 7420 6f66 206f 7574 7075 7420   list of output 
+00001600: 6c69 6e65 7320 6765 6e65 7261 7465 6420  lines generated 
+00001610: 736f 2066 6172 0a20 2020 2020 2020 203a  so far.        :
+00001620: 7061 7261 6d20 6865 6164 696e 673a 2074  param heading: t
+00001630: 6865 206f 7574 7075 7420 6865 6164 696e  he output headin
+00001640: 670a 2020 2020 2020 2020 3a70 6172 616d  g.        :param
+00001650: 2070 726f 6a65 6374 735f 7769 7468 6f75   projects_withou
+00001660: 745f 7072 6f66 696c 6573 3a20 6c69 7374  t_profiles: list
+00001670: 206f 6620 5072 6f6a 6563 7473 2077 6974   of Projects wit
+00001680: 6820 6e6f 2050 726f 6669 6c65 730a 2020  h no Profiles.  
+00001690: 2020 2020 2020 3a70 6172 616d 2066 6f75        :param fou
+000016a0: 6e64 5f74 6173 6b73 3a20 6c69 7374 206f  nd_tasks: list o
+000016b0: 6620 5461 736b 7320 666f 756e 640a 2020  f Tasks found.  
+000016c0: 2020 2020 2020 3a70 6172 616d 206f 7572        :param our
+000016d0: 5f74 6173 6b5f 656c 656d 656e 743a 2078  _task_element: x
+000016e0: 6d6c 2065 6c65 6d65 6e74 206f 6620 6f75  ml element of ou
+000016f0: 7220 5461 736b 0a20 2020 2020 2020 203a  r Task.        :
+00001700: 7061 7261 6d20 636f 6c6f 726d 6170 3a20  param colormap: 
+00001710: 6f75 7470 7574 2063 6f6c 6f72 7320 746f  output colors to
+00001720: 2075 7365 0a20 2020 2020 2020 203a 7061   use.        :pa
+00001730: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
+00001740: 3a20 7275 6e74 696d 6520 6172 6775 6d65  : runtime argume
+00001750: 6e74 730a 2020 2020 2020 2020 3a70 6172  nts.        :par
+00001760: 616d 2061 6c6c 5f74 6173 6b65 725f 6974  am all_tasker_it
+00001770: 656d 733a 2061 6c6c 2050 726f 6a65 6374  ems: all Project
+00001780: 732f 5072 6f66 696c 6573 2f54 6173 6b73  s/Profiles/Tasks
+00001790: 2f53 6365 6e65 730a 2020 2020 2020 2020  /Scenes.        
+000017a0: 3a72 6574 7572 6e3a 206c 6973 7420 6f66  :return: list of
+000017b0: 2066 6f75 6e64 2054 6173 6b73 0a20 2020   found Tasks.   
+000017c0: 20da 0c61 6c6c 5f70 726f 6a65 6374 7372   ..all_projectsr
+000017d0: 2a00 0000 7229 0000 00da 046e 616d 65da  *...r).....name.
+000017e0: 1164 6973 706c 6179 5f74 6173 6b65 726e  .display_taskern
+000017f0: 6574 54da 1373 696e 676c 655f 7072 6f66  etT..single_prof
+00001800: 696c 655f 6e61 6d65 7237 0000 00da 0d70  ile_namer7.....p
+00001810: 726f 6669 6c65 5f63 6f6c 6f72 7215 0000  rofile_colorr...
+00001820: 007a 203c 656d 3e50 726f 6a65 6374 2068  .z <em>Project h
+00001830: 6173 206e 6f20 5072 6f66 696c 6573 3c2f  as no Profiles</
+00001840: 656d 3e46 7216 0000 00da 1073 696e 676c  em>Fr......singl
+00001850: 655f 7461 736b 5f6e 616d 6572 3500 0000  e_task_namer5...
+00001860: 290b 7223 0000 0072 2400 0000 7226 0000  ).r#...r$...r&..
+00001870: 0072 3900 0000 720a 0000 0072 0300 0000  .r9...r....r....
+00001880: 7208 0000 0072 0500 0000 7202 0000 0072  r....r....r....r
+00001890: 3100 0000 7209 0000 0029 0e72 1000 0000  1...r....).r....
+000018a0: 720c 0000 0072 1100 0000 720e 0000 0072  r....r....r....r
+000018b0: 0d00 0000 721c 0000 0072 1200 0000 720f  ....r....r....r.
+000018c0: 0000 0072 1300 0000 7220 0000 0072 2800  ...r....r ...r(.
+000018d0: 0000 7225 0000 005a 0b70 726f 6669 6c65  ..r%...Z.profile
+000018e0: 5f69 6473 7227 0000 0072 1d00 0000 721d  _idsr'...r....r.
+000018f0: 0000 0072 1e00 0000 7217 0000 0007 0100  ...r....r.......
+00001900: 0073 ba00 0000 0c19 1002 0201 0468 0c99  .s...........h..
+00001910: 0a03 0203 0201 0201 0201 0201 0201 0201  ................
+00001920: 0201 0201 04f8 020a 0803 0e01 0202 0201  ................
+00001930: 0201 0201 0201 0201 0201 0201 08f9 0209  ................
+00001940: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001950: 0201 0201 04f6 060f 02ff 0602 02fe 0204  ................
+00001960: 0280 0202 0201 0201 0201 0201 0201 0201  ................
+00001970: 0201 0201 0201 0201 02fb 04fb 100d 1803  ................
+00001980: 0202 0201 0201 0201 0201 0201 0201 0201  ................
+00001990: 0201 0201 04f7 080d 0201 0201 0201 0201  ................
+000019a0: 0201 0201 0201 0201 04f9 100a 0602 02ff  ................
+000019b0: 0602 02fe 0603 02fd 1005 0801 02fa 0409  ................
+000019c0: 7217 0000 0029 23da 1664 6566 7573 6564  r....)#..defused
+000019d0: 786d 6c2e 456c 656d 656e 7454 7265 65da  xml.ElementTree.
+000019e0: 0a64 6566 7573 6564 786d 6c5a 136d 6170  .defusedxmlZ.map
+000019f0: 7461 736b 6572 2e73 7263 2e74 6173 6b73  tasker.src.tasks
+00001a00: da03 7372 6372 2f00 0000 da16 6d61 7074  ..srcr/.....mapt
+00001a10: 6173 6b65 722e 7372 632e 6672 6d74 6874  asker.src.frmtht
+00001a20: 6d6c 7202 0000 005a 146d 6170 7461 736b  mlr....Z.maptask
+00001a30: 6572 2e73 7263 2e67 6574 6964 7372 0300  er.src.getidsr..
+00001a40: 0000 5a14 6d61 7074 6173 6b65 722e 7372  ..Z.maptasker.sr
+00001a50: 632e 6b69 6461 7070 7204 0000 00da 156d  c.kidappr......m
+00001a60: 6170 7461 736b 6572 2e73 7263 2e6f 7574  aptasker.src.out
+00001a70: 7075 746c 7205 0000 0072 0600 0000 5a16  putlr....r....Z.
+00001a80: 6d61 7074 6173 6b65 722e 7372 632e 7072  maptasker.src.pr
+00001a90: 696f 7269 7479 7207 0000 005a 166d 6170  iorityr....Z.map
+00001aa0: 7461 736b 6572 2e73 7263 2e70 726f 6669  tasker.src.profi
+00001ab0: 6c65 7372 0800 0000 5a14 6d61 7074 6173  lesr....Z.maptas
+00001ac0: 6b65 722e 7372 632e 7363 656e 6573 7209  ker.src.scenesr.
+00001ad0: 0000 005a 136d 6170 7461 736b 6572 2e73  ...Z.maptasker.s
+00001ae0: 7263 2e73 6861 7265 720a 0000 00da 166d  rc.sharer......m
+00001af0: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
+00001b00: 636f 6e73 7472 0b00 0000 7218 0000 0072  constr....r....r
+00001b10: 1900 0000 da03 7374 7272 1f00 0000 da0b  ......strr......
+00001b20: 456c 656d 656e 7454 7265 65da 0358 4d4c  ElementTree..XML
+00001b30: 7226 0000 0072 3100 0000 da04 626f 6f6c  r&...r1.....bool
+00001b40: 7239 0000 0072 1700 0000 721d 0000 0072  r9...r....r....r
+00001b50: 1d00 0000 721d 0000 0072 1e00 0000 da08  ....r....r......
+00001b60: 3c6d 6f64 756c 653e 0100 0000 73ba 0000  <module>....s...
+00001b70: 0008 0e12 020c 010c 010c 010c 010c 010c  ................
+00001b80: 010c 010c 010c 010c 0102 0602 0102 ff02  ................
+00001b90: 0202 fe02 0302 fd02 0402 fc02 0502 fb02  ................
+00001ba0: 0602 fa02 0702 f902 0802 f802 090a f71a  ................
+00001bb0: 2a02 1902 0102 ff02 0202 fe02 0302 fd02  *...............
+00001bc0: 0402 fc02 0502 fb02 0602 fa02 0702 f902  ................
+00001bd0: 0802 f802 0902 f702 0a0a f602 6502 0102  ............e...
+00001be0: ff02 0202 fe06 0302 fd02 0402 fc02 0502  ................
+00001bf0: fb02 0602 fa02 0702 f902 0802 f802 090a  ................
+00001c00: f702 3e02 0102 ff02 0202 fe02 0302 fd02  ..>.............
+00001c10: 0402 fc02 0502 fb06 0602 fa02 0702 f902  ................
+00001c20: 0802 f802 0902 f702 0a0e f6              ...........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/runcli.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/runcli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/rungui.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/rungui.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 23 17:42:41 2023 UTC, .py size: 4154 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 918f 1c64 3a10 0000  o..........d:...
+00000000: 6f0d 0d0a 0000 0000 ee25 3464 3510 0000  o........%4d5...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c06 6d08 5a08 0100 6501 7226 6400  d.l.m.Z...e.r&d.
 00000070: 6406 6c09 6d0a 610a 0100 6407 6408 8400  d.l.m.a...d.d...
@@ -26,76 +26,74 @@
 00000190: 696b 7275 6269 6e40 676d 6169 6c2e 636f  ikrubin@gmail.co
 000001a0: 6d2f 4d79 2044 7269 7665 2f50 7974 686f  m/My Drive/Pytho
 000001b0: 6e2f 6d61 7074 6173 6b65 722f 6d61 7074  n/maptasker/mapt
 000001c0: 6173 6b65 722f 7372 632f 7275 6e67 7569  asker/src/rungui
 000001d0: 2e70 79da 0f6f 7574 7075 745f 616e 645f  .py..output_and_
 000001e0: 7175 6974 2100 0000 7306 0000 0004 0108  quit!...s.......
 000001f0: 010e 0172 0d00 0000 6302 0000 0000 0000  ...r....c.......
-00000200: 0000 0000 0008 0000 000a 0000 0043 0000  .............C..
-00000210: 0073 1401 0000 7c01 7208 6401 6402 6c00  .s....|.r.d.d.l.
+00000200: 0000 0000 0007 0000 0008 0000 0043 0000  .............C..
+00000210: 0073 0201 0000 7c01 7208 6401 6402 6c00  .s....|.r.d.d.l.
 00000220: 6d01 6101 0100 7401 8300 7d02 7c02 a002  m.a...t...}.|...
 00000230: a100 0100 7c02 6a03 7219 7404 6403 8301  ....|.j.r.t.d...
 00000240: 0100 7403 8300 0100 7c02 6a05 7324 7404  ..t.....|.j.s$t.
 00000250: 6404 8301 0100 7403 6405 8301 0100 7406  d.....t.d.....t.
 00000260: 8300 7d03 7a09 7407 7c02 6a08 8301 7c03  ..}.z.t.|.j...|.
-00000270: 6406 3c00 5700 6e14 0400 7409 7944 0100  d.<.W.n...t.yD..
-00000280: 7d04 0100 7a08 6407 7d05 5700 5900 6400  }...z.d.}.W.Y.d.
-00000290: 7d04 7e04 6e05 6400 7d04 7e04 7701 7700  }.~.n.d.}.~.w.w.
-000002a0: 7c02 6a0a 7c03 6408 3c00 7c02 6a0b 7c03  |.j.|.d.<.|.j.|.
-000002b0: 6409 3c00 7c02 6a0c 7c03 640a 3c00 7c02  d.<.|.j.|.d.<.|.
-000002c0: 6a0d 7c03 640b 3c00 7c02 6a0e 7c03 640c  j.|.d.<.|.j.|.d.
-000002d0: 3c00 7c02 6a0f 7c03 640d 3c00 7410 7c02  <.|.j.|.d.<.t.|.
-000002e0: 6a11 7c00 8302 7d00 7c02 6a12 727a 7c02  j.|...}.|.j.rz|.
-000002f0: 6a12 a013 a100 4400 5d08 5c02 7d06 7d07  j.....D.].\.}.}.
-00000300: 7c07 7c00 7c06 3c00 7171 7c02 6a14 7c03  |.|.|.<.qq|.j.|.
-00000310: 640e 3c00 7401 a015 7c02 a101 0100 7e02  d.<.t...|.....~.
-00000320: 6201 7c03 7c00 6602 5300 290f 4e72 0100  b.|.|.f.S.).Nr..
-00000330: 0000 7207 0000 007a 1850 726f 6772 616d  ..r....z.Program
-00000340: 2065 7869 7465 642e 2047 6f6f 6462 7965   exited. Goodbye
-00000350: 2e7a 2650 726f 6772 616d 2063 616e 6365  .z&Program cance
-00000360: 6c6c 6564 2062 6520 7573 6572 2028 6b69  lled be user (ki
-00000370: 6c6c 6564 2047 5549 29e9 6300 0000 da14  lled GUI).c.....
-00000380: 6469 7370 6c61 795f 6465 7461 696c 5f6c  display_detail_l
-00000390: 6576 656c e901 0000 00da 1a64 6973 706c  evel.......displ
-000003a0: 6179 5f70 726f 6669 6c65 5f63 6f6e 6469  ay_profile_condi
-000003b0: 7469 6f6e 73da 1364 6973 706c 6179 5f70  tions..display_p
-000003c0: 7265 6665 7265 6e63 6573 da11 6469 7370  references..disp
-000003d0: 6c61 795f 7461 736b 6572 6e65 74da 1373  lay_taskernet..s
-000003e0: 696e 676c 655f 7072 6f6a 6563 745f 6e61  ingle_project_na
-000003f0: 6d65 da13 7369 6e67 6c65 5f70 726f 6669  me..single_profi
-00000400: 6c65 5f6e 616d 65da 1073 696e 676c 655f  le_name..single_
-00000410: 7461 736b 5f6e 616d 6572 0a00 0000 2916  task_namer....).
-00000420: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
-00000430: 7573 6572 696e 7472 7208 0000 00da 086d  userintrr......m
-00000440: 6169 6e6c 6f6f 70da 0465 7869 7472 0d00  ainloop..exitr..
-00000450: 0000 5a0a 676f 5f70 726f 6772 616d 7203  ..Z.go_programr.
-00000460: 0000 00da 0369 6e74 720f 0000 00da 0945  .....intr......E
-00000470: 7863 6570 7469 6f6e 7211 0000 0072 1200  xceptionr....r..
-00000480: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00000490: 0072 1600 0000 7204 0000 005a 0f61 7070  .r....r....Z.app
-000004a0: 6561 7261 6e63 655f 6d6f 6465 5a0c 636f  earance_modeZ.co
-000004b0: 6c6f 725f 6c6f 6f6b 7570 da05 6974 656d  lor_lookup..item
-000004c0: 7372 0a00 0000 da04 7175 6974 2908 da08  sr......quit)...
-000004d0: 636f 6c6f 726d 6170 5a07 7573 655f 6775  colormapZ.use_gu
-000004e0: 695a 0a75 7365 725f 696e 7075 74da 0970  iZ.user_input..p
-000004f0: 726f 675f 6172 6773 da01 6572 0f00 0000  rog_args..er....
-00000500: da03 6b65 79da 0576 616c 7565 720b 0000  ..key..valuer...
-00000510: 0072 0b00 0000 720c 0000 00da 0b70 726f  .r....r......pro
-00000520: 6365 7373 5f67 7569 2a00 0000 7344 0000  cess_gui*...sD..
-00000530: 0004 020c 0106 0308 0106 0208 0106 0106  ................
-00000540: 0308 0108 0106 0302 0312 010e 0110 0108  ................
-00000550: 8002 ff0a 030a 010a 010a 010a 010a 010c  ................
-00000560: 0206 0212 010a 010a 030a 0302 0102 0102  ................
-00000570: 0302 0104 fe72 2300 0000 4e29 0dda 146d  .....r#...N)...m
-00000580: 6170 7461 736b 6572 2e73 7263 2e63 6f6e  aptasker.src.con
-00000590: 6669 6772 0200 0000 da16 6d61 7074 6173  figr......maptas
-000005a0: 6b65 722e 7372 632e 696e 6974 7061 7267  ker.src.initparg
-000005b0: 7203 0000 00da 166d 6170 7461 736b 6572  r......maptasker
-000005c0: 2e73 7263 2e63 6f6c 726d 6f64 6572 0400  .src.colrmoder..
-000005d0: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
-000005e0: 632e 7379 7363 6f6e 7374 7205 0000 0072  c.sysconstr....r
-000005f0: 0600 0000 7217 0000 0072 0800 0000 720d  ....r....r....r.
-00000600: 0000 0072 2300 0000 720b 0000 0072 0b00  ...r#...r....r..
-00000610: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
-00000620: 6f64 756c 653e 0100 0000 7312 0000 000c  odule>....s.....
-00000630: 130c 010c 010c 010c 0104 020c 0108 060c  ................
-00000640: 09                                       .
+00000270: 6406 3c00 5700 6e0b 0400 7409 793b 0100  d.<.W.n...t.y;..
+00000280: 0100 0100 6407 7d04 5900 6e01 7700 7c02  ....d.}.Y.n.w.|.
+00000290: 6a0a 7c03 6408 3c00 7c02 6a0b 7c03 6409  j.|.d.<.|.j.|.d.
+000002a0: 3c00 7c02 6a0c 7c03 640a 3c00 7c02 6a0d  <.|.j.|.d.<.|.j.
+000002b0: 7c03 640b 3c00 7c02 6a0e 7c03 640c 3c00  |.d.<.|.j.|.d.<.
+000002c0: 7c02 6a0f 7c03 640d 3c00 7410 7c02 6a11  |.j.|.d.<.t.|.j.
+000002d0: 7c00 8302 7d00 7c02 6a12 7271 7c02 6a12  |...}.|.j.rq|.j.
+000002e0: a013 a100 4400 5d08 5c02 7d05 7d06 7c06  ....D.].\.}.}.|.
+000002f0: 7c00 7c05 3c00 7168 7c02 6a14 7c03 640e  |.|.<.qh|.j.|.d.
+00000300: 3c00 7401 a015 7c02 a101 0100 7e02 6201  <.t...|.....~.b.
+00000310: 7c03 7c00 6602 5300 290f 4e72 0100 0000  |.|.f.S.).Nr....
+00000320: 7207 0000 007a 1850 726f 6772 616d 2065  r....z.Program e
+00000330: 7869 7465 642e 2047 6f6f 6462 7965 2e7a  xited. Goodbye.z
+00000340: 2650 726f 6772 616d 2063 616e 6365 6c6c  &Program cancell
+00000350: 6564 2062 6520 7573 6572 2028 6b69 6c6c  ed be user (kill
+00000360: 6564 2047 5549 29e9 6300 0000 da14 6469  ed GUI).c.....di
+00000370: 7370 6c61 795f 6465 7461 696c 5f6c 6576  splay_detail_lev
+00000380: 656c e901 0000 00da 1a64 6973 706c 6179  el.......display
+00000390: 5f70 726f 6669 6c65 5f63 6f6e 6469 7469  _profile_conditi
+000003a0: 6f6e 73da 1364 6973 706c 6179 5f70 7265  ons..display_pre
+000003b0: 6665 7265 6e63 6573 da11 6469 7370 6c61  ferences..displa
+000003c0: 795f 7461 736b 6572 6e65 74da 1373 696e  y_taskernet..sin
+000003d0: 676c 655f 7072 6f6a 6563 745f 6e61 6d65  gle_project_name
+000003e0: da13 7369 6e67 6c65 5f70 726f 6669 6c65  ..single_profile
+000003f0: 5f6e 616d 65da 1073 696e 676c 655f 7461  _name..single_ta
+00000400: 736b 5f6e 616d 6572 0a00 0000 2916 da16  sk_namer....)...
+00000410: 6d61 7074 6173 6b65 722e 7372 632e 7573  maptasker.src.us
+00000420: 6572 696e 7472 7208 0000 00da 086d 6169  erintrr......mai
+00000430: 6e6c 6f6f 70da 0465 7869 7472 0d00 0000  nloop..exitr....
+00000440: 5a0a 676f 5f70 726f 6772 616d 7203 0000  Z.go_programr...
+00000450: 00da 0369 6e74 720f 0000 00da 0954 7970  ...intr......Typ
+00000460: 6545 7272 6f72 7211 0000 0072 1200 0000  eErrorr....r....
+00000470: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000480: 1600 0000 7204 0000 005a 0f61 7070 6561  ....r....Z.appea
+00000490: 7261 6e63 655f 6d6f 6465 5a0c 636f 6c6f  rance_modeZ.colo
+000004a0: 725f 6c6f 6f6b 7570 da05 6974 656d 7372  r_lookup..itemsr
+000004b0: 0a00 0000 da04 7175 6974 2907 da08 636f  ......quit)...co
+000004c0: 6c6f 726d 6170 5a07 7573 655f 6775 695a  lormapZ.use_guiZ
+000004d0: 0a75 7365 725f 696e 7075 74da 0970 726f  .user_input..pro
+000004e0: 675f 6172 6773 720f 0000 00da 036b 6579  g_argsr......key
+000004f0: da05 7661 6c75 6572 0b00 0000 720b 0000  ..valuer....r...
+00000500: 0072 0c00 0000 da0b 7072 6f63 6573 735f  .r......process_
+00000510: 6775 692a 0000 0073 4200 0000 0402 0c01  gui*...sB.......
+00000520: 0603 0801 0602 0801 0601 0603 0801 0801  ................
+00000530: 0603 0203 1201 0c01 0801 02ff 0a03 0a01  ................
+00000540: 0a01 0a01 0a01 0a01 0c02 0602 1201 0a01  ................
+00000550: 0a03 0a03 0201 0201 0203 0201 04fe 7222  ..............r"
+00000560: 0000 004e 290d da14 6d61 7074 6173 6b65  ...N)...maptaske
+00000570: 722e 7372 632e 636f 6e66 6967 7202 0000  r.src.configr...
+00000580: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+00000590: 2e69 6e69 7470 6172 6772 0300 0000 da16  .initpargr......
+000005a0: 6d61 7074 6173 6b65 722e 7372 632e 636f  maptasker.src.co
+000005b0: 6c72 6d6f 6465 7204 0000 00da 166d 6170  lrmoder......map
+000005c0: 7461 736b 6572 2e73 7263 2e73 7973 636f  tasker.src.sysco
+000005d0: 6e73 7472 0500 0000 7206 0000 0072 1700  nstr....r....r..
+000005e0: 0000 7208 0000 0072 0d00 0000 7222 0000  ..r....r....r"..
+000005f0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
+00000600: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000610: 0000 0073 1200 0000 0c13 0c01 0c01 0c01  ...s............
+00000620: 0c01 0402 0c01 0806 0c09                 ..........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/scenes.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/scenes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 14:44:36 2023 UTC, .py size: 7762 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,266 +1,273 @@
-00000000: 6f0d 0d0a 0000 0000 d437 2c64 521e 0000  o........7,dR...
+00000000: 6f0d 0d0a 0000 0000 3b8e 3564 fe1e 0000  o.......;.5d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0010 0000 0040 0000 0073 f200 0000 6400  .....@...s....d.
+00000020: 0010 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 6d04 0200 0100 6d05 5a05 0100  d.l.m.....m.Z...
 00000050: 6400 6402 6c06 6d07 5a07 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6400 6404 6c0a 6d0b  l.m.Z...d.d.l.m.
-00000070: 5a0b 0100 6405 6406 6407 6408 6409 640a  Z...d.d.d.d.d.d.
-00000080: 640b 640c 640d 640e 640f 6410 6411 6412  d.d.d.d.d.d.d.d.
-00000090: 6413 6414 9c0f 5a0c 6700 6415 a201 5a0d  d.d...Z.g.d...Z.
-000000a0: 6416 6502 6a0e 6417 650f 6418 650f 6419  d.e.j.d.e.d.e.d.
-000000b0: 6510 641a 6401 660a 641b 641c 8404 5a11  e.d.d.f.d.d...Z.
-000000c0: 641d 6512 6419 6510 6512 1900 641e 6510  d.e.d.e.e...d.e.
-000000d0: 6512 1900 6418 650f 6417 650f 641f 650f  e...d.e.d.e.d.e.
-000000e0: 641a 6401 660e 6420 6421 8404 5a13 6422  d.d.f.d d!..Z.d"
-000000f0: 6502 6a0e 6417 650f 6418 650f 6419 6510  e.j.d.e.d.e.d.e.
-00000100: 6423 6502 6a0e 6424 6510 641f 650f 641a  d#e.j.d$e.d.e.d.
-00000110: 6401 6610 6425 6426 8404 5a14 6401 5300  d.f.d%d&..Z.d.S.
-00000120: 2927 e900 0000 004e 2901 da09 6d79 5f6f  )'.....N)...my_o
-00000130: 7574 7075 7429 01da 0b74 6167 5f69 6e5f  utput)...tag_in_
-00000140: 7479 7065 a901 da0c 7072 6f63 6573 735f  type....process_
-00000150: 6c69 7374 7a0c 4368 6563 6b20 4368 616e  listz.Check Chan
-00000160: 6765 5a03 5441 507a 0c46 6f63 7573 2043  geZ.TAPz.Focus C
-00000170: 6861 6e67 657a 0d49 7465 6d20 5365 6c65  hangez.Item Sele
-00000180: 6374 6564 da03 4b65 795a 044c 696e 6b7a  cted..KeyZ.Linkz
-00000190: 084c 4f4e 4720 5441 50da 034d 6170 7a08  .LONG TAP..Mapz.
-000001a0: 4c6f 6e67 204d 6170 7a09 5061 6765 204c  Long Mapz.Page L
-000001b0: 6f61 645a 0653 5452 4f4b 457a 0e56 616c  oadZ.STROKEz.Val
-000001c0: 7565 2053 656c 6563 7465 645a 0556 6964  ue SelectedZ.Vid
-000001d0: 656f 7a08 4954 454d 2054 4150 7a0d 4954  eoz.ITEM TAPz.IT
-000001e0: 454d 204c 4f4e 4720 5441 5029 0fda 0f63  EM LONG TAP)...c
-000001f0: 6865 636b 6368 616e 6765 5461 736b da09  heckchangeTask..
-00000200: 636c 6963 6b54 6173 6bda 0f66 6f63 7573  clickTask..focus
-00000210: 6368 616e 6765 5461 736b da10 6974 656d  changeTask..item
-00000220: 7365 6c65 6374 6564 5461 736b da07 6b65  selectedTask..ke
-00000230: 7954 6173 6bda 0d6c 696e 6b63 6c69 636b  yTask..linkclick
-00000240: 5461 736b da0d 6c6f 6e67 636c 6963 6b54  Task..longclickT
-00000250: 6173 6bda 0c6d 6170 636c 6963 6b54 6173  ask..mapclickTas
-00000260: 6bda 106d 6170 6c6f 6e67 636c 6963 6b54  k..maplongclickT
-00000270: 6173 6bda 0e70 6167 656c 6f61 6465 6454  ask..pageloadedT
-00000280: 6173 6bda 0a73 7472 6f6b 6554 6173 6bda  ask..strokeTask.
-00000290: 1176 616c 7565 7365 6c65 6374 6564 5461  .valueselectedTa
-000002a0: 736b da09 7669 6465 6f54 6173 6bda 0d69  sk..videoTask..i
-000002b0: 7465 6d63 6c69 636b 5461 736b da11 6974  temclickTask..it
-000002c0: 656d 6c6f 6e67 636c 6963 6b54 6173 6b29  emlongclickTask)
-000002d0: 07da 0563 6461 7465 da05 6564 6174 655a  ...cdate..edateZ
-000002e0: 0a68 6569 6768 744c 616e 645a 0a68 6569  .heightLandZ.hei
-000002f0: 6768 7450 6f72 74da 036e 6d65 5a09 7769  ghtPort..nmeZ.wi
-00000300: 6474 684c 616e 645a 0977 6964 7468 506f  dthLandZ.widthPo
-00000310: 7274 da05 6368 696c 64da 0863 6f6c 6f72  rt..child..color
-00000320: 6d61 70da 0c70 726f 6772 616d 5f61 7267  map..program_arg
-00000330: 73da 0b6f 7574 7075 745f 6c69 7374 da06  s..output_list..
-00000340: 7265 7475 726e 6304 0000 0000 0000 0000  returnc.........
-00000350: 0000 0007 0000 000d 0000 0043 0000 0073  ...........C...s
-00000360: 5400 0000 7c00 6a00 a001 6401 a101 7d04  T...|.j...d...}.
-00000370: 7c00 a002 6402 a101 7d05 7c05 6a03 7d06  |...d...}.|.j.}.
-00000380: 7404 7c01 7c02 7c03 6403 6404 7c01 6405  t.|.|.|.d.d.|.d.
-00000390: 1900 9b00 7c02 6406 1900 9b00 6407 7c04  ....|.d.....d.|.
-000003a0: 6408 1900 9b00 6409 7c06 9b00 640a 9d08  d.....d.|...d...
-000003b0: 8305 0100 640b 5300 290c 6129 0100 000a  ....d.S.).a)....
-000003c0: 2020 2020 476f 2074 6872 6f75 6768 2053      Go through S
-000003d0: 6365 6e65 2773 203c 7878 7845 6c65 6d65  cene's <xxxEleme
-000003e0: 6e74 3e20 7461 6773 2061 6e64 206f 7574  nt> tags and out
-000003f0: 7075 7420 7468 656d 0a20 2020 2020 2020  put them.       
-00000400: 203a 7061 7261 6d20 6368 696c 643a 2070   :param child: p
-00000410: 6f69 6e74 6572 2074 6f20 273c 7878 7845  ointer to '<xxxE
-00000420: 6c65 6d65 6e74 2720 5363 656e 6520 786d  lement' Scene xm
-00000430: 6c20 7374 6174 656d 656e 740a 2020 2020  l statement.    
-00000440: 2020 2020 3a70 6172 616d 2063 6f6c 6f72      :param color
-00000450: 6d61 703a 2063 6f6c 6f72 7320 746f 2075  map: colors to u
-00000460: 7365 0a20 2020 2020 2020 203a 7061 7261  se.        :para
-00000470: 6d20 7072 6f67 7261 6d5f 6172 6773 3a20  m program_args: 
-00000480: 7072 6f67 7261 6d20 7275 6e74 696d 6520  program runtime 
-00000490: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
-000004a0: 2020 3a70 6172 616d 206f 7574 7075 745f    :param output_
-000004b0: 6c69 7374 3a20 6c69 7374 206f 6620 6f75  list: list of ou
-000004c0: 7470 7574 206c 696e 6573 0a20 2020 2020  tput lines.     
-000004d0: 2020 203a 7265 7475 726e 3a20 6e6f 7468     :return: noth
-000004e0: 696e 670a 2020 2020 da07 456c 656d 656e  ing.    ..Elemen
-000004f0: 74da 0353 7472 e904 0000 007a 133c 7370  t..Str.....z.<sp
-00000500: 616e 2073 7479 6c65 3d22 636f 6c6f 723a  an style="color:
-00000510: da0b 7363 656e 655f 636f 6c6f 72da 0b66  ..scene_color..f
-00000520: 6f6e 745f 746f 5f75 7365 7a1c 3e26 6e62  ont_to_usez.>&nb
-00000530: 7370 3b26 6e62 7370 3b26 6e62 7370 3b45  sp;&nbsp;&nbsp;E
-00000540: 6c65 6d65 6e74 3a20 7201 0000 007a 0720  lement: r....z. 
-00000550: 6e61 6d65 6420 7a07 3c2f 7370 616e 3e4e  named z.</span>N
-00000560: 2905 da03 7461 67da 0573 706c 6974 da04  )...tag..split..
-00000570: 6669 6e64 da04 7465 7874 7202 0000 0029  find..textr....)
-00000580: 0772 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000590: 721d 0000 005a 0c65 6c65 6d65 6e74 5f74  r....Z.element_t
-000005a0: 7970 655a 106e 616d 655f 786d 6c5f 656c  ypeZ.name_xml_el
-000005b0: 656d 656e 745a 0c65 6c65 6d65 6e74 5f6e  ementZ.element_n
-000005c0: 616d 65a9 0072 2800 0000 fa75 2f55 7365  ame..r(....u/Use
-000005d0: 7273 2f6d 696b 7275 6269 6e2f 4c69 6272  rs/mikrubin/Libr
-000005e0: 6172 792f 436c 6f75 6453 746f 7261 6765  ary/CloudStorage
-000005f0: 2f47 6f6f 676c 6544 7269 7665 2d6d 696b  /GoogleDrive-mik
-00000600: 7275 6269 6e40 676d 6169 6c2e 636f 6d2f  rubin@gmail.com/
-00000610: 4d79 2044 7269 7665 2f50 7974 686f 6e2f  My Drive/Python/
-00000620: 6d61 7074 6173 6b65 722f 6d61 7074 6173  maptasker/maptas
-00000630: 6b65 722f 7372 632f 7363 656e 6573 2e70  ker/src/scenes.p
-00000640: 79da 1267 6574 5f73 6365 6e65 5f65 6c65  y..get_scene_ele
-00000650: 6d65 6e74 7331 0000 0073 2600 0000 0c0b  ments1...s&.....
-00000660: 0a01 0601 0201 0201 0201 0201 0201 0202  ................
-00000670: 0601 02ff 0601 04ff 0602 04fe 0202 06fe  ................
-00000680: 04fa 040c 722a 0000 00da 086d 795f 7363  ....r*.....my_sc
-00000690: 656e 65da 0b74 6173 6b73 5f66 6f75 6e64  ene..tasks_found
-000006a0: da10 616c 6c5f 7461 736b 6572 5f69 7465  ..all_tasker_ite
-000006b0: 6d73 6306 0000 0000 0000 0000 0000 000e  msc.............
-000006c0: 0000 000b 0000 0043 0000 0073 1401 0000  .......C...s....
-000006d0: 6401 6402 6c00 6d01 7d06 0100 7c05 6403  d.d.l.m.}...|.d.
-000006e0: 1900 7c00 1900 4400 5d7b 7d07 7c07 6a02  ..|...D.]{}.|.j.
-000006f0: 7403 7600 7214 710c 7c07 6a02 6404 6b02  t.v.r.q.|.j.d.k.
-00000700: 721c 0100 6405 5300 7404 7c07 6a02 6406  r...d.S.t.|.j.d.
-00000710: 8302 7287 7c03 6407 1900 6408 6b02 722f  ..r.|.d...d.k.r/
-00000720: 7405 7c07 7c04 7c03 7c01 8304 0100 7c07  t.|.|.|.|.....|.
-00000730: 4400 5d55 7d08 7404 7c08 6a02 6409 8302  D.]U}.t.|.j.d...
-00000740: 727f 7c08 6a06 6701 7d09 640a 7c09 6401  r.|.j.g.}.d.|.d.
-00000750: 1900 7601 727d 7407 7c04 7c03 7c01 640b  ..v.r}t.|.|.|.d.
-00000760: 640c 8305 0100 7408 a009 7c08 6a06 7c02  d.....t...|.j.|.
-00000770: 7c09 640c 7c05 640d 1900 a105 5c02 7d0a  |.d.|.d.....\.}.
-00000780: 7d0b 7c08 6a06 6701 7d09 640e 7d0c 640f  }.|.j.g.}.d.}.d.
-00000790: 740a 7c08 6a02 1900 9b00 7c0c 9b00 9d03  t.|.j.....|.....
-000007a0: 7d0d 7c06 7c0d 7c01 7c09 7c0a 7c02 7c03  }.|.|.|.|.|.|.|.
-000007b0: 7c04 7c05 8308 0100 7407 7c04 7c03 7c01  |.|.....t.|.|.|.
-000007c0: 640b 640c 8305 0100 7131 0100 6e08 7c08  d.d.....q1..n.|.
-000007d0: 6a02 6410 6b02 7286 0100 6e01 7131 710c  j.d.k.r...n.q1q.
-000007e0: 6405 5300 2911 615c 0100 000a 0a20 2020  d.S.).a\.....   
-000007f0: 203a 7061 7261 6d20 6d79 5f73 6365 6e65   :param my_scene
-00000800: 3a20 6e61 6d65 206f 6620 5363 656e 6520  : name of Scene 
-00000810: 746f 2070 726f 6365 7373 0a20 2020 203a  to process.    :
-00000820: 7061 7261 6d20 6f75 7470 7574 5f6c 6973  param output_lis
-00000830: 743a 206c 6973 7420 6f66 206f 7574 7075  t: list of outpu
-00000840: 7420 6c69 6e65 730a 2020 2020 3a70 6172  t lines.    :par
-00000850: 616d 2074 6173 6b73 5f66 6f75 6e64 3a20  am tasks_found: 
-00000860: 6c69 7374 206f 6620 5461 736b 7320 666f  list of Tasks fo
-00000870: 756e 6420 736f 2066 6172 0a20 2020 203a  und so far.    :
-00000880: 7061 7261 6d20 7072 6f67 7261 6d5f 6172  param program_ar
-00000890: 6773 3a20 6469 6374 696f 6e61 7279 206f  gs: dictionary o
-000008a0: 6620 7275 6e74 696d 6520 6172 6775 6d65  f runtime argume
-000008b0: 6e74 730a 2020 2020 3a70 6172 616d 2063  nts.    :param c
-000008c0: 6f6c 6f72 6d61 703a 2064 6963 7469 6f6e  olormap: diction
-000008d0: 6172 7920 6f66 2063 6f6c 6f72 7320 746f  ary of colors to
-000008e0: 2075 7365 0a20 2020 203a 7061 7261 6d20   use.    :param 
-000008f0: 616c 6c5f 7461 736b 6572 5f69 7465 6d73  all_tasker_items
-00000900: 3a20 6469 6374 696f 6e61 7279 206f 6620  : dictionary of 
-00000910: 5461 736b 6572 2050 726f 6a65 6374 732f  Tasker Projects/
-00000920: 5072 6f66 696c 6573 2f54 6173 6b73 2f53  Profiles/Tasks/S
-00000930: 6365 6e65 730a 2020 2020 3a72 6574 7572  cenes.    :retur
-00000940: 6e3a 0a20 2020 2072 0100 0000 7204 0000  n:.    r....r...
-00000950: 00da 0a61 6c6c 5f73 6365 6e65 735a 1150  ...all_scenesZ.P
-00000960: 726f 7065 7274 6965 7345 6c65 6d65 6e74  ropertiesElement
-00000970: 4e54 da14 6469 7370 6c61 795f 6465 7461  NT..display_deta
-00000980: 696c 5f6c 6576 656c e903 0000 0046 fa01  il_level.....F..
-00000990: 2de9 0100 0000 da00 da09 616c 6c5f 7461  -.........all_ta
-000009a0: 736b 737a 0f26 6e62 7370 3b26 6e62 7370  sksz.&nbsp;&nbsp
-000009b0: 3b49 443a 7a16 266e 6273 703b 2623 3435  ;ID:z.&nbsp;&#45
-000009c0: 3b26 2334 353b 5461 736b 3a20 7220 0000  ;&#45;Task: r ..
-000009d0: 0029 0bda 166d 6170 7461 736b 6572 2e73  .)...maptasker.s
-000009e0: 7263 2e70 726f 636c 6973 7472 0500 0000  rc.proclistr....
-000009f0: 7224 0000 00da 1453 4345 4e45 5f54 4147  r$.....SCENE_TAG
-00000a00: 535f 544f 5f49 474e 4f52 4572 0300 0000  S_TO_IGNOREr....
-00000a10: 722a 0000 0072 2700 0000 7202 0000 00da  r*...r'...r.....
-00000a20: 0574 6173 6b73 da0d 6765 745f 7461 736b  .tasks..get_task
-00000a30: 5f6e 616d 65da 1053 4345 4e45 5f54 4153  _name..SCENE_TAS
-00000a40: 4b5f 5459 5045 5329 0e72 2b00 0000 721d  K_TYPES).r+...r.
-00000a50: 0000 0072 2c00 0000 721c 0000 0072 1b00  ...r,...r....r..
-00000a60: 0000 722d 0000 0072 0500 0000 721a 0000  ..r-...r....r...
-00000a70: 005a 0973 7562 5f63 6869 6c64 5a0e 7465  .Z.sub_childZ.te
-00000a80: 6d70 5f74 6173 6b5f 6c69 7374 5a0c 7461  mp_task_listZ.ta
-00000a90: 736b 5f65 6c65 6d65 6e74 5a0c 6e61 6d65  sk_elementZ.name
-00000aa0: 5f6f 665f 7461 736b da05 6578 7472 61da  _of_task..extra.
-00000ab0: 0974 6173 6b5f 7479 7065 7228 0000 0072  .task_typer(...r
-00000ac0: 2800 0000 7229 0000 00da 0d70 726f 6365  (...r).....proce
-00000ad0: 7373 5f73 6365 6e65 4e00 0000 735c 0000  ss_sceneN...s\..
-00000ae0: 000c 1310 030a 0102 010a 0106 010c 010c  ................
-00000af0: 020e 0108 010c 0208 020c 0210 0104 0104  ................
-00000b00: 0102 0102 0102 0106 0108 fb08 0804 0102  ................
-00000b10: 0208 0102 ff02 0104 ff02 ff02 0502 0102  ................
-00000b20: 0102 0102 0102 0102 0102 0102 0104 f812  ................
-00000b30: 0a04 020a 0104 0102 ff02 8004 0272 3c00  .............r<.
-00000b40: 0000 da07 7072 6f6a 6563 74da 106f 7572  ....project..our
-00000b50: 5f74 6173 6b5f 656c 656d 656e 74da 0b66  _task_element..f
-00000b60: 6f75 6e64 5f74 6173 6b73 6307 0000 0000  ound_tasksc.....
-00000b70: 0000 0000 0000 0009 0000 0009 0000 0043  ...............C
-00000b80: 0000 0073 9a00 0000 6401 7d07 7400 a001  ...s....d.}.t...
-00000b90: 7402 a101 8f0e 0100 7c00 a003 6402 a101  t.......|...d...
-00000ba0: 6a04 7d07 5700 6401 0400 0400 8303 0100  j.}.W.d.........
-00000bb0: 6e08 3100 7318 7701 0100 0100 0100 5900  n.1.s.w.......Y.
-00000bc0: 0100 7c07 6401 7501 724b 7c07 a005 6403  ..|.d.u.rK|...d.
-00000bd0: a101 7d08 7c03 6404 1900 6405 6b02 7234  ..}.|.d...d.k.r4
-00000be0: 7406 7c01 7c02 7c03 6406 6407 8305 0100  t.|.|.|.d.d.....
-00000bf0: 7c08 6408 1900 724b 7407 6409 7c03 7c08  |.d...rKt.d.|.|.
-00000c00: 7c04 7c05 7c02 7c01 7c06 8308 0100 7406  |.|.|.|.|.....t.
-00000c10: 7c01 7c02 7c03 640a 6407 8305 0100 6401  |.|.|.d.d.....d.
-00000c20: 5300 290b 6101 0200 000a 2020 2020 476f  S.).a.....    Go
-00000c30: 2074 6872 6f75 6768 2061 6c6c 2053 6365   through all Sce
-00000c40: 6e65 7320 666f 7220 5072 6f6a 6563 742c  nes for Project,
-00000c50: 2067 6574 2074 6865 6972 2064 6574 6169   get their detai
-00000c60: 6c20 616e 6420 6f75 7470 7574 2069 740a  l and output it.
-00000c70: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-00000c80: 726f 6a65 6374 3a20 786d 6c20 656c 656d  roject: xml elem
-00000c90: 656e 7420 6f66 2050 726f 6a65 6374 2077  ent of Project w
-00000ca0: 6520 6172 6520 7072 6f63 6573 7369 6e67  e are processing
+00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 0100  Z...d.d.l.m.Z...
+00000080: 6406 6407 6408 6409 640a 640b 640c 640d  d.d.d.d.d.d.d.d.
+00000090: 640e 640f 6410 6411 6412 6413 6414 6415  d.d.d.d.d.d.d.d.
+000000a0: 9c0f 5a0e 6700 6416 a201 5a0f 6417 6502  ..Z.g.d...Z.d.e.
+000000b0: 6a10 6a11 6418 6512 6419 6512 641a 6513  j.j.d.e.d.e.d.e.
+000000c0: 641b 6401 660a 641c 641d 8404 5a14 641e  d.d.f.d.d...Z.d.
+000000d0: 6515 641a 6513 6515 1900 641f 6513 6515  e.d.e.e...d.e.e.
+000000e0: 1900 6419 6512 6418 6512 6420 6512 641b  ..d.e.d.e.d e.d.
+000000f0: 6401 660e 6421 6422 8404 5a16 6423 6502  d.f.d!d"..Z.d#e.
+00000100: 6a10 6a11 6418 6512 6419 6512 641a 6513  j.j.d.e.d.e.d.e.
+00000110: 6424 6502 6a10 6a11 6425 6513 6420 6512  d$e.j.j.d%e.d e.
+00000120: 641b 6401 6610 6426 6427 8404 5a17 6401  d.d.f.d&d'..Z.d.
+00000130: 5300 2928 e900 0000 004e 2901 da09 6d79  S.)(.....N)...my
+00000140: 5f6f 7574 7075 7429 01da 0b74 6167 5f69  _output)...tag_i
+00000150: 6e5f 7479 7065 a901 da0c 7072 6f63 6573  n_type....proces
+00000160: 735f 6c69 7374 2901 da0b 666f 726d 6174  s_list)...format
+00000170: 5f68 746d 6c7a 0c43 6865 636b 2043 6861  _htmlz.Check Cha
+00000180: 6e67 655a 0354 4150 7a0c 466f 6375 7320  ngeZ.TAPz.Focus 
+00000190: 4368 616e 6765 7a0d 4974 656d 2053 656c  Changez.Item Sel
+000001a0: 6563 7465 64da 034b 6579 5a04 4c69 6e6b  ected..KeyZ.Link
+000001b0: 7a08 4c4f 4e47 2054 4150 da03 4d61 707a  z.LONG TAP..Mapz
+000001c0: 084c 6f6e 6720 4d61 707a 0950 6167 6520  .Long Mapz.Page 
+000001d0: 4c6f 6164 5a06 5354 524f 4b45 7a0e 5661  LoadZ.STROKEz.Va
+000001e0: 6c75 6520 5365 6c65 6374 6564 5a05 5669  lue SelectedZ.Vi
+000001f0: 6465 6f7a 0849 5445 4d20 5441 507a 0d49  deoz.ITEM TAPz.I
+00000200: 5445 4d20 4c4f 4e47 2054 4150 290f da0f  TEM LONG TAP)...
+00000210: 6368 6563 6b63 6861 6e67 6554 6173 6bda  checkchangeTask.
+00000220: 0963 6c69 636b 5461 736b da0f 666f 6375  .clickTask..focu
+00000230: 7363 6861 6e67 6554 6173 6bda 1069 7465  schangeTask..ite
+00000240: 6d73 656c 6563 7465 6454 6173 6bda 076b  mselectedTask..k
+00000250: 6579 5461 736b da0d 6c69 6e6b 636c 6963  eyTask..linkclic
+00000260: 6b54 6173 6bda 0d6c 6f6e 6763 6c69 636b  kTask..longclick
+00000270: 5461 736b da0c 6d61 7063 6c69 636b 5461  Task..mapclickTa
+00000280: 736b da10 6d61 706c 6f6e 6763 6c69 636b  sk..maplongclick
+00000290: 5461 736b da0e 7061 6765 6c6f 6164 6564  Task..pageloaded
+000002a0: 5461 736b da0a 7374 726f 6b65 5461 736b  Task..strokeTask
+000002b0: da11 7661 6c75 6573 656c 6563 7465 6454  ..valueselectedT
+000002c0: 6173 6bda 0976 6964 656f 5461 736b da0d  ask..videoTask..
+000002d0: 6974 656d 636c 6963 6b54 6173 6bda 1169  itemclickTask..i
+000002e0: 7465 6d6c 6f6e 6763 6c69 636b 5461 736b  temlongclickTask
+000002f0: 2907 da05 6364 6174 65da 0565 6461 7465  )...cdate..edate
+00000300: 5a0a 6865 6967 6874 4c61 6e64 5a0a 6865  Z.heightLandZ.he
+00000310: 6967 6874 506f 7274 da03 6e6d 655a 0977  ightPort..nmeZ.w
+00000320: 6964 7468 4c61 6e64 5a09 7769 6474 6850  idthLandZ.widthP
+00000330: 6f72 74da 0563 6869 6c64 da08 636f 6c6f  ort..child..colo
+00000340: 726d 6170 da0c 7072 6f67 7261 6d5f 6172  rmap..program_ar
+00000350: 6773 da0b 6f75 7470 7574 5f6c 6973 74da  gs..output_list.
+00000360: 0672 6574 7572 6e63 0400 0000 0000 0000  .returnc........
+00000370: 0000 0000 0700 0000 0d00 0000 4300 0000  ............C...
+00000380: 734c 0000 007c 006a 00a0 0164 01a1 017d  sL...|.j...d...}
+00000390: 047c 00a0 0264 02a1 017d 057c 056a 037d  .|...d...}.|.j.}
+000003a0: 0674 047c 017c 027c 0364 0374 057c 0164  .t.|.|.|.d.t.|.d
+000003b0: 0464 0564 067c 0464 0719 009b 0064 087c  .d.d.|.d.....d.|
+000003c0: 069b 009d 0464 0983 0583 0501 0064 0a53  .....d.......d.S
+000003d0: 0029 0b61 2901 0000 0a20 2020 2047 6f20  .).a)....    Go 
+000003e0: 7468 726f 7567 6820 5363 656e 6527 7320  through Scene's 
+000003f0: 3c78 7878 456c 656d 656e 743e 2074 6167  <xxxElement> tag
+00000400: 7320 616e 6420 6f75 7470 7574 2074 6865  s and output the
+00000410: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
+00000420: 2063 6869 6c64 3a20 706f 696e 7465 7220   child: pointer 
+00000430: 746f 2027 3c78 7878 456c 656d 656e 7427  to '<xxxElement'
+00000440: 2053 6365 6e65 2078 6d6c 2073 7461 7465   Scene xml state
+00000450: 6d65 6e74 0a20 2020 2020 2020 203a 7061  ment.        :pa
+00000460: 7261 6d20 636f 6c6f 726d 6170 3a20 636f  ram colormap: co
+00000470: 6c6f 7273 2074 6f20 7573 650a 2020 2020  lors to use.    
+00000480: 2020 2020 3a70 6172 616d 2070 726f 6772      :param progr
+00000490: 616d 5f61 7267 733a 2070 726f 6772 616d  am_args: program
+000004a0: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
+000004b0: 7473 0a20 2020 2020 2020 203a 7061 7261  ts.        :para
+000004c0: 6d20 6f75 7470 7574 5f6c 6973 743a 206c  m output_list: l
+000004d0: 6973 7420 6f66 206f 7574 7075 7420 6c69  ist of output li
+000004e0: 6e65 730a 2020 2020 2020 2020 3a72 6574  nes.        :ret
+000004f0: 7572 6e3a 206e 6f74 6869 6e67 0a20 2020  urn: nothing.   
+00000500: 20da 0745 6c65 6d65 6e74 da03 5374 72e9   ..Element..Str.
+00000510: 0400 0000 da0b 7363 656e 655f 636f 6c6f  ......scene_colo
+00000520: 72da 007a 1b26 6e62 7370 3b26 6e62 7370  r..z.&nbsp;&nbsp
+00000530: 3b26 6e62 7370 3b45 6c65 6d65 6e74 3a20  ;&nbsp;Element: 
+00000540: 7201 0000 007a 0720 6e61 6d65 6420 544e  r....z. named TN
+00000550: 2906 da03 7461 67da 0573 706c 6974 da04  )...tag..split..
+00000560: 6669 6e64 da04 7465 7874 7202 0000 0072  find..textr....r
+00000570: 0600 0000 2907 721b 0000 0072 1c00 0000  ....).r....r....
+00000580: 721d 0000 0072 1e00 0000 5a0c 656c 656d  r....r....Z.elem
+00000590: 656e 745f 7479 7065 5a10 6e61 6d65 5f78  ent_typeZ.name_x
+000005a0: 6d6c 5f65 6c65 6d65 6e74 da0c 656c 656d  ml_element..elem
+000005b0: 656e 745f 6e61 6d65 a900 722a 0000 00fa  ent_name..r*....
+000005c0: 752f 5573 6572 732f 6d69 6b72 7562 696e  u/Users/mikrubin
+000005d0: 2f4c 6962 7261 7279 2f43 6c6f 7564 5374  /Library/CloudSt
+000005e0: 6f72 6167 652f 476f 6f67 6c65 4472 6976  orage/GoogleDriv
+000005f0: 652d 6d69 6b72 7562 696e 4067 6d61 696c  e-mikrubin@gmail
+00000600: 2e63 6f6d 2f4d 7920 4472 6976 652f 5079  .com/My Drive/Py
+00000610: 7468 6f6e 2f6d 6170 7461 736b 6572 2f6d  thon/maptasker/m
+00000620: 6170 7461 736b 6572 2f73 7263 2f73 6365  aptasker/src/sce
+00000630: 6e65 732e 7079 da12 6765 745f 7363 656e  nes.py..get_scen
+00000640: 655f 656c 656d 656e 7473 3200 0000 7322  e_elements2...s"
+00000650: 0000 000c 0e0a 0106 0102 0102 0102 0102  ................
+00000660: 0102 0102 0102 0102 0102 0112 0102 0102  ................
+00000670: fb04 fb04 0e72 2c00 0000 da08 6d79 5f73  .....r,.....my_s
+00000680: 6365 6e65 da0b 7461 736b 735f 666f 756e  cene..tasks_foun
+00000690: 64da 1061 6c6c 5f74 6173 6b65 725f 6974  d..all_tasker_it
+000006a0: 656d 7363 0600 0000 0000 0000 0000 0000  emsc............
+000006b0: 0e00 0000 0b00 0000 4300 0000 7314 0100  ........C...s...
+000006c0: 0064 0164 026c 006d 017d 0601 007c 0564  .d.d.l.m.}...|.d
+000006d0: 0319 007c 0019 0044 005d 7b7d 077c 076a  ...|...D.]{}.|.j
+000006e0: 0274 0376 0072 1471 0c7c 076a 0264 046b  .t.v.r.q.|.j.d.k
+000006f0: 0272 1c01 0064 0553 0074 047c 076a 0264  .r...d.S.t.|.j.d
+00000700: 0683 0272 877c 0364 0719 0064 086b 0272  ...r.|.d...d.k.r
+00000710: 2f74 057c 077c 047c 037c 0183 0401 007c  /t.|.|.|.|.....|
+00000720: 0744 005d 557d 0874 047c 086a 0264 0983  .D.]U}.t.|.j.d..
+00000730: 0272 7f7c 086a 0667 017d 0964 0a7c 0964  .r.|.j.g.}.d.|.d
+00000740: 0119 0076 0172 7d74 077c 047c 037c 0164  ...v.r}t.|.|.|.d
+00000750: 0b64 0c83 0501 0074 08a0 097c 086a 067c  .d.....t...|.j.|
+00000760: 027c 0964 0c7c 0564 0d19 00a1 055c 027d  .|.d.|.d.....\.}
+00000770: 0a7d 0b7c 086a 0667 017d 0964 0e7d 0c64  .}.|.j.g.}.d.}.d
+00000780: 0f74 0a7c 086a 0219 009b 007c 0c9b 009d  .t.|.j.....|....
+00000790: 037d 0d7c 067c 0d7c 017c 097c 0a7c 027c  .}.|.|.|.|.|.|.|
+000007a0: 037c 047c 0583 0801 0074 077c 047c 037c  .|.|.....t.|.|.|
+000007b0: 0164 0b64 0c83 0501 0071 3101 006e 087c  .d.d.....q1..n.|
+000007c0: 086a 0264 106b 0272 8601 006e 0171 3171  .j.d.k.r...n.q1q
+000007d0: 0c64 0553 0029 1161 a901 0000 0a20 2020  .d.S.).a.....   
+000007e0: 2050 726f 6365 7373 2074 6865 2050 726f   Process the Pro
+000007f0: 6a65 6374 2773 2053 6365 6e65 2873 292c  ject's Scene(s),
+00000800: 206f 6e65 2061 7420 6120 7469 6d65 0a20   one at a time. 
+00000810: 2020 2020 2020 203a 7061 7261 6d20 6d79         :param my
+00000820: 5f73 6365 6e65 3a20 6e61 6d65 206f 6620  _scene: name of 
+00000830: 5363 656e 6520 746f 2070 726f 6365 7373  Scene to process
+00000840: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000850: 6f75 7470 7574 5f6c 6973 743a 206c 6973  output_list: lis
+00000860: 7420 6f66 206f 7574 7075 7420 6c69 6e65  t of output line
+00000870: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
+00000880: 2074 6173 6b73 5f66 6f75 6e64 3a20 6c69   tasks_found: li
+00000890: 7374 206f 6620 5461 736b 7320 666f 756e  st of Tasks foun
+000008a0: 6420 736f 2066 6172 0a20 2020 2020 2020  d so far.       
+000008b0: 203a 7061 7261 6d20 7072 6f67 7261 6d5f   :param program_
+000008c0: 6172 6773 3a20 6469 6374 696f 6e61 7279  args: dictionary
+000008d0: 206f 6620 7275 6e74 696d 6520 6172 6775   of runtime argu
+000008e0: 6d65 6e74 730a 2020 2020 2020 2020 3a70  ments.        :p
+000008f0: 6172 616d 2063 6f6c 6f72 6d61 703a 2064  aram colormap: d
+00000900: 6963 7469 6f6e 6172 7920 6f66 2063 6f6c  ictionary of col
+00000910: 6f72 7320 746f 2075 7365 0a20 2020 2020  ors to use.     
+00000920: 2020 203a 7061 7261 6d20 616c 6c5f 7461     :param all_ta
+00000930: 736b 6572 5f69 7465 6d73 3a20 6469 6374  sker_items: dict
+00000940: 696f 6e61 7279 206f 6620 5461 736b 6572  ionary of Tasker
+00000950: 2050 726f 6a65 6374 732f 5072 6f66 696c   Projects/Profil
+00000960: 6573 2f54 6173 6b73 2f53 6365 6e65 730a  es/Tasks/Scenes.
+00000970: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00000980: 0a20 2020 2072 0100 0000 7204 0000 00da  .    r....r.....
+00000990: 0a61 6c6c 5f73 6365 6e65 735a 1150 726f  .all_scenesZ.Pro
+000009a0: 7065 7274 6965 7345 6c65 6d65 6e74 4e54  pertiesElementNT
+000009b0: da14 6469 7370 6c61 795f 6465 7461 696c  ..display_detail
+000009c0: 5f6c 6576 656c e903 0000 0046 fa01 2de9  _level.....F..-.
+000009d0: 0100 0000 7224 0000 00da 0961 6c6c 5f74  ....r$.....all_t
+000009e0: 6173 6b73 7a0f 266e 6273 703b 266e 6273  asksz.&nbsp;&nbs
+000009f0: 703b 4944 3a7a 1626 6e62 7370 3b26 2334  p;ID:z.&nbsp;&#4
+00000a00: 353b 2623 3435 3b54 6173 6b3a 2072 2100  5;&#45;Task: r!.
+00000a10: 0000 290b da16 6d61 7074 6173 6b65 722e  ..)...maptasker.
+00000a20: 7372 632e 7072 6f63 6c69 7374 7205 0000  src.proclistr...
+00000a30: 0072 2500 0000 da14 5343 454e 455f 5441  .r%.....SCENE_TA
+00000a40: 4753 5f54 4f5f 4947 4e4f 5245 7203 0000  GS_TO_IGNOREr...
+00000a50: 0072 2c00 0000 7228 0000 0072 0200 0000  .r,...r(...r....
+00000a60: da05 7461 736b 73da 0d67 6574 5f74 6173  ..tasks..get_tas
+00000a70: 6b5f 6e61 6d65 da10 5343 454e 455f 5441  k_name..SCENE_TA
+00000a80: 534b 5f54 5950 4553 290e 722d 0000 0072  SK_TYPES).r-...r
+00000a90: 1e00 0000 722e 0000 0072 1d00 0000 721c  ....r....r....r.
+00000aa0: 0000 0072 2f00 0000 7205 0000 0072 1b00  ...r/...r....r..
+00000ab0: 0000 5a09 7375 625f 6368 696c 645a 0e74  ..Z.sub_childZ.t
+00000ac0: 656d 705f 7461 736b 5f6c 6973 745a 0c74  emp_task_listZ.t
+00000ad0: 6173 6b5f 656c 656d 656e 745a 0c6e 616d  ask_elementZ.nam
+00000ae0: 655f 6f66 5f74 6173 6bda 0565 7874 7261  e_of_task..extra
+00000af0: da09 7461 736b 5f74 7970 6572 2a00 0000  ..task_typer*...
+00000b00: 722a 0000 0072 2b00 0000 da0d 7072 6f63  r*...r+.....proc
+00000b10: 6573 735f 7363 656e 6554 0000 0073 5c00  ess_sceneT...s\.
+00000b20: 0000 0c13 1003 0a01 0201 0a01 0601 0c01  ................
+00000b30: 0c02 0e01 0801 0c02 0802 0c02 1001 0401  ................
+00000b40: 0401 0201 0201 0201 0601 08fb 0808 0401  ................
+00000b50: 0202 0801 02ff 0201 04ff 02ff 0205 0201  ................
+00000b60: 0201 0201 0201 0201 0201 0201 0201 04f8  ................
+00000b70: 120a 0402 0a01 0401 02ff 0280 0402 723d  ..............r=
+00000b80: 0000 00da 0770 726f 6a65 6374 da10 6f75  .....project..ou
+00000b90: 725f 7461 736b 5f65 6c65 6d65 6e74 da0b  r_task_element..
+00000ba0: 666f 756e 645f 7461 736b 7363 0700 0000  found_tasksc....
+00000bb0: 0000 0000 0000 0000 0900 0000 0900 0000  ................
+00000bc0: 4300 0000 739a 0000 0064 017d 0774 00a0  C...s....d.}.t..
+00000bd0: 0174 02a1 018f 0e01 007c 00a0 0364 02a1  .t.......|...d..
+00000be0: 016a 047d 0757 0064 0104 0004 0083 0301  .j.}.W.d........
+00000bf0: 006e 0831 0073 1877 0101 0001 0001 0059  .n.1.s.w.......Y
+00000c00: 0001 007c 0764 0175 0172 4b7c 07a0 0564  ...|.d.u.rK|...d
+00000c10: 03a1 017d 087c 0364 0419 0064 056b 0272  ...}.|.d...d.k.r
+00000c20: 3474 067c 017c 027c 0364 0664 0783 0501  4t.|.|.|.d.d....
+00000c30: 007c 0864 0819 0072 4b74 0764 097c 037c  .|.d...rKt.d.|.|
+00000c40: 087c 047c 057c 027c 017c 0683 0801 0074  .|.|.|.|.|.....t
+00000c50: 067c 017c 027c 0364 0a64 0783 0501 0064  .|.|.|.d.d.....d
+00000c60: 0153 0029 0b61 0102 0000 0a20 2020 2047  .S.).a.....    G
+00000c70: 6f20 7468 726f 7567 6820 616c 6c20 5363  o through all Sc
+00000c80: 656e 6573 2066 6f72 2050 726f 6a65 6374  enes for Project
+00000c90: 2c20 6765 7420 7468 6569 7220 6465 7461  , get their deta
+00000ca0: 696c 2061 6e64 206f 7574 7075 7420 6974  il and output it
 00000cb0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000cc0: 636f 6c6f 726d 6170 3a20 636f 6c6f 7273  colormap: colors
-00000cd0: 2074 6f20 7573 6520 696e 206f 7574 7075   to use in outpu
-00000ce0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-00000cf0: 2070 726f 6772 616d 5f61 7267 733a 2072   program_args: r
-00000d00: 756e 7469 6d65 2061 7267 756d 656e 7473  untime arguments
-00000d10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000d20: 6f75 7470 7574 5f6c 6973 743a 206c 6973  output_list: lis
-00000d30: 7420 6f66 206f 7574 7075 7420 6c69 6e65  t of output line
-00000d40: 7320 6372 6561 7465 6420 7468 7573 2066  s created thus f
-00000d50: 6172 0a20 2020 2020 2020 203a 7061 7261  ar.        :para
-00000d60: 6d20 6f75 725f 7461 736b 5f65 6c65 6d65  m our_task_eleme
-00000d70: 6e74 3a20 786d 6c20 656c 656d 656e 7420  nt: xml element 
-00000d80: 706f 696e 7469 6e67 2074 6f20 6f75 7220  pointing to our 
-00000d90: 5461 736b 0a20 2020 2020 2020 203a 7061  Task.        :pa
-00000da0: 7261 6d20 666f 756e 645f 7461 736b 733a  ram found_tasks:
-00000db0: 206c 6973 7420 6f66 2054 6173 6b73 2066   list of Tasks f
-00000dc0: 6f75 6e64 2073 6f20 6661 720a 2020 2020  ound so far.    
-00000dd0: 2020 2020 3a70 6172 616d 2061 6c6c 5f74      :param all_t
-00000de0: 6173 6b65 725f 6974 656d 733a 2061 6c6c  asker_items: all
-00000df0: 2050 726f 6a65 6374 732f 5072 6f66 696c   Projects/Profil
-00000e00: 6573 2f54 6173 6b73 2f53 6365 6e65 730a  es/Tasks/Scenes.
-00000e10: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000e20: 206e 6164 610a 2020 2020 4e5a 0673 6365   nada.    NZ.sce
-00000e30: 6e65 73fa 012c e9ff ffff ff7a 053c 2f75  nes..,.....z.</u
-00000e40: 6c3e 7232 0000 0072 3300 0000 7201 0000  l>r2...r3...r...
-00000e50: 007a 0653 6365 6e65 3a72 2100 0000 2908  .z.Scene:r!...).
-00000e60: da0a 636f 6e74 6578 746c 6962 da08 7375  ..contextlib..su
-00000e70: 7070 7265 7373 da09 4578 6365 7074 696f  ppress..Exceptio
-00000e80: 6e72 2600 0000 7227 0000 0072 2500 0000  nr&...r'...r%...
-00000e90: 7202 0000 0072 0500 0000 2909 723d 0000  r....r....).r=..
-00000ea0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000eb0: 723e 0000 0072 3f00 0000 722d 0000 005a  r>...r?...r-...Z
-00000ec0: 0b73 6365 6e65 5f6e 616d 6573 5a0a 7363  .scene_namesZ.sc
-00000ed0: 656e 655f 6c69 7374 7228 0000 0072 2800  ene_listr(...r(.
-00000ee0: 0000 7229 0000 00da 1670 726f 6365 7373  ..r).....process
-00000ef0: 5f70 726f 6a65 6374 5f73 6365 6e65 7399  _project_scenes.
-00000f00: 0000 0073 2a00 0000 0414 0c01 0e01 1cff  ...s*...........
-00000f10: 0802 0a01 0c05 1001 0802 0201 0201 0201  ................
-00000f20: 0201 0201 0201 0201 0201 0201 04f8 100b  ................
-00000f30: 0401 7245 0000 0029 1572 4200 0000 da15  ..rE...).rB.....
-00000f40: 786d 6c2e 6574 7265 652e 456c 656d 656e  xml.etree.Elemen
-00000f50: 7454 7265 65da 0378 6d6c da13 6d61 7074  tTree..xml..mapt
-00000f60: 6173 6b65 722e 7372 632e 7461 736b 73da  asker.src.tasks.
-00000f70: 0373 7263 7237 0000 00da 156d 6170 7461  .srcr7.....mapta
-00000f80: 736b 6572 2e73 7263 2e6f 7574 7075 746c  sker.src.outputl
-00000f90: 7202 0000 00da 156d 6170 7461 736b 6572  r......maptasker
-00000fa0: 2e73 7263 2e78 6d6c 6461 7461 7203 0000  .src.xmldatar...
-00000fb0: 0072 3500 0000 7205 0000 0072 3900 0000  .r5...r....r9...
-00000fc0: 7236 0000 00da 0565 7472 6565 da04 6469  r6.....etree..di
-00000fd0: 6374 da04 6c69 7374 722a 0000 00da 0373  ct..listr*.....s
-00000fe0: 7472 723c 0000 0072 4500 0000 7228 0000  trr<...rE...r(..
-00000ff0: 0072 2800 0000 7228 0000 0072 2900 0000  .r(...r(...r)...
-00001000: da08 3c6d 6f64 756c 653e 0100 0000 7384  ..<module>....s.
-00001010: 0000 0008 0c08 0212 010c 010c 010c 0102  ................
-00001020: 0302 0102 0102 0102 0102 0102 0102 0102  ................
-00001030: 0102 0102 0102 0102 0102 0102 0106 f108  ................
-00001040: 1102 0b04 0102 ff02 0102 ff02 0102 ff02  ................
-00001050: 0102 ff02 020a fe02 1d02 0102 ff06 0202  ................
-00001060: fe06 0302 fd02 0402 fc02 0502 fb02 0602  ................
-00001070: fa02 070a f902 4b04 0102 ff02 0202 fe02  ......K.........
-00001080: 0302 fd02 0402 fc04 0502 fb02 0602 fa02  ................
-00001090: 0702 f902 080e f8                        .......
+00000cc0: 7072 6f6a 6563 743a 2078 6d6c 2065 6c65  project: xml ele
+00000cd0: 6d65 6e74 206f 6620 5072 6f6a 6563 7420  ment of Project 
+00000ce0: 7765 2061 7265 2070 726f 6365 7373 696e  we are processin
+00000cf0: 670a 2020 2020 2020 2020 3a70 6172 616d  g.        :param
+00000d00: 2063 6f6c 6f72 6d61 703a 2063 6f6c 6f72   colormap: color
+00000d10: 7320 746f 2075 7365 2069 6e20 6f75 7470  s to use in outp
+00000d20: 7574 0a20 2020 2020 2020 203a 7061 7261  ut.        :para
+00000d30: 6d20 7072 6f67 7261 6d5f 6172 6773 3a20  m program_args: 
+00000d40: 7275 6e74 696d 6520 6172 6775 6d65 6e74  runtime argument
+00000d50: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
+00000d60: 206f 7574 7075 745f 6c69 7374 3a20 6c69   output_list: li
+00000d70: 7374 206f 6620 6f75 7470 7574 206c 696e  st of output lin
+00000d80: 6573 2063 7265 6174 6564 2074 6875 7320  es created thus 
+00000d90: 6661 720a 2020 2020 2020 2020 3a70 6172  far.        :par
+00000da0: 616d 206f 7572 5f74 6173 6b5f 656c 656d  am our_task_elem
+00000db0: 656e 743a 2078 6d6c 2065 6c65 6d65 6e74  ent: xml element
+00000dc0: 2070 6f69 6e74 696e 6720 746f 206f 7572   pointing to our
+00000dd0: 2054 6173 6b0a 2020 2020 2020 2020 3a70   Task.        :p
+00000de0: 6172 616d 2066 6f75 6e64 5f74 6173 6b73  aram found_tasks
+00000df0: 3a20 6c69 7374 206f 6620 5461 736b 7320  : list of Tasks 
+00000e00: 666f 756e 6420 736f 2066 6172 0a20 2020  found so far.   
+00000e10: 2020 2020 203a 7061 7261 6d20 616c 6c5f       :param all_
+00000e20: 7461 736b 6572 5f69 7465 6d73 3a20 616c  tasker_items: al
+00000e30: 6c20 5072 6f6a 6563 7473 2f50 726f 6669  l Projects/Profi
+00000e40: 6c65 732f 5461 736b 732f 5363 656e 6573  les/Tasks/Scenes
+00000e50: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00000e60: 3a20 6e61 6461 0a20 2020 204e 5a06 7363  : nada.    NZ.sc
+00000e70: 656e 6573 fa01 2ce9 ffff ffff 7a05 3c2f  enes..,.....z.</
+00000e80: 756c 3e72 3400 0000 7224 0000 0072 0100  ul>r4...r$...r..
+00000e90: 0000 7a06 5363 656e 653a 7222 0000 0029  ..z.Scene:r"...)
+00000ea0: 08da 0a63 6f6e 7465 7874 6c69 62da 0873  ...contextlib..s
+00000eb0: 7570 7072 6573 73da 0945 7863 6570 7469  uppress..Excepti
+00000ec0: 6f6e 7227 0000 0072 2800 0000 7226 0000  onr'...r(...r&..
+00000ed0: 0072 0200 0000 7205 0000 0029 0972 3e00  .r....r....).r>.
+00000ee0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000ef0: 0072 3f00 0000 7240 0000 0072 2f00 0000  .r?...r@...r/...
+00000f00: 5a0b 7363 656e 655f 6e61 6d65 735a 0a73  Z.scene_namesZ.s
+00000f10: 6365 6e65 5f6c 6973 7472 2a00 0000 722a  cene_listr*...r*
+00000f20: 0000 0072 2b00 0000 da16 7072 6f63 6573  ...r+.....proces
+00000f30: 735f 7072 6f6a 6563 745f 7363 656e 6573  s_project_scenes
+00000f40: 9f00 0000 732a 0000 0004 140c 010e 011c  ....s*..........
+00000f50: ff08 020a 010c 0510 0108 0202 0102 0102  ................
+00000f60: 0102 0102 0102 0102 0102 0102 0104 f810  ................
+00000f70: 0b04 0172 4600 0000 2918 7243 0000 00da  ...rF...).rC....
+00000f80: 1664 6566 7573 6564 786d 6c2e 456c 656d  .defusedxml.Elem
+00000f90: 656e 7454 7265 65da 0a64 6566 7573 6564  entTree..defused
+00000fa0: 786d 6cda 136d 6170 7461 736b 6572 2e73  xml..maptasker.s
+00000fb0: 7263 2e74 6173 6b73 da03 7372 6372 3800  rc.tasks..srcr8.
+00000fc0: 0000 da15 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
+00000fd0: 632e 6f75 7470 7574 6c72 0200 0000 da15  c.outputlr......
+00000fe0: 6d61 7074 6173 6b65 722e 7372 632e 786d  maptasker.src.xm
+00000ff0: 6c64 6174 6172 0300 0000 7236 0000 0072  ldatar....r6...r
+00001000: 0500 0000 da16 6d61 7074 6173 6b65 722e  ......maptasker.
+00001010: 7372 632e 6672 6d74 6874 6d6c 7206 0000  src.frmthtmlr...
+00001020: 0072 3a00 0000 7237 0000 00da 0b45 6c65  .r:...r7.....Ele
+00001030: 6d65 6e74 5472 6565 da03 584d 4cda 0464  mentTree..XML..d
+00001040: 6963 74da 046c 6973 7472 2c00 0000 da03  ict..listr,.....
+00001050: 7374 7272 3d00 0000 7246 0000 0072 2a00  strr=...rF...r*.
+00001060: 0000 722a 0000 0072 2a00 0000 722b 0000  ..r*...r*...r+..
+00001070: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001080: 8600 0000 080c 0802 1201 0c01 0c01 0c01  ................
+00001090: 0c01 0203 0201 0201 0201 0201 0201 0201  ................
+000010a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000010b0: 06f1 0811 020b 0601 02ff 0202 02fe 0203  ................
+000010c0: 02fd 0204 02fc 0205 0afb 0222 0201 02ff  ..........."....
+000010d0: 0602 02fe 0603 02fd 0204 02fc 0205 02fb  ................
+000010e0: 0206 02fa 0207 0af9 024b 0601 02ff 0202  .........K......
+000010f0: 02fe 0203 02fd 0204 02fc 0605 02fb 0206  ................
+00001100: 02fa 0207 02f9 0208 0ef8                 ..........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/servicec.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/servicec.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/share.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/share.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 14:24:15 2023 UTC, .py size: 4300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,124 @@
-00000000: 6f0d 0d0a 0000 0000 0f33 2c64 cc10 0000  o........3,d....
+00000000: 6f0d 0d0a 0000 0000 9e47 3c64 c210 0000  o........G<d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6405 6502 6a09 6406 650a 6407 650a  ..d.e.j.d.e.d.e.
-00000070: 6408 650b 6409 6401 660a 640a 640b 8404  d.e.d.d.f.d.d...
-00000080: 5a0c 640c 650d 6406 650a 6407 650a 6408  Z.d.e.d.e.d.e.d.
-00000090: 650b 6409 650d 660a 640d 640e 8404 5a0e  e.d.e.f.d.d...Z.
-000000a0: 6401 5300 290f e900 0000 004e 2901 da09  d.S.)......N)...
-000000b0: 6d79 5f6f 7574 7075 7429 01da 1072 656d  my_output)...rem
-000000c0: 6f76 655f 6874 6d6c 5f74 6167 7329 01da  ove_html_tags)..
-000000d0: 0b46 4f4e 545f 544f 5f55 5345 da0c 726f  .FONT_TO_USE..ro
-000000e0: 6f74 5f65 6c65 6d65 6e74 da08 636f 6c6f  ot_element..colo
-000000f0: 726d 6170 da0c 7072 6f67 7261 6d5f 6172  rmap..program_ar
-00000100: 6773 da0b 6f75 7470 7574 5f6c 6973 74da  gs..output_list.
-00000110: 0672 6574 7572 6e63 0400 0000 0000 0000  .returnc........
-00000120: 0000 0000 0800 0000 0600 0000 4300 0000  ............C...
-00000130: 7376 0000 007c 00a0 0064 01a1 017d 047c  sv...|...d...}.|
-00000140: 0464 0075 0172 357c 04a0 0064 02a1 017d  .d.u.r5|...d...}
-00000150: 057c 0564 0075 0172 1974 017c 057c 017c  .|.d.u.r.t.|.|.|
-00000160: 027c 0383 0401 007c 04a0 0064 03a1 017d  .|.....|...d...}
-00000170: 067c 0664 0075 0172 377c 066a 0272 3964  .|.d.u.r7|.j.r9d
-00000180: 047c 066a 029b 009d 027d 0774 037c 017c  .|.j.....}.t.|.|
-00000190: 027c 0364 057c 0783 0501 0064 0053 0064  .|.d.|.....d.S.d
-000001a0: 0053 0064 0053 0064 0053 0029 064e da05  .S.d.S.d.S.).N..
-000001b0: 5368 6172 65da 0164 da01 677a 2126 6e62  Share..d..gz!&nb
-000001c0: 7370 3b26 6e62 7370 3b54 6173 6b65 724e  sp;&nbsp;TaskerN
-000001d0: 6574 2073 6561 7263 6820 6f6e 3a20 e902  et search on: ..
-000001e0: 0000 0029 04da 0466 696e 64da 1a64 6573  ...)...find..des
-000001f0: 6372 6970 7469 6f6e 5f65 6c65 6d65 6e74  cription_element
-00000200: 5f6f 7574 7075 74da 0474 6578 7472 0200  _output..textr..
-00000210: 0000 2908 7205 0000 0072 0600 0000 7207  ..).r....r....r.
-00000220: 0000 0072 0800 0000 da0d 7368 6172 655f  ...r......share_
-00000230: 656c 656d 656e 74da 1364 6573 6372 6970  element..descrip
-00000240: 7469 6f6e 5f65 6c65 6d65 6e74 5a0e 7365  tion_elementZ.se
-00000250: 6172 6368 5f65 6c65 6d65 6e74 da0a 6f75  arch_element..ou
-00000260: 745f 7374 7269 6e67 a900 7214 0000 00fa  t_string..r.....
-00000270: 742f 5573 6572 732f 6d69 6b72 7562 696e  t/Users/mikrubin
-00000280: 2f4c 6962 7261 7279 2f43 6c6f 7564 5374  /Library/CloudSt
-00000290: 6f72 6167 652f 476f 6f67 6c65 4472 6976  orage/GoogleDriv
-000002a0: 652d 6d69 6b72 7562 696e 4067 6d61 696c  e-mikrubin@gmail
-000002b0: 2e63 6f6d 2f4d 7920 4472 6976 652f 5079  .com/My Drive/Py
-000002c0: 7468 6f6e 2f6d 6170 7461 736b 6572 2f6d  thon/maptasker/m
-000002d0: 6170 7461 736b 6572 2f73 7263 2f73 6861  aptasker/src/sha
-000002e0: 7265 2e70 79da 0573 6861 7265 1800 0000  re.py..share....
-000002f0: 731a 0000 000a 0708 010a 0208 0202 0108  s...............
-00000300: 0104 ff0a 040e 010c 0314 0104 f208 0a72  ...............r
-00000310: 1600 0000 7212 0000 0063 0400 0000 0000  ....r....c......
-00000320: 0000 0000 0000 0900 0000 0600 0000 4300  ..............C.
-00000330: 0000 73f6 0000 0064 017c 006a 009b 009d  ..s....d.|.j....
-00000340: 027d 0464 027c 0164 0319 009b 0074 019b  .}.d.|.d.....t..
-00000350: 0064 049d 047d 057c 04a0 0264 057c 05a1  .d...}.|...d.|..
-00000360: 027d 047c 04a0 0264 067c 05a1 027d 047c  .}.|...d.|...}.|
-00000370: 04a0 0264 077c 05a1 027d 047c 04a0 0264  ...d.|...}.|...d
-00000380: 087c 05a1 027d 047c 04a0 0264 097c 059b  .|...}.|...d.|..
-00000390: 00a1 027d 047c 04a0 0264 0a64 0ba1 027d  ...}.|...d.d...}
-000003a0: 0464 0b7d 067c 057c 0476 0172 6e74 037c  .d.}.|.|.v.rnt.|
-000003b0: 0483 0144 005d 2c5c 027d 077d 087c 0864  ...D.],\.}.}.|.d
-000003c0: 0c6b 0272 4f7c 047c 0764 0d17 0019 0064  .k.rO|.|.d.....d
-000003d0: 0c6b 0273 5b7c 0864 0e6b 0272 677c 047c  .k.s[|.d.k.rg|.|
-000003e0: 0764 0d17 0019 0064 0c6b 0272 677c 069b  .d.....d.k.rg|..
-000003f0: 0064 0f7c 0164 0319 009b 0074 019b 0064  .d.|.d.....t...d
-00000400: 049d 056e 037c 067c 0817 007d 0671 3f7c  ...n.|.|...}.q?|
-00000410: 067d 047c 049b 007d 0474 047c 017c 027c  .}.|...}.t.|.|.|
-00000420: 0364 107c 0483 0501 0064 1153 0029 1261  .d.|.....d.S.).a
-00000430: 2c01 0000 0a20 2020 2057 6520 6861 7665  ,....    We have
-00000440: 2061 2054 6173 6b65 726e 6574 2064 6573   a Taskernet des
-00000450: 6372 6970 7469 6f6e 2028 3c53 6861 7265  cription (<Share
-00000460: 3e29 2e20 2050 726f 6365 7373 2069 740a  >).  Process it.
-00000470: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00000480: 6573 6372 6970 7469 6f6e 5f65 6c65 6d65  escription_eleme
-00000490: 6e74 3a20 7468 6520 786d 6c20 656c 656d  nt: the xml elem
-000004a0: 656e 7420 7769 7468 2074 6865 2064 6573  ent with the des
-000004b0: 6372 6970 7469 6f6e 0a20 2020 2020 2020  cription.       
-000004c0: 203a 7061 7261 6d20 636f 6c6f 726d 6170   :param colormap
-000004d0: 3a20 7468 6520 636f 6c6f 7273 2074 6f20  : the colors to 
-000004e0: 7573 6520 666f 7220 7468 6520 6f75 7470  use for the outp
-000004f0: 7574 0a20 2020 2020 2020 203a 7061 7261  ut.        :para
-00000500: 6d20 7072 6f67 7261 6d5f 6172 6773 3a20  m program_args: 
-00000510: 7468 6520 7275 6e74 696d 6520 6172 6775  the runtime argu
-00000520: 6d65 6e74 730a 2020 2020 2020 2020 3a70  ments.        :p
-00000530: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
-00000540: 3a20 7468 6520 6f75 7470 7574 206c 696e  : the output lin
-00000550: 6573 2074 6875 7320 6661 720a 2020 2020  es thus far.    
-00000560: 7a23 266e 6273 703b 266e 6273 703b 5461  z#&nbsp;&nbsp;Ta
-00000570: 736b 6572 4e65 7420 6465 7363 7269 7074  skerNet descript
-00000580: 696f 6e3a 207a 373c 2f70 3e3c 7020 7374  ion: z7</p><p st
-00000590: 796c 653d 226d 6172 6769 6e2d 6c65 6674  yle="margin-left
-000005a0: 3a32 3070 783b 6d61 7267 696e 2d72 6967  :20px;margin-rig
-000005b0: 6874 3a35 3070 783b 636f 6c6f 723a da0f  ht:50px;color:..
-000005c0: 7461 736b 6572 6e65 745f 636f 6c6f 72fa  taskernet_color.
-000005d0: 013e 7a03 3c70 3e7a 053c 6272 2f3e 7a04  .>z.<p>z.<br/>z.
-000005e0: 3c68 313e fa01 0d7a 043c 6c69 3e7a 053c  <h1>...z.<li>z.<
-000005f0: 2f6c 693e da00 fa01 20e9 0100 0000 fa01  /li>.... .......
-00000600: 2d7a 333c 7020 7374 796c 653d 226d 6172  -z3<p style="mar
-00000610: 6769 6e2d 6c65 6674 3a32 3070 783b 6d61  gin-left:20px;ma
-00000620: 7267 696e 2d72 6967 6874 3a35 3070 783b  rgin-right:50px;
-00000630: 636f 6c6f 723a 720d 0000 004e 2905 7210  color:r....N).r.
-00000640: 0000 0072 0400 0000 da07 7265 706c 6163  ...r......replac
-00000650: 65da 0965 6e75 6d65 7261 7465 7202 0000  e..enumerater...
-00000660: 0029 0972 1200 0000 7206 0000 0072 0700  .).r....r....r..
-00000670: 0000 7208 0000 0072 1300 0000 5a0b 696e  ..r....r....Z.in
-00000680: 6465 6e74 5f68 746d 6c5a 086e 6577 5f6c  dent_htmlZ.new_l
-00000690: 696e 655a 0870 6f73 6974 696f 6e5a 0f63  ineZ.positionZ.c
-000006a0: 6861 7261 6374 6572 5f69 6e64 6578 7214  haracter_indexr.
-000006b0: 0000 0072 1400 0000 7215 0000 0072 0f00  ...r....r....r..
-000006c0: 0000 3200 0000 7338 0000 000c 0b02 0206  ..2...s8........
-000006d0: 0102 ff02 0106 ff02 ff0c 060c 010c 010c  ................
-000006e0: 010e 010c 0104 0408 0110 0118 0418 0106  ................
-000006f0: fd06 0102 ff02 0108 ff06 0404 fb04 0706  ................
-00000700: 0114 0272 0f00 0000 290f da02 7265 da15  ...r....)...re..
-00000710: 786d 6c2e 6574 7265 652e 456c 656d 656e  xml.etree.Elemen
-00000720: 7454 7265 65da 0378 6d6c da15 6d61 7074  tTree..xml..mapt
-00000730: 6173 6b65 722e 7372 632e 6f75 7470 7574  asker.src.output
-00000740: 6c72 0200 0000 da15 6d61 7074 6173 6b65  lr......maptaske
-00000750: 722e 7372 632e 786d 6c64 6174 6172 0300  r.src.xmldatar..
-00000760: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
-00000770: 632e 7379 7363 6f6e 7374 7204 0000 00da  c.sysconstr.....
-00000780: 0565 7472 6565 da04 6469 6374 da04 6c69  .etree..dict..li
-00000790: 7374 7216 0000 00da 0373 7472 720f 0000  str......strr...
-000007a0: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
-000007b0: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000007c0: 0000 0073 3600 0000 0802 080d 0c03 0c01  ...s6...........
-000007d0: 0c01 0203 0401 02ff 0202 02fe 0203 02fd  ................
-000007e0: 0204 02fc 0205 0afb 021a 0201 02ff 0201  ................
-000007f0: 02ff 0201 02ff 0201 02ff 0202 0efe       ..............
+00000020: 000a 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
+00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6404  ..d.d.l.m.Z...d.
+00000050: 6501 6a06 6a07 6405 6508 6406 6508 6407  e.j.j.d.e.d.e.d.
+00000060: 6509 6408 6401 660a 6409 640a 8404 5a0a  e.d.d.f.d.d...Z.
+00000070: 640b 6501 6a06 6405 6508 6406 6508 6407  d.e.j.d.e.d.e.d.
+00000080: 6509 6408 6401 660a 640c 640d 8404 5a0b  e.d.d.f.d.d...Z.
+00000090: 6401 5300 290e e900 0000 004e 2901 da09  d.S.)......N)...
+000000a0: 6d79 5f6f 7574 7075 7429 01da 0b46 4f4e  my_output)...FON
+000000b0: 545f 544f 5f55 5345 da0c 726f 6f74 5f65  T_TO_USE..root_e
+000000c0: 6c65 6d65 6e74 da08 636f 6c6f 726d 6170  lement..colormap
+000000d0: da0c 7072 6f67 7261 6d5f 6172 6773 da0b  ..program_args..
+000000e0: 6f75 7470 7574 5f6c 6973 74da 0672 6574  output_list..ret
+000000f0: 7572 6e63 0400 0000 0000 0000 0000 0000  urnc............
+00000100: 0800 0000 0600 0000 4300 0000 7376 0000  ........C...sv..
+00000110: 007c 00a0 0064 01a1 017d 047c 0464 0075  .|...d...}.|.d.u
+00000120: 0172 357c 04a0 0064 02a1 017d 057c 0564  .r5|...d...}.|.d
+00000130: 0075 0172 1974 017c 057c 017c 027c 0383  .u.r.t.|.|.|.|..
+00000140: 0401 007c 04a0 0064 03a1 017d 067c 0664  ...|...d...}.|.d
+00000150: 0075 0172 377c 066a 0272 3964 047c 066a  .u.r7|.j.r9d.|.j
+00000160: 029b 009d 027d 0774 037c 017c 027c 0364  .....}.t.|.|.|.d
+00000170: 057c 0783 0501 0064 0053 0064 0053 0064  .|.....d.S.d.S.d
+00000180: 0053 0064 0053 0029 064e da05 5368 6172  .S.d.S.).N..Shar
+00000190: 65da 0164 da01 677a 2126 6e62 7370 3b26  e..d..gz!&nbsp;&
+000001a0: 6e62 7370 3b54 6173 6b65 724e 6574 2073  nbsp;TaskerNet s
+000001b0: 6561 7263 6820 6f6e 3a20 e902 0000 0029  earch on: .....)
+000001c0: 04da 0466 696e 64da 1a64 6573 6372 6970  ...find..descrip
+000001d0: 7469 6f6e 5f65 6c65 6d65 6e74 5f6f 7574  tion_element_out
+000001e0: 7075 74da 0474 6578 7472 0200 0000 2908  put..textr....).
+000001f0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00000200: 0700 0000 da0d 7368 6172 655f 656c 656d  ......share_elem
+00000210: 656e 74da 1364 6573 6372 6970 7469 6f6e  ent..description
+00000220: 5f65 6c65 6d65 6e74 5a0e 7365 6172 6368  _elementZ.search
+00000230: 5f65 6c65 6d65 6e74 da0a 6f75 745f 7374  _element..out_st
+00000240: 7269 6e67 a900 7213 0000 00fa 742f 5573  ring..r.....t/Us
+00000250: 6572 732f 6d69 6b72 7562 696e 2f4c 6962  ers/mikrubin/Lib
+00000260: 7261 7279 2f43 6c6f 7564 5374 6f72 6167  rary/CloudStorag
+00000270: 652f 476f 6f67 6c65 4472 6976 652d 6d69  e/GoogleDrive-mi
+00000280: 6b72 7562 696e 4067 6d61 696c 2e63 6f6d  krubin@gmail.com
+00000290: 2f4d 7920 4472 6976 652f 5079 7468 6f6e  /My Drive/Python
+000002a0: 2f6d 6170 7461 736b 6572 2f6d 6170 7461  /maptasker/mapta
+000002b0: 736b 6572 2f73 7263 2f73 6861 7265 2e70  sker/src/share.p
+000002c0: 79da 0573 6861 7265 1500 0000 731a 0000  y..share....s...
+000002d0: 000a 0708 010a 0208 0202 0108 0104 ff0a  ................
+000002e0: 040e 010c 0314 0104 f208 0a72 1500 0000  ...........r....
+000002f0: 7211 0000 0063 0400 0000 0000 0000 0000  r....c..........
+00000300: 0000 0900 0000 0600 0000 4300 0000 73f6  ..........C...s.
+00000310: 0000 0064 017c 006a 009b 009d 027d 0464  ...d.|.j.....}.d
+00000320: 027c 0164 0319 009b 0074 019b 0064 049d  .|.d.....t...d..
+00000330: 047d 057c 04a0 0264 057c 05a1 027d 047c  .}.|...d.|...}.|
+00000340: 04a0 0264 067c 05a1 027d 047c 04a0 0264  ...d.|...}.|...d
+00000350: 077c 05a1 027d 047c 04a0 0264 087c 05a1  .|...}.|...d.|..
+00000360: 027d 047c 04a0 0264 097c 059b 00a1 027d  .}.|...d.|.....}
+00000370: 047c 04a0 0264 0a64 0ba1 027d 0464 0b7d  .|...d.d...}.d.}
+00000380: 067c 057c 0476 0172 6e74 037c 0483 0144  .|.|.v.rnt.|...D
+00000390: 005d 2c5c 027d 077d 087c 0864 0c6b 0272  .],\.}.}.|.d.k.r
+000003a0: 4f7c 047c 0764 0d17 0019 0064 0c6b 0273  O|.|.d.....d.k.s
+000003b0: 5b7c 0864 0e6b 0272 677c 047c 0764 0d17  [|.d.k.rg|.|.d..
+000003c0: 0019 0064 0c6b 0272 677c 069b 0064 0f7c  ...d.k.rg|...d.|
+000003d0: 0164 0319 009b 0074 019b 0064 049d 056e  .d.....t...d...n
+000003e0: 037c 067c 0817 007d 0671 3f7c 067d 047c  .|.|...}.q?|.}.|
+000003f0: 049b 007d 0474 047c 017c 027c 0364 107c  ...}.t.|.|.|.d.|
+00000400: 0483 0501 0064 1153 0029 1261 2c01 0000  .....d.S.).a,...
+00000410: 0a20 2020 2057 6520 6861 7665 2061 2054  .    We have a T
+00000420: 6173 6b65 726e 6574 2064 6573 6372 6970  askernet descrip
+00000430: 7469 6f6e 2028 3c53 6861 7265 3e29 2e20  tion (<Share>). 
+00000440: 2050 726f 6365 7373 2069 740a 2020 2020   Process it.    
+00000450: 2020 2020 3a70 6172 616d 2064 6573 6372      :param descr
+00000460: 6970 7469 6f6e 5f65 6c65 6d65 6e74 3a20  iption_element: 
+00000470: 7468 6520 786d 6c20 656c 656d 656e 7420  the xml element 
+00000480: 7769 7468 2074 6865 2064 6573 6372 6970  with the descrip
+00000490: 7469 6f6e 0a20 2020 2020 2020 203a 7061  tion.        :pa
+000004a0: 7261 6d20 636f 6c6f 726d 6170 3a20 7468  ram colormap: th
+000004b0: 6520 636f 6c6f 7273 2074 6f20 7573 6520  e colors to use 
+000004c0: 666f 7220 7468 6520 6f75 7470 7574 0a20  for the output. 
+000004d0: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
+000004e0: 6f67 7261 6d5f 6172 6773 3a20 7468 6520  ogram_args: the 
+000004f0: 7275 6e74 696d 6520 6172 6775 6d65 6e74  runtime argument
+00000500: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
+00000510: 206f 7574 7075 745f 6c69 7374 3a20 7468   output_list: th
+00000520: 6520 6f75 7470 7574 206c 696e 6573 2074  e output lines t
+00000530: 6875 7320 6661 720a 2020 2020 7a17 5461  hus far.    z.Ta
+00000540: 736b 6572 4e65 7420 6465 7363 7269 7074  skerNet descript
+00000550: 696f 6e3a 207a 373c 2f70 3e3c 7020 7374  ion: z7</p><p st
+00000560: 796c 653d 226d 6172 6769 6e2d 6c65 6674  yle="margin-left
+00000570: 3a32 3070 783b 6d61 7267 696e 2d72 6967  :20px;margin-rig
+00000580: 6874 3a35 3070 783b 636f 6c6f 723a da0f  ht:50px;color:..
+00000590: 7461 736b 6572 6e65 745f 636f 6c6f 72fa  taskernet_color.
+000005a0: 013e 7a03 3c70 3e7a 053c 6272 2f3e 7a04  .>z.<p>z.<br/>z.
+000005b0: 3c68 313e fa01 0d7a 043c 6c69 3e7a 053c  <h1>...z.<li>z.<
+000005c0: 2f6c 693e da00 fa01 20e9 0100 0000 fa01  /li>.... .......
+000005d0: 2d7a 333c 7020 7374 796c 653d 226d 6172  -z3<p style="mar
+000005e0: 6769 6e2d 6c65 6674 3a32 3070 783b 6d61  gin-left:20px;ma
+000005f0: 7267 696e 2d72 6967 6874 3a35 3070 783b  rgin-right:50px;
+00000600: 636f 6c6f 723a 720c 0000 004e 2905 720f  color:r....N).r.
+00000610: 0000 0072 0300 0000 da07 7265 706c 6163  ...r......replac
+00000620: 65da 0965 6e75 6d65 7261 7465 7202 0000  e..enumerater...
+00000630: 0029 0972 1100 0000 7205 0000 0072 0600  .).r....r....r..
+00000640: 0000 7207 0000 0072 1200 0000 5a0b 696e  ..r....r....Z.in
+00000650: 6465 6e74 5f68 746d 6c5a 086e 6577 5f6c  dent_htmlZ.new_l
+00000660: 696e 65da 0870 6f73 6974 696f 6e5a 0f63  ine..positionZ.c
+00000670: 6861 7261 6374 6572 5f69 6e64 6578 7213  haracter_indexr.
+00000680: 0000 0072 1300 0000 7214 0000 0072 0e00  ...r....r....r..
+00000690: 0000 2f00 0000 7338 0000 000c 0e02 0206  ../...s8........
+000006a0: 0102 ff02 0106 ff02 ff0c 060c 010c 010c  ................
+000006b0: 010e 010c 0104 0408 0110 0118 0418 0106  ................
+000006c0: fd06 0102 ff02 0108 ff06 0404 fb04 0706  ................
+000006d0: 0114 0272 0e00 0000 290c da16 6465 6675  ...r....)...defu
+000006e0: 7365 6478 6d6c 2e45 6c65 6d65 6e74 5472  sedxml.ElementTr
+000006f0: 6565 da0a 6465 6675 7365 6478 6d6c da15  ee..defusedxml..
+00000700: 6d61 7074 6173 6b65 722e 7372 632e 6f75  maptasker.src.ou
+00000710: 7470 7574 6c72 0200 0000 da16 6d61 7074  tputlr......mapt
+00000720: 6173 6b65 722e 7372 632e 7379 7363 6f6e  asker.src.syscon
+00000730: 7374 7203 0000 00da 0b45 6c65 6d65 6e74  str......Element
+00000740: 5472 6565 da03 584d 4cda 0464 6963 74da  Tree..XML..dict.
+00000750: 046c 6973 7472 1500 0000 720e 0000 0072  .listr....r....r
+00000760: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
+00000770: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000780: 0073 3200 0000 080d 0c03 0c01 0203 0601  .s2.............
+00000790: 02ff 0202 02fe 0203 02fd 0204 02fc 0205  ................
+000007a0: 0afb 021a 0401 02ff 0202 02fe 0203 02fd  ................
+000007b0: 0204 02fc 0205 0efb                      ........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/shellsort.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/shellsort.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/sysconst.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/sysconst.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 17:43:19 2023 UTC, .py size: 4082 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,149 +1,148 @@
-00000000: 6f0d 0d0a 0000 0000 b761 2c64 f20f 0000  o........a,d....
+00000000: 6f0d 0d0a 0000 0000 952b 3864 d70f 0000  o........+8d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9601 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
-00000040: 6d02 5a02 0100 6403 5a03 6404 5a04 6405  m.Z...d.Z.d.Z.d.
-00000050: 5a05 6406 5a06 6407 5a07 6408 5a08 6409  Z.d.Z.d.Z.d.Z.d.
-00000060: 6501 9b00 640a 9d03 5a09 640b 5a0a 6900  e...d...Z.d.Z.i.
-00000070: 640c 640d 9301 640e 640d 9301 640f 6410  d.d...d.d...d.d.
-00000080: 9301 6411 6410 9301 6412 6413 9301 6414  ..d.d...d.d...d.
-00000090: 6413 9301 6415 6416 9301 6417 6416 9301  d...d.d...d.d...
-000000a0: 6418 6419 9301 641a 6419 9301 641b 641c  d.d...d.d...d.d.
-000000b0: 9301 641d 641e 9301 641f 6420 9301 6421  ..d.d...d.d ..d!
-000000c0: 6420 9301 6422 6423 9301 6424 6423 9301  d ..d"d#..d$d#..
-000000d0: 6425 6426 9301 6900 6427 6426 9301 6428  d%d&..i.d'd&..d(
-000000e0: 6429 9301 642a 642b 9301 642c 642b 9301  d)..d*d+..d,d+..
-000000f0: 642d 642e 9301 642f 642e 9301 6430 6431  d-d...d/d...d0d1
-00000100: 9301 6432 6431 9301 6433 6434 9301 6435  ..d2d1..d3d4..d5
-00000110: 6434 9301 6436 6437 9301 6438 6437 9301  d4..d6d7..d8d7..
-00000120: 6439 643a 9301 643b 643a 9301 643c 643d  d9d:..d;d:..d<d=
-00000130: 9301 643e 643d 9301 a501 5a0b 6900 640e  ..d>d=....Z.i.d.
-00000140: 640c 9301 6411 640f 9301 6414 6412 9301  d...d.d...d.d...
-00000150: 6417 643f 9301 641a 6440 9301 641b 6441  d.d?..d.d@..d.dA
-00000160: 9301 641d 6442 9301 6421 6443 9301 6424  ..d.dB..d!dC..d$
-00000170: 6444 9301 6427 6445 9301 6428 6446 9301  dD..d'dE..d(dF..
-00000180: 642c 642a 9301 642f 6447 9301 6432 6448  d,d*..d/dG..d2dH
-00000190: 9301 6435 6449 9301 6438 644a 9301 643b  ..d5dI..d8dJ..d;
-000001a0: 644b 9301 643e 643c 6901 a501 5a0c 6502  dK..d>d<i...Z.e.
-000001b0: a00d 644c a101 5a0e 644d 5a0f 644d 5a10  ..dL..Z.dMZ.dMZ.
-000001c0: 644e 5300 294f e900 0000 0029 01da 0b4f  dNS.)O.....)...O
-000001d0: 5554 5055 545f 464f 4e54 2901 da07 6c6f  UTPUT_FONT)...lo
-000001e0: 6767 696e 677a 1255 6e6e 616d 6564 2f41  ggingz.Unnamed/A
-000001f0: 6e6f 6e79 6d6f 7573 2e7a 174d 6170 5461  nonymous.z.MapTa
-00000200: 736b 6572 2076 6572 7369 6f6e 2031 2e33  sker version 1.3
-00000210: 2e32 7a34 474e 5520 4745 4e45 5241 4c20  .2z4GNU GENERAL 
-00000220: 5055 424c 4943 204c 4943 454e 5345 2028  PUBLIC LICENSE (
-00000230: 5665 7273 696f 6e20 332c 2032 3920 4a75  Version 3, 29 Ju
-00000240: 6e65 2032 3030 3729 7a0c 2d6e 6f6e 6520  ne 2007)z.-none 
-00000250: 666f 756e 642e 7a17 2e4d 6170 5461 736b  found.z..MapTask
-00000260: 6572 5f52 756e 436f 756e 742e 7478 747a  er_RunCount.txtz
-00000270: 182e 4d61 7054 6173 6b65 725f 6172 6775  ..MapTasker_argu
-00000280: 6d65 6e74 732e 7478 747a 0d3b 666f 6e74  ments.txtz.;font
-00000290: 2d66 616d 696c 793a fa01 227a 104e 6f6e  -family:.."z.Non
-000002a0: 6520 6f72 2075 6e6e 616d 6564 215a 0850  e or unnamed!Z.P
-000002b0: 726f 6a65 6374 73da 0d70 726f 6a65 6374  rojects..project
-000002c0: 5f63 6f6c 6f72 da07 5072 6f6a 6563 745a  _color..ProjectZ
-000002d0: 0850 726f 6669 6c65 73da 0d70 726f 6669  .Profiles..profi
-000002e0: 6c65 5f63 6f6c 6f72 da07 5072 6f66 696c  le_color..Profil
-000002f0: 655a 0554 6173 6b73 da0a 7461 736b 5f63  eZ.Tasks..task_c
-00000300: 6f6c 6f72 da04 5461 736b 7a0e 2854 6173  olor..Taskz.(Tas
-00000310: 6b29 2041 6374 696f 6e73 da0c 6163 7469  k) Actions..acti
-00000320: 6f6e 5f63 6f6c 6f72 5a06 4163 7469 6f6e  on_colorZ.Action
-00000330: 7a11 4469 7361 626c 6564 2050 726f 6669  z.Disabled Profi
-00000340: 6c65 735a 1664 6973 6162 6c65 645f 7072  lesZ.disabled_pr
-00000350: 6f66 696c 655f 636f 6c6f 725a 0f44 6973  ofile_colorZ.Dis
-00000360: 6162 6c65 6450 726f 6669 6c65 5a0b 556e  abledProfileZ.Un
-00000370: 6b6e 6f77 6e54 6173 6bda 1275 6e6b 6e6f  knownTask..unkno
-00000380: 776e 5f74 6173 6b5f 636f 6c6f 725a 0e44  wn_task_colorZ.D
-00000390: 6973 6162 6c65 6441 6374 696f 6eda 1564  isabledAction..d
-000003a0: 6973 6162 6c65 645f 6163 7469 6f6e 5f63  isabled_action_c
-000003b0: 6f6c 6f72 7a11 4163 7469 6f6e 2043 6f6e  olorz.Action Con
-000003c0: 6469 7469 6f6e 73da 1661 6374 696f 6e5f  ditions..action_
-000003d0: 636f 6e64 6974 696f 6e5f 636f 6c6f 725a  condition_colorZ
-000003e0: 0f41 6374 696f 6e43 6f6e 6469 7469 6f6e  .ActionCondition
-000003f0: 7a12 5072 6f66 696c 6520 436f 6e64 6974  z.Profile Condit
-00000400: 696f 6e73 5a17 7072 6f66 696c 655f 636f  ionsZ.profile_co
-00000410: 6e64 6974 696f 6e5f 636f 6c6f 725a 1050  ndition_colorZ.P
-00000420: 726f 6669 6c65 436f 6e64 6974 696f 6e7a  rofileConditionz
-00000430: 0d4c 6175 6e63 6865 7220 5461 736b 5a13  .Launcher TaskZ.
-00000440: 6c61 756e 6368 6572 5f74 6173 6b5f 636f  launcher_task_co
-00000450: 6c6f 725a 0c4c 6175 6e63 6865 7254 6173  lorZ.LauncherTas
-00000460: 6b5a 0a42 6163 6b67 726f 756e 645a 1062  kZ.BackgroundZ.b
-00000470: 6163 6b67 726f 756e 645f 636f 6c6f 725a  ackground_colorZ
-00000480: 0653 6365 6e65 73da 0b73 6365 6e65 5f63  .Scenes..scene_c
-00000490: 6f6c 6f72 5a05 5363 656e 655a 0742 756c  olorZ.SceneZ.Bul
-000004a0: 6c65 7473 da0c 6275 6c6c 6574 5f63 6f6c  lets..bullet_col
-000004b0: 6f72 5a06 4275 6c6c 6574 7a0d 4163 7469  orZ.Bulletz.Acti
-000004c0: 6f6e 204c 6162 656c 73da 1261 6374 696f  on Labels..actio
-000004d0: 6e5f 6c61 6265 6c5f 636f 6c6f 725a 0b41  n_label_colorZ.A
-000004e0: 6374 696f 6e4c 6162 656c 7a0c 4163 7469  ctionLabelz.Acti
-000004f0: 6f6e 204e 616d 6573 da11 6163 7469 6f6e  on Names..action
-00000500: 5f6e 616d 655f 636f 6c6f 725a 0a41 6374  _name_colorZ.Act
-00000510: 696f 6e4e 616d 657a 1554 6173 6b65 724e  ionNamez.TaskerN
-00000520: 6574 2049 6e66 6f72 6d61 7469 6f6e da0f  et Information..
-00000530: 7461 736b 6572 6e65 745f 636f 6c6f 725a  taskernet_colorZ
-00000540: 0d54 6173 6b65 724e 6574 496e 666f 7a12  .TaskerNetInfoz.
-00000550: 5461 736b 6572 2050 7265 6665 7265 6e63  Tasker Preferenc
-00000560: 6573 5a11 7072 6566 6572 656e 6365 735f  esZ.preferences_
-00000570: 636f 6c6f 725a 0b50 7265 6665 7265 6e63  colorZ.Preferenc
-00000580: 6573 7a11 5472 6169 6c69 6e67 2043 6f6d  esz.Trailing Com
-00000590: 6d65 6e74 735a 1774 7261 696c 696e 675f  mentsZ.trailing_
-000005a0: 636f 6d6d 656e 7473 5f63 6f6c 6f72 5a10  comments_colorZ.
-000005b0: 5472 6169 6c69 6e67 436f 6d6d 656e 7473  TrailingComments
-000005c0: 7a0e 5461 736b 2027 6163 7469 6f6e 7327  z.Task 'actions'
-000005d0: 7a13 2764 6973 6162 6c65 6427 2050 726f  z.'disabled' Pro
-000005e0: 6669 6c65 737a 0f27 756e 6b6e 6f77 6e27  filesz.'unknown'
-000005f0: 2054 6173 6b73 7a17 6469 7361 626c 6564   Tasksz.disabled
-00000600: 2054 6173 6b20 2761 6374 696f 6e73 277a   Task 'actions'z
-00000610: 1854 6173 6b20 6163 7469 6f6e 2027 636f  .Task action 'co
-00000620: 6e64 6974 696f 6e73 277a 1450 726f 6669  nditions'z.Profi
-00000630: 6c65 2027 636f 6e64 6974 696f 6e73 277a  le 'conditions'z
-00000640: 1950 726f 6a65 6374 2773 2027 6c61 756e  .Project's 'laun
-00000650: 6368 6572 2720 5461 736b 7a11 6f75 7470  cher' Taskz.outp
-00000660: 7574 2062 6163 6b67 726f 756e 647a 0c6c  ut backgroundz.l
-00000670: 6973 7420 6275 6c6c 6574 737a 1454 6173  ist bulletsz.Tas
-00000680: 6b20 6163 7469 6f6e 2027 6c61 6265 6c73  k action 'labels
-00000690: 277a 1354 6173 6b20 6163 7469 6f6e 2027  'z.Task action '
-000006a0: 6e61 6d65 7327 7a17 5461 736b 6572 4e65  names'z.TaskerNe
-000006b0: 7420 2769 6e66 6f72 6d61 7469 6f6e 277a  t 'information'z
-000006c0: 1454 6173 6b65 7220 2770 7265 6665 7265  .Tasker 'prefere
-000006d0: 6e63 6573 275a 094d 6170 5461 736b 6572  nces'Z.MapTasker
-000006e0: 464e 2911 da14 6d61 7074 6173 6b65 722e  FN)...maptasker.
-000006f0: 7372 632e 636f 6e66 6967 7202 0000 0072  src.configr....r
-00000700: 0300 0000 da11 554e 4b4e 4f57 4e5f 5441  ......UNKNOWN_TA
-00000710: 534b 5f4e 414d 455a 0a4d 595f 5645 5253  SK_NAMEZ.MY_VERS
-00000720: 494f 4e5a 0a4d 595f 4c49 4345 4e53 455a  IONZ.MY_LICENSEZ
-00000730: 0a4e 4f5f 5052 4f4a 4543 545a 0c43 4f55  .NO_PROJECTZ.COU
-00000740: 4e54 4552 5f46 494c 455a 0e41 5247 554d  NTER_FILEZ.ARGUM
-00000750: 454e 5453 5f46 494c 45da 0b46 4f4e 545f  ENTS_FILE..FONT_
-00000760: 544f 5f55 5345 5a0a 4e4f 5f50 524f 4649  TO_USEZ.NO_PROFI
-00000770: 4c45 5a14 5459 5045 535f 4f46 5f43 4f4c  LEZ.TYPES_OF_COL
-00000780: 4f52 5f4e 414d 4553 5a0f 5459 5045 535f  OR_NAMESZ.TYPES_
-00000790: 4f46 5f43 4f4c 4f52 535a 0967 6574 4c6f  OF_COLORSZ.getLo
-000007a0: 6767 6572 da06 6c6f 6767 6572 da09 6465  gger..logger..de
-000007b0: 6275 675f 6f75 745a 0d44 4542 5547 5f50  bug_outZ.DEBUG_P
-000007c0: 524f 4752 414d a900 7219 0000 0072 1900  ROGRAM..r....r..
-000007d0: 0000 fa77 2f55 7365 7273 2f6d 696b 7275  ...w/Users/mikru
-000007e0: 6269 6e2f 4c69 6272 6172 792f 436c 6f75  bin/Library/Clou
-000007f0: 6453 746f 7261 6765 2f47 6f6f 676c 6544  dStorage/GoogleD
-00000800: 7269 7665 2d6d 696b 7275 6269 6e40 676d  rive-mikrubin@gm
-00000810: 6169 6c2e 636f 6d2f 4d79 2044 7269 7665  ail.com/My Drive
-00000820: 2f50 7974 686f 6e2f 6d61 7074 6173 6b65  /Python/maptaske
-00000830: 722f 6d61 7074 6173 6b65 722f 7372 632f  r/maptasker/src/
-00000840: 7379 7363 6f6e 7374 2e70 79da 083c 6d6f  sysconst.py..<mo
-00000850: 6475 6c65 3e01 0000 0073 ea00 0000 0c0d  dule>....s......
-00000860: 0c01 0403 0401 0401 0401 0401 0401 0c01  ................
-00000870: 0401 0207 0401 02ff 0402 02fe 0403 02fd  ................
-00000880: 0404 02fc 0405 02fb 0406 02fa 0407 02f9  ................
-00000890: 0408 02f8 0409 02f7 040a 02f6 040b 02f5  ................
-000008a0: 040c 02f4 040d 02f3 040e 02f2 040f 02f1  ................
-000008b0: 0410 02f0 0411 04ef 0412 02ee 0413 02ed  ................
-000008c0: 0414 02ec 0415 02eb 0416 02ea 0417 02e9  ................
-000008d0: 0418 02e8 0419 02e7 041a 02e6 041b 02e5  ................
-000008e0: 041c 02e4 041d 02e3 041e 02e2 041f 02e1  ................
-000008f0: 0420 02e0 0421 06df 0225 0401 02ff 0402  . ...!...%......
-00000900: 02fe 0403 02fd 0404 02fc 0405 02fb 0406  ................
-00000910: 02fa 0407 02f9 0408 02f8 0409 02f7 040a  ................
-00000920: 02f6 040b 02f5 040c 02f4 040d 02f3 040e  ................
-00000930: 02f2 040f 02f1 0410 02f0 0411 02ef 0412  ................
-00000940: 06ee 0a15 0401 0801                      ........
+00000020: 0004 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 5a02 6403 5a03 6404 5a04 6405 5a05 6406  Z.d.Z.d.Z.d.Z.d.
+00000050: 5a06 6407 5a07 6408 5a08 6409 6501 9b00  Z.d.Z.d.Z.d.e...
+00000060: 9d02 5a09 640a 5a0a 6900 640b 640c 9301  ..Z.d.Z.i.d.d...
+00000070: 640d 640c 9301 640e 640f 9301 6410 640f  d.d...d.d...d.d.
+00000080: 9301 6411 6412 9301 6413 6412 9301 6414  ..d.d...d.d...d.
+00000090: 6415 9301 6416 6415 9301 6417 6418 9301  d...d.d...d.d...
+000000a0: 6419 6418 9301 641a 641b 9301 641c 641d  d.d...d.d...d.d.
+000000b0: 9301 641e 641f 9301 6420 641f 9301 6421  ..d.d...d d...d!
+000000c0: 6422 9301 6423 6422 9301 6424 6425 9301  d"..d#d"..d$d%..
+000000d0: 6900 6426 6425 9301 6427 6428 9301 6429  i.d&d%..d'd(..d)
+000000e0: 642a 9301 642b 642a 9301 642c 642d 9301  d*..d+d*..d,d-..
+000000f0: 642e 642d 9301 642f 6430 9301 6431 6430  d.d-..d/d0..d1d0
+00000100: 9301 6432 6433 9301 6434 6433 9301 6435  ..d2d3..d4d3..d5
+00000110: 6436 9301 6437 6436 9301 6438 6439 9301  d6..d7d6..d8d9..
+00000120: 643a 6439 9301 643b 643c 9301 643d 643c  d:d9..d;d<..d=d<
+00000130: 9301 a501 5a0b 6900 640d 640b 9301 6410  ....Z.i.d.d...d.
+00000140: 640e 9301 6413 6411 9301 6416 643e 9301  d...d.d...d.d>..
+00000150: 6419 643f 9301 641a 6440 9301 641c 6441  d.d?..d.d@..d.dA
+00000160: 9301 6420 6442 9301 6423 6443 9301 6426  ..d dB..d#dC..d&
+00000170: 6444 9301 6427 6445 9301 642b 6429 9301  dD..d'dE..d+d)..
+00000180: 642e 6446 9301 6431 6447 9301 6434 6448  d.dF..d1dG..d4dH
+00000190: 9301 6437 6449 9301 643a 644a 9301 643d  ..d7dI..d:dJ..d=
+000001a0: 643b 6901 a501 5a0c 6502 a00d 644b a101  d;i...Z.e...dK..
+000001b0: 5a0e 644c 5a0f 644d 5a10 6402 5300 294e  Z.dLZ.dMZ.d.S.)N
+000001c0: e900 0000 0029 01da 0b4f 5554 5055 545f  .....)...OUTPUT_
+000001d0: 464f 4e54 4e7a 1255 6e6e 616d 6564 2f41  FONTNz.Unnamed/A
+000001e0: 6e6f 6e79 6d6f 7573 2e7a 174d 6170 5461  nonymous.z.MapTa
+000001f0: 736b 6572 2076 6572 7369 6f6e 2031 2e33  sker version 1.3
+00000200: 2e33 7a34 474e 5520 4745 4e45 5241 4c20  .3z4GNU GENERAL 
+00000210: 5055 424c 4943 204c 4943 454e 5345 2028  PUBLIC LICENSE (
+00000220: 5665 7273 696f 6e20 332c 2032 3920 4a75  Version 3, 29 Ju
+00000230: 6e65 2032 3030 3729 7a0c 2d6e 6f6e 6520  ne 2007)z.-none 
+00000240: 666f 756e 642e 7a17 2e4d 6170 5461 736b  found.z..MapTask
+00000250: 6572 5f52 756e 436f 756e 742e 7478 747a  er_RunCount.txtz
+00000260: 192e 4d61 7054 6173 6b65 725f 6172 6775  ..MapTasker_argu
+00000270: 6d65 6e74 732e 6a73 6f6e 7a0d 3b66 6f6e  ments.jsonz.;fon
+00000280: 742d 6661 6d69 6c79 3a7a 104e 6f6e 6520  t-family:z.None 
+00000290: 6f72 2075 6e6e 616d 6564 215a 0850 726f  or unnamed!Z.Pro
+000002a0: 6a65 6374 73da 0d70 726f 6a65 6374 5f63  jects..project_c
+000002b0: 6f6c 6f72 da07 5072 6f6a 6563 745a 0850  olor..ProjectZ.P
+000002c0: 726f 6669 6c65 73da 0d70 726f 6669 6c65  rofiles..profile
+000002d0: 5f63 6f6c 6f72 da07 5072 6f66 696c 655a  _color..ProfileZ
+000002e0: 0554 6173 6b73 da0a 7461 736b 5f63 6f6c  .Tasks..task_col
+000002f0: 6f72 da04 5461 736b 7a0e 2854 6173 6b29  or..Taskz.(Task)
+00000300: 2041 6374 696f 6e73 da0c 6163 7469 6f6e   Actions..action
+00000310: 5f63 6f6c 6f72 5a06 4163 7469 6f6e 7a11  _colorZ.Actionz.
+00000320: 4469 7361 626c 6564 2050 726f 6669 6c65  Disabled Profile
+00000330: 735a 1664 6973 6162 6c65 645f 7072 6f66  sZ.disabled_prof
+00000340: 696c 655f 636f 6c6f 725a 0f44 6973 6162  ile_colorZ.Disab
+00000350: 6c65 6450 726f 6669 6c65 5a0b 556e 6b6e  ledProfileZ.Unkn
+00000360: 6f77 6e54 6173 6bda 1275 6e6b 6e6f 776e  ownTask..unknown
+00000370: 5f74 6173 6b5f 636f 6c6f 725a 0e44 6973  _task_colorZ.Dis
+00000380: 6162 6c65 6441 6374 696f 6eda 1564 6973  abledAction..dis
+00000390: 6162 6c65 645f 6163 7469 6f6e 5f63 6f6c  abled_action_col
+000003a0: 6f72 7a11 4163 7469 6f6e 2043 6f6e 6469  orz.Action Condi
+000003b0: 7469 6f6e 73da 1661 6374 696f 6e5f 636f  tions..action_co
+000003c0: 6e64 6974 696f 6e5f 636f 6c6f 725a 0f41  ndition_colorZ.A
+000003d0: 6374 696f 6e43 6f6e 6469 7469 6f6e 7a12  ctionConditionz.
+000003e0: 5072 6f66 696c 6520 436f 6e64 6974 696f  Profile Conditio
+000003f0: 6e73 5a17 7072 6f66 696c 655f 636f 6e64  nsZ.profile_cond
+00000400: 6974 696f 6e5f 636f 6c6f 725a 1050 726f  ition_colorZ.Pro
+00000410: 6669 6c65 436f 6e64 6974 696f 6e7a 0d4c  fileConditionz.L
+00000420: 6175 6e63 6865 7220 5461 736b 5a13 6c61  auncher TaskZ.la
+00000430: 756e 6368 6572 5f74 6173 6b5f 636f 6c6f  uncher_task_colo
+00000440: 725a 0c4c 6175 6e63 6865 7254 6173 6b5a  rZ.LauncherTaskZ
+00000450: 0a42 6163 6b67 726f 756e 645a 1062 6163  .BackgroundZ.bac
+00000460: 6b67 726f 756e 645f 636f 6c6f 725a 0653  kground_colorZ.S
+00000470: 6365 6e65 73da 0b73 6365 6e65 5f63 6f6c  cenes..scene_col
+00000480: 6f72 5a05 5363 656e 655a 0742 756c 6c65  orZ.SceneZ.Bulle
+00000490: 7473 da0c 6275 6c6c 6574 5f63 6f6c 6f72  ts..bullet_color
+000004a0: 5a06 4275 6c6c 6574 7a0d 4163 7469 6f6e  Z.Bulletz.Action
+000004b0: 204c 6162 656c 73da 1261 6374 696f 6e5f   Labels..action_
+000004c0: 6c61 6265 6c5f 636f 6c6f 725a 0b41 6374  label_colorZ.Act
+000004d0: 696f 6e4c 6162 656c 7a0c 4163 7469 6f6e  ionLabelz.Action
+000004e0: 204e 616d 6573 da11 6163 7469 6f6e 5f6e   Names..action_n
+000004f0: 616d 655f 636f 6c6f 725a 0a41 6374 696f  ame_colorZ.Actio
+00000500: 6e4e 616d 657a 1554 6173 6b65 724e 6574  nNamez.TaskerNet
+00000510: 2049 6e66 6f72 6d61 7469 6f6e da0f 7461   Information..ta
+00000520: 736b 6572 6e65 745f 636f 6c6f 725a 0d54  skernet_colorZ.T
+00000530: 6173 6b65 724e 6574 496e 666f 7a12 5461  askerNetInfoz.Ta
+00000540: 736b 6572 2050 7265 6665 7265 6e63 6573  sker Preferences
+00000550: 5a11 7072 6566 6572 656e 6365 735f 636f  Z.preferences_co
+00000560: 6c6f 725a 0b50 7265 6665 7265 6e63 6573  lorZ.Preferences
+00000570: 7a11 5472 6169 6c69 6e67 2043 6f6d 6d65  z.Trailing Comme
+00000580: 6e74 735a 1774 7261 696c 696e 675f 636f  ntsZ.trailing_co
+00000590: 6d6d 656e 7473 5f63 6f6c 6f72 5a10 5472  mments_colorZ.Tr
+000005a0: 6169 6c69 6e67 436f 6d6d 656e 7473 7a0e  ailingCommentsz.
+000005b0: 5461 736b 2027 6163 7469 6f6e 7327 7a13  Task 'actions'z.
+000005c0: 2764 6973 6162 6c65 6427 2050 726f 6669  'disabled' Profi
+000005d0: 6c65 737a 0f27 756e 6b6e 6f77 6e27 2054  lesz.'unknown' T
+000005e0: 6173 6b73 7a17 6469 7361 626c 6564 2054  asksz.disabled T
+000005f0: 6173 6b20 2761 6374 696f 6e73 277a 1854  ask 'actions'z.T
+00000600: 6173 6b20 6163 7469 6f6e 2027 636f 6e64  ask action 'cond
+00000610: 6974 696f 6e73 277a 1450 726f 6669 6c65  itions'z.Profile
+00000620: 2027 636f 6e64 6974 696f 6e73 277a 1950   'conditions'z.P
+00000630: 726f 6a65 6374 2773 2027 6c61 756e 6368  roject's 'launch
+00000640: 6572 2720 5461 736b 7a11 6f75 7470 7574  er' Taskz.output
+00000650: 2062 6163 6b67 726f 756e 647a 0c6c 6973   backgroundz.lis
+00000660: 7420 6275 6c6c 6574 737a 1454 6173 6b20  t bulletsz.Task 
+00000670: 6163 7469 6f6e 2027 6c61 6265 6c73 277a  action 'labels'z
+00000680: 1354 6173 6b20 6163 7469 6f6e 2027 6e61  .Task action 'na
+00000690: 6d65 7327 7a17 5461 736b 6572 4e65 7420  mes'z.TaskerNet 
+000006a0: 2769 6e66 6f72 6d61 7469 6f6e 277a 1454  'information'z.T
+000006b0: 6173 6b65 7220 2770 7265 6665 7265 6e63  asker 'preferenc
+000006c0: 6573 275a 094d 6170 5461 736b 6572 4654  es'Z.MapTaskerFT
+000006d0: 2911 da14 6d61 7074 6173 6b65 722e 7372  )...maptasker.sr
+000006e0: 632e 636f 6e66 6967 7202 0000 005a 076c  c.configr....Z.l
+000006f0: 6f67 6769 6e67 da11 554e 4b4e 4f57 4e5f  ogging..UNKNOWN_
+00000700: 5441 534b 5f4e 414d 455a 0a4d 595f 5645  TASK_NAMEZ.MY_VE
+00000710: 5253 494f 4e5a 0a4d 595f 4c49 4345 4e53  RSIONZ.MY_LICENS
+00000720: 455a 0a4e 4f5f 5052 4f4a 4543 545a 0c43  EZ.NO_PROJECTZ.C
+00000730: 4f55 4e54 4552 5f46 494c 455a 0e41 5247  OUNTER_FILEZ.ARG
+00000740: 554d 454e 5453 5f46 494c 45da 0b46 4f4e  UMENTS_FILE..FON
+00000750: 545f 544f 5f55 5345 5a0a 4e4f 5f50 524f  T_TO_USEZ.NO_PRO
+00000760: 4649 4c45 5a14 5459 5045 535f 4f46 5f43  FILEZ.TYPES_OF_C
+00000770: 4f4c 4f52 5f4e 414d 4553 5a0f 5459 5045  OLOR_NAMESZ.TYPE
+00000780: 535f 4f46 5f43 4f4c 4f52 535a 0967 6574  S_OF_COLORSZ.get
+00000790: 4c6f 6767 6572 da06 6c6f 6767 6572 da09  Logger..logger..
+000007a0: 6465 6275 675f 6f75 745a 0d44 4542 5547  debug_outZ.DEBUG
+000007b0: 5f50 524f 4752 414d a900 7217 0000 0072  _PROGRAM..r....r
+000007c0: 1700 0000 fa77 2f55 7365 7273 2f6d 696b  .....w/Users/mik
+000007d0: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
+000007e0: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
+000007f0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
+00000800: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
+00000810: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
+00000820: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
+00000830: 632f 7379 7363 6f6e 7374 2e70 79da 083c  c/sysconst.py..<
+00000840: 6d6f 6475 6c65 3e01 0000 0073 ea00 0000  module>....s....
+00000850: 0c0d 0801 0403 0401 0401 0401 0401 0401  ................
+00000860: 0a01 0401 0207 0401 02ff 0402 02fe 0403  ................
+00000870: 02fd 0404 02fc 0405 02fb 0406 02fa 0407  ................
+00000880: 02f9 0408 02f8 0409 02f7 040a 02f6 040b  ................
+00000890: 02f5 040c 02f4 040d 02f3 040e 02f2 040f  ................
+000008a0: 02f1 0410 02f0 0411 04ef 0412 02ee 0413  ................
+000008b0: 02ed 0414 02ec 0415 02eb 0416 02ea 0417  ................
+000008c0: 02e9 0418 02e8 0419 02e7 041a 02e6 041b  ................
+000008d0: 02e5 041c 02e4 041d 02e3 041e 02e2 041f  ................
+000008e0: 02e1 0420 02e0 0421 06df 0225 0401 02ff  ... ...!...%....
+000008f0: 0402 02fe 0403 02fd 0404 02fc 0405 02fb  ................
+00000900: 0406 02fa 0407 02f9 0408 02f8 0409 02f7  ................
+00000910: 040a 02f6 040b 02f5 040c 02f4 040d 02f3  ................
+00000920: 040e 02f2 040f 02f1 0410 02f0 0411 02ef  ................
+00000930: 0412 06ee 0a15 0401 0801                 ..........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/taskactn.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/taskactn.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  3 19:11:00 2023 UTC, .py size: 5247 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,149 +1,155 @@
-00000000: 6f0d 0d0a 0000 0000 c424 2b64 7f14 0000  o........$+d....
+00000000: 6f0d 0d0a 0000 0000 f239 3864 bc16 0000  o........98d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
+00000020: 0012 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a04 0100 6400 6402 6c05 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 0100 6400 6403 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
-00000060: 6400 6404 6c07 6d09 5a09 0100 6405 6501  d.d.l.m.Z...d.e.
-00000070: 6a0a 6406 650b 650c 1900 6407 650d 6408  j.d.e.e...d.e.d.
-00000080: 650c 6409 650c 640a 650b 650c 1900 640b  e.d.e.d.e.e...d.
-00000090: 650d 640c 650d 640d 6401 6612 640e 640f  e.d.e.d.d.f.d.d.
-000000a0: 8404 5a0e 640b 650d 6407 650d 6406 650b  ..Z.d.e.d.e.d.e.
-000000b0: 6410 650f 6411 650b 6409 6501 6a0a 6a10  d.e.d.e.d.e.j.j.
-000000c0: 640d 6401 660e 6412 6413 8404 5a11 6401  d.d.f.d.d...Z.d.
-000000d0: 5300 2914 e900 0000 004e 2901 da09 6d79  S.)......N)...my
-000000e0: 5f6f 7574 7075 7429 01da 066c 6f67 6765  _output)...logge
-000000f0: 7229 01da 1155 4e4b 4e4f 574e 5f54 4153  r)...UNKNOWN_TAS
-00000100: 4b5f 4e41 4d45 da08 7468 655f 7461 736b  K_NAME..the_task
-00000110: da0b 6f75 7470 7574 5f6c 6973 74da 0c70  ..output_list..p
-00000120: 726f 6772 616d 5f61 7267 73da 096c 6973  rogram_args..lis
-00000130: 745f 7479 7065 da08 7468 655f 6974 656d  t_type..the_item
-00000140: da0b 7461 736b 735f 666f 756e 64da 0863  ..tasks_found..c
-00000150: 6f6c 6f72 6d61 70da 0961 6c6c 5f74 6173  olormap..all_tas
-00000160: 6b73 da06 7265 7475 726e 6308 0000 0000  ks..returnc.....
-00000170: 0000 0000 0000 000d 0000 0007 0000 0043  ...............C
-00000180: 0000 0073 f000 0000 7400 7c04 7600 730a  ...s....t.|.v.s.
-00000190: 7c02 6401 1900 6402 6b04 7276 6403 7c03  |.d...d.k.rvd.|.
-000001a0: 7600 7210 6404 6e04 7c04 a001 6405 a101  v.r.d.n.|...d...
-000001b0: 7d08 7402 7c08 8301 6406 6b04 7237 7c08  }.t.|...d.k.r7|.
-000001c0: 6406 1900 a001 6407 6406 a102 6402 1900  d.....d.d...d...
-000001d0: 7c08 6406 3c00 7403 a004 7c08 6406 1900  |.d.<.t...|.d...
-000001e0: 7c05 7c08 6406 1900 6701 6408 7c07 a105  |.|.d...g.d.|...
-000001f0: 5c02 7d00 7d09 7c00 726b 7403 a005 7c00  \.}.}.|.rkt...|.
-00000200: 7c06 7c02 a103 0400 7d0a 7269 7406 7c06  |.|.....}.rit.|.
-00000210: 7c02 7c01 6406 6408 8305 0100 6406 7d0b  |.|.d.d.....d.}.
-00000220: 7407 7c06 7c02 7c01 7c0b 7c0a 7c04 8306  t.|.|.|.|.|.|...
-00000230: 0100 6403 7c03 7600 7269 7406 7c06 7c02  ..d.|.v.rit.|.|.
-00000240: 7c01 6409 6408 8305 0100 7406 7c06 7c02  |.d.d.....t.|.|.
-00000250: 7c01 6409 6408 8305 0100 6400 5300 640a  |.d.d.....d.S.d.
-00000260: 7d0c 7408 a009 7c0c a101 0100 740a 7c0c  }.t...|.....t.|.
-00000270: 8301 0100 6400 5300 290b 4eda 1464 6973  ....d.S.).N..dis
-00000280: 706c 6179 5f64 6574 6169 6c5f 6c65 7665  play_detail_leve
-00000290: 6c72 0100 0000 7a0f 2623 3435 3b26 2334  lr....z.&#45;&#4
-000002a0: 353b 5461 736b 3ada 0178 7a09 5461 736b  5;Task:..xz.Task
-000002b0: 2049 443a 20e9 0100 0000 fa01 20da 00e9   ID: ....... ...
-000002c0: 0300 0000 7a17 4572 726f 723a 204e 6f20  ....z.Error: No 
-000002d0: 5461 736b 2066 6f75 6e64 2121 2129 0b72  Task found!!!).r
-000002e0: 0400 0000 da05 7370 6c69 74da 036c 656e  ......split..len
-000002f0: da05 7461 736b 73da 0d67 6574 5f74 6173  ..tasks..get_tas
-00000300: 6b5f 6e61 6d65 da0b 6765 745f 6163 7469  k_name..get_acti
-00000310: 6f6e 7372 0200 0000 da16 6f75 7470 7574  onsr......output
-00000320: 5f6c 6973 745f 6f66 5f61 6374 696f 6e73  _list_of_actions
-00000330: 7203 0000 00da 0564 6562 7567 da05 7072  r......debug..pr
-00000340: 696e 7429 0d72 0500 0000 7206 0000 0072  int).r....r....r
-00000350: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-00000360: 0000 0072 0b00 0000 720c 0000 005a 0774  ...r....r....Z.t
-00000370: 656d 705f 6964 da04 6b61 6b61 da05 616c  emp_id..kaka..al
-00000380: 6973 74da 0c61 6374 696f 6e5f 636f 756e  ist..action_coun
-00000390: 74da 0965 7272 6f72 5f6d 7367 a900 7220  t..error_msg..r 
-000003a0: 0000 00fa 772f 5573 6572 732f 6d69 6b72  ....w/Users/mikr
-000003b0: 7562 696e 2f4c 6962 7261 7279 2f43 6c6f  ubin/Library/Clo
-000003c0: 7564 5374 6f72 6167 652f 476f 6f67 6c65  udStorage/Google
-000003d0: 4472 6976 652d 6d69 6b72 7562 696e 4067  Drive-mikrubin@g
-000003e0: 6d61 696c 2e63 6f6d 2f4d 7920 4472 6976  mail.com/My Driv
-000003f0: 652f 5079 7468 6f6e 2f6d 6170 7461 736b  e/Python/maptask
-00000400: 6572 2f6d 6170 7461 736b 6572 2f73 7263  er/maptasker/src
-00000410: 2f74 6173 6b61 6374 6e2e 7079 da1b 6765  /taskactn.py..ge
-00000420: 745f 7461 736b 5f61 6374 696f 6e73 5f61  t_task_actions_a
-00000430: 6e64 5f6f 7574 7075 7419 0000 0073 3000  nd_output....s0.
-00000440: 0000 140b 1603 0c02 1801 0401 1401 08ff  ................
-00000450: 0404 1201 0201 0a01 04ff 0403 0201 0c01  ................
-00000460: 04ff 0804 1001 1001 0405 04fd 0a01 0801  ................
-00000470: 0401 7222 0000 0072 1e00 0000 721d 0000  ..r"...r....r...
-00000480: 0063 0600 0000 0000 0000 0000 0000 0700  .c..............
-00000490: 0000 0a00 0000 4300 0000 73ce 0000 007c  ......C...s....|
-000004a0: 0444 005d 5a7d 067c 0664 0175 0172 5c64  .D.]Z}.|.d.u.r\d
-000004b0: 027c 0676 0072 1574 007c 007c 017c 0264  .|.v.r.t.|.|.|.d
-000004c0: 037c 0683 0501 006e 2b7c 0664 0164 0485  .|.....n+|.d.d..
-000004d0: 0219 0064 056b 0272 2974 007c 007c 017c  ...d.k.r)t.|.|.|
-000004e0: 0264 0364 067c 069b 009d 0283 0501 006e  .d.d.|.........n
-000004f0: 1774 007c 007c 017c 0264 0364 0674 017c  .t.|.|.|.d.d.t.|
-00000500: 0383 01a0 0264 03a1 019b 0064 077c 069b  .....d.....d.|..
-00000510: 009d 0483 0501 007c 0364 0837 007d 037c  .......|.d.7.}.|
-00000520: 0364 036b 0272 507c 0164 0919 0064 0a6b  .d.k.rP|.d...d.k
-00000530: 0272 5074 037c 0576 0072 5001 006e 0d7c  .rPt.|.v.rP..n.|
-00000540: 0164 0919 0064 086b 0272 5c74 037c 0576  .d...d.k.r\t.|.v
-00000550: 0172 5c01 006e 0171 0274 007c 007c 017c  .r\..n.q.t.|.|.|
-00000560: 0264 0464 0b83 0501 0064 0153 0029 0c61  .d.d.....d.S.).a
-00000570: d801 0000 6f75 7470 7574 2074 6865 206c  ....output the l
-00000580: 6973 7420 6f66 2054 6173 6b20 4163 7469  ist of Task Acti
-00000590: 6f6e 730a 0a20 2020 2050 6172 616d 6574  ons..    Paramet
-000005a0: 6572 733a 0a20 2020 2020 2020 203a 7061  ers:.        :pa
-000005b0: 7261 6d20 636f 6c6f 726d 6170 3a20 6469  ram colormap: di
-000005c0: 6374 696f 6e61 7279 206f 6620 636f 6c6f  ctionary of colo
-000005d0: 7273 2074 6f20 7573 650a 2020 2020 2020  rs to use.      
-000005e0: 2020 3a70 6172 616d 2070 726f 6772 616d    :param program
-000005f0: 5f61 7267 733a 2064 6963 7469 6f6e 6172  _args: dictionar
-00000600: 7920 6f66 2070 726f 6772 616d 2072 756e  y of program run
-00000610: 7469 6d65 2061 7267 756d 656e 7473 0a20  time arguments. 
-00000620: 2020 2020 2020 203a 7061 7261 6d20 6f75         :param ou
-00000630: 7470 7574 5f6c 6973 743a 206c 6973 7420  tput_list: list 
-00000640: 696e 746f 2077 6869 6368 2074 6f20 6164  into which to ad
-00000650: 6420 7468 6520 6f75 7470 7574 206c 696e  d the output lin
-00000660: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
-00000670: 6d20 6163 7469 6f6e 5f63 6f75 6e74 3a20  m action_count: 
-00000680: 636f 756e 7420 6f66 2054 6173 6b20 6163  count of Task ac
-00000690: 7469 6f6e 730a 2020 2020 2020 2020 3a70  tions.        :p
-000006a0: 6172 616d 2061 6c69 7374 3a20 6c69 7374  aram alist: list
-000006b0: 206f 6620 7461 736b 2061 6374 696f 6e73   of task actions
-000006c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000006d0: 7468 655f 6974 656d 3a20 7468 6520 7370  the_item: the sp
-000006e0: 6563 6966 6963 2054 6173 6b27 7320 6465  ecific Task's de
-000006f0: 7461 696c 6564 206c 696e 650a 0a20 2020  tailed line..   
-00000700: 2052 6574 7572 6e73 3a20 7468 6520 636f   Returns: the co
-00000710: 756e 7420 6f66 2074 6865 206e 756d 6265  unt of the numbe
-00000720: 7220 6f66 2074 696d 6573 2074 6865 2070  r of times the p
-00000730: 726f 6772 616d 2068 6173 2062 6565 6e20  rogram has been 
-00000740: 6361 6c6c 6564 0a0a 2020 2020 4e7a 094c  called..    Nz.L
-00000750: 6162 656c 2066 6f72 e902 0000 0072 1300  abel for.....r..
-00000760: 0000 7a03 2e2e 2e7a 0841 6374 696f 6e3a  ..z....z.Action:
-00000770: 207a 0820 3c2f 7370 616e 3e72 1000 0000   z. </span>r....
-00000780: 720e 0000 0072 0100 0000 7212 0000 0029  r....r....r....)
-00000790: 0472 0200 0000 da03 7374 72da 057a 6669  .r......str..zfi
-000007a0: 6c6c 7204 0000 0029 0772 0b00 0000 7207  llr....).r....r.
-000007b0: 0000 0072 0600 0000 721e 0000 0072 1d00  ...r....r....r..
-000007c0: 0000 7209 0000 005a 0774 6163 7469 6f6e  ..r....Z.taction
-000007d0: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
-000007e0: 1900 0000 4600 0000 7330 0000 0008 1508  ....F...s0......
-000007f0: 0108 0112 0110 0118 0102 0202 0102 0102  ................
-00000800: 0102 0118 0104 fb08 0708 020c 0108 0104  ................
-00000810: 020c 0208 0104 0202 8010 0104 0172 1900  .............r..
-00000820: 0000 2912 da15 786d 6c2e 6574 7265 652e  ..)...xml.etree.
-00000830: 456c 656d 656e 7454 7265 65da 0378 6d6c  ElementTree..xml
-00000840: da13 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
-00000850: 7461 736b 73da 0373 7263 7216 0000 00da  tasks..srcr.....
-00000860: 156d 6170 7461 736b 6572 2e73 7263 2e6f  .maptasker.src.o
-00000870: 7574 7075 746c 7202 0000 00da 166d 6170  utputlr......map
-00000880: 7461 736b 6572 2e73 7263 2e73 7973 636f  tasker.src.sysco
-00000890: 6e73 7472 0300 0000 7204 0000 00da 0565  nstr....r......e
-000008a0: 7472 6565 da04 6c69 7374 7224 0000 00da  tree..listr$....
-000008b0: 0464 6963 7472 2200 0000 da03 696e 74da  .dictr".....int.
-000008c0: 0b45 6c65 6d65 6e74 5472 6565 7219 0000  .ElementTreer...
-000008d0: 0072 2000 0000 7220 0000 0072 2000 0000  .r ...r ...r ...
-000008e0: 7221 0000 00da 083c 6d6f 6475 6c65 3e01  r!.....<module>.
-000008f0: 0000 0073 4e00 0000 080d 1202 0c01 0c01  ...sN...........
-00000900: 0c01 0206 0401 02ff 0602 02fe 0203 02fd  ................
-00000910: 0204 02fc 0205 02fb 0606 02fa 0207 02f9  ................
-00000920: 0208 02f8 0209 0af7 022d 0201 02ff 0202  .........-......
-00000930: 02fe 0203 02fd 0204 02fc 0205 02fb 0606  ................
-00000940: 02fa 0207 0ef9                           ......
+00000060: 6400 6404 6c07 6d09 5a09 0100 6400 6405  d.d.l.m.Z...d.d.
+00000070: 6c0a 6d0b 5a0b 0100 6406 6501 6a0c 6a0d  l.m.Z...d.e.j.j.
+00000080: 6407 650e 650f 1900 6408 6510 6409 650f  d.e.e...d.e.d.e.
+00000090: 640a 650f 640b 650e 650f 1900 640c 6510  d.e.d.e.e...d.e.
+000000a0: 640d 6510 640e 6401 6612 640f 6410 8404  d.e.d.d.f.d.d...
+000000b0: 5a11 640c 6510 6408 6510 6407 650e 6411  Z.d.e.d.e.d.e.d.
+000000c0: 6512 6412 650e 640a 6501 6a0c 6a0d 640e  e.d.e.d.e.j.j.d.
+000000d0: 6401 660e 6413 6414 8404 5a13 6401 5300  d.f.d.d...Z.d.S.
+000000e0: 2915 e900 0000 004e 2901 da09 6d79 5f6f  )......N)...my_o
+000000f0: 7574 7075 7429 01da 066c 6f67 6765 7229  utput)...logger)
+00000100: 01da 1155 4e4b 4e4f 574e 5f54 4153 4b5f  ...UNKNOWN_TASK_
+00000110: 4e41 4d45 2901 da0b 666f 726d 6174 5f68  NAME)...format_h
+00000120: 746d 6cda 0874 6865 5f74 6173 6bda 0b6f  tml..the_task..o
+00000130: 7574 7075 745f 6c69 7374 da0c 7072 6f67  utput_list..prog
+00000140: 7261 6d5f 6172 6773 da09 6c69 7374 5f74  ram_args..list_t
+00000150: 7970 65da 0874 6865 5f69 7465 6dda 0b74  ype..the_item..t
+00000160: 6173 6b73 5f66 6f75 6e64 da08 636f 6c6f  asks_found..colo
+00000170: 726d 6170 da09 616c 6c5f 7461 736b 73da  rmap..all_tasks.
+00000180: 0672 6574 7572 6e63 0800 0000 0000 0000  .returnc........
+00000190: 0000 0000 0d00 0000 0700 0000 4300 0000  ............C...
+000001a0: 73f0 0000 0074 007c 0476 0073 0a7c 0264  s....t.|.v.s.|.d
+000001b0: 0119 0064 026b 0472 7664 037c 0376 0072  ...d.k.rvd.|.v.r
+000001c0: 1064 046e 047c 04a0 0164 05a1 017d 0874  .d.n.|...d...}.t
+000001d0: 027c 0883 0164 066b 0472 377c 0864 0619  .|...d.k.r7|.d..
+000001e0: 00a0 0164 0764 06a1 0264 0219 007c 0864  ...d.d...d...|.d
+000001f0: 063c 0074 03a0 047c 0864 0619 007c 057c  .<.t...|.d...|.|
+00000200: 0864 0619 0067 0164 087c 07a1 055c 027d  .d...g.d.|...\.}
+00000210: 007d 097c 0072 6b74 03a0 057c 007c 067c  .}.|.rkt...|.|.|
+00000220: 02a1 0304 007d 0a72 6974 067c 067c 027c  .....}.rit.|.|.|
+00000230: 0164 0664 0883 0501 0064 067d 0b74 077c  .d.d.....d.}.t.|
+00000240: 067c 027c 017c 0b7c 0a7c 0483 0601 0064  .|.|.|.|.|.....d
+00000250: 037c 0376 0072 6974 067c 067c 027c 0164  .|.v.rit.|.|.|.d
+00000260: 0964 0883 0501 0074 067c 067c 027c 0164  .d.....t.|.|.|.d
+00000270: 0964 0883 0501 0064 0053 0064 0a7d 0c74  .d.....d.S.d.}.t
+00000280: 08a0 097c 0ca1 0101 0074 0a7c 0c83 0101  ...|.....t.|....
+00000290: 0064 0053 0029 0b4e da14 6469 7370 6c61  .d.S.).N..displa
+000002a0: 795f 6465 7461 696c 5f6c 6576 656c 7201  y_detail_levelr.
+000002b0: 0000 007a 0f26 2334 353b 2623 3435 3b54  ...z.&#45;&#45;T
+000002c0: 6173 6b3a da01 787a 0954 6173 6b20 4944  ask:..xz.Task ID
+000002d0: 3a20 e901 0000 00fa 0120 da00 e903 0000  : ....... ......
+000002e0: 007a 1745 7272 6f72 3a20 4e6f 2054 6173  .z.Error: No Tas
+000002f0: 6b20 666f 756e 6421 2121 290b 7204 0000  k found!!!).r...
+00000300: 00da 0573 706c 6974 da03 6c65 6eda 0574  ...split..len..t
+00000310: 6173 6b73 da0d 6765 745f 7461 736b 5f6e  asks..get_task_n
+00000320: 616d 65da 0b67 6574 5f61 6374 696f 6e73  ame..get_actions
+00000330: 7202 0000 00da 166f 7574 7075 745f 6c69  r......output_li
+00000340: 7374 5f6f 665f 6163 7469 6f6e 7372 0300  st_of_actionsr..
+00000350: 0000 da05 6465 6275 67da 0570 7269 6e74  ....debug..print
+00000360: 290d 7206 0000 0072 0700 0000 7208 0000  ).r....r....r...
+00000370: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000380: 720c 0000 0072 0d00 0000 5a07 7465 6d70  r....r....Z.temp
+00000390: 5f69 64da 046b 616b 61da 0561 6c69 7374  _id..kaka..alist
+000003a0: da0c 6163 7469 6f6e 5f63 6f75 6e74 da09  ..action_count..
+000003b0: 6572 726f 725f 6d73 67a9 0072 2100 0000  error_msg..r!...
+000003c0: fa77 2f55 7365 7273 2f6d 696b 7275 6269  .w/Users/mikrubi
+000003d0: 6e2f 4c69 6272 6172 792f 436c 6f75 6453  n/Library/CloudS
+000003e0: 746f 7261 6765 2f47 6f6f 676c 6544 7269  torage/GoogleDri
+000003f0: 7665 2d6d 696b 7275 6269 6e40 676d 6169  ve-mikrubin@gmai
+00000400: 6c2e 636f 6d2f 4d79 2044 7269 7665 2f50  l.com/My Drive/P
+00000410: 7974 686f 6e2f 6d61 7074 6173 6b65 722f  ython/maptasker/
+00000420: 6d61 7074 6173 6b65 722f 7372 632f 7461  maptasker/src/ta
+00000430: 736b 6163 746e 2e70 79da 1b67 6574 5f74  skactn.py..get_t
+00000440: 6173 6b5f 6163 7469 6f6e 735f 616e 645f  ask_actions_and_
+00000450: 6f75 7470 7574 1a00 0000 7330 0000 0014  output....s0....
+00000460: 0b16 030c 0218 0104 0114 0108 ff04 0412  ................
+00000470: 0102 010a 0104 ff04 0302 010c 0104 ff08  ................
+00000480: 0410 0110 0104 0504 fd0a 0108 0104 0172  ...............r
+00000490: 2300 0000 721f 0000 0072 1e00 0000 6306  #...r....r....c.
+000004a0: 0000 0000 0000 0000 0000 0007 0000 000e  ................
+000004b0: 0000 0043 0000 0073 cc00 0000 7c04 4400  ...C...s....|.D.
+000004c0: 5d59 7d06 7c06 6401 7501 725b 7c06 6401  ]Y}.|.d.u.r[|.d.
+000004d0: 6402 8502 1900 6403 6b02 7222 7400 7c00  d.....d.k.r"t.|.
+000004e0: 7c01 7c02 6404 7401 7c00 6405 6406 6407  |.|.d.t.|.d.d.d.
+000004f0: 7c06 9b00 9d02 6408 8305 8305 0100 6e1d  |.....d.......n.
+00000500: 7400 7c00 7c01 7c02 6404 7401 7c00 6405  t.|.|.|.d.t.|.d.
+00000510: 6406 6407 7402 7c03 8301 a003 6404 a101  d.d.t.|.....d...
+00000520: 9b00 6409 7c06 9b00 9d04 6408 8305 8305  ..d.|.....d.....
+00000530: 0100 7c03 640a 3700 7d03 7c03 6404 6b02  ..|.d.7.}.|.d.k.
+00000540: 724f 7c01 640b 1900 640c 6b02 724f 7404  rO|.d...d.k.rOt.
+00000550: 7c05 7600 724f 0100 6e0d 7c01 640b 1900  |.v.rO..n.|.d...
+00000560: 640a 6b02 725b 7404 7c05 7601 725b 0100  d.k.r[t.|.v.r[..
+00000570: 6e01 7102 7400 7c00 7c01 7c02 6402 6406  n.q.t.|.|.|.d.d.
+00000580: 8305 0100 6401 5300 290d 61d8 0100 006f  ....d.S.).a....o
+00000590: 7574 7075 7420 7468 6520 6c69 7374 206f  utput the list o
+000005a0: 6620 5461 736b 2041 6374 696f 6e73 0a0a  f Task Actions..
+000005b0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+000005c0: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+000005d0: 6f6c 6f72 6d61 703a 2064 6963 7469 6f6e  olormap: diction
+000005e0: 6172 7920 6f66 2063 6f6c 6f72 7320 746f  ary of colors to
+000005f0: 2075 7365 0a20 2020 2020 2020 203a 7061   use.        :pa
+00000600: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
+00000610: 3a20 6469 6374 696f 6e61 7279 206f 6620  : dictionary of 
+00000620: 7072 6f67 7261 6d20 7275 6e74 696d 6520  program runtime 
+00000630: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
+00000640: 2020 3a70 6172 616d 206f 7574 7075 745f    :param output_
+00000650: 6c69 7374 3a20 6c69 7374 2069 6e74 6f20  list: list into 
+00000660: 7768 6963 6820 746f 2061 6464 2074 6865  which to add the
+00000670: 206f 7574 7075 7420 6c69 6e65 730a 2020   output lines.  
+00000680: 2020 2020 2020 3a70 6172 616d 2061 6374        :param act
+00000690: 696f 6e5f 636f 756e 743a 2063 6f75 6e74  ion_count: count
+000006a0: 206f 6620 5461 736b 2061 6374 696f 6e73   of Task actions
+000006b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000006c0: 616c 6973 743a 206c 6973 7420 6f66 2074  alist: list of t
+000006d0: 6173 6b20 6163 7469 6f6e 730a 2020 2020  ask actions.    
+000006e0: 2020 2020 3a70 6172 616d 2074 6865 5f69      :param the_i
+000006f0: 7465 6d3a 2074 6865 2073 7065 6369 6669  tem: the specifi
+00000700: 6320 5461 736b 2773 2064 6574 6169 6c65  c Task's detaile
+00000710: 6420 6c69 6e65 0a0a 2020 2020 5265 7475  d line..    Retu
+00000720: 726e 733a 2074 6865 2063 6f75 6e74 206f  rns: the count o
+00000730: 6620 7468 6520 6e75 6d62 6572 206f 6620  f the number of 
+00000740: 7469 6d65 7320 7468 6520 7072 6f67 7261  times the progra
+00000750: 6d20 6861 7320 6265 656e 2063 616c 6c65  m has been calle
+00000760: 640a 0a20 2020 204e 7214 0000 007a 032e  d..    Nr....z..
+00000770: 2e2e e902 0000 00da 0c61 6374 696f 6e5f  .........action_
+00000780: 636f 6c6f 7272 1300 0000 7a08 4163 7469  colorr....z.Acti
+00000790: 6f6e 3a20 467a 083c 2f73 7061 6e3e 2072  on: Fz.</span> r
+000007a0: 1100 0000 720f 0000 0072 0100 0000 2905  ....r....r....).
+000007b0: 7202 0000 0072 0500 0000 da03 7374 72da  r....r......str.
+000007c0: 057a 6669 6c6c 7204 0000 0029 0772 0c00  .zfillr....).r..
+000007d0: 0000 7208 0000 0072 0700 0000 721f 0000  ..r....r....r...
+000007e0: 0072 1e00 0000 720a 0000 005a 0774 6163  .r....r....Z.tac
+000007f0: 7469 6f6e 7221 0000 0072 2100 0000 7222  tionr!...r!...r"
+00000800: 0000 0072 1a00 0000 4700 0000 7348 0000  ...r....G...sH..
+00000810: 0008 1508 0110 0302 0102 0102 0102 0102  ................
+00000820: 0102 0110 0102 ff06 fb02 0b02 0102 0102  ................
+00000830: 0102 0102 0102 0102 0102 0118 0102 0102  ................
+00000840: fb04 fb08 0d08 020c 0108 0104 020c 0208  ................
+00000850: 0104 0202 8010 0104 0172 1a00 0000 2914  .........r....).
+00000860: da16 6465 6675 7365 6478 6d6c 2e45 6c65  ..defusedxml.Ele
+00000870: 6d65 6e74 5472 6565 da0a 6465 6675 7365  mentTree..defuse
+00000880: 6478 6d6c da13 6d61 7074 6173 6b65 722e  dxml..maptasker.
+00000890: 7372 632e 7461 736b 73da 0373 7263 7217  src.tasks..srcr.
+000008a0: 0000 00da 156d 6170 7461 736b 6572 2e73  .....maptasker.s
+000008b0: 7263 2e6f 7574 7075 746c 7202 0000 00da  rc.outputlr.....
+000008c0: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
+000008d0: 7973 636f 6e73 7472 0300 0000 7204 0000  ysconstr....r...
+000008e0: 00da 166d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+000008f0: 2e66 726d 7468 746d 6c72 0500 0000 da0b  .frmthtmlr......
+00000900: 456c 656d 656e 7454 7265 65da 0358 4d4c  ElementTree..XML
+00000910: da04 6c69 7374 7226 0000 00da 0464 6963  ..listr&.....dic
+00000920: 7472 2300 0000 da03 696e 7472 1a00 0000  tr#.....intr....
+00000930: 7221 0000 0072 2100 0000 7221 0000 0072  r!...r!...r!...r
+00000940: 2200 0000 da08 3c6d 6f64 756c 653e 0100  ".....<module>..
+00000950: 0000 7350 0000 0008 0d12 020c 010c 010c  ..sP............
+00000960: 010c 0102 0606 0102 ff06 0202 fe02 0302  ................
+00000970: fd02 0402 fc02 0502 fb06 0602 fa02 0702  ................
+00000980: f902 0802 f802 090a f702 2d02 0102 ff02  ..........-.....
+00000990: 0202 fe02 0302 fd02 0402 fc02 0502 fb06  ................
+000009a0: 0602 fa02 070e f9                        .......
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/tasks.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/tasks.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 15:44:52 2023 UTC, .py size: 15228 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,497 +1,501 @@
-00000000: 6f0d 0d0a 0000 0000 f445 2c64 7c3b 0000  o........E,d|;..
+00000000: 6f0d 0d0a 0000 0000 2b49 3c64 093c 0000  o.......+I<d.<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 001c 0000 0040 0000 0073 9601 0000 6400  .....@...s....d.
+00000020: 001c 0000 0040 0000 0073 9e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 6d03  ..m.Z...d.d.l.m.
 00000050: 0200 0100 6d07 5a08 0100 6400 6402 6c09  ....m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6400 6403 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6404 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6405 6c0f 6d10 5a10 0100 6400 6406 6c11  d.l.m.Z...d.d.l.
 00000090: 6d12 5a12 0100 6400 6407 6c11 6d13 5a13  m.Z...d.d.l.m.Z.
 000000a0: 0100 6400 6408 6c11 6d14 5a14 0100 6400  ..d.d.l.m.Z...d.
 000000b0: 6409 6c15 6d16 5a16 0100 640a 6501 6a17  d.l.m.Z...d.e.j.
-000000c0: 640b 6518 640c 6518 640d 6519 6608 640e  d.e.d.e.d.e.f.d.
-000000d0: 640f 8404 5a1a 6410 651b 6411 6519 6412  d...Z.d.e.d.e.d.
-000000e0: 6519 6413 651b 6414 6518 640d 651c 6501  e.d.e.d.e.d.e.e.
-000000f0: 6a17 651b 6602 1900 660c 6415 6416 8404  j.e.f...f.d.d...
-00000100: 5a1d 6410 651b 6417 6519 6418 6518 640d  Z.d.e.d.e.d.e.d.
-00000110: 651c 651b 6501 6a17 6602 1900 6608 6419  e.e.e.j.f...f.d.
-00000120: 641a 8404 5a1e 6410 651b 641b 6518 640d  d...Z.d.e.d.e.d.
-00000130: 651f 6606 641c 641d 8404 5a20 641e 651b  e.f.d.d...Z d.e.
-00000140: 641f 6519 6420 651b 6421 651b 6422 651b  d.e.d e.d!e.d"e.
-00000150: 6423 6518 6424 6519 6425 6501 6a17 6426  d#e.d$e.d%e.j.d&
-00000160: 6519 6427 6518 640b 6518 6428 6518 640d  e.d'e.d.e.d(e.d.
-00000170: 6401 661a 6429 642a 8404 5a21 641f 6519  d.f.d)d*..Z!d.e.
-00000180: 641e 651b 6425 6501 6a17 6424 6519 6420  d.e.d%e.j.d$e.d 
-00000190: 651b 6421 651b 6426 6519 6422 651b 640b  e.d!e.d&e.d"e.d.
-000001a0: 6518 6428 6518 6427 6518 6423 6518 642b  e.d(e.d'e.d#e.d+
-000001b0: 651f 640d 651f 661c 642c 642d 8404 5a22  e.d.e.f.d,d-..Z"
-000001c0: 6401 5300 292e e900 0000 004e 2901 da0b  d.S.)......N)...
-000001d0: 7461 675f 696e 5f74 7970 6529 01da 0b67  tag_in_type)...g
-000001e0: 6574 5f6b 6964 5f61 7070 2901 da0c 6765  et_kid_app)...ge
-000001f0: 745f 7072 696f 7269 7479 2901 da07 6765  t_priority)...ge
-00000200: 745f 6964 7329 01da 1155 4e4b 4e4f 574e  t_ids)...UNKNOWN
-00000210: 5f54 4153 4b5f 4e41 4d45 2901 da0a 4e4f  _TASK_NAME)...NO
-00000220: 5f50 524f 4a45 4354 2901 da06 6c6f 6767  _PROJECT)...logg
-00000230: 6572 2901 da0a 7368 656c 6c5f 736f 7274  er)...shell_sort
-00000240: da0c 6375 7272 656e 745f 7461 736b da08  ..current_task..
-00000250: 636f 6c6f 726d 6170 da09 7072 6f67 5f61  colormap..prog_a
-00000260: 7267 73da 0672 6574 7572 6e63 0300 0000  rgs..returnc....
-00000270: 0000 0000 0000 0000 0d00 0000 0a00 0000  ................
-00000280: 4300 0000 7352 0100 0067 007d 037a 077c  C...sR...g.}.z.|
-00000290: 00a0 0064 01a1 017d 0457 006e 2304 0074  ...d...}.W.n#..t
-000002a0: 0179 2c01 007d 0501 007a 1774 027c 0083  .y,..}...z.t.|..
-000002b0: 0101 0064 027d 0674 027c 0683 0101 0074  ...d.}.t.|.....t
-000002c0: 03a0 047c 06a1 0101 0067 0057 0006 0059  ...|.....g.W...Y
-000002d0: 0064 037d 057e 0553 0064 037d 057e 0577  .d.}.~.S.d.}.~.w
-000002e0: 0177 007c 0472 a764 047d 0764 057d 0874  .w.|.r.d.}.d.}.t
-000002f0: 057c 0483 0164 056b 0472 3f74 067c 0464  .|...d.k.r?t.|.d
-00000300: 0664 0783 0301 007c 0444 005d 657d 097c  .d.....|.D.]e}.|
-00000310: 09a0 0764 08a1 017d 0a74 08a0 097c 0a7c  ...d...}.t...|.|
-00000320: 0964 067c 0164 097c 02a1 067d 0b74 03a0  .d.|.d.|...}.t..
-00000330: 0464 0a74 0a7c 096a 0b64 0b19 0083 0117  .d.t.|.j.d......
-00000340: 0064 0c17 007c 0a6a 0c17 0064 0d17 007c  .d...|.j...d...|
-00000350: 0b17 0064 0e17 0074 0a7c 096a 0b83 0117  ...d...t.|.j....
-00000360: 00a1 0101 0064 0f7c 0b76 0073 7a64 107c  .....d.|.v.szd.|
-00000370: 0b76 0073 7a64 117c 0b76 0072 887c 0864  .v.szd.|.v.r.|.d
-00000380: 1238 007d 0874 057c 0783 017d 0c7c 0764  .8.}.t.|...}.|.d
-00000390: 137c 0c85 0219 007d 0774 08a0 0d7c 037c  .|.....}.t...|.|
-000003a0: 0b7c 0a7c 087c 07a1 0501 0064 147c 0b76  .|.|.|.....d.|.v
-000003b0: 0073 9d64 107c 0b76 0073 9d64 157c 0b76  .s.d.|.v.s.d.|.v
-000003c0: 0072 a67c 0864 1237 007d 087c 079b 0064  .r.|.d.7.}.|...d
-000003d0: 169d 027d 0771 417c 0353 0029 1761 1d01  ...}.qA|.S.).a..
-000003e0: 0000 0a20 2020 2052 6574 7572 6e20 6120  ...    Return a 
-000003f0: 6c69 7374 206f 6620 5461 736b 2773 2061  list of Task's a
-00000400: 6374 696f 6e73 2066 6f72 2074 6865 2067  ctions for the g
-00000410: 6976 656e 2054 6173 6b0a 2020 2020 2020  iven Task.      
-00000420: 2020 3a70 6172 616d 2063 7572 7265 6e74    :param current
-00000430: 5f74 6173 6b3a 2078 6d6c 2065 6c65 6d65  _task: xml eleme
-00000440: 6e74 206f 6620 7468 6520 5461 736b 2077  nt of the Task w
-00000450: 6520 6172 6520 6765 7474 696e 6720 6163  e are getting ac
-00000460: 7469 6f6e 7320 666f 720a 2020 2020 2020  tions for.      
-00000470: 2020 3a70 6172 616d 2063 6f6c 6f72 6d61    :param colorma
-00000480: 703a 2063 6f6c 6f72 7320 746f 2075 7365  p: colors to use
-00000490: 2069 6e20 6f75 7470 7574 0a20 2020 2020   in output.     
-000004a0: 2020 203a 7061 7261 6d20 7072 6f67 5f61     :param prog_a
-000004b0: 7267 733a 2072 756e 7469 6d65 2061 7267  rgs: runtime arg
-000004c0: 756d 656e 7473 0a20 2020 2020 2020 203a  uments.        :
-000004d0: 7265 7475 726e 3a20 6c69 7374 206f 6620  return: list of 
-000004e0: 5461 736b 2027 6163 7469 6f6e 2720 6f75  Task 'action' ou
-000004f0: 7470 7574 206c 696e 6573 0a20 2020 20da  tput lines.    .
-00000500: 0641 6374 696f 6e7a 1945 7272 6f72 3a20  .Actionz.Error: 
-00000510: 4e6f 2061 6374 696f 6e20 666f 756e 6421  No action found!
-00000520: 2121 4eda 0072 0100 0000 5446 da04 636f  !!N..r....TF..co
-00000530: 6465 da01 747a 0854 6173 6b20 4944 3ada  de..tz.Task ID:.
-00000540: 0273 727a 0620 436f 6465 3a7a 0b20 7461  .srz. Code:z. ta
-00000550: 736b 5f63 6f64 653a 7a0c 4163 7469 6f6e  sk_code:z.Action
-00000560: 2061 7474 723a 7a07 3e45 6e64 2049 667a   attr:z.>End Ifz
-00000570: 053e 456c 7365 7a08 3e45 6e64 2046 6f72  .>Elsez.>End For
-00000580: e901 0000 00e9 1800 0000 7a03 3e49 667a  ..........z.>Ifz
-00000590: 043e 466f 727a 1826 6e62 7370 3b26 6e62  .>Forz.&nbsp;&nb
-000005a0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b29  sp;&nbsp;&nbsp;)
-000005b0: 0eda 0766 696e 6461 6c6c da09 4578 6365  ...findall..Exce
-000005c0: 7074 696f 6eda 0570 7269 6e74 7208 0000  ption..printr...
-000005d0: 00da 0564 6562 7567 da03 6c65 6e72 0900  ...debug..lenr..
-000005e0: 0000 da04 6669 6e64 da0f 6163 7469 6f6e  ....find..action
-000005f0: 5f65 7661 6c75 6174 65da 0f67 6574 5f61  _evaluate..get_a
-00000600: 6374 696f 6e5f 636f 6465 da03 7374 72da  ction_code..str.
-00000610: 0661 7474 7269 62da 0474 6578 74da 0c62  .attrib..text..b
-00000620: 7569 6c64 5f61 6374 696f 6e29 0d72 0a00  uild_action).r..
-00000630: 0000 720b 0000 0072 0c00 0000 5a08 7461  ..r....r....Z.ta
-00000640: 736b 6c69 7374 5a0c 7461 736b 5f61 6374  sklistZ.task_act
-00000650: 696f 6e73 da01 65da 0965 7272 6f72 5f6d  ions..e..error_m
-00000660: 7367 5a12 696e 6465 6e74 6174 696f 6e5f  sgZ.indentation_
-00000670: 616d 6f75 6e74 5a0b 696e 6465 6e74 6174  amountZ.indentat
-00000680: 696f 6eda 0661 6374 696f 6eda 0563 6869  ion..action..chi
-00000690: 6c64 5a09 7461 736b 5f63 6f64 655a 0d6c  ldZ.task_codeZ.l
-000006a0: 656e 6774 685f 696e 6465 6e74 a900 7225  ength_indent..r%
-000006b0: 0000 00fa 742f 5573 6572 732f 6d69 6b72  ....t/Users/mikr
-000006c0: 7562 696e 2f4c 6962 7261 7279 2f43 6c6f  ubin/Library/Clo
-000006d0: 7564 5374 6f72 6167 652f 476f 6f67 6c65  udStorage/Google
-000006e0: 4472 6976 652d 6d69 6b72 7562 696e 4067  Drive-mikrubin@g
-000006f0: 6d61 696c 2e63 6f6d 2f4d 7920 4472 6976  mail.com/My Driv
-00000700: 652f 5079 7468 6f6e 2f6d 6170 7461 736b  e/Python/maptask
-00000710: 6572 2f6d 6170 7461 736b 6572 2f73 7263  er/maptasker/src
-00000720: 2f74 6173 6b73 2e70 79da 0b67 6574 5f61  /tasks.py..get_a
-00000730: 6374 696f 6e73 2100 0000 7368 0000 0004  ctions!...sh....
-00000740: 0802 020e 010e 0108 0104 0108 010a 0110  ................
-00000750: 0108 8002 fb04 0604 0104 010c 030c 0108  ................
-00000760: 020a 0104 020c 0104 ff04 0302 010c 0102  ................
-00000770: ff02 0202 fe04 0302 fd02 0402 fc02 0502  ................
-00000780: fb02 0602 fa08 0702 f904 ff08 0c08 0108  ................
-00000790: 0108 0208 010c 0104 010a 0104 ff18 0408  ................
-000007a0: 020a 0102 8004 0272 2700 0000 da0b 7468  .......r'.....th
-000007b0: 655f 7461 736b 5f69 64da 1a74 6173 6b73  e_task_id..tasks
-000007c0: 5f74 6861 745f 6861 7665 5f62 6565 6e5f  _that_have_been_
-000007d0: 666f 756e 64da 1174 6173 6b5f 6f75 7470  found..task_outp
-000007e0: 7574 5f6c 696e 6573 da09 7461 736b 5f74  ut_lines..task_t
-000007f0: 7970 65da 0961 6c6c 5f74 6173 6b73 6305  ype..all_tasksc.
-00000800: 0000 0000 0000 0000 0000 0009 0000 000a  ................
-00000810: 0000 0043 0000 0073 fa00 0000 7c00 a000  ...C...s....|...
-00000820: a100 7275 7c04 7c00 1900 7d05 7c01 a001  ..ru|.|...}.|...
-00000830: 7c00 a101 0100 6401 7c00 9b00 9d02 7d06  |.....d.|.....}.
-00000840: 7a29 7c05 a002 6402 a101 6a03 7d07 7c03  z)|...d...j.}.|.
-00000850: 6403 6b02 7228 7c02 a001 7c07 9b00 6404  d.k.r(|...|...d.
-00000860: 7c06 9b00 9d03 a101 0100 6e0f 7c02 a001  |.........n.|...
-00000870: 7c07 9b00 6405 7c06 9b00 9d03 a101 0100  |...d.|.........
-00000880: 5700 7c05 7c07 6602 5300 5700 7c05 7c07  W.|.|.f.S.W.|.|.
-00000890: 6602 5300 0400 7404 7974 0100 7d08 0100  f.S...t.yt..}...
-000008a0: 7a2d 7405 7d07 7c03 6403 6b02 7254 7c02  z-t.}.|.d.k.rT|.
-000008b0: a001 7405 9b00 6404 7c06 9b00 9d03 a101  ..t...d.|.......
-000008c0: 0100 6e13 7c02 a001 7405 9b00 6405 7c06  ..n.|...t...d.|.
-000008d0: 9b00 9d03 a101 0100 5700 5900 6406 7d08  ........W.Y.d.}.
-000008e0: 7e08 7c05 7c07 6602 5300 5700 5900 6406  ~.|.|.f.S.W.Y.d.
-000008f0: 7d08 7e08 7c05 7c07 6602 5300 6406 7d08  }.~.|.|.f.S.d.}.
-00000900: 7e08 7701 7700 6406 7d05 6407 7d07 7c05  ~.w.w.d.}.d.}.|.
-00000910: 7c07 6602 5300 2908 6178 0100 000a 2020  |.f.S.).ax....  
-00000920: 2020 4765 7420 7468 6520 6e61 6d65 206f    Get the name o
-00000930: 6620 7468 6520 7461 736b 2067 6976 656e  f the task given
-00000940: 2074 6865 2054 6173 6b20 4944 0a20 2020   the Task ID.   
-00000950: 2020 2020 203a 7061 7261 6d20 7468 655f       :param the_
-00000960: 7461 736b 5f69 643a 2074 6865 2054 6173  task_id: the Tas
-00000970: 6b27 7320 4944 2028 652e 672e 2027 3437  k's ID (e.g. '47
-00000980: 2729 0a20 2020 2020 2020 203a 7061 7261  ').        :para
-00000990: 6d20 7461 736b 735f 7468 6174 5f68 6176  m tasks_that_hav
-000009a0: 655f 6265 656e 5f66 6f75 6e64 3a20 6c69  e_been_found: li
-000009b0: 7374 206f 6620 5461 736b 7320 666f 756e  st of Tasks foun
-000009c0: 6420 736f 2066 6172 0a20 2020 2020 2020  d so far.       
-000009d0: 203a 7061 7261 6d20 7461 736b 5f6f 7574   :param task_out
-000009e0: 7075 745f 6c69 6e65 733a 206c 6973 7420  put_lines: list 
-000009f0: 6f66 2054 6173 6b73 0a20 2020 2020 2020  of Tasks.       
-00000a00: 203a 7061 7261 6d20 7461 736b 5f74 7970   :param task_typ
-00000a10: 653a 2054 7970 6520 6f66 2054 6173 6b20  e: Type of Task 
-00000a20: 2845 6e74 7279 2c20 4578 6974 2c20 5363  (Entry, Exit, Sc
-00000a30: 656e 6529 0a20 2020 2020 2020 203a 7061  ene).        :pa
-00000a40: 7261 6d20 616c 6c5f 7461 736b 733a 2061  ram all_tasks: a
-00000a50: 6c6c 2054 6173 6b73 2069 6e20 786d 6c0a  ll Tasks in xml.
-00000a60: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000a70: 2054 6173 6b27 7320 786d 6c20 656c 656d   Task's xml elem
-00000a80: 656e 742c 2054 6173 6b27 7320 6e61 6d65  ent, Task's name
-00000a90: 0a20 2020 207a 1526 6e62 7370 3b26 6e62  .    z.&nbsp;&nb
-00000aa0: 7370 3b54 6173 6b20 4944 3a20 da03 6e6d  sp;Task ID: ..nm
-00000ab0: 65da 0445 7869 747a 2526 6e62 7370 3b26  e..Exitz%&nbsp;&
-00000ac0: 6e62 7370 3b26 6e62 7370 3b26 6e62 7370  nbsp;&nbsp;&nbsp
-00000ad0: 3b3c 3c3c 2045 7869 7420 5461 736b 7a26  ;<<< Exit Taskz&
-00000ae0: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
-00000af0: 703b 266e 6273 703b 3c3c 3c20 456e 7472  p;&nbsp;<<< Entr
-00000b00: 7920 5461 736b 4e72 0f00 0000 2906 da07  y TaskNr....)...
-00000b10: 6973 6469 6769 74da 0661 7070 656e 6472  isdigit..appendr
-00000b20: 1a00 0000 721f 0000 0072 1600 0000 7206  ....r....r....r.
-00000b30: 0000 0029 0972 2800 0000 7229 0000 0072  ...).r(...r)...r
-00000b40: 2a00 0000 722b 0000 0072 2c00 0000 da04  *...r+...r,.....
-00000b50: 7461 736b da05 6578 7472 61da 0974 6173  task..extra..tas
-00000b60: 6b5f 6e61 6d65 7221 0000 0072 2500 0000  k_namer!...r%...
-00000b70: 7225 0000 0072 2600 0000 da0d 6765 745f  r%...r&.....get_
-00000b80: 7461 736b 5f6e 616d 6564 0000 0073 4200  task_named...sB.
-00000b90: 0000 0810 0801 0a01 0a01 0201 0c01 0801  ................
-00000ba0: 0401 0c01 06ff 0405 0c01 06ff 0812 02e9  ................
-00000bb0: 0817 0ef1 0401 0801 0401 0c01 06ff 0405  ................
-00000bc0: 0c01 0eff 0807 0af4 080c 0880 02f1 040c  ................
-00000bd0: 0401 0802 7234 0000 00da 1670 726f 6a65  ....r4.....proje
-00000be0: 6374 735f 7769 7468 5f6e 6f5f 7461 736b  cts_with_no_task
-00000bf0: 73da 0c61 6c6c 5f70 726f 6a65 6374 7363  s..all_projectsc
-00000c00: 0300 0000 0000 0000 0000 0000 0600 0000  ................
-00000c10: 0900 0000 4300 0000 7356 0000 0074 007d  ....C...sV...t.}
-00000c20: 0364 017d 047c 0264 0175 0172 277c 0244  .d.}.|.d.u.r'|.D
-00000c30: 005d 1c7d 047c 04a0 0164 02a1 016a 027d  .].}.|...d...j.}
-00000c40: 0374 0364 0369 0069 0067 007c 047c 037c  .t.d.i.i.g.|.|.|
-00000c50: 0183 077d 057c 007c 0576 0072 267c 037c  ...}.|.|.v.r&|.|
-00000c60: 0466 0202 0001 0053 0071 0a7c 037c 0466  .f.....S.q.|.|.f
-00000c70: 0253 0029 0461 4b01 0000 0a20 2020 2046  .S.).aK....    F
-00000c80: 696e 6420 7468 6520 5072 6f6a 6563 7420  ind the Project 
-00000c90: 6265 6c6f 6e67 696e 6720 746f 2074 6865  belonging to the
-00000ca0: 2054 6173 6b20 6964 2070 6173 7365 6420   Task id passed 
-00000cb0: 696e 0a20 2020 2020 2020 203a 7061 7261  in.        :para
-00000cc0: 6d20 7468 655f 7461 736b 5f69 643a 2074  m the_task_id: t
-00000cd0: 6865 2049 4420 6f66 2074 6865 2054 6173  he ID of the Tas
-00000ce0: 6b0a 2020 2020 2020 2020 3a70 6172 616d  k.        :param
-00000cf0: 2070 726f 6a65 6374 735f 7769 7468 5f6e   projects_with_n
-00000d00: 6f5f 7461 736b 733a 206c 6973 7420 6f66  o_tasks: list of
-00000d10: 2050 726f 6a65 6374 7320 7468 6174 2064   Projects that d
-00000d20: 6f20 6e6f 7420 6861 7665 2061 6e79 2054  o not have any T
-00000d30: 6173 6b73 0a20 2020 2020 2020 203a 7061  asks.        :pa
-00000d40: 7261 6d20 616c 6c5f 7072 6f6a 6563 7473  ram all_projects
-00000d50: 3a20 616c 6c20 5461 736b 6572 2050 726f  : all Tasker Pro
-00000d60: 6a65 6374 730a 2020 2020 2020 2020 3a72  jects.        :r
-00000d70: 6574 7572 6e3a 206e 616d 6520 6f66 2074  eturn: name of t
-00000d80: 6865 2050 726f 6a65 6374 2074 6861 7420  he Project that 
-00000d90: 6265 6c6f 6e67 7320 746f 2074 6869 7320  belongs to this 
-00000da0: 7461 736b 2061 6e64 2074 6865 2050 726f  task and the Pro
-00000db0: 6a65 6374 2078 6d6c 2065 6c65 6d65 6e74  ject xml element
-00000dc0: 0a20 2020 204e da04 6e61 6d65 4629 0472  .    N..nameF).r
-00000dd0: 0700 0000 721a 0000 0072 1f00 0000 7205  ....r....r....r.
-00000de0: 0000 0029 0672 2800 0000 7235 0000 0072  ...).r(...r5...r
-00000df0: 3600 0000 5a09 7072 6f6a 5f6e 616d 65da  6...Z.proj_name.
-00000e00: 0770 726f 6a65 6374 da08 7461 736b 5f69  .project..task_i
-00000e10: 6473 7225 0000 0072 2500 0000 7226 0000  dsr%...r%...r&..
-00000e20: 00da 1967 6574 5f70 726f 6a65 6374 5f66  ...get_project_f
-00000e30: 6f72 5f73 6f6c 6f5f 7461 736b 9800 0000  or_solo_task....
-00000e40: 7318 0000 0004 0a04 0108 0108 020c 0102  s...............
-00000e50: 010e 0104 ff08 030c 0102 ff08 0272 3a00  .............r:.
-00000e60: 0000 da0a 616c 6c5f 7363 656e 6573 6302  ....all_scenesc.
-00000e70: 0000 0000 0000 0000 0000 0005 0000 0006  ................
-00000e80: 0000 0043 0000 0073 6000 0000 7c01 a000  ...C...s`...|...
-00000e90: a100 4400 5d29 7d02 7c02 4400 5d24 7d03  ..D.])}.|.D.]$}.
-00000ea0: 7401 7c03 6a02 6401 8302 722c 7c03 4400  t.|.j.d...r,|.D.
-00000eb0: 5d19 7d04 7401 7c04 6a02 6402 8302 7224  ].}.t.|.j.d...r$
-00000ec0: 7c00 7c04 6a03 6b02 7224 0100 0100 0100  |.|.j.k.r$......
-00000ed0: 6401 5300 7c03 6a02 6403 6b02 722b 0100  d.S.|.j.d.k.r+..
-00000ee0: 6e01 7112 7108 7104 6402 5300 2904 6118  n.q.q.q.d.S.).a.
-00000ef0: 0100 000a 2020 2020 4964 656e 7469 6679  ....    Identify
-00000f00: 2077 6865 7468 6572 2074 6865 2054 6173   whether the Tas
-00000f10: 6b20 7061 7373 6564 2069 6e20 6973 2070  k passed in is p
-00000f20: 6172 7420 6f66 2061 2053 6365 6e65 3a20  art of a Scene: 
-00000f30: 5472 7565 203d 2079 6573 2c20 4661 6c73  True = yes, Fals
-00000f40: 6520 3d20 6e6f 0a20 2020 2020 2020 203a  e = no.        :
-00000f50: 7061 7261 6d20 7468 655f 7461 736b 5f69  param the_task_i
-00000f60: 643a 2074 6865 2069 6420 6f66 2074 6865  d: the id of the
-00000f70: 2054 6173 6b20 746f 2063 6865 636b 2061   Task to check a
-00000f80: 6761 696e 7374 0a20 2020 2020 2020 203a  gainst.        :
-00000f90: 7061 7261 6d20 616c 6c5f 7363 656e 6573  param all_scenes
-00000fa0: 3a20 616c 6c20 5363 656e 6573 2069 6e20  : all Scenes in 
-00000fb0: 5461 736b 6572 2063 6f6e 6669 6775 7261  Tasker configura
-00000fc0: 7469 6f6e 0a20 2020 2020 2020 203a 7265  tion.        :re
-00000fd0: 7475 726e 3a20 5472 7565 2069 6620 5461  turn: True if Ta
-00000fe0: 736b 2069 7320 7061 7274 206f 6620 6120  sk is part of a 
-00000ff0: 5363 656e 652c 2046 616c 7365 206f 7468  Scene, False oth
-00001000: 6572 7769 7365 0a20 2020 2054 46da 0353  erwise.    TF..S
-00001010: 7472 2904 da06 7661 6c75 6573 7202 0000  tr)...valuesr...
-00001020: 00da 0374 6167 721f 0000 0029 0572 2800  ...tagr....).r(.
-00001030: 0000 723b 0000 00da 0576 616c 7565 7224  ..r;.....valuer$
-00001040: 0000 005a 0873 7562 6368 696c 6472 2500  ...Z.subchildr%.
-00001050: 0000 7225 0000 0072 2600 0000 da0d 7461  ..r%...r&.....ta
-00001060: 736b 5f69 6e5f 7363 656e 65b3 0000 0073  sk_in_scene....s
-00001070: 1c00 0000 0c08 0801 0c01 0801 0a03 02ff  ................
-00001080: 0a02 0a02 0a01 0401 0202 0280 02f4 040d  ................
-00001090: 7240 0000 00da 0d6f 7572 5f74 6173 6b5f  r@.....our_task_
-000010a0: 6e61 6d65 da0b 6f75 7470 7574 5f6c 6973  name..output_lis
-000010b0: 74da 0c70 726f 6a65 6374 5f6e 616d 65da  t..project_name.
-000010c0: 0c70 726f 6669 6c65 5f6e 616d 65da 0768  .profile_name..h
-000010d0: 6561 6469 6e67 da0b 666f 756e 645f 6974  eading..found_it
-000010e0: 656d 73da 0974 6173 6b5f 6c69 7374 da10  ems..task_list..
-000010f0: 6f75 725f 7461 736b 5f65 6c65 6d65 6e74  our_task_element
-00001100: da13 6c69 7374 5f6f 665f 666f 756e 645f  ..list_of_found_
-00001110: 7461 736b 73da 1061 6c6c 5f74 6173 6b65  tasks..all_taske
-00001120: 725f 6974 656d 73da 0c70 726f 6772 616d  r_items..program
-00001130: 5f61 7267 7363 0c00 0000 0000 0000 0000  _argsc..........
-00001140: 0000 1100 0000 0a00 0000 4300 0000 730a  ..........C...s.
-00001150: 0100 0064 0164 026c 006d 017d 0c01 0074  ...d.d.l.m.}...t
-00001160: 02a0 0364 037c 0b64 0419 009b 0064 057c  ...d.|.d.....d.|
-00001170: 009b 009d 04a1 0101 007c 0b64 0419 007c  .........|.d...|
-00001180: 006b 0272 5664 067c 0564 073c 0074 04a0  .k.rVd.|.d.<.t..
-00001190: 0564 067c 017c 027c 037c 047c 0a7c 0ba1  .d.|.|.|.|.|.|..
-000011a0: 0701 0067 007d 0d74 067c 0683 0164 086b  ...g.}.t.|...d.k
-000011b0: 0472 4774 067c 0083 017d 0e7c 0644 005d  .rGt.|...}.|.D.]
-000011c0: 0f7d 0f7c 007c 0f64 097c 0e85 0219 006b  .}.|.|.d.|.....k
-000011d0: 0272 457c 0f67 017d 0d01 006e 0171 366e  .rE|.g.}...n.q6n
-000011e0: 027c 067d 0d7c 0c64 0a7c 017c 0d7c 077c  .|.}.|.d.|.|.|.|
-000011f0: 087c 0b7c 0a7c 0983 0801 0064 0953 0074  .|.|.|.....d.S.t
-00001200: 067c 0683 0164 086b 0472 817c 0644 005d  .|...d.k.r.|.D.]
-00001210: 247d 107c 0b64 0419 007c 1076 0072 8074  $}.|.d...|.v.r.t
-00001220: 04a0 077c 0a7c 0b7c 0164 0864 0ba1 0501  ...|.|.|.d.d....
-00001230: 007c 1067 017d 067c 0c64 0a7c 017c 067c  .|.g.}.|.d.|.|.|
-00001240: 077c 087c 0b7c 0a7c 0983 0801 0001 0064  .|.|.|.|.......d
-00001250: 0953 0071 5e64 0953 0064 0953 0029 0c61  .S.q^d.S.d.S.).a
-00001260: db02 0000 0a20 2020 2050 726f 6365 7373  .....    Process
-00001270: 2061 2073 696e 676c 6520 5461 736b 206f   a single Task o
-00001280: 6e6c 790a 2020 2020 2020 2020 3a70 6172  nly.        :par
-00001290: 616d 206f 7572 5f74 6173 6b5f 6e61 6d65  am our_task_name
-000012a0: 3a20 6e61 6d65 206f 6620 7468 6520 5461  : name of the Ta
-000012b0: 736b 2074 6f20 7072 6f63 6573 730a 2020  sk to process.  
-000012c0: 2020 2020 2020 3a70 6172 616d 206f 7574        :param out
-000012d0: 7075 745f 6c69 7374 3a20 7768 6572 6520  put_list: where 
-000012e0: 7468 6520 6f75 7470 7574 206c 696e 6520  the output line 
-000012f0: 676f 6573 2066 6f72 2054 6173 6b0a 2020  goes for Task.  
-00001300: 2020 2020 2020 3a70 6172 616d 2070 726f        :param pro
-00001310: 6a65 6374 5f6e 616d 653a 206e 616d 6520  ject_name: name 
-00001320: 6f66 2074 6865 2050 726f 6a65 6374 2054  of the Project T
-00001330: 6173 6b20 6265 6c6f 6e67 7320 746f 0a20  ask belongs to. 
-00001340: 2020 2020 2020 203a 7061 7261 6d20 7072         :param pr
-00001350: 6f66 696c 655f 6e61 6d65 3a20 6e61 6d65  ofile_name: name
-00001360: 206f 6620 7468 6520 5072 6f66 696c 6520   of the Profile 
-00001370: 7468 6520 5461 736b 2062 656c 6f6e 6773  the Task belongs
-00001380: 2074 6f0a 2020 2020 2020 2020 3a70 6172   to.        :par
-00001390: 616d 2068 6561 6469 6e67 3a20 7468 6520  am heading: the 
-000013a0: 6865 6164 696e 672c 2069 6620 616e 790a  heading, if any.
-000013b0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-000013c0: 6f75 6e64 5f69 7465 6d73 3a20 7369 6e67  ound_items: sing
-000013d0: 6c65 206e 616d 6520 666f 7220 5072 6f6a  le name for Proj
-000013e0: 6563 742f 5072 6f66 696c 652f 5461 736b  ect/Profile/Task
-000013f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001400: 7461 736b 5f6c 6973 743a 206c 6973 7420  task_list: list 
-00001410: 6f66 2054 6173 6b73 0a20 2020 2020 2020  of Tasks.       
-00001420: 203a 7061 7261 6d20 6f75 725f 7461 736b   :param our_task
-00001430: 5f65 6c65 6d65 6e74 3a20 7468 6520 786d  _element: the xm
-00001440: 6c20 656c 656d 656e 7420 666f 7220 7468  l element for th
-00001450: 6973 2054 6173 6b0a 2020 2020 2020 2020  is Task.        
-00001460: 3a70 6172 616d 206c 6973 745f 6f66 5f66  :param list_of_f
-00001470: 6f75 6e64 5f74 6173 6b73 3a20 616c 6c20  ound_tasks: all 
-00001480: 5461 736b 7320 7072 6f63 6573 7365 6420  Tasks processed 
-00001490: 736f 2066 6172 0a20 2020 2020 2020 203a  so far.        :
-000014a0: 7061 7261 6d20 616c 6c5f 7461 736b 6572  param all_tasker
-000014b0: 5f69 7465 6d73 3a20 616c 6c20 5072 6f6a  _items: all Proj
-000014c0: 6563 7473 2f50 726f 6669 6c65 732f 5461  ects/Profiles/Ta
-000014d0: 736b 732f 5363 656e 6573 0a20 2020 2020  sks/Scenes.     
-000014e0: 2020 203a 7061 7261 6d20 636f 6c6f 726d     :param colorm
-000014f0: 6170 3a20 636f 6c6f 7273 2074 6f20 7573  ap: colors to us
-00001500: 6520 696e 206f 7574 7075 740a 2020 2020  e in output.    
-00001510: 2020 2020 3a70 6172 616d 2070 726f 6772      :param progr
-00001520: 616d 5f61 7267 733a 2072 756e 7469 6d65  am_args: runtime
-00001530: 2061 7267 756d 656e 7473 0a20 2020 2072   arguments.    r
-00001540: 0100 0000 a901 da0c 7072 6f63 6573 735f  ........process_
-00001550: 6c69 7374 7a17 7461 736b 7320 7369 6e67  listz.tasks sing
-00001560: 6c65 2074 6173 6b20 6e61 6d65 3ada 1073  le task name:..s
-00001570: 696e 676c 655f 7461 736b 5f6e 616d 657a  ingle_task_namez
-00001580: 0f20 6f75 7220 5461 736b 206e 616d 653a  . our Task name:
-00001590: 54da 1173 696e 676c 655f 7461 736b 5f66  T..single_task_f
-000015a0: 6f75 6e64 7213 0000 004e fa05 5461 736b  oundr....N..Task
-000015b0: 3a72 0f00 0000 2908 da16 6d61 7074 6173  :r....)...maptas
-000015c0: 6b65 722e 7372 632e 7072 6f63 6c69 7374  ker.src.proclist
-000015d0: 724d 0000 0072 0800 0000 7218 0000 00da  rM...r....r.....
-000015e0: 0c62 7569 6c64 5f6f 7574 7075 74da 1272  .build_output..r
-000015f0: 6566 7265 7368 5f6f 7572 5f6f 7574 7075  efresh_our_outpu
-00001600: 7472 1900 0000 da09 6d79 5f6f 7574 7075  tr......my_outpu
-00001610: 7429 1172 4100 0000 7242 0000 0072 4300  t).rA...rB...rC.
-00001620: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
-00001630: 0072 4700 0000 7248 0000 0072 4900 0000  .rG...rH...rI...
-00001640: 724a 0000 0072 0b00 0000 724b 0000 0072  rJ...r....rK...r
-00001650: 4d00 0000 5a13 7465 6d70 6f72 6172 795f  M...Z.temporary_
-00001660: 7461 736b 5f6c 6973 745a 1474 6865 5f74  task_listZ.the_t
-00001670: 6173 6b5f 6e61 6d65 5f6c 656e 6774 68da  ask_name_length.
-00001680: 0469 7465 6d5a 0974 6173 6b5f 6974 656d  .itemZ.task_item
-00001690: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-000016a0: 0e64 6f5f 7369 6e67 6c65 5f74 6173 6bcf  .do_single_task.
-000016b0: 0000 0073 7400 0000 0c1e 0402 0c01 0201  ...st...........
-000016c0: 04ff 04ff 0c04 0802 0402 0201 0201 0201  ................
-000016d0: 0201 0201 0201 0201 04f9 040b 0c01 0801  ................
-000016e0: 0801 1001 0601 0401 02fe 0280 0404 0202  ................
-000016f0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001700: 08f8 0c0b 0802 0c01 0401 0a01 04ff 0603  ................
-00001710: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001720: 0201 04f8 060d 02ee 04fd 0402 7256 0000  ............rV..
-00001730: 00da 0864 6f5f 6578 7472 6163 0d00 0000  ...do_extrac....
-00001740: 0000 0000 0000 0000 1000 0000 0d00 0000  ................
-00001750: 4300 0000 73d6 0000 0064 0164 026c 006d  C...s....d.d.l.m
-00001760: 017d 0d01 007c 0c72 317c 0964 0319 0064  .}...|.r1|.d...d
-00001770: 046b 0272 3174 027c 0283 0104 007d 0e72  .k.r1t.|.....}.r
-00001780: 1f7c 0364 0119 009b 0064 057c 0e9b 009d  .|.d.....d.|....
-00001790: 037c 0364 013c 0074 037c 0264 0683 0204  .|.d.<.t.|.d....
-000017a0: 007d 0f72 317c 0364 0119 009b 0064 057c  .}.r1|.d.....d.|
-000017b0: 0f9b 009d 037c 0364 013c 007c 0164 076b  .....|.d.<.|.d.k
-000017c0: 0372 4a7c 0964 0819 0072 4a74 047c 017c  .rJ|.d...rJt.|.|
-000017d0: 007c 047c 057c 077c 0b7c 037c 027c 067c  .|.|.|.|.|.|.|.|
-000017e0: 0a7c 087c 0983 0c01 0064 0953 007c 0372  .|.|.....d.S.|.r
-000017f0: 6974 05a0 067c 087c 097c 0064 0a64 07a1  it...|.|.|.d.d..
-00001800: 0501 007c 0d64 0b7c 007c 037c 027c 067c  ...|.d.|.|.|.|.|
-00001810: 097c 087c 0a83 0801 0074 05a0 067c 087c  .|.|.....t...|.|
-00001820: 097c 0064 0464 07a1 0501 0064 0653 0029  .|.d.d.....d.S.)
-00001830: 0c61 5c03 0000 0a20 2020 2057 6520 6861  .a\....    We ha
-00001840: 7665 2061 2073 696e 676c 6520 5461 736b  ve a single Task
-00001850: 206f 7220 6120 6c69 7374 206f 6620 5461   or a list of Ta
-00001860: 736b 732e 2020 4f75 7470 7574 2069 742f  sks.  Output it/
-00001870: 7468 656d 2e0a 2020 2020 2020 2020 3a70  them..        :p
-00001880: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
-00001890: 3a20 6c69 7374 206f 6620 6f75 7470 7574  : list of output
-000018a0: 206c 696e 6573 2067 656e 6572 6174 6564   lines generated
-000018b0: 2074 6875 7320 6661 720a 2020 2020 2020   thus far.      
-000018c0: 2020 3a70 6172 616d 206f 7572 5f74 6173    :param our_tas
-000018d0: 6b5f 6e61 6d65 3a20 6e61 6d65 206f 6620  k_name: name of 
-000018e0: 5461 736b 0a20 2020 2020 2020 203a 7061  Task.        :pa
-000018f0: 7261 6d20 6f75 725f 7461 736b 5f65 6c65  ram our_task_ele
-00001900: 6d65 6e74 3a20 5461 736b 2078 6d6c 2065  ment: Task xml e
-00001910: 6c65 6d65 6e74 0a20 2020 2020 2020 203a  lement.        :
-00001920: 7061 7261 6d20 7461 736b 5f6c 6973 743a  param task_list:
-00001930: 2054 6173 6b20 6c69 7374 0a20 2020 2020   Task list.     
-00001940: 2020 203a 7061 7261 6d20 7072 6f6a 6563     :param projec
-00001950: 745f 6e61 6d65 3a20 6e61 6d65 206f 6620  t_name: name of 
-00001960: 6375 7272 656e 7420 5072 6f6a 6563 740a  current Project.
-00001970: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-00001980: 726f 6669 6c65 5f6e 616d 653a 206e 616d  rofile_name: nam
-00001990: 6520 6f66 2063 7572 7265 6e74 2050 726f  e of current Pro
-000019a0: 6669 6c65 0a20 2020 2020 2020 203a 7061  file.        :pa
-000019b0: 7261 6d20 6c69 7374 5f6f 665f 666f 756e  ram list_of_foun
-000019c0: 645f 7461 736b 733a 206c 6973 7420 6f66  d_tasks: list of
-000019d0: 2054 6173 6b73 2066 6f75 6e64 2073 6f20   Tasks found so 
-000019e0: 6661 720a 2020 2020 2020 2020 3a70 6172  far.        :par
-000019f0: 616d 2068 6561 6469 6e67 3a20 6375 7272  am heading: curr
-00001a00: 656e 7420 6865 6164 696e 670a 2020 2020  ent heading.    
-00001a10: 2020 2020 3a70 6172 616d 2063 6f6c 6f72      :param color
-00001a20: 6d61 703a 2063 6f6c 6f72 7320 746f 2075  map: colors to u
-00001a30: 7365 2069 6e20 6f75 7470 7574 0a20 2020  se in output.   
-00001a40: 2020 2020 203a 7061 7261 6d20 7072 6f67       :param prog
-00001a50: 7261 6d5f 6172 6773 3a20 7275 6e74 696d  ram_args: runtim
-00001a60: 6520 6172 6775 6d65 6e74 730a 2020 2020  e arguments.    
-00001a70: 2020 2020 3a70 6172 616d 2061 6c6c 5f74      :param all_t
-00001a80: 6173 6b65 725f 6974 656d 733a 2061 6c6c  asker_items: all
-00001a90: 2050 726f 6a65 6374 732f 5072 6f66 696c   Projects/Profil
-00001aa0: 6573 2f54 6173 6b73 2f53 6365 6e65 730a  es/Tasks/Scenes.
-00001ab0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00001ac0: 6f75 6e64 5f69 7465 6d73 3a20 7369 6e67  ound_items: sing
-00001ad0: 6c65 2050 726f 6a65 6374 2f50 726f 6669  le Project/Profi
-00001ae0: 6c65 2f54 6173 6b20 746f 2073 6561 7263  le/Task to searc
-00001af0: 6820 666f 720a 2020 2020 2020 2020 3a70  h for.        :p
-00001b00: 6172 616d 2064 6f5f 6578 7472 613a 2066  aram do_extra: f
-00001b10: 6c61 6720 746f 2064 6f2f 6f75 7470 7574  lag to do/output
-00001b20: 2065 7874 7261 2054 6173 6b20 7374 7566   extra Task stuf
-00001b30: 660a 2020 2020 2020 2020 3a72 6574 7572  f.        :retur
-00001b40: 6e3a 2054 7275 6520 6966 2077 6520 6172  n: True if we ar
-00001b50: 6520 7365 6172 6368 696e 6720 666f 7220  e searching for 
-00001b60: 6120 7369 6e67 6c65 2054 6173 6b20 616e  a single Task an
-00001b70: 6420 666f 756e 6420 6974 2e20 204f 7468  d found it.  Oth
-00001b80: 6572 7769 7365 2c20 4661 6c73 650a 2020  erwise, False.  
-00001b90: 2020 7201 0000 0072 4c00 0000 da14 6469    r....rL.....di
-00001ba0: 7370 6c61 795f 6465 7461 696c 5f6c 6576  splay_detail_lev
-00001bb0: 656c e903 0000 00fa 0120 4672 0f00 0000  el....... Fr....
-00001bc0: 724e 0000 0054 7213 0000 0072 5000 0000  rN...Tr....rP...
-00001bd0: 2907 7251 0000 0072 4d00 0000 7203 0000  ).rQ...rM...r...
-00001be0: 0072 0400 0000 7256 0000 0072 5200 0000  .r....rV...rR...
-00001bf0: 7254 0000 0029 1072 4200 0000 7241 0000  rT...).rB...rA..
-00001c00: 0072 4800 0000 7247 0000 0072 4300 0000  .rH...rG...rC...
-00001c10: 7244 0000 0072 4900 0000 7245 0000 0072  rD...rI...rE...r
-00001c20: 0b00 0000 724b 0000 0072 4a00 0000 7246  ....rK...rJ...rF
-00001c30: 0000 0072 5700 0000 724d 0000 00da 0c6b  ...rW...rM.....k
-00001c40: 6964 5f61 7070 5f69 6e66 6fda 0870 7269  id_app_info..pri
-00001c50: 6f72 6974 7972 2500 0000 7225 0000 0072  orityr%...r%...r
-00001c60: 2600 0000 da0b 6f75 7470 7574 5f74 6173  &.....output_tas
-00001c70: 6b32 0100 0073 4800 0000 0c21 1003 0c01  k2...sH....!....
-00001c80: 1601 0e01 1601 1003 0201 0201 0201 0201  ................
-00001c90: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001ca0: 0201 04f4 040e 0401 1202 0202 0201 0201  ................
-00001cb0: 0201 0201 0201 0201 0201 0201 04f8 120b  ................
-00001cc0: 0402 725d 0000 0029 23da 1578 6d6c 2e65  ..r]...)#..xml.e
-00001cd0: 7472 6565 2e45 6c65 6d65 6e74 5472 6565  tree.ElementTree
-00001ce0: da03 786d 6cda 156d 6170 7461 736b 6572  ..xml..maptasker
-00001cf0: 2e73 7263 2e61 6374 696f 6e65 da03 7372  .src.actione..sr
-00001d00: 63da 0761 6374 696f 6e65 721b 0000 00da  c..actioner.....
-00001d10: 156d 6170 7461 736b 6572 2e73 7263 2e6f  .maptasker.src.o
-00001d20: 7574 7075 746c da07 6f75 7470 7574 6c72  utputl..outputlr
-00001d30: 5200 0000 da15 6d61 7074 6173 6b65 722e  R.....maptasker.
-00001d40: 7372 632e 786d 6c64 6174 6172 0200 0000  src.xmldatar....
-00001d50: da14 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
-00001d60: 6b69 6461 7070 7203 0000 00da 166d 6170  kidappr......map
-00001d70: 7461 736b 6572 2e73 7263 2e70 7269 6f72  tasker.src.prior
-00001d80: 6974 7972 0400 0000 da14 6d61 7074 6173  ityr......maptas
-00001d90: 6b65 722e 7372 632e 6765 7469 6473 7205  ker.src.getidsr.
-00001da0: 0000 00da 166d 6170 7461 736b 6572 2e73  .....maptasker.s
-00001db0: 7263 2e73 7973 636f 6e73 7472 0600 0000  rc.sysconstr....
-00001dc0: 7207 0000 0072 0800 0000 da17 6d61 7074  r....r......mapt
-00001dd0: 6173 6b65 722e 7372 632e 7368 656c 6c73  asker.src.shells
-00001de0: 6f72 7472 0900 0000 da05 6574 7265 65da  ortr......etree.
-00001df0: 0464 6963 74da 046c 6973 7472 2700 0000  .dict..listr'...
-00001e00: 721d 0000 00da 0574 7570 6c65 7234 0000  r......tupler4..
-00001e10: 0072 3a00 0000 da04 626f 6f6c 7240 0000  .r:.....boolr@..
-00001e20: 0072 5600 0000 725d 0000 0072 2500 0000  .rV...r]...r%...
-00001e30: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-00001e40: 083c 6d6f 6475 6c65 3e01 0000 0073 b600  .<module>....s..
-00001e50: 0000 080d 1201 1202 0c01 0c01 0c01 0c01  ................
-00001e60: 0c01 0c01 0c01 0c02 1c07 0243 0201 02ff  ...........C....
-00001e70: 0202 02fe 0203 02fd 0204 02fc 0205 02fb  ................
-00001e80: 0c06 0afa 0234 0201 02ff 0201 02ff 0201  .....4..........
-00001e90: 02ff 0c02 0afe 161b 021c 0201 02ff 0202  ................
-00001ea0: 02fe 0203 02fd 0204 02fc 0205 02fb 0206  ................
-00001eb0: 02fa 0207 02f9 0408 02f8 0209 02f7 020a  ................
-00001ec0: 02f6 020b 02f5 020c 02f4 020d 0af3 0263  ...............c
-00001ed0: 0201 02ff 0202 02fe 0403 02fd 0204 02fc  ................
-00001ee0: 0205 02fb 0206 02fa 0207 02f9 0208 02f8  ................
-00001ef0: 0209 02f7 020a 02f6 020b 02f5 020c 02f4  ................
-00001f00: 020d 02f3 020e 0ef2                      ........
+000000c0: 6a18 640b 6519 640c 6519 640d 651a 6608  j.d.e.d.e.d.e.f.
+000000d0: 640e 640f 8404 5a1b 6410 651c 6411 651a  d.d...Z.d.e.d.e.
+000000e0: 6412 651a 6413 651c 6414 6519 640d 651d  d.e.d.e.d.e.d.e.
+000000f0: 6501 6a17 6a18 651c 6602 1900 660c 6415  e.j.j.e.f...f.d.
+00000100: 6416 8404 5a1e 6410 651c 6417 651a 6418  d...Z.d.e.d.e.d.
+00000110: 6519 640d 651d 651c 6501 6a17 6602 1900  e.d.e.e.e.j.f...
+00000120: 6608 6419 641a 8404 5a1f 6410 651c 641b  f.d.d...Z.d.e.d.
+00000130: 6519 640d 6520 6606 641c 641d 8404 5a21  e.d.e f.d.d...Z!
+00000140: 641e 651c 641f 651a 6420 651c 6421 651c  d.e.d.e.d e.d!e.
+00000150: 6422 651c 6423 6519 6424 651a 6425 6501  d"e.d#e.d$e.d%e.
+00000160: 6a17 6a18 6426 651a 6427 6519 640b 6519  j.j.d&e.d'e.d.e.
+00000170: 6428 6519 640d 6401 661a 6429 642a 8404  d(e.d.d.f.d)d*..
+00000180: 5a22 641f 651a 641e 651c 6425 6501 6a17  Z"d.e.d.e.d%e.j.
+00000190: 6a18 6424 651a 6420 651c 6421 651c 6426  j.d$e.d e.d!e.d&
+000001a0: 651a 6422 651c 640b 6519 6428 6519 6427  e.d"e.d.e.d(e.d'
+000001b0: 6519 6423 6519 642b 6520 640d 6520 661c  e.d#e.d+e d.e f.
+000001c0: 642c 642d 8404 5a23 6401 5300 292e e900  d,d-..Z#d.S.)...
+000001d0: 0000 004e 2901 da0b 7461 675f 696e 5f74  ...N)...tag_in_t
+000001e0: 7970 6529 01da 0b67 6574 5f6b 6964 5f61  ype)...get_kid_a
+000001f0: 7070 2901 da0c 6765 745f 7072 696f 7269  pp)...get_priori
+00000200: 7479 2901 da07 6765 745f 6964 7329 01da  ty)...get_ids)..
+00000210: 1155 4e4b 4e4f 574e 5f54 4153 4b5f 4e41  .UNKNOWN_TASK_NA
+00000220: 4d45 2901 da0a 4e4f 5f50 524f 4a45 4354  ME)...NO_PROJECT
+00000230: 2901 da06 6c6f 6767 6572 2901 da0a 7368  )...logger)...sh
+00000240: 656c 6c5f 736f 7274 da0c 6375 7272 656e  ell_sort..curren
+00000250: 745f 7461 736b da08 636f 6c6f 726d 6170  t_task..colormap
+00000260: da09 7072 6f67 5f61 7267 73da 0672 6574  ..prog_args..ret
+00000270: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
+00000280: 0c00 0000 0900 0000 4300 0000 7346 0100  ........C...sF..
+00000290: 0067 007d 037a 077c 00a0 0064 01a1 017d  .g.}.z.|...d...}
+000002a0: 0457 006e 1c04 0074 016a 0279 2501 0001  .W.n...t.j.y%...
+000002b0: 0001 0074 0364 027c 0083 0201 0064 037d  ...t.d.|.....d.}
+000002c0: 0574 037c 0583 0101 0074 04a0 057c 05a1  .t.|.....t...|..
+000002d0: 0101 0067 0006 0059 0053 0077 007c 0472  ...g...Y.S.w.|.r
+000002e0: a164 047d 0664 057d 0774 067c 0483 0164  .d.}.d.}.t.|...d
+000002f0: 056b 0472 3874 077c 0464 0664 0783 0301  .k.r8t.|.d.d....
+00000300: 007c 0444 005d 667d 087c 08a0 0864 08a1  .|.D.]f}.|...d..
+00000310: 017d 0974 09a0 0a7c 097c 0864 067c 0164  .}.t...|.|.d.|.d
+00000320: 097c 02a1 067d 0a74 04a0 0564 0a74 0b7c  .|...}.t...d.t.|
+00000330: 086a 0c64 0b19 0083 0117 0064 0c17 007c  .j.d.......d...|
+00000340: 096a 0d17 0064 0d17 007c 0a17 0064 0e17  .j...d...|...d..
+00000350: 0074 0b7c 086a 0c83 0117 00a1 0101 0064  .t.|.j.........d
+00000360: 0f7c 0a76 0073 7364 107c 0a76 0073 7364  .|.v.ssd.|.v.ssd
+00000370: 117c 0a76 0072 817c 0764 1238 007d 0774  .|.v.r.|.d.8.}.t
+00000380: 067c 0683 017d 0b7c 0664 137c 0b85 0219  .|...}.|.d.|....
+00000390: 007d 0674 09a0 0e7c 017c 037c 0a7c 097c  .}.t...|.|.|.|.|
+000003a0: 077c 06a1 0601 0064 147c 0a76 0073 9764  .|.....d.|.v.s.d
+000003b0: 107c 0a76 0073 9764 157c 0a76 0072 a07c  .|.v.s.d.|.v.r.|
+000003c0: 0764 1237 007d 077c 069b 0064 169d 027d  .d.7.}.|...d...}
+000003d0: 0671 3a7c 0353 0029 1761 1d01 0000 0a20  .q:|.S.).a..... 
+000003e0: 2020 2052 6574 7572 6e20 6120 6c69 7374     Return a list
+000003f0: 206f 6620 5461 736b 2773 2061 6374 696f   of Task's actio
+00000400: 6e73 2066 6f72 2074 6865 2067 6976 656e  ns for the given
+00000410: 2054 6173 6b0a 2020 2020 2020 2020 3a70   Task.        :p
+00000420: 6172 616d 2063 7572 7265 6e74 5f74 6173  aram current_tas
+00000430: 6b3a 2078 6d6c 2065 6c65 6d65 6e74 206f  k: xml element o
+00000440: 6620 7468 6520 5461 736b 2077 6520 6172  f the Task we ar
+00000450: 6520 6765 7474 696e 6720 6163 7469 6f6e  e getting action
+00000460: 7320 666f 720a 2020 2020 2020 2020 3a70  s for.        :p
+00000470: 6172 616d 2063 6f6c 6f72 6d61 703a 2063  aram colormap: c
+00000480: 6f6c 6f72 7320 746f 2075 7365 2069 6e20  olors to use in 
+00000490: 6f75 7470 7574 0a20 2020 2020 2020 203a  output.        :
+000004a0: 7061 7261 6d20 7072 6f67 5f61 7267 733a  param prog_args:
+000004b0: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
+000004c0: 7473 0a20 2020 2020 2020 203a 7265 7475  ts.        :retu
+000004d0: 726e 3a20 6c69 7374 206f 6620 5461 736b  rn: list of Task
+000004e0: 2027 6163 7469 6f6e 2720 6f75 7470 7574   'action' output
+000004f0: 206c 696e 6573 0a20 2020 20da 0641 6374   lines.    ..Act
+00000500: 696f 6e7a 1674 6173 6b73 2e70 7920 6375  ionz.tasks.py cu
+00000510: 7272 656e 7420 5461 736b 3a7a 1945 7272  rrent Task:z.Err
+00000520: 6f72 3a20 4e6f 2061 6374 696f 6e20 666f  or: No action fo
+00000530: 756e 6421 2121 da00 7201 0000 0054 46da  und!!!..r....TF.
+00000540: 0463 6f64 65da 0174 7a08 5461 736b 2049  .code..tz.Task I
+00000550: 443a da02 7372 7a06 2043 6f64 653a 7a0b  D:..srz. Code:z.
+00000560: 2074 6173 6b5f 636f 6465 3a7a 0c41 6374   task_code:z.Act
+00000570: 696f 6e20 6174 7472 3a7a 073e 456e 6420  ion attr:z.>End 
+00000580: 4966 7a05 3e45 6c73 657a 083e 456e 6420  Ifz.>Elsez.>End 
+00000590: 466f 72e9 0100 0000 e918 0000 007a 033e  For..........z.>
+000005a0: 4966 7a04 3e46 6f72 7a18 266e 6273 703b  Ifz.>Forz.&nbsp;
+000005b0: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
+000005c0: 703b 290f da07 6669 6e64 616c 6cda 0a64  p;)...findall..d
+000005d0: 6566 7573 6564 786d 6cda 1344 6566 7573  efusedxml..Defus
+000005e0: 6564 586d 6c45 7863 6570 7469 6f6e da05  edXmlException..
+000005f0: 7072 696e 7472 0800 0000 da05 6465 6275  printr......debu
+00000600: 67da 036c 656e 7209 0000 00da 0466 696e  g..lenr......fin
+00000610: 64da 0f61 6374 696f 6e5f 6576 616c 7561  d..action_evalua
+00000620: 7465 da0f 6765 745f 6163 7469 6f6e 5f63  te..get_action_c
+00000630: 6f64 65da 0373 7472 da06 6174 7472 6962  ode..str..attrib
+00000640: da04 7465 7874 da0c 6275 696c 645f 6163  ..text..build_ac
+00000650: 7469 6f6e 290c 720a 0000 0072 0b00 0000  tion).r....r....
+00000660: 720c 0000 005a 0874 6173 6b6c 6973 745a  r....Z.tasklistZ
+00000670: 0c74 6173 6b5f 6163 7469 6f6e 73da 0965  .task_actions..e
+00000680: 7272 6f72 5f6d 7367 5a12 696e 6465 6e74  rror_msgZ.indent
+00000690: 6174 696f 6e5f 616d 6f75 6e74 5a0b 696e  ation_amountZ.in
+000006a0: 6465 6e74 6174 696f 6eda 0661 6374 696f  dentation..actio
+000006b0: 6eda 0563 6869 6c64 5a09 7461 736b 5f63  n..childZ.task_c
+000006c0: 6f64 655a 0d6c 656e 6774 685f 696e 6465  odeZ.length_inde
+000006d0: 6e74 a900 7225 0000 00fa 742f 5573 6572  nt..r%....t/User
+000006e0: 732f 6d69 6b72 7562 696e 2f4c 6962 7261  s/mikrubin/Libra
+000006f0: 7279 2f43 6c6f 7564 5374 6f72 6167 652f  ry/CloudStorage/
+00000700: 476f 6f67 6c65 4472 6976 652d 6d69 6b72  GoogleDrive-mikr
+00000710: 7562 696e 4067 6d61 696c 2e63 6f6d 2f4d  ubin@gmail.com/M
+00000720: 7920 4472 6976 652f 5079 7468 6f6e 2f6d  y Drive/Python/m
+00000730: 6170 7461 736b 6572 2f6d 6170 7461 736b  aptasker/maptask
+00000740: 6572 2f73 7263 2f74 6173 6b73 2e70 79da  er/src/tasks.py.
+00000750: 0b67 6574 5f61 6374 696f 6e73 2100 0000  .get_actions!...
+00000760: 7366 0000 0004 0a02 020e 010e 010a 0104  sf..............
+00000770: 0108 010a 0108 0102 fb04 0604 0104 010c  ................
+00000780: 030c 0108 020a 0104 020c 0104 ff04 0302  ................
+00000790: 010c 0102 ff02 0202 fe04 0302 fd02 0402  ................
+000007a0: fc02 0502 fb02 0602 fa08 0702 f904 ff08  ................
+000007b0: 0c08 0108 0108 0208 010c 0104 010c 0104  ................
+000007c0: ff18 0408 020a 0102 8004 0272 2700 0000  ...........r'...
+000007d0: da0b 7468 655f 7461 736b 5f69 64da 1a74  ..the_task_id..t
+000007e0: 6173 6b73 5f74 6861 745f 6861 7665 5f62  asks_that_have_b
+000007f0: 6565 6e5f 666f 756e 64da 1174 6173 6b5f  een_found..task_
+00000800: 6f75 7470 7574 5f6c 696e 6573 da09 7461  output_lines..ta
+00000810: 736b 5f74 7970 65da 0961 6c6c 5f74 6173  sk_type..all_tas
+00000820: 6b73 6305 0000 0000 0000 0000 0000 0009  ksc.............
+00000830: 0000 000a 0000 0043 0000 0073 fa00 0000  .......C...s....
+00000840: 7c00 a000 a100 7275 7c04 7c00 1900 7d05  |.....ru|.|...}.
+00000850: 7c01 a001 7c00 a101 0100 6401 7c00 9b00  |...|.....d.|...
+00000860: 9d02 7d06 7a29 7c05 a002 6402 a101 6a03  ..}.z)|...d...j.
+00000870: 7d07 7c03 6403 6b02 7228 7c02 a001 7c07  }.|.d.k.r(|...|.
+00000880: 9b00 6404 7c06 9b00 9d03 a101 0100 6e0f  ..d.|.........n.
+00000890: 7c02 a001 7c07 9b00 6405 7c06 9b00 9d03  |...|...d.|.....
+000008a0: a101 0100 5700 7c05 7c07 6602 5300 5700  ....W.|.|.f.S.W.
+000008b0: 7c05 7c07 6602 5300 0400 7404 7974 0100  |.|.f.S...t.yt..
+000008c0: 7d08 0100 7a2d 7405 7d07 7c03 6403 6b02  }...z-t.}.|.d.k.
+000008d0: 7254 7c02 a001 7405 9b00 6404 7c06 9b00  rT|...t...d.|...
+000008e0: 9d03 a101 0100 6e13 7c02 a001 7405 9b00  ......n.|...t...
+000008f0: 6405 7c06 9b00 9d03 a101 0100 5700 5900  d.|.........W.Y.
+00000900: 6406 7d08 7e08 7c05 7c07 6602 5300 5700  d.}.~.|.|.f.S.W.
+00000910: 5900 6406 7d08 7e08 7c05 7c07 6602 5300  Y.d.}.~.|.|.f.S.
+00000920: 6406 7d08 7e08 7701 7700 6406 7d05 6407  d.}.~.w.w.d.}.d.
+00000930: 7d07 7c05 7c07 6602 5300 2908 6178 0100  }.|.|.f.S.).ax..
+00000940: 000a 2020 2020 4765 7420 7468 6520 6e61  ..    Get the na
+00000950: 6d65 206f 6620 7468 6520 7461 736b 2067  me of the task g
+00000960: 6976 656e 2074 6865 2054 6173 6b20 4944  iven the Task ID
+00000970: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000980: 7468 655f 7461 736b 5f69 643a 2074 6865  the_task_id: the
+00000990: 2054 6173 6b27 7320 4944 2028 652e 672e   Task's ID (e.g.
+000009a0: 2027 3437 2729 0a20 2020 2020 2020 203a   '47').        :
+000009b0: 7061 7261 6d20 7461 736b 735f 7468 6174  param tasks_that
+000009c0: 5f68 6176 655f 6265 656e 5f66 6f75 6e64  _have_been_found
+000009d0: 3a20 6c69 7374 206f 6620 5461 736b 7320  : list of Tasks 
+000009e0: 666f 756e 6420 736f 2066 6172 0a20 2020  found so far.   
+000009f0: 2020 2020 203a 7061 7261 6d20 7461 736b       :param task
+00000a00: 5f6f 7574 7075 745f 6c69 6e65 733a 206c  _output_lines: l
+00000a10: 6973 7420 6f66 2054 6173 6b73 0a20 2020  ist of Tasks.   
+00000a20: 2020 2020 203a 7061 7261 6d20 7461 736b       :param task
+00000a30: 5f74 7970 653a 2054 7970 6520 6f66 2054  _type: Type of T
+00000a40: 6173 6b20 2845 6e74 7279 2c20 4578 6974  ask (Entry, Exit
+00000a50: 2c20 5363 656e 6529 0a20 2020 2020 2020  , Scene).       
+00000a60: 203a 7061 7261 6d20 616c 6c5f 7461 736b   :param all_task
+00000a70: 733a 2061 6c6c 2054 6173 6b73 2069 6e20  s: all Tasks in 
+00000a80: 786d 6c0a 2020 2020 2020 2020 3a72 6574  xml.        :ret
+00000a90: 7572 6e3a 2054 6173 6b27 7320 786d 6c20  urn: Task's xml 
+00000aa0: 656c 656d 656e 742c 2054 6173 6b27 7320  element, Task's 
+00000ab0: 6e61 6d65 0a20 2020 207a 1526 6e62 7370  name.    z.&nbsp
+00000ac0: 3b26 6e62 7370 3b54 6173 6b20 4944 3a20  ;&nbsp;Task ID: 
+00000ad0: da03 6e6d 655a 0445 7869 747a 2526 6e62  ..nmeZ.Exitz%&nb
+00000ae0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+00000af0: 6e62 7370 3b3c 3c3c 2045 7869 7420 5461  nbsp;<<< Exit Ta
+00000b00: 736b 7a26 266e 6273 703b 266e 6273 703b  skz&&nbsp;&nbsp;
+00000b10: 266e 6273 703b 266e 6273 703b 3c3c 3c20  &nbsp;&nbsp;<<< 
+00000b20: 456e 7472 7920 5461 736b 4e72 0f00 0000  Entry TaskNr....
+00000b30: 2906 da07 6973 6469 6769 74da 0661 7070  )...isdigit..app
+00000b40: 656e 6472 1b00 0000 7220 0000 00da 0945  endr....r .....E
+00000b50: 7863 6570 7469 6f6e 7206 0000 0029 0972  xceptionr....).r
+00000b60: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
+00000b70: 0000 0072 2c00 0000 da04 7461 736b da05  ...r,.....task..
+00000b80: 6578 7472 615a 0974 6173 6b5f 6e61 6d65  extraZ.task_name
+00000b90: da01 6572 2500 0000 7225 0000 0072 2600  ..er%...r%...r&.
+00000ba0: 0000 da0d 6765 745f 7461 736b 5f6e 616d  ....get_task_nam
+00000bb0: 6566 0000 0073 4200 0000 0810 0801 0a01  ef...sB.........
+00000bc0: 0a01 0201 0c01 0801 0401 0c01 06ff 0405  ................
+00000bd0: 0c01 06ff 0812 02e9 0817 0ef1 0401 0801  ................
+00000be0: 0401 0c01 06ff 0405 0c01 0eff 0807 0af4  ................
+00000bf0: 080c 0880 02f1 040c 0401 0802 7234 0000  ............r4..
+00000c00: 00da 1670 726f 6a65 6374 735f 7769 7468  ...projects_with
+00000c10: 5f6e 6f5f 7461 736b 73da 0c61 6c6c 5f70  _no_tasks..all_p
+00000c20: 726f 6a65 6374 7363 0300 0000 0000 0000  rojectsc........
+00000c30: 0000 0000 0600 0000 0900 0000 4300 0000  ............C...
+00000c40: 7356 0000 0074 007d 0364 017d 047c 0264  sV...t.}.d.}.|.d
+00000c50: 0175 0172 277c 0244 005d 1c7d 047c 04a0  .u.r'|.D.].}.|..
+00000c60: 0164 02a1 016a 027d 0374 0364 0369 0069  .d...j.}.t.d.i.i
+00000c70: 0067 007c 047c 037c 0183 077d 057c 007c  .g.|.|.|...}.|.|
+00000c80: 0576 0072 267c 037c 0466 0202 0001 0053  .v.r&|.|.f.....S
+00000c90: 0071 0a7c 037c 0466 0253 0029 0461 4b01  .q.|.|.f.S.).aK.
+00000ca0: 0000 0a20 2020 2046 696e 6420 7468 6520  ...    Find the 
+00000cb0: 5072 6f6a 6563 7420 6265 6c6f 6e67 696e  Project belongin
+00000cc0: 6720 746f 2074 6865 2054 6173 6b20 6964  g to the Task id
+00000cd0: 2070 6173 7365 6420 696e 0a20 2020 2020   passed in.     
+00000ce0: 2020 203a 7061 7261 6d20 7468 655f 7461     :param the_ta
+00000cf0: 736b 5f69 643a 2074 6865 2049 4420 6f66  sk_id: the ID of
+00000d00: 2074 6865 2054 6173 6b0a 2020 2020 2020   the Task.      
+00000d10: 2020 3a70 6172 616d 2070 726f 6a65 6374    :param project
+00000d20: 735f 7769 7468 5f6e 6f5f 7461 736b 733a  s_with_no_tasks:
+00000d30: 206c 6973 7420 6f66 2050 726f 6a65 6374   list of Project
+00000d40: 7320 7468 6174 2064 6f20 6e6f 7420 6861  s that do not ha
+00000d50: 7665 2061 6e79 2054 6173 6b73 0a20 2020  ve any Tasks.   
+00000d60: 2020 2020 203a 7061 7261 6d20 616c 6c5f       :param all_
+00000d70: 7072 6f6a 6563 7473 3a20 616c 6c20 5461  projects: all Ta
+00000d80: 736b 6572 2050 726f 6a65 6374 730a 2020  sker Projects.  
+00000d90: 2020 2020 2020 3a72 6574 7572 6e3a 206e        :return: n
+00000da0: 616d 6520 6f66 2074 6865 2050 726f 6a65  ame of the Proje
+00000db0: 6374 2074 6861 7420 6265 6c6f 6e67 7320  ct that belongs 
+00000dc0: 746f 2074 6869 7320 7461 736b 2061 6e64  to this task and
+00000dd0: 2074 6865 2050 726f 6a65 6374 2078 6d6c   the Project xml
+00000de0: 2065 6c65 6d65 6e74 0a20 2020 204e da04   element.    N..
+00000df0: 6e61 6d65 4629 0472 0700 0000 721b 0000  nameF).r....r...
+00000e00: 0072 2000 0000 7205 0000 0029 0672 2800  .r ...r....).r(.
+00000e10: 0000 7235 0000 0072 3600 0000 5a09 7072  ..r5...r6...Z.pr
+00000e20: 6f6a 5f6e 616d 65da 0770 726f 6a65 6374  oj_name..project
+00000e30: da08 7461 736b 5f69 6473 7225 0000 0072  ..task_idsr%...r
+00000e40: 2500 0000 7226 0000 00da 1967 6574 5f70  %...r&.....get_p
+00000e50: 726f 6a65 6374 5f66 6f72 5f73 6f6c 6f5f  roject_for_solo_
+00000e60: 7461 736b 9a00 0000 7318 0000 0004 0a04  task....s.......
+00000e70: 0108 0108 020c 0102 010e 0104 ff08 030c  ................
+00000e80: 0102 ff08 0272 3a00 0000 da0a 616c 6c5f  .....r:.....all_
+00000e90: 7363 656e 6573 6302 0000 0000 0000 0000  scenesc.........
+00000ea0: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00000eb0: 6000 0000 7c01 a000 a100 4400 5d29 7d02  `...|.....D.])}.
+00000ec0: 7c02 4400 5d24 7d03 7401 7c03 6a02 6401  |.D.]$}.t.|.j.d.
+00000ed0: 8302 722c 7c03 4400 5d19 7d04 7401 7c04  ..r,|.D.].}.t.|.
+00000ee0: 6a02 6402 8302 7224 7c00 7c04 6a03 6b02  j.d...r$|.|.j.k.
+00000ef0: 7224 0100 0100 0100 6401 5300 7c03 6a02  r$......d.S.|.j.
+00000f00: 6403 6b02 722b 0100 6e01 7112 7108 7104  d.k.r+..n.q.q.q.
+00000f10: 6402 5300 2904 6118 0100 000a 2020 2020  d.S.).a.....    
+00000f20: 4964 656e 7469 6679 2077 6865 7468 6572  Identify whether
+00000f30: 2074 6865 2054 6173 6b20 7061 7373 6564   the Task passed
+00000f40: 2069 6e20 6973 2070 6172 7420 6f66 2061   in is part of a
+00000f50: 2053 6365 6e65 3a20 5472 7565 203d 2079   Scene: True = y
+00000f60: 6573 2c20 4661 6c73 6520 3d20 6e6f 0a20  es, False = no. 
+00000f70: 2020 2020 2020 203a 7061 7261 6d20 7468         :param th
+00000f80: 655f 7461 736b 5f69 643a 2074 6865 2069  e_task_id: the i
+00000f90: 6420 6f66 2074 6865 2054 6173 6b20 746f  d of the Task to
+00000fa0: 2063 6865 636b 2061 6761 696e 7374 0a20   check against. 
+00000fb0: 2020 2020 2020 203a 7061 7261 6d20 616c         :param al
+00000fc0: 6c5f 7363 656e 6573 3a20 616c 6c20 5363  l_scenes: all Sc
+00000fd0: 656e 6573 2069 6e20 5461 736b 6572 2063  enes in Tasker c
+00000fe0: 6f6e 6669 6775 7261 7469 6f6e 0a20 2020  onfiguration.   
+00000ff0: 2020 2020 203a 7265 7475 726e 3a20 5472       :return: Tr
+00001000: 7565 2069 6620 5461 736b 2069 7320 7061  ue if Task is pa
+00001010: 7274 206f 6620 6120 5363 656e 652c 2046  rt of a Scene, F
+00001020: 616c 7365 206f 7468 6572 7769 7365 0a20  alse otherwise. 
+00001030: 2020 2054 46da 0353 7472 2904 da06 7661     TF..Str)...va
+00001040: 6c75 6573 7202 0000 00da 0374 6167 7220  luesr......tagr 
+00001050: 0000 0029 0572 2800 0000 723b 0000 00da  ...).r(...r;....
+00001060: 0576 616c 7565 7224 0000 005a 0873 7562  .valuer$...Z.sub
+00001070: 6368 696c 6472 2500 0000 7225 0000 0072  childr%...r%...r
+00001080: 2600 0000 da0d 7461 736b 5f69 6e5f 7363  &.....task_in_sc
+00001090: 656e 65b5 0000 0073 1c00 0000 0c08 0801  ene....s........
+000010a0: 0c01 0801 0a03 02ff 0a02 0a02 0a01 0401  ................
+000010b0: 0202 0280 02f4 040d 7240 0000 00da 0d6f  ........r@.....o
+000010c0: 7572 5f74 6173 6b5f 6e61 6d65 da0b 6f75  ur_task_name..ou
+000010d0: 7470 7574 5f6c 6973 74da 0c70 726f 6a65  tput_list..proje
+000010e0: 6374 5f6e 616d 65da 0c70 726f 6669 6c65  ct_name..profile
+000010f0: 5f6e 616d 65da 0768 6561 6469 6e67 da0b  _name..heading..
+00001100: 666f 756e 645f 6974 656d 73da 0974 6173  found_items..tas
+00001110: 6b5f 6c69 7374 da10 6f75 725f 7461 736b  k_list..our_task
+00001120: 5f65 6c65 6d65 6e74 da13 6c69 7374 5f6f  _element..list_o
+00001130: 665f 666f 756e 645f 7461 736b 73da 1061  f_found_tasks..a
+00001140: 6c6c 5f74 6173 6b65 725f 6974 656d 73da  ll_tasker_items.
+00001150: 0c70 726f 6772 616d 5f61 7267 7363 0c00  .program_argsc..
+00001160: 0000 0000 0000 0000 0000 1100 0000 0a00  ................
+00001170: 0000 4300 0000 730a 0100 0064 0164 026c  ..C...s....d.d.l
+00001180: 006d 017d 0c01 0074 02a0 0364 037c 0b64  .m.}...t...d.|.d
+00001190: 0419 009b 0064 057c 009b 009d 04a1 0101  .....d.|........
+000011a0: 007c 0b64 0419 007c 006b 0272 5664 067c  .|.d...|.k.rVd.|
+000011b0: 0564 073c 0074 04a0 0564 067c 017c 027c  .d.<.t...d.|.|.|
+000011c0: 037c 047c 0a7c 0ba1 0701 0067 007d 0d74  .|.|.|.....g.}.t
+000011d0: 067c 0683 0164 086b 0472 4774 067c 0083  .|...d.k.rGt.|..
+000011e0: 017d 0e7c 0644 005d 0f7d 0f7c 007c 0f64  .}.|.D.].}.|.|.d
+000011f0: 097c 0e85 0219 006b 0272 457c 0f67 017d  .|.....k.rE|.g.}
+00001200: 0d01 006e 0171 366e 027c 067d 0d7c 0c64  ...n.q6n.|.}.|.d
+00001210: 0a7c 017c 0d7c 077c 087c 0b7c 0a7c 0983  .|.|.|.|.|.|.|..
+00001220: 0801 0064 0953 0074 067c 0683 0164 086b  ...d.S.t.|...d.k
+00001230: 0472 817c 0644 005d 247d 107c 0b64 0419  .r.|.D.]$}.|.d..
+00001240: 007c 1076 0072 8074 04a0 077c 0a7c 0b7c  .|.v.r.t...|.|.|
+00001250: 0164 0864 0ba1 0501 007c 1067 017d 067c  .d.d.....|.g.}.|
+00001260: 0c64 0a7c 017c 067c 077c 087c 0b7c 0a7c  .d.|.|.|.|.|.|.|
+00001270: 0983 0801 0001 0064 0953 0071 5e64 0953  .......d.S.q^d.S
+00001280: 0064 0953 0029 0c61 db02 0000 0a20 2020  .d.S.).a.....   
+00001290: 2050 726f 6365 7373 2061 2073 696e 676c   Process a singl
+000012a0: 6520 5461 736b 206f 6e6c 790a 2020 2020  e Task only.    
+000012b0: 2020 2020 3a70 6172 616d 206f 7572 5f74      :param our_t
+000012c0: 6173 6b5f 6e61 6d65 3a20 6e61 6d65 206f  ask_name: name o
+000012d0: 6620 7468 6520 5461 736b 2074 6f20 7072  f the Task to pr
+000012e0: 6f63 6573 730a 2020 2020 2020 2020 3a70  ocess.        :p
+000012f0: 6172 616d 206f 7574 7075 745f 6c69 7374  aram output_list
+00001300: 3a20 7768 6572 6520 7468 6520 6f75 7470  : where the outp
+00001310: 7574 206c 696e 6520 676f 6573 2066 6f72  ut line goes for
+00001320: 2054 6173 6b0a 2020 2020 2020 2020 3a70   Task.        :p
+00001330: 6172 616d 2070 726f 6a65 6374 5f6e 616d  aram project_nam
+00001340: 653a 206e 616d 6520 6f66 2074 6865 2050  e: name of the P
+00001350: 726f 6a65 6374 2054 6173 6b20 6265 6c6f  roject Task belo
+00001360: 6e67 7320 746f 0a20 2020 2020 2020 203a  ngs to.        :
+00001370: 7061 7261 6d20 7072 6f66 696c 655f 6e61  param profile_na
+00001380: 6d65 3a20 6e61 6d65 206f 6620 7468 6520  me: name of the 
+00001390: 5072 6f66 696c 6520 7468 6520 5461 736b  Profile the Task
+000013a0: 2062 656c 6f6e 6773 2074 6f0a 2020 2020   belongs to.    
+000013b0: 2020 2020 3a70 6172 616d 2068 6561 6469      :param headi
+000013c0: 6e67 3a20 7468 6520 6865 6164 696e 672c  ng: the heading,
+000013d0: 2069 6620 616e 790a 2020 2020 2020 2020   if any.        
+000013e0: 3a70 6172 616d 2066 6f75 6e64 5f69 7465  :param found_ite
+000013f0: 6d73 3a20 7369 6e67 6c65 206e 616d 6520  ms: single name 
+00001400: 666f 7220 5072 6f6a 6563 742f 5072 6f66  for Project/Prof
+00001410: 696c 652f 5461 736b 0a20 2020 2020 2020  ile/Task.       
+00001420: 203a 7061 7261 6d20 7461 736b 5f6c 6973   :param task_lis
+00001430: 743a 206c 6973 7420 6f66 2054 6173 6b73  t: list of Tasks
+00001440: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001450: 6f75 725f 7461 736b 5f65 6c65 6d65 6e74  our_task_element
+00001460: 3a20 7468 6520 786d 6c20 656c 656d 656e  : the xml elemen
+00001470: 7420 666f 7220 7468 6973 2054 6173 6b0a  t for this Task.
+00001480: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
+00001490: 6973 745f 6f66 5f66 6f75 6e64 5f74 6173  ist_of_found_tas
+000014a0: 6b73 3a20 616c 6c20 5461 736b 7320 7072  ks: all Tasks pr
+000014b0: 6f63 6573 7365 6420 736f 2066 6172 0a20  ocessed so far. 
+000014c0: 2020 2020 2020 203a 7061 7261 6d20 616c         :param al
+000014d0: 6c5f 7461 736b 6572 5f69 7465 6d73 3a20  l_tasker_items: 
+000014e0: 616c 6c20 5072 6f6a 6563 7473 2f50 726f  all Projects/Pro
+000014f0: 6669 6c65 732f 5461 736b 732f 5363 656e  files/Tasks/Scen
+00001500: 6573 0a20 2020 2020 2020 203a 7061 7261  es.        :para
+00001510: 6d20 636f 6c6f 726d 6170 3a20 636f 6c6f  m colormap: colo
+00001520: 7273 2074 6f20 7573 6520 696e 206f 7574  rs to use in out
+00001530: 7075 740a 2020 2020 2020 2020 3a70 6172  put.        :par
+00001540: 616d 2070 726f 6772 616d 5f61 7267 733a  am program_args:
+00001550: 2072 756e 7469 6d65 2061 7267 756d 656e   runtime argumen
+00001560: 7473 0a20 2020 2072 0100 0000 a901 da0c  ts.    r........
+00001570: 7072 6f63 6573 735f 6c69 7374 7a17 7461  process_listz.ta
+00001580: 736b 7320 7369 6e67 6c65 2074 6173 6b20  sks single task 
+00001590: 6e61 6d65 3ada 1073 696e 676c 655f 7461  name:..single_ta
+000015a0: 736b 5f6e 616d 657a 0f20 6f75 7220 5461  sk_namez. our Ta
+000015b0: 736b 206e 616d 653a 54da 1173 696e 676c  sk name:T..singl
+000015c0: 655f 7461 736b 5f66 6f75 6e64 7213 0000  e_task_foundr...
+000015d0: 004e fa05 5461 736b 3a72 0f00 0000 2908  .N..Task:r....).
+000015e0: da16 6d61 7074 6173 6b65 722e 7372 632e  ..maptasker.src.
+000015f0: 7072 6f63 6c69 7374 724d 0000 0072 0800  proclistrM...r..
+00001600: 0000 7219 0000 00da 0c62 7569 6c64 5f6f  ..r......build_o
+00001610: 7574 7075 74da 1272 6566 7265 7368 5f6f  utput..refresh_o
+00001620: 7572 5f6f 7574 7075 7472 1a00 0000 da09  ur_outputr......
+00001630: 6d79 5f6f 7574 7075 7429 1172 4100 0000  my_output).rA...
+00001640: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
+00001650: 4500 0000 7246 0000 0072 4700 0000 7248  E...rF...rG...rH
+00001660: 0000 0072 4900 0000 724a 0000 0072 0b00  ...rI...rJ...r..
+00001670: 0000 724b 0000 0072 4d00 0000 5a13 7465  ..rK...rM...Z.te
+00001680: 6d70 6f72 6172 795f 7461 736b 5f6c 6973  mporary_task_lis
+00001690: 745a 1474 6865 5f74 6173 6b5f 6e61 6d65  tZ.the_task_name
+000016a0: 5f6c 656e 6774 68da 0469 7465 6d5a 0974  _length..itemZ.t
+000016b0: 6173 6b5f 6974 656d 7225 0000 0072 2500  ask_itemr%...r%.
+000016c0: 0000 7226 0000 00da 0e64 6f5f 7369 6e67  ..r&.....do_sing
+000016d0: 6c65 5f74 6173 6bd1 0000 0073 7400 0000  le_task....st...
+000016e0: 0c1e 0402 0c01 0201 04ff 04ff 0c04 0802  ................
+000016f0: 0403 0201 0201 0201 0201 0201 0201 0201  ................
+00001700: 04f9 040b 0c01 0801 0801 1001 0601 0401  ................
+00001710: 02fe 0280 0404 0202 0201 0201 0201 0201  ................
+00001720: 0201 0201 0201 0201 08f8 0c0b 0802 0c01  ................
+00001730: 0401 0a01 04ff 0603 0201 0201 0201 0201  ................
+00001740: 0201 0201 0201 0201 0201 04f8 060d 02ee  ................
+00001750: 04fd 0402 7256 0000 00da 0864 6f5f 6578  ....rV.....do_ex
+00001760: 7472 6163 0d00 0000 0000 0000 0000 0000  trac............
+00001770: 1000 0000 0d00 0000 4300 0000 73d6 0000  ........C...s...
+00001780: 0064 0164 026c 006d 017d 0d01 007c 0c72  .d.d.l.m.}...|.r
+00001790: 317c 0964 0319 0064 046b 0272 3174 027c  1|.d...d.k.r1t.|
+000017a0: 0283 0104 007d 0e72 1f7c 0364 0119 009b  .....}.r.|.d....
+000017b0: 0064 057c 0e9b 009d 037c 0364 013c 0074  .d.|.....|.d.<.t
+000017c0: 037c 0264 0683 0204 007d 0f72 317c 0364  .|.d.....}.r1|.d
+000017d0: 0119 009b 0064 057c 0f9b 009d 037c 0364  .....d.|.....|.d
+000017e0: 013c 007c 0164 076b 0372 4a7c 0964 0819  .<.|.d.k.rJ|.d..
+000017f0: 0072 4a74 047c 017c 007c 047c 057c 077c  .rJt.|.|.|.|.|.|
+00001800: 0b7c 037c 027c 067c 0a7c 087c 0983 0c01  .|.|.|.|.|.|....
+00001810: 0064 0953 007c 0372 6974 05a0 067c 087c  .d.S.|.rit...|.|
+00001820: 097c 0064 0a64 07a1 0501 007c 0d64 0b7c  .|.d.d.....|.d.|
+00001830: 007c 037c 027c 067c 097c 087c 0a83 0801  .|.|.|.|.|.|....
+00001840: 0074 05a0 067c 087c 097c 0064 0464 07a1  .t...|.|.|.d.d..
+00001850: 0501 0064 0653 0029 0c61 5c03 0000 0a20  ...d.S.).a\.... 
+00001860: 2020 2057 6520 6861 7665 2061 2073 696e     We have a sin
+00001870: 676c 6520 5461 736b 206f 7220 6120 6c69  gle Task or a li
+00001880: 7374 206f 6620 5461 736b 732e 2020 4f75  st of Tasks.  Ou
+00001890: 7470 7574 2069 742f 7468 656d 2e0a 2020  tput it/them..  
+000018a0: 2020 2020 2020 3a70 6172 616d 206f 7574        :param out
+000018b0: 7075 745f 6c69 7374 3a20 6c69 7374 206f  put_list: list o
+000018c0: 6620 6f75 7470 7574 206c 696e 6573 2067  f output lines g
+000018d0: 656e 6572 6174 6564 2074 6875 7320 6661  enerated thus fa
+000018e0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+000018f0: 206f 7572 5f74 6173 6b5f 6e61 6d65 3a20   our_task_name: 
+00001900: 6e61 6d65 206f 6620 5461 736b 0a20 2020  name of Task.   
+00001910: 2020 2020 203a 7061 7261 6d20 6f75 725f       :param our_
+00001920: 7461 736b 5f65 6c65 6d65 6e74 3a20 5461  task_element: Ta
+00001930: 736b 2078 6d6c 2065 6c65 6d65 6e74 0a20  sk xml element. 
+00001940: 2020 2020 2020 203a 7061 7261 6d20 7461         :param ta
+00001950: 736b 5f6c 6973 743a 2054 6173 6b20 6c69  sk_list: Task li
+00001960: 7374 0a20 2020 2020 2020 203a 7061 7261  st.        :para
+00001970: 6d20 7072 6f6a 6563 745f 6e61 6d65 3a20  m project_name: 
+00001980: 6e61 6d65 206f 6620 6375 7272 656e 7420  name of current 
+00001990: 5072 6f6a 6563 740a 2020 2020 2020 2020  Project.        
+000019a0: 3a70 6172 616d 2070 726f 6669 6c65 5f6e  :param profile_n
+000019b0: 616d 653a 206e 616d 6520 6f66 2063 7572  ame: name of cur
+000019c0: 7265 6e74 2050 726f 6669 6c65 0a20 2020  rent Profile.   
+000019d0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
+000019e0: 5f6f 665f 666f 756e 645f 7461 736b 733a  _of_found_tasks:
+000019f0: 206c 6973 7420 6f66 2054 6173 6b73 2066   list of Tasks f
+00001a00: 6f75 6e64 2073 6f20 6661 720a 2020 2020  ound so far.    
+00001a10: 2020 2020 3a70 6172 616d 2068 6561 6469      :param headi
+00001a20: 6e67 3a20 6375 7272 656e 7420 6865 6164  ng: current head
+00001a30: 696e 670a 2020 2020 2020 2020 3a70 6172  ing.        :par
+00001a40: 616d 2063 6f6c 6f72 6d61 703a 2063 6f6c  am colormap: col
+00001a50: 6f72 7320 746f 2075 7365 2069 6e20 6f75  ors to use in ou
+00001a60: 7470 7574 0a20 2020 2020 2020 203a 7061  tput.        :pa
+00001a70: 7261 6d20 7072 6f67 7261 6d5f 6172 6773  ram program_args
+00001a80: 3a20 7275 6e74 696d 6520 6172 6775 6d65  : runtime argume
+00001a90: 6e74 730a 2020 2020 2020 2020 3a70 6172  nts.        :par
+00001aa0: 616d 2061 6c6c 5f74 6173 6b65 725f 6974  am all_tasker_it
+00001ab0: 656d 733a 2061 6c6c 2050 726f 6a65 6374  ems: all Project
+00001ac0: 732f 5072 6f66 696c 6573 2f54 6173 6b73  s/Profiles/Tasks
+00001ad0: 2f53 6365 6e65 730a 2020 2020 2020 2020  /Scenes.        
+00001ae0: 3a70 6172 616d 2066 6f75 6e64 5f69 7465  :param found_ite
+00001af0: 6d73 3a20 7369 6e67 6c65 2050 726f 6a65  ms: single Proje
+00001b00: 6374 2f50 726f 6669 6c65 2f54 6173 6b20  ct/Profile/Task 
+00001b10: 746f 2073 6561 7263 6820 666f 720a 2020  to search for.  
+00001b20: 2020 2020 2020 3a70 6172 616d 2064 6f5f        :param do_
+00001b30: 6578 7472 613a 2066 6c61 6720 746f 2064  extra: flag to d
+00001b40: 6f2f 6f75 7470 7574 2065 7874 7261 2054  o/output extra T
+00001b50: 6173 6b20 7374 7566 660a 2020 2020 2020  ask stuff.      
+00001b60: 2020 3a72 6574 7572 6e3a 2054 7275 6520    :return: True 
+00001b70: 6966 2077 6520 6172 6520 7365 6172 6368  if we are search
+00001b80: 696e 6720 666f 7220 6120 7369 6e67 6c65  ing for a single
+00001b90: 2054 6173 6b20 616e 6420 666f 756e 6420   Task and found 
+00001ba0: 6974 2e20 204f 7468 6572 7769 7365 2c20  it.  Otherwise, 
+00001bb0: 4661 6c73 650a 2020 2020 7201 0000 0072  False.    r....r
+00001bc0: 4c00 0000 da14 6469 7370 6c61 795f 6465  L.....display_de
+00001bd0: 7461 696c 5f6c 6576 656c e903 0000 00fa  tail_level......
+00001be0: 0120 4672 0f00 0000 724e 0000 0054 7213  . Fr....rN...Tr.
+00001bf0: 0000 0072 5000 0000 2907 7251 0000 0072  ...rP...).rQ...r
+00001c00: 4d00 0000 7203 0000 0072 0400 0000 7256  M...r....r....rV
+00001c10: 0000 0072 5200 0000 7254 0000 0029 1072  ...rR...rT...).r
+00001c20: 4200 0000 7241 0000 0072 4800 0000 7247  B...rA...rH...rG
+00001c30: 0000 0072 4300 0000 7244 0000 0072 4900  ...rC...rD...rI.
+00001c40: 0000 7245 0000 0072 0b00 0000 724b 0000  ..rE...r....rK..
+00001c50: 0072 4a00 0000 7246 0000 0072 5700 0000  .rJ...rF...rW...
+00001c60: 724d 0000 00da 0c6b 6964 5f61 7070 5f69  rM.....kid_app_i
+00001c70: 6e66 6fda 0870 7269 6f72 6974 7972 2500  nfo..priorityr%.
+00001c80: 0000 7225 0000 0072 2600 0000 da0b 6f75  ..r%...r&.....ou
+00001c90: 7470 7574 5f74 6173 6b35 0100 0073 4800  tput_task5...sH.
+00001ca0: 0000 0c21 1003 0c01 1601 0e01 1601 1003  ...!............
+00001cb0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001cc0: 0201 0201 0201 0201 0201 04f4 040e 0401  ................
+00001cd0: 1202 0202 0201 0201 0201 0201 0201 0201  ................
+00001ce0: 0201 0201 04f8 120b 0402 725d 0000 0029  ..........r]...)
+00001cf0: 24da 1664 6566 7573 6564 786d 6c2e 456c  $..defusedxml.El
+00001d00: 656d 656e 7454 7265 6572 1600 0000 da15  ementTreer......
+00001d10: 6d61 7074 6173 6b65 722e 7372 632e 6163  maptasker.src.ac
+00001d20: 7469 6f6e 65da 0373 7263 da07 6163 7469  tione..src..acti
+00001d30: 6f6e 6572 1c00 0000 da15 6d61 7074 6173  oner......maptas
+00001d40: 6b65 722e 7372 632e 6f75 7470 7574 6cda  ker.src.outputl.
+00001d50: 076f 7574 7075 746c 7252 0000 00da 156d  .outputlrR.....m
+00001d60: 6170 7461 736b 6572 2e73 7263 2e78 6d6c  aptasker.src.xml
+00001d70: 6461 7461 7202 0000 00da 146d 6170 7461  datar......mapta
+00001d80: 736b 6572 2e73 7263 2e6b 6964 6170 7072  sker.src.kidappr
+00001d90: 0300 0000 da16 6d61 7074 6173 6b65 722e  ......maptasker.
+00001da0: 7372 632e 7072 696f 7269 7479 7204 0000  src.priorityr...
+00001db0: 00da 146d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
+00001dc0: 2e67 6574 6964 7372 0500 0000 da16 6d61  .getidsr......ma
+00001dd0: 7074 6173 6b65 722e 7372 632e 7379 7363  ptasker.src.sysc
+00001de0: 6f6e 7374 7206 0000 0072 0700 0000 7208  onstr....r....r.
+00001df0: 0000 00da 176d 6170 7461 736b 6572 2e73  .....maptasker.s
+00001e00: 7263 2e73 6865 6c6c 736f 7274 7209 0000  rc.shellsortr...
+00001e10: 00da 0b45 6c65 6d65 6e74 5472 6565 da03  ...ElementTree..
+00001e20: 584d 4cda 0464 6963 74da 046c 6973 7472  XML..dict..listr
+00001e30: 2700 0000 721e 0000 00da 0574 7570 6c65  '...r......tuple
+00001e40: 7234 0000 0072 3a00 0000 da04 626f 6f6c  r4...r:.....bool
+00001e50: 7240 0000 0072 5600 0000 725d 0000 0072  r@...rV...r]...r
+00001e60: 2500 0000 7225 0000 0072 2500 0000 7226  %...r%...r%...r&
+00001e70: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001e80: 0073 c600 0000 080d 1201 1202 0c01 0c01  .s..............
+00001e90: 0c01 0c01 0c01 0c01 0c01 0c02 0207 0601  ................
+00001ea0: 02ff 0201 02ff 0201 02ff 0202 0afe 0245  ...............E
+00001eb0: 0201 02ff 0202 02fe 0203 02fd 0204 02fc  ................
+00001ec0: 0205 02fb 0e06 0afa 0234 0201 02ff 0201  .........4......
+00001ed0: 02ff 0201 02ff 0c02 0afe 161b 021c 0201  ................
+00001ee0: 02ff 0202 02fe 0203 02fd 0204 02fc 0205  ................
+00001ef0: 02fb 0206 02fa 0207 02f9 0608 02f8 0209  ................
+00001f00: 02f7 020a 02f6 020b 02f5 020c 02f4 020d  ................
+00001f10: 0af3 0264 0201 02ff 0202 02fe 0603 02fd  ...d............
+00001f20: 0204 02fc 0205 02fb 0206 02fa 0207 02f9  ................
+00001f30: 0208 02f8 0209 02f7 020a 02f6 020b 02f5  ................
+00001f40: 020c 02f4 020d 02f3 020e 0ef2            ............
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/taskuniq.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/taskuniq.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 17:52:29 2023 UTC, .py size: 9526 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,215 +1,212 @@
-00000000: 6f0d 0d0a 0000 0000 dd63 2c64 3625 0000  o........c,d6%..
+00000000: 6f0d 0d0a 0000 0000 1e21 3c64 f125 0000  o........!<d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
+00000020: 0012 0000 0040 0000 0073 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 0200 0100 6d05 5a06 0100  d.l.m.....m.Z...
 00000050: 6400 6402 6c07 6d04 0200 0100 6d08 5a08  d.d.l.m.....m.Z.
 00000060: 0100 6400 6403 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6404 6c09 6d0b 5a0b 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
-00000080: 6d0c 5a0c 0100 6406 6501 650d 1900 6407  m.Z...d.e.e...d.
-00000090: 6502 6501 650d 1900 6501 6602 1900 6408  e.e.e...e.f...d.
-000000a0: 6501 650d 1900 6409 650e 640a 650e 640b  e.e...d.e.d.e.d.
-000000b0: 650e 640c 6402 660e 640d 640e 8404 5a0f  e.d.d.f.d.d...Z.
-000000c0: 640f 6510 6602 6410 6411 8404 5a11 6406  d.e.f.d.d...Z.d.
-000000d0: 6501 650d 1900 6407 6501 6412 6501 650d  e.e...d.e.d.e.e.
-000000e0: 1900 640b 650e 6409 650e 6413 650d 640a  ..d.e.d.e.d.e.d.
-000000f0: 650e 6414 650e 640c 6402 6612 6415 6416  e.d.e.d.d.f.d.d.
-00000100: 8404 5a12 6402 5300 2917 e900 0000 0029  ..Z.d.S.)......)
-00000110: 02da 044c 6973 74da 0555 6e69 6f6e 4e29  ...List..UnionN)
-00000120: 01da 0b46 4f4e 545f 544f 5f55 5345 2901  ...FONT_TO_USE).
-00000130: da11 554e 4b4e 4f57 4e5f 5441 534b 5f4e  ..UNKNOWN_TASK_N
-00000140: 414d 4529 01da 0a4e 4f5f 5052 4f4a 4543  AME)...NO_PROJEC
-00000150: 54da 0b6f 7574 7075 745f 6c69 7374 da16  T..output_list..
-00000160: 7072 6f6a 6563 7473 5f77 6974 685f 6e6f  projects_with_no
-00000170: 5f74 6173 6b73 da19 7072 6f6a 6563 7473  _tasks..projects
-00000180: 5f77 6974 686f 7574 5f70 726f 6669 6c65  _without_profile
-00000190: 73da 0b66 6f75 6e64 5f69 7465 6d73 da08  s..found_items..
-000001a0: 636f 6c6f 726d 6170 da0c 7072 6f67 7261  colormap..progra
-000001b0: 6d5f 6172 6773 da06 7265 7475 726e 6306  m_args..returnc.
-000001c0: 0000 0000 0000 0000 0000 0007 0000 000d  ................
-000001d0: 0000 0043 0000 0073 c400 0000 7400 7c01  ...C...s....t.|.
-000001e0: 8301 6401 6b04 7234 7c03 6402 1900 7334  ..d.k.r4|.d...s4
-000001f0: 7401 a002 7c04 7c05 7c00 6401 6403 7c04  t...|.|.|.d.d.|.
-00000200: 6404 1900 9b00 7403 9b00 6405 9d04 a105  d.....t...d.....
-00000210: 0100 7c01 4400 5d16 7d06 7401 a002 7c04  ..|.D.].}.t...|.
-00000220: 7c05 7c00 6406 6407 7c04 6404 1900 9b00  |.|.d.d.|.d.....
-00000230: 7403 9b00 6408 7c06 9b00 6409 9d06 a105  t...d.|...d.....
-00000240: 0100 711d 7c02 7260 7401 a002 7c04 7c05  ..q.|.r`t...|.|.
-00000250: 7c00 6401 640a 7c04 6404 1900 9b00 7403  |.d.d.|.d.....t.
-00000260: 9b00 640b 9d04 a105 0100 7c02 4400 5d16  ..d.......|.D.].
-00000270: 7d06 7401 a002 7c04 7c05 7c00 6406 6407  }.t...|.|.|.d.d.
-00000280: 7c04 6404 1900 9b00 7403 9b00 6408 7c06  |.d.....t...d.|.
-00000290: 9b00 640c 9d06 a105 0100 7149 6400 5300  ..d.......qId.S.
-000002a0: 290d 4e72 0100 0000 da11 7369 6e67 6c65  ).Nr......single
-000002b0: 5f74 6173 6b5f 666f 756e 647a 173c 6872  _task_foundz.<hr
-000002c0: 3e3c 7370 616e 2073 7479 6c65 3d22 636f  ><span style="co
-000002d0: 6c6f 723a da17 7472 6169 6c69 6e67 5f63  lor:..trailing_c
-000002e0: 6f6d 6d65 6e74 735f 636f 6c6f 727a 2a3e  omments_colorz*>
-000002f0: 3c65 6d3e 5072 6f6a 6563 7473 2057 6974  <em>Projects Wit
-00000300: 686f 7574 2054 6173 6b73 2e2e 2e3c 2f65  hout Tasks...</e
-00000310: 6d3e 3c2f 7370 616e 3ee9 0400 0000 fa13  m></span>.......
-00000320: 3c73 7061 6e20 7374 796c 653d 2263 6f6c  <span style="col
-00000330: 6f72 3a7a 093e 5072 6f6a 6563 7420 7a14  or:z.>Project z.
-00000340: 2068 6173 206e 6f20 5461 736b 733c 2f73   has no Tasks</s
-00000350: 7061 6e3e 7a16 3c68 723e 3c73 7061 6e20  pan>z.<hr><span 
-00000360: 7374 796c 653d 636f 6c6f 723a 7a26 3e3c  style=color:z&><
-00000370: 656d 3e50 726f 6a65 6374 7320 5769 7468  em>Projects With
-00000380: 6f75 7420 5072 6f66 696c 6573 2e2e 2e3c  out Profiles...<
-00000390: 2f65 6d3e 7a10 2068 6173 206e 6f20 5072  /em>z. has no Pr
-000003a0: 6f66 696c 6573 2904 da03 6c65 6eda 0c62  ofiles)...len..b
-000003b0: 7569 6c64 5f6f 7574 7075 74da 096d 795f  uild_output..my_
-000003c0: 6f75 7470 7574 7204 0000 0029 0772 0700  outputr....).r..
-000003d0: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-000003e0: 0072 0b00 0000 720c 0000 00da 0469 7465  .r....r......ite
-000003f0: 6da9 0072 1600 0000 fa77 2f55 7365 7273  m..r.....w/Users
-00000400: 2f6d 696b 7275 6269 6e2f 4c69 6272 6172  /mikrubin/Librar
-00000410: 792f 436c 6f75 6453 746f 7261 6765 2f47  y/CloudStorage/G
-00000420: 6f6f 676c 6544 7269 7665 2d6d 696b 7275  oogleDrive-mikru
-00000430: 6269 6e40 676d 6169 6c2e 636f 6d2f 4d79  bin@gmail.com/My
-00000440: 2044 7269 7665 2f50 7974 686f 6e2f 6d61   Drive/Python/ma
-00000450: 7074 6173 6b65 722f 6d61 7074 6173 6b65  ptasker/maptaske
-00000460: 722f 7372 632f 7461 736b 756e 6971 2e70  r/src/taskuniq.p
-00000470: 79da 2270 726f 6365 7373 5f6d 6973 7369  y."process_missi
-00000480: 6e67 5f74 6173 6b73 5f61 6e64 5f70 726f  ng_tasks_and_pro
-00000490: 6669 6c65 731a 0000 0073 6600 0000 1409  files....sf.....
-000004a0: 0401 0201 0201 0201 0201 0202 0601 02ff  ................
-000004b0: 0201 06ff 04fa 080b 0401 0201 0201 0201  ................
-000004c0: 0201 0a02 0201 04ff 0201 06ff 06fa 040c  ................
-000004d0: 0401 0201 0201 0201 0201 0202 0601 02ff  ................
-000004e0: 0201 06ff 04fa 080b 0401 0201 0201 0201  ................
-000004f0: 0201 0202 0601 02ff 0201 04ff 0202 06fe  ................
-00000500: 06fa 040b 7218 0000 00da 0c68 6176 655f  ....r......have_
-00000510: 6865 6164 696e 6763 0b00 0000 0000 0000  headingc........
-00000520: 0000 0000 1300 0000 0f00 0000 4300 0000  ............C...
-00000530: 7352 0100 0064 017d 0b64 025c 027d 0c7d  sR...d.}.d.\.}.}
-00000540: 0d74 00a0 017c 017c 077c 0a64 0319 00a1  .t...|.|.|.d....
-00000550: 035c 027d 0e7d 0f74 00a0 027c 017c 0267  .\.}.}.t...|.|.g
-00000560: 0064 017c 0a64 0419 00a1 055c 027d 107d  .d.|.d.....\.}.}
-00000570: 117c 1174 036b 0272 3974 039b 0064 057c  .|.t.k.r9t...d.|
-00000580: 019b 009d 037d 1174 00a0 047c 017c 0a64  .....}.t...|.|.d
-00000590: 0619 00a1 0272 367c 067c 0d7c 0566 0353  .....r6|.|.|.f.S
-000005a0: 0064 077d 0c6e 027c 117d 0b7c 0564 0837  .d.}.n.|.}.|.d.7
-000005b0: 007d 057c 0673 6a74 05a0 067c 097c 037c  .}.|.sjt...|.|.|
-000005c0: 0064 0964 0aa1 0501 0074 05a0 067c 097c  .d.d.....t...|.|
-000005d0: 037c 0064 0964 0b7c 0964 0c19 009b 007c  .|.d.d.|.d.....|
-000005e0: 0364 0d19 009b 0064 0e9d 0464 0f17 00a1  .d.....d...d....
-000005f0: 0501 0074 05a0 067c 097c 037c 0064 0864  ...t...|.|.|.d.d
-00000600: 01a1 0501 0064 077d 067c 0c73 887c 0e74  .....d.}.|.s.|.t
-00000610: 076b 0372 887c 0364 1019 0072 807c 1164  .k.r.|.d...r.|.d
-00000620: 117c 019b 0064 127c 0e9b 0064 139d 0537  .|...d.|...d...7
-00000630: 007d 116e 087c 1164 127c 0e9b 0064 139d  .}.n.|.d.|...d..
-00000640: 0337 007d 117c 0c72 907c 0364 1419 0064  .7.}.|.r.|.d...d
-00000650: 156b 0272 a47c 1167 017d 1274 00a0 087c  .k.r.|.g.}.t...|
-00000660: 007c 0b7c 107c 127c 0e64 1667 007c 087c  .|.|.|.|.d.g.|.|
-00000670: 097c 037c 0a7c 0464 17a1 0d7d 0d7c 067c  .|.|.|.d...}.|.|
-00000680: 0d7c 0566 0353 0029 184e da00 2902 4646  .|.f.S.).N..).FF
-00000690: da0c 616c 6c5f 7072 6f6a 6563 7473 da09  ..all_projects..
-000006a0: 616c 6c5f 7461 736b 737a 1526 6e62 7370  all_tasksz.&nbsp
-000006b0: 3b26 6e62 7370 3b54 6173 6b20 4944 3a20  ;&nbsp;Task ID: 
-000006c0: da0a 616c 6c5f 7363 656e 6573 54e9 0100  ..all_scenesT...
-000006d0: 0000 7201 0000 007a 043c 6872 3e72 1100  ..r....z.<hr>r..
-000006e0: 0000 720f 0000 00da 0b66 6f6e 745f 746f  ..r......font_to
-000006f0: 5f75 7365 fa01 3e7a 3154 6173 6b73 2074  _use..>z1Tasks t
-00000700: 6861 7420 6172 6520 6e6f 7420 6361 6c6c  hat are not call
-00000710: 6564 2062 7920 616e 7920 5072 6f66 696c  ed by any Profil
-00000720: 652e 2e2e 3c73 7061 6e3e da05 6465 6275  e...<span>..debu
-00000730: 677a 0f20 7769 7468 2054 6173 6b20 4944  gz. with Task ID
-00000740: 3a20 7a0f 202e 2e2e 696e 2050 726f 6a65  : z. ...in Proje
-00000750: 6374 207a 1420 3c65 6d3e 4e6f 2050 726f  ct z. <em>No Pro
-00000760: 6669 6c65 3c2f 656d 3eda 1464 6973 706c  file</em>..displ
-00000770: 6179 5f64 6574 6169 6c5f 6c65 7665 6ce9  ay_detail_level.
-00000780: 0300 0000 da04 4e6f 6e65 4629 09da 0574  ......NoneF)...t
-00000790: 6173 6b73 da19 6765 745f 7072 6f6a 6563  asks..get_projec
-000007a0: 745f 666f 725f 736f 6c6f 5f74 6173 6bda  t_for_solo_task.
-000007b0: 0d67 6574 5f74 6173 6b5f 6e61 6d65 7205  .get_task_namer.
-000007c0: 0000 00da 0d74 6173 6b5f 696e 5f73 6365  .....task_in_sce
-000007d0: 6e65 7213 0000 0072 1400 0000 7206 0000  ner....r....r...
-000007e0: 00da 0b6f 7574 7075 745f 7461 736b 2913  ...output_task).
-000007f0: 7207 0000 00da 0774 6173 6b5f 6964 da0b  r......task_id..
-00000800: 666f 756e 645f 7461 736b 7372 0c00 0000  found_tasksr....
-00000810: 720a 0000 00da 1275 6e6e 616d 6564 5f74  r......unnamed_t
-00000820: 6173 6b5f 636f 756e 7472 1900 0000 7208  ask_countr....r.
-00000830: 0000 00da 0768 6561 6469 6e67 720b 0000  .....headingr...
-00000840: 00da 1061 6c6c 5f74 6173 6b65 725f 6974  ...all_tasker_it
-00000850: 656d 73da 0d74 6865 5f74 6173 6b5f 6e61  ems..the_task_na
-00000860: 6d65 5a0c 756e 6b6e 6f77 6e5f 7461 736b  meZ.unknown_task
-00000870: da0d 7370 6563 6966 6963 5f74 6173 6bda  ..specific_task.
-00000880: 0c70 726f 6a65 6374 5f6e 616d 655a 0b74  .project_nameZ.t
-00000890: 6865 5f70 726f 6a65 6374 da0c 7461 736b  he_project..task
-000008a0: 5f65 6c65 6d65 6e74 da09 7461 736b 5f6e  _element..task_n
-000008b0: 616d 65da 0974 6173 6b5f 6c69 7374 7216  ame..task_listr.
-000008c0: 0000 0072 1600 0000 7217 0000 00da 2170  ...r....r.....!p
-000008d0: 726f 6365 7373 5f73 6f6c 6f5f 7461 736b  rocess_solo_task
-000008e0: 5f77 6974 685f 6e6f 5f70 726f 6669 6c65  _with_no_profile
-000008f0: 5a00 0000 737a 0000 0004 0d08 0104 030a  Z...sz..........
-00000900: 0108 ff04 050e 0108 ff08 030e 0110 020a  ................
-00000910: 0106 0104 0208 0104 0304 010a 0104 ff04  ................
-00000920: 0302 0102 0102 0102 0102 0206 0102 ff06  ................
-00000930: 0106 ff02 0202 fe04 fa04 0b0a 0104 ff04  ................
-00000940: 030c 0208 0102 0110 0106 ff10 0504 030c  ................
-00000950: 0106 0204 0302 0102 0102 0102 0102 0102  ................
-00000960: 0102 0102 0102 0102 0102 0102 0102 0104  ................
-00000970: f30a 0f72 3500 0000 da10 666f 756e 645f  ...r5.....found_
-00000980: 7461 736b 735f 6c69 7374 722d 0000 0072  tasks_listr-...r
-00000990: 2e00 0000 6308 0000 0000 0000 0000 0000  ....c...........
-000009a0: 000d 0000 000d 0000 0043 0000 0073 0001  .........C...s..
-000009b0: 0000 6401 7d08 6402 7d09 6403 7d0a 7c07  ..d.}.d.}.d.}.|.
-000009c0: 6404 1900 4400 5d21 7d0b 7c04 6405 1900  d...D.]!}.|.d...
-000009d0: 7212 0100 6e1a 7c0b 7c02 7601 722b 7400  r...n.|.|.v.r+t.
-000009e0: 7c00 7c0b 7c02 7c03 7c04 7c08 7c0a 7c01  |.|.|.|.|.|.|.|.
-000009f0: 7c05 7c06 7c07 830b 5c03 7d0a 7d0c 7d08  |.|.|...\.}.}.}.
-00000a00: 7c0c 722b 0100 6e01 710a 7c08 6401 6b04  |.r+..n.q.|.d.k.
-00000a10: 7268 7c03 6406 1900 6401 6b04 723f 7401  rh|.d...d.k.r?t.
-00000a20: a002 7c06 7c03 7c00 6401 6402 a105 0100  ..|.|.|.d.d.....
-00000a30: 7401 a002 7c06 7c03 7c00 6407 6402 a105  t...|.|.|.d.d...
-00000a40: 0100 7c04 6405 1900 7368 7c03 6406 1900  ..|.d...sh|.d...
-00000a50: 6401 6b03 7268 7401 a002 7c06 7c03 7c00  d.k.rht...|.|.|.
-00000a60: 6401 6408 7c06 6409 1900 9b00 7c03 640a  d.d.|.d.....|.d.
-00000a70: 1900 9b00 640b 7c08 9b00 640c 9d06 a105  ....d.|...d.....
-00000a80: 0100 7c09 640d 7500 7275 7401 a002 7c06  ..|.d.u.rut...|.
-00000a90: 7c03 7c00 6407 6402 a105 0100 7401 a002  |.|.d.d.....t...
-00000aa0: 7c06 7c03 7c00 6407 6402 a105 0100 6400  |.|.|.d.d.....d.
-00000ab0: 5300 290e 4e72 0100 0000 721a 0000 0046  S.).Nr....r....F
-00000ac0: 721c 0000 0072 0e00 0000 7222 0000 0072  r....r....r"...r
-00000ad0: 2300 0000 7211 0000 00da 1275 6e6b 6e6f  #...r......unkno
-00000ae0: 776e 5f74 6173 6b5f 636f 6c6f 7272 1f00  wn_task_colorr..
-00000af0: 0000 7a16 3e54 6865 7265 2061 7265 2061  ..z.>There are a
-00000b00: 2074 6f74 616c 206f 6620 7a34 2075 6e6e   total of z4 unn
-00000b10: 616d 6564 2054 6173 6b73 206e 6f74 2061  amed Tasks not a
-00000b20: 7373 6f63 6961 7465 6420 7769 7468 2061  ssociated with a
-00000b30: 2050 726f 6669 6c65 213c 2f73 7061 6e3e   Profile!</span>
-00000b40: 5429 0372 3500 0000 7213 0000 0072 1400  T).r5...r....r..
-00000b50: 0000 290d 7207 0000 0072 0800 0000 7236  ..).r....r....r6
-00000b60: 0000 0072 0c00 0000 720a 0000 0072 2d00  ...r....r....r-.
-00000b70: 0000 720b 0000 0072 2e00 0000 722c 0000  ..r....r....r,..
-00000b80: 0072 3300 0000 7219 0000 0072 2a00 0000  .r3...r....r*...
-00000b90: 7230 0000 0072 1600 0000 7216 0000 0072  r0...r....r....r
-00000ba0: 1700 0000 da23 7072 6f63 6573 735f 7461  .....#process_ta
-00000bb0: 736b 735f 6e6f 745f 6361 6c6c 6564 5f62  sks_not_called_b
-00000bc0: 795f 7072 6f66 696c 65b7 0000 0073 7000  y_profile....sp.
-00000bd0: 0000 040a 0401 0401 0c03 0201 0201 04ff  ................
-00000be0: 0403 0806 0202 0201 0201 0201 0201 0201  ................
-00000bf0: 0201 0201 0201 0201 0201 0201 02f5 08ff  ................
-00000c00: 040f 0401 0280 0803 0c01 1201 0401 0a01  ................
-00000c10: 04ff 0605 02ff 0c02 0402 0201 0201 0201  ................
-00000c20: 0201 0202 0601 02ff 0601 04ff 0202 06fe  ................
-00000c30: 04fa 080d 0401 0a01 04ff 0404 0a01 04ff  ................
-00000c40: 0403 7238 0000 0029 13da 0674 7970 696e  ..r8...)...typin
-00000c50: 6772 0200 0000 7203 0000 00da 156d 6170  gr....r......map
-00000c60: 7461 736b 6572 2e73 7263 2e6f 7574 7075  tasker.src.outpu
-00000c70: 746c da03 7372 63da 076f 7574 7075 746c  tl..src..outputl
-00000c80: 7213 0000 00da 136d 6170 7461 736b 6572  r......maptasker
-00000c90: 2e73 7263 2e74 6173 6b73 7225 0000 00da  .src.tasksr%....
-00000ca0: 166d 6170 7461 736b 6572 2e73 7263 2e73  .maptasker.src.s
-00000cb0: 7973 636f 6e73 7472 0400 0000 7205 0000  ysconstr....r...
-00000cc0: 0072 0600 0000 da03 7374 72da 0464 6963  .r......str..dic
-00000cd0: 7472 1800 0000 da04 626f 6f6c 7235 0000  tr......boolr5..
-00000ce0: 0072 3800 0000 7216 0000 0072 1600 0000  .r8...r....r....
-00000cf0: 7216 0000 0072 1700 0000 da08 3c6d 6f64  r....r......<mod
-00000d00: 756c 653e 0100 0000 7356 0000 0010 0d12  ule>....sV......
-00000d10: 0212 010c 010c 010c 0102 0606 0102 ff0e  ................
-00000d20: 0202 fe06 0302 fd02 0402 fc02 0502 fb02  ................
-00000d30: 0602 fa02 070a f902 4002 070a f902 5d06  ........@.....].
-00000d40: 0102 ff02 0202 fe06 0302 fd02 0402 fc02  ................
-00000d50: 0502 fb02 0602 fa02 0702 f902 0802 f802  ................
-00000d60: 090e f7                                  ...
+00000070: 6404 6c0b 6d0c 5a0c 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
+00000080: 6d0d 5a0d 0100 6400 6406 6c0b 6d0e 5a0e  m.Z...d.d.l.m.Z.
+00000090: 0100 6407 6501 650f 1900 6408 6502 6501  ..d.e.e...d.e.e.
+000000a0: 650f 1900 6501 6602 1900 6409 6501 650f  e...e.f...d.e.e.
+000000b0: 1900 640a 6510 640b 6510 640c 6510 640d  ..d.e.d.e.d.e.d.
+000000c0: 6402 660e 640e 640f 8404 5a11 6410 6512  d.f.d.d...Z.d.e.
+000000d0: 6602 6411 6412 8404 5a13 6407 6501 650f  f.d.d...Z.d.e.e.
+000000e0: 1900 6408 6501 6413 6501 650f 1900 640c  ..d.e.d.e.e...d.
+000000f0: 6510 640a 6510 6414 650f 640b 6510 6415  e.d.e.d.e.d.e.d.
+00000100: 6510 640d 6402 6612 6416 6417 8404 5a14  e.d.d.f.d.d...Z.
+00000110: 6402 5300 2918 e900 0000 0029 02da 044c  d.S.)......)...L
+00000120: 6973 74da 0555 6e69 6f6e 4e29 01da 0b66  ist..UnionN)...f
+00000130: 6f72 6d61 745f 6874 6d6c 2901 da0b 464f  ormat_html)...FO
+00000140: 4e54 5f54 4f5f 5553 4529 01da 1155 4e4b  NT_TO_USE)...UNK
+00000150: 4e4f 574e 5f54 4153 4b5f 4e41 4d45 2901  NOWN_TASK_NAME).
+00000160: da0a 4e4f 5f50 524f 4a45 4354 da0b 6f75  ..NO_PROJECT..ou
+00000170: 7470 7574 5f6c 6973 74da 1670 726f 6a65  tput_list..proje
+00000180: 6374 735f 7769 7468 5f6e 6f5f 7461 736b  cts_with_no_task
+00000190: 73da 1970 726f 6a65 6374 735f 7769 7468  s..projects_with
+000001a0: 6f75 745f 7072 6f66 696c 6573 da0b 666f  out_profiles..fo
+000001b0: 756e 645f 6974 656d 73da 0863 6f6c 6f72  und_items..color
+000001c0: 6d61 70da 0c70 726f 6772 616d 5f61 7267  map..program_arg
+000001d0: 73da 0672 6574 7572 6e63 0600 0000 0000  s..returnc......
+000001e0: 0000 0000 0000 0700 0000 0e00 0000 4300  ..............C.
+000001f0: 0000 73b8 0000 0074 007c 0183 0164 016b  ..s....t.|...d.k
+00000200: 0472 317c 0364 0219 0073 3174 01a0 027c  .r1|.d...s1t...|
+00000210: 047c 057c 0064 0174 037c 0464 0364 0464  .|.|.d.t.|.d.d.d
+00000220: 0564 0683 05a1 0501 007c 0144 005d 157d  .d.......|.D.].}
+00000230: 0674 01a0 027c 047c 057c 0064 0774 037c  .t...|.|.|.d.t.|
+00000240: 0464 0364 0464 087c 069b 0064 099d 0364  .d.d.d.|...d...d
+00000250: 0683 05a1 0501 0071 1b7c 0272 5a74 01a0  .......q.|.rZt..
+00000260: 027c 047c 057c 0064 0174 037c 0464 0364  .|.|.|.d.t.|.d.d
+00000270: 0a64 0b64 0683 05a1 0501 007c 0244 005d  .d.d.......|.D.]
+00000280: 157d 0674 01a0 027c 047c 057c 0064 0774  .}.t...|.|.|.d.t
+00000290: 037c 0464 0364 0464 0c7c 069b 0064 0d9d  .|.d.d.d.|...d..
+000002a0: 0364 0683 05a1 0501 0071 4464 0053 0029  .d.......qDd.S.)
+000002b0: 0e4e 7201 0000 00da 1173 696e 676c 655f  .Nr......single_
+000002c0: 7461 736b 5f66 6f75 6e64 da17 7472 6169  task_found..trai
+000002d0: 6c69 6e67 5f63 6f6d 6d65 6e74 735f 636f  ling_comments_co
+000002e0: 6c6f 72da 007a 263c 6872 3e3c 656d 3e50  lor..z&<hr><em>P
+000002f0: 726f 6a65 6374 7320 5769 7468 6f75 7420  rojects Without 
+00000300: 5461 736b 732e 2e2e 3c2f 656d 3e54 e904  Tasks...</em>T..
+00000310: 0000 007a 0850 726f 6a65 6374 207a 1c20  ...z.Project z. 
+00000320: 6861 7320 6e6f 203c 656d 3e4e 616d 6564  has no <em>Named
+00000330: 3c2f 656d 3e20 5461 736b 737a 043c 6272  </em> Tasksz.<br
+00000340: 3e7a 253c 656d 3e50 726f 6a65 6374 7320  >z%<em>Projects 
+00000350: 5769 7468 6f75 7420 5072 6f66 696c 6573  Without Profiles
+00000360: 2e2e 2e3c 2f65 6d3e 7a09 3e50 726f 6a65  ...</em>z.>Proje
+00000370: 6374 207a 1020 6861 7320 6e6f 2050 726f  ct z. has no Pro
+00000380: 6669 6c65 7329 04da 036c 656e da0c 6275  files)...len..bu
+00000390: 696c 645f 6f75 7470 7574 da09 6d79 5f6f  ild_output..my_o
+000003a0: 7574 7075 7472 0400 0000 2907 7208 0000  utputr....).r...
+000003b0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+000003c0: 720c 0000 0072 0d00 0000 da04 6974 656d  r....r......item
+000003d0: a900 7217 0000 00fa 772f 5573 6572 732f  ..r.....w/Users/
+000003e0: 6d69 6b72 7562 696e 2f4c 6962 7261 7279  mikrubin/Library
+000003f0: 2f43 6c6f 7564 5374 6f72 6167 652f 476f  /CloudStorage/Go
+00000400: 6f67 6c65 4472 6976 652d 6d69 6b72 7562  ogleDrive-mikrub
+00000410: 696e 4067 6d61 696c 2e63 6f6d 2f4d 7920  in@gmail.com/My 
+00000420: 4472 6976 652f 5079 7468 6f6e 2f6d 6170  Drive/Python/map
+00000430: 7461 736b 6572 2f6d 6170 7461 736b 6572  tasker/maptasker
+00000440: 2f73 7263 2f74 6173 6b75 6e69 712e 7079  /src/taskuniq.py
+00000450: da22 7072 6f63 6573 735f 6d69 7373 696e  ."process_missin
+00000460: 675f 7461 736b 735f 616e 645f 7072 6f66  g_tasks_and_prof
+00000470: 696c 6573 1b00 0000 7372 0000 0014 0904  iles....sr......
+00000480: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000490: 0102 0102 0102 fb04 fb08 0e04 0102 0102  ................
+000004a0: 0102 0102 0102 0102 0102 0102 010a 0102  ................
+000004b0: 0102 fb06 fb04 0f04 0102 0102 0102 0102  ................
+000004c0: 0102 0102 0102 0102 0102 0102 0102 fb04  ................
+000004d0: fb08 0d04 0102 0102 0102 0102 0102 0102  ................
+000004e0: 0102 0102 010a 0102 0102 fb06 fb04 0d72  ...............r
+000004f0: 1900 0000 da0c 6861 7665 5f68 6561 6469  ......have_headi
+00000500: 6e67 630b 0000 0000 0000 0000 0000 0013  ngc.............
+00000510: 0000 000f 0000 0043 0000 0073 4601 0000  .......C...sF...
+00000520: 6401 7d0b 6402 5c02 7d0c 7d0d 7400 a001  d.}.d.\.}.}.t...
+00000530: 7c01 7c07 7c0a 6403 1900 a103 5c02 7d0e  |.|.|.d.....\.}.
+00000540: 7d0f 7400 a002 7c01 7c02 6700 6401 7c0a  }.t...|.|.g.d.|.
+00000550: 6404 1900 a105 5c02 7d10 7d11 7c11 7403  d.....\.}.}.|.t.
+00000560: 6b02 7239 7403 9b00 6405 7c01 9b00 9d03  k.r9t...d.|.....
+00000570: 7d11 7400 a004 7c01 7c0a 6406 1900 a102  }.t...|.|.d.....
+00000580: 7236 7c06 7c0d 7c05 6603 5300 6407 7d0c  r6|.|.|.f.S.d.}.
+00000590: 6e02 7c11 7d0b 7c05 6408 3700 7d05 7c06  n.|.}.|.d.7.}.|.
+000005a0: 7364 7405 a006 7c09 7c03 7c00 6409 640a  sdt...|.|.|.d.d.
+000005b0: a105 0100 7405 a006 7c09 7c03 7c00 6409  ....t...|.|.|.d.
+000005c0: 7407 7c09 640b 6401 640c 6407 8305 a105  t.|.d.d.d.d.....
+000005d0: 0100 7405 a006 7c09 7c03 7c00 6408 6401  ..t...|.|.|.d.d.
+000005e0: a105 0100 6407 7d06 7c0c 7382 7c0e 7408  ....d.}.|.s.|.t.
+000005f0: 6b03 7282 7c03 640d 1900 727a 7c11 640e  k.r.|.d...rz|.d.
+00000600: 7c01 9b00 640f 7c0e 9b00 6410 9d05 3700  |...d.|...d...7.
+00000610: 7d11 6e08 7c11 640f 7c0e 9b00 6410 9d03  }.n.|.d.|...d...
+00000620: 3700 7d11 7c0c 728a 7c03 6411 1900 6412  7.}.|.r.|.d...d.
+00000630: 6b02 729e 7c11 6701 7d12 7400 a009 7c00  k.r.|.g.}.t...|.
+00000640: 7c0b 7c10 7c12 7c0e 6413 6700 7c08 7c09  |.|.|.|.d.g.|.|.
+00000650: 7c03 7c0a 7c04 6414 a10d 7d0d 7c06 7c0d  |.|.|.d...}.|.|.
+00000660: 7c05 6603 5300 2915 4e72 1100 0000 2902  |.f.S.).Nr....).
+00000670: 4646 da0c 616c 6c5f 7072 6f6a 6563 7473  FF..all_projects
+00000680: da09 616c 6c5f 7461 736b 737a 1526 6e62  ..all_tasksz.&nb
+00000690: 7370 3b26 6e62 7370 3b54 6173 6b20 4944  sp;&nbsp;Task ID
+000006a0: 3a20 da0a 616c 6c5f 7363 656e 6573 54e9  : ..all_scenesT.
+000006b0: 0100 0000 7201 0000 007a 043c 6872 3e72  ....r....z.<hr>r
+000006c0: 1000 0000 7a2b 5461 736b 7320 7468 6174  ....z+Tasks that
+000006d0: 2061 7265 206e 6f74 2063 616c 6c65 6420   are not called 
+000006e0: 6279 2061 6e79 2050 726f 6669 6c65 2e2e  by any Profile..
+000006f0: 2eda 0564 6562 7567 7a0f 2077 6974 6820  ...debugz. with 
+00000700: 5461 736b 2049 443a 207a 0f20 2e2e 2e69  Task ID: z. ...i
+00000710: 6e20 5072 6f6a 6563 7420 7a14 203c 656d  n Project z. <em
+00000720: 3e4e 6f20 5072 6f66 696c 653c 2f65 6d3e  >No Profile</em>
+00000730: da14 6469 7370 6c61 795f 6465 7461 696c  ..display_detail
+00000740: 5f6c 6576 656c e903 0000 00da 044e 6f6e  _level.......Non
+00000750: 6546 290a da05 7461 736b 73da 1967 6574  eF)...tasks..get
+00000760: 5f70 726f 6a65 6374 5f66 6f72 5f73 6f6c  _project_for_sol
+00000770: 6f5f 7461 736b da0d 6765 745f 7461 736b  o_task..get_task
+00000780: 5f6e 616d 6572 0600 0000 da0d 7461 736b  _namer......task
+00000790: 5f69 6e5f 7363 656e 6572 1400 0000 7215  _in_scener....r.
+000007a0: 0000 0072 0400 0000 7207 0000 00da 0b6f  ...r....r......o
+000007b0: 7574 7075 745f 7461 736b 2913 7208 0000  utput_task).r...
+000007c0: 00da 0774 6173 6b5f 6964 da0b 666f 756e  ...task_id..foun
+000007d0: 645f 7461 736b 7372 0d00 0000 720b 0000  d_tasksr....r...
+000007e0: 00da 1275 6e6e 616d 6564 5f74 6173 6b5f  ...unnamed_task_
+000007f0: 636f 756e 7472 1a00 0000 7209 0000 00da  countr....r.....
+00000800: 0768 6561 6469 6e67 720c 0000 00da 1061  .headingr......a
+00000810: 6c6c 5f74 6173 6b65 725f 6974 656d 73da  ll_tasker_items.
+00000820: 0d74 6865 5f74 6173 6b5f 6e61 6d65 5a0c  .the_task_nameZ.
+00000830: 756e 6b6e 6f77 6e5f 7461 736b da0d 7370  unknown_task..sp
+00000840: 6563 6966 6963 5f74 6173 6bda 0c70 726f  ecific_task..pro
+00000850: 6a65 6374 5f6e 616d 655a 0b74 6865 5f70  ject_nameZ.the_p
+00000860: 726f 6a65 6374 da0c 7461 736b 5f65 6c65  roject..task_ele
+00000870: 6d65 6e74 da09 7461 736b 5f6e 616d 65da  ment..task_name.
+00000880: 0974 6173 6b5f 6c69 7374 7217 0000 0072  .task_listr....r
+00000890: 1700 0000 7218 0000 00da 2170 726f 6365  ....r.....!proce
+000008a0: 7373 5f73 6f6c 6f5f 7461 736b 5f77 6974  ss_solo_task_wit
+000008b0: 685f 6e6f 5f70 726f 6669 6c65 6500 0000  h_no_profilee...
+000008c0: 737a 0000 0004 0d08 0104 030a 0108 ff04  sz..............
+000008d0: 050e 0108 ff08 030e 0110 020a 0106 0104  ................
+000008e0: 0208 0104 0304 010a 0104 ff04 0302 0102  ................
+000008f0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000900: 0102 fb04 fb04 0d0a 0104 ff04 030c 0208  ................
+00000910: 0102 0110 0106 ff10 0504 030c 0106 0204  ................
+00000920: 0302 0102 0102 0102 0102 0102 0102 0102  ................
+00000930: 0102 0102 0102 0102 0102 0104 f30a 0f72  ...............r
+00000940: 3300 0000 da10 666f 756e 645f 7461 736b  3.....found_task
+00000950: 735f 6c69 7374 722b 0000 0072 2c00 0000  s_listr+...r,...
+00000960: 6308 0000 0000 0000 0000 0000 000d 0000  c...............
+00000970: 000d 0000 0043 0000 0073 fa00 0000 6401  .....C...s....d.
+00000980: 7d08 6402 7d09 6403 7d0a 7c07 6404 1900  }.d.}.d.}.|.d...
+00000990: 4400 5d21 7d0b 7c04 6405 1900 7212 0100  D.]!}.|.d...r...
+000009a0: 6e1a 7c0b 7c02 7601 722b 7400 7c00 7c0b  n.|.|.v.r+t.|.|.
+000009b0: 7c02 7c03 7c04 7c08 7c0a 7c01 7c05 7c06  |.|.|.|.|.|.|.|.
+000009c0: 7c07 830b 5c03 7d0a 7d0c 7d08 7c0c 722b  |...\.}.}.}.|.r+
+000009d0: 0100 6e01 710a 7c08 6401 6b04 7265 7c03  ..n.q.|.d.k.re|.
+000009e0: 6406 1900 6401 6b04 723f 7401 a002 7c06  d...d.k.r?t...|.
+000009f0: 7c03 7c00 6401 6402 a105 0100 7401 a002  |.|.d.d.....t...
+00000a00: 7c06 7c03 7c00 6407 6402 a105 0100 7c04  |.|.|.d.d.....|.
+00000a10: 6405 1900 7365 7c03 6406 1900 6401 6b03  d...se|.d...d.k.
+00000a20: 7265 7401 a002 7c06 7c03 7c00 6401 7403  ret...|.|.|.d.t.
+00000a30: 7c06 6408 6402 6409 7c08 9b00 640a 9d03  |.d.d.d.|...d...
+00000a40: 640b 8305 a105 0100 7c09 640b 7500 7272  d.......|.d.u.rr
+00000a50: 7401 a002 7c06 7c03 7c00 6407 6402 a105  t...|.|.|.d.d...
+00000a60: 0100 7401 a002 7c06 7c03 7c00 6407 6402  ..t...|.|.|.d.d.
+00000a70: a105 0100 6400 5300 290c 4e72 0100 0000  ....d.S.).Nr....
+00000a80: 7211 0000 0046 721c 0000 0072 0f00 0000  r....Fr....r....
+00000a90: 7220 0000 0072 2100 0000 da12 756e 6b6e  r ...r!.....unkn
+00000aa0: 6f77 6e5f 7461 736b 5f63 6f6c 6f72 7a15  own_task_colorz.
+00000ab0: 5468 6572 6520 6172 6520 6120 746f 7461  There are a tota
+00000ac0: 6c20 6f66 207a 2d20 756e 6e61 6d65 6420  l of z- unnamed 
+00000ad0: 5461 736b 7320 6e6f 7420 6173 736f 6369  Tasks not associ
+00000ae0: 6174 6564 2077 6974 6820 6120 5072 6f66  ated with a Prof
+00000af0: 696c 6521 5429 0472 3300 0000 7214 0000  ile!T).r3...r...
+00000b00: 0072 1500 0000 7204 0000 0029 0d72 0800  .r....r....).r..
+00000b10: 0000 7209 0000 0072 3400 0000 720d 0000  ..r....r4...r...
+00000b20: 0072 0b00 0000 722b 0000 0072 0c00 0000  .r....r+...r....
+00000b30: 722c 0000 0072 2a00 0000 7231 0000 0072  r,...r*...r1...r
+00000b40: 1a00 0000 7228 0000 0072 2e00 0000 7217  ....r(...r....r.
+00000b50: 0000 0072 1700 0000 7218 0000 00da 2370  ...r....r.....#p
+00000b60: 726f 6365 7373 5f74 6173 6b73 5f6e 6f74  rocess_tasks_not
+00000b70: 5f63 616c 6c65 645f 6279 5f70 726f 6669  _called_by_profi
+00000b80: 6c65 c400 0000 7370 0000 0004 0a04 0104  le....sp........
+00000b90: 010c 0302 0102 0104 ff04 0308 0602 0202  ................
+00000ba0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000bb0: 0102 0102 0102 f508 ff04 0f04 0102 8008  ................
+00000bc0: 030c 0112 0104 010a 0104 ff06 0502 ff0c  ................
+00000bd0: 0204 0202 0102 0102 0102 0102 0102 0102  ................
+00000be0: 0102 010a 0202 0302 f804 fb08 1104 010a  ................
+00000bf0: 0104 ff04 040a 0104 ff04 0372 3600 0000  ...........r6...
+00000c00: 2915 da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
+00000c10: 0300 0000 da15 6d61 7074 6173 6b65 722e  ......maptasker.
+00000c20: 7372 632e 6f75 7470 7574 6cda 0373 7263  src.outputl..src
+00000c30: da07 6f75 7470 7574 6c72 1400 0000 da13  ..outputlr......
+00000c40: 6d61 7074 6173 6b65 722e 7372 632e 7461  maptasker.src.ta
+00000c50: 736b 7372 2300 0000 da16 6d61 7074 6173  sksr#.....maptas
+00000c60: 6b65 722e 7372 632e 6672 6d74 6874 6d6c  ker.src.frmthtml
+00000c70: 7204 0000 00da 166d 6170 7461 736b 6572  r......maptasker
+00000c80: 2e73 7263 2e73 7973 636f 6e73 7472 0500  .src.sysconstr..
+00000c90: 0000 7206 0000 0072 0700 0000 da03 7374  ..r....r......st
+00000ca0: 72da 0464 6963 7472 1900 0000 da04 626f  r..dictr......bo
+00000cb0: 6f6c 7233 0000 0072 3600 0000 7217 0000  olr3...r6...r...
+00000cc0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000cd0: da08 3c6d 6f64 756c 653e 0100 0000 7358  ..<module>....sX
+00000ce0: 0000 0010 0d12 0212 010c 010c 010c 010c  ................
+00000cf0: 0102 0606 0102 ff0e 0202 fe06 0302 fd02  ................
+00000d00: 0402 fc02 0502 fb02 0602 fa02 070a f902  ................
+00000d10: 4a02 070a f902 5f06 0102 ff02 0202 fe06  J....._.........
+00000d20: 0302 fd02 0402 fc02 0502 fb02 0602 fa02  ................
+00000d30: 0702 f902 0802 f802 090e f7              ...........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/userintr.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/userintr.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 23 17:42:41 2023 UTC, .py size: 28690 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,831 +1,887 @@
-00000000: 6f0d 0d0a 0000 0000 918f 1c64 1270 0000  o..........d.p..
+00000000: 6f0d 0d0a 0000 0000 c420 3464 8977 0000  o........ 4d.w..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6500 a007 6405  d.l.m.Z...e...d.
-00000060: a101 0100 6500 a008 6406 a101 0100 6407  ....e...d.....d.
-00000070: 5a09 4700 6408 6409 8400 6409 6500 6a0a  Z.G.d.d...d.e.j.
-00000080: 8303 5a0b 6401 5300 290a e900 0000 004e  ..Z.d.S.)......N
-00000090: 2901 da08 4173 6b43 6f6c 6f72 2901 da11  )...AskColor)...
-000000a0: 7361 7665 5f72 6573 746f 7265 5f61 7267  save_restore_arg
-000000b0: 7329 01da 1454 5950 4553 5f4f 465f 434f  s)...TYPES_OF_CO
-000000c0: 4c4f 525f 4e41 4d45 53da 0653 7973 7465  LOR_NAMES..Syste
-000000d0: 6d5a 0462 6c75 6561 6706 0000 4d61 7054  mZ.blueag...MapT
-000000e0: 6173 6b65 7220 6469 7370 6c61 7973 2079  asker displays y
-000000f0: 6f75 7220 416e 6472 6f69 6420 5461 736b  our Android Task
-00000100: 6572 2063 6f6e 6669 6775 7261 7469 6f6e  er configuration
-00000110: 2062 6173 6564 206f 6e20 796f 7572 2075   based on your u
-00000120: 706c 6f61 6465 6420 5461 736b 6572 2062  ploaded Tasker b
-00000130: 6163 6b75 7020 6669 6c65 2028 652e 672e  ackup file (e.g.
-00000140: 2022 6261 636b 7570 2e78 6d6c 2229 2e20   "backup.xml"). 
-00000150: 2054 6865 2064 6973 706c 6179 2077 696c   The display wil
-00000160: 6c20 6f70 7469 6f6e 616c 6c79 2069 6e63  l optionally inc
-00000170: 6c75 6465 2061 6c6c 2050 726f 6a65 6374  lude all Project
-00000180: 732c 2050 726f 6669 6c65 732c 2054 6173  s, Profiles, Tas
-00000190: 6b73 2061 6e64 2074 6865 6972 2061 6374  ks and their act
-000001a0: 696f 6e73 2c20 5072 6f66 696c 652f 5461  ions, Profile/Ta
-000001b0: 736b 2063 6f6e 6469 7469 6f6e 7320 616e  sk conditions an
-000001c0: 6420 6f74 6865 7220 5072 6f66 696c 652f  d other Profile/
-000001d0: 5461 736b 2072 656c 6174 6564 2069 6e66  Task related inf
-000001e0: 6f72 6d61 7469 6f6e 2e0a 0a2a 2044 6973  ormation...* Dis
-000001f0: 706c 6179 206f 7074 696f 6e73 2061 7265  play options are
-00000200: 3a0a 2020 2020 4c65 7665 6c20 303a 2064  :.    Level 0: d
-00000210: 6973 706c 6179 2066 6972 7374 2054 6173  isplay first Tas
-00000220: 6b20 6163 7469 6f6e 206f 6e6c 792c 2066  k action only, f
-00000230: 6f72 2075 6e6e 616d 6564 2054 6173 6b73  or unnamed Tasks
-00000240: 206f 6e6c 7920 2873 696c 656e 7429 0a20   only (silent). 
-00000250: 2020 204c 6576 656c 2031 203d 2064 6973     Level 1 = dis
-00000260: 706c 6179 2061 6c6c 2054 6173 6b20 6163  play all Task ac
-00000270: 7469 6f6e 2064 6574 6169 6c73 2066 6f72  tion details for
-00000280: 2075 6e6b 6e6f 776e 2054 6173 6b73 206f   unknown Tasks o
-00000290: 6e6c 7920 2864 6566 6175 6c74 290a 2020  nly (default).  
-000002a0: 2020 4c65 7665 6c20 3220 3d20 6469 7370    Level 2 = disp
-000002b0: 6c61 7920 6675 6c6c 2054 6173 6b20 6163  lay full Task ac
-000002c0: 7469 6f6e 206e 616d 6520 6f6e 2065 7665  tion name on eve
-000002d0: 7279 2054 6173 6b0a 2020 2020 4c65 7665  ry Task.    Leve
-000002e0: 6c20 3320 3d20 6469 7370 6c61 7920 6675  l 3 = display fu
-000002f0: 6c6c 2054 6173 6b20 6163 7469 6f6e 2064  ll Task action d
-00000300: 6574 6169 6c73 206f 6e20 6576 6572 7920  etails on every 
-00000310: 5461 736b 2077 6974 6820 6163 7469 6f6e  Task with action
-00000320: 2064 6574 6169 6c73 0a0a 2a20 4469 7370   details..* Disp
-00000330: 6c61 7920 436f 6e64 6974 696f 6e73 3a20  lay Conditions: 
-00000340: 5475 726e 206f 6e20 7468 6520 6469 7370  Turn on the disp
-00000350: 6c61 7920 6f66 2050 726f 6669 6c65 2061  lay of Profile a
-00000360: 6e64 2054 6173 6b20 636f 6e64 6974 696f  nd Task conditio
-00000370: 6e73 2e0a 0a2a 2044 6973 706c 6179 2054  ns...* Display T
-00000380: 6173 6b65 724e 6574 2049 6e66 6f20 2d20  askerNet Info - 
-00000390: 4966 2061 7661 696c 6162 6c65 2c20 6469  If available, di
-000003a0: 7370 6c61 7920 5461 736b 6572 4e65 7420  splay TaskerNet 
-000003b0: 7075 626c 6973 6869 6e67 2069 6e66 6f72  publishing infor
-000003c0: 6d61 7469 6f6e 0a0a 2a20 4469 7370 6c61  mation..* Displa
-000003d0: 7920 5461 736b 6572 2050 7265 6665 7265  y Tasker Prefere
-000003e0: 6e63 6573 202d 2064 6973 706c 6179 2054  nces - display T
-000003f0: 6173 6b65 7227 7320 7379 7374 656d 2050  asker's system P
-00000400: 7265 6665 7265 6e63 6573 0a0a 2a20 5361  references..* Sa
-00000410: 7665 2053 6574 7469 6e67 7320 2d20 5361  ve Settings - Sa
-00000420: 7665 2074 6865 7365 2073 6574 7469 6e67  ve these setting
-00000430: 7320 666f 7220 6c61 7465 7220 7573 652e  s for later use.
-00000440: 0a0a 2a20 5265 7374 6f72 6520 5365 7474  ..* Restore Sett
-00000450: 696e 6773 202d 2052 6573 746f 7265 2074  ings - Restore t
-00000460: 6865 2073 6574 7469 6e67 7320 6672 6f6d  he settings from
-00000470: 2061 2070 7265 7669 6f75 736c 7920 7361   a previously sa
-00000480: 7665 6420 7365 7373 696f 6e2e 0a0a 2a20  ved session...* 
-00000490: 4170 7065 6172 616e 6365 204d 6f64 653a  Appearance Mode:
-000004a0: 2044 6172 6b2c 204c 6967 6874 2c20 6f72   Dark, Light, or
-000004b0: 2053 7973 7465 6d20 6465 6661 756c 742e   System default.
-000004c0: 0a0a 2a20 5265 7365 7420 4f70 7469 6f6e  ..* Reset Option
-000004d0: 733a 2043 6c65 6172 2065 7665 7279 7468  s: Clear everyth
-000004e0: 696e 6720 616e 6420 7374 6172 7420 616e  ing and start an
-000004f0: 6577 2e0a 0a2a 2052 756e 3a20 5275 6e20  ew...* Run: Run 
-00000500: 7468 6520 7072 6f67 7261 6d20 7769 7468  the program with
-00000510: 2074 6865 2073 6574 7469 6e67 7320 7072   the settings pr
-00000520: 6f76 6964 6564 2e0a 0a2a 2053 7065 6369  ovided...* Speci
-00000530: 6669 6320 4e61 6d65 2074 6162 3a20 656e  fic Name tab: en
-00000540: 7465 7220 6120 7369 6e67 6c65 2c20 7370  ter a single, sp
-00000550: 6563 6966 6963 206e 616d 6564 2069 7465  ecific named ite
-00000560: 6d20 746f 2064 6973 706c 6179 2e2e 2e0a  m to display....
-00000570: 2020 202d 2050 726f 6a65 6374 204e 616d     - Project Nam
-00000580: 653a 2065 6e74 6572 2061 2073 7065 6369  e: enter a speci
-00000590: 6669 6320 5072 6f6a 6563 7420 746f 2064  fic Project to d
-000005a0: 6973 706c 6179 0a20 2020 2d20 5072 6f66  isplay.   - Prof
-000005b0: 696c 6520 4e61 6d65 3a20 656e 7465 7220  ile Name: enter 
-000005c0: 6120 7370 6563 6966 6963 2050 726f 6669  a specific Profi
-000005d0: 6c65 2074 6f20 6469 7370 6c61 790a 2020  le to display.  
-000005e0: 202d 2054 6173 6b20 4e61 6d65 3a20 656e   - Task Name: en
-000005f0: 7465 7220 6120 7370 6563 6966 6963 2054  ter a specific T
-00000600: 6173 6b20 746f 2064 6973 706c 6179 0a20  ask to display. 
-00000610: 2020 2854 6865 7365 2074 6872 6565 2061    (These three a
-00000620: 7265 2065 7863 6c75 7369 7665 3a20 656e  re exclusive: en
-00000630: 7465 7220 6f6e 6520 6f6e 6c79 290a 0a2a  ter one only)..*
-00000640: 2043 6f6c 6f72 7320 7461 623a 2073 656c   Colors tab: sel
-00000650: 6563 7420 636f 6c6f 7273 2066 6f72 2076  ect colors for v
-00000660: 6172 696f 7573 2065 6c65 6d65 6e74 7320  arious elements 
-00000670: 6f66 2074 6865 2064 6973 706c 6179 0a20  of the display. 
-00000680: 2020 2020 2020 2020 2020 2020 2028 652e               (e.
-00000690: 672e 2063 6f6c 6f72 2066 6f72 2050 726f  g. color for Pro
-000006a0: 6a65 6374 732c 2050 726f 6669 6c65 732c  jects, Profiles,
-000006b0: 2054 6173 6b73 2c20 6574 632e 290a 0a2a   Tasks, etc.)..*
-000006c0: 2045 7869 743a 2045 7869 7420 7468 6520   Exit: Exit the 
-000006d0: 7072 6f67 7261 6d20 2871 7569 7429 2e0a  program (quit)..
-000006e0: 0a4e 6f74 653a 2059 6f75 2077 696c 6c20  .Note: You will 
-000006f0: 6265 2070 726f 6d70 7465 6420 746f 2069  be prompted to i
-00000700: 6465 6e74 6966 7920 796f 7572 2054 6173  dentify your Tas
-00000710: 6b65 7220 6261 636b 7570 2066 696c 6520  ker backup file 
-00000720: 6f6e 6365 0a20 2020 2020 2079 6f75 2068  once.      you h
-00000730: 6974 2074 6865 2027 5275 6e27 2062 7574  it the 'Run' but
-00000740: 746f 6e63 0000 0000 0000 0000 0000 0000  tonc............
-00000750: 0000 0000 0300 0000 0000 0000 73d4 0000  ............s...
-00000760: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
-00000770: 0284 085a 0364 0365 0466 0264 0464 0584  ...Z.d.e.f.d.d..
-00000780: 045a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
-00000790: 005a 0764 0a64 0b84 005a 0864 0c64 0d84  .Z.d.d...Z.d.d..
-000007a0: 005a 0964 0e64 0f84 005a 0a64 1064 1184  .Z.d.d...Z.d.d..
-000007b0: 005a 0b64 1265 0c66 0264 1364 1484 045a  .Z.d.e.f.d.d...Z
-000007c0: 0d64 1565 0c66 0264 1664 1784 045a 0e64  .d.e.f.d.d...Z.d
-000007d0: 1865 0c66 0264 1964 1a84 045a 0f64 1b64  .e.f.d.d...Z.d.d
-000007e0: 1c84 005a 1064 1d64 1e84 005a 1164 1f64  ...Z.d.d...Z.d.d
-000007f0: 2084 005a 1264 2164 2284 005a 1364 2364   ..Z.d!d"..Z.d#d
-00000800: 2484 005a 1464 2564 2684 005a 1564 2764  $..Z.d%d&..Z.d'd
-00000810: 2884 005a 1664 2964 2a84 005a 1764 2b64  (..Z.d)d*..Z.d+d
-00000820: 2c84 005a 1864 2d64 2e84 005a 1987 0004  ,..Z.d-d...Z....
-00000830: 005a 1a53 0029 2fda 054d 7947 7569 6301  .Z.S.)/..MyGuic.
-00000840: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-00000850: 0000 0003 0000 0073 0205 0000 7400 8300  .......s....t...
-00000860: a001 a100 0100 7c00 a002 6401 a101 0100  ......|...d.....
-00000870: 7c00 a003 6402 a101 0100 7c00 6a04 6403  |...d.....|.j.d.
-00000880: 6403 6404 8d02 0100 7c00 6a04 6405 6406  d.d.....|.j.d.d.
-00000890: 6404 8d02 0100 7c00 6a05 6406 6403 6404  d.....|.j.d.d.d.
-000008a0: 8d02 0100 7406 6a07 7c00 6407 6406 6408  ....t.j.|.d.d.d.
-000008b0: 8d03 7c00 5f08 7c00 6a08 6a09 6406 6406  ..|._.|.j.j.d.d.
-000008c0: 6409 640a 640b 8d04 0100 7c00 6a08 6a05  d.d.d.....|.j.j.
-000008d0: 640c 6403 6404 8d02 0100 7406 6a0a 7c00  d.d.d.....t.j.|.
-000008e0: 6a08 640d 7406 6a0b 640e 640f 6410 8d02  j.d.t.j.d.d.d...
-000008f0: 6411 8d03 7c00 5f0c 7c00 6a0c 6a09 6406  d...|._.|.j.j.d.
-00000900: 6406 640e 6412 6413 8d04 0100 7406 6a0a  d.d.d.d.....t.j.
-00000910: 7c00 6a08 6414 6415 6416 8d03 7c00 5f0d  |.j.d.d.d...|._.
-00000920: 7c00 6a0d 6a09 6403 6406 640e 6417 6413  |.j.j.d.d.d.d.d.
-00000930: 8d04 0100 7406 6a0e 7c00 6a08 6700 6418  ....t.j.|.j.g.d.
-00000940: a201 7c00 6a0f 6419 8d03 7c00 5f10 7c00  ..|.j.d...|._.|.
-00000950: 6a10 6a09 641a 6406 640e 6417 6413 8d04  j.j.d.d.d.d.d...
-00000960: 0100 7406 6a11 7c00 6a08 7c00 6a12 641b  ..t.j.|.j.|.j.d.
-00000970: 641c 641d 641e 8d05 7c00 5f13 7c00 6a13  d.d.d...|._.|.j.
-00000980: 6a09 641f 6406 640e 6420 6415 6421 8d05  j.d.d.d.d d.d!..
-00000990: 0100 7406 6a11 7c00 6a08 7c00 6a14 6422  ..t.j.|.j.|.j.d"
-000009a0: 641c 641d 641e 8d05 7c00 5f15 7c00 6a15  d.d.d...|._.|.j.
-000009b0: 6a09 6423 6406 640e 6420 6415 6421 8d05  j.d#d.d.d d.d!..
-000009c0: 0100 7406 6a11 7c00 6a08 7c00 6a16 6424  ..t.j.|.j.|.j.d$
-000009d0: 641c 641d 641e 8d05 7c00 5f17 7c00 6a17  d.d.d...|._.|.j.
-000009e0: 6a09 6425 6406 640e 6420 6415 6421 8d05  j.d%d.d.d d.d!..
-000009f0: 0100 7406 6a18 7c00 6a08 6426 641a 6427  ..t.j.|.j.d&d.d'
-00000a00: 7c00 6a19 6428 8d05 7c00 5f1a 7c00 6a1a  |.j.d(..|._.|.j.
-00000a10: 6a09 6409 6406 6420 640e 6429 6421 8d05  j.d.d.d d.d)d!..
-00000a20: 0100 7406 6a18 7c00 6a08 6426 641a 642a  ..t.j.|.j.d&d.d*
-00000a30: 7c00 6a1b 6428 8d05 7c00 5f1c 7c00 6a1c  |.j.d(..|._.|.j.
-00000a40: 6a09 642b 6406 6420 6406 642c 6421 8d05  j.d+d.d d.d,d!..
-00000a50: 0100 7406 6a0a 7c00 6a08 642d 6415 6416  ..t.j.|.j.d-d.d.
-00000a60: 8d03 7c00 5f1d 7c00 6a1d 6a09 642e 6406  ..|._.|.j.j.d.d.
-00000a70: 640e 6420 6413 8d04 0100 7406 6a0e 7c00  d.d d.....t.j.|.
-00000a80: 6a08 6700 642f a201 7c00 6a1e 6419 8d03  j.g.d/..|.j.d...
-00000a90: 7c00 5f1f 7c00 6a1f 6a09 640c 6406 6406  |._.|.j.j.d.d.d.
-00000aa0: 642c 6430 8d04 0100 7406 6a18 7c00 6431  d,d0....t.j.|.d1
-00000ab0: 641a 6432 7c00 6a20 6433 8d05 7c00 5f21  d.d2|.j d3..|._!
-00000ac0: 7c00 6a21 6a09 6409 6406 6434 6434 640a  |.j!j.d.d.d4d4d.
-00000ad0: 6421 8d05 0100 7406 6a18 7c00 6431 641a  d!....t.j.|.d1d.
-00000ae0: 6435 7c00 6a22 6436 6437 8d06 7c00 5f23  d5|.j"d6d7..|._#
-00000af0: 7c00 6a23 6a09 642b 6406 6434 6434 640a  |.j#j.d+d.d4d4d.
-00000b00: 6421 8d05 0100 7406 6a18 7c00 6431 641a  d!....t.j.|.d1d.
-00000b10: 6438 7c00 6a24 6439 6437 8d06 7c00 5f25  d8|.j$d9d7..|._%
-00000b20: 7c00 6a25 6a09 642b 641a 6434 6434 6413  |.j%j.d+d.d4d4d.
-00000b30: 8d04 0100 7406 6a26 7c00 643a 643b 643c  ....t.j&|.d:d;d<
-00000b40: 8d03 7c00 5f27 7c00 6a27 6a28 6426 643d  ..|._'|.j'j(d&d=
-00000b50: 8d01 0100 7c00 6a27 6a09 6406 6403 643e  ....|.j'j.d.d.d>
-00000b60: 643e 640a 6421 8d05 0100 7406 6a29 7c00  d>d.d!....t.j)|.
-00000b70: 643b 6426 643f 8d03 7c00 5f2a 7c00 6a2a  d;d&d?..|._*|.j*
-00000b80: 6a09 6406 641a 643e 643e 640a 6421 8d05  j.d.d.d>d>d.d!..
-00000b90: 0100 7c00 6a2a a02b 6440 a101 0100 7c00  ..|.j*.+d@....|.
-00000ba0: 6a2a a02b 6441 a101 0100 7c00 6a2a a02b  j*.+dA....|.j*.+
-00000bb0: 6442 a101 0100 7c00 6a2a a02c 6440 a101  dB....|.j*.,d@..
-00000bc0: 6a04 6406 6403 6404 8d02 0100 7c00 6a2a  j.d.d.d.....|.j*
-00000bd0: a02c 6441 a101 6a04 6406 6403 6404 8d02  .,dA..j.d.d.d...
-00000be0: 0100 7406 6a2d 7c00 6a2a a02c 6440 a101  ..t.j-|.j*.,d@..
-00000bf0: 6443 7c00 6a2e 6426 6444 6445 8d05 7c00  dC|.j.d&dDdE..|.
-00000c00: 5f2f 7c00 6a2f 6a09 6403 6406 640e 6446  _/|.j/j.d.d.d.dF
-00000c10: 640a 6421 8d05 0100 7406 6a2d 7c00 6a2a  d.d!....t.j-|.j*
-00000c20: a02c 6440 a101 6447 7c00 6a30 6426 6444  .,d@..dG|.j0d&dD
-00000c30: 6445 8d05 7c00 5f31 7c00 6a31 6a09 641a  dE..|._1|.j1j.d.
-00000c40: 6406 640e 6446 640a 6421 8d05 0100 7406  d.d.dFd.d!....t.
-00000c50: 6a2d 7c00 6a2a a02c 6440 a101 6448 7c00  j-|.j*.,d@..dH|.
-00000c60: 6a32 6426 6444 6445 8d05 7c00 5f33 7c00  j2d&dDdE..|._3|.
-00000c70: 6a33 6a09 641f 6406 640e 6446 640a 6421  j3j.d.d.d.dFd.d!
-00000c80: 8d05 0100 7406 6a0a 7c00 6a2a a02c 6440  ....t.j.|.j*.,d@
-00000c90: a101 6449 6415 6416 8d03 7c00 5f34 7c00  ..dId.d...|._4|.
-00000ca0: 6a34 6a09 6423 6406 640e 6446 6413 8d04  j4j.d#d.d.dFd...
-00000cb0: 0100 7406 6a0a 7c00 6a2a a02c 6441 a101  ..t.j.|.j*.,dA..
-00000cc0: 644a 644b 8d02 7c00 5f35 7c00 6a35 6a09  dJdK..|._5|.j5j.
-00000cd0: 6406 6406 6406 6406 6413 8d04 0100 7406  d.d.d.d.d.....t.
-00000ce0: 6a0e 7c00 6a2a a02c 6441 a101 6700 644c  j.|.j*.,dA..g.dL
-00000cf0: a201 7c00 6a36 6419 8d03 7c00 5f37 7c00  ..|.j6d...|._7|.
-00000d00: 6a37 6a09 6403 6406 640e 6446 6413 8d04  j7j.d.d.d.dFd...
-00000d10: 0100 7406 6a11 7c00 6a2a a02c 6442 a101  ..t.j.|.j*.,dB..
-00000d20: 644d 7c00 6a38 641c 641d 644e 8d05 7c00  dM|.j8d.d.dN..|.
-00000d30: 5f39 7c00 6a27 6a28 6426 644f 8d01 0100  _9|.j'j(d&dO....
-00000d40: 7c00 6a39 6a3a 640e 6420 6450 8d02 0100  |.j9j:d.d dP....
-00000d50: 7c00 a03b 641c a101 0100 6400 5300 2951  |..;d.....d.S.)Q
-00000d60: 4e7a 194d 6170 5461 736b 6572 2052 756e  Nz.MapTasker Run
-00000d70: 7469 6d65 204f 7074 696f 6e73 5a08 3131  time OptionsZ.11
-00000d80: 3030 7836 3030 e901 0000 0029 01da 0677  00x600.....)...w
-00000d90: 6569 6768 7429 02e9 0200 0000 e903 0000  eight)..........
-00000da0: 0072 0100 0000 e98c 0000 0029 02da 0577  .r.........)...w
-00000db0: 6964 7468 5a0d 636f 726e 6572 5f72 6164  idthZ.corner_rad
-00000dc0: 6975 73e9 0600 0000 da04 6e73 6577 2904  ius.......nsew).
-00000dd0: da03 726f 77da 0663 6f6c 756d 6e5a 0772  ..row..columnZ.r
-00000de0: 6f77 7370 616e da06 7374 6963 6b79 e909  owspan..sticky..
-00000df0: 0000 00da 094d 6170 5461 736b 6572 e914  .....MapTasker..
-00000e00: 0000 005a 0462 6f6c 6429 02da 0473 697a  ...Z.bold)...siz
-00000e10: 6572 0800 0000 2902 da04 7465 7874 da04  er....)...text..
-00000e20: 666f 6e74 2902 7214 0000 00e9 0a00 0000  font).r.........
-00000e30: a904 720f 0000 0072 1000 0000 da04 7061  ..r....r......pa
-00000e40: 6478 da04 7061 6479 7a15 4469 7370 6c61  dx..padyz.Displa
-00000e50: 7920 4465 7461 696c 204c 6576 656c 3ada  y Detail Level:.
-00000e60: 0177 2902 7216 0000 00da 0661 6e63 686f  .w).r......ancho
-00000e70: 7229 0272 1800 0000 7201 0000 00a9 04da  r).r....r.......
-00000e80: 0130 da01 31da 0132 da01 3329 02da 0676  .0..1..2..3)...v
-00000e90: 616c 7565 73da 0763 6f6d 6d61 6e64 7209  alues..commandr.
-00000ea0: 0000 007a 1244 6973 706c 6179 2043 6f6e  ...z.Display Con
-00000eb0: 6469 7469 6f6e 7354 4629 0472 2400 0000  ditionsTF).r$...
-00000ec0: 7216 0000 00da 076f 6e76 616c 7565 da08  r......onvalue..
-00000ed0: 6f66 6676 616c 7565 720a 0000 0072 1800  offvaluer....r..
-00000ee0: 0000 2905 720f 0000 0072 1000 0000 721a  ..).r....r....r.
-00000ef0: 0000 0072 1b00 0000 7211 0000 007a 1644  ...r....r....z.D
-00000f00: 6973 706c 6179 2054 6173 6b65 724e 6574  isplay TaskerNet
-00000f10: 2049 6e66 6fe9 0400 0000 7a1a 4469 7370   Info.....z.Disp
-00000f20: 6c61 7920 5461 736b 6572 2050 7265 6665  lay Tasker Prefe
-00000f30: 7265 6e63 6573 e905 0000 007a 0723 3635  rences.....z.#65
-00000f40: 3633 6666 7a0d 5361 7665 2053 6574 7469  63ffz.Save Setti
-00000f50: 6e67 7329 04da 0c62 6f72 6465 725f 636f  ngs)...border_co
-00000f60: 6c6f 72da 0c62 6f72 6465 725f 7769 6474  lor..border_widt
-00000f70: 6872 1600 0000 7224 0000 00da 0173 7a10  hr....r$.....sz.
-00000f80: 5265 7374 6f72 6520 5365 7474 696e 6773  Restore Settings
-00000f90: e907 0000 00da 016e 7a14 4755 4920 4170  .......nz.GUI Ap
-00000fa0: 7065 6172 616e 6365 204d 6f64 653a e908  pearance Mode:..
-00000fb0: 0000 0029 03da 054c 6967 6874 da04 4461  ...)...Light..Da
-00000fc0: 726b 7205 0000 0029 0472 0f00 0000 7210  rkr....).r....r.
-00000fd0: 0000 0072 1a00 0000 7211 0000 007a 0723  ...r....r....z.#
-00000fe0: 3234 3646 4236 7a0d 5265 7365 7420 4f70  246FB6z.Reset Op
-00000ff0: 7469 6f6e 7329 05da 066d 6173 7465 72da  tions)...master.
-00001000: 0866 675f 636f 6c6f 7272 2a00 0000 7216  .fg_colorr*...r.
-00001010: 0000 0072 2400 0000 2902 7214 0000 0072  ...r$...).r....r
-00001020: 1400 0000 5a03 5275 6e29 027a 0723 3042  ....Z.Run).z.#0B
-00001030: 4630 3735 7a07 2331 4144 3633 4429 0672  F075z.#1AD63D).r
-00001040: 3100 0000 7232 0000 0072 2a00 0000 7216  1...r2...r*...r.
-00001050: 0000 0072 2400 0000 da0a 7465 7874 5f63  ...r$.....text_c
-00001060: 6f6c 6f72 da04 4578 6974 da03 5265 64e9  olor..Exit..Red.
-00001070: 6400 0000 e9fa 0000 0029 02da 0668 6569  d........)...hei
-00001080: 6768 7472 0c00 0000 2901 5a16 7363 726f  ghtr....).Z.scro
-00001090: 6c6c 6261 725f 6275 7474 6f6e 5f63 6f6c  llbar_button_col
-000010a0: 6f72 2902 7214 0000 0072 0100 0000 2902  or).r....r....).
-000010b0: 720c 0000 005a 1973 6567 6d65 6e74 6564  r....Z.segmented
-000010c0: 5f62 7574 746f 6e5f 6667 5f63 6f6c 6f72  _button_fg_color
-000010d0: 7a0d 5370 6563 6966 6963 204e 616d 65da  z.Specific Name.
-000010e0: 0643 6f6c 6f72 735a 0544 6562 7567 7a0c  .ColorsZ.Debugz.
-000010f0: 5072 6f6a 6563 7420 4e61 6d65 7a07 2331  Project Namez.#1
-00001100: 6263 3966 6629 0472 1600 0000 7224 0000  bc9ff).r....r$..
-00001110: 0072 3200 0000 7229 0000 0029 0272 1800  .r2...r)...).r..
-00001120: 0000 7218 0000 007a 0c50 726f 6669 6c65  ..r....z.Profile
-00001130: 204e 616d 657a 0954 6173 6b20 4e61 6d65   Namez.Task Name
-00001140: 7a0f 2850 6963 6b20 4f4e 4c59 204f 6e65  z.(Pick ONLY One
-00001150: 297a 1f53 6574 2056 6172 696f 7573 2044  )z.Set Various D
-00001160: 6973 706c 6179 2043 6f6c 6f72 7320 4865  isplay Colors He
-00001170: 7265 a901 7216 0000 0029 0fda 0850 726f  re..r....)...Pro
-00001180: 6a65 6374 73da 0850 726f 6669 6c65 737a  jects..Profilesz
-00001190: 1144 6973 6162 6c65 6420 5072 6f66 696c  .Disabled Profil
-000011a0: 6573 7a0d 4c61 756e 6368 6572 2054 6173  esz.Launcher Tas
-000011b0: 6b7a 1250 726f 6669 6c65 2043 6f6e 6469  kz.Profile Condi
-000011c0: 7469 6f6e 73da 0554 6173 6b73 7a0e 2854  tions..Tasksz.(T
-000011d0: 6173 6b29 2041 6374 696f 6e73 7a11 4163  ask) Actionsz.Ac
-000011e0: 7469 6f6e 2043 6f6e 6469 7469 6f6e 737a  tion Conditionsz
-000011f0: 0d41 6374 696f 6e20 4c61 6265 6c73 7a0c  .Action Labelsz.
-00001200: 4163 7469 6f6e 204e 616d 6573 da06 5363  Action Names..Sc
-00001210: 656e 6573 da0a 4261 636b 6772 6f75 6e64  enes..Background
-00001220: da07 4275 6c6c 6574 737a 1554 6173 6b65  ..Bulletsz.Taske
-00001230: 724e 6574 2049 6e66 6f72 6d61 7469 6f6e  rNet Information
-00001240: 7a12 5461 736b 6572 2050 7265 6665 7265  z.Tasker Prefere
-00001250: 6e63 6573 7a0a 4465 6275 6720 4d6f 6465  ncesz.Debug Mode
-00001260: 2904 7216 0000 0072 2400 0000 7225 0000  ).r....r$...r%..
-00001270: 0072 2600 0000 2901 7229 0000 0029 0272  .r&...).r)...).r
-00001280: 1a00 0000 721b 0000 0029 3cda 0573 7570  ....r....)<..sup
-00001290: 6572 da08 5f5f 696e 6974 5f5f da05 7469  er..__init__..ti
-000012a0: 746c 65da 0867 656f 6d65 7472 79da 1467  tle..geometry..g
-000012b0: 7269 645f 636f 6c75 6d6e 636f 6e66 6967  rid_columnconfig
-000012c0: 7572 65da 1167 7269 645f 726f 7763 6f6e  ure..grid_rowcon
-000012d0: 6669 6775 7265 da0d 6375 7374 6f6d 746b  figure..customtk
-000012e0: 696e 7465 725a 0843 546b 4672 616d 655a  interZ.CTkFrameZ
-000012f0: 0d73 6964 6562 6172 5f66 7261 6d65 da04  .sidebar_frame..
-00001300: 6772 6964 da08 4354 6b4c 6162 656c 5a07  grid..CTkLabelZ.
-00001310: 4354 6b46 6f6e 745a 0a6c 6f67 6f5f 6c61  CTkFontZ.logo_la
-00001320: 6265 6c5a 0c64 6574 6169 6c5f 6c61 6265  belZ.detail_labe
-00001330: 6c5a 0d43 546b 4f70 7469 6f6e 4d65 6e75  lZ.CTkOptionMenu
-00001340: da15 6465 7461 696c 5f73 656c 6563 7465  ..detail_selecte
-00001350: 645f 6576 656e 74da 1573 6964 6562 6172  d_event..sidebar
-00001360: 5f64 6574 6169 6c5f 6f70 7469 6f6e 5a0b  _detail_optionZ.
-00001370: 4354 6b43 6865 636b 426f 78da 0f63 6f6e  CTkCheckBox..con
-00001380: 6469 7469 6f6e 5f65 7665 6e74 da10 636f  dition_event..co
-00001390: 6e64 6974 696f 6e5f 6275 7474 6f6e da17  ndition_button..
-000013a0: 6469 7370 6c61 795f 7461 736b 6572 6e65  display_taskerne
-000013b0: 745f 6576 656e 74da 1864 6973 706c 6179  t_event..display
-000013c0: 5f74 6173 6b65 726e 6574 5f62 7574 746f  _taskernet_butto
-000013d0: 6eda 1964 6973 706c 6179 5f70 7265 6665  n..display_prefe
-000013e0: 7265 6e63 6573 5f65 7665 6e74 da1a 6469  rences_event..di
-000013f0: 7370 6c61 795f 7072 6566 6572 656e 6365  splay_preference
-00001400: 735f 6275 7474 6f6e 5a09 4354 6b42 7574  s_buttonZ.CTkBut
-00001410: 746f 6eda 1373 6176 655f 7365 7474 696e  ton..save_settin
-00001420: 6773 5f65 7665 6e74 5a14 7361 7665 5f73  gs_eventZ.save_s
-00001430: 6574 7469 6e67 735f 6275 7474 6f6e da16  ettings_button..
-00001440: 7265 7374 6f72 655f 7365 7474 696e 6773  restore_settings
-00001450: 5f65 7665 6e74 5a17 7265 7374 6f72 655f  _eventZ.restore_
-00001460: 7365 7474 696e 6773 5f62 7574 746f 6e5a  settings_buttonZ
-00001470: 1561 7070 6561 7261 6e63 655f 6d6f 6465  .appearance_mode
-00001480: 5f6c 6162 656c da1c 6368 616e 6765 5f61  _label..change_a
-00001490: 7070 6561 7261 6e63 655f 6d6f 6465 5f65  ppearance_mode_e
-000014a0: 7665 6e74 da1b 6170 7065 6172 616e 6365  vent..appearance
-000014b0: 5f6d 6f64 655f 6f70 7469 6f6e 656d 656e  _mode_optionemen
-000014c0: 75da 1472 6573 6574 5f73 6574 7469 6e67  u..reset_setting
-000014d0: 735f 6576 656e 745a 0c72 6573 6574 5f62  s_eventZ.reset_b
-000014e0: 7574 746f 6eda 0b72 756e 5f70 726f 6772  utton..run_progr
-000014f0: 616d 5a0a 7275 6e5f 6275 7474 6f6e da0c  amZ.run_button..
-00001500: 6578 6974 5f70 726f 6772 616d 5a0b 6578  exit_programZ.ex
-00001510: 6974 5f62 7574 746f 6eda 0a43 546b 5465  it_button..CTkTe
-00001520: 7874 626f 78da 0774 6578 7462 6f78 da09  xtbox..textbox..
-00001530: 636f 6e66 6967 7572 655a 0a43 546b 5461  configureZ.CTkTa
-00001540: 6276 6965 77da 0774 6162 7669 6577 da03  bview..tabview..
-00001550: 6164 64da 0374 6162 5a0e 4354 6b52 6164  add..tabZ.CTkRad
-00001560: 696f 4275 7474 6f6e da19 7369 6e67 6c65  ioButton..single
-00001570: 5f70 726f 6a65 6374 5f6e 616d 655f 6576  _project_name_ev
-00001580: 656e 74da 1473 7472 696e 675f 696e 7075  ent..string_inpu
-00001590: 745f 6275 7474 6f6e 31da 1973 696e 676c  t_button1..singl
-000015a0: 655f 7072 6f66 696c 655f 6e61 6d65 5f65  e_profile_name_e
-000015b0: 7665 6e74 da14 7374 7269 6e67 5f69 6e70  vent..string_inp
-000015c0: 7574 5f62 7574 746f 6e32 da16 7369 6e67  ut_button2..sing
-000015d0: 6c65 5f74 6173 6b5f 6e61 6d65 5f65 7665  le_task_name_eve
-000015e0: 6e74 da14 7374 7269 6e67 5f69 6e70 7574  nt..string_input
-000015f0: 5f62 7574 746f 6e33 5a0a 6e61 6d65 5f6c  _button3Z.name_l
-00001600: 6162 656c 5a0b 6c61 6265 6c5f 7461 625f  abelZ.label_tab_
-00001610: 32da 0c63 6f6c 6f72 735f 6576 656e 745a  2..colors_eventZ
-00001620: 1263 6f6c 6f72 735f 6f70 7469 6f6e 656d  .colors_optionem
-00001630: 656e 75da 1464 6562 7567 5f63 6865 636b  enu..debug_check
-00001640: 626f 785f 6576 656e 74da 0e64 6562 7567  box_event..debug
-00001650: 5f63 6865 636b 626f 78da 0470 6163 6bda  _checkbox..pack.
-00001660: 0c73 6574 5f64 6566 6175 6c74 73a9 01da  .set_defaults...
-00001670: 0473 656c 66a9 01da 095f 5f63 6c61 7373  .self....__class
-00001680: 5f5f a900 fa77 2f55 7365 7273 2f6d 696b  __...w/Users/mik
-00001690: 7275 6269 6e2f 4c69 6272 6172 792f 436c  rubin/Library/Cl
-000016a0: 6f75 6453 746f 7261 6765 2f47 6f6f 676c  oudStorage/Googl
-000016b0: 6544 7269 7665 2d6d 696b 7275 6269 6e40  eDrive-mikrubin@
-000016c0: 676d 6169 6c2e 636f 6d2f 4d79 2044 7269  gmail.com/My Dri
-000016d0: 7665 2f50 7974 686f 6e2f 6d61 7074 6173  ve/Python/maptas
-000016e0: 6b65 722f 6d61 7074 6173 6b65 722f 7372  ker/maptasker/sr
-000016f0: 632f 7573 6572 696e 7472 2e70 7972 4200  c/userintr.pyrB.
-00001700: 0000 3c00 0000 7362 0100 000a 010a 030a  ..<...sb........
-00001710: 010e 030e 010e 0112 0314 0110 0204 0104  ................
-00001720: 0102 010c 0108 fd14 0504 0308 0108 ff14  ................
-00001730: 0304 0104 0106 0104 0108 fd14 0504 0304  ................
-00001740: 0104 0102 0102 0102 0108 fb16 0704 0304  ................
-00001750: 0104 0102 0102 0102 0108 fb06 070a 0106  ................
-00001760: ff04 0504 0104 0102 0102 0102 0108 fb06  ................
-00001770: 070a 0106 ff04 0504 0102 0102 0102 0104  ................
-00001780: 0108 fb16 0704 0304 0102 0102 0102 0104  ................
-00001790: 0108 fb16 0704 0308 0108 ff14 0304 0104  ................
-000017a0: 0106 0104 0108 fd14 0504 0302 0102 0102  ................
-000017b0: 0102 0104 0108 fb06 070a 0106 ff04 0502  ................
-000017c0: 0102 0102 0102 0104 0102 0108 fa06 080a  ................
-000017d0: 0106 ff04 0502 0102 0102 0102 0104 0102  ................
-000017e0: 0108 fa14 0812 030e 0116 0104 0306 0108  ................
-000017f0: ff16 030c 010c 010c 010c 0104 0106 ff16  ................
-00001800: 0304 030a 0102 0104 0102 0102 0108 fb06  ................
-00001810: 070a 0106 ff04 050a 0102 0104 0102 0102  ................
-00001820: 0108 fb06 070a 0106 ff04 050a 0102 0104  ................
-00001830: 0102 0102 0108 fb06 070a 0106 ff04 050e  ................
-00001840: 0108 ff14 0304 030c 0108 ff14 0304 010a  ................
-00001850: 0106 0104 1108 ed14 1504 030a 0102 0104  ................
-00001860: 0102 0102 0108 fb0e 0710 010e 037a 0e4d  .............z.M
-00001870: 7947 7569 2e5f 5f69 6e69 745f 5fda 0a66  yGui.__init__..f
-00001880: 6972 7374 5f74 696d 6563 0200 0000 0000  irst_timec......
-00001890: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-000018a0: 0000 73a4 0000 007c 006a 006a 0167 0064  ..s....|.j.j.g.d
-000018b0: 01a2 0164 028d 0101 007c 006a 00a0 0264  ...d.....|.j...d
-000018c0: 03a1 0101 0064 047c 005f 0364 0504 007c  .....d.|._.d...|
-000018d0: 005f 0404 007c 005f 0504 007c 005f 0604  ._...|._...|._..
-000018e0: 007c 005f 0704 007c 005f 0804 007c 005f  .|._...|._...|._
-000018f0: 0904 007c 005f 0a7c 005f 0b64 0604 007c  ...|._.|._.d...|
-00001900: 005f 0c04 007c 005f 0d7c 005f 0e64 077c  ._...|._.|._.d.|
-00001910: 005f 0f7c 006a 10a0 0264 08a1 0101 0067  ._.|.j...d.....g
-00001920: 007c 005f 1164 087c 005f 127c 0172 4d7c  .|._.d.|._.|.rM|
-00001930: 006a 13a0 1464 0964 0a74 1517 00a1 0201  .j...d.d.t......
-00001940: 0069 007c 005f 1664 0053 0029 0b4e 721e  .i.|._.d.S.).Nr.
-00001950: 0000 0029 0172 2300 0000 7220 0000 0072  ...).r#...r ...r
-00001960: 0700 0000 46da 0072 0900 0000 7205 0000  ....F..r....r...
-00001970: 00fa 0330 2e30 7a10 4d61 7054 6173 6b65  ...0.0z.MapTaske
-00001980: 7220 4865 6c70 0a0a 2917 724b 0000 0072  r Help..).rK...r
-00001990: 5b00 0000 da03 7365 74da 1464 6973 706c  [.....set..displ
-000019a0: 6179 5f64 6574 6169 6c5f 6c65 7665 6cda  ay_detail_level.
-000019b0: 1a64 6973 706c 6179 5f70 726f 6669 6c65  .display_profile
-000019c0: 5f63 6f6e 6469 7469 6f6e 73da 1364 6973  _conditions..dis
-000019d0: 706c 6179 5f70 7265 6665 7265 6e63 6573  play_preferences
-000019e0: da11 6469 7370 6c61 795f 7461 736b 6572  ..display_tasker
-000019f0: 6e65 74da 0564 6562 7567 5a0e 636c 6561  net..debugZ.clea
-00001a00: 725f 7365 7474 696e 6773 da05 7265 7365  r_settings..rese
-00001a10: 74da 0465 7869 74da 0a67 6f5f 7072 6f67  t..exit..go_prog
-00001a20: 7261 6dda 1373 696e 676c 655f 7072 6f6a  ram..single_proj
-00001a30: 6563 745f 6e61 6d65 da13 7369 6e67 6c65  ect_name..single
-00001a40: 5f70 726f 6669 6c65 5f6e 616d 65da 1073  _profile_name..s
-00001a50: 696e 676c 655f 7461 736b 5f6e 616d 65da  ingle_task_name.
-00001a60: 0e63 6f6c 6f72 5f74 6578 745f 726f 7772  .color_text_rowr
-00001a70: 5500 0000 da0c 636f 6c6f 725f 6c61 6265  U.....color_labe
-00001a80: 6c73 da0f 6170 7065 6172 616e 6365 5f6d  ls..appearance_m
-00001a90: 6f64 6572 5a00 0000 da06 696e 7365 7274  oderZ.....insert
-00001aa0: da09 494e 464f 5f54 4558 54da 0c63 6f6c  ..INFO_TEXT..col
-00001ab0: 6f72 5f6c 6f6f 6b75 7029 0272 6b00 0000  or_lookup).rk...
-00001ac0: 7270 0000 0072 6e00 0000 726e 0000 0072  rp...rn...rn...r
-00001ad0: 6f00 0000 7269 0000 002f 0100 0073 3000  o...ri.../...s0.
-00001ae0: 0000 1201 0c01 0601 0207 08fa 0401 02ff  ................
-00001af0: 0403 02fd 0405 02fb 0406 02fa 0406 02fa  ................
-00001b00: 0806 1201 0601 0c01 0601 0601 0401 1201  ................
-00001b10: 0a01 7a12 4d79 4775 692e 7365 745f 6465  ..z.MyGui.set_de
-00001b20: 6661 756c 7473 6302 0000 0000 0000 0000  faultsc.........
-00001b30: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00001b40: 5000 0000 7400 6a01 7c00 6401 6402 8d02  P...t.j.|.d.d...
-00001b50: 7c00 5f02 7c00 6a02 6a03 6403 6404 6405  |._.|.j.j.d.d.d.
-00001b60: 6405 6406 8d04 0100 7c00 6a02 a004 6407  d.d.....|.j...d.
-00001b70: 7c01 a102 0100 7c00 6a02 6a05 6408 6409  |.....|.j.j.d.d.
-00001b80: 640a 8d02 0100 7c00 6a02 a006 a100 0100  d.....|.j.......
-00001b90: 6400 5300 290b 4e72 3700 0000 a901 720c  d.S.).Nr7.....r.
-00001ba0: 0000 0072 2700 0000 7209 0000 0072 1400  ...r'...r....r..
-00001bb0: 0000 7219 0000 0072 7200 0000 da08 6469  ..r....rr.....di
-00001bc0: 7361 626c 6564 7235 0000 00a9 02da 0573  sabledr5.......s
-00001bd0: 7461 7465 7233 0000 00a9 0772 4700 0000  tater3.....rG...
-00001be0: 7259 0000 0072 5a00 0000 7248 0000 0072  rY...rZ...rH...r
-00001bf0: 8200 0000 725b 0000 00da 0966 6f63 7573  ....r[.....focus
-00001c00: 5f73 6574 2902 726b 0000 00da 0d65 7272  _set).rk.....err
-00001c10: 6f72 5f6d 6573 7361 6765 726e 0000 0072  or_messagern...r
-00001c20: 6e00 0000 726f 0000 00da 1164 6973 706c  n...ro.....displ
-00001c30: 6179 5f65 7272 6f72 5f62 6f78 4601 0000  ay_error_boxF...
-00001c40: 730e 0000 0010 0114 010e 0106 0104 0106  s...............
-00001c50: ff0e 037a 174d 7947 7569 2e64 6973 706c  ...z.MyGui.displ
-00001c60: 6179 5f65 7272 6f72 5f62 6f78 6303 0000  ay_error_boxc...
-00001c70: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00001c80: 0043 0000 0073 6200 0000 7c02 7204 6401  .C...sb...|.r.d.
-00001c90: 6e01 6402 7d03 7400 6a01 7c00 6403 6404  n.d.}.t.j.|.d.d.
-00001ca0: 8d02 7c00 5f02 7c00 6a02 6a03 6405 6406  ..|._.|.j.j.d.d.
-00001cb0: 6407 6407 6408 8d04 0100 7c00 6a02 a004  d.d.d.....|.j...
-00001cc0: 6409 7c01 9b00 640a 9d02 a102 0100 7c00  d.|...d.......|.
-00001cd0: 6a02 6a05 640b 7c03 640c 8d02 0100 7c00  j.j.d.|.d.....|.
-00001ce0: 6a02 a006 a100 0100 6400 5300 290d 4eda  j.......d.S.).N.
-00001cf0: 0547 7265 656e 7235 0000 0069 5802 0000  .Greenr5...iX...
-00001d00: 7285 0000 0072 2700 0000 7207 0000 0072  r....r'...r....r
-00001d10: 1400 0000 7219 0000 0072 7200 0000 da01  ....r....rr.....
-00001d20: 0a72 8600 0000 7287 0000 0072 8900 0000  .r....r....r....
-00001d30: 2904 726b 0000 00da 076d 6573 7361 6765  ).rk.....message
-00001d40: 5a04 676f 6f64 da05 636f 6c6f 7272 6e00  Z.good..colorrn.
-00001d50: 0000 726e 0000 0072 6f00 0000 da13 6469  ..rn...ro.....di
-00001d60: 7370 6c61 795f 6d65 7373 6167 655f 626f  splay_message_bo
-00001d70: 7852 0100 0073 1000 0000 0c01 1001 1401  xR...s..........
-00001d80: 1401 0601 0401 06ff 0e03 7a19 4d79 4775  ..........z.MyGu
-00001d90: 692e 6469 7370 6c61 795f 6d65 7373 6167  i.display_messag
-00001da0: 655f 626f 7863 0300 0000 0000 0000 0000  e_boxc..........
-00001db0: 0000 0400 0000 0600 0000 4300 0000 738c  ..........C...s.
-00001dc0: 0000 0064 017d 037c 0173 0d64 027c 0217  ...d.}.|.s.d.|..
-00001dd0: 0064 0317 007d 0364 047c 005f 007c 006a  .d...}.d.|._.|.j
-00001de0: 0172 167c 006a 0272 1664 057d 036e 117c  .r.|.j.r.d.}.n.|
-00001df0: 006a 0172 1f7c 006a 0372 1f64 067d 036e  .j.r.|.j.r.d.}.n
-00001e00: 087c 006a 0272 277c 006a 0372 2764 077d  .|.j.r'|.j.r'd.}
-00001e10: 037c 0372 387c 00a0 047c 03a1 0101 0064  .|.r8|...|.....d
-00001e20: 085c 037c 005f 017c 005f 027c 005f 0364  .\.|._.|._.|._.d
-00001e30: 0053 007c 00a0 0564 097c 019b 0064 0a7c  .S.|...d.|...d.|
-00001e40: 029b 009d 0464 0ba1 0201 0064 0053 0029  .....d.....d.S.)
-00001e50: 0c4e 7271 0000 007a 2145 7272 6f72 3a0a  .Nrq...z!Error:.
-00001e60: 0a54 6865 206e 616d 6520 656e 7465 7265  .The name entere
-00001e70: 6420 666f 7220 7468 6520 7a16 2069 7320  d for the z. is 
-00001e80: 626c 616e 6b21 0a0a 5472 7920 6167 6169  blank!..Try agai
-00001e90: 6e2e 467a 5b45 7272 6f72 3a0a 0a59 6f75  n.Fz[Error:..You
-00001ea0: 2068 6176 6520 656e 7465 7265 6420 626f   have entered bo
-00001eb0: 7468 2061 2050 726f 6a65 6374 2061 6e64  th a Project and
-00001ec0: 2061 2050 726f 6669 6c65 206e 616d 6521   a Profile name!
-00001ed0: 0a0a 5472 7920 6167 6169 6e20 616e 6420  ..Try again and 
-00001ee0: 6f6e 6c79 2073 656c 6563 7420 6f6e 652e  only select one.
-00001ef0: 7a58 4572 726f 723a 0a0a 596f 7520 6861  zXError:..You ha
-00001f00: 7665 2065 6e74 6572 6564 2062 6f74 6820  ve entered both 
-00001f10: 6120 5072 6f6a 6563 7420 616e 6420 6120  a Project and a 
-00001f20: 5461 736b 206e 616d 6521 0a0a 5472 7920  Task name!..Try 
-00001f30: 6167 6169 6e20 616e 6420 6f6e 6c79 2073  again and only s
-00001f40: 656c 6563 7420 6f6e 652e 7a58 4572 726f  elect one.zXErro
-00001f50: 723a 0a0a 596f 7520 6861 7665 2065 6e74  r:..You have ent
-00001f60: 6572 6564 2062 6f74 6820 6120 5072 6f66  ered both a Prof
-00001f70: 696c 6520 616e 6420 6120 5461 736b 206e  ile and a Task n
-00001f80: 616d 6521 0a0a 5472 7920 6167 6169 6e20  ame!..Try again 
-00001f90: 616e 6420 6f6e 6c79 2073 656c 6563 7420  and only select 
-00001fa0: 6f6e 652e 2903 7271 0000 0072 7100 0000  one.).rq...rq...
-00001fb0: 7271 0000 007a 1244 6973 706c 6179 206f  rq...z.Display o
-00001fc0: 6e6c 7920 7468 6520 277a 0227 2054 2906  nly the 'z.' T).
-00001fd0: 5a0a 6e61 6d65 645f 6974 656d 727c 0000  Z.named_itemr|..
-00001fe0: 0072 7d00 0000 727e 0000 0072 8c00 0000  .r}...r~...r....
-00001ff0: 7291 0000 0029 0472 6b00 0000 da08 7468  r....).rk.....th
-00002000: 655f 6e61 6d65 da0c 656c 656d 656e 745f  e_name..element_
-00002010: 6e61 6d65 728b 0000 0072 6e00 0000 726e  namer....rn...rn
-00002020: 0000 0072 6f00 0000 da0a 6368 6563 6b5f  ...ro.....check_
-00002030: 6e61 6d65 5f01 0000 7338 0000 0004 0104  name_...s8......
-00002040: 0102 0202 0102 ff02 0202 fe02 ff06 050c  ................
-00002050: 0102 0204 ff0c 0402 0204 ff0c 0402 0202  ................
-00002060: ff04 050a 0102 0502 fc04 0104 0108 0104  ................
-00002070: 0310 0108 ff7a 104d 7947 7569 2e63 6865  .....z.MyGui.che
-00002080: 636b 5f6e 616d 6563 0100 0000 0000 0000  ck_namec........
-00002090: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-000020a0: f34c 0000 0064 017d 017c 00a0 007c 01a1  .L...d.}.|...|..
-000020b0: 0101 007c 006a 01a0 02a1 0001 007c 006a  ...|.j.......|.j
-000020c0: 03a0 02a1 0001 0074 046a 0564 0264 0364  .......t.j.d.d.d
-000020d0: 048d 027d 027c 02a0 06a1 007c 005f 077c  ...}.|.....|._.|
-000020e0: 00a0 087c 006a 0764 05a1 0201 0064 0053  ...|.j.d.....d.S
-000020f0: 0029 064e 7271 0000 007a 1345 6e74 6572  .).Nrq...z.Enter
-00002100: 2050 726f 6a65 6374 206e 616d 653a 7a18   Project name:z.
-00002110: 4469 7370 6c61 7920 5370 6563 6966 6963  Display Specific
-00002120: 2050 726f 6a65 6374 a902 7216 0000 0072   Project..r....r
-00002130: 4300 0000 da07 5072 6f6a 6563 7429 0972  C.....Project).r
-00002140: 8c00 0000 7262 0000 00da 0864 6573 656c  ....rb.....desel
-00002150: 6563 7472 6400 0000 7247 0000 00da 0e43  ectrd...rG.....C
-00002160: 546b 496e 7075 7444 6961 6c6f 67da 0967  TkInputDialog..g
-00002170: 6574 5f69 6e70 7574 727c 0000 0072 9400  et_inputr|...r..
-00002180: 0000 a903 726b 0000 0072 8b00 0000 da06  ....rk...r......
-00002190: 6469 616c 6f67 726e 0000 0072 6e00 0000  dialogrn...rn...
-000021a0: 726f 0000 0072 5f00 0000 8701 0000 f312  ro...r_.........
-000021b0: 0000 0004 020a 010a 020a 0104 0204 0106  ................
-000021c0: ff0a 0412 027a 1f4d 7947 7569 2e73 696e  .....z.MyGui.sin
-000021d0: 676c 655f 7072 6f6a 6563 745f 6e61 6d65  gle_project_name
-000021e0: 5f65 7665 6e74 6301 0000 0000 0000 0000  _eventc.........
-000021f0: 0000 0003 0000 0004 0000 0043 0000 0072  ...........C...r
-00002200: 9500 0000 2906 4e72 7100 0000 7a13 456e  ....).Nrq...z.En
-00002210: 7465 7220 5072 6f66 696c 6520 6e61 6d65  ter Profile name
-00002220: 3a7a 1844 6973 706c 6179 2053 7065 6369  :z.Display Speci
-00002230: 6669 6320 5072 6f66 696c 6572 9600 0000  fic Profiler....
-00002240: da07 5072 6f66 696c 6529 0972 8c00 0000  ..Profile).r....
-00002250: 7260 0000 0072 9800 0000 7264 0000 0072  r`...r....rd...r
-00002260: 4700 0000 7299 0000 0072 9a00 0000 727d  G...r....r....r}
-00002270: 0000 0072 9400 0000 729b 0000 0072 6e00  ...r....r....rn.
-00002280: 0000 726e 0000 0072 6f00 0000 7261 0000  ..rn...ro...ra..
-00002290: 009a 0100 0072 9d00 0000 7a1f 4d79 4775  .....r....z.MyGu
-000022a0: 692e 7369 6e67 6c65 5f70 726f 6669 6c65  i.single_profile
-000022b0: 5f6e 616d 655f 6576 656e 7463 0100 0000  _name_eventc....
-000022c0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-000022d0: 4300 0000 7295 0000 0029 064e 7271 0000  C...r....).Nrq..
-000022e0: 007a 1045 6e74 6572 2054 6173 6b20 6e61  .z.Enter Task na
-000022f0: 6d65 3a7a 1544 6973 706c 6179 2053 7065  me:z.Display Spe
-00002300: 6369 6669 6320 5461 736b 7296 0000 00da  cific Taskr.....
-00002310: 0454 6173 6b29 0972 8c00 0000 7260 0000  .Task).r....r`..
-00002320: 0072 9800 0000 7262 0000 0072 4700 0000  .r....rb...rG...
-00002330: 7299 0000 0072 9a00 0000 727e 0000 0072  r....r....r~...r
-00002340: 9400 0000 729b 0000 0072 6e00 0000 726e  ....r....rn...rn
-00002350: 0000 0072 6f00 0000 7263 0000 00ad 0100  ...ro...rc......
-00002360: 0072 9d00 0000 7a1c 4d79 4775 692e 7369  .r....z.MyGui.si
-00002370: 6e67 6c65 5f74 6173 6b5f 6e61 6d65 5f65  ngle_task_name_e
-00002380: 7665 6e74 da13 6e65 775f 6170 7065 6172  vent..new_appear
-00002390: 616e 6365 5f6d 6f64 6563 0200 0000 0000  ance_modec......
-000023a0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000023b0: 0000 7314 0000 0074 00a0 017c 01a1 0101  ..s....t...|....
-000023c0: 007c 017c 005f 0264 0053 00a9 014e 2903  .|.|._.d.S...N).
-000023d0: 7247 0000 00da 1373 6574 5f61 7070 6561  rG.....set_appea
-000023e0: 7261 6e63 655f 6d6f 6465 7281 0000 0029  rance_moder....)
-000023f0: 0272 6b00 0000 72a0 0000 0072 6e00 0000  .rk...r....rn...
-00002400: 726e 0000 0072 6f00 0000 7254 0000 00c0  rn...ro...rT....
-00002410: 0100 0073 0400 0000 0a01 0a01 7a22 4d79  ...s........z"My
-00002420: 4775 692e 6368 616e 6765 5f61 7070 6561  Gui.change_appea
-00002430: 7261 6e63 655f 6d6f 6465 5f65 7665 6e74  rance_mode_event
-00002440: da0e 6469 7370 6c61 795f 6465 7461 696c  ..display_detail
-00002450: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002460: 0002 0000 0043 0000 0073 0a00 0000 7c01  .....C...s....|.
-00002470: 7c00 5f00 6400 5300 72a1 0000 0029 0172  |._.d.S.r....).r
-00002480: 7400 0000 2902 726b 0000 0072 a300 0000  t...).rk...r....
-00002490: 726e 0000 0072 6e00 0000 726f 0000 0072  rn...rn...ro...r
-000024a0: 4a00 0000 c701 0000 7302 0000 000a 017a  J.......s......z
-000024b0: 1b4d 7947 7569 2e64 6574 6169 6c5f 7365  .MyGui.detail_se
-000024c0: 6c65 6374 6564 5f65 7665 6e74 da13 636f  lected_event..co
-000024d0: 6c6f 725f 7365 6c65 6374 6564 5f69 7465  lor_selected_ite
-000024e0: 6d63 0200 0000 0000 0000 0000 0000 0500  mc..............
-000024f0: 0000 0700 0000 4300 0000 7396 0000 0074  ......C...s....t
-00002500: 0083 007d 027c 02a0 01a1 007d 037c 0364  ...}.|.....}.|.d
-00002510: 0075 0172 497c 006a 027d 047c 037c 006a  .u.rI|.j.}.|.|.j
-00002520: 0374 047c 0119 003c 007c 006a 05a0 0674  .t.|...<.|.j...t
-00002530: 076a 087c 006a 09a0 0a64 01a1 017c 019b  .j.|.j...d...|..
-00002540: 0064 029d 027c 0364 038d 03a1 0101 007c  .d...|.d.......|
-00002550: 006a 0564 0419 006a 0b7c 006a 0264 0564  .j.d...j.|.j.d.d
-00002560: 0564 0564 068d 0401 007c 0004 006a 0264  .d.d.....|...j.d
-00002570: 0737 0002 005f 027c 00a0 0c7c 019b 0064  .7..._.|...|...d
-00002580: 087c 039b 009d 0364 09a1 0201 0064 0053  .|.....d.....d.S
-00002590: 0064 0053 0029 0a4e 7239 0000 007a 0920  .d.S.).Nr9...z. 
-000025a0: 3c3c 2063 6f6c 6f72 2902 7216 0000 0072  << color).r....r
-000025b0: 3300 0000 e9ff ffff ff72 0100 0000 7219  3........r....r.
-000025c0: 0000 0072 0700 0000 7a12 2063 6f6c 6f72  ...r....z. color
-000025d0: 2063 6861 6e67 6564 2074 6f20 5429 0d72   changed to T).r
-000025e0: 0200 0000 da03 6765 7472 7f00 0000 7284  ......getr....r.
-000025f0: 0000 0072 0400 0000 7280 0000 00da 0661  ...r....r......a
-00002600: 7070 656e 6472 4700 0000 7249 0000 0072  ppendrG...rI...r
-00002610: 5c00 0000 725e 0000 0072 4800 0000 7291  \...r^...rH...r.
-00002620: 0000 0029 0572 6b00 0000 72a4 0000 005a  ...).rk...r....Z
-00002630: 0a70 6963 6b5f 636f 6c6f 7272 9000 0000  .pick_colorr....
-00002640: 720f 0000 0072 6e00 0000 726e 0000 0072  r....rn...rn...r
-00002650: 6f00 0000 7265 0000 00cd 0100 0073 2a00  o...re.......s*.
-00002660: 0000 0602 0801 0801 0601 0202 0cff 0603  ................
-00002670: 0401 0a01 0801 0201 04fd 04ff 0a07 0a01  ................
-00002680: 06ff 0e03 0401 0e01 08ff 04f0 7a12 4d79  ............z.My
-00002690: 4775 692e 636f 6c6f 7273 5f65 7665 6e74  Gui.colors_event
-000026a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000026b0: 0002 0000 0043 0000 00f3 1000 0000 7c00  .....C........|.
-000026c0: 6a00 a001 a100 7c00 5f02 6400 5300 72a1  j.....|._.d.S.r.
-000026d0: 0000 0029 0372 4d00 0000 72a6 0000 0072  ...).rM...r....r
-000026e0: 7500 0000 726a 0000 0072 6e00 0000 726e  u...rj...rn...rn
-000026f0: 0000 0072 6f00 0000 724c 0000 00e8 0100  ...ro...rL......
-00002700: 00f3 0200 0000 1001 7a15 4d79 4775 692e  ........z.MyGui.
-00002710: 636f 6e64 6974 696f 6e5f 6576 656e 7463  condition_eventc
-00002720: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002730: 0200 0000 4300 0000 72a8 0000 0072 a100  ....C...r....r..
-00002740: 0000 2903 7251 0000 0072 a600 0000 7276  ..).rQ...r....rv
-00002750: 0000 0072 6a00 0000 726e 0000 0072 6e00  ...rj...rn...rn.
-00002760: 0000 726f 0000 0072 5000 0000 ee01 0000  ..ro...rP.......
-00002770: 72a9 0000 007a 1f4d 7947 7569 2e64 6973  r....z.MyGui.dis
-00002780: 706c 6179 5f70 7265 6665 7265 6e63 6573  play_preferences
-00002790: 5f65 7665 6e74 6301 0000 0000 0000 0000  _eventc.........
-000027a0: 0000 0001 0000 0002 0000 0043 0000 0072  ...........C...r
-000027b0: a800 0000 72a1 0000 0029 0372 4f00 0000  ....r....).rO...
-000027c0: 72a6 0000 0072 7700 0000 726a 0000 0072  r....rw...rj...r
-000027d0: 6e00 0000 726e 0000 0072 6f00 0000 724e  n...rn...ro...rN
-000027e0: 0000 00f4 0100 0072 a900 0000 7a1d 4d79  .......r....z.My
-000027f0: 4775 692e 6469 7370 6c61 795f 7461 736b  Gui.display_task
-00002800: 6572 6e65 745f 6576 656e 7463 0100 0000  ernet_eventc....
-00002810: 0000 0000 0000 0000 0200 0000 0900 0000  ................
-00002820: 4300 0000 734a 0000 007c 006a 007c 006a  C...sJ...|.j.|.j
-00002830: 017c 006a 027c 006a 037c 006a 047c 006a  .|.j.|.j.|.j.|.j
-00002840: 057c 006a 067c 006a 0764 019c 087d 0174  .|.j.|.j.d...}.t
-00002850: 0864 027c 006a 097c 0183 035c 027d 017c  .d.|.j.|...\.}.|
-00002860: 005f 097c 00a0 0a64 0364 02a1 0201 0064  ._.|...d.d.....d
-00002870: 0053 0029 044e 2908 7274 0000 0072 7500  .S.).N).rt...ru.
-00002880: 0000 7276 0000 0072 7700 0000 727c 0000  ..rv...rw...r|..
-00002890: 0072 7d00 0000 727e 0000 0072 7800 0000  .r}...r~...rx...
-000028a0: 547a 0f53 6574 7469 6e67 7320 7361 7665  Tz.Settings save
-000028b0: 642e 290b 7274 0000 0072 7500 0000 7276  d.).rt...ru...rv
-000028c0: 0000 0072 7700 0000 727c 0000 0072 7d00  ...rw...r|...r}.
-000028d0: 0000 727e 0000 0072 7800 0000 7203 0000  ..r~...rx...r...
-000028e0: 0072 8400 0000 7291 0000 0029 0272 6b00  .r....r....).rk.
-000028f0: 0000 da09 7465 6d70 5f61 7267 7372 6e00  ....temp_argsrn.
-00002900: 0000 726e 0000 0072 6f00 0000 7252 0000  ..rn...ro...rR..
-00002910: 00fa 0100 0073 1a00 0000 0402 0401 0401  .....s..........
-00002920: 0401 0401 0401 0401 0401 06f8 020a 0801  ................
-00002930: 0aff 1003 7a19 4d79 4775 692e 7361 7665  ....z.MyGui.save
-00002940: 5f73 6574 7469 6e67 735f 6576 656e 7463  _settings_eventc
-00002950: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-00002960: 0400 0000 4300 0000 7344 0100 0064 017d  ....C...sD...d.}
-00002970: 037c 0104 0064 026b 0272 1801 007c 0272  .|...d.k.r...|.r
-00002980: 117c 006a 00a0 01a1 0001 007c 0353 007c  .|.j.......|.S.|
-00002990: 006a 00a0 02a1 0001 007c 0353 0004 0064  .j.......|.S...d
-000029a0: 036b 0272 2701 007c 006a 03a0 0474 057c  .k.r'..|.j...t.|
-000029b0: 0283 01a1 0101 007c 0353 0004 0064 046b  .......|.S...d.k
-000029c0: 0272 3c01 007c 0272 357c 006a 06a0 01a1  .r<..|.r5|.j....
-000029d0: 0001 007c 0353 007c 006a 06a0 02a1 0001  ...|.S.|.j......
-000029e0: 007c 0353 0004 0064 056b 0272 5101 007c  .|.S...d.k.rQ..|
-000029f0: 0272 4a7c 006a 07a0 01a1 0001 007c 0353  .rJ|.j.......|.S
-00002a00: 007c 006a 07a0 02a1 0001 007c 0353 0004  .|.j.......|.S..
-00002a10: 0064 066b 0272 6601 007c 0272 5f7c 006a  .d.k.rf..|.r_|.j
-00002a20: 08a0 01a1 0001 007c 0353 007c 006a 08a0  .......|.S.|.j..
-00002a30: 02a1 0001 007c 0353 0004 0064 076b 0272  .....|.S...d.k.r
-00002a40: 7701 007c 0272 757c 039b 0064 087c 029b  w..|.ru|...d.|..
-00002a50: 0064 099d 047d 037c 0353 0004 0064 0a6b  .d...}.|.S...d.k
-00002a60: 0272 8801 007c 0272 867c 039b 0064 0b7c  .r...|.r.|...d.|
-00002a70: 029b 0064 099d 047d 037c 0353 0064 0c6b  ...d...}.|.S.d.k
-00002a80: 0272 977c 0272 957c 039b 0064 0d7c 029b  .r.|.r.|...d.|..
-00002a90: 0064 099d 047d 037c 0353 0009 007c 00a0  .d...}.|.S...|..
-00002aa0: 0964 0e7c 029b 009d 02a1 0101 007c 0353  .d.|.........|.S
-00002ab0: 0029 0f4e 7271 0000 0072 7800 0000 7274  .).Nrq...rx...rt
-00002ac0: 0000 0072 7500 0000 7276 0000 0072 7700  ...ru...rv...rw.
-00002ad0: 0000 727c 0000 007a 0f50 726f 6a65 6374  ..r|...z.Project
-00002ae0: 2073 6574 2074 6f20 7a02 2e0a 727d 0000   set to z...r}..
-00002af0: 007a 0f50 726f 6669 6c65 2073 6574 2074  .z.Profile set t
-00002b00: 6f20 727e 0000 007a 0c54 6173 6b20 7365  o r~...z.Task se
-00002b10: 7420 746f 207a 1d52 7574 726f 6821 2020  t to z.Rutroh!  
-00002b20: 556e 6465 6669 6e65 6420 6172 6775 6d65  Undefined argume
-00002b30: 6e74 3a20 290a 7267 0000 00da 0673 656c  nt: ).rg.....sel
-00002b40: 6563 7472 9800 0000 724b 0000 0072 7300  ectr....rK...rs.
-00002b50: 0000 da03 7374 7272 4d00 0000 7251 0000  ....strrM...rQ..
-00002b60: 0072 4f00 0000 7291 0000 0029 0472 6b00  .rO...r....).rk.
-00002b70: 0000 da03 6b65 79da 0576 616c 7565 728f  ....key..valuer.
-00002b80: 0000 0072 6e00 0000 726e 0000 0072 6f00  ...rn...rn...ro.
-00002b90: 0000 da0f 7265 7374 6f72 655f 6469 7370  ....restore_disp
-00002ba0: 6c61 790d 0200 0073 5800 0000 0401 0201  lay....sX.......
-00002bb0: 0a01 0401 0a01 041f 0ae3 041d 0ae4 1001  ................
-00002bc0: 041b 0ae6 0401 0a01 0418 0aea 0416 0aeb  ................
-00002bd0: 0401 0a01 0413 0aef 0411 0af0 0401 0a01  ................
-00002be0: 040e 0af4 040c 0af5 0401 1001 0409 0af8  ................
-00002bf0: 0401 1001 0406 06fb 0401 1001 0403 02fe  ................
-00002c00: 1001 0401 7a15 4d79 4775 692e 7265 7374  ....z.MyGui.rest
-00002c10: 6f72 655f 6469 7370 6c61 7963 0100 0000  ore_displayc....
-00002c20: 0000 0000 0000 0000 0700 0000 0700 0000  ................
-00002c30: 4300 0000 73e0 0000 007c 00a0 0064 01a1  C...s....|...d..
-00002c40: 0101 0069 007d 0174 0164 017c 006a 027c  ...i.}.t.d.|.j.|
-00002c50: 0183 035c 027d 017c 005f 027c 0173 167c  ...\.}.|._.|.s.|
-00002c60: 006a 0272 6864 025c 027d 027d 037c 01a0  .j.rhd.\.}.}.|..
-00002c70: 03a1 0044 005d 1a5c 027d 047d 057c 0464  ...D.].\.}.}.|.d
-00002c80: 0075 0172 3874 047c 007c 047c 0583 0301  .u.r8t.|.|.|....
-00002c90: 007c 00a0 057c 047c 05a1 0204 007d 0372  .|...|.|.....}.r
-00002ca0: 387c 027c 0317 007d 0271 1e64 0364 0484  8|.|...}.q.d.d..
-00002cb0: 0074 06a0 03a1 0044 0083 017d 067c 006a  .t.....D...}.|.j
-00002cc0: 02a0 03a1 0044 005d 155c 027d 047d 057c  .....D.].\.}.}.|
-00002cd0: 0464 0075 0172 5c7c 029b 0064 057c 067c  .d.u.r\|...d.|.|
-00002ce0: 0419 009b 0064 067c 059b 0064 079d 067d  .....d.|...d...}
-00002cf0: 0271 477c 00a0 077c 029b 0064 089d 0264  .qG|...|...d...d
-00002d00: 09a1 0201 0064 0053 007c 00a0 0764 0a64  .....d.S.|...d.d
-00002d10: 01a1 0201 0064 0053 0029 0b4e 4629 0272  .....d.S.).NF).r
-00002d20: 7100 0000 7271 0000 0063 0100 0000 0000  q...rq...c......
-00002d30: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
-00002d40: 0000 7316 0000 0069 007c 005d 075c 027d  ..s....i.|.].\.}
-00002d50: 017d 027c 027c 0193 0271 0253 0072 6e00  .}.|.|...q.S.rn.
-00002d60: 0000 726e 0000 0029 03da 022e 30da 016b  ..rn...)....0..k
-00002d70: da01 7672 6e00 0000 726e 0000 0072 6f00  ..vrn...rn...ro.
-00002d80: 0000 da0a 3c64 6963 7463 6f6d 703e 4602  ....<dictcomp>F.
-00002d90: 0000 7302 0000 0016 007a 304d 7947 7569  ..s......z0MyGui
-00002da0: 2e72 6573 746f 7265 5f73 6574 7469 6e67  .restore_setting
-00002db0: 735f 6576 656e 742e 3c6c 6f63 616c 733e  s_event.<locals>
-00002dc0: 2e3c 6469 6374 636f 6d70 3efa 0120 7a0e  .<dictcomp>.. z.
-00002dd0: 2063 6f6c 6f72 2073 6574 2074 6f20 728e   color set to r.
-00002de0: 0000 007a 130a 5365 7474 696e 6773 2072  ...z..Settings r
-00002df0: 6573 746f 7265 642e 547a 174e 6f20 7365  estored.Tz.No se
-00002e00: 7474 696e 6773 2066 696c 6520 666f 756e  ttings file foun
-00002e10: 642e 2908 7269 0000 0072 0300 0000 7284  d.).ri...r....r.
-00002e20: 0000 00da 0569 7465 6d73 da07 7365 7461  .....items..seta
-00002e30: 7474 7272 af00 0000 7204 0000 0072 9100  ttrr....r....r..
-00002e40: 0000 2907 726b 0000 0072 aa00 0000 5a0c  ..).rk...r....Z.
-00002e50: 616c 6c5f 6d65 7373 6167 6573 5a0b 6e65  all_messagesZ.ne
-00002e60: 775f 6d65 7373 6167 6572 ad00 0000 72ae  w_messager....r.
-00002e70: 0000 005a 0f69 6e76 5f63 6f6c 6f72 5f6e  ...Z.inv_color_n
-00002e80: 616d 6573 726e 0000 0072 6e00 0000 726f  amesrn...rn...ro
-00002e90: 0000 0072 5300 0000 3602 0000 732a 0000  ...rS...6...s*..
-00002ea0: 000a 0104 0102 0208 010a ff0a 0408 0110  ................
-00002eb0: 0108 010c 0110 0108 0102 8012 0212 0108  ................
-00002ec0: 0118 0202 ff02 8016 0410 037a 1c4d 7947  ...........z.MyG
-00002ed0: 7569 2e72 6573 746f 7265 5f73 6574 7469  ui.restore_setti
-00002ee0: 6e67 735f 6576 656e 7463 0100 0000 0000  ngs_eventc......
-00002ef0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00002f00: 0000 738c 0000 007c 006a 00a0 0164 01a1  ..s....|.j...d..
-00002f10: 0101 007c 006a 02a0 03a1 0001 007c 006a  ...|.j.......|.j
-00002f20: 04a0 03a1 0001 007c 006a 05a0 03a1 0001  .......|.j......
-00002f30: 007c 006a 06a0 0164 02a1 0101 0074 07a0  .|.j...d.....t..
-00002f40: 0864 02a1 0101 007c 006a 09a0 03a1 0001  .d.....|.j......
-00002f50: 007c 00a0 0a64 0364 04a1 0201 007c 00a0  .|...d.d.....|..
-00002f60: 0b64 05a1 0101 007c 006a 0c72 3f7c 006a  .d.....|.j.r?|.j
-00002f70: 0c44 005d 087d 017c 016a 0d64 0564 068d  .D.].}.|.j.d.d..
-00002f80: 0101 0071 367c 00a0 0e64 07a1 0101 0064  ...q6|...d.....d
-00002f90: 0053 0029 084e 7220 0000 0072 0500 0000  .S.).Nr ...r....
-00002fa0: 7a0f 5365 7474 696e 6773 2072 6573 6574  z.Settings reset
-00002fb0: 2e54 7271 0000 0072 3a00 0000 4629 0f72  .Trq...r:...F).r
-00002fc0: 4b00 0000 7273 0000 0072 4d00 0000 7298  K...rs...rM...r.
-00002fd0: 0000 0072 5100 0000 724f 0000 0072 5500  ...rQ...rO...rU.
-00002fe0: 0000 7247 0000 0072 a200 0000 7267 0000  ..rG...r....rg..
-00002ff0: 0072 9100 0000 728c 0000 0072 8000 0000  .r....r....r....
-00003000: 725b 0000 0072 6900 0000 2902 726b 0000  r[...ri...).rk..
-00003010: 00da 056c 6162 656c 726e 0000 0072 6e00  ...labelrn...rn.
-00003020: 0000 726f 0000 0072 5600 0000 5502 0000  ..ro...rV...U...
-00003030: 731a 0000 000c 010a 010a 010a 010c 010a  s...............
-00003040: 010a 010c 010a 0106 010a 010e 010e 017a  ...............z
-00003050: 1a4d 7947 7569 2e72 6573 6574 5f73 6574  .MyGui.reset_set
-00003060: 7469 6e67 735f 6576 656e 7463 0100 0000  tings_eventc....
-00003070: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00003080: 4300 0000 731c 0000 007c 006a 00a0 01a1  C...s....|.j....
-00003090: 007c 005f 027c 00a0 0364 0164 02a1 0201  .|._.|...d.d....
-000030a0: 0064 0053 0029 034e 7a3e 4465 6275 6720  .d.S.).Nz>Debug 
-000030b0: 6d6f 6465 2072 6571 7569 7265 7320 5461  mode requires Ta
-000030c0: 736b 6572 2062 6163 6b75 7020 6669 6c65  sker backup file
-000030d0: 2074 6f20 6265 206e 616d 6564 3a20 6261   to be named: ba
-000030e0: 636b 7570 2e78 6d6c 5429 0472 6700 0000  ckup.xmlT).rg...
-000030f0: 72a6 0000 0072 7800 0000 7291 0000 0072  r....rx...r....r
-00003100: 6a00 0000 726e 0000 0072 6e00 0000 726f  j...rn...rn...ro
-00003110: 0000 0072 6600 0000 6702 0000 7308 0000  ...rf...g...s...
-00003120: 000c 0104 0104 0108 ff7a 1a4d 7947 7569  .........z.MyGui
-00003130: 2e64 6562 7567 5f63 6865 636b 626f 785f  .debug_checkbox_
-00003140: 6576 656e 7463 0100 0000 0000 0000 0000  eventc..........
-00003150: 0000 0100 0000 0200 0000 4300 0000 f312  ..........C.....
-00003160: 0000 0064 017c 005f 007c 00a0 01a1 0001  ...d.|._.|......
-00003170: 0064 0053 00a9 024e 5429 0272 7b00 0000  .d.S...NT).r{...
-00003180: da04 7175 6974 726a 0000 0072 6e00 0000  ..quitrj...rn...
-00003190: 726e 0000 0072 6f00 0000 7257 0000 0070  rn...ro...rW...p
-000031a0: 0200 00f3 0400 0000 0601 0c01 7a11 4d79  ............z.My
-000031b0: 4775 692e 7275 6e5f 7072 6f67 7261 6d63  Gui.run_programc
-000031c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000031d0: 0200 0000 4300 0000 72b8 0000 0072 b900  ....C...r....r..
-000031e0: 0000 2902 727a 0000 0072 ba00 0000 726a  ..).rz...r....rj
-000031f0: 0000 0072 6e00 0000 726e 0000 0072 6f00  ...rn...rn...ro.
-00003200: 0000 7258 0000 0077 0200 0072 bb00 0000  ..rX...w...r....
-00003210: 7a12 4d79 4775 692e 6578 6974 5f70 726f  z.MyGui.exit_pro
-00003220: 6772 616d 291b da08 5f5f 6e61 6d65 5f5f  gram)...__name__
-00003230: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00003240: 7175 616c 6e61 6d65 5f5f 7242 0000 00da  qualname__rB....
-00003250: 0462 6f6f 6c72 6900 0000 728c 0000 0072  .boolri...r....r
-00003260: 9100 0000 7294 0000 0072 5f00 0000 7261  ....r....r_...ra
-00003270: 0000 0072 6300 0000 72ac 0000 0072 5400  ...rc...r....rT.
-00003280: 0000 724a 0000 0072 6500 0000 724c 0000  ..rJ...re...rL..
-00003290: 0072 5000 0000 724e 0000 0072 5200 0000  .rP...rN...rR...
-000032a0: 72af 0000 0072 5300 0000 7256 0000 0072  r....rS...rV...r
-000032b0: 6600 0000 7257 0000 0072 5800 0000 da0d  f...rW...rX.....
-000032c0: 5f5f 636c 6173 7363 656c 6c5f 5f72 6e00  __classcell__rn.
-000032d0: 0000 726e 0000 0072 6c00 0000 726f 0000  ..rn...rl...ro..
-000032e0: 0072 0600 0000 3b00 0000 732e 0000 0008  .r....;...s.....
-000032f0: 000c 0100 7f0e 7408 1708 0c08 0d08 2808  ......t.......(.
-00003300: 1308 130e 130e 070e 0608 1b08 0608 0608  ................
-00003310: 0608 1308 2908 1f08 1208 0910 0772 0600  ....)........r..
-00003320: 0000 290c 7247 0000 005a 1f43 546b 436f  ..).rG...Z.CTkCo
-00003330: 6c6f 7250 6963 6b65 722e 6374 6b5f 636f  lorPicker.ctk_co
-00003340: 6c6f 725f 7069 636b 6572 7202 0000 00da  lor_pickerr.....
-00003350: 176d 6170 7461 736b 6572 2e73 7263 2e67  .maptasker.src.g
-00003360: 6574 7075 7461 7267 7203 0000 00da 166d  etputargr......m
-00003370: 6170 7461 736b 6572 2e73 7263 2e73 7973  aptasker.src.sys
-00003380: 636f 6e73 7472 0400 0000 72a2 0000 005a  constr....r....Z
-00003390: 1773 6574 5f64 6566 6175 6c74 5f63 6f6c  .set_default_col
-000033a0: 6f72 5f74 6865 6d65 7283 0000 005a 0343  or_themer....Z.C
-000033b0: 546b 7206 0000 0072 6e00 0000 726e 0000  Tkr....rn...rn..
-000033c0: 0072 6e00 0000 726f 0000 00da 083c 6d6f  .rn...ro.....<mo
-000033d0: 6475 6c65 3e01 0000 0073 1200 0000 0812  dule>....s......
-000033e0: 0c02 0c01 0c01 0a03 0a02 0203 02ff 161d  ................
+00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6501  ..d.d.l.m.Z...e.
+00000070: a00a 6406 a101 0100 6501 a00b 6407 a101  ..d.....e...d...
+00000080: 0100 6408 5a0c 4700 6409 640a 8400 640a  ..d.Z.G.d.d...d.
+00000090: 6501 6a0d 8303 5a0e 6401 5300 290b e900  e.j...Z.d.S.)...
+000000a0: 0000 004e 2901 da04 5061 7468 2901 da08  ...N)...Path)...
+000000b0: 4173 6b43 6f6c 6f72 2901 da11 7361 7665  AskColor)...save
+000000c0: 5f72 6573 746f 7265 5f61 7267 7329 01da  _restore_args)..
+000000d0: 1454 5950 4553 5f4f 465f 434f 4c4f 525f  .TYPES_OF_COLOR_
+000000e0: 4e41 4d45 53da 0653 7973 7465 6d5a 0462  NAMES..SystemZ.b
+000000f0: 6c75 6561 6706 0000 4d61 7054 6173 6b65  lueag...MapTaske
+00000100: 7220 6469 7370 6c61 7973 2079 6f75 7220  r displays your 
+00000110: 416e 6472 6f69 6420 5461 736b 6572 2063  Android Tasker c
+00000120: 6f6e 6669 6775 7261 7469 6f6e 2062 6173  onfiguration bas
+00000130: 6564 206f 6e20 796f 7572 2075 706c 6f61  ed on your uploa
+00000140: 6465 6420 5461 736b 6572 2062 6163 6b75  ded Tasker backu
+00000150: 7020 6669 6c65 2028 652e 672e 2022 6261  p file (e.g. "ba
+00000160: 636b 7570 2e78 6d6c 2229 2e20 2054 6865  ckup.xml").  The
+00000170: 2064 6973 706c 6179 2077 696c 6c20 6f70   display will op
+00000180: 7469 6f6e 616c 6c79 2069 6e63 6c75 6465  tionally include
+00000190: 2061 6c6c 2050 726f 6a65 6374 732c 2050   all Projects, P
+000001a0: 726f 6669 6c65 732c 2054 6173 6b73 2061  rofiles, Tasks a
+000001b0: 6e64 2074 6865 6972 2061 6374 696f 6e73  nd their actions
+000001c0: 2c20 5072 6f66 696c 652f 5461 736b 2063  , Profile/Task c
+000001d0: 6f6e 6469 7469 6f6e 7320 616e 6420 6f74  onditions and ot
+000001e0: 6865 7220 5072 6f66 696c 652f 5461 736b  her Profile/Task
+000001f0: 2072 656c 6174 6564 2069 6e66 6f72 6d61   related informa
+00000200: 7469 6f6e 2e0a 0a2a 2044 6973 706c 6179  tion...* Display
+00000210: 206f 7074 696f 6e73 2061 7265 3a0a 2020   options are:.  
+00000220: 2020 4c65 7665 6c20 303a 2064 6973 706c    Level 0: displ
+00000230: 6179 2066 6972 7374 2054 6173 6b20 6163  ay first Task ac
+00000240: 7469 6f6e 206f 6e6c 792c 2066 6f72 2075  tion only, for u
+00000250: 6e6e 616d 6564 2054 6173 6b73 206f 6e6c  nnamed Tasks onl
+00000260: 7920 2873 696c 656e 7429 0a20 2020 204c  y (silent).    L
+00000270: 6576 656c 2031 203d 2064 6973 706c 6179  evel 1 = display
+00000280: 2061 6c6c 2054 6173 6b20 6163 7469 6f6e   all Task action
+00000290: 2064 6574 6169 6c73 2066 6f72 2075 6e6b   details for unk
+000002a0: 6e6f 776e 2054 6173 6b73 206f 6e6c 7920  nown Tasks only 
+000002b0: 2864 6566 6175 6c74 290a 2020 2020 4c65  (default).    Le
+000002c0: 7665 6c20 3220 3d20 6469 7370 6c61 7920  vel 2 = display 
+000002d0: 6675 6c6c 2054 6173 6b20 6163 7469 6f6e  full Task action
+000002e0: 206e 616d 6520 6f6e 2065 7665 7279 2054   name on every T
+000002f0: 6173 6b0a 2020 2020 4c65 7665 6c20 3320  ask.    Level 3 
+00000300: 3d20 6469 7370 6c61 7920 6675 6c6c 2054  = display full T
+00000310: 6173 6b20 6163 7469 6f6e 2064 6574 6169  ask action detai
+00000320: 6c73 206f 6e20 6576 6572 7920 5461 736b  ls on every Task
+00000330: 2077 6974 6820 6163 7469 6f6e 2064 6574   with action det
+00000340: 6169 6c73 0a0a 2a20 4469 7370 6c61 7920  ails..* Display 
+00000350: 436f 6e64 6974 696f 6e73 3a20 5475 726e  Conditions: Turn
+00000360: 206f 6e20 7468 6520 6469 7370 6c61 7920   on the display 
+00000370: 6f66 2050 726f 6669 6c65 2061 6e64 2054  of Profile and T
+00000380: 6173 6b20 636f 6e64 6974 696f 6e73 2e0a  ask conditions..
+00000390: 0a2a 2044 6973 706c 6179 2054 6173 6b65  .* Display Taske
+000003a0: 724e 6574 2049 6e66 6f20 2d20 4966 2061  rNet Info - If a
+000003b0: 7661 696c 6162 6c65 2c20 6469 7370 6c61  vailable, displa
+000003c0: 7920 5461 736b 6572 4e65 7420 7075 626c  y TaskerNet publ
+000003d0: 6973 6869 6e67 2069 6e66 6f72 6d61 7469  ishing informati
+000003e0: 6f6e 0a0a 2a20 4469 7370 6c61 7920 5461  on..* Display Ta
+000003f0: 736b 6572 2050 7265 6665 7265 6e63 6573  sker Preferences
+00000400: 202d 2064 6973 706c 6179 2054 6173 6b65   - display Taske
+00000410: 7227 7320 7379 7374 656d 2050 7265 6665  r's system Prefe
+00000420: 7265 6e63 6573 0a0a 2a20 5361 7665 2053  rences..* Save S
+00000430: 6574 7469 6e67 7320 2d20 5361 7665 2074  ettings - Save t
+00000440: 6865 7365 2073 6574 7469 6e67 7320 666f  hese settings fo
+00000450: 7220 6c61 7465 7220 7573 652e 0a0a 2a20  r later use...* 
+00000460: 5265 7374 6f72 6520 5365 7474 696e 6773  Restore Settings
+00000470: 202d 2052 6573 746f 7265 2074 6865 2073   - Restore the s
+00000480: 6574 7469 6e67 7320 6672 6f6d 2061 2070  ettings from a p
+00000490: 7265 7669 6f75 736c 7920 7361 7665 6420  reviously saved 
+000004a0: 7365 7373 696f 6e2e 0a0a 2a20 4170 7065  session...* Appe
+000004b0: 6172 616e 6365 204d 6f64 653a 2044 6172  arance Mode: Dar
+000004c0: 6b2c 204c 6967 6874 2c20 6f72 2053 7973  k, Light, or Sys
+000004d0: 7465 6d20 6465 6661 756c 742e 0a0a 2a20  tem default...* 
+000004e0: 5265 7365 7420 4f70 7469 6f6e 733a 2043  Reset Options: C
+000004f0: 6c65 6172 2065 7665 7279 7468 696e 6720  lear everything 
+00000500: 616e 6420 7374 6172 7420 616e 6577 2e0a  and start anew..
+00000510: 0a2a 2052 756e 3a20 5275 6e20 7468 6520  .* Run: Run the 
+00000520: 7072 6f67 7261 6d20 7769 7468 2074 6865  program with the
+00000530: 2073 6574 7469 6e67 7320 7072 6f76 6964   settings provid
+00000540: 6564 2e0a 0a2a 2053 7065 6369 6669 6320  ed...* Specific 
+00000550: 4e61 6d65 2074 6162 3a20 656e 7465 7220  Name tab: enter 
+00000560: 6120 7369 6e67 6c65 2c20 7370 6563 6966  a single, specif
+00000570: 6963 206e 616d 6564 2069 7465 6d20 746f  ic named item to
+00000580: 2064 6973 706c 6179 2e2e 2e0a 2020 202d   display....   -
+00000590: 2050 726f 6a65 6374 204e 616d 653a 2065   Project Name: e
+000005a0: 6e74 6572 2061 2073 7065 6369 6669 6320  nter a specific 
+000005b0: 5072 6f6a 6563 7420 746f 2064 6973 706c  Project to displ
+000005c0: 6179 0a20 2020 2d20 5072 6f66 696c 6520  ay.   - Profile 
+000005d0: 4e61 6d65 3a20 656e 7465 7220 6120 7370  Name: enter a sp
+000005e0: 6563 6966 6963 2050 726f 6669 6c65 2074  ecific Profile t
+000005f0: 6f20 6469 7370 6c61 790a 2020 202d 2054  o display.   - T
+00000600: 6173 6b20 4e61 6d65 3a20 656e 7465 7220  ask Name: enter 
+00000610: 6120 7370 6563 6966 6963 2054 6173 6b20  a specific Task 
+00000620: 746f 2064 6973 706c 6179 0a20 2020 2854  to display.   (T
+00000630: 6865 7365 2074 6872 6565 2061 7265 2065  hese three are e
+00000640: 7863 6c75 7369 7665 3a20 656e 7465 7220  xclusive: enter 
+00000650: 6f6e 6520 6f6e 6c79 290a 0a2a 2043 6f6c  one only)..* Col
+00000660: 6f72 7320 7461 623a 2073 656c 6563 7420  ors tab: select 
+00000670: 636f 6c6f 7273 2066 6f72 2076 6172 696f  colors for vario
+00000680: 7573 2065 6c65 6d65 6e74 7320 6f66 2074  us elements of t
+00000690: 6865 2064 6973 706c 6179 0a20 2020 2020  he display.     
+000006a0: 2020 2020 2020 2020 2028 652e 672e 2063           (e.g. c
+000006b0: 6f6c 6f72 2066 6f72 2050 726f 6a65 6374  olor for Project
+000006c0: 732c 2050 726f 6669 6c65 732c 2054 6173  s, Profiles, Tas
+000006d0: 6b73 2c20 6574 632e 290a 0a2a 2045 7869  ks, etc.)..* Exi
+000006e0: 743a 2045 7869 7420 7468 6520 7072 6f67  t: Exit the prog
+000006f0: 7261 6d20 2871 7569 7429 2e0a 0a4e 6f74  ram (quit)...Not
+00000700: 653a 2059 6f75 2077 696c 6c20 6265 2070  e: You will be p
+00000710: 726f 6d70 7465 6420 746f 2069 6465 6e74  rompted to ident
+00000720: 6966 7920 796f 7572 2054 6173 6b65 7220  ify your Tasker 
+00000730: 6261 636b 7570 2066 696c 6520 6f6e 6365  backup file once
+00000740: 0a20 2020 2020 2079 6f75 2068 6974 2074  .      you hit t
+00000750: 6865 2027 5275 6e27 2062 7574 746f 6e63  he 'Run' buttonc
+00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000770: 0300 0000 0000 0000 73dc 0000 0065 005a  ........s....e.Z
+00000780: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00000790: 0364 0365 0466 0264 0464 0584 045a 0564  .d.e.f.d.d...Z.d
+000007a0: 0664 0784 005a 0664 0864 0984 005a 0764  .d...Z.d.d...Z.d
+000007b0: 0a64 0b84 005a 0864 0c64 0d84 005a 0964  .d...Z.d.d...Z.d
+000007c0: 0e64 0f84 005a 0a64 1064 1184 005a 0b64  .d...Z.d.d...Z.d
+000007d0: 1265 0c66 0264 1364 1484 045a 0d64 1565  .e.f.d.d...Z.d.e
+000007e0: 0c66 0264 1664 1784 045a 0e64 1865 0c66  .f.d.d...Z.d.e.f
+000007f0: 0264 1964 1a84 045a 0f64 1b64 1c84 005a  .d.d...Z.d.d...Z
+00000800: 1064 1d64 1e84 005a 1164 1f64 2084 005a  .d.d...Z.d.d ..Z
+00000810: 1264 2164 2284 005a 1364 2364 2484 005a  .d!d"..Z.d#d$..Z
+00000820: 1464 2564 2684 005a 1564 2764 2884 005a  .d%d&..Z.d'd(..Z
+00000830: 1664 2964 2a84 005a 1764 2b64 2c84 005a  .d)d*..Z.d+d,..Z
+00000840: 1864 2d64 2e84 005a 1964 2f64 3084 005a  .d-d...Z.d/d0..Z
+00000850: 1a87 0004 005a 1b53 0029 31da 054d 7947  .....Z.S.)1..MyG
+00000860: 7569 6301 0000 0000 0000 0000 0000 0001  uic.............
+00000870: 0000 0008 0000 0003 0000 0073 0205 0000  ...........s....
+00000880: 7400 8300 a001 a100 0100 7c00 a002 6401  t.........|...d.
+00000890: a101 0100 7c00 a003 6402 a101 0100 7c00  ....|...d.....|.
+000008a0: 6a04 6403 6403 6404 8d02 0100 7c00 6a04  j.d.d.d.....|.j.
+000008b0: 6405 6406 6404 8d02 0100 7c00 6a05 6406  d.d.d.....|.j.d.
+000008c0: 6403 6404 8d02 0100 7406 6a07 7c00 6407  d.d.....t.j.|.d.
+000008d0: 6406 6408 8d03 7c00 5f08 7c00 6a08 6a09  d.d...|._.|.j.j.
+000008e0: 6406 6406 6409 640a 640b 8d04 0100 7c00  d.d.d.d.d.....|.
+000008f0: 6a08 6a05 640c 6403 6404 8d02 0100 7406  j.j.d.d.d.....t.
+00000900: 6a0a 7c00 6a08 640d 7406 6a0b 640e 640f  j.|.j.d.t.j.d.d.
+00000910: 6410 8d02 6411 8d03 7c00 5f0c 7c00 6a0c  d...d...|._.|.j.
+00000920: 6a09 6406 6406 640e 6412 6413 8d04 0100  j.d.d.d.d.d.....
+00000930: 7406 6a0a 7c00 6a08 6414 6415 6416 8d03  t.j.|.j.d.d.d...
+00000940: 7c00 5f0d 7c00 6a0d 6a09 6403 6406 640e  |._.|.j.j.d.d.d.
+00000950: 6417 6413 8d04 0100 7406 6a0e 7c00 6a08  d.d.....t.j.|.j.
+00000960: 6700 6418 a201 7c00 6a0f 6419 8d03 7c00  g.d...|.j.d...|.
+00000970: 5f10 7c00 6a10 6a09 641a 6406 640e 6417  _.|.j.j.d.d.d.d.
+00000980: 6413 8d04 0100 7406 6a11 7c00 6a08 7c00  d.....t.j.|.j.|.
+00000990: 6a12 641b 641c 641d 641e 8d05 7c00 5f13  j.d.d.d.d...|._.
+000009a0: 7c00 6a13 6a09 641f 6406 640e 6420 6415  |.j.j.d.d.d.d d.
+000009b0: 6421 8d05 0100 7406 6a11 7c00 6a08 7c00  d!....t.j.|.j.|.
+000009c0: 6a14 6422 641c 641d 641e 8d05 7c00 5f15  j.d"d.d.d...|._.
+000009d0: 7c00 6a15 6a09 6423 6406 640e 6420 6415  |.j.j.d#d.d.d d.
+000009e0: 6421 8d05 0100 7406 6a11 7c00 6a08 7c00  d!....t.j.|.j.|.
+000009f0: 6a16 6424 641c 641d 641e 8d05 7c00 5f17  j.d$d.d.d...|._.
+00000a00: 7c00 6a17 6a09 6425 6406 640e 6420 6415  |.j.j.d%d.d.d d.
+00000a10: 6421 8d05 0100 7406 6a18 7c00 6a08 6426  d!....t.j.|.j.d&
+00000a20: 641a 6427 7c00 6a19 6428 8d05 7c00 5f1a  d.d'|.j.d(..|._.
+00000a30: 7c00 6a1a 6a09 6409 6406 6420 640e 6429  |.j.j.d.d.d d.d)
+00000a40: 6421 8d05 0100 7406 6a18 7c00 6a08 6426  d!....t.j.|.j.d&
+00000a50: 641a 642a 7c00 6a1b 6428 8d05 7c00 5f1c  d.d*|.j.d(..|._.
+00000a60: 7c00 6a1c 6a09 642b 6406 6420 6406 642c  |.j.j.d+d.d d.d,
+00000a70: 6421 8d05 0100 7406 6a0a 7c00 6a08 642d  d!....t.j.|.j.d-
+00000a80: 6415 6416 8d03 7c00 5f1d 7c00 6a1d 6a09  d.d...|._.|.j.j.
+00000a90: 642e 6406 640e 6420 6413 8d04 0100 7406  d.d.d.d d.....t.
+00000aa0: 6a0e 7c00 6a08 6700 642f a201 7c00 6a1e  j.|.j.g.d/..|.j.
+00000ab0: 6419 8d03 7c00 5f1f 7c00 6a1f 6a09 640c  d...|._.|.j.j.d.
+00000ac0: 6406 6406 642c 6430 8d04 0100 7406 6a18  d.d.d,d0....t.j.
+00000ad0: 7c00 6431 641a 6432 7c00 6a20 6433 8d05  |.d1d.d2|.j d3..
+00000ae0: 7c00 5f21 7c00 6a21 6a09 6409 6406 6434  |._!|.j!j.d.d.d4
+00000af0: 6434 640a 6421 8d05 0100 7406 6a18 7c00  d4d.d!....t.j.|.
+00000b00: 6431 641a 6435 7c00 6a22 6436 6437 8d06  d1d.d5|.j"d6d7..
+00000b10: 7c00 5f23 7c00 6a23 6a09 642b 6406 6434  |._#|.j#j.d+d.d4
+00000b20: 6434 640a 6421 8d05 0100 7406 6a18 7c00  d4d.d!....t.j.|.
+00000b30: 6431 641a 6438 7c00 6a24 6439 6437 8d06  d1d.d8|.j$d9d7..
+00000b40: 7c00 5f25 7c00 6a25 6a09 642b 641a 6434  |._%|.j%j.d+d.d4
+00000b50: 6434 6413 8d04 0100 7406 6a26 7c00 643a  d4d.....t.j&|.d:
+00000b60: 643b 643c 8d03 7c00 5f27 7c00 6a27 6a28  d;d<..|._'|.j'j(
+00000b70: 6426 643d 8d01 0100 7c00 6a27 6a09 6406  d&d=....|.j'j.d.
+00000b80: 6403 643e 643e 640a 6421 8d05 0100 7406  d.d>d>d.d!....t.
+00000b90: 6a29 7c00 643b 6426 643f 8d03 7c00 5f2a  j)|.d;d&d?..|._*
+00000ba0: 7c00 6a2a 6a09 6406 641a 643e 643e 640a  |.j*j.d.d.d>d>d.
+00000bb0: 6421 8d05 0100 7c00 6a2a a02b 6440 a101  d!....|.j*.+d@..
+00000bc0: 0100 7c00 6a2a a02b 6441 a101 0100 7c00  ..|.j*.+dA....|.
+00000bd0: 6a2a a02b 6442 a101 0100 7c00 6a2a a02c  j*.+dB....|.j*.,
+00000be0: 6440 a101 6a04 6406 6403 6404 8d02 0100  d@..j.d.d.d.....
+00000bf0: 7c00 6a2a a02c 6441 a101 6a04 6406 6403  |.j*.,dA..j.d.d.
+00000c00: 6404 8d02 0100 7406 6a2d 7c00 6a2a a02c  d.....t.j-|.j*.,
+00000c10: 6440 a101 6443 7c00 6a2e 6426 6444 6445  d@..dC|.j.d&dDdE
+00000c20: 8d05 7c00 5f2f 7c00 6a2f 6a09 6403 6406  ..|._/|.j/j.d.d.
+00000c30: 640e 6446 640a 6421 8d05 0100 7406 6a2d  d.dFd.d!....t.j-
+00000c40: 7c00 6a2a a02c 6440 a101 6447 7c00 6a30  |.j*.,d@..dG|.j0
+00000c50: 6426 6444 6445 8d05 7c00 5f31 7c00 6a31  d&dDdE..|._1|.j1
+00000c60: 6a09 641a 6406 640e 6446 640a 6421 8d05  j.d.d.d.dFd.d!..
+00000c70: 0100 7406 6a2d 7c00 6a2a a02c 6440 a101  ..t.j-|.j*.,d@..
+00000c80: 6448 7c00 6a32 6426 6444 6445 8d05 7c00  dH|.j2d&dDdE..|.
+00000c90: 5f33 7c00 6a33 6a09 641f 6406 640e 6446  _3|.j3j.d.d.d.dF
+00000ca0: 640a 6421 8d05 0100 7406 6a0a 7c00 6a2a  d.d!....t.j.|.j*
+00000cb0: a02c 6440 a101 6449 6415 6416 8d03 7c00  .,d@..dId.d...|.
+00000cc0: 5f34 7c00 6a34 6a09 6423 6406 640e 6446  _4|.j4j.d#d.d.dF
+00000cd0: 6413 8d04 0100 7406 6a0a 7c00 6a2a a02c  d.....t.j.|.j*.,
+00000ce0: 6441 a101 644a 644b 8d02 7c00 5f35 7c00  dA..dJdK..|._5|.
+00000cf0: 6a35 6a09 6406 6406 6406 6406 6413 8d04  j5j.d.d.d.d.d...
+00000d00: 0100 7406 6a0e 7c00 6a2a a02c 6441 a101  ..t.j.|.j*.,dA..
+00000d10: 6700 644c a201 7c00 6a36 6419 8d03 7c00  g.dL..|.j6d...|.
+00000d20: 5f37 7c00 6a37 6a09 6403 6406 640e 6446  _7|.j7j.d.d.d.dF
+00000d30: 6413 8d04 0100 7406 6a11 7c00 6a2a a02c  d.....t.j.|.j*.,
+00000d40: 6442 a101 644d 7c00 6a38 641c 641d 644e  dB..dM|.j8d.d.dN
+00000d50: 8d05 7c00 5f39 7c00 6a27 6a28 6426 644f  ..|._9|.j'j(d&dO
+00000d60: 8d01 0100 7c00 6a39 6a3a 640e 6420 6450  ....|.j9j:d.d dP
+00000d70: 8d02 0100 7c00 a03b 641c a101 0100 6400  ....|..;d.....d.
+00000d80: 5300 2951 4e7a 194d 6170 5461 736b 6572  S.)QNz.MapTasker
+00000d90: 2052 756e 7469 6d65 204f 7074 696f 6e73   Runtime Options
+00000da0: 5a08 3131 3030 7836 3030 e901 0000 0029  Z.1100x600.....)
+00000db0: 01da 0677 6569 6768 7429 02e9 0200 0000  ...weight)......
+00000dc0: e903 0000 0072 0100 0000 e98c 0000 0029  .....r.........)
+00000dd0: 02da 0577 6964 7468 5a0d 636f 726e 6572  ...widthZ.corner
+00000de0: 5f72 6164 6975 73e9 0600 0000 da04 6e73  _radius.......ns
+00000df0: 6577 2904 da03 726f 77da 0663 6f6c 756d  ew)...row..colum
+00000e00: 6e5a 0772 6f77 7370 616e da06 7374 6963  nZ.rowspan..stic
+00000e10: 6b79 e909 0000 00da 094d 6170 5461 736b  ky.......MapTask
+00000e20: 6572 e914 0000 005a 0462 6f6c 6429 02da  er.....Z.bold)..
+00000e30: 0473 697a 6572 0900 0000 2902 da04 7465  .sizer....)...te
+00000e40: 7874 da04 666f 6e74 2902 7215 0000 00e9  xt..font).r.....
+00000e50: 0a00 0000 a904 7210 0000 0072 1100 0000  ......r....r....
+00000e60: da04 7061 6478 da04 7061 6479 7a15 4469  ..padx..padyz.Di
+00000e70: 7370 6c61 7920 4465 7461 696c 204c 6576  splay Detail Lev
+00000e80: 656c 3ada 0177 2902 7217 0000 00da 0661  el:..w).r......a
+00000e90: 6e63 686f 7229 0272 1900 0000 7201 0000  nchor).r....r...
+00000ea0: 00a9 04da 0130 da01 31da 0132 da01 3329  .....0..1..2..3)
+00000eb0: 02da 0676 616c 7565 73da 0763 6f6d 6d61  ...values..comma
+00000ec0: 6e64 720a 0000 007a 1244 6973 706c 6179  ndr....z.Display
+00000ed0: 2043 6f6e 6469 7469 6f6e 7354 4629 0472   ConditionsTF).r
+00000ee0: 2500 0000 7217 0000 00da 076f 6e76 616c  %...r......onval
+00000ef0: 7565 da08 6f66 6676 616c 7565 720b 0000  ue..offvaluer...
+00000f00: 0072 1900 0000 2905 7210 0000 0072 1100  .r....).r....r..
+00000f10: 0000 721b 0000 0072 1c00 0000 7212 0000  ..r....r....r...
+00000f20: 007a 1644 6973 706c 6179 2054 6173 6b65  .z.Display Taske
+00000f30: 724e 6574 2049 6e66 6fe9 0400 0000 7a1a  rNet Info.....z.
+00000f40: 4469 7370 6c61 7920 5461 736b 6572 2050  Display Tasker P
+00000f50: 7265 6665 7265 6e63 6573 e905 0000 007a  references.....z
+00000f60: 0723 3635 3633 6666 7a0d 5361 7665 2053  .#6563ffz.Save S
+00000f70: 6574 7469 6e67 7329 04da 0c62 6f72 6465  ettings)...borde
+00000f80: 725f 636f 6c6f 72da 0c62 6f72 6465 725f  r_color..border_
+00000f90: 7769 6474 6872 1700 0000 7225 0000 00da  widthr....r%....
+00000fa0: 0173 7a10 5265 7374 6f72 6520 5365 7474  .sz.Restore Sett
+00000fb0: 696e 6773 e907 0000 00da 016e 7a14 4755  ings.......nz.GU
+00000fc0: 4920 4170 7065 6172 616e 6365 204d 6f64  I Appearance Mod
+00000fd0: 653a e908 0000 0029 03da 054c 6967 6874  e:.....)...Light
+00000fe0: da04 4461 726b 7206 0000 0029 0472 1000  ..Darkr....).r..
+00000ff0: 0000 7211 0000 0072 1b00 0000 7212 0000  ..r....r....r...
+00001000: 007a 0723 3234 3646 4236 7a0d 5265 7365  .z.#246FB6z.Rese
+00001010: 7420 4f70 7469 6f6e 7329 05da 066d 6173  t Options)...mas
+00001020: 7465 72da 0866 675f 636f 6c6f 7272 2b00  ter..fg_colorr+.
+00001030: 0000 7217 0000 0072 2500 0000 2902 7215  ..r....r%...).r.
+00001040: 0000 0072 1500 0000 5a03 5275 6e29 027a  ...r....Z.Run).z
+00001050: 0723 3042 4630 3735 7a07 2331 4144 3633  .#0BF075z.#1AD63
+00001060: 4429 0672 3200 0000 7233 0000 0072 2b00  D).r2...r3...r+.
+00001070: 0000 7217 0000 0072 2500 0000 da0a 7465  ..r....r%.....te
+00001080: 7874 5f63 6f6c 6f72 5a04 4578 6974 da03  xt_colorZ.Exit..
+00001090: 5265 64e9 6400 0000 e9fa 0000 0029 02da  Red.d........)..
+000010a0: 0668 6569 6768 7472 0d00 0000 2901 5a16  .heightr....).Z.
+000010b0: 7363 726f 6c6c 6261 725f 6275 7474 6f6e  scrollbar_button
+000010c0: 5f63 6f6c 6f72 2902 7215 0000 0072 0100  _color).r....r..
+000010d0: 0000 2902 720d 0000 005a 1973 6567 6d65  ..).r....Z.segme
+000010e0: 6e74 6564 5f62 7574 746f 6e5f 6667 5f63  nted_button_fg_c
+000010f0: 6f6c 6f72 7a0d 5370 6563 6966 6963 204e  olorz.Specific N
+00001100: 616d 65da 0643 6f6c 6f72 735a 0544 6562  ame..ColorsZ.Deb
+00001110: 7567 7a0c 5072 6f6a 6563 7420 4e61 6d65  ugz.Project Name
+00001120: 7a07 2331 6263 3966 6629 0472 1700 0000  z.#1bc9ff).r....
+00001130: 7225 0000 0072 3300 0000 722a 0000 0029  r%...r3...r*...)
+00001140: 0272 1900 0000 7219 0000 007a 0c50 726f  .r....r....z.Pro
+00001150: 6669 6c65 204e 616d 657a 0954 6173 6b20  file Namez.Task 
+00001160: 4e61 6d65 7a0f 2850 6963 6b20 4f4e 4c59  Namez.(Pick ONLY
+00001170: 204f 6e65 297a 1f53 6574 2056 6172 696f   One)z.Set Vario
+00001180: 7573 2044 6973 706c 6179 2043 6f6c 6f72  us Display Color
+00001190: 7320 4865 7265 a901 7217 0000 0029 0fda  s Here..r....)..
+000011a0: 0850 726f 6a65 6374 73da 0850 726f 6669  .Projects..Profi
+000011b0: 6c65 737a 1144 6973 6162 6c65 6420 5072  lesz.Disabled Pr
+000011c0: 6f66 696c 6573 7a0d 4c61 756e 6368 6572  ofilesz.Launcher
+000011d0: 2054 6173 6bfa 1250 726f 6669 6c65 2043   Task..Profile C
+000011e0: 6f6e 6469 7469 6f6e 73da 0554 6173 6b73  onditions..Tasks
+000011f0: 7a0e 2854 6173 6b29 2041 6374 696f 6e73  z.(Task) Actions
+00001200: fa11 4163 7469 6f6e 2043 6f6e 6469 7469  ..Action Conditi
+00001210: 6f6e 737a 0d41 6374 696f 6e20 4c61 6265  onsz.Action Labe
+00001220: 6c73 7a0c 4163 7469 6f6e 204e 616d 6573  lsz.Action Names
+00001230: da06 5363 656e 6573 da0a 4261 636b 6772  ..Scenes..Backgr
+00001240: 6f75 6e64 da07 4275 6c6c 6574 73fa 1554  ound..Bullets..T
+00001250: 6173 6b65 724e 6574 2049 6e66 6f72 6d61  askerNet Informa
+00001260: 7469 6f6e fa12 5461 736b 6572 2050 7265  tion..Tasker Pre
+00001270: 6665 7265 6e63 6573 7a0a 4465 6275 6720  ferencesz.Debug 
+00001280: 4d6f 6465 2904 7217 0000 0072 2500 0000  Mode).r....r%...
+00001290: 7226 0000 0072 2700 0000 2901 722a 0000  r&...r'...).r*..
+000012a0: 0029 0272 1b00 0000 721c 0000 0029 3cda  .).r....r....)<.
+000012b0: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
+000012c0: da05 7469 746c 65da 0867 656f 6d65 7472  ..title..geometr
+000012d0: 79da 1467 7269 645f 636f 6c75 6d6e 636f  y..grid_columnco
+000012e0: 6e66 6967 7572 65da 1167 7269 645f 726f  nfigure..grid_ro
+000012f0: 7763 6f6e 6669 6775 7265 da0d 6375 7374  wconfigure..cust
+00001300: 6f6d 746b 696e 7465 725a 0843 546b 4672  omtkinterZ.CTkFr
+00001310: 616d 655a 0d73 6964 6562 6172 5f66 7261  ameZ.sidebar_fra
+00001320: 6d65 da04 6772 6964 da08 4354 6b4c 6162  me..grid..CTkLab
+00001330: 656c 5a07 4354 6b46 6f6e 745a 0a6c 6f67  elZ.CTkFontZ.log
+00001340: 6f5f 6c61 6265 6c5a 0c64 6574 6169 6c5f  o_labelZ.detail_
+00001350: 6c61 6265 6c5a 0d43 546b 4f70 7469 6f6e  labelZ.CTkOption
+00001360: 4d65 6e75 da15 6465 7461 696c 5f73 656c  Menu..detail_sel
+00001370: 6563 7465 645f 6576 656e 74da 1573 6964  ected_event..sid
+00001380: 6562 6172 5f64 6574 6169 6c5f 6f70 7469  ebar_detail_opti
+00001390: 6f6e 5a0b 4354 6b43 6865 636b 426f 78da  onZ.CTkCheckBox.
+000013a0: 0f63 6f6e 6469 7469 6f6e 5f65 7665 6e74  .condition_event
+000013b0: da10 636f 6e64 6974 696f 6e5f 6275 7474  ..condition_butt
+000013c0: 6f6e da17 6469 7370 6c61 795f 7461 736b  on..display_task
+000013d0: 6572 6e65 745f 6576 656e 74da 1864 6973  ernet_event..dis
+000013e0: 706c 6179 5f74 6173 6b65 726e 6574 5f62  play_taskernet_b
+000013f0: 7574 746f 6eda 1964 6973 706c 6179 5f70  utton..display_p
+00001400: 7265 6665 7265 6e63 6573 5f65 7665 6e74  references_event
+00001410: da1a 6469 7370 6c61 795f 7072 6566 6572  ..display_prefer
+00001420: 656e 6365 735f 6275 7474 6f6e 5a09 4354  ences_buttonZ.CT
+00001430: 6b42 7574 746f 6eda 1373 6176 655f 7365  kButton..save_se
+00001440: 7474 696e 6773 5f65 7665 6e74 5a14 7361  ttings_eventZ.sa
+00001450: 7665 5f73 6574 7469 6e67 735f 6275 7474  ve_settings_butt
+00001460: 6f6e da16 7265 7374 6f72 655f 7365 7474  on..restore_sett
+00001470: 696e 6773 5f65 7665 6e74 5a17 7265 7374  ings_eventZ.rest
+00001480: 6f72 655f 7365 7474 696e 6773 5f62 7574  ore_settings_but
+00001490: 746f 6e5a 1561 7070 6561 7261 6e63 655f  tonZ.appearance_
+000014a0: 6d6f 6465 5f6c 6162 656c da1c 6368 616e  mode_label..chan
+000014b0: 6765 5f61 7070 6561 7261 6e63 655f 6d6f  ge_appearance_mo
+000014c0: 6465 5f65 7665 6e74 da1b 6170 7065 6172  de_event..appear
+000014d0: 616e 6365 5f6d 6f64 655f 6f70 7469 6f6e  ance_mode_option
+000014e0: 656d 656e 75da 1472 6573 6574 5f73 6574  emenu..reset_set
+000014f0: 7469 6e67 735f 6576 656e 745a 0c72 6573  tings_eventZ.res
+00001500: 6574 5f62 7574 746f 6eda 0b72 756e 5f70  et_button..run_p
+00001510: 726f 6772 616d 5a0a 7275 6e5f 6275 7474  rogramZ.run_butt
+00001520: 6f6e da0c 6578 6974 5f70 726f 6772 616d  on..exit_program
+00001530: 5a0b 6578 6974 5f62 7574 746f 6eda 0a43  Z.exit_button..C
+00001540: 546b 5465 7874 626f 78da 0774 6578 7462  TkTextbox..textb
+00001550: 6f78 da09 636f 6e66 6967 7572 655a 0a43  ox..configureZ.C
+00001560: 546b 5461 6276 6965 77da 0774 6162 7669  TkTabview..tabvi
+00001570: 6577 da03 6164 64da 0374 6162 5a0e 4354  ew..add..tabZ.CT
+00001580: 6b52 6164 696f 4275 7474 6f6e da19 7369  kRadioButton..si
+00001590: 6e67 6c65 5f70 726f 6a65 6374 5f6e 616d  ngle_project_nam
+000015a0: 655f 6576 656e 74da 1473 7472 696e 675f  e_event..string_
+000015b0: 696e 7075 745f 6275 7474 6f6e 31da 1973  input_button1..s
+000015c0: 696e 676c 655f 7072 6f66 696c 655f 6e61  ingle_profile_na
+000015d0: 6d65 5f65 7665 6e74 da14 7374 7269 6e67  me_event..string
+000015e0: 5f69 6e70 7574 5f62 7574 746f 6e32 da16  _input_button2..
+000015f0: 7369 6e67 6c65 5f74 6173 6b5f 6e61 6d65  single_task_name
+00001600: 5f65 7665 6e74 da14 7374 7269 6e67 5f69  _event..string_i
+00001610: 6e70 7574 5f62 7574 746f 6e33 5a0a 6e61  nput_button3Z.na
+00001620: 6d65 5f6c 6162 656c 5a0b 6c61 6265 6c5f  me_labelZ.label_
+00001630: 7461 625f 32da 0c63 6f6c 6f72 735f 6576  tab_2..colors_ev
+00001640: 656e 745a 1263 6f6c 6f72 735f 6f70 7469  entZ.colors_opti
+00001650: 6f6e 656d 656e 75da 1464 6562 7567 5f63  onemenu..debug_c
+00001660: 6865 636b 626f 785f 6576 656e 74da 0e64  heckbox_event..d
+00001670: 6562 7567 5f63 6865 636b 626f 78da 0470  ebug_checkbox..p
+00001680: 6163 6bda 0c73 6574 5f64 6566 6175 6c74  ack..set_default
+00001690: 73a9 01da 0473 656c 66a9 01da 095f 5f63  s....self....__c
+000016a0: 6c61 7373 5f5f a900 fa77 2f55 7365 7273  lass__...w/Users
+000016b0: 2f6d 696b 7275 6269 6e2f 4c69 6272 6172  /mikrubin/Librar
+000016c0: 792f 436c 6f75 6453 746f 7261 6765 2f47  y/CloudStorage/G
+000016d0: 6f6f 676c 6544 7269 7665 2d6d 696b 7275  oogleDrive-mikru
+000016e0: 6269 6e40 676d 6169 6c2e 636f 6d2f 4d79  bin@gmail.com/My
+000016f0: 2044 7269 7665 2f50 7974 686f 6e2f 6d61   Drive/Python/ma
+00001700: 7074 6173 6b65 722f 6d61 7074 6173 6b65  ptasker/maptaske
+00001710: 722f 7372 632f 7573 6572 696e 7472 2e70  r/src/userintr.p
+00001720: 7972 4600 0000 3d00 0000 7362 0100 000a  yrF...=...sb....
+00001730: 010a 030a 010e 030e 010e 0112 0314 0110  ................
+00001740: 0204 0104 0102 010c 0108 fd14 0504 0308  ................
+00001750: 0108 ff14 0304 0104 0106 0104 0108 fd14  ................
+00001760: 0504 0304 0104 0102 0102 0102 0108 fb16  ................
+00001770: 0704 0304 0104 0102 0102 0102 0108 fb06  ................
+00001780: 070a 0106 ff04 0504 0104 0102 0102 0102  ................
+00001790: 0108 fb06 070a 0106 ff04 0504 0102 0102  ................
+000017a0: 0102 0104 0108 fb16 0704 0304 0102 0102  ................
+000017b0: 0102 0104 0108 fb16 0704 0308 0108 ff14  ................
+000017c0: 0304 0104 0106 0104 0108 fd14 0504 0302  ................
+000017d0: 0102 0102 0102 0104 0108 fb06 070a 0106  ................
+000017e0: ff04 0502 0102 0102 0102 0104 0102 0108  ................
+000017f0: fa06 080a 0106 ff04 0502 0102 0102 0102  ................
+00001800: 0104 0102 0108 fa14 0812 030e 0116 0104  ................
+00001810: 0306 0108 ff16 030c 010c 010c 010c 0104  ................
+00001820: 0106 ff16 0304 030a 0102 0104 0102 0102  ................
+00001830: 0108 fb06 070a 0106 ff04 050a 0102 0104  ................
+00001840: 0102 0102 0108 fb06 070a 0106 ff04 050a  ................
+00001850: 0102 0104 0102 0102 0108 fb06 070a 0106  ................
+00001860: ff04 050e 0108 ff14 0304 030c 0108 ff14  ................
+00001870: 0304 010a 0106 0104 1108 ed14 1504 030a  ................
+00001880: 0102 0104 0102 0102 0108 fb0e 0710 010e  ................
+00001890: 037a 0e4d 7947 7569 2e5f 5f69 6e69 745f  .z.MyGui.__init_
+000018a0: 5fda 0a66 6972 7374 5f74 696d 6563 0200  _..first_timec..
+000018b0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+000018c0: 0000 4300 0000 73a4 0000 007c 006a 006a  ..C...s....|.j.j
+000018d0: 0167 0064 01a2 0164 028d 0101 007c 006a  .g.d...d.....|.j
+000018e0: 00a0 0264 03a1 0101 0064 047c 005f 0364  ...d.....d.|._.d
+000018f0: 0504 007c 005f 0404 007c 005f 0504 007c  ...|._...|._...|
+00001900: 005f 0604 007c 005f 0704 007c 005f 0804  ._...|._...|._..
+00001910: 007c 005f 0904 007c 005f 0a7c 005f 0b64  .|._...|._.|._.d
+00001920: 0604 007c 005f 0c04 007c 005f 0d7c 005f  ...|._...|._.|._
+00001930: 0e64 077c 005f 0f7c 006a 10a0 0264 08a1  .d.|._.|.j...d..
+00001940: 0101 0067 007c 005f 1164 087c 005f 127c  ...g.|._.d.|._.|
+00001950: 0172 4d7c 006a 13a0 1464 0964 0a74 1517  .rM|.j...d.d.t..
+00001960: 00a1 0201 0069 007c 005f 1664 0053 0029  .....i.|._.d.S.)
+00001970: 0b4e 721f 0000 0029 0172 2400 0000 7221  .Nr....).r$...r!
+00001980: 0000 0072 0800 0000 46da 0072 0a00 0000  ...r....F..r....
+00001990: 7206 0000 00fa 0330 2e30 7a10 4d61 7054  r......0.0z.MapT
+000019a0: 6173 6b65 7220 4865 6c70 0a0a 2917 724f  asker Help..).rO
+000019b0: 0000 0072 5f00 0000 da03 7365 74da 1464  ...r_.....set..d
+000019c0: 6973 706c 6179 5f64 6574 6169 6c5f 6c65  isplay_detail_le
+000019d0: 7665 6cda 1a64 6973 706c 6179 5f70 726f  vel..display_pro
+000019e0: 6669 6c65 5f63 6f6e 6469 7469 6f6e 73da  file_conditions.
+000019f0: 1364 6973 706c 6179 5f70 7265 6665 7265  .display_prefere
+00001a00: 6e63 6573 da11 6469 7370 6c61 795f 7461  nces..display_ta
+00001a10: 736b 6572 6e65 74da 0564 6562 7567 5a0e  skernet..debugZ.
+00001a20: 636c 6561 725f 7365 7474 696e 6773 da05  clear_settings..
+00001a30: 7265 7365 74da 0465 7869 74da 0a67 6f5f  reset..exit..go_
+00001a40: 7072 6f67 7261 6dda 1373 696e 676c 655f  program..single_
+00001a50: 7072 6f6a 6563 745f 6e61 6d65 da13 7369  project_name..si
+00001a60: 6e67 6c65 5f70 726f 6669 6c65 5f6e 616d  ngle_profile_nam
+00001a70: 65da 1073 696e 676c 655f 7461 736b 5f6e  e..single_task_n
+00001a80: 616d 65da 0e63 6f6c 6f72 5f74 6578 745f  ame..color_text_
+00001a90: 726f 7772 5900 0000 da0c 636f 6c6f 725f  rowrY.....color_
+00001aa0: 6c61 6265 6c73 da0f 6170 7065 6172 616e  labels..appearan
+00001ab0: 6365 5f6d 6f64 6572 5e00 0000 da06 696e  ce_moder^.....in
+00001ac0: 7365 7274 da09 494e 464f 5f54 4558 54da  sert..INFO_TEXT.
+00001ad0: 0c63 6f6c 6f72 5f6c 6f6f 6b75 7029 0272  .color_lookup).r
+00001ae0: 6f00 0000 7274 0000 0072 7200 0000 7272  o...rt...rr...rr
+00001af0: 0000 0072 7300 0000 726d 0000 0030 0100  ...rs...rm...0..
+00001b00: 0073 3000 0000 1201 0c01 0601 0207 08fa  .s0.............
+00001b10: 0401 02ff 0403 02fd 0405 02fb 0406 02fa  ................
+00001b20: 0406 02fa 0806 1201 0601 0c01 0601 0601  ................
+00001b30: 0401 1201 0a01 7a12 4d79 4775 692e 7365  ......z.MyGui.se
+00001b40: 745f 6465 6661 756c 7473 6302 0000 0000  t_defaultsc.....
+00001b50: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
+00001b60: 0000 0073 5000 0000 7400 6a01 7c00 6401  ...sP...t.j.|.d.
+00001b70: 6402 8d02 7c00 5f02 7c00 6a02 6a03 6403  d...|._.|.j.j.d.
+00001b80: 6404 6405 6405 6406 8d04 0100 7c00 6a02  d.d.d.d.....|.j.
+00001b90: a004 6407 7c01 a102 0100 7c00 6a02 6a05  ..d.|.....|.j.j.
+00001ba0: 6408 6409 640a 8d02 0100 7c00 6a02 a006  d.d.d.....|.j...
+00001bb0: a100 0100 6400 5300 290b 4e72 3700 0000  ....d.S.).Nr7...
+00001bc0: a901 720d 0000 0072 2800 0000 720a 0000  ..r....r(...r...
+00001bd0: 0072 1500 0000 721a 0000 0072 7600 0000  .r....r....rv...
+00001be0: da08 6469 7361 626c 6564 7235 0000 00a9  ..disabledr5....
+00001bf0: 02da 0573 7461 7465 7234 0000 00a9 0772  ...stater4.....r
+00001c00: 4b00 0000 725d 0000 0072 5e00 0000 724c  K...r]...r^...rL
+00001c10: 0000 0072 8600 0000 725f 0000 00da 0966  ...r....r_.....f
+00001c20: 6f63 7573 5f73 6574 2902 726f 0000 00da  ocus_set).ro....
+00001c30: 0d65 7272 6f72 5f6d 6573 7361 6765 7272  .error_messagerr
+00001c40: 0000 0072 7200 0000 7273 0000 00da 1164  ...rr...rs.....d
+00001c50: 6973 706c 6179 5f65 7272 6f72 5f62 6f78  isplay_error_box
+00001c60: 4701 0000 730e 0000 0010 0114 010e 0106  G...s...........
+00001c70: 0104 0106 ff0e 037a 174d 7947 7569 2e64  .......z.MyGui.d
+00001c80: 6973 706c 6179 5f65 7272 6f72 5f62 6f78  isplay_error_box
+00001c90: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00001ca0: 0006 0000 0043 0000 0073 6200 0000 7c02  .....C...sb...|.
+00001cb0: 7204 6401 6e01 6402 7d03 7400 6a01 7c00  r.d.n.d.}.t.j.|.
+00001cc0: 6403 6404 8d02 7c00 5f02 7c00 6a02 6a03  d.d...|._.|.j.j.
+00001cd0: 6405 6406 6407 6407 6408 8d04 0100 7c00  d.d.d.d.d.....|.
+00001ce0: 6a02 a004 6409 7c01 9b00 640a 9d02 a102  j...d.|...d.....
+00001cf0: 0100 7c00 6a02 6a05 640b 7c03 640c 8d02  ..|.j.j.d.|.d...
+00001d00: 0100 7c00 6a02 a006 a100 0100 6400 5300  ..|.j.......d.S.
+00001d10: 290d 4eda 0547 7265 656e 7235 0000 0069  ).N..Greenr5...i
+00001d20: 5802 0000 7289 0000 0072 2800 0000 7208  X...r....r(...r.
+00001d30: 0000 0072 1500 0000 721a 0000 0072 7600  ...r....r....rv.
+00001d40: 0000 da01 0a72 8a00 0000 728b 0000 0072  .....r....r....r
+00001d50: 8d00 0000 2904 726f 0000 00da 076d 6573  ....).ro.....mes
+00001d60: 7361 6765 5a04 676f 6f64 da05 636f 6c6f  sageZ.good..colo
+00001d70: 7272 7200 0000 7272 0000 0072 7300 0000  rrr...rr...rs...
+00001d80: da13 6469 7370 6c61 795f 6d65 7373 6167  ..display_messag
+00001d90: 655f 626f 7853 0100 0073 1000 0000 0c01  e_boxS...s......
+00001da0: 1001 1401 1401 0601 0401 06ff 0e03 7a19  ..............z.
+00001db0: 4d79 4775 692e 6469 7370 6c61 795f 6d65  MyGui.display_me
+00001dc0: 7373 6167 655f 626f 7863 0300 0000 0000  ssage_boxc......
+00001dd0: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
+00001de0: 0000 738c 0000 0064 017d 037c 0173 0d64  ..s....d.}.|.s.d
+00001df0: 027c 0217 0064 0317 007d 0364 047c 005f  .|...d...}.d.|._
+00001e00: 007c 006a 0172 167c 006a 0272 1664 057d  .|.j.r.|.j.r.d.}
+00001e10: 036e 117c 006a 0172 1f7c 006a 0372 1f64  .n.|.j.r.|.j.r.d
+00001e20: 067d 036e 087c 006a 0272 277c 006a 0372  .}.n.|.j.r'|.j.r
+00001e30: 2764 077d 037c 0372 387c 00a0 047c 03a1  'd.}.|.r8|...|..
+00001e40: 0101 0064 085c 037c 005f 017c 005f 027c  ...d.\.|._.|._.|
+00001e50: 005f 0364 0053 007c 00a0 0564 097c 019b  ._.d.S.|...d.|..
+00001e60: 0064 0a7c 029b 009d 0464 0ba1 0201 0064  .d.|.....d.....d
+00001e70: 0053 0029 0c4e 7275 0000 007a 2145 7272  .S.).Nru...z!Err
+00001e80: 6f72 3a0a 0a54 6865 206e 616d 6520 656e  or:..The name en
+00001e90: 7465 7265 6420 666f 7220 7468 6520 7a16  tered for the z.
+00001ea0: 2069 7320 626c 616e 6b21 0a0a 5472 7920   is blank!..Try 
+00001eb0: 6167 6169 6e2e 467a 5b45 7272 6f72 3a0a  again.Fz[Error:.
+00001ec0: 0a59 6f75 2068 6176 6520 656e 7465 7265  .You have entere
+00001ed0: 6420 626f 7468 2061 2050 726f 6a65 6374  d both a Project
+00001ee0: 2061 6e64 2061 2050 726f 6669 6c65 206e   and a Profile n
+00001ef0: 616d 6521 0a0a 5472 7920 6167 6169 6e20  ame!..Try again 
+00001f00: 616e 6420 6f6e 6c79 2073 656c 6563 7420  and only select 
+00001f10: 6f6e 652e 7a58 4572 726f 723a 0a0a 596f  one.zXError:..Yo
+00001f20: 7520 6861 7665 2065 6e74 6572 6564 2062  u have entered b
+00001f30: 6f74 6820 6120 5072 6f6a 6563 7420 616e  oth a Project an
+00001f40: 6420 6120 5461 736b 206e 616d 6521 0a0a  d a Task name!..
+00001f50: 5472 7920 6167 6169 6e20 616e 6420 6f6e  Try again and on
+00001f60: 6c79 2073 656c 6563 7420 6f6e 652e 7a58  ly select one.zX
+00001f70: 4572 726f 723a 0a0a 596f 7520 6861 7665  Error:..You have
+00001f80: 2065 6e74 6572 6564 2062 6f74 6820 6120   entered both a 
+00001f90: 5072 6f66 696c 6520 616e 6420 6120 5461  Profile and a Ta
+00001fa0: 736b 206e 616d 6521 0a0a 5472 7920 6167  sk name!..Try ag
+00001fb0: 6169 6e20 616e 6420 6f6e 6c79 2073 656c  ain and only sel
+00001fc0: 6563 7420 6f6e 652e 2903 7275 0000 0072  ect one.).ru...r
+00001fd0: 7500 0000 7275 0000 007a 1244 6973 706c  u...ru...z.Displ
+00001fe0: 6179 206f 6e6c 7920 7468 6520 277a 0227  ay only the 'z.'
+00001ff0: 2054 2906 5a0a 6e61 6d65 645f 6974 656d   T).Z.named_item
+00002000: 7280 0000 0072 8100 0000 7282 0000 0072  r....r....r....r
+00002010: 9000 0000 7295 0000 0029 0472 6f00 0000  ....r....).ro...
+00002020: da08 7468 655f 6e61 6d65 5a0c 656c 656d  ..the_nameZ.elem
+00002030: 656e 745f 6e61 6d65 728f 0000 0072 7200  ent_namer....rr.
+00002040: 0000 7272 0000 0072 7300 0000 da0a 6368  ..rr...rs.....ch
+00002050: 6563 6b5f 6e61 6d65 6001 0000 7338 0000  eck_name`...s8..
+00002060: 0004 0104 0102 0202 0102 ff02 0202 fe02  ................
+00002070: ff06 050c 0102 0204 ff0c 0402 0204 ff0c  ................
+00002080: 0402 0202 ff04 050a 0102 0502 fc04 0104  ................
+00002090: 0108 0104 0310 0108 ff7a 104d 7947 7569  .........z.MyGui
+000020a0: 2e63 6865 636b 5f6e 616d 6563 0100 0000  .check_namec....
+000020b0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+000020c0: 4300 0000 f34c 0000 0064 017d 017c 00a0  C....L...d.}.|..
+000020d0: 007c 01a1 0101 007c 006a 01a0 02a1 0001  .|.....|.j......
+000020e0: 007c 006a 03a0 02a1 0001 0074 046a 0564  .|.j.......t.j.d
+000020f0: 0264 0364 048d 027d 027c 02a0 06a1 007c  .d.d...}.|.....|
+00002100: 005f 077c 00a0 087c 006a 0764 05a1 0201  ._.|...|.j.d....
+00002110: 0064 0053 0029 064e 7275 0000 007a 1345  .d.S.).Nru...z.E
+00002120: 6e74 6572 2050 726f 6a65 6374 206e 616d  nter Project nam
+00002130: 653a 7a18 4469 7370 6c61 7920 5370 6563  e:z.Display Spec
+00002140: 6966 6963 2050 726f 6a65 6374 a902 7217  ific Project..r.
+00002150: 0000 0072 4700 0000 da07 5072 6f6a 6563  ...rG.....Projec
+00002160: 7429 0972 9000 0000 7266 0000 00da 0864  t).r....rf.....d
+00002170: 6573 656c 6563 7472 6800 0000 724b 0000  eselectrh...rK..
+00002180: 00da 0e43 546b 496e 7075 7444 6961 6c6f  ...CTkInputDialo
+00002190: 67da 0967 6574 5f69 6e70 7574 7280 0000  g..get_inputr...
+000021a0: 0072 9700 0000 a903 726f 0000 0072 8f00  .r......ro...r..
+000021b0: 0000 da06 6469 616c 6f67 7272 0000 0072  ....dialogrr...r
+000021c0: 7200 0000 7273 0000 0072 6300 0000 8801  r...rs...rc.....
+000021d0: 0000 f312 0000 0004 020a 010a 020a 0104  ................
+000021e0: 0204 0106 ff0a 0412 027a 1f4d 7947 7569  .........z.MyGui
+000021f0: 2e73 696e 676c 655f 7072 6f6a 6563 745f  .single_project_
+00002200: 6e61 6d65 5f65 7665 6e74 6301 0000 0000  name_eventc.....
+00002210: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00002220: 0000 0072 9800 0000 2906 4e72 7500 0000  ...r....).Nru...
+00002230: 7a13 456e 7465 7220 5072 6f66 696c 6520  z.Enter Profile 
+00002240: 6e61 6d65 3a7a 1844 6973 706c 6179 2053  name:z.Display S
+00002250: 7065 6369 6669 6320 5072 6f66 696c 6572  pecific Profiler
+00002260: 9900 0000 da07 5072 6f66 696c 6529 0972  ......Profile).r
+00002270: 9000 0000 7264 0000 0072 9b00 0000 7268  ....rd...r....rh
+00002280: 0000 0072 4b00 0000 729c 0000 0072 9d00  ...rK...r....r..
+00002290: 0000 7281 0000 0072 9700 0000 729e 0000  ..r....r....r...
+000022a0: 0072 7200 0000 7272 0000 0072 7300 0000  .rr...rr...rs...
+000022b0: 7265 0000 009b 0100 0072 a000 0000 7a1f  re.......r....z.
+000022c0: 4d79 4775 692e 7369 6e67 6c65 5f70 726f  MyGui.single_pro
+000022d0: 6669 6c65 5f6e 616d 655f 6576 656e 7463  file_name_eventc
+000022e0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000022f0: 0400 0000 4300 0000 7298 0000 0029 064e  ....C...r....).N
+00002300: 7275 0000 007a 1045 6e74 6572 2054 6173  ru...z.Enter Tas
+00002310: 6b20 6e61 6d65 3a7a 1544 6973 706c 6179  k name:z.Display
+00002320: 2053 7065 6369 6669 6320 5461 736b 7299   Specific Taskr.
+00002330: 0000 00da 0454 6173 6b29 0972 9000 0000  .....Task).r....
+00002340: 7264 0000 0072 9b00 0000 7266 0000 0072  rd...r....rf...r
+00002350: 4b00 0000 729c 0000 0072 9d00 0000 7282  K...r....r....r.
+00002360: 0000 0072 9700 0000 729e 0000 0072 7200  ...r....r....rr.
+00002370: 0000 7272 0000 0072 7300 0000 7267 0000  ..rr...rs...rg..
+00002380: 00ae 0100 0072 a000 0000 7a1c 4d79 4775  .....r....z.MyGu
+00002390: 692e 7369 6e67 6c65 5f74 6173 6b5f 6e61  i.single_task_na
+000023a0: 6d65 5f65 7665 6e74 da13 6e65 775f 6170  me_event..new_ap
+000023b0: 7065 6172 616e 6365 5f6d 6f64 6563 0200  pearance_modec..
+000023c0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000023d0: 0000 4300 0000 7314 0000 0074 00a0 017c  ..C...s....t...|
+000023e0: 01a1 0101 007c 017c 005f 0264 0053 00a9  .....|.|._.d.S..
+000023f0: 014e 2903 724b 0000 00da 1373 6574 5f61  .N).rK.....set_a
+00002400: 7070 6561 7261 6e63 655f 6d6f 6465 7285  ppearance_moder.
+00002410: 0000 0029 0272 6f00 0000 72a3 0000 0072  ...).ro...r....r
+00002420: 7200 0000 7272 0000 0072 7300 0000 7258  r...rr...rs...rX
+00002430: 0000 00c1 0100 0073 0400 0000 0a01 0a01  .......s........
+00002440: 7a22 4d79 4775 692e 6368 616e 6765 5f61  z"MyGui.change_a
+00002450: 7070 6561 7261 6e63 655f 6d6f 6465 5f65  ppearance_mode_e
+00002460: 7665 6e74 da0e 6469 7370 6c61 795f 6465  vent..display_de
+00002470: 7461 696c 6302 0000 0000 0000 0000 0000  tailc...........
+00002480: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00002490: 0000 7c01 7c00 5f00 6400 5300 72a4 0000  ..|.|._.d.S.r...
+000024a0: 0029 0172 7800 0000 2902 726f 0000 0072  .).rx...).ro...r
+000024b0: a600 0000 7272 0000 0072 7200 0000 7273  ....rr...rr...rs
+000024c0: 0000 0072 4e00 0000 c801 0000 7302 0000  ...rN.......s...
+000024d0: 000a 017a 1b4d 7947 7569 2e64 6574 6169  ...z.MyGui.detai
+000024e0: 6c5f 7365 6c65 6374 6564 5f65 7665 6e74  l_selected_event
+000024f0: da13 636f 6c6f 725f 7365 6c65 6374 6564  ..color_selected
+00002500: 5f69 7465 6d63 0200 0000 0000 0000 0000  _itemc..........
+00002510: 0000 0800 0000 0800 0000 4300 0000 73d6  ..........C...s.
+00002520: 0000 0067 0064 01a2 017d 027c 006a 007c  ...g.d...}.|.j.|
+00002530: 006a 007c 006a 017c 006a 0267 047d 0374  .j.|.j.|.j.g.}.t
+00002540: 03a0 0474 05a1 018f 3001 007c 02a0 067c  ...t....0..|...|
+00002550: 01a1 017d 047c 037c 0419 0073 3c7c 01a0  ...}.|.|...s<|..
+00002560: 0764 0264 03a1 027d 057c 05a0 0764 0464  .d.d...}.|...d.d
+00002570: 03a1 027d 057c 00a0 0864 057c 059b 0064  ...}.|...d.|...d
+00002580: 069d 0364 07a1 0201 0009 0057 0064 0004  ...d.......W.d..
+00002590: 0004 0083 0301 0064 0053 0057 0064 0004  .......d.S.W.d..
+000025a0: 0004 0083 0301 006e 0831 0073 4677 0101  .......n.1.sFw..
+000025b0: 0001 0001 0059 0001 0074 0983 007d 067c  .....Y...t...}.|
+000025c0: 06a0 0aa1 007d 077c 0764 0075 0172 697c  .....}.|.d.u.ri|
+000025d0: 00a0 087c 019b 0064 087c 079b 009d 0364  ...|...d.|.....d
+000025e0: 07a1 0201 007c 00a0 0b7c 077c 01a1 0201  .....|...|.|....
+000025f0: 0064 0053 0064 0053 0029 094e 2904 723d  .d.S.d.S.).N).r=
+00002600: 0000 0072 3f00 0000 7243 0000 0072 4400  ...r?...rC...rD.
+00002610: 0000 7a08 5072 6f66 696c 6520 7275 0000  ..z.Profile ru..
+00002620: 007a 0741 6374 696f 6e20 7a08 4469 7370  .z.Action z.Disp
+00002630: 6c61 7920 7a17 2069 7320 6e6f 7420 7365  lay z. is not se
+00002640: 7420 746f 2064 6973 706c 6179 2146 fa12  t to display!F..
+00002650: 2063 6f6c 6f72 2063 6861 6e67 6564 2074   color changed t
+00002660: 6f20 290c 7279 0000 0072 7b00 0000 727a  o ).ry...r{...rz
+00002670: 0000 00da 0a63 6f6e 7465 7874 6c69 62da  .....contextlib.
+00002680: 0873 7570 7072 6573 73da 0945 7863 6570  .suppress..Excep
+00002690: 7469 6f6e da05 696e 6465 78da 0772 6570  tion..index..rep
+000026a0: 6c61 6365 7295 0000 0072 0300 0000 da03  lacer....r......
+000026b0: 6765 74da 1865 7874 7261 6374 5f63 6f6c  get..extract_col
+000026c0: 6f72 5f66 726f 6d5f 6576 656e 7429 0872  or_from_event).r
+000026d0: 6f00 0000 72a7 0000 005a 0d77 6172 6e69  o...r....Z.warni
+000026e0: 6e67 5f63 6865 636b 5a0d 6368 6563 6b5f  ng_checkZ.check_
+000026f0: 6167 6169 6e73 745a 0974 6865 5f69 6e64  againstZ.the_ind
+00002700: 6578 5a12 7468 655f 6f75 7470 7574 5f6d  exZ.the_output_m
+00002710: 6573 7361 6765 5a0a 7069 636b 5f63 6f6c  essageZ.pick_col
+00002720: 6f72 7294 0000 0072 7200 0000 7272 0000  orr....rr...rr..
+00002730: 0072 7300 0000 7269 0000 00ce 0100 0073  .rs...ri.......s
+00002740: 3400 0000 0801 0407 0401 0401 0401 04fc  4...............
+00002750: 0c09 0a01 0801 0c01 0c01 0401 0c01 04ff  ................
+00002760: 0203 10f8 0202 1cfe 060a 0801 0801 0401  ................
+00002770: 0e01 04ff 1005 04fa 7a12 4d79 4775 692e  ........z.MyGui.
+00002780: 636f 6c6f 7273 5f65 7665 6e74 6303 0000  colors_eventc...
+00002790: 0000 0000 0000 0000 0004 0000 0007 0000  ................
+000027a0: 0043 0000 0073 7c00 0000 7c00 6a00 7d03  .C...s|...|.j.}.
+000027b0: 7c01 7c00 6a01 7402 7c02 1900 3c00 7c00  |.|.j.t.|...<.|.
+000027c0: 6a03 a004 7405 6a06 7c00 6a07 a008 6401  j...t.j.|.j...d.
+000027d0: a101 7c02 9b00 6402 9d02 7c01 6403 8d03  ..|...d...|.d...
+000027e0: a101 0100 7c00 6a03 6404 1900 6a09 7c00  ....|.j.d...j.|.
+000027f0: 6a00 6405 6405 6405 6406 8d04 0100 7c00  j.d.d.d.d.....|.
+00002800: 0400 6a00 6407 3700 0200 5f00 7c00 a00a  ..j.d.7..._.|...
+00002810: 7c02 9b00 6408 7c01 9b00 9d03 6409 a102  |...d.|.....d...
+00002820: 0100 6400 5300 290a 4e72 3900 0000 7a09  ..d.S.).Nr9...z.
+00002830: 203c 3c20 636f 6c6f 7229 0272 1700 0000   << color).r....
+00002840: 7234 0000 00e9 ffff ffff 7201 0000 0072  r4........r....r
+00002850: 1a00 0000 7208 0000 0072 a800 0000 5429  ....r....r....T)
+00002860: 0b72 8300 0000 7288 0000 0072 0500 0000  .r....r....r....
+00002870: 7284 0000 00da 0661 7070 656e 6472 4b00  r......appendrK.
+00002880: 0000 724d 0000 0072 6000 0000 7262 0000  ..rM...r`...rb..
+00002890: 0072 4c00 0000 7295 0000 0029 0472 6f00  .rL...r....).ro.
+000028a0: 0000 7294 0000 0072 a700 0000 7210 0000  ..r....r....r...
+000028b0: 0072 7200 0000 7272 0000 0072 7300 0000  .rr...rr...rs...
+000028c0: 72af 0000 00f2 0100 0073 1e00 0000 0601  r........s......
+000028d0: 0202 0cff 0603 0401 0a01 0801 0201 04fd  ................
+000028e0: 04ff 1a07 0e01 0401 0e01 08ff 7a1e 4d79  ............z.My
+000028f0: 4775 692e 6578 7472 6163 745f 636f 6c6f  Gui.extract_colo
+00002900: 725f 6672 6f6d 5f65 7665 6e74 6301 0000  r_from_eventc...
+00002910: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00002920: 0043 0000 00f3 1000 0000 7c00 6a00 a001  .C........|.j...
+00002930: a100 7c00 5f02 6400 5300 72a4 0000 0029  ..|._.d.S.r....)
+00002940: 0372 5100 0000 72ae 0000 0072 7900 0000  .rQ...r....ry...
+00002950: 726e 0000 0072 7200 0000 7272 0000 0072  rn...rr...rr...r
+00002960: 7300 0000 7250 0000 0007 0200 00f3 0200  s...rP..........
+00002970: 0000 1001 7a15 4d79 4775 692e 636f 6e64  ....z.MyGui.cond
+00002980: 6974 696f 6e5f 6576 656e 7463 0100 0000  ition_eventc....
+00002990: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000029a0: 4300 0000 72b2 0000 0072 a400 0000 2903  C...r....r....).
+000029b0: 7255 0000 0072 ae00 0000 727a 0000 0072  rU...r....rz...r
+000029c0: 6e00 0000 7272 0000 0072 7200 0000 7273  n...rr...rr...rs
+000029d0: 0000 0072 5400 0000 0d02 0000 72b3 0000  ...rT.......r...
+000029e0: 007a 1f4d 7947 7569 2e64 6973 706c 6179  .z.MyGui.display
+000029f0: 5f70 7265 6665 7265 6e63 6573 5f65 7665  _preferences_eve
+00002a00: 6e74 6301 0000 0000 0000 0000 0000 0001  ntc.............
+00002a10: 0000 0002 0000 0043 0000 0072 b200 0000  .......C...r....
+00002a20: 72a4 0000 0029 0372 5300 0000 72ae 0000  r....).rS...r...
+00002a30: 0072 7b00 0000 726e 0000 0072 7200 0000  .r{...rn...rr...
+00002a40: 7272 0000 0072 7300 0000 7252 0000 0013  rr...rs...rR....
+00002a50: 0200 0072 b300 0000 7a1d 4d79 4775 692e  ...r....z.MyGui.
+00002a60: 6469 7370 6c61 795f 7461 736b 6572 6e65  display_taskerne
+00002a70: 745f 6576 656e 7463 0100 0000 0000 0000  t_eventc........
+00002a80: 0000 0000 0200 0000 0900 0000 4300 0000  ............C...
+00002a90: 734a 0000 007c 006a 007c 006a 017c 006a  sJ...|.j.|.j.|.j
+00002aa0: 027c 006a 037c 006a 047c 006a 057c 006a  .|.j.|.j.|.j.|.j
+00002ab0: 067c 006a 0764 019c 087d 0174 0864 027c  .|.j.d...}.t.d.|
+00002ac0: 006a 097c 0183 035c 027d 017c 005f 097c  .j.|...\.}.|._.|
+00002ad0: 00a0 0a64 0364 02a1 0201 0064 0053 0029  ...d.d.....d.S.)
+00002ae0: 044e 2908 7278 0000 0072 7900 0000 727a  .N).rx...ry...rz
+00002af0: 0000 0072 7b00 0000 7280 0000 0072 8100  ...r{...r....r..
+00002b00: 0000 7282 0000 0072 7c00 0000 547a 0f53  ..r....r|...Tz.S
+00002b10: 6574 7469 6e67 7320 7361 7665 642e 290b  ettings saved.).
+00002b20: 7278 0000 0072 7900 0000 727a 0000 0072  rx...ry...rz...r
+00002b30: 7b00 0000 7280 0000 0072 8100 0000 7282  {...r....r....r.
+00002b40: 0000 0072 7c00 0000 7204 0000 0072 8800  ...r|...r....r..
+00002b50: 0000 7295 0000 0029 0272 6f00 0000 da09  ..r....).ro.....
+00002b60: 7465 6d70 5f61 7267 7372 7200 0000 7272  temp_argsrr...rr
+00002b70: 0000 0072 7300 0000 7256 0000 0019 0200  ...rs...rV......
+00002b80: 0073 1a00 0000 0402 0401 0401 0401 0401  .s..............
+00002b90: 0401 0401 0401 06f8 020a 0801 0aff 1003  ................
+00002ba0: 7a19 4d79 4775 692e 7361 7665 5f73 6574  z.MyGui.save_set
+00002bb0: 7469 6e67 735f 6576 656e 7463 0300 0000  tings_eventc....
+00002bc0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00002bd0: 4300 0000 7346 0100 0064 017d 037c 0104  C...sF...d.}.|..
+00002be0: 0064 026b 0272 1801 007c 0272 117c 006a  .d.k.r...|.r.|.j
+00002bf0: 00a0 01a1 0001 007c 0353 007c 006a 00a0  .......|.S.|.j..
+00002c00: 02a1 0001 007c 0353 0004 0064 036b 0272  .....|.S...d.k.r
+00002c10: 2701 007c 006a 03a0 0474 057c 0283 01a1  '..|.j...t.|....
+00002c20: 0101 007c 0353 0004 0064 046b 0272 3c01  ...|.S...d.k.r<.
+00002c30: 007c 0272 357c 006a 06a0 01a1 0001 007c  .|.r5|.j.......|
+00002c40: 0353 007c 006a 06a0 02a1 0001 007c 0353  .S.|.j.......|.S
+00002c50: 0004 0064 056b 0272 5101 007c 0272 4a7c  ...d.k.rQ..|.rJ|
+00002c60: 006a 07a0 01a1 0001 007c 0353 007c 006a  .j.......|.S.|.j
+00002c70: 07a0 02a1 0001 007c 0353 0004 0064 066b  .......|.S...d.k
+00002c80: 0272 6601 007c 0272 5f7c 006a 08a0 01a1  .rf..|.r_|.j....
+00002c90: 0001 007c 0353 007c 006a 08a0 02a1 0001  ...|.S.|.j......
+00002ca0: 007c 0353 0004 0064 076b 0272 7701 007c  .|.S...d.k.rw..|
+00002cb0: 0272 757c 039b 0064 087c 029b 0064 099d  .ru|...d.|...d..
+00002cc0: 047d 037c 0353 0004 0064 0a6b 0272 8801  .}.|.S...d.k.r..
+00002cd0: 007c 0272 867c 039b 0064 0b7c 029b 0064  .|.r.|...d.|...d
+00002ce0: 099d 047d 037c 0353 0064 0c6b 0272 977c  ...}.|.S.d.k.r.|
+00002cf0: 0272 957c 039b 0064 0d7c 029b 0064 099d  .r.|...d.|...d..
+00002d00: 047d 037c 0353 0009 007c 00a0 0964 0e7c  .}.|.S...|...d.|
+00002d10: 029b 009d 0264 0fa1 0201 007c 0353 0029  .....d.....|.S.)
+00002d20: 104e 7275 0000 0072 7c00 0000 7278 0000  .Nru...r|...rx..
+00002d30: 0072 7900 0000 727a 0000 0072 7b00 0000  .ry...rz...r{...
+00002d40: 7280 0000 007a 0f50 726f 6a65 6374 2073  r....z.Project s
+00002d50: 6574 2074 6f20 7a02 2e0a 7281 0000 007a  et to z...r....z
+00002d60: 0f50 726f 6669 6c65 2073 6574 2074 6f20  .Profile set to 
+00002d70: 7282 0000 007a 0c54 6173 6b20 7365 7420  r....z.Task set 
+00002d80: 746f 207a 1d52 7574 726f 6821 2020 556e  to z.Rutroh!  Un
+00002d90: 6465 6669 6e65 6420 6172 6775 6d65 6e74  defined argument
+00002da0: 3a20 4629 0a72 6b00 0000 da06 7365 6c65  : F).rk.....sele
+00002db0: 6374 729b 0000 0072 4f00 0000 7277 0000  ctr....rO...rw..
+00002dc0: 00da 0373 7472 7251 0000 0072 5500 0000  ...strrQ...rU...
+00002dd0: 7253 0000 0072 9500 0000 2904 726f 0000  rS...r....).ro..
+00002de0: 00da 036b 6579 da05 7661 6c75 6572 9300  ...key..valuer..
+00002df0: 0000 7272 0000 0072 7200 0000 7273 0000  ..rr...rr...rs..
+00002e00: 00da 0f72 6573 746f 7265 5f64 6973 706c  ...restore_displ
+00002e10: 6179 2c02 0000 7358 0000 0004 0102 010a  ay,...sX........
+00002e20: 0104 010a 0104 1f0a e304 1d0a e410 0104  ................
+00002e30: 1b0a e604 010a 0104 180a ea04 160a eb04  ................
+00002e40: 010a 0104 130a ef04 110a f004 010a 0104  ................
+00002e50: 0e0a f404 0c0a f504 0110 0104 090a f804  ................
+00002e60: 0110 0104 0606 fb04 0110 0104 0302 fe12  ................
+00002e70: 0104 017a 154d 7947 7569 2e72 6573 746f  ...z.MyGui.resto
+00002e80: 7265 5f64 6973 706c 6179 6301 0000 0000  re_displayc.....
+00002e90: 0000 0000 0000 0007 0000 0008 0000 0043  ...............C
+00002ea0: 0000 0073 1601 0000 7c00 a000 6401 a101  ...s....|...d...
+00002eb0: 0100 6900 7d01 7401 6401 7c00 6a02 7c01  ..i.}.t.d.|.j.|.
+00002ec0: 8303 5c02 7d01 7c00 5f02 7a11 7c01 6402  ..\.}.|._.z.|.d.
+00002ed0: 1900 7221 7c00 a003 7c01 6402 1900 6401  ..r!|...|.d...d.
+00002ee0: a102 0100 5700 6400 5300 5700 6e09 0400  ....W.d.S.W.n...
+00002ef0: 7404 792b 0100 0100 0100 5900 6e01 7700  t.y+......Y.n.w.
+00002f00: 7c01 7331 7c00 6a02 7283 6403 5c02 7d02  |.s1|.j.r.d.\.}.
+00002f10: 7d03 7c01 a005 a100 4400 5d1a 5c02 7d04  }.|.....D.].\.}.
+00002f20: 7d05 7c04 6400 7501 7253 7406 7c00 7c04  }.|.d.u.rSt.|.|.
+00002f30: 7c05 8303 0100 7c00 a007 7c04 7c05 a102  |.....|...|.|...
+00002f40: 0400 7d03 7253 7c02 7c03 1700 7d02 7139  ..}.rS|.|...}.q9
+00002f50: 6404 6405 8400 7408 a005 a100 4400 8301  d.d...t.....D...
+00002f60: 7d06 7c00 6a02 a005 a100 4400 5d15 5c02  }.|.j.....D.].\.
+00002f70: 7d04 7d05 7c04 6400 7501 7277 7c02 9b00  }.}.|.d.u.rw|...
+00002f80: 6406 7c06 7c04 1900 9b00 6407 7c05 9b00  d.|.|.....d.|...
+00002f90: 6408 9d06 7d02 7162 7c00 a003 7c02 9b00  d...}.qb|...|...
+00002fa0: 6409 9d02 640a a102 0100 6400 5300 7c00  d...d.....d.S.|.
+00002fb0: a003 640b 6401 a102 0100 6400 5300 290c  ..d.d.....d.S.).
+00002fc0: 4e46 da03 6d73 6729 0272 7500 0000 7275  NF..msg).ru...ru
+00002fd0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002fe0: 0300 0000 0400 0000 5300 0000 7316 0000  ........S...s...
+00002ff0: 0069 007c 005d 075c 027d 017d 027c 027c  .i.|.].\.}.}.|.|
+00003000: 0193 0271 0253 0072 7200 0000 7272 0000  ...q.S.rr...rr..
+00003010: 0029 03da 022e 30da 016b da01 7672 7200  .)....0..k..vrr.
+00003020: 0000 7272 0000 0072 7300 0000 da0a 3c64  ..rr...rs.....<d
+00003030: 6963 7463 6f6d 703e 6d02 0000 7302 0000  ictcomp>m...s...
+00003040: 0016 007a 304d 7947 7569 2e72 6573 746f  ...z0MyGui.resto
+00003050: 7265 5f73 6574 7469 6e67 735f 6576 656e  re_settings_even
+00003060: 742e 3c6c 6f63 616c 733e 2e3c 6469 6374  t.<locals>.<dict
+00003070: 636f 6d70 3efa 0120 7a0e 2063 6f6c 6f72  comp>.. z. color
+00003080: 2073 6574 2074 6f20 7292 0000 007a 130a   set to r....z..
+00003090: 5365 7474 696e 6773 2072 6573 746f 7265  Settings restore
+000030a0: 642e 547a 174e 6f20 7365 7474 696e 6773  d.Tz.No settings
+000030b0: 2066 696c 6520 666f 756e 642e 2909 726d   file found.).rm
+000030c0: 0000 0072 0400 0000 7288 0000 0072 9500  ...r....r....r..
+000030d0: 0000 da08 4b65 7945 7272 6f72 da05 6974  ....KeyError..it
+000030e0: 656d 73da 0773 6574 6174 7472 72b9 0000  ems..setattrr...
+000030f0: 0072 0500 0000 2907 726f 0000 0072 b400  .r....).ro...r..
+00003100: 0000 5a0c 616c 6c5f 6d65 7373 6167 6573  ..Z.all_messages
+00003110: 5a0b 6e65 775f 6d65 7373 6167 6572 b700  Z.new_messager..
+00003120: 0000 72b8 0000 005a 0f69 6e76 5f63 6f6c  ..r....Z.inv_col
+00003130: 6f72 5f6e 616d 6573 7272 0000 0072 7200  or_namesrr...rr.
+00003140: 0000 7273 0000 0072 5700 0000 5502 0000  ..rs...rW...U...
+00003150: 733a 0000 000a 0104 0102 0208 010a ff02  s:..............
+00003160: 0408 0110 0106 0104 fe0c 0304 0102 ff0a  ................
+00003170: 0408 0110 0108 010c 0110 0108 0102 8012  ................
+00003180: 0212 0108 0118 0202 ff02 8016 0410 037a  ...............z
+00003190: 1c4d 7947 7569 2e72 6573 746f 7265 5f73  .MyGui.restore_s
+000031a0: 6574 7469 6e67 735f 6576 656e 7463 0100  ettings_eventc..
+000031b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000031c0: 0000 4300 0000 738c 0000 007c 006a 00a0  ..C...s....|.j..
+000031d0: 0164 01a1 0101 007c 006a 02a0 03a1 0001  .d.....|.j......
+000031e0: 007c 006a 04a0 03a1 0001 007c 006a 05a0  .|.j.......|.j..
+000031f0: 03a1 0001 007c 006a 06a0 0164 02a1 0101  .....|.j...d....
+00003200: 0074 07a0 0864 02a1 0101 007c 006a 09a0  .t...d.....|.j..
+00003210: 03a1 0001 007c 00a0 0a64 0364 04a1 0201  .....|...d.d....
+00003220: 007c 00a0 0b64 05a1 0101 007c 006a 0c72  .|...d.....|.j.r
+00003230: 3f7c 006a 0c44 005d 087d 017c 016a 0d64  ?|.j.D.].}.|.j.d
+00003240: 0564 068d 0101 0071 367c 00a0 0e64 07a1  .d.....q6|...d..
+00003250: 0101 0064 0053 0029 084e 7221 0000 0072  ...d.S.).Nr!...r
+00003260: 0600 0000 7a0f 5365 7474 696e 6773 2072  ....z.Settings r
+00003270: 6573 6574 2e54 7275 0000 0072 3a00 0000  eset.Tru...r:...
+00003280: 4629 0f72 4f00 0000 7277 0000 0072 5100  F).rO...rw...rQ.
+00003290: 0000 729b 0000 0072 5500 0000 7253 0000  ..r....rU...rS..
+000032a0: 0072 5900 0000 724b 0000 0072 a500 0000  .rY...rK...r....
+000032b0: 726b 0000 0072 9500 0000 7290 0000 0072  rk...r....r....r
+000032c0: 8400 0000 725f 0000 0072 6d00 0000 2902  ....r_...rm...).
+000032d0: 726f 0000 00da 056c 6162 656c 7272 0000  ro.....labelrr..
+000032e0: 0072 7200 0000 7273 0000 0072 5a00 0000  .rr...rs...rZ...
+000032f0: 7c02 0000 731a 0000 000c 010a 010a 010a  |...s...........
+00003300: 010c 010a 010a 010c 010a 0106 010a 010e  ................
+00003310: 010e 017a 1a4d 7947 7569 2e72 6573 6574  ...z.MyGui.reset
+00003320: 5f73 6574 7469 6e67 735f 6576 656e 7463  _settings_eventc
+00003330: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00003340: 0400 0000 4300 0000 734e 0000 007c 006a  ....C...sN...|.j
+00003350: 00a0 01a1 007c 005f 027c 006a 0272 1f74  .....|._.|.j.r.t
+00003360: 0364 0183 01a0 04a1 0072 177c 00a0 0564  .d.......r.|...d
+00003370: 0264 03a1 0201 0064 0053 007c 00a0 0564  .d.....d.S.|...d
+00003380: 0464 05a1 0201 0064 0053 007c 00a0 0564  .d.....d.S.|...d
+00003390: 0664 03a1 0201 0064 0053 0029 074e 7a0a  .d.....d.S.).Nz.
+000033a0: 6261 636b 7570 2e78 6d6c 7a13 4465 6275  backup.xmlz.Debu
+000033b0: 6720 6d6f 6465 2065 6e61 626c 6564 2e54  g mode enabled.T
+000033c0: 7a53 4465 6275 6720 6d6f 6465 2072 6571  zSDebug mode req
+000033d0: 7569 7265 7320 5461 736b 6572 2062 6163  uires Tasker bac
+000033e0: 6b75 7020 6669 6c65 2074 6f20 6265 206e  kup file to be n
+000033f0: 616d 6564 3a20 2762 6163 6b75 702e 786d  amed: 'backup.xm
+00003400: 6c27 2c20 7768 6963 6820 6973 206d 6973  l', which is mis
+00003410: 7369 6e67 2146 7a14 4465 6275 6720 6d6f  sing!Fz.Debug mo
+00003420: 6465 2064 6973 6162 6c65 642e 2906 726b  de disabled.).rk
+00003430: 0000 0072 ae00 0000 727c 0000 0072 0200  ...r....r|...r..
+00003440: 0000 da07 6973 5f66 696c 6572 9500 0000  ....is_filer....
+00003450: 726e 0000 0072 7200 0000 7272 0000 0072  rn...rr...rr...r
+00003460: 7300 0000 726a 0000 008e 0200 0073 1200  s...rj.......s..
+00003470: 0000 0c01 0601 0c01 1001 0402 0202 0203  ................
+00003480: 08fb 1008 7a1a 4d79 4775 692e 6465 6275  ....z.MyGui.debu
+00003490: 675f 6368 6563 6b62 6f78 5f65 7665 6e74  g_checkbox_event
+000034a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000034b0: 0002 0000 0043 0000 00f3 1200 0000 6401  .....C........d.
+000034c0: 7c00 5f00 7c00 a001 a100 0100 6400 5300  |._.|.......d.S.
+000034d0: a902 4e54 2902 727f 0000 00da 0471 7569  ..NT).r......qui
+000034e0: 7472 6e00 0000 7272 0000 0072 7200 0000  trn...rr...rr...
+000034f0: 7273 0000 0072 5b00 0000 a102 0000 f304  rs...r[.........
+00003500: 0000 0006 010c 017a 114d 7947 7569 2e72  .......z.MyGui.r
+00003510: 756e 5f70 726f 6772 616d 6301 0000 0000  un_programc.....
+00003520: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00003530: 0000 0072 c500 0000 72c6 0000 0029 0272  ...r....r....).r
+00003540: 7e00 0000 72c7 0000 0072 6e00 0000 7272  ~...r....rn...rr
+00003550: 0000 0072 7200 0000 7273 0000 0072 5c00  ...rr...rs...r\.
+00003560: 0000 a802 0000 72c8 0000 007a 124d 7947  ......r....z.MyG
+00003570: 7569 2e65 7869 745f 7072 6f67 7261 6d29  ui.exit_program)
+00003580: 1cda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00003590: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000035a0: 616d 655f 5f72 4600 0000 da04 626f 6f6c  ame__rF.....bool
+000035b0: 726d 0000 0072 9000 0000 7295 0000 0072  rm...r....r....r
+000035c0: 9700 0000 7263 0000 0072 6500 0000 7267  ....rc...re...rg
+000035d0: 0000 0072 b600 0000 7258 0000 0072 4e00  ...r....rX...rN.
+000035e0: 0000 7269 0000 0072 af00 0000 7250 0000  ..ri...r....rP..
+000035f0: 0072 5400 0000 7252 0000 0072 5600 0000  .rT...rR...rV...
+00003600: 72b9 0000 0072 5700 0000 725a 0000 0072  r....rW...rZ...r
+00003610: 6a00 0000 725b 0000 0072 5c00 0000 da0d  j...r[...r\.....
+00003620: 5f5f 636c 6173 7363 656c 6c5f 5f72 7200  __classcell__rr.
+00003630: 0000 7272 0000 0072 7000 0000 7273 0000  ..rr...rp...rs..
+00003640: 0072 0700 0000 3c00 0000 7330 0000 0008  .r....<...s0....
+00003650: 000c 0100 7f0e 7408 1708 0c08 0d08 2808  ......t.......(.
+00003660: 1308 130e 130e 070e 0608 2408 1508 0608  ..........$.....
+00003670: 0608 0608 1308 2908 2708 1208 1310 0772  ......).'......r
+00003680: 0700 0000 290f 72a9 0000 0072 4b00 0000  ....).r....rK...
+00003690: da07 7061 7468 6c69 6272 0200 0000 5a1f  ..pathlibr....Z.
+000036a0: 4354 6b43 6f6c 6f72 5069 636b 6572 2e63  CTkColorPicker.c
+000036b0: 746b 5f63 6f6c 6f72 5f70 6963 6b65 7272  tk_color_pickerr
+000036c0: 0300 0000 da17 6d61 7074 6173 6b65 722e  ......maptasker.
+000036d0: 7372 632e 6765 7470 7574 6172 6772 0400  src.getputargr..
+000036e0: 0000 da16 6d61 7074 6173 6b65 722e 7372  ....maptasker.sr
+000036f0: 632e 7379 7363 6f6e 7374 7205 0000 0072  c.sysconstr....r
+00003700: a500 0000 5a17 7365 745f 6465 6661 756c  ....Z.set_defaul
+00003710: 745f 636f 6c6f 725f 7468 656d 6572 8700  t_color_themer..
+00003720: 0000 5a03 4354 6b72 0700 0000 7272 0000  ..Z.CTkr....rr..
+00003730: 0072 7200 0000 7272 0000 0072 7300 0000  .rr...rr...rs...
+00003740: da08 3c6d 6f64 756c 653e 0100 0000 7316  ..<module>....s.
+00003750: 0000 0008 1208 010c 010c 010c 010c 010a  ................
+00003760: 030a 0202 0302 ff16 1d                   .........
```

### Comparing `maptasker-1.3.2/maptasker/src/__pycache__/xmldata.cpython-310.pyc` & `maptasker-1.3.3/maptasker/src/__pycache__/xmldata.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr  4 13:54:26 2023 UTC, .py size: 6623 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,159 @@
-00000000: 6f0d 0d0a 0000 0000 122c 2c64 df19 0000  o........,,d....
+00000000: 6f0d 0d0a 0000 0000 cb5d 3464 711a 0000  o........]4dq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
-00000040: 6d02 5a02 0100 6403 6503 6404 6504 6405  m.Z...d.e.d.e.d.
-00000050: 6504 6606 6406 6407 8404 5a05 6408 6409  e.f.d.d...Z.d.d.
-00000060: 8400 5a06 6405 6507 6602 640a 640b 8404  ..Z.d.e.f.d.d...
-00000070: 5a08 640c 6503 640d 6503 6405 6503 6606  Z.d.e.d.e.d.e.f.
-00000080: 640e 640f 8404 5a09 6410 5300 2911 e900  d.d...Z.d.S.)...
-00000090: 0000 0029 01da 1070 726f 6365 7373 5f78  ...)...process_x
-000000a0: 6d6c 5f6c 6973 7429 01da 1364 726f 705f  ml_list)...drop_
-000000b0: 7472 6169 6c69 6e67 5f63 6f6d 6d61 da03  trailing_comma..
-000000c0: 7461 67da 0466 6c61 67da 0672 6574 7572  tag..flag..retur
-000000d0: 6e63 0200 0000 0000 0000 0000 0000 0400  nc..............
-000000e0: 0000 0200 0000 4300 0000 732a 0000 0067  ......C...s*...g
-000000f0: 0064 01a2 017d 0267 0064 02a2 017d 037c  .d...}.g.d...}.|
-00000100: 0172 0e7c 007c 0276 0070 147c 010c 006f  .r.|.|.v.p.|...o
-00000110: 147c 007c 0376 0053 0029 037a ff65 7661  .|.|.v.S.).z.eva
-00000120: 6c75 6174 6520 7468 6520 786d 6c20 7461  luate the xml ta
-00000130: 6720 746f 2073 6565 2069 6620 6974 2069  g to see if it i
-00000140: 7320 6f6e 6520 6f66 206f 7572 2070 7265  s one of our pre
-00000150: 6465 6669 6e65 6420 7479 7065 730a 0a20  defined types.. 
-00000160: 2020 2050 6172 616d 6574 6572 733a 2074     Parameters: t
-00000170: 6865 2074 6167 2074 6f20 6576 616c 7561  he tag to evalua
-00000180: 7465 2c20 616e 6420 7768 6574 6865 7220  te, and whether 
-00000190: 7468 6973 2069 7320 6120 5363 656e 6520  this is a Scene 
-000001a0: 6f72 206e 6f74 2028 7768 6963 680a 2020  or not (which.  
-000001b0: 2020 2020 2020 2020 2020 6465 7465 726d            determ
-000001c0: 696e 6573 2077 6869 6368 206c 6973 7420  ines which list 
-000001d0: 6f66 2074 7970 6573 2074 6f20 6c6f 6f6b  of types to look
-000001e0: 2066 6f72 290a 0a20 2020 2052 6574 7572   for)..    Retur
-000001f0: 6e73 3a20 5472 7565 2069 6620 7461 6720  ns: True if tag 
-00000200: 666f 756e 642c 2046 616c 7365 206f 7468  found, False oth
-00000210: 6572 7769 7365 0a0a 2020 2020 2908 5a0b  erwise..    ).Z.
-00000220: 4c69 7374 456c 656d 656e 745a 0b54 6578  ListElementZ.Tex
-00000230: 7445 6c65 6d65 6e74 5a0c 496d 6167 6545  tElementZ.ImageE
-00000240: 6c65 6d65 6e74 5a0d 4275 7474 6f6e 456c  lementZ.ButtonEl
-00000250: 656d 656e 745a 0b4f 7661 6c45 6c65 6d65  ementZ.OvalEleme
-00000260: 6e74 5a0f 4564 6974 5465 7874 456c 656d  ntZ.EditTextElem
-00000270: 656e 745a 0b52 6563 7445 6c65 6d65 6e74  entZ.RectElement
-00000280: 5a0a 5765 6245 6c65 6d65 6e74 290f 5a0f  Z.WebElement).Z.
-00000290: 6368 6563 6b63 6861 6e67 6554 6173 6b5a  checkchangeTaskZ
-000002a0: 0963 6c69 636b 5461 736b 5a0f 666f 6375  .clickTaskZ.focu
-000002b0: 7363 6861 6e67 6554 6173 6b5a 1069 7465  schangeTaskZ.ite
-000002c0: 6d73 656c 6563 7465 6454 6173 6b5a 076b  mselectedTaskZ.k
-000002d0: 6579 5461 736b 5a0d 6c69 6e6b 636c 6963  eyTaskZ.linkclic
-000002e0: 6b54 6173 6b5a 0d6c 6f6e 6763 6c69 636b  kTaskZ.longclick
-000002f0: 5461 736b 5a0c 6d61 7063 6c69 636b 5461  TaskZ.mapclickTa
-00000300: 736b 5a10 6d61 706c 6f6e 6763 6c69 636b  skZ.maplongclick
-00000310: 5461 736b 5a0e 7061 6765 6c6f 6164 6564  TaskZ.pageloaded
-00000320: 5461 736b 5a0a 7374 726f 6b65 5461 736b  TaskZ.strokeTask
-00000330: 5a11 7661 6c75 6573 656c 6563 7465 6454  Z.valueselectedT
-00000340: 6173 6b5a 0976 6964 656f 5461 736b 5a0d  askZ.videoTaskZ.
-00000350: 6974 656d 636c 6963 6b54 6173 6b5a 1169  itemclickTaskZ.i
-00000360: 7465 6d6c 6f6e 6763 6c69 636b 5461 736b  temlongclickTask
-00000370: a900 2904 7204 0000 0072 0500 0000 5a18  ..).r....r....Z.
-00000380: 7363 656e 655f 7461 736b 5f65 6c65 6d65  scene_task_eleme
-00000390: 6e74 5f74 7970 6573 5a16 7363 656e 655f  nt_typesZ.scene_
-000003a0: 7461 736b 5f63 6c69 636b 5f74 7970 6573  task_click_types
-000003b0: 7207 0000 0072 0700 0000 fa76 2f55 7365  r....r.....v/Use
-000003c0: 7273 2f6d 696b 7275 6269 6e2f 4c69 6272  rs/mikrubin/Libr
-000003d0: 6172 792f 436c 6f75 6453 746f 7261 6765  ary/CloudStorage
-000003e0: 2f47 6f6f 676c 6544 7269 7665 2d6d 696b  /GoogleDrive-mik
-000003f0: 7275 6269 6e40 676d 6169 6c2e 636f 6d2f  rubin@gmail.com/
-00000400: 4d79 2044 7269 7665 2f50 7974 686f 6e2f  My Drive/Python/
-00000410: 6d61 7074 6173 6b65 722f 6d61 7074 6173  maptasker/maptas
-00000420: 6b65 722f 7372 632f 786d 6c64 6174 612e  ker/src/xmldata.
-00000430: 7079 da0b 7461 675f 696e 5f74 7970 6515  py..tag_in_type.
-00000440: 0000 0073 1000 0000 0809 080a 0413 0601  ...s............
-00000450: 02ff 0602 0601 02fc 7209 0000 0063 0300  ........r....c..
-00000460: 0000 0000 0000 0000 0000 0900 0000 0800  ................
-00000470: 0000 4300 0000 73ca 0000 0067 007d 037c  ..C...s....g.}.|
-00000480: 0044 005d 5c7d 047c 046a 0064 016b 0272  .D.]\}.|.j.d.k.r
-00000490: 607c 046a 01a0 0264 02a1 017d 057c 0144  `|.j...d...}.|.D
-000004a0: 005d 4c7d 067c 067c 056b 0272 5f7c 01a0  .]L}.|.|.k.r_|..
-000004b0: 037c 06a1 017d 0764 037d 087c 046a 01a0  .|...}.d.}.|.j..
-000004c0: 0264 04a1 0164 0075 0172 2f7c 046a 01a0  .d...d.u.r/|.j..
-000004d0: 0264 04a1 017d 086e 0d7c 04a0 0464 05a1  .d...}.n.|...d..
-000004e0: 0164 0075 0172 3c7c 04a0 0464 05a1 016a  .d.u.r<|...d...j
-000004f0: 057d 087c 0872 5a74 067c 027c 0719 0083  .}.|.rZt.|.|....
-00000500: 0174 0775 0072 4f74 087c 027c 077c 087c  .t.u.rOt.|.|.|.|
-00000510: 037c 0183 0501 006e 097c 03a0 097c 027c  .|.....n.|...|.|
-00000520: 0719 007c 0817 00a1 0101 0001 006e 067c  ...|.........n.|
-00000530: 03a0 0964 03a1 0101 0071 1371 0474 0a7c  ...d.....q.q.t.|
-00000540: 0383 0153 0029 064e da03 496e 74da 0273  ...S.).N..Int..s
-00000550: 72da 00da 0376 616c da03 7661 7229 0b72  r....val..var).r
-00000560: 0400 0000 da06 6174 7472 6962 da03 6765  ......attrib..ge
-00000570: 74da 0569 6e64 6578 da04 6669 6e64 da04  t..index..find..
-00000580: 7465 7874 da04 7479 7065 da04 6c69 7374  text..type..list
-00000590: 7202 0000 00da 0661 7070 656e 6472 0300  r......appendr..
-000005a0: 0000 2909 da06 6163 7469 6f6e da09 6172  ..)...action..ar
-000005b0: 6775 6d65 6e74 73da 056e 616d 6573 da0d  guments..names..
-000005c0: 6d61 7463 685f 7265 7375 6c74 73da 0563  match_results..c
-000005d0: 6869 6c64 da07 7468 655f 6172 67da 0361  hild..the_arg..a
-000005e0: 7267 da0c 6172 675f 6c6f 6361 7469 6f6e  rg..arg_location
-000005f0: da0d 7468 655f 696e 745f 7661 6c75 6572  ..the_int_valuer
-00000600: 0700 0000 7207 0000 0072 0800 0000 da1d  ....r....r......
-00000610: 6765 745f 786d 6c5f 696e 745f 6172 6775  get_xml_int_argu
-00000620: 6d65 6e74 5f74 6f5f 7661 6c75 654e 0000  ment_to_valueN..
-00000630: 0073 4000 0000 0401 0802 0a01 0c01 0801  .s@.............
-00000640: 0801 0a01 0401 1001 0601 0201 06ff 0e03  ................
-00000650: 0c01 0401 1002 0201 0201 0201 0201 0201  ................
-00000660: 0201 06fb 0408 0a01 04ff 0403 0402 0201  ................
-00000670: 04ff 0480 0804 7220 0000 0063 0300 0000  ......r ...c....
-00000680: 0000 0000 0000 0000 0800 0000 0600 0000  ................
-00000690: 4300 0000 737a 0000 0067 007d 037c 0044  C...sz...g.}.|.D
-000006a0: 005d 347d 047c 046a 0064 016b 0272 387c  .]4}.|.j.d.k.r8|
-000006b0: 046a 01a0 0264 02a1 017d 057c 0144 005d  .j...d...}.|.D.]
-000006c0: 247d 067c 067c 056b 0272 377c 01a0 037c  $}.|.|.k.r7|...|
-000006d0: 06a1 017d 077c 046a 0464 0075 0172 307c  ...}.|.j.d.u.r0|
-000006e0: 03a0 057c 027c 0719 007c 046a 0417 0064  ...|.|...|.j...d
-000006f0: 0317 00a1 0101 006e 057c 03a0 0564 04a1  .......n.|...d..
-00000700: 0101 0001 006e 0171 1371 0474 067c 0383  .....n.q.q.t.|..
-00000710: 0153 0029 054e da03 5374 7272 0b00 0000  .S.).N..Strr....
-00000720: 7a02 2c20 720c 0000 0029 0772 0400 0000  z., r....).r....
-00000730: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000740: 1300 0000 7216 0000 0072 0300 0000 2908  ....r....r....).
-00000750: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00000760: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
-00000770: 0000 0072 1e00 0000 7207 0000 0072 0700  ...r....r....r..
-00000780: 0000 7208 0000 00da 1d67 6574 5f78 6d6c  ..r......get_xml
-00000790: 5f73 7472 5f61 7267 756d 656e 745f 746f  _str_argument_to
-000007a0: 5f76 616c 7565 7a00 0000 731c 0000 0004  _valuez...s.....
-000007b0: 0108 010a 010c 0108 0108 010a 010a 011a  ................
-000007c0: 010a 0204 0102 fa02 8008 0772 2200 0000  ...........r"...
-000007d0: 7213 0000 00da 0b72 6570 6c61 6365 6d65  r......replaceme
-000007e0: 6e74 6302 0000 0000 0000 0000 0000 0004  ntc.............
-000007f0: 0000 0005 0000 0043 0000 0073 2000 0000  .......C...s ...
-00000800: 6401 6402 6c00 7d02 7c02 a001 6403 a101  d.d.l.}.|...d...
-00000810: 7d03 7c02 a002 7c03 7c01 7c00 a103 5300  }.|...|.|.|...S.
-00000820: 2904 7abc 5265 6d6f 7665 2068 746d 6c20  ).z.Remove html 
-00000830: 7461 6773 2066 726f 6d20 6120 7374 7269  tags from a stri
-00000840: 6e67 0a20 2020 203a 7061 7261 6d20 7465  ng.    :param te
-00000850: 7874 3a20 7465 7874 2066 726f 6d20 7768  xt: text from wh
-00000860: 6963 6820 4854 4d4c 2069 7320 746f 2062  ich HTML is to b
-00000870: 6520 7265 6d6f 7665 640a 2020 2020 3a70  e removed.    :p
-00000880: 6172 616d 2072 6570 6c61 6365 6d65 6e74  aram replacement
-00000890: 3a20 7465 7874 2074 6f20 7265 706c 6163  : text to replac
-000008a0: 6520 4854 4d4c 2077 6974 682c 2069 6620  e HTML with, if 
-000008b0: 616e 790a 2020 2020 3a72 6574 7572 6e3a  any.    :return:
-000008c0: 2074 6865 2074 6578 7420 7769 7468 2048   the text with H
-000008d0: 544d 4c20 7265 6d6f 7665 640a 2020 2020  TML removed.    
-000008e0: 7201 0000 004e 7a05 3c2e 2a3f 3e29 03da  r....Nz.<.*?>)..
-000008f0: 0272 65da 0763 6f6d 7069 6c65 da03 7375  .re..compile..su
-00000900: 6229 0472 1300 0000 7223 0000 0072 2400  b).r....r#...r$.
-00000910: 0000 da05 636c 6561 6e72 0700 0000 7207  ....cleanr....r.
-00000920: 0000 0072 0800 0000 da10 7265 6d6f 7665  ...r......remove
-00000930: 5f68 746d 6c5f 7461 6773 8a00 0000 7306  _html_tags....s.
-00000940: 0000 0008 060a 020e 0172 2800 0000 4e29  .........r(...N)
-00000950: 0ada 146d 6170 7461 736b 6572 2e73 7263  ...maptasker.src
-00000960: 2e61 6374 696f 6e72 0200 0000 7203 0000  .actionr....r...
-00000970: 00da 0373 7472 da04 626f 6f6c 7209 0000  ...str..boolr...
-00000980: 0072 2000 0000 7215 0000 0072 2200 0000  .r ...r....r"...
-00000990: 7228 0000 0072 0700 0000 7207 0000 0072  r(...r....r....r
-000009a0: 0700 0000 7208 0000 00da 083c 6d6f 6475  ....r......<modu
-000009b0: 6c65 3e01 0000 0073 0c00 0000 0c0d 0c01  le>....s........
-000009c0: 1606 0839 0e2c 1a10                      ...9.,..
+00000020: 0006 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
+00000030: 6500 6401 6501 6402 6501 6606 6403 6404  e.d.e.d.e.f.d.d.
+00000040: 8404 5a02 6405 6406 8400 5a03 6402 6504  ..Z.d.d...Z.d.e.
+00000050: 6602 6407 6408 8404 5a05 6409 6500 640a  f.d.d...Z.d.e.d.
+00000060: 6500 6402 6500 6606 640b 640c 8404 5a06  e.d.e.f.d.d...Z.
+00000070: 640d 5300 290e da03 7461 67da 0466 6c61  d.S.)...tag..fla
+00000080: 67da 0672 6574 7572 6e63 0200 0000 0000  g..returnc......
+00000090: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
+000000a0: 0000 732a 0000 0067 0064 01a2 017d 0267  ..s*...g.d...}.g
+000000b0: 0064 02a2 017d 037c 0172 0e7c 007c 0276  .d...}.|.r.|.|.v
+000000c0: 0070 147c 010c 006f 147c 007c 0376 0053  .p.|...o.|.|.v.S
+000000d0: 0029 037a ff65 7661 6c75 6174 6520 7468  .).z.evaluate th
+000000e0: 6520 786d 6c20 7461 6720 746f 2073 6565  e xml tag to see
+000000f0: 2069 6620 6974 2069 7320 6f6e 6520 6f66   if it is one of
+00000100: 206f 7572 2070 7265 6465 6669 6e65 6420   our predefined 
+00000110: 7479 7065 730a 0a20 2020 2050 6172 616d  types..    Param
+00000120: 6574 6572 733a 2074 6865 2074 6167 2074  eters: the tag t
+00000130: 6f20 6576 616c 7561 7465 2c20 616e 6420  o evaluate, and 
+00000140: 7768 6574 6865 7220 7468 6973 2069 7320  whether this is 
+00000150: 6120 5363 656e 6520 6f72 206e 6f74 2028  a Scene or not (
+00000160: 7768 6963 680a 2020 2020 2020 2020 2020  which.          
+00000170: 2020 6465 7465 726d 696e 6573 2077 6869    determines whi
+00000180: 6368 206c 6973 7420 6f66 2074 7970 6573  ch list of types
+00000190: 2074 6f20 6c6f 6f6b 2066 6f72 290a 0a20   to look for).. 
+000001a0: 2020 2052 6574 7572 6e73 3a20 5472 7565     Returns: True
+000001b0: 2069 6620 7461 6720 666f 756e 642c 2046   if tag found, F
+000001c0: 616c 7365 206f 7468 6572 7769 7365 0a0a  alse otherwise..
+000001d0: 2020 2020 2908 5a0b 4c69 7374 456c 656d      ).Z.ListElem
+000001e0: 656e 745a 0b54 6578 7445 6c65 6d65 6e74  entZ.TextElement
+000001f0: 5a0c 496d 6167 6545 6c65 6d65 6e74 5a0d  Z.ImageElementZ.
+00000200: 4275 7474 6f6e 456c 656d 656e 745a 0b4f  ButtonElementZ.O
+00000210: 7661 6c45 6c65 6d65 6e74 5a0f 4564 6974  valElementZ.Edit
+00000220: 5465 7874 456c 656d 656e 745a 0b52 6563  TextElementZ.Rec
+00000230: 7445 6c65 6d65 6e74 5a0a 5765 6245 6c65  tElementZ.WebEle
+00000240: 6d65 6e74 290f 5a0f 6368 6563 6b63 6861  ment).Z.checkcha
+00000250: 6e67 6554 6173 6b5a 0963 6c69 636b 5461  ngeTaskZ.clickTa
+00000260: 736b 5a0f 666f 6375 7363 6861 6e67 6554  skZ.focuschangeT
+00000270: 6173 6b5a 1069 7465 6d73 656c 6563 7465  askZ.itemselecte
+00000280: 6454 6173 6b5a 076b 6579 5461 736b 5a0d  dTaskZ.keyTaskZ.
+00000290: 6c69 6e6b 636c 6963 6b54 6173 6b5a 0d6c  linkclickTaskZ.l
+000002a0: 6f6e 6763 6c69 636b 5461 736b 5a0c 6d61  ongclickTaskZ.ma
+000002b0: 7063 6c69 636b 5461 736b 5a10 6d61 706c  pclickTaskZ.mapl
+000002c0: 6f6e 6763 6c69 636b 5461 736b 5a0e 7061  ongclickTaskZ.pa
+000002d0: 6765 6c6f 6164 6564 5461 736b 5a0a 7374  geloadedTaskZ.st
+000002e0: 726f 6b65 5461 736b 5a11 7661 6c75 6573  rokeTaskZ.values
+000002f0: 656c 6563 7465 6454 6173 6b5a 0976 6964  electedTaskZ.vid
+00000300: 656f 5461 736b 5a0d 6974 656d 636c 6963  eoTaskZ.itemclic
+00000310: 6b54 6173 6b5a 1169 7465 6d6c 6f6e 6763  kTaskZ.itemlongc
+00000320: 6c69 636b 5461 736b a900 2904 7201 0000  lickTask..).r...
+00000330: 0072 0200 0000 5a18 7363 656e 655f 7461  .r....Z.scene_ta
+00000340: 736b 5f65 6c65 6d65 6e74 5f74 7970 6573  sk_element_types
+00000350: 5a16 7363 656e 655f 7461 736b 5f63 6c69  Z.scene_task_cli
+00000360: 636b 5f74 7970 6573 7204 0000 0072 0400  ck_typesr....r..
+00000370: 0000 fa76 2f55 7365 7273 2f6d 696b 7275  ...v/Users/mikru
+00000380: 6269 6e2f 4c69 6272 6172 792f 436c 6f75  bin/Library/Clou
+00000390: 6453 746f 7261 6765 2f47 6f6f 676c 6544  dStorage/GoogleD
+000003a0: 7269 7665 2d6d 696b 7275 6269 6e40 676d  rive-mikrubin@gm
+000003b0: 6169 6c2e 636f 6d2f 4d79 2044 7269 7665  ail.com/My Drive
+000003c0: 2f50 7974 686f 6e2f 6d61 7074 6173 6b65  /Python/maptaske
+000003d0: 722f 6d61 7074 6173 6b65 722f 7372 632f  r/maptasker/src/
+000003e0: 786d 6c64 6174 612e 7079 da0b 7461 675f  xmldata.py..tag_
+000003f0: 696e 5f74 7970 6513 0000 0073 1000 0000  in_type....s....
+00000400: 0809 080a 0413 0601 02ff 0602 0601 02fc  ................
+00000410: 7206 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00000420: 0000 0b00 0000 0800 0000 4300 0000 73e2  ..........C...s.
+00000430: 0000 0064 0164 026c 006d 017d 0301 0064  ...d.d.l.m.}...d
+00000440: 0164 036c 006d 027d 0401 0067 007d 057c  .d.l.m.}...g.}.|
+00000450: 0044 005d 5c7d 067c 066a 0364 046b 0272  .D.]\}.|.j.d.k.r
+00000460: 6c7c 066a 04a0 0564 05a1 017d 077c 0144  l|.j...d...}.|.D
+00000470: 005d 4c7d 087c 087c 076b 0272 6b7c 01a0  .]L}.|.|.k.rk|..
+00000480: 067c 08a1 017d 0964 067d 0a7c 066a 04a0  .|...}.d.}.|.j..
+00000490: 0564 07a1 0164 0075 0172 3b7c 066a 04a0  .d...d.u.r;|.j..
+000004a0: 0564 07a1 017d 0a6e 0d7c 06a0 0764 08a1  .d...}.n.|...d..
+000004b0: 0164 0075 0172 487c 06a0 0764 08a1 016a  .d.u.rH|...d...j
+000004c0: 087d 0a7c 0a72 6674 097c 027c 0919 0083  .}.|.rft.|.|....
+000004d0: 0174 0a75 0072 5b7c 037c 027c 097c 0a7c  .t.u.r[|.|.|.|.|
+000004e0: 057c 0183 0501 006e 097c 05a0 0b7c 027c  .|.....n.|...|.|
+000004f0: 0919 007c 0a17 00a1 0101 0001 006e 067c  ...|.........n.|
+00000500: 05a0 0b64 06a1 0101 0071 1f71 107c 047c  ...d.....q.q.|.|
+00000510: 0583 0153 0029 094e e900 0000 0029 01da  ...S.).N.....)..
+00000520: 1070 726f 6365 7373 5f78 6d6c 5f6c 6973  .process_xml_lis
+00000530: 74a9 01da 1364 726f 705f 7472 6169 6c69  t....drop_traili
+00000540: 6e67 5f63 6f6d 6d61 da03 496e 74da 0273  ng_comma..Int..s
+00000550: 72da 00da 0376 616c da03 7661 7229 0cda  r....val..var)..
+00000560: 146d 6170 7461 736b 6572 2e73 7263 2e61  .maptasker.src.a
+00000570: 6374 696f 6e72 0800 0000 720a 0000 0072  ctionr....r....r
+00000580: 0100 0000 da06 6174 7472 6962 da03 6765  ......attrib..ge
+00000590: 74da 0569 6e64 6578 da04 6669 6e64 da04  t..index..find..
+000005a0: 7465 7874 da04 7479 7065 da04 6c69 7374  text..type..list
+000005b0: da06 6170 7065 6e64 290b da06 6163 7469  ..append)...acti
+000005c0: 6f6e da09 6172 6775 6d65 6e74 73da 056e  on..arguments..n
+000005d0: 616d 6573 7208 0000 0072 0a00 0000 da0d  amesr....r......
+000005e0: 6d61 7463 685f 7265 7375 6c74 73da 0563  match_results..c
+000005f0: 6869 6c64 da07 7468 655f 6172 67da 0361  hild..the_arg..a
+00000600: 7267 da0c 6172 675f 6c6f 6361 7469 6f6e  rg..arg_location
+00000610: da0d 7468 655f 696e 745f 7661 6c75 6572  ..the_int_valuer
+00000620: 0400 0000 7204 0000 0072 0500 0000 da1d  ....r....r......
+00000630: 6765 745f 786d 6c5f 696e 745f 6172 6775  get_xml_int_argu
+00000640: 6d65 6e74 5f74 6f5f 7661 6c75 654c 0000  ment_to_valueL..
+00000650: 0073 4400 0000 0c02 0c01 0402 0802 0a01  .sD.............
+00000660: 0c01 0801 0801 0a01 0401 1001 0601 0201  ................
+00000670: 06ff 0e03 0c01 0401 1002 0201 0201 0201  ................
+00000680: 0201 0201 0201 06fb 0408 0a01 04ff 0403  ................
+00000690: 0402 0201 04ff 0480 0804 7222 0000 0063  ..........r"...c
+000006a0: 0300 0000 0000 0000 0000 0000 0900 0000  ................
+000006b0: 0600 0000 4300 0000 7386 0000 0064 0164  ....C...s....d.d
+000006c0: 026c 006d 017d 0301 0067 007d 047c 0044  .l.m.}...g.}.|.D
+000006d0: 005d 347d 057c 056a 0264 036b 0272 3e7c  .]4}.|.j.d.k.r>|
+000006e0: 056a 03a0 0464 04a1 017d 067c 0144 005d  .j...d...}.|.D.]
+000006f0: 247d 077c 077c 066b 0272 3d7c 01a0 057c  $}.|.|.k.r=|...|
+00000700: 07a1 017d 087c 056a 0664 0075 0172 367c  ...}.|.j.d.u.r6|
+00000710: 04a0 077c 027c 0819 007c 056a 0617 0064  ...|.|...|.j...d
+00000720: 0517 00a1 0101 006e 057c 04a0 0764 06a1  .......n.|...d..
+00000730: 0101 0001 006e 0171 1971 0a7c 037c 0483  .....n.q.q.|.|..
+00000740: 0153 0029 074e 7207 0000 0072 0900 0000  .S.).Nr....r....
+00000750: da03 5374 7272 0c00 0000 7a02 2c20 720d  ..Strr....z., r.
+00000760: 0000 0029 0872 1000 0000 720a 0000 0072  ...).r....r....r
+00000770: 0100 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00000780: 0000 0072 1500 0000 7218 0000 0029 0972  ...r....r....).r
+00000790: 1900 0000 721a 0000 0072 1b00 0000 720a  ....r....r....r.
+000007a0: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+000007b0: 0000 721f 0000 0072 2000 0000 7204 0000  ..r....r ...r...
+000007c0: 0072 0400 0000 7205 0000 00da 1d67 6574  .r....r......get
+000007d0: 5f78 6d6c 5f73 7472 5f61 7267 756d 656e  _xml_str_argumen
+000007e0: 745f 746f 5f76 616c 7565 7c00 0000 731e  t_to_value|...s.
+000007f0: 0000 000c 0104 0208 010a 010c 0108 0108  ................
+00000800: 010a 010a 011a 010a 0204 0102 fa02 8008  ................
+00000810: 0772 2400 0000 7215 0000 00da 0b72 6570  .r$...r......rep
+00000820: 6c61 6365 6d65 6e74 6302 0000 0000 0000  lacementc.......
+00000830: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+00000840: 0073 2000 0000 6401 6402 6c00 7d02 7c02  .s ...d.d.l.}.|.
+00000850: a001 6403 a101 7d03 7c02 a002 7c03 7c01  ..d...}.|...|.|.
+00000860: 7c00 a103 5300 2904 7abc 5265 6d6f 7665  |...S.).z.Remove
+00000870: 2068 746d 6c20 7461 6773 2066 726f 6d20   html tags from 
+00000880: 6120 7374 7269 6e67 0a20 2020 203a 7061  a string.    :pa
+00000890: 7261 6d20 7465 7874 3a20 7465 7874 2066  ram text: text f
+000008a0: 726f 6d20 7768 6963 6820 4854 4d4c 2069  rom which HTML i
+000008b0: 7320 746f 2062 6520 7265 6d6f 7665 640a  s to be removed.
+000008c0: 2020 2020 3a70 6172 616d 2072 6570 6c61      :param repla
+000008d0: 6365 6d65 6e74 3a20 7465 7874 2074 6f20  cement: text to 
+000008e0: 7265 706c 6163 6520 4854 4d4c 2077 6974  replace HTML wit
+000008f0: 682c 2069 6620 616e 790a 2020 2020 3a72  h, if any.    :r
+00000900: 6574 7572 6e3a 2074 6865 2074 6578 7420  eturn: the text 
+00000910: 7769 7468 2048 544d 4c20 7265 6d6f 7665  with HTML remove
+00000920: 640a 2020 2020 7207 0000 004e 7a05 3c2e  d.    r....Nz.<.
+00000930: 2a3f 3e29 03da 0272 65da 0763 6f6d 7069  *?>)...re..compi
+00000940: 6c65 da03 7375 6229 0472 1500 0000 7225  le..sub).r....r%
+00000950: 0000 0072 2600 0000 5a05 636c 6561 6e72  ...r&...Z.cleanr
+00000960: 0400 0000 7204 0000 0072 0500 0000 da10  ....r....r......
+00000970: 7265 6d6f 7665 5f68 746d 6c5f 7461 6773  remove_html_tags
+00000980: 8e00 0000 7306 0000 0008 060a 020e 0172  ....s..........r
+00000990: 2900 0000 4e29 07da 0373 7472 da04 626f  )...N)...str..bo
+000009a0: 6f6c 7206 0000 0072 2200 0000 7217 0000  olr....r"...r...
+000009b0: 0072 2400 0000 7229 0000 0072 0400 0000  .r$...r)...r....
+000009c0: 7204 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
+000009d0: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
+000009e0: 0000 1612 0839 0e30 1a12                 .....9.0..
```

### Comparing `maptasker-1.3.2/maptasker/src/actargs.py` & `maptasker-1.3.3/maptasker/src/actargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 # ########################################################################################## #
 from maptasker.src.actiond import process_condition_list
 from maptasker.src.sysconst import logger
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 import maptasker.src.action as get_action
 
 
 def get_action_arguments(
     evaluated_results: dict,
     arg: object,
     argeval: list,
     argtype: list,
-    code_action: xml.etree,
-    action_type: xml.etree,
+    code_action: defusedxml.ElementTree.XML,
+    action_type: defusedxml.ElementTree.XML,
     colormap: dict,
     program_args: dict,
 ) -> dict:
     """
 
     :param evaluated_results: all the Action argument "types" and "arguments"
     :param arg: the incoming argument
```

### Comparing `maptasker-1.3.2/maptasker/src/action.py` & `maptasker-1.3.3/maptasker/src/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 
 import sys
 
 from maptasker.src.shellsort import shell_sort
+from maptasker.src.frmthtml import format_html
+from maptasker.src.xmldata import remove_html_tags
 from maptasker.src.sysconst import logger
-from maptasker.src.sysconst import FONT_TO_USE
 
 
 # #######################################################################################
 # Given a Task's Action, find all 'arg(n)' xml elements and return as a sorted list
 # Input:
 #   action: list of actions or parameters
 #   ignore_list: xml to ignore (e.g. label, on, etc.
@@ -40,17 +41,19 @@
             continue
         else:
             master_list.append(child)  # Build out list of args
     # If we have args then sort them and convert to string
     if master_list:
         # Sort args by their number (e.g. arg0, arg1, arg2, ...)
         shell_sort(master_list, True, False)
+        # Now go through args and build our "type" and "arg" lists
         for child in master_list:
             type_list.append(child.tag)  # one of: 'Str' 'Int' 'Bundle' 'App'
             arg_list.append(child.attrib.get("sr"))
+        # Build list of arg position only (numeric part of argn)
         arg_nums = [
             str(ind) for ind, x in enumerate(arg_list)
         ]  # Build list of arg position only (numeric part of argn)
 
     return arg_list, type_list, arg_nums
 
 
@@ -200,47 +203,48 @@
     return
 
 
 # ####################################################################################################
 # Get Task's label, disabled flag and any conditions
 # ####################################################################################################
 def get_label_disabled_condition(child, colormap):
-    disabled_action_html = (
-        ' </span><span style="color:'
-        + colormap["disabled_action_color"]
-        + FONT_TO_USE
-        + '>[DISABLED]</span>'
-    )
-
     task_label = ""
     task_conditions = ""
     the_action_code = child.find("code").text
     if child.find("label") is not None:
         lbl = child.find("label").text
-        # We have to be careful what we strip out and what we replace for the label to maintain
-        #  as much of the visual context as possible without blowing-up everything else that follows.
-        if lbl not in ["", "\n"]:
-            task_label = clean_label(lbl, colormap)
+        # Make sure the label doesn't have any HTML crap in it
+        task_label = clean_label(lbl, colormap)
 
-    action_disabled = disabled_action_html if child.find("on") is not None else ""
+    action_disabled = (
+        format_html(colormap, "disabled_action_color", "", " [DISABLED]", True)
+        if child.find("on") is not None
+        else ""
+    )
     if child.find("ConditionList") is not None:  # If condition on Action?
         condition_count = 0
         boolean_to_inject = ""
         booleans = []
         for children in child.find("ConditionList"):
             if "bool" in children.tag:
                 booleans.append(children.text)
             elif children.tag == "Condition" and the_action_code != "37":
                 string1, operator, string2 = evaluate_condition(children)
                 if condition_count != 0:
                     boolean_to_inject = f"{booleans[condition_count - 1].upper()} "
-                task_conditions = (
-                    f'{task_conditions} <span style='
-                    f' "color:{colormap["action_condition_color"]}"></span>'
-                    f' ({boolean_to_inject}condition:  If {string1}{operator}{string2})'
+                task_conditions = format_html(
+                    colormap,
+                    "action_condition_color",
+                    "",
+                    (
+                        f' ({boolean_to_inject}condition:  '
+                        f'If {string1}{operator}'
+                        f'{string2})'
+                    ),
+                    True,
                 )
                 condition_count += 1
         if the_action_code == "35":  # Wait Until?
             task_conditions = task_conditions.replace(
                 "condition:  If", "<em>UNTIL</em>"
             )
 
@@ -248,41 +252,29 @@
 
 
 # ####################################################################################################
 # Given the Task action's label, get rid of anything that could be problematic for the output format
 # ####################################################################################################
 def clean_label(lbl, colormap):
     # Look for label with <font color=...> embedded
-    lbl = lbl.replace("\n", "")
-    lbl = lbl.replace("</font>", "")
-    lbl = lbl.replace("</big>", "")
-    lbl = lbl.replace("</font></font>", "</font>")
-    font_count = lbl.count("<font")
-    if (
-        font_count > 0
-    ):  # Make sure we end with the same number combination of <font> and </font>
-        end_font_count = lbl.count("/font")
-        if font_count > end_font_count:
-            lbl = f'{lbl}<span style="color:{colormap["action_label_color"]}"'
-
-    return (
-        f' <span style="color:{colormap["action_label_color"]}">...with label:'
-        f' {lbl}</span></b>'
+    lbl = remove_html_tags(lbl, "")
+
+    return format_html(
+        colormap, "action_label_color", "", f" ...with label: {lbl}", True
     )
 
 
 # ####################################################################################################
 # Chase after relevant data after <code> Task action
 # code_flag identifies the type of xml data to go after based on the specific code in <code>xxx</code>
 # Get the: label, whether to continue Task after error, etc.
 # ####################################################################################################
 def get_extra_stuff(code_action, action_type, colormap, program_args):
-    if (
-        action_type
-    ):  # Only get extras if this is a Task action (vs. a Profile condition)
+    # Only get extras if this is a Task action (vs. a Profile condition)
+    if action_type:
         extra_stuff = get_label_disabled_condition(
             code_action, colormap
         )  # Look for extra Task stiff: label, disabled, conditions
         if (
             "<font" in extra_stuff and "</font>" not in extra_stuff
         ):  # Make sure we terminate any fonts
             extra_stuff = f"{extra_stuff}</font>"
@@ -295,26 +287,27 @@
         ):  # Make sure we terminate any bold
             extra_stuff = f"{extra_stuff}</b>"
     else:
         extra_stuff = ""
     if (
         program_args["debug"] and action_type
     ):  # Add the code if this is an Action and in debug mode
-        extra_stuff = (
-            f'{extra_stuff}</span><span'
-            f' style="color:Red{program_args["font_to_use"]}>&nbsp;&nbsp;code:'
-            + code_action.find("code").text
-            + "-"
+        extra_stuff = format_html(
+            colormap,
+            "Yellow",
+            "",
+            f'&nbsp;&nbsp;code: {code_action.find("code").text}-',
+            False,
         )
 
     # See if Task action is to be continued after error
     child = code_action.find("se")
     if child is not None and child.text == "false":
         extra_stuff = f" [Continue Task After Error]{extra_stuff}"
-    return extra_stuff
+    return f"{extra_stuff}</span>"
 
 
 # ####################################################################################################
 # Get the application specifics for the given code
 # ####################################################################################################
 def get_app_details(code_child, action_type, colormap, program_args):
     extra_stuff = get_extra_stuff(code_child, action_type, colormap, program_args)
```

### Comparing `maptasker-1.3.2/maptasker/src/actionc.py` & `maptasker-1.3.3/maptasker/src/actionc.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/actiond.py` & `maptasker-1.3.3/maptasker/src/actiond.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,37 +7,37 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 from typing import Any
 
 import maptasker.src.action as get_action
 from maptasker.src.sysconst import logger
 from maptasker.src.actionc import action_codes
 
 ignore_list = ["code", "label", "se", "on", "ListElementItem", "pri", "pin"]
 
 
 # #######################################################################################
 # Provide the Action dictionary to the caller
 # #######################################################################################
-def get_dict() -> xml.etree.ElementTree:
+def get_dict() -> defusedxml.ElementTree:
     return action_codes
 
 
 # #######################################################################################
 # Update the dictionary for the Action code
 # #######################################################################################
 def update_action_codes(
-    action: xml.etree.ElementTree, dict_code: xml.etree.ElementTree
-) -> xml.etree.ElementTree:
+    action: defusedxml.ElementTree.XML, dict_code: defusedxml.ElementTree
+) -> defusedxml.ElementTree:
     # #######################################################################################
     # Update dictionary entry for this code in the format of an output line
     # dict = { 'the_code':
     #               {num_args: num,
     #                args: arg0, arg1, ... type: Int/Str  }
     # #######################################################################################
     arg_list, type_list, arg_nums = get_action.get_args(action, ignore_list)
@@ -53,16 +53,16 @@
     return
 
 
 # #######################################################################################
 # Build the dictionary for the Action code
 # #######################################################################################
 def build_new_action_codes(
-    action: xml.etree.ElementTree, dict_code: xml.etree.ElementTree
-) -> xml.etree.ElementTree:
+    action: defusedxml.ElementTree.XML, dict_code: defusedxml.ElementTree
+) -> defusedxml.ElementTree:
     logger.info(f"...for {dict_code}")
 
     # #######################################################################################
     # Create a dictionary entry for this code in the format of an output line
     # dict = { 'the_code':
     #               {num_args: num, args: ['arg0', 'arg1', ...], types: ['Str', 'Int', ...]
     # #######################################################################################
@@ -79,19 +79,19 @@
 # #######################################################################################
 # Build the dictionary for each Action code
 # child = pointer to <code> xml
 # action = pointer to root xml (<Action> or <Profile>)
 # adder = empty if <action>.  Else it is a Profile condition, and we need to make key unique
 # #######################################################################################
 def build_action_codes(
-    child: xml.etree.ElementTree,
-    action: xml.etree.ElementTree,
-    adder: xml.etree.ElementTree,
-    program_args: xml.etree.ElementTree,
-) -> xml.etree.ElementTree:
+    child: defusedxml.ElementTree.XML,
+    action: defusedxml.ElementTree.XML,
+    adder: defusedxml.ElementTree.XML,
+    program_args: defusedxml.ElementTree.XML,
+) -> defusedxml.ElementTree:
     #  multiplier = 10 if adder else 1
     dict_code = child.text + adder
     if (
         dict_code not in action_codes
     ):  # We have a code that is not yet in the dictionary?
         build_new_action_codes(action, dict_code)
         logger.debug(f"build_new_action_codes: {dict_code} ", action_codes[dict_code])
@@ -102,29 +102,29 @@
     return
 
 
 # ####################################################################################################
 # See if the display name is already in our Action dictionary.  If not, add it.
 # ####################################################################################################
 def add_name_to_action_codes(
-    dict_code: xml.etree.ElementTree, display_name: xml.etree.ElementTree
-) -> xml.etree.ElementTree:
+    dict_code: defusedxml.ElementTree.XML, display_name: defusedxml.ElementTree
+) -> defusedxml.ElementTree:
     if dict_code not in action_codes:
         build_new_action_codes("", dict_code)
     if display_name not in action_codes[dict_code]:
         action_codes[dict_code]["display"] = display_name
     return
 
 
 # ####################################################################################################
 # Trundle through ConditionList "If" conditions
 # Return the list of conditions and list of associated booleans
 # ####################################################################################################
 def process_condition_list(
-    code_action: xml.etree.ElementTree.Element,
+    code_action: defusedxml.ElementTree.XML,
 ) -> tuple[list[list[Any]], list[str]]:
     condition_list, boolean_list = [], []
     condition_list_str = code_action.find("ConditionList")
     if condition_list_str is not None:
         for child in condition_list_str:
             if "bool" in child.tag:
                 operation = child.text.upper()
```

### Comparing `maptasker-1.3.2/maptasker/src/actione.py` & `maptasker-1.3.3/maptasker/src/actione.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 #          code_child: used to parse the specific <code> xml for action details.                                     #
 #          code_action: the nnn in <code>nnn</code> xml                                                              #
 #          action_type: true if Task action, False if not (e.g. a Profile state or event condition)                  #
 #                                                                                                                    #
 ######################################################################################################################
 import copy
 import re
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 import maptasker.src.actionr as action_results
-from maptasker.src.config import CONTINUE_LIMIT
+
 from maptasker.src.action import get_extra_stuff
+from maptasker.src.frmthtml import format_html
 from maptasker.src.actionc import action_codes
 from maptasker.src.sysconst import logger
 from maptasker.src.sysconst import FONT_TO_USE
 
 pattern = re.compile(r",[, ]+")
+
+
 # pattern1 = re.compile(r'<.*?>')  # Get rid of all <something> html code
 
 
 # ####################################################################################################
 # Delete crap that might be in the label
 # ####################################################################################################
 def cleanup_the_result(results):
@@ -85,16 +88,16 @@
     return
 
 
 # ####################################################################################################
 # Given an action code, evaluate it for display
 # ####################################################################################################
 def get_action_code(
-    code_child: xml.etree.ElementTree,
-    code_action: xml.etree.ElementTree,
+    code_child: defusedxml.ElementTree.XML,
+    code_action: defusedxml.ElementTree.XML,
     action_type: bool,
     colormap: dict,
     code_type: str,
     program_args: dict,
 ) -> str:
     """
     Given an action code, evaluate it for display
@@ -116,22 +119,18 @@
             f"Code {dict_code} not yet"
             f" mapped{get_extra_stuff(code_action, action_type, colormap, program_args)}"
         )
         logger.debug(f"unmapped task code: {dict_code} ")
 
     else:
         # The code is in our dictionary.  Add the display name
-        the_result = (
-            '<span style="color:'
-            + colormap["action_name_color"]
-            + program_args["font_to_use"]
-            + '>'
-            + action_codes[dict_code]["display"]
-            + "</span>"
-        )  # Just get the basics for now
+        the_result = format_html(
+            colormap, "action_name_color", "", action_codes[dict_code]["display"], True
+        )
+
         if "numargs" in action_codes[dict_code]:
             numargs = action_codes[dict_code]["numargs"]
         else:
             numargs = 0
         # If there are required args, then parse them
         if numargs != 0 and "reqargs" in action_codes[dict_code]:
             the_result = action_results.get_action_results(
@@ -170,20 +169,21 @@
     the_result = cleanup_the_result(the_result)
     return the_result
 
 
 # #############################################################################################
 # Construct Task Action output line
 # #############################################################################################
-def build_action(alist, tcode, code_element, indent, indent_amt):
+def build_action(colormap, alist, tcode, code_element, indent, indent_amt):
+    from maptasker.src.config import CONTINUE_LIMIT
+
     # Calculate total indentation to put in front of action
     count = indent
     if count != 0:
-        tcode = tcode.replace(f"{FONT_TO_USE}>", f"{FONT_TO_USE}>{indent_amt}", 1)
-        # tcode = indent_amt + tcode
+        tcode = tcode.replace(f'{FONT_TO_USE}">', f'{FONT_TO_USE}">{indent_amt}', 1)
         count = 0
     if count < 0:
         tcode = indent_amt + tcode
 
     # Break-up very long actions at new line
     if tcode != "":
         newline = tcode.find("\n")  # Break-up new line breaks
@@ -197,19 +197,26 @@
             count = 0
             for item in array_of_lines:
                 if count == 0:
                     alist.append(item)
                 else:
                     alist.append(f"...{item}")
                 count += 1
-                if (
-                    count == CONTINUE_LIMIT
-                ):  # Only display up to so many continued lines
+                # Only display up to so many continued lines
+                if count == CONTINUE_LIMIT:
                     alist.append(
-                        '<span style="color:red"> ... continue limit of'
-                        f' {str(CONTINUE_LIMIT)} reached.  See "CONTINUE_LIMIT =" in'
-                        ' code for details</span>'
+                        format_html(
+                            colormap,
+                            "Red",
+                            "",
+                            (
+                                f' ... continue limit of {str(CONTINUE_LIMIT)} '
+                                'reached.  See "CONTINUE_LIMIT =" in config.py for '
+                                'details'
+                            ),
+                            True,
+                        )
                     )
                     break
     else:
         alist.append(f"Action {code_element.text}: not yet mapped")
     return
```

### Comparing `maptasker-1.3.2/maptasker/src/actionr.py` & `maptasker-1.3.3/maptasker/src/actionr.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 # ########################################################################################## #
 import sys
-import xml.etree.ElementTree  # Need for type hints
 from collections import defaultdict
 
+import defusedxml.ElementTree  # Need for type hints
+
 import maptasker.src.action as get_action
 from maptasker.src.actargs import action_args
 from maptasker.src.actionc import action_codes
+from maptasker.src.frmthtml import format_html
 from maptasker.src.sysconst import logger
 from maptasker.src.xmldata import get_xml_int_argument_to_value
 from maptasker.src.xmldata import get_xml_str_argument_to_value
 
 
 # ####################################################################################################
 # Given a list of positional items, return a string in the correct order based on position
@@ -66,17 +68,17 @@
 
 
 # ####################################################################################################
 # For the given code, save the display_name, required arg list and associated type list in dictionary
 # Then evaluate the data against the master dictionary of actions
 # ####################################################################################################
 def evaluate_action_args(
-    dict_code: xml.etree.ElementTree,
+    dict_code: defusedxml.ElementTree.XML,
     arg_list: list,
-    code_action: xml.etree.ElementTree,
+    code_action: defusedxml.ElementTree.XML,
     action_type: bool,
     colormap: dict,
     program_args: dict,
     lookup_code_entry: dict,
     evaluate_list: list,
     evaluated_results: dict,
 ) -> tuple:
@@ -108,43 +110,27 @@
 
 # ####################################################################################################
 # For the given code, save the display_name, required arg list and associated type list in dictionary
 # Then evaluate the data against the master dictionary of actions
 # ####################################################################################################
 def get_action_results(
     dict_code: str,
-    lookup_code_entry: xml.etree.ElementTree,
-    code_action: xml.etree.ElementTree,
+    lookup_code_entry: defusedxml.ElementTree.XML,
+    code_action: defusedxml.ElementTree.XML,
     action_type: bool,
-    colormap: xml.etree.ElementTree,
+    colormap: defusedxml.ElementTree.XML,
     arg_list: list[str],
     evaluate_list: list[str],
-    program_args: xml.etree.ElementTree,
+    program_args: defusedxml.ElementTree.XML,
 ) -> str:
     evaluated_results = defaultdict(
         lambda: []
     )  # Setup default dictionary as empty list
     two_blanks = "&nbsp;&nbsp;"
     result = ""
-    if "s" in dict_code or "e" in dict_code:  # Condition (State/Event)?
-        display_name_color = ""
-        display_detail_color = ""
-    else:  # We have a Task
-        display_name_color = (
-            '<span style="color:'
-            + colormap["action_name_color"]
-            + program_args["font_to_use"]
-            + '>'
-        )
-        display_detail_color = (
-            '</span><span style="color:'
-            + colormap["action_color"]
-            + program_args["font_to_use"]
-            + '>'
-        )
 
     # Save the associated data
     # action_codes[dict_code]['display'] = display_name
     lookup_code_entry[dict_code]["reqargs"] = arg_list
     lookup_code_entry[dict_code]["evalargs"] = evaluate_list
     # If just displaying action names or there are no action details, then just display the name
     if arg_list and program_args["display_detail_level"] != 2:
@@ -156,20 +142,25 @@
             action_type,
             colormap,
             program_args,
             lookup_code_entry,
             evaluate_list,
             evaluated_results,
         )
-    # Evaluate the required args
 
     # If we have results from evaluation, then go put them in their appropriate order
     if evaluated_results["returning_something"]:
         result = get_results_in_arg_order(evaluated_results)
-    return (
-        display_name_color
-        + action_codes[dict_code]["display"]
-        + display_detail_color
-        + two_blanks
-        + result
-        + get_action.get_extra_stuff(code_action, action_type, colormap, program_args)
+
+    # Return the properly formatted HTML with the Action name and extra stuff
+    return format_html(
+        colormap, "action_name_color", "", action_codes[dict_code]["display"], True
+    ) + format_html(
+        colormap,
+        "action_color",
+        "",
+        (
+            f"{two_blanks}{result}</span>"
+            f"{get_action.get_extra_stuff(code_action, action_type, colormap, program_args)}"
+        ),
+        False,
     )
```

### Comparing `maptasker-1.3.2/maptasker/src/actiont.py` & `maptasker-1.3.3/maptasker/src/actiont.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/caveats.py` & `maptasker-1.3.3/maptasker/src/caveats.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,59 +8,56 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 import maptasker.src.outputl as build_output
+from maptasker.src.frmthtml import format_html
 
 
 def display_caveats(output_list: list[str], program_args: dict, colormap: dict) -> None:
     """output the program caveats
     Output the program caveats at the very end
         Parameters: list into which all output has been added, the program runtime arguments,
                     the dictionary of colors to use
 
         Returns: the count of the number of times the program has been called
 
     """
-    caveat1 = (
-        f'<span style="color:{colormap["trailing_comments_color"]}'
-        + program_args["font_to_use"]
-        + ">CAVEATS:\n"
-    )
+    caveat1 = format_html(colormap, "trailing_comments_color", "", "CAVEATS:\n", False)
     caveat3 = (
         "- This has only been tested on my own backup.xml file."
         "  For problems, report them on https://github.com/mctinker/Map-Tasker."
     )
     caveat4 = (
         '- Tasks that are identified as "Unnamed/Anonymous" have no name and are'
         ' considered Anonymous.\n'
     )
     caveat6 = (
-        '- Tasker fields that have embedded HTML (e.g. color=...>") will result in the'
-        ' remaining label displayed in that same color/font.'
+        '- All attempts are made to retain embedded HTML (e.g. color=...>") in Tasker'
+        ' fields, but is stripped out of Action labels and TaskerNet comments.'
     )
     build_output.my_output(colormap, program_args, output_list, 0, "<hr>")  # line
     build_output.my_output(colormap, program_args, output_list, 4, caveat1)  # caveat
     if program_args["display_detail_level"] > 0:  # Caveat about Actions
         caveat2 = (
             "- Most but not all Task actions have been mapped and will display as such."
-            "  Likewise for Profile conditions and Plug-ins.\n</span>"
+            "  Likewise for Profile conditions and Plug-ins.\n"
         )
         build_output.my_output(
             colormap, program_args, output_list, 4, caveat2
         )  # caveat
     build_output.my_output(colormap, program_args, output_list, 4, caveat3)  # caveat
     build_output.my_output(colormap, program_args, output_list, 4, caveat4)  # caveat
     if (
         program_args["display_detail_level"] == 0
-    ):  # Caveat about -d0 option and 1sat Action for unnamed Tasks
+    ):  # Caveat about -d0 option and 1st Action for unnamed Tasks
         caveat5 = (
             '- For option -d0, Tasks that are identified as "Unnamed/Anonymous" will'
-            ' have their first Task only listed....\n  just like Tasker does.\n'
+            ' have their first Action only listed....\n  just like Tasker does.\n'
         )
         build_output.my_output(
             colormap, program_args, output_list, 4, caveat5
         )  # caveat
-    build_output.my_output(colormap, program_args, output_list, 4, caveat6)  # caveat
+    build_output.my_output(colormap, program_args, output_list, 4, f"{caveat6}</span>")
     return
```

### Comparing `maptasker-1.3.2/maptasker/src/colors.py` & `maptasker-1.3.3/maptasker/src/colors.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/colrmode.py` & `maptasker-1.3.3/maptasker/src/colrmode.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             "profile_color": "Aqua",
             "disabled_profile_color": "Red",
             "launcher_task_color": "GreenYellow",
             "task_color": "Yellow",
             "unknown_task_color": "Red",
             "scene_color": "Lime",
             "bullet_color": "White",
-            "action_name_color": "PaleGoldenrod",
+            "action_name_color": "Gold",
             "action_color": "DarkOrange",
             "action_label_color": "Magenta",
             "action_condition_color": "PapayaWhip",
             "disabled_action_color": "Crimson",
             "profile_condition_color": "Lavender",
             "background_color": "DarkBlue",
             "trailing_comments_color": "PeachPuff",
```

### Comparing `maptasker-1.3.2/maptasker/src/condition.py` & `maptasker-1.3.3/maptasker/src/condition.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/config.py` & `maptasker-1.3.3/maptasker/src/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import logging
 
 # Add the following statement to your Terminal Shell configuration file (BASH, Fish, etc.
 #  to eliminate the runtime msg: DEPRECATION WARNING: The system version of Tk is deprecated and may be removed...
 #  'export TK_SILENCE_DEPRECATION = 1' (without quotes)
 
 
 # ####################################################################################################
```

### Comparing `maptasker-1.3.2/maptasker/src/debug.py` & `maptasker-1.3.3/maptasker/src/debug.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,61 +9,63 @@
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 import sys
 import maptasker.src.outputl as build_output
-
-debug_style = '<span style="color:White;font-family:Courier">'
+from maptasker.src.frmthtml import format_html
 
 
 def debug1(colormap: dict, program_args: dict, output_list: list) -> None:
     """
     Output our runtime arguments
         :param colormap: colors to use
         :param program_args: other runtime arguments
         :param output_list: where the output goes
     """
     build_output.my_output(
         colormap,
         program_args,
         output_list,
         4,
-        f'{debug_style}sys.argv:{str(sys.argv)}</span>',
+        format_html(colormap, "White", "", f"sys.argv:{str(sys.argv)}", True),
     )
+    # )
     build_output.my_output(
         colormap,
         program_args,
         output_list,
         4,
         '',
     )
     for key, value in program_args.items():
         build_output.my_output(
             colormap,
             program_args,
             output_list,
             4,
-            f"{debug_style}{key}: {value}</span>",
+            format_html(colormap, "White", "", f"{key}: {value}", True),
         )
     build_output.my_output(
         colormap,
         program_args,
         output_list,
         4,
         '',
     )
     for key, value in colormap.items():
         build_output.my_output(
             colormap,
             program_args,
             output_list,
             4,
-            f"{debug_style}colormap for {key} set to {value}</span>",
+            format_html(
+                colormap, "White", "", f"colormap for {key} set to {value}", True
+            ),
         )
     build_output.my_output(
         colormap,
         program_args,
         output_list,
         4,
         '',
```

### Comparing `maptasker-1.3.2/maptasker/src/getids.py` & `maptasker-1.3.3/maptasker/src/getids.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 from maptasker.src.outputl import my_output
-from maptasker.src.sysconst import NO_PROFILE
-import xml.etree.ElementTree  # Need for type hints
+
+import defusedxml.ElementTree  # Need for type hints
 
 
 def get_ids(
     doing_project: bool,
     program_args: dict,
     colormap: dict,
     output_list: list,
-    project: xml.etree,
+    project: defusedxml.ElementTree.XML,
     project_name: str,
     projects_without_profiles: list,
 ) -> list:
     """
     Find either Project 'pids' (Profile IDs) or 'tids' (Task IDs)
     :param doing_project: True if this is searching for Project IDs
     :param program_args: runtime arguments
@@ -43,12 +43,12 @@
         ids_to_find = 'pids'
         my_output(colormap, program_args, output_list, 1, "")  # Start Profile list
     else:
         ids_to_find = 'tids'
     try:
         # Get a list of the Profiles for this Project
         project_pids = project.find(ids_to_find).text
-    except Exception:  # Project has no Profiles
+    except AttributeError:  # Project has no Profiles
         if project_name not in projects_without_profiles:
             projects_without_profiles.append(project_name)
 
     return project_pids.split(",") if project_pids != "" else []
```

### Comparing `maptasker-1.3.2/maptasker/src/getputarg.py` & `maptasker-1.3.3/maptasker/src/getputarg.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,38 +7,58 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import pickle
-from pathlib import Path
+import json
 
 from maptasker.src.sysconst import ARGUMENTS_FILE
 from maptasker.src.sysconst import logger
+from pathlib import Path
 
 
 # #######################################################################################
-# Save program arguments
+# Save and restore colors to use and program arguments
 # #######################################################################################
-def save_restore_args(to_save, colormap, temp_args):
-    dir_path = Path.cwd()
+def save_restore_args(
+    to_save: bool, colormap: dict, temp_args: dict
+) -> tuple[dict, dict]:
+    """
+    Save and restore colors to use and program arguments
+        :param to_save: True if we are to save the info, False to restore the info
+        :param colormap: colors to use in output
+        :param temp_args: runtime arguments
+        :return: colors and runtime arguments saved/restored
+    """
+    the_file = f"{Path.cwd()}/{ARGUMENTS_FILE}"
     if to_save:
         # Save dictionaries
-        with open(f"{dir_path}/{ARGUMENTS_FILE}", "wb") as f:
-            pickle.dump(colormap, f)
-            pickle.dump(temp_args, f)
-
+        list_to_save = [colormap, temp_args]
+        with open(the_file, "w") as f:
+            json.dump(list_to_save, f)
+            f.close()
     else:
         # Restore dictionaries
         try:
-            with open(f"{dir_path}/{ARGUMENTS_FILE}", "rb") as f:
-                colormap = pickle.load(f)
-                temp_args = pickle.load(f)
-        except Exception as e:  # no saved file
-            error_msg = "'-r' Error: There are no saved items found to restore!"
+            with open(the_file, "r") as f:
+                list_to_restore = json.load(f)
+                colormap = list_to_restore[0]
+                temp_args = list_to_restore[1]
+                f.close()
+        # Handle file not found condition
+        except OSError:
+            error_msg = "'-r' Error: No settings file found to restore!"
+            print(error_msg)
+            logger.debug(error_msg)
+            temp_args = colormap = {"msg": "No settings file found to restore!"}
+        # Handle file format error
+        except json.decoder.JSONDecodeError:  # no saved file
+            error_msg = f"'-r' Error: The settings file,  {ARGUMENTS_FILE} is corrupt!"
             print(error_msg)
             logger.debug(error_msg)
-            temp_args, colormap = {}, {}
+            temp_args = colormap = {
+                "msg": "The settings file is corrupt!  Re-save your settings."
+            }
 
     return temp_args, colormap
```

### Comparing `maptasker-1.3.2/maptasker/src/initparg.py` & `maptasker-1.3.3/maptasker/src/initparg.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/kidapp.py` & `maptasker-1.3.3/maptasker/src/kidapp.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 
-def get_kid_app(element: xml.etree) -> str:
+def get_kid_app(element: defusedxml.ElementTree) -> str:
     """
-Get any associated Kid Application info and return it
-    :param element: root element to search for <Kid>
-    :return: the Kid App info
+    Get any associated Kid Application info and return it
+        :param element: root element to search for <Kid>
+        :return: the Kid App info
     """
     kid_package = kid_version = kid_features = kid_plugins = ""
     four_spaces = "&nbsp;&nbsp;&nbsp;&nbsp;"
     kid_element = element.find("Kid")
     if kid_element is None:
         return ""
 
@@ -39,8 +39,12 @@
             kid_plugins = f" {kid_plugins}{num_plugin+1}={item.text}, "
             num_plugin += 1
     if kid_features:
         kid_features = f"<br>{four_spaces}Features:{kid_features[:len(kid_features)-2]}"
     if kid_plugins:
         kid_plugins = f"<br>{four_spaces}Plugins:{kid_plugins[:len(kid_plugins)-2]}"
 
-    return f'<br>&nbsp;&nbsp;&nbsp;[Kid App: Package:{kid_package}, Version Name:{kid_version}, Target Android Version:{kid_target} {kid_features} {kid_plugins}]'
+    return (
+        f'<br>&nbsp;&nbsp;&nbsp;[Kid App: Package:{kid_package}, Version'
+        f' Name:{kid_version}, Target Android'
+        f' Version:{kid_target} {kid_features} {kid_plugins}]'
+    )
```

### Comparing `maptasker-1.3.2/maptasker/src/mapit.py` & `maptasker-1.3.3/maptasker/src/mapit.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,39 +28,40 @@
 #                                                                                            #
 # Reference: https://github.com/Taskomater/Tasker-XML-Info                                   #
 #                                                                                            #
 # ########################################################################################## #
 
 import sys
 import webbrowser  # To be removed in Python 10.13 (2023?)
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 from os import getcwd
 from typing import List, Dict
 
 import maptasker.src.outputl as build_output
 import maptasker.src.proginit as initialize
 import maptasker.src.projects as projects
 import maptasker.src.taskuniq as special_tasks
 from maptasker.src.caveats import display_caveats
 from maptasker.src.prefers import get_preferences
 from maptasker.src.sysconst import logger
 
+
 # import os
 # print('Path:', os.getcwd())
 # print('__file__={0:<35} | __name__={1:<25} | __package__={2:<25}'.format(__file__,__name__,str(__package__)))
 
 
 # #######################################################################################
 # Clean up our memory hogs
 # #######################################################################################
 def clean_up_memory(
-    tree: xml.etree.ElementTree.ElementTree,
-    root: xml.etree.ElementTree.Element,
+    tree: defusedxml.ElementTree.XML,
+    root: defusedxml.ElementTree.XML,
     output_list: List[str],
-    all_tasker_items: Dict[str, List[xml.etree.ElementTree.Element]],
+    all_tasker_items: Dict[str, List[defusedxml.ElementTree.XML]],
 ) -> None:
     """
     Clean up our memory hogs
         :param tree: xml tree to empty
         :param root: root xml that was parsed from backup file
         :param output_list: list of output lines to clear
         :param all_tasker_items: All Projects/Profiles/Tasks/Scenes
@@ -103,27 +104,29 @@
                     + action_number
                     + ":"
                     + item[action_position + 8 + len(action_number) :]
                 )
                 output_line = temp
             else:
                 output_line = item
+            output_line = output_line.replace("</span></span>", "</span>")
+            output_line = output_line.replace("</p></p>", "</p>")
             out_file.write(output_line)
     logger.info("Function Exit: write_out_the_file")
     return
 
 
 # ###############################################################################################
 # Cleanup memory and let user know there was no match found for Task/Profile
 # ###############################################################################################
 def clean_up_and_exit(
     name: str,
     profile_or_task_name: str,
-    tree: xml.etree,
-    root: xml.etree,
+    tree: defusedxml.ElementTree.XML,
+    root: defusedxml.ElementTree.XML,
     output_list: list,
     all_tasker_items: dict,
 ) -> None:
     """
     Cleanup memory and let user know there was no match found for Task/Profile
         :param name: the name to add to the log/print output
         :param profile_or_task_name: name of the Profile or Task to clean
@@ -209,15 +212,14 @@
         tree,
         root,
         filename,
         all_tasker_items,
     ) = initialize.start_up(output_list)
 
     # Development only parameters here:
-    # program_args["debug"] = True
     # program_args["display_detail_level"] = 3
     # program_args["display_profile_conditions"] = True
     # program_args['display_preferences'] = True
     # program_args['display_taskernet'] = True
 
     #######################################################################################
     # Process Tasker Preferences
@@ -347,15 +349,15 @@
     clean_up_memory(tree, root, output_list, all_tasker_items)
 
     # Display final output
     logger.debug("MapTasker program ended normally")
     my_rc = 0
     try:
         webbrowser.open(f"file://{my_output_dir}{my_file_name}", new=2)
-    except Exception as e:
+    except webbrowser.Error:
         error_msg = (
             "Error: Failed to open output in browser: your browser is not supported."
         )
         print(error_msg)
         logger.debug(error_msg)
         my_rc = 1
     print("You can find 'MapTasker.html' in the current folder.  Program end.")
```

### Comparing `maptasker-1.3.2/maptasker/src/outputl.py` & `maptasker-1.3.3/maptasker/src/outputl.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 import maptasker.src.actione as action_evaluate
 from maptasker.src.debug import debug1
+from maptasker.src.frmthtml import format_html
 from maptasker.src.sysconst import FONT_TO_USE
 from maptasker.src.sysconst import UNKNOWN_TASK_NAME
 from maptasker.src.sysconst import debug_out
 from maptasker.src.sysconst import logger
 
 
 # #######################################################################################
@@ -32,23 +33,44 @@
     profile_name: str,
     heading: str,
     colormap: dict,
     program_args: dict,
 ) -> None:
     output_list.clear()
 
+    # Output the heading
     my_output(colormap, program_args, output_list, 0, FONT_TO_USE + heading)
     # If debugging, put out our runtime arguments first
     if program_args["debug"]:
         debug1(colormap, program_args, output_list)
-    my_output(colormap, program_args, output_list, 1, "")  # Start Project list
-    my_output(colormap, program_args, output_list, 2, f"Project: {project_name}")
+
+    # Start the Project list (<ul>)
+    my_output(colormap, program_args, output_list, 1, "")
+    # Output the Project name as list item (<li>)
+    my_output(
+        colormap,
+        program_args,
+        output_list,
+        2,
+        format_html(colormap, "project_color", "", f"Project: {project_name}", True),
+    )
+
+    # Are we to include the Profile?
     if include_the_profile:
-        my_output(colormap, program_args, output_list, 1, "")  # Start Profile list
-        my_output(colormap, program_args, output_list, 2, f"Profile: {profile_name}")
+        # Start Profile list
+        my_output(colormap, program_args, output_list, 1, "")
+        my_output(
+            colormap,
+            program_args,
+            output_list,
+            2,
+            format_html(
+                colormap, "profile_color", "", f"Profile: {profile_name}", True
+            ),
+        )
         my_output(colormap, program_args, output_list, 1, "")  # Start Project list
     return
 
 
 # #############################################################################################
 # Generate an updated output line with HTML style details
 # Input is a dictionary containing the requirements:
@@ -58,62 +80,50 @@
 #  is_list - boolean: True= is a list HTML element
 #  span - boolean: True= requires a <span> element
 #  font - font to use
 # #############################################################################################
 def put_style(style_details: dict) -> str:
     """
     Add appropriate HTML style tags based on parameters in dictionary passed in
-        :param style_details: dictionary
+        :param style_details: True if we are to output a list (<li>), False if not
         :return: updated output line with style details added
     """
     line_with_style = ""
     if style_details["is_list"]:
         line_with_style = (
             f'<li style="color:{style_details["color1"]}"><span style="color:'
-            f'{style_details["color2"]}{style_details["font"]}>'
+            f'{style_details["color2"]}{style_details["font"]}">'
             f'{style_details["element"]}</span></li>\n'
         )
 
     elif style_details["is_taskernet"]:
         line_with_style = (
-            '<p style="margin-left:20px;margin-right:50px;"><p style="color:'
-            f'{style_details["color2"]}{FONT_TO_USE}>'
+            '<p style="margin-left:20px;margin-right:50px;color:'
+            f'{style_details["color2"]}{FONT_TO_USE}">'
             f'{style_details["element"]}</p>\n'
             f'<p style="color:{style_details["color1"]}">'
         )
         line_with_style = line_with_style.replace("<span></span>", "")
 
     return line_with_style
 
 
 # #############################################################################################
 # Generate the output string based on the input XML <code> passed in
 # Returns a formatted string for output based on the input codes
 # #############################################################################################
-def ulify_list_item(element: xml.etree, colormap: dict, font_to_use: str) -> str:
-    if element[:7] == "Project":  # Project ========================
-        return put_style(
-            style_details={
-                "is_list": True,
-                "color1": colormap['bullet_color'],
-                "color2": colormap["project_color"],
-                "font": font_to_use,
-                "element": element,
-            }
-        )
-    elif element[:7] == "Profile":  # Profile ========================
-        return put_style(
-            style_details={
-                "is_list": True,
-                "color1": colormap['bullet_color'],
-                "color2": colormap["profile_color"],
-                "font": font_to_use,
-                "element": element,
-            }
-        )
+def ulify_list_item(
+    element: defusedxml.ElementTree.XML, colormap: dict, font_to_use: str
+) -> str:
+    if (
+        f'{font_to_use}">Project:' in element or "Project has no Profiles" in element
+    ):  # Project ========================
+        return f'<li style=color:{colormap["bullet_color"]}>{element}</span></li>\n'
+    elif f'{font_to_use}">Profile:' in element:  # Profile ========================
+        return f'<li style=color:{colormap["bullet_color"]}>{element}</span></li>\n'
     elif (
         element[:5] == "Task:" or "&#45;&#45;Task:" in element
     ):  # Task or Scene's Task ========================
         return (
             put_style(
                 style_details={
                     "is_list": True,
@@ -150,46 +160,28 @@
         ):  # If this is continued from the previous line, indicate so and ensure proper font
             if element[11:] == "":
                 return ""
             tmp = action_evaluate.cleanup_the_result(
                 element.replace("Action: ...", "&nbsp;&nbsp;continued >>> ")
             )
             element = tmp
-        return put_style(
-            style_details={
-                "is_list": True,
-                "color1": colormap['bullet_color'],
-                "color2": colormap["action_color"],
-                "font": font_to_use,
-                "element": element,
-            }
-        )
-    elif "Label for" in element:  # Label
-        return put_style(
-            style_details={
-                "is_list": True,
-                "color1": colormap['bullet_color'],
-                "color2": colormap["action_label_color"],
-                "font": font_to_use,
-                "element": element,
-            }
-        )
+        return f'<li style=color:{colormap["bullet_color"]}>{element}</span></li>\n'
     elif "TaskerNet " in element:  # TaskerNet
         return put_style(
             style_details={
                 "is_list": False,
                 "color1": colormap['bullet_color'],
                 "color2": colormap["taskernet_color"],
                 "font": font_to_use,
                 "element": element,
                 "is_taskernet": True,
             }
         )
     else:  # Must be additional item
-        return f"<li {element}" + "</li>\n"
+        return f"<li {element}" + "</span></li>\n"
 
 
 # #############################################################################################
 # Generate the output string based on the input XML <code> passed in
 # Returns a formatted string for output based on the input codes
 # #############################################################################################
 def ulify(element, lvl, colormap, font_to_use):
@@ -212,15 +204,30 @@
             string = element + "<br>\n"
     return string
 
 
 # #############################################################################################
 # Write line of output
 # #############################################################################################
-def my_output(colormap, program_args, output_list, list_level, out_string):
+def my_output(
+    colormap: dict,
+    program_args: dict,
+    output_list: list,
+    list_level: int,
+    out_string: str,
+) -> None:
+    """
+    Add line to the list of output lines
+        :param colormap: colors to use in the output
+        :param program_args: runtime arguments
+        :param output_list: list of all output lines thus far
+        :param list_level: level we are outputting
+        :param out_string: the string to add to the output
+        :return: none
+    """
     if (
         "Task ID:" in out_string and program_args["debug"] is False
     ):  # Drop ID: nnn since we don't need it anymore
         temp_element = out_string.split("Task ID:")
         out_string = temp_element[0]
     output_list.append(
         ulify(out_string, list_level, colormap, program_args["font_to_use"])
```

### Comparing `maptasker-1.3.2/maptasker/src/parsearg.py` & `maptasker-1.3.3/maptasker/src/parsearg.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/prefers.py` & `maptasker-1.3.3/maptasker/src/prefers.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,31 +12,29 @@
 #                                                                                            #
 # ########################################################################################## #
 import gc
 import re
 from operator import itemgetter
 
 from maptasker.src.outputl import my_output
+from maptasker.src.frmthtml import format_html
 from maptasker.src.servicec import service_codes
-from maptasker.src.sysconst import FONT_TO_USE
 
 
 def process_service(
     colormap: dict, service_name: str, service_value: str, output_lines: list
 ) -> None:
     """
     We have a service xml element that we have mapped as a preference.  Process it.
         :param colormap: colors to use in output
         :param service_name: name of the preference in <Service xml
         :param service_value: value of the preference in <Service xml
         :param output_lines: accumulated output lines generated thus far (to append to)
     """
-    preferences_html = (
-        " <span style=\"color:" + colormap["preferences_color"] + FONT_TO_USE + '>'
-    )
+    preferences_html = format_html(colormap, "preferences_color", "", "", False)
     blank = "&nbsp;"
 
     # Get the name to display
     output_service_name = service_codes[service_name]["display"]
     # Left justify and fill to 15 characters
     output_service_name = output_service_name.ljust(45, '.')
 
@@ -55,20 +53,27 @@
         packages_end = [m.start() for m in re.finditer('}', service_value)]
         for number, position in enumerate(packages):
             package_names = (
                 f"{package_names}<br>{blank * 50}{service_value[position + 14:packages_end[number]]}"
             )
         service_value = package_names
 
-    # Add the output details to our list of output stuff
     output_lines.append(
         [
             service_codes[service_name]['num'],
             (
-                f"{preferences_html}{blank * 2}{output_service_name}{blank * 4}{service_value}</span>"
+                format_html(
+                    colormap,
+                    "preferences_color",
+                    "",
+                    (
+                        f"{preferences_html}{blank * 2}{output_service_name}{blank * 4}{service_value}"
+                    ),
+                    True,
+                )
             ),
         ]
     )
 
 
 def get_preferences(
     output_list: list, program_args: dict, colormap: dict, all_tasker_items: dict
@@ -94,29 +99,32 @@
         "Action",
         "Action > Reset Error Notifications",
         "Misc",
         "Misc > Debugging",
         "Unlisted (Perhaps Deprecated)",
     ]
     output_lines = []
-    preferences_html = (
-        ' <span style="color:' + colormap["preferences_color"] + FONT_TO_USE + '>'
-    )
+    preferences_html = format_html(colormap, "preferences_color", "", "", False)
     blank = "&nbsp;"
     first_time = True
 
     # Output title line
     my_output(
         colormap,
         program_args,
         output_list,
         4,
         (
-            f"{preferences_html}Tasker Preferences"
-            " >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>></span>"
+            format_html(
+                colormap,
+                "preferences_color",
+                "",
+                "Tasker Preferences >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>",
+                True,
+            )
         ),
     )
 
     # Go through each <Service xml element
     current_section = 999
     dummy_num = 100
     for service in all_tasker_items["all_services"]:
@@ -134,17 +142,23 @@
             if first_time:
                 first_time = False
                 output_lines.append([dummy_num, "<br>"])
             # Add the output details to our list of output stuff
             output_lines.append(
                 [
                     dummy_num,
-                    (
-                        f"{preferences_html}&nbsp;&nbsp;Not yet mapped:"
-                        f" {service_name}{blank * 4}type:{service_type}{blank * 4}value:{service_value}</span>"
+                    format_html(
+                        colormap,
+                        "preferences_color",
+                        "",
+                        (
+                            f"{blank * 2}Not yet"
+                            f" mapped:{service_name}{blank * 4}type:{service_type}{blank * 4}value:{service_value}"
+                        ),
+                        True,
                     ),
                 ]
             )
             dummy_num += 1
 
     # All service xml elements have been processed.
     # Sort our output by order of display in Tasker (key=list element 0)
@@ -159,17 +173,20 @@
             if item[1]["num"] == num and current_section != item[1]["section"]:
                 # Add the preference in the order it appears in Tasker
                 my_output(
                     colormap,
                     program_args,
                     output_list,
                     4,
-                    (
-                        f"<br>{preferences_html}&nbsp;Section:"
-                        f" {section_names[item[1]['section']]}</span>"
+                    format_html(
+                        colormap,
+                        "preferences_color",
+                        "",
+                        f"<br>&nbsp;Section: {section_names[item[1]['section']]}",
+                        True,
                     ),
                 )
                 current_section = item[1]["section"]
         my_output(colormap, program_args, output_list, 4, line[1])
 
     my_output(
         colormap,
```

### Comparing `maptasker-1.3.2/maptasker/src/priority.py` & `maptasker-1.3.3/maptasker/src/priority.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 
-def get_priority(element: xml.etree, event: bool) -> str:
+def get_priority(element: defusedxml.ElementTree.XML, event: bool) -> str:
     """
-Get any associated priority for the Task/Profile
-    :param element: root element to search for
-    :param event: True if this is for an 'Event' condition, False if not
-    :return: the priority or none
+    Get any associated priority for the Task/Profile
+        :param element: root element to search for
+        :param event: True if this is for an 'Event' condition, False if not
+        :return: the priority or none
     """
 
     priority_element = element.find("pri")
     if priority_element is None:
         return ""
     elif event:
-        return f'Priority:{priority_element.text}'
+        return f' Priority:{priority_element.text}'
     else:
         return f'<br>&nbsp;&nbsp;&nbsp;[Priority: {priority_element.text}]'
```

### Comparing `maptasker-1.3.2/maptasker/src/proclist.py` & `maptasker-1.3.3/maptasker/src/proclist.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 from maptasker.src.outputl import my_output
 
 from maptasker.src.taskactn import get_task_actions_and_output
 from maptasker.src.sysconst import logger
 from maptasker.src.sysconst import UNKNOWN_TASK_NAME
 
@@ -23,15 +23,15 @@
 # #######################################################################################
 # Process Task/Scene text/line item: call recursively for Tasks within Scenes
 # #######################################################################################
 def process_list(
     list_type: str,
     output_list: list,
     the_list: list,
-    the_task: xml.etree,
+    the_task: defusedxml.ElementTree.XML,
     tasks_found: list,
     program_args: dict,
     colormap: dict,
     all_tasker_items: dict,
 ) -> None:
     """
     Process Task/Scene text/line item: call recursively for Tasks within Scenes
```

### Comparing `maptasker-1.3.2/maptasker/src/profiles.py` & `maptasker-1.3.3/maptasker/src/profiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 import maptasker.src.condition as condition
 import maptasker.src.tasks as tasks
 
 # from maptasker.src.kidapp import get_kid_app
 from maptasker.src.outputl import my_output
 from maptasker.src.outputl import refresh_our_output
+from maptasker.src.frmthtml import format_html
+from maptasker.src.xmldata import remove_html_tags
 
 from maptasker.src.share import share
 from maptasker.src.sysconst import NO_PROFILE
 
 
 # #######################################################################################
 # Get a specific Profile's Tasks (maximum of two:entry and exit)
 # #######################################################################################
 def get_profile_tasks(
-    the_profile: xml.etree,
+    the_profile: defusedxml.ElementTree.XML,
     found_tasks_list: list,
     task_output_line: list,
     program_args: dict,
     all_tasks: dict,
     found_items: dict,
-) -> tuple[xml.etree, str]:
+) -> tuple[defusedxml.ElementTree.XML, str]:
     keys_we_dont_want = ["cdate", "edate", "flags", "id"]
     the_task_element, the_task_name = "", ""
 
     for child in the_profile:
         if child.tag in keys_we_dont_want:
             continue
         if "mid" in child.tag:
@@ -62,133 +64,129 @@
     return the_task_element, the_task_name
 
 
 # #######################################################################################
 # Get the Profile's key attributes: limit, launcher task, run conditions
 # #######################################################################################
 def build_profile_line(
-    project: xml.etree,
-    profile: xml.etree,
+    project: defusedxml.ElementTree.XML,
+    profile: defusedxml.ElementTree.XML,
     output_list: list,
     program_args: dict,
     colormap: dict,
-) -> tuple:
-    # Set up html to use
-    profile_color_html = (
-        '<span style="color:'
-        + colormap["profile_color"]
-        + program_args["font_to_use"]
-        + "></span>"
-    )
-    disabled_profile_html = (
-        '<span style="color:'
-        + colormap["disabled_profile_color"]
-        + program_args["font_to_use"]
-        + '>[DISABLED]</span>'
-    )
-    launcher_task_html = (
-        '  style="color:'
-        + colormap["launcher_task_color"]
-        + '"[Launcher Task]'
-        + profile_color_html
+) -> str:
+    """
+    Get the Profile's key attributes: limit, launcher task, run conditions and output it
+        :param project: the Project xml element
+        :param profile: the Profile xml element
+        :param output_list: the list of output lines built thus far
+        :param program_args: runtime arguments
+        :param colormap: colors to use in output
+        :return: Profile name
+    """
+    flags = condition_text = ""
+
+    # Set up HTML to use
+    disabled_profile_html = format_html(
+        colormap, "disabled_profile_color", "", "[DISABLED]", True
     )
-    condition_color_html = (
-        '<span style="color:'
-        + colormap["profile_condition_color"]
-        + program_args["font_to_use"]
-        + '>'
+    launcher_task_html = format_html(
+        colormap, "launcher_task_color", "", "[Launcher Task]", True
     )
-    profile_condition = ""
 
     # Look for disabled Profile
     limit = profile.find("limit")  # Is the Profile disabled?
     if limit is not None and limit.text == "true":
         disabled = disabled_profile_html
     else:
         disabled = ""
-    launcher_xml = project.find(
-        "ProfileVariable"
-    )  # Is there a Launcher Task with this Project?
+
+    # Is there a Launcher Task with this Project?
+    launcher_xml = project.find("ProfileVariable")
     launcher = launcher_task_html if launcher_xml is not None else ""
 
     # See if there is a Kid app and/or Priority (FOR FUTURE USE)
     # kid_app_info = ''
     # if program_args["display_detail_level"] == 3:
     #     kid_app_info = get_kid_app(profile)
     #     priority = get_priority(profile, False)
 
     # Display flags for debug mode
-    flags = ""
     if program_args["debug"]:
         flags = profile.find("flags")
         if flags is not None:
-            flags = (
-                f' <span style="color:GreenYellow{program_args["font_to_use"]}>flags:'
-                f' {flags.text}</span><span'
-                f' style="color:Red{program_args["font_to_use"]}>'
+            flags = format_html(
+                colormap, "GreenYellow", "", f" flags: {flags.text}", True
             )
+        else:
+            flags = ""
 
-    # Check for Profile 'conditions'
-    profile_name = ""
+    # Get the Profile's conditions
     if program_args["display_profile_conditions"]:
-        profile_condition = condition.parse_profile_condition(
+        if profile_conditions := condition.parse_profile_condition(
             profile, colormap, program_args
-        )  # Get the Profile's condition
-        if profile_condition:
-            profile_name = (
-                f"{condition_color_html} ({profile_condition})</span>"
-                f" {profile_name}{launcher}{disabled} {flags}</span>"
+        ):
+            # Strip pre-existing HTML from conmditions, since some condition codes may be same as Actions
+            # And the Actions would have plugged in the action_color HTML
+            profile_conditions = remove_html_tags(profile_conditions, "")
+            condition_text = format_html(
+                colormap,
+                "profile_condition_color",
+                "",
+                f" ({profile_conditions})",
+                True,
             )
 
-    # Start formulating the Profile output line
+    # Get the Profile name
     try:
-        profile_name = profile.find("nme").text + profile_name  # Get Profile's name
-    except Exception as e:  # no Profile name
-        if program_args["display_profile_conditions"]:
-            profile_condition = condition.parse_profile_condition(
-                profile, colormap, program_args
-            )  # Get the Profile's condition
-            profile_name = (
-                f"{NO_PROFILE}</span>{condition_color_html} ({profile_condition})</span>"
-                f" {profile_color_html}{launcher}{disabled}{flags}"
-                if profile_condition
-                else profile_name + NO_PROFILE + launcher + disabled
-            )
-        else:
-            profile_name = profile_name + NO_PROFILE + launcher + disabled
+        the_profile_name = profile.find("nme").text  # Get Profile's name
+    except AttributeError:  # no Profile name
+        the_profile_name = NO_PROFILE
+
+    # Add html color and font for Profile name
+    profile_name = format_html(
+        colormap, "profile_color", "", f"Profile: {the_profile_name} ", True
+    )
 
+    # If we are debugging, add the Profile ID
     if program_args["debug"]:
         profile_id = profile.find("id").text
-        profile_name = f"{profile_name} ID:{profile_id}"
+        profile_name = (
+            f'{profile_name} {format_html(colormap, "Yellow", "", f"ID:{profile_id}", True)}'
+        )
+
+    # Okay, string it all together
+    profile_name = f"{profile_name} {condition_text} {launcher}{disabled} {flags}"
+
     # Output the Profile line
     my_output(
         colormap,
         program_args,
         output_list,
         2,
-        f"Profile: {profile_name}",
+        profile_name,
     )
-    return limit, launcher, profile_condition, profile_name
+    return the_profile_name
 
 
 # #######################################################################################
 # process_projects: go through all Projects Profiles...and output them
 # #######################################################################################
 def process_profiles(
     output_list: list,
-    project: xml.etree,
+    project: defusedxml.ElementTree.XML,
     project_name: str,
     profile_ids: list,
     list_of_found_tasks: list,
     program_args: dict,
     heading: str,
     colormap: dict,
     all_tasker_items: dict,
     found_items: dict,
-) -> xml.etree:
+) -> defusedxml.ElementTree:
     """
     Go through Project's Profiles and output each
         :param output_list: list of each output line generated so far
         :param project: Project to process
         :param project_name: Project's name
         :param profile_ids: list of Profiles in Project
         :param list_of_found_tasks: list of Tasks found
@@ -209,38 +207,41 @@
         # Are we searching for a specific Profile?
         if program_args["single_profile_name"]:
             try:
                 profile_name = profile.find("nme").text
                 if program_args["single_profile_name"] != profile_name:
                     continue  # Not our Profile...go to next Profile ID
                 found_items["single_profile_found"] = True
+                # Clear the output list to prepare for single Profile only
                 refresh_our_output(
                     False,
                     output_list,
                     project_name,
                     "",
                     heading,
                     colormap,
                     program_args,
                 )
-            except Exception as e:  # no Profile name...go to next Profile ID
+                # Start Profile list
+                my_output(colormap, program_args, output_list, 1, "")
+            except AttributeError:  # no Profile name...go to next Profile ID
                 continue
+        # Get Task xml element and name
         task_list = []  # Profile's Tasks will be filled in here
-        task_output_line = ' '
         our_task_element, our_task_name = get_profile_tasks(
             profile,
             list_of_found_tasks,
             task_list,
             program_args,
             all_tasker_items["all_tasks"],
             found_items,
         )
 
         # Examine Profile attributes and output Profile line
-        limit, launcher, profile_condition, profile_name = build_profile_line(
+        profile_name = build_profile_line(
             project, profile, output_list, program_args, colormap
         )
 
         # Process any <Share> information from TaskerNet
         if program_args["display_taskernet"]:
             share(profile, colormap, program_args, output_list)
```

### Comparing `maptasker-1.3.2/maptasker/src/progargs.py` & `maptasker-1.3.3/maptasker/src/progargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/proginit.py` & `maptasker-1.3.3/maptasker/src/proginit.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,46 +9,42 @@
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 
 import atexit
-import contextlib
 import datetime
 import sys
 from json import dumps, loads  # For write and read counter
-from os import rename
 from pathlib import Path
 
 # importing tkinter and tkinter.ttk and all their functions and classes
 from tkinter import *
 from tkinter import messagebox
-import xml.etree.ElementTree  # Need for type hints
 
 # importing askopenfile (from class filedialog) and messagebox functions
 # from class filedialog
 from tkinter.filedialog import askopenfile
-from typing import Any, Tuple, Dict, List
-from xml.etree.ElementTree import ElementTree, Element
+from typing import Any
 
+import maptasker.src.migrate as old_to_new
 import maptasker.src.outputl as build_output
 import maptasker.src.progargs as get_args
-from maptasker.src.config import GUI
-
+from maptasker.src.frmthtml import format_html
+from maptasker.src.colrmode import set_color_mode
 from maptasker.src.config import DARK_MODE
+from maptasker.src.config import GUI
 from maptasker.src.debug import debug1
-from maptasker.src.sysconst import ARGUMENTS_FILE
 from maptasker.src.sysconst import COUNTER_FILE
 from maptasker.src.sysconst import FONT_TO_USE
 from maptasker.src.sysconst import MY_VERSION
 from maptasker.src.sysconst import logger
 from maptasker.src.sysconst import logging
 from maptasker.src.taskerd import get_the_xml_data
-from maptasker.src.colrmode import set_color_mode
 
 
 # #############################################################################################
 # Use a counter to determine if this is the first time run.
 #  If first time only, then provide a user prompt to locate the backup file
 # #############################################################################################
 def read_counter():
@@ -98,15 +94,15 @@
 
     # dir_path = path.dirname(path.realpath(__file__))  # Get current directory
     dir_path = Path.cwd()
     logger.info(f"dir_path: {dir_path}")
     if program_args["debug"]:
         try:
             filename = open(f"{dir_path}/backup.xml", "r")
-        except Exception:
+        except OSError:
             error_msg = (
                 f"Error: The backup.xml file was not found in {dir_path}.  Program"
                 " terminated!"
             )
             logger.debug(error_msg)
             print(error_msg)
             exit(3)
@@ -207,21 +203,25 @@
         sys.exit(3)
     else:
         # Format the output heading
         heading = (
             '<html>\n<head>\n<title>MapTasker</title>\n<body style="background-color:'
             + colormap["background_color"]
             + '">\n'
-            + '<span style="color:LawnGreen'
-            + FONT_TO_USE
-            + ">Tasker Mapping................"
-            "&nbsp;&nbsp;&nbsp;Tasker version:"
-            f" {root.attrib['tv']}"
-            "&nbsp;&nbsp;&nbsp;&nbsp;Map-Tasker version:"
-            f" {MY_VERSION}</span>"
+            + format_html(
+                colormap,
+                "LawnGreen",
+                "",
+                (
+                    "<b>Tasker Mapping................&nbsp;&nbsp;&nbsp;Tasker version:"
+                    f" {root.attrib['tv']}&nbsp;&nbsp;&nbsp;&nbsp;Map-Tasker version:"
+                    f" {MY_VERSION}</b>"
+                ),
+                True,
+            )
         )
         # Start the output with heading
         build_output.my_output(colormap, program_args, output_list, 0, heading)
 
     # If we are debugging, output the runtime arguments and colors
     if program_args["debug"]:
         debug1(colormap, program_args, output_list)
@@ -241,18 +241,18 @@
         :type output_list: tuple[
     """
     colormap = setup_colors()  # Get our map of colors
 
     # Get any arguments passed to program
     logger.info(f"sys.argv{str(sys.argv)}")
 
-    # Rename any old argument file to new name for clarity (one time only operation)
-    dir_path = Path.cwd()
-    with contextlib.suppress(FileNotFoundError):
-        rename(f"{dir_path}/.arguments.txt", f"{dir_path}/{ARGUMENTS_FILE}")
+    # Rename/convert any old argument file to new name/format for clarity (one time only operation)
+    old_to_new.migrate()
+
+    # Get runtime arguments
     program_args, colormap = get_args.get_program_arguments(colormap)
 
     # Setup program key elements
     tree, root, filename, all_tasker_items, output_list, heading = setup(
         colormap, program_args, output_list
     )
```

### Comparing `maptasker-1.3.2/maptasker/src/projects.py` & `maptasker-1.3.3/maptasker/src/projects.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
+import maptasker.src.tasks as tasks
+from maptasker.src.frmthtml import format_html
+from maptasker.src.getids import get_ids
+from maptasker.src.kidapp import get_kid_app
 from maptasker.src.outputl import my_output
 from maptasker.src.outputl import refresh_our_output
-from maptasker.src.profiles import process_profiles
-from maptasker.src.share import share
-from maptasker.src.kidapp import get_kid_app
 from maptasker.src.priority import get_priority
-from maptasker.src.getids import get_ids
+from maptasker.src.profiles import process_profiles
 from maptasker.src.scenes import process_project_scenes
-import maptasker.src.tasks as tasks
+from maptasker.src.share import share
 from maptasker.src.sysconst import NO_PROFILE
-from maptasker.src.sysconst import FONT_TO_USE
 
 
 # #######################################################################################
 # process_projects: go through all Projects Profiles...and output them
 # #######################################################################################
 def process_projects_and_their_profiles(
     output_list: list,
@@ -68,35 +68,32 @@
     my_output(colormap, program_args, output_list, 3, "")  # Close Project list
 
     # Return a list of Tasks found thus far with duplicates remove
     # Reference: https://www.pythonmorsels.com/deduplicate-lists/
     return list(dict.fromkeys(found_tasks).keys())
 
 
-def get_launcher_task(
-    project: xml.etree, colormap: dict, project_color_html: str
-) -> str:
+def get_launcher_task(project: defusedxml.ElementTree.XML, colormap: dict) -> str:
     """
     If Project has a launcher Task, get it
         :param project: xml element of Project we are processing
         :param colormap: colors to use in output
-        :param project_color_html: html to use that defines the color
         :return: information related to launcher Task
     """
     launcher_task_info = ""
     share_element = project.find("Share")
     if share_element is not None:
         launcher_task_element = share_element.find("t")
         if launcher_task_element is not None and launcher_task_element.text is not None:
-            launcher_task_info = (
-                '</span><span style="color:'
-                + colormap["launcher_task_color"]
-                + FONT_TO_USE
-                + f'>[Launcher Task: {launcher_task_element.text}]</span> '
-                + project_color_html
+            launcher_task_info = format_html(
+                colormap,
+                "launcher_task_color",
+                "",
+                f'[Launcher Task: {launcher_task_element.text}] ',
+                True,
             )
     return launcher_task_info
 
 
 # #############################################################################################
 # Process all Tasks in Project that are not referenced by a Profile
 # #############################################################################################
@@ -140,32 +137,36 @@
             # We have a Project's Task that has not yet been output
             our_task_element, our_task_name = tasks.get_task_name(
                 the_id, found_tasks, [], "", all_tasker_items['all_tasks']
             )
             # We have to remove this Task from found Tasks since it was added by get_task_name
             found_tasks.remove(the_id)
 
-            # Only print the Task header if there are Tasks not found in any Profile, and we are not looking for a single item
+            # Only print the Task header if there are Tasks not found in any Profile, and we are not looking for a
+            # single item
             if (
                 output_the_heading
                 and task_ids
                 and not (found_items["single_profile_found"])
                 and not (found_items["single_task_found"])
             ):
                 my_output(
                     colormap,
                     program_args,
                     output_list,
                     4,
-                    (
-                        '<br><span'
-                        f' style="color:{colormap["task_color"]};font-family:'
-                        f'{program_args["font_to_use"]}>&nbsp;&nbsp;&nbsp;The'
-                        f' following Tasks in Project {project_name} are not in any'
-                        ' Profile...</span><br>'
+                    format_html(
+                        colormap,
+                        "task_color",
+                        "",
+                        (
+                            "<br>&nbsp;&nbsp;&nbsp;The following Tasks in Project"
+                            f" {project_name} are not in any Profile...<br>"
+                        ),
+                        True,
                     ),
                 )
                 my_output(colormap, program_args, output_list, 1, "")
                 output_the_heading = False
 
                 # Format the output line
             task_list = [
@@ -196,15 +197,15 @@
 
 # #############################################################################################
 # Add extra info to Project output line as appropriate and then output it.
 # #############################################################################################
 def get_extra_and_output_project(
     program_args: dict,
     colormap: dict,
-    project: xml.etree,
+    project: defusedxml.ElementTree.XML,
     project_name: str,
     found_items: dict,
     heading: str,
     output_list: list,
     launcher_task_info: str,
 ) -> bool:
     """
@@ -221,44 +222,55 @@
     """
     # See if there is a Kid app and get the Project's priority
     kid_app_info = priority = ''
     if program_args["display_detail_level"] == 3:
         kid_app_info = get_kid_app(project)
         priority = get_priority(project, False)
 
+    # Get the name in a format with proper HTML code wrapped around it
+    project_name_details = format_html(
+        colormap, "project_color", "", f"Project: {project_name}", True
+    )
+
     # Are we looking for a specific Project?
     if program_args["single_project_name"]:
         if project_name != program_args["single_project_name"]:
             return True
         # We found our single Project
         found_items["single_project_found"] = True
         refresh_our_output(
-            False, output_list, project_name, "", heading, colormap, program_args
+            False,
+            output_list,
+            f"{project_name_details} {launcher_task_info}{priority}{kid_app_info}",
+            "",
+            heading,
+            colormap,
+            program_args,
         )
     else:
         my_output(
             colormap,
             program_args,
             output_list,
             2,
-            f"Project: {project_name} {launcher_task_info}{priority}{kid_app_info}",
+            f"{project_name_details} {launcher_task_info}{priority}{kid_app_info}",
         )
     return False
 
 
 # #############################################################################################
 # Go through all the Projects, get their detail and output it
 # #############################################################################################
 def process_projects(
     found_items: dict,
     output_list: list,
     heading: str,
     projects_without_profiles: list,
     found_tasks: list,
-    our_task_element: xml.etree,
+    our_task_element: defusedxml.ElementTree.XML,
     colormap: dict,
     program_args: dict,
     all_tasker_items: dict,
 ) -> list:
     """
     Go through all the Projects, get their detail and output it
         :param found_items: all items found so far
@@ -268,30 +280,23 @@
         :param found_tasks: list of Tasks found
         :param our_task_element: xml element of our Task
         :param colormap: output colors to use
         :param program_args: runtime arguments
         :param all_tasker_items: all Projects/Profiles/Tasks/Scenes
         :return: list of found Tasks
     """
-    # Set up html to use
-    project_color_html = (
-        '<span style="color:'
-        + colormap["project_color"]
-        + program_args["font_to_use"]
-        + ">"
-    )
 
     for project in all_tasker_items["all_projects"]:
         # Don't bother with another Project if we've done a single Task or Profile only
         if found_items["single_task_found"] or found_items["single_profile_found"]:
             break
         project_name = project.find("name").text
 
         # See if there is a Launcher task
-        launcher_task_info = get_launcher_task(project, colormap, project_color_html)
+        launcher_task_info = get_launcher_task(project, colormap)
 
         # Get some extra details and output the Project information
         if get_extra_and_output_project(
             program_args,
             colormap,
             project,
             project_name,
@@ -336,19 +341,20 @@
                 continue  # On to next Project
         else:
             my_output(
                 colormap,
                 program_args,
                 output_list,
                 2,
-                (
-                    '</span><span style="color:'
-                    + colormap["profile_color"]
-                    + FONT_TO_USE
-                    + '><em>Project has no Profiles</em></span>'
+                format_html(
+                    colormap,
+                    "profile_color",
+                    "",
+                    "<em>Project has no Profiles</em>",
+                    False,
                 ),
             )
         my_output(colormap, program_args, output_list, 3, "")  # Close Profile list
 
         # # See if there are Tasks in Project that have no Profile
         if task_ids := get_ids(False, {}, {}, [], project, project_name, []):
             # Process Tasks in Project that are not referenced by a Profile
```

### Comparing `maptasker-1.3.2/maptasker/src/runcli.py` & `maptasker-1.3.3/maptasker/src/runcli.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/rungui.py` & `maptasker-1.3.3/maptasker/src/rungui.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     # Convert runtime argument default values to a dictionary
     prog_args = initialize_runtime_arguments()
 
     # 'Run' button hit.  Get all the input from GUI variables
     try:
         prog_args["display_detail_level"] = int(user_input.display_detail_level)
-    except Exception as e:
+    except TypeError:
         display_detail_level = 1
     # Ok, load up the arguments from the GUI
     prog_args["display_profile_conditions"] = user_input.display_profile_conditions
     prog_args["display_preferences"] = user_input.display_preferences
     prog_args["display_taskernet"] = user_input.display_taskernet
     prog_args["single_project_name"] = user_input.single_project_name
     prog_args["single_profile_name"] = user_input.single_profile_name
```

### Comparing `maptasker-1.3.2/maptasker/src/scenes.py` & `maptasker-1.3.3/maptasker/src/scenes.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 import contextlib
 
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 import maptasker.src.tasks as tasks
 from maptasker.src.outputl import my_output
 from maptasker.src.xmldata import tag_in_type
 from maptasker.src.proclist import process_list
+from maptasker.src.frmthtml import format_html
 
 SCENE_TASK_TYPES = {
     "checkchangeTask": "Check Change",
     "clickTask": "TAP",
     "focuschangeTask": "Focus Change",
     "itemselectedTask": "Item Selected",
     "keyTask": "Key",
@@ -43,15 +44,18 @@
     'nme',
     'widthLand',
     'widthPort',
 ]
 
 
 def get_scene_elements(
-    child: xml.etree, colormap: dict, program_args: dict, output_list: list
+    child: defusedxml.ElementTree.XML,
+    colormap: dict,
+    program_args: dict,
+    output_list: list,
 ) -> None:
     """
     Go through Scene's <xxxElement> tags and output them
         :param child: pointer to '<xxxElement' Scene xml statement
         :param colormap: colors to use
         :param program_args: program runtime arguments
         :param output_list: list of output lines
@@ -61,18 +65,20 @@
     name_xml_element = child.find('Str')
     element_name = name_xml_element.text
     my_output(
         colormap,
         program_args,
         output_list,
         4,
-        (
-            '<span'
-            f' style="color:{colormap["scene_color"]}{program_args["font_to_use"]}>&nbsp;&nbsp;&nbsp;Element:'
-            f' {element_type[0]} named {element_name}</span>'
+        format_html(
+            colormap,
+            "scene_color",
+            "",
+            f"&nbsp;&nbsp;&nbsp;Element: {element_type[0]} named {element_name}",
+            True,
         ),
     )
 
     return
 
 
 def process_scene(
@@ -80,22 +86,22 @@
     output_list: list[str],
     tasks_found: list[str],
     program_args: dict,
     colormap: dict,
     all_tasker_items: dict,
 ) -> None:
     """
-
-    :param my_scene: name of Scene to process
-    :param output_list: list of output lines
-    :param tasks_found: list of Tasks found so far
-    :param program_args: dictionary of runtime arguments
-    :param colormap: dictionary of colors to use
-    :param all_tasker_items: dictionary of Tasker Projects/Profiles/Tasks/Scenes
-    :return:
+    Process the Project's Scene(s), one at a time
+        :param my_scene: name of Scene to process
+        :param output_list: list of output lines
+        :param tasks_found: list of Tasks found so far
+        :param program_args: dictionary of runtime arguments
+        :param colormap: dictionary of colors to use
+        :param all_tasker_items: dictionary of Tasker Projects/Profiles/Tasks/Scenes
+        :return:
     """
     # This import statement must reside here to avoid an error
     from maptasker.src.proclist import process_list
 
     # Go through all the children of the Scene looking for 'click' Tasks
     for child in all_tasker_items["all_scenes"][my_scene]:
         if child.tag in SCENE_TAGS_TO_IGNORE:
@@ -147,19 +153,19 @@
     return
 
 
 # #############################################################################################
 # Go through all Scenes for Project, get their detail and output it
 # #############################################################################################
 def process_project_scenes(
-    project: xml.etree,
+    project: defusedxml.ElementTree.XML,
     colormap: dict,
     program_args: dict,
     output_list: list,
-    our_task_element: xml.etree,
+    our_task_element: defusedxml.ElementTree.XML,
     found_tasks: list,
     all_tasker_items: dict,
 ) -> None:
     """
     Go through all Scenes for Project, get their detail and output it
         :param project: xml element of Project we are processing
         :param colormap: colors to use in output
```

### Comparing `maptasker-1.3.2/maptasker/src/servicec.py` & `maptasker-1.3.3/maptasker/src/servicec.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/share.py` & `maptasker-1.3.3/maptasker/src/share.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 #! /usr/bin/env python3
 
-import re
-
 # ########################################################################################## #
 #                                                                                            #
-# share: process TaskerNet 'Share" information                                               #
+# share: process TaskerNet "Share" information                                               #
 #                                                                                            #
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 
 from maptasker.src.outputl import my_output
-from maptasker.src.xmldata import remove_html_tags
 from maptasker.src.sysconst import FONT_TO_USE
 
 
 def share(
-    root_element: xml.etree,
+    root_element: defusedxml.ElementTree.XML,
     colormap: dict,
     program_args: dict,
     output_list: list,
 ) -> None:
     # Get the <share> element, if any
-    share_element: xml.etree = root_element.find("Share")
+    share_element: defusedxml.ElementTree = root_element.find("Share")
     if share_element is not None:
         #  We have a <Share> .  Find the description
         description_element = share_element.find("d")
         # Process the description
         if description_element is not None:
             description_element_output(
                 description_element, colormap, program_args, output_list
@@ -44,25 +41,28 @@
             # my_output(colormap, program_args, output_list, 4, "")  # Force new line
             out_string = f"&nbsp;&nbsp;TaskerNet search on: {search_element.text}"
             my_output(colormap, program_args, output_list, 2, out_string)
 
 
 # Process the description <d> element
 def description_element_output(
-    description_element: str, colormap: dict, program_args: dict, output_list: list
-) -> str:
+    description_element: defusedxml.ElementTree,
+    colormap: dict,
+    program_args: dict,
+    output_list: list,
+) -> None:
     """
     We have a Taskernet description (<Share>).  Process it
         :param description_element: the xml element with the description
         :param colormap: the colors to use for the output
         :param program_args: the runtime arguments
         :param output_list: the output lines thus far
     """
     # We need to properly format this since it has embedded stuff that screws it up
-    out_string = f"&nbsp;&nbsp;TaskerNet description: {description_element.text}"
+    out_string = f"TaskerNet description: {description_element.text}"
     indent_html = (
         '</p><p'
         f' style="margin-left:20px;margin-right:50px;color:{colormap["taskernet_color"]}{FONT_TO_USE}>'
     )
 
     # Indent the description and override various embedded HTML attributes
     out_string = out_string.replace("<p>", indent_html)
```

### Comparing `maptasker-1.3.2/maptasker/src/shellsort.py` & `maptasker-1.3.3/maptasker/src/shellsort.py`

 * *Files identical despite different names*

### Comparing `maptasker-1.3.2/maptasker/src/sysconst.py` & `maptasker-1.3.3/maptasker/src/sysconst.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
 from maptasker.src.config import OUTPUT_FONT
-from maptasker.src.config import logging
+import logging
 
 # Global constants
 UNKNOWN_TASK_NAME = "Unnamed/Anonymous."
-MY_VERSION = "MapTasker version 1.3.2"
+MY_VERSION = "MapTasker version 1.3.3"
 MY_LICENSE = "GNU GENERAL PUBLIC LICENSE (Version 3, 29 June 2007)"
 NO_PROJECT = "-none found."
 COUNTER_FILE = ".MapTasker_RunCount.txt"
-ARGUMENTS_FILE = ".MapTasker_arguments.txt"
-FONT_TO_USE = f';font-family:{OUTPUT_FONT}"'
+ARGUMENTS_FILE = ".MapTasker_arguments.json"
+FONT_TO_USE = f';font-family:{OUTPUT_FONT}'
 NO_PROFILE = "None or unnamed!"
 
 #  List of color arguments and their names
 #  Two different key/value structures in one:
 #    1- Used as lookup for color selection in GUI.  E.g. key=Disabled Profiles
 #    2- Used as color lookup from runtime parameters.  E.g. DisabledProfile (must follow #1)
 #       Only needed for keys that are different between case #1 and case #2
```

### Comparing `maptasker-1.3.2/maptasker/src/taskactn.py` & `maptasker-1.3.3/maptasker/src/taskactn.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 
 import maptasker.src.tasks as tasks
 from maptasker.src.outputl import my_output
 from maptasker.src.sysconst import logger
 from maptasker.src.sysconst import UNKNOWN_TASK_NAME
+from maptasker.src.frmthtml import format_html
 
 
 # #######################################################################################
 # For this specific Task, get its Actions and output the Task and Actions
 # #######################################################################################
 def get_task_actions_and_output(
-    the_task: xml.etree,
+    the_task: defusedxml.ElementTree.XML,
     output_list: list[str],
     program_args: dict,
     list_type: str,
     the_item: str,
     tasks_found: list[str],
     colormap: dict,
     all_tasks: dict,
@@ -69,15 +70,15 @@
 # #######################################################################################
 def output_list_of_actions(
     colormap: dict,
     program_args: dict,
     output_list: list,
     action_count: int,
     alist: list,
-    the_item: xml.etree.ElementTree,
+    the_item: defusedxml.ElementTree.XML,
 ) -> None:
     """output the list of Task Actions
 
     Parameters:
         :param colormap: dictionary of colors to use
         :param program_args: dictionary of program runtime arguments
         :param output_list: list into which to add the output lines
@@ -86,25 +87,40 @@
         :param the_item: the specific Task's detailed line
 
     Returns: the count of the number of times the program has been called
 
     """
     for taction in alist:
         if taction is not None:
-            if "Label for" in taction:
-                my_output(colormap, program_args, output_list, 2, taction)
-            elif taction[:3] == "...":
-                my_output(colormap, program_args, output_list, 2, f"Action: {taction}")
+            # if "Label for" in taction:
+            #     my_output(colormap, program_args, output_list, 2, taction)
+            if taction[:3] == "...":
+                my_output(
+                    colormap,
+                    program_args,
+                    output_list,
+                    2,
+                    format_html(
+                        colormap, "action_color", "", f"Action: {taction}", False
+                    ),
+                )
             else:
+                #  Output the Action count = line number of action (fill to 2 leading zeros)
                 my_output(
                     colormap,
                     program_args,
                     output_list,
                     2,
-                    f"Action: {str(action_count).zfill(2)} </span>{taction}",
+                    format_html(
+                        colormap,
+                        "action_color",
+                        "",
+                        f"Action: {str(action_count).zfill(2)}</span> {taction}",
+                        False,
+                    ),
                 )
                 action_count += 1
             if (
                 action_count == 2
                 and program_args["display_detail_level"] == 0
                 and UNKNOWN_TASK_NAME in the_item
             ):  # Just show first Task if unknown Task
```

### Comparing `maptasker-1.3.2/maptasker/src/taskerd.py` & `maptasker-1.3.3/maptasker/src/taskerd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #! /usr/bin/env python3
+import defusedxml
+from defusedxml.ElementTree import parse
 
 # ########################################################################################## #
 #                                                                                            #
 # taskerd: get Tasker data from backup xml                                                   #
 #                                                                                            #
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree as ET  # This built-in code will parse the xml for us
 from maptasker.src.sysconst import logger
 
 
 # ###############################################################################################
 # Convert list of xml to dictionary
 # ###############################################################################################
 def move_xml_to_table(all_xml, is_scene: bool):
@@ -31,16 +32,16 @@
 # ###############################################################################################
 # Load all of the Projects, Profiles and Tasks into a format we can easily navigate through
 # ###############################################################################################
 def get_the_xml_data(filename):
     logger.info("entry")
     # Import xml
     try:
-        tree = ET.parse(filename)
-    except Exception as e:
+        tree = parse(filename)
+    except defusedxml.ElementTree.ParseError:
         error_msg = f"Error parsing {filename}"
         print(error_msg)
         logger.debug(error_msg)
         exit(1)
 
     root = tree.getroot()
 
@@ -57,11 +58,11 @@
 
     # Return all data in a dictionary for easier access
     all_tasker_items = {
         "all_projects": all_projects,
         "all_profiles": all_profiles,
         "all_scenes": all_scenes,
         "all_tasks": all_tasks,
-        "all_services": all_services
+        "all_services": all_services,
     }
     logger.info("exit")
     return tree, root, all_tasker_items
```

### Comparing `maptasker-1.3.2/maptasker/src/tasks.py` & `maptasker-1.3.3/maptasker/src/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-import xml.etree.ElementTree  # Need for type hints
+import defusedxml.ElementTree  # Need for type hints
 import maptasker.src.actione as action_evaluate
 
 import maptasker.src.outputl as build_output
 from maptasker.src.xmldata import tag_in_type
 from maptasker.src.kidapp import get_kid_app
 from maptasker.src.priority import get_priority
 from maptasker.src.getids import get_ids
@@ -26,28 +26,30 @@
 from maptasker.src.shellsort import shell_sort
 
 
 # #######################################################################################
 # Navigate through Task's Actions and identify each
 # Return a list of Task's actions for the given Task
 # #######################################################################################
-def get_actions(current_task: xml.etree, colormap: dict, prog_args: dict) -> list:
+def get_actions(
+    current_task: defusedxml.ElementTree.XML, colormap: dict, prog_args: dict
+) -> list:
     """
     Return a list of Task's actions for the given Task
         :param current_task: xml element of the Task we are getting actions for
         :param colormap: colors to use in output
         :param prog_args: runtime arguments
         :return: list of Task 'action' output lines
     """
     tasklist = []
 
     try:
         task_actions = current_task.findall("Action")
-    except Exception as e:
-        print(current_task)
+    except defusedxml.DefusedXmlException:
+        print("tasks.py current Task:", current_task)
         error_msg = "Error: No action found!!!"
         print(error_msg)
         logger.debug(error_msg)
         return []
     if task_actions:
         indentation_amount = ""
         indentation = 0
@@ -78,15 +80,15 @@
                 or ">Else" in task_code
                 or ">End For" in task_code
             ):  # Do we un-indent?
                 indentation -= 1
                 length_indent = len(indentation_amount)
                 indentation_amount = indentation_amount[24:length_indent]
             action_evaluate.build_action(
-                tasklist, task_code, child, indentation, indentation_amount
+                colormap, tasklist, task_code, child, indentation, indentation_amount
             )
             if (
                 ">If" in task_code or ">Else" in task_code or ">For" in task_code
             ):  # Do we indent?
                 indentation += 1
                 indentation_amount = f"{indentation_amount}&nbsp;&nbsp;&nbsp;&nbsp;"
 
@@ -99,15 +101,15 @@
 # #######################################################################################
 def get_task_name(
     the_task_id: str,
     tasks_that_have_been_found: list,
     task_output_lines: list,
     task_type: str,
     all_tasks: dict,
-) -> tuple[xml.etree, str]:
+) -> tuple[defusedxml.ElementTree.XML, str]:
     """
     Get the name of the task given the Task ID
         :param the_task_id: the Task's ID (e.g. '47')
         :param tasks_that_have_been_found: list of Tasks found so far
         :param task_output_lines: list of Tasks
         :param task_type: Type of Task (Entry, Exit, Scene)
         :param all_tasks: all Tasks in xml
@@ -147,15 +149,15 @@
 
 
 # #######################################################################################
 # Find the Project belonging to the Task id passed in
 # #######################################################################################
 def get_project_for_solo_task(
     the_task_id: str, projects_with_no_tasks: list, all_projects: dict
-) -> tuple[str, xml.etree]:
+) -> tuple[str, defusedxml.ElementTree]:
     """
     Find the Project belonging to the Task id passed in
         :param the_task_id: the ID of the Task
         :param projects_with_no_tasks: list of Projects that do not have any Tasks
         :param all_projects: all Tasker Projects
         :return: name of the Project that belongs to this task and the Project xml element
     """
@@ -208,15 +210,15 @@
     our_task_name: str,
     output_list: list,
     project_name: str,
     profile_name: str,
     heading: str,
     found_items: dict,
     task_list: list,
-    our_task_element: xml.etree,
+    our_task_element: defusedxml.ElementTree.XML,
     list_of_found_tasks: list,
     all_tasker_items: dict,
     colormap: dict,
     program_args: dict,
 ) -> None:
     """
     Process a single Task only
@@ -239,14 +241,15 @@
     logger.debug(
         f'tasks single task name:{program_args["single_task_name"]} our Task'
         f' name:{our_task_name}'
     )
     if program_args["single_task_name"] == our_task_name:
         # We have the single Task we are looking for
         found_items["single_task_found"] = True
+
         # Clear output list
         build_output.refresh_our_output(
             True,
             output_list,
             project_name,
             profile_name,
             heading,
@@ -302,15 +305,15 @@
 
 # #######################################################################################
 # output_task: we have a Task and need to generate the output
 # #######################################################################################
 def output_task(
     output_list: list,
     our_task_name: str,
-    our_task_element: xml.etree,
+    our_task_element: defusedxml.ElementTree.XML,
     task_list: list,
     project_name: str,
     profile_name: str,
     list_of_found_tasks: list,
     heading: str,
     colormap: dict,
     program_args: dict,
```

### Comparing `maptasker-1.3.2/maptasker/src/userintr.py` & `maptasker-1.3.3/maptasker/src/userintr.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
+import contextlib
 import customtkinter
-
+from pathlib import Path
 from CTkColorPicker.ctk_color_picker import AskColor
 from maptasker.src.getputarg import save_restore_args
 from maptasker.src.sysconst import TYPES_OF_COLOR_NAMES
 
 # Color Modes: "System" (standard), "Dark", "Light"
 customtkinter.set_appearance_mode("System")
 # Themes: "blue" (standard), "green", "dark-blue"
@@ -455,37 +456,67 @@
     def detail_selected_event(self, display_detail: str):
         self.display_detail_level = display_detail
 
     # #######################################################################################
     # Process color selection
     # #######################################################################################
     def colors_event(self, color_selected_item: str):
+        warning_check = [
+            "Profile Conditions",
+            "Action Conditions",
+            "TaskerNet Information",
+            "Tasker Preferences",
+        ]
+        check_against = [
+            self.display_profile_conditions,
+            self.display_profile_conditions,
+            self.display_taskernet,
+            self.display_preferences,
+        ]
+
+        # Let's first make sure that if a color has been chosen for a display flag, that the flag is True (e.g.
+        # display this colored item)
+        with contextlib.suppress(Exception):
+            the_index = warning_check.index(color_selected_item)
+            if not check_against[the_index]:
+                the_output_message = color_selected_item.replace("Profile ", "")
+                the_output_message = the_output_message.replace("Action ", "")
+                self.display_message_box(
+                    f"Display {the_output_message} is not set to display!", False
+                )
+                return
         # Put up color picker and get the color
         pick_color = AskColor()  # Open the Color Picker
         color = pick_color.get()  # Get the color
         if color is not None:
-            row = self.color_text_row
-            self.color_lookup[TYPES_OF_COLOR_NAMES[color_selected_item]] = (
-                color  # Add color for the selected item to our dictionary
-            )
-            self.color_labels.append(
-                customtkinter.CTkLabel(
-                    self.tabview.tab("Colors"),
-                    text=f"{color_selected_item} << color",
-                    text_color=color,
-                )
-            )
-            self.color_labels[-1].grid(
-                row=self.color_text_row, column=0, padx=0, pady=0
-            )
-            self.color_text_row += 1
             self.display_message_box(
-                f"{color_selected_item} color changed to {color}", True
+                f"{color_selected_item} color changed to {color}", False
             )
 
+            # Okay, plug in the selected color for the selected named item
+            self.extract_color_from_event(color, color_selected_item)
+
+    def extract_color_from_event(self, color, color_selected_item):
+        row = self.color_text_row
+        self.color_lookup[TYPES_OF_COLOR_NAMES[color_selected_item]] = (
+            color  # Add color for the selected item to our dictionary
+        )
+        self.color_labels.append(
+            customtkinter.CTkLabel(
+                self.tabview.tab("Colors"),
+                text=f"{color_selected_item} << color",
+                text_color=color,
+            )
+        )
+        self.color_labels[-1].grid(row=self.color_text_row, column=0, padx=0, pady=0)
+        self.color_text_row += 1
+        self.display_message_box(
+            f"{color_selected_item} color changed to {color}", True
+        )
+
     # #######################################################################################
     # Process the 'conditions' checkbox
     # #######################################################################################
     def condition_event(self):
         self.display_profile_conditions = self.condition_button.get()
 
     # #######################################################################################
@@ -553,27 +584,35 @@
             case "single_profile_name":
                 if value:
                     message = f"{message}Profile set to {value}.\n"
             case "single_task_name":
                 if value:
                     message = f"{message}Task set to {value}.\n"
             case _:
-                self.display_message_box(f"Rutroh!  Undefined argument: {value}")
+                self.display_message_box(f"Rutroh!  Undefined argument: {value}", False)
         return message
 
     # #######################################################################################
     # Process the 'Restore Settings' checkbox
     # #######################################################################################
     def restore_settings_event(self):
         self.set_defaults(False)  # Reset all values
         temp_args = {}
         # Restore all changes that have been saved
         temp_args, self.color_lookup = save_restore_args(
             False, self.color_lookup, temp_args
         )
+        # Check for errors
+        try:
+            if temp_args["msg"]:
+                self.display_message_box(temp_args["msg"], False)
+                return
+        except KeyError:  # Ignore if key not found.
+            pass
+
         # Restore progargs values
         if temp_args or self.color_lookup:
             all_messages, new_message = '', ''
             for key, value in temp_args.items():
                 if key is not None:
                     setattr(self, key, value)
                     if new_message := self.restore_display(key, value):
@@ -610,17 +649,27 @@
         self.set_defaults(False)  # Reset all defaults
 
     # #######################################################################################
     # Process Debug Mode checkbox
     # #######################################################################################
     def debug_checkbox_event(self):
         self.debug = self.debug_checkbox.get()
-        self.display_message_box(
-            "Debug mode requires Tasker backup file to be named: backup.xml", True
-        )
+        if self.debug:
+            if Path("backup.xml").is_file():
+                self.display_message_box("Debug mode enabled.", True)
+            else:
+                self.display_message_box(
+                    (
+                        "Debug mode requires Tasker backup file to be named:"
+                        " 'backup.xml', which is missing!"
+                    ),
+                    False,
+                )
+        else:
+            self.display_message_box("Debug mode disabled.", True)
 
     # #######################################################################################
     # The 'Run' program button has been pressed.  Set the run flag and close the GUI
     # #######################################################################################
     def run_program(self):
         self.go_program = True
         self.quit()
```

### Comparing `maptasker-1.3.2/maptasker/src/xmldata.py` & `maptasker-1.3.3/maptasker/src/xmldata.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # GNU General Public License v3.0                                                            #
 # Permissions of this strong copyleft license are conditioned on making available            #
 # complete source code of licensed works and modifications, which include larger works       #
 # using a licensed work, under the same license. Copyright and license notices must be       #
 # preserved. Contributors provide an express grant of patent rights.                         #
 #                                                                                            #
 # ########################################################################################## #
-from maptasker.src.action import process_xml_list
-from maptasker.src.action import drop_trailing_comma
 
 
 # #######################################################################################
 # See if the xml tag is one of the predefined types and return result
 # #######################################################################################
 def tag_in_type(tag: str, flag: bool) -> bool:
     """evaluate the xml tag to see if it is one of our predefined types
@@ -72,14 +70,18 @@
 #  names = list of entries to substitute the argn value against.
 #    ...It can be a list, which signifies a pull-down list of options to map against:
 #         [ preceding_text1, value1, evaluated_text1, preceding_text2, value2, evaluated_text2, ...]
 #         ['', 'e', 'name'] > Test for '1' and plug in 'name' if '1'
 #         ['some_text', 'l', lookup_code] > use lookup_values dictionary to translate code and plug in value
 # ####################################################################################################
 def get_xml_int_argument_to_value(action, arguments, names):
+    # These imports MUST be here and not at top to avoid circular import error
+    from maptasker.src.action import process_xml_list
+    from maptasker.src.action import drop_trailing_comma
+
     match_results = []
 
     for child in action:
         if child.tag == "Int":
             the_arg = child.attrib.get("sr")
             for arg in arguments:
                 if arg == the_arg:
@@ -116,14 +118,16 @@
 
 # ####################################################################################################
 #  Given an action code (xml), find Str (string) args and match with names
 #  Example:
 #  3 Strs with arg0, arg1 and arg2, to be filled in with their matching name0, name1 and name2 + the associated text
 # ####################################################################################################
 def get_xml_str_argument_to_value(action, arguments, names) -> list:
+    from maptasker.src.action import drop_trailing_comma
+
     match_results = []
     for child in action:
         if child.tag == "Str":
             the_arg = child.attrib.get("sr")
             for arg in arguments:
                 if arg == the_arg:
                     arg_location = arguments.index(arg)
```

### Comparing `maptasker-1.3.2/pyproject.toml` & `maptasker-1.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maptasker"
-version = "1.3.2"
+version = "1.3.3"
 description = "Utility to display your entire Android 'Tasker' configuration on your MAC."
 authors = ["Michael Rubin <mikrubin@gmail.com>"]
 readme = "README_PyPl.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/mctinker/Map-Tasker"
 keywords = ["tasker", "Tasker", "map tasker"]
 packages = [
@@ -15,14 +15,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 customtkinter = "^5.1.2"
 ctkcolorpicker = "^0.3.0"
 pillow = "^9.4.0"
 darkdetect = "^0.8.0"
+defusedxml = "^0.7.1"
 
 [tool.poetry.scripts]
 maptasker = "maptasker.main:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mctinker/Map-Tasker/issues"
 "Change Log" = "https://github.com/mctinker/Map-Tasker/CHANGELOG.md"
```

### Comparing `maptasker-1.3.2/PKG-INFO` & `maptasker-1.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: maptasker
-Version: 1.3.2
+Version: 1.3.3
 Summary: Utility to display your entire Android 'Tasker' configuration on your MAC.
 Home-page: https://github.com/mctinker/Map-Tasker
 License: GPL-3.0-or-later
 Keywords: tasker,Tasker,map tasker
 Author: Michael Rubin
 Author-email: mikrubin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ctkcolorpicker (>=0.3.0,<0.4.0)
 Requires-Dist: customtkinter (>=5.1.2,<6.0.0)
 Requires-Dist: darkdetect (>=0.8.0,<0.9.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Project-URL: Bug Tracker, https://github.com/mctinker/Map-Tasker/issues
 Project-URL: Change Log, https://github.com/mctinker/Map-Tasker/CHANGELOG.md
 Project-URL: Repository, https://github.com/mctinker/Map-Tasker
 Description-Content-Type: text/markdown
 
 # MapTasker
```

