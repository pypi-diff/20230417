# Comparing `tmp/ligo-followup-advocate-1.1.dev1.tar.gz` & `tmp/ligo-followup-advocate-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "./ligo-followup-advocate-1.1.dev1.tar", last modified: Thu Aug 22 02:10:15 2019, max compression
+gzip compressed data, was "ligo-followup-advocate-1.2.0.tar", last modified: Mon Apr 17 01:11:08 2023, max compression
```

## Comparing `ligo-followup-advocate-1.1.dev1.tar` & `ligo-followup-advocate-1.2.0.tar`

### file list

```diff
@@ -1,137 +1,149 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/
--rw-rw-rw-   0 root         (0) root         (0)      110 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/
--rw-r--r--   0 root         (0) root         (0)       77 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5530 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       71 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      796 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        5 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/namespace_packages.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4195 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/test_tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M2468/
--rw-rw-rw-   0 root         (0) root         (0)      986 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)     3956 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M2468/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M2468/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M2468/files/p_astro.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/
--rw-rw-rw-   0 root         (0) root         (0)     7997 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     1642 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/
--rw-rw-rw-   0 root         (0) root         (0)   777600 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/bayestar-gbm.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)       89 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)   777600 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)     4478 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)      968 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/superevent.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/
--rw-rw-rw-   0 root         (0) root         (0)     6501 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     1432 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     1585 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/LALInference.v1.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)     4487 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
--rw-rw-rw-   0 root         (0) root         (0)       80 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)     4478 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)      950 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/superevent.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1122/
--rw-rw-rw-   0 root         (0) root         (0)      633 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1122/files.json
--rw-rw-rw-   0 root         (0) root         (0)     1931 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5566/
--rw-rw-rw-   0 root         (0) root         (0)      986 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5566/files.json
--rw-rw-rw-   0 root         (0) root         (0)     3957 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5566/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5678/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     3961 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5678/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5678/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)       44 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5678/files/em_bright.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     1880 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files/
--rw-rw-rw-   0 root         (0) root         (0)       31 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)       57 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/
--rw-rw-rw-   0 root         (0) root         (0)      991 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/files.json
--rw-rw-rw-   0 root         (0) root         (0)     1880 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/files/
--rw-rw-rw-   0 root         (0) root         (0)       30 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       37 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       57 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1234/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     3958 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1234/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1234/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)       44 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1234/files/em_bright.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/
--rw-rw-rw-   0 root         (0) root         (0)      515 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/files.json
--rw-rw-rw-   0 root         (0) root         (0)     1880 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/files/
--rw-rw-rw-   0 root         (0) root         (0)       32 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       57 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/files/distances_pygrb.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/
--rw-rw-rw-   0 root         (0) root         (0)      987 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/files.json
--rw-rw-rw-   0 root         (0) root         (0)     1880 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/files/
--rw-rw-rw-   0 root         (0) root         (0)       31 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       57 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E5678/
--rw-rw-rw-   0 root         (0) root         (0)       98 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     1883 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E5678/files/
--rw-rw-rw-   0 root         (0) root         (0)     5761 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E5678/files/initial.data
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/
--rw-rw-rw-   0 root         (0) root         (0)     4895 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/logs.json
--rw-rw-rw-   0 root         (0) root         (0)      736 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/files/
--rw-rw-rw-   0 root         (0) root         (0)     4468 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)   111816 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/files/cWB.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)      959 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/superevent.json
--rw-r--r--   0 root         (0) root         (0)      500 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/tool.py
--rw-rw-rw-   0 root         (0) root         (0)    17581 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/jinja.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1252 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/update_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2093 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/initial_body.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/authors.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1218 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/skymap_info.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      770 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/em_bright.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      406 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/p_astro.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     8363 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)        0 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      425 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/initial_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1476 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      166 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/retraction.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      600 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1661 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/RAVEN_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1770 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      143 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      217 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/userguide_conclusion.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      934 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/RAVEN_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      304 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      376 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/compare_skymaps.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       56 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/ligo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      539 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    68611 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/versioneer.py
--rw-rw-rw-   0 root         (0) root         (0)    17895 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/COPYING.md
--rw-r--r--   0 root         (0) root         (0)      796 2019-08-22 02:10:15.000000 ligo-followup-advocate-1.1.dev1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2019-08-22 02:10:09.000000 ligo-followup-advocate-1.1.dev1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.784361 ligo-followup-advocate-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    17895 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/COPYING.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-17 01:11:08.784361 ligo-followup-advocate-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.747361 ligo-followup-advocate-1.2.0/ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.785361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/
+-rw-rw-rw-   0 root         (0) root         (0)    21061 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-17 01:11:08.785361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/jinja.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.751361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/authors.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/compare_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/em_bright.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/initial_body.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/initial_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     8568 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/p_astro.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/retraction.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/skymap_info.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/update_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/userguide_conclusion.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.752361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.745361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.752361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.753361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.753361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.753361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.754361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.755361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.755361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.756361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.756361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.757361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.757361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.757361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/
+-rw-rw-rw-   0 root         (0) root         (0)     3956 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.759361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/
+-rw-rw-rw-   0 root         (0) root         (0)     3957 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.759361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.759361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.765361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5870 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.766361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.766361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.768361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.782361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/voevents.json
+-rw-rw-rw-   0 root         (0) root         (0)     4791 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.783361 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6315 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-04-17 01:11:08.785361 ligo-followup-advocate-1.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/SOURCES.txt` & `ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -45,61 +45,73 @@
 ligo/followup_advocate/test/data/E1234/event.json
 ligo/followup_advocate/test/data/E1234/files.json
 ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
 ligo/followup_advocate/test/data/E1234/files/distances_x.json
 ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
 ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
 ligo/followup_advocate/test/data/E1234/files/initial.data
+ligo/followup_advocate/test/data/E1235/event.json
+ligo/followup_advocate/test/data/E1235/files.json
+ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+ligo/followup_advocate/test/data/E1235/files/initial.data
 ligo/followup_advocate/test/data/E2244/event.json
 ligo/followup_advocate/test/data/E2244/files.json
 ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
 ligo/followup_advocate/test/data/E2244/files/distances_x.json
 ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
 ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
 ligo/followup_advocate/test/data/E5678/event.json
 ligo/followup_advocate/test/data/E5678/files.json
 ligo/followup_advocate/test/data/E5678/files/initial.data
 ligo/followup_advocate/test/data/M1122/event.json
 ligo/followup_advocate/test/data/M1122/files.json
 ligo/followup_advocate/test/data/M1234/event.json
 ligo/followup_advocate/test/data/M1234/files.json
-ligo/followup_advocate/test/data/M1234/files/em_bright.json
-ligo/followup_advocate/test/data/M1234/files/p_astro.json
 ligo/followup_advocate/test/data/M2468/event.json
 ligo/followup_advocate/test/data/M2468/files.json
 ligo/followup_advocate/test/data/M2468/files/p_astro.json
 ligo/followup_advocate/test/data/M5566/event.json
 ligo/followup_advocate/test/data/M5566/files.json
 ligo/followup_advocate/test/data/M5678/event.json
 ligo/followup_advocate/test/data/M5678/files.json
-ligo/followup_advocate/test/data/M5678/files/em_bright.json
-ligo/followup_advocate/test/data/M5678/files/p_astro.json
 ligo/followup_advocate/test/data/S1234/files.json
 ligo/followup_advocate/test/data/S1234/logs.json
 ligo/followup_advocate/test/data/S1234/superevent.json
 ligo/followup_advocate/test/data/S1234/voevents.json
 ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml
-ligo/followup_advocate/test/data/S1234/files/bayestar-gbm.fits.gz
+ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
 ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
 ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
 ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+ligo/followup_advocate/test/data/S1234/files/em_bright.json
+ligo/followup_advocate/test/data/S1234/files/p_astro.json
 ligo/followup_advocate/test/data/S2468/files.json
 ligo/followup_advocate/test/data/S2468/logs.json
 ligo/followup_advocate/test/data/S2468/superevent.json
 ligo/followup_advocate/test/data/S2468/voevents.json
 ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
-ligo/followup_advocate/test/data/S2468/files/cWB.fits.gz
+ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
 ligo/followup_advocate/test/data/S5678/files.json
 ligo/followup_advocate/test/data/S5678/logs.json
 ligo/followup_advocate/test/data/S5678/superevent.json
 ligo/followup_advocate/test/data/S5678/voevents.json
-ligo/followup_advocate/test/data/S5678/files/LALInference.v1.fits.gz
+ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
 ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
 ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
 ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+ligo/followup_advocate/test/data/S5678/files/em_bright.json
+ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+ligo/followup_advocate/test/data/S5678/files/p_astro.json
+ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
 ligo_followup_advocate.egg-info/PKG-INFO
 ligo_followup_advocate.egg-info/SOURCES.txt
 ligo_followup_advocate.egg-info/dependency_links.txt
 ligo_followup_advocate.egg-info/entry_points.txt
