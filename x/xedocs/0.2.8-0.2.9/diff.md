# Comparing `tmp/xedocs-0.2.8.tar.gz` & `tmp/xedocs-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xedocs-0.2.8.tar", max compression
+gzip compressed data, was "xedocs-0.2.9.tar", max compression
```

## Comparing `xedocs-0.2.8.tar` & `xedocs-0.2.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     4587 2023-01-16 20:16:22.220434 xedocs-0.2.8/README.rst
--rw-r--r--   0        0        0     2069 2023-01-16 20:16:22.224434 xedocs-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       36 2023-01-16 20:16:22.224434 xedocs-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0    10491 2023-01-16 20:16:22.224434 xedocs-0.2.8/tests/test_corrections.py
--rw-r--r--   0        0        0      902 2023-01-16 20:16:22.224434 xedocs-0.2.8/tests/test_xedocs.py
--rw-r--r--   0        0        0     1783 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/__init__.py
--rw-r--r--   0        0        0     4365 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/_settings.py
--rw-r--r--   0        0        0     1197 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/_straxen_plugin.py
--rw-r--r--   0        0        0      971 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/api.py
--rw-r--r--   0        0        0     3493 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/cli.py
--rw-r--r--   0        0        0     2079 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/clock.py
--rw-r--r--   0        0        0     2101 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/contexts.py
--rw-r--r--   0        0        0     1720 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/database_interface.py
--rw-r--r--   0        0        0        0 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/databases/__init__.py
--rw-r--r--   0        0        0     2551 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/databases/api.py
--rw-r--r--   0        0        0     2221 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/databases/github.py
--rw-r--r--   0        0        0     2681 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/databases/local.py
--rw-r--r--   0        0        0     1440 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/databases/mongo.py
--rw-r--r--   0        0        0     1273 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/databases/utilix.py
--rw-r--r--   0        0        0      808 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/dispatchers.py
--rw-r--r--   0        0        0     2098 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/entrypoints.py
--rw-r--r--   0        0        0      343 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/__init__.py
--rw-r--r--   0        0        0       51 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/analysis/__init__.py
--rw-r--r--   0        0        0      111 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/analysis/base_analysis.py
--rw-r--r--   0        0        0     1812 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/analysis/processing_requests.py
--rw-r--r--   0        0        0     2007 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/base_schemas.py
--rw-r--r--   0        0        0      190 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/calibrations/__init__.py
--rw-r--r--   0        0        0     1045 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/calibrations/base_calibrations.py
--rw-r--r--   0        0        0      412 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/calibrations/diffused_calibration.py
--rw-r--r--   0        0        0      206 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/calibrations/ibelt_calibrations.py
--rw-r--r--   0        0        0      650 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/calibrations/sources.py
--rw-r--r--   0        0        0      345 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/calibrations/utube_calibrations.py
--rw-r--r--   0        0        0      368 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/constants.py
--rw-r--r--   0        0        0      180 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/context_config.py
--rw-r--r--   0        0        0      568 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/context_lineage.py
--rw-r--r--   0        0        0      628 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/__init__.py
--rw-r--r--   0        0        0      488 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/avg_se_gain.py
--rw-r--r--   0        0        0     9784 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/base_corrections.py
--rw-r--r--   0        0        0     2674 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/base_references.py
--rw-r--r--   0        0        0      473 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/baseline_samples_nv.py
--rw-r--r--   0        0        0      304 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/bayes_model.py
--rw-r--r--   0        0        0      524 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/electron_diffusion_cte.py
--rw-r--r--   0        0        0     1161 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/electron_drift.py
--rw-r--r--   0        0        0      949 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/electron_lifetime.py
--rw-r--r--   0        0        0     1204 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/extraction_efficiency.py
--rw-r--r--   0        0        0      894 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/field_distortion.py
--rw-r--r--   0        0        0     1216 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/field_simulation.py
--rw-r--r--   0        0        0      212 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/global_versions.py
--rw-r--r--   0        0        0      723 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/hit_thresholds.py
--rw-r--r--   0        0        0     1159 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/lone_hits.py
--rw-r--r--   0        0        0      549 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/pmt_gains.py
--rw-r--r--   0        0        0     1409 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/position_reconstruction.py
--rw-r--r--   0        0        0      589 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/relative_light_yield.py
--rw-r--r--   0        0        0      458 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/s1_aft_xyz.py
--rw-r--r--   0        0        0      664 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/s1_xyz.py
--rw-r--r--   0        0        0     1207 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/s2_xy.py
--rw-r--r--   0        0        0     1143 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/corrections/se_gains.py
--rw-r--r--   0        0        0      514 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/detector_numbers.py
--rw-r--r--   0        0        0      599 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/fax.py
--rw-r--r--   0        0        0      165 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/operations_reports/__init__.py
--rw-r--r--   0        0        0      349 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/operations_reports/abnormal_rates.py
--rw-r--r--   0        0        0      301 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/operations_reports/anode_ramp.py
--rw-r--r--   0        0        0      374 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/operations_reports/anode_washing.py
--rw-r--r--   0        0        0      780 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/operations_reports/base_report.py
--rw-r--r--   0        0        0      501 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/operations_reports/hotspot.py
--rw-r--r--   0        0        0     2573 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/plugin_lineages.py
--rw-r--r--   0        0        0      171 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/pmt_data/__init__.py
--rw-r--r--   0        0        0      182 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/pmt_data/base_pmt_data.py
--rw-r--r--   0        0        0      457 2023-01-16 20:16:22.224434 xedocs-0.2.8/xedocs/schemas/pmt_data/gain_calculation.py
--rw-r--r--   0        0        0     1233 2023-01-16 20:16:22.228434 xedocs-0.2.8/xedocs/schemas/pmt_data/pmt_installs.py
--rw-r--r--   0        0        0      271 2023-01-16 20:16:22.228434 xedocs-0.2.8/xedocs/schemas/pmt_data/pmts.py
--rw-r--r--   0        0        0      428 2023-01-16 20:16:22.228434 xedocs-0.2.8/xedocs/schemas/pmt_data/voltage_changes.py
--rw-r--r--   0        0        0      428 2023-01-16 20:16:22.228434 xedocs-0.2.8/xedocs/schemas/pmt_data/voltage_settings.py
--rw-r--r--   0        0        0     1420 2023-01-16 20:16:22.228434 xedocs-0.2.8/xedocs/utils.py
--rw-r--r--   0        0        0    28413 2023-01-16 20:16:22.228434 xedocs-0.2.8/xedocs/widgets.py
--rw-r--r--   0        0        0     6245 2023-01-16 20:16:22.228434 xedocs-0.2.8/xedocs/xedocs.py
--rw-r--r--   0        0        0     6345 1970-01-01 00:00:00.000000 xedocs-0.2.8/setup.py
--rw-r--r--   0        0        0     5608 1970-01-01 00:00:00.000000 xedocs-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     4587 2023-01-18 20:18:50.749458 xedocs-0.2.9/README.rst
+-rw-r--r--   0        0        0     2069 2023-01-18 20:18:50.753458 xedocs-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-01-18 20:18:50.753458 xedocs-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0    10491 2023-01-18 20:18:50.753458 xedocs-0.2.9/tests/test_corrections.py
+-rw-r--r--   0        0        0      902 2023-01-18 20:18:50.753458 xedocs-0.2.9/tests/test_xedocs.py
+-rw-r--r--   0        0        0     1783 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/__init__.py
+-rw-r--r--   0        0        0     4399 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/_settings.py
+-rw-r--r--   0        0        0     1197 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/_straxen_plugin.py
+-rw-r--r--   0        0        0      971 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/api.py
+-rw-r--r--   0        0        0     3493 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/cli.py
+-rw-r--r--   0        0        0     2079 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/clock.py
+-rw-r--r--   0        0        0     2101 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/contexts.py
+-rw-r--r--   0        0        0     1720 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/database_interface.py
+-rw-r--r--   0        0        0        0 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/databases/__init__.py
+-rw-r--r--   0        0        0     2552 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/databases/api.py
+-rw-r--r--   0        0        0     2222 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/databases/github.py
+-rw-r--r--   0        0        0     3521 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/databases/local.py
+-rw-r--r--   0        0        0     1440 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/databases/mongo.py
+-rw-r--r--   0        0        0     1273 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/databases/utilix.py
+-rw-r--r--   0        0        0      808 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/dispatchers.py
+-rw-r--r--   0        0        0     2098 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/entrypoints.py
+-rw-r--r--   0        0        0      343 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/__init__.py
+-rw-r--r--   0        0        0       51 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/analysis/__init__.py
+-rw-r--r--   0        0        0      111 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/analysis/base_analysis.py
+-rw-r--r--   0        0        0     1812 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/analysis/processing_requests.py
+-rw-r--r--   0        0        0     2007 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/base_schemas.py
+-rw-r--r--   0        0        0      190 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/calibrations/__init__.py
+-rw-r--r--   0        0        0     1045 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/calibrations/base_calibrations.py
+-rw-r--r--   0        0        0      412 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/calibrations/diffused_calibration.py
+-rw-r--r--   0        0        0      206 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/calibrations/ibelt_calibrations.py
+-rw-r--r--   0        0        0      650 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/calibrations/sources.py
+-rw-r--r--   0        0        0      345 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/calibrations/utube_calibrations.py
+-rw-r--r--   0        0        0      368 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/constants.py
+-rw-r--r--   0        0        0      180 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/context_config.py
+-rw-r--r--   0        0        0      568 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/context_lineage.py
+-rw-r--r--   0        0        0      628 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/__init__.py
+-rw-r--r--   0        0        0      488 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/avg_se_gain.py
+-rw-r--r--   0        0        0     9784 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/base_corrections.py
+-rw-r--r--   0        0        0     2674 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/base_references.py
+-rw-r--r--   0        0        0      473 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/baseline_samples_nv.py
+-rw-r--r--   0        0        0      304 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/bayes_model.py
+-rw-r--r--   0        0        0      524 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/electron_diffusion_cte.py
+-rw-r--r--   0        0        0     1161 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/electron_drift.py
+-rw-r--r--   0        0        0      949 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/electron_lifetime.py
+-rw-r--r--   0        0        0     1204 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/extraction_efficiency.py
+-rw-r--r--   0        0        0      894 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/field_distortion.py
+-rw-r--r--   0        0        0     1216 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/field_simulation.py
+-rw-r--r--   0        0        0      212 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/global_versions.py
+-rw-r--r--   0        0        0      723 2023-01-18 20:18:50.753458 xedocs-0.2.9/xedocs/schemas/corrections/hit_thresholds.py
+-rw-r--r--   0        0        0     1159 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/lone_hits.py
+-rw-r--r--   0        0        0      549 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/pmt_gains.py
+-rw-r--r--   0        0        0     1409 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/position_reconstruction.py
+-rw-r--r--   0        0        0      589 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/relative_light_yield.py
+-rw-r--r--   0        0        0      458 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/s1_aft_xyz.py
+-rw-r--r--   0        0        0      664 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/s1_xyz.py
+-rw-r--r--   0        0        0     1207 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/s2_xy.py
+-rw-r--r--   0        0        0     1143 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/corrections/se_gains.py
+-rw-r--r--   0        0        0      514 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/detector_numbers.py
+-rw-r--r--   0        0        0      599 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/fax.py
+-rw-r--r--   0        0        0      165 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/operations_reports/__init__.py
+-rw-r--r--   0        0        0      349 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/operations_reports/abnormal_rates.py
+-rw-r--r--   0        0        0      301 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/operations_reports/anode_ramp.py
+-rw-r--r--   0        0        0      374 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/operations_reports/anode_washing.py
+-rw-r--r--   0        0        0      780 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/operations_reports/base_report.py
+-rw-r--r--   0        0        0      501 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/operations_reports/hotspot.py
+-rw-r--r--   0        0        0     2573 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/plugin_lineages.py
+-rw-r--r--   0        0        0      171 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/pmt_data/__init__.py
+-rw-r--r--   0        0        0      182 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/pmt_data/base_pmt_data.py
+-rw-r--r--   0        0        0      457 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/pmt_data/gain_calculation.py
+-rw-r--r--   0        0        0     1233 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/pmt_data/pmt_installs.py
+-rw-r--r--   0        0        0      271 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/pmt_data/pmts.py
+-rw-r--r--   0        0        0      428 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/pmt_data/voltage_changes.py
+-rw-r--r--   0        0        0      428 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/schemas/pmt_data/voltage_settings.py
+-rw-r--r--   0        0        0     1420 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/utils.py
+-rw-r--r--   0        0        0    28413 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/widgets.py
+-rw-r--r--   0        0        0     6460 2023-01-18 20:18:50.757458 xedocs-0.2.9/xedocs/xedocs.py
+-rw-r--r--   0        0        0     6345 1970-01-01 00:00:00.000000 xedocs-0.2.9/setup.py
+-rw-r--r--   0        0        0     5608 1970-01-01 00:00:00.000000 xedocs-0.2.9/PKG-INFO
```

### Comparing `xedocs-0.2.8/README.rst` & `xedocs-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/pyproject.toml` & `xedocs-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "xedocs"
-version = "0.2.8"
+version = "0.2.9"
 homepage = "https://github.com/XENONnT/xedocs"
 description = "Top-level package for xedocs."
 authors = ["Yossi Mosbacher <joe.mosbacher@gmail.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `xedocs-0.2.8/tests/test_corrections.py` & `xedocs-0.2.9/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/tests/test_xedocs.py` & `xedocs-0.2.9/tests/test_xedocs.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/__init__.py` & `xedocs-0.2.9/xedocs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for xedocs."""
 
 __author__ = """Yossi Mosbacher"""
 __email__ = "joe.mosbacher@gmail.com"
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `xedocs-0.2.8/xedocs/_settings.py` & `xedocs-0.2.9/xedocs/_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         env_file = XEDOCS_ENV
         env_file_encoding = "utf-8"
 
     _DATABASE_INTERFACE_CLASSES = {}
 
     DATABASES = ["development_db", "straxen_db"]
     CONFIG_DIR = dirs.user_config_dir
+    DATA_DIR = dirs.user_data_dir
 
     clock = SimpleClock()
 
     _database_interfaces = {}
 
     def database_interfaces(self, database: str):
         interfaces = self._database_interfaces.get(database, {})
```

### Comparing `xedocs-0.2.8/xedocs/_straxen_plugin.py` & `xedocs-0.2.9/xedocs/_straxen_plugin.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/api.py` & `xedocs-0.2.9/xedocs/api.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/cli.py` & `xedocs-0.2.9/xedocs/cli.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/clock.py` & `xedocs-0.2.9/xedocs/clock.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/contexts.py` & `xedocs-0.2.9/xedocs/contexts.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/database_interface.py` & `xedocs-0.2.9/xedocs/database_interface.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/databases/api.py` & `xedocs-0.2.9/xedocs/databases/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class ApiSettings(BaseSettings):
     class Config:
         env_prefix = "XEDOCS_API_"
         env_file = XEDOCS_API_ENV
 
-    PRIORITY: int = 2
+    PRIORITY: int = -1
     URL_TEMPLATE: str = "{base_url}/{version}/{database}/{name}"
     BASE_URL: str = "https://api.xedocs.yossisprojects.com"
     VERSION: str = "v1"
     AUDIENCE: str = "https://api.cmt.xenonnt.org"
     READONLY: bool = False
     TOKEN: str = None
     USERNAME: str = None
```

### Comparing `xedocs-0.2.8/xedocs/databases/github.py` & `xedocs-0.2.9/xedocs/databases/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class GithubSettings(BaseSettings):
     class Config:
         env_prefix = "XEDOCS_GITHUB_"
         env_file = XEDOCS_GITHUB_ENV
 
-    PRIORITY: int = 3
+    PRIORITY: int = -1
     ORG: str = "XENONnT"
     REPO: str = "xedocs-data"
     URL_TEMPLATE: str = "github://{org}:{repo}@/{database}/{category}/{name}/*.json"
     USERNAME: str = default_github_username()
     TOKEN: str = default_github_token()
```

### Comparing `xedocs-0.2.8/xedocs/databases/mongo.py` & `xedocs-0.2.9/xedocs/databases/mongo.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/databases/utilix.py` & `xedocs-0.2.9/xedocs/databases/utilix.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/dispatchers.py` & `xedocs-0.2.9/xedocs/dispatchers.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/entrypoints.py` & `xedocs-0.2.9/xedocs/entrypoints.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/analysis/processing_requests.py` & `xedocs-0.2.9/xedocs/schemas/analysis/processing_requests.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/base_schemas.py` & `xedocs-0.2.9/xedocs/schemas/base_schemas.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/calibrations/base_calibrations.py` & `xedocs-0.2.9/xedocs/schemas/calibrations/base_calibrations.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/calibrations/sources.py` & `xedocs-0.2.9/xedocs/schemas/calibrations/sources.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/context_lineage.py` & `xedocs-0.2.9/xedocs/schemas/context_lineage.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/__init__.py` & `xedocs-0.2.9/xedocs/schemas/corrections/__init__.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/base_corrections.py` & `xedocs-0.2.9/xedocs/schemas/corrections/base_corrections.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/base_references.py` & `xedocs-0.2.9/xedocs/schemas/corrections/base_references.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/electron_diffusion_cte.py` & `xedocs-0.2.9/xedocs/schemas/corrections/electron_diffusion_cte.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/electron_drift.py` & `xedocs-0.2.9/xedocs/schemas/corrections/electron_drift.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/electron_lifetime.py` & `xedocs-0.2.9/xedocs/schemas/corrections/electron_lifetime.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/extraction_efficiency.py` & `xedocs-0.2.9/xedocs/schemas/corrections/extraction_efficiency.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/field_distortion.py` & `xedocs-0.2.9/xedocs/schemas/corrections/field_distortion.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/field_simulation.py` & `xedocs-0.2.9/xedocs/schemas/corrections/field_simulation.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/hit_thresholds.py` & `xedocs-0.2.9/xedocs/schemas/corrections/hit_thresholds.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/lone_hits.py` & `xedocs-0.2.9/xedocs/schemas/corrections/lone_hits.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/pmt_gains.py` & `xedocs-0.2.9/xedocs/schemas/corrections/pmt_gains.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/position_reconstruction.py` & `xedocs-0.2.9/xedocs/schemas/corrections/position_reconstruction.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/relative_light_yield.py` & `xedocs-0.2.9/xedocs/schemas/corrections/relative_light_yield.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/s1_xyz.py` & `xedocs-0.2.9/xedocs/schemas/corrections/s1_xyz.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/s2_xy.py` & `xedocs-0.2.9/xedocs/schemas/corrections/s2_xy.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/corrections/se_gains.py` & `xedocs-0.2.9/xedocs/schemas/corrections/se_gains.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/detector_numbers.py` & `xedocs-0.2.9/xedocs/schemas/detector_numbers.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/fax.py` & `xedocs-0.2.9/xedocs/schemas/fax.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/operations_reports/base_report.py` & `xedocs-0.2.9/xedocs/schemas/operations_reports/base_report.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/plugin_lineages.py` & `xedocs-0.2.9/xedocs/schemas/plugin_lineages.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/schemas/pmt_data/pmt_installs.py` & `xedocs-0.2.9/xedocs/schemas/pmt_data/pmt_installs.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/utils.py` & `xedocs-0.2.9/xedocs/utils.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/widgets.py` & `xedocs-0.2.9/xedocs/widgets.py`

 * *Files identical despite different names*

### Comparing `xedocs-0.2.8/xedocs/xedocs.py` & `xedocs-0.2.9/xedocs/xedocs.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,36 +173,45 @@
         raise ValueError("No API interface class found.")
     interface = interface_class(database)
     schema = find_schema(schema)
     return interface.datasource_for_schema(schema)
 
 
 def download_db(
-    db_name="straxen_db", schemas=None, path=None, batch_size=10_000, verbose=True
+    dbname="straxen_db", schemas=None, path=None, batch_size=10_000, verbose=True
 ):
     """Download data from a remote database to a local database."""
     import tinydb
 
     if schemas is None:
         schemas = list_schemas()
 
     if not isinstance(schemas, list):
         schemas = [schemas]
 
     with tqdm(total=len(schemas)) as pbar:
 
         for schema in schemas:
             schema = find_schema(schema)
-            accessor = get_accessor(schema, db_name)
+            accessor = get_accessor(schema, dbname)
             pbar.set_description(f"Downloading {schema._ALIAS}")
 
+            basepath = None
+
             if path is None:
-                basepath = settings.local_path_for_schema(schema, db=db_name)
+                path = settings.DATA_DIR
+
+            interface = settings._database_interfaces.get(dbname, {}).get(
+                "local_repo", None
+            )
+
+            if interface is None:
+                basepath = Path(path) / dbname / schema._CATEGORY / schema._ALIAS
             else:
-                basepath = Path(path) / db_name / schema._CATEGORY / schema._ALIAS
+                basepath = interface.base_path_for_schema(schema)
 
             def write_docs(docs, num=1):
                 fpath = basepath / f"{num}.json"
                 db = tinydb.TinyDB(fpath, create_dirs=True, indent=4)
                 table = db.table(schema._ALIAS)
                 table.truncate()
                 table.insert_multiple(docs)
```

### Comparing `xedocs-0.2.8/setup.py` & `xedocs-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                           'local_repo = '
                           'xedocs.databases.local:LocalRepoDatabase',
                           'mongo = xedocs.databases.mongo:MongoDatabase',
                           'utilix = xedocs.databases.utilix:UtilixDatabase']}
 
 setup_kwargs = {
     'name': 'xedocs',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Top-level package for xedocs.',
     'long_description': "=======================================\nXeDocs - XENON Metadata management tool\n=======================================\nxedocs is meant to replace cmt and bodega as well as helping tracking all shared documents especially if\nthey need to be versioned.\n\nWhat does Xedocs give you\n=========================\n\nData reading\n------------\n\n- Read data from multiple formats (e.g. mongodb, pandas) and locations with a simple unified interface.\n- Custom logic implemented on the document class, e.g. creating a tensorflow model from the data etc.\n- Multiple APIs for reading data, fun functional, ODM style, pandas and xarray.\n- Read data as objects, dataframes, dicts, json.\n    \nWriting data\n------------\n\n- Write data to multiple storage backends with the same interface\n- Custom per-collection rules for data insertion, deletion and updating.\n- Schema validation and type coercion so storage has uniform and consistent data.\n    \nOther\n-----\n\n- Custom panel widgets for graphical representation of data, web client\n- Auto-generated API server and client + openapi documentation\n- CLI for viewing and downloading data\n\n\nBasic Usage\n-----------\n\nExplore the available schemas\n\n.. code-block:: python\n\n    import xedocs\n\n    >>> xedocs.list_schemas()\n    >>> ['detector_numbers',\n        'fax_configs',\n        'plugin_lineages',\n        'context_lineages',\n        'pmt_gains',\n        'global_versions',\n        'electron_drift_velocities',\n        ...]\n\n    >>> xedocs.help('pmt_gains')\n\n    >>>\n            Schema name: pmt_gains\n            Index fields: ['version', 'time', 'detector', 'pmt']\n            Column fields: ['created_date', 'comments', 'value']\n    \n\nRead/write data from the shared development database, \nthis database is writable from the default analysis username/password\n\n.. code-block:: python\n\n    import xedocs\n\n    db = xedocs.development_db\n\n    docs = db.pmt_gains.find_docs(version='v1', pmt=[1,2,3,5], time='2021-01-01T00:00:00', detector='tpc')\n    gains = [doc.value for doc in docs]\n\n    doc = db.pmt_gains.find_one(version='v1', pmt=1, time='2021-01-01T00:00:00', detector='tpc')\n    pmt1_gain = doc.value\n\nRead from the straxen processing database, this database is read-only for the default analysis username/password\n\n\n.. code-block:: python\n\n    import xedocs\n\n    db = xedocs.straxen_db\n\n    ...\n    \nYou can also query documents directly from the schema class, \nSchemas will query the straxen database by default, if no explicit datasource is given.\n\n.. code-block:: python\n\n    from xedocs.schemas import DetectorNumber\n\n    drift_velocity = DetectorNumber.straxen_db.find_one(field='drift_velocity', version='v1')\n    \n    # Returns a Bodega object with attributes value, description etc.\n    drift_velocity.value\n\n    all_v1_documents = DetectorNumber.straxen_db.find(version='v1')\n\n\n\nRead data from alternative data sources specified by path, \ne.g csv files which will be loaded by pandas.\n\n.. code-block:: python\n\n    from xedocs.schemas import DetectorNumber\n    \n    g1_doc = DetectorNumber.find_one(datasource='/path/to/file.csv', version='v1', field='g1')\n    g1_value = g1_doc.value\n    g1_error = g1_doc.uncertainty\n\nThe path can also be a github URL or any other URL supported by fsspec. \n\n.. code-block:: python\n\n    from xedocs.schemas import DetectorNumber\n    \n    g1_doc = DetectorNumber.find_one(\n                             datasource='github://org:repo@/path/to/file.csv', \n                             version='v1', \n                             field='g1')\n\n\nSupported data sources\n\n    - MongoDB collections\n    - TinyDB tables\n    - JSON files\n    - REST API clients\n\nPlease open an issue on rframe_ if you want support for an additional data format.\n\nIf you want a new datasource to be available from a schema class, you can register it to the class:\n\n.. code-block:: python\n\n    from xedocs.schemas import DetectorNumber\n    \n    DetectorNumber.register_datasource('github://org:repo@/path/to/file.csv', name='github_repo')\n\n    # The source will now be available under the given name:\n\n    g1_doc = DetectorNumber.github_repo.find_one(version='v1', field='g1')\n\n\nDocumentation\n-------------\nFull documentation hosted by Readthedocs_\n\nCredits\n-------\n\n\nThis package was created with Cookiecutter_ and the `briggySmalls/cookiecutter-pypackage`_ project template.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`briggySmalls/cookiecutter-pypackage`: https://github.com/briggySmalls/cookiecutter-pypackage\n.. _Readthedocs: https://xedocs.readthedocs.io/en/latest/\n.. _rframe: https://github.com/jmosbacher/rframe",
     'author': 'Yossi Mosbacher',
     'author_email': 'joe.mosbacher@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/XENONnT/xedocs',
```

### Comparing `xedocs-0.2.8/PKG-INFO` & `xedocs-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xedocs
-Version: 0.2.8
+Version: 0.2.9
 Summary: Top-level package for xedocs.
 Home-page: https://github.com/XENONnT/xedocs
 Author: Yossi Mosbacher
 Author-email: joe.mosbacher@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

