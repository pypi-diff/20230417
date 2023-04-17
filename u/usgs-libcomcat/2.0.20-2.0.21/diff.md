# Comparing `tmp/usgs-libcomcat-2.0.20.tar.gz` & `tmp/usgs-libcomcat-2.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-libcomcat-2.0.20.tar", last modified: Thu Dec 22 00:19:13 2022, max compression
+gzip compressed data, was "usgs-libcomcat-2.0.21.tar", last modified: Mon Apr 17 20:52:32 2023, max compression
```

## Comparing `usgs-libcomcat-2.0.20.tar` & `usgs-libcomcat-2.0.21.tar`

### file list

```diff
@@ -1,197 +1,198 @@
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.513475 usgs-libcomcat-2.0.20/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       97 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/.codecov.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       35 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/.gitattributes
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.413475 usgs-libcomcat-2.0.20/.github/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.423475 usgs-libcomcat-2.0.20/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      706 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      600 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      653 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/.github/ISSUE_TEMPLATE/process-update-request.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      206 2022-12-08 15:39:57.000000 usgs-libcomcat-2.0.20/.gitignore
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1786 2022-12-08 17:00:30.000000 usgs-libcomcat-2.0.20/.gitlab-ci.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      222 2022-11-18 13:39:52.000000 usgs-libcomcat-2.0.20/CODE_OF_CONDUCT.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      736 2022-11-18 23:59:33.000000 usgs-libcomcat-2.0.20/CONTRIBUTING.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2022-11-18 13:39:52.000000 usgs-libcomcat-2.0.20/DISCLAIMER.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2263 2022-11-18 13:39:52.000000 usgs-libcomcat-2.0.20/LICENSE.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7030 2022-12-22 00:19:13.513475 usgs-libcomcat-2.0.20/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3954 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/README.md
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      215 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/clean_vcr
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1191 2022-12-07 15:40:25.000000 usgs-libcomcat-2.0.20/code.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.423475 usgs-libcomcat-2.0.20/docs/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    26400 2022-11-18 23:59:33.000000 usgs-libcomcat-2.0.20/docs/api.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    31339 2022-11-18 23:59:33.000000 usgs-libcomcat-2.0.20/docs/cli.md
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3194 2022-12-22 00:04:16.000000 usgs-libcomcat-2.0.20/install.sh
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3685 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/makedocs.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.433475 usgs-libcomcat-2.0.20/notebooks/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   131214 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/AssociatingCatalogues.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1158324 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/Classes.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    99601 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/ComparingMagnitudes.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   365190 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/Dataframes.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    66223 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/DetailEvent.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   191637 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/EventHistory.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    34125 2022-12-07 15:40:25.000000 usgs-libcomcat-2.0.20/notebooks/GetSMDYFIPairs.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   142968 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/PhasesAndMagnitudes.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   202623 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/Search.ipynb
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.433475 usgs-libcomcat-2.0.20/notebooks/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   143865 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/notebooks/data/ci38457511_history.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    17550 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/data/events.xlsx
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.413475 usgs-libcomcat-2.0.20/notebooks/events/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.443475 usgs-libcomcat-2.0.20/notebooks/events/ci10537093/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   150113 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/ci10537093/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   226467 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/ci10537093/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.443475 usgs-libcomcat-2.0.20/notebooks/events/ci10542525/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    77195 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/ci10542525/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   227063 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/ci10542525/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.443475 usgs-libcomcat-2.0.20/notebooks/events/nc71330090/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4433 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71330090/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   194356 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71330090/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.443475 usgs-libcomcat-2.0.20/notebooks/events/nc71336726/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   164089 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71336726/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   376033 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71336726/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.443475 usgs-libcomcat-2.0.20/notebooks/events/nc71337451/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    67007 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71337451/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   305249 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71337451/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.453475 usgs-libcomcat-2.0.20/notebooks/events/nc71338066/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   141571 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338066/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   623129 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338066/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.453475 usgs-libcomcat-2.0.20/notebooks/events/nc71338171/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3883 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338171/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204869 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338171/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.453475 usgs-libcomcat-2.0.20/notebooks/events/nc71338196/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1693 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338196/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   192023 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338196/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.453475 usgs-libcomcat-2.0.20/notebooks/events/nc71338301/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      316 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338301/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   193288 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338301/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.453475 usgs-libcomcat-2.0.20/notebooks/events/nc71338406/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1412 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338406/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   192002 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338406/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.453475 usgs-libcomcat-2.0.20/notebooks/events/nc71338851/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       42 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338851/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   192009 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71338851/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.453475 usgs-libcomcat-2.0.20/notebooks/events/nc71346081/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1415 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71346081/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   229348 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71346081/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.463475 usgs-libcomcat-2.0.20/notebooks/events/nc71348851/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    53136 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71348851/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   276332 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71348851/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.463475 usgs-libcomcat-2.0.20/notebooks/events/nc71350686/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6900 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71350686/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   257426 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/nc71350686/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.463475 usgs-libcomcat-2.0.20/notebooks/events/uu50393545/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6376 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/uu50393545/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    22390 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/uu50393545/stationlist.json
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.463475 usgs-libcomcat-2.0.20/notebooks/events/uw10782693/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      315 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/uw10782693/dyfi_geo_1km.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   107985 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/notebooks/events/uw10782693/stationlist.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1410 2022-12-22 00:05:13.000000 usgs-libcomcat-2.0.20/pyproject.toml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3422 2022-11-08 22:17:38.000000 usgs-libcomcat-2.0.20/read_phases.m
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2022-12-22 00:19:13.513475 usgs-libcomcat-2.0.20/setup.cfg
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.413475 usgs-libcomcat-2.0.20/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.413475 usgs-libcomcat-2.0.20/src/data/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.483475 usgs-libcomcat-2.0.20/src/data/cassettes/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2676 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_catalogs.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2362 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_contributors.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1690 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_count.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  5146280 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_detail.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  2184087 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_detail_product_versions.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6299780 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_dyfi.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1702846 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_get_detail_data_frame.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    78392 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_get_event.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  2490828 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_get_pager_data_frame.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3967 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_get_summary_data_frame.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1234578 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_magnitude_dataframe.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   103525 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_moment_supplement.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   100906 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_nan_mags.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1234601 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_phase_dataframe.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    92746 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_product.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   233365 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_search.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4292 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_search_nullmag.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   404298 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/data/cassettes/test_summary.yaml
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.483475 usgs-libcomcat-2.0.20/src/libcomcat/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       93 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/__init__.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    18456 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/_version.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.483475 usgs-libcomcat-2.0.20/src/libcomcat/bin/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/__init__.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7957 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/findid.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    19989 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/getcsv.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    17605 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/geteventhist.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8845 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/getmags.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    11005 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/getpager.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    12388 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/getphases.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    16145 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/bin/getproduct.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    41453 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/classes.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.493475 usgs-libcomcat-2.0.20/src/libcomcat/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   324036 2022-12-07 15:40:25.000000 usgs-libcomcat-2.0.20/src/libcomcat/data/economy.xml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   214515 2022-12-07 15:40:25.000000 usgs-libcomcat-2.0.20/src/libcomcat/data/fatality.xml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        5 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.cpg
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   546979 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.dbf
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      143 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.prj
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)  1612740 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.shp
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2028 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.shx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    76028 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/src/libcomcat/dataframes.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      864 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/exceptions.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2278 2022-11-18 14:29:12.000000 usgs-libcomcat-2.0.20/src/libcomcat/logging.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24107 2022-11-18 23:34:36.000000 usgs-libcomcat-2.0.20/src/libcomcat/search.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      327 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/libcomcat/test_utils.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    11702 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/src/libcomcat/utils.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.483475 usgs-libcomcat-2.0.20/src/libcomcat.egg-info/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2022-12-07 23:06:55.000000 usgs-libcomcat-2.0.20/src/libcomcat.egg-info/dependency_links.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      295 2022-12-07 23:06:55.000000 usgs-libcomcat-2.0.20/src/libcomcat.egg-info/entry_points.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      305 2022-12-07 23:06:55.000000 usgs-libcomcat-2.0.20/src/libcomcat.egg-info/requires.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       10 2022-12-07 23:06:55.000000 usgs-libcomcat-2.0.20/src/libcomcat.egg-info/top_level.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.493475 usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7030 2022-12-22 00:19:13.000000 usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5941 2022-12-22 00:19:13.000000 usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/SOURCES.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2022-12-22 00:19:13.000000 usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/dependency_links.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      295 2022-12-22 00:19:13.000000 usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/entry_points.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2022-12-22 00:19:13.000000 usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/requires.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       15 2022-12-22 00:19:13.000000 usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/top_level.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.423475 usgs-libcomcat-2.0.20/tests/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.493475 usgs-libcomcat-2.0.20/tests/bin/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3714 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/bin/findid_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9734 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/bin/getcsv_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3121 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/bin/geteventhist_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4954 2022-12-08 17:00:30.000000 usgs-libcomcat-2.0.20/tests/bin/getmags_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5431 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/bin/getpager_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4262 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/bin/getphases_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5690 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/tests/bin/getproduct_test.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.493475 usgs-libcomcat-2.0.20/tests/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    20627 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/big_noaa.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      618 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_iscgem910478.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      754 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_iscgem910478_allsources.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      332 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_iscgem910478_shaking.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4822 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5276 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_allsources.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5688 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_allsources_contributing.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5234 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_contributing.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      369 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_destroyed.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      725 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_landslide_shaking.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2039 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/sample_catalogue.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12315 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/us2000ahv0_phases.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    14358 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/data/us2000ahv0_phases.xlsx
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.493475 usgs-libcomcat-2.0.20/tests/libcomcat/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2022-12-22 00:19:13.513475 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000) 10292125 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_detailevent.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   555084 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_detailsummary.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    35619 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_moment.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    37387 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_product.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   112318 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_summary.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   215788 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_association.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   175646 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_detailed.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  2319941 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_dyfi.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1651485 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_history.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   115077 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_magnitude.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1430148 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_pager.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   115121 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_phase.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3015 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_summary.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1758 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_count.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    29202 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_id.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2937 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_null.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2122 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_scenario.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    47526 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_search.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1861 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/utils_catalogs.yaml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1756 2022-11-18 13:41:41.000000 usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/utils_contributors.yaml
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10788 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/tests/libcomcat/classes_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10849 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/tests/libcomcat/dataframes_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2100 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/tests/libcomcat/search_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4927 2022-12-20 23:32:19.000000 usgs-libcomcat-2.0.20/tests/libcomcat/utils_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.491456 usgs-libcomcat-2.0.21/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       97 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/.codecov.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       35 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/.gitattributes
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.381456 usgs-libcomcat-2.0.21/.github/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.391456 usgs-libcomcat-2.0.21/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      706 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      600 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      653 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/.github/ISSUE_TEMPLATE/process-update-request.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      206 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/.gitignore
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1786 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/.gitlab-ci.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      222 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/CODE_OF_CONDUCT.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      736 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/CONTRIBUTING.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/DISCLAIMER.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2263 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/LICENSE.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7030 2023-04-17 20:52:32.491456 usgs-libcomcat-2.0.21/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3954 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/README.md
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      215 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/clean_vcr
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1191 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/code.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.391456 usgs-libcomcat-2.0.21/docs/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    26400 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/docs/api.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    31339 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/docs/cli.md
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3194 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/install.sh
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3685 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/makedocs.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.401455 usgs-libcomcat-2.0.21/notebooks/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   131214 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/AssociatingCatalogues.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1158324 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/Classes.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    99601 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/ComparingMagnitudes.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   365190 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/Dataframes.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    66223 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/DetailEvent.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   191637 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/EventHistory.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    34125 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/GetSMDYFIPairs.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   142968 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/PhasesAndMagnitudes.ipynb
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   202623 2023-04-17 18:34:20.000000 usgs-libcomcat-2.0.21/notebooks/Search.ipynb
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.401455 usgs-libcomcat-2.0.21/notebooks/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   143865 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/data/ci38457511_history.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    17550 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/data/events.xlsx
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.381456 usgs-libcomcat-2.0.21/notebooks/events/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.401455 usgs-libcomcat-2.0.21/notebooks/events/ci10537093/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   150113 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/ci10537093/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   226467 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/ci10537093/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.401455 usgs-libcomcat-2.0.21/notebooks/events/ci10542525/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    77195 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/ci10542525/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   227063 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/ci10542525/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.401455 usgs-libcomcat-2.0.21/notebooks/events/nc71330090/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4433 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71330090/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   194356 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71330090/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.411455 usgs-libcomcat-2.0.21/notebooks/events/nc71336726/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   164089 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71336726/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   376033 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71336726/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.411455 usgs-libcomcat-2.0.21/notebooks/events/nc71337451/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    67007 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71337451/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   305249 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71337451/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.411455 usgs-libcomcat-2.0.21/notebooks/events/nc71338066/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   141571 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338066/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   623129 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338066/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.411455 usgs-libcomcat-2.0.21/notebooks/events/nc71338171/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3883 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338171/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204869 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338171/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.411455 usgs-libcomcat-2.0.21/notebooks/events/nc71338196/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1693 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338196/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   192023 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338196/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.411455 usgs-libcomcat-2.0.21/notebooks/events/nc71338301/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      316 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338301/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   193288 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338301/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.411455 usgs-libcomcat-2.0.21/notebooks/events/nc71338406/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1412 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338406/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   192002 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338406/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.421455 usgs-libcomcat-2.0.21/notebooks/events/nc71338851/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       42 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338851/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   192009 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71338851/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.421455 usgs-libcomcat-2.0.21/notebooks/events/nc71346081/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1415 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71346081/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   229348 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71346081/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.421455 usgs-libcomcat-2.0.21/notebooks/events/nc71348851/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    53136 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71348851/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   276332 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71348851/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.421455 usgs-libcomcat-2.0.21/notebooks/events/nc71350686/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6900 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71350686/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   257426 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/nc71350686/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.421455 usgs-libcomcat-2.0.21/notebooks/events/uu50393545/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6376 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/uu50393545/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    22390 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/uu50393545/stationlist.json
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.421455 usgs-libcomcat-2.0.21/notebooks/events/uw10782693/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      315 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/uw10782693/dyfi_geo_1km.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   107985 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/notebooks/events/uw10782693/stationlist.json
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1410 2023-04-17 18:35:46.000000 usgs-libcomcat-2.0.21/pyproject.toml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3422 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/read_phases.m
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-04-17 20:52:32.491456 usgs-libcomcat-2.0.21/setup.cfg
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.391456 usgs-libcomcat-2.0.21/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.381456 usgs-libcomcat-2.0.21/src/data/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.431455 usgs-libcomcat-2.0.21/src/data/cassettes/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2676 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_catalogs.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2362 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_contributors.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1690 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_count.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  5146280 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_detail.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  2184087 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_detail_product_versions.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6299780 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_dyfi.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1702846 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_get_detail_data_frame.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    78392 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_get_event.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  2490828 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_get_pager_data_frame.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   110468 2023-04-17 18:36:30.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_get_product_bytes.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3967 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_get_summary_data_frame.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1234578 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_magnitude_dataframe.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   103525 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_moment_supplement.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   100906 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_nan_mags.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1234601 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_phase_dataframe.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    92746 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_product.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   233365 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_search.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4292 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_search_nullmag.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   404298 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/data/cassettes/test_summary.yaml
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.441455 usgs-libcomcat-2.0.21/src/libcomcat/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       93 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/__init__.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    18456 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/_version.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.441455 usgs-libcomcat-2.0.21/src/libcomcat/bin/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/__init__.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7957 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/findid.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    19989 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/getcsv.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    16608 2023-04-17 20:22:22.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/geteventhist.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8607 2023-04-17 20:38:25.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/getmags.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    11005 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/getpager.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    12388 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/getphases.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    16145 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/bin/getproduct.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    41453 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/classes.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.441455 usgs-libcomcat-2.0.21/src/libcomcat/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   324036 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/data/economy.xml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   214515 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/data/fatality.xml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        5 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.cpg
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   546979 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.dbf
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      143 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.prj
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)  1612740 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.shp
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2028 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.shx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    76028 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/dataframes.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      864 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/exceptions.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2278 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/logging.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    25711 2023-04-17 18:36:30.000000 usgs-libcomcat-2.0.21/src/libcomcat/search.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      327 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/test_utils.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    11702 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat/utils.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.441455 usgs-libcomcat-2.0.21/src/libcomcat.egg-info/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat.egg-info/dependency_links.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      295 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat.egg-info/entry_points.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      305 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat.egg-info/requires.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       10 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/src/libcomcat.egg-info/top_level.txt
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.441455 usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7030 2023-04-17 20:52:32.000000 usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5988 2023-04-17 20:52:32.000000 usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/SOURCES.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-04-17 20:52:32.000000 usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/dependency_links.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      295 2023-04-17 20:52:32.000000 usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/entry_points.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-04-17 20:52:32.000000 usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/requires.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       15 2023-04-17 20:52:32.000000 usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/top_level.txt
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.391456 usgs-libcomcat-2.0.21/tests/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.441455 usgs-libcomcat-2.0.21/tests/bin/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3714 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/bin/findid_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9734 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/bin/getcsv_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3121 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/bin/geteventhist_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4954 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/bin/getmags_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5431 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/bin/getpager_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4262 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/bin/getphases_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5690 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/bin/getproduct_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.451455 usgs-libcomcat-2.0.21/tests/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    20627 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/big_noaa.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      618 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_iscgem910478.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      754 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_iscgem910478_allsources.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      332 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_iscgem910478_shaking.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4822 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5276 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_allsources.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5688 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_allsources_contributing.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5234 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_contributing.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      369 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_destroyed.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      725 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_landslide_shaking.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2039 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/sample_catalogue.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12315 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/us2000ahv0_phases.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    14358 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/data/us2000ahv0_phases.xlsx
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.451455 usgs-libcomcat-2.0.21/tests/libcomcat/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-17 20:52:32.491456 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000) 10292125 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_detailevent.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   555084 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_detailsummary.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    35619 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_moment.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    37387 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_product.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   112318 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_summary.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   215788 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_association.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   175646 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_detailed.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  2319941 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_dyfi.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1651485 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_history.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   115077 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_magnitude.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  1430148 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_pager.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   115121 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_phase.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3015 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_summary.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1758 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_count.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    29202 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_id.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2937 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_null.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2122 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_scenario.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    47526 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_search.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1861 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/utils_catalogs.yaml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1756 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/utils_contributors.yaml
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10788 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/classes_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10849 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/dataframes_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2415 2023-04-17 18:36:30.000000 usgs-libcomcat-2.0.21/tests/libcomcat/search_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4927 2023-02-26 16:16:52.000000 usgs-libcomcat-2.0.21/tests/libcomcat/utils_test.py
```

### Comparing `usgs-libcomcat-2.0.20/.github/ISSUE_TEMPLATE/bug_report.md` & `usgs-libcomcat-2.0.21/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/.github/ISSUE_TEMPLATE/feature_request.md` & `usgs-libcomcat-2.0.21/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/.github/ISSUE_TEMPLATE/process-update-request.md` & `usgs-libcomcat-2.0.21/.github/ISSUE_TEMPLATE/process-update-request.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/.gitlab-ci.yml` & `usgs-libcomcat-2.0.21/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/CONTRIBUTING.md` & `usgs-libcomcat-2.0.21/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/DISCLAIMER.md` & `usgs-libcomcat-2.0.21/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/LICENSE.md` & `usgs-libcomcat-2.0.21/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/PKG-INFO` & `usgs-libcomcat-2.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-libcomcat
-Version: 2.0.20
+Version: 2.0.21
 Summary: Python wrapper around ComCat web API
 Author-email: Mike Hearne <mhearne@usgs.gov>, Heather Hunsinger <hhunsinger@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usgs-libcomcat Version: 2.0.20 Summary: Python