-ligo_followup_advocate.egg-info/namespace_packages.txt
 ligo_followup_advocate.egg-info/requires.txt
 ligo_followup_advocate.egg-info/top_level.txt
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo_followup_advocate.egg-info/PKG-INFO` & `ligo-followup-advocate-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.1.dev1
-Summary: LIGO/Virgo Follow-up Advocate Tools
+Version: 1.2.0
+Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
+Maintainer: Brandon Piotrzkowski
+Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
-Description: This package provides tools for LIGO/Virgo follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >= 3.6
+Requires-Python: >=3.8
+License-File: COPYING.md
+
+This package provides tools for LIGO/Virgo/KAGRA follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/test_tool.py` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/test_tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 class MockGraceDb(object):
 
     def __init__(self, service):
         assert service == 'https://gracedb.invalid/api/'
         self.service_url = service
 
     def _open(self, graceid, filename):
-        if filename.endswith('.fits.gz'):
+        if '.fits.gz' in filename:
             # url = ('https://dcc.ligo.org/public/0145/T1700453/001/'
             #        'LALInference_v1.fits.gz')
             # filename = astropy.utils.data.download_file(url, cache=True)
             filename = os.path.join('data', graceid, filename)
             return open(pkg_resources.resource_filename(__name__,
                                                         filename), 'rb')
         else:
             filename = os.path.join('data', graceid, filename)
             if 'bayestar-gbm' in filename:
                 filename += '.gz'
                 return open(pkg_resources.resource_filename(
                     __name__, filename), 'rb')
 
-            elif filename.endswith('.fits'):
+            elif '.fits' in filename:
                 return open(pkg_resources.resource_filename(
                     __name__, filename), 'rb')
 
             else:
                 f = open(pkg_resources.resource_filename(__name__, filename))
 
                 def get_json():
@@ -80,18 +80,24 @@
 
 
 def test_skymap_update(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_update', 'S5678', ['sky_localization']])
 
 
+def test_raven_update(mock_gracedb):
+    main(['--service', 'https://gracedb.invalid/api/',
+          'compose_update', 'S5678',
+          ['raven']])
+
+
 def test_general_update(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_update', 'S5678',
-          ['sky_localization', 'p_astro', 'em_bright']])
+          ['sky_localization', 'p_astro', 'em_bright', 'raven']])
 
 
 def test_classification_update(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_update', 'S5678', ['p_astro', 'em_bright']])
 
 
@@ -102,19 +108,29 @@
 
 
 def test_raven_with_initial_circular(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/', 'compose_raven',
           'S1234'])
 
 
+def test_raven_with_snews(mock_gracedb):
+    main(['--service', 'https://gracedb.invalid/api/', 'compose_raven',
+          'S2468'])
+
+
 def test_raven_without_initial_circular(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/', 'compose_raven',
           'S5678'])
 
 
+def test_medium_latency_cbc_only_detection(mock_gracedb):
+    main(['--service', 'https://gracedb.invalid/api/',
+          'compose_grb_medium_latency', 'E1235'])
+
+
 def test_medium_latency_cbc_detection(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_grb_medium_latency', 'E1234'])
 
 
 def test_medium_latency_cbc_burst_detection(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
@@ -130,7 +146,12 @@
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_grb_medium_latency', 'E2244'])
 
 
 def test_retraction(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/', 'compose_retraction',
           'S1234'])
+
+
+def test_retraction_early_warning(mock_gracedb):
+    main(['--service', 'https://gracedb.invalid/api/', 'compose_retraction',
+          'S5678'])
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M2468/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M2468/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/logs.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/logs.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991666666666666%*

 * *Differences: {"'log'": "{12: {'file': "*

 * *          "'https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz,0', "*

 * *          "'filename': 'bayestar-ext.fits.gz'}}"}*

```diff
@@ -158,17 +158,17 @@
             "tag_names": [],
             "tags": "https://gracedb-dev1.ligo.org/api/events/S1234/log/12/tag/"
         },
         {
             "N": 13,
             "comment": "Combined LVC-Fermi sky map using bayestar.fits.gz",
             "created": "2018-06-28 04:08:44 UTC",
-            "file": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-gbm.fits.gz,0",
+            "file": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz,0",
             "file_version": 0,
-            "filename": "bayestar-gbm.fits.gz",
+            "filename": "bayestar-ext.fits.gz",
             "issuer": "leo.singer@LIGO.ORG",
             "self": "https://gracedb-dev1.ligo.org/api/events/S1234/log/13",
             "tag_names": [
                 "sky_loc",
                 "public"
             ],
             "tags": "https://gracedb-dev1.ligo.org/api/events/S1234/log/13/tag/"
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7894736842105263%*

 * *Differences: {"'bayestar-ext.fits.gz'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz'",*

 * * "'em_bright.json'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/em_bright.json'",*

 * * "'p_astro.json'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/p_astro.json'",*

 * * 'delete': "['bayestar-gbm.fits.gz']"}*

```diff
@@ -1,18 +1,20 @@
 {
     "S1234-1-Initial.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-1-Initial.xml",
     "S1234-2-Update.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-2-Update.xml",
-    "bayestar-gbm.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-gbm.fits.gz",
+    "bayestar-ext.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz",
     "bayestar.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz",
     "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz,0",
     "bayestar.multiorder.fits": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits",
     "bayestar.multiorder.fits,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits,0",
     "coinc.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coinc.xml",
     "coinc.xml,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coinc.xml,0",
     "coincidence_far.json": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coincidence_far.json",
+    "em_bright.json": "https://gracedb-dev1.ligo.org/api/events/S1234/files/em_bright.json",
     "event.log": "https://gracedb-dev1.ligo.org/api/events/S1234/files/event.log",
     "event.log,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/event.log,0",
     "initial.data": "https://gracedb-dev1.ligo.org/api/events/S1234/files/initial.data",
     "initial.data,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/initial.data,0",
+    "p_astro.json": "https://gracedb-dev1.ligo.org/api/events/S1234/files/p_astro.json",
     "psd.xml.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/psd.xml.gz",
     "psd.xml.gz,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/psd.xml.gz,0"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/voevents.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/bayestar-gbm.fits.gz` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

 * *Files 3% similar despite different names*

#### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-1-Initial">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S2468-1-Initial">
   <Who>
     <Date>2018-06-28T13:42:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
     </Param>
     <Param name="Pkt_Ser_Num" dataType="string" value="1"/>
-    <Param name="SupereventID" dataType="string" value="S1234" ucd="meta.id">
+    <Param name="SupereventID" dataType="string" value="S2468" ucd="meta.id">
       <Description>Identifier in GraceDB</Description>
     </Param>
     <Param name="AlertType" dataType="string" value="Initial" ucd="meta.version" unit="">
       <Description>VOEvent alert type</Description>
     </Param>
     <Param name="Retraction" dataType="string" value="false" ucd="meta.code" unit="">
       <Description>Set to true if the event is retracted.</Description>
@@ -25,15 +25,15 @@
     </Param>
     <Param name="Vetted" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates whether this candidate has undergone basic vetting by humans</Description>
     </Param>
     <Param name="OpenAlert" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is an open alert if 1, no if 0</Description>
     </Param>
-    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S1234/view/" ucd="meta.ref.url">
+    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S2468/view/" ucd="meta.ref.url">
       <Description>Web page for evolving status of this GW candidate</Description>
     </Param>
     <Param name="Instruments" dataType="string" value="H1,L1" ucd="meta.code">
       <Description>List of instruments used in analysis to identify this event</Description>
     </Param>
     <Param name="FAR" dataType="float" value="9.11069936486e-14" ucd="arith.rate;stat.falsealarm" unit="Hz">
       <Description>False alarm rate for GW candidates with this strength or greater</Description>
@@ -43,16 +43,16 @@
     </Param>
     <Param name="Pipeline" dataType="string" value="gstlal" ucd="meta.code" unit="">
       <Description>Low-latency data analysis pipeline</Description>
     </Param>
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
-    <Group type="GW_SKYMAP" name="BAYESTAR">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.fits.gz" ucd="meta.ref.url" unit="">
+    <Group type="GW_SKYMAP" name="cWB">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S2468/files/cwb.multiorder.fits" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S1234/superevent.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/files.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('coinc.xml', "*

 * *            "'https://gracedb-dev1.ligo.org/api/events/M1234/files/coinc.xml'), ('initial.data', "*

 * *            "'https://gracedb-dev1.ligo.org/api/events/M1234/files/initial.data'), "*

 * *            "('initial.data,0', "*

 * *            "'https://gracedb-dev1.ligo.org/api/events/M1234/files/initial.data,0'), "*

 * *            "('event.log,0', 'https://gracedb-dev1.ligo.org/api/events/M1234/files/event.log,0'), "*

 * *            "('psd.xml.gz,0', "*

 * *            "'https://gracedb-dev […]*

```diff
@@ -1,29 +1,14 @@
 {
-    "created": "2018-06-28 03:08:38 UTC",
-    "em_events": [
-        "E1234"
-    ],
-    "gw_events": [
-        "M1234",
-        "M5678",
-        "M2468"
-    ],
-    "labels": [
-        "EM_COINC"
-    ],
-    "links": {
-        "emobservations": "https://gracedb-dev1.ligo.org/api/superevents/S1234/emobservations/",
-        "events": "https://gracedb-dev1.ligo.org/api/superevents/S1234/events/",
-        "files": "https://gracedb-dev1.ligo.org/api/superevents/S1234/files/",
-        "labels": "https://gracedb-dev1.ligo.org/api/superevents/S1234/labels/",
-        "logs": "https://gracedb-dev1.ligo.org/api/superevents/S1234/logs/",
-        "self": "https://gracedb-dev1.ligo.org/api/superevents/S1234/",
-        "voevents": "https://gracedb-dev1.ligo.org/api/superevents/S1234/voevents/"
-    },
-    "preferred_event": "M1234",
-    "submitter": "leo.singer@LIGO.ORG",
-    "superevent_id": "S1234",
-    "t_0": 1214190502.74,
-    "t_end": 1214190503.74,
-    "t_start": 1214190501.74
+    "bayestar.fits.gz": "https://gracedb-dev1.ligo.org/api/events/M1234/files/bayestar.fits.gz",
+    "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/M1234/files/bayestar.fits.gz,0",
+    "coinc.xml": "https://gracedb-dev1.ligo.org/api/events/M1234/files/coinc.xml",
+    "coinc.xml,0": "https://gracedb-dev1.ligo.org/api/events/M1234/files/coinc.xml,0",
+    "em_bright.json": "https://gracedb-dev1.ligo.org/api/events/M1234/files/em_bright.json",
+    "event.log": "https://gracedb-dev1.ligo.org/api/events/M1234/files/event.log",
+    "event.log,0": "https://gracedb-dev1.ligo.org/api/events/M1234/files/event.log,0",
+    "initial.data": "https://gracedb-dev1.ligo.org/api/events/M1234/files/initial.data",
+    "initial.data,0": "https://gracedb-dev1.ligo.org/api/events/M1234/files/initial.data,0",
+    "p_astro.json": "https://gracedb-dev1.ligo.org/api/events/M1234/files/p_astro.json",
+    "psd.xml.gz": "https://gracedb-dev1.ligo.org/api/events/M1234/files/psd.xml.gz",
+    "psd.xml.gz,0": "https://gracedb-dev1.ligo.org/api/events/M1234/files/psd.xml.gz,0"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/logs.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/logs.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9803571428571428%*

 * *Differences: {"'log'": "{9: {'filename': 'LALInference.fits.gz'}, 13: {'self': "*

 * *          "'https://gracedb-dev1.ligo.org/api/events/S5678/log/14', 'tags': "*

 * *          "'https://gracedb-dev1.ligo.org/api/events/S5678/log/14/tag/', 'N': 14}, insert: [(11, "*

 * *          "OrderedDict([('comment', 'Combined LVC-Fermi sky map bayestar.fits.gz'), "*

 * *          "('file_version', 0), ('tag_names', ['sky_loc', 'public']), ('file', "*

 * *          "'https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz,0'), "*

 * *        […]*

```diff
@@ -121,15 +121,15 @@
         },
         {
             "N": 10,
             "comment": "lalinference sky localization complete",
             "created": "2018-06-28 04:08:44 UTC",
             "file": "https://gracedb-dev1.ligo.org/api/events/S5678/files/LALInference.v1.fits.gz,0",
             "file_version": 0,
-            "filename": "LALInference.v1.fits.gz",
+            "filename": "LALInference.fits.gz",
             "issuer": "leo.singer@LIGO.ORG",
             "self": "https://gracedb-dev1.ligo.org/api/events/S5678/log/10",
             "tag_names": [
                 "sky_loc",
                 "lvem",
                 "public"
             ],
@@ -145,21 +145,51 @@
             "issuer": "leo.singer@LIGO.ORG",
             "self": "https://gracedb-dev1.ligo.org/api/events/S5678/log/11",
             "tag_names": [],
             "tags": "https://gracedb-dev1.ligo.org/api/events/S5678/log/11/tag/"
         },
         {
             "N": 12,
+            "comment": "Combined LVC-Fermi sky map bayestar.fits.gz",
+            "created": "2018-06-28 04:08:44 UTC",
+            "file": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz,0",
+            "file_version": 0,
+            "filename": "bayestar-ext.fits.gz",
+            "issuer": "leo.singer@LIGO.ORG",
+            "self": "https://gracedb-dev1.ligo.org/api/events/S1234/log/12",
+            "tag_names": [
+                "sky_loc",
+                "public"
+            ],
+            "tags": "https://gracedb-dev1.ligo.org/api/events/S1234/log/12/tag/"
+        },
+        {
+            "N": 13,
+            "comment": "Combined LVC-Fermi sky map using bayestar.fits.gz",
+            "created": "2018-06-28 04:08:44 UTC",
+            "file": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.png,0",
+            "file_version": 0,
+            "filename": "bayestar-ext.png",
+            "issuer": "leo.singer@LIGO.ORG",
+            "self": "https://gracedb-dev1.ligo.org/api/events/S1234/log/13",
+            "tag_names": [
+                "sky_loc",
+                "public"
+            ],
+            "tags": "https://gracedb-dev1.ligo.org/api/events/S1234/log/13/tag/"
+        },
+        {
+            "N": 14,
             "comment": "Tagged message 10: lvem ",
             "created": "2018-06-28 04:08:44 UTC",
             "file": null,
             "file_version": null,
             "filename": "",
             "issuer": "leo.singer@LIGO.ORG",
-            "self": "https://gracedb-dev1.ligo.org/api/events/S5678/log/12",
+            "self": "https://gracedb-dev1.ligo.org/api/events/S5678/log/14",
             "tag_names": [],
-            "tags": "https://gracedb-dev1.ligo.org/api/events/S5678/log/12/tag/"
+            "tags": "https://gracedb-dev1.ligo.org/api/events/S5678/log/14/tag/"
         }
     ],
     "numRows": 9,
     "start": 0
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.46153846153846156%*

 * *Differences: {"'LALInference.fits.gz'": "'https://gracedb-dev1.ligo.org/api/events/S5678/files/LALInference.fits.gz'",*

 * * "'LALInference.fits.gz,0'": "'https://gracedb-dev1.ligo.org/api/events/S5678/files/LALInference.fits.gz,0'",*

 * * "'bayestar.multiorder.fits'": "'https://gracedb-dev1.ligo.org/api/events/S5678/files/bayestar.fits.gz'",*

 * * "'bayestar.multiorder.fits,0'": "'https://gracedb-dev1.ligo.org/api/events/S5678/files/bayestar.fits.gz'",*

 * * "'combined-ext.fits.gz,1'": "'https://gracedb-dev1.ligo.org/api/events/S1234/file […]*

```diff
@@ -1,17 +1,25 @@
 {
-    "LALInference.v1.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S5678/files/LALInference.v1.fits.gz",
-    "LALInference.v1.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/LALInference.v1.fits.gz,0",
+    "LALInference.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S5678/files/LALInference.fits.gz",
+    "LALInference.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/LALInference.fits.gz,0",
     "S5678-1-Initial.xml": "https://gracedb-dev1.ligo.org/api/events/S5678/files/S5678-1-Initial.xml",
     "S5678-2-Update.xml": "https://gracedb-dev1.ligo.org/api/events/S5678/files/S5678-2-Update.xml",
     "bayestar.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S5678/files/bayestar.fits.gz",
-    "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/bayestar.fits.gz,0",
+    "bayestar.multiorder.fits": "https://gracedb-dev1.ligo.org/api/events/S5678/files/bayestar.fits.gz",
+    "bayestar.multiorder.fits,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/bayestar.fits.gz",
     "coinc.xml": "https://gracedb-dev1.ligo.org/api/events/S5678/files/coinc.xml",
     "coinc.xml,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/coinc.xml,0",
     "coincidence_far.json": "https://gracedb-dev1.ligo.org/api/events/S5678/files/coincidence_far.json",
+    "combined-ext.fits.gz,1": "https://gracedb-dev1.ligo.org/api/events/S1234/files/combined-ext.fits.gz,1",
+    "combined-ext.mulitorder.fits": "https://gracedb-dev1.ligo.org/api/events/S1234/files/combined-ext.mulitorder.fits,1",
+    "combined-ext.mulitorder.fits,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/combined-ext.mulitorder.fits,0",
+    "em_bright.json": "https://gracedb-dev1.ligo.org/api/events/S5678/files/em_bright.json",
+    "em_bright.json,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/em_bright.json,0",
     "event.log": "https://gracedb-dev1.ligo.org/api/events/S5678/files/event.log",
     "event.log,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/event.log,0",
     "initial.data": "https://gracedb-dev1.ligo.org/api/events/S5678/files/initial.data",
     "initial.data,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/initial.data,0",
+    "p_astro.json": "https://gracedb-dev1.ligo.org/api/events/S5678/files/p_astro.json",
+    "p_astro.json,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/p_astro.json,0",
     "psd.xml.gz": "https://gracedb-dev1.ligo.org/api/events/S5678/files/psd.xml.gz",
     "psd.xml.gz,0": "https://gracedb-dev1.ligo.org/api/events/S5678/files/psd.xml.gz,0"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/voevents.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/LALInference.v1.fits.gz` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml`

 * *Files 8% similar despite different names*

#### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml`

```diff
@@ -1,39 +1,39 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S5678-2-Update">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-1-Initial">
   <Who>
-    <Date>2018-06-28T14:42:02</Date>
+    <Date>2018-06-28T13:42:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
     </Param>
     <Param name="Pkt_Ser_Num" dataType="string" value="1"/>
-    <Param name="SupereventID" dataType="string" value="S5678" ucd="meta.id">
+    <Param name="SupereventID" dataType="string" value="S1234" ucd="meta.id">
       <Description>Identifier in GraceDB</Description>
     </Param>
-    <Param name="AlertType" dataType="string" value="Update" ucd="meta.version" unit="">
+    <Param name="AlertType" dataType="string" value="Initial" ucd="meta.version" unit="">
       <Description>VOEvent alert type</Description>
     </Param>
     <Param name="Retraction" dataType="string" value="false" ucd="meta.code" unit="">
       <Description>Set to true if the event is retracted.</Description>
     </Param>
     <Param name="HardwareInj" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is a hardware injection if 1, no if 0</Description>
     </Param>
-    <Param name="Vetted" dataType="int" value="1" ucd="meta.number" unit="">
+    <Param name="Vetted" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates whether this candidate has undergone basic vetting by humans</Description>
     </Param>
     <Param name="OpenAlert" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is an open alert if 1, no if 0</Description>
     </Param>
-    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S5678/view/" ucd="meta.ref.url">
+    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S1234/view/" ucd="meta.ref.url">
       <Description>Web page for evolving status of this GW candidate</Description>
     </Param>
     <Param name="Instruments" dataType="string" value="H1,L1" ucd="meta.code">
       <Description>List of instruments used in analysis to identify this event</Description>
     </Param>
     <Param name="FAR" dataType="float" value="9.11069936486e-14" ucd="arith.rate;stat.falsealarm" unit="Hz">
       <Description>False alarm rate for GW candidates with this strength or greater</Description>
@@ -43,30 +43,33 @@
     </Param>
     <Param name="Pipeline" dataType="string" value="gstlal" ucd="meta.code" unit="">
       <Description>Low-latency data analysis pipeline</Description>
     </Param>
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
-    <Group type="GW_SKYMAP" name="LALInference">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S5678/files/LALInference.v1.fits.gz" ucd="meta.ref.url" unit="">
+    <Param dataType="int" name="Significant" ucd="meta.number" value="1">
+      <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
+    </Param>
+    <Group type="GW_SKYMAP" name="BAYESTAR">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.fits.gz" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time>
             <TimeInstant>
-              <ISOTime>2018-06-28T14:35:16.911085</ISOTime>
+              <ISOTime>2018-06-28T13:35:16.911085</ISOTime>
             </TimeInstant>
           </Time>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

 * *Files 18% similar despite different names*

#### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

```diff
@@ -43,16 +43,46 @@
     </Param>
     <Param name="Pipeline" dataType="string" value="gstlal" ucd="meta.code" unit="">
       <Description>Low-latency data analysis pipeline</Description>
     </Param>
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
+    <Param dataType="int" name="Significant" ucd="meta.number" value="0">
+      <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
+    </Param>
+    <Group name="External Coincidence" type="External Coincidence">
+      <Param name="External_GCN_Notice_Id" value="1364244245" ucd="meta.id" dataType="string">
+        <Description>GCN trigger ID of external event</Description>
+      </Param>
+      <Param name="External_Ivorn" value="ivo://lvk.internal/AGILE#O3-replay_event2023-03-30T20:43:47.992Z" ucd="meta.id" dataType="string">
+        <Description>IVORN of external event</Description>
+      </Param>
+      <Param name="External_Observatory" value="AGILE" ucd="meta.code" dataType="string">
+        <Description>External Observatory</Description>
+      </Param>
+      <Param name="External_Search" value="GRB" ucd="meta.code" dataType="string">
+        <Description>External astrophysical search</Description>
+      </Param>
+      <Param name="Time_Difference" value="2.1" ucd="meta.code" dataType="float">
+        <Description>Time difference between GW candidate and external event, centered on the GW candidate</Description>
+      </Param>
+      <Param name="Time_Coincidence_FAR" value="3.8934000570776255e-13" unit="Hz" ucd="arith.rate;stat.falsealarm" dataType="float">
+        <Description>Estimated coincidence false alarm rate in Hz using timing</Description>
+      </Param>
+      <Param name="Time_Sky_Position_Coincidence_FAR" value="9.640269821382047e-11" unit="Hz" ucd="arith.rate;stat.falsealarm" dataType="float">
+        <Description>Estimated coincidence false alarm rate in Hz using timing and sky position</Description>
+      </Param>
+      <Param name="joint_skymap_fits" value="https://gracedb-playground.ligo.org/api/superevents/S230330ax/files/combined-ext.multiorder.fits,0" ucd="meta.ref.url" dataType="string">
+        <Description>Combined GW-External Sky Map FITS</Description>
+      </Param>
+      <Description>Properties of joint coincidence found by RAVEN</Description>
+    </Group>
     <Group type="GW_SKYMAP" name="BAYESTAR">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S5678/files/bayestar.fits.gz" ucd="meta.ref.url" unit="">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S5678/files/bayestar.multiorder.fits" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S5678/superevent.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/files.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('coinc.xml', "*

 * *            "'https://gracedb-dev1.ligo.org/api/events/M5678/files/coinc.xml'), ('initial.data', "*

 * *            "'https://gracedb-dev1.ligo.org/api/events/M5678/files/initial.data'), "*

 * *            "('initial.data,0', "*

 * *            "'https://gracedb-dev1.ligo.org/api/events/M5678/files/initial.data,0'), "*

 * *            "('event.log,0', 'https://gracedb-dev1.ligo.org/api/events/M5678/files/event.log,0'), "*

 * *            "('psd.xml.gz,0', "*

 * *            "'https://gracedb-dev […]*

```diff
@@ -1,27 +1,13 @@
 {
-    "created": "2018-06-28 03:08:38 UTC",
-    "em_events": [
-        "E5678"
-    ],
-    "gw_events": [
-        "M5678"
-    ],
-    "labels": [
-        "EM_COINC"
-    ],
-    "links": {
-        "emobservations": "https://gracedb-dev1.ligo.org/api/superevents/S5678/emobservations/",
-        "events": "https://gracedb-dev1.ligo.org/api/superevents/S5678/events/",
-        "files": "https://gracedb-dev1.ligo.org/api/superevents/S5678/files/",
-        "labels": "https://gracedb-dev1.ligo.org/api/superevents/S5678/labels/",
-        "logs": "https://gracedb-dev1.ligo.org/api/superevents/S5678/logs/",
-        "self": "https://gracedb-dev1.ligo.org/api/superevents/S5678/",
-        "voevents": "https://gracedb-dev1.ligo.org/api/superevents/S5678/voevents/"
-    },
-    "preferred_event": "M5678",
-    "submitter": "leo.singer@LIGO.ORG",
-    "superevent_id": "S5678",
-    "t_0": 1214190502.74,
-    "t_end": 1214190503.74,
-    "t_start": 1214190501.74
+    "bayestar.fits.gz": "https://gracedb-dev1.ligo.org/api/events/M5678/files/bayestar.fits.gz",
+    "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/bayestar.fits.gz,0",
+    "coinc.xml": "https://gracedb-dev1.ligo.org/api/events/M5678/files/coinc.xml",
+    "coinc.xml,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/coinc.xml,0",
+    "event.log": "https://gracedb-dev1.ligo.org/api/events/M5678/files/event.log",
+    "event.log,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/event.log,0",
+    "initial.data": "https://gracedb-dev1.ligo.org/api/events/M5678/files/initial.data",
+    "initial.data,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/initial.data,0",
+    "p_astro.json": "https://gracedb-dev1.ligo.org/api/events/M5678/files/p_astro.json",
+    "psd.xml.gz": "https://gracedb-dev1.ligo.org/api/events/M5678/files/psd.xml.gz",
+    "psd.xml.gz,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/psd.xml.gz,0"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1122/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1122/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5566/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/files.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'em_bright.json'": "'https://gracedb-dev1.ligo.org/api/events/M5678/files/em_bright.json'"}*

```diff
@@ -1,12 +1,13 @@
 {
     "bayestar.fits.gz": "https://gracedb-dev1.ligo.org/api/events/M5678/files/bayestar.fits.gz",
     "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/bayestar.fits.gz,0",
     "coinc.xml": "https://gracedb-dev1.ligo.org/api/events/M5678/files/coinc.xml",
     "coinc.xml,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/coinc.xml,0",
+    "em_bright.json": "https://gracedb-dev1.ligo.org/api/events/M5678/files/em_bright.json",
     "event.log": "https://gracedb-dev1.ligo.org/api/events/M5678/files/event.log",
     "event.log,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/event.log,0",
     "initial.data": "https://gracedb-dev1.ligo.org/api/events/M5678/files/initial.data",
     "initial.data,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/initial.data,0",
     "p_astro.json": "https://gracedb-dev1.ligo.org/api/events/M5678/files/p_astro.json",
     "psd.xml.gz": "https://gracedb-dev1.ligo.org/api/events/M5678/files/psd.xml.gz",
     "psd.xml.gz,0": "https://gracedb-dev1.ligo.org/api/events/M5678/files/psd.xml.gz,0"
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5566/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M5678/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/event.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'pipeline'": "'MBTA'"}*

```diff
@@ -98,12 +98,12 @@
         "log": "https://gracedb-dev1.ligo.org/api/events/M5678/log/",
         "neighbors": "https://gracedb-dev1.ligo.org/api/events/M5678/neighbors/",
         "self": "https://gracedb-dev1.ligo.org/api/events/M5678",
         "tags": "https://gracedb-dev1.ligo.org/api/events/M5678/tag/"
     },
     "nevents": 2,
     "offline": false,
-    "pipeline": "MBTAOnline",
+    "pipeline": "MBTA",
     "search": "MDC",
     "submitter": "leo.singer@LIGO.ORG",
     "superevent": "S180628g"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/event.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995098039215686%*

 * *Differences: {"'extra_attributes'": "{'GRB': {'error_radius': 0.05}}"}*

```diff
@@ -4,15 +4,15 @@
         "GRB": {
             "T90": null,
             "author_ivorn": "ivo://nasa.gsfc.tan/gcn",
             "author_shortname": "VO-GCN",
             "coord_system": "UTC-FK5-GEO",
             "dec": 78.5044,
             "designation": "GRB XXXXXXXXX",
-            "error_radius": 0.0,
+            "error_radius": 0.05,
             "how_description": "Swift Satellite, BAT Instrument",
             "how_reference_url": "http://gcn.gsfc.nasa.gov/swift.html",
             "ivorn": "ivo://nasa.gsfc.gcn/SWIFT#BAT_Lightcurve_876016-496",
             "observatory_location_id": "GEOLUN",
             "ra": 248.2071,
             "redshift": null,
             "trigger_duration": 16.384,
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1234/files/initial.data` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E2244/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/event.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9558823529411765%*

 * *Differences: {"'graceid'": "'E1122'",*

 * * "'links'": "{'neighbors': 'https://gracedb-pcdev1.ligo.org/api/events/E1122/neighbors/', 'files': "*

 * *            "'https://gracedb-pcdev1.ligo.org/api/events/E1122/files/', 'log': "*

 * *            "'https://gracedb-pcdev1.ligo.org/api/events/E1122/log/', 'tags': "*

 * *            "'https://gracedb-pcdev1.ligo.org/api/events/E1122/tag/', 'self': "*

 * *            "'https://gracedb-pcdev1.ligo.org/api/events/E1122', 'labels': "*

 * *            "'https://gracedb-pcdev1.ligo.org/api/events/E1122/label […]*

```diff
@@ -18,27 +18,27 @@
             "trigger_duration": 16.384,
             "trigger_id": "876016"
         }
     },
     "far": null,
     "far_is_upper_limit": false,
     "gpstime": 1214190503.74,
-    "graceid": "E2244",
+    "graceid": "E1122",
     "group": "External",
     "instruments": "",
     "labels": [],
     "likelihood": null,
     "links": {
-        "emobservations": "https://gracedb-pcdev1.ligo.org/api/events/E2244/emobservation/",
-        "files": "https://gracedb-pcdev1.ligo.org/api/events/E2244/files/",
-        "labels": "https://gracedb-pcdev1.ligo.org/api/events/E2244/labels/",
-        "log": "https://gracedb-pcdev1.ligo.org/api/events/E2244/log/",
-        "neighbors": "https://gracedb-pcdev1.ligo.org/api/events/E2244/neighbors/",
-        "self": "https://gracedb-pcdev1.ligo.org/api/events/E2244",
-        "tags": "https://gracedb-pcdev1.ligo.org/api/events/E2244/tag/"
+        "emobservations": "https://gracedb-pcdev1.ligo.org/api/events/E1122/emobservation/",
+        "files": "https://gracedb-pcdev1.ligo.org/api/events/E1122/files/",
+        "labels": "https://gracedb-pcdev1.ligo.org/api/events/E1122/labels/",
+        "log": "https://gracedb-pcdev1.ligo.org/api/events/E1122/log/",
+        "neighbors": "https://gracedb-pcdev1.ligo.org/api/events/E1122/neighbors/",
+        "self": "https://gracedb-pcdev1.ligo.org/api/events/E1122",
+        "tags": "https://gracedb-pcdev1.ligo.org/api/events/E1122/tag/"
     },
     "nevents": null,
     "offline": false,
     "pipeline": "Swift",
     "search": "GRB",
     "submitter": "emfollow",
     "superevent": "S1234"
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/M1234/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1133/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/event.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9362745098039217%*

 * *Differences: {"'extra_attributes'": "{'GRB': {'trigger_id': '1000215', 'trigger_duration': None, "*

 * *                       "'author_shortname': 'SNEWS (via VO-TAN)', 'how_reference_url': "*

 * *                       "'http://gcn.gsfc.nasa.gov/snews.html', 'designation': None, "*

 * *                       "'how_description': 'SNEWS: SuperNova Early Warning System', "*

 * *                       "'error_radius': 360.0, 'ra': 0.0, 'dec': 0.0, 'ivorn': "*

 * *                       "'ivo://nasa.gsfc.gcn/SNEWS#Event2019-02-12T17:00:02.00_10002 […]*

```diff
@@ -1,26 +1,26 @@
 {
     "created": "2018-12-13 13:01:30 UTC",
     "extra_attributes": {
         "GRB": {
             "T90": null,
             "author_ivorn": "ivo://nasa.gsfc.tan/gcn",
-            "author_shortname": "VO-GCN",
+            "author_shortname": "SNEWS (via VO-TAN)",
             "coord_system": "UTC-FK5-GEO",
-            "dec": 78.5044,
-            "designation": "GRB XXXXXXXXX",
-            "error_radius": 0.0,
-            "how_description": "Swift Satellite, BAT Instrument",
-            "how_reference_url": "http://gcn.gsfc.nasa.gov/swift.html",
-            "ivorn": "ivo://nasa.gsfc.gcn/SWIFT#BAT_Lightcurve_876016-496",
+            "dec": 0.0,
+            "designation": null,
+            "error_radius": 360.0,
+            "how_description": "SNEWS: SuperNova Early Warning System",
+            "how_reference_url": "http://gcn.gsfc.nasa.gov/snews.html",
+            "ivorn": "ivo://nasa.gsfc.gcn/SNEWS#Event2019-02-12T17:00:02.00_1000215-127",
             "observatory_location_id": "GEOLUN",
-            "ra": 248.2071,
+            "ra": 0.0,
             "redshift": null,
-            "trigger_duration": 16.384,
-            "trigger_id": "876016"
+            "trigger_duration": null,
+            "trigger_id": "1000215"
         }
     },
     "far": null,
     "far_is_upper_limit": false,
     "gpstime": 1214190503.74,
     "graceid": "E1133",
     "group": "External",
@@ -34,12 +34,12 @@
         "log": "https://gracedb-pcdev1.ligo.org/api/events/E1133/log/",
         "neighbors": "https://gracedb-pcdev1.ligo.org/api/events/E1133/neighbors/",
         "self": "https://gracedb-pcdev1.ligo.org/api/events/E1133",
         "tags": "https://gracedb-pcdev1.ligo.org/api/events/E1133/tag/"
     },
     "nevents": null,
     "offline": false,
-    "pipeline": "Swift",
-    "search": "GRB",
+    "pipeline": "SNEWS",
+    "search": "Supernova",
     "submitter": "emfollow",
     "superevent": "S1234"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E1122/event.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/event.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9215686274509803%*

 * *Differences: {"'extra_attributes'": "{'GRB': {'trigger_id': '206740', 'trigger_duration': None, "*

 * *                       "'author_shortname': 'INTEGRAL (via VO-GCN)', 'how_reference_url': "*

 * *                       "'http://gcn.gsfc.nasa.gov/integral.html', 'designation': None, "*

 * *                       "'how_description': 'INTEGRAL Satellite', 'error_radius': 0.05, 'ra': "*

 * *                       "350.65, 'dec': -4.2607, 'ivorn': "*

 * *                       "'ivo://nasa.gsfc.gcn/INTEGRAL#Offline_Pos_010132-3-186'}}",*

 * * "'grace […]*

```diff
@@ -1,45 +1,45 @@
 {
     "created": "2018-12-13 13:01:30 UTC",
     "extra_attributes": {
         "GRB": {
             "T90": null,
             "author_ivorn": "ivo://nasa.gsfc.tan/gcn",
-            "author_shortname": "VO-GCN",
+            "author_shortname": "INTEGRAL (via VO-GCN)",
             "coord_system": "UTC-FK5-GEO",
-            "dec": 78.5044,
-            "designation": "GRB XXXXXXXXX",
-            "error_radius": 0.0,
-            "how_description": "Swift Satellite, BAT Instrument",
-            "how_reference_url": "http://gcn.gsfc.nasa.gov/swift.html",
-            "ivorn": "ivo://nasa.gsfc.gcn/SWIFT#BAT_Lightcurve_876016-496",
+            "dec": -4.2607,
+            "designation": null,
+            "error_radius": 0.05,
+            "how_description": "INTEGRAL Satellite",
+            "how_reference_url": "http://gcn.gsfc.nasa.gov/integral.html",
+            "ivorn": "ivo://nasa.gsfc.gcn/INTEGRAL#Offline_Pos_010132-3-186",
             "observatory_location_id": "GEOLUN",
-            "ra": 248.2071,
+            "ra": 350.65,
             "redshift": null,
-            "trigger_duration": 16.384,
-            "trigger_id": "876016"
+            "trigger_duration": null,
+            "trigger_id": "206740"
         }
     },
     "far": null,
     "far_is_upper_limit": false,
     "gpstime": 1214190503.74,
-    "graceid": "E1122",
+    "graceid": "E1234",
     "group": "External",
     "instruments": "",
     "labels": [],
     "likelihood": null,
     "links": {
-        "emobservations": "https://gracedb-pcdev1.ligo.org/api/events/E1122/emobservation/",
-        "files": "https://gracedb-pcdev1.ligo.org/api/events/E1122/files/",
-        "labels": "https://gracedb-pcdev1.ligo.org/api/events/E1122/labels/",
-        "log": "https://gracedb-pcdev1.ligo.org/api/events/E1122/log/",
-        "neighbors": "https://gracedb-pcdev1.ligo.org/api/events/E1122/neighbors/",
-        "self": "https://gracedb-pcdev1.ligo.org/api/events/E1122",
-        "tags": "https://gracedb-pcdev1.ligo.org/api/events/E1122/tag/"
+        "emobservations": "https://gracedb-pcdev1.ligo.org/api/events/E1234/emobservation/",
+        "files": "https://gracedb-pcdev1.ligo.org/api/events/E1234/files/",
+        "labels": "https://gracedb-pcdev1.ligo.org/api/events/E1234/labels/",
+        "log": "https://gracedb-pcdev1.ligo.org/api/events/E1234/log/",
+        "neighbors": "https://gracedb-pcdev1.ligo.org/api/events/E1234/neighbors/",
+        "self": "https://gracedb-pcdev1.ligo.org/api/events/E1234",
+        "tags": "https://gracedb-pcdev1.ligo.org/api/events/E1234/tag/"
     },
     "nevents": null,
     "offline": false,
-    "pipeline": "Swift",
+    "pipeline": "INTEGRAL",
     "search": "GRB",
     "submitter": "emfollow",
     "superevent": "S1234"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/E5678/files/initial.data` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/logs.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/logs.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111111%*

 * *Differences: {"'log'": "{6: {'file': "*

 * *          "'https://gracedb-dev1.ligo.org/api/events/S2468/files/cwb.mulitorder.fits,0', "*

 * *          "'filename': 'cwb.mulitorder.fits'}}"}*

```diff
@@ -79,17 +79,17 @@
             "tag_names": [],
             "tags": "https://gracedb-dev1.ligo.org/api/events/S2468/log/6/tag/"
         },
         {
             "N": 7,
             "comment": "cwb sky localization complete",
             "created": "2018-06-28 03:08:44 UTC",
-            "file": "https://gracedb-dev1.ligo.org/api/events/S2468/files/cWB.fits.gz,0",
+            "file": "https://gracedb-dev1.ligo.org/api/events/S2468/files/cwb.mulitorder.fits,0",
             "file_version": 0,
-            "filename": "cWB.fits.gz",
+            "filename": "cwb.mulitorder.fits",
             "issuer": "leo.singer@LIGO.ORG",
             "self": "https://gracedb-dev1.ligo.org/api/events/S2468/log/7",
             "tag_names": [
                 "sky_loc",
                 "lvem",
                 "public"
             ],
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/files.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5555555555555556%*

 * *Differences: {"'cwb.multiorder.fits'": "'https://gracedb-playground.ligo.org/api/events/S2468/files/cwb.multiorder.fits'",*

 * * "'cwb.multiorder.fits,0'": "'https://gracedb-playground.ligo.org/api/events/S2468/files/cwb.multiorder.fits'",*

 * * 'delete': "['cWB.fits.gz,0', 'cWB.fits.gz']"}*

```diff
@@ -1,9 +1,9 @@
 {
     "S2468-1-Initial.xml": "https://gracedb-dev1.ligo.org/api/events/S2468/files/S2468-1-Initial.xml",
-    "cWB.fits.gz": "https://gracedb-playground.ligo.org/api/events/S2468/files/cWB.fits.gz",
-    "cWB.fits.gz,0": "https://gracedb-playground.ligo.org/api/events/S2468/files/cWB.fits.gz,0",
+    "cwb.multiorder.fits": "https://gracedb-playground.ligo.org/api/events/S2468/files/cwb.multiorder.fits",
+    "cwb.multiorder.fits,0": "https://gracedb-playground.ligo.org/api/events/S2468/files/cwb.multiorder.fits",
     "event.log": "https://gracedb-playground.ligo.org/api/events/S2468/files/event.log",
     "event.log,0": "https://gracedb-playground.ligo.org/api/events/S2468/files/event.log,0",
     "trigger_1227349206.7390.txt": "https://gracedb-playground.ligo.org/api/events/S2468/files/trigger_1227349206.7390.txt",
     "trigger_1227349206.7390.txt,0": "https://gracedb-playground.ligo.org/api/events/S2468/files/trigger_1227349206.7390.txt,0"
 }
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/voevents.json` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

 * *Files 18% similar despite different names*

#### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

```diff
@@ -1,39 +1,39 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S2468-1-Initial">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S5678-2-Update">
   <Who>
-    <Date>2018-06-28T13:42:02</Date>
+    <Date>2018-06-28T14:42:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
     </Param>
     <Param name="Pkt_Ser_Num" dataType="string" value="1"/>
-    <Param name="SupereventID" dataType="string" value="S2468" ucd="meta.id">
+    <Param name="SupereventID" dataType="string" value="S5678" ucd="meta.id">
       <Description>Identifier in GraceDB</Description>
     </Param>
-    <Param name="AlertType" dataType="string" value="Initial" ucd="meta.version" unit="">
+    <Param name="AlertType" dataType="string" value="Update" ucd="meta.version" unit="">
       <Description>VOEvent alert type</Description>
     </Param>
     <Param name="Retraction" dataType="string" value="false" ucd="meta.code" unit="">
       <Description>Set to true if the event is retracted.</Description>
     </Param>
     <Param name="HardwareInj" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is a hardware injection if 1, no if 0</Description>
     </Param>
-    <Param name="Vetted" dataType="int" value="0" ucd="meta.number" unit="">
+    <Param name="Vetted" dataType="int" value="1" ucd="meta.number" unit="">
       <Description>Indicates whether this candidate has undergone basic vetting by humans</Description>
     </Param>
     <Param name="OpenAlert" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is an open alert if 1, no if 0</Description>
     </Param>
-    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S2468/view/" ucd="meta.ref.url">
+    <Param name="SupereventPage" dataType="string" value="https://gracedb-playground.ligo.org/superevents/S5678/view/" ucd="meta.ref.url">
       <Description>Web page for evolving status of this GW candidate</Description>
     </Param>
     <Param name="Instruments" dataType="string" value="H1,L1" ucd="meta.code">
       <Description>List of instruments used in analysis to identify this event</Description>
     </Param>
     <Param name="FAR" dataType="float" value="9.11069936486e-14" ucd="arith.rate;stat.falsealarm" unit="Hz">
       <Description>False alarm rate for GW candidates with this strength or greater</Description>
@@ -43,30 +43,60 @@
     </Param>
     <Param name="Pipeline" dataType="string" value="gstlal" ucd="meta.code" unit="">
       <Description>Low-latency data analysis pipeline</Description>
     </Param>
     <Param name="Search" dataType="string" value="MDC" ucd="meta.code" unit="">
       <Description>Specific low-latency search</Description>
     </Param>
-    <Group type="GW_SKYMAP" name="cWB">
-      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S2468/files/cWB.fits.gz" ucd="meta.ref.url" unit="">
+    <Param dataType="int" name="Significant" ucd="meta.number" value="0">
+      <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
+    </Param>
+    <Group name="External Coincidence" type="External Coincidence">
+      <Param name="External_GCN_Notice_Id" value="1364244245" ucd="meta.id" dataType="string">
+        <Description>GCN trigger ID of external event</Description>
+      </Param>
+      <Param name="External_Ivorn" value="ivo://lvk.internal/AGILE#O3-replay_event2023-03-30T20:43:47.992Z" ucd="meta.id" dataType="string">
+        <Description>IVORN of external event</Description>
+      </Param>
+      <Param name="External_Observatory" value="AGILE" ucd="meta.code" dataType="string">
+        <Description>External Observatory</Description>
+      </Param>
+      <Param name="External_Search" value="GRB" ucd="meta.code" dataType="string">
+        <Description>External astrophysical search</Description>
+      </Param>
+      <Param name="Time_Difference" value="2.1" ucd="meta.code" dataType="float">
+        <Description>Time difference between GW candidate and external event, centered on the GW candidate</Description>
+      </Param>
+      <Param name="Time_Coincidence_FAR" value="3.8934000570776255e-13" unit="Hz" ucd="arith.rate;stat.falsealarm" dataType="float">
+        <Description>Estimated coincidence false alarm rate in Hz using timing</Description>
+      </Param>
+      <Param name="Time_Sky_Position_Coincidence_FAR" value="9.640269821382047e-11" unit="Hz" ucd="arith.rate;stat.falsealarm" dataType="float">
+        <Description>Estimated coincidence false alarm rate in Hz using timing and sky position</Description>
+      </Param>
+      <Param name="joint_skymap_fits" value="https://gracedb-playground.ligo.org/api/superevents/S230330ax/files/combined-ext.fits.gz,1" ucd="meta.ref.url" dataType="string">
+        <Description>Combined GW-External Sky Map FITS</Description>
+      </Param>
+      <Description>Properties of joint coincidence found by RAVEN</Description>
+    </Group>
+    <Group type="GW_SKYMAP" name="LALInference">
+      <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S5678/files/bilby.fits.gz,0" ucd="meta.ref.url" unit="">
         <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time>
             <TimeInstant>
-              <ISOTime>2018-06-28T13:35:16.911085</ISOTime>
+              <ISOTime>2018-06-28T14:35:16.911085</ISOTime>
             </TimeInstant>
           </Time>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/tool.py` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/tool.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/__init__.py` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,125 +10,135 @@
 import healpy as hp
 import lxml.etree
 import numpy as np
 from astropy.io.fits import getheader
 from ligo.gracedb import rest
 from ligo.skymap.io.fits import read_sky_map
 from ligo.skymap.postprocess.ellipse import find_ellipse
-from ligo.skymap.postprocess.find_injection import find_injection_moc
+from ligo.skymap.postprocess.crossmatch import crossmatch
 
 from .jinja import env
 from ._version import get_versions
 
 __version__ = get_versions()['version']
 del get_versions
 
 
 def authors(authors, service=rest.DEFAULT_SERVICE_URL):
     """Write GCN Circular author list"""
     return env.get_template('authors.jinja2').render(authors=authors).strip()
 
 
 def guess_skyloc_pipeline(comments):
-    comments = comments.upper()
-    skyloc_pipelines = ['cWB', 'BAYESTAR', 'LIB', 'LALInference', 'UNKNOWN']
+    skyloc_pipelines = ['cWB', 'BAYESTAR', 'Bilby', 'LIB', 'LALInference',
+                        'oLIB', 'MLy', 'UNKNOWN']
     for skyloc_pipeline in skyloc_pipelines:
-        if skyloc_pipeline.upper() in comments:
+        if skyloc_pipeline.upper() in comments.upper():
             break
     return skyloc_pipeline
 
 
 def main_dict(gracedb_id, client):
     """Create general dictionary to pass to compose circular"""
 
     event = client.superevent(gracedb_id).json()
-    preferred_event_id = event['preferred_event']
-    preferred_event = client.event(preferred_event_id).json()
+    preferred_event = event['preferred_event_data']
     preferred_pipeline = preferred_event['pipeline']
-    gw_events = event['gw_events']
-    other_pipelines = []
+    other_pipelines = list(event["pipeline_preferred_events"].keys())
+    other_pipelines.remove(preferred_pipeline)
 
-    for gw_event in gw_events:
-        pipeline = client.event(gw_event).json()['pipeline']
-        if pipeline not in other_pipelines and pipeline != preferred_pipeline:
-            other_pipelines.append(pipeline)
     voevents = client.voevents(gracedb_id).json()['voevents']
-    log = client.logs(gracedb_id).json()['log']
+    if not voevents:
+        raise ValueError(
+            "{} has no VOEvent to generate circulars from.".format(
+                gracedb_id))
+
+    pipelines = [preferred_pipeline] + other_pipelines
+    citation_index = {pipeline.lower(): pipelines.index(pipeline) + 1 for
+                      pipeline in pipelines}
 
     gpstime = float(preferred_event['gpstime'])
     event_time = astropy.time.Time(gpstime, format='gps').utc
 
+    # Grab latest p_astro and em_bright files
+    superevent_files = client.files(gracedb_id).json()
+    em_brightfilename = 'em_bright'
+    p_astrofilename = 'p_astro'
+    em_brightfiles = []
+    p_astrofiles = []
+
+    for file in superevent_files:
+        if em_brightfilename in file and '.png' not in file:
+            em_brightfiles.append(file)
+        elif p_astrofilename in file and '.png' not in file:
+            p_astrofiles.append(file)
+
+    if em_brightfiles:
+        source_classification = client.files(
+            gracedb_id, em_brightfiles[-1]).json()
+        source_classification = {
+            key: 100 * value for key, value in source_classification.items()}
+        citation_index['em_bright'] = max(citation_index.values()) + 1
+    else:
+        source_classification = {}
+
+    if p_astrofiles:
+        classifications = client.files(
+            gracedb_id, p_astrofiles[-1]).json()
+        classifications = {
+            key: 100 * value for key, value in classifications.items()}
+    else:
+        classifications = {}
+
     skymaps = {}
     for voevent in voevents:
         voevent_text = client.files(gracedb_id, voevent['filename']).read()
         root = lxml.etree.fromstring(voevent_text)
         alert_type = root.find(
             './What/Param[@name="AlertType"]').attrib['value'].lower()
         url = root.find('./What/Group/Param[@name="skymap_fits"]')
         if url is None:
             continue
         url = url.attrib['value']
         _, filename = os.path.split(url)
         skyloc_pipeline = guess_skyloc_pipeline(filename)
         issued_time = astropy.time.Time(root.find('./Who/Date').text).datetime
         if filename not in skymaps:
-            for message in log:
-                if filename == message['filename']:
-                    tag_names = message['tag_names']
-                    if 'sky_loc' in tag_names and 'public' in tag_names:
-                        skymaps[filename] = dict(
-                            alert_type=alert_type,
-                            pipeline=skyloc_pipeline,
-                            filename=filename,
-                            latency=issued_time-event_time.datetime)
-                    break
+            skymaps[filename] = dict(
+                alert_type=alert_type,
+                pipeline=skyloc_pipeline,
+                filename=filename,
+                latency=issued_time-event_time.datetime)
+            if skyloc_pipeline.lower() not in citation_index:
+                citation_index[skyloc_pipeline.lower()] = \
+                    max(citation_index.values()) + 1
     skymaps = list(skymaps.values())
-    preferred_event_files = client.files(preferred_event_id).json()
-    em_brightfile = 'em_bright.json'
-    if em_brightfile in preferred_event_files:
-        source_classification = client.files(
-            preferred_event_id, em_brightfile).json()
-        source_classification = {
-            key: 100 * value for key, value in source_classification.items()}
-
-    else:
-        source_classification = {}
-
-    # adding the p_atro informations if available
-    p_astro_file = 'p_astro.json'
-    if p_astro_file in preferred_event_files:
-        classifications = client.files(preferred_event_id, p_astro_file).json()
-
-        # Convert to percent for consistency with em_bright
-        classifications = {
-            key: 100 * value for key, value in classifications.items()}
-    else:
-        classifications = {}
 
     o = urllib.parse.urlparse(client.service_url)
 
     kwargs = dict(
         subject='Identification',
         gracedb_id=gracedb_id,
         gracedb_service_url=urllib.parse.urlunsplit(
             (o.scheme, o.netloc, '/superevents/', '', '')),
         group=preferred_event['group'],
         pipeline=preferred_pipeline,
         other_pipelines=other_pipelines,
-        all_pipelines=[preferred_pipeline] + other_pipelines,
+        all_pipelines=pipelines,
         gpstime='{0:.03f}'.format(round(float(preferred_event['gpstime']), 3)),
         search=preferred_event.get('search', ''),
         far=preferred_event['far'],
         utctime=event_time.iso,
         instruments=preferred_event['instruments'].split(','),
         skymaps=skymaps,
         prob_has_ns=source_classification.get('HasNS'),
         prob_has_remnant=source_classification.get('HasRemnant'),
         include_ellipse=None,
-        classifications=classifications)
+        classifications=classifications,
+        citation_index=citation_index)
 
     if skymaps:
         preferred_skymap = skymaps[-1]['filename']
         cl = 90
         include_ellipse, ra, dec, a, b, pa, area, greedy_area = \
             uncertainty_ellipse(gracedb_id, preferred_skymap, client, cl=cl)
         kwargs.update(
@@ -182,91 +192,18 @@
 def compose_raven(gracedb_id, authors=(),
                   service=rest.DEFAULT_SERVICE_URL, client=None):
     """Compose EM_COINC RAVEN GCN Circular draft"""
 
     if client is None:
         client = rest.GraceDb(service)
 
-    event = client.superevent(gracedb_id).json()
-
-    if 'EM_COINC' not in event['labels']:
-        return
-
-    preferred_event_id = event['preferred_event']
-    preferred_event = client.event(preferred_event_id).json()
-    group = preferred_event['group']
-    superevent_far = preferred_event['far']
-    gpstime = float(preferred_event['gpstime'])
-
-    for em_event_id in event['em_events']:
-        em_event = client.event(em_event_id).json()
-        em_event_gpstime = float(em_event['gpstime'])
-        external_pipeline = em_event['pipeline']
-        # FIXME in GraceDb: Even SNEWS triggers have an extra attribute GRB.
-        external_trigger_id = em_event['extra_attributes']['GRB']['trigger_id']
-        snews = (em_event['search'] == 'Supernova')
-        grb = em_event['search'] in ['GRB', 'SubGRB']
-        subthreshold = (em_event['search'] == 'SubGRB')
-
-    o = urllib.parse.urlparse(client.service_url)
-    kwargs = dict(
-        gracedb_service_url=urllib.parse.urlunsplit(
-            (o.scheme, o.netloc, '/superevents/', '', '')),
-        gracedb_id=gracedb_id,
-        group=group,
-        superevent_far=preferred_event['far'],
-        external_pipeline=external_pipeline,
-        external_trigger=external_trigger_id,
-        snews=snews,
-        grb=grb,
-        subthreshold=subthreshold,
-        latency=abs(round(em_event_gpstime-gpstime, 1)),
-        beforeafter='before' if gpstime > em_event_gpstime else 'after')
-
-    if grb:
-        # Grab GRB coincidence FARs
-        files = client.files(gracedb_id).json()
-        coinc_far_file = 'coincidence_far.json'
-        if coinc_far_file in files:
-            coincidence_far = client.files(gracedb_id, coinc_far_file).json()
-            time_coinc_far = coincidence_far.get('temporal_coinc_far')
-            space_time_coinc_far = coincidence_far.get(
-                'spatiotemporal_coinc_far')
-            kwargs.update(
-                time_coinc_far=time_coinc_far,
-                space_time_coinc_far=space_time_coinc_far)
-
-        # Find combined sky map for GRB
-        logs = client.logs(gracedb_id).json()['log']
-        for message in reversed(logs):
-            comment = message['comment']
-            filename = message['filename']
-            if (filename.endswith('-gbm.fits.gz')
-                    or 'LVC-Fermi sky map' in comment):
-                cl = 90
-                include_ellipse, ra, dec, a, b, pa, area, greedy_area = \
-                    uncertainty_ellipse(gracedb_id, filename, client, cl=cl)
-                kwargs.update(
-                    combined_skymap=filename,
-                    cl=cl,
-                    combined_skymap_include_ellipse=include_ellipse,
-                    combined_skymap_ra=coord.Longitude(ra*u.deg),
-                    combined_skymap_dec=coord.Latitude(dec*u.deg),
-                    combined_skymap_a=coord.Angle(a*u.deg),
-                    combined_skymap_b=coord.Angle(b*u.deg),
-                    combined_skymap_pa=coord.Angle(pa*u.deg),
-                    combined_skymap_ellipse_area=area,
-                    combined_skymap_greedy_area=greedy_area)
-
+    kwargs = dict()
+    kwargs = _update_raven_parameters(gracedb_id, kwargs, client)
     kwargs.update(main_dict(gracedb_id, client=client))
-    if (group.lower() == 'cbc' and superevent_far < 1 / (60 * 86400)) or \
-            (group.lower() == 'burst' and superevent_far < 1 / (365 * 86400)):
-        kwargs.update(change_significance_statement=False)
-    else:
-        kwargs.update(change_significance_statement=True)
+    kwargs.update(update_alert=False)
 
     subject = (
         env.get_template('RAVEN_subject.jinja2').render(**kwargs)
         .strip())
     body = (
         env.get_template('RAVEN_circular.jinja2').render(**kwargs)
         .strip())
@@ -301,64 +238,95 @@
         pipeline=pipeline,
         external_trigger=external_trigger,
         exclusions=[],
         detections=[])
 
     files = client.files(gracedb_id).json()
 
+    citation_index = {}
+    index = 1
     xpipeline_fap_file = 'false_alarm_probability_x.json'
     if xpipeline_fap_file in files:
         xpipeline_fap = client.files(gracedb_id, xpipeline_fap_file).json()
         online_xpipeline_fap = xpipeline_fap.get('Online Xpipeline')
         if online_xpipeline_fap < 0.001:
-            kwargs['detections'].append('Burst')
+            kwargs['detections'].append('xpipeline')
             kwargs.update(online_xpipeline_fap=online_xpipeline_fap)
         else:
-            kwargs['exclusions'].append('Burst')
+            kwargs['exclusions'].append('xpipeline')
             xpipeline_distances_file = 'distances_x.json'
             xpipeline_distances = client.files(gracedb_id,
                                                xpipeline_distances_file).json()
             burst_exclusion = xpipeline_distances.get('Burst Exclusion')
             kwargs.update(burst_exclusion=burst_exclusion)
+        citation_index['xpipeline'] = index
+        index += 1
 
     pygrb_fap_file = 'false_alarm_probability_pygrb.json'
     if pygrb_fap_file in files:
         pygrb_fap = client.files(gracedb_id, pygrb_fap_file).json()
         online_pygrb_fap = pygrb_fap.get('Online PyGRB')
         if online_pygrb_fap < 0.01:
-            kwargs['detections'].append('CBC')
+            kwargs['detections'].append('pygrb')
             kwargs.update(online_pygrb_fap=online_pygrb_fap)
         else:
-            kwargs['exclusions'].append('CBC')
+            kwargs['exclusions'].append('pygrb')
             pygrb_distances_file = 'distances_pygrb.json'
             pygrb_distances = client.files(gracedb_id,
                                            pygrb_distances_file).json()
             nsns_exclusion = pygrb_distances.get('NSNS Exclusion')
             nsbh_exclusion = pygrb_distances.get('NSBH Exclusion')
             kwargs.update(nsbh_exclusion=nsbh_exclusion,
                           nsns_exclusion=nsns_exclusion)
+        citation_index['pygrb'] = index
+
+    kwargs.update(citation_index=citation_index)
 
     subject = (
         env.get_template('medium_latency_grb_subject.jinja2').render(**kwargs)
         .strip())
     body = (
         env.get_template('medium_latency_grb_circular.jinja2').render(**kwargs)
         .strip())
     return '{0}\n{1}'.format(subject, body)
 
 
 def compose_update(gracedb_id, authors=(),
                    service=rest.DEFAULT_SERVICE_URL,
-                   update_types=['sky_localization', 'p_astro', 'em_bright'],
+                   update_types=['sky_localization', 'p_astro',
+                                 'em_bright', 'raven'],
                    client=None):
     """Compose GCN update circular"""
     if client is None:
         client = rest.GraceDb(service)
 
     kwargs = main_dict(gracedb_id, client=client)
+    kwargs.pop('citation_index', None)
+
+    # Adjust files for update type alert
+    citation_index = {}
+    skymaps = []
+    index = 1
+    if 'em_bright' in update_types or 'sky_localization' in update_types:
+        updated_skymap = kwargs.get('skymaps')[-1]
+        kwargs.update(updated_skymap=updated_skymap)
+        citation_index[updated_skymap['pipeline'].lower()] = index
+        skymaps = [updated_skymap]
+        if 'em_bright' in update_types:
+            index += 1
+            citation_index['em_bright'] = index
+
+    kwargs.update(skymaps=skymaps,
+                  citation_index=citation_index,
+                  all_pipelines=[],
+                  update_alert=True)
+
+    if 'raven' in update_types:
+        kwargs = _update_raven_parameters(gracedb_id, kwargs, client)
+
     kwargs.update(authors=authors)
     kwargs.update(change_significance_statement=False)
     kwargs.update(subject='Update')
     kwargs.update(update_types=update_types)
 
     subject = env.get_template('subject.jinja2').render(**kwargs).strip()
     body = env.get_template(
@@ -368,20 +336,25 @@
 
 def compose_retraction(gracedb_id, authors=(),
                        service=rest.DEFAULT_SERVICE_URL, client=None):
     """Compose GCN retraction circular"""
     if client is None:
         client = rest.GraceDb(service)
     event = client.superevent(gracedb_id).json()
-    preferred_event = client.event(event['preferred_event']).json()
+    preferred_event = event['preferred_event_data']
+    labels = event['labels']
+    earlywarning = \
+        ('EARLY_WARNING' in labels and
+         {'EM_SelectedConfident', 'SIGNIF_LOCKED'}.isdisjoint(labels))
 
     kwargs = dict(
                  subject='Retraction',
                  gracedb_id=gracedb_id,
                  group=preferred_event['group'],
+                 earlywarning=earlywarning,
                  authors=authors
              )
 
     subject = env.get_template('subject.jinja2').render(**kwargs).strip()
     body = env.get_template('retraction.jinja2').render(**kwargs).strip()
     return '{0}\n{1}'.format(subject, body)
 
@@ -436,24 +409,150 @@
     joint_areas = [(mask & masks[-1]).sum() * deg2perpix for mask in masks]
 
     kwargs = dict(params=zip(filenames, pipelines, areas, joint_areas))
 
     return env.get_template('compare_skymaps.jinja2').render(**kwargs)
 
 
-def uncertainty_ellipse(graceid, filename, client, cl=90):
-    """Compute uncertainty ellipses for a given sky map"""
+def uncertainty_ellipse(graceid, filename, client, cl=90,
+                        ratio_ellipse_cl_areas=1.35):
+    """Compute uncertainty ellipses for a given sky map
+
+    Parameters
+    ----------
+    graceid: str
+        ID of the trigger used by GraceDB
+    filename: str
+        File name of sky map
+    client: class
+        REST API client for HTTP connection
+    cl: float
+        Percentage of minimal credible area
+    ratio_ellipse_cl_areas: float
+        Ratio between ellipse area and minimal credible area from cl
+    """
     if filename.endswith('.gz'):
         # Try using the multi-res sky map if it exists
         try:
             new_filename = filename.replace('.fits.gz', '.multiorder.fits')
             skymap = read_map_gracedb(graceid, new_filename, client)
         except (IOError, rest.HTTPError):
             skymap = read_map_gracedb(graceid, filename, client)
     else:
         skymap = read_map_gracedb(graceid, filename, client)
 
-    result = find_injection_moc(skymap, contours=[cl / 100])
+    result = crossmatch(skymap, contours=[cl / 100])
     greedy_area = result.contour_areas[0]
     ra, dec, a, b, pa, ellipse_area = find_ellipse(skymap, cl=cl)
-    return ellipse_area <= 1.35*greedy_area, ra, dec, a, b, pa, \
-        ellipse_area, greedy_area
+    return ellipse_area <= ratio_ellipse_cl_areas*greedy_area, ra, dec, a, b, \
+        pa, ellipse_area, greedy_area
+
+
+def _update_raven_parameters(gracedb_id, kwargs, client):
+    """Update kwargs with parameters for RAVEN coincidence"""
+
+    event = client.superevent(gracedb_id).json()
+
+    if 'EM_COINC' not in event['labels']:
+        raise ValueError("No EM_COINC label for {}".format(gracedb_id))
+
+    preferred_event = event['preferred_event_data']
+    group = preferred_event['group']
+    gpstime = float(preferred_event['gpstime'])
+    event_time = astropy.time.Time(gpstime, format='gps').utc
+
+    em_event_id = event['em_type']
+    em_event = client.event(em_event_id).json()
+    em_event_gpstime = float(em_event['gpstime'])
+    external_pipeline = em_event['pipeline']
+    # Get all other pipelines, removing duplicates
+    other_ext_pipelines = \
+        [*set(client.event(id).json()['pipeline'] for id
+              in event['em_events'])]
+    # Remove preferred pipeline
+    other_ext_pipelines.remove(external_pipeline)
+    # FIXME in GraceDb: Even SNEWS triggers have an extra attribute GRB.
+    external_trigger_id = em_event['extra_attributes']['GRB']['trigger_id']
+    snews = (em_event['search'] == 'Supernova')
+    grb = em_event['search'] in ['GRB', 'SubGRB', 'SubGRBTargeted', 'MDC']
+    subthreshold = em_event['search'] in ['SubGRB', 'SubGRBTargeted']
+    subthreshold_targeted = em_event['search'] == 'SubGRBTargeted'
+    far_grb = em_event['far']
+
+    o = urllib.parse.urlparse(client.service_url)
+    kwargs.update(
+        gracedb_service_url=urllib.parse.urlunsplit(
+            (o.scheme, o.netloc, '/superevents/', '', '')),
+        gracedb_id=gracedb_id,
+        group=group,
+        external_pipeline=external_pipeline,
+        external_trigger=external_trigger_id,
+        snews=snews,
+        grb=grb,
+        subthreshold=subthreshold,
+        subthreshold_targeted=subthreshold_targeted,
+        other_ext_pipelines=other_ext_pipelines,
+        far_grb=far_grb,
+        latency=abs(round(em_event_gpstime-gpstime, 1)),
+        beforeafter='before' if gpstime > em_event_gpstime else 'after')
+
+    if grb:
+        # Grab GRB coincidence FARs
+        time_coinc_far = event['time_coinc_far']
+        space_time_coinc_far = event['space_coinc_far']
+        kwargs.update(
+            time_coinc_far=time_coinc_far,
+            space_time_coinc_far=space_time_coinc_far,
+            ext_ra=em_event['extra_attributes']['GRB']['ra'],
+            ext_dec=em_event['extra_attributes']['GRB']['dec'],
+            ext_error=em_event['extra_attributes']['GRB']['error_radius'])
+
+        # Find combined sky maps for GRB
+        voevents = client.voevents(gracedb_id).json()['voevents']
+        combined_skymaps = {}
+        if not voevents:
+            raise ValueError(
+                "{} has no VOEvent to generate circulars from.".format(
+                    gracedb_id))
+        for i, voevent in enumerate(voevents):
+            voevent_text = client.files(gracedb_id, voevent['filename']).read()
+            root = lxml.etree.fromstring(voevent_text)
+            alert_type = root.find(
+                './What/Param[@name="AlertType"]').attrib['value'].lower()
+            # Check if significant GW alert already queued or sent
+            change_significance_statement = \
+                {'EM_SelectedConfident', 'SIGNIF_LOCKED'}.isdisjoint(
+                    event['labels'])
+            url = root.find('./What/Group/Param[@name="joint_skymap_fits"]')
+            if url is None:
+                continue
+            url = url.attrib['value']
+            _, filename = os.path.split(url)
+            issued_time = astropy.time.Time(
+                              root.find('./Who/Date').text).datetime
+            if filename not in combined_skymaps:
+                combined_skymaps[filename] = dict(
+                    alert_type=alert_type,
+                    filename=filename,
+                    latency=issued_time-event_time.datetime)
+
+        if combined_skymaps:
+            combined_skymaps = list(combined_skymaps.values())
+            combined_skymap = combined_skymaps[-1]['filename']
+            cl = 90
+            include_ellipse, ra, dec, a, b, pa, area, greedy_area = \
+                uncertainty_ellipse(gracedb_id, combined_skymap, client, cl=cl)
+            kwargs.update(
+                combined_skymap=combined_skymap,
+                combined_skymaps=combined_skymaps,
+                cl=cl,
+                combined_skymap_include_ellipse=include_ellipse,
+                combined_skymap_ra=coord.Longitude(ra*u.deg),
+                combined_skymap_dec=coord.Latitude(dec*u.deg),
+                combined_skymap_a=coord.Angle(a*u.deg),
+                combined_skymap_b=coord.Angle(b*u.deg),
+                combined_skymap_pa=coord.Angle(pa*u.deg),
+                combined_skymap_ellipse_area=area,
+                combined_skymap_greedy_area=greedy_area,
+                change_significance_statement=change_significance_statement)
+
+    return kwargs
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/jinja.py` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/jinja.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 import humanize.number
 import humanize.time
 import jinja2
 
 __all__ = ('env',)
 
 env = jinja2.Environment(
-    loader=jinja2.PackageLoader(__name__, 'templates'),
+    loader=jinja2.PackageLoader(__package__, 'templates'),
     # The options below are suggested by the Chromium Jinja style guide,
     # https://www.chromium.org/developers/jinja.
     keep_trailing_newline=True,  # newline-terminate generated files
-    lstrip_blocks=True,  # so can indent control flow tags
+    lstrip_blocks=False,  # so can preserve whitespace at the state of line
     trim_blocks=True,  # so don't need {%- -%} everywhere
     extensions=['jinja2.ext.loopcontrols']
 )
 
 _rewrap_regex = re.compile(
     r'^[ \t]+.+\n|([^ \t\n]+[^\n]*\n)+|.*',
     flags=re.MULTILINE)
 
 
 def rewrap(text):
-    """Rewrap the given text, paragraph by paragraph. Treat any line that begins
-    with whitespace as a separate paragraph, and any consecutive sequence of
-    lines that do not begin with whitespace as a paragraph."""
+    """Rewrap the given text, paragraph by paragraph. Treat any line that
+    begins with whitespace as a separate paragraph, and any consecutive
+    sequence of lines that do not begin with whitespace as a paragraph."""
     return '\n'.join(textwrap.fill(text[match.start():match.end()])
                      for match in _rewrap_regex.finditer(text))
 
 
 env.filters['log10'] = math.log10
 env.filters['rewrap'] = rewrap
 env.filters['apnumber'] = humanize.number.apnumber
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/update_circular.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/update_circular.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,28 @@
                                naturalinstruments, renamegroup %}
 
 {% include 'authors.jinja2' %}
 
 {% filter rewrap %}
 We have conducted further analysis of the {{naturalinstruments(instruments)}} data around
 the time of the {{renamegroup(group)}} ({{(group)}}) candidate {{gracedb_id}}
-(GCN ***CITE ORIGINAL GCN ID, e.g. 25012***). {% if skymaps|length != 0 and 'sky_localization' in update_types %}
+(GCN Circular ***CITE ORIGINAL GCN ID, e.g. 25012***). {% if skymaps|length != 0 and 'sky_localization' in update_types %}
 Parameter estimation has been performed using
-{{citeskymap(skymaps[-1].pipeline, [], [skymaps[-1]])}} and a new sky map, {{preferred_skymap}},
+{{citeskymap(updated_skymap.pipeline, citation_index)}} and a new sky map, {{preferred_skymap}},
 distributed via GCN Notice, is available for retrieval from the
 GraceDB event page:
 
 {{ gracedb_service_url }}{{ gracedb_id }}
 {% else %}
 
 {% endif %}
 
-{% if skymaps|length != 0 and 'sky_localization' in update_types %}{%- include 'skymap_info.jinja2' -%}{% endif %}
-{% if 'em_bright' in update_types %}{% include 'em_bright.jinja2' %}{% endif %}
 {% if 'p_astro' in update_types %}{% include 'p_astro.jinja2' %}{% endif %}
+{% if 'em_bright' in update_types %}{% include 'em_bright.jinja2' %}{% endif %}
+{% if skymaps|length != 0 and 'sky_localization' in update_types %}{%- include 'skymap_info.jinja2' -%}{% endif %}
+{% if 'raven' in update_types %}{% include 'RAVEN_circular.jinja2' %}{% endif %}
 {% include 'userguide_conclusion.jinja2' %}
 
-{% if (skymaps|length != 0 and 'sky_localization' in update_types) or ('p_astro' in update_types) %}
-{{citenumberedpipelines([], [skymaps[-1]])}}
+{% if (skymaps|length != 0 and 'sky_localization' in update_types) or ('em_bright' in update_types) %}
+{% include 'numbered_pipeline_citations.jinja2' %}
 {% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/initial_body.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/initial_body.jinja2`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 {% from 'macros.jinja2' import oxford_commas, evidence_for, probability,
                             naturalinstruments, naturalfar,
                             naturalclassifications, naturalotherpipelines,
                             renamegroup, citeskymap %}
 {% filter rewrap %}
 We identified the {{renamegroup(group)}} candidate {{gracedb_id}} during real-time processing of data from
-{{naturalinstruments(instruments)}} at {{utctime}} UTC (GPS time: {{gpstime}}).
-The candidate was found by the {{naturalotherpipelines(pipeline, other_pipelines)}}
+{{naturalinstruments(instruments, )}} at {{utctime}} UTC (GPS time: {{gpstime}}).
+The candidate was found by the {{naturalotherpipelines(pipeline, other_pipelines, citation_index)}}
 analysis pipeline{% if ([pipeline] + other_pipelines)|length > 1 %}s{% endif %}.
 
 {% if change_significance_statement %}
-This gravitational wave candidate is not significant enough on its own to produce a public alert
-but its coincidence with the {% if snews %}SNEWS neutrino{% endif %}{% if grb %}GRB{% endif %} trigger increases its significance.
+Based on the analysis of gravitational-wave data alone, this candidate does not meet our criteria for a high-significance public alert.
+However, a search performed by the RAVEN pipeline found a significant coincidence between this candidate and {{external_trigger}}.
 {% else %}
 {{gracedb_id}} is an event of interest because its false alarm rate, as
 estimated by the online analysis, is {{naturalfar(far)}}.
 {% endif %}
 The event's properties can be found at this URL:
 {{ gracedb_service_url }}{{ gracedb_id }}
 
-{% if not grb and classifications|length > 0 %}
+{% if not update_alert %}
+{% if classifications|length > 0 %}
 {%- include 'p_astro.jinja2' -%}
 {% endif %}
-{% if not grb and prob_has_ns is not none %}
+{% if prob_has_ns is not none %}
 {%- include 'em_bright.jinja2' -%}
 {% endif %}
 {% if skymaps|length == 0 %}
 No{% else %}{{ skymaps|length|apnumber|capitalize }}{% endif %} {% if combined_skymap is not defined %}sky map{% else %}GW-only sky map{% endif %}{% if skymaps|length == 1 %} is{% else %}s are{% endif %} available at this time{% if skymaps|length > 0 %} and can be retrieved from the GraceDB event page:{% else %}.{% endif %}
 
 {% for skymap in skymaps %}
- * {{skymap.filename}}, an {% if skymap.alert_type == 'initial' %}initial{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, all_pipelines, skymaps)}}, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate
+ * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, citation_index)}}, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate event time.
 {% endfor %}
 
 {% if skymaps|length != 0 %}{%- include 'skymap_info.jinja2' -%}{% endif %}
+{% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/skymap_info.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/skymap_info.jinja2`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 {% if not include_ellipse %}
 {{greedy_area|round|int}} deg2.
 {% else %}
 well fit by an ellipse with an area of {{ellipse_area|round|int}} deg2 described
 by the following DS9 region (right ascension, declination, semi-major axis,
 semi-minor axis, position angle of the semi-minor axis):
    icrs; ellipse(
-      {{- ra.to('15 arcsec').round().to_string(unit='hourangle', pad=True,
-                                               alwayssign=False) }},
-      {{- ' ' }}{{ dec.to('arcsec').round().to_string(unit='deg', pad=True,
-                                                      alwayssign=True) }},
-      {{- ' ' }}{{ a.round().to_string(fields=1, unit='deg') }},
-      {{- ' ' }}{{ b.round().to_string(fields=1, unit='deg') }},
-      {{- ' ' }}{{ pa.round().to_string(fields=1, unit='deg') }})
+      {{- ra.to_string(unit='hourangle', fields=2, pad=True, alwayssign=False) }},
+      {{- ' ' }}{{ dec.to_string(unit='deg', fields=2, pad=True, alwayssign=True) }},
+      {{- ' ' }}{{ a.to_string(unit='deg', precision=2, decimal=True) }}d,
+      {{- ' ' }}{{ b.to_string(unit='deg', precision=2, decimal=True) }}d,
+      {{- ' ' }}{{ pa.to_string(unit='deg', precision=2, decimal=True) }}d)
 {% endif %}
 {% if distmu %}
 Marginalized over the whole sky, the a posteriori luminosity distance estimate is {{distmu|round|int}} +/- {{distsig|round|int}} Mpc (a posteriori mean +/- standard deviation).
 {% endif %}
 
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/macros.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/macros.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 %
 {%- endmacro %}
 
 
 Macro to write Update type in natural-language
 
 {% macro naturalupdatetype(update_type) %}
-{% if 'sky_localization' == update_type|lower %}Sky Localization{% elif 'p_astro' == update_type|lower %}Source Classification
-{% elif 'em_bright' == update_type|lower %}EM Bright Classification{% endif %}
+{% if 'sky_localization' == update_type|lower %}Sky localization{% elif 'p_astro' == update_type|lower %}Source Classification{% elif 'em_bright' == update_type|lower %}EM Bright Classification{% elif 'raven' == update_type|lower %}Coincidence with External Event{% endif %}
 {%- endmacro %}
 
 
 Macro to write Update type subject
 {% macro naturalupdatesubject(update_types) %}
 {% if update_types|length == 1 %}{{naturalupdatetype(update_types[0])}}
 {% elif update_types|length == 2 %}{{naturalupdatetype(update_types[0])}} and {{naturalupdatetype(update_types[1])}}
@@ -64,15 +63,16 @@
 Macro to transform a list like ['H1', 'L1', 'V1'] to natural-language list like
 "H1 (LIGO Hanford Observatory), L1 (LIGO Livingston Observatory), and V1 (Virgo
 Observatory)".
 
 {% macro naturalinstruments(instruments) %}
 {% set long_instruments = {'H1': 'LIGO Hanford Observatory',
                            'L1': 'LIGO Livingston Observatory',
-                           'V1': 'Virgo Observatory'} %}
+                           'V1': 'Virgo Observatory',
+                           'K1': 'KAGRA Observatory'} %}
 {% call(instrument) oxford_commas(instruments) %}
 {% if instrument in long_instruments %}
 {{long_instruments[instrument]}} ({{instrument}})
 {%- else %}
 {{instrument}}
 {%- endif %}
 {%- endcall %}
