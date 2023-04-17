# Comparing `tmp/peegy-1.3.6.tar.gz` & `tmp/peegy-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peegy-1.3.6.tar", last modified: Sat Apr 15 08:16:52 2023, max compression
+gzip compressed data, was "peegy-1.3.7.tar", last modified: Mon Apr 17 15:31:37 2023, max compression
```

## Comparing `peegy-1.3.6.tar` & `peegy-1.3.7.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.154836 peegy-1.3.6/
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-04-15 07:57:16.000000 peegy-1.3.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-15 08:16:52.153836 peegy-1.3.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.975818 peegy-1.3.6/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10796 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_abr_peak_detection.py
--rw-rw-rw-   0 root         (0) root         (0)    17277 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_eog_removal_template_.py
--rw-rw-rw-   0 root         (0) root         (0)    10930 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_peak_detection.py
--rw-rw-rw-   0 root         (0) root         (0)     8276 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_peak_detection_bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)    10923 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_peak_detection_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    12109 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_video.py
--rw-rw-rw-   0 root         (0) root         (0)    12378 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_weighted_average.py
--rw-rw-rw-   0 root         (0) root         (0)    10304 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_acc_weighted_vs_standard_average.py
--rw-rw-rw-   0 root         (0) root         (0)    15470 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_dss_frequency_domain_bias_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12503 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_dss_time_domain_bias_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_f_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11144 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_ht2_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11861 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_ht2_test_weighted_average.py
--rw-rw-rw-   0 root         (0) root         (0)     8671 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
--rw-rw-rw-   0 root         (0) root         (0)     6918 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_no_layout.py
--rw-rw-rw-   0 root         (0) root         (0)     6851 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_assr_phase_locking_value_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12611 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_ffr_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     7895 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_using_own_data_trials.py
--rw-rw-rw-   0 root         (0) root         (0)     7952 2023-04-15 07:57:16.000000 peegy-1.3.6/examples/example_using_own_raw_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.977818 peegy-1.3.6/peegy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.986819 peegy-1.3.6/peegy/definitions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/channel_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    31413 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/edf_bdf_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    57262 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/eegReaderAbstractClasses.py
--rw-rw-rw-   0 root         (0) root         (0)     9074 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/eeg_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     7273 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/events.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/definitions/tables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.987819 peegy-1.3.6/peegy/directories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/directories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/directories/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.991820 peegy-1.3.6/peegy/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20916 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/edf_bdf_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.992820 peegy-1.3.6/peegy/io/eeg/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/eeg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/eeg/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.994820 peegy-1.3.6/peegy/io/external_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.998820 peegy-1.3.6/peegy/io/external_tools/aep_gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    11573 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/dataReadingTools.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/extsys_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    20273 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/external_tools/file_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4695 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/generic_csv_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.004821 peegy-1.3.6/peegy/io/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10450 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/data_storage_reading_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    16923 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/data_storage_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    29181 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/storage/plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/synergy_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/io/xml_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.018822 peegy-1.3.6/peegy/layouts/
--rw-rw-rw-   0 root         (0) root         (0)    10895 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/KIT-160.lay
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5612 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi128.lay
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi16.lay
--rw-rw-rw-   0 root         (0) root         (0)     7045 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi160.lay
--rw-rw-rw-   0 root         (0) root         (0)    11339 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi256.lay
--rw-rw-rw-   0 root         (0) root         (0)     1379 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32.lay
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32_2_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32_fnirs_MP.lay
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi32_fnirs_jaime.lay
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi64.lay
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi64_2_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)     2903 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/biosemi64_3_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)      597 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/emotive14.lay
--rw-rw-rw-   0 root         (0) root         (0)     5248 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/layouts.py
--rw-rw-rw-   0 root         (0) root         (0)     3821 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/layouts/neuroscan64.lay
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.022823 peegy-1.3.6/peegy/plot/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50150 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/plot/eeg_ave_epochs_plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/plot/eeg_plot_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.023823 peegy-1.3.6/peegy/processing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.023823 peegy-1.3.6/peegy/processing/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3067 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/events/event_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.081829 peegy-1.3.6/peegy/processing/pipe/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/attach.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.082829 peegy-1.3.6/peegy/processing/pipe/bootstrap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/bootstrap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12387 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/bootstrap/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)    25813 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     1988 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/detection.py
--rw-rw-rw-   0 root         (0) root         (0)    30969 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/epochs.py
--rw-rw-rw-   0 root         (0) root         (0)    33757 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/general.py
--rw-rw-rw-   0 root         (0) root         (0)     9032 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    13088 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/io.py
--rw-rw-rw-   0 root         (0) root         (0)     4961 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)    15881 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     6983 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/regression.py
--rw-rw-rw-   0 root         (0) root         (0)    22084 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/simulate.py
--rw-rw-rw-   0 root         (0) root         (0)    38597 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/spatial_filtering.py
--rw-rw-rw-   0 root         (0) root         (0)    27211 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10453 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/pipe/time_frequency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.084829 peegy-1.3.6/peegy/processing/statistics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/statistics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/statistics/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    14461 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/statistics/eeg_statistic_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.085829 peegy-1.3.6/peegy/processing/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/system/memory.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/system/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.088829 peegy-1.3.6/peegy/processing/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.090829 peegy-1.3.6/peegy/processing/tools/detection/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/detection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8780 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/detection/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     9602 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/detection/time_domain_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    20468 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/eeg_epoch_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    69736 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/epochs_processing_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.091830 peegy-1.3.6/peegy/processing/tools/filters/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15600 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/eegFiltering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.092830 peegy-1.3.6/peegy/processing/tools/filters/eog_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/eog_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19679 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/eog_tools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/resampling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.094830 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     6169 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.095830 peegy-1.3.6/peegy/processing/tools/fitting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/fitting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/fitting/fitting_functions.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/math_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.095830 peegy-1.3.6/peegy/processing/tools/multiprocessing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/multiprocessing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.097830 peegy-1.3.6/peegy/processing/tools/template_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/template_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13598 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/template_generator/auditory_waveforms.py
--rw-rw-rw-   0 root         (0) root         (0)    37074 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/template_generator/h0.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.098830 peegy-1.3.6/peegy/processing/tools/video/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/video/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/video/recording.py
--rw-rw-rw-   0 root         (0) root         (0)    48703 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/processing/tools/weightedAverage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.148835 peegy-1.3.6/peegy/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.150836 peegy-1.3.6/peegy/test/artifact_removal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3258 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/ir_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/regression_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     4857 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/artifact_removal/xcorr_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/dss_unit_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/eeg_test_resampling.py
--rw-rw-rw-   0 root         (0) root         (0)     3638 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/javerager_test.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/read_data_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3406 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_assr_moving_average.py
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_average_spectrogram_power.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_biosemi_class.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_biosemi_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_bootstraping.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_edf_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eeg_notch_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eog_removal_correlation.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eog_template_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_eog_template_valderrama_20118.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_et_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2582 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_fir_filter_mt.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_fir_filter_ols.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_fiter_mt.py
--rw-rw-rw-   0 root         (0) root         (0)     5716 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_freq_noise_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     3476 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_freq_noise_estimation_plots.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_frequency_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_generic_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     2032 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_hotelling_t2.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_ica_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_noise_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_norm_corr.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_parse_processing_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_peakdetection.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_phase_locking_value.py
--rw-rw-rw-   0 root         (0) root         (0)     6025 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_pooled_freq_noise_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_scrolling.py
--rw-rw-rw-   0 root         (0) root         (0)     5499 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_example1.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_example6.py
--rw-rw-rw-   0 root         (0) root         (0)     6047 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     7065 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain_2.py
--rw-rw-rw-   0 root         (0) root         (0)     8319 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_w_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/test/test_xml_to_dict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.150836 peegy-1.3.6/peegy/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.151836 peegy-1.3.6/peegy/tools/aep_gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/aep_gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.152836 peegy-1.3.6/peegy/tools/signal_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/signal_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4417 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/signal_generator/noise_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.153836 peegy-1.3.6/peegy/tools/units/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/units/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-15 07:57:16.000000 peegy-1.3.6/peegy/tools/units/unit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:51.979818 peegy-1.3.6/peegy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6684 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      527 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-15 08:16:51.000000 peegy-1.3.6/peegy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 08:16:52.154836 peegy-1.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-15 07:57:16.000000 peegy-1.3.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 08:16:52.153836 peegy-1.3.6/test_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 07:57:16.000000 peegy-1.3.6/test_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.256821 peegy-1.3.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-04-17 15:12:09.000000 peegy-1.3.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-17 15:31:37.255821 peegy-1.3.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.144813 peegy-1.3.7/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10796 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_abr_peak_detection.py
+-rw-rw-rw-   0 root         (0) root         (0)    17277 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_eog_removal_template_.py
+-rw-rw-rw-   0 root         (0) root         (0)    10930 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_peak_detection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8276 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_peak_detection_bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    10923 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_peak_detection_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)    12109 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_video.py
+-rw-rw-rw-   0 root         (0) root         (0)    12378 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_weighted_average.py
+-rw-rw-rw-   0 root         (0) root         (0)    10304 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_weighted_vs_standard_average.py
+-rw-rw-rw-   0 root         (0) root         (0)    15471 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_dss_frequency_domain_bias_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12503 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_dss_time_domain_bias_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9505 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_f_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    11144 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_ht2_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    11861 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_ht2_test_weighted_average.py
+-rw-rw-rw-   0 root         (0) root         (0)     8671 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6918 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_no_layout.py
+-rw-rw-rw-   0 root         (0) root         (0)     6851 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_phase_locking_value_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12611 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_ffr_artifact_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     7895 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_using_own_data_trials.py
+-rw-rw-rw-   0 root         (0) root         (0)     7952 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_using_own_raw_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.145814 peegy-1.3.7/peegy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.154814 peegy-1.3.7/peegy/definitions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/channel_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31413 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/edf_bdf_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    57262 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/eegReaderAbstractClasses.py
+-rw-rw-rw-   0 root         (0) root         (0)     9074 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/eeg_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7273 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/tables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.156814 peegy-1.3.7/peegy/directories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/directories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/directories/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.160815 peegy-1.3.7/peegy/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20916 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/edf_bdf_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.162815 peegy-1.3.7/peegy/io/eeg/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/eeg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7491 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/eeg/reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.163815 peegy-1.3.7/peegy/io/external_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.168815 peegy-1.3.7/peegy/io/external_tools/aep_gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    11573 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/dataReadingTools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/extsys_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    20273 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/file_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4695 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/generic_csv_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.172815 peegy-1.3.7/peegy/io/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10450 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/data_storage_reading_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    16923 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/data_storage_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    29181 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/synergy_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/xml_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.185816 peegy-1.3.7/peegy/layouts/
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/KIT-160.lay
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi128.lay
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi16.lay
+-rw-rw-rw-   0 root         (0) root         (0)     7045 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi160.lay
+-rw-rw-rw-   0 root         (0) root         (0)    11339 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi256.lay
+-rw-rw-rw-   0 root         (0) root         (0)     1379 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32.lay
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32_2_EXT.lay
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32_fnirs_MP.lay
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32_fnirs_jaime.lay
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi64.lay
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi64_2_EXT.lay
+-rw-rw-rw-   0 root         (0) root         (0)     2903 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi64_3_EXT.lay
+-rw-rw-rw-   0 root         (0) root         (0)      597 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/emotive14.lay
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/layouts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3821 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/neuroscan64.lay
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.188817 peegy-1.3.7/peegy/plot/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50150 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/plot/eeg_ave_epochs_plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3001 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/plot/eeg_plot_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.188817 peegy-1.3.7/peegy/processing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.189817 peegy-1.3.7/peegy/processing/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3067 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/events/event_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.205818 peegy-1.3.7/peegy/processing/pipe/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/attach.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.206818 peegy-1.3.7/peegy/processing/pipe/bootstrap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/bootstrap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12254 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/bootstrap/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    25813 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/detection.py
+-rw-rw-rw-   0 root         (0) root         (0)    30969 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)    33757 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     9032 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13088 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     5252 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)    15881 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6983 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)    22084 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/simulate.py
+-rw-rw-rw-   0 root         (0) root         (0)    38597 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/spatial_filtering.py
+-rw-rw-rw-   0 root         (0) root         (0)    27211 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6463 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10453 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/time_frequency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.208818 peegy-1.3.7/peegy/processing/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/statistics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/statistics/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14461 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/statistics/eeg_statistic_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.211818 peegy-1.3.7/peegy/processing/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/system/memory.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/system/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.214819 peegy-1.3.7/peegy/processing/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.216819 peegy-1.3.7/peegy/processing/tools/detection/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/detection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8780 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/detection/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9602 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/detection/time_domain_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    20468 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/eeg_epoch_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    69736 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/epochs_processing_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.218819 peegy-1.3.7/peegy/processing/tools/filters/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15600 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/eegFiltering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.219819 peegy-1.3.7/peegy/processing/tools/filters/eog_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/eog_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19679 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/eog_tools/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/resampling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.220819 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6169 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.221819 peegy-1.3.7/peegy/processing/tools/fitting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/fitting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/fitting/fitting_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/math_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.222819 peegy-1.3.7/peegy/processing/tools/multiprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/multiprocessing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.224819 peegy-1.3.7/peegy/processing/tools/template_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/template_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13598 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/template_generator/auditory_waveforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    37074 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/template_generator/h0.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.224819 peegy-1.3.7/peegy/processing/tools/video/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/video/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/video/recording.py
+-rw-rw-rw-   0 root         (0) root         (0)    48703 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/weightedAverage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.249821 peegy-1.3.7/peegy/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.251821 peegy-1.3.7/peegy/test/artifact_removal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3258 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/ir_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/regression_artifact_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4857 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/xcorr_artifact_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/dss_unit_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/eeg_test_resampling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3638 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/javerager_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/read_data_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3406 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_assr_moving_average.py
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_average_spectrogram_power.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_biosemi_class.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_biosemi_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_bootstraping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_edf_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eeg_notch_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eog_removal_correlation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3472 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eog_template_removal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eog_template_valderrama_20118.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_et_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2582 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_fir_filter_mt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_fir_filter_ols.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_fiter_mt.py
+-rw-rw-rw-   0 root         (0) root         (0)     5716 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_freq_noise_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3476 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_freq_noise_estimation_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_frequency_average_epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_generic_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_hotelling_t2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_ica_average_epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_noise_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_norm_corr.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_parse_processing_chain.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_peakdetection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_phase_locking_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     6025 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_pooled_freq_noise_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_scrolling.py
+-rw-rw-rw-   0 root         (0) root         (0)     5499 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_example1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_example6.py
+-rw-rw-rw-   0 root         (0) root         (0)     6047 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     7065 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     8319 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_w_average_epochs.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_xml_to_dict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.252821 peegy-1.3.7/peegy/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.252821 peegy-1.3.7/peegy/tools/aep_gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/aep_gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.253821 peegy-1.3.7/peegy/tools/signal_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/signal_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/signal_generator/noise_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.254821 peegy-1.3.7/peegy/tools/units/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/units/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/units/unit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.147814 peegy-1.3.7/peegy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-17 15:31:36.000000 peegy-1.3.7/peegy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6684 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 15:31:37.256821 peegy-1.3.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-17 15:12:09.000000 peegy-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.255821 peegy-1.3.7/test_data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/test_data/__init__.py
```

### Comparing `peegy-1.3.6/LICENSE.txt` & `peegy-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/PKG-INFO` & `peegy-1.3.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peegy
-Version: 1.3.6
+Version: 1.3.7
 Summary: Tools to pipeline bulk analyses of EEG and other modalities.
 Home-page: https://jundurraga.gitlab.io/peegy/
 Author: Jaime A. Undurraga
 Author-email: jaime.undurraga@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `peegy-1.3.6/examples/example_abr_peak_detection.py` & `peegy-1.3.7/examples/example_abr_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_acc_eog_removal_template_.py` & `peegy-1.3.7/examples/example_acc_eog_removal_template_.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_acc_peak_detection.py` & `peegy-1.3.7/examples/example_acc_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_acc_peak_detection_bootstrap.py` & `peegy-1.3.7/examples/example_acc_peak_detection_bootstrap.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_acc_peak_detection_filters.py` & `peegy-1.3.7/examples/example_acc_peak_detection_filters.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_acc_video.py` & `peegy-1.3.7/examples/example_acc_video.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_acc_weighted_average.py` & `peegy-1.3.7/examples/example_acc_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_acc_weighted_vs_standard_average.py` & `peegy-1.3.7/examples/example_acc_weighted_vs_standard_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_assr_dss_frequency_domain_bias_test.py` & `peegy-1.3.7/examples/example_assr_dss_frequency_domain_bias_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                            fs=fs,
                            n_channels=n_channels,
                            snr=0.001,
                            layout_file_name='biosemi32.lay',
                            event_times=event_times,
                            event_code=1.0,
                            figures_subset_folder='assr_dss_frequency_domain_test',
-                           return_noise_only=True,
+                           return_noise_only=False,
                            mixing_matrix=np.diag(np.ones(n_channels))/n_channels,
                            noise_attenuation=3,
                            noise_seed=0)
 reader.run()
 
 # %%
 # Resize events
```