+Metadata-Version: 2.1 Name: usgs-libcomcat Version: 2.0.21 Summary: Python
 wrapper around ComCat web API Author-email: Mike Hearne
 usgs.gov>, Heather Hunsinger
 usgs.gov> License: License ======= Unless otherwise noted, This project is in
 the public domain in the United States because it contains materials that
 originally came from the United States Geological Survey, an agency of the
 United States Department of Interior. For more information, see the official
 USGS copyright policy at https://www2.usgs.gov/visual-id/
```

### Comparing `usgs-libcomcat-2.0.20/README.md` & `usgs-libcomcat-2.0.21/README.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/code.json` & `usgs-libcomcat-2.0.21/code.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/docs/api.md` & `usgs-libcomcat-2.0.21/docs/api.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/docs/cli.md` & `usgs-libcomcat-2.0.21/docs/cli.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/install.sh` & `usgs-libcomcat-2.0.21/install.sh`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/makedocs.py` & `usgs-libcomcat-2.0.21/makedocs.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/AssociatingCatalogues.ipynb` & `usgs-libcomcat-2.0.21/notebooks/AssociatingCatalogues.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/Classes.ipynb` & `usgs-libcomcat-2.0.21/notebooks/Classes.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/ComparingMagnitudes.ipynb` & `usgs-libcomcat-2.0.21/notebooks/ComparingMagnitudes.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/Dataframes.ipynb` & `usgs-libcomcat-2.0.21/notebooks/Dataframes.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/DetailEvent.ipynb` & `usgs-libcomcat-2.0.21/notebooks/DetailEvent.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/EventHistory.ipynb` & `usgs-libcomcat-2.0.21/notebooks/EventHistory.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/GetSMDYFIPairs.ipynb` & `usgs-libcomcat-2.0.21/notebooks/GetSMDYFIPairs.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/PhasesAndMagnitudes.ipynb` & `usgs-libcomcat-2.0.21/notebooks/PhasesAndMagnitudes.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/Search.ipynb` & `usgs-libcomcat-2.0.21/notebooks/Search.ipynb`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/data/ci38457511_history.xlsx` & `usgs-libcomcat-2.0.21/notebooks/data/ci38457511_history.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/data/events.xlsx` & `usgs-libcomcat-2.0.21/notebooks/data/events.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/ci10537093/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/ci10537093/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/ci10537093/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/ci10537093/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/ci10542525/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/ci10542525/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/ci10542525/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/ci10542525/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71330090/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71330090/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71330090/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71330090/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71336726/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71336726/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71336726/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71336726/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71337451/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71337451/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71337451/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71337451/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338066/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338066/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338066/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338066/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338171/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338171/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338171/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338171/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338196/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338196/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338196/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338196/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338301/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338301/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338406/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338406/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338406/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338406/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71338851/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71338851/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71346081/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71346081/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71346081/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71346081/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71348851/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71348851/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71348851/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71348851/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71350686/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/nc71350686/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/nc71350686/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/nc71350686/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/uu50393545/dyfi_geo_1km.geojson` & `usgs-libcomcat-2.0.21/notebooks/events/uu50393545/dyfi_geo_1km.geojson`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/uu50393545/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/uu50393545/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/notebooks/events/uw10782693/stationlist.json` & `usgs-libcomcat-2.0.21/notebooks/events/uw10782693/stationlist.json`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/pyproject.toml` & `usgs-libcomcat-2.0.21/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "usgs-libcomcat"
-version = "2.0.20"
+version = "2.0.21"
 description = "Python wrapper around ComCat web API"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Heather Hunsinger", email="hhunsinger@usgs.gov"},
 ]
 license = {file = "LICENSE.md"}
 readme = "README.md"