@@ -80,85 +80,75 @@
 
 
 {% set skymapcitationnumber = namespace(count=0) %}
 
 Macro to cite sky maps. Since citations are enumerated, the citation number must start with
 number of all GW analysis pipelines + 1.
 
-{% macro citeskymap(skymappipeline, all_pipelines, skymaps) %}
-{% set skymapcitationnumber.count = 0 %}
-{% for skymap in skymaps %}
-{% if skymap.pipeline|lower in skymapcitations %}{% set skymapcitationnumber.count = skymapcitationnumber.count + 1 %}{% endif %}
-{% if skymap.pipeline == skymappipeline %}{% break %}{% endif %}
-{% endfor %}
-{{skymappipeline}}{% if skymappipeline|lower in skymapcitations %} [{{ all_pipelines|length + skymapcitationnumber.count }}]
+{% macro citeskymap(skymappipeline, citation_index) %}
+{{skymappipeline}}{% if skymappipeline|lower in citations %} [{{ citation_index[skymappipeline|lower] }}]
 {%- endif -%}
 {%- endmacro %}
 
 
 Macro to simply write the citation number of a skymap in brackets.
 
-{% macro citeskymap_number(skymappipeline, all_pipelines, skymaps) %}
-{% set skymapcitationnumber.count = 0 %}
-{% for skymap in skymaps %}
-{% if skymap.pipeline|lower in skymapcitations %}{% set skymapcitationnumber.count = skymapcitationnumber.count + 1 %}{% endif %}
-{% if skymap.pipeline == skymappipeline %}{% break %}{% endif %}
-{% endfor %}
-{% if skymappipeline|lower in skymapcitations %}[{{ all_pipelines|length + skymapcitationnumber.count }}]
+{% macro citeskymap_number(skymappipeline, citation_index) %}
+{% if skymappipeline|lower in citations %}[{{ citation_index[skymappipeline|lower] }}]
 {%- endif -%}
 {%- endmacro %}
 
 
 Macro to transform a list of other GW analysis pipelines like ['gstlal', 'mbtaonline', 'pycbc']
 to a natural-language list like "gstlal [2], mbtaonline [3], and pycbc [4]".
 