### Comparing `peegy-1.3.6/examples/example_assr_dss_time_domain_bias_test.py` & `peegy-1.3.7/examples/example_assr_dss_time_domain_bias_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_assr_f_test.py` & `peegy-1.3.7/examples/example_assr_f_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_assr_ht2_test.py` & `peegy-1.3.7/examples/example_assr_ht2_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_assr_ht2_test_weighted_average.py` & `peegy-1.3.7/examples/example_assr_ht2_test_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_assr_ht2_test_wrong_bias_frequnecy.py` & `peegy-1.3.7/examples/example_assr_ht2_test_wrong_bias_frequnecy.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_assr_no_layout.py` & `peegy-1.3.7/examples/example_assr_no_layout.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_assr_phase_locking_value_test.py` & `peegy-1.3.7/examples/example_assr_phase_locking_value_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_ffr_artifact_removal.py` & `peegy-1.3.7/examples/example_ffr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_using_own_data_trials.py` & `peegy-1.3.7/examples/example_using_own_data_trials.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/examples/example_using_own_raw_data.py` & `peegy-1.3.7/examples/example_using_own_raw_data.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/definitions/channel_definitions.py` & `peegy-1.3.7/peegy/definitions/channel_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/definitions/edf_bdf_reader.py` & `peegy-1.3.7/peegy/definitions/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/definitions/eegReaderAbstractClasses.py` & `peegy-1.3.7/peegy/definitions/eegReaderAbstractClasses.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/definitions/eeg_definitions.py` & `peegy-1.3.7/peegy/definitions/eeg_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/definitions/events.py` & `peegy-1.3.7/peegy/definitions/events.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/definitions/tables.py` & `peegy-1.3.7/peegy/definitions/tables.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/directories/tools.py` & `peegy-1.3.7/peegy/directories/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/edf_bdf_reader.py` & `peegy-1.3.7/peegy/io/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/eeg/reader.py` & `peegy-1.3.7/peegy/io/eeg/reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/external_tools/aep_gui/aep_matlab_tools.py` & `peegy-1.3.7/peegy/io/external_tools/aep_gui/aep_matlab_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/external_tools/aep_gui/dataReadingTools.py` & `peegy-1.3.7/peegy/io/external_tools/aep_gui/dataReadingTools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/external_tools/aep_gui/extsys_tools.py` & `peegy-1.3.7/peegy/io/external_tools/aep_gui/extsys_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py` & `peegy-1.3.7/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/external_tools/file_tools.py` & `peegy-1.3.7/peegy/io/external_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/generic_csv_reader.py` & `peegy-1.3.7/peegy/io/generic_csv_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/storage/data_storage_reading_tools.py` & `peegy-1.3.7/peegy/io/storage/data_storage_reading_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/storage/data_storage_tools.py` & `peegy-1.3.7/peegy/io/storage/data_storage_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/storage/plot_tools.py` & `peegy-1.3.7/peegy/io/storage/plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/synergy_reader.py` & `peegy-1.3.7/peegy/io/synergy_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/io/xml_tools.py` & `peegy-1.3.7/peegy/io/xml_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/KIT-160.lay` & `peegy-1.3.7/peegy/layouts/KIT-160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi128.lay` & `peegy-1.3.7/peegy/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi16.lay` & `peegy-1.3.7/peegy/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi160.lay` & `peegy-1.3.7/peegy/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi256.lay` & `peegy-1.3.7/peegy/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi32.lay` & `peegy-1.3.7/peegy/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi32_2_EXT.lay` & `peegy-1.3.7/peegy/layouts/biosemi32_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi32_fnirs_MP.lay` & `peegy-1.3.7/peegy/layouts/biosemi32_fnirs_MP.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi32_fnirs_jaime.lay` & `peegy-1.3.7/peegy/layouts/biosemi32_fnirs_jaime.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi64.lay` & `peegy-1.3.7/peegy/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi64_2_EXT.lay` & `peegy-1.3.7/peegy/layouts/biosemi64_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/biosemi64_3_EXT.lay` & `peegy-1.3.7/peegy/layouts/biosemi64_3_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/emotive14.lay` & `peegy-1.3.7/peegy/layouts/emotive14.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/layouts.py` & `peegy-1.3.7/peegy/layouts/layouts.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/layouts/neuroscan64.lay` & `peegy-1.3.7/peegy/layouts/neuroscan64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/plot/eeg_ave_epochs_plot_tools.py` & `peegy-1.3.7/peegy/plot/eeg_ave_epochs_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/plot/eeg_plot_tools.py` & `peegy-1.3.7/peegy/plot/eeg_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/events/event_tools.py` & `peegy-1.3.7/peegy/processing/events/event_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/attach.py` & `peegy-1.3.7/peegy/processing/pipe/attach.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/bootstrap/bootstrap.py` & `peegy-1.3.7/peegy/processing/pipe/bootstrap/bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,17 +95,17 @@
         # the origin input_process is copied to ensure nothing is done to the original reference process
         if self.origin_input_process is not None:
             _origin_input_process = copy.copy(self.origin_input_process)
         else:
             _origin_input_process = copy.copy(list(self.at_each_bootstrap_do.values())[0].input_process)
 
         # ensure that the reference process is used by the pipeline