```

### Comparing `usgs-libcomcat-2.0.20/read_phases.m` & `usgs-libcomcat-2.0.21/read_phases.m`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_catalogs.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_catalogs.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_contributors.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_contributors.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_count.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_count.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_detail.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_detail.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_detail_product_versions.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_detail_product_versions.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_dyfi.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_dyfi.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_get_detail_data_frame.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_get_detail_data_frame.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_get_event.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_get_event.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_get_pager_data_frame.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_get_pager_data_frame.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_get_summary_data_frame.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_get_summary_data_frame.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_magnitude_dataframe.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_magnitude_dataframe.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_moment_supplement.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_moment_supplement.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_nan_mags.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_nan_mags.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_phase_dataframe.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_phase_dataframe.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_product.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_product.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_search.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_search.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_search_nullmag.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_search_nullmag.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/data/cassettes/test_summary.yaml` & `usgs-libcomcat-2.0.21/src/data/cassettes/test_summary.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/_version.py` & `usgs-libcomcat-2.0.21/src/libcomcat/_version.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/bin/findid.py` & `usgs-libcomcat-2.0.21/src/libcomcat/bin/findid.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/bin/getcsv.py` & `usgs-libcomcat-2.0.21/src/libcomcat/bin/getcsv.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/bin/geteventhist.py` & `usgs-libcomcat-2.0.21/src/libcomcat/bin/geteventhist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 #!/usr/bin/env python
 import argparse
-import sys
 import os.path
-from datetime import timedelta
+import sys
 import textwrap
-
-# third party imports
-import pandas as pd
-from openpyxl import load_workbook, styles
-from obspy.geodetics.base import gps2dist_azimuth
-import numpy as np
+from datetime import timedelta
 
 # local imports
 import libcomcat
-from libcomcat.search import search, get_event_by_id
-from libcomcat.dataframes import (get_history_data_frame, split_history_frame,
-                                  PRODUCTS, TIMEFMT, PRODUCT_COLUMNS)
+import numpy as np
+
+# third party imports
+import pandas as pd
+from libcomcat.dataframes import (
+    PRODUCT_COLUMNS,
+    PRODUCTS,
+    TIMEFMT,
+    get_history_data_frame,
+    split_history_frame,
+)
 from libcomcat.logging import setup_logger
+from libcomcat.search import get_event_by_id, search
+from obspy.geodetics.base import gps2dist_azimuth
+from openpyxl import load_workbook, styles
 
-DISPLAY_TIME_FMT = '%Y-%m-%d %H:%M:%S'
+DISPLAY_TIME_FMT = "%Y-%m-%d %H:%M:%S"
 
 
-class MyFormatter(argparse.RawTextHelpFormatter,
-                  argparse.ArgumentDefaultsHelpFormatter):
+class MyFormatter(
+    argparse.RawTextHelpFormatter, argparse.ArgumentDefaultsHelpFormatter
+):
     pass
 
 
-COLORS = {'dyfi': 'FADBD8',
-          'finite-fault': 'CD6155',
-          'focal-mechanism': 'EC7063',
-          'ground-failure': 'D1F2EB',
-          'losspager': 'FCF3CF',
-          'moment-tensor': 'F7DC6F',
-          'oaf': '7FB3D5',
-          'origin': 'C39BD3',
-          'phase-data': 'E59866',
-          'shakemap': '58D68D',
-          'default': '99A3A4'}
+COLORS = {
+    "dyfi": "FADBD8",
+    "finite-fault": "CD6155",
+    "focal-mechanism": "EC7063",
+    "ground-failure": "D1F2EB",
+    "losspager": "FCF3CF",
+    "moment-tensor": "F7DC6F",
+    "oaf": "7FB3D5",
+    "origin": "C39BD3",
+    "phase-data": "E59866",
+    "shakemap": "58D68D",
+    "default": "99A3A4",
+}
 
 
 def get_parser():
-    desc = '''Print out ComCat event history.
+    desc = """Print out ComCat event history.
 
     This program summarizes the history of an event through the
     products found in ComCat. The products that can be described are:
     'dyfi', 'finite-fault', 'focal-mechanism', 'ground-failure',
     'losspager', 'moment-tensor', 'oaf', 'origin', 'phase-data',
     and 'shakemap'.
 
@@ -106,342 +114,348 @@
     into separate spreadsheets:
 
     geteventhist ci38457511 -d ~/tmp/ridgecrest -f excel -p origin shakemap --split
 
     To print one product table (say, origins) to stdout in HTML format:
 
     geteventhist ci38996632  -p origin --web --split > ~/test.html
-    '''
-    parser = argparse.ArgumentParser(description=desc,
-                                     formatter_class=MyFormatter)
+    """
+    parser = argparse.ArgumentParser(description=desc, formatter_class=MyFormatter)
     # positional arguments
-    parser.add_argument('eventid',
-                        metavar='EVENTID', help='ComCat event ID.')
+    parser.add_argument("eventid", metavar="EVENTID", help="ComCat event ID.")
 
     # optional arguments
-    ohelp = '''Directory where files are stored.'''
-    parser.add_argument('-d', '--outdir', help=ohelp,
-                        default=os.path.expanduser('~'))
-    parser.add_argument('--exclude-products',
-                        help='COMCAT products to be excluded from the spreadsheet.',
-                        nargs='*', default=[])
-    parser.add_argument('-f', '--format', help="Output format. Options include 'csv', 'tab', and 'excel'. Default is 'csv'.",
-                        choices=['excel', 'csv', 'tab'],
-                        default='csv', dest='format')
-    loghelp = '''Send debugging, informational, warning and error messages to a file.
-    '''
-    parser.add_argument('--logfile', default='stderr', help=loghelp)
-    levelhelp = '''Set the minimum logging level. The logging levels are(low to high):
+    ohelp = """Directory where files are stored."""
+    parser.add_argument("-d", "--outdir", help=ohelp, default=os.path.expanduser("~"))
+    parser.add_argument(
+        "--exclude-products",
+        help="COMCAT products to be excluded from the spreadsheet.",
+        nargs="*",
+        default=[],
+    )
+    parser.add_argument(
+        "-f",
+        "--format",
+        help="Output format. Options include 'csv', 'tab', and 'excel'. Default is 'csv'.",
+        choices=["excel", "csv", "tab"],
+        default="csv",
+        dest="format",
+    )
+    loghelp = """Send debugging, informational, warning and error messages to a file.
+    """
+    parser.add_argument("--logfile", default="stderr", help=loghelp)
+    levelhelp = """Set the minimum logging level. The logging levels are(low to high):
 
      - debug: Debugging message will be printed, most likely for developers.
               Most verbose.
      - info: Only informational messages, warnings, and errors will be printed.
      - warning: Only warnings(i.e., could not retrieve information for a
                 single event out of many) and errors will be printed.
      - error: Only errors will be printed, after which program will stop.
               Least verbose.
-    '''
-    parser.add_argument('--loglevel', default='info',
-                        choices=['debug', 'info', 'warning', 'error'],
-                        help=levelhelp)
-    phelp = '''Limit to only the products specified. If no products are
+    """
+    parser.add_argument(
+        "--loglevel",
+        default="info",
+        choices=["debug", "info", "warning", "error"],
+        help=levelhelp,
+    )
+    phelp = """Limit to only the products specified. If no products are
     specified, all will be listed. See the full list of products here:
     See the full list here: https://usgs.github.io/pdl/userguide/products/index.html.
-    '''
-    parser.add_argument('-p', '--product-type', help=phelp,
-                        nargs='*', default=[])
-    rhelp = '''Search for other unassociated earthquakes
+    """
+    parser.add_argument("-p", "--product-type", help=phelp, nargs="*", default=[])
+    rhelp = """Search for other unassociated earthquakes
     inside a search radius (km). (Requires use of -w.)
-    '''
-    parser.add_argument('-r', '--radius', help=rhelp, type=float)
-    shelp = 'Split descriptions of single-product queries into separate columns.'
-    parser.add_argument('--split',
-                        help=shelp,
-                        action='store_true',
-                        default=False)
-    parser.add_argument('--version', action='version',
-                        version=libcomcat.__version__, help='Version of libcomcat.')
-    parser.add_argument('--web', help='Print HTML tables to stdout.',
-                        default=False, action='store_true')
-    whelp = 'Limit by time window in seconds. (Requires use of -r.)'
-    parser.add_argument('-w', '--window', type=float,
-                        help=whelp)
+    """
+    parser.add_argument("-r", "--radius", help=rhelp, type=float)
+    shelp = "Split descriptions of single-product queries into separate columns."
+    parser.add_argument("--split", help=shelp, action="store_true", default=False)
+    parser.add_argument(
+        "--version",
+        action="version",
+        version=libcomcat.__version__,
+        help="Version of libcomcat.",
+    )
+    parser.add_argument(
+        "--web", help="Print HTML tables to stdout.", default=False, action="store_true"
+    )
+    whelp = "Limit by time window in seconds. (Requires use of -r.)"
+    parser.add_argument("-w", "--window", type=float, help=whelp)
     return parser
 
 
 def _mod_tframe(event, tevent, tframe):
     newframe = pd.DataFrame(columns=tframe.columns)
-    tframe['Authoritative Event ID'] = event.id
-    tframe['Associated'] = False
+    tframe["Authoritative Event ID"] = event.id
+    tframe["Associated"] = False
+    newrows = []
     for idx, row in tframe.iterrows():
-        if row['Product'] not in ['origin', 'phase-data']:
-            newframe = newframe.append(row)
-        parts = row['Description'].split('|')
+        if row["Product"] not in ["origin", "phase-data"]:
+            newrows.append(row)
+        parts = row["Description"].split("|")
         authlat = event.latitude
         authlon = event.longitude
         authtime = event.time
         olat = tevent.latitude
         olon = tevent.longitude
         otime = tevent.time
         dist_m, _, _ = gps2dist_azimuth(authlat, authlon, olat, olon)
         dist = dist_m / 1000.0
         tdiff = (otime - authtime).total_seconds()
-        dstr = 'Distance from auth. origin(km)# % .1f' % dist
-        tstr = 'Offset from auth. origin (sec)# %.1f' % tdiff
+        dstr = "Distance from auth. origin(km)# % .1f" % dist
+        tstr = "Offset from auth. origin (sec)# %.1f" % tdiff
         newparts = parts[0:-2] + [dstr, tstr]
-        row['Description'] = '|'.join(newparts)
-        newframe = newframe.append(row)
+        row["Description"] = "|".join(newparts)
+        newrows.append(row)
+    newframe = pd.DataFrame(data=newrows)
     return newframe
 
 
 def save_dataframe(outdir, format, event, dataframe, product=None):
-    border = styles.Border(left=styles.Side(border_style=None,
-                                            color='FFFFFF'),
-                           right=styles.Side(border_style=None,
-                                             color='FFFFFF'),
-                           top=styles.Side(border_style=None,
-                                           color='FFFFFF'),
-                           bottom=styles.Side(border_style=None,
-                                              color='FFFFFF'),
-                           diagonal=styles.Side(border_style=None,
-                                                color='FFFFFF'),
-                           diagonal_direction=0,
-                           outline=styles.Side(border_style=None,
-                                               color='FFFFFF'),
-                           vertical=styles.Side(border_style=None,
-                                                color='FFFFFF'),
-                           horizontal=styles.Side(border_style=None,
-                                                  color='FFFFFF')
-                           )
+    border = styles.Border(
+        left=styles.Side(border_style=None, color="FFFFFF"),
+        right=styles.Side(border_style=None, color="FFFFFF"),
+        top=styles.Side(border_style=None, color="FFFFFF"),
+        bottom=styles.Side(border_style=None, color="FFFFFF"),
+        diagonal=styles.Side(border_style=None, color="FFFFFF"),
+        diagonal_direction=0,
+        outline=styles.Side(border_style=None, color="FFFFFF"),
+        vertical=styles.Side(border_style=None, color="FFFFFF"),
+        horizontal=styles.Side(border_style=None, color="FFFFFF"),
+    )
 
-    if format == 'excel':
+    if format == "excel":
         if product is not None:
-            outfile = os.path.join(outdir,
-                                   event.id + '_' + product + '.xlsx')
+            outfile = os.path.join(outdir, event.id + "_" + product + ".xlsx")
         else:
-            outfile = os.path.join(outdir, event.id + '.xlsx')
+            outfile = os.path.join(outdir, event.id + ".xlsx")
         dataframe.to_excel(outfile, index=False)
         wb = load_workbook(outfile)
         ws = wb.active
         ws.insert_rows(0, amount=6)
-        ws.cell(1, 1, value='Event ID')
+        ws.cell(1, 1, value="Event ID")
         ws.cell(1, 2, value=event.id)
-        ws.cell(2, 1, value='Origin Time')
+        ws.cell(2, 1, value="Origin Time")
         ws.cell(2, 2, value=event.time.strftime(TIMEFMT))
-        ws.cell(3, 1, value='Magnitude')
+        ws.cell(3, 1, value="Magnitude")
         ws.cell(3, 2, value=event.magnitude)
-        ws.cell(4, 1, value='Latitude')
+        ws.cell(4, 1, value="Latitude")
         ws.cell(4, 2, value=event.latitude)
-        ws.cell(5, 1, value='Longitude')
+        ws.cell(5, 1, value="Longitude")
         ws.cell(5, 2, value=event.longitude)
-        ws.cell(6, 1, value='Depth')
+        ws.cell(6, 1, value="Depth")
         ws.cell(6, 2, value=event.depth)
 
         fills = {}
         for product, color in COLORS.items():
             my_color = styles.colors.Color(rgb=color)
-            my_fill = styles.fills.PatternFill(patternType='solid',
-                                               fgColor=my_color)
+            my_fill = styles.fills.PatternFill(patternType="solid", fgColor=my_color)
             fills[product] = my_fill
 
         # color rows by product type
         for row in ws.iter_rows(min_row=8, min_col=2, max_col=2):
             mycell = row[0]
             if mycell.value in fills:
                 fill = fills[mycell.value]
             else:
-                fill = fills['default']
-            row_range = '%i:%i' % (mycell.row, mycell.row)
+                fill = fills["default"]
+            row_range = "%i:%i" % (mycell.row, mycell.row)
             for cell in ws[row_range]:
                 cell.fill = fill
                 # TODO - figure out why this doesn't do anything!
                 cell.border = border
 
         wb.save(outfile)
     else:
         if product is not None:
-            outfile = os.path.join(outdir,
-                                   event.id + '_' + product + '.csv')
+            outfile = os.path.join(outdir, event.id + "_" + product + ".csv")
         else:
-            outfile = os.path.join(outdir, event.id + '.csv')
-        if format == 'tab':
-            dataframe.to_csv(outfile, sep='\t', index=False)
+            outfile = os.path.join(outdir, event.id + ".csv")
+        if format == "tab":
+            dataframe.to_csv(outfile, sep="\t", index=False)
         else:
             dataframe.to_csv(outfile, index=False)
-        cdata = open(outfile, 'rt').read()
-        with open(outfile, 'wt') as f:
-            f.write('# Event ID: %s\n' % event.id)
-            f.write('# Origin Time: %s\n' % event.time.strftime(TIMEFMT))
-            f.write('# Magnitude: %s\n' % event.magnitude)
-            f.write('# Latitude: %s\n' % event.latitude)
-            f.write('# Longitude: %s\n' % event.longitude)
-            f.write('# Depth: %s\n' % event.depth)
+        cdata = open(outfile, "rt").read()
+        with open(outfile, "wt") as f:
+            f.write("# Event ID: %s\n" % event.id)
+            f.write("# Origin Time: %s\n" % event.time.strftime(TIMEFMT))
+            f.write("# Magnitude: %s\n" % event.magnitude)
+            f.write("# Latitude: %s\n" % event.latitude)
+            f.write("# Longitude: %s\n" % event.longitude)
+            f.write("# Depth: %s\n" % event.depth)
             f.write(cdata)
 
     return outfile
 
 
 def web_print(event, dataframe):
-    etable_fmt = '''
+    etable_fmt = """
     <pre >
     Event ID: % s
     Origin Time: % s
     Magnitude: % .1f
     Latitude: % .4f
     Longitude: % .4f
     Depth: % .1f
     </pre>
-    '''
-    etable_tpl = (event.id,
-                  event.time.strftime(TIMEFMT),
-                  event.magnitude,
-                  event.latitude,
-                  event.longitude,
-                  event.depth)
+    """
+    etable_tpl = (
+        event.id,
+        event.time.strftime(TIMEFMT),
+        event.magnitude,
+        event.latitude,
+        event.longitude,
+        event.depth,
+    )
     etable = etable_fmt % etable_tpl
     print(textwrap.dedent(etable))
     print(dataframe.to_html(index=False, border=0, max_rows=None, max_cols=None))
 
 
 def simplify_times(dataframe):
     # re-format all time columns to be like: 2019-01-01 17:34:16.1
     # first figure out all the time-like columns
     # df['date'] = pd.to_datetime(df["date"].dt.strftime('%Y-%m'))
     dtypes = dataframe.dtypes
-    for idx, dtype in dtypes.iteritems():
+    for idx, dtype in dtypes.items():
         if np.issubdtype(dtype, np.datetime64):
             dataframe[idx] = pd.to_datetime(
-                dataframe[idx].dt.strftime(DISPLAY_TIME_FMT))
+                dataframe[idx].dt.strftime(DISPLAY_TIME_FMT)
+            )
 
 
 def main():
-    pd.set_option('display.width', 1000)
-    pd.set_option('display.max_rows', 1000)
-    pd.set_option('display.max_colwidth', -1)
-    pd.set_option('display.max_columns', 1000)
+    pd.set_option("display.width", 1000)
+    pd.set_option("display.max_rows", 1000)
+    pd.set_option("display.max_colwidth", None)
+    pd.set_option("display.max_columns", 1000)
     pd.set_option("display.colheader_justify", "left")
     parser = get_parser()
     args = parser.parse_args()
 
     setup_logger(args.logfile, args.loglevel)
 
     # make sure that input products are in the list of supported products
     if not set(args.product_type) <= set(PRODUCTS):
         unsupported = list(set(args.product_type) - set(PRODUCTS))
-        fmt = 'The following event products are not supported: '
-        print(fmt % (','.join(unsupported)))
+        fmt = "The following event products are not supported: "
+        print(fmt % (",".join(unsupported)))
         sys.exit(1)
 
     # make sure that excluded products are in the list of supported products
     if not set(args.exclude_products) <= set(PRODUCTS):
         unsupported = list(set(args.exclude_products) - set(PRODUCTS))
-        fmt = ('The following event products you want to exclude '
-               'are not supported: ')
-        print(fmt % (','.join(unsupported)))
+        fmt = "The following event products you want to exclude " "are not supported: "
+        print(fmt % (",".join(unsupported)))
         sys.exit(1)
 
     # web output and directory output are mutually exclusive
     if args.outdir and args.web:
-        if args.outdir != os.path.expanduser('~'):
-            msg = '''The -d and --web options are mutually exclusive, meaning
+        if args.outdir != os.path.expanduser("~"):
+            msg = """The -d and --web options are mutually exclusive, meaning
             that you cannot choose to write files to a directory and print
             HTML output to the screen simultaneously. Please choose one of
             those two options and try again.
-            '''
+            """
             print(msg)
             sys.exit(1)
         else:
             args.outdir = None
     if args.radius and not args.window:
-        msg = '''To define a time and distance range, the radius and window
+        msg = """To define a time and distance range, the radius and window
          options must both be set.
-        '''
+        """
         print(msg)
         sys.exit(1)
     if args.window and not args.radius:
-        msg = '''To define a time and distance range, the radius and window
+        msg = """To define a time and distance range, the radius and window
          options must both be set.
-        '''
+        """
         print(msg)
         sys.exit(1)
     if args.product_type:
         products = args.product_type
     else:
         products = PRODUCTS
 
     if args.exclude_products:
         products = set(products) - set(args.exclude_products)
 
     try:
         detail_event = get_event_by_id(args.eventid, includesuperseded=True)
         dataframe, event = get_history_data_frame(detail_event, products)
     except Exception as e:
-        fmt = '''Failed to retrieve event history data for
+        fmt = """Failed to retrieve event history data for
         event % s. Error message is as follows. Exiting.
         "%s"
-        '''
+        """
         tpl = (args.eventid, str(e))
         print(fmt % tpl)
         sys.exit(1)
 
     if args.radius:
         radius_km = args.radius
         radius_secs = args.window
         stime = event.time - timedelta(seconds=radius_secs)
         etime = event.time + timedelta(seconds=radius_secs)
 
-        eventlist = search(starttime=stime,
-                           endtime=etime,
-                           latitude=event.latitude,
-                           longitude=event.longitude,
-                           maxradiuskm=radius_km)
+        eventlist = search(
+            starttime=stime,
+            endtime=etime,
+            latitude=event.latitude,
+            longitude=event.longitude,
+            maxradiuskm=radius_km,
+        )
         for tevent in eventlist:
             if tevent.id == event.id:
                 continue
             detail = tevent.getDetailEvent(includesuperseded=True)
             tframe = get_history_data_frame(detail, products)
             newframe = _mod_tframe(event, tevent, tframe)
             dataframe = dataframe.append(newframe, ignore_index=True)
 
         # now re-sort by update time
-        dataframe = dataframe.sort_values('Update Time')
+        dataframe = dataframe.sort_values("Update Time")
         dataframe = dataframe[PRODUCT_COLUMNS]
     else:
         # since "Authoritative Event ID" and "Associated" columns are only applicable when
         # we're including other events in our results, drop those columns
         # if we're not doing that.
-        drop_columns = ['Authoritative Event ID', 'Associated']
-        dataframe = dataframe.drop(drop_columns, axis='columns')
+        drop_columns = ["Authoritative Event ID", "Associated"]
+        dataframe = dataframe.drop(drop_columns, axis="columns")
 
     if args.outdir is not None and not os.path.isdir(args.outdir):
         os.makedirs(args.outdir)
 
     if args.split:
-        df_products = dataframe['Product'].unique().tolist()
+        df_products = dataframe["Product"].unique().tolist()
         available_products = set(df_products) & set(products)
         # TODO: Consider merging phase-data and origin products
         # somehow in this process
         for product in available_products:
             pframe = split_history_frame(dataframe, product=product)
             simplify_times(pframe)
             if args.web:
                 web_print(event, pframe)
             else:
-                outfile = save_dataframe(args.outdir, args.format, event,
-                                         pframe, product=product)
-                print('%i rows saved to %s' % (len(pframe), outfile))
+                outfile = save_dataframe(
+                    args.outdir, args.format, event, pframe, product=product
+                )
+                print("%i rows saved to %s" % (len(pframe), outfile))
         sys.exit(0)
 
     if args.outdir:
-        outfile = save_dataframe(args.outdir, args.format, event,
-                                 dataframe, product=None)
+        outfile = save_dataframe(
+            args.outdir, args.format, event, dataframe, product=None
+        )
 
-        print('%i rows saved to %s' % (len(dataframe), outfile))
+        print("%i rows saved to %s" % (len(dataframe), outfile))
     elif args.web:
         simplify_times(dataframe)
         web_print(event, dataframe)
 
     sys.exit(0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/bin/getpager.py` & `usgs-libcomcat-2.0.21/src/libcomcat/bin/getpager.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/bin/getphases.py` & `usgs-libcomcat-2.0.21/src/libcomcat/bin/getphases.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/bin/getproduct.py` & `usgs-libcomcat-2.0.21/src/libcomcat/bin/getproduct.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/classes.py` & `usgs-libcomcat-2.0.21/src/libcomcat/classes.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/data/economy.xml` & `usgs-libcomcat-2.0.21/src/libcomcat/data/economy.xml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/data/fatality.xml` & `usgs-libcomcat-2.0.21/src/libcomcat/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.dbf` & `usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.dbf`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.shp` & `usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.shp`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/data/ne_50m_admin_0_countries.shx` & `usgs-libcomcat-2.0.21/src/libcomcat/data/ne_50m_admin_0_countries.shx`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/dataframes.py` & `usgs-libcomcat-2.0.21/src/libcomcat/dataframes.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/exceptions.py` & `usgs-libcomcat-2.0.21/src/libcomcat/exceptions.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/logging.py` & `usgs-libcomcat-2.0.21/src/libcomcat/logging.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/search.py` & `usgs-libcomcat-2.0.21/src/libcomcat/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -663,7 +663,50 @@
             loc_row[latname] = float(origin["latitude"])
             loc_row[lonname] = float(origin["longitude"])
             loc_row[depname] = float(origin["depth"])
     except Exception as e:
         msg = 'Failed to download event %s, error "%s".' % (eventid, str(e))
 
     return (mag_row, loc_row, msg)