-{% macro naturalotherpipelines(preferred_pipeline, other_pipelines, conjunction='and') %}
+{% macro naturalotherpipelines(preferred_pipeline, other_pipelines, citation_index, conjunction='and') %}
 {% for pipeline in [preferred_pipeline] + other_pipelines %}
-{% if 'pycbc' == pipeline|lower %}PyCBC Live{% elif 'gstlal' == pipeline|lower %}GstLAL{% elif 'spiir' == pipeline|lower %}SPIIR{% else %}{{pipeline}}{% endif %} [{{loop.index}}]
+{% if 'pycbc' == pipeline|lower %}PyCBC Live{% elif 'gstlal' == pipeline|lower %}GstLAL{% elif 'spiir' == pipeline|lower %}SPIIR{% else %}{{pipeline}}{% endif %} [{{citation_index[pipeline|lower]}}]
 {%- if loop.length > 2 and not loop.last %},{% endif %}
 {%- if loop.length > 1 and not loop.last %} {% endif %}
 {%- if loop.length > 1 and loop.revindex == 2 %}{{conjunction}} {% endif %}
 {% endfor %}
 {%- endmacro %}
 
 
 Macro to enumerate and cite all GW analysis pipelines involved for the superevent; including the
 skymap pipelines.
 
-{%- macro citenumberedpipelines(all_pipelines, skymaps) -%}
-{% for pipeline in all_pipelines %}
-{% if pipeline == 'Burst'%}
- [{{loop.index}}] {{citations['xpipeline']}}
-{% elif pipeline == 'CBC'%}
- [{{loop.index}}] {{citations['pygrb']}}
-{% else %}
- [{{loop.index}}] {{citations[pipeline|lower]}}
-{% endif %}
-{% endfor %}
-{% set skymapcitationnumber.count = 0 %}
-{% for skymap in skymaps %}
-{% if skymap.pipeline|lower in skymapcitations %} {% set skymapcitationnumber.count = skymapcitationnumber.count + 1 %}
-[{{ all_pipelines|length + skymapcitationnumber.count }}] {{skymapcitations[skymap.pipeline|lower]}}
-{% endif %}
+{%- macro citenumberedpipelines(citation_index) -%}
+{% for key in citation_index %}
+ [{{ citation_index[key|lower] }}] {{citations[key|lower]}}
 {% endfor %}
 {%- endmacro -%}
 
 
 Macro to transform a list of GRB-GW exclusions/detections like ['CBC', 'Burst'] to a natural-language
 list like "triggered CBC pipeline (PyGRB) [1] and triggered Burst pipeline (X-Pipeline) [2]".
 