-        for _process in list(self.at_each_bootstrap_do.values()):
+        for _key, _process in list(self.at_each_bootstrap_do.items()):
             if _process.input_process.name == _origin_input_process.name:
-                _process = _origin_input_process
+                self.at_each_bootstrap_do[_key].input_process = _origin_input_process
 
         # first run pipeline to extract actual values to be tested against bootstrapped tables
         self.at_each_bootstrap_do.run(force=True)
         # extract reference tables
         ref_table = get_tables(pipeline=self.at_each_bootstrap_do, targets=self.bootstrap_targets)
         # get event information
         _n_events = self.n_events
@@ -142,31 +142,26 @@
                                                                epoch_length=_epoch_length,
                                                                min_time=_min_time,
                                                                max_time=_max_time,
                                                                n_events=_n_events
                                                                )
             # run pipeline with new events
             self.at_each_bootstrap_do.run(force=True)
-            if _i == 0:
-                bootstrapped_tables = get_tables(pipeline=self.at_each_bootstrap_do, targets=self.bootstrap_targets)
-                bootstrapped_tables['bootstrap_number'] = _i
-
-            else:
-                _current_tables = get_tables(pipeline=self.at_each_bootstrap_do, targets=self.bootstrap_targets)
-                _current_tables['bootstrap_number'] = _i
-                bootstrapped_tables = pd.concat([bootstrapped_tables, _current_tables])
+            _current_tables = get_tables(pipeline=self.at_each_bootstrap_do, targets=self.bootstrap_targets)
+            _current_tables['bootstrap_number'] = _i
+            bootstrapped_tables = pd.concat([bootstrapped_tables, _current_tables])
         # compute statistics
         ref_table = ref_table.rename(columns={'value': 'statistic_value'})
         columns_left = set(bootstrapped_tables.keys()).difference(['value', 'bootstrap_number'])
         columns_right = set(ref_table.keys()).difference(['statistic_value'])
         common_cols = list(columns_left.intersection(columns_right))
         bootstrapped_and_ref_tables = pd.merge(bootstrapped_tables,
                                                ref_table,
                                                how='left',
-                                               on=common_cols
+                                               on=common_cols,
                                                )
 
         df_boots = bootstrapped_and_ref_tables.groupby(list(set(bootstrapped_and_ref_tables.keys()).difference(
             ['value', 'bootstrap_number'])), as_index=False).apply(
             lambda x: pd.Series({'stats': get_bootstrap_estimates(samples=x['value'],
                                                                   statistic=x['statistic_value'],
                                                                   alpha_level=self.alpha_level,
@@ -176,15 +171,15 @@
          df_boots['median'],
          df_boots['std'],
          df_boots['ci_lower'],
          df_boots['ci_upper'],
          df_boots['sample_size'],
          df_boots['p_value']) = zip(*df_boots.stats)
         df_boots['one_sided'] = self.one_sided
-        df_boots = df_boots.drop(['stats'], axis=1)
+        df_boots = df_boots.drop(['stats', 'data_source'], axis=1)
         # join boot table and reference table
         self.output_node.statistical_tests = Tables(table_name=TestType.bootstrap,
                                                     data=df_boots,
                                                     data_source=self.name)
 
 
 def get_bootstrap_estimates(samples: np.array = None,
@@ -220,14 +215,14 @@
         for _target in targets:
             if _target.table_name in _value.output_node.statistical_tests.keys():
                 _columns = list(set(_value.output_node.statistical_tests[_target.table_name].keys()) &
                                 set(_target.target_values))
                 if len(_columns):
                     df = _value.output_node.statistical_tests[_target.table_name]
                     df = df[_target.group_by + _target.target_values + ['data_source']]
-                    df = pd.melt(df, ignore_index=False,
-                                 id_vars=set(set(df.keys())).difference(_target.target_values),
-                                 value_vars=_target.target_values,
-                                 var_name='statistic')
-                    df['table_name'] = _target.table_name
-                    output = pandas.concat([output, df], ignore_index=True)
+                    melted_df = pd.melt(df, ignore_index=False,
+                                        id_vars=set(set(df.keys())).difference(_target.target_values),
+                                        value_vars=_target.target_values,
+                                        var_name='statistic')
+                    melted_df['table_name'] = _target.table_name
+                    output = pandas.concat([output, melted_df], ignore_index=True)
     return output
```

### Comparing `peegy-1.3.6/peegy/processing/pipe/definitions.py` & `peegy-1.3.7/peegy/processing/pipe/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/detection.py` & `peegy-1.3.7/peegy/processing/pipe/detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/epochs.py` & `peegy-1.3.7/peegy/processing/pipe/epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/general.py` & `peegy-1.3.7/peegy/processing/pipe/general.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/interpolation.py` & `peegy-1.3.7/peegy/processing/pipe/interpolation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/io.py` & `peegy-1.3.7/peegy/processing/pipe/io.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/pipeline.py` & `peegy-1.3.7/peegy/processing/pipe/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,22 @@
         while _label in all_names:
             _label = label + '_' + str(count)
             count = count + 1
         if count > 0:
             print('PipePool item "{:}" already exists. Renamed to "{:}"'.format(label, _label))
         return _label
 
+    def replace(self, key, value):
+        assert isinstance(value, InputOutputProcess)
+        super(PipePool, self).__setitem__(key, value)
+        # we add the new item as class variable
+        setattr(self, key, value)
+        # set name of InoutOutputProcess
+        value.name = key
+
     def __getitem__(self, key):
         out = None
         if key in self.keys():
             out = super(PipePool, self).__getitem__(key)
         return out
 
     def run(self, force: bool = False):
```

### Comparing `peegy-1.3.6/peegy/processing/pipe/plot.py` & `peegy-1.3.7/peegy/processing/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/regression.py` & `peegy-1.3.7/peegy/processing/pipe/regression.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/simulate.py` & `peegy-1.3.7/peegy/processing/pipe/simulate.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/spatial_filtering.py` & `peegy-1.3.7/peegy/processing/pipe/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/statistics.py` & `peegy-1.3.7/peegy/processing/pipe/statistics.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/storage.py` & `peegy-1.3.7/peegy/processing/pipe/storage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/pipe/time_frequency.py` & `peegy-1.3.7/peegy/processing/pipe/time_frequency.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/statistics/definitions.py` & `peegy-1.3.7/peegy/processing/statistics/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/statistics/eeg_statistic_tools.py` & `peegy-1.3.7/peegy/processing/statistics/eeg_statistic_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/system/progress.py` & `peegy-1.3.7/peegy/processing/system/progress.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/detection/definitions.py` & `peegy-1.3.7/peegy/processing/tools/detection/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/detection/time_domain_tools.py` & `peegy-1.3.7/peegy/processing/tools/detection/time_domain_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/eeg_epoch_operators.py` & `peegy-1.3.7/peegy/processing/tools/eeg_epoch_operators.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/epochs_processing_tools.py` & `peegy-1.3.7/peegy/processing/tools/epochs_processing_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/filters/eegFiltering.py` & `peegy-1.3.7/peegy/processing/tools/filters/eegFiltering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/filters/eog_tools/tools.py` & `peegy-1.3.7/peegy/processing/tools/filters/eog_tools/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/filters/resampling.py` & `peegy-1.3.7/peegy/processing/tools/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/definitions.py` & `peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py` & `peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py` & `peegy-1.3.7/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/template_generator/auditory_waveforms.py` & `peegy-1.3.7/peegy/processing/tools/template_generator/auditory_waveforms.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/template_generator/h0.json` & `peegy-1.3.7/peegy/processing/tools/template_generator/h0.json`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/video/recording.py` & `peegy-1.3.7/peegy/processing/tools/video/recording.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/processing/tools/weightedAverage.py` & `peegy-1.3.7/peegy/processing/tools/weightedAverage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/artifact_removal/ir_test.py` & `peegy-1.3.7/peegy/test/artifact_removal/ir_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/artifact_removal/regression_artifact_removal.py` & `peegy-1.3.7/peegy/test/artifact_removal/regression_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/artifact_removal/xcorr_artifact_removal.py` & `peegy-1.3.7/peegy/test/artifact_removal/xcorr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/dss_unit_tests.py` & `peegy-1.3.7/peegy/test/dss_unit_tests.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/eeg_test_resampling.py` & `peegy-1.3.7/peegy/test/eeg_test_resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/javerager_test.py` & `peegy-1.3.7/peegy/test/javerager_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/read_data_test.py` & `peegy-1.3.7/peegy/test/read_data_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_assr_moving_average.py` & `peegy-1.3.7/peegy/test/test_assr_moving_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_average_spectrogram_power.py` & `peegy-1.3.7/peegy/test/test_average_spectrogram_power.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_biosemi_class.py` & `peegy-1.3.7/peegy/test/test_biosemi_class.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_biosemi_reader.py` & `peegy-1.3.7/peegy/test/test_biosemi_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_bootstraping.py` & `peegy-1.3.7/peegy/test/test_bootstraping.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_edf_reader.py` & `peegy-1.3.7/peegy/test/test_edf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_eeg_notch_filter.py` & `peegy-1.3.7/peegy/test/test_eeg_notch_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_eog_removal_correlation.py` & `peegy-1.3.7/peegy/test/test_eog_removal_correlation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_eog_template_removal.py` & `peegy-1.3.7/peegy/test/test_eog_template_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_eog_template_valderrama_20118.py` & `peegy-1.3.7/peegy/test/test_eog_template_valderrama_20118.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_et_tools.py` & `peegy-1.3.7/peegy/test/test_et_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_filter.py` & `peegy-1.3.7/peegy/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_fir_filter_mt.py` & `peegy-1.3.7/peegy/test/test_fir_filter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_fir_filter_ols.py` & `peegy-1.3.7/peegy/test/test_fir_filter_ols.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_fiter_mt.py` & `peegy-1.3.7/peegy/test/test_fiter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_freq_noise_estimation.py` & `peegy-1.3.7/peegy/test/test_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_freq_noise_estimation_plots.py` & `peegy-1.3.7/peegy/test/test_freq_noise_estimation_plots.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_frequency_average_epochs.py` & `peegy-1.3.7/peegy/test/test_frequency_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_hotelling_t2.py` & `peegy-1.3.7/peegy/test/test_hotelling_t2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_ica_average_epochs.py` & `peegy-1.3.7/peegy/test/test_ica_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_multiprocessing.py` & `peegy-1.3.7/peegy/test/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_noise_generator.py` & `peegy-1.3.7/peegy/test/test_noise_generator.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_norm_corr.py` & `peegy-1.3.7/peegy/test/test_norm_corr.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_peakdetection.py` & `peegy-1.3.7/peegy/test/test_peakdetection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_phase_locking_value.py` & `peegy-1.3.7/peegy/test/test_phase_locking_value.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_pooled_freq_noise_estimation.py` & `peegy-1.3.7/peegy/test/test_pooled_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_scrolling.py` & `peegy-1.3.7/peegy/test/test_scrolling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_spatial_filtering_example1.py` & `peegy-1.3.7/peegy/test/test_spatial_filtering_example1.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_spatial_filtering_example6.py` & `peegy-1.3.7/peegy/test/test_spatial_filtering_example6.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain.py` & `peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_spatial_filtering_freq_domain_2.py` & `peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain_2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/test/test_w_average_epochs.py` & `peegy-1.3.7/peegy/test/test_w_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/tools/signal_generator/noise_functions.py` & `peegy-1.3.7/peegy/tools/signal_generator/noise_functions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy/tools/units/unit_tools.py` & `peegy-1.3.7/peegy/tools/units/unit_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy.egg-info/PKG-INFO` & `peegy-1.3.7/peegy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peegy
-Version: 1.3.6
+Version: 1.3.7
 Summary: Tools to pipeline bulk analyses of EEG and other modalities.
 Home-page: https://jundurraga.gitlab.io/peegy/
 Author: Jaime A. Undurraga
 Author-email: jaime.undurraga@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `peegy-1.3.6/peegy.egg-info/SOURCES.txt` & `peegy-1.3.7/peegy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/peegy.egg-info/requires.txt` & `peegy-1.3.7/peegy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.3.6/setup.py` & `peegy-1.3.7/setup.py`

 * *Files identical despite different names*