+
+
+def get_product_bytes(
+    eventid, product, content, source="preferred", version="preferred"
+):
+    """Retrieve Product content given an eventid.
+
+    Args:
+        eventid (str): ComCat event ID.
+        product (str): Name of product (origin, shakemap, etc.) to
+                       retrieve.
+        content (str): Regular expression representing content file name.
+        version (enum): Any one of:
+            - 'preferred' Get the preferred version.
+            - 'first' Get the first version.
+            - 'last' Get the last version.
+            - 'all' Get all versions.
+        source (str): Any one of:
+            - 'preferred' Get version(s) of products from preferred source.
+            - 'all' Get version(s) of products from all sources.
+            - Any valid source network for this type of product
+            ('us','ak',etc.)
+    Returns:
+    bytes: Bytes containing the desired file content.
+    """
+    detail = get_event_by_id(eventid)
+    return get_product_bytes_from_detail(
+        detail, product, content, source=source, version=version
+    )
+
+
+def get_product_bytes_from_detail(
+    detail, product, content, source="preferred", version="preferred"
+):
+    products = detail.getProducts(product, source=source, version=version)
+    if not len(products):
+        raise KeyError(f"No product {product} for event {detail.id}")
+    product = products[0]
+    name = product.getContentName(content)
+    if name is None:
+        raise KeyError(f"No content matching string {content} for product {product}")
+    pbytes, _ = product.getContentBytes(name)
+    return pbytes
```

### Comparing `usgs-libcomcat-2.0.20/src/libcomcat/utils.py` & `usgs-libcomcat-2.0.21/src/libcomcat/utils.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/PKG-INFO` & `usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-libcomcat
-Version: 2.0.20
+Version: 2.0.21
 Summary: Python wrapper around ComCat web API
 Author-email: Mike Hearne <mhearne@usgs.gov>, Heather Hunsinger <hhunsinger@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usgs-libcomcat Version: 2.0.20 Summary: Python