-{%- macro naturalgrbmediumlatencypipelines(somelist) -%}
-{% for item in somelist %}
-{% if item == 'Burst' %}X-Pipeline GRB-unmodeled transient analysis{% else %}PyGRB binary merger analysis{% endif %} [{{loop.index}}]
+{%- macro naturalgrbmediumlatencypipelines(pipelines, citation_index) -%}
+{% for pipeline in pipelines %}
+{% if pipeline == 'xpipeline' %}X-Pipeline GRB-unmodeled transient analysis{% elif pipeline == 'pygrb' %}PyGRB binary merger analysis{% endif %} [{{citation_index[pipeline|lower]}}]
 {%- if loop.length > 1 and not loop.last %} {% endif %}
 {%- if loop.length > 1 and loop.revindex == 2 %}and {% endif %}
 {% endfor %}
 {%- endmacro %}
 
 
+Macro to transform a list of other external pipelines like ['Fermi', 'Swift', 'INTEGRAL']
+to a natural-language list like "Fermi-GBM, Swift/BAT, and INTEGRAL".
+
+{% macro naturalotherexternalpipelines(other_pipelines, conjunction='and') %}
+{% for pipeline in other_pipelines %}
+{{grbmission(pipeline)}}
+{%- if loop.length > 2 and not loop.last %},{% endif %}
+{%- if loop.length > 1 and not loop.last %} {% endif %}
+{%- if loop.length > 1 and loop.revindex == 2 %}{{conjunction}} {% endif %}
+{% endfor %}
+{%- endmacro %}
+
 Macro to round FAPs to single decimal place
 
 {% macro naturalfap(fap) %}
 {{'%.1e'|format(fap)}}
 {%- endmacro %}
 
 
@@ -204,15 +194,30 @@
 
 Macro to include which mission reported the GRB.
 
 {%- macro grbmission(external_pipeline) -%}
 {%- if external_pipeline|lower == 'fermi' -%}
 Fermi GBM
 {%- elif external_pipeline|lower == 'swift' -%}
-Swift BAT
+Swift/BAT
+{%- elif external_pipeline|lower == 'agile' -%}
+AGILE MCAL
+{%- else -%}
+{{external_pipeline}}
+{%- endif -%}
+{%- endmacro -%}
+
+
+Macro to include which subthreshold targeted mission reported the GRB.
+
+{%- macro grbmission_targeted(external_pipeline) -%}
+{%- if external_pipeline|lower == 'fermi' -%}
+Fermi GBM
+{%- elif external_pipeline|lower == 'swift' -%}
+Swift/BAT-GUANO
 {%- else -%}
 {{external_pipeline}}
 {%- endif -%}
 {%- endmacro -%}
 
 
 Macro to include the word `trigger' or not when referring to external_trigger.
@@ -225,20 +230,19 @@
 {%- endif -%}
 {%- endmacro -%}
 
 
 Dictionary of common citations.
 
 {% set citations = {'pycbc': 'Nitz et al. PRD 98, 024050 (2018)',
-                    'mbtaonline': 'Adams et al. CQG 33, 175012 (2016)',
+                    'mbta': 'Adams et al. CQG 33, 175012 (2016)',
                     'gstlal': 'Messick et al. PRD 95, 042001 (2017)',
                     'spiir': 'Qi Chu, PhD Thesis, The University of Western Australia (2017)',
                     'cwb': 'Klimenko et al. PRD 93, 042004 (2016)',
                     'olib': 'Lynch et al. PRD 95, 104046 (2017)',
+                    'mly': 'Skliris et al. arXiv:2009.14611 (2020)',
+                    'em_bright': 'Chatterjee et al. The Astrophysical Journal 896, 1 (2020)',
                     'pygrb': 'Williamson et al. PRD 90, 122004 (2014)',
-                    'xpipeline': 'Was et al. PRD 86, 022003 (2012)'} %}
-
-
-Dictionary of sky map citations.
-
-{% set skymapcitations = {'bayestar': 'Singer & Price PRD 93, 024013 (2016)',
-                          'lalinference': 'Veitch et al. PRD 91, 042003 (2015)'} %}
+                    'xpipeline': 'Was et al. PRD 86, 022003 (2012)',
+                    'bayestar': 'Singer & Price PRD 93, 024013 (2016)',
+                    'bilby': 'Ashton et al. ApJS 241, 27 (2019)',
+                    'lalinference': 'Veitch et al. PRD 91, 042003 (2015)'} %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% from 'macros.jinja2' import naturalgrbmediumlatencypipelines,
                                grbmission, propername %}
 {% filter rewrap %}
-The {{naturalgrbmediumlatencypipelines(exclusions)}} did not find a candidate gravitational wave (GW) event associated with GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
+The {{naturalgrbmediumlatencypipelines(exclusions, citation_index)}} did not find a candidate gravitational wave (GW) event associated with GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 
 Preliminary exclusion distances with the below assumptions:
 
-{% if 'CBC' in exclusions %}
+{% if 'pygrb' in exclusions %}
 NS-NS: {{nsns_exclusion}} Mpc, 90% CL {{'\n'}}
 NS-BH: {{nsbh_exclusion}} Mpc, 90% CL {{'\n'}}
 {% endif %}
-{% if 'Burst' in exclusions %}
+{% if 'xpipeline' in exclusions %}
 Rotational model: {{burst_exclusion}} Mpc, 90% CL {{'\n'}} 
 {% endif %}
 
-{% if 'CBC' in exclusions %}
+{% if 'pygrb' in exclusions %}
 Exclusion distance from a Gaussian distribution of mass, uniform distribution of spin and inclination. NS-NS: a Gaussian distribution of component masses 1-3 M_sun, uniform distributions of spin 0-0.4, and inclination angle up to a maximum of 30 deg. NS-BH: as above for NS; BH mass and spin distributions 3-15 M_sun, 0-0.98.
 {% endif %}
-{% if 'Burst' in exclusions %}
+{% if 'xpipeline' in exclusions %}
 Unmodeled transient exclusion distance from an ad hoc rotational model with a circularly polarized, sine-Gaussian waveform with Q-factor = 9 and center frequency = 150 Hz, assuming E_GW = 10^-2 M_sun c^2 of energy emitted as GWs. Exclusion distance scales roughly as sqrt(E_GW).
 {% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,13 @@
                             naturalclassifications,
                             citations, citenumberedpipelines %}
 {% include 'authors.jinja2' %}
 
 {% filter rewrap %}
 {% if detections|length > 0 %}
 {% include 'medium_latency_grb_detection_circular.jinja2' %}
-{{citenumberedpipelines(detections, [])}}
 {% elif exclusions|length > 0 %}
 {% include 'medium_latency_grb_exclusion_circular.jinja2' %}
-{{citenumberedpipelines(exclusions, [])}}
 {% endif %}
+{% include 'numbered_pipeline_citations.jinja2' %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/RAVEN_circular.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_circular.jinja2`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-{% from 'macros.jinja2' import naturalfar, grbmission, propername %}
-{% include 'authors.jinja2' %}
+{% from 'macros.jinja2' import naturalfar, grbmission, grbmission_targeted, naturalotherexternalpipelines, propername %}
+{% if not update_alert %}{% include 'authors.jinja2' %}
 
 {% include 'initial_body.jinja2' %}