+Metadata-Version: 2.1 Name: usgs-libcomcat Version: 2.0.21 Summary: Python
 wrapper around ComCat web API Author-email: Mike Hearne
 usgs.gov>, Heather Hunsinger
 usgs.gov> License: License ======= Unless otherwise noted, This project is in
 the public domain in the United States because it contains materials that
 originally came from the United States Geological Survey, an agency of the
 United States Department of Interior. For more information, see the official
 USGS copyright policy at https://www2.usgs.gov/visual-id/
```

### Comparing `usgs-libcomcat-2.0.20/src/usgs_libcomcat.egg-info/SOURCES.txt` & `usgs-libcomcat-2.0.21/src/usgs_libcomcat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 src/data/cassettes/test_count.yaml
 src/data/cassettes/test_detail.yaml
 src/data/cassettes/test_detail_product_versions.yaml
 src/data/cassettes/test_dyfi.yaml
 src/data/cassettes/test_get_detail_data_frame.yaml
 src/data/cassettes/test_get_event.yaml
 src/data/cassettes/test_get_pager_data_frame.yaml
+src/data/cassettes/test_get_product_bytes.yaml
 src/data/cassettes/test_get_summary_data_frame.yaml
 src/data/cassettes/test_magnitude_dataframe.yaml
 src/data/cassettes/test_moment_supplement.yaml
 src/data/cassettes/test_nan_mags.yaml
 src/data/cassettes/test_phase_dataframe.yaml
 src/data/cassettes/test_product.yaml
 src/data/cassettes/test_search.yaml