-
+{% endif %}
 {% filter rewrap %}
 A search performed by the RAVEN pipeline found a temporal coincidence between
 {{gracedb_id}} and a {% if snews %}SNEWS supernova{% elif grb %}{% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}}{% endif %} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 The {% if snews %}neutrino{% elif grb %}GRB{% endif %} trigger time is {{latency}} seconds {{beforeafter}} the GW candidate event.
 {% if grb %}
-The estimated joint false alarm rate for the time coincidence is {{naturalfar(time_coinc_far)}}.
-{% endif %}
+The estimated joint false alarm rate for the coincidence using just timing info is {{naturalfar(time_coinc_far)}}.
+{% if subthreshold_targeted %}The GRB candidate was found during a joint targeted search between the LIGO/Virgo/KAGRA collaboration and {{grbmission_targeted(external_pipeline)}}, and has a false alarm rate of {{naturalfar(far_grb)}}. {% endif %}
+{% if other_ext_pipelines %}RAVEN has also identified {% if other_ext_pipelines|length == 1 %}an additional detection{% elif other_ext_pipelines|length > 1%}additional detections{% endif %} from {{naturalotherexternalpipelines(other_ext_pipelines)}}.{% endif %}
 
-{% if grb %}{%- include 'p_astro.jinja2' -%}
 
-{%- include 'em_bright.jinja2' -%}
 {% endif %}
-
-{% if combined_skymap is not defined %}
-{% include 'userguide_conclusion.jinja2'%}
-{% else %}
-A combined sky map is also available:
- * {{combined_skymap}}, the normalized product of the GW and GRB localizations.
+{% if combined_skymap %}
+{% if combined_skymaps|length == 1 %}A combined sky map is{% else %}Combined sky maps are{% endif %} also available:
+{% for skymap in combined_skymaps %}
+ * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% else %}updated{% endif %} localization, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate event time.
+{% endfor %}
 
 For the {{combined_skymap}} sky map, the {{cl}}% credible region is {{combined_skymap_greedy_area|round|int}} deg2.
-{% if space_time_coinc_far is not none %}
+{% endif %}
+{% if external_pipeline|lower == 'swift'%}
+The joint localization is dominated by the {{grbmission(external_pipeline)}} candidate, which was identified with right ascension, declination of {{'%0.3f' % ext_ra|float}}, {{'%0.3f' % ext_dec|float}}{% if ext_error %} and 90% containment error radius of {{'%0.3f' % ext_error|float}} deg{% endif %}.
+{% endif %}
+{% if combined_skymap and space_time_coinc_far is not none %}
 Considering the overlap of the individual sky maps, the estimated joint false alarm rate for the spatial and temporal coincidence is {{naturalfar(space_time_coinc_far)}}.
-{% else %}
+{% elif combined_skymap and space_time_coinc_far is none %}
 The spatial and temporal coincidence is not yet available.
 {% endif %}
 
+{% if not update_alert %}
 {% include 'userguide_conclusion.jinja2'%}
-{% endif %}
 {% include 'numbered_pipeline_citations.jinja2' %}
+{% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% from 'macros.jinja2' import naturalgrbmediumlatencypipelines,
                                naturalfap, grbmission, propername %}
 {% filter rewrap %}
-The {{naturalgrbmediumlatencypipelines(detections)}} made{% if detections|length == 1 %} a{% endif %} preliminary identification of {% if detections|length == 1 %}a {% endif %}gravitational wave (GW) candidate{% if detections|length == 2 %}s{% endif %} associated with the time and sky position of GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
+The {{naturalgrbmediumlatencypipelines(detections, citation_index)}} made{% if detections|length == 1 %} a{% endif %} preliminary identification of {% if detections|length == 1 %}a {% endif %}gravitational wave (GW) candidate{% if detections|length == 2 %}s{% endif %} associated with the time and sky position of GRB {{grbmission(pipeline)}} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 
 {% if detections|length == 2 %}
 In PyGRB, the candidate is consistent with a binary coalescence with False Alarm Probability of {{naturalfap(online_pygrb_fap)}}.
 
 In X-Pipeline, the candidate is an unmodeled GW transient with False Alarm Probability of {{naturalfap(online_xpipeline_fap)}}.
 {% elif detections| length == 1%}
 The candidate is {% if 'Burst' in detections %}an unmodeled GW transient{% else %}consistent with a binary coalescence{% endif %} with False Alarm Probability of {% if 'Burst' in detections %}{{online_xpipeline_fap}}{% else %}{{online_pygrb_fap}}{% endif %}.
```

### Comparing `ligo-followup-advocate-1.1.dev1/ligo/followup_advocate/templates/RAVEN_subject.jinja2` & `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_subject.jinja2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 {% from 'macros.jinja2' import grbmission, renamegroup, propername %}
 {% if not change_significance_statement %}
-SUBJECT: LIGO/Virgo {{gracedb_id}}: Identification of a GW {{renamegroup(group)}} candidate possibly associated with {% if subthreshold %} sub-threshold{% endif %} {{grbmission(external_pipeline)}} {{propername(external_trigger)}}
+SUBJECT: LIGO/Virgo/KAGRA {{gracedb_id}}: Identification of a GW {{renamegroup(group)}} candidate possibly associated with {% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}} {{propername(external_trigger)}}
 {% else %}
-SUBJECT: {{grbmission(external_pipeline)}} {{propername(external_trigger)}}: LIGO/Virgo identification of a possible sub-threshold GW {{renamegroup(group)}} counterpart, {{gracedb_id}}
+SUBJECT: {{grbmission(external_pipeline)}} {{propername(external_trigger)}}: LIGO/Virgo/KAGRA identification of a low-significance GW {{renamegroup(group)}} counterpart, {{gracedb_id}}
 {% if subthreshold%} **NOTE TO ADVOCATES: If our circular is the first one to mention the sub-threshold GRB, please use the subject line:
-SUBJECT: LIGO/Virgo {{gracedb_id}}: Identification of a GW {{renamegroup(group)}} candidate possibly associated with {% if subthreshold %} sub-threshold{% endif %} {{grbmission(external_pipeline)}} {{propername(external_trigger)}}**{% endif %}
+SUBJECT: LIGO/Virgo/KAGRA {{gracedb_id}}: Identification of a GW {{renamegroup(group)}} candidate possibly associated with {% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}} {{propername(external_trigger)}}**{% endif %}
 {% endif %}
```

### Comparing `ligo-followup-advocate-1.1.dev1/setup.py` & `ligo-followup-advocate-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/setup.cfg` & `ligo-followup-advocate-1.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -5,51 +5,53 @@
 source = ligo
 omit = ligo/followup_advocate/test/*
 
 [flake8]
 exclude = 
 	ligo/followup_advocate/_version.py
 	versioneer.py
+ignore = W503,W504,D100,D101,D102,D103,D104,D107,D202,D205,D209,D400,D401,D403,E126,E226
 
 [metadata]
 name = ligo-followup-advocate
 license = GPL-2+
 license_file = COPYING.md
-description = LIGO/Virgo Follow-up Advocate Tools
-long_description = This package provides tools for LIGO/Virgo follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
+description = LIGO/Virgo/KAGRA Follow-up Advocate Tools
+long_description = This package provides tools for LIGO/Virgo/KAGRA follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
 author = Leo Singer
 author_email = leo.singer@ligo.org
+maintainer = Brandon Piotrzkowski
+maintainer_email = brandon.piotrzkowski@ligo.org
 url = https://git.ligo.org/emfollow/ligo-followup-advocate
 classifiers = 
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 	Operating System :: POSIX
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.8
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 scripts = bin/ligo-followup-advocate
 
 [options]
 packages = find:
-python_requires = >= 3.6
-namespace_packages = ligo
+python_requires = >= 3.8
 tests_require = 
 	pytest >= 3.0
 	pytest-mock
 
 [options.entry_points]
 console_scripts = 
 	ligo-followup-advocate = ligo.followup_advocate.tool:main
 
 [options.package_data]
 ligo.followup_advocate.templates = *.jinja2
-ligo.followup_advocate.test = data/*/*.json, data/*/files/*.json, data/*/files/*.xml, data/*/files/*.fits, data/*/files/*.fits.gz, data/*/files/*.data
+ligo.followup_advocate.test = data/*/*.json, data/*/files/*.json, data/*/files/*.xml, data/*/files/*.fits, data/*/files/*.fits.gz, data/*/files/*.data, data/*/files/*.fits.gz*, data/*/files/*.json*
 
 [versioneer]
-vcs = git
+VCS = git
 versionfile_build = ligo/followup_advocate/_version.py
 versionfile_source = ligo/followup_advocate/_version.py
 tag_prefix = v
 parentdir_prefix = ligo-followup-advocate-
 
 [egg_info]
 tag_build =
```

### Comparing `ligo-followup-advocate-1.1.dev1/versioneer.py` & `ligo-followup-advocate-1.2.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/COPYING.md` & `ligo-followup-advocate-1.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.1.dev1/PKG-INFO` & `ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.1.dev1
-Summary: LIGO/Virgo Follow-up Advocate Tools
+Version: 1.2.0
+Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
+Maintainer: Brandon Piotrzkowski
+Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
-Description: This package provides tools for LIGO/Virgo follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >= 3.6
+Requires-Python: >=3.8
+License-File: COPYING.md
+
+This package provides tools for LIGO/Virgo/KAGRA follow-up advocates to assist in tasks such as drafting astronomical bulletins for gravitational-wave detections.
```

### Comparing `ligo-followup-advocate-1.1.dev1/README.md` & `ligo-followup-advocate-1.2.0/README.md`

 * *Files identical despite different names*