```

### Comparing `usgs-libcomcat-2.0.20/tests/bin/findid_test.py` & `usgs-libcomcat-2.0.21/tests/bin/findid_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/bin/getcsv_test.py` & `usgs-libcomcat-2.0.21/tests/bin/getcsv_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/bin/geteventhist_test.py` & `usgs-libcomcat-2.0.21/tests/bin/geteventhist_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/bin/getmags_test.py` & `usgs-libcomcat-2.0.21/tests/bin/getmags_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/bin/getpager_test.py` & `usgs-libcomcat-2.0.21/tests/bin/getpager_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/bin/getphases_test.py` & `usgs-libcomcat-2.0.21/tests/bin/getphases_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/bin/getproduct_test.py` & `usgs-libcomcat-2.0.21/tests/bin/getproduct_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/big_noaa.csv` & `usgs-libcomcat-2.0.21/tests/data/big_noaa.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/impact_iscgem910478.csv` & `usgs-libcomcat-2.0.21/tests/data/impact_iscgem910478.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/impact_iscgem910478_allsources.csv` & `usgs-libcomcat-2.0.21/tests/data/impact_iscgem910478_allsources.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg.csv` & `usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_allsources.csv` & `usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_allsources.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_allsources_contributing.csv` & `usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_allsources_contributing.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_contributing.csv` & `usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_contributing.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/impact_usp0005rcg_landslide_shaking.csv` & `usgs-libcomcat-2.0.21/tests/data/impact_usp0005rcg_landslide_shaking.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/sample_catalogue.csv` & `usgs-libcomcat-2.0.21/tests/data/sample_catalogue.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/us2000ahv0_phases.csv` & `usgs-libcomcat-2.0.21/tests/data/us2000ahv0_phases.csv`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/data/us2000ahv0_phases.xlsx` & `usgs-libcomcat-2.0.21/tests/data/us2000ahv0_phases.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_detailevent.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_detailevent.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_detailsummary.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_detailsummary.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_moment.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_moment.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_product.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_product.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/classes_summary.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/classes_summary.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_association.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_association.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_detailed.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_detailed.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_dyfi.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_dyfi.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_history.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_history.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_magnitude.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_magnitude.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_pager.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_pager.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_phase.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_phase.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/dataframes_summary.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/dataframes_summary.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_count.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_count.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_id.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_id.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_null.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_null.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_scenario.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_scenario.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/search_search.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/search_search.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/utils_catalogs.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/utils_catalogs.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/cassettes/utils_contributors.yaml` & `usgs-libcomcat-2.0.21/tests/libcomcat/cassettes/utils_contributors.yaml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/classes_test.py` & `usgs-libcomcat-2.0.21/tests/libcomcat/classes_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/dataframes_test.py` & `usgs-libcomcat-2.0.21/tests/libcomcat/dataframes_test.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/search_test.py` & `usgs-libcomcat-2.0.21/tests/libcomcat/search_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 
 # stdlib imports
+import json
 import os.path
 from datetime import datetime, timedelta
 
 # third party imports
 import numpy as np
 
 from libcomcat.classes import DetailEvent
 
 # local imports
-from libcomcat.search import count, get_event_by_id, search
+from libcomcat.search import count, get_event_by_id, get_product_bytes, search
 from libcomcat.test_utils import vcr
 
 
 @vcr.use_cassette()
 def test_get_event():
     eventid = "ci3144585"
     event = get_event_by_id(eventid)
@@ -80,13 +81,23 @@
             host="error",
         )
     except Exception as e:
         passed = False
     assert passed == False
 
 
+@vcr.use_cassette()
+def test_get_product_bytes():
+    eventid = "nc216859"
+    product = "shakemap"
+    content = "rupture.json"
+    rupture = json.loads(get_product_bytes(eventid, product, content).decode("utf8"))
+    rupture["metadata"]["mag"] == 6.9
+
+
 if __name__ == "__main__":
+    test_get_product_bytes()
     test_search_nullmag()
     test_get_event()
     test_count()
     test_search()
     test_url_error()
```

### Comparing `usgs-libcomcat-2.0.20/tests/libcomcat/utils_test.py` & `usgs-libcomcat-2.0.21/tests/libcomcat/utils_test.py`

 * *Files identical despite different names*

